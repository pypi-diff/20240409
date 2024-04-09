# Comparing `tmp/tcr_roboclaw-0.1.0.tar.gz` & `tmp/tcr_roboclaw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcr_roboclaw-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcr_roboclaw-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcr_roboclaw-0.1.0.tar` & `tcr_roboclaw-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     2413 2023-05-29 13:55:15.298515 tcr_roboclaw-0.1.0/.gitignore
--rw-r--r--   0        0        0      538 2023-08-25 19:21:23.076135 tcr_roboclaw-0.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2300 2023-08-25 19:21:23.076135 tcr_roboclaw-0.1.0/README.md
--rw-r--r--   0        0        0   564304 2023-08-25 19:21:23.092135 tcr_roboclaw-0.1.0/docs/roboclaw_datasheet_2x15A.pdf
--rw-r--r--   0        0        0  1343556 2023-08-25 19:21:23.104135 tcr_roboclaw-0.1.0/docs/roboclaw_user_manual.pdf
--rw-r--r--   0        0        0     1217 2023-08-25 19:21:23.104135 tcr_roboclaw-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      110 2023-08-25 19:21:39.264175 tcr_roboclaw-0.1.0/setup.cfg
--rw-r--r--   0        0        0      151 2023-08-25 19:21:39.264175 tcr_roboclaw-0.1.0/tcr_roboclaw/__init__.py
--rw-r--r--   0        0        0   152078 2023-08-25 19:21:23.104135 tcr_roboclaw-0.1.0/tcr_roboclaw/roboclaw.py
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 tcr_roboclaw-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2413 2023-05-29 13:55:15.298515 tcr_roboclaw-0.1.1/.gitignore
+-rw-r--r--   0        0        0      538 2023-08-25 19:30:09.013512 tcr_roboclaw-0.1.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     2300 2023-08-25 19:24:17.048570 tcr_roboclaw-0.1.1/README.md
+-rw-r--r--   0        0        0   564304 2023-08-25 19:24:17.056571 tcr_roboclaw-0.1.1/docs/roboclaw_datasheet_2x15A.pdf
+-rw-r--r--   0        0        0  1343556 2023-08-25 19:24:17.064571 tcr_roboclaw-0.1.1/docs/roboclaw_user_manual.pdf
+-rw-r--r--   0        0        0      332 2024-03-09 20:42:22.006349 tcr_roboclaw-0.1.1/examples/getting_started.py
+-rw-r--r--   0        0        0      626 2024-04-09 13:55:48.820141 tcr_roboclaw-0.1.1/examples/mixed.py
+-rw-r--r--   0        0        0     1234 2024-04-09 14:27:48.218529 tcr_roboclaw-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-04-09 14:31:32.621091 tcr_roboclaw-0.1.1/setup.cfg
+-rw-r--r--   0        0        0      151 2024-04-09 14:31:32.621091 tcr_roboclaw-0.1.1/tcr_roboclaw/__init__.py
+-rw-r--r--   0        0        0   152421 2024-04-09 14:27:15.358248 tcr_roboclaw-0.1.1/tcr_roboclaw/roboclaw.py
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 tcr_roboclaw-0.1.1/PKG-INFO
```

### Comparing `tcr_roboclaw-0.1.0/.gitignore` & `tcr_roboclaw-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcr_roboclaw-0.1.0/CHANGELOG.rst` & `tcr_roboclaw-0.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `tcr_roboclaw-0.1.0/README.md` & `tcr_roboclaw-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tcr_roboclaw-0.1.0/docs/roboclaw_datasheet_2x15A.pdf` & `tcr_roboclaw-0.1.1/docs/roboclaw_datasheet_2x15A.pdf`

 * *Files identical despite different names*

### Comparing `tcr_roboclaw-0.1.0/docs/roboclaw_user_manual.pdf` & `tcr_roboclaw-0.1.1/docs/roboclaw_user_manual.pdf`

 * *Files identical despite different names*

### Comparing `tcr_roboclaw-0.1.0/pyproject.toml` & `tcr_roboclaw-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
-requires = ["flit"]
-build-backend = "flit.buildapi"
+requires = ["flit_core >=2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "tcr-roboclaw"
 description = "An easy to install version of Basicmicro's RoboClaw Python library"
 authors = [{ name = "damienlarocque", email = "phicoltan@gmail.com" }]
 dependencies = ["pyserial"]
 readme = "README.md"
```

### Comparing `tcr_roboclaw-0.1.0/tcr_roboclaw/roboclaw.py` & `tcr_roboclaw-0.1.1/tcr_roboclaw/roboclaw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1904,75 +1904,81 @@
         Returns:
             bool: Command Acknowledgement
         """
         return self._write1(self.address, self.CMD.SETMAXLB, val)
 
     def SetM1VelocityPID(
         self,
-        p: int,
-        i: int,
-        d: int,
+        p: float,
+        i: float,
+        d: float,
         qpps: int,
     ) -> bool:
         """28 - Set Velocity PID Constants M1
 
         Several motor and quadrature combinations can be used with RoboClaw.
         In some cases, the default PID values will need to be tuned for the driven system.
         This gives greater flexibility in what motor and encoder combinations can be used.
         The RoboClaw PID system consist of four constants starting with QPPS, P = Proportional, I= Integral and D= Derivative.
         QPPS (quadrature pulses per second) is the speed of the encoder when the motor is at 100% power. P, I, D are the default values used after a reset.
 
+        The values of P, I, D are given as a ratio of 65536,
+        such that 1.0 -> 65536 =  0x00010000
+
         Args:
-            - p (int): proportional constant (default: 0x00010000)
-            - i (int): integral constant (default: 0x00008000)
-            - d (int): derivative constant (default: 0x00004000)
+            - p (float): proportional constant (default: 1.0 = 0x00010000)
+            - i (float): integral constant (default: 0.5 = 0x00008000)
+            - d (float): derivative constant (default: 0.25 = 0x00004000)
             - qpps (int): encoder speed when the motor is at 100% power (default: 44000)
 
         Returns:
             bool: Command Acknowledgement
         """
         return self._write4444(
             self.address,
             self.CMD.SETM1PID,
-            d * 65536,
-            p * 65536,
-            i * 65536,
+            int(d * 65536),
+            int(p * 65536),
+            int(i * 65536),
             qpps,
         )
 
     def SetM2VelocityPID(
         self,
-        p: int,
-        i: int,
-        d: int,
+        p: float,
+        i: float,
+        d: float,
         qpps: int,
     ) -> bool:
         """29 - Set Velocity PID Constants M2
 
         Several motor and quadrature combinations can be used with RoboClaw.
         In some cases, the default PID values will need to be tuned for the driven system.
         This gives greater flexibility in what motor and encoder combinations can be used.
         The RoboClaw PID system consist of four constants starting with QPPS, P = Proportional, I= Integral and D= Derivative.
         QPPS (quadrature pulses per second) is the speed of the encoder when the motor is at 100% power. P, I, D are the default values used after a reset.
 
+        The values of P, I, D are given as a ratio of 65536,
+        such that 1.0 -> 65536 =  0x00010000
+
         Args:
-            - p (int): proportional constant (default: 0x00010000)
-            - i (int): integral constant (default: 0x00008000)
-            - d (int): derivative constant (default: 0x00004000)
+            - p (float): proportional constant (default: 1.0 = 0x00010000)
+            - i (float): integral constant (default: 0.5 = 0x00008000)
+            - d (float): derivative constant (default: 0.25 = 0x00004000)
             - qpps (int): encoder speed when the motor is at 100% power (default: 44000)
 
         Returns:
             bool: Command Acknowledgement
         """
         return self._write4444(
             self.address,
             self.CMD.SETM2PID,
-            d * 65536,
-            p * 65536,
-            i * 65536,
+            int(d * 65536),
+            int(p * 65536),
+            int(i * 65536),
             qpps,
         )
 
     def ReadISpeedM1(self) -> Sequence[int, int, int]:
         """30 - Read Raw Speed M1
 
         Read the pulses counted in that last 300th of a second.
@@ -3898,15 +3904,18 @@
             - m1_blanking (int): M1 Current blanking percentage. The range is 0 to 6554 (0 to 20%).
             - m2_blanking (int): M2 Current blanking percentage. The range is 0 to 6554 (0 to 20%).
 
         Returns:
             bool: Command acknowledgement
         """
         return self._write22(
-            self.address, self.CMD.SETCURRENTBLANKINGPERCENTAGE, m1_blanking, m2_blanking
+            self.address,
+            self.CMD.SETCURRENTBLANKINGPERCENTAGE,
+            m1_blanking,
+            m2_blanking,
         )
 
     def GetCurrentBlankingPercentage(self) -> Sequence[int, int, int]:
         """118 - Read Current Blanking Percentage
 
         Read the current blanking percentages.
```

### Comparing `tcr_roboclaw-0.1.0/PKG-INFO` & `tcr_roboclaw-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcr-roboclaw
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy to install version of Basicmicro's RoboClaw Python library
 Author-email: damienlarocque <phicoltan@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

