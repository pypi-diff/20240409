# Comparing `tmp/menlo-syncro-0.0.38.tar.gz` & `tmp/menlo-syncro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menlo-syncro-0.0.38.tar", last modified: Tue Oct 31 11:43:24 2023, max compression
+gzip compressed data, was "menlo-syncro-0.1.0.tar", last modified: Tue Apr  9 12:28:24 2024, max compression
```

## Comparing `menlo-syncro-0.0.38.tar` & `menlo-syncro-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 11:43:24.481073 menlo-syncro-0.0.38/
--rw-r--r--   0 florin    (1000) florin    (1000)       71 2023-10-31 11:43:14.000000 menlo-syncro-0.0.38/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-02-09 13:57:37.000000 menlo-syncro-0.0.38/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     1452 2023-10-31 11:43:24.481073 menlo-syncro-0.0.38/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      573 2023-10-31 11:43:14.000000 menlo-syncro-0.0.38/README.md
--rw-r--r--   0 florin    (1000) florin    (1000)     1133 2023-10-31 11:43:14.000000 menlo-syncro-0.0.38/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)       38 2023-10-31 11:43:24.481073 menlo-syncro-0.0.38/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 11:43:24.477073 menlo-syncro-0.0.38/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 11:43:24.479073 menlo-syncro-0.0.38/src/menlo_syncro.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     1452 2023-10-31 11:43:24.000000 menlo-syncro-0.0.38/src/menlo_syncro.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      388 2023-10-31 11:43:24.000000 menlo-syncro-0.0.38/src/menlo_syncro.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-10-31 11:43:24.000000 menlo-syncro-0.0.38/src/menlo_syncro.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       42 2023-10-31 11:43:24.000000 menlo-syncro-0.0.38/src/menlo_syncro.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        9 2023-10-31 11:43:24.000000 menlo-syncro-0.0.38/src/menlo_syncro.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 11:43:24.480073 menlo-syncro-0.0.38/src/syncster/
--rw-r--r--   0 florin    (1000) florin    (1000)      851 2023-02-09 13:57:37.000000 menlo-syncro-0.0.38/src/syncster/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      413 2023-10-31 11:43:24.000000 menlo-syncro-0.0.38/src/syncster/_version.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5408 2023-02-09 13:57:37.000000 menlo-syncro-0.0.38/src/syncster/crc.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19705 2023-02-09 13:57:37.000000 menlo-syncro-0.0.38/src/syncster/hrt.py
--rw-r--r--   0 florin    (1000) florin    (1000)    13718 2023-02-09 13:57:37.000000 menlo-syncro-0.0.38/src/syncster/rbp.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4244 2023-02-09 13:57:37.000000 menlo-syncro-0.0.38/src/syncster/syncro.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:28:24.823280 menlo-syncro-0.1.0/
+-rw-r--r--   0 florin    (1000) florin    (1000)       71 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     1538 2024-04-09 12:28:24.823280 menlo-syncro-0.1.0/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      573 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/README.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     1225 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)       38 2024-04-09 12:28:24.823280 menlo-syncro-0.1.0/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:28:24.820280 menlo-syncro-0.1.0/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:28:24.822280 menlo-syncro-0.1.0/src/menlo_syncro.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     1538 2024-04-09 12:28:24.000000 menlo-syncro-0.1.0/src/menlo_syncro.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      386 2024-04-09 12:28:24.000000 menlo-syncro-0.1.0/src/menlo_syncro.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-09 12:28:24.000000 menlo-syncro-0.1.0/src/menlo_syncro.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       65 2024-04-09 12:28:24.000000 menlo-syncro-0.1.0/src/menlo_syncro.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        9 2024-04-09 12:28:24.000000 menlo-syncro-0.1.0/src/menlo_syncro.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:28:24.822280 menlo-syncro-0.1.0/src/syncster/
+-rw-r--r--   0 florin    (1000) florin    (1000)      851 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/src/syncster/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-09 12:28:24.000000 menlo-syncro-0.1.0/src/syncster/_version.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5408 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/src/syncster/crc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    22306 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/src/syncster/hrt.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    13811 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/src/syncster/rbp.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:28:24.822280 menlo-syncro-0.1.0/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)      344 2024-04-09 09:56:11.000000 menlo-syncro-0.1.0/tests/test_syncro.py
```

### Comparing `menlo-syncro-0.0.38/COPYING.md` & `menlo-syncro-0.1.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `menlo-syncro-0.0.38/PKG-INFO` & `menlo-syncro-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menlo-syncro
-Version: 0.0.38
+Version: 0.1.0
 Summary: Unofficial Python framework for communication with the Menlo Syncro RRE laser synchronization unit
 Author-email: Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/syncster
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: COPYING.md
 Requires-Dist: pyserial
 Requires-Dist: pyyaml
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: caproto; extra == "test"
 
 Synster -- Python API for Menlo Syncro box
 ==========================================
 
 Dependencies
 ------------
```

### Comparing `menlo-syncro-0.0.38/README.md` & `menlo-syncro-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `menlo-syncro-0.0.38/pyproject.toml` & `menlo-syncro-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,24 @@
 [project.urls]
 "Source Code" = "https://gitlab.com/codedump2/syncster"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
+    "pytest-asyncio",
+    "caproto"
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-ra"
+addopts = "-ra -s"
 log_cli = true
 testpaths = [
     "tests",
 ]
 
 [tool.setuptools_scm]
 write_to = "src/syncster/_version.py"
+
+[project.scripts]
+#moo = "syncster.application:main"
```

### Comparing `menlo-syncro-0.0.38/src/menlo_syncro.egg-info/PKG-INFO` & `menlo-syncro-0.1.0/src/menlo_syncro.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menlo-syncro
-Version: 0.0.38
+Version: 0.1.0
 Summary: Unofficial Python framework for communication with the Menlo Syncro RRE laser synchronization unit
 Author-email: Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/syncster
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: COPYING.md
 Requires-Dist: pyserial
 Requires-Dist: pyyaml
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: caproto; extra == "test"
 
 Synster -- Python API for Menlo Syncro box
 ==========================================
 
 Dependencies
 ------------
```

### Comparing `menlo-syncro-0.0.38/src/syncster/__init__.py` & `menlo-syncro-0.1.0/src/syncster/__init__.py`

 * *Files identical despite different names*

### Comparing `menlo-syncro-0.0.38/src/syncster/crc.py` & `menlo-syncro-0.1.0/src/syncster/crc.py`

 * *Files identical despite different names*

### Comparing `menlo-syncro-0.0.38/src/syncster/hrt.py` & `menlo-syncro-0.1.0/src/syncster/hrt.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 #        You should have received a copy of the GNU General Public License
 #        along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 from syncster import rbp
 import logging, struct
 
+logger = logging.getLogger(__name__)
+
 '''
 This implements structures and definitions for handling the
 Hierarchical Register Tree (HRT). It starts off with the minimal
 device tree as defined by the Menlo documentation, and offers
 ways to easily extend the register definitions.
 '''
 
@@ -63,15 +65,15 @@
          it into a bytearray first.
 
        - "units": optional; if it exists, it is a hint as to the units of the data
          (usually only useful to the end user and/or for displaying purposes).
 '''
 
 RegisterDataTypes = {
-    
+   
     0x01: { "label": "NONE", "format": None },
     0x02: { "label": "NODE", "format": None },
 
     # Docs say this is supposed to be one U8 value, but my device returns 3 bytes, e.g. (2, 1, 1)
     0x03: { "label": "REGVERS", "format": lambda b: "%dB" % len(b) },
     
     0x04: { "label": "SUBREGS", "format": lambda b: "%dB" % len(b) },
@@ -79,22 +81,21 @@
     # String parameter is sent 0-terminated, but we'll parse it without the 0.    
     0x05: { "label": "REGDEF", "format": lambda b: "B%dsxB" % (len(b)-3),
             "format_keys": { "type": int,
                              "label": lambda s: s.decode('ascii'),
                              "access": lambda s: ["", "rw", "r", "w"][s] } },
     
     0x07: { "label": "ADDRESS", "format": "B" },
-    0x08: { "label": "TYPE", "format": ">H" },
+    0x08: { "label": "TYPE", "format": "<H" },
 
-    # format: SERS 
-    0x09: { "label": "SER", "format": "BB>H", "format_keys": [ "day", "month", "year" ] },
+    0x09: { "label": "SERS", "format": "<BBH", "format_keys": [ "day", "month", "year" ] },
 
     0x0a: { "label": "REMOTE_SERVICEMODE", "format": "B" },
     
-    0x0d: { "label": "TSTAMP", "format": ">L>H", "format_keys": [ "sec", "msec" ] },
+    0x0d: { "label": "TSTAMP", "format": "<LH", "format_keys": [ "sec", "msec" ] },
     
     0x0f: { "label": "DEVID", "format": lambda b: "%dsx" % (len(b)-1) },
 
     # format: VERS
     0x10: { "label": "VERS", "format": "BBBB", "format_keys": [ "build", "patch", "minor", "major" ] },
 
     #0x20: { "label": "EDIP_BMP", "format": lambda b: "%dB" % len(b) },
@@ -102,51 +103,55 @@
 
     0x30: { "label": "REMODE_EDIP", "format": "B" },
     0x31: { "label": "REMODE_AMP", "format": "B" },
     0x32: { "label": "REMODE_SEED", "format": "B" },
     0x33: { "label": "REMODE_SPI", "format": lambda b: "%dB" % len(b) },
     
     0x50: { "label": "SAVESETTINGS", "format": "B" },
-    0x51: { "label": "U16_mA", "format": ">l", "units": "mA" },
-    0x52: { "label": "CALIB_DAC", "format": ">H>H>H>H>l>l" },
-    0x53: { "label": "CALIB_ADC", "format": ">H>H>H>H" },
-    0x54: { "label": "S32_mV", "format": ">H", "units": "mV" },
+    0x51: { "label": "U16_mA", "format": "<H", "units": "mA" },
+    0x52: { "label": "CALIB_DAC", "format": "<llllHH" },
+    0x53: { "label": "CALIB_ADC", "format": "<llll" },
+    0x54: { "label": "S32_mV", "format": "<l", "units": "mV" },
     0x55: { "label": "U8_enum", "format": "B" },
     0x56: { "label": "U8_bool", "format": "B" },
 
-    0x57: { "label": "S32_mV", "format": ">H", "units": "mV" },
-    0x58: { "label": "S32",    "format": ">H", "units": "steps" },
-    0x59: { "label": "S32_mC", "format": ">H", "units": "m°C" },
-    0x5a: { "label": "S32_uC", "format": ">H", "units": "μ°C" },
+    0x57: { "label": "S32_mV", "format": "<l", "units": "mV" },
+    0x58: { "label": "S32",    "format": "<l", "units": "steps" },
+    0x59: { "label": "S32_mC", "format": "<l", "units": "m°C" },
+    0x5a: { "label": "S32_uC", "format": "<l", "units": "μ°C" },
     
-    0x5b: { "label": "U32_Hz", "format": ">H",  "units": "Hz" },
-    0x5b: { "label": "U32_mHz", "format": ">H", "units": "mHz" },
-    0x5b: { "label": "U32_kHz", "format": ">H", "units": "kHz" },
-    0x5b: { "label": "U32_mW", "format": ">H",  "units": "mW" },
+    0x5b: { "label": "U32_Hz", "format": "<l",  "units": "Hz" },
+    0x5b: { "label": "U32_mHz", "format": "<l", "units": "mHz" },
+    0x5b: { "label": "U32_kHz", "format": "<l", "units": "kHz" },
+    0x5b: { "label": "U32_mW", "format": "<l",  "units": "mW" },
     
-    0x5f: { "label": "S32_uV", "format": ">H", "units": "uV" },
+    0x5f: { "label": "S32_uV", "format": "<l", "units": "uV" },
 
-    0x60: { "label": "U32_us", "format": ">H", "units": "us" },
+    0x60: { "label": "U32_us", "format": "<l", "units": "us" },
 
-    0x61: { "label": "S32_mA", "format": ">H",   "units": "mA" },
-    0x62: { "label": "S32_mW_K", "format": ">H", "units": "mW/K" },
-    0x63: { "label": "S32_mJ_K", "format": ">H", "units": "mJ/K" },
+    0x61: { "label": "S32_mA", "format": "<l",   "units": "mA" },
+    0x62: { "label": "S32_mW_K", "format": "<l", "units": "mW/K" },
+    0x63: { "label": "S32_mJ_K", "format": "<l", "units": "mJ/K" },
     
-    0x81: { "label": "U16", "format": ">l" },
+    0x81: { "label": "U16", "format": "<H" },
+
+    0xae: { "label": "SYNCHRO_TRACKLOG",
+            "format": "<llll",
+            "format_keys": [ "lb_out", "t1_pos", "lb_in", "t2_pos" ] },
 
     # This is from the main documentation (does this contain one or several such lines?)
-    #0xe4: { "label": "LOGHIST", "format": lambda b: (">L>HBB>L>L" * (len(b)/16)),
+    #0xe4: { "label": "LOGHIST", "format": lambda b: ("<L>HBB>L>L" * (len(b)/16)),
     #        #"format_keys": [ "sec", "msec", "context", "event", "val", "ref" ] },
     #       }
 
     # This is from the Syncro RRE documentation, apparently it contains
     # up to 50 such entries. Strategy here would be to auto-sense that the
     # buffer size is a multiple of the format size and run struct.iter_unpack(),
     # then return an array of log entries.
-    0xe4: { "format": ">L>lB BBBB >l>l>L>L",
+    0xe4: { "format": "<LlBBBBBllHH",
             "format_keys": [ "sec", "msec", "remain",
                              "level", "context", "subcontext1", "subcontext2",
                              "msgid", "line", "val", "ref" ] },
            
 }
 
 '''
@@ -207,35 +212,35 @@
             how to unpack the data using `struct.unpack()`) or "type" (a numerical
             key of `RegisterDataTypes`)
 
         '''
         self.dev = dev
         self.src = src
         self.dst = dst
-        self.access = rspec.get('access', 'r')        
+        self.access = rspec.get('access', 'r')
         
         self.addr = \
             bytearray(addr_prefix or b'') + \
             bytearray(rspec['addr']) + \
             bytearray(addr_suffix or b'')
         
         if "format" in rspec:
             fmt_dict = rspec
         else:
             try:
                 fmt_dict = RegisterDataTypes[rspec['type']]
             except KeyError:
-                logging.warning("Missing type definition for 0x%.2x -- decoding as byte array" % rspec['type'])
+                logger.warning("Missing type definition for 0x%.2x -- decoding as byte array" % rspec['type'])
                 fmt_dict = { 'format': lambda b: '%dB' % len(b) }
             
         self.fmt = fmt_dict['format']
         self.fmt_keys = fmt_dict.get('format_keys', None)
 
 
-    def _read(self):
+    def _read(self, addr=None):
 
         if 'r' not in self.access:
             raise RuntimeError("Register %x cannot be read (access: %s)"
                                % (self.addr, self.access))
         
         # Reading operation only.
         response = self.dev.req(rbp.Message(src=self.src, dest=self.dst,
@@ -247,25 +252,25 @@
         dat = response.payload[1:]
         #reg = response.payload[:len(self.addr)]
         #dat = response.payload[len(self.addr):]
 
         # format is either an unpack string, or a callable generating an unpack string.
         fmt = self.fmt(dat) if hasattr(self.fmt, "__call__") else self.fmt
 
-        logging.debug("Response: %r" % response)
-        logging.debug("Format: %s" % fmt)
+        logger.debug("Response: %r" % response)
+        logger.debug("Format: %s" % fmt)
 
         #print ()
         #print ("Message:", response)
         #print ("Register:", reg)
         #print ("Datagram:", dat)
         #print ("Format:", fmt)
 
         tmp_data = struct.iter_unpack(fmt, dat)
-        logging.debug ("Unpack:", tmp_data)
+        logger.debug ("Unpack:", tmp_data)
 
         # apply field naming -- note that we treat all data as if it
         # had been iter-inp
         if self.fmt_keys is not None:
             data = []
             for dt in tmp_data:
                 # if fmt_keys is a dictionary, the 'value' is in fact a translator.                
@@ -281,61 +286,117 @@
             data = data[0]
 
         # reduce again to only blank element if unpacking only resulted in one single item
         if len(data)==1:
             data = data[0]
 
         return data
-    
+
+
+    def _write_values(self, *args):
+        
+        if 'w' not in self.access:
+            raise RuntimeError(f"Register {self.addr} cannot be modified (access: '{self.access}')")
+
+        # format is either an unpack string, or a callable generating an unpack string.
+        if hasattr(self.fmt, "__call__"):
+            raise RuntimeError(f'Cannot pack data using a callable format spec')
+        
+        data = struct.pack(self.fmt, *args)
+        
+        response = self.dev.req(rbp.Message(src=self.src, dest=self.dst,
+                                            cmd=rbp.Commands.WRITE,
+                                            data=self.addr+data))
+
+        logger.debug("Response: %r" % response)
+
+        return response
+
         
     def __call__(self, *args, **kw):
         '''
         Reads/writes data to register, or, optionally, to/from named register fields.
         FIXME: how do we access indivitual fields by name only, without accessing other
                fields of a specific register?...
         '''
 
         if len(args) == 0 and len(kw) == 0:
             return self._read()
 
         elif len(args) > 0:
+            if len(kw) > 0:
+                raise RuntimeError(f'You may write values into registers either '
+                                   f'by value or by name, not both')
             # Writing operation, by value(s)
-            pass
+            self._write_values(*args)
             
         else:
+            if len(args) > 0:
+                raise RuntimeError(f'You may write values into registers either '
+                                   f'by value or by name, not both')
             # Writing operation, by name(s)
-            pass
+            raise RuntimeError('Writing by name not implemented')
+            pass        
 
 
 class NodeAccess:
     '''
     Offers easy Python-esque access to HRT registers by name, as members of
-    a class (this class).
+    a class (this class). Each HRT node may contain two types of entries:
+    "subnodes" and "registers".
+
+    A register is an endpoint, essentially containing useful data, that can
+    be accessed using the RBP commands `READ` and `WRITE`, and which may receive
+    replies in the form of `ACK`, `NACK`, `DGRAM` or others.
+
+    Each node has at least 3 registers. They are specified in `IntrospectionTree`:
+    
+      - `RegVers`: a register containing a data tuple specifying the register
+        version implemented within the device;
+
+      - `Subregs`: a register containg an array of integers (bytes) with the
+        IDs of all the node entries
+
+      - `RegDefs`: a register containing definitions (name, data type, access type)
+        for each of the registers in `Subregs`.
+     
     '''
     def __init__(self, dev=None, node=None, tree=None, recurse=1, **raParams):
-        '''
-        Initializes members based on device (an `synster.rbp.Device`) and
-        tree information. The tree information is analogous to `IntrospectionTree`.
+        '''  Initializes a HRT node access class based on device  and tree information.
+        
+        The tree information is analogous to `IntrospectionTree`.
         It uses `hrt.RegisterAccess` under the hood. `raParams` are
-        passed on as parameters for `RegisterAccess` calls and may contain
+        passed on as parameters for `RegisterAccess` calls and may contain        
         supplementary settings as `addr_prefix` or similar.
+
+        Args:
+        
+            dev: a `rbp.Device` object
+
+            node: a list of integers (node address). If the list is empty, the root
+              is accessed.
+
+            tree: a dictionary of the expected entries on the node to access. If this
+              is `None`, the node is assumed to contain at least the `hrt.IntrospectionTree`
+              items (typically true only for a root node) and the complete list is
+              obtained by introspection using those registers.
         '''
 
         if recurse < 0:
             raise RuntimeError("Recursion too deep")
         
         self._dev = dev or rbp.Device()
 
         # Node is supposed to be a sequence of bytes. For convenience, we accept
         # single integer values, but convert them to sequences as soon as possible.
         if node is None:
             self._node = []
         else:
             self._node = node if hasattr(node, "__len__") else [node]
-            logging.debug("New access for node: %r" % (self._node,))
+            logger.debug("New access for node: %r" % (self._node,))
 
         # Rely on 'node' and enquire a tree layout from the device itself.
         if tree is not None:
             _tree = tree
         else:
             _tree = ls_node(dev=self._dev, node=self._node)
         
@@ -360,15 +421,15 @@
             key_cnt = 2
             while (key in self._subs) or (key in self._regs):
                 key = "%s%d" % (key_orig, key_cnt)
                 key_cnt += 1
 
             self._tree[key] = _tree[k]
 
-            logging.debug("New key: %s" % key)
+            logger.debug("New key: %s" % key)
             
             if v['access'] == '':
                 # For subregisters, we do lazy-loading only to avoid recursion
                 # within the device introspection data itself.
                 self._subs[key] = v
             else:
                 self._regs[key] = RegisterAccess(self._dev, **raParams, **v)
```

### Comparing `menlo-syncro-0.0.38/src/syncster/rbp.py` & `menlo-syncro-0.1.0/src/syncster/rbp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 #        You should have received a copy of the GNU General Public License
 #        along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 from syncster.crc import crc16
 import struct, logging, serial
 
+logger = logging.getLogger(__name__)
+
 class ByteTagger(object):
     '''
     Helper object to allow a more expressive attribution of byte values <-> string.
     Initiate as:
     ```
         >>> foo = ByteTagger({'bar': 42, 'goo': 43})
         >>> foo.bar
@@ -189,14 +191,18 @@
         return self._cmd
 
     @property
     def payload(self):
         return self._data
 
 
+    def __repr__(self):
+        return self.__str__()
+
+
     def __str__(self):
         if self.command in [ Commands.READ, Commands.WRITE, Commands.ECHO ]:
             addr = "%.2x -> %.2x:" % (self.source, self.destination)
         else:
             addr = "%.2x <- %.2x:" % (self.destination, self.source)
 
         payload = " ".join([("%c"%x if x>32 and x<128 else "%.2x"%x)
@@ -316,15 +322,15 @@
         Sends one message, waits for response and interprets the response.
         If the message is a READ, the function returns the coresponding DGRAM message.
         If the message is a WRITE, the function checks for ACK/NACK and raises an IOError exception.
         If the message is an ECHO, the function returns one or more of the corresponding REPLY.
         '''
 
         while True:
-            logging.debug("Request: %r" % msg)
+            logger.debug("Request: %r" % msg)
             self.sendMsg(msg)
             r = self.recvMsg()
         
             if r.command in [ Commands.DGRAM, Commands.REPLY, Commands.ACK ]:
                 return r
 
             if r.command == Commands.CRCERR:
```

