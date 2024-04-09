# Comparing `tmp/winiel-rfid-sensor-0.0.4.tar.gz` & `tmp/winiel-rfid-sensor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winiel-rfid-sensor-0.0.4.tar", last modified: Fri Mar 29 06:53:13 2024, max compression
+gzip compressed data, was "winiel-rfid-sensor-0.0.5.tar", last modified: Tue Apr  9 05:13:37 2024, max compression
```

## Comparing `winiel-rfid-sensor-0.0.4.tar` & `winiel-rfid-sensor-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-03-29 06:53:13.801811 winiel-rfid-sensor-0.0.4/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-03-29 06:53:13.801350 winiel-rfid-sensor-0.0.4/PKG-INFO
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       38 2024-03-29 06:53:13.801922 winiel-rfid-sensor-0.0.4/setup.cfg
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      687 2024-03-29 06:53:02.000000 winiel-rfid-sensor-0.0.4/setup.py
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-03-29 06:53:13.798186 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       22 2024-03-29 06:53:08.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor/__init__.py
--rw-r--r--   0 yongjinsohn   (501) staff       (20)     4544 2024-03-29 06:51:45.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor/rfid_sensor.py
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-03-29 06:53:13.800803 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-03-29 06:53:13.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/PKG-INFO
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      323 2024-03-29 06:53:13.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 06:53:13.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 04:23:22.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/not-zip-safe
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       15 2024-03-29 06:53:13.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/requires.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       19 2024-03-29 06:53:13.000000 winiel-rfid-sensor-0.0.4/winiel_rfid_sensor.egg-info/top_level.txt
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-09 05:13:37.119896 winiel-rfid-sensor-0.0.5/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-09 05:13:37.119468 winiel-rfid-sensor-0.0.5/PKG-INFO
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       38 2024-04-09 05:13:37.119988 winiel-rfid-sensor-0.0.5/setup.cfg
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      687 2024-04-09 05:11:55.000000 winiel-rfid-sensor-0.0.5/setup.py
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-09 05:13:37.115997 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       22 2024-04-09 05:11:55.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/__init__.py
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)     4567 2024-04-09 05:10:17.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/rfid_sensor.py
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-09 05:13:37.118984 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      323 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 04:23:22.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/not-zip-safe
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       15 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/requires.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       19 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/top_level.txt
```

### Comparing `winiel-rfid-sensor-0.0.4/setup.py` & `winiel-rfid-sensor-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='winiel-rfid-sensor',
-    version='0.0.4',
+    version='0.0.5',
     description='PYPI tutorial package creation written by winiel',
     author='winiel',
     author_email='winiel@naver.com ',
     url='https://github.com/winiel',
     install_requires=['pyserial', 'pyusb'],
     packages=find_packages(exclude=[]),
     keywords=['winiel', 'rfid', 'sensor'],
```

### Comparing `winiel-rfid-sensor-0.0.4/winiel_rfid_sensor/rfid_sensor.py` & `winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/rfid_sensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 
 import serial
 
 
 class RfidSensor():
     results = {}
 
-    def __init__(self, arduino_port='/dev/cu.usbmodem143301', baud_rate=115200, timeout=1 ):
+    def __init__(self, arduino_port='/dev/cu.usbmodem143301', baud_rate=115200, duration=1 ):
         # Arduino가 연결된 시리얼 포트와 바우드 레이트 설정
 
         # 시리얼 연결 초기화
-        self.ser = serial.Serial(arduino_port, baud_rate, timeout=timeout)
+        self.ser = serial.Serial(arduino_port, baud_rate, timeout=1)
         self.ser.flush()
 
+
+
         # 장치가 데이터 전송 준비를 할 수 있도록 잠시 대기
         time.sleep(2)
 
-        thread1 = threading.Thread(target=self._threading, args=( ))
+        thread1 = threading.Thread(target=self._threading, args=(duration, ))
         thread1.start()
 
 
     def sensorClose(self):
         self.ser.close()
 
-    def _threading(self):
+    def _threading(self, duration):
         while True:
-            self._sensor_data(1)
+            self._sensor_data(duration)
 
 
     def _sensor_data(self, duration=1):
         try:
 
             start_time = time.time()
             data_by_id = {}
```

