# Comparing `tmp/pymycobot-3.4.4.tar.gz` & `tmp/pymycobot-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.4.4.tar", last modified: Tue Mar 26 09:09:10 2024, max compression
+gzip compressed data, was "pymycobot-3.4.5.tar", last modified: Tue Apr  9 10:02:31 2024, max compression
```

## Comparing `pymycobot-3.4.4.tar` & `pymycobot-3.4.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 09:09:10.918685 pymycobot-3.4.4/
--rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.4/LICENSE
--rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0    63353 2024-03-26 09:09:10.916686 pymycobot-3.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 09:09:10.882677 pymycobot-3.4.4/pymycobot/
--rw-rw-rw-   0        0        0    35096 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     2067 2024-03-26 09:08:57.000000 pymycobot-3.4.4/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.4/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    20587 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/common.py
--rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.4/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0    16504 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/error.py
--rw-rw-rw-   0        0        0    43733 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/generate.py
--rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.4/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.4/pymycobot/log.py
--rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.4/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8459 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mecharmsocket.py
--rw-rw-rw-   0        0        0     7042 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mercury.py
--rw-rw-rw-   0        0        0    16399 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mercury_api.py
--rw-rw-rw-   0        0        0     6394 2024-03-01 10:10:12.000000 pymycobot-3.4.4/pymycobot/mercurychassis.py
--rw-rw-rw-   0        0        0     2211 2024-03-21 08:57:25.000000 pymycobot-3.4.4/pymycobot/mercurychassisocket.py
--rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.4/pymycobot/mercurysocket.py
--rw-rw-rw-   0        0        0    12964 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/myagv.py
--rw-rw-rw-   0        0        0    11294 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/myarm.py
--rw-rw-rw-   0        0        0     8871 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/myarmsocket.py
--rw-rw-rw-   0        0        0    15120 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     6123 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4544 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     9844 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     9524 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0    85313 2024-03-21 08:57:25.000000 pymycobot-3.4.4/pymycobot/mycobotpro630.py
--rw-rw-rw-   0        0        0     8955 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     9916 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     8607 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.4/pymycobot/public.py
--rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.4/pymycobot/robot_limit.json
--rw-rw-rw-   0        0        0    22021 2024-03-26 09:07:04.000000 pymycobot-3.4.4/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.4/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:09:10.915684 pymycobot-3.4.4/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    63353 2024-03-26 09:09:10.000000 pymycobot-3.4.4/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2024-03-26 09:09:10.000000 pymycobot-3.4.4/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 09:09:10.000000 pymycobot-3.4.4/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-26 09:09:10.000000 pymycobot-3.4.4/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-26 09:09:10.000000 pymycobot-3.4.4/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-18 01:52:28.000000 pymycobot-3.4.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 09:09:10.918685 pymycobot-3.4.4/setup.cfg
--rw-rw-rw-   0        0        0     3216 2023-11-01 10:12:51.000000 pymycobot-3.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 09:09:10.914683 pymycobot-3.4.4/tests/
--rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.4/tests/test_api.py
--rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.4/tests/test_generator.py
--rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.4/tests/test_socket.py
--rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:02:31.007134 pymycobot-3.4.5/
+-rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.5/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    63942 2024-04-09 10:02:31.006135 pymycobot-3.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 10:02:30.971629 pymycobot-3.4.5/pymycobot/
+-rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     2067 2024-04-09 09:58:11.000000 pymycobot-3.4.5/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.5/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    21490 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/common.py
+-rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.5/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/error.py
+-rw-rw-rw-   0        0        0    44048 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.5/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.5/pymycobot/log.py
+-rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.5/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mecharmsocket.py
+-rw-rw-rw-   0        0        0     7042 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mercury.py
+-rw-rw-rw-   0        0        0    16852 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mercury_api.py
+-rw-rw-rw-   0        0        0     6394 2024-03-01 10:10:12.000000 pymycobot-3.4.5/pymycobot/mercurychassis.py
+-rw-rw-rw-   0        0        0     2211 2024-03-21 08:57:25.000000 pymycobot-3.4.5/pymycobot/mercurychassisocket.py
+-rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.5/pymycobot/mercurysocket.py
+-rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.5/pymycobot/myagv.py
+-rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/myarmsocket.py
+-rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0    85325 2024-04-09 09:54:24.000000 pymycobot-3.4.5/pymycobot/mycobotpro630.py
+-rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.5/pymycobot/public.py
+-rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.5/pymycobot/robot_limit.json
+-rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.5/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.5/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:02:31.005134 pymycobot-3.4.5/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    63942 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 10:02:30.000000 pymycobot-3.4.5/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:02:31.007134 pymycobot-3.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:02:31.004134 pymycobot-3.4.5/tests/
+-rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_api.py
+-rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_generator.py
+-rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_socket.py
+-rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.5/tests/test_utils.py
```

### Comparing `pymycobot-3.4.4/LICENSE` & `pymycobot-3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/PKG-INFO` & `pymycobot-3.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.4
+Version: 3.4.5
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
+Requires-Dist: python-can
 
 # This is Python API for ElephantRobotics product
 
 ![Python 2.7](https://img.shields.io/badge/Python-v2.7%5E-green?logo=python)
 ![Python 3](https://img.shields.io/badge/Python-v3%5E-green?logo=python)
 [![pypi_version](https://img.shields.io/pypi/v/pymycobot?label=pypi)](https://pypi.org/project/pigit)
 
@@ -199,14 +200,16 @@
     - [set\_transponder\_mode](#set_transponder_mode-1)
     - [set\_HTS\_gripper\_torque](#set_hts_gripper_torque)
     - [get\_HTS\_gripper\_torque](#get_hts_gripper_torque)
     - [get\_gripper\_protect\_current](#get_gripper_protect_current)
     - [init\_gripper](#init_gripper)
     - [set\_gripper\_protect\_current](#set_gripper_protect_current)
     - [set\_four\_pieces\_zero](#set_four_pieces_zero)
+    - [jog\_rpy](#jog_rpy)
+    - [set\_void\_compensate](#set_void_compensate)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
     - [gpio\_init](#gpio_init)
     - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
   - [get\_port\_list](#get_port_list)
@@ -1482,14 +1485,33 @@
 - **Prototype**: `set_four_pieces_zero()`
 
 - **Description**: Set the zero position of the four-piece motor.
 
 - **Return**
   - `int`: 1 - Set successful. 0 - Set failed.
 
+### jog_rpy
+
+- **Prototype**: `jog_rpy(end_direction, direction)`
+
+- **Description**: Rotate the end around a fixed axis in the base coordinate system.
+
+- **Parameters**
+  - `end_direction (int)`: Roll, Pitch, Yaw (1-3)
+  - `direction (int)`: 1 - forward rotation, 0 - reverse rotation
+
+### set_void_compensate
+
+- **Prototype**: `set_void_compensate(mode)`
+
+- **Description**: Set void compensation mode.
+
+- **Parameters**
+  - `mode (int)`: 0 - close, 1 - open
+
 ## Raspberry pi -- GPIO
 
 ### gpio_init
 
 - **Prototype**: `gpio_init()`
 
 - **Description**: Init GPIO module, and set BCM mode.
```

### Comparing `pymycobot-3.4.4/README.md` & `pymycobot-3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/Interface.py` & `pymycobot-3.4.5/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/__init__.py` & `pymycobot-3.4.5/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.4.4"
+__version__ = "3.4.5"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.4.4/pymycobot/bluet.py` & `pymycobot-3.4.5/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/common.py` & `pymycobot-3.4.5/pymycobot/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,17 @@
     GET_END_TYPE = 0x8A
     WRITE_MOVE_C = 0x8C
 
     # Impact checking
     SET_JOINT_CURRENT = 0x90
     GET_JOINT_CURRENT = 0x91
     SET_CURRENT_STATE = 0x92
+    GET_POS_OVER = 0x94
+    CLEAR_ENCODERS_ERROR = 0x95
+    GET_DOWN_ENCODERS = 0x96
 
     # planning speed
     GET_PLAN_SPEED = 0xD0
     GET_PLAN_ACCELERATION = 0xD1
     SET_PLAN_SPEED = 0xD2
     SET_PLAN_ACCELERATION = 0xD3
     move_round = 0xD4
@@ -195,14 +198,15 @@
     GET_SERVO_SPEED = 0xE1
     GET_SERVO_CURRENTS = 0xE2
     GET_SERVO_VOLTAGES = 0xE3
     GET_SERVO_STATUS = 0xE4
     GET_SERVO_TEMPS = 0xE5
     GET_SERVO_LASTPDI = 0xE6
     SERVO_RESTORE = 0xE7
+    SET_VOID_COMPENSATE = 0xE7
     SET_ERROR_DETECT_MODE = 0xE8
     GET_ERROR_DETECT_MODE = 0xE9
     
     MERCURY_GET_BASE_COORDS = 0xF0
     MERCURY_SET_BASE_COORD = 0xF1
     MERCURY_SET_BASE_COORDS = 0xF2
     MERCURY_JOG_BASE_COORD = 0xF3
@@ -419,14 +423,21 @@
         #         res.append(i)
         #     return res    
         if data_len in [6, 8, 12, 14, 16, 24, 26, 60]:
             if data_len == 8 and arm == 14 and cmd_id == ProtocolCode.IS_INIT_CALIBRATION:
                 for v in valid_data:
                     res.append(v)
                 return res
+            elif data_len == 8 and arm == 14 and cmd_id == ProtocolCode.GET_DOWN_ENCODERS:
+                i = 0
+                while i < data_len:
+                    byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
+                    i+=4
+                    res.append(byte_value)
+                return res
             for header_i in range(0, len(valid_data), 2):
                 one = valid_data[header_i : header_i + 2]
                 res.append(self._decode_int16(one))
         elif data_len == 2:
             if genre in [
                 ProtocolCode.GET_PLAN_SPEED,
                 ProtocolCode.GET_PLAN_ACCELERATION,
@@ -459,15 +470,26 @@
                 elif i in range(32,112):
                     res.append(3)
                 else:
                     res.append(i)
         elif data_len == 28:
             for i in range(0, data_len, 4):
                 byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
-                res.append(byte_value)
+                res.append(byte_value) 
+        elif data_len == 40:
+            i = 0
+            while i < data_len:
+                if i < 28:
+                    byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
+                    res.append(byte_value) 
+                    i+=4
+                else:
+                    one = valid_data[i : i + 2]
+                    res.append(self._decode_int16(one))
+                    i+=2
         elif data_len == 30:
             i = 0
             res = []
             while i < 30:
                 if i < 9 or i >= 23:
                     res.append(valid_data[i])
                     i+=1
```

### Comparing `pymycobot-3.4.4/pymycobot/elephantrobot.py` & `pymycobot-3.4.5/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/error.py` & `pymycobot-3.4.5/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/generate.py` & `pymycobot-3.4.5/pymycobot/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1213,8 +1213,17 @@
         """Rotate the end around a fixed axis in the base coordinate system
 
         Args:
             end_direction (int):  Roll, Pitch, Yaw (1-3)
             direction (int): 1 - forward rotation, 0 - reverse rotation
         """
         self.calibration_parameters(class_name = self.__class__.__name__, end_direction=end_direction)
-        return self._mesg(ProtocolCode.JOG_ABSOLUTE, end_direction, direction)
+        return self._mesg(ProtocolCode.JOG_ABSOLUTE, end_direction, direction)
+    
+    def set_void_compensate(self, mode):
+        """Set void compensation mode
+
+        Args:
+            mode (int): 0 - close, 1 - open
+        """
+        self.calibration_parameters(class_name = self.__class__.__name__, mode=mode)
+        return self._mesg(ProtocolCode.SET_VOID_COMPENSATE, mode)
```

### Comparing `pymycobot-3.4.4/pymycobot/log.py` & `pymycobot-3.4.5/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mecharmsocket.py` & `pymycobot-3.4.5/pymycobot/mecharmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mercury.py` & `pymycobot-3.4.5/pymycobot/mercury.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mercury_api.py` & `pymycobot-3.4.5/pymycobot/mercury_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,8 +465,21 @@
 
         Returns:
             int: 1 - pause completion
         """
         if deceleration:
             return self._mesg(ProtocolCode.PAUSE, has_reply=True)
         else:
-            return self._mesg(ProtocolCode.PAUSE, 1, has_reply=True)
+            return self._mesg(ProtocolCode.PAUSE, 1, has_reply=True)
+        
+    def get_modified_version(self):
+        return self._mesg(ProtocolCode.ROBOT_VERSION, has_reply=True)
+    
+    def get_pos_over(self):
+        return self._mesg(ProtocolCode.GET_POS_OVER, has_reply=True)
+    
+    def clear_encoders_error(self):
+        return self._mesg(ProtocolCode.CLEAR_ENCODERS_ERROR)
+    
+    def get_down_encoders(self):
+        return self._mesg(ProtocolCode.GET_DOWN_ENCODERS, has_reply=True)
+
```

### Comparing `pymycobot-3.4.4/pymycobot/mercurychassis.py` & `pymycobot-3.4.5/pymycobot/mercurychassis.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mercurychassisocket.py` & `pymycobot-3.4.5/pymycobot/mercurychassisocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mercurysocket.py` & `pymycobot-3.4.5/pymycobot/mercurysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/myagv.py` & `pymycobot-3.4.5/pymycobot/myagv.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,791 +21,857 @@
 00000140: 2020 2020 4745 545f 4649 524d 5741 5245      GET_FIRMWARE
 00000150: 5f56 4552 5349 4f4e 203d 205b 3078 3031  _VERSION = [0x01
 00000160: 2c20 3078 3033 5d0d 0a20 2020 2047 4554  , 0x03]..    GET
 00000170: 5f4d 4f54 4f52 535f 4355 5252 454e 5420  _MOTORS_CURRENT 
 00000180: 3d20 5b30 7830 312c 2030 7830 345d 0d0a  = [0x01, 0x04]..
 00000190: 2020 2020 4745 545f 4241 5454 4552 595f      GET_BATTERY_
 000001a0: 494e 464f 203d 205b 3078 3031 2c20 3078  INFO = [0x01, 0x
-000001b0: 3035 5d0d 0a0d 0a63 6c61 7373 204d 7941  05]....class MyA
-000001c0: 6776 2844 6174 6150 726f 6365 7373 6f72  gv(DataProcessor
-000001d0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-000001e0: 6974 5f5f 2873 656c 662c 2070 6f72 743d  it__(self, port=
-000001f0: 222f 6465 762f 7474 7941 4d41 3022 2c20  "/dev/ttyAMA0", 
-00000200: 6261 7564 7261 7465 3d22 3131 3532 3030  baudrate="115200
-00000210: 222c 2074 696d 656f 7574 3d30 2e31 2c20  ", timeout=0.1, 
-00000220: 6465 6275 673d 4661 6c73 6529 3a0d 0a20  debug=False):.. 
-00000230: 2020 2020 2020 2073 656c 662e 6465 6275         self.debu
-00000240: 6720 3d20 6465 6275 670d 0a20 2020 2020  g = debug..     
-00000250: 2020 2073 6574 7570 5f6c 6f67 6769 6e67     setup_logging
-00000260: 2873 656c 662e 6465 6275 6729 0d0a 2020  (self.debug)..  
-00000270: 2020 2020 2020 7365 6c66 2e6c 6f67 203d        self.log =
-00000280: 206c 6f67 6769 6e67 2e67 6574 4c6f 6767   logging.getLogg
-00000290: 6572 285f 5f6e 616d 655f 5f29 0d0a 2020  er(__name__)..  
-000002a0: 2020 2020 2020 7365 6c66 2e5f 7365 7269        self._seri
-000002b0: 616c 5f70 6f72 7420 3d20 7365 7269 616c  al_port = serial
-000002c0: 2e53 6572 6961 6c28 290d 0a20 2020 2020  .Serial()..     
-000002d0: 2020 2073 656c 662e 5f73 6572 6961 6c5f     self._serial_
-000002e0: 706f 7274 2e70 6f72 7420 3d20 706f 7274  port.port = port
-000002f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000300: 7365 7269 616c 5f70 6f72 742e 6261 7564  serial_port.baud
-00000310: 7261 7465 203d 2062 6175 6472 6174 650d  rate = baudrate.
-00000320: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-00000330: 6572 6961 6c5f 706f 7274 2e74 696d 656f  erial_port.timeo
-00000340: 7574 203d 2074 696d 656f 7574 0d0a 2020  ut = timeout..  
-00000350: 2020 2020 2020 7365 6c66 2e5f 7365 7269        self._seri
-00000360: 616c 5f70 6f72 742e 7274 7320 3d20 4661  al_port.rts = Fa
-00000370: 6c73 650d 0a20 2020 2020 2020 2073 656c  lse..        sel
-00000380: 662e 5f73 6572 6961 6c5f 706f 7274 2e6f  f._serial_port.o
-00000390: 7065 6e28 290d 0a20 2020 2020 2020 200d  pen()..        .
-000003a0: 0a20 2020 2064 6566 205f 7772 6974 6528  .    def _write(
-000003b0: 7365 6c66 2c20 636f 6d6d 616e 6429 3a0d  self, command):.
-000003c0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-000003d0: 6572 6961 6c5f 706f 7274 2e72 6573 6574  erial_port.reset
-000003e0: 5f69 6e70 7574 5f62 7566 6665 7228 290d  _input_buffer().
-000003f0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-00000400: 672e 6465 6275 6728 225f 7772 6974 653a  g.debug("_write:
-00000410: 207b 7d22 2e66 6f72 6d61 7428 5b68 6578   {}".format([hex
-00000420: 2869 2920 666f 7220 6920 696e 2063 6f6d  (i) for i in com
-00000430: 6d61 6e64 5d29 290d 0a20 2020 2020 2020  mand]))..       
-00000440: 2073 656c 662e 5f73 6572 6961 6c5f 706f   self._serial_po
-00000450: 7274 2e77 7269 7465 2863 6f6d 6d61 6e64  rt.write(command
-00000460: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000470: 5f73 6572 6961 6c5f 706f 7274 2e66 6c75  _serial_port.flu
-00000480: 7368 2829 0d0a 2020 2020 2020 2020 0d0a  sh()..        ..
-00000490: 2020 2020 6465 6620 5f72 6561 6428 7365      def _read(se
-000004a0: 6c66 2c20 636f 6d6d 616e 6429 3a0d 0a20  lf, command):.. 
-000004b0: 2020 2020 2020 2064 6174 6173 203d 2062         datas = b
-000004c0: 2727 0d0a 2020 2020 2020 2020 6b20 3d20  ''..        k = 
-000004d0: 300d 0a20 2020 2020 2020 2070 7265 203d  0..        pre =
-000004e0: 2030 0d0a 2020 2020 2020 2020 656e 6420   0..        end 
-000004f0: 3d20 350d 0a20 2020 2020 2020 2074 203d  = 5..        t =
-00000500: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
-00000510: 2020 2020 2020 6966 2063 6f6d 6d61 6e64        if command
-00000520: 5b6b 2d31 5d20 3d3d 2032 393a 0d0a 2020  [k-1] == 29:..  
-00000530: 2020 2020 2020 2020 2020 656e 6420 3d20            end = 
-00000540: 3330 0d0a 2020 2020 2020 2020 7768 696c  30..        whil
-00000550: 6520 7469 6d65 2e74 696d 6528 2920 2d20  e time.time() - 
-00000560: 7420 3c20 302e 323a 0d0a 2020 2020 2020  t < 0.2:..      
-00000570: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
-00000580: 662e 5f73 6572 6961 6c5f 706f 7274 2e72  f._serial_port.r
-00000590: 6561 6428 290d 0a20 2020 2020 2020 2020  ead()..         
-000005a0: 2020 206b 202b 3d20 310d 0a20 2020 2020     k += 1..     
-000005b0: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
-000005c0: 6461 7461 5f6c 656e 3a22 2c65 6e64 290d  data_len:",end).
-000005d0: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
-000005e0: 7269 6e74 2864 6174 612c 206c 656e 2864  rint(data, len(d
-000005f0: 6174 6173 292c 206b 2c20 656e 6429 0d0a  atas), k, end)..
-00000600: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00000610: 656e 2864 6174 6173 2920 3d3d 2034 3a0d  en(datas) == 4:.
-00000620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000630: 2023 2070 7269 6e74 2822 2d2d 2d2d 2d2d   # print("------
-00000640: 3a22 2c64 6174 6173 2c20 636f 6d6d 616e  :",datas, comman
-00000650: 642c 206b 2c20 656e 6429 0d0a 2020 2020  d, k, end)..    
-00000660: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00000670: 6174 6173 5b2d 325d 203d 3d20 3078 3031  atas[-2] == 0x01
-00000680: 2061 6e64 2064 6174 6173 5b2d 315d 203d   and datas[-1] =
-00000690: 3d20 3078 3035 3a0d 0a20 2020 2020 2020  = 0x05:..       
-000006a0: 2020 2020 2020 2020 2020 2020 2065 6e64               end
-000006b0: 203d 2037 0d0a 2020 2020 2020 2020 2020   = 7..          
-000006c0: 2020 2020 2020 6461 7461 7320 2b3d 2064        datas += d
-000006d0: 6174 610d 0a20 2020 2020 2020 2020 2020  ata..           
-000006e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000006f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00000700: 2065 6c69 6620 6c65 6e28 6461 7461 7329   elif len(datas)
-00000710: 203d 3d20 656e 643a 0d0a 2020 2020 2020   == end:..      
-00000720: 2020 2020 2020 2020 2020 6461 7461 7320            datas 
-00000730: 2b3d 2064 6174 610d 0a20 2020 2020 2020  += data..       
-00000740: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
-00000750: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00000760: 206c 656e 2864 6174 6173 2920 3e20 343a   len(datas) > 4:
-00000770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000780: 2020 6461 7461 7320 2b3d 2064 6174 610d    datas += data.
-00000790: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-000007a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000007b0: 6c65 6e28 6461 7461 7329 203e 3d20 323a  len(datas) >= 2:
-000007c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000007d0: 2020 6461 7461 5f6c 656e 203d 2073 7472    data_len = str
-000007e0: 7563 742e 756e 7061 636b 2822 6222 2c20  uct.unpack("b", 
-000007f0: 6461 7461 295b 305d 0d0a 2020 2020 2020  data)[0]..      
-00000800: 2020 2020 2020 2020 2020 6966 2063 6f6d            if com
-00000810: 6d61 6e64 5b2d 315d 203d 3d20 3239 206f  mand[-1] == 29 o
-00000820: 7220 6461 7461 5f6c 656e 203d 3d20 636f  r data_len == co
-00000830: 6d6d 616e 645b 6b2d 315d 3a0d 0a20 2020  mmand[k-1]:..   
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 2064 6174 6173 202b 3d20 6461 7461 0d0a   datas += data..
-00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000870: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00000880: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-00000890: 203d 2062 2727 0d0a 2020 2020 2020 2020   = b''..        
-000008a0: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
-000008b0: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-000008c0: 2020 2020 2020 2070 7265 203d 2030 0d0a         pre = 0..
-000008d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000008e0: 2064 6174 6120 3d3d 2062 225c 7866 6522   data == b"\xfe"
-000008f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000900: 2020 2069 6620 6461 7461 7320 3d3d 2062     if datas == b
-00000910: 2727 3a0d 0a20 2020 2020 2020 2020 2020  '':..           
-00000920: 2020 2020 2020 2020 2064 6174 6173 202b           datas +
-00000930: 3d20 6461 7461 0d0a 2020 2020 2020 2020  = data..        
-00000940: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00000950: 2021 3d20 313a 0d0a 2020 2020 2020 2020   != 1:..        
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 6b20 3d20 310d 0a20 2020 2020 2020 2020  k = 1..         
-00000980: 2020 2020 2020 2020 2020 2070 7265 203d             pre =
-00000990: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-000009a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000009c0: 6620 6b20 2d20 3120 3d3d 2070 7265 3a0d  f k - 1 == pre:.
-000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009e0: 2020 2020 2020 2020 2064 6174 6173 202b           datas +
-000009f0: 3d20 6461 7461 0d0a 2020 2020 2020 2020  = data..        
-00000a00: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000a10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000a20: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-00000a30: 203d 2062 225c 7866 6522 0d0a 2020 2020   = b"\xfe"..    
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2020 6b20 3d20 310d 0a20 2020 2020      k = 1..     
+000001b0: 3035 5d0d 0a20 2020 2053 4554 5f47 5952  05]..    SET_GYR
+000001c0: 4f5f 5354 4154 4520 3d20 5b30 7830 312c  O_STATE = [0x01,
+000001d0: 2030 7830 375d 0d0a 2020 2020 4745 545f   0x07]..    GET_
+000001e0: 4759 524f 5f53 5441 5445 203d 205b 3078  GYRO_STATE = [0x
+000001f0: 3031 2c20 3078 3038 5d0d 0a20 2020 2047  01, 0x08]..    G
+00000200: 4554 5f4d 4f44 4946 4945 445f 5645 5253  ET_MODIFIED_VERS
+00000210: 494f 4e20 3d20 5b30 7830 312c 2030 7830  ION = [0x01, 0x0
+00000220: 395d 0d0a 0d0a 636c 6173 7320 4d79 4167  9]....class MyAg
+00000230: 7628 4461 7461 5072 6f63 6573 736f 7229  v(DataProcessor)
+00000240: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+00000250: 745f 5f28 7365 6c66 2c20 706f 7274 3d22  t__(self, port="
+00000260: 2f64 6576 2f74 7479 414d 4130 222c 2062  /dev/ttyAMA0", b
+00000270: 6175 6472 6174 653d 2231 3135 3230 3022  audrate="115200"
+00000280: 2c20 7469 6d65 6f75 743d 302e 312c 2064  , timeout=0.1, d
+00000290: 6562 7567 3d46 616c 7365 293a 0d0a 2020  ebug=False):..  
+000002a0: 2020 2020 2020 7365 6c66 2e64 6562 7567        self.debug
+000002b0: 203d 2064 6562 7567 0d0a 2020 2020 2020   = debug..      
+000002c0: 2020 7365 7475 705f 6c6f 6767 696e 6728    setup_logging(
+000002d0: 7365 6c66 2e64 6562 7567 290d 0a20 2020  self.debug)..   
+000002e0: 2020 2020 2073 656c 662e 6c6f 6720 3d20       self.log = 
+000002f0: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+00000300: 7228 5f5f 6e61 6d65 5f5f 290d 0a20 2020  r(__name__)..   
+00000310: 2020 2020 2073 656c 662e 5f73 6572 6961       self._seria
+00000320: 6c5f 706f 7274 203d 2073 6572 6961 6c2e  l_port = serial.
+00000330: 5365 7269 616c 2829 0d0a 2020 2020 2020  Serial()..      
+00000340: 2020 7365 6c66 2e5f 7365 7269 616c 5f70    self._serial_p
+00000350: 6f72 742e 706f 7274 203d 2070 6f72 740d  ort.port = port.
+00000360: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+00000370: 6572 6961 6c5f 706f 7274 2e62 6175 6472  erial_port.baudr
+00000380: 6174 6520 3d20 6261 7564 7261 7465 0d0a  ate = baudrate..
+00000390: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+000003a0: 7269 616c 5f70 6f72 742e 7469 6d65 6f75  rial_port.timeou
+000003b0: 7420 3d20 7469 6d65 6f75 740d 0a20 2020  t = timeout..   
+000003c0: 2020 2020 2073 656c 662e 5f73 6572 6961       self._seria
+000003d0: 6c5f 706f 7274 2e72 7473 203d 2046 616c  l_port.rts = Fal
+000003e0: 7365 0d0a 2020 2020 2020 2020 7365 6c66  se..        self
+000003f0: 2e5f 7365 7269 616c 5f70 6f72 742e 6f70  ._serial_port.op
+00000400: 656e 2829 0d0a 2020 2020 2020 2020 0d0a  en()..        ..
+00000410: 2020 2020 6465 6620 5f77 7269 7465 2873      def _write(s
+00000420: 656c 662c 2063 6f6d 6d61 6e64 293a 0d0a  elf, command):..
+00000430: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00000440: 7269 616c 5f70 6f72 742e 7265 7365 745f  rial_port.reset_
+00000450: 696e 7075 745f 6275 6666 6572 2829 0d0a  input_buffer()..
+00000460: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00000470: 2e64 6562 7567 2822 5f77 7269 7465 3a20  .debug("_write: 
+00000480: 7b7d 222e 666f 726d 6174 285b 6865 7828  {}".format([hex(
+00000490: 6929 2066 6f72 2069 2069 6e20 636f 6d6d  i) for i in comm
+000004a0: 616e 645d 2929 0d0a 2020 2020 2020 2020  and]))..        
+000004b0: 7365 6c66 2e5f 7365 7269 616c 5f70 6f72  self._serial_por
+000004c0: 742e 7772 6974 6528 636f 6d6d 616e 6429  t.write(command)
+000004d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000004e0: 7365 7269 616c 5f70 6f72 742e 666c 7573  serial_port.flus
+000004f0: 6828 290d 0a20 2020 2020 2020 200d 0a20  h()..        .. 
+00000500: 2020 2064 6566 205f 7265 6164 2873 656c     def _read(sel
+00000510: 662c 2063 6f6d 6d61 6e64 293a 0d0a 2020  f, command):..  
+00000520: 2020 2020 2020 6461 7461 7320 3d20 6227        datas = b'
+00000530: 270d 0a20 2020 2020 2020 206b 203d 2030  '..        k = 0
+00000540: 0d0a 2020 2020 2020 2020 7072 6520 3d20  ..        pre = 
+00000550: 300d 0a20 2020 2020 2020 2065 6e64 203d  0..        end =
+00000560: 2035 0d0a 2020 2020 2020 2020 7420 3d20   5..        t = 
+00000570: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
+00000580: 2020 2020 2069 6620 636f 6d6d 616e 645b       if command[
+00000590: 6b2d 315d 203d 3d20 3239 3a0d 0a20 2020  k-1] == 29:..   
+000005a0: 2020 2020 2020 2020 2065 6e64 203d 2032           end = 2
+000005b0: 380d 0a20 2020 2020 2020 2065 6c69 6620  8..        elif 
+000005c0: 636f 6d6d 616e 645b 6b2d 315d 203d 3d20  command[k-1] == 
+000005d0: 3431 3a0d 0a20 2020 2020 2020 2020 2020  41:..           
+000005e0: 2065 6e64 203d 2034 300d 0a20 2020 2020   end = 40..     
+000005f0: 2020 2077 6869 6c65 2074 696d 652e 7469     while time.ti
+00000600: 6d65 2829 202d 2074 203c 2030 2e32 3a0d  me() - t < 0.2:.
+00000610: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00000620: 6120 3d20 7365 6c66 2e5f 7365 7269 616c  a = self._serial
+00000630: 5f70 6f72 742e 7265 6164 2829 0d0a 2020  _port.read()..  
+00000640: 2020 2020 2020 2020 2020 6b20 2b3d 2031            k += 1
+00000650: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000660: 206c 656e 2864 6174 6173 2920 3d3d 2034   len(datas) == 4
+00000670: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000680: 2020 2069 6620 6461 7461 735b 2d32 5d20     if datas[-2] 
+00000690: 3d3d 2030 7830 3120 616e 6420 6461 7461  == 0x01 and data
+000006a0: 735b 2d31 5d20 3d3d 2030 7830 353a 0d0a  s[-1] == 0x05:..
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2020 2020 656e 6420 3d20 370d 0a20 2020      end = 7..   
+000006d0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+000006e0: 6173 202b 3d20 6461 7461 0d0a 2020 2020  as += data..    
+000006f0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00000700: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+00000710: 656e 2864 6174 6173 2920 3d3d 2065 6e64  en(datas) == end
+00000720: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000730: 2020 2064 6174 6173 202b 3d20 6461 7461     datas += data
+00000740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000750: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00000760: 2020 2020 2065 6c69 6620 6c65 6e28 6461       elif len(da
+00000770: 7461 7329 203e 2034 3a0d 0a20 2020 2020  tas) > 4:..     
+00000780: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00000790: 202b 3d20 6461 7461 0d0a 2020 2020 2020   += data..      
+000007a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000007b0: 2020 2020 656c 6966 206c 656e 2864 6174      elif len(dat
+000007c0: 6173 2920 3e3d 2032 3a0d 0a20 2020 2020  as) >= 2:..     
+000007d0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+000007e0: 6c65 6e20 3d20 7374 7275 6374 2e75 6e70  len = struct.unp
+000007f0: 6163 6b28 2262 222c 2064 6174 6129 5b30  ack("b", data)[0
+00000800: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00000810: 2020 2069 6620 636f 6d6d 616e 645b 2d31     if command[-1
+00000820: 5d20 3d3d 2032 3920 6f72 2063 6f6d 6d61  ] == 29 or comma
+00000830: 6e64 5b2d 315d 203d 3d20 3431 206f 7220  nd[-1] == 41 or 
+00000840: 6461 7461 5f6c 656e 203d 3d20 636f 6d6d  data_len == comm
+00000850: 616e 645b 6b2d 315d 3a0d 0a20 2020 2020  and[k-1]:..     
+00000860: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00000870: 6174 6173 202b 3d20 6461 7461 0d0a 2020  atas += data..  
+00000880: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00000890: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000008a0: 2020 2020 2020 2020 2064 6174 6173 203d           datas =
+000008b0: 2062 2727 0d0a 2020 2020 2020 2020 2020   b''..          
+000008c0: 2020 2020 2020 2020 2020 6b20 3d20 300d            k = 0.
+000008d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008e0: 2020 2020 2070 7265 203d 2030 0d0a 2020       pre = 0..  
+000008f0: 2020 2020 2020 2020 2020 656c 6966 2064            elif d
+00000900: 6174 6120 3d3d 2062 225c 7866 6522 3a0d  ata == b"\xfe":.
+00000910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000920: 2069 6620 6461 7461 7320 3d3d 2062 2727   if datas == b''
+00000930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000940: 2020 2020 2020 2064 6174 6173 202b 3d20         datas += 
+00000950: 6461 7461 0d0a 2020 2020 2020 2020 2020  data..          
+00000960: 2020 2020 2020 2020 2020 6966 206b 2021            if k !
+00000970: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+00000980: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
+00000990: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
+000009a0: 2020 2020 2020 2020 2070 7265 203d 206b           pre = k
+000009b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000009c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000009d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000009e0: 6b20 2d20 3120 3d3d 2070 7265 3a0d 0a20  k - 1 == pre:.. 
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2020 2020 2064 6174 6173 202b 3d20         datas += 
+00000a10: 6461 7461 0d0a 2020 2020 2020 2020 2020  data..          
+00000a20: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00000a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a40: 2020 2020 2020 2020 2064 6174 6173 203d           datas =
+00000a50: 2062 225c 7866 6522 0d0a 2020 2020 2020   b"\xfe"..      
 00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 2020 2070 7265 203d 2030 0d0a 2020 2020     pre = 0..    
-00000a80: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000a90: 2020 2020 2020 2064 6174 6173 203d 2062         datas = b
-00000aa0: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
-00000ab0: 2e6c 6f67 2e64 6562 7567 2822 5f72 6561  .log.debug("_rea
-00000ac0: 643a 207b 7d22 2e66 6f72 6d61 7428 5b68  d: {}".format([h
-00000ad0: 6578 2864 6174 6129 2066 6f72 2064 6174  ex(data) for dat
-00000ae0: 6120 696e 2064 6174 6173 5d29 290d 0a20  a in datas])).. 
-00000af0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00000b00: 7461 730d 0a20 2020 2020 2020 2020 2020  tas..           
-00000b10: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-00000b20: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00000b30: 6d65 7367 2873 656c 662c 2067 656e 7265  mesg(self, genre
-00000b40: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00000b50: 7329 3a0d 0a20 2020 2020 2020 2022 2222  s):..        """
-00000b60: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
-00000b70: 3a0d 0a20 2020 2020 2020 2020 2020 2067  :..            g
-00000b80: 656e 7265 3a20 636f 6d6d 616e 6420 7479  enre: command ty
-00000b90: 7065 2028 436f 6d6d 616e 6429 0d0a 2020  pe (Command)..  
-00000ba0: 2020 2020 2020 2020 2020 2a61 7267 733a            *args:
-00000bb0: 206f 7468 6572 2064 6174 612e 0d0a 2020   other data...  
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2049 7420 6973 2063 6f6e 7665 7274 6564   It is converted
-00000be0: 2074 6f20 6f63 7461 6c20 6279 2064 6566   to octal by def
-00000bf0: 6175 6c74 2e0d 0a20 2020 2020 2020 2020  ault...         
-00000c00: 2020 2020 2020 2020 2020 4966 2074 6865            If the
-00000c10: 2064 6174 6120 6e65 6564 7320 746f 2062   data needs to b
-00000c20: 6520 656e 6361 7073 756c 6174 6564 2069  e encapsulated i
-00000c30: 6e74 6f20 6865 7861 6465 6369 6d61 6c2c  nto hexadecimal,
-00000c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c50: 2020 2020 2074 6865 2061 7272 6179 2069       the array i
-00000c60: 7320 7573 6564 2074 6f20 696e 636c 7564  s used to includ
-00000c70: 6520 7468 656d 2e20 2844 6174 6120 6361  e them. (Data ca
-00000c80: 6e6e 6f74 2062 6520 6e65 7374 6564 290d  nnot be nested).
-00000c90: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-00000ca0: 7761 7267 733a 2073 7570 706f 7274 2060  wargs: support `
-00000cb0: 6861 735f 7265 706c 7960 0d0a 2020 2020  has_reply`..    
-00000cc0: 2020 2020 2020 2020 2020 2020 6861 735f              has_
-00000cd0: 7265 706c 793a 2057 6865 7468 6572 2074  reply: Whether t
-00000ce0: 6865 7265 2069 7320 6120 7265 7475 726e  here is a return
-00000cf0: 2076 616c 7565 2074 6f20 6163 6365 7074   value to accept
-00000d00: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00000d10: 2020 2020 2020 2020 6861 735f 7265 706c          has_repl
-00000d20: 7920 3d20 6b77 6172 6773 2e67 6574 2822  y = kwargs.get("
-00000d30: 6861 735f 7265 706c 7922 2c20 4e6f 6e65  has_reply", None
-00000d40: 290d 0a20 2020 2020 2020 2072 6561 6c5f  )..        real_
-00000d50: 636f 6d6d 616e 6420 3d20 7365 6c66 2e5f  command = self._
-00000d60: 7072 6f63 6573 735f 6461 7461 5f63 6f6d  process_data_com
-00000d70: 6d61 6e64 2867 656e 7265 2c20 7365 6c66  mand(genre, self
-00000d80: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-00000d90: 655f 5f2c 2061 7267 7329 0d0a 2020 2020  e__, args)..    
-00000da0: 2020 2020 636f 6d6d 616e 6420 3d20 5b0d      command = [.
-00000db0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-00000dc0: 746f 636f 6c43 6f64 652e 4845 4144 4552  tocolCode.HEADER
-00000dd0: 2e76 616c 7565 2c0d 0a20 2020 2020 2020  .value,..       
-00000de0: 2020 2020 2050 726f 746f 636f 6c43 6f64       ProtocolCod
-00000df0: 652e 4845 4144 4552 2e76 616c 7565 2c0d  e.HEADER.value,.
-00000e00: 0a20 2020 2020 2020 205d 0d0a 2020 2020  .        ]..    
-00000e10: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00000e20: 6528 6765 6e72 652c 206c 6973 7429 3a0d  e(genre, list):.
-00000e30: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00000e40: 2064 6174 6120 696e 2067 656e 7265 3a0d   data in genre:.
-00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e60: 2063 6f6d 6d61 6e64 2e61 7070 656e 6428   command.append(
-00000e70: 6461 7461 290d 0a20 2020 2020 2020 2065  data)..        e
-00000e80: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000e90: 2020 636f 6d6d 616e 642e 6170 7065 6e64    command.append
-00000ea0: 2867 656e 7265 290d 0a20 2020 2020 2020  (genre)..       
-00000eb0: 2063 6f6d 6d61 6e64 2e61 7070 656e 6428   command.append(
-00000ec0: 7265 616c 5f63 6f6d 6d61 6e64 290d 0a20  real_command).. 
-00000ed0: 2020 2020 2020 2063 6f6d 6d61 6e64 203d         command =
-00000ee0: 2073 656c 662e 5f66 6c61 7474 656e 2863   self._flatten(c
-00000ef0: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
-00000f00: 2069 6620 6765 6e72 6520 3d3d 2050 726f   if genre == Pro
-00000f10: 746f 636f 6c43 6f64 652e 5345 545f 4c45  tocolCode.SET_LE
-00000f20: 442e 7661 6c75 653a 0d0a 2020 2020 2020  D.value:..      
-00000f30: 2020 2020 2020 636f 6d6d 616e 642e 6170        command.ap
-00000f40: 7065 6e64 2873 756d 2863 6f6d 6d61 6e64  pend(sum(command
-00000f50: 5b32 3a5d 2920 2620 3078 6666 290d 0a20  [2:]) & 0xff).. 
-00000f60: 2020 2020 2020 2065 6c69 6620 6765 6e72         elif genr
-00000f70: 6520 3d3d 2050 726f 746f 636f 6c43 6f64  e == ProtocolCod
-00000f80: 652e 4745 545f 4649 524d 5741 5245 5f56  e.GET_FIRMWARE_V
-00000f90: 4552 5349 4f4e 2e76 616c 7565 3a0d 0a20  ERSION.value:.. 
-00000fa0: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
-00000fb0: 6e64 2e61 7070 656e 6428 3429 0d0a 2020  nd.append(4)..  
-00000fc0: 2020 2020 2020 656c 6966 2067 656e 7265        elif genre
-00000fd0: 203d 3d20 5072 6f74 6f63 6f6c 436f 6465   == ProtocolCode
-00000fe0: 2e47 4554 5f4d 4f54 4f52 535f 4355 5252  .GET_MOTORS_CURR
-00000ff0: 454e 542e 7661 6c75 653a 0d0a 2020 2020  ENT.value:..    
-00001000: 2020 2020 2020 2020 636f 6d6d 616e 642e          command.
-00001010: 6170 7065 6e64 2835 290d 0a20 2020 2020  append(5)..     
-00001020: 2020 2065 6c69 6620 6765 6e72 6520 3d3d     elif genre ==
-00001030: 2050 726f 746f 636f 6c43 6f64 652e 4745   ProtocolCode.GE
-00001040: 545f 4241 5454 4552 595f 494e 464f 2e76  T_BATTERY_INFO.v
-00001050: 616c 7565 3a0d 0a20 2020 2020 2020 2020  alue:..         
-00001060: 2020 2063 6f6d 6d61 6e64 2e61 7070 656e     command.appen
-00001070: 6428 3629 0d0a 2020 2020 2020 2020 656c  d(6)..        el
-00001080: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00001090: 2023 2064 656c 2063 6f6d 6d61 6e64 5b32   # del command[2
-000010a0: 5d0d 0a20 2020 2020 2020 2020 2020 2063  ]..            c
-000010b0: 6f6d 6d61 6e64 2e61 7070 656e 6428 7375  ommand.append(su
-000010c0: 6d28 636f 6d6d 616e 645b 323a 5d29 2026  m(command[2:]) &
-000010d0: 2030 7866 6629 0d0a 2020 2020 2020 2020   0xff)..        
-000010e0: 7365 6c66 2e5f 7772 6974 6528 636f 6d6d  self._write(comm
-000010f0: 616e 6429 0d0a 2020 2020 2020 2020 6966  and)..        if
-00001100: 2068 6173 5f72 6570 6c79 3a0d 0a20 2020   has_reply:..   
-00001110: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00001120: 7365 6c66 2e5f 7265 6164 2863 6f6d 6d61  self._read(comma
-00001130: 6e64 290d 0a20 2020 2020 2020 2020 2020  nd)..           
-00001140: 2069 6620 6461 7461 3a0d 0a20 2020 2020   if data:..     
-00001150: 2020 2020 2020 2020 2020 2069 6620 6765             if ge
-00001160: 6e72 6520 3d3d 2050 726f 746f 636f 6c43  nre == ProtocolC
-00001170: 6f64 652e 4745 545f 4649 524d 5741 5245  ode.GET_FIRMWARE
-00001180: 5f56 4552 5349 4f4e 2e76 616c 7565 3a0d  _VERSION.value:.
-00001190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011a0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000011b0: 2e5f 696e 7432 636f 6f72 6428 6461 7461  ._int2coord(data
-000011c0: 5b34 5d29 0d0a 2020 2020 2020 2020 2020  [4])..          
-000011d0: 2020 2020 2020 656c 6966 2067 656e 7265        elif genre
-000011e0: 203d 3d20 5072 6f74 6f63 6f6c 436f 6465   == ProtocolCode
-000011f0: 2e47 4554 5f4d 4f54 4f52 535f 4355 5252  .GET_MOTORS_CURR
-00001200: 454e 542e 7661 6c75 653a 0d0a 2020 2020  ENT.value:..    
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 7265 7475 726e 2073 656c 662e 5f64 6563  return self._dec
-00001230: 6f64 655f 696e 7431 3628 6461 7461 5b34  ode_int16(data[4
-00001240: 3a36 5d29 0d0a 2020 2020 2020 2020 2020  :6])..          
-00001250: 2020 2020 2020 656c 6966 2050 726f 746f        elif Proto
-00001260: 636f 6c43 6f64 652e 4745 545f 4241 5454  colCode.GET_BATT
-00001270: 4552 595f 494e 464f 2e76 616c 7565 3a0d  ERY_INFO.value:.
-00001280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001290: 2020 2020 2062 7974 655f 3120 3d20 6269       byte_1 = bi
-000012a0: 6e28 6461 7461 5b34 5d29 5b32 3a5d 0d0a  n(data[4])[2:]..
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 7265 7320 3d5b 5d0d 0a20 2020      res =[]..   
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2077 6869 6c65 206c 656e 2862 7974 655f   while len(byte_
-000012f0: 3129 2021 3d20 363a 0d0a 2020 2020 2020  1) != 6:..      
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 6279 7465 5f31 203d 2022 3022 2b62    byte_1 = "0"+b
-00001320: 7974 655f 310d 0a20 2020 2020 2020 2020  yte_1..         
-00001330: 2020 2020 2020 2020 2020 2072 6573 2e61             res.a
-00001340: 7070 656e 6428 6279 7465 5f31 290d 0a20  ppend(byte_1).. 
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 2072 6573 2e61 7070 656e 6428 7365     res.append(se
-00001370: 6c66 2e5f 696e 7432 636f 6f72 6428 6461  lf._int2coord(da
-00001380: 7461 5b35 5d29 290d 0a20 2020 2020 2020  ta[5]))..       
-00001390: 2020 2020 2020 2020 2020 2020 2072 6573               res
-000013a0: 2e61 7070 656e 6428 7365 6c66 2e5f 696e  .append(self._in
-000013b0: 7432 636f 6f72 6428 6461 7461 5b36 5d29  t2coord(data[6])
-000013c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000013d0: 2020 2020 2020 2069 6620 6279 7465 5f31         if byte_1
-000013e0: 5b30 5d20 3d3d 2022 3022 3a0d 0a20 2020  [0] == "0":..   
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 2020 2072 6573 5b2d 315d 203d 2030       res[-1] = 0
-00001410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001420: 2020 2020 2020 656c 6966 2062 7974 655f        elif byte_
-00001430: 315b 315d 203d 3d20 2230 223a 0d0a 2020  1[1] == "0":..  
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 2020 2020 2020 7265 735b 315d 203d 2030        res[1] = 0
-00001460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001470: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00001480: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001490: 7072 696e 7428 7265 7329 0d0a 2020 2020  print(res)..    
-000014a0: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
-000014b0: 0a20 2020 200d 0a20 2020 2064 6566 2073  .    ..    def s
-000014c0: 6574 5f6c 6564 2873 656c 662c 206d 6f64  et_led(self, mod
-000014d0: 652c 2052 2c20 472c 2042 293a 0d0a 2020  e, R, G, B):..  
-000014e0: 2020 2020 2020 2222 2253 6574 2075 7020        """Set up 
-000014f0: 4c45 4420 6c69 6768 7473 0d0a 0d0a 2020  LED lights....  
-00001500: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00001510: 2020 2020 2020 2020 206d 6f64 6520 2869           mode (i
-00001520: 6e74 293a 2031 202d 2053 6574 204c 4544  nt): 1 - Set LED
-00001530: 206c 6967 6874 2063 6f6c 6f72 2e20 3220   light color. 2 
-00001540: 2d20 5365 7420 7468 6520 4c45 4420 6c69  - Set the LED li
-00001550: 6768 7420 746f 2062 6c69 6e6b 0d0a 2020  ght to blink..  
-00001560: 2020 2020 2020 2020 2020 5220 2869 6e74            R (int
-00001570: 293a 2030 207e 2032 3535 0d0a 2020 2020  ): 0 ~ 255..    
-00001580: 2020 2020 2020 2020 4720 2869 6e74 293a          G (int):
-00001590: 2030 207e 2032 3535 0d0a 2020 2020 2020   0 ~ 255..      
-000015a0: 2020 2020 2020 4220 2869 6e74 293a 2030        B (int): 0
-000015b0: 207e 2032 3535 0d0a 2020 2020 2020 2020   ~ 255..        
-000015c0: 2222 220d 0a20 2020 2020 2020 2063 616c  """..        cal
-000015d0: 6962 7261 7469 6f6e 5f70 6172 616d 6574  ibration_paramet
-000015e0: 6572 7328 636c 6173 735f 6e61 6d65 203d  ers(class_name =
-000015f0: 2073 656c 662e 5f5f 636c 6173 735f 5f2e   self.__class__.
-00001600: 5f5f 6e61 6d65 5f5f 2c20 7267 623d 5b52  __name__, rgb=[R
-00001610: 2c47 2c42 5d2c 206c 6564 5f6d 6f64 653d  ,G,B], led_mode=
-00001620: 6d6f 6465 290d 0a20 2020 2020 2020 2072  mode)..        r
-00001630: 6574 7572 6e20 7365 6c66 2e5f 6d65 7367  eturn self._mesg
-00001640: 2850 726f 746f 636f 6c43 6f64 652e 5345  (ProtocolCode.SE
-00001650: 545f 4c45 442e 7661 6c75 652c 206d 6f64  T_LED.value, mod
-00001660: 652c 2052 2c20 472c 2042 290d 0a20 2020  e, R, G, B)..   
-00001670: 200d 0a20 2020 2064 6566 2067 6574 5f66   ..    def get_f
-00001680: 6972 6d77 6172 655f 7665 7273 696f 6e28  irmware_version(
-00001690: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000016a0: 2222 2247 6574 2066 6972 6d77 6172 6520  """Get firmware 
-000016b0: 7665 7273 696f 6e20 6e75 6d62 6572 0d0a  version number..
-000016c0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000016d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000016e0: 2e5f 6d65 7367 2850 726f 746f 636f 6c43  ._mesg(ProtocolC
-000016f0: 6f64 652e 4745 545f 4649 524d 5741 5245  ode.GET_FIRMWARE
-00001700: 5f56 4552 5349 4f4e 2e76 616c 7565 2c20  _VERSION.value, 
-00001710: 6861 735f 7265 706c 7920 3d20 5472 7565  has_reply = True
-00001720: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
-00001730: 2067 6574 5f6d 6f74 6f72 735f 6375 7272   get_motors_curr
-00001740: 656e 7428 7365 6c66 293a 0d0a 2020 2020  ent(self):..    
-00001750: 2020 2020 2222 2247 6574 2074 6865 2074      """Get the t
-00001760: 6f74 616c 2063 7572 7265 6e74 206f 6620  otal current of 
-00001770: 7468 6520 6d6f 746f 720d 0a20 2020 2020  the motor..     
-00001780: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00001790: 7265 7475 726e 2073 656c 662e 5f6d 6573  return self._mes
-000017a0: 6728 5072 6f74 6f63 6f6c 436f 6465 2e47  g(ProtocolCode.G
-000017b0: 4554 5f4d 4f54 4f52 535f 4355 5252 454e  ET_MOTORS_CURREN
-000017c0: 542e 7661 6c75 652c 2068 6173 5f72 6570  T.value, has_rep
-000017d0: 6c79 203d 2054 7275 6529 0d0a 2020 2020  ly = True)..    
-000017e0: 0d0a 2020 2020 6465 6620 6765 745f 6261  ..    def get_ba
-000017f0: 7474 6572 795f 696e 666f 2873 656c 6629  ttery_info(self)
-00001800: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
-00001810: 6164 2062 6174 7465 7279 2069 6e66 6f72  ad battery infor
-00001820: 6d61 7469 6f6e 0d0a 2020 2020 2020 2020  mation..        
-00001830: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00001840: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-00001850: 6973 7420 3a20 5b62 6174 7465 7279 5f64  ist : [battery_d
-00001860: 6174 612c 2062 6174 7465 7279 5f31 5f76  ata, battery_1_v
-00001870: 6f6c 7461 6765 2c20 6261 7474 6572 795f  oltage, battery_
-00001880: 325f 766f 6c74 6167 655d 2e0d 0a20 2020  2_voltage]...   
-00001890: 2020 2020 2020 2020 2020 2020 2062 6174               bat
-000018a0: 7465 7279 5f64 6174 613a 0d0a 2020 2020  tery_data:..    
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 4120 7374 7269 6e67 206f 6620 6c65 6e67  A string of leng
-000018d0: 7468 2036 2c20 7265 7072 6573 656e 7465  th 6, represente
-000018e0: 6420 6672 6f6d 206c 6566 7420 746f 2072  d from left to r
-000018f0: 6967 6874 3a20 0d0a 2020 2020 2020 2020  ight: ..        
-00001900: 2020 2020 2020 2020 2020 2020 6269 7435              bit5
-00001910: 2c20 6269 7434 2c20 6269 7433 2c20 6269  , bit4, bit3, bi
-00001920: 7432 2c20 6269 7431 2c20 6269 7430 2e0d  t2, bit1, bit0..
-00001930: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00001940: 2020 2020 2020 2062 6974 3520 3a20 4261         bit5 : Ba
-00001950: 7474 6572 7920 3220 6973 2069 6e73 6572  ttery 2 is inser
-00001960: 7465 6420 696e 746f 2074 6865 2069 6e74  ted into the int
-00001970: 6572 6661 6365 2031 206d 6561 6e73 2069  erface 1 means i
-00001980: 6e73 6572 7465 642c 2030 2069 7320 6e6f  nserted, 0 is no
-00001990: 7420 696e 7365 7274 6564 2e0d 0a20 2020  t inserted...   
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2062 6974 3420 3a20 4261 7474 6572 7920   bit4 : Battery 
-000019c0: 3120 6973 2069 6e73 6572 7465 6420 696e  1 is inserted in
-000019d0: 746f 2074 6865 2069 6e74 6572 6661 6365  to the interface
-000019e0: 2c20 3120 6d65 616e 7320 696e 7365 7274  , 1 means insert
-000019f0: 6564 2c20 3020 6973 206e 6f74 2069 6e73  ed, 0 is not ins
-00001a00: 6572 7465 642e 0d0a 2020 2020 2020 2020  erted...        
-00001a10: 2020 2020 2020 2020 2020 2020 6269 7433              bit3
-00001a20: 203a 2054 6865 2061 6461 7074 6572 2069   : The adapter i
-00001a30: 7320 706c 7567 6765 6420 696e 746f 2074  s plugged into t
-00001a40: 6865 2069 6e74 6572 6661 6365 2031 206d  he interface 1 m
-00001a50: 6561 6e73 2070 6c75 6767 6564 2069 6e2c  eans plugged in,
-00001a60: 2030 206e 6f74 2070 6c75 6767 6564 2069   0 not plugged i
-00001a70: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-00001a80: 2020 2020 2020 2020 6269 7432 203a 2054          bit2 : T
-00001a90: 6865 2063 6861 7267 696e 6720 7069 6c65  he charging pile
-00001aa0: 2069 7320 696e 7365 7274 6564 2069 6e74   is inserted int
-00001ab0: 6f20 7468 6520 696e 7465 7266 6163 652c  o the interface,
-00001ac0: 2031 206d 6561 6e73 2070 6c75 6767 6564   1 means plugged
-00001ad0: 2069 6e2c 2030 2069 7320 6e6f 7420 706c   in, 0 is not pl
-00001ae0: 7567 6765 6420 696e 2e0d 0a20 2020 2020  ugged in...     
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00001b00: 6974 3120 3a20 4261 7474 6572 7920 3220  it1 : Battery 2 
-00001b10: 6368 6172 6769 6e67 206c 6967 6874 2030  charging light 0
-00001b20: 206d 6561 6e73 206f 6666 2c20 3120 6d65   means off, 1 me
-00001b30: 616e 7320 6f6e 2e0d 0a20 2020 2020 2020  ans on...       
-00001b40: 2020 2020 2020 2020 2020 2020 2062 6974               bit
-00001b50: 3020 3a20 4261 7474 6572 7920 3120 6368  0 : Battery 1 ch
-00001b60: 6172 6769 6e67 206c 6967 6874 2c20 3020  arging light, 0 
-00001b70: 6d65 616e 7320 6f66 662c 2031 206d 6561  means off, 1 mea
-00001b80: 6e73 206f 6e2e 0d0a 2020 2020 2020 2020  ns on...        
-00001b90: 2020 2020 2020 2020 6261 7474 6572 795f          battery_
-00001ba0: 315f 766f 6c74 6167 6520 3a20 4261 7474  1_voltage : Batt
-00001bb0: 6572 7920 3120 766f 6c74 6167 6520 696e  ery 1 voltage in
-00001bc0: 2076 6f6c 7473 2e0d 0a20 2020 2020 2020   volts...       
-00001bd0: 2020 2020 2020 2020 2062 6174 7465 7279           battery
-00001be0: 5f32 5f76 6f6c 7461 6765 203a 2042 6174  _2_voltage : Bat
-00001bf0: 7465 7279 2032 2076 6f6c 7461 6765 2069  tery 2 voltage i
-00001c00: 6e20 766f 6c74 732e 0d0a 2020 2020 2020  n volts...      
-00001c10: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00001c20: 6574 7572 6e20 7365 6c66 2e5f 6d65 7367  eturn self._mesg
-00001c30: 2850 726f 746f 636f 6c43 6f64 652e 4745  (ProtocolCode.GE
-00001c40: 545f 4241 5454 4552 595f 494e 464f 2e76  T_BATTERY_INFO.v
-00001c50: 616c 7565 2c20 6861 735f 7265 706c 7920  alue, has_reply 
-00001c60: 3d20 5472 7565 290d 0a20 2020 200d 0a20  = True)..    .. 
-00001c70: 2020 2023 2064 6566 206d 6f76 655f 636f     # def move_co
-00001c80: 6e74 726f 6c28 7365 6c66 2c20 6469 7265  ntrol(self, dire
-00001c90: 6374 696f 6e5f 312c 2064 6972 6563 7469  ction_1, directi
-00001ca0: 6f6e 5f32 2c20 6469 7265 6374 696f 6e5f  on_2, direction_
-00001cb0: 3329 3a0d 0a20 2020 2023 2020 2020 2022  3):..    #     "
-00001cc0: 2222 436f 6e74 726f 6c20 7468 6520 6361  ""Control the ca
-00001cd0: 7220 746f 2072 6f74 6174 6520 666f 7277  r to rotate forw
-00001ce0: 6172 642c 2062 6163 6b77 6172 642c 206c  ard, backward, l
-00001cf0: 6566 742c 2072 6967 6874 2061 6e64 2066  eft, right and f
-00001d00: 6f72 7761 7264 2f63 6f75 6e74 6572 636c  orward/countercl
-00001d10: 6f63 6b77 6973 650d 0a0d 0a20 2020 2023  ockwise....    #
-00001d20: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
-00001d30: 2320 2020 2020 2020 2020 6469 7265 6374  #         direct
-00001d40: 696f 6e5f 3120 2869 6e74 293a 2043 6f6e  ion_1 (int): Con
-00001d50: 7472 6f6c 2066 6f72 7761 7264 206f 7220  trol forward or 
-00001d60: 6261 636b 7761 7264 3a20 3020 7e20 3132  backward: 0 ~ 12
-00001d70: 3720 6973 2062 6163 6b77 6172 642c 2031  7 is backward, 1
-00001d80: 3239 207e 2032 3535 2069 7320 666f 7277  29 ~ 255 is forw
-00001d90: 6172 642c 2031 3238 2069 7320 7374 6f70  ard, 128 is stop
-00001da0: 2e0d 0a20 2020 2023 2020 2020 2020 2020  ...    #        
-00001db0: 2064 6972 6563 7469 6f6e 5f32 2028 696e   direction_2 (in
-00001dc0: 7429 3a20 636f 6e74 726f 6c20 6c65 6674  t): control left
-00001dd0: 2061 6e64 2072 6967 6874 206d 6f76 656d   and right movem
-00001de0: 656e 743a 2030 207e 2031 3237 2069 7320  ent: 0 ~ 127 is 
-00001df0: 7269 6768 742c 2031 3239 207e 2032 3535  right, 129 ~ 255
-00001e00: 2069 7320 6c65 6674 2c20 3132 3820 6973   is left, 128 is
-00001e10: 2073 746f 702e 0d0a 2020 2020 2320 2020   stop...    #   
-00001e20: 2020 2020 2020 6469 7265 6374 696f 6e5f        direction_
-00001e30: 3320 2869 6e74 293a 2063 6f6e 7472 6f6c  3 (int): control
-00001e40: 2072 6f74 6174 696f 6e3a 2030 207e 2031   rotation: 0 ~ 1
-00001e50: 3237 2069 7320 636c 6f63 6b77 6973 652c  27 is clockwise,
-00001e60: 2031 3239 207e 2032 3535 2069 7320 636f   129 ~ 255 is co
-00001e70: 756e 7465 7263 6c6f 636b 7769 7365 2c20  unterclockwise, 
-00001e80: 3132 3820 6973 2073 746f 702e 0d0a 2020  128 is stop...  
-00001e90: 2020 2320 2020 2020 2222 220d 0a20 2020    #     """..   
-00001ea0: 2023 2020 2020 2063 616c 6962 7261 7469   #     calibrati
-00001eb0: 6f6e 5f70 6172 616d 6574 6572 7328 636c  on_parameters(cl
-00001ec0: 6173 735f 6e61 6d65 203d 2073 656c 662e  ass_name = self.
-00001ed0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-00001ee0: 5f5f 2c20 6469 7265 6374 696f 6e5f 313d  __, direction_1=
-00001ef0: 6469 7265 6374 696f 6e5f 312c 2064 6972  direction_1, dir
-00001f00: 6563 7469 6f6e 5f32 3d64 6972 6563 7469  ection_2=directi
-00001f10: 6f6e 5f32 2c64 6972 6563 7469 6f6e 5f33  on_2,direction_3
-00001f20: 3d64 6972 6563 7469 6f6e 5f33 290d 0a20  =direction_3).. 
-00001f30: 2020 2023 2020 2020 2072 6574 7572 6e20     #     return 
-00001f40: 7365 6c66 2e5f 6d65 7367 2864 6972 6563  self._mesg(direc
-00001f50: 7469 6f6e 5f31 2c20 6469 7265 6374 696f  tion_1, directio
-00001f60: 6e5f 322c 2064 6972 6563 7469 6f6e 5f33  n_2, direction_3
-00001f70: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
-00001f80: 2067 6f5f 6168 6561 6428 7365 6c66 2c20   go_ahead(self, 
-00001f90: 676f 5f73 7065 6564 2c20 7469 6d65 6f75  go_speed, timeou
-00001fa0: 743d 3529 3a0d 0a20 2020 2020 2020 2022  t=5):..        "
-00001fb0: 2222 436f 6e74 726f 6c20 7468 6520 6361  ""Control the ca
-00001fc0: 7220 746f 206d 6f76 6520 666f 7277 6172  r to move forwar
-00001fd0: 642e 2053 656e 6420 636f 6e74 726f 6c20  d. Send control 
-00001fe0: 636f 6d6d 616e 6473 2065 7665 7279 2031  commands every 1
-00001ff0: 3030 6d73 2e20 7769 7468 2061 2064 6566  00ms. with a def
-00002000: 6175 6c74 206d 6f74 696f 6e20 7469 6d65  ault motion time
-00002010: 206f 6620 3520 7365 636f 6e64 732e 0d0a   of 5 seconds...
-00002020: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-00002030: 0a20 2020 2020 2020 2020 2020 2067 6f5f  .            go_
-00002040: 7370 6565 6420 2869 6e74 293a 2031 207e  speed (int): 1 ~
-00002050: 2031 3237 2069 7320 666f 7277 6172 642e   127 is forward.
-00002060: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-00002070: 6d65 6f75 7420 2869 6e74 293a 2064 6566  meout (int): def
-00002080: 6175 6c74 2035 2073 2e0d 0a20 2020 2020  ault 5 s...     
-00002090: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000020a0: 2320 676f 5f73 7065 6564 2028 696e 7429  # go_speed (int)
-000020b0: 3a20 3132 3920 7e20 3235 3520 6973 2066  : 129 ~ 255 is f
-000020c0: 6f72 7761 7264 0d0a 2020 2020 2020 2020  orward..        
-000020d0: 6361 6c69 6272 6174 696f 6e5f 7061 7261  calibration_para
-000020e0: 6d65 7465 7273 2863 6c61 7373 5f6e 616d  meters(class_nam
-000020f0: 6520 3d20 7365 6c66 2e5f 5f63 6c61 7373  e = self.__class
-00002100: 5f5f 2e5f 5f6e 616d 655f 5f2c 2064 6174  __.__name__, dat
-00002110: 613d 676f 5f73 7065 6564 290d 0a20 2020  a=go_speed)..   
-00002120: 2020 2020 2074 203d 2074 696d 652e 7469       t = time.ti
-00002130: 6d65 2829 0d0a 2020 2020 2020 2020 7768  me()..        wh
-00002140: 696c 6520 7469 6d65 2e74 696d 6528 2920  ile time.time() 
-00002150: 2d20 7420 3c20 7469 6d65 6f75 743a 0d0a  - t < timeout:..
-00002160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002170: 2e5f 6d65 7367 2831 3238 2b67 6f5f 7370  ._mesg(128+go_sp
-00002180: 6565 642c 2031 3238 2c20 3132 3829 0d0a  eed, 128, 128)..
-00002190: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-000021a0: 2e73 6c65 6570 2830 2e31 290d 0a20 2020  .sleep(0.1)..   
-000021b0: 2020 2020 2073 656c 662e 7374 6f70 2829       self.stop()
-000021c0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000021d0: 6465 6620 7265 7472 6561 7428 7365 6c66  def retreat(self
-000021e0: 2c20 6261 636b 5f73 7065 6564 2c20 7469  , back_speed, ti
-000021f0: 6d65 6f75 743d 3529 3a0d 0a20 2020 2020  meout=5):..     
-00002200: 2020 2022 2222 436f 6e74 726f 6c20 7468     """Control th
-00002210: 6520 6361 7220 6261 636b 2e20 5365 6e64  e car back. Send
-00002220: 2063 6f6e 7472 6f6c 2063 6f6d 6d61 6e64   control command
-00002230: 7320 6576 6572 7920 3130 306d 732e 2077  s every 100ms. w
-00002240: 6974 6820 6120 6465 6661 756c 7420 6d6f  ith a default mo
-00002250: 7469 6f6e 2074 696d 6520 6f66 2035 2073  tion time of 5 s
-00002260: 6563 6f6e 6473 0d0a 0d0a 2020 2020 2020  econds....      
-00002270: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00002280: 2020 2020 2062 6163 6b5f 7370 6565 6420       back_speed 
-00002290: 2869 6e74 293a 2031 207e 2031 3237 2069  (int): 1 ~ 127 i
-000022a0: 7320 6261 636b 7761 7264 0d0a 2020 2020  s backward..    
-000022b0: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
-000022c0: 2869 6e74 293a 2064 6566 6175 6c74 2035  (int): default 5
-000022d0: 2073 2e0d 0a20 2020 2020 2020 2022 2222   s...        """
-000022e0: 0d0a 2020 2020 2020 2020 6361 6c69 6272  ..        calibr
-000022f0: 6174 696f 6e5f 7061 7261 6d65 7465 7273  ation_parameters
-00002300: 2863 6c61 7373 5f6e 616d 6520 3d20 7365  (class_name = se
-00002310: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
-00002320: 616d 655f 5f2c 2064 6174 613d 6261 636b  ame__, data=back
-00002330: 5f73 7065 6564 290d 0a20 2020 2020 2020  _speed)..       
-00002340: 2074 203d 2074 696d 652e 7469 6d65 2829   t = time.time()
-00002350: 0d0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-00002360: 7469 6d65 2e74 696d 6528 2920 2d20 7420  time.time() - t 
-00002370: 3c20 7469 6d65 6f75 743a 0d0a 2020 2020  < timeout:..    
-00002380: 2020 2020 2020 2020 7365 6c66 2e5f 6d65          self._me
-00002390: 7367 2831 3238 2d62 6163 6b5f 7370 6565  sg(128-back_spee
-000023a0: 642c 2031 3238 2c20 3132 3829 0d0a 2020  d, 128, 128)..  
-000023b0: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-000023c0: 6c65 6570 2830 2e31 290d 0a20 2020 2020  leep(0.1)..     
-000023d0: 2020 2073 656c 662e 7374 6f70 2829 0d0a     self.stop()..
-000023e0: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-000023f0: 6620 7061 6e5f 6c65 6674 2873 656c 662c  f pan_left(self,
-00002400: 2070 616e 5f6c 6566 745f 7370 6565 642c   pan_left_speed,
-00002410: 2074 696d 656f 7574 3d35 293a 0d0a 2020   timeout=5):..  
-00002420: 2020 2020 2020 2222 2243 6f6e 7472 6f6c        """Control
-00002430: 2074 6865 2063 6172 2074 6f20 7061 6e20   the car to pan 
-00002440: 746f 2074 6865 206c 6566 742e 2053 656e  to the left. Sen
-00002450: 6420 636f 6e74 726f 6c20 636f 6d6d 616e  d control comman
-00002460: 6473 2065 7665 7279 2031 3030 6d73 2e20  ds every 100ms. 
-00002470: 7769 7468 2061 2064 6566 6175 6c74 206d  with a default m
-00002480: 6f74 696f 6e20 7469 6d65 206f 6620 3520  otion time of 5 
-00002490: 7365 636f 6e64 730d 0a0d 0a20 2020 2020  seconds....     
-000024a0: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-000024b0: 2020 2020 2020 7061 6e5f 6c65 6674 5f73        pan_left_s
-000024c0: 7065 6564 2028 696e 7429 3a20 3120 7e20  peed (int): 1 ~ 
-000024d0: 3132 370d 0a20 2020 2020 2020 2020 2020  127..           
-000024e0: 2074 696d 656f 7574 2028 696e 7429 3a20   timeout (int): 
-000024f0: 6465 6661 756c 7420 3520 732e 0d0a 2020  default 5 s...  
-00002500: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00002510: 2020 2023 2070 616e 5f6c 6566 745f 7370     # pan_left_sp
-00002520: 6565 6420 2869 6e74 293a 2031 3239 207e  eed (int): 129 ~
-00002530: 2032 3535 0d0a 2020 2020 2020 2020 6361   255..        ca
-00002540: 6c69 6272 6174 696f 6e5f 7061 7261 6d65  libration_parame
-00002550: 7465 7273 2863 6c61 7373 5f6e 616d 6520  ters(class_name 
-00002560: 3d20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  = self.__class__
-00002570: 2e5f 5f6e 616d 655f 5f2c 2064 6174 613d  .__name__, data=
-00002580: 7061 6e5f 6c65 6674 5f73 7065 6564 290d  pan_left_speed).
-00002590: 0a20 2020 2020 2020 2074 203d 2074 696d  .        t = tim
-000025a0: 652e 7469 6d65 2829 0d0a 2020 2020 2020  e.time()..      
-000025b0: 2020 7768 696c 6520 7469 6d65 2e74 696d    while time.tim
-000025c0: 6528 2920 2d20 7420 3c20 7469 6d65 6f75  e() - t < timeou
-000025d0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-000025e0: 7365 6c66 2e5f 6d65 7367 2831 3238 2c20  self._mesg(128, 
-000025f0: 3132 382b 7061 6e5f 6c65 6674 5f73 7065  128+pan_left_spe
-00002600: 6564 2c20 3132 3829 0d0a 2020 2020 2020  ed, 128)..      
-00002610: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00002620: 2830 2e31 290d 0a20 2020 2020 2020 2073  (0.1)..        s
-00002630: 656c 662e 7374 6f70 2829 0d0a 2020 2020  elf.stop()..    
-00002640: 2020 2020 0d0a 2020 2020 6465 6620 7061      ..    def pa
-00002650: 6e5f 7269 6768 7428 7365 6c66 2c20 7061  n_right(self, pa
-00002660: 6e5f 7269 6768 745f 7370 6565 642c 2074  n_right_speed, t
-00002670: 696d 656f 7574 3d35 293a 0d0a 2020 2020  imeout=5):..    
-00002680: 2020 2020 2222 2243 6f6e 7472 6f6c 2074      """Control t
-00002690: 6865 2063 6172 2074 6f20 7061 6e20 746f  he car to pan to
-000026a0: 2074 6865 2072 6967 6874 2e20 5365 6e64   the right. Send
-000026b0: 2063 6f6e 7472 6f6c 2063 6f6d 6d61 6e64   control command
-000026c0: 7320 6576 6572 7920 3130 306d 732e 2077  s every 100ms. w
-000026d0: 6974 6820 6120 6465 6661 756c 7420 6d6f  ith a default mo
-000026e0: 7469 6f6e 2074 696d 6520 6f66 2035 2073  tion time of 5 s
-000026f0: 6563 6f6e 6473 0d0a 0d0a 2020 2020 2020  econds....      
-00002700: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00002710: 2020 2020 2070 616e 5f72 6967 6874 5f73       pan_right_s
-00002720: 7065 6564 2028 696e 7429 3a20 3120 7e20  peed (int): 1 ~ 
-00002730: 3132 370d 0a20 2020 2020 2020 2020 2020  127..           
-00002740: 2074 696d 656f 7574 2028 696e 7429 3a20   timeout (int): 
-00002750: 6465 6661 756c 7420 3520 732e 0d0a 2020  default 5 s...  
-00002760: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00002770: 2020 2063 616c 6962 7261 7469 6f6e 5f70     calibration_p
-00002780: 6172 616d 6574 6572 7328 636c 6173 735f  arameters(class_
-00002790: 6e61 6d65 203d 2073 656c 662e 5f5f 636c  name = self.__cl
-000027a0: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20  ass__.__name__, 
-000027b0: 7061 6e5f 7269 6768 745f 7370 6565 643d  pan_right_speed=
-000027c0: 7061 6e5f 7269 6768 745f 7370 6565 6429  pan_right_speed)
-000027d0: 0d0a 2020 2020 2020 2020 7420 3d20 7469  ..        t = ti
-000027e0: 6d65 2e74 696d 6528 290d 0a20 2020 2020  me.time()..     
-000027f0: 2020 2077 6869 6c65 2074 696d 652e 7469     while time.ti
-00002800: 6d65 2829 202d 2074 203c 2074 696d 656f  me() - t < timeo
-00002810: 7574 3a0d 0a20 2020 2020 2020 2020 2020  ut:..           
-00002820: 2073 656c 662e 5f6d 6573 6728 3132 382c   self._mesg(128,
-00002830: 2031 3238 2d70 616e 5f72 6967 6874 5f73   128-pan_right_s
-00002840: 7065 6564 2c20 3132 3829 0d0a 2020 2020  peed, 128)..    
-00002850: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-00002860: 6570 2830 2e31 290d 0a20 2020 2020 2020  ep(0.1)..       
-00002870: 2073 656c 662e 7374 6f70 2829 0d0a 2020   self.stop()..  
-00002880: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00002890: 636c 6f63 6b77 6973 655f 726f 7461 7469  clockwise_rotati
-000028a0: 6f6e 2873 656c 662c 2072 6f74 6174 655f  on(self, rotate_
-000028b0: 7269 6768 745f 7370 6565 642c 2074 696d  right_speed, tim
-000028c0: 656f 7574 3d35 293a 0d0a 2020 2020 2020  eout=5):..      
-000028d0: 2020 2222 2243 6f6e 7472 6f6c 2074 6865    """Control the
-000028e0: 2063 6172 2074 6f20 726f 7461 7465 2063   car to rotate c
-000028f0: 6c6f 636b 7769 7365 2e20 5365 6e64 2063  lockwise. Send c
-00002900: 6f6e 7472 6f6c 2063 6f6d 6d61 6e64 7320  ontrol commands 
-00002910: 6576 6572 7920 3130 306d 732e 2077 6974  every 100ms. wit
-00002920: 6820 6120 6465 6661 756c 7420 6d6f 7469  h a default moti
-00002930: 6f6e 2074 696d 6520 6f66 2035 2073 6563  on time of 5 sec
-00002940: 6f6e 6473 0d0a 0d0a 2020 2020 2020 2020  onds....        
-00002950: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00002960: 2020 2063 6c6f 636b 7769 7365 5f72 6f74     clockwise_rot
-00002970: 6174 696f 6e5f 7370 6565 6420 2869 6e74  ation_speed (int
-00002980: 293a 2031 207e 2031 3237 0d0a 2020 2020  ): 1 ~ 127..    
-00002990: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
-000029a0: 2869 6e74 293a 2064 6566 6175 6c74 2035  (int): default 5
-000029b0: 2073 2e0d 0a20 2020 2020 2020 2022 2222   s...        """
-000029c0: 0d0a 2020 2020 2020 2020 6361 6c69 6272  ..        calibr
-000029d0: 6174 696f 6e5f 7061 7261 6d65 7465 7273  ation_parameters
-000029e0: 2863 6c61 7373 5f6e 616d 6520 3d20 7365  (class_name = se
-000029f0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
-00002a00: 616d 655f 5f2c 2072 6f74 6174 655f 7269  ame__, rotate_ri
-00002a10: 6768 745f 7370 6565 643d 726f 7461 7465  ght_speed=rotate
-00002a20: 5f72 6967 6874 5f73 7065 6564 290d 0a20  _right_speed).. 
-00002a30: 2020 2020 2020 2074 203d 2074 696d 652e         t = time.
-00002a40: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
-00002a50: 7768 696c 6520 7469 6d65 2e74 696d 6528  while time.time(
-00002a60: 2920 2d20 7420 3c20 7469 6d65 6f75 743a  ) - t < timeout:
-00002a70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00002a80: 6c66 2e5f 6d65 7367 2831 3238 2c20 3132  lf._mesg(128, 12
-00002a90: 382c 2031 3238 2d72 6f74 6174 655f 7269  8, 128-rotate_ri
-00002aa0: 6768 745f 7370 6565 6429 0d0a 2020 2020  ght_speed)..    
-00002ab0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-00002ac0: 6570 2830 2e31 290d 0a20 2020 2020 2020  ep(0.1)..       
-00002ad0: 2073 656c 662e 7374 6f70 2829 0d0a 2020   self.stop()..  
-00002ae0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002af0: 0d0a 2020 2020 6465 6620 636f 756e 7465  ..    def counte
-00002b00: 7263 6c6f 636b 7769 7365 5f72 6f74 6174  rclockwise_rotat
-00002b10: 696f 6e28 7365 6c66 2c20 726f 7461 7465  ion(self, rotate
-00002b20: 5f6c 6566 745f 7370 6565 642c 2074 696d  _left_speed, tim
-00002b30: 656f 7574 3d35 293a 0d0a 2020 2020 2020  eout=5):..      
-00002b40: 2020 2222 2243 6f6e 7472 6f6c 2074 6865    """Control the
-00002b50: 2063 6172 2074 6f20 726f 7461 7465 2063   car to rotate c
-00002b60: 6f75 6e74 6572 636c 6f63 6b77 6973 652e  ounterclockwise.
-00002b70: 2053 656e 6420 636f 6e74 726f 6c20 636f   Send control co
-00002b80: 6d6d 616e 6473 2065 7665 7279 2031 3030  mmands every 100
-00002b90: 6d73 2e20 7769 7468 2061 2064 6566 6175  ms. with a defau
-00002ba0: 6c74 206d 6f74 696f 6e20 7469 6d65 206f  lt motion time o
-00002bb0: 6620 3520 7365 636f 6e64 730d 0a0d 0a20  f 5 seconds.... 
-00002bc0: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
-00002bd0: 2020 2020 2020 2020 2020 636c 6f63 6b77            clockw
-00002be0: 6973 655f 726f 7461 7469 6f6e 5f73 7065  ise_rotation_spe
-00002bf0: 6564 2028 696e 7429 3a20 3120 7e20 3132  ed (int): 1 ~ 12
-00002c00: 370d 0a20 2020 2020 2020 2020 2020 2074  7..            t
-00002c10: 696d 656f 7574 2028 696e 7429 3a20 6465  imeout (int): de
-00002c20: 6661 756c 7420 3520 732e 0d0a 2020 2020  fault 5 s...    
-00002c30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00002c40: 2063 616c 6962 7261 7469 6f6e 5f70 6172   calibration_par
-00002c50: 616d 6574 6572 7328 636c 6173 735f 6e61  ameters(class_na
-00002c60: 6d65 203d 2073 656c 662e 5f5f 636c 6173  me = self.__clas
-00002c70: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20 726f  s__.__name__, ro
-00002c80: 7461 7465 5f6c 6566 745f 7370 6565 643d  tate_left_speed=
-00002c90: 726f 7461 7465 5f6c 6566 745f 7370 6565  rotate_left_spee
-00002ca0: 6429 0d0a 2020 2020 2020 2020 7420 3d20  d)..        t = 
-00002cb0: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00002cc0: 2020 2020 2077 6869 6c65 2074 696d 652e       while time.
-00002cd0: 7469 6d65 2829 202d 2074 203c 2074 696d  time() - t < tim
-00002ce0: 656f 7574 3a0d 0a20 2020 2020 2020 2020  eout:..         
-00002cf0: 2020 2073 656c 662e 5f6d 6573 6728 3132     self._mesg(12
-00002d00: 382c 2031 3238 2c20 3132 382b 726f 7461  8, 128, 128+rota
-00002d10: 7465 5f6c 6566 745f 7370 6565 6429 0d0a  te_left_speed)..
-00002d20: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00002d30: 2e73 6c65 6570 2830 2e31 290d 0a20 2020  .sleep(0.1)..   
-00002d40: 2020 2020 2073 656c 662e 7374 6f70 2829       self.stop()
-00002d50: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00002d60: 6465 6620 7374 6f70 2873 656c 6629 3a0d  def stop(self):.
-00002d70: 0a20 2020 2020 2020 2022 2222 7374 6f70  .        """stop
-00002d80: 206d 6f74 696f 6e0d 0a20 2020 2020 2020   motion..       
-00002d90: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-00002da0: 6c66 2e5f 6d65 7367 2831 3238 2c20 3132  lf._mesg(128, 12
-00002db0: 382c 2031 3238 290d 0a20 2020 2020 2020  8, 128)..       
-00002dc0: 200d 0a20 2020 2064 6566 2067 6574 5f6d   ..    def get_m
-00002dd0: 6375 5f69 6e66 6f28 7365 6c66 293a 0d0a  cu_info(self):..
-00002de0: 2020 2020 2020 2020 2222 2222 2222 0d0a          """"""..
-00002df0: 2020 2020 2020 2020 6461 7461 7320 3d20          datas = 
-00002e00: 7365 6c66 2e5f 7265 6164 285b 3078 6665  self._read([0xfe
-00002e10: 2c20 3078 6665 2c20 3239 5d29 0d0a 2020  , 0xfe, 29])..  
-00002e20: 2020 2020 2020 7265 7320 3d20 5b5d 0d0a        res = []..
-00002e30: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
-00002e40: 320d 0a20 2020 2020 2020 2077 6869 6c65  2..        while
-00002e50: 2069 6e64 6578 203c 206c 656e 2864 6174   index < len(dat
-00002e60: 6173 2920 2d20 323a 0d0a 2020 2020 2020  as) - 2:..      
-00002e70: 2020 2020 2020 6966 2069 6e64 6578 203c        if index <
-00002e80: 2035 3a0d 0a20 2020 2020 2020 2020 2020   5:..           
-00002e90: 2020 2020 2072 6573 2e61 7070 656e 6428       res.append(
-00002ea0: 6461 7461 735b 696e 6465 785d 290d 0a20  datas[index]).. 
-00002eb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002ec0: 6e64 6578 2b3d 310d 0a20 2020 2020 2020  ndex+=1..       
-00002ed0: 2020 2020 2065 6c69 6620 696e 6465 7820       elif index 
-00002ee0: 3c20 3137 206f 7220 696e 6465 7820 3e3d  < 17 or index >=
-00002ef0: 2032 303a 0d0a 2020 2020 2020 2020 2020   20:..          
-00002f00: 2020 2020 2020 7265 732e 6170 7065 6e64        res.append
-00002f10: 2873 656c 662e 5f64 6563 6f64 655f 696e  (self._decode_in
-00002f20: 7431 3628 6461 7461 735b 696e 6465 783a  t16(datas[index:
-00002f30: 696e 6465 782b 325d 2929 0d0a 2020 2020  index+2]))..    
-00002f40: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00002f50: 782b 3d32 0d0a 2020 2020 2020 2020 2020  x+=2..          
-00002f60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002f70: 2020 2020 656c 6966 2069 6e64 6578 203d      elif index =
-00002f80: 3d20 3137 3a0d 0a20 2020 2020 2020 2020  = 17:..         
-00002f90: 2020 2020 2020 2062 7974 655f 3120 3d20         byte_1 = 
-00002fa0: 6269 6e28 6461 7461 735b 696e 6465 785d  bin(datas[index]
-00002fb0: 295b 323a 5d0d 0a20 2020 2020 2020 2020  )[2:]..         
-00002fc0: 2020 2020 2020 2077 6869 6c65 206c 656e         while len
-00002fd0: 2862 7974 655f 3129 2021 3d20 363a 0d0a  (byte_1) != 6:..
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2020 2020 2020 2020 6279 7465 5f31 203d          byte_1 =
-00003000: 2022 3022 2b62 7974 655f 310d 0a20 2020   "0"+byte_1..   
-00003010: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00003020: 2e61 7070 656e 6428 6279 7465 5f31 290d  .append(byte_1).
-00003030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003040: 2069 6e64 6578 2b3d 310d 0a20 2020 2020   index+=1..     
-00003050: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00003060: 2020 2020 2020 2020 2065 6c69 6620 696e           elif in
-00003070: 6465 7820 3c20 3230 3a0d 0a20 2020 2020  dex < 20:..     
-00003080: 2020 2020 2020 2020 2020 2072 6573 2e61             res.a
-00003090: 7070 656e 6428 7365 6c66 2e5f 696e 7432  ppend(self._int2
-000030a0: 636f 6f72 6428 6461 7461 735b 696e 6465  coord(datas[inde
-000030b0: 785d 2929 0d0a 2020 2020 2020 2020 2020  x]))..          
-000030c0: 2020 2020 2020 696e 6465 782b 3d31 0d0a        index+=1..
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000030f0: 2072 6573 0d0a 2020 2020 0d0a 2020 2020   res..    ..    
-00003100: 6465 6620 7265 7374 6f72 6528 7365 6c66  def restore(self
-00003110: 293a 0d0a 2020 2020 2020 2020 2222 224d  ):..        """M
-00003120: 6f74 6f72 2073 7461 6c6c 2072 6563 6f76  otor stall recov
-00003130: 6572 7922 2222 0d0a 2020 2020 2020 2020  ery"""..        
-00003140: 7365 6c66 2e5f 6d65 7367 2850 726f 746f  self._mesg(Proto
-00003150: 636f 6c43 6f64 652e 5245 5354 4f52 452e  colCode.RESTORE.
-00003160: 7661 6c75 652c 2031 290d 0a20 2020 200d  value, 1)..    .
-00003170: 0a20 2020 2023 2064 6566 2067 6574 5f62  .    # def get_b
-00003180: 6174 7465 7279 5f76 6f6c 7461 6765 2873  attery_voltage(s
-00003190: 656c 662c 206e 756d 3d31 293a 0d0a 2020  elf, num=1):..  
-000031a0: 2020 2320 2020 2020 2222 2247 6574 2062    #     """Get b
-000031b0: 6174 7465 7279 2076 6f6c 7461 6765 0d0a  attery voltage..
-000031c0: 0d0a 2020 2020 2320 2020 2020 4172 6773  ..    #     Args
-000031d0: 3a0d 0a20 2020 2023 2020 2020 2020 2020  :..    #        
-000031e0: 206e 756d 2028 696e 742c 206f 7074 696f   num (int, optio
-000031f0: 6e61 6c29 3a20 4261 7474 6572 7920 4944  nal): Battery ID
-00003200: 206e 756d 6265 722e 2044 6566 6175 6c74   number. Default
-00003210: 7320 746f 2031 2e0d 0a20 2020 2023 2020  s to 1...    #  
-00003220: 2020 2022 2222 0d0a 2020 2020 2320 2020     """..    #   
-00003230: 2020 6d63 755f 6461 7461 203d 2073 656c    mcu_data = sel
-00003240: 662e 6765 745f 6d63 755f 696e 666f 2829  f.get_mcu_info()
-00003250: 0d0a 2020 2020 2320 2020 2020 7265 7475  ..    #     retu
-00003260: 726e 2073 656c 662e 5f6d 6573 6728 5072  rn self._mesg(Pr
-00003270: 6f74 6f63 6f6c 436f 6465 2e47 4554 5f42  otocolCode.GET_B
-00003280: 4154 5445 5259 5f49 4e46 4f2e 7661 6c75  ATTERY_INFO.valu
-00003290: 652c 2068 6173 5f72 6570 6c79 203d 2054  e, has_reply = T
-000032a0: 7275 6529                                rue)
+00000a70: 2020 6b20 3d20 310d 0a20 2020 2020 2020    k = 1..       
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2070 7265 203d 2030 0d0a 2020 2020 2020   pre = 0..      
+00000aa0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000ab0: 2020 2020 2064 6174 6173 203d 2062 2727       datas = b''
+00000ac0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00000ad0: 6f67 2e64 6562 7567 2822 5f72 6561 643a  og.debug("_read:
+00000ae0: 207b 7d22 2e66 6f72 6d61 7428 5b68 6578   {}".format([hex
+00000af0: 2864 6174 6129 2066 6f72 2064 6174 6120  (data) for data 
+00000b00: 696e 2064 6174 6173 5d29 290d 0a20 2020  in datas]))..   
+00000b10: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
+00000b20: 730d 0a20 2020 2020 2020 2020 2020 200d  s..            .
+00000b30: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00000b40: 2020 200d 0a20 2020 2064 6566 205f 6d65     ..    def _me
+00000b50: 7367 2873 656c 662c 2067 656e 7265 2c20  sg(self, genre, 
+00000b60: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00000b70: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00000b80: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
+00000b90: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
+00000ba0: 7265 3a20 636f 6d6d 616e 6420 7479 7065  re: command type
+00000bb0: 2028 436f 6d6d 616e 6429 0d0a 2020 2020   (Command)..    
+00000bc0: 2020 2020 2020 2020 2a61 7267 733a 206f          *args: o
+00000bd0: 7468 6572 2064 6174 612e 0d0a 2020 2020  ther data...    
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000bf0: 7420 6973 2063 6f6e 7665 7274 6564 2074  t is converted t
+00000c00: 6f20 6f63 7461 6c20 6279 2064 6566 6175  o octal by defau
+00000c10: 6c74 2e0d 0a20 2020 2020 2020 2020 2020  lt...           
+00000c20: 2020 2020 2020 2020 4966 2074 6865 2064          If the d
+00000c30: 6174 6120 6e65 6564 7320 746f 2062 6520  ata needs to be 
+00000c40: 656e 6361 7073 756c 6174 6564 2069 6e74  encapsulated int
+00000c50: 6f20 6865 7861 6465 6369 6d61 6c2c 0d0a  o hexadecimal,..
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 2020 2074 6865 2061 7272 6179 2069 7320     the array is 
+00000c80: 7573 6564 2074 6f20 696e 636c 7564 6520  used to include 
+00000c90: 7468 656d 2e20 2844 6174 6120 6361 6e6e  them. (Data cann
+00000ca0: 6f74 2062 6520 6e65 7374 6564 290d 0a20  ot be nested).. 
+00000cb0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+00000cc0: 7267 733a 2073 7570 706f 7274 2060 6861  rgs: support `ha
+00000cd0: 735f 7265 706c 7960 0d0a 2020 2020 2020  s_reply`..      
+00000ce0: 2020 2020 2020 2020 2020 6861 735f 7265            has_re
+00000cf0: 706c 793a 2057 6865 7468 6572 2074 6865  ply: Whether the
+00000d00: 7265 2069 7320 6120 7265 7475 726e 2076  re is a return v
+00000d10: 616c 7565 2074 6f20 6163 6365 7074 2e0d  alue to accept..
+00000d20: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00000d30: 2020 2020 2020 6861 735f 7265 706c 7920        has_reply 
+00000d40: 3d20 6b77 6172 6773 2e67 6574 2822 6861  = kwargs.get("ha
+00000d50: 735f 7265 706c 7922 2c20 4e6f 6e65 290d  s_reply", None).
+00000d60: 0a20 2020 2020 2020 2072 6561 6c5f 636f  .        real_co
+00000d70: 6d6d 616e 6420 3d20 7365 6c66 2e5f 7072  mmand = self._pr
+00000d80: 6f63 6573 735f 6461 7461 5f63 6f6d 6d61  ocess_data_comma
+00000d90: 6e64 2867 656e 7265 2c20 7365 6c66 2e5f  nd(genre, self._
+00000da0: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
+00000db0: 5f2c 2061 7267 7329 0d0a 2020 2020 2020  _, args)..      
+00000dc0: 2020 636f 6d6d 616e 6420 3d20 5b0d 0a20    command = [.. 
+00000dd0: 2020 2020 2020 2020 2020 2050 726f 746f             Proto
+00000de0: 636f 6c43 6f64 652e 4845 4144 4552 2e76  colCode.HEADER.v
+00000df0: 616c 7565 2c0d 0a20 2020 2020 2020 2020  alue,..         
+00000e00: 2020 2050 726f 746f 636f 6c43 6f64 652e     ProtocolCode.
+00000e10: 4845 4144 4552 2e76 616c 7565 2c0d 0a20  HEADER.value,.. 
+00000e20: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00000e30: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00000e40: 6765 6e72 652c 206c 6973 7429 3a0d 0a20  genre, list):.. 
+00000e50: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+00000e60: 6174 6120 696e 2067 656e 7265 3a0d 0a20  ata in genre:.. 
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000e80: 6f6d 6d61 6e64 2e61 7070 656e 6428 6461  ommand.append(da
+00000e90: 7461 290d 0a20 2020 2020 2020 2065 6c73  ta)..        els
+00000ea0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000eb0: 636f 6d6d 616e 642e 6170 7065 6e64 2867  command.append(g
+00000ec0: 656e 7265 290d 0a20 2020 2020 2020 2063  enre)..        c
+00000ed0: 6f6d 6d61 6e64 2e61 7070 656e 6428 7265  ommand.append(re
+00000ee0: 616c 5f63 6f6d 6d61 6e64 290d 0a20 2020  al_command)..   
+00000ef0: 2020 2020 2063 6f6d 6d61 6e64 203d 2073       command = s
+00000f00: 656c 662e 5f66 6c61 7474 656e 2863 6f6d  elf._flatten(com
+00000f10: 6d61 6e64 290d 0a20 2020 2020 2020 2069  mand)..        i
+00000f20: 6620 6765 6e72 6520 3d3d 2050 726f 746f  f genre == Proto
+00000f30: 636f 6c43 6f64 652e 5345 545f 4c45 442e  colCode.SET_LED.
+00000f40: 7661 6c75 653a 0d0a 2020 2020 2020 2020  value:..        
+00000f50: 2020 2020 636f 6d6d 616e 642e 6170 7065      command.appe
+00000f60: 6e64 2873 756d 2863 6f6d 6d61 6e64 5b32  nd(sum(command[2
+00000f70: 3a5d 2920 2620 3078 6666 290d 0a20 2020  :]) & 0xff)..   
+00000f80: 2020 2020 2065 6c69 6620 6765 6e72 6520       elif genre 
+00000f90: 3d3d 2050 726f 746f 636f 6c43 6f64 652e  == ProtocolCode.
+00000fa0: 4745 545f 4649 524d 5741 5245 5f56 4552  GET_FIRMWARE_VER
+00000fb0: 5349 4f4e 2e76 616c 7565 3a0d 0a20 2020  SION.value:..   
+00000fc0: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
+00000fd0: 2e61 7070 656e 6428 3429 0d0a 2020 2020  .append(4)..    
+00000fe0: 2020 2020 656c 6966 2067 656e 7265 203d      elif genre =
+00000ff0: 3d20 5072 6f74 6f63 6f6c 436f 6465 2e47  = ProtocolCode.G
+00001000: 4554 5f4d 4f54 4f52 535f 4355 5252 454e  ET_MOTORS_CURREN
+00001010: 542e 7661 6c75 653a 0d0a 2020 2020 2020  T.value:..      
+00001020: 2020 2020 2020 636f 6d6d 616e 642e 6170        command.ap
+00001030: 7065 6e64 2835 290d 0a20 2020 2020 2020  pend(5)..       
+00001040: 2065 6c69 6620 6765 6e72 6520 3d3d 2050   elif genre == P
+00001050: 726f 746f 636f 6c43 6f64 652e 4745 545f  rotocolCode.GET_
+00001060: 4241 5454 4552 595f 494e 464f 2e76 616c  BATTERY_INFO.val
+00001070: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+00001080: 2063 6f6d 6d61 6e64 2e61 7070 656e 6428   command.append(
+00001090: 3629 0d0a 2020 2020 2020 2020 656c 7365  6)..        else
+000010a0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+000010b0: 2064 656c 2063 6f6d 6d61 6e64 5b32 5d0d   del command[2].
+000010c0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000010d0: 6d61 6e64 2e61 7070 656e 6428 7375 6d28  mand.append(sum(
+000010e0: 636f 6d6d 616e 645b 323a 5d29 2026 2030  command[2:]) & 0
+000010f0: 7866 6629 0d0a 2020 2020 2020 2020 7365  xff)..        se
+00001100: 6c66 2e5f 7772 6974 6528 636f 6d6d 616e  lf._write(comman
+00001110: 6429 0d0a 2020 2020 2020 2020 6966 2068  d)..        if h
+00001120: 6173 5f72 6570 6c79 3a0d 0a20 2020 2020  as_reply:..     
+00001130: 2020 2020 2020 2064 6174 6120 3d20 7365         data = se
+00001140: 6c66 2e5f 7265 6164 2863 6f6d 6d61 6e64  lf._read(command
+00001150: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00001160: 6620 6461 7461 3a0d 0a20 2020 2020 2020  f data:..       
+00001170: 2020 2020 2020 2020 2069 6620 6765 6e72           if genr
+00001180: 6520 696e 205b 5072 6f74 6f63 6f6c 436f  e in [ProtocolCo
+00001190: 6465 2e47 4554 5f46 4952 4d57 4152 455f  de.GET_FIRMWARE_
+000011a0: 5645 5253 494f 4e2e 7661 6c75 655d 3a0d  VERSION.value]:.
+000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000011d0: 2e5f 696e 7432 636f 6f72 6428 6461 7461  ._int2coord(data
+000011e0: 5b34 5d29 0d0a 2020 2020 2020 2020 2020  [4])..          
+000011f0: 2020 2020 2020 656c 6966 2067 656e 7265        elif genre
+00001200: 203d 3d20 5072 6f74 6f63 6f6c 436f 6465   == ProtocolCode
+00001210: 2e47 4554 5f4d 4f54 4f52 535f 4355 5252  .GET_MOTORS_CURR
+00001220: 454e 542e 7661 6c75 653a 0d0a 2020 2020  ENT.value:..    
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 7265 7475 726e 2073 656c 662e 5f64 6563  return self._dec
+00001250: 6f64 655f 696e 7431 3628 6461 7461 5b34  ode_int16(data[4
+00001260: 3a36 5d29 0d0a 2020 2020 2020 2020 2020  :6])..          
+00001270: 2020 2020 2020 656c 6966 2067 656e 7265        elif genre
+00001280: 203d 3d20 5072 6f74 6f63 6f6c 436f 6465   == ProtocolCode
+00001290: 2e47 4554 5f42 4154 5445 5259 5f49 4e46  .GET_BATTERY_INF
+000012a0: 4f2e 7661 6c75 653a 0d0a 2020 2020 2020  O.value:..      
+000012b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000012c0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+000012d0: 2020 2020 2020 2020 2020 2020 6279 7465              byte
+000012e0: 5f31 203d 2062 696e 2864 6174 615b 345d  _1 = bin(data[4]
+000012f0: 295b 323a 5d0d 0a20 2020 2020 2020 2020  )[2:]..         
+00001300: 2020 2020 2020 2020 2020 2072 6573 203d             res =
+00001310: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00001320: 2020 2020 2020 2020 7768 696c 6520 6c65          while le
+00001330: 6e28 6279 7465 5f31 2920 213d 2036 3a0d  n(byte_1) != 6:.
+00001340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001350: 2020 2020 2020 2020 2062 7974 655f 3120           byte_1 
+00001360: 3d20 2230 222b 6279 7465 5f31 0d0a 2020  = "0"+byte_1..  
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2020 7265 732e 6170 7065 6e64 2862 7974    res.append(byt
+00001390: 655f 3129 0d0a 2020 2020 2020 2020 2020  e_1)..          
+000013a0: 2020 2020 2020 2020 2020 7265 732e 6170            res.ap
+000013b0: 7065 6e64 2873 656c 662e 5f69 6e74 3263  pend(self._int2c
+000013c0: 6f6f 7264 2864 6174 615b 355d 2929 0d0a  oord(data[5]))..
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 7265 732e 6170 7065 6e64 2873      res.append(s
+000013f0: 656c 662e 5f69 6e74 3263 6f6f 7264 2864  elf._int2coord(d
+00001400: 6174 615b 365d 2929 0d0a 2020 2020 2020  ata[6]))..      
+00001410: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001420: 2062 7974 655f 315b 305d 203d 3d20 2230   byte_1[0] == "0
+00001430: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00001440: 2020 2020 2020 2020 2020 2020 7265 735b              res[
+00001450: 2d31 5d20 3d20 300d 0a20 2020 2020 2020  -1] = 0..       
+00001460: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00001470: 6620 6279 7465 5f31 5b31 5d20 3d3d 2022  f byte_1[1] == "
+00001480: 3022 3a0d 0a20 2020 2020 2020 2020 2020  0":..           
+00001490: 2020 2020 2020 2020 2020 2020 2072 6573               res
+000014a0: 5b31 5d20 3d20 300d 0a20 2020 2020 2020  [1] = 0..       
+000014b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000014c0: 7572 6e20 7265 730d 0a20 2020 2020 2020  urn res..       
+000014d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000014e0: 6461 7461 5b34 5d0d 0a20 2020 2020 2020  data[4]..       
+000014f0: 2020 2020 2023 2070 7269 6e74 2872 6573       # print(res
+00001500: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00001510: 6e20 4e6f 6e65 0d0a 2020 2020 0d0a 2020  n None..    ..  
+00001520: 2020 6465 6620 7365 745f 6c65 6428 7365    def set_led(se
+00001530: 6c66 2c20 6d6f 6465 2c20 522c 2047 2c20  lf, mode, R, G, 
+00001540: 4229 3a0d 0a20 2020 2020 2020 2022 2222  B):..        """
+00001550: 5365 7420 7570 204c 4544 206c 6967 6874  Set up LED light
+00001560: 730d 0a0d 0a20 2020 2020 2020 2041 7267  s....        Arg
+00001570: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001580: 6d6f 6465 2028 696e 7429 3a20 3120 2d20  mode (int): 1 - 
+00001590: 5365 7420 4c45 4420 6c69 6768 7420 636f  Set LED light co
+000015a0: 6c6f 722e 2032 202d 2053 6574 2074 6865  lor. 2 - Set the
+000015b0: 204c 4544 206c 6967 6874 2074 6f20 626c   LED light to bl
+000015c0: 696e 6b0d 0a20 2020 2020 2020 2020 2020  ink..           
+000015d0: 2052 2028 696e 7429 3a20 3020 7e20 3235   R (int): 0 ~ 25
+000015e0: 350d 0a20 2020 2020 2020 2020 2020 2047  5..            G
+000015f0: 2028 696e 7429 3a20 3020 7e20 3235 350d   (int): 0 ~ 255.
+00001600: 0a20 2020 2020 2020 2020 2020 2042 2028  .            B (
+00001610: 696e 7429 3a20 3020 7e20 3235 350d 0a20  int): 0 ~ 255.. 
+00001620: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00001630: 2020 2020 6361 6c69 6272 6174 696f 6e5f      calibration_
+00001640: 7061 7261 6d65 7465 7273 2863 6c61 7373  parameters(class
+00001650: 5f6e 616d 6520 3d20 7365 6c66 2e5f 5f63  _name = self.__c
+00001660: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f2c  lass__.__name__,
+00001670: 2072 6762 3d5b 522c 472c 425d 2c20 6c65   rgb=[R,G,B], le
+00001680: 645f 6d6f 6465 3d6d 6f64 6529 0d0a 2020  d_mode=mode)..  
+00001690: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000016a0: 662e 5f6d 6573 6728 5072 6f74 6f63 6f6c  f._mesg(Protocol
+000016b0: 436f 6465 2e53 4554 5f4c 4544 2e76 616c  Code.SET_LED.val
+000016c0: 7565 2c20 6d6f 6465 2c20 522c 2047 2c20  ue, mode, R, G, 
+000016d0: 4229 0d0a 2020 2020 0d0a 2020 2020 6465  B)..    ..    de
+000016e0: 6620 6765 745f 6669 726d 7761 7265 5f76  f get_firmware_v
+000016f0: 6572 7369 6f6e 2873 656c 6629 3a0d 0a20  ersion(self):.. 
+00001700: 2020 2020 2020 2022 2222 4765 7420 6669         """Get fi
+00001710: 726d 7761 7265 2076 6572 7369 6f6e 206e  rmware version n
+00001720: 756d 6265 720d 0a20 2020 2020 2020 2022  umber..        "
+00001730: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+00001740: 726e 2073 656c 662e 5f6d 6573 6728 5072  rn self._mesg(Pr
+00001750: 6f74 6f63 6f6c 436f 6465 2e47 4554 5f46  otocolCode.GET_F
+00001760: 4952 4d57 4152 455f 5645 5253 494f 4e2e  IRMWARE_VERSION.
+00001770: 7661 6c75 652c 2068 6173 5f72 6570 6c79  value, has_reply
+00001780: 203d 2054 7275 6529 0d0a 2020 2020 0d0a   = True)..    ..
+00001790: 2020 2020 6465 6620 6765 745f 6d6f 746f      def get_moto
+000017a0: 7273 5f63 7572 7265 6e74 2873 656c 6629  rs_current(self)
+000017b0: 3a0d 0a20 2020 2020 2020 2022 2222 4765  :..        """Ge
+000017c0: 7420 7468 6520 746f 7461 6c20 6375 7272  t the total curr
+000017d0: 656e 7420 6f66 2074 6865 206d 6f74 6f72  ent of the motor
+000017e0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000017f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001800: 6c66 2e5f 6d65 7367 2850 726f 746f 636f  lf._mesg(Protoco
+00001810: 6c43 6f64 652e 4745 545f 4d4f 544f 5253  lCode.GET_MOTORS
+00001820: 5f43 5552 5245 4e54 2e76 616c 7565 2c20  _CURRENT.value, 
+00001830: 6861 735f 7265 706c 7920 3d20 5472 7565  has_reply = True
+00001840: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
+00001850: 2067 6574 5f62 6174 7465 7279 5f69 6e66   get_battery_inf
+00001860: 6f28 7365 6c66 293a 0d0a 2020 2020 2020  o(self):..      
+00001870: 2020 2222 2252 6561 6420 6261 7474 6572    """Read batter
+00001880: 7920 696e 666f 726d 6174 696f 6e0d 0a20  y information.. 
+00001890: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000018a0: 2052 6574 7572 6e3a 0d0a 2020 2020 2020   Return:..      
+000018b0: 2020 2020 2020 6c69 7374 203a 205b 6261        list : [ba
+000018c0: 7474 6572 795f 6461 7461 2c20 6261 7474  ttery_data, batt
+000018d0: 6572 795f 315f 766f 6c74 6167 652c 2062  ery_1_voltage, b
+000018e0: 6174 7465 7279 5f32 5f76 6f6c 7461 6765  attery_2_voltage
+000018f0: 5d2e 0d0a 2020 2020 2020 2020 2020 2020  ]...            
+00001900: 2020 2020 6261 7474 6572 795f 6461 7461      battery_data
+00001910: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001920: 2020 2020 2020 2041 2073 7472 696e 6720         A string 
+00001930: 6f66 206c 656e 6774 6820 362c 2072 6570  of length 6, rep
+00001940: 7265 7365 6e74 6564 2066 726f 6d20 6c65  resented from le
+00001950: 6674 2074 6f20 7269 6768 743a 200d 0a20  ft to right: .. 
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2062 6974 352c 2062 6974 342c 2062     bit5, bit4, b
+00001980: 6974 332c 2062 6974 322c 2062 6974 312c  it3, bit2, bit1,
+00001990: 2062 6974 302e 0d0a 0d0a 2020 2020 2020   bit0.....      
+000019a0: 2020 2020 2020 2020 2020 2020 2020 6269                bi
+000019b0: 7435 203a 2042 6174 7465 7279 2032 2069  t5 : Battery 2 i
+000019c0: 7320 696e 7365 7274 6564 2069 6e74 6f20  s inserted into 
+000019d0: 7468 6520 696e 7465 7266 6163 6520 3120  the interface 1 
+000019e0: 6d65 616e 7320 696e 7365 7274 6564 2c20  means inserted, 
+000019f0: 3020 6973 206e 6f74 2069 6e73 6572 7465  0 is not inserte
+00001a00: 642e 0d0a 2020 2020 2020 2020 2020 2020  d...            
+00001a10: 2020 2020 2020 2020 6269 7434 203a 2042          bit4 : B
+00001a20: 6174 7465 7279 2031 2069 7320 696e 7365  attery 1 is inse
+00001a30: 7274 6564 2069 6e74 6f20 7468 6520 696e  rted into the in
+00001a40: 7465 7266 6163 652c 2031 206d 6561 6e73  terface, 1 means
+00001a50: 2069 6e73 6572 7465 642c 2030 2069 7320   inserted, 0 is 
+00001a60: 6e6f 7420 696e 7365 7274 6564 2e0d 0a20  not inserted... 
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2062 6974 3320 3a20 5468 6520 6164     bit3 : The ad
+00001a90: 6170 7465 7220 6973 2070 6c75 6767 6564  apter is plugged
+00001aa0: 2069 6e74 6f20 7468 6520 696e 7465 7266   into the interf
+00001ab0: 6163 6520 3120 6d65 616e 7320 706c 7567  ace 1 means plug
+00001ac0: 6765 6420 696e 2c20 3020 6e6f 7420 706c  ged in, 0 not pl
+00001ad0: 7567 6765 6420 696e 2e0d 0a20 2020 2020  ugged in...     
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00001af0: 6974 3220 3a20 5468 6520 6368 6172 6769  it2 : The chargi
+00001b00: 6e67 2070 696c 6520 6973 2069 6e73 6572  ng pile is inser
+00001b10: 7465 6420 696e 746f 2074 6865 2069 6e74  ted into the int
+00001b20: 6572 6661 6365 2c20 3120 6d65 616e 7320  erface, 1 means 
+00001b30: 706c 7567 6765 6420 696e 2c20 3020 6973  plugged in, 0 is
+00001b40: 206e 6f74 2070 6c75 6767 6564 2069 6e2e   not plugged in.
+00001b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001b60: 2020 2020 2020 6269 7431 203a 2042 6174        bit1 : Bat
+00001b70: 7465 7279 2032 2063 6861 7267 696e 6720  tery 2 charging 
+00001b80: 6c69 6768 7420 3020 6d65 616e 7320 6f66  light 0 means of
+00001b90: 662c 2031 206d 6561 6e73 206f 6e2e 0d0a  f, 1 means on...
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 6269 7430 203a 2042 6174 7465      bit0 : Batte
+00001bc0: 7279 2031 2063 6861 7267 696e 6720 6c69  ry 1 charging li
+00001bd0: 6768 742c 2030 206d 6561 6e73 206f 6666  ght, 0 means off
+00001be0: 2c20 3120 6d65 616e 7320 6f6e 2e0d 0a20  , 1 means on... 
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00001c00: 6174 7465 7279 5f31 5f76 6f6c 7461 6765  attery_1_voltage
+00001c10: 203a 2042 6174 7465 7279 2031 2076 6f6c   : Battery 1 vol
+00001c20: 7461 6765 2069 6e20 766f 6c74 732e 0d0a  tage in volts...
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 6261 7474 6572 795f 325f 766f 6c74 6167  battery_2_voltag
+00001c50: 6520 3a20 4261 7474 6572 7920 3220 766f  e : Battery 2 vo
+00001c60: 6c74 6167 6520 696e 2076 6f6c 7473 2e0d  ltage in volts..
+00001c70: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001c80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001c90: 662e 5f6d 6573 6728 5072 6f74 6f63 6f6c  f._mesg(Protocol
+00001ca0: 436f 6465 2e47 4554 5f42 4154 5445 5259  Code.GET_BATTERY
+00001cb0: 5f49 4e46 4f2e 7661 6c75 652c 2068 6173  _INFO.value, has
+00001cc0: 5f72 6570 6c79 203d 2054 7275 6529 0d0a  _reply = True)..
+00001cd0: 2020 2020 0d0a 2020 2020 2320 6465 6620      ..    # def 
+00001ce0: 6d6f 7665 5f63 6f6e 7472 6f6c 2873 656c  move_control(sel
+00001cf0: 662c 2064 6972 6563 7469 6f6e 5f31 2c20  f, direction_1, 
+00001d00: 6469 7265 6374 696f 6e5f 322c 2064 6972  direction_2, dir
+00001d10: 6563 7469 6f6e 5f33 293a 0d0a 2020 2020  ection_3):..    
+00001d20: 2320 2020 2020 2222 2243 6f6e 7472 6f6c  #     """Control
+00001d30: 2074 6865 2063 6172 2074 6f20 726f 7461   the car to rota
+00001d40: 7465 2066 6f72 7761 7264 2c20 6261 636b  te forward, back
+00001d50: 7761 7264 2c20 6c65 6674 2c20 7269 6768  ward, left, righ
+00001d60: 7420 616e 6420 666f 7277 6172 642f 636f  t and forward/co
+00001d70: 756e 7465 7263 6c6f 636b 7769 7365 0d0a  unterclockwise..
+00001d80: 0d0a 2020 2020 2320 2020 2020 4172 6773  ..    #     Args
+00001d90: 3a0d 0a20 2020 2023 2020 2020 2020 2020  :..    #        
+00001da0: 2064 6972 6563 7469 6f6e 5f31 2028 696e   direction_1 (in
+00001db0: 7429 3a20 436f 6e74 726f 6c20 666f 7277  t): Control forw
+00001dc0: 6172 6420 6f72 2062 6163 6b77 6172 643a  ard or backward:
+00001dd0: 2030 207e 2031 3237 2069 7320 6261 636b   0 ~ 127 is back
+00001de0: 7761 7264 2c20 3132 3920 7e20 3235 3520  ward, 129 ~ 255 
+00001df0: 6973 2066 6f72 7761 7264 2c20 3132 3820  is forward, 128 
+00001e00: 6973 2073 746f 702e 0d0a 2020 2020 2320  is stop...    # 
+00001e10: 2020 2020 2020 2020 6469 7265 6374 696f          directio
+00001e20: 6e5f 3220 2869 6e74 293a 2063 6f6e 7472  n_2 (int): contr
+00001e30: 6f6c 206c 6566 7420 616e 6420 7269 6768  ol left and righ
+00001e40: 7420 6d6f 7665 6d65 6e74 3a20 3020 7e20  t movement: 0 ~ 
+00001e50: 3132 3720 6973 2072 6967 6874 2c20 3132  127 is right, 12
+00001e60: 3920 7e20 3235 3520 6973 206c 6566 742c  9 ~ 255 is left,
+00001e70: 2031 3238 2069 7320 7374 6f70 2e0d 0a20   128 is stop... 
+00001e80: 2020 2023 2020 2020 2020 2020 2064 6972     #         dir
+00001e90: 6563 7469 6f6e 5f33 2028 696e 7429 3a20  ection_3 (int): 
+00001ea0: 636f 6e74 726f 6c20 726f 7461 7469 6f6e  control rotation
+00001eb0: 3a20 3020 7e20 3132 3720 6973 2063 6c6f  : 0 ~ 127 is clo
+00001ec0: 636b 7769 7365 2c20 3132 3920 7e20 3235  ckwise, 129 ~ 25
+00001ed0: 3520 6973 2063 6f75 6e74 6572 636c 6f63  5 is countercloc
+00001ee0: 6b77 6973 652c 2031 3238 2069 7320 7374  kwise, 128 is st
+00001ef0: 6f70 2e0d 0a20 2020 2023 2020 2020 2022  op...    #     "
+00001f00: 2222 0d0a 2020 2020 2320 2020 2020 6361  ""..    #     ca
+00001f10: 6c69 6272 6174 696f 6e5f 7061 7261 6d65  libration_parame
+00001f20: 7465 7273 2863 6c61 7373 5f6e 616d 6520  ters(class_name 
+00001f30: 3d20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  = self.__class__
+00001f40: 2e5f 5f6e 616d 655f 5f2c 2064 6972 6563  .__name__, direc
+00001f50: 7469 6f6e 5f31 3d64 6972 6563 7469 6f6e  tion_1=direction
+00001f60: 5f31 2c20 6469 7265 6374 696f 6e5f 323d  _1, direction_2=
+00001f70: 6469 7265 6374 696f 6e5f 322c 6469 7265  direction_2,dire
+00001f80: 6374 696f 6e5f 333d 6469 7265 6374 696f  ction_3=directio
+00001f90: 6e5f 3329 0d0a 2020 2020 2320 2020 2020  n_3)..    #     
+00001fa0: 7265 7475 726e 2073 656c 662e 5f6d 6573  return self._mes
+00001fb0: 6728 6469 7265 6374 696f 6e5f 312c 2064  g(direction_1, d
+00001fc0: 6972 6563 7469 6f6e 5f32 2c20 6469 7265  irection_2, dire
+00001fd0: 6374 696f 6e5f 3329 0d0a 2020 2020 0d0a  ction_3)..    ..
+00001fe0: 2020 2020 6465 6620 676f 5f61 6865 6164      def go_ahead
+00001ff0: 2873 656c 662c 2067 6f5f 7370 6565 642c  (self, go_speed,
+00002000: 2074 696d 656f 7574 3d35 293a 0d0a 2020   timeout=5):..  
+00002010: 2020 2020 2020 2222 2243 6f6e 7472 6f6c        """Control
+00002020: 2074 6865 2063 6172 2074 6f20 6d6f 7665   the car to move
+00002030: 2066 6f72 7761 7264 2e20 5365 6e64 2063   forward. Send c
+00002040: 6f6e 7472 6f6c 2063 6f6d 6d61 6e64 7320  ontrol commands 
+00002050: 6576 6572 7920 3130 306d 732e 2077 6974  every 100ms. wit
+00002060: 6820 6120 6465 6661 756c 7420 6d6f 7469  h a default moti
+00002070: 6f6e 2074 696d 6520 6f66 2035 2073 6563  on time of 5 sec
+00002080: 6f6e 6473 2e0d 0a0d 0a20 2020 2020 2020  onds.....       
+00002090: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+000020a0: 2020 2020 676f 5f73 7065 6564 2028 696e      go_speed (in
+000020b0: 7429 3a20 3120 7e20 3132 3720 6973 2066  t): 1 ~ 127 is f
+000020c0: 6f72 7761 7264 2e0d 0a20 2020 2020 2020  orward...       
+000020d0: 2020 2020 2074 696d 656f 7574 2028 696e       timeout (in
+000020e0: 7429 3a20 6465 6661 756c 7420 3520 732e  t): default 5 s.
+000020f0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00002100: 2020 2020 2020 2023 2067 6f5f 7370 6565         # go_spee
+00002110: 6420 2869 6e74 293a 2031 3239 207e 2032  d (int): 129 ~ 2
+00002120: 3535 2069 7320 666f 7277 6172 640d 0a20  55 is forward.. 
+00002130: 2020 2020 2020 2063 616c 6962 7261 7469         calibrati
+00002140: 6f6e 5f70 6172 616d 6574 6572 7328 636c  on_parameters(cl
+00002150: 6173 735f 6e61 6d65 203d 2073 656c 662e  ass_name = self.
+00002160: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
+00002170: 5f5f 2c20 6461 7461 3d67 6f5f 7370 6565  __, data=go_spee
+00002180: 6429 0d0a 2020 2020 2020 2020 7420 3d20  d)..        t = 
+00002190: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
+000021a0: 2020 2020 2077 6869 6c65 2074 696d 652e       while time.
+000021b0: 7469 6d65 2829 202d 2074 203c 2074 696d  time() - t < tim
+000021c0: 656f 7574 3a0d 0a20 2020 2020 2020 2020  eout:..         
+000021d0: 2020 2073 656c 662e 5f6d 6573 6728 3132     self._mesg(12
+000021e0: 382b 676f 5f73 7065 6564 2c20 3132 382c  8+go_speed, 128,
+000021f0: 2031 3238 290d 0a20 2020 2020 2020 2020   128)..         
+00002200: 2020 2074 696d 652e 736c 6565 7028 302e     time.sleep(0.
+00002210: 3129 0d0a 2020 2020 2020 2020 7365 6c66  1)..        self
+00002220: 2e73 746f 7028 290d 0a20 2020 2020 2020  .stop()..       
+00002230: 200d 0a20 2020 2064 6566 2072 6574 7265   ..    def retre
+00002240: 6174 2873 656c 662c 2062 6163 6b5f 7370  at(self, back_sp
+00002250: 6565 642c 2074 696d 656f 7574 3d35 293a  eed, timeout=5):
+00002260: 0d0a 2020 2020 2020 2020 2222 2243 6f6e  ..        """Con
+00002270: 7472 6f6c 2074 6865 2063 6172 2062 6163  trol the car bac
+00002280: 6b2e 2053 656e 6420 636f 6e74 726f 6c20  k. Send control 
+00002290: 636f 6d6d 616e 6473 2065 7665 7279 2031  commands every 1
+000022a0: 3030 6d73 2e20 7769 7468 2061 2064 6566  00ms. with a def
+000022b0: 6175 6c74 206d 6f74 696f 6e20 7469 6d65  ault motion time
+000022c0: 206f 6620 3520 7365 636f 6e64 730d 0a0d   of 5 seconds...
+000022d0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+000022e0: 2020 2020 2020 2020 2020 2020 6261 636b              back
+000022f0: 5f73 7065 6564 2028 696e 7429 3a20 3120  _speed (int): 1 
+00002300: 7e20 3132 3720 6973 2062 6163 6b77 6172  ~ 127 is backwar
+00002310: 640d 0a20 2020 2020 2020 2020 2020 2074  d..            t
+00002320: 696d 656f 7574 2028 696e 7429 3a20 6465  imeout (int): de
+00002330: 6661 756c 7420 3520 732e 0d0a 2020 2020  fault 5 s...    
+00002340: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002350: 2063 616c 6962 7261 7469 6f6e 5f70 6172   calibration_par
+00002360: 616d 6574 6572 7328 636c 6173 735f 6e61  ameters(class_na
+00002370: 6d65 203d 2073 656c 662e 5f5f 636c 6173  me = self.__clas
+00002380: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20 6461  s__.__name__, da
+00002390: 7461 3d62 6163 6b5f 7370 6565 6429 0d0a  ta=back_speed)..
+000023a0: 2020 2020 2020 2020 7420 3d20 7469 6d65          t = time
+000023b0: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
+000023c0: 2077 6869 6c65 2074 696d 652e 7469 6d65   while time.time
+000023d0: 2829 202d 2074 203c 2074 696d 656f 7574  () - t < timeout
+000023e0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000023f0: 656c 662e 5f6d 6573 6728 3132 382d 6261  elf._mesg(128-ba
+00002400: 636b 5f73 7065 6564 2c20 3132 382c 2031  ck_speed, 128, 1
+00002410: 3238 290d 0a20 2020 2020 2020 2020 2020  28)..           
+00002420: 2074 696d 652e 736c 6565 7028 302e 3129   time.sleep(0.1)
+00002430: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00002440: 746f 7028 290d 0a20 2020 2020 2020 200d  top()..        .
+00002450: 0a20 2020 2064 6566 2070 616e 5f6c 6566  .    def pan_lef
+00002460: 7428 7365 6c66 2c20 7061 6e5f 6c65 6674  t(self, pan_left
+00002470: 5f73 7065 6564 2c20 7469 6d65 6f75 743d  _speed, timeout=
+00002480: 3529 3a0d 0a20 2020 2020 2020 2022 2222  5):..        """
+00002490: 436f 6e74 726f 6c20 7468 6520 6361 7220  Control the car 
+000024a0: 746f 2070 616e 2074 6f20 7468 6520 6c65  to pan to the le
+000024b0: 6674 2e20 5365 6e64 2063 6f6e 7472 6f6c  ft. Send control
+000024c0: 2063 6f6d 6d61 6e64 7320 6576 6572 7920   commands every 
+000024d0: 3130 306d 732e 2077 6974 6820 6120 6465  100ms. with a de
+000024e0: 6661 756c 7420 6d6f 7469 6f6e 2074 696d  fault motion tim
+000024f0: 6520 6f66 2035 2073 6563 6f6e 6473 0d0a  e of 5 seconds..
+00002500: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
+00002510: 0a20 2020 2020 2020 2020 2020 2070 616e  .            pan
+00002520: 5f6c 6566 745f 7370 6565 6420 2869 6e74  _left_speed (int
+00002530: 293a 2031 207e 2031 3237 0d0a 2020 2020  ): 1 ~ 127..    
+00002540: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
+00002550: 2869 6e74 293a 2064 6566 6175 6c74 2035  (int): default 5
+00002560: 2073 2e0d 0a20 2020 2020 2020 2022 2222   s...        """
+00002570: 0d0a 2020 2020 2020 2020 2320 7061 6e5f  ..        # pan_
+00002580: 6c65 6674 5f73 7065 6564 2028 696e 7429  left_speed (int)
+00002590: 3a20 3132 3920 7e20 3235 350d 0a20 2020  : 129 ~ 255..   
+000025a0: 2020 2020 2063 616c 6962 7261 7469 6f6e       calibration
+000025b0: 5f70 6172 616d 6574 6572 7328 636c 6173  _parameters(clas
+000025c0: 735f 6e61 6d65 203d 2073 656c 662e 5f5f  s_name = self.__
+000025d0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+000025e0: 2c20 6461 7461 3d70 616e 5f6c 6566 745f  , data=pan_left_
+000025f0: 7370 6565 6429 0d0a 2020 2020 2020 2020  speed)..        
+00002600: 7420 3d20 7469 6d65 2e74 696d 6528 290d  t = time.time().
+00002610: 0a20 2020 2020 2020 2077 6869 6c65 2074  .        while t
+00002620: 696d 652e 7469 6d65 2829 202d 2074 203c  ime.time() - t <
+00002630: 2074 696d 656f 7574 3a0d 0a20 2020 2020   timeout:..     
+00002640: 2020 2020 2020 2073 656c 662e 5f6d 6573         self._mes
+00002650: 6728 3132 382c 2031 3238 2b70 616e 5f6c  g(128, 128+pan_l
+00002660: 6566 745f 7370 6565 642c 2031 3238 290d  eft_speed, 128).
+00002670: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00002680: 652e 736c 6565 7028 302e 3129 0d0a 2020  e.sleep(0.1)..  
+00002690: 2020 2020 2020 7365 6c66 2e73 746f 7028        self.stop(
+000026a0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+000026b0: 2064 6566 2070 616e 5f72 6967 6874 2873   def pan_right(s
+000026c0: 656c 662c 2070 616e 5f72 6967 6874 5f73  elf, pan_right_s
+000026d0: 7065 6564 2c20 7469 6d65 6f75 743d 3529  peed, timeout=5)
+000026e0: 3a0d 0a20 2020 2020 2020 2022 2222 436f  :..        """Co
+000026f0: 6e74 726f 6c20 7468 6520 6361 7220 746f  ntrol the car to
+00002700: 2070 616e 2074 6f20 7468 6520 7269 6768   pan to the righ
+00002710: 742e 2053 656e 6420 636f 6e74 726f 6c20  t. Send control 
+00002720: 636f 6d6d 616e 6473 2065 7665 7279 2031  commands every 1
+00002730: 3030 6d73 2e20 7769 7468 2061 2064 6566  00ms. with a def
+00002740: 6175 6c74 206d 6f74 696f 6e20 7469 6d65  ault motion time
+00002750: 206f 6620 3520 7365 636f 6e64 730d 0a0d   of 5 seconds...
+00002760: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00002770: 2020 2020 2020 2020 2020 2020 7061 6e5f              pan_
+00002780: 7269 6768 745f 7370 6565 6420 2869 6e74  right_speed (int
+00002790: 293a 2031 207e 2031 3237 0d0a 2020 2020  ): 1 ~ 127..    
+000027a0: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
+000027b0: 2869 6e74 293a 2064 6566 6175 6c74 2035  (int): default 5
+000027c0: 2073 2e0d 0a20 2020 2020 2020 2022 2222   s...        """
+000027d0: 0d0a 2020 2020 2020 2020 6361 6c69 6272  ..        calibr
+000027e0: 6174 696f 6e5f 7061 7261 6d65 7465 7273  ation_parameters
+000027f0: 2863 6c61 7373 5f6e 616d 6520 3d20 7365  (class_name = se
+00002800: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+00002810: 616d 655f 5f2c 2070 616e 5f72 6967 6874  ame__, pan_right
+00002820: 5f73 7065 6564 3d70 616e 5f72 6967 6874  _speed=pan_right
+00002830: 5f73 7065 6564 290d 0a20 2020 2020 2020  _speed)..       
+00002840: 2074 203d 2074 696d 652e 7469 6d65 2829   t = time.time()
+00002850: 0d0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
+00002860: 7469 6d65 2e74 696d 6528 2920 2d20 7420  time.time() - t 
+00002870: 3c20 7469 6d65 6f75 743a 0d0a 2020 2020  < timeout:..    
+00002880: 2020 2020 2020 2020 7365 6c66 2e5f 6d65          self._me
+00002890: 7367 2831 3238 2c20 3132 382d 7061 6e5f  sg(128, 128-pan_
+000028a0: 7269 6768 745f 7370 6565 642c 2031 3238  right_speed, 128
+000028b0: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+000028c0: 696d 652e 736c 6565 7028 302e 3129 0d0a  ime.sleep(0.1)..
+000028d0: 2020 2020 2020 2020 7365 6c66 2e73 746f          self.sto
+000028e0: 7028 290d 0a20 2020 2020 2020 200d 0a20  p()..        .. 
+000028f0: 2020 2064 6566 2063 6c6f 636b 7769 7365     def clockwise
+00002900: 5f72 6f74 6174 696f 6e28 7365 6c66 2c20  _rotation(self, 
+00002910: 726f 7461 7465 5f72 6967 6874 5f73 7065  rotate_right_spe
+00002920: 6564 2c20 7469 6d65 6f75 743d 3529 3a0d  ed, timeout=5):.
+00002930: 0a20 2020 2020 2020 2022 2222 436f 6e74  .        """Cont
+00002940: 726f 6c20 7468 6520 6361 7220 746f 2072  rol the car to r
+00002950: 6f74 6174 6520 636c 6f63 6b77 6973 652e  otate clockwise.
+00002960: 2053 656e 6420 636f 6e74 726f 6c20 636f   Send control co
+00002970: 6d6d 616e 6473 2065 7665 7279 2031 3030  mmands every 100
+00002980: 6d73 2e20 7769 7468 2061 2064 6566 6175  ms. with a defau
+00002990: 6c74 206d 6f74 696f 6e20 7469 6d65 206f  lt motion time o
+000029a0: 6620 3520 7365 636f 6e64 730d 0a0d 0a20  f 5 seconds.... 
+000029b0: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+000029c0: 2020 2020 2020 2020 2020 636c 6f63 6b77            clockw
+000029d0: 6973 655f 726f 7461 7469 6f6e 5f73 7065  ise_rotation_spe
+000029e0: 6564 2028 696e 7429 3a20 3120 7e20 3132  ed (int): 1 ~ 12
+000029f0: 370d 0a20 2020 2020 2020 2020 2020 2074  7..            t
+00002a00: 696d 656f 7574 2028 696e 7429 3a20 6465  imeout (int): de
+00002a10: 6661 756c 7420 3520 732e 0d0a 2020 2020  fault 5 s...    
+00002a20: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002a30: 2063 616c 6962 7261 7469 6f6e 5f70 6172   calibration_par
+00002a40: 616d 6574 6572 7328 636c 6173 735f 6e61  ameters(class_na
+00002a50: 6d65 203d 2073 656c 662e 5f5f 636c 6173  me = self.__clas
+00002a60: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20 726f  s__.__name__, ro
+00002a70: 7461 7465 5f72 6967 6874 5f73 7065 6564  tate_right_speed
+00002a80: 3d72 6f74 6174 655f 7269 6768 745f 7370  =rotate_right_sp
+00002a90: 6565 6429 0d0a 2020 2020 2020 2020 7420  eed)..        t 
+00002aa0: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
+00002ab0: 2020 2020 2020 2077 6869 6c65 2074 696d         while tim
+00002ac0: 652e 7469 6d65 2829 202d 2074 203c 2074  e.time() - t < t
+00002ad0: 696d 656f 7574 3a0d 0a20 2020 2020 2020  imeout:..       
+00002ae0: 2020 2020 2073 656c 662e 5f6d 6573 6728       self._mesg(
+00002af0: 3132 382c 2031 3238 2c20 3132 382d 726f  128, 128, 128-ro
+00002b00: 7461 7465 5f72 6967 6874 5f73 7065 6564  tate_right_speed
+00002b10: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00002b20: 696d 652e 736c 6565 7028 302e 3129 0d0a  ime.sleep(0.1)..
+00002b30: 2020 2020 2020 2020 7365 6c66 2e73 746f          self.sto
+00002b40: 7028 290d 0a20 2020 2020 2020 200d 0a20  p()..        .. 
+00002b50: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00002b60: 2063 6f75 6e74 6572 636c 6f63 6b77 6973   counterclockwis
+00002b70: 655f 726f 7461 7469 6f6e 2873 656c 662c  e_rotation(self,
+00002b80: 2072 6f74 6174 655f 6c65 6674 5f73 7065   rotate_left_spe
+00002b90: 6564 2c20 7469 6d65 6f75 743d 3529 3a0d  ed, timeout=5):.
+00002ba0: 0a20 2020 2020 2020 2022 2222 436f 6e74  .        """Cont
+00002bb0: 726f 6c20 7468 6520 6361 7220 746f 2072  rol the car to r
+00002bc0: 6f74 6174 6520 636f 756e 7465 7263 6c6f  otate counterclo
+00002bd0: 636b 7769 7365 2e20 5365 6e64 2063 6f6e  ckwise. Send con
+00002be0: 7472 6f6c 2063 6f6d 6d61 6e64 7320 6576  trol commands ev
+00002bf0: 6572 7920 3130 306d 732e 2077 6974 6820  ery 100ms. with 
+00002c00: 6120 6465 6661 756c 7420 6d6f 7469 6f6e  a default motion
+00002c10: 2074 696d 6520 6f66 2035 2073 6563 6f6e   time of 5 secon
+00002c20: 6473 0d0a 0d0a 2020 2020 2020 2020 4172  ds....        Ar
+00002c30: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+00002c40: 2063 6c6f 636b 7769 7365 5f72 6f74 6174   clockwise_rotat
+00002c50: 696f 6e5f 7370 6565 6420 2869 6e74 293a  ion_speed (int):
+00002c60: 2031 207e 2031 3237 0d0a 2020 2020 2020   1 ~ 127..      
+00002c70: 2020 2020 2020 7469 6d65 6f75 7420 2869        timeout (i
+00002c80: 6e74 293a 2064 6566 6175 6c74 2035 2073  nt): default 5 s
+00002c90: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00002ca0: 2020 2020 2020 2020 6361 6c69 6272 6174          calibrat
+00002cb0: 696f 6e5f 7061 7261 6d65 7465 7273 2863  ion_parameters(c
+00002cc0: 6c61 7373 5f6e 616d 6520 3d20 7365 6c66  lass_name = self
+00002cd0: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+00002ce0: 655f 5f2c 2072 6f74 6174 655f 6c65 6674  e__, rotate_left
+00002cf0: 5f73 7065 6564 3d72 6f74 6174 655f 6c65  _speed=rotate_le
+00002d00: 6674 5f73 7065 6564 290d 0a20 2020 2020  ft_speed)..     
+00002d10: 2020 2074 203d 2074 696d 652e 7469 6d65     t = time.time
+00002d20: 2829 0d0a 2020 2020 2020 2020 7768 696c  ()..        whil
+00002d30: 6520 7469 6d65 2e74 696d 6528 2920 2d20  e time.time() - 
+00002d40: 7420 3c20 7469 6d65 6f75 743a 0d0a 2020  t < timeout:..  
+00002d50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00002d60: 6d65 7367 2831 3238 2c20 3132 382c 2031  mesg(128, 128, 1
+00002d70: 3238 2b72 6f74 6174 655f 6c65 6674 5f73  28+rotate_left_s
+00002d80: 7065 6564 290d 0a20 2020 2020 2020 2020  peed)..         
+00002d90: 2020 2074 696d 652e 736c 6565 7028 302e     time.sleep(0.
+00002da0: 3129 0d0a 2020 2020 2020 2020 7365 6c66  1)..        self
+00002db0: 2e73 746f 7028 290d 0a20 2020 2020 2020  .stop()..       
+00002dc0: 200d 0a20 2020 2064 6566 2073 746f 7028   ..    def stop(
+00002dd0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00002de0: 2222 2273 746f 7020 6d6f 7469 6f6e 0d0a  """stop motion..
+00002df0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00002e00: 2020 2020 2073 656c 662e 5f6d 6573 6728       self._mesg(
+00002e10: 3132 382c 2031 3238 2c20 3132 3829 0d0a  128, 128, 128)..
+00002e20: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00002e30: 6620 6765 745f 6d63 755f 696e 666f 2873  f get_mcu_info(s
+00002e40: 656c 662c 2076 6572 7369 6f6e 3d31 2e30  elf, version=1.0
+00002e50: 293a 0d0a 2020 2020 2020 2020 2222 2222  ):..        """"
+00002e60: 2222 0d0a 2020 2020 2020 2020 6966 2076  ""..        if v
+00002e70: 6572 7369 6f6e 203d 3d20 312e 303a 0d0a  ersion == 1.0:..
+00002e80: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00002e90: 5f6c 656e 203d 2032 390d 0a20 2020 2020  _len = 29..     
+00002ea0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00002eb0: 2020 2020 2020 6461 7461 5f6c 656e 203d        data_len =
+00002ec0: 2034 310d 0a20 2020 2020 2020 2064 6174   41..        dat
+00002ed0: 6173 203d 2073 656c 662e 5f72 6561 6428  as = self._read(
+00002ee0: 5b30 7866 652c 2030 7866 652c 2064 6174  [0xfe, 0xfe, dat
+00002ef0: 615f 6c65 6e5d 290d 0a20 2020 2020 2020  a_len])..       
+00002f00: 2072 6573 203d 205b 5d0d 0a20 2020 2020   res = []..     
+00002f10: 2020 2069 6e64 6578 203d 2032 0d0a 2020     index = 2..  
+00002f20: 2020 2020 2020 7768 696c 6520 696e 6465        while inde
+00002f30: 7820 3c20 6c65 6e28 6461 7461 7329 202d  x < len(datas) -
+00002f40: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00002f50: 2069 6620 696e 6465 7820 3c20 353a 0d0a   if index < 5:..
+00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f70: 7265 732e 6170 7065 6e64 2864 6174 6173  res.append(datas
+00002f80: 5b69 6e64 6578 5d29 0d0a 2020 2020 2020  [index])..      
+00002f90: 2020 2020 2020 2020 2020 696e 6465 782b            index+
+00002fa0: 3d31 0d0a 2020 2020 2020 2020 2020 2020  =1..            
+00002fb0: 656c 6966 2069 6e64 6578 203c 2031 3720  elif index < 17 
+00002fc0: 6f72 2028 696e 6465 7820 3e3d 2032 3020  or (index >= 20 
+00002fd0: 616e 6420 696e 6465 7820 3c20 3238 293a  and index < 28):
+00002fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ff0: 2020 7265 732e 6170 7065 6e64 2873 656c    res.append(sel
+00003000: 662e 5f64 6563 6f64 655f 696e 7431 3628  f._decode_int16(
+00003010: 6461 7461 735b 696e 6465 783a 696e 6465  datas[index:inde
+00003020: 782b 325d 2929 0d0a 2020 2020 2020 2020  x+2]))..        
+00003030: 2020 2020 2020 2020 696e 6465 782b 3d32          index+=2
+00003040: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00003050: 6966 2069 6e64 6578 203e 3d20 3238 2061  if index >= 28 a
+00003060: 6e64 2069 6e64 6578 203c 3d20 3332 3a0d  nd index <= 32:.
+00003070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003080: 2072 6573 2e61 7070 656e 6428 7365 6c66   res.append(self
+00003090: 2e5f 696e 7432 616e 676c 6528 7365 6c66  ._int2angle(self
+000030a0: 2e5f 6465 636f 6465 5f69 6e74 3136 2864  ._decode_int16(d
+000030b0: 6174 6173 5b69 6e64 6578 3a69 6e64 6578  atas[index:index
+000030c0: 2b32 5d29 2929 0d0a 2020 2020 2020 2020  +2])))..        
+000030d0: 2020 2020 2020 2020 696e 6465 782b 3d32          index+=2
+000030e0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000030f0: 6966 2069 6e64 6578 203d 3d20 3137 3a0d  if index == 17:.
+00003100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003110: 2062 7974 655f 3120 3d20 6269 6e28 6461   byte_1 = bin(da
+00003120: 7461 735b 696e 6465 785d 295b 323a 5d0d  tas[index])[2:].
+00003130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003140: 2077 6869 6c65 206c 656e 2862 7974 655f   while len(byte_
+00003150: 3129 2021 3d20 363a 0d0a 2020 2020 2020  1) != 6:..      
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 6279 7465 5f31 203d 2022 3022 2b62    byte_1 = "0"+b
+00003180: 7974 655f 310d 0a20 2020 2020 2020 2020  yte_1..         
+00003190: 2020 2020 2020 2072 6573 2e61 7070 656e         res.appen
+000031a0: 6428 6279 7465 5f31 290d 0a20 2020 2020  d(byte_1)..     
+000031b0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+000031c0: 2b3d 310d 0a20 2020 2020 2020 2020 2020  +=1..           
+000031d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000031e0: 2020 2065 6c69 6620 696e 6465 7820 3c20     elif index < 
+000031f0: 3230 206f 7220 2869 6e64 6578 203e 2033  20 or (index > 3
+00003200: 3220 616e 6420 696e 6465 7820 3c20 3431  2 and index < 41
+00003210: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00003220: 2020 2020 7265 732e 6170 7065 6e64 2873      res.append(s
+00003230: 656c 662e 5f69 6e74 3263 6f6f 7264 2864  elf._int2coord(d
+00003240: 6174 6173 5b69 6e64 6578 5d29 290d 0a20  atas[index])).. 
+00003250: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003260: 6e64 6578 2b3d 310d 0a20 2020 2020 2020  ndex+=1..       
+00003270: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003280: 2020 2072 6574 7572 6e20 7265 730d 0a20     return res.. 
+00003290: 2020 200d 0a20 2020 2064 6566 2072 6573     ..    def res
+000032a0: 746f 7265 2873 656c 6629 3a0d 0a20 2020  tore(self):..   
+000032b0: 2020 2020 2022 2222 4d6f 746f 7220 7374       """Motor st
+000032c0: 616c 6c20 7265 636f 7665 7279 2222 220d  all recovery""".
+000032d0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+000032e0: 6573 6728 5072 6f74 6f63 6f6c 436f 6465  esg(ProtocolCode
+000032f0: 2e52 4553 544f 5245 2e76 616c 7565 2c20  .RESTORE.value, 
+00003300: 3129 0d0a 2020 2020 2020 2020 0d0a 2020  1)..        ..  
+00003310: 2020 6465 6620 7365 745f 6779 726f 5f73    def set_gyro_s
+00003320: 7461 7465 2873 656c 662c 2073 7461 7465  tate(self, state
+00003330: 3d31 293a 0d0a 2020 2020 2020 2020 2222  =1):..        ""
+00003340: 2253 6574 2067 7972 6f73 636f 7065 2063  "Set gyroscope c
+00003350: 616c 6962 7261 7469 6f6e 2073 7461 7475  alibration statu
+00003360: 7320 2873 6176 6520 6166 7465 7220 706f  s (save after po
+00003370: 7765 7220 6661 696c 7572 6529 0d0a 0d0a  wer failure)....
+00003380: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+00003390: 2020 2020 2020 2020 2020 2073 7461 7465             state
+000033a0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
+000033b0: 3a20 3120 2d20 6f70 656e 2e20 3020 2d20  : 1 - open. 0 - 
+000033c0: 636c 6f73 652e 2044 6566 6175 6c74 7320  close. Defaults 
+000033d0: 746f 2031 2e0d 0a20 2020 2020 2020 2022  to 1...        "
+000033e0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000033f0: 2e5f 6d65 7367 2850 726f 746f 636f 6c43  ._mesg(ProtocolC
+00003400: 6f64 652e 5345 545f 4759 524f 5f53 5441  ode.SET_GYRO_STA
+00003410: 5445 2e76 616c 7565 2c20 7374 6174 6529  TE.value, state)
+00003420: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00003430: 6465 6620 6765 745f 6779 726f 5f73 7461  def get_gyro_sta
+00003440: 7465 2873 656c 6629 3a0d 0a20 2020 2020  te(self):..     
+00003450: 2020 2022 2222 4765 7420 6779 726f 7363     """Get gyrosc
+00003460: 6f70 6520 6361 6c69 6272 6174 696f 6e20  ope calibration 
+00003470: 7374 6174 7573 0d0a 0d0a 2020 2020 2020  status....      
+00003480: 2020 5265 7475 726e 3a0d 0a20 2020 2020    Return:..     
+00003490: 2020 2020 2020 2031 202d 206f 7065 6e0d         1 - open.
+000034a0: 0a20 2020 2020 2020 2020 2020 2030 202d  .            0 -
+000034b0: 2063 6c6f 7365 0d0a 2020 2020 2020 2020   close..        
+000034c0: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+000034d0: 7572 6e20 7365 6c66 2e5f 6d65 7367 2850  urn self._mesg(P
+000034e0: 726f 746f 636f 6c43 6f64 652e 4745 545f  rotocolCode.GET_
+000034f0: 4759 524f 5f53 5441 5445 2e76 616c 7565  GYRO_STATE.value
+00003500: 2c20 6861 735f 7265 706c 7920 3d20 5472  , has_reply = Tr
+00003510: 7565 290d 0a20 2020 200d 0a20 2020 2064  ue)..    ..    d
+00003520: 6566 2067 6574 5f6d 6f64 6966 6965 645f  ef get_modified_
+00003530: 7665 7273 696f 6e28 7365 6c66 293a 0d0a  version(self):..
+00003540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00003550: 656c 662e 5f6d 6573 6728 5072 6f74 6f63  elf._mesg(Protoc
+00003560: 6f6c 436f 6465 2e47 4554 5f4d 4f44 4946  olCode.GET_MODIF
+00003570: 4945 445f 5645 5253 494f 4e2e 7661 6c75  IED_VERSION.valu
+00003580: 652c 2068 6173 5f72 6570 6c79 203d 2054  e, has_reply = T
+00003590: 7275 6529 0d0a 2020 2020 0d0a 2020 2020  rue)..    ..    
+000035a0: 2320 6465 6620 6765 745f 6261 7474 6572  # def get_batter
+000035b0: 795f 766f 6c74 6167 6528 7365 6c66 2c20  y_voltage(self, 
+000035c0: 6e75 6d3d 3129 3a0d 0a20 2020 2023 2020  num=1):..    #  
+000035d0: 2020 2022 2222 4765 7420 6261 7474 6572     """Get batter
+000035e0: 7920 766f 6c74 6167 650d 0a0d 0a20 2020  y voltage....   
+000035f0: 2023 2020 2020 2041 7267 733a 0d0a 2020   #     Args:..  
+00003600: 2020 2320 2020 2020 2020 2020 6e75 6d20    #         num 
+00003610: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
+00003620: 2042 6174 7465 7279 2049 4420 6e75 6d62   Battery ID numb
+00003630: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
+00003640: 312e 0d0a 2020 2020 2320 2020 2020 2222  1...    #     ""
+00003650: 220d 0a20 2020 2023 2020 2020 206d 6375  "..    #     mcu
+00003660: 5f64 6174 6120 3d20 7365 6c66 2e67 6574  _data = self.get
+00003670: 5f6d 6375 5f69 6e66 6f28 290d 0a20 2020  _mcu_info()..   
+00003680: 2023 2020 2020 2072 6574 7572 6e20 7365   #     return se
+00003690: 6c66 2e5f 6d65 7367 2850 726f 746f 636f  lf._mesg(Protoco
+000036a0: 6c43 6f64 652e 4745 545f 4241 5454 4552  lCode.GET_BATTER
+000036b0: 595f 494e 464f 2e76 616c 7565 2c20 6861  Y_INFO.value, ha
+000036c0: 735f 7265 706c 7920 3d20 5472 7565 29    s_reply = True)
```

### Comparing `pymycobot-3.4.4/pymycobot/myarm.py` & `pymycobot-3.4.5/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/myarmsocket.py` & `pymycobot-3.4.5/pymycobot/myarmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mybuddy.py` & `pymycobot-3.4.5/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mybuddybluetooth.py` & `pymycobot-3.4.5/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mybuddyemoticon.py` & `pymycobot-3.4.5/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mybuddysocket.py` & `pymycobot-3.4.5/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mycobot.py` & `pymycobot-3.4.5/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mycobotpro630.py` & `pymycobot-3.4.5/pymycobot/mycobotpro630.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import platform
 import time
 import math
 from enum import Enum
 import subprocess
 import logging
 import os
+import can
 from pymycobot.log import setup_logging
 
 
 def is_debian_os():
     try:
         # 执行 lsb_release -a 命令，并捕获输出
         result = subprocess.run(['lsb_release', '-a'], capture_output=True, text=True, check=True)
@@ -626,15 +627,15 @@
         Args:
             power_on_only (bool, optional): Only do power on. Defaults to False.
 
         Returns:
             bool: True if start successful, False otherwise.
         """
         self._power_off()
-        time.sleep(0.5)
+        time.sleep(1.0)
         power_on_ok = self.is_power_on()
         power_on_retry_count = 0
         while (not power_on_ok) and (power_on_retry_count <= 10):
             if power_on_only:
                 self._power_on_only()
             else:
                 self._power_on()
```

### Comparing `pymycobot-3.4.4/pymycobot/mycobotsocket.py` & `pymycobot-3.4.5/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mypalletizer.py` & `pymycobot-3.4.5/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/mypalletizersocket.py` & `pymycobot-3.4.5/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/public.py` & `pymycobot-3.4.5/pymycobot/public.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/robot_limit.json` & `pymycobot-3.4.5/pymycobot/robot_limit.json`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/ultraArm.py` & `pymycobot-3.4.5/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot/utils.py` & `pymycobot-3.4.5/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.4.5/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.4
+Version: 3.4.5
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
+Requires-Dist: python-can
 
 # This is Python API for ElephantRobotics product
 
 ![Python 2.7](https://img.shields.io/badge/Python-v2.7%5E-green?logo=python)
 ![Python 3](https://img.shields.io/badge/Python-v3%5E-green?logo=python)
 [![pypi_version](https://img.shields.io/pypi/v/pymycobot?label=pypi)](https://pypi.org/project/pigit)
 
@@ -199,14 +200,16 @@
     - [set\_transponder\_mode](#set_transponder_mode-1)
     - [set\_HTS\_gripper\_torque](#set_hts_gripper_torque)
     - [get\_HTS\_gripper\_torque](#get_hts_gripper_torque)
     - [get\_gripper\_protect\_current](#get_gripper_protect_current)
     - [init\_gripper](#init_gripper)
     - [set\_gripper\_protect\_current](#set_gripper_protect_current)
     - [set\_four\_pieces\_zero](#set_four_pieces_zero)
+    - [jog\_rpy](#jog_rpy)
+    - [set\_void\_compensate](#set_void_compensate)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
     - [gpio\_init](#gpio_init)
     - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
   - [get\_port\_list](#get_port_list)
@@ -1482,14 +1485,33 @@
 - **Prototype**: `set_four_pieces_zero()`
 
 - **Description**: Set the zero position of the four-piece motor.
 
 - **Return**
   - `int`: 1 - Set successful. 0 - Set failed.
 
+### jog_rpy
+
+- **Prototype**: `jog_rpy(end_direction, direction)`
+
+- **Description**: Rotate the end around a fixed axis in the base coordinate system.
+
+- **Parameters**
+  - `end_direction (int)`: Roll, Pitch, Yaw (1-3)
+  - `direction (int)`: 1 - forward rotation, 0 - reverse rotation
+
+### set_void_compensate
+
+- **Prototype**: `set_void_compensate(mode)`
+
+- **Description**: Set void compensation mode.
+
+- **Parameters**
+  - `mode (int)`: 0 - close, 1 - open
+
 ## Raspberry pi -- GPIO
 
 ### gpio_init
 
 - **Prototype**: `gpio_init()`
 
 - **Description**: Init GPIO module, and set BCM mode.
```

### Comparing `pymycobot-3.4.4/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.4.5/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/setup.py` & `pymycobot-3.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,10 +84,10 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["pyserial"],
+    install_requires=["pyserial","python-can"],
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*",
 )
```

### Comparing `pymycobot-3.4.4/tests/test_api.py` & `pymycobot-3.4.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/tests/test_generator.py` & `pymycobot-3.4.5/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.4/tests/test_socket.py` & `pymycobot-3.4.5/tests/test_socket.py`

 * *Files identical despite different names*

