# Comparing `tmp/CodingRider-2.2.tar.gz` & `tmp/CodingRider-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodingRider-2.2.tar", last modified: Mon Apr  8 06:14:47 2024, max compression
+gzip compressed data, was "CodingRider-2.3.tar", last modified: Tue Apr  9 06:23:53 2024, max compression
```

## Comparing `CodingRider-2.2.tar` & `CodingRider-2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 06:14:47.974104 CodingRider-2.2/
-drwxrwxrwx   0        0        0        0 2024-04-08 06:14:47.965532 CodingRider-2.2/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-04-05 06:35:16.000000 CodingRider-2.2/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-2.2/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-2.2/CodingRider/crc.py
--rw-rw-rw-   0        0        0    44020 2024-04-05 00:11:47.000000 CodingRider-2.2/CodingRider/drone.py
--rw-rw-rw-   0        0        0    73725 2024-04-08 00:29:36.000000 CodingRider-2.2/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-2.2/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-2.2/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-2.2/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:14:47.972104 CodingRider-2.2/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      626 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 06:14:47.000000 CodingRider-2.2/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-2.2/LICENSE
--rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2024-04-08 06:14:47.973106 CodingRider-2.2/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 06:14:47.974104 CodingRider-2.2/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-04-08 00:30:32.000000 CodingRider-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:23:53.799744 CodingRider-2.3/
+drwxrwxrwx   0        0        0        0 2024-04-09 06:23:53.790837 CodingRider-2.3/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-04-05 06:35:16.000000 CodingRider-2.3/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-2.3/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-2.3/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    44020 2024-04-05 00:11:47.000000 CodingRider-2.3/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    73925 2024-04-09 06:19:26.000000 CodingRider-2.3/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-2.3/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-2.3/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-2.3/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:23:53.798144 CodingRider-2.3/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      626 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 06:23:53.000000 CodingRider-2.3/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-2.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2024-04-09 06:23:53.798736 CodingRider-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 06:23:53.799744 CodingRider-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-04-09 06:16:55.000000 CodingRider-2.3/setup.py
```

### Comparing `CodingRider-2.2/CodingRider/crc.py` & `CodingRider-2.3/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.2/CodingRider/drone.py` & `CodingRider-2.3/CodingRider/drone.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.2/CodingRider/protocol.py` & `CodingRider-2.3/CodingRider/protocol.py`

 * *Files identical despite different names*

```diff
@@ -37,14 +37,15 @@
     Ping                        = 0x01      # 통신 확인
     Ack                         = 0x02      # 데이터 수신에 대한 응답
     Error                       = 0x03      # 오류(reserve, 비트 플래그는 추후에 지정)
     Request                     = 0x04      # 지정한 타입의 데이터 요청
     Message                     = 0x05      # 문자열 데이터
     Address                     = 0x06      # 장치 주소(MAC이 있는 경우 MAC) 혹은 고유번호(MAC이 없는 경우 UUID)
     Information                 = 0x07      # 펌웨어 및 장치 정보
+    Monitor                     = 0x0F      # 디버깅용 값 배열 전송. 첫번째 바이트에 타입, 두 번째 바이트에 페이지 지정(수신 받는 데이터의 저장 경로 구분)
     Control                     = 0x10      # 조종
 
     Command                     = 0x11      # 명령
     Pairing                     = 0x12      # 페어링
     Rssi                        = 0x13      # RSSI
     
     Battle                      = 0x1F      # 전투
```

### Comparing `CodingRider-2.2/CodingRider/receiver.py` & `CodingRider-2.3/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.2/CodingRider/storage.py` & `CodingRider-2.3/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.2/CodingRider/system.py` & `CodingRider-2.3/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `CodingRider-2.2/CodingRider.egg-info/PKG-INFO` & `CodingRider-2.3/CodingRider.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.2
+Version: 2.3
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CodingRider-2.2/PKG-INFO` & `CodingRider-2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.2
+Version: 2.3
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CodingRider-2.2/setup.py` & `CodingRider-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.2",
+    version = "2.3",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```

