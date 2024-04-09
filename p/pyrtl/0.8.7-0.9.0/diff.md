# Comparing `tmp/pyrtl-0.8.7.tar.gz` & `tmp/pyrtl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrtl-0.8.7.tar", last modified: Mon Jul 15 06:48:55 2019, max compression
+gzip compressed data, was "dist/pyrtl-0.9.0.tar", last modified: Sat Mar  6 02:01:39 2021, max compression
```

## Comparing `pyrtl-0.8.7.tar` & `pyrtl-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 sherwood   (502) staff       (20)        0 2019-07-15 06:48:55.000000 pyrtl-0.8.7/
--rw-r--r--   0 sherwood   (502) staff       (20)     1015 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PKG-INFO
-drwxr-xr-x   0 sherwood   (502) staff       (20)        0 2019-07-15 06:48:55.000000 pyrtl-0.8.7/pyrtl/
--rw-r--r--   0 sherwood   (502) staff       (20)    40712 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/simulation.py
-drwxr-xr-x   0 sherwood   (502) staff       (20)        0 2019-07-15 06:48:55.000000 pyrtl-0.8.7/pyrtl/rtllib/
--rw-r--r--   0 sherwood   (502) staff       (20)     9943 2017-04-28 22:35:59.000000 pyrtl-0.8.7/pyrtl/rtllib/multipliers.py
--rw-r--r--   0 sherwood   (502) staff       (20)    19973 2017-04-28 22:35:59.000000 pyrtl-0.8.7/pyrtl/rtllib/aes.py
--rw-r--r--   0 sherwood   (502) staff       (20)        0 2015-10-11 05:04:13.000000 pyrtl-0.8.7/pyrtl/rtllib/__init__.py
--rw-r--r--   0 sherwood   (502) staff       (20)     7265 2017-04-28 22:35:59.000000 pyrtl-0.8.7/pyrtl/rtllib/muxes.py
--rw-r--r--   0 sherwood   (502) staff       (20)     5458 2018-01-09 19:19:27.000000 pyrtl-0.8.7/pyrtl/rtllib/testingutils.py
--rw-r--r--   0 sherwood   (502) staff       (20)    10915 2017-04-28 22:35:59.000000 pyrtl-0.8.7/pyrtl/rtllib/adders.py
--rw-r--r--   0 sherwood   (502) staff       (20)     2993 2017-04-28 22:35:59.000000 pyrtl-0.8.7/pyrtl/rtllib/libutils.py
--rw-r--r--   0 sherwood   (502) staff       (20)     1834 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/rtllib/barrel.py
--rw-r--r--   0 sherwood   (502) staff       (20)    11274 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/rtllib/prngs.py
-drwxr-xr-x   0 sherwood   (502) staff       (20)        0 2019-07-15 06:48:55.000000 pyrtl-0.8.7/pyrtl/analysis/
--rw-r--r--   0 sherwood   (502) staff       (20)      114 2016-06-28 00:17:17.000000 pyrtl-0.8.7/pyrtl/analysis/__init__.py
--rw-r--r--   0 sherwood   (502) staff       (20)    16198 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/analysis/estimate.py
--rw-r--r--   0 sherwood   (502) staff       (20)    19689 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/helperfuncs.py
--rw-r--r--   0 sherwood   (502) staff       (20)    15810 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/memory.py
--rw-r--r--   0 sherwood   (502) staff       (20)    25813 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/corecircuits.py
--rw-r--r--   0 sherwood   (502) staff       (20)     3319 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/__init__.py
--rw-r--r--   0 sherwood   (502) staff       (20)    39396 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/core.py
--rw-r--r--   0 sherwood   (502) staff       (20)    14770 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/verilog.py
--rw-r--r--   0 sherwood   (502) staff       (20)    30991 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/wire.py
--rw-r--r--   0 sherwood   (502) staff       (20)    25336 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/inputoutput.py
--rw-r--r--   0 sherwood   (502) staff       (20)     9067 2019-05-25 05:54:03.000000 pyrtl-0.8.7/pyrtl/transform.py
--rw-r--r--   0 sherwood   (502) staff       (20)    25547 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/compilesim.py
--rw-r--r--   0 sherwood   (502) staff       (20)    11292 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/conditional.py
--rw-r--r--   0 sherwood   (502) staff       (20)      467 2015-10-11 05:04:13.000000 pyrtl-0.8.7/pyrtl/pyrtlexceptions.py
--rw-r--r--   0 sherwood   (502) staff       (20)     8033 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/toFirrtl.py
--rw-r--r--   0 sherwood   (502) staff       (20)    21260 2019-07-15 06:36:08.000000 pyrtl-0.8.7/pyrtl/passes.py
-drwxr-xr-x   0 sherwood   (502) staff       (20)        0 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PyRTL.egg-info/
--rw-r--r--   0 sherwood   (502) staff       (20)     1015 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PyRTL.egg-info/PKG-INFO
--rw-r--r--   0 sherwood   (502) staff       (20)     1188 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PyRTL.egg-info/SOURCES.txt
--rw-r--r--   0 sherwood   (502) staff       (20)       30 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PyRTL.egg-info/requires.txt
--rw-r--r--   0 sherwood   (502) staff       (20)       12 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PyRTL.egg-info/top_level.txt
--rw-r--r--   0 sherwood   (502) staff       (20)        1 2019-07-15 06:48:55.000000 pyrtl-0.8.7/PyRTL.egg-info/dependency_links.txt
-drwxr-xr-x   0 sherwood   (502) staff       (20)        0 2019-07-15 06:48:55.000000 pyrtl-0.8.7/tests/
--rw-r--r--   0 sherwood   (502) staff       (20)     5912 2019-07-15 06:36:08.000000 pyrtl-0.8.7/tests/test_signed.py
--rw-r--r--   0 sherwood   (502) staff       (20)    28198 2019-07-15 06:36:08.000000 pyrtl-0.8.7/tests/test_compilesim.py
--rw-r--r--   0 sherwood   (502) staff       (20)     6268 2017-04-28 22:35:59.000000 pyrtl-0.8.7/tests/test_transform.py
--rw-r--r--   0 sherwood   (502) staff       (20)    23714 2017-04-28 22:35:59.000000 pyrtl-0.8.7/tests/test_core.py
--rw-r--r--   0 sherwood   (502) staff       (20)        0 2015-10-11 05:04:13.000000 pyrtl-0.8.7/tests/__init__.py
--rw-r--r--   0 sherwood   (502) staff       (20)    21199 2017-04-28 22:35:59.000000 pyrtl-0.8.7/tests/test_passes.py
--rw-r--r--   0 sherwood   (502) staff       (20)    25834 2019-07-15 06:36:08.000000 pyrtl-0.8.7/tests/test_helperfuncs.py
--rw-r--r--   0 sherwood   (502) staff       (20)    14912 2017-04-28 22:35:59.000000 pyrtl-0.8.7/tests/test_memblock.py
--rw-r--r--   0 sherwood   (502) staff       (20)    18154 2017-04-28 22:35:59.000000 pyrtl-0.8.7/tests/test_conditional.py
--rw-r--r--   0 sherwood   (502) staff       (20)    10981 2019-07-15 06:36:08.000000 pyrtl-0.8.7/tests/test_wire.py
--rw-r--r--   0 sherwood   (502) staff       (20)    29219 2019-07-15 06:36:08.000000 pyrtl-0.8.7/tests/test_simulation.py
--rw-r--r--   0 sherwood   (502) staff       (20)     7566 2019-07-15 06:36:08.000000 pyrtl-0.8.7/tests/test_inputoutput.py
--rw-r--r--   0 sherwood   (502) staff       (20)     3555 2018-01-09 19:19:27.000000 pyrtl-0.8.7/tests/test_estimate.py
--rw-r--r--   0 sherwood   (502) staff       (20)      735 2015-12-28 17:58:05.000000 pyrtl-0.8.7/tests/test_examples.py
--rw-r--r--   0 sherwood   (502) staff       (20)     6822 2019-07-15 06:36:08.000000 pyrtl-0.8.7/README.md
--rw-r--r--   0 sherwood   (502) staff       (20)     1225 2019-07-15 06:36:08.000000 pyrtl-0.8.7/setup.py
--rw-r--r--   0 sherwood   (502) staff       (20)      245 2019-07-15 06:48:55.000000 pyrtl-0.8.7/setup.cfg
+drwxr-xr-x   0 sherwood   (501) staff       (20)        0 2021-03-06 02:01:39.000000 pyrtl-0.9.0/
+-rw-r--r--   0 sherwood   (501) staff       (20)     1010 2021-03-06 02:01:39.000000 pyrtl-0.9.0/PKG-INFO
+drwxr-xr-x   0 sherwood   (501) staff       (20)        0 2021-03-06 02:01:39.000000 pyrtl-0.9.0/PyRTL.egg-info/
+-rw-r--r--   0 sherwood   (501) staff       (20)     1010 2021-03-06 02:01:38.000000 pyrtl-0.9.0/PyRTL.egg-info/PKG-INFO
+-rw-r--r--   0 sherwood   (501) staff       (20)     1192 2021-03-06 02:01:38.000000 pyrtl-0.9.0/PyRTL.egg-info/SOURCES.txt
+-rw-r--r--   0 sherwood   (501) staff       (20)        1 2021-03-06 02:01:38.000000 pyrtl-0.9.0/PyRTL.egg-info/dependency_links.txt
+-rw-r--r--   0 sherwood   (501) staff       (20)       30 2021-03-06 02:01:38.000000 pyrtl-0.9.0/PyRTL.egg-info/requires.txt
+-rw-r--r--   0 sherwood   (501) staff       (20)       12 2021-03-06 02:01:38.000000 pyrtl-0.9.0/PyRTL.egg-info/top_level.txt
+-rw-r--r--   0 sherwood   (501) staff       (20)     6822 2019-07-15 06:36:08.000000 pyrtl-0.9.0/README.md
+drwxr-xr-x   0 sherwood   (501) staff       (20)        0 2021-03-06 02:01:39.000000 pyrtl-0.9.0/pyrtl/
+-rw-r--r--   0 sherwood   (501) staff       (20)     3663 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/__init__.py
+drwxr-xr-x   0 sherwood   (501) staff       (20)        0 2021-03-06 02:01:39.000000 pyrtl-0.9.0/pyrtl/analysis/
+-rw-r--r--   0 sherwood   (501) staff       (20)      114 2016-06-28 00:17:17.000000 pyrtl-0.9.0/pyrtl/analysis/__init__.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    16451 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/analysis/estimate.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    34022 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/compilesim.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    11290 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/conditional.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    43332 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/core.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    28509 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/corecircuits.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    37948 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/helperfuncs.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    32631 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/inputoutput.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    16010 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/memory.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    22933 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/passes.py
+-rw-r--r--   0 sherwood   (501) staff       (20)      467 2015-10-11 05:04:13.000000 pyrtl-0.9.0/pyrtl/pyrtlexceptions.py
+drwxr-xr-x   0 sherwood   (501) staff       (20)        0 2021-03-06 02:01:39.000000 pyrtl-0.9.0/pyrtl/rtllib/
+-rw-r--r--   0 sherwood   (501) staff       (20)        0 2015-10-11 05:04:13.000000 pyrtl-0.9.0/pyrtl/rtllib/__init__.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    10922 2020-11-10 02:13:05.000000 pyrtl-0.9.0/pyrtl/rtllib/adders.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    19965 2020-11-10 02:13:05.000000 pyrtl-0.9.0/pyrtl/rtllib/aes.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     1834 2019-07-15 06:36:08.000000 pyrtl-0.9.0/pyrtl/rtllib/barrel.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     3005 2020-11-10 02:13:05.000000 pyrtl-0.9.0/pyrtl/rtllib/libutils.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     9951 2020-11-10 02:13:05.000000 pyrtl-0.9.0/pyrtl/rtllib/multipliers.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     7262 2020-11-10 02:13:05.000000 pyrtl-0.9.0/pyrtl/rtllib/muxes.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    11274 2019-07-15 06:36:08.000000 pyrtl-0.9.0/pyrtl/rtllib/prngs.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     5460 2020-11-10 02:13:05.000000 pyrtl-0.9.0/pyrtl/rtllib/testingutils.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    51389 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/simulation.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     9411 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/transform.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    15577 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/verilog.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    29766 2021-03-06 01:47:40.000000 pyrtl-0.9.0/pyrtl/wire.py
+-rw-r--r--   0 sherwood   (501) staff       (20)      234 2021-03-06 02:01:39.000000 pyrtl-0.9.0/setup.cfg
+-rw-r--r--   0 sherwood   (501) staff       (20)     1225 2021-03-06 01:59:19.000000 pyrtl-0.9.0/setup.py
+drwxr-xr-x   0 sherwood   (501) staff       (20)        0 2021-03-06 02:01:39.000000 pyrtl-0.9.0/tests/
+-rw-r--r--   0 sherwood   (501) staff       (20)        0 2015-10-11 05:04:13.000000 pyrtl-0.9.0/tests/__init__.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    39810 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_compilesim.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    18121 2020-11-10 02:13:05.000000 pyrtl-0.9.0/tests/test_conditional.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    25869 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_core.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     3588 2020-11-10 02:13:05.000000 pyrtl-0.9.0/tests/test_estimate.py
+-rw-r--r--   0 sherwood   (501) staff       (20)      737 2020-11-10 02:13:05.000000 pyrtl-0.9.0/tests/test_examples.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    41226 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_helperfuncs.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    16508 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_inputoutput.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    15450 2020-11-10 02:13:05.000000 pyrtl-0.9.0/tests/test_memblock.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    23560 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_passes.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     7541 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_signed.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    47165 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_simulation.py
+-rw-r--r--   0 sherwood   (501) staff       (20)     7101 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_transform.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    18940 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_verilog.py
+-rw-r--r--   0 sherwood   (501) staff       (20)    12110 2021-03-06 01:47:40.000000 pyrtl-0.9.0/tests/test_wire.py
```

### Comparing `pyrtl-0.8.7/PKG-INFO` & `pyrtl-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyrtl
-Version: 0.8.7
+Version: 0.9.0
 Summary: RTL-level Hardware Design and Simulation Toolkit
 Home-page: http://ucsbarchlab.github.io/PyRTL/
 Author: Timothy Sherwood, John Clow, and UCSBarchlab
 Author-email: sherwood@cs.ucsb.edu
 License: UNKNOWN
-Download-URL: https://github.com/UCSBarchlab/PyRTL/tarball/0.8.7
-Description-Content-Type: UNKNOWN
+Download-URL: https://github.com/UCSBarchlab/PyRTL/tarball/0.9.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -19,7 +18,8 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: System :: Hardware
+Provides-Extra: blif parsing
```

### Comparing `pyrtl-0.8.7/pyrtl/simulation.py` & `pyrtl-0.9.0/pyrtl/simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numbers
 import collections
 
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
 from .core import working_block, PostSynthBlock, _PythonSanitizer
 from .wire import Input, Register, Const, Output, WireVector
 from .memory import RomBlock
-from .helperfuncs import check_rtl_assertions, _currently_in_ipython
+from .helperfuncs import check_rtl_assertions, _currently_in_jupyter_notebook
 from .verilog import _VerilogSanitizer
 
 # ----------------------------------------------------------------
 #    __                         ___    __
 #   /__` |  |\/| |  | |     /\   |  | /  \ |\ |
 #   .__/ |  |  | \__/ |___ /~~\  |  | \__/ | \|
 #
@@ -57,15 +57,15 @@
 
         :param tracer: an instance of SimulationTrace used to store execution results.
             Defaults to a new SimulationTrace with no params passed to it.  If None is
             passed, no tracer is instantiated (which is good for long running simulations).
             If the default (true) is passed, Simulation will create a new tracer automatically
             which can be referenced by the member variable .tracer
         :param register_value_map: Defines the initial value for
-          the roms specified. Format: {Register: value}.
+          the registers specified. Format: {Register: value}.
         :param memory_value_map: Defines initial values for many
           addresses in a single or multiple memory. Format: {Memory: {address: Value}}.
           Memory is a memory block, address is the address of a value
         :param default_value: is the value that all unspecified registers and
           memories will initialize to. If no default_value is specified, it will
           use the value stored in the object (default to 0)
         :param block: the hardware block to be traced (which might be of type PostSynthesisBlock).
@@ -175,20 +175,20 @@
                 raise PyrtlError(
                     'step provided a value for input for "%s" which is '
                     'not a known input ' % name)
             if not isinstance(provided_inputs[i], numbers.Integral) or provided_inputs[i] < 0:
                 raise PyrtlError(
                     'step provided an input "%s" which is not a valid '
                     'positive integer' % provided_inputs[i])
-            if len(bin(provided_inputs[i]))-2 > sim_wire.bitwidth:
+            if len(bin(provided_inputs[i])) - 2 > sim_wire.bitwidth:
                 raise PyrtlError(
                     'the bitwidth for "%s" is %d, but the provided input '
                     '%d requires %d bits to represent'
                     % (name, sim_wire.bitwidth,
-                       provided_inputs[i], len(bin(provided_inputs[i]))-2))
+                       provided_inputs[i], len(bin(provided_inputs[i])) - 2))
 
             self.value[sim_wire] = provided_inputs[i]
             supplied_inputs.add(sim_wire)
 
         # Check that only inputs are specified, and set the values
         if input_set != supplied_inputs:
             for i in input_set.difference(supplied_inputs):
@@ -213,22 +213,135 @@
             argval = self.value[net.args[0]]
             self.regvalue[net.dests[0]] = self._sanitize(argval, net.dests[0])
 
         # finally, if any of the rtl_assert assertions are failing then we should
         # raise the appropriate exceptions
         check_rtl_assertions(self)
 
+    def step_multiple(self, provided_inputs={}, expected_outputs={}, nsteps=None,
+                      file=sys.stdout, stop_after_first_error=False):
+        """ Take the simulation forward N cycles, where N is the number of values
+         for each provided input.
+
+        :param provided_inputs: a dictionary mapping wirevectors to their values for N steps
+        :param expected_outputs: a dictionary mapping wirevectors to their expected values
+            for N steps
+        :param nsteps: number of steps to take (defaults to None, meaning step for each
+            supplied input value)
+        :param file: where to write the output (if there are unexpected outputs detected)
+        :param stop_after_first_error: a boolean flag indicating whether to stop the simulation
+            after encountering the first error (defaults to False)
+
+        All input wires must be in the provided_inputs in order for the simulation
+        to accept these values. Additionally, the length of the array of provided values for each
+        input must be the same.
+
+        When 'nsteps' is specified, then it must be *less than or equal* to the number of values
+        supplied for each input when 'provided_inputs' is non-empty. When 'provided_inputs' is
+        empty (which may be a legitimate case for a design that takes no inputs), then 'nsteps'
+        will be used.  When 'nsteps' is not specified, then the simulation will take the number
+        of steps equal to the number of values supplied for each input.
+
+        Example: if we have inputs named 'a' and 'b' and output 'o', we can call:
+        sim.step_multiple({'a': [0,1], 'b': [23,32]}, {'o': [42, 43]}) to simulate 2 cycles,
+        where in the first cycle 'a' and 'b' take on 0 and 23, respectively, and 'o' is expected to
+        have the value 42, and in the second cycle 'a' and 'b' take on 1 and 32, respectively, and
+        'o' is expected to have the value 43.
+
+        If your values are all single digit, you can also specify them in a single string, e.g.
+        sim.step_multiple({'a': '01', 'b': '01'}) will simulate 2 cycles, with 'a' and 'b' taking on
+        0 and 0, respectively, on the first cycle and '1' and '1', respectively, on the second
+        cycle.
+
+        Example: if the design had no inputs, like so:
+
+            a = pyrtl.Register(8)
+            b = pyrtl.Output(8, 'b')
+
+            a.next <<= a + 1
+            b <<= a
+
+            sim = pyrtl.Simulation()
+            sim.step_multiple(nsteps=3)
+
+        Using sim.step_multiple(nsteps=3) simulates 3 cycles, after which we would expect the value
+        of 'b' to be 2.
+
+        """
+
+        if not nsteps and len(provided_inputs) == 0:
+            raise PyrtlError('need to supply either input values or a number of steps to simulate')
+
+        if len(provided_inputs) > 0:
+            longest = sorted(list(provided_inputs.items()),
+                             key=lambda t: len(t[1]),
+                             reverse=True)[0]
+            msteps = len(longest[1])
+            if nsteps:
+                if (nsteps > msteps):
+                    raise PyrtlError('nsteps is specified but is greater than the '
+                                     'number of values supplied for each input')
+            else:
+                nsteps = msteps
+
+        if nsteps < 1:
+            raise PyrtlError("must simulate at least one step")
+
+        if list(filter(lambda l: len(l) < nsteps, provided_inputs.values())):
+            raise PyrtlError(
+                "must supply a value for each provided wire "
+                "for each step of simulation")
+
+        if list(filter(lambda l: len(l) < nsteps, expected_outputs.values())):
+            raise PyrtlError(
+                "any expected outputs must have a supplied value "
+                "each step of simulation")
+
+        failed = []
+        for i in range(nsteps):
+            self.step({w: int(v[i]) for w, v in provided_inputs.items()})
+
+            for expvar in expected_outputs.keys():
+                expected = int(expected_outputs[expvar][i])
+                actual = self.inspect(expvar)
+                if expected != actual:
+                    failed.append((i, expvar, expected, actual))
+
+            if failed and stop_after_first_error:
+                break
+
+        if failed:
+            if stop_after_first_error:
+                s = "(stopped after step with first error):"
+            else:
+                s = "on one or more steps:"
+            file.write("Unexpected output " + s + "\n")
+            file.write("{0:>5} {1:>10} {2:>8} {3:>8}\n"
+                       .format("step", "name", "expected", "actual"))
+
+            def _sort_tuple(t):
+                # Sort by step and then wire name
+                return (t[0], _trace_sort_key(t[1]))
+
+            failed_sorted = sorted(failed, key=_sort_tuple)
+            for (step, name, expected, actual) in failed_sorted:
+                file.write("{0:>5} {1:>10} {2:>8} {3:>8}\n".format(step, name, expected, actual))
+            file.flush()
+
     def inspect(self, w):
         """ Get the value of a wirevector in the last simulation cycle.
 
         :param w: the name of the WireVector to inspect
             (passing in a WireVector instead of a name is deprecated)
         :return: value of w in the current step of simulation
 
         Will throw KeyError if w does not exist in the simulation.
+
+        Examples ::
+            sim.inspect('a') == 10  # returns value of wire 'a' at current step
         """
         wire = self.block.wirevector_by_name.get(w, w)
         return self.value[wire]
 
     def inspect_mem(self, mem):
         """ Get the values in a map during the current simulation cycle.
 
@@ -307,15 +420,15 @@
 #    ___       __  ___     __
 #   |__   /\  /__`  |     /__` |  |\/|
 #   |    /~~\ .__/  |     .__/ |  |  |
 #
 
 
 class FastSimulation(object):
-    """A class for running JIT implementations of blocks.
+    """A class for running JIT-to-python implementations of blocks.
     """
 
     # Dev Notes:
     #  Wire name processing:
     #  Sanitized names are only used when using and assigning variables inside of
     #  the generated function. Normal names are used when interacting with
     #  the dictionaries passed in and created by the exec'ed function.
@@ -431,14 +544,124 @@
         self.context.update(ins)  # also gets old register values
         if self.tracer is not None:
             self.tracer.add_fast_step(self)
 
         # check the rtl assertions
         check_rtl_assertions(self)
 
+    def step_multiple(self, provided_inputs={}, expected_outputs={}, nsteps=None,
+                      file=sys.stdout, stop_after_first_error=False):
+        """ Take the simulation forward N cycles, where N is the number of values
+         for each provided input.
+
+        :param provided_inputs: a dictionary mapping wirevectors to their values for N steps
+        :param expected_outputs: a dictionary mapping wirevectors to their expected values
+            for N steps
+        :param nsteps: number of steps to take (defaults to None, meaning step for each
+            supplied input value)
+        :param file: where to write the output (if there are unexpected outputs detected)
+        :param stop_after_first_error: a boolean flag indicating whether to stop the simulation
+            after the step where the first errors are encountered (defaults to False)
+
+        All input wires must be in the provided_inputs in order for the simulation
+        to accept these values. Additionally, the length of the array of provided values for each
+        input must be the same.
+
+        When 'nsteps' is specified, then it must be *less than or equal* to the number of values
+        supplied for each input when 'provided_inputs' is non-empty. When 'provided_inputs' is
+        empty (which may be a legitimate case for a design that takes no inputs), then 'nsteps'
+        will be used.  When 'nsteps' is not specified, then the simulation will take the number
+        of steps equal to the number of values supplied for each input.
+
+        Example: if we have inputs named 'a' and 'b' and output 'o', we can call:
+        sim.step_multiple({'a': [0,1], 'b': [23,32]}, {'o': [42, 43]}) to simulate 2 cycles,
+        where in the first cycle 'a' and 'b' take on 0 and 23, respectively, and 'o' is expected to
+        have the value 42, and in the second cycle 'a' and 'b' take on 1 and 32, respectively, and
+        'o' is expected to have the value 43.
+
+        If your values are all single digit, you can also specify them in a single string, e.g.
+        sim.step_multiple({'a': '01', 'b': '01'}) will simulate 2 cycles, with 'a' and 'b' taking on
+        0 and 0, respectively, on the first cycle and '1' and '1', respectively, on the second
+        cycle.
+
+        Example: if the design had no inputs, like so:
+
+            a = pyrtl.Register(8)
+            b = pyrtl.Output(8, 'b')
+
+            a.next <<= a + 1
+            b <<= a
+
+            sim = pyrtl.Simulation()
+            sim.step_multiple(nsteps=3)
+
+        Using sim.step_multiple(nsteps=3) simulates 3 cycles, after which we would expect the value
+        of 'b' to be 2.
+
+        """
+
+        if not nsteps and len(provided_inputs) == 0:
+            raise PyrtlError('need to supply either input values or a number of steps to simulate')
+
+        if len(provided_inputs) > 0:
+            longest = sorted(list(provided_inputs.items()),
+                             key=lambda t: len(t[1]),
+                             reverse=True)[0]
+            msteps = len(longest[1])
+            if nsteps:
+                if (nsteps > msteps):
+                    raise PyrtlError('nsteps is specified but is greater than the '
+                                     'number of values supplied for each input')
+            else:
+                nsteps = msteps
+
+        if nsteps < 1:
+            raise PyrtlError("must simulate at least one step")
+
+        if list(filter(lambda l: len(l) < nsteps, provided_inputs.values())):
+            raise PyrtlError(
+                "must supply a value for each provided wire "
+                "for each step of simulation")
+
+        if list(filter(lambda l: len(l) < nsteps, expected_outputs.values())):
+            raise PyrtlError(
+                "any expected outputs must have a supplied value "
+                "each step of simulation")
+
+        failed = []
+        for i in range(nsteps):
+            self.step({w: int(v[i]) for w, v in provided_inputs.items()})
+
+            for expvar in expected_outputs.keys():
+                expected = int(expected_outputs[expvar][i])
+                actual = self.inspect(expvar)
+                if expected != actual:
+                    failed.append((i, expvar, expected, actual))
+
+            if failed and stop_after_first_error:
+                break
+
+        if failed:
+            if stop_after_first_error:
+                s = "(stopped after step with first error):"
+            else:
+                s = "on one or more steps:"
+            file.write("Unexpected output " + s + "\n")
+            file.write("{0:>5} {1:>10} {2:>8} {3:>8}\n"
+                       .format("step", "name", "expected", "actual"))
+
+            def _sort_tuple(t):
+                # Sort by step and then wire name
+                return (t[0], _trace_sort_key(t[1]))
+
+            failed_sorted = sorted(failed, key=_sort_tuple)
+            for (step, name, expected, actual) in failed_sorted:
+                file.write("{0:>5} {1:>10} {2:>8} {3:>8}\n".format(step, name, expected, actual))
+            file.flush()
+
     def inspect(self, w):
         """ Get the value of a wirevector in the last simulation cycle.
 
         :param w: the name of the WireVector to inspect
             (passing in a WireVector instead of a name is deprecated)
         :return: value of w in the current step of simulation
 
@@ -483,15 +706,15 @@
     def _arg_varname(self, wire):
         """
         Input, Const, and Registers have special input values
         """
         if isinstance(wire, (Input, Register)):
             return 'd[' + repr(wire.name) + ']'  # passed in
         elif isinstance(wire, Const):
-            return str(wire.val)  # hardcoded
+            return str(int(wire.val))  # hardcoded
         else:
             return self._varname(wire)
 
     def _dest_varname(self, wire):
         if isinstance(wire, Output):
             return 'outs[' + repr(wire.name) + ']'
         elif isinstance(wire, Register):
@@ -524,15 +747,15 @@
     _prog_start = """def sim_func(d):
     regs = {}
     outs = {}
     mem_ws = []"""
 
     def _compiled(self):
         """Return a string of the self.block compiled to a block of
-         code that can be execed to get a function to execute"""
+         code that can be executed to get a function to execute"""
         # Dev Notes:
         # Because of fast locals in functions in both CPython and PyPy, getting a
         # function to execute makes the code a few times faster than
         # just executing it in the global exec scope.
         prog = [self._prog_start]
 
         simple_func = {  # OPS
@@ -570,17 +793,17 @@
         for net in self.block:
             if net.op in simple_func:
                 argvals = (self._arg_varname(arg) for arg in net.args)
                 expr = simple_func[net.op](*argvals)
             elif net.op == 'c':
                 expr = ''
                 for i in range(len(net.args)):
-                    if expr is not '':
+                    if expr != '':
                         expr += ' | '
-                    shiftby = sum(len(j) for j in net.args[i+1:])
+                    shiftby = sum(len(j) for j in net.args[i + 1:])
                     expr += shift(self._arg_varname(net.args[i]), '<<', shiftby)
             elif net.op == 's':
                 source = self._arg_varname(net.args[0])
                 expr = ''
                 split_length = 0
                 split_start_bit = -2
                 split_res_start_bit = -1
@@ -622,17 +845,17 @@
                 mask = str(net.dests[0].bitmask)
                 prog.append('    %s = %s & %s' % (result, mask, expr))
 
         # add traced wires to dict
         if self.tracer is not None:
             for wire_name in self.tracer.trace:
                 wire = self.block.wirevector_by_name[wire_name]
-                if not isinstance(wire, (Input, Const, Register, Output)):
-                    v_wire_name = self._varname(wire)
-                    prog.append('    outs["%s"] = %s' % (wire_name, v_wire_name))
+                if not isinstance(wire, (Input, Register, Output)):
+                    value = int(wire.val) if isinstance(wire, Const) else self._varname(wire)
+                    prog.append('    outs["%s"] = %s' % (wire_name, value))
 
         prog.append("    return regs, outs, mem_ws")
         return '\n'.join(prog)
 
 
 # ----------------------------------------------------------------
 #    ___  __        __   ___
@@ -669,23 +892,23 @@
         :param current_val: the value to be rendered
         :param symbol_len: and integer for how big to draw the current value
 
         Returns a string of printed length symbol_len that will draw the
         representation of current_val.  The input prior_val is used to
         render transitions.
         """
-        sl = symbol_len-1
+        sl = symbol_len - 1
         if len(w) > 1:
             out = self._revstart
             if current_val != self.prior_val:
                 out += self._x + hex(current_val).rstrip('L').ljust(sl)[:sl]
             elif n == 0:
                 out += hex(current_val).rstrip('L').ljust(symbol_len)[:symbol_len]
             else:
-                out += ' '*symbol_len
+                out += ' ' * symbol_len
             out += self._revstop
         else:
             pretty_map = {
                 (0, 0): self._low + self._low * sl,
                 (0, 1): self._up + self._high * sl,
                 (1, 0): self._down + self._low * sl,
                 (1, 1): self._high + self._high * sl,
@@ -744,36 +967,38 @@
         if isinstance(key, WireVector):
             import warnings
             warnings.warn(
                 'Access to trace by WireVector instead of name is deprecated.',
                 DeprecationWarning)
             key = key.name
         if key not in self.__data:
-            raise PyrtlError('cannot find "%s" in trace -- if using CompiledSim you make be '
-                             'attempting to access internal states but only inputs/output are '
+            raise PyrtlError('Cannot find "%s" in trace -- if using CompiledSim, you may be '
+                             'attempting to access internal states but only inputs/outputs are '
                              'available.' % key)
         return self.__data[key]
 
 
 class SimulationTrace(object):
     """ Storage and presentation of simulation waveforms. """
 
     def __init__(self, wires_to_track=None, block=None):
         """
         Creates a new Simulation Trace
 
-        :param wires_to_track: The wires that the tracer should track
-        :param block:
+        :param wires_to_track: The wires that the tracer should track.
+            If unspecified, will track all explicitly-named wires.
+            If set to 'all', will track all wires, including internal wires.
+        :param block: Block containing logic to trace
         """
         self.block = working_block(block)
 
         def is_internal_name(name):
-            return (name.startswith('tmp') or name.startswith('const') or
+            return (name.startswith('tmp') or name.startswith('const_')
                     # or name.startswith('synth_')
-                    name.endswith("'"))
+                    or name.endswith("'"))
 
         if wires_to_track is None:
             wires_to_track = [w for w in self.block.wirevector_set if not is_internal_name(w.name)]
         elif wires_to_track == 'all':
             wires_to_track = self.block.wirevector_set
 
         if not len(wires_to_track):
@@ -843,20 +1068,20 @@
     def print_vcd(self, file=sys.stdout, include_clock=False):
         """ Print the trace out as a VCD File for use in other tools.
 
         :param file: file to open and output vcd dump to.
         :param include_clock: boolean specifying if the implicit clk should be included.
 
         Dumps the current trace to file as a "value change dump" file.  The file parameter
-        defaults to _stdout_ and the include_clock defaults to True.
+        defaults to _stdout_ and the include_clock defaults to False.
 
         Examples ::
 
             sim_trace.print_vcd()
-            sim_trace.print_vcd("my_waveform.vcd", include_clock=False)
+            sim_trace.print_vcd("my_waveform.vcd", include_clock=True)
         """
         # dump header info
         # file_timestamp = time.strftime("%a, %d %b %Y %H:%M:%S (UTC/GMT)", time.gmtime())
         # print >>file, " ".join(["$date", file_timestamp, "$end"])
         self.internal_names = _VerilogSanitizer('_vcd_tmp_')
         for wire in self.wires_to_track:
             self.internal_names.make_valid_string(wire.name)
@@ -883,45 +1108,44 @@
         print(' '.join(['$dumpvars']), file=file)
         print_trace_strs(0)
         print(' '.join(['$end']), file=file)
 
         # dump values
         endtime = max([len(self.trace[w]) for w in self.trace])
         for timestamp in range(endtime):
-            print(''.join(['#', str(timestamp*10)]), file=file)
+            print(''.join(['#', str(timestamp * 10)]), file=file)
             print_trace_strs(timestamp)
             if include_clock:
                 print('b1 clk', file=file)
                 print('', file=file)
-                print(''.join(['#', str(timestamp*10+5)]), file=file)
+                print(''.join(['#', str(timestamp * 10 + 5)]), file=file)
                 print('b0 clk', file=file)
             print('', file=file)
-        print(''.join(['#', str(endtime*10)]), file=file)
+        print(''.join(['#', str(endtime * 10)]), file=file)
         file.flush()
 
     def render_trace(
             self, trace_list=None, file=sys.stdout, render_cls=default_renderer(),
             symbol_len=5, segment_size=5, segment_delim=' ', extra_line=True):
 
         """ Render the trace to a file using unicode and ASCII escape sequences.
 
-        :param trace_list: A list of signals to be output in the specified order.
+        :param trace_list: A list of signal names to be output in the specified order.
         :param file: The place to write output, default to stdout.
         :param render_cls: A class that translates traces into output bytes.
         :param symbol_len: The "length" of each rendered cycle in characters.
         :param segment_size: Traces are broken in the segments of this number of cycles.
         :param segment_delim: The character to be output between segments.
-        :param extra_line: A Boolean to determin if we should print a blank line between signals.
+        :param extra_line: A Boolean to determine if we should print a blank line between signals.
 
         The resulting output can be viewed directly on the terminal or looked
         at with "more" or "less -R" which both should handle the ASCII escape
-        sequences used in rendering. render_trace takes the following optional
-        arguments.
+        sequences used in rendering.
         """
-        if _currently_in_ipython():
+        if _currently_in_jupyter_notebook():
             from IPython.display import display, HTML, Javascript  # pylint: disable=import-error
             from .inputoutput import trace_to_html
             htmlstring = trace_to_html(self, trace_list=trace_list, sortkey=_trace_sort_key)
             html_elem = HTML(htmlstring)
             display(html_elem)
             # print(htmlstring)
             js_stuff = """
@@ -965,22 +1189,28 @@
         elif any(isinstance(x, WireVector) for x in trace_list):
             import warnings
             warnings.warn(
                 'Access to trace by WireVector instead of name is deprecated.',
                 DeprecationWarning)
             trace_list = [getattr(x, 'name', x) for x in trace_list]
 
+        if not trace_list:
+            raise PyrtlError(
+                "Empty trace list. This may have occurred because "
+                "untraceable wires were removed prior to simulation, "
+                "if a CompiledSimulation was used.")
+
         # print the 'ruler' which is just a list of 'ticks'
         # mapped by the pretty map
 
-        maxnamelen = max(len(w) for w in self.trace)
+        maxnamelen = max(len(w) for w in trace_list)
         maxtracelen = max(len(v) for v in self.trace.values())
         if segment_size is None:
             segment_size = maxtracelen
-        spaces = ' '*(maxnamelen+1)
+        spaces = ' ' * (maxnamelen + 1)
         ticks = [renderer.tick_segment(n, symbol_len, segment_size)
                  for n in range(0, maxtracelen, segment_size)]
         print(spaces + segment_delim.join(ticks), file=file)
 
         # now all the traces
         for w in trace_list:
             if extra_line:
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/multipliers.py` & `pyrtl-0.9.0/pyrtl/rtllib/multipliers.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,23 +106,23 @@
     """ returns a WireVector sum of rem_bits multiplies (in one clock cycle)
     note: this method requires a lot of area because of the indexing in the else statement """
     if rem_bits == 0:
         return sum_sf
     else:
         a_curr_val = areg[curr_bit].sign_extended(len(breg))
         if curr_bit == 0:  # if no shift
-            return(_one_cycle_mult(areg, breg, rem_bits-1,  # areg, breg, rem_bits
+            return(_one_cycle_mult(areg, breg, rem_bits - 1,  # areg, breg, rem_bits
                                    sum_sf + (a_curr_val & breg),  # sum_sf
-                                   curr_bit+1))  # curr_bit
+                                   curr_bit + 1))  # curr_bit
         else:
             return _one_cycle_mult(
-                areg, breg, rem_bits-1,  # areg, breg, rem_bits
-                sum_sf + (a_curr_val &
-                          pyrtl.concat(breg, pyrtl.Const(0, curr_bit))),  # sum_sf
-                curr_bit+1  # curr_bit
+                areg, breg, rem_bits - 1,  # areg, breg, rem_bits
+                sum_sf + (a_curr_val
+                          & pyrtl.concat(breg, pyrtl.Const(0, curr_bit))),  # sum_sf
+                curr_bit + 1  # curr_bit
             )
 
 
 def tree_multiplier(A, B, reducer=adders.wallace_reducer, adder_func=adders.kogge_stone):
     """ Build an fast unclocked multiplier for inputs A and B using a Wallace or Dada Tree.
 
     :param WireVector A, B: two input wires for the multiplication
@@ -249,10 +249,10 @@
                 bits[i + j].append(a & b)
 
     for wire in add_wires:
         for bit_loc, bit in enumerate(wire):
             bits[bit_loc].append(bit)
 
     import math
-    result_bitwidth = (longest_wire_len +
-                       int(math.ceil(math.log(len(add_wires) + len(mult_pairs), 2))))
+    result_bitwidth = (longest_wire_len
+                       + int(math.ceil(math.log(len(add_wires) + len(mult_pairs), 2))))
     return reducer(bits, result_bitwidth, adder_func)
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/aes.py` & `pyrtl-0.9.0/pyrtl/rtllib/aes.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,18 +240,18 @@
         subbed = [self.inv_sbox[byte] if inverse else self.sbox[byte]
                   for byte in libutils.partition_wire(in_vector, 8)]
         return pyrtl.concat_list(subbed)
 
     @staticmethod
     def _inv_shift_rows(in_vector):
         a = libutils.partition_wire(in_vector, 8)
-        return pyrtl.concat_list((a[12], a[9],  a[6],  a[3],
-                                  a[0],  a[13], a[10], a[7],
-                                  a[4],  a[1],  a[14], a[11],
-                                  a[8],  a[5],  a[2],  a[15]))
+        return pyrtl.concat_list((a[12], a[9], a[6], a[3],
+                                  a[0], a[13], a[10], a[7],
+                                  a[4], a[1], a[14], a[11],
+                                  a[8], a[5], a[2], a[15]))
 
     @staticmethod
     def _shift_rows(in_vector):
         a = libutils.partition_wire(in_vector, 8)
         return pyrtl.concat_list((a[4], a[9], a[14], a[3],
                                   a[8], a[13], a[2], a[7],
                                   a[12], a[1], a[6], a[11],
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/muxes.py` & `pyrtl-0.9.0/pyrtl/rtllib/muxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     else:
         half = len(vals) // 2
         return pyrtl.select(pyrtl.rtl_any(*selects[:half]),
                             truecase=prioritized_mux(selects[:half], vals[:half]),
                             falsecase=prioritized_mux(selects[half:], vals[half:]))
 
 
-def _is_equivelent(w1, w2):
+def _is_equivalent(w1, w2):
     if isinstance(w1, pyrtl.Const) & isinstance(w2, pyrtl.Const):
         return (w1.val == w2.val) & (w1.bitwidth == w2.bitwidth)
     return w1 is w2
 
 
 SparseDefault = "default"
 
@@ -91,23 +91,23 @@
         except KeyError:
             raise pyrtl.PyrtlError("Failed to retrieve values for smartmux. "
                                    "The length of sel might be wrong")
     else:
         half = 2**(len(sel) - 1)
 
         first_dict = {indx: wire for indx, wire in vals.items() if indx < half}
-        second_dict = {indx-half: wire for indx, wire in vals.items() if indx >= half}
+        second_dict = {indx - half: wire for indx, wire in vals.items() if indx >= half}
         if not len(first_dict):
             return sparse_mux(sel[:-1], second_dict)
         if not len(second_dict):
             return sparse_mux(sel[:-1], first_dict)
 
         false_result = sparse_mux(sel[:-1], first_dict)
         true_result = sparse_mux(sel[:-1], second_dict)
-    if _is_equivelent(false_result, true_result):
+    if _is_equivalent(false_result, true_result):
         return true_result
     return pyrtl.select(sel[-1], falsecase=false_result, truecase=true_result)
 
 
 class MultiSelector(object):
     """
     The MultiSelector allows you to specify multiple wire value results
@@ -123,15 +123,15 @@
         ms.option(val1, data0, data1, data2, ...)
         ms.option(val2, data0_2, data1_2, data2_2, ...)
 
     This means that when the select wire equals the val1 wire
     the results will have the values in the coresponding data wires
     (all ints are converted to wires)
     """
-    def __init__(self, signal_wire,  *dest_wires):
+    def __init__(self, signal_wire, *dest_wires):
         self._final = False
         self.dest_wires = dest_wires
         self.signal_wire = signal_wire
         self.instructions = []
         self.dest_instrs_info = {dest_w: [] for dest_w in dest_wires}
 
     def __enter__(self):
@@ -149,15 +149,15 @@
 
     def _check_finalized(self):
         if self._final:
             raise pyrtl.PyrtlError("Cannot change InstrConnector, already finalized")
 
     def option(self, select_val, *data_signals):
         self._check_finalized()
-        instr, ib = pyrtl.wire._gen_val_and_bitwidth(select_val, self.signal_wire.bitwidth)
+        instr, ib = pyrtl.infer_val_and_bitwidth(select_val, self.signal_wire.bitwidth)
         if instr in self.instructions:
             raise pyrtl.PyrtlError("instruction %s already exists" % str(select_val))
         self.instructions.append(instr)
         self._add_signal(data_signals)
 
     def default(self, *data_signals):
         self._check_finalized()
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/testingutils.py` & `pyrtl-0.9.0/pyrtl/rtllib/testingutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     else:
         raise pyrtl.PyrtlError("A max or exact bitwidth must be specified")
     return min_bitwidth, max_bitwidth
 
 
 def inverse_power_dist(bitwidth):
     # Note that this is not uniformly distributed
-    return int(2**random.uniform(0, bitwidth)-1)
+    return int(2**random.uniform(0, bitwidth) - 1)
 
 
 def uniform_dist(bitwidth):
     return random.randrange(2**bitwidth)
 
 
 def make_inputs_and_values(num_wires, max_bitwidth=None, exact_bitwidth=None,
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/adders.py` & `pyrtl-0.9.0/pyrtl/rtllib/adders.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     cur_gen = gen[0]
     cur_prop = prop[0]
     for i in range(1, len(prop)):
         cur_gen = gen[i] | (prop[i] & cur_gen)
         cur_prop = cur_prop & prop[i]
         sum_bit = pyrtl.concat(prop[i] ^ carry[i - 1], sum_bit)
-        carry.append(gen[i] | (prop[i] & carry[i-1]))
+        carry.append(gen[i] | (prop[i] & carry[i - 1]))
     cout = cur_gen | (cur_prop & cin)
     return sum_bit, cout
 
 
 def wallace_reducer(wire_array_2, result_bitwidth, final_adder=kogge_stone):
     """
     The reduction and final adding part of a dada tree. Useful for adding many numbers together
@@ -202,15 +202,15 @@
                 raise pyrtl.PyrtlError(
                     "The item {} is not a valid element for the wire_array_2. "
                     "It must be a WireVector of bitwidth 1".format(a_wire))
 
     max_width = max(len(i) for i in wire_array_2)
     reduction_schedule = [2]
     while reduction_schedule[-1] <= max_width:
-        reduction_schedule.append(int(reduction_schedule[-1]*3/2))
+        reduction_schedule.append(int(reduction_schedule[-1] * 3 / 2))
 
     for reduction_target in reversed(reduction_schedule[:-1]):
         deferred = [[] for weight in range(result_bitwidth + 1)]
         last_round = (max(len(i) for i in wire_array_2) == 3)
         for i, w_array in enumerate(wire_array_2):  # Start with low weights and start reducing
             while len(w_array) + len(deferred[i]) > reduction_target:
                 if len(w_array) + len(deferred[i]) - reduction_target >= 2:
@@ -246,14 +246,15 @@
 
     import six
     wires_to_zip = wire_array_2[single_w_index:]
     add_wires = tuple(six.moves.zip_longest(*wires_to_zip, fillvalue=pyrtl.Const(0)))
     adder_result = adder(pyrtl.concat_list(add_wires[0]), pyrtl.concat_list(add_wires[1]))
     return pyrtl.concat(adder_result, *reversed(result))
 
+
 """
 Some adders that utilize these tree reducers
 """
 
 
 def fast_group_adder(wires_to_add, reducer=wallace_reducer, final_adder=kogge_stone):
     """
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/libutils.py` & `pyrtl-0.9.0/pyrtl/rtllib/libutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,29 +41,29 @@
     """
     correctbw = abs(val).bit_length() + 1
     if bitwidth < correctbw:
         raise pyrtl.PyrtlError("please choose a larger target bitwidth")
     if val >= 0:
         return val
     else:
-        return (~abs(val) & (2**bitwidth-1)) + 1  # flip the bits and add one
+        return (~abs(val) & (2 ** bitwidth - 1)) + 1  # flip the bits and add one
 
 
 def rev_twos_comp_repr(val, bitwidth):
     """
     Takes a two's-complement represented value and
     converts it to a signed integer based on the provided bitwidth.
     For use with Simulation.inspect() etc. when expecting negative numbers,
     which it does not recognize
     """
     valbl = val.bit_length()
-    if bitwidth < val.bit_length() or val == 2**(bitwidth-1):
+    if bitwidth < val.bit_length() or val == 2 ** (bitwidth - 1):
         raise pyrtl.PyrtlError("please choose a larger target bitwidth")
     if bitwidth == valbl:  # MSB is a 1, value is negative
-        return -((~val & (2**bitwidth-1)) + 1)  # flip the bits, add one, and make negative
+        return -((~val & (2 ** bitwidth - 1)) + 1)  # flip the bits, add one, and make negative
     else:
         return val
 
 
 def _shifted_reg_next(reg, direct, num=1):
     """
     Creates a shifted 'next' property for shifted (left or right) register.\n
```

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/barrel.py` & `pyrtl-0.9.0/pyrtl/rtllib/barrel.py`

 * *Files identical despite different names*

### Comparing `pyrtl-0.8.7/pyrtl/rtllib/prngs.py` & `pyrtl-0.9.0/pyrtl/rtllib/prngs.py`

 * *Files identical despite different names*

### Comparing `pyrtl-0.8.7/pyrtl/analysis/estimate.py` & `pyrtl-0.9.0/pyrtl/analysis/estimate.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 from ..core import working_block
 from ..wire import Input, Const, Register
 from ..pyrtlexceptions import PyrtlError, PyrtlInternalError
 from ..verilog import output_to_verilog
 from ..memory import RomBlock
+from ..helperfuncs import _currently_in_jupyter_notebook, _print_netlist_latex
 
 
 # --------------------------------------------------------------------
 #         __   ___          ___  __  ___              ___    __
 #    /\  |__) |__   /\     |__  /__`  |  |  |\/|  /\   |  | /  \ |\ |
 #   /~~\ |  \ |___ /~~\    |___ .__/  |  |  |  | /~~\  |  | \__/ | \|
 #
@@ -67,19 +68,19 @@
         else:
             return -958 + (150 * width) + (45 * width**2)
 
     def stdcell_estimate(net):
         if net.op in 'w~sc':
             return 0
         elif net.op in '&|n':
-            return 40/8.0 * len(net.args[0])   # 40 lambda
+            return 40 / 8.0 * len(net.args[0])   # 40 lambda
         elif net.op in '^=<>x':
-            return 80/8.0 * len(net.args[0])   # 80 lambda
+            return 80 / 8.0 * len(net.args[0])   # 80 lambda
         elif net.op == 'r':
-            return 144/8.0 * len(net.args[0])  # 144 lambda
+            return 144 / 8.0 * len(net.args[0])  # 144 lambda
         elif net.op in '+-':
             return adder_stdcell_estimate(len(net.args[0]))
         elif net.op == '*':
             return multiplier_stdcell_estimate(len(net.args[0]))
         elif net.op in 'm@':
             return 0  # memories handled elsewhere
         else:
@@ -101,15 +102,15 @@
     # first, sum up the area of all of the logic elements (including registers)
     total_tracks = sum(stdcell_estimate(a_net) for a_net in block.logic)
     total_length_in_nm = total_tracks * 8 * 55
     # each track is then 72 lambda tall, and converted from nm2 to mm2
     area_in_mm2_for_130nm = (total_length_in_nm * (72 * 55)) / 1e12
 
     # scaling from 130nm to the target tech
-    logic_area = area_in_mm2_for_130nm / (130.0/tech_in_nm)**2
+    logic_area = area_in_mm2_for_130nm / (130.0 / tech_in_nm) ** 2
 
     # now sum up the area of the memories
     mem_area = 0
     for mem in set(net.op_param[1] for net in block.logic_subset('@m')):
         bits, ports, is_rom = _bits_ports_and_isrom_from_memory(mem)
         mem_area += mem_area_estimate(tech_in_nm, bits, ports, is_rom)
 
@@ -247,23 +248,23 @@
         """
         cp_length = self.max_length()
         scale_factor = 130.0 / tech_in_nm
         if ffoverhead is None:
             clock_period_in_ps = scale_factor * (cp_length + 189 + 194)
         else:
             clock_period_in_ps = (scale_factor * cp_length) + ffoverhead
-        return 1e6 * 1.0/clock_period_in_ps
+        return 1e6 * 1.0 / clock_period_in_ps
 
     def max_length(self):
-        """Returns the max timing delay of the circuit.
+        """Returns the max timing delay of the circuit in ps.
 
         The result assumes that the circuit is implemented in a 130nm process, and that there is no
         setup or hold time associated with the circuit.  The resulting value is in picoseconds.  If
         an proper estimation of timing is required it is recommended to us "max_freq" to determine
-        the clock period as it more accurately consideres scaling and setup/hold.
+        the clock period as it more accurately considers scaling and setup/hold.
         """
         return max(self.timing_map.values())
 
     def print_max_length(self):
         """Prints the max timing delay of the circuit """
         print("The total block timing delay is ", self.max_length())
 
@@ -310,23 +311,26 @@
         if print_cp:
             self.print_critical_paths(critical_paths)
         return critical_paths
 
     @staticmethod
     def print_critical_paths(critical_paths):
         """ Prints the results of the critical path length analysis.
-            Done by default by the `timing_critical_path()` function.
+            Done by default by the `TimingAnalysis().critical_path()` function.
         """
         line_indent = " " * 2
         #  print the critical path
         for cp_with_num in enumerate(critical_paths):
             print("Critical path", cp_with_num[0], ":")
             print(line_indent, "The first wire is:", cp_with_num[1][0])
-            for net in cp_with_num[1][1]:
-                print(line_indent, (net))
+            if _currently_in_jupyter_notebook():
+                _print_netlist_latex(list(net for net in cp_with_num[1][1]))
+            else:
+                for net in cp_with_num[1][1]:
+                    print(line_indent, (net))
             print()
 
 
 # --------------------------------------------------------------------
 #          __   __       __
 #     \ / /  \ /__` \ / /__`
 #      |  \__/ .__/  |  .__/
@@ -344,29 +348,29 @@
     library.  In the standard vsc 130nm library, the area is in a number of
     "tracks", each of which is about 1.74 square um (see area estimation
     for more details) and the delay is in ps.
 
     http://www.vlsitechnology.org/html/vsc_description.html
 
     May raise `PyrtlError` if yosys is not configured correctly, and
-    `PyrtlInternalError` if the call to yosys was not able successfully
+    `PyrtlInternalError` if the call to yosys was not successful
     """
 
     if abc_cmd is None:
         abc_cmd = 'strash;scorr;ifraig;retime;dch,-f;map;print_stats;'
     else:
         # first, replace whitespace with commas as per yosys requirements
         re.sub(r"\s+", ',', abc_cmd)
         # then append with "print_stats" to generate the area and delay info
         abc_cmd = '%s;print_stats;' % abc_cmd
 
     def extract_area_delay_from_yosys_output(yosys_output):
         report_lines = [line for line in yosys_output.split('\n') if 'ABC: netlist' in line]
-        area = re.match('.*area\s*=\s*([0-9\.]*)', report_lines[0]).group(1)
-        delay = re.match('.*delay\s*=\s*([0-9\.]*)', report_lines[0]).group(1)
+        area = re.match(r'.*area\s*=\s*([0-9\.]*)', report_lines[0]).group(1)
+        delay = re.match(r'.*delay\s*=\s*([0-9\.]*)', report_lines[0]).group(1)
         return float(area), float(delay)
 
     yosys_arg_template = """-p
     read_verilog %s;
     synth -top toplevel;
     dfflibmap -liberty %s;
     abc -liberty %s -script +%s
```

### Comparing `pyrtl-0.8.7/pyrtl/helperfuncs.py` & `pyrtl-0.9.0/pyrtl/passes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,538 +1,636 @@
-""" Helper functions that make constructing hardware easier.
+"""
+Passes contains prebuilt transformantion passes to do optimization,
+lowering of the design to single wire gates (synthesis), along with other
+ways to change a block.
 """
 
 from __future__ import print_function, unicode_literals
 
-import numbers
-import six
-import math
-
-from .core import working_block, _NameIndexer
+from .core import working_block, set_working_block, _get_debug_mode, LogicNet, PostSynthBlock
+from .helperfuncs import _NetCount
+from .corecircuits import (_basic_mult, _basic_add, _basic_sub, _basic_eq,
+                           _basic_lt, _basic_gt, _basic_select, concat_list,
+                           as_wires, concat)
+from .memory import MemBlock
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
 from .wire import WireVector, Input, Output, Const, Register
-
-# -----------------------------------------------------------------
-#        ___       __   ___  __   __
-#  |__| |__  |    |__) |__  |__) /__`
-#  |  | |___ |___ |    |___ |  \ .__/
-#
-
-
-probeIndexer = _NameIndexer('Probe-')
+from .transform import net_transform, _get_new_block_mem_instance, copy_block, replace_wires
+from . import transform  # transform.all_nets looks better than all_nets
 
 
-def probe(w, name=None):
-    """ Print useful information about a WireVector when in debug mode.
-
-    :param w: WireVector from which to get info
-    :param name: optional name for probe (defaults to an autogenerated name)
-    :return: original WireVector w
+# --------------------------------------------------------------------
+#   __   __  ___           __      ___    __
+#  /  \ |__)  |  |  |\/| |  /  /\   |  | /  \ |\ |
+#  \__/ |     |  |  |  | | /_ /~~\  |  | \__/ | \|
+#
 
-    Probe can be inserted into a existing design easily as it returns the
-    original wire unmodified. For example ``y <<= x[0:3] + 4`` could be turned
-    into ``y <<= probe(x)[0:3] + 4`` to give visibility into both the origin of
-    ``x`` (including the line that WireVector was originally created) and
-    the run-time values of ``x`` (which will be named and thus show up by
-    default in a trace.  Likewise ``y <<= probe(x[0:3]) + 4``,
-    ``y <<= probe(x[0:3] + 4)``, and ``probe(y) <<= x[0:3] + 4`` are all
-    valid uses of `probe`.
 
-    Note: `probe` does actually add a wire to the working block of w (which can
-    confuse various post-processing transforms such as output to verilog).
+def optimize(update_working_block=True, block=None, skip_sanity_check=False):
     """
-    if not isinstance(w, WireVector):
-        raise PyrtlError('Only WireVectors can be probed')
-
-    if name is None:
-        name = '(%s: %s)' % (probeIndexer.make_valid_string(), w.name)
-    print("Probe: " + name + ' ' + get_stack(w))
-
-    p = Output(name=name)
-    p <<= w  # late assigns len from w automatically
-    return w
-
+    Return an optimized version of a synthesized hardware block.
 
-assertIndexer = _NameIndexer('assertion')
+    :param Boolean update_working_block: Don't copy the block and optimize the
+    new block
+    :param Block block: the block to optimize (defaults to working block)
 
-
-def rtl_assert(w, exp, block=None):
-    """ Add hardware assertions to be checked on the RTL design.
-
-    :param w: should be a WireVector
-    :param Exception exp: Exception to throw when assertion fails
-    :param Block block: block to which the assertion should be added (default to working block)
-    :return: the Output wire for the assertion (can be ignored in most cases)
-
-    If at any time during execution the wire w is not `true` (i.e. asserted low)
-    then simulation will raise exp.
+    Note:
+    optimize works on all hardware designs, both synthesized and non synthesized
     """
     block = working_block(block)
+    if not update_working_block:
+        block = copy_block(block)
 
-    if not isinstance(w, WireVector):
-        raise PyrtlError('Only WireVectors can be asserted with rtl_assert')
-    if len(w) != 1:
-        raise PyrtlError('rtl_assert checks only a WireVector of bitwidth 1')
-    if not isinstance(exp, Exception):
-        raise PyrtlError('the second argument to rtl_assert must be an instance of Exception')
-    if isinstance(exp, KeyError):
-        raise PyrtlError('the second argument to rtl_assert cannot be a KeyError')
-    if w not in block.wirevector_set:
-        raise PyrtlError('assertion wire not part of the block to which it is being added')
-    if w not in block.wirevector_set:
-        raise PyrtlError('assertion not a known wirevector in the target block')
-
-    if w in block.rtl_assert_dict:
-        raise PyrtlInternalError('assertion conflicts with existing registered assertion')
-
-    assert_wire = Output(bitwidth=1, name=assertIndexer.make_valid_string(), block=block)
-    assert_wire <<= w
-    block.rtl_assert_dict[assert_wire] = exp
-    return assert_wire
-
+    with set_working_block(block, no_sanity_check=True):
+        if (not skip_sanity_check) or _get_debug_mode():
+            block.sanity_check()
+        _remove_wire_nets(block)
+        constant_propagation(block, True)
+        _remove_unlistened_nets(block)
+        common_subexp_elimination(block)
+        if (not skip_sanity_check) or _get_debug_mode():
+            block.sanity_check()
+    return block
+
+
+class _ProducerList(object):
+    """  Maps from wire to its immediate producer and finds ultimate producers
+    """
+    def __init__(self):
+        self.dict = {}  # map from wirevector to its direct producer wirevector
+
+    def __getitem__(self, item):  # this is really to make pylint happy
+        raise PyrtlError("You usually don't want the immediate producer")
+
+    def __setitem__(self, key, item):
+        self.dict[key] = item
+
+    def find_producer(self, item):
+        if item in self.dict:
+            return self.find_producer(self.dict[item])
+        else:
+            return item
+
+
+def _remove_wire_nets(block):
+    """ Remove all wire nodes from the block. """
+
+    wire_src_dict = _ProducerList()
+    wire_removal_set = set()  # set of all wirevectors to be removed
+
+    # one pass to build the map of value producers and
+    # all of the nets and wires to be removed
+    for net in block.logic:
+        if net.op == 'w':
+            wire_src_dict[net.dests[0]] = net.args[0]
+            if not isinstance(net.dests[0], Output):
+                wire_removal_set.add(net.dests[0])
+
+    # second full pass to create the new logic without the wire nets
+    new_logic = set()
+    for net in block.logic:
+        if net.op != 'w' or isinstance(net.dests[0], Output):
+            new_args = tuple(wire_src_dict.find_producer(x) for x in net.args)
+            new_net = LogicNet(net.op, net.op_param, new_args, net.dests)
+            new_logic.add(new_net)
+
+    # now update the block with the new logic and remove wirevectors
+    block.logic = new_logic
+    for dead_wirevector in wire_removal_set:
+        del block.wirevector_by_name[dead_wirevector.name]
+        block.wirevector_set.remove(dead_wirevector)
+
+    block.sanity_check()
+
+
+def constant_propagation(block, silence_unexpected_net_warnings=False):
+    """ Removes excess constants in the block.
+
+    Note on resulting block:
+    The output of the block can have wirevectors that are driven but not
+    listened to. This is to be expected. These are to be removed by the
+    _remove_unlistened_nets function
+    """
+    net_count = _NetCount(block)
+    while net_count.shrinking():
+        _constant_prop_pass(block, silence_unexpected_net_warnings)
+
+
+def _constant_prop_pass(block, silence_unexpected_net_warnings=False):
+    """ Does one constant propagation pass """
+    valid_net_ops = '~&|^nrwcsm@'
+    no_optimization_ops = 'wcsm@'
+    one_var_ops = {
+        '~': lambda x: 1 - x,
+        'r': lambda x: x   # This is only valid for constant folding purposes
+    }
+    two_var_ops = {
+        '&': lambda l, r: l & r,
+        '|': lambda l, r: l | r,
+        '^': lambda l, r: l ^ r,
+        'n': lambda l, r: 1 - (l & r),
+    }
+
+    def _constant_prop_error(net, error_str):
+        if not silence_unexpected_net_warnings:
+            raise PyrtlError("Unexpected net, {}, has {}".format(net, error_str))
+
+    def constant_prop_check(net_checking):
+        def replace_net(new_net):
+            nets_to_remove.add(net_checking)
+            nets_to_add.add(new_net)
+
+        def replace_net_with_const(const_val):
+            new_const_wire = Const(bitwidth=1, val=const_val, block=block)
+            wire_add_set.add(new_const_wire)
+            replace_net_with_wire(new_const_wire)
+
+        def replace_net_with_wire(new_wire):
+            if isinstance(net_checking.dests[0], Output):
+                replace_net(LogicNet('w', None, args=(new_wire,),
+                                     dests=net_checking.dests))
+            else:
+                nets_to_remove.add(net_checking)
+                new_wire_src[net_checking.dests[0]] = new_wire
 
-def check_rtl_assertions(sim):
-    """ Checks the values in sim to see if any registers assertions fail.
+        if net_checking.op not in valid_net_ops:
+            _constant_prop_error(net_checking, "has a net not handled by constant_propagation")
+            return  # skip if we are ignoring unoptimizable ops
+
+        num_constants = sum((isinstance(arg, Const) for arg in net_checking.args))
+
+        if num_constants == 0 or net_checking.op in no_optimization_ops:
+            return  # assuming wire nets are already optimized
+
+        if (net_checking.op in two_var_ops) and num_constants == 1:
+            long_wires = [w for w in net_checking.args + net_checking.dests if len(w) != 1]
+            if len(long_wires):
+                _constant_prop_error(net_checking, "has wire(s) {} with bitwidths that are not 1"
+                                     .format(long_wires))
+                return  # skip if we are ignoring unoptimizable ops
+
+            # special case
+            const_wire, other_wire = net_checking.args
+            if isinstance(other_wire, Const):
+                const_wire, other_wire = other_wire, const_wire
+
+            outputs = [two_var_ops[net_checking.op](const_wire.val, other_val)
+                       for other_val in (0, 1)]
+
+            if outputs[0] == outputs[1]:
+                replace_net_with_const(outputs[0])
+            elif outputs[0] == 0:
+                replace_net_with_wire(other_wire)
+            else:
+                replace_net(LogicNet('~', None, args=(other_wire,),
+                                     dests=net_checking.dests))
 
-    :param sim: Simulation in which to check the assertions
-    :return: None
-    """
+        else:
+            # this optimization is actually compatible with long wires
+            if net_checking.op in two_var_ops:
+                output = two_var_ops[net_checking.op](net_checking.args[0].val,
+                                                      net_checking.args[1].val)
+            else:
+                output = one_var_ops[net_checking.op](net_checking.args[0].val)
+            replace_net_with_const(output)
 
-    for (w, exp) in sim.block.rtl_assert_dict.items():
-        try:
-            value = sim.inspect(w)
-            if not value:
-                raise exp
-        except KeyError:
-            pass
+    new_wire_src = _ProducerList()
+    wire_add_set = set()
+    nets_to_add = set()
+    nets_to_remove = set()
 
+    for a_net in block.logic:
+        constant_prop_check(a_net)
+    # second full pass to cleanup
 
-def log2(integer_val):
-    """ Return the log base 2 of the integer provided.
+    new_logic = set()
+    for net in block.logic.union(nets_to_add) - nets_to_remove:
+        new_args = tuple(new_wire_src.find_producer(x) for x in net.args)
+        new_net = LogicNet(net.op, net.op_param, new_args, net.dests)
+        new_logic.add(new_net)
 
-    :param integer_val: The integer to take the log base 2 of.
-    :return: The log base 2 of integer_val, or throw PyRTL error if not power of 2
+    block.logic = new_logic
+    for new_wirevector in wire_add_set:
+        block.add_wirevector(new_wirevector)
 
-    This function is useful when checking that powers of 2 are provided on inputs to functions.
-    It throws an error if a negative value is provided or if the value provided is not an even
-    power of two.
+    _remove_unused_wires(block)
 
-    Examples: ::
 
-        log2(2)  # returns 1
-        log2(256)  # returns 8
-        addrwidth = log2(size_of_memory)  # will fail if size_of_memory is not a power of two
+def common_subexp_elimination(block=None, abs_thresh=1, percent_thresh=0):
     """
-    i = integer_val
-    if not isinstance(i, int):
-        raise PyrtlError('this function can only take integers')
-    if i <= 0:
-        raise PyrtlError('this function can only take positive numbers 1 or greater')
-    if i & (i-1) != 0:
-        raise PyrtlError('this function can only take even powers of 2')
-    return i.bit_length() - 1
-
+    Common Subexpression Elimination for PyRTL blocks
 
-def truncate(wirevector_or_integer, bitwidth):
-    """ Returns a wirevector or integer truncated to the specified bitwidth
-
-    :param wirevector_or_integer: Either a wirevector or and integer to be truncated
-    :param bitwidth: The length to which the first argument should be truncated.
-    :return: Returns a tuncated wirevector or integer as appropriate
-
-    This function truncates the most significant bits of the input, leaving a result
-    that is only "bitwidth" bits wide.  For integers this is performed with a simple
-    bitmask of size "bitwidth".  For wirevectors the function calls WireVector.truncate
-    and returns a wirevector of the specified bitwidth.
-
-    Examples: ::
-
-        truncate(9,3)  # returns 3  (0b101 truncates to 0b101)
-        truncate(5,3)  # returns 3  (0b1001 truncates to 0b001)
-        truncate(-1,3)  # returns 7  (-0b1 truncates to 0b111)
-        y = truncate(x+1, x.bitwidth)  # y.bitwdith will equal x.bitwidth
+    :param block: the block to run the subexpression elimination on
+    :param abs_thresh: absolute threshold for stopping optimization
+    :param percent_thresh: percent threshold for stopping optimization
     """
-    if bitwidth < 1:
-        raise PyrtlError('bitwidth must be a positive integer')
-    x = wirevector_or_integer
-    try:
-        return x.truncate(bitwidth)
-    except AttributeError:
-        return x & ((1 << bitwidth)-1)
-
-
-def input_list(names, bitwidth=None):
-    """ Allocate and return a list of Inputs.
+    block = working_block(block)
+    net_count = _NetCount(block)
 
-    :param names: Names for the Inputs. Can be a list or single comma/space-separated string
-    :param bitwidth: The desired bitwidth for the resulting Inputs.
-    :return: List of Inputs.
+    while net_count.shrinking(block, percent_thresh, abs_thresh):
+        net_table = _find_common_subexps(block)
+        _replace_subexps(block, net_table)
+
+
+ops_where_arg_order_matters = 'm@xc<>-'
+
+
+def _find_common_subexps(block):
+    net_table = {}  # {net (without dest) : [net, ...]
+    t = tuple()  # just a placeholder
+    const_dict = {}
+    for net in block.logic:
+        if net.op in ops_where_arg_order_matters:
+            new_args = tuple(_const_to_int(w, const_dict) for w in net.args)
+        else:
+            new_args = tuple(sorted((_const_to_int(w, const_dict) for w in net.args), key=hash))
+        net_sub = LogicNet(net[0], net[1], new_args, t)  # don't care about dests
+        if net_sub in net_table:
+            net_table[net_sub].append(net)
+        else:
+            net_table[net_sub] = [net]
+    return net_table
+
+
+def _const_to_int(wire, const_dict):
+    if isinstance(wire, Const):
+        # a very bad hack to make sure two consts will compare
+        # correctly with an 'is'
+        bitwidth = wire.bitwidth
+        val = wire.val
+        if bitwidth not in const_dict:
+            const_dict[bitwidth] = {val: (bitwidth, val)}
+        else:
+            if val not in const_dict[bitwidth]:
+                const_dict[bitwidth][val] = (bitwidth, val)
+        return const_dict[bitwidth][val]
+
+    return wire
+
+
+def _replace_subexps(block, net_table):
+    wire_map = {}
+    unnecessary_nets = []
+    for nets in net_table.values():
+        _process_nets_to_discard(nets, wire_map, unnecessary_nets)
+
+    block.logic.difference_update(unnecessary_nets)
+    replace_wires(wire_map, block)
+
+
+def _has_normal_dest_wire(net):
+    return not isinstance(net.dests[0], (Register, Output))
+
+
+def _process_nets_to_discard(nets, wire_map, unnecessary_nets):
+    if len(nets) == 1:
+        return  # also deals with nets with no dest wires
+    nets_to_consider = list(filter(_has_normal_dest_wire, nets))
+
+    if len(nets_to_consider) > 1:  # needed to handle cases with only special wires
+        net_to_keep = nets_to_consider[0]
+        nets_to_discard = nets_to_consider[1:]
+        dest_w = net_to_keep.dests[0]
+        for net in nets_to_discard:
+            old_dst = net.dests[0]
+            wire_map[old_dst] = dest_w
+            unnecessary_nets.append(net)
+
+
+def _remove_unlistened_nets(block):
+    """ Removes all nets that are not connected to an output wirevector
+    """
+
+    listened_nets = set()
+    listened_wires = set()
+    prev_listened_net_count = 0
+
+    def add_to_listened(net):
+        listened_nets.add(net)
+        listened_wires.update(net.args)
+
+    for a_net in block.logic:
+        if a_net.op == '@':
+            add_to_listened(a_net)
+        elif any(isinstance(destW, Output) for destW in a_net.dests):
+            add_to_listened(a_net)
+
+    while len(listened_nets) > prev_listened_net_count:
+        prev_listened_net_count = len(listened_nets)
+
+        for net in block.logic - listened_nets:
+            if any((destWire in listened_wires) for destWire in net.dests):
+                add_to_listened(net)
+
+    block.logic = listened_nets
+    _remove_unused_wires(block)
+
+
+def _remove_unused_wires(block, keep_inputs=True):
+    """ Removes all unconnected wires from a block"""
+    valid_wires = set()
+    for logic_net in block.logic:
+        valid_wires.update(logic_net.args, logic_net.dests)
+
+    wire_removal_set = block.wirevector_set.difference(valid_wires)
+    for removed_wire in wire_removal_set:
+        if isinstance(removed_wire, Input):
+            term = " optimized away"
+            if keep_inputs:
+                valid_wires.add(removed_wire)
+                term = " deemed useless by optimization"
+
+            print("Input Wire, " + removed_wire.name + " has been" + term)
+        if isinstance(removed_wire, Output):
+            PyrtlInternalError("Output wire, " + removed_wire.name + " not driven")
+
+    block.wirevector_set = valid_wires
+
+# --------------------------------------------------------------------
+#    __           ___       ___  __     __
+#   /__` \ / |\ |  |  |__| |__  /__` | /__`
+#   .__/  |  | \|  |  |  | |___ .__/ | .__/
+#
 
-    Equivalent to: ::
 
-        wirevector_list(names, bitwidth, wvtype=pyrtl.wire.Input)
-
-    """
-    return wirevector_list(names, bitwidth, wvtype=Input)
+def synthesize(update_working_block=True, block=None):
+    """ Lower the design to just single-bit "and", "or", "xor", and "not" gates.
 
+    :param update_working_block: Boolean specifying if working block update
+    :param block: The block you want to synthesize
+    :return: The newly synthesized block (of type PostSynthesisBlock).
+
+    Takes as input a block (default to working block) and creates a new
+    block which is identical in function but uses only single bit gates
+    and excludes many of the more complicated primitives.  The new block
+    should consist *almost* exclusively of the combination elements
+    of w, &, |, ^, and ~ and sequential elements of registers (which are
+    one bit as well).  The two exceptions are for inputs/outputs (so that
+    we can keep the same interface) which are immediately broken down into
+    the individual bits and memories (read and write ports) which
+    require the reassembly and disassembly of the wirevectors immediately
+    before and after. These are the only two places where 'c' and 's' ops
+    should exist.
+
+    The block that results from synthesis is actually of type
+    "PostSynthesisBlock" which contains a mapping from the original inputs
+    and outputs to the inputs and outputs of this block.  This is used during
+    simulation to map the input/outputs so that the same testbench can be
+    used both pre and post synthesis (see documentation for Simulation for
+    more details).
+    """
+
+    block_pre = working_block(block)
+    block_pre.sanity_check()  # before going further, make sure that presynth is valid
+    block_in = copy_block(block_pre, update_working_block=False)
+
+    block_out = PostSynthBlock()
+    # resulting block should only have one of a restricted set of net ops
+    block_out.legal_ops = set('~&|^nrwcsm@')
+    wirevector_map = {}  # map from (vector,index) -> new_wire
+
+    with set_working_block(block_out, no_sanity_check=True):
+        # First, replace advanced operators with simpler ones
+        for op, fun in [
+                ('*', _basic_mult),
+                ('+', _basic_add),
+                ('-', _basic_sub),
+                ('x', _basic_select),
+                ('=', _basic_eq),
+                ('<', _basic_lt),
+                ('>', _basic_gt)]:
+            net_transform(_replace_op(op, fun), block_in)
+
+        # Next, create all of the new wires for the new block
+        # from the original wires and store them in the wirevector_map
+        # for reference.
+        for wirevector in block_in.wirevector_subset():
+            for i in range(len(wirevector)):
+                new_name = '_'.join((wirevector.name, 'synth', str(i)))
+                if isinstance(wirevector, Const):
+                    new_val = (wirevector.val >> i) & 0x1
+                    new_wirevector = Const(bitwidth=1, val=new_val)
+                elif isinstance(wirevector, (Input, Output)):
+                    new_wirevector = WireVector(name="tmp_" + new_name, bitwidth=1)
+                else:
+                    new_wirevector = wirevector.__class__(name=new_name, bitwidth=1)
+                wirevector_map[(wirevector, i)] = new_wirevector
+
+        # Now connect up the inputs and outputs to maintain the interface
+        for wirevector in block_in.wirevector_subset(Input):
+            input_vector = Input(name=wirevector.name, bitwidth=len(wirevector))
+            for i in range(len(wirevector)):
+                wirevector_map[(wirevector, i)] <<= input_vector[i]
+        for wirevector in block_in.wirevector_subset(Output):
+            output_vector = Output(name=wirevector.name, bitwidth=len(wirevector))
+            output_bits = [wirevector_map[(wirevector, i)]
+                           for i in range(len(output_vector))]
+            output_vector <<= concat_list(output_bits)
+
+        # Now that we have all the wires built and mapped, walk all the blocks
+        # and map the logic to the equivalent set of primitives in the system
+        out_mems = block_out.mem_map  # dictionary: PreSynth Map -> PostSynth Map
+        for net in block_in.logic:
+            _decompose(net, wirevector_map, out_mems, block_out)
+
+    if update_working_block:
+        set_working_block(block_out, no_sanity_check=True)
+    return block_out
+
+
+def _replace_op(op, fun):
+    def _replace_op_inner(net):
+        if net.op != op:
+            return True
+        dest = net.dests[0]
+        dest <<= fun(*net.args)
+        return False
+    return _replace_op_inner
 
-def output_list(names, bitwidth=None):
-    """ Allocate and return a list of Outputs.
 
-    :param names: Names for the Outputs. Can be a list or single comma/space-separated string
-    :param bitwidth: The desired bitwidth for the resulting Outputs.
-    :return: List of Outputs.
+def _decompose(net, wv_map, mems, block_out):
+    """ Add the wires and logicnets to block_out and wv_map to decompose net """
 
-    Equivalent to: ::
+    def arg(x, i):
+        # return the mapped wire vector for argument x, wire number i
+        return wv_map[(net.args[x], i)]
+
+    def destlen():
+        # return iterator over length of the destination in bits
+        return range(len(net.dests[0]))
+
+    def assign_dest(i, v):
+        # assign v to the wiremap for dest[0], wire i
+        wv_map[(net.dests[0], i)] <<= v
+
+    one_var_ops = {
+        'w': lambda w: w,
+        '~': lambda w: ~w,
+    }
+    c_two_var_ops = {
+        '&': lambda l, r: l & r,
+        '|': lambda l, r: l | r,
+        '^': lambda l, r: l ^ r,
+        'n': lambda l, r: l.nand(r),
+    }
+
+    if net.op in one_var_ops:
+        for i in destlen():
+            assign_dest(i, one_var_ops[net.op](arg(0, i)))
+    elif net.op in c_two_var_ops:
+        for i in destlen():
+            assign_dest(i, c_two_var_ops[net.op](arg(0, i), arg(1, i)))
+    elif net.op == 's':
+        for i in destlen():
+            selected_bit = arg(0, net.op_param[i])
+            assign_dest(i, selected_bit)
+    elif net.op == 'c':
+        arg_wirelist = []
+        # generate list of wires for vectors being concatenated
+        for arg_vector in net.args:
+            arg_vector_as_list = [wv_map[(arg_vector, i)] for i in range(len(arg_vector))]
+            arg_wirelist = arg_vector_as_list + arg_wirelist
+        for i in destlen():
+            assign_dest(i, arg_wirelist[i])
+    elif net.op == 'r':
+        for i in destlen():
+            args = (arg(0, i),)
+            dests = (wv_map[(net.dests[0], i)],)
+            new_net = LogicNet('r', None, args=args, dests=dests)
+            block_out.add_net(new_net)
+    elif net.op == 'm':
+        arg0list = [arg(0, i) for i in range(len(net.args[0]))]
+        addr = concat_list(arg0list)
+        new_mem = _get_new_block_mem_instance(net.op_param, mems, block_out)[1]
+        data = as_wires(new_mem[addr])
+        for i in destlen():
+            assign_dest(i, data[i])
+    elif net.op == '@':
+        addrlist = [arg(0, i) for i in range(len(net.args[0]))]
+        addr = concat_list(addrlist)
+        datalist = [arg(1, i) for i in range(len(net.args[1]))]
+        data = concat_list(datalist)
+        enable = arg(2, 0)
+        new_mem = _get_new_block_mem_instance(net.op_param, mems, block_out)[1]
+        new_mem[addr] <<= MemBlock.EnabledWrite(data=data, enable=enable)
+    else:
+        raise PyrtlInternalError('Unable to synthesize the following net '
+                                 'due to unimplemented op :\n%s' % str(net))
+    return
 
-        wirevector_list(names, bitwidth, wvtype=pyrtl.wire.Output)
 
+@transform.all_nets
+def nand_synth(net):
     """
-    return wirevector_list(names, bitwidth, wvtype=Output)
-
-
-def register_list(names, bitwidth=None):
-    """ Allocate and return a list of Registers.
-
-    :param names: Names for the Registers. Can be a list or single comma/space-separated string
-    :param bitwidth: The desired bitwidth for the resulting Registers.
-    :return: List of Registers.
-
-    Equivalent to: ::
-
-        wirevector_list(names, bitwidth, wvtype=pyrtl.wire.Register)
+    Synthesizes an Post-Synthesis block into one consisting of nands and inverters in place
 
+    :param block: The block to synthesize.
     """
-    return wirevector_list(names, bitwidth, wvtype=Register)
-
-
-def wirevector_list(names, bitwidth=None, wvtype=WireVector):
-    """ Allocate and return a list of WireVectors.
-
-    :param names: Names for the WireVectors. Can be a list or single comma/space-separated string
-    :param bitwidth: The desired bitwidth for the resulting WireVectors.
-    :param WireVector wvtype: Which WireVector type to create.
-    :return: List of WireVectors.
-
-    Additionally, the ``names`` string can also contain an additional bitwidth specification
-    separated by a ``/`` in the name. This cannot be used in combination with a ``bitwidth``
-    value other than ``1``.
-
-    Examples: ::
-
-        wirevector_list(['name1', 'name2', 'name3'])
-        wirevector_list('name1, name2, name3')
-        wirevector_list('input1 input2 input3', bitwidth=8, wvtype=pyrtl.wire.Input)
-        wirevector_list('output1, output2 output3', bitwidth=3, wvtype=pyrtl.wire.Output)
-        wirevector_list('two_bits/2, four_bits/4, eight_bits/8')
-        wirevector_list(['name1', 'name2', 'name3'], bitwidth=[2, 4, 8])
-
-    """
-    if isinstance(names, str):
-        names = names.replace(',', ' ').split()
-
-    if any('/' in name for name in names) and bitwidth is not None:
-        raise PyrtlError('only one of optional "/" or bitwidth parameter allowed')
-
-    if bitwidth is None:
-        bitwidth = 1
-    if isinstance(bitwidth, numbers.Integral):
-        bitwidth = [bitwidth]*len(names)
-    if len(bitwidth) != len(names):
-        raise ValueError('number of names ' + str(len(names))
-                         + ' should match number of bitwidths ' + str(len(bitwidth)))
-
-    wirelist = []
-    for fullname, bw in zip(names, bitwidth):
-        try:
-            name, bw = fullname.split('/')
-        except ValueError:
-            name, bw = fullname, bw
-        wirelist.append(wvtype(bitwidth=int(bw), name=name))
-    return wirelist
-
+    if net.op in '~nrwcsm@':
+        return True
 
-def val_to_signed_integer(value, bitwidth):
-    """ Return value as intrepreted as a signed integer under twos complement.
+    def arg(num):
+        return net.args[num]
 
-    :param value: a python integer holding the value to convert
-    :param bitwidth: the length of the integer in bits to assume for conversion
+    dest = net.dests[0]
+    if net.op == '&':
+        dest <<= ~(arg(0).nand(arg(1)))
+    elif net.op == '|':
+        dest <<= (~arg(0)).nand(~arg(1))
+    elif net.op == '^':
+        temp_0 = arg(0).nand(arg(1))
+        dest <<= temp_0.nand(arg(0)).nand(temp_0.nand(arg(1)))
+    else:
+        raise PyrtlError("Op, '{}' is not supported in nand_synth".format(net.op))
 
-    Given an unsigned integer (not a wirevector!) covert that to a signed
-    integer.  This is useful for printing and interpreting values which are
-    negative numbers in twos complement. ::
 
-        val_to_signed_integer(0xff, 8) == -1
+@transform.all_nets
+def and_inverter_synth(net):
     """
-    if isinstance(value, WireVector) or isinstance(bitwidth, WireVector):
-        raise PyrtlError('inputs must not be wirevectors')
-    if bitwidth < 1:
-        raise PyrtlError('bitwidth must be a positive integer')
-
-    neg_mask = 1 << (bitwidth - 1)
-    neg_part = value & neg_mask
-
-    pos_mask = neg_mask - 1
-    pos_part = value & pos_mask
-
-    return pos_part - neg_part
-
-
-def formatted_str_to_val(data, format, enum_set=None):
-    """ Return an unsigned integer representation of the data given format specified.
-
-    :param data: a string holding the value to convert
-    :param format: a string holding a format which will be used to convert the data string
-    :param enum_set: an iterable of enums which are used as part of the converstion process
-
-    Given a string (not a wirevector!) covert that to an unsigned integer ready for input
-    to the simulation enviornment.  This helps deal with signed/unsigned numbers (simulation
-    assumes the values have been converted via two's complement already), but it also takes
-    hex, binary, and enum types as inputs.  It is easiest to see how it works with some
-    examples. ::
-
-        formatted_str_to_val('2', 's3') == 2  # 0b010
-        formatted_str_to_val('-1', 's3') == 7  # 0b111
-        formatted_str_to_val('101', 'b3') == 5
-        formatted_str_to_val('5', 'u3') == 5
-        formatted_str_to_val('-3', 's3') == 5
-        formatted_str_to_val('a', 'x3') == 10
-        class Ctl(Enum):
-            ADD = 5
-            SUB = 12
-        formatted_str_to_val('ADD', 'e3/Ctl', [Ctl]) == 5
-        formatted_str_to_val('SUB', 'e3/Ctl', [Ctl]) == 12
+    Transforms a decomposed block into one consisting of ands and inverters in place
 
+    :param block: The block to synthesize
     """
-    type = format[0]
-    bitwidth = int(format[1:].split('/')[0])
-    bitmask = (1 << bitwidth)-1
-    if type == 's':
-        rval = int(data) & bitmask
-    elif type == 'x':
-        rval = int(data, 16)
-    elif type == 'b':
-        rval = int(data, 2)
-    elif type == 'u':
-        rval = int(data)
-        if rval < 0:
-            raise PyrtlError('unsigned format requested, but negative value provided')
-    elif type == 'e':
-        enumname = format.split('/')[1]
-        enum_inst_list = [e for e in enum_set if e.__name__ == enumname]
-        if len(enum_inst_list) == 0:
-            raise PyrtlError('enum "{}" not found in passed enum_set "{}"'
-                             .format(enumname, enum_set))
-        rval = getattr(enum_inst_list[0], data).value
-    else:
-        raise PyrtlError('unknown format type {}'.format(format))
-    return rval
-
-
-def val_to_formatted_str(val, format, enum_set=None):
-    """ Return a string representation of the value given format specified.
-
-    :param val: a string holding an unsigned integer to convert
-    :param format: a string holding a format which will be used to convert the data string
-    :param enum_set: an iterable of enums which are used as part of the converstion process
-
-    Given an unsigned integer (not a wirevector!) covert that to a strong ready for output
-    to a human to interpret.  This helps deal with signed/unsigned numbers (simulation
-    operates on values that have been converted via two's complement), but it also generates
-    hex, binary, and enum types as outputs.  It is easiest to see how it works with some
-    examples. ::
-
-        formatted_str_to_val(2, 's3') == '2'
-        formatted_str_to_val(7, 's3') == '-1'
-        formatted_str_to_val(5, 'b3') == '101'
-        formatted_str_to_val(5, 'u3') == '5'
-        formatted_str_to_val(5, 's3') == '-3'
-        formatted_str_to_val(10, 'x3') == 'a'
-        class Ctl(Enum):
-            ADD = 5
-            SUB = 12
-        formatted_str_to_val('ADD', 'e3/Ctl', [Ctl]) == 5
-        formatted_str_to_val('SUB', 'e3/Ctl', [Ctl]) == 12
-
-    """
-    type = format[0]
-    bitwidth = int(format[1:].split('/')[0])
-    bitmask = (1 << bitwidth)-1
-    if type == 's':
-        rval = str(val_to_signed_integer(val, bitwidth))
-    elif type == 'x':
-        rval = hex(val)[2:]  # cuts off '0x' at the start
-    elif type == 'b':
-        rval = bin(val)[2:]  # cuts off '0b' at the start
-    elif type == 'u':
-        rval = str(int(val))  # nothing fancy
-    elif type == 'e':
-        enumname = format.split('/')[1]
-        enum_inst_list = [e for e in enum_set if e.__name__ == enumname]
-        if len(enum_inst_list) == 0:
-            raise PyrtlError('enum "{}" not found in passed enum_set "{}"'
-                             .format(enumname, enum_set))
-        rval = enum_inst_list[0](val).name
-    else:
-        raise PyrtlError('unknown format type {}'.format(format))
-    return rval
-
-
-def get_stacks(*wires):
-    call_stack = getattr(wires[0], 'init_call_stack', None)
-    if not call_stack:
-        return '    No call info found for wires: use set_debug_mode() ' \
-               'to provide more information\n'
-    else:
-        return '\n'.join(str(wire) + ":\n" + get_stack(wire) for wire in wires)
-
+    if net.op in '~&rwcsm@':
+        return True
 
-def get_stack(wire):
-    if not isinstance(wire, WireVector):
-        raise PyrtlError('Only WireVectors can be traced')
+    def arg(num):
+        return net.args[num]
 
-    call_stack = getattr(wire, 'init_call_stack', None)
-    if call_stack:
-        frames = ' '.join(frame for frame in call_stack[:-1])
-        return "Wire Traceback, most recent call last \n" + frames + "\n"
+    dest = net.dests[0]
+    if net.op == '|':
+        dest <<= ~(~arg(0) & ~arg(1))
+    elif net.op == '^':
+        all_1 = arg(0) & arg(1)
+        all_0 = ~arg(0) & ~arg(1)
+        dest <<= all_0 & ~all_1
+    elif net.op == 'n':
+        dest <<= ~(arg(0) & arg(1))
     else:
-        return '    No call info found for wire: use set_debug_mode()'\
-               ' to provide more information'
+        raise PyrtlError("Op, '{}' is not supported in and_inv_synth".format(net.op))
 
 
-def _check_for_loop(block=None):
-    block = working_block(block)
-    logic_left = block.logic.copy()
-    wires_left = block.wirevector_subset(exclude=(Input, Const, Output, Register))
-    prev_logic_left = len(logic_left) + 1
-    while prev_logic_left > len(logic_left):
-        prev_logic_left = len(logic_left)
-        nets_to_remove = set()  # bc it's not safe to mutate a set inside its own iterator
-        for net in logic_left:
-            if not any(n_wire in wires_left for n_wire in net.args):
-                nets_to_remove.add(net)
-                wires_left.difference_update(net.dests)
-        logic_left -= nets_to_remove
-
-    if 0 == len(logic_left):
-        return None
-    return wires_left, logic_left
-
-
-def find_loop(block=None):
-    block = working_block(block)
-    block.sanity_check()  # make sure that the block is sane first
-
-    result = _check_for_loop(block)
-    if not result:
-        return
-    wires_left, logic_left = result
-    import random
-
-    class _FilteringState(object):
-        def __init__(self, dst_w):
-            self.dst_w = dst_w
-            self.arg_num = -1
-
-    def dead_end():
-        # clean up after a wire is found to not be part of the loop
-        wires_left.discard(cur_item.dst_w)
-        current_wires.discard(cur_item.dst_w)
-        del checking_stack[-1]
-
-    # now making a map to quickly look up nets
-    dest_nets = {dest_w: net_ for net_ in logic_left for dest_w in net_.dests}
-    initial_w = random.sample(wires_left, 1)[0]
-
-    current_wires = set()
-    checking_stack = [_FilteringState(initial_w)]
-
-    # we don't use a recursive method as Python has a limited stack (default: 999 frames)
-    while len(checking_stack):
-        cur_item = checking_stack[-1]
-        if cur_item.arg_num == -1:
-            #  first time testing this item
-            if cur_item.dst_w not in wires_left:
-                dead_end()
-                continue
-            current_wires.add(cur_item.dst_w)
-            cur_item.net = dest_nets[cur_item.dst_w]
-            if cur_item.net.op == 'r':
-                dead_end()
-                continue
-        cur_item.arg_num += 1  # go to the next item
-        if cur_item.arg_num == len(cur_item.net.args):
-            dead_end()
-            continue
-        next_wire = cur_item.net.args[cur_item.arg_num]
-        if next_wire not in current_wires:
-            current_wires.add(next_wire)
-            checking_stack.append(_FilteringState(next_wire))
-        else:  # We have found the loop!!!!!
-            loop_info = []
-            for f_state in reversed(checking_stack):
-                loop_info.append(f_state)
-                if f_state.dst_w is next_wire:
-                    break
-            else:
-                raise PyrtlError("Shouldn't get here! Couldn't figure out the loop")
-            return loop_info
-    raise PyrtlError("Error in detecting loop")
-
-
-def find_and_print_loop(block=None):
-    loop_data = find_loop(block)
-    print_loop(loop_data)
-    return loop_data
+@transform.all_nets
+def two_way_concat(net):
+    """
+    Transforms a block such that all n-way (n > 2) concats are replaced
+    with series of 2-way concats.
 
+    :param block: The block to transform
+
+    This is useful for preparing the netlist for output to other formats, like
+    FIRRTL or BTOR2, whose 'concatenate' operation ('cat' and 'concat', respectively),
+    only allow two arguments (most-significant wire and least-significant wire).
+    """
+
+    # Turns a netlist of the form (where [] denote nets):
+    #
+    #  w1  w2  w3
+    #   |  |   |
+    #   [concat]
+    #      |
+    #      w4
+    #
+    # into:
+    #
+    #  w1 w2   w3
+    #   | |    |
+    # [concat] |
+    #      |   |
+    #     [concat]
+    #        |
+    #      [wire]
+    #        |
+    #        w4
+    if net.op != 'c':
+        return True
 
-def print_loop(loop_data):
-    if not loop_data:
-        print("No Loop Found")
-    else:
-        print("Loop found:")
-        print('\n'.join("{}".format(fs.net) for fs in loop_data))
-        # print '\n'.join("{} (dest wire: {})".format(fs.net, fs.dst_w) for fs in loop_info)
-        print("")
+    if len(net.args) <= 2:
+        return True
 
+    w = concat(net.args[0], net.args[1])
+    for a in net.args[2:]:
+        w = concat(w, a)
 
-def _currently_in_ipython():
-    """ Return true if running under ipython, otherwise return False. """
-    try:
-        __IPYTHON__  # pylint: disable=undefined-variable
-        return True
-    except NameError:
-        return False
+    dest = net.dests[0]
+    dest <<= w
 
 
-class _NetCount(object):
+@transform.all_nets
+def one_bit_selects(net):
     """
-    Helper class to track when to stop an iteration that depends on number of nets
+    Converts arbitrary-sliced selects to concatenations of 1-bit selects
 
-    Mainly useful for iterations that are for optimization
+    :param block: The block to transform
+
+    This is useful for preparing the netlist for output to other formats, like
+    FIRRTL or BTOR2, whose 'select' operation ('bits' and 'slice', respectively)
+    require contiguous ranges. Python slices are not necessarily contiguous ranges,
+    e.g. the range [::2] (syntactic sugar for slice(None, None, 2)) produces indices
+    0, 2, 4, etc. up to the length of the list on which it is used.
     """
-    def __init__(self, block=None):
-        self.block = working_block(block)
-        self.prev_nets = len(self.block.logic) * 1000
-
-    def shrank(self, block=None, percent_diff=0, abs_diff=1):
-        """
-        Returns whether a block has less nets than before
-
-        :param Block block: block to check (if changed)
-        :param Number percent_diff: percentage difference threshold
-        :param int abs_diff: absolute difference threshold
-        :return: boolean
-
-        This function checks whether the change in the number of
-        nets is greater than the percentage and absolute difference
-        thresholds.
-        """
-        if block is None:
-            block = self.block
-        cur_nets = len(block.logic)
-        net_goal = self.prev_nets * (1 - percent_diff) - abs_diff
-        less_nets = (cur_nets <= net_goal)
-        self.prev_nets = cur_nets
-        return less_nets
+    if net.op != 's':
+        return True
 
-    shrinking = shrank
+    catlist = [net.args[0][i] for i in net.op_param]
+    dest = net.dests[0]
+    dest <<= concat_list(catlist)
```

### Comparing `pyrtl-0.8.7/pyrtl/memory.py` & `pyrtl-0.9.0/pyrtl/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Defines PyRTL memories.
 These blocks of memories can be read (potentially async) and written (sync)
 
 MemBlocks supports any number of the following operations:
 
 * read: `d = mem[address]`
-* write: `mem[address] = d`
-* write with an enable: `mem[address] = MemBlock.EnabledWrite(d,enable=we)`
+* write: `mem[address] <<= d`
+* write with an enable: `mem[address] <<= MemBlock.EnabledWrite(d,enable=we)`
 
 Based on the number of reads and writes a memory will be inferred
 with the correct number of ports to support that
 """
 
 from __future__ import print_function, unicode_literals
 import collections
@@ -29,14 +29,19 @@
 
 _memIndex = _NameIndexer()
 
 _MemAssignment = collections.namedtuple('_MemAssignment', 'rhs, is_conditional')
 """_MemAssignment is the type returned from assignment by |= or <<="""
 
 
+def _reset_memory_indexer():
+    global _memIndex
+    _memIndex = _NameIndexer()
+
+
 class _MemIndexed(WireVector):
     """ Object used internally to route memory assigns correctly.
 
     The normal PyRTL user should never need to be aware that this class exists,
     hence the underscore in the name.  It presents a very similar interface to
     wiresVectors (all of the normal wirevector operations should still work),
     but if you try to *set* the value with <<= or |= then it will generate a
@@ -84,15 +89,15 @@
 class _MemReadBase(object):
     """This is the base class for the memories and ROM blocks and
     it implements the read and initialization operations needed for
     both of them"""
 
     # FIXME: right now read port is built unconditionally (no read enable)
 
-    def __init__(self,  bitwidth, addrwidth, name, max_read_ports, asynchronous, block):
+    def __init__(self, bitwidth, addrwidth, name, max_read_ports, asynchronous, block):
         self.max_read_ports = max_read_ports
         self.read_ports = 0
         self.block = working_block(block)
         name = next_tempvar_name(name)
 
         if bitwidth <= 0:
             raise PyrtlError('bitwidth must be >= 1')
@@ -101,14 +106,15 @@
 
         self.bitwidth = bitwidth
         self.name = name
         self.addrwidth = addrwidth
         self.readport_nets = []
         self.id = _memIndex.next_index()
         self.asynchronous = asynchronous
+        self.block._add_memblock(self)
 
     def __getitem__(self, item):
         """ Builds circuitry to retrieve an item from the memory """
         item = as_wires(item, bitwidth=self.addrwidth, truncating=False)
         if len(item) > self.addrwidth:
             raise PyrtlError('memory index bitwidth > addrwidth')
         return _MemIndexed(mem=self, index=item)
@@ -144,17 +150,17 @@
     """ MemBlock is the object for specifying block memories.  In can be
     indexed like an array for both reading and writing.  Writes under a conditional
     are automatically converted to enabled writes.   For example, consider the following
     examples where `addr`, `data`, and `we` are all WireVectors.
 
     Usage::
 
-        data <<= memory[addr]  (infer read port)
+        data = memory[addr]  (infer read port)
         memory[addr] <<= data  (infer write port)
-        mem[address] = MemBlock.EnabledWrite(data,enable=we)
+        mem[address] <<= MemBlock.EnabledWrite(data,enable=we)
 
     When the address of a memory is assigned to using a EnableWrite object
     items will only be written to the memory when the enable WireVector is
     set to high (1)
     """
     # FIXME: write ports assume that only one port is under control of the conditional
     EnabledWrite = collections.namedtuple('EnabledWrite', 'data, enable')
@@ -284,29 +290,29 @@
             using values straight from a register. (aka make sure that reads
             are synchronous)
         :param bool pad_with_zeros: If true, extend any missing romdata with zeros out until the
             size of the romblock so that any access to the rom is well defined.  Otherwise, the
             simulation should throw an error on access of unintialized data.  If you are generating
             verilog from the rom, you will need to specify a value for every address (in which case
             setting this to True will help), however for testing and simulation it useful to know if
-            you are off the end of explicitly specified values (which is wy it is False by default)
+            you are off the end of explicitly specified values (which is why it is False by default)
         :param block: The block to add to, defaults to the working block
         """
 
         super(RomBlock, self).__init__(bitwidth, addrwidth, name, max_read_ports,
                                        asynchronous, block)
         self.data = romdata
         self.build_new_roms = build_new_roms
         self.current_copy = self
         self.pad_with_zeros = pad_with_zeros
 
     def __getitem__(self, item):
         import numbers
         if isinstance(item, numbers.Number):
-            raise PyrtlError("There is no point in indexing into a RomBlock with an int "
+            raise PyrtlError("There is no point in indexing into a RomBlock with an int. "
                              "Instead, get the value from the source data for this Rom")
             # If you really know what you are doing, use a Const WireVector instead.
         return super(RomBlock, self).__getitem__(item)
 
     def _get_read_data(self, address):
         import types
         try:
@@ -322,23 +328,27 @@
         else:
             try:
                 value = self.data[address]
             except KeyError:
                 if self.pad_with_zeros:
                     value = 0
                 else:
-                    raise PyrtlError("""RomBlock key is invalid,
-                                      consider using pad_with_zeros=True for defaults""")
+                    raise PyrtlError(
+                        "RomBlock key is invalid, "
+                        "consider using pad_with_zeros=True for defaults"
+                    )
             except IndexError:
                 if self.pad_with_zeros:
                     value = 0
                 else:
-                    raise PyrtlError("""RomBlock index is invalid,
-                                     consider using pad_with_zeros=True for defaults""")
-            except:
+                    raise PyrtlError(
+                        "RomBlock index is invalid, "
+                        "consider using pad_with_zeros=True for defaults"
+                    )
+            except Exception:
                 raise PyrtlError("invalid type for RomBlock data object")
 
         try:
             if value < 0 or value >= 2**self.bitwidth:
                 raise PyrtlError("invalid value for RomBlock data")
         except TypeError:
             raise PyrtlError("Value: {} from rom {} has an invalid type"
```

### Comparing `pyrtl-0.8.7/pyrtl/corecircuits.py` & `pyrtl-0.9.0/pyrtl/corecircuits.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def mux(index, *mux_ins, **kwargs):
     """ Multiplexer returning the value of the wire in .
 
     :param WireVector index: used as the select input to the multiplexer
     :param WireVector mux_ins: additional WireVector arguments selected when select>1
     :param WireVector kwargs: additional WireVectors, keyword arg "default"
-      If you are selecting between less items than your index can address, you can
+      If you are selecting between fewer items than your index can address, you can
       use the "default" keyword argument to auto-expand those terms.  For example,
       if you have a 3-bit index but are selecting between 6 options, you need to specify
       a value for those other 2 possible values of index (0b110 and 0b111).
     :return: WireVector of length of the longest input (not including select)
 
     To avoid confusion, if you are using the mux where the select is a "predicate"
     (meaning something that you are checking the truth value of rather than using it
@@ -82,22 +82,22 @@
                   truecase=mux(index[0:-1], *mux_ins[half:]))
 
 
 def select(sel, truecase, falsecase):
     """ Multiplexer returning falsecase for select==0, otherwise truecase.
 
     :param WireVector sel: used as the select input to the multiplexer
-    :param WireVector falsecase: the WireVector selected if select==0
     :param WireVector truecase: the WireVector selected if select==1
+    :param WireVector falsecase: the WireVector selected if select==0
 
     The hardware this generates is exactly the same as "mux" but by putting the
     true case as the first argument it matches more of the C-style ternary operator
-    semantics which can be helpful for readablity.
+    semantics which can be helpful for readability.
 
-    Example of mux as "ternary operator" to take the max of 'a' and 5: ::
+    Example of mux as "ternary operator" to take the min of 'a' and 5: ::
 
         select( a<5, truecase=a, falsecase=5 )
     """
     sel, f, t = (as_wires(w) for w in (sel, falsecase, truecase))
     f, t = match_bitwidth(f, t)
     outwire = WireVector(bitwidth=len(f))
 
@@ -111,15 +111,15 @@
 
     :param WireVector args: inputs to be concatenated
     :return: WireVector with length equal to the sum of the args' lengths
 
     You can provide multiple arguments and they will be combined with the right-most
     argument being the least significant bits of the result.  Note that if you have
     a list of arguments to concat together you will likely want index 0 to be the least
-    significant bit and so if you unpack the list into the arguements here it will be
+    significant bit and so if you unpack the list into the arguments here it will be
     backwards.  The function concat_list is provided for that case specifically.
 
     Example using concat to combine two bytes into a 16-bit quantity: ::
 
         concat( msb, lsb )
     """
     if len(args) <= 0:
@@ -141,52 +141,70 @@
 
 def concat_list(wire_list):
     """ Concatenates a list of WireVectors into a single WireVector
 
     :param wire_list: list of WireVectors to concat
     :return: WireVector with length equal to the sum of the args' lengths
 
-    This take a list of wirevectors and concats them all into a single wire
-    vector with the element at index 0 serving as the least significant bits.
-    This is useful when you have a variable number of wirevectors to concatenate,
+    This take a list of WireVectors and concats them all into a single
+    WireVector with the element at index 0 serving as the least significant bits.
+    This is useful when you have a variable number of WireVectors to concatenate,
     otherwise "concat" is prefered.
 
     Example using concat to combine two bytes into a 16-bit quantity: ::
 
         mylist = [ lsb, msb ]
         concat_list( mylist )
 
     """
     return concat(*reversed(wire_list))
 
 
 def signed_add(a, b):
-    """ Return wirevector for result of signed addition.
+    """ Return a WireVector for result of signed addition.
 
-    :param a: a wirevector to serve as first input to addition
-    :param b: a wirevector to serve as second input to addition
+    :param a: a WireVector to serve as first input to addition
+    :param b: a WireVector to serve as second input to addition
 
-    Given a length n and length m wirevector the result of the
+    Given a length n and length m WireVector the result of the
     signed addition is length max(n,m)+1.  The inputs are twos
-    complement sign extended to the same length before adding."""
+    complement sign extended to the same length before adding.
+    If an integer is passed to either a or b, it will be converted
+    automatically to a two's complemented constant"""
+    if isinstance(a, int):
+        a = Const(a, signed=True)
+    if isinstance(b, int):
+        b = Const(b, signed=True)
     a, b = match_bitwidth(as_wires(a), as_wires(b), signed=True)
     result_len = len(a) + 1
     ext_a = a.sign_extended(result_len)
     ext_b = b.sign_extended(result_len)
     # add and truncate to the correct length
     return (ext_a + ext_b)[0:result_len]
 
 
 def mult_signed(a, b):
     # mult_signed is now deprecated, use "signed_mult" instead
     return signed_mult(a, b)
 
 
 def signed_mult(a, b):
-    """ Return a*b where a and b are treated as signed values. """
+    """ Return a*b where a and b are treated as signed values.
+
+    :param a: a wirevector to serve as first input to multiplication
+    :param b: a wirevector to serve as second input to multiplication
+
+    If an integer is passed to either a or b, it will be converted
+    automatically to a two's complemented constant"""
+    # if an integer, convert to a two's complement constant
+    if isinstance(a, int):
+        a = Const(a, signed=True)
+    if isinstance(b, int):
+        b = Const(b, signed=True)
+    # if not a wirevector yet, use standard conversion method
     a, b = as_wires(a), as_wires(b)
     final_len = len(a) + len(b)
     # sign extend both inputs to the final target length
     a, b = a.sign_extended(final_len), b.sign_extended(final_len)
     # the result is the multiplication of both, but truncated
     # TODO: this may make estimates based on the multiplication overly
     # pessimistic as half of the multiply result is thrown right away!
@@ -237,15 +255,15 @@
     :param shift_amount: WireVector specifying amount to shift
     :return: WireVector of same length as bits_to_shift
 
     This function returns a new WireVector of length equal to the length
     of the input `bits_to_shift` but where the bits have been shifted
     to the left.  An arithemetic shift is one that treats the value as
     as signed number, although for left shift arithmetic and logic shift
-    are identical.  Note that `shift_amount` is treated as unsigned.
+    they are identical.  Note that `shift_amount` is treated as unsigned.
     """
     # shift left arithmetic and logical are the same thing
     return shift_left_logical(bits_to_shift, shift_amount)
 
 
 def shift_right_arithmetic(bits_to_shift, shift_amount):
     """ Shift right arithmetic operation.
@@ -302,29 +320,30 @@
     a, shamt = _check_shift_inputs(bits_to_shift, shift_amount)
     bit_in = Const(0)  # shift in a 0
     dir = Const(0)  # shift right
     return barrel.barrel_shifter(bits_to_shift, bit_in, dir, shift_amount)
 
 
 def match_bitwidth(*args, **opt):
-    """ Matches the bitwidth of all of the input arguments with zero or sign extend
+    """ Matches the bitwidth of all of the input arguments with zero or sign extension,
+        returning new WireVectors
 
     :param args: WireVectors of which to match bitwidths
     :param opt: Optional keyword argument 'signed=True' (defaults to False)
     :return: tuple of args in order with extended bits
 
     Example of matching the bitwidths of two WireVectors `a` and `b` with
     with zero extention: ::
 
-        a,b = match_bitwidth(a, b)
+        a, b = match_bitwidth(a, b)
 
     Example of matching the bitwidths of three WireVectors `a`,`b`, and `c` with
     with sign extention: ::
 
-        a,b = match_bitwidth(a, b, c, signed=True)
+        a, b = match_bitwidth(a, b, c, signed=True)
     """
     # TODO: when we drop 2.7 support, this code should be cleaned up with explicit
     # kwarg support for "signed" rather than the less than helpful "**opt"
     if len(opt) == 0:
         signed = False
     else:
         if len(opt) > 1 or 'signed' not in opt:
@@ -335,15 +354,15 @@
     if signed:
         return (wv.sign_extended(max_len) for wv in args)
     else:
         return (wv.zero_extended(max_len) for wv in args)
 
 
 def as_wires(val, bitwidth=None, truncating=True, block=None):
-    """ Return wires from val which may be wires, integers, strings, or bools.
+    """ Return wires from val which may be wires, integers (including IntEnums), strings, or bools.
 
     :param val: a wirevector-like object or something that can be converted into
       a Const
     :param bitwidth: The bitwidth the resulting wire should be
     :param bool truncating: determines whether bits will be dropped to achieve
      the desired bitwidth if it is too long (if true, the most-significant bits
      will be dropped)
@@ -354,15 +373,15 @@
     a Const WireVector). An example: ::
 
         def myhardware(input_a, input_b):
             a = as_wires(input_a)
             b = as_wires(input_b)
         myhardware(3, x)
 
-    The function as_wires will covert the 3 to Const but keep `x` unchanged
+    The function as_wires will convert the 3 to Const but keep `x` unchanged
     assuming it is a WireVector.
 
     """
     from .memory import _MemIndexed
     block = working_block(block)
 
     if isinstance(val, (int, six.string_types)):
@@ -385,88 +404,127 @@
     elif bitwidth and truncating and bitwidth < val.bitwidth:
         return val[:bitwidth]  # truncate the upper bits
     else:
         return val
 
 
 def bitfield_update(w, range_start, range_end, newvalue, truncating=False):
-    """ Return wirevector w but with some of the bits overwritten by newvalue.
+    """ Return WireVector w but with some of the bits overwritten by newvalue.
 
-    :param w: a wirevector to use as the starting point for the update
+    :param w: a WireVector to use as the starting point for the update
     :param range_start: the start of the range of bits to be updated
     :param range_end: the end of the range of bits to be updated
     :param newvalue: the value to be written in to the start:end range
-    :param truncating: if true, clip the newvalue to be the proper number of bits
+    :param truncating: if true, silently clip newvalue to the proper bitwidth rather than
+          throw an error if the value provided is too large
 
-    Given a wirevector w, this function returns a new wirevector that
+    Given a WireVector w, this function returns a new WireVector that
     is identical to w except in the range of bits specified.  In that
     specified range, the value newvalue is swapped in.  For example:
-    `bitfield_update(w, 20, 23, 0x7)` will return return a wirevector
+    `bitfield_update(w, 20, 23, 0x7)` will return return a WireVector
     of the same length as w, and with the same values as w, but with
     bits 20, 21, and 22 all set to 1.
 
     Note that range_start and range_end will be inputs to a slice and
-    so standar Python slicing rules apply (e.g. negative values for
+    so standard Python slicing rules apply (e.g. negative values for
     end-relative indexing and support for None). ::
 
         w = bitfield_update(w, 20, 23, 0x7)  # sets bits 20, 21, 22 to 1
         w = bitfield_update(w, 20, 23, 0x6)  # sets bit 20 to 0, bits 21 and 22 to 1
         w = bitfield_update(w, 20, None, 0x7)  # assuming w is 32 bits, sets bits 31..20 = 0x7
         w = bitfield_update(w, -1, None, 0x1)  # set the LSB (bit) to 1
     """
     from .corecircuits import concat_list
 
     w = as_wires(w)
     idxs = list(range(len(w)))  # we make a list of integers and slice those up to use as indexes
-    idxs_lower = idxs[0:range_start]
     idxs_middle = idxs[range_start:range_end]
-    idxs_upper = idxs[range_end:]
-
     if len(idxs_middle) == 0:
         raise PyrtlError('Cannot update bitfield of size 0 (i.e. there are no bits to update)')
+    idxs_lower = idxs[:idxs_middle[0]]
+    idxs_upper = idxs[idxs_middle[-1] + 1:]
+
     newvalue = as_wires(newvalue, bitwidth=len(idxs_middle), truncating=truncating)
     if len(idxs_middle) != len(newvalue):
         raise PyrtlError('Cannot update bitfield of length %d with value of length %d '
                          'unless truncating=True is specified' % (len(idxs_middle), len(newvalue)))
 
     result_list = []
     if idxs_lower:
-        result_list.append(w[idxs_lower[0]:idxs_lower[-1]+1])
+        result_list.append(w[idxs_lower[0]:idxs_lower[-1] + 1])
     result_list.append(newvalue)
     if idxs_upper:
-        result_list.append(w[idxs_upper[0]:idxs_upper[-1]+1])
+        result_list.append(w[idxs_upper[0]:idxs_upper[-1] + 1])
     result = concat_list(result_list)
 
     if len(result) != len(w):
         raise PyrtlInternalError('len(result)=%d, len(original)=%d' % (len(result), len(w)))
     return result
 
 
+def bitfield_update_set(w, update_set, truncating=False):
+    """ Return WireVector w but with some of the bits overwritten by values in update_set.
+
+    :param w: a WireVector to use as the starting point for the update
+    :param update_set: a map from tuples of integers (bit ranges) to the new values
+    :param truncating: if true, silently clip new values to the proper bitwidth rather than
+          throw an error if the value provided is too large
+
+    Given a WireVector w, this function returns a new WireVector that is identical to w except
+    in the range of bits specified.  When multiple non-overlapping fields need to be updated
+    in a single cycle this provides a clearer way to describe that behavior than iterative calls to
+    bitfield_update (although that is, in fact, what it is doing).
+
+        w = bitfield_update_set(w, {
+                (20, 23):    0x6,      # sets bit 20 to 0, bits 21 and 22 to 1
+                (26, None):  0x7,      # assuming w is 32 bits, sets bits 31..26 to 0x7
+                (-1, None):  0x0       # set the LSB (bit) to 0
+                })
+    """
+    w = as_wires(w)
+    # keep a list of bits that are updated to find overlaps
+    setlist = [False] * len(w)
+    # call bitfield for each one
+    for range in update_set:
+        range_start, range_end = range
+        new_value = update_set[range]
+        # check for overlaps
+        setbits = setlist[range_start:range_end]
+        if any(setbits):
+            raise PyrtlError('Bitfields for update are overlapping')
+        setlist[range_start:range_end] = [True] * len(setbits)
+        # do the actual update
+        w = bitfield_update(w, range_start, range_end, new_value, truncating)
+    return w
+
+
 def enum_mux(cntrl, table, default=None, strict=True):
     """ Build a mux for the control signals specified by an enum.
 
-    :param cntrl: is a wirevector and control for the mux.
-    :param table: is a dictionary of the form mapping enum->wirevector.
-    :param default: is a wirevector to use when the key is not present. In addtion
+    :param cntrl: is a WireVector and control for the mux.
+    :param table: is a dictionary of the form mapping enum->WireVector.
+    :param default: is a WireVector to use when the key is not present. In addition
         it is possible to use the key 'otherwise' to specify a default value, but
         it is an error if both are supplied.
     :param strict: is flag, that when set, will cause enum_mux to check
         that the dictionary has an entry for every possible value in the enum.
         Note that if a default is set, then this check is not performed as
         the default will provide valid values for any underspecified keys.
-    :return: a wirevector which is the result of the mux.
+    :return: a WireVector which is the result of the mux.
     ::
 
-        class Command(Enum):
+        from enum import IntEnum
+
+        class Command(IntEnum):
             ADD = 1
             SUB = 2
-        enum_mux(cntrl, {ADD: a+b, SUB: a-b})
-        enum_mux(cntrl, {ADD: a+b}, strict=False)  # SUB case undefined
-        enum_mux(cntrl, {ADD: a+b, otherwise: a-b})
-        enum_mux(cntrl, {ADD: a+b}, default=a-b)
+        enum_mux(cntrl, {Command.ADD: a+b, Command.SUB: a-b})
+        enum_mux(cntrl, {Command.ADD: a+b}, strict=False)  # SUB case undefined
+        enum_mux(cntrl, {Command.ADD: a+b, otherwise: a-b})
+        enum_mux(cntrl, {Command.ADD: a+b}, default=a-b)
 
     """
     # check dictionary keys are of the right type
     keytypeset = set(type(x) for x in table.keys() if x is not otherwise)
     if len(keytypeset) != 1:
         raise PyrtlError('table mixes multiple types {} as keys'.format(keytypeset))
     keytype = list(keytypeset)[0]
@@ -542,15 +600,15 @@
     if len(vector) == 1:
         return vector[0]
     rest = _apply_op_over_all_bits(op, vector[1:])
     return op(vector[0], rest)
 
 
 def rtl_any(*vectorlist):
-    """ Hardware equivalent of python native "any".
+    """ Hardware equivalent of Python native "any".
 
     :param WireVector vectorlist: all arguments are WireVectors of length 1
     :return: WireVector of length 1
 
     Returns a 1-bit WireVector which will hold a '1' if any of the inputs
     are '1' (i.e. it is a big ol' OR gate)
     """
@@ -559,15 +617,15 @@
     converted_vectorlist = [as_wires(v) for v in vectorlist]
     if any(len(v) != 1 for v in converted_vectorlist):
         raise PyrtlError('only length 1 WireVectors can be inputs to rtl_any')
     return or_all_bits(concat_list(converted_vectorlist))
 
 
 def rtl_all(*vectorlist):
-    """ Hardware equivalent of python native "all".
+    """ Hardware equivalent of Python native "all".
 
     :param WireVector vectorlist: all arguments are WireVectors of length 1
     :return: WireVector of length 1
 
     Returns a 1-bit WireVector which will hold a '1' only if all of the
     inputs are '1' (i.e. it is a big ol' AND gate)
     """
@@ -658,10 +716,10 @@
 def _basic_gt(a, b):
     return _basic_lt(b, a)
 
 
 def _basic_select(s, a, b):
     assert len(a) == len(b)
     assert len(s) == 1
-    sa = concat(*[~s]*len(a))
-    sb = concat(*[s]*len(b))
+    sa = concat(*[~s] * len(a))
+    sb = concat(*[s] * len(b))
     return (a & sa) | (b & sb)
```

### Comparing `pyrtl-0.8.7/pyrtl/__init__.py` & `pyrtl-0.9.0/pyrtl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # core rtl constructs
 from .core import LogicNet
 from .core import Block
 from .core import PostSynthBlock
 from .core import working_block
 from .core import reset_working_block
 from .core import set_working_block
+from .core import temp_working_block
 from .core import set_debug_mode
 
 # convenience classes for building hardware
 from .wire import WireVector
 from .wire import Input, Output
 from .wire import Const
 from .wire import Register
@@ -22,22 +23,26 @@
 
 from .helperfuncs import input_list
 from .helperfuncs import output_list
 from .helperfuncs import register_list
 from .helperfuncs import wirevector_list
 from .helperfuncs import log2
 from .helperfuncs import truncate
+from .helperfuncs import match_bitpattern
+from .helperfuncs import chop
 from .helperfuncs import val_to_signed_integer
 from .helperfuncs import val_to_formatted_str
 from .helperfuncs import formatted_str_to_val
+from .helperfuncs import infer_val_and_bitwidth
 from .helperfuncs import probe
 from .helperfuncs import rtl_assert
 from .helperfuncs import check_rtl_assertions
 from .helperfuncs import find_loop
 from .helperfuncs import find_and_print_loop
+from .helperfuncs import Bundle
 
 from .corecircuits import and_all_bits
 from .corecircuits import or_all_bits
 from .corecircuits import xor_all_bits
 from .corecircuits import rtl_any
 from .corecircuits import rtl_all
 from .corecircuits import mux
@@ -46,14 +51,15 @@
 from .corecircuits import concat_list
 from .corecircuits import parity
 from .corecircuits import tree_reduce
 from .corecircuits import as_wires
 from .corecircuits import match_bitwidth
 from .corecircuits import enum_mux
 from .corecircuits import bitfield_update
+from .corecircuits import bitfield_update_set
 from .corecircuits import signed_add
 from .corecircuits import signed_mult
 from .corecircuits import signed_lt
 from .corecircuits import signed_le
 from .corecircuits import signed_gt
 from .corecircuits import signed_ge
 from .corecircuits import shift_left_arithmetic
@@ -77,14 +83,15 @@
 from .simulation import SimulationTrace
 from .compilesim import CompiledSimulation
 
 # input and output to file format routines
 from .inputoutput import input_from_blif
 from .inputoutput import output_to_trivialgraph
 from .inputoutput import output_to_graphviz
+from .inputoutput import output_to_svg
 from .inputoutput import output_to_firrtl
 from .inputoutput import block_to_graphviz_string
 from .inputoutput import block_to_svg
 from .inputoutput import trace_to_html
 
 # extraction to verilog and verilog testbench
 from .verilog import output_to_verilog
@@ -94,10 +101,11 @@
 # different analysis and transform passes
 from .passes import common_subexp_elimination
 from .passes import constant_propagation
 from .passes import synthesize
 from .passes import nand_synth
 from .passes import and_inverter_synth
 from .passes import optimize
-
+from .passes import one_bit_selects
+from .passes import two_way_concat
 
 from .transform import net_transform, wire_transform, replace_wire, copy_block, clone_wire
```

### Comparing `pyrtl-0.8.7/pyrtl/core.py` & `pyrtl-0.9.0/pyrtl/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 * `modes` -- access methods for "modes" such as debug
 
 """
 from __future__ import print_function, unicode_literals
 import collections
 import re
 import keyword
-# from .helperfuncs import _currently_in_ipython
+
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
 
 
 # -----------------------------------------------------------------
 #    __        __   __
 #   |__) |    /  \ /  ` |__/
 #   |__) |___ \__/ \__, |  \
@@ -59,54 +59,52 @@
         ('<', None, (a1, a2), (out)) => check a2 greater than a1, put result into out (0 | 1)
         ('>', None, (a1, a2), (out)) => check a1 greater than a2, put result into out (0 | 1)
         ('w', None, (w1), (w2) => directional wire w/ no logical operation: connects w1 to w2
         ('x', None, (x, a1, a2), (out)) => mux: connect a1 (x=0), a2 (x=1) to out;
                                            x must be one bit; len(a1) = len(a2)
         ('c', None, (*args), (out)) => concatenates *args (wires) into single WireVector;
                                        puts first arg at MSB, last arg at LSB
-        ('s', (sel), (wire), (out)) => selects bits frm wire based on sel (std slicing syntax),
+        ('s', (sel), (wire), (out)) => selects bits from wire based on sel (std slicing syntax),
                                        puts into out
         ('r', None, (next), (r1)) => on positive clock edge: copies next to r1
         ('m', (memid, mem), (addr), (data)) => read address addr of mem (w/ id memid),
                                                put it into data
         ('@', (memid, mem), (addr, data, wr_en), ()) => write data to mem (w/ id memid) at
                                                         address addr; req. write enable (wr_en)
 
     """
 
     def __str__(self):
         rhs = ', '.join(str(x) for x in self.args)
         lhs = ', '.join(str(x) for x in self.dests)
         options = '' if self.op_param is None else '(' + str(self.op_param) + ')'
 
-        in_ipython = False
-        try:
-            from IPython.display import display, Markdown, Latex, Math
-            in_ipython = True
-        except ImportError:
-            pass
+        from .helperfuncs import _currently_in_jupyter_notebook
 
-        if in_ipython:
+        if _currently_in_jupyter_notebook():
             # Output the working block as a Latex table
             # Escape all Underscores
             rhs = rhs.replace('_', "\\_")
             lhs = lhs.replace('_', "\\_")
             options = options.replace('_', "\\_")
-            if self.op in '~&|':
+            if self.op in '&|':
                 return "{} & \\leftarrow \\{} \\, - & {} {} \\\\".format(
                        lhs, self.op, rhs, options)
             elif self.op in "wn+-*<>xcsr":
                 return "{} & \\leftarrow {} \\, - & {} {} \\\\".format(
                        lhs, self.op, rhs, options)
             elif self.op in "=":
                 return "{} & \\leftarrow \\, {} \\, - & {} {} \\\\".format(
                        lhs, self.op, rhs, options)
             elif self.op in "^":
                 return "{} & \\leftarrow \\oplus \\, - & {} {} \\\\".format(
                        lhs, rhs, options)
+            elif self.op in "~":
+                return "{} & \\leftarrow \\sim \\, - & {} {} \\\\".format(
+                       lhs, rhs, options)
 
             elif self.op in 'm@':
                 memid, memblock = self.op_param
                 extrainfo = 'memid=' + str(memid)
                 extrainfo = extrainfo.replace("_", "\\_")
                 name = memblock.name
                 name = name.replace("_", "\\_")
@@ -142,22 +140,22 @@
         # it seems that namedtuple is not always hashable
         return hash(tuple(self))
 
     def __eq__(self, other):
         # We can't be going and calling __eq__ recursively on the logic nets for all of
         # the args and dests because that will actually *create* new logic nets which is
         # very much not what people would expect to happen.  Instead we define equality
-        # as the immutable fields as being equal and the list of args and dests as being
+        # as the immutable fields being equal and the list of args and dests being
         # references to the same objects.
-        return (self.op == other.op and
-                self.op_param == other.op_param and
-                len(self.args) == len(other.args) and
-                len(self.dests) == len(other.dests) and
-                all(self.args[i] is other.args[i] for i in range(len(self.args))) and
-                all(self.dests[i] is other.dests[i] for i in range(len(self.dests))))
+        return (self.op == other.op
+                and self.op_param == other.op_param
+                and len(self.args) == len(other.args)
+                and len(self.dests) == len(other.dests)
+                and all(self.args[i] is other.args[i] for i in range(len(self.args)))
+                and all(self.dests[i] is other.dests[i] for i in range(len(self.dests))))
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def _compare_error(self, other):
         """ Throw error when LogicNets are compared.
 
@@ -184,101 +182,99 @@
 
     The logic structure is primarily contained in self.logic which holds a set of
     "LogicNet"s. Each LogicNet describes a primitive operation (such as an adder
     or memory).  The primitive is described by a 4-tuple of:
 
     1) the op (a single character describing the operation such as '+' or 'r'),
     2) a set of hard parameters to that primitives (such as the constants to
-       select from the "selection" op.
+       select from the "selection" op).
     3) the tuple "args" which list the wirevectors hooked up as inputs to
        this particular net.
     4) the tuple "dests" which list the wirevectors hooked up as output for
        this particular net.
 
     Below is a list of the basic operations.  These properties (more formally
-    specified) should all be checked by the class method sanity_check.
+    specified) should all be checked by the class method 'sanity_check'.
 
-    * Most logical and arithmetic ops are pretty self explanatory, each takes
-      exactly two arguments and they should perform the arithmetic or logical
+    * Most logical and arithmetic ops are pretty self explanatory. Each takes
+      exactly two arguments, and they should perform the arithmetic or logical
       operation specified. OPS: ('&','|','^','n','~','+','-','*').  All inputs must
       be the same bitwidth.  Logical operations produce as many bits as are in
-      the input, while '+' and '-' produce n+1 bits, and '*' produced 2n bits.
+      the input, while '+' and '-' produce n+1 bits, and '*' produces 2n bits.
 
     * In addition there are some operations for performing comparisons
       that should perform the operation specified.  The '=' op is checking
       to see if the bits of the vectors are equal, while '<' and '>' do
       unsigned arithmetic comparison.  All comparisons generate a single bit
       of output (1 for true, 0 for false).
 
     * The 'w' operator is simply a directional wire and has no logic function.
 
     * The 'x' operator is a mux which takes a select bit and two signals.
-      If the value of the select bit is 0 it selects the second argument, if
+      If the value of the select bit is 0 it selects the second argument; if
       it is 1 it selects the third argument.  Select must be a single bit, while
       the other two arguments must be the same length.
 
-    * The 'c' operator is the concatiation operator and combines any number of
+    * The 'c' operator is the concatenation operator and combines any number of
       wirevectors (a,b,...,z) into a single new wirevector with "a" in the MSB
       and "z" (or whatever is last) in the LSB position.
 
     * The 's' operator is the selection operator and chooses, based on the
-      op_param specificied, a subset of the logic bits from a WireVector to
+      op_param specified, a subset of the logic bits from a WireVector to
       select.  Repeats are accepted.
 
     * The 'r' operator is a register and on posedge, simply copies the value
-      from the input to the output of the register
+      from the input to the output of the register.
 
     * The 'm' operator is a memory block read port, which supports async reads (acting
-      like combonational logic). Multiple read (and write) ports are possible to
+      like combinational logic). Multiple read (and write) ports are possible to
       the same memory but each 'm' defines only one of those. The op_param
       is a tuple containing two references: the mem id, and a reference to the
       MemBlock containing this port. The MemBlock should only be used for debug and
       sanity checks. Each read port has one addr (an arg) and one data (a dest).
 
-    * The '@' (update) operator is a memory block write port, which supports syncronous writes
+    * The '@' (update) operator is a memory block write port, which supports synchronous writes
       (writes are "latched" at posedge).  Multiple write (and read) ports are possible
       to the same memory but each '@' defines only one of those. The op_param
       is a tuple containing two references: the mem id, and a reference to the MemoryBlock.
       Writes have three args (addr, data, and write enable).  The dests should be an
       empty tuple.  You will not see a written value change until the following cycle.
       If multiple writes happen to the same address in the same cycle the behavior is currently
       undefined.
 
     The connecting elements (args and dests) should be WireVectors or derived
     from WireVector, and should be registered with the block using
-    the method add_wirevector.  Nets should be registered using add_net.
+    the method 'add_wirevector'.  Nets should be registered using 'add_net'.
 
-    In addition, there is a member legal_ops which defines the set of operations
+    In addition, there is a member 'legal_ops' which defines the set of operations
     that can be legally added to the block.  By default it is set to all of the above
     defined operations, but it can be useful in certain cases to only allow a
     subset of operations (such as when transforms are being done that are "lowering"
-    the blocks to more primitive ops.
+    the blocks to more primitive ops).
     """
 
     def __init__(self):
         """Creates an empty hardware block."""
         self.logic = set()  # set of nets, each is a LogicNet named tuple
         self.wirevector_set = set()  # set of all wirevectors
         self.wirevector_by_name = {}  # map from name->wirevector, used for performance
         # pre-synthesis wirevectors to post-synthesis vectors
         self.legal_ops = set('w~&|^n+-*<>=xcsrm@')  # set of legal OPS
         self.rtl_assert_dict = {}   # map from wirevectors -> exceptions, used by rtl_assert
+        self.memblock_by_name = {}  # map from name->memblock, for easy access to memblock objs
 
     def __str__(self):
         """String form has one LogicNet per line."""
-        try:
-            from IPython.display import display, Markdown, Latex, Math
-            out = '\n\begin{array}{ \| c \| c \| l \| }\n'
-            out += '\n\hline\n'
-            out += '\\hline\n'.join(str(l) for l in self)
-            out += '\hline\n\end{array}\n'
-            display(Latex(out))
+        from .helperfuncs import _currently_in_jupyter_notebook, _print_netlist_latex
+
+        if _currently_in_jupyter_notebook():
+            _print_netlist_latex(list(self))
             return ' '
-        except ImportError:
-            return '\n'.join(str(l) for l in self)
+        else:
+            return '\n'.join(str(net) for net in self)
 
     def add_wirevector(self, wirevector):
         """ Add a wirevector object to the block."""
         self.sanity_check_wirevector(wirevector)
         self.wirevector_set.add(wirevector)
         self.wirevector_by_name[wirevector.name] = wirevector
 
@@ -293,14 +289,85 @@
         The passed net, which must be of type LogicNet, is checked and then
         added to the block.  No wires are added by this member, they must be
         added seperately with add_wirevector."""
 
         self.sanity_check_net(net)
         self.logic.add(net)
 
+    def _add_memblock(self, mem):
+        """ Registers a memory to the block.
+
+        Note that this is done automatically when a memory block is
+        created and isn't intended for use by PyRTL end users.
+        This is so non-local memories can be accessed later on
+        (e.g. for instantiating during a simulation).
+        """
+        self.sanity_check_memblock(mem)
+        self.memblock_by_name[mem.name] = mem
+
+    def get_memblock_by_name(self, name, strict=False):
+        """ Get a reference to a memory stored in this block by name.
+
+        By fallthrough, if a matching memblock cannot be found the value None is
+        returned.  However, if the argument strict is set to True, then this will
+        instead throw a PyrtlError when no match is found.
+
+        This useful for when a block defines its own internal memory block, and
+        during simulation you want to instantiate that memory with certain values
+        for testing. Since the Simulation constructor requires a reference to the
+        memory object itself, but the block you're testing defines the memory internally,
+        this allows you to get the object reference.
+
+        Note that this requires you know the name of the memory block, meaning that
+        you most likely need to have named it yourself.
+
+        For example:
+
+            def special_memory(read_addr, write_addr, data, wen):
+                mem = pyrtl.MemBlock(bitwidth=32, addrwidth=5, name='special_mem')
+                mem[write_addr] <<= pyrtl.MemBlock.EnabledWrite(data, wen & (write_addr > 0))
+                return mem[read_addr]
+
+            read_addr = pyrtl.Input(5, 'read_addr')
+            write_addr = pyrtl.Input(5, 'write_addr')
+            data = pyrtl.Input(32, 'data')
+            wen = pyrtl.Input(1, 'wen')
+            res = pyrtl.Output(32, 'res')
+
+            res <<= special_memory(read_addr, write_addr, data, wen)
+
+            # Can only access it after the `special_memory` block has been instantiated/called
+            special_mem = pyrtl.working_block().get_memblock_by_name('special_mem')
+
+            sim = pyrtl.Simulation(memory_value_map={
+                special_mem: {
+                    0: 5,
+                    1: 6,
+                    2: 7,
+                }
+            })
+
+            inputs = {
+                'read_addr':  '012012',
+                'write_addr': '012012',
+                'data':       '890333',
+                'wen':        '111000',
+            }
+            expected = {
+                'res': '567590',
+            }
+            sim.step_multiple(inputs, expected)
+        """
+        if name in self.memblock_by_name:
+            return self.memblock_by_name[name]
+        elif strict:
+            raise PyrtlError('error, block does not have a memblock named %s' % name)
+        else:
+            return None
+
     def wirevector_subset(self, cls=None, exclude=tuple()):
         """Return set of wirevectors, filtered by the type or tuple of types provided as cls.
 
         If no cls is specified, the full set of wirevectors associated with the Block are
         returned.  If cls is a single type, or a tuple of types, only those wirevectors of
         the matching types will be returned.  This is helpful for getting all inputs, outputs,
         or registers of a block for example."""
@@ -339,32 +406,34 @@
     def net_connections(self, include_virtual_nodes=False):
         """ Returns a representation of the current block useful for creating a graph.
 
         :param include_virtual_nodes: if enabled, the wire itself will be used to
           signal an external source or sink (such as the source for an Input net).
           If disabled, these nodes will be excluded from the adjacency dictionaries
         :return wire_src_dict, wire_sink_dict
-          Returns two dictionaries: one that map WireVectors to the logic
-          nets that creates their signal and one that maps WireVectors to
+          Returns two dictionaries: one that maps WireVectors to the logic
+          net that creates their signal and one that maps WireVectors to
           a list of logic nets that use the signal
 
         These dictionaries make the creation of a graph much easier, as
         well as facilitate other places in which one would need wire source
-        and wire sink information
+        and wire sink information.
 
-        Look at input_output.net_graph for one such graph that uses the information
-        from this function
+        Look at inputoutput.net_graph for one such graph that uses the information
+        from this function.
         """
         src_list = {}
         dst_list = {}
 
         def add_wire_src(edge, node):
             if edge in src_list:
-                raise PyrtlError('Wire "{}" has multiple drivers (check for multiple assignments '
-                                 'with "<<=" or accidental mixing of "|=" and "<<=")'.format(edge))
+                raise PyrtlError('Wire "{}" has multiple drivers: [{}] and [{}] (check for '
+                                 'multiple assignments with "<<=" or accidental mixing of '
+                                 '"|=" and "<<=")'
+                                 .format(edge, str(src_list[edge]).strip(), str(node).strip()))
             src_list[edge] = node
 
         def add_wire_dst(edge, node):
             if edge in dst_list:
                 # if node in dst_list[edge]:
                 #     raise PyrtlError("The net already exists in the graph")
                 dst_list[edge].append(node)
@@ -390,19 +459,19 @@
         """ IPython display support for Block. """
         from .inputoutput import block_to_svg
         return block_to_svg(self)
 
     def __iter__(self):
         """ BlockIterator iterates over the block passed on init in topographic order.
         The input is a Block, and when a LogicNet is returned it is always the case
-        that all of it's "parents" have already been returned earlier in the iteration.
+        that all of its "parents" have already been returned earlier in the iteration.
 
         Note: this method will throw an error if there are loops in the
-        logic that do not involve registers
-        Also, the order of the nets is not guaranteed to be the the same
+        logic that do not involve registers.
+        Also, the order of the nets is not guaranteed to be the same
         over multiple iterations"""
         from .wire import Input, Const, Register
         src_dict, dest_dict = self.net_connections()
         to_clear = self.wirevector_subset((Input, Const, Register))
         cleared = set()
         remaining = self.logic.copy()
         try:
@@ -447,16 +516,16 @@
         # check for unique names
         wirevector_names_set = set(x.name for x in self.wirevector_set)
         if len(self.wirevector_set) != len(wirevector_names_set):
             wirevector_names_list = [x.name for x in self.wirevector_set]
             for w in wirevector_names_set:
                 wirevector_names_list.remove(w)
             raise PyrtlError('Duplicate wire names found for the following '
-                             'different signals: %s (make sure you are not using "tmp"'
-                             'or "const_" as a signal name because those are reserved for'
+                             'different signals: %s (make sure you are not using "tmp" '
+                             'or "const_" as a signal name because those are reserved for '
                              'internal use)' % repr(wirevector_names_list))
 
         # check for dead input wires (not connected to anything)
         all_input_and_consts = self.wirevector_subset((Input, Const))
 
         # The following line also checks for duplicate wire drivers
         wire_src_dict, wire_dst_dict = self.net_connections()
@@ -537,17 +606,25 @@
         """ Check that w is a valid wirevector type. """
         from .wire import WireVector
         if not isinstance(w, WireVector):
             raise PyrtlError(
                 'error attempting to pass an input of type "%s" '
                 'instead of WireVector' % type(w))
 
+    def sanity_check_memblock(self, m):
+        """ Check that m is a valid memblock type. """
+        from .memory import _MemReadBase
+        if not isinstance(m, _MemReadBase):
+            raise PyrtlError(
+                'error attempting to pass an input of type "%s" '
+                'instead of _MemReadBase' % type(m))
+
     def sanity_check_net(self, net):
         """ Check that net is a valid LogicNet. """
-        from .wire import Input, Output, Const
+        from .wire import Input, Output, Const, Register
         from .memory import _MemReadBase
 
         # general sanity checks that apply to all operations
         if not isinstance(net, LogicNet):
             raise PyrtlInternalError('error, net must be of type LogicNet')
         if not isinstance(net.args, tuple):
             raise PyrtlInternalError('error, LogicNet args must be tuple')
@@ -557,26 +634,28 @@
             self.sanity_check_wirevector(w)
             if w._block is not self:
                 raise PyrtlInternalError('error, net references different block')
             if w not in self.wirevector_set:
                 raise PyrtlInternalError('error, net with unknown source "%s"' % w.name)
 
         # checks that input and output wirevectors are not misused
-        for w in net.dests:
-            if isinstance(w, (Input, Const)):
-                raise PyrtlInternalError('error, Inputs, Consts cannot be destinations to a net')
-        for w in net.args:
-            if isinstance(w, Output):
-                raise PyrtlInternalError('error, Outputs cannot be arguments for a net')
+        bad_dests = set(filter(lambda w: isinstance(w, (Input, Const)), net.dests))
+        if bad_dests:
+            raise PyrtlInternalError('error, Inputs, Consts cannot be destinations to a net (%s)' %
+                                     ','.join(map(str, bad_dests)))
+        bad_args = set(filter(lambda w: isinstance(w, (Output)), net.args))
+        if bad_args:
+            raise PyrtlInternalError('error, Outputs cannot be arguments for a net (%s)' %
+                                     ','.join(map(str, bad_args)))
 
         if net.op not in self.legal_ops:
             raise PyrtlInternalError('error, net op "%s" not from acceptable set %s' %
                                      (net.op, self.legal_ops))
 
-        # operation specific checks on arguments
+        # operation-specific checks on arguments
         if net.op in 'w~rsm' and len(net.args) != 1:
             raise PyrtlInternalError('error, op only allowed 1 argument')
         if net.op in '&|^n+-*<>=' and len(net.args) != 2:
             raise PyrtlInternalError('error, op only allowed 2 arguments')
         if net.op == 'x':
             if len(net.args) != 3:
                 raise PyrtlInternalError('error, op only allowed 3 arguments')
@@ -591,15 +670,15 @@
         if net.op in 'm@' and net.args[0].bitwidth != net.op_param[1].addrwidth:
             raise PyrtlInternalError('error, mem addrwidth mismatch')
         if net.op == '@' and net.args[1].bitwidth != net.op_param[1].bitwidth:
             raise PyrtlInternalError('error, mem bitwidth mismatch')
         if net.op == '@' and net.args[2].bitwidth != 1:
             raise PyrtlInternalError('error, mem write enable must be 1 bit')
 
-        # operation specific checks on op_params
+        # operation-specific checks on op_params
         if net.op in 'w~&|^n+-*<>=xcr' and net.op_param is not None:
             raise PyrtlInternalError('error, op_param should be None')
         if net.op == 's':
             if not isinstance(net.op_param, tuple):
                 raise PyrtlInternalError('error, select op requires tuple op_param')
             for p in net.op_param:
                 if not isinstance(p, int):
@@ -612,14 +691,22 @@
             if len(net.op_param) != 2:
                 raise PyrtlInternalError('error, mem op requires 2 op_params in tuple')
             if not isinstance(net.op_param[0], int):
                 raise PyrtlInternalError('error, mem op requires first operand as int')
             if not isinstance(net.op_param[1], _MemReadBase):
                 raise PyrtlInternalError('error, mem op requires second operand of a memory type')
 
+        # operation-specific checks on destinations
+        if net.op in 'w~&|^n+-*<>=xcsrm' and len(net.dests) != 1:
+            raise PyrtlInternalError('error, op only allowed 1 destination')
+        if net.op == '@' and net.dests != ():
+            raise PyrtlInternalError('error, mem write dest should be empty tuple')
+        if net.op == 'r' and not isinstance(net.dests[0], Register):
+            raise PyrtlInternalError('error, dest of next op should be a Register')
+
         # check destination validity
         if net.op in 'w~&|^nr' and net.dests[0].bitwidth > net.args[0].bitwidth:
             raise PyrtlInternalError('error, upper bits of destination unassigned')
         if net.op in '<>=' and net.dests[0].bitwidth != 1:
             raise PyrtlInternalError('error, destination should be of bitwidth=1')
         if net.op in '+-' and net.dests[0].bitwidth > net.args[0].bitwidth + 1:
             raise PyrtlInternalError('error, upper bits of destination unassigned')
@@ -629,16 +716,14 @@
             raise PyrtlInternalError('error, upper bits of mux output undefined')
         if net.op == 'c' and net.dests[0].bitwidth > sum(x.bitwidth for x in net.args):
             raise PyrtlInternalError('error, upper bits of concat output undefined')
         if net.op == 's' and net.dests[0].bitwidth > len(net.op_param):
             raise PyrtlInternalError('error, upper bits of select output undefined')
         if net.op == 'm' and net.dests[0].bitwidth != net.op_param[1].bitwidth:
             raise PyrtlInternalError('error, mem read dest bitwidth mismatch')
-        if net.op == '@' and net.dests != ():
-            raise PyrtlInternalError('error, mem write dest should be empty tuple')
 
 
 class PostSynthBlock(Block):
     """ This is a block with extra metadata required to maintain the
     pre synthesis interface post synthesis
     """
 
@@ -664,14 +749,18 @@
 # are useful for developers to adjust behaviors in the different modes
 # but should not be set directly by users.
 debug_mode = False
 _setting_keep_wirevector_call_stack = False
 _setting_slower_but_more_descriptive_tmps = False
 
 
+def _get_debug_mode():
+    return debug_mode
+
+
 def _get_useful_callpoint_name():
     """ Attempts to find the lowest user-level call into the pyrtl module
     :return (string, int) or None: the file name and line number respectively
 
     This function walks back the current frame stack attempting to find the
     first frame that is not part of the pyrtl module.  The filename (stripped
     of path and .py extention) and line number of that call are returned.
@@ -690,15 +779,15 @@
             modname = inspect.getmodule(frame[0]).__name__
             if not modname.startswith('pyrtl.'):
                 full_filename = frame[0].f_code.co_filename
                 filename = full_filename.split('/')[-1].rstrip('.py')
                 lineno = frame[0].f_lineno
                 loc = (filename, lineno)
                 break
-    except:
+    except Exception:
         loc = None
     finally:
         del frame_stack
     return loc
 
 
 def working_block(block=None):
@@ -720,23 +809,14 @@
 
 def reset_working_block():
     """ Reset the working block to be empty. """
     global _singleton_block
     _singleton_block = Block()
 
 
-def _currently_in_ipython():
-    """ Return true if running under ipython, otherwise return False. """
-    try:
-        __IPYTHON__  # pylint: disable=undefined-variable
-        return True
-    except NameError:
-        return False
-
-
 class set_working_block(object):
     """ Set the working block to be the block passed as argument.
         Compatible with the 'with' statement
 
         Sanity checks will only be run if the new block is different
         from the original block
     """
@@ -758,25 +838,33 @@
     def __enter__(self):
         return self.old_block
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._set_working_block(self.old_block, no_sanity_check=True)
 
 
+def temp_working_block():
+    """ Set the working block to be new temporary block.
+        If used with the 'with' statement the block will be reset to the
+        original value (at the time of call) at exit of the context.
+    """
+    return set_working_block(Block())
+
+
 def set_debug_mode(debug=True):
     """ Set the global debug mode. """
     global debug_mode
     global _setting_keep_wirevector_call_stack
     global _setting_slower_but_more_descriptive_tmps
     debug_mode = debug
     _setting_keep_wirevector_call_stack = debug
     _setting_slower_but_more_descriptive_tmps = debug
 
 
-_py_regex = '^[^\d\W]\w*\Z'
+_py_regex = r'^[^\d\W]\w*\Z'
 
 
 class _NameIndexer(object):
     """ Provides internal names that are based on a prefix and an index"""
     def __init__(self, internal_prefix='_sani_temp'):
         self.internal_prefix = internal_prefix
         self.internal_index = 0
```

### Comparing `pyrtl-0.8.7/pyrtl/verilog.py` & `pyrtl-0.9.0/pyrtl/verilog.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 
 Each of the functions in inputoutput take a block and a file descriptor.
 The functions provided either read the file and update the Block
 accordingly, or write information from the Block out to the file.
 """
 
 from __future__ import print_function, unicode_literals
+import re
 
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
 from .core import working_block, _NameSanitizer
 from .wire import WireVector, Input, Output, Const, Register
 from .corecircuits import concat
 from .memory import RomBlock
+from .inputoutput import _name_sorted, _net_sorted
 
 
 # ----------------------------------------------------------------
 #         ___  __          __   __
 #   \  / |__  |__) | |    /  \ / _`
 #    \/  |___ |  \ | |___ \__/ \__>
 #
 
 def output_to_verilog(dest_file, block=None):
     """ A function to walk the block and output it in verilog format to the open file. """
 
     block = working_block(block)
     file = dest_file
-    internal_names = _VerilogSanitizer('_verout_tmp_')
+    internal_names = _VerilogSanitizer('_ver_out_tmp_')
 
     for wire in block.wirevector_set:
         internal_names.make_valid_string(wire.name)
 
     def varname(wire):
         return internal_names[wire.name]
 
@@ -43,15 +45,15 @@
 
 def OutputToVerilog(dest_file, block=None):
     """ A deprecated function to output verilog, use "output_to_verilog" instead. """
     return output_to_verilog(dest_file, block)
 
 
 class _VerilogSanitizer(_NameSanitizer):
-    _ver_regex = '[_A-Za-z][_a-zA-Z0-9\$]*$'
+    _ver_regex = r'[_A-Za-z][_a-zA-Z0-9\$]*$'
 
     _verilog_reserved = \
         """always and assign automatic begin buf bufif0 bufif1 case casex casez cell cmos
         config deassign default defparam design disable edge else end endcase endconfig
         endfunction endgenerate endmodule endprimitive endspecify endtable endtask
         event for force forever fork function generate genvar highz0 highz1 if ifnone
         incdir include initial inout input instance integer join large liblist library
@@ -66,17 +68,17 @@
 
     def __init__(self, internal_prefix='_sani_temp', map_valid_vals=True):
         self._verilog_reserved_set = frozenset(self._verilog_reserved.split())
         super(_VerilogSanitizer, self).__init__(self._ver_regex, internal_prefix,
                                                 map_valid_vals, self._extra_checks)
 
     def _extra_checks(self, str):
-        return(str not in self._verilog_reserved_set and  # is not a Verilog reserved keyword
-               str != 'clk' and                           # not the clock signal
-               len(str) <= 1024)                          # not too long to be a Verilog id
+        return(str not in self._verilog_reserved_set  # is not a Verilog reserved keyword
+               and str != 'clk'                       # not the clock signal
+               and len(str) <= 1024)                  # not too long to be a Verilog id
 
 
 def _verilog_vector_size_decl(n):
     return '' if n == 1 else '[{:d}:0]'.format(n - 1)
 
 
 def _verilog_vector_decl(w):
@@ -92,15 +94,15 @@
     return inputs, outputs, registers, wires, memories
 
 
 def _to_verilog_header(file, block, varname):
     """ Print the header of the verilog implementation. """
 
     def name_sorted(wires):
-        return sorted(wires, key=lambda w: varname(w))
+        return _name_sorted(wires, name_mapper=varname)
 
     def name_list(wires):
         return [varname(w) for w in wires]
 
     print('// Generated automatically via PyRTL', file=file)
     print('// As one initial test of synthesis, map to FPGA with:', file=file)
     print('//   yosys -p "synth_xilinx -top toplevel" thisfile.v\n', file=file)
@@ -119,52 +121,57 @@
     for w in name_sorted(inputs):
         print('    input{:s} {:s};'.format(_verilog_vector_decl(w), varname(w)), file=file)
     for w in name_sorted(outputs):
         print('    output{:s} {:s};'.format(_verilog_vector_decl(w), varname(w)), file=file)
     print('', file=file)
 
     # memories and registers
-    for m in memories:
+    for m in sorted(memories, key=lambda m: m.id):
         memwidth_str = _verilog_vector_size_decl(m.bitwidth)
         memsize_str = _verilog_vector_size_decl(1 << m.addrwidth)
         print('    reg{:s} mem_{}{:s}; //{}'.format(memwidth_str, m.id,
                                                     memsize_str, m.name), file=file)
-    for w in registers:
+    for w in name_sorted(registers):
         print('    reg{:s} {:s};'.format(_verilog_vector_decl(w), varname(w)), file=file)
-    print('', file=file)
+    if (memories or registers):
+        print('', file=file)
 
     # wires
-    for w in wires:
+    for w in name_sorted(wires):
         print('    wire{:s} {:s};'.format(_verilog_vector_decl(w), varname(w)), file=file)
     print('', file=file)
 
     # Write the initial values for read-only memories.
     # If we ever add support outside of simulation for initial values
     #  for MemBlocks, that would also go here.
     roms = {m for m in memories if isinstance(m, RomBlock)}
-    for m in roms:
+    for m in sorted(roms, key=lambda m: m.id):
         print('    initial begin', file=file)
         for i in range(1 << m.addrwidth):
             mem_elem_str = 'mem_{}[{:d}]'.format(m.id, i)
             mem_data_str = "{:d}'h{:x}".format(m.bitwidth, m._get_read_data(i))
             print('        {:s}={:s};'.format(mem_elem_str, mem_data_str), file=file)
         print('    end', file=file)
         print('', file=file)
 
 
 def _to_verilog_combinational(file, block, varname):
     """ Print the combinational logic of the verilog implementation. """
+
+    def name_sorted(wires):
+        return _name_sorted(wires, name_mapper=varname)
+
     print('    // Combinational', file=file)
 
     # assign constants (these could be folded for readability later)
-    for const in block.wirevector_subset(Const):
+    for const in name_sorted(block.wirevector_subset(Const)):
         print('    assign {:s} = {:d};'.format(varname(const), const.val), file=file)
 
     # walk the block and output combination logic
-    for net in block.logic:
+    for net in _net_sorted(block.logic, varname):
         if net.op in 'w~':  # unary ops
             opstr = '' if net.op == 'w' else net.op
             t = (varname(net.dests[0]), opstr, varname(net.args[0]))
             print('    assign %s = %s%s;' % t, file=file)
         elif net.op in '&|^+-*<>':  # binary ops
             t = (varname(net.dests[0]), varname(net.args[0]),
                  net.op, varname(net.args[1]))
@@ -194,41 +201,44 @@
         else:
             raise PyrtlInternalError("nets with op '{}' not supported".format(net.op))
     print('', file=file)
 
 
 def _to_verilog_sequential(file, block, varname):
     """ Print the sequential logic of the verilog implementation. """
+    if not block.logic_subset(op='r'):
+        return
+
     print('    // Registers', file=file)
     print('    always @( posedge clk )', file=file)
     print('    begin', file=file)
-    for net in block.logic:
+    for net in _net_sorted(block.logic, varname):
         if net.op == 'r':
             dest, src = (varname(net.dests[0]), varname(net.args[0]))
             print('        {:s} <= {:s};'.format(dest, src), file=file)
     print('    end', file=file)
     print('', file=file)
 
 
 def _to_verilog_memories(file, block, varname):
     """ Print the memories of the verilog implementation. """
     memories = {n.op_param[1] for n in block.logic_subset('m@')}
-    for m in memories:
+    for m in sorted(memories, key=lambda m: m.id):
         print('    // Memory mem_{}: {}'.format(m.id, m.name), file=file)
         print('    always @( posedge clk )', file=file)
         print('    begin', file=file)
-        for net in block.logic_subset('@'):
+        for net in _net_sorted(block.logic_subset('@'), varname):
             if net.op_param[1] == m:
                 t = (varname(net.args[2]), net.op_param[0],
                      varname(net.args[0]), varname(net.args[1]))
                 print(('        if (%s) begin\n'
                        '                mem_%s[%s] <= %s;\n'
                        '        end') % t, file=file)
         print('    end', file=file)
-        for net in block.logic_subset('m'):
+        for net in _net_sorted(block.logic_subset('m'), varname):
             if net.op_param[1] == m:
                 dest = varname(net.dests[0])
                 m_id = net.op_param[0]
                 index = varname(net.args[0])
                 print('    assign {:s} = mem_{}[{:s}];'.format(dest, m_id, index), file=file)
         print('', file=file)
 
@@ -239,22 +249,24 @@
 
 # ----------------------------------------------------------------
 #   ___  ___  __  ___  __   ___       __
 #    |  |__  /__`  |  |__) |__  |\ | /  ` |__|
 #    |  |___ .__/  |  |__) |___ | \| \__, |  |
 #
 
-def output_verilog_testbench(dest_file, simulation_trace=None, vcd="waveform.vcd",
-                             cmd=None, block=None):
-    """Output a verilog testbanch for the block/inputs used in the simulation trace.
+def output_verilog_testbench(dest_file, simulation_trace=None, toplevel_include=None,
+                             vcd="waveform.vcd", cmd=None, block=None):
+    """Output a Verilog testbench for the block/inputs used in the simulation trace.
 
     :param dest_file: an open file to which the test bench will be printed.
     :param simulation_trace: a simulation trace from which the inputs will be extracted
         for inclusion in the test bench.  The test bench generated will just replay the
         inputs played to the simulation cycle by cycle.
+    :param toplevel_include: name of the file containing the toplevel module this testbench
+        is testing.  If not None, an '`include' directive will be added to the top.
     :param vcd: By default the testbench generator will include a command in the testbench
         to write the output of the testbench execution to a .vcd file (via $dumpfile), and
         this parameter is the string of the name of the file to use.  If None is specified
         instead, then no dumpfile will be used.
     :param cmd: The string passed as cmd will be copied verbatim into the testbench at the
         just before the end of each cycle. This is useful for doing things like printing
         specific values out during testbench evaluation (e.g. cmd='$display("%d", out);'
@@ -279,14 +291,19 @@
 
     inputs, outputs, registers, wires, memories = _verilog_block_parts(block)
 
     ver_name = _VerilogSanitizer('_ver_out_tmp_')
     for wire in block.wirevector_set:
         ver_name.make_valid_string(wire.name)
 
+    # Output an include, if given
+    if toplevel_include:
+        print('`include "{:s}"'.format(toplevel_include), file=dest_file)
+        print('', file=dest_file)
+
     # Output header
     print('module tb();', file=dest_file)
 
     # Declare all block inputs as reg
     print('    reg clk;', file=dest_file)
     for w in inputs:
         print('    reg {:s} {:s};'.format(_verilog_vector_decl(w), ver_name[w.name]),
```

### Comparing `pyrtl-0.8.7/pyrtl/wire.py` & `pyrtl-0.9.0/pyrtl/wire.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 from __future__ import print_function, unicode_literals
 
 import numbers
 import six
 import re
+import sys
 
 from . import core  # needed for _setting_keep_wirevector_call_stack
 
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
 from .core import working_block, LogicNet, _NameIndexer
 
 # ----------------------------------------------------------------
@@ -28,21 +29,27 @@
 #
 
 
 _wvIndexer = _NameIndexer("tmp")
 _constIndexer = _NameIndexer("const_")
 
 
+def _reset_wire_indexers():
+    global _wvIndexer, _constIndexer
+    _wvIndexer = _NameIndexer("tmp")
+    _constIndexer = _NameIndexer("const_")
+
+
 def next_tempvar_name(name=""):
     if name == '':  # sadly regex checks are sometimes too slow
         wire_name = _wvIndexer.make_valid_string()
         callpoint = core._get_useful_callpoint_name()
         if callpoint:  # returns none if debug mode is false
             filename, lineno = callpoint
-            safename = re.sub('[\W]+', '', filename)  # strip out non alphanumeric characters
+            safename = re.sub(r'[\W]+', '', filename)  # strip out non alphanumeric characters
             wire_name += '_%s_line%d' % (safename, lineno)
         return wire_name
     else:
         if name.lower() in ['clk', 'clock']:
             raise PyrtlError('Clock signals should never be explicit')
         return name
 
@@ -374,17 +381,17 @@
             op_param=selectednums,
             args=(self,),
             dests=(outwire,))
         working_block().add_net(net)
         return outwire
 
     def __lshift__(self, other):
-        raise PyrtlError('Shifting using the << and >> operators are not supported'
-                         'in PyRTL.'
-                         'If you are trying to select bits in a wire, use'
+        raise PyrtlError('Shifting using the << and >> operators are not supported '
+                         'in PyRTL. '
+                         'If you are trying to select bits in a wire, use '
                          'the indexing operator (wire[indexes]) instead.\n\n'
                          'For example: wire[2:9] selects the wires from index 2 to '
                          'index 8 to make a new length 7 wire. \n\n If you are really '
                          'trying to *execution time* shift you can use "shift_left_arithmetic", '
                          '"shift_right_arithmetic", "shift_left_logical", "shift_right_logical"')
 
     __rshift__ = __lshift__
@@ -492,20 +499,35 @@
         else:
             from .corecircuits import concat
             if isinstance(extbit, int):
                 extbit = Const(extbit, bitwidth=1)
             extvector = WireVector(bitwidth=numext)
             net = LogicNet(
                 op='s',
-                op_param=(0,)*numext,
+                op_param=(0,) * numext,
                 args=(extbit,),
                 dests=(extvector,))
             working_block().add_net(net)
             return concat(extvector, self)
 
+    def as_bundle(self, obj):
+        from .helperfuncs import Bundle
+
+        bundle_bw = Bundle.get_bundle_bitwidth(obj)
+
+        if len(self) != bundle_bw:
+            raise PyrtlError(
+                "Width of wire %s (%d) does not equal width of bundle %s (%d)"
+                % (str(self.name), len(self), str(obj.name), bundle_bw)
+            )
+
+        w = Bundle(obj)
+        w <<= self
+        return w
+
 
 # -----------------------------------------------------------------------
 #  ___     ___  ___       __   ___  __           ___  __  ___  __   __   __
 # |__  \_/  |  |__  |\ | |  \ |__  |  \    \  / |__  /  `  |  /  \ |__) /__`
 # |___ / \  |  |___ | \| |__/ |___ |__/     \/  |___ \__,  |  \__/ |  \ .__/
 #
 
@@ -531,146 +553,89 @@
             'Inputs, such as "%s", cannot have values generated internally. '
             "aka they can't have other wires driving it"
             % str(self.name))
 
 
 class Output(WireVector):
     """ A WireVector type denoting outputs of a block (no readers)
+
     Even though Output seems to have valid ops such as __or__ , using
     them will throw an error.
     """
     _code = 'O'
 
     def __init__(self, bitwidth=None, name='', block=None):
         super(Output, self).__init__(bitwidth, name, block)
 
 
 class Const(WireVector):
     """ A WireVector representation of a constant value
 
-    Converts from bool, integer, or verilog-style strings to a constant
+    Converts from bool, integer, or Verilog-style strings to a constant
     of the specified bitwidth.  If the bitwidth is too short to represent
-    the specified constant then an error is raised.  If a possitive
-    integer is specified the bitwidth can be infered from the constant.
+    the specified constant, then an error is raised.  If a positive
+    integer is specified, the bitwidth can be inferred from the constant.
     If a negative integer is provided in the simulation, it is converted
     to a two's complement representation of the specified bitwidth."""
 
     _code = 'C'
 
-    def __init__(self, val, bitwidth=None, block=None):
+    def __init__(self, val, bitwidth=None, name='', signed=False, block=None):
         """ Construct a constant implementation at initialization
 
-        :param int or str val: The value for the const wirevector
+        :param int, bool, or str val: the value for the const wirevector
+        :param int: the desired bitwidth of the resulting const
+        :param signed: specify if bits should be used for twos complement
         :return: a wirevector object representing a const wire
 
         Descriptions for all parameters not listed above can be found at
         py:method:: WireVector.__init__()
+
+        For details of how constants are converted fron int, bool, and
+        strings (for verilog constants), see documentation for the
+        helper function infer_val_and_bitwidth.  Please note that a
+        a constant generated with signed=True is still just a raw bitvector
+        and all arthimetic on it is unsigned by default.  The signed=True
+        argument is only used for proper inference of WireVector size and certain
+        bitwidth sanity checks assuming a two's complement representation of
+        the constants.
         """
         self._validate_bitwidth(bitwidth)
-        num, bitwidth = _gen_val_and_bitwidth(val, bitwidth)
+        from .helperfuncs import infer_val_and_bitwidth
+        num, bitwidth = infer_val_and_bitwidth(val, bitwidth, signed)
 
         if num < 0:
             raise PyrtlInternalError(
                 'Const somehow evaluating to negative integer after checks')
         if (num >> bitwidth) != 0:
-            raise PyrtlError(
-                'error constant "%s" cannot fit in the specified %d bits'
-                % (str(num), bitwidth))
+            raise PyrtlInternalError(
+                'constant %d returned by infer_val_and_bitwidth somehow not fitting in %d bits'
+                % (num, bitwidth))
 
-        name = _constIndexer.make_valid_string() + '_' + str(val)
+        name = name if name else _constIndexer.make_valid_string() + '_' + str(val)
 
         super(Const, self).__init__(bitwidth=bitwidth, name=name, block=block)
         # add the member "val" to track the value of the constant
         self.val = num
 
     def __ilshift__(self, other):
         """ This is an illegal op for Consts. Their value is set in the __init__ function"""
         raise PyrtlError(
             'ConstWires, such as "%s", should never be assigned to with <<='
             % str(self.name))
 
     def __ior__(self, _):
-        """ This is an illegal op for Inputs. They cannot be assigned to in this way """
+        """ This is an illegal op for Consts. They cannot be assigned to in this way """
         raise PyrtlError(
             'Connection using |= operator attempted on Const. '
             'ConstWires, such as "%s", cannot have values generated internally. '
             "aka they cannot have other wires driving it"
             % str(self.name))
 
 
-def _gen_val_and_bitwidth(val, bitwidth=None):
-    if isinstance(val, bool):
-        return _convert_bool(val, bitwidth)
-    elif isinstance(val, numbers.Integral):
-        return _validate_const_int(val, bitwidth)
-    elif isinstance(val, six.string_types):
-        return _convert_verilog_str(val, bitwidth)
-    else:
-        raise PyrtlError('error, the value of Const is of an improper type, "%s"'
-                         'proper types are bool, int, and string' % type(val))
-
-
-def _convert_bool(bool_val, bitwidth=None):
-    num = int(bool_val)
-    if bitwidth is None:
-        bitwidth = 1
-    if bitwidth != 1:
-        raise PyrtlError('error, boolean has bitwidth not equal to 1')
-    return num, bitwidth
-
-
-def _validate_const_int(val, bitwidth=None):
-    if val >= 0:
-        num = val
-        # infer bitwidth if it is not specified explicitly
-        if bitwidth is None:
-            bitwidth = len(bin(num)) - 2  # the -2 for the "0b" at the start of the string
-    else:  # val is negative
-        if bitwidth is None:
-            raise PyrtlError(
-                'negative Const values must have bitwidth declared explicitly')
-        if (val >> bitwidth-1) != -1:
-            raise PyrtlError('insufficient bits for negative number')
-        num = val & ((1 << bitwidth) - 1)  # result is a twos complement value
-    return num, bitwidth
-
-
-def _convert_verilog_str(val, bitwidth=None):
-    bases = {'b': 2, 'o': 8, 'd': 10, 'h': 16, 'x': 16}
-    if bitwidth is not None:
-        raise PyrtlError('error, bitwidth parameter of const should be'
-                         ' unspecified when the const is created from a string'
-                         ' (instead use verilog style specification)')
-    neg = False
-    if val.startswith('-'):
-        neg = True
-        val = val[1:]
-    split_string = val.lower().split("'")
-    if len(split_string) != 2:
-        raise PyrtlError('error, string for Const not in verilog style format')
-    try:
-        bitwidth = int(split_string[0])
-        sval = split_string[1]
-        if sval[0] == 's':
-            raise PyrtlError('signed integers are not supported in verilog-style Const')
-        base = 10
-        if sval[0] in bases:
-            base = bases[sval[0]]
-            sval = sval[1:]
-        sval = sval.replace('_', '')
-        num = int(sval, base)
-    except (IndexError, ValueError):
-        raise PyrtlError('error, string for Const not in verilog style format')
-    if neg and num:
-        if (num >> bitwidth-1):
-            raise PyrtlError('insufficient bits for negative number')
-        num = (1 << bitwidth) - num
-    return num, bitwidth
-
-
 class Register(WireVector):
     """ A WireVector with a register state element embedded.
 
     Registers only update their outputs on posedge of an implicit
     clk signal.  The "value" in the current cycle can be accessed
     by just referencing the Register itself.  To set the value for
     the next cycle (after the next posedge) you write to the
@@ -701,15 +666,15 @@
             return self.reg._next_ilshift(other)
 
         def __ior__(self, other):
             return self.reg._next_ior(other)
 
         def __bool__(self):
             """ Use of a _next in a statement like "a or b" is forbidden."""
-            raise PyrtlError('cannot covert Register.next to compile-time boolean.  This error '
+            raise PyrtlError('cannot convert Register.next to compile-time boolean.  This error '
                              'often happens when you attempt to use a Register.next with "==" or '
                              'something that calls "__eq__", such as when you test if a '
                              'Register.next is "in" something')
 
         __nonzero__ = __bool__  # for Python 2 and 3 compatibility
 
     class _NextSetter(object):
```

### Comparing `pyrtl-0.8.7/pyrtl/inputoutput.py` & `pyrtl-0.9.0/pyrtl/inputoutput.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,36 +9,37 @@
 from __future__ import print_function, unicode_literals
 import re
 import collections
 
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
 from .core import working_block, _NameSanitizer
 from .wire import WireVector, Input, Output, Const, Register
-from .corecircuits import concat
+from .corecircuits import concat_list
 from .memory import RomBlock
+from .passes import two_way_concat, one_bit_selects
 
 
 # -----------------------------------------------------------------
 #            __       ___
 #    | |\ | |__) |  |  |
 #    | | \| |    \__/  |
 
 
-def input_from_blif(blif, block=None, merge_io_vectors=True):
+def input_from_blif(blif, block=None, merge_io_vectors=True, clock_name='clk'):
     """ Read an open blif file or string as input, updating the block appropriately
 
     Assumes the blif has been flattened and their is only a single module.
     Assumes that there is only one single shared clock and reset
     Assumes that output is generated by Yosys with formals in a particular order
     Ignores reset signal (which it assumes is input only to the flip flops)
     """
     import pyparsing
     import six
     from pyparsing import (Word, Literal, OneOrMore, ZeroOrMore,
-                           Suppress, Group, Keyword)
+                           Suppress, Group, Keyword, Optional, oneOf)
 
     block = working_block(block)
 
     try:
         blif_string = blif.read()
     except AttributeError:
         if isinstance(blif, six.string_types):
@@ -53,43 +54,51 @@
         return Suppress(Literal(x))
 
     def twire(x):
         """ find or make wire named x and return it """
         s = block.get_wirevector_by_name(x)
         if s is None:
             s = WireVector(bitwidth=1, name=x)
+        if isinstance(s, Output) and (merge_io_vectors or len(x) == 1):
+            # To allow an output wire to be used as an argument (legal in BLIF),
+            # use the intermediate wire that was created in its place. extract_outputs()
+            # creates this intermediate wire.
+            s = block.get_wirevector_by_name(x + '[0]')
         return s
 
     # Begin BLIF language definition
-    signal_start = pyparsing.alphas + '$:[]_<>\\\/'
-    signal_middle = pyparsing.alphas + pyparsing.nums + '$:[]_<>\\\/.'
+    signal_start = pyparsing.alphas + r'$:[]_<>\\\/?'
+    signal_middle = pyparsing.alphas + pyparsing.nums + r'$:[]_<>\\\/.?'
     signal_id = Word(signal_start, signal_middle)
     header = SKeyword('.model') + signal_id('model_name')
     input_list = Group(SKeyword('.inputs') + OneOrMore(signal_id))('input_list')
     output_list = Group(SKeyword('.outputs') + OneOrMore(signal_id))('output_list')
 
     cover_atom = Word('01-')
     cover_list = Group(ZeroOrMore(cover_atom))('cover_list')
     namesignal_list = Group(OneOrMore(signal_id))('namesignal_list')
     name_def = Group(SKeyword('.names') + namesignal_list + cover_list)('name_def')
 
     # asynchronous Flip-flop
-    dffas_formal = (SLiteral('C=') + signal_id('C') +
-                    SLiteral('R=') + signal_id('R') +
-                    SLiteral('D=') + signal_id('D') +
-                    SLiteral('Q=') + signal_id('Q'))
+    dffas_formal = (SLiteral('C=') + signal_id('C')
+                    + SLiteral('R=') + signal_id('R')
+                    + SLiteral('D=') + signal_id('D')
+                    + SLiteral('Q=') + signal_id('Q'))
     dffas_keyword = SKeyword('$_DFF_PN0_') | SKeyword('$_DFF_PP0_')
     dffas_def = Group(SKeyword('.subckt') + dffas_keyword + dffas_formal)('dffas_def')
 
     # synchronous Flip-flop
-    dffs_def = Group(SKeyword('.latch') +
-                     signal_id('D') +
-                     signal_id('Q') +
-                     SLiteral('re') +
-                     signal_id('C'))('dffs_def')
+    dffs_init_val = Optional(oneOf("0 1 2 3"), default=Literal("0"))
+    # TODO I think <type> and <control> ('re' and 'C') below are technically optional too
+    dffs_def = Group(SKeyword('.latch')
+                     + signal_id('D')
+                     + signal_id('Q')
+                     + SLiteral('re')
+                     + signal_id('C')
+                     + dffs_init_val('I'))('dffs_def')
     command_def = name_def | dffas_def | dffs_def
     command_list = Group(OneOrMore(command_def))('command_list')
 
     footer = SKeyword('.end')
     model_def = Group(header + input_list + output_list + command_list + footer)
     model_list = OneOrMore(model_def)
     parser = model_list.ignore(pyparsing.pythonStyleComment)
@@ -102,15 +111,15 @@
     ff_clk_set = set([])
 
     def extract_inputs(model):
         start_names = [re.sub(r'\[([0-9]+)\]$', '', x) for x in model['input_list']]
         name_counts = collections.Counter(start_names)
         for input_name in name_counts:
             bitwidth = name_counts[input_name]
-            if input_name == 'clk':
+            if input_name == clock_name:
                 clk_set.add(input_name)
             elif not merge_io_vectors or bitwidth == 1:
                 block.add_wirevector(Input(bitwidth=1, name=input_name))
             else:
                 wire_in = Input(bitwidth=bitwidth, name=input_name, block=block)
                 for i in range(bitwidth):
                     bit_name = input_name + '[' + str(i) + ']'
@@ -119,37 +128,43 @@
 
     def extract_outputs(model):
         start_names = [re.sub(r'\[([0-9]+)\]$', '', x) for x in model['output_list']]
         name_counts = collections.Counter(start_names)
         for output_name in name_counts:
             bitwidth = name_counts[output_name]
             if not merge_io_vectors or bitwidth == 1:
-                block.add_wirevector(Output(bitwidth=1, name=output_name))
+                # To allow an output wire to be used as an argument (legal in BLIF),
+                # create an intermediate wire that will be used in its place. twire()
+                # checks for this and uses the intermediate wire when needed
+                w = WireVector(bitwidth=1, name=output_name + '[0]')
+                out = Output(bitwidth=1, name=output_name)
+                out <<= w
             else:
                 wire_out = Output(bitwidth=bitwidth, name=output_name, block=block)
                 bit_list = []
                 for i in range(bitwidth):
                     bit_name = output_name + '[' + str(i) + ']'
                     bit_wire = WireVector(bitwidth=1, name=bit_name, block=block)
                     bit_list.append(bit_wire)
-                wire_out <<= concat(*bit_list)
+                wire_out <<= concat_list(bit_list)
 
     def extract_commands(model):
         # for each "command" (dff or net) in the model
         for command in model['command_list']:
             # if it is a net (specified as a cover)
             if command.getName() == 'name_def':
                 extract_cover(command)
             # else if the command is a d flop flop
             elif command.getName() == 'dffas_def' or command.getName() == 'dffs_def':
                 extract_flop(command)
             else:
                 raise PyrtlError('unknown command type')
 
     def extract_cover(command):
+        # pylint: disable=invalid-unary-operand-type
         netio = command['namesignal_list']
         if len(command['cover_list']) == 0:
             output_wire = twire(netio[0])
             output_wire <<= Const(0, bitwidth=1, block=block)  # const "FALSE"
         elif command['cover_list'].asList() == ['1']:
             output_wire = twire(netio[0])
             output_wire <<= Const(1, bitwidth=1, block=block)  # const "TRUE"
@@ -194,64 +209,107 @@
             ff_clk_set.add(command['C'])
 
         # Create register and assign next state to D and output to Q
         regname = command['Q'] + '_reg'
         flop = Register(bitwidth=1, name=regname)
         flop.next <<= twire(command['D'])
         flop_output = twire(command['Q'])
+        init_val = command['I']
+        if init_val == "1":
+            # e.g. in Verilog: `initial reg <= 1;`
+            raise PyrtlError("Initializing latches to 1 is not supported. "
+                             "Acceptable values are: 0, 2 (don't care), and 3 (unknown); "
+                             "in any case, PyRTL will ensure all stateful elements come up 0. "
+                             "For finer control over the initial value, use specialized reset "
+                             "logic.")
         flop_output <<= flop
 
     for model in result:
         extract_inputs(model)
         extract_outputs(model)
         extract_commands(model)
 
 
 # ----------------------------------------------------------------
 #    __       ___  __       ___
 #   /  \ |  |  |  |__) |  |  |
 #   \__/ \__/  |  |    \__/  |
 #
 
+
+def _natural_sort_key(key):
+    """ Convert the key into a form such that it will be sorted naturally,
+        e.g. such that "tmp4" appears before "tmp18".
+    """
+    def convert(text):
+        return int(text) if text.isdigit() else text
+    return [convert(c) for c in re.split(r'(\d+)', key)]
+
+
+def _net_sorted(logic, name_mapper=lambda w: w.name):
+    # Sort nets based on the name of the destination
+    # wire, unless it's a memory write net.
+    def natural_keys(n):
+        if n.op == '@':
+            # Sort based on the name of the wr_en wire, since
+            # this particular net is used within 'always begin ... end'
+            # blocks for memory update logic.
+            key = str(n.args[2])
+        else:
+            key = name_mapper(n.dests[0])
+        return _natural_sort_key(key)
+    return sorted(logic, key=natural_keys)
+
+
+def _name_sorted(wires, name_mapper=lambda w: w.name):
+    return sorted(wires, key=lambda w: _natural_sort_key(name_mapper(w)))
+
+
 def output_to_firrtl(open_file, rom_blocks=None, block=None):
     """ Output the block as firrtl code to the output file.
 
     Output_to_firrtl(open_file, rom_block, block)
     If rom is intialized in pyrtl code, you can pass in the rom_blocks as a list [rom1, rom2, ...]
     """
     block = working_block(block)
+
+    # FIRRTL only allows 'bits' operations to have two parameters: a high and low
+    # index representing the inclusive bounds of a contiguous range. PyRTL uses
+    # slice syntax, which aren't always contiguous, so we need to convert them.
+    one_bit_selects(block=block)  # pylint: disable=no-value-for-parameter,unexpected-keyword-arg
+
+    # FIRRTL only allows 'concatenate' operations to have two arguments,
+    # but PyRTL's 'c' op allows an arbitrary number of wires. We need to convert
+    # these n-way concats to series of two-way concats accordingly.
+    two_way_concat(block=block)  # pylint: disable=no-value-for-parameter,unexpected-keyword-arg
+
     f = open_file
     # write out all the implicit stuff
-    f.write("circuit Example : \n")
-    f.write("  module Example : \n")
+    f.write("circuit Example :\n")
+    f.write("  module Example :\n")
     f.write("    input clock : Clock\n    input reset : UInt<1>\n")
     # write out IO signals, wires and registers
-    wireRegDefs = ""
-    for wire in list(block.wirevector_subset()):
-        if type(wire) == Input:
-            f.write("    input %s : UInt<%d>\n" % (wire.name, wire.bitwidth))
-        elif type(wire) == Output:
-            f.write("    output %s : UInt<%d>\n" % (wire.name, wire.bitwidth))
-        elif type(wire) == WireVector:
-            wireRegDefs += "    wire {} : UInt<{}>\n".format(wire.name, wire.bitwidth)
-        elif type(wire) == Register:
-            wireRegDefs += "    reg {} : UInt<{}>, clock\n".format(wire.name, wire.bitwidth)
-        elif type(wire) == Const:
-            # some const is in the form like const_0_1'b1, is this legal operation?
-            wire.name = wire.name.split("'").pop(0)
-            wireRegDefs += "    node {} = UInt<{}>({})\n".format(wire.name, wire.bitwidth, wire.val)
-        else:
-            return 1
-    f.write(wireRegDefs)
+    for wire in _name_sorted(block.wirevector_subset(Input)):
+        f.write("    input %s : UInt<%d>\n" % (wire.name, wire.bitwidth))
+    for wire in _name_sorted(block.wirevector_subset(Output)):
+        f.write("    output %s : UInt<%d>\n" % (wire.name, wire.bitwidth))
+    for wire in _name_sorted(block.wirevector_subset(exclude=(Input, Output, Register, Const))):
+        f.write("    wire %s : UInt<%d>\n" % (wire.name, wire.bitwidth))
+    for wire in _name_sorted(block.wirevector_subset(Register)):
+        f.write("    reg %s : UInt<%d>, clock\n" % (wire.name, wire.bitwidth))
+    for wire in _name_sorted(block.wirevector_subset(Const)):
+        # some const is in the form like const_0_1'b1, is this legal operation?
+        wire.name = wire.name.split("'").pop(0)
+        f.write("    node %s = UInt<%d>(%d)\n" % (wire.name, wire.bitwidth, wire.val))
     f.write("\n")
 
     # write "Main"
     node_cntr = 0
     initializedMem = []
-    for log_net in list(block.logic_subset()):
+    for log_net in _net_sorted(block.logic_subset()):
         if log_net.op == '&':
             f.write("    %s <= and(%s, %s)\n" % (log_net.dests[0].name, log_net.args[0].name,
                                                  log_net.args[1].name))
         elif log_net.op == '|':
             f.write("    %s <= or(%s, %s)\n" % (log_net.dests[0].name, log_net.args[0].name,
                                                 log_net.args[1].name))
         elif log_net.op == '^':
@@ -284,24 +342,29 @@
                                                 log_net.args[1].name))
         elif log_net.op == 'w':
             f.write("    %s <= %s\n" % (log_net.dests[0].name, log_net.args[0].name))
         elif log_net.op == 'x':
             f.write("    %s <= mux(%s, %s, %s)\n" % (log_net.dests[0].name, log_net.args[0].name,
                                                      log_net.args[2].name, log_net.args[1].name))
         elif log_net.op == 'c':
+            if len(log_net.args) != 2:
+                raise PyrtlInternalError(
+                    "Expected concat net to have only two "
+                    "argument wires; has %d" % len(log_net.args)
+                )
             f.write("    %s <= cat(%s, %s)\n" % (log_net.dests[0].name, log_net.args[0].name,
                                                  log_net.args[1].name))
         elif log_net.op == 's':
-            selEnd = log_net.op_param[0]
-            if len(log_net.op_param) < 2:
-                selBegin = selEnd
-            else:
-                selBegin = log_net.op_param[len(log_net.op_param)-1]
+            if len(log_net.op_param) != 1:
+                raise PyrtlInternalError(
+                    "Expected select net to have single "
+                    "select bit; has %d" % len(log_net.op_param)
+                )
             f.write("    %s <= bits(%s, %s, %s)\n" % (log_net.dests[0].name, log_net.args[0].name,
-                                                      selBegin, selEnd))
+                                                      log_net.op_param[0], log_net.op_param[0]))
         elif log_net.op == 'r':
             f.write("    %s <= mux(reset, UInt<%s>(0), %s)\n" %
                     (log_net.dests[0].name, log_net.dests[0].bitwidth, log_net.args[0].name))
         elif log_net.op == 'm':
             # if there are rom blocks, need to be initialized
             if rom_blocks is not None:
                 if not log_net.op_param[0] in initializedMem:
@@ -351,15 +414,14 @@
                      log_net.args[0].name))
             f.write("      T_%d <= %s\n" % (node_cntr, log_net.args[1].name))
             f.write("      skip\n")
             node_cntr += 1
         else:
             pass
 
-    f.close()
     return 0
 
 
 def _trivialgraph_default_namer(thing, is_edge=True):
     """ Returns a "good" string for thing in printed graphs. """
     if is_edge:
         if thing.name is None or thing.name.startswith('tmp'):
@@ -374,25 +436,31 @@
         try:
             return thing.op + str(thing.op_param or '')
         except AttributeError:
             raise PyrtlError('no naming rule for "%s"' % str(thing))
 
 
 def net_graph(block=None, split_state=False):
-    """ Return a graph representation of the current block.
+    """ Return a graph representation of the given block.
+
+    :param block: block to use (defaults to current working block)
+    :param split_state: if True, split connections to/from a register update net; this
+        means that registers will be appear as source nodes of the network, and
+        'r' nets (i.e. the logic for setting a register's next value) will
+        be treated as sink nodes of the network
 
     Graph has the following form:
         { node1: { nodeA: edge1A, nodeB: edge1B},
           node2: { nodeB: edge2B, nodeC: edge2C},
           ...
         }
 
     aka: edge = graph[source][dest]
 
-    Each node can be either a logic net or a WireVector (e.g. an Input, and Output, a
+    Each node can be either a logic net or a WireVector (e.g. an Input, an Output, a
     Const or even an undriven WireVector (which acts as a source or sink in the network)
     Each edge is a WireVector or derived type (Input, Output, Register, etc.)
     Note that inputs, consts, and outputs will be both "node" and "edge".
     WireVectors that are not connected to any nets are not returned as part
     of the graph.
     """
     # FIXME: make it not try to add unused wires (issue #204)
@@ -412,36 +480,36 @@
     for w in dangle_set:
         graph[w] = {}
     if split_state:
         for w in block.wirevector_subset(Register):
             graph[w] = {}
 
     # add all of the edges
-    for w in (dest_set & arg_set):
+    for w in (dest_set | arg_set):
         try:
             _from = wire_src_dict[w]
         except Exception:
-            _from = w
+            _from = w  # e.g. an Input/Const
         if split_state and isinstance(w, Register):
             _from = w
 
         try:
             _to_list = wire_dst_dict[w]
         except Exception:
-            _to_list = [w]
+            _to_list = [w]  # e.g. an Output
 
         for _to in _to_list:
             graph[_from][_to] = w
 
     return graph
 
 
-def output_to_trivialgraph(file, namer=_trivialgraph_default_namer, block=None):
+def output_to_trivialgraph(file, namer=_trivialgraph_default_namer, block=None, split_state=False):
     """ Walk the block and output it in trivial graph format to the open file. """
-    graph = net_graph(block)
+    graph = net_graph(block, split_state)
     node_index_map = {}  # map node -> index
 
     # print the list of nodes
     for index, node in enumerate(graph):
         print('%d %s' % (index, namer(node, is_edge=False)), file=file)
         node_index_map[node] = index
 
@@ -452,105 +520,180 @@
         for _to in graph[_from]:
             from_index = node_index_map[_from]
             to_index = node_index_map[_to]
             edge = graph[_from][_to]
             print('%d %d %s' % (from_index, to_index, namer(edge)), file=file)
 
 
-def _graphviz_default_namer(thing, is_edge=True, is_to_splitmerge=False):
-    """ Returns a "good" graphviz label for thing. """
-    if is_edge:
-        if (thing.name is None or
-                thing.name.startswith('tmp') or
-                isinstance(thing, (Input, Output, Const, Register))):
-            name = ''
-        else:
-            name = '/'.join([thing.name, str(len(thing))])
-        penwidth = 2 if len(thing) == 1 else 6
-        arrowhead = 'none' if is_to_splitmerge else 'normal'
-        return '[label="%s", penwidth="%d", arrowhead="%s"]' % (name, penwidth, arrowhead)
+def _default_edge_namer(edge, is_to_splitmerge=False, extra_edge_info=None):
+    """
+    A function for naming an edge for use in the graphviz graph.
 
-    elif isinstance(thing, Const):
-        return '[label="%d", shape=circle, fillcolor=lightgrey]' % thing.val
-    elif isinstance(thing, (Input, Output)):
-        return '[label="%s", shape=circle, fillcolor=none]' % thing.name
-    elif isinstance(thing, Register):
-        return '[label="%s", shape=square, fillcolor=gold]' % thing.name
-    elif isinstance(thing, WireVector):
-        return '[label="", shape=circle, fillcolor=none]'
+    :param edge: the edge (i.e. WireVector or deriving class)
+    :param is_to_splitmerge: if the node to which the edge points
+                             is a select or concat operation
+    :param extra_edge_info: a map from edge to any additional data you want
+                            to print associated with it (e.g. timing data).
+    :return: a function that can be called by graph namer function you pass
+             in to block_to_graphviz_string
+    """
+
+    name = '' if edge.name is None else '/'.join([edge.name, str(len(edge))])
+    if extra_edge_info and edge in extra_edge_info:
+        # Always label an edge if present in the extra_edge_info map
+        name = name + " (" + str(extra_edge_info[edge]) + ")"
+    elif (edge.name is None
+          or edge.name.startswith('tmp')
+          or isinstance(edge, (Input, Output, Const, Register))):
+        name = ''
+
+    penwidth = 2 if len(edge) == 1 else 6
+    arrowhead = 'none' if is_to_splitmerge else 'normal'
+    return '[label="%s", penwidth="%d", arrowhead="%s"]' % (name, penwidth, arrowhead)
+
+
+def _default_node_namer(node, split_state=False, extra_node_info=None):
+    def label(v):
+        if extra_node_info and node in extra_node_info:
+            v = v + "(" + str(extra_node_info[node]) + ")"
+        return v
+
+    if isinstance(node, Const):
+        name = node.name + ': ' if not node.name.startswith('const_') else ''
+        return '[label="%s", shape=circle, fillcolor=lightgrey]' % label(name + str(node.val))
+    elif isinstance(node, Input):
+        return '[label="%s", shape=invhouse, fillcolor=coral]' % label(node.name)
+    elif isinstance(node, Output):
+        return '[label="%s", shape=house, fillcolor=lawngreen]' % label(node.name)
+    elif isinstance(node, Register):
+        return '[label="%s", shape=square, fillcolor=gold]' % label(node.name)
+    elif isinstance(node, WireVector):
+        return '[label="%s", shape=circle, fillcolor=none]' % label(node.name)
     else:
         try:
-            if thing.op == '&':
-                return '[label="and"]'
-            elif thing.op == '|':
-                return '[label="or"]'
-            elif thing.op == '^':
-                return '[label="xor"]'
-            elif thing.op == '~':
-                return '[label="not"]'
-            elif thing.op == 'x':
-                return '[label="mux"]'
-            elif thing.op in 'sc':
-                return '[label="", height=.1, width=.1]'
-            elif thing.op == 'r':
-                name = thing.dests[0].name or ''
-                return '[label="%s.next", shape=square, fillcolor=gold]' % name
-            elif thing.op == 'w':
-                return '[label="buf"]'
+            if node.op == '&':
+                return '[label="%s"]' % label("and")
+            elif node.op == '|':
+                return '[label="%s"]' % label("or")
+            elif node.op == '^':
+                return '[label="%s"]' % label("xor")
+            elif node.op == '~':
+                return '[label="%s", shape=invtriangle]' % label("not")
+            elif node.op == 'x':
+                return '[label="%s", shape=invtrapezium]' % label("mux")
+            elif node.op == 's':
+                selEnd = node.op_param[0]
+                if len(node.op_param) < 2:
+                    selBegin = selEnd
+                else:
+                    selBegin = node.op_param[len(node.op_param) - 1]
+                return '[label="%s", height=.1, width=.1]' % \
+                    (label("bits(%s,%s)" % (selBegin, selEnd)))
+            elif node.op in 'c':
+                return '[label="%s", height=.1, width=.1]' % label("concat")
+            elif node.op == 'r':
+                name = node.dests[0].name or ''
+                name = ("%s.next" % name) if split_state else name
+                return '[label="%s", shape=square, fillcolor=gold]' % label(name)
+            elif node.op == 'w':
+                return '[label="%s", height=.1, width=.1]' % label("")
             else:
-                return '[label="%s"]' % (thing.op + str(thing.op_param or ''))
+                return '[label="%s"]' % label(node.op + str(node.op_param or ''))
         except AttributeError:
-            raise PyrtlError('no naming rule for "%s"' % str(thing))
+            raise PyrtlError('no naming rule for "%s"' % str(node))
+
+
+def graphviz_default_namer(
+        thing,
+        is_edge,
+        is_to_splitmerge,
+        split_state,
+        node_namer=_default_node_namer,
+        edge_namer=_default_edge_namer):
+    """ Returns a "good" graphviz label for thing. """
+    if is_edge:
+        return edge_namer(thing, is_to_splitmerge=is_to_splitmerge)
+    else:
+        return node_namer(thing, split_state=split_state)
 
 
-def output_to_graphviz(file, namer=_graphviz_default_namer, block=None):
+def graphviz_detailed_namer(
+        extra_node_info=None,
+        extra_edge_info=None):
+    """ Returns a detailed namer that prints extra information about nodes/edges in the given maps
+
+        :param extra_node_info: A map from node to some object about that node
+                                (its string representation will be printed next to the node's label)
+        :param extra_edge_info: A map from edge to some object about that edge
+                                (its string representation will be printed next to the edge's label)
+        :return: a function that can be used as the namer function for block_to_graphviz_string
+    """
+
+    def node_namer(node, split_state):
+        return _default_node_namer(node, split_state, extra_node_info)
+
+    def edge_namer(edge, is_to_splitmerge):
+        return _default_edge_namer(edge, is_to_splitmerge, extra_edge_info)
+
+    def namer(thing, is_edge, is_to_splitmerge, split_state):
+        return graphviz_default_namer(
+            thing, is_edge, is_to_splitmerge, split_state,
+            node_namer=node_namer, edge_namer=edge_namer)
+    return namer
+
+
+def output_to_graphviz(file, namer=graphviz_default_namer, block=None, split_state=True):
     """ Walk the block and output it in graphviz format to the open file. """
-    print(block_to_graphviz_string(block, namer), file=file)
+    print(block_to_graphviz_string(block, namer, split_state), file=file)
 
 
-def block_to_graphviz_string(block=None, namer=_graphviz_default_namer):
+def block_to_graphviz_string(block=None, namer=graphviz_default_namer, split_state=True):
     """ Return a graphviz string for the block. """
-    graph = net_graph(block, split_state=True)
+    graph = net_graph(block, split_state)
     node_index_map = {}  # map node -> index
 
     rstring = """\
               digraph g {\n
               graph [splines="spline"];
               node [shape=circle, style=filled, fillcolor=lightblue1,
-                    fontcolor=grey, fontname=helvetica, penwidth=0,
+                    fontcolor=black, fontname=helvetica, penwidth=0,
                     fixedsize=true];
               edge [labelfloat=false, penwidth=2, color=deepskyblue, arrowsize=.5];
               """
 
     # print the list of nodes
     for index, node in enumerate(graph):
-        label = namer(node, is_edge=False)
+        label = namer(node, False, False, split_state)
         rstring += '    n%s %s;\n' % (index, label)
         node_index_map[node] = index
 
     # print the list of edges
     for _from in graph:
         for _to in graph[_from]:
             from_index = node_index_map[_from]
             to_index = node_index_map[_to]
             edge = graph[_from][_to]
             is_to_splitmerge = True if hasattr(_to, 'op') and _to.op in 'cs' else False
-            label = namer(edge, is_to_splitmerge=is_to_splitmerge)
+            label = namer(edge, True, is_to_splitmerge, False)
             rstring += '   n%d -> n%d %s;\n' % (from_index, to_index, label)
 
     rstring += '}\n'
     return rstring
 
 
-def block_to_svg(block=None):
+def output_to_svg(file, block=None, split_state=True):
+    """ Output the block as an SVG to the open file. """
+    print(block_to_svg(block, split_state), file=file)
+
+
+def block_to_svg(block=None, split_state=True):
     """ Return an SVG for the block. """
-    block = working_block(block)
     try:
         from graphviz import Source
-        return Source(block_to_graphviz_string())._repr_svg_()
+        return Source(block_to_graphviz_string(block, split_state=split_state))._repr_svg_()
     except ImportError:
         raise PyrtlError('need graphviz installed (try "pip install graphviz")')
 
 
 def trace_to_html(simtrace, trace_list=None, sortkey=None):
     """ Return a HTML block showing the trace. """
 
@@ -570,15 +713,15 @@
         <script type="WaveDrom">
         { signal : [
         %s
         ]}
         </script>
 
         """
-        )
+    )
 
     def extract(w):
         wavelist = []
         datalist = []
         last = None
         for i, value in enumerate(trace[w]):
             if last == value:
```

### Comparing `pyrtl-0.8.7/pyrtl/transform.py` & `pyrtl-0.9.0/pyrtl/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,19 @@
 
 def net_transform(transform_func, block=None, **kwargs):
     """
     Maps nets to new sets of nets according to a custom function
 
     :param transform_func:
         Function signature: func(orig_net (logicnet)) -> keep_orig_net (bool)
+    :param block: optional block to work on (defaults to working block)
     :return:
+
+    If transform_func does not return True, the original net is removed from
+    the block's logic set. The net's argument wire/destination wires are not removed.
     """
     block = working_block(block)
     with set_working_block(block, True):
         for net in block.logic.copy():
             keep_orig_net = transform_func(net, **kwargs)
             if not keep_orig_net:
                 block.logic.remove(net)
@@ -138,15 +142,15 @@
         if len(net_.dests) == 1:
             src_nets[net_.dests[0]] = net_
         block.add_net(new_net)
 
     # src and dst in this function are all relative to wires
     block = working_block(block)
     if new_src is not orig_wire and orig_wire in src_nets:
-        # don't need to add the new_src and new_dst because they were made added at creation
+        # don't need to add the new_src and new_dst because they were made at creation
         net = src_nets[orig_wire]
         new_net = LogicNet(
             op=net.op, op_param=net.op_param, args=net.args,
             dests=tuple(new_src if w is orig_wire else w for w in net.dests))
         remove_net(net)
         add_net(new_net)
 
@@ -164,22 +168,24 @@
 
 
 def clone_wire(old_wire, name=None):
     """
     Makes a copy of any existing wire
 
     :param old_wire: The wire to clone
-    :param name: a name fo rhte new wire
+    :param name: a name for the new wire
 
     Note that this function is mainly intended to be used when the
     two wires are from different blocks. Making two wires with the
     same name in the same block is not allowed
     """
     if isinstance(old_wire, Const):
-        return Const(old_wire.val, old_wire.bitwidth)
+        if name is None:
+            return Const(old_wire.val, old_wire.bitwidth, name=old_wire.name)
+        return Const(old_wire.val, old_wire.bitwidth, name=name)
     else:
         if name is None:
             return old_wire.__class__(old_wire.bitwidth, name=old_wire.name)
         return old_wire.__class__(old_wire.bitwidth, name=name)
 
 
 def copy_block(block=None, update_working_block=True):
```

### Comparing `pyrtl-0.8.7/pyrtl/compilesim.py` & `pyrtl-0.9.0/pyrtl/compilesim.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,52 +3,43 @@
 import ctypes
 import subprocess
 import tempfile
 import shutil
 import collections
 from os import path
 import platform
+import sys
 import _ctypes
 
 from .core import working_block
 from .wire import Input, Output, Const, WireVector, Register
-from .memory import RomBlock
+from .memory import MemBlock, RomBlock
 from .pyrtlexceptions import PyrtlError, PyrtlInternalError
-from .simulation import SimulationTrace
+from .simulation import SimulationTrace, _trace_sort_key
 
 
 __all__ = ['CompiledSimulation']
 
 
 class DllMemInspector(collections.Mapping):
-    """Dictionary-like access to a memory array in a CompiledSimulation."""
+    """Dictionary-like access to a hashmap in a CompiledSimulation."""
 
     def __init__(self, sim, mem):
         self._aw = mem.addrwidth
-        bw = mem.bitwidth
-        self._limbs = limbs = sim._limbs(mem)
+        self._limbs = sim._limbs(mem)
         self._vn = vn = sim.varname[mem]
-        if bw <= 8:
-            scalar = ctypes.c_uint8
-        elif bw <= 16:
-            scalar = ctypes.c_uint16
-        elif bw <= 32:
-            scalar = ctypes.c_uint32
-        else:
-            scalar = ctypes.c_uint64
-        array_type = scalar*(len(self)*limbs)
-        self._buf = array_type.in_dll(sim._dll, vn)
+        self._mem = ctypes.c_void_p.in_dll(sim._dll, vn)
         self._sim = sim  # keep reference to avoid freeing dll
 
     def __getitem__(self, ind):
+        arr = self._sim._mem_lookup(self._mem, ind)
         val = 0
-        limbs = self._limbs
-        for n in reversed(range(ind*limbs, (ind+1)*limbs)):
+        for n in reversed(range(self._limbs)):
             val <<= 64
-            val |= self._buf[n]
+            val |= arr[n]
         return val
 
     def __iter__(self):
         return iter(range(len(self)))
 
     def __len__(self):
         return 1 << self._aw
@@ -59,22 +50,20 @@
                 return True
         return all(self[x] == other.get(x, 0) for x in self)
 
 
 class CompiledSimulation(object):
     """Simulate a block, compiling to C for efficiency.
 
-    THIS IS AN EXPERIMENTAL SIMULATION CLASS.
-    NO SUPPORT WILL BE GIVEN TO PEOPLE WHO CANNOT GET IT TO RUN.
-    EXPECT THE API TO CHANGE IN THE FUTURE.
-
     This module provides significant speed improvements over FastSimulation,
     at the cost of somewhat longer setup time.
     Generally this will do better than FastSimulation for simulations requiring over 1000 steps.
     It is not built to be a debugging tool, though it may help with debugging.
+    Note that only Input and Output wires can be traced using CompiledSimulation.  This code
+    is still experimental, but has been used on designs of significant scale to good effect.
 
     In order to use this, you need:
         - A 64-bit processor
         - GCC (tested on version 4.8.4)
         - A 64-bit build of Python
     If using the multiplication operand, only some architectures are supported:
         - x86-64 / amd64
@@ -98,14 +87,15 @@
 
         self.default_value = default_value
         self._regmap, self._memmap = register_value_map, memory_value_map
         self._uid_counter = 0
         self.varname = {}  # mapping from wires and memories to C variables
 
         self._create_dll()
+        self._initialize_mems()
 
     def inspect_mem(self, mem):
         """Get a view into the contents of a MemBlock."""
         return DllMemInspector(self, mem)
 
     def inspect(self, w):
         """Get the latest value of the wire given, if possible."""
@@ -124,46 +114,156 @@
     def step(self, inputs):
         """Run one step of the simulation.
 
         The argument is a mapping from input names to the values for the step.
         """
         self.run([inputs])
 
+    def step_multiple(self, provided_inputs={}, expected_outputs={}, nsteps=None,
+                      file=sys.stdout, stop_after_first_error=False):
+        """ Take the simulation forward N cycles, where N is the number of values
+         for each provided input.
+
+        :param provided_inputs: a dictionary mapping wirevectors to their values for N steps
+        :param expected_outputs: a dictionary mapping wirevectors to their expected values
+            for N steps
+        :param nsteps: number of steps to take (defaults to None, meaning step for each
+            supplied input value)
+        :param file: where to write the output (if there are unexpected outputs detected)
+        :param stop_after_first_error: a boolean flag indicating whether to stop the simulation
+            after the step where the first errors are encountered (defaults to False)
+
+        All input wires must be in the provided_inputs in order for the simulation
+        to accept these values. Additionally, the length of the array of provided values for each
+        input must be the same.
+
+        When 'nsteps' is specified, then it must be *less than or equal* to the number of values
+        supplied for each input when 'provided_inputs' is non-empty. When 'provided_inputs' is
+        empty (which may be a legitimate case for a design that takes no inputs), then 'nsteps'
+        will be used.  When 'nsteps' is not specified, then the simulation will take the number
+        of steps equal to the number of values supplied for each input.
+
+        Example: if we have inputs named 'a' and 'b' and output 'o', we can call:
+        sim.step_multiple({'a': [0,1], 'b': [23,32]}, {'o': [42, 43]}) to simulate 2 cycles,
+        where in the first cycle 'a' and 'b' take on 0 and 23, respectively, and 'o' is expected to
+        have the value 42, and in the second cycle 'a' and 'b' take on 1 and 32, respectively, and
+        'o' is expected to have the value 43.
+
+        If your values are all single digit, you can also specify them in a single string, e.g.
+        sim.step_multiple({'a': '01', 'b': '01'}) will simulate 2 cycles, with 'a' and 'b' taking on
+        0 and 0, respectively, on the first cycle and '1' and '1', respectively, on the second
+        cycle.
+
+        Example: if the design had no inputs, like so:
+
+            a = pyrtl.Register(8)
+            b = pyrtl.Output(8, 'b')
+
+            a.next <<= a + 1
+            b <<= a
+
+            sim = pyrtl.Simulation()
+            sim.step_multiple(nsteps=3)
+
+        Using sim.step_multiple(nsteps=3) simulates 3 cycles, after which we would expect the value
+        of 'b' to be 2.
+
+        """
+
+        if not nsteps and len(provided_inputs) == 0:
+            raise PyrtlError('need to supply either input values or a number of steps to simulate')
+
+        if len(provided_inputs) > 0:
+            longest = sorted(list(provided_inputs.items()),
+                             key=lambda t: len(t[1]),
+                             reverse=True)[0]
+            msteps = len(longest[1])
+            if nsteps:
+                if (nsteps > msteps):
+                    raise PyrtlError('nsteps is specified but is greater than the '
+                                     'number of values supplied for each input')
+            else:
+                nsteps = msteps
+
+        if nsteps < 1:
+            raise PyrtlError("must simulate at least one step")
+
+        if list(filter(lambda l: len(l) < nsteps, provided_inputs.values())):
+            raise PyrtlError(
+                "must supply a value for each provided wire "
+                "for each step of simulation")
+
+        if list(filter(lambda l: len(l) < nsteps, expected_outputs.values())):
+            raise PyrtlError(
+                "any expected outputs must have a supplied value "
+                "each step of simulation")
+
+        failed = []
+        for i in range(nsteps):
+            self.step({w: int(v[i]) for w, v in provided_inputs.items()})
+
+            for expvar in expected_outputs.keys():
+                expected = int(expected_outputs[expvar][i])
+                actual = self.inspect(expvar)
+                if expected != actual:
+                    failed.append((i, expvar, expected, actual))
+
+            if failed and stop_after_first_error:
+                break
+
+        if failed:
+            if stop_after_first_error:
+                s = "(stopped after step with first error):"
+            else:
+                s = "on one or more steps:"
+            file.write("Unexpected output " + s + "\n")
+            file.write("{0:>5} {1:>10} {2:>8} {3:>8}\n"
+                       .format("step", "name", "expected", "actual"))
+
+            def _sort_tuple(t):
+                # Sort by step and then wire name
+                return (t[0], _trace_sort_key(t[1]))
+
+            failed_sorted = sorted(failed, key=_sort_tuple)
+            for (step, name, expected, actual) in failed_sorted:
+                file.write("{0:>5} {1:>10} {2:>8} {3:>8}\n".format(step, name, expected, actual))
+            file.flush()
+
     def run(self, inputs):
         """Run many steps of the simulation.
 
-        The argument is a list of input mappings for each step,
-        and its length is the number of steps to be executed.
+        :param inputs: A list of input mappings for each step;
+          its length is the number of steps to be executed.
         """
         steps = len(inputs)
         # create i/o arrays of the appropriate length
-        ibuf_type = ctypes.c_uint64*(steps*self._ibufsz)
-        obuf_type = ctypes.c_uint64*(steps*self._obufsz)
+        ibuf_type = ctypes.c_uint64 * (steps * self._ibufsz)
+        obuf_type = ctypes.c_uint64 * (steps * self._obufsz)
         ibuf = ibuf_type()
         obuf = obuf_type()
         # these array will be passed to _crun
         self._crun.argtypes = [ctypes.c_uint64, ibuf_type, obuf_type]
 
         # build the input array
         for n, inmap in enumerate(inputs):
             for w in inmap:
                 if isinstance(w, WireVector):
                     name = w.name
                 else:
                     name = w
                 start, count = self._inputpos[name]
-                start += n*self._ibufsz
+                start += n * self._ibufsz
                 val = inmap[w]
                 if val >= 1 << self._inputbw[name]:
                     raise PyrtlError(
                         'Wire {} has value {} which cannot be represented '
                         'using its bitwidth'.format(name, val))
                 # pack input
-                for pos in range(start, start+count):
-                    ibuf[pos] = val & ((1 << 64)-1)
+                for pos in range(start, start + count):
+                    ibuf[pos] = val & ((1 << 64) - 1)
                     val >>= 64
 
         # run the simulation
         self._crun(steps, ibuf, obuf)
 
         # save traced wires
         for name in self.tracer.trace:
@@ -176,15 +276,15 @@
                 buf, sz = ibuf, self._ibufsz
             else:
                 raise PyrtlInternalError('Untraceable wire in tracer')
             res = []
             for n in range(steps):
                 val = 0
                 # unpack output
-                for pos in reversed(range(start, start+count)):
+                for pos in reversed(range(start, start + count)):
                     val <<= 64
                     val |= buf[pos]
                 res.append(val)
                 start += sz
             self.tracer.trace[name].extend(res)
 
     def _traceable(self, wv):
@@ -211,42 +311,46 @@
         self.tracer._wires = {wv.name: wv for wv in wvs}
         self.tracer.trace.__init__(wvs)
 
     def _create_dll(self):
         """Create a dynamically-linked library implementing the simulation logic."""
         self._dir = tempfile.mkdtemp()
         with open(path.join(self._dir, 'pyrtlsim.c'), 'w') as f:
-            self._create_code(lambda s: f.write(s+'\n'))
+            self._create_code(lambda s: f.write(s + '\n'))
         if platform.system() == 'Darwin':
             shared = '-dynamiclib'
         else:
             shared = '-shared'
-        subprocess.check_call([
-            'gcc', '-O0', '-march=native', '-std=c99', '-m64',
-            shared, '-fPIC',
-            path.join(self._dir, 'pyrtlsim.c'), '-o', path.join(self._dir, 'pyrtlsim.so'),
-            ], shell=(platform.system() == 'Windows'))
+        subprocess.check_call(['gcc', '-O0', '-march=native', '-std=c99', '-m64',
+                               shared, '-fPIC',
+                               path.join(self._dir, 'pyrtlsim.c'),
+                               '-o', path.join(self._dir, 'pyrtlsim.so'), ],
+                              shell=(platform.system() == 'Windows'))
         self._dll = ctypes.CDLL(path.join(self._dir, 'pyrtlsim.so'))
         self._crun = self._dll.sim_run_all
         self._crun.restype = None  # argtypes set on use
+        self._initialize_mems = self._dll.initialize_mems
+        self._initialize_mems.restype = None
+        self._mem_lookup = self._dll.lookup
+        self._mem_lookup.restype = ctypes.POINTER(ctypes.c_uint64)
 
     def _limbs(self, w):
         """Number of 64-bit words needed to store value of wire."""
-        return (w.bitwidth+63)//64
+        return (w.bitwidth + 63) // 64
 
     def _makeini(self, w, v):
         """C initializer string for a wire with a given value."""
         pieces = []
-        for n in range(self._limbs(w)):
-            pieces.append(hex(v & ((1 << 64)-1)))
+        for _ in range(self._limbs(w)):
+            pieces.append(hex(v & ((1 << 64) - 1)))
             v >>= 64
         return ','.join(pieces).join('{}')
 
-    def _memwidth(self, m):
-        """Bitwidth of integer type sufficient to hold memory entry.
+    def _romwidth(self, m):
+        """Bitwidth of integer type sufficient to hold rom entry.
 
         On large memories, returns 64; an array will be needed.
         """
         if m.bitwidth <= 8:
             return 8
         if m.bitwidth <= 16:
             return 16
@@ -256,61 +360,70 @@
 
     def _makemask(self, dest, res, pos):
         """Create a bitmask.
 
         The value being masked is of width `res`.
         Limb number `pos` of `dest` is being assigned to.
         """
-        if (res is None or dest.bitwidth < res) and 0 < (dest.bitwidth - 64*pos) < 64:
-            return '&0x{:X}'.format((1 << (dest.bitwidth % 64))-1)
+        if (res is None or dest.bitwidth < res) and 0 < (dest.bitwidth - 64 * pos) < 64:
+            return '&0x{:X}'.format((1 << (dest.bitwidth % 64)) - 1)
         return ''
 
     def _getarglimb(self, arg, n):
         """Get the nth limb of the given wire.
 
         Returns '0' when the wire does not have sufficient limbs.
         """
-        return '{vn}[{n}]'.format(vn=self.varname[arg], n=n) if arg.bitwidth > 64*n else '0'
+        return '{vn}[{n}]'.format(vn=self.varname[arg], n=n) if arg.bitwidth > 64 * n else '0'
 
     def _clean_name(self, prefix, obj):
         """Create a C variable name with the given prefix based on the name of obj."""
         return '{}{}_{}'.format(prefix, self._uid(), ''.join(c for c in obj.name if c.isalnum()))
 
     def _uid(self):
         """Get an auto-incrementing number suitable for use as a unique identifier."""
         x = self._uid_counter
         self._uid_counter += 1
         return x
 
-    def _declare_mem(self, write, mem):
-        self.varname[mem] = vn = self._clean_name('m', mem)
-        if isinstance(mem, RomBlock):
+    def _declare_roms(self, write, roms):
+        for mem in roms:
+            self.varname[mem] = vn = self._clean_name('m', mem)
             # extract data from mem
             romval = [mem._get_read_data(n) for n in range(1 << mem.addrwidth)]
             write('static const uint{width}_t {name}[][{limbs}] = {{'.format(
-                name=vn, width=self._memwidth(mem), limbs=self._limbs(mem)))
+                name=vn, width=self._romwidth(mem), limbs=self._limbs(mem)))
             for rv in romval:
-                write(self._makeini(mem, rv)+',')
+                write(self._makeini(mem, rv) + ',')
             write('};')
-        else:
+
+    def _declare_mems(self, write, mems):
+        for mem in mems:
+            self.varname[mem] = vn = self._clean_name('m', mem)
             write('EXPORT')
+            write('hashmap_t *{name};'.format(name=vn))
+
+        next_tmp = 0
+        write('EXPORT')
+        write('void initialize_mems() {')
+        for mem in mems:
+            # Create hashmap
+            write('{name} = create_hash_map(256, {limbs});'.format(
+                name=self.varname[mem], limbs=self._limbs(mem)
+            ))
             if mem in self._memmap:
-                highest = min(1 << mem.addrwidth, max(self._memmap[mem])+1)
-                memval = [self._memmap[mem].get(n, 0) for n in range(highest)]
-                write('uint{width}_t {name}[{size}][{limbs}] = {{'.format(
-                    name=vn, width=self._memwidth(mem),
-                    size=1 << mem.addrwidth, limbs=self._limbs(mem)))
-                for mv in memval:
-                    write(self._makeini(mem, mv)+',')
-                write('};')
-            else:
-                # initialize to zero by default
-                write('uint{width}_t {name}[{size}][{limbs}] = {{{{0}}}};'.format(
-                    name=vn, width=self._memwidth(mem),
-                    size=1 << mem.addrwidth, limbs=self._limbs(mem)))
+                # Insert default values
+                for k, v in self._memmap[mem].items():
+                    write('val_t t{n}[] = {val};'.format(
+                        n=next_tmp, val=self._makeini(mem, v)))
+                    write('insert({name}, {key}, t{n});'.format(
+                        name=self.varname[mem], key=k, n=next_tmp
+                    ))
+                    next_tmp += 1
+        write('}')
 
     def _declare_wv(self, write, w):
         self.varname[w] = vn = self._clean_name('w', w)
         if isinstance(w, Const):
             write('const uint64_t {name}[{limbs}] = {val};'.format(
                 limbs=self._limbs(w), name=vn, val=self._makeini(w, w.val)))
         elif isinstance(w, Register):
@@ -319,17 +432,22 @@
                 val=self._makeini(w, self._regmap.get(w, self.default_value))))
         else:
             write('uint64_t {name}[{limbs}];'.format(limbs=self._limbs(w), name=vn))
 
     def _build_memread(self, write, op, param, args, dest):
         mem = param[1]
         for n in range(self._limbs(dest)):
-            write('{dest}[{n}] = {mem}[{addr}[0]][{n}]{mask};'.format(
-                dest=self.varname[dest], n=n, mem=self.varname[mem],
-                addr=self.varname[args[0]], mask=self._makemask(dest, mem.bitwidth, n)))
+            if isinstance(mem, RomBlock):
+                write('{dest}[{n}] = {mem}[{addr}[0]][{n}]{mask};'.format(
+                    dest=self.varname[dest], n=n, mem=self.varname[mem],
+                    addr=self.varname[args[0]], mask=self._makemask(dest, mem.bitwidth, n)))
+            else:
+                write('{dest}[{n}] = lookup({mem}, {addr}[0])[{n}]{mask};'.format(
+                    dest=self.varname[dest], n=n, mem=self.varname[mem],
+                    addr=self.varname[args[0]], mask=self._makemask(dest, mem.bitwidth, n)))
 
     def _build_wire(self, write, op, param, args, dest):
         for n in range(self._limbs(dest)):
             write('{dest}[{n}] = {arg}[{n}]{mask};'.format(
                 dest=self.varname[dest], n=n, arg=self.varname[args[0]],
                 mask=self._makemask(dest, args[0].bitwidth, n)))
 
@@ -393,15 +511,15 @@
         write('carry = 0;')
         for n in range(self._limbs(dest)):
             arg0 = self._getarglimb(args[0], n)
             arg1 = self._getarglimb(args[1], n)
             write('tmp = {arg0}+{arg1};'.format(arg0=arg0, arg1=arg1))
             write('{dest}[{n}] = (tmp + carry){mask};'.format(
                 dest=self.varname[dest], n=n,
-                mask=self._makemask(dest, max(args[0].bitwidth, args[1].bitwidth)+1, n)))
+                mask=self._makemask(dest, max(args[0].bitwidth, args[1].bitwidth) + 1, n)))
             write('carry = (tmp < {arg0})|({dest}[{n}] < tmp);'.format(
                 arg0=arg0, dest=self.varname[dest], n=n))
 
     def _build_sub(self, write, op, param, args, dest):
         write('carry = 0;')
         for n in range(self._limbs(dest)):
             arg0 = self._getarglimb(args[0], n)
@@ -415,67 +533,149 @@
     def _build_mul(self, write, op, param, args, dest):
         for n in range(self._limbs(dest)):
             write('{dest}[{n}] = 0;'.format(dest=self.varname[dest], n=n))
         for p0 in range(self._limbs(args[0])):
             write('carry = 0;')
             arg0 = self._getarglimb(args[0], p0)
             for p1 in range(self._limbs(args[1])):
-                if self._limbs(dest) <= p0+p1:
+                if self._limbs(dest) <= p0 + p1:
                     break
                 arg1 = self._getarglimb(args[1], p1)
                 write('mul128({arg0}, {arg1}, tmplo, tmphi);'.format(arg0=arg0, arg1=arg1))
-                write('tmp = {dest}[{p}];'.format(dest=self.varname[dest], p=p0+p1))
+                write('tmp = {dest}[{p}];'.format(dest=self.varname[dest], p=p0 + p1))
                 write('tmplo += carry; carry = tmplo < carry; tmplo += tmp;')
                 write('tmphi += carry + (tmplo < tmp); carry = tmphi;')
                 write('{dest}[{p}] = tmplo{mask};'.format(
-                    dest=self.varname[dest], p=p0+p1,
-                    mask=self._makemask(dest, args[0].bitwidth+args[1].bitwidth, p0+p1)))
-            if self._limbs(dest) > p0+self._limbs(args[1]):
+                    dest=self.varname[dest], p=p0 + p1,
+                    mask=self._makemask(dest, args[0].bitwidth + args[1].bitwidth, p0 + p1)))
+            if self._limbs(dest) > p0 + self._limbs(args[1]):
                 write('{dest}[{p}] = carry{mask};'.format(
-                    dest=self.varname[dest], p=p0+self._limbs(args[1]),
+                    dest=self.varname[dest], p=p0 + self._limbs(args[1]),
                     mask=self._makemask(
-                        dest, args[0].bitwidth+args[1].bitwidth, p0+self._limbs(args[1]))))
+                        dest, args[0].bitwidth + args[1].bitwidth, p0 + self._limbs(args[1]))))
 
     def _build_concat(self, write, op, param, args, dest):
         cattotal = sum(x.bitwidth for x in args)
         pieces = (
-            (self.varname[a], l, 0, min(64, a.bitwidth-64*l))
-            for a in reversed(args) for l in range(self._limbs(a)))
+            (self.varname[a], lx, 0, min(64, a.bitwidth - 64 * lx))
+            for a in reversed(args) for lx in range(self._limbs(a)))
         curr = next(pieces)
         for n in range(self._limbs(dest)):
             res = []
             dpos = 0
             while True:
                 arg, alimb, astart, asize = curr
                 res.append('(({arg}[{limb}]>>{start})<<{pos})'.format(
                     arg=arg, limb=alimb, start=astart, pos=dpos))
                 dpos += asize
-                if dpos >= dest.bitwidth-64*n:
+                if dpos >= dest.bitwidth - 64 * n:
                     break
                 if dpos > 64:
-                    curr = (arg, alimb, 64-(dpos-asize), dpos-64)
+                    curr = (arg, alimb, 64 - (dpos - asize), dpos - 64)
                     break
                 curr = next(pieces)
                 if dpos == 64:
                     break
             write('{dest}[{n}] = ({res}){mask};'.format(
                 dest=self.varname[dest], n=n, res='|'.join(res),
                 mask=self._makemask(dest, cattotal, n)))
 
     def _build_select(self, write, op, param, args, dest):
         for n in range(self._limbs(dest)):
             bits = [
                 '((1&({src}[{limb}]>>{sb}))<<{db})'.format(
-                    src=self.varname[args[0]], sb=(b % 64), limb=(b//64), db=en)
-                for en, b in enumerate(param[64*n:min(dest.bitwidth, 64*(n+1))])]
+                    src=self.varname[args[0]], sb=(b % 64), limb=(b // 64), db=en)
+                for en, b in enumerate(param[64 * n:min(dest.bitwidth, 64 * (n + 1))])]
             write('{dest}[{n}] = {bits};'.format(
                 dest=self.varname[dest], n=n, bits='|'.join(bits)))
 
+    def _declare_mem_helpers(self, write):
+        helpers = '''
+            typedef uint64_t val_t;
+
+            typedef struct node
+            {
+                uint64_t key;
+                val_t *val;
+                struct node *next;
+            } node_t;
+
+            typedef struct hashmap
+            {
+                int size;
+                int val_limbs;
+                val_t *default_value;
+                node_t **list;
+            } hashmap_t;
+
+            hashmap_t *create_hash_map(int size, int val_limbs)
+            {
+                int i;
+                hashmap_t *h = (hashmap_t *) malloc(sizeof(hashmap_t));
+                h->size = size;
+                h->val_limbs = val_limbs;
+                h->list = (node_t **) malloc(sizeof(node_t *) * size);
+                h->default_value = (val_t *) malloc(sizeof(val_t) * val_limbs);
+                for (i = 0; i < val_limbs; i++)
+                    h->default_value[i] = 0;
+                for (i = 0; i < size; i++)
+                    h->list[i] = NULL;
+                return h;
+            }
+
+            int hash_code(hashmap_t *h, uint64_t key)
+            {
+                return key % h->size;
+            }
+
+            void insert(hashmap_t *h, uint64_t key, val_t val[])
+            {
+                int pos = hash_code(h, key);
+                struct node *list = h->list[pos];
+                struct node *new_node = (node_t *) malloc(sizeof(node_t));
+                struct node *temp = list;
+                while (temp)
+                {
+                    if (temp->key == key)
+                    {
+                        memcpy(temp->val, val, sizeof(val_t) * h->val_limbs);
+                        return;
+                    }
+                    temp = temp->next;
+                }
+                new_node->key = key;
+                new_node->val = (val_t *) malloc(sizeof(val_t) * h->val_limbs);
+                memcpy(new_node->val, val, sizeof(val_t) * h->val_limbs);
+                new_node->next = list;
+                h->list[pos] = new_node;
+            }
+
+            EXPORT
+            val_t* lookup(hashmap_t *h, uint64_t key)
+            {
+                int pos = hash_code(h, key);
+                node_t *list = h->list[pos];
+                node_t *temp = list;
+                while (temp)
+                {
+                    if (temp->key == key)
+                    {
+                        return temp->val;
+                    }
+                    temp = temp->next;
+                }
+                return h->default_value;
+            }
+        '''
+        write(helpers)
+
     def _create_code(self, write):
         write('#include <stdint.h>')
+        write('#include <stdlib.h>')
+        write('#include <string.h>')
 
         # windows dllexport needed to make symbols visible
         if platform.system() == 'Windows':
             write('#define EXPORT __declspec(dllexport)')
         else:
             write('#define EXPORT')
 
@@ -498,16 +698,19 @@
         # declare memories
         mems = {net.op_param[1] for net in self.block.logic_subset('m@')}
         for key in self._memmap:
             if key not in mems:
                 raise PyrtlError('unrecognized MemBlock in memory_value_map')
             if isinstance(key, RomBlock):
                 raise PyrtlError('RomBlock in memory_value_map')
-        for mem in mems:
-            self._declare_mem(write, mem)
+        self._declare_mem_helpers(write)
+        roms = {mem for mem in mems if isinstance(mem, RomBlock)}
+        self._declare_roms(write, roms)
+        mems = {mem for mem in mems if isinstance(mem, MemBlock)}
+        self._declare_mems(write, mems)
 
         # single step function
         write('static void sim_run_step(uint64_t inputs[], uint64_t outputs[]) {')
         write('uint64_t tmp, carry, tmphi, tmplo;')  # temporary variables
 
         # declare wire vectors
         for w in self.block.wirevector_set:
@@ -553,20 +756,19 @@
                 op=op, args=', '.join(self.varname[x] for x in args), dest=self.varname[dest]))
             op_builders[op](write, op, param, args, dest)
 
         # memory writes
         for net in self.block.logic_subset('@'):
             mem = net.op_param[1]
             write('if ({enable}[0]) {{'.format(enable=self.varname[net.args[2]]))
-            for n in range(self._limbs(mem)):
-                write('{mem}[{addr}[0]][{n}] = {vn}[{n}];'.format(
-                    mem=self.varname[mem],
-                    addr=self.varname[net.args[0]],
-                    vn=self.varname[net.args[1]],
-                    n=n))
+            write('insert({mem}, {addr}[0], {vn});'.format(
+                mem=self.varname[mem],
+                addr=self.varname[net.args[0]],
+                vn=self.varname[net.args[1]]
+            ))
             write('}')
 
         # register updates
         regnets = list(self.block.logic_subset('r'))
         for x, net in enumerate(regnets):
             rin = net.args[0]
             write('uint64_t regtmp{x}[{limbs}];'.format(x=x, limbs=self._limbs(rin)))
```

### Comparing `pyrtl-0.8.7/pyrtl/conditional.py` & `pyrtl-0.9.0/pyrtl/conditional.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         _depth = 1
 
     def __exit__(self, *exc_info):
         try:
             _finalize()
         finally:
             # even if the above finalization throws an error we need to
-            # return reset the state to prevent errors from bleeding over
+            # reset the state to prevent errors from bleeding over
             _reset_conditional_state()  # sets _depth back to 0
 
 
 class _Otherwise(object):
     """ helper type of global "otherwise". """
     def __enter__(self):
         _push_condition(otherwise)
@@ -118,15 +118,15 @@
 
 def _push_condition(predicate):
     """As we enter new conditions, this pushes them on the predicate stack."""
     global _depth
     _check_under_condition()
     _depth += 1
     if predicate is not otherwise and len(predicate) > 1:
-        raise PyrtlError('all predicates for conditional assignments must wirevectors of len 1')
+        raise PyrtlError('all predicates for conditional assignments must be wirevectors of len 1')
     _conditions_list_stack[-1].append(predicate)
     _conditions_list_stack.append([])
 
 
 def _pop_condition():
     """As we exit conditions, this pops them off the stack."""
     global _depth
@@ -233,15 +233,15 @@
         lastother = None
         for i, p in enumerate(predlist[:-1]):
             if p is otherwise:
                 lastother = i
         if lastother is None:
             return predlist[:-1]
         else:
-            return predlist[lastother+1:-1]
+            return predlist[lastother + 1:-1]
 
     select = None
     pred_set = set()
 
     # for all conditions except the current children (which should be [])
     for predlist in _conditions_list_stack[:-1]:
         # negate all of the predicates between "otherwise" and the current one
```

### Comparing `pyrtl-0.8.7/PyRTL.egg-info/PKG-INFO` & `pyrtl-0.9.0/PyRTL.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyrtl
-Version: 0.8.7
+Version: 0.9.0
 Summary: RTL-level Hardware Design and Simulation Toolkit
 Home-page: http://ucsbarchlab.github.io/PyRTL/
 Author: Timothy Sherwood, John Clow, and UCSBarchlab
 Author-email: sherwood@cs.ucsb.edu
 License: UNKNOWN
-Download-URL: https://github.com/UCSBarchlab/PyRTL/tarball/0.8.7
-Description-Content-Type: UNKNOWN
+Download-URL: https://github.com/UCSBarchlab/PyRTL/tarball/0.9.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -19,7 +18,8 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: System :: Hardware
+Provides-Extra: blif parsing
```

### Comparing `pyrtl-0.8.7/PyRTL.egg-info/SOURCES.txt` & `pyrtl-0.9.0/PyRTL.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 pyrtl/corecircuits.py
 pyrtl/helperfuncs.py
 pyrtl/inputoutput.py
 pyrtl/memory.py
 pyrtl/passes.py
 pyrtl/pyrtlexceptions.py
 pyrtl/simulation.py
-pyrtl/toFirrtl.py
 pyrtl/transform.py
 pyrtl/verilog.py
 pyrtl/wire.py
 pyrtl.egg-info/PKG-INFO
 pyrtl.egg-info/SOURCES.txt
 pyrtl.egg-info/dependency_links.txt
 pyrtl.egg-info/requires.txt
@@ -46,8 +45,9 @@
 tests/test_helperfuncs.py
 tests/test_inputoutput.py
 tests/test_memblock.py
 tests/test_passes.py
 tests/test_signed.py
 tests/test_simulation.py
 tests/test_transform.py
+tests/test_verilog.py
 tests/test_wire.py
```

### Comparing `pyrtl-0.8.7/tests/test_compilesim.py` & `pyrtl-0.9.0/tests/test_compilesim.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # and more work is required to more elegantly check compiledsim across multiple
 # architectures.
 import subprocess
 try:
     version = subprocess.check_output(['gcc', '--version'])
 except OSError:
     raise unittest.SkipTest('CompiledSimulation testing requires gcc')
-    
+
 
 class TraceWithBasicOpsBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         self.bitwidth = 3
         self.r = pyrtl.Register(bitwidth=self.bitwidth, name='r')
         self.o = pyrtl.Output(bitwidth=self.bitwidth, name='o')
@@ -144,15 +144,15 @@
     def test_print_trace_single_dig_notcompact(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") + self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
                 self.in1: i,
-                self.in2: 5-i
+                self.in2: 5 - i
             })
         correct_outp = ("      --- Values in base 10 ---\n"
                         "in1       0 1 2 3 4\n"
                         "in1_probe 0 1 2 3 4\n"
                         "in2       5 4 3 2 1\n"
                         "out       5 5 5 5 5\n")
         output = six.StringIO()
@@ -161,16 +161,16 @@
 
     def test_print_trace_base2(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") + self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
-                self.in1: 4*i,
-                self.in2: 4*(5 - i)
+                self.in1: 4 * i,
+                self.in2: 4 * (5 - i)
             })
         correct_outp = ("      --- Values in base 2 ---\n"
                         "in1           0   100  1000  1100 10000\n"
                         "in1_probe     0   100  1000  1100 10000\n"
                         "in2       10100 10000  1100  1000   100\n"
                         "out       10100 10100 10100 10100 10100\n")
         output = six.StringIO()
@@ -179,16 +179,16 @@
 
     def test_print_trace_base8(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") + self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
-                self.in1: 6*i,
-                self.in2: 6*(5 - i)
+                self.in1: 6 * i,
+                self.in2: 6 * (5 - i)
             })
         correct_outp = ("      --- Values in base 8 ---\n"
                         "in1        0  6 14 22 30\n"
                         "in1_probe  0  6 14 22 30\n"
                         "in2       36 30 22 14  6\n"
                         "out       36 36 36 36 36\n")
         output = six.StringIO()
@@ -197,16 +197,16 @@
 
     def test_print_trace_base16(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") * self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
-                self.in1: 9*i,
-                self.in2: 9*(5 - i)
+                self.in1: 9 * i,
+                self.in2: 9 * (5 - i)
             })
         correct_outp = ("      --- Values in base 16 ---\n"
                         "in1         0   9  12  1b  24\n"
                         "in1_probe   0   9  12  1b  24\n"
                         "in2        2d  24  1b  12   9\n"
                         "out         0 144 1e6 1e6 144\n")
         output = six.StringIO()
@@ -255,30 +255,29 @@
         out2 = pyrtl.Output(16, "out3")
         out1 <<= in1 + in2
         out2 <<= in3 | truth
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(10):
             sim.step({
-                'in1': 2*i,
-                'in2': 3*i,
-                'in3': 40 - 2*i
+                'in1': 2 * i,
+                'in2': 3 * i,
+                'in3': 40 - 2 * i
             })
         correct_outp = (" --- Values in base 10 ---\n"
                         "in1   0  2  4  6  8 10 12 14 16 18\n"
                         "in2   0  3  6  9 12 15 18 21 24 27\n"
                         "in3  40 38 36 34 32 30 28 26 24 22\n"
                         "out2  0  5 10 15 20 25 30 35 40 45\n"
                         "out3 41 39 37 35 33 31 29 27 25 23\n")
         output = six.StringIO()
         sim_trace.print_trace(output)
         self.assertEqual(output.getvalue(), correct_outp)
 
 
-
 class SimInputValidationBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def test_input_out_of_bitwidth(self):
         counter = pyrtl.Register(bitwidth=3, name='counter')
         i = pyrtl.Input(bitwidth=2, name='i')
@@ -288,14 +287,217 @@
         sim = self.sim(tracer=sim_trace)
         for cycle in range(4):
             sim.step({i: cycle})
         with self.assertRaises(pyrtl.PyrtlError):
             sim.step({i: 5})
 
 
+class SimStepMultipleBase(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+        in1 = pyrtl.Input(4, "in1")
+        in2 = pyrtl.Input(4, "in2")
+        out1 = pyrtl.Output(4, "out1")
+        out1 <<= (in1 ^ in2) + pyrtl.Const(1)
+        out2 = pyrtl.Output(4, "out2")
+        out2 <<= in1 | in2
+        self.inputs = {
+            'in1': [0, 1, 3, 15, 14],
+            'in2': [6, 6, 6, 6, 6],
+        }
+
+    def test_step_multiple_nsteps_no_inputs(self):
+        pyrtl.reset_working_block()
+        a = pyrtl.Register(8)
+        b = pyrtl.Output(8, 'b')
+        a.next <<= a + 1
+        b <<= a
+
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+        sim.step_multiple(nsteps=5)
+
+        correct_output = ("--- Values in base 10 ---\n"
+                          "b 0 1 2 3 4\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_nsteps_gt_ninputs(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple(self.inputs, nsteps=6)
+        self.assertEqual(str(error.exception),
+                         'nsteps is specified but is greater than the '
+                         'number of values supplied for each input')
+
+    def test_step_multiple_no_inputs(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple()
+        self.assertEqual(str(error.exception),
+                         'need to supply either input values '
+                         'or a number of steps to simulate')
+
+    def test_step_multiple_bad_nsteps1(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple({'in1': [], 'in2': []})
+        self.assertEqual(str(error.exception),
+                         'must simulate at least one step')
+
+    def test_step_multiple_bad_nsteps2(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple(self.inputs, nsteps=-1)
+        self.assertEqual(str(error.exception),
+                         'must simulate at least one step')
+
+    def test_step_multiple_no_values_for_each_step_of_input(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple({'in1': [0, 1, 3], 'in2': [1]})
+        self.assertEqual(str(error.exception),
+                         'must supply a value for each provided wire '
+                         'for each step of simulation')
+
+    def test_step_multiple_no_values_for_each_step_of_given_outputs(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple(self.inputs,
+                              {'out1': [7, 8, 6, 10, 9],
+                               'out2': [6, 7, 7, 15]})
+        self.assertEqual(str(error.exception),
+                         'any expected outputs must have a supplied value '
+                         'each step of simulation')
+
+    def test_step_multiple_no_expected_check(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        sim.step_multiple(self.inputs)
+
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1   0  1  3 15 14\n"
+                          "in2   6  6  6  6  6\n"
+                          "out1  7  8  6 10  9\n"
+                          "out2  6  7  7 15 14\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_no_errors(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 8, 6, 10, 9],
+            'out2': [6, 7, 7, 15, 14],
+        }
+        sim.step_multiple(self.inputs, expected)
+
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1   0  1  3 15 14\n"
+                          "in2   6  6  6  6  6\n"
+                          "out1  7  8  6 10  9\n"
+                          "out2  6  7  7 15 14\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_no_errors_nsteps_specified(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 8, 6, 10, 9],
+            'out2': [6, 7, 7, 15, 14],
+        }
+        sim.step_multiple(self.inputs, expected, nsteps=3)
+
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1  0 1 3\n"
+                          "in2  6 6 6\n"
+                          "out1 7 8 6\n"
+                          "out2 6 7 7\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_many_errors_report_only_first(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 9, 4, 10, 9],
+            'out2': [6, 2, 7, 8, 14],
+        }
+        output = six.StringIO()
+        sim.step_multiple(self.inputs, expected, file=output, stop_after_first_error=True)
+
+        # Test the output about unexpected values
+        correct_output = ("Unexpected output (stopped after step with first error):\n"
+                          " step       name expected   actual\n"
+                          "    1       out1        9        8\n"
+                          "    1       out2        2        7\n")
+        self.assertEqual(output.getvalue(), correct_output)
+
+        # Test that the trace stopped after the step with the first error
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1  0 1\n"
+                          "in2  6 6\n"
+                          "out1 7 8\n"
+                          "out2 6 7\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_many_errors_report_all(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 9, 4, 10, 9],
+            'out2': [6, 2, 7, 8, 14],
+        }
+        output = six.StringIO()
+        sim.step_multiple(self.inputs, expected, file=output)
+
+        # Test the output about unexpected values
+        correct_output = ("Unexpected output on one or more steps:\n"
+                          " step       name expected   actual\n"
+                          "    1       out1        9        8\n"
+                          "    1       out2        2        7\n"
+                          "    2       out1        4        6\n"
+                          "    3       out2        8       15\n")
+        self.assertEqual(output.getvalue(), correct_output)
+
+        # Test that the trace still produced all the steps
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1   0  1  3 15 14\n"
+                          "in2   6  6  6  6  6\n"
+                          "out1  7  8  6 10  9\n"
+                          "out2  6  7  7 15 14\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+
 class TraceWithAdderBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         bitwidth = 3
         self.r = pyrtl.Register(bitwidth=bitwidth, name='r')
         self.result = _basic_add(self.r, pyrtl.Const(1).zero_extended(bitwidth))
         self.r.next <<= self.result
@@ -310,15 +512,16 @@
 
         # step through 15 cycles
         for i in range(15):
             sim.step({})
 
         output = six.StringIO()
         sim_trace.print_trace(output, compact=True)
-        sim_trace.render_trace()  # want to make sure the code at least runs
+        file = six.StringIO()
+        sim_trace.render_trace(file=file)  # want to make sure the code at least runs
         self.assertEqual(output.getvalue(), 'o 012345670123456\n')
 
 
 class SimulationVCDWithAdderBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         bitwidth = 3
@@ -455,15 +658,15 @@
         input_signals = [[0, 1, 4, 5],
                          [4, 1, 0, 5],
                          [0, 4, 1, 6],
                          [1, 1, 0, 0],
                          [6, 0, 6, 7]]
         for signals in input_signals:
             sim.step({self.read_addr1: signals[0], self.read_addr2: signals[1],
-                           self.write_addr: signals[2], self.write_data: signals[3]})
+                      self.write_addr: signals[2], self.write_data: signals[3]})
 
         output = six.StringIO()
         self.sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), 'o1 05560\no2 00560\n')
 
     def test_simple2_memblock(self):
         sim = self.sim(tracer=self.sim_trace)
@@ -540,25 +743,90 @@
         mem_val_map = {self.mem1: {0: 0, 1: 1},
                        self.mem2: {0: 4, 1: 5}}
         self.sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=self.sim_trace, memory_value_map=mem_val_map)
         for i in range(2, 8):
             sim.step({
                 self.read_addr1: i,
-                self.read_addr2: 8-i+1,
+                self.read_addr2: 8 - i + 1,
                 read_addr3: i,
                 self.write_addr: 0,
                 self.write_data: 0
             })
         output = six.StringIO()
         self.sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), 'o1 000000\n'
                                             'o2 000000\n'
                                             'o3 000000\n')
 
+    def test_mem_val_map_empty_mapping(self):
+        read_addr3 = pyrtl.Input(self.addrwidth)
+        self.output3 = pyrtl.Output(self.bitwidth, "o3")
+        self.output3 <<= self.mem2[read_addr3]
+        mem_val_map = {self.mem1: {0: 0, 1: 1},
+                       self.mem2: {}}
+        self.sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=self.sim_trace, memory_value_map=mem_val_map)
+        for i in range(2, 8):
+            sim.step({
+                self.read_addr1: i,
+                self.read_addr2: 8 - i + 1,
+                read_addr3: i,
+                self.write_addr: 0,
+                self.write_data: 0
+            })
+        output = six.StringIO()
+        self.sim_trace.print_trace(output, compact=True)
+        self.assertEqual(output.getvalue(), 'o1 000000\n'
+                                            'o2 000000\n'
+                                            'o3 000000\n')
+
+
+class MemBlockLargeBase(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+        self.bitwidth = 68
+        self.addrwidth = 32
+        self.output1 = pyrtl.Output(self.bitwidth, "o1")
+        self.output2 = pyrtl.Output(self.bitwidth, "o2")
+        self.read_addr1 = pyrtl.Input(self.addrwidth)
+        self.read_addr2 = pyrtl.Input(self.addrwidth)
+        self.write_addr = pyrtl.Input(self.addrwidth)
+        self.write_data = pyrtl.Input(self.bitwidth)
+        self.mem = pyrtl.MemBlock(bitwidth=self.bitwidth, addrwidth=self.addrwidth, name='mem')
+        self.output1 <<= self.mem[self.read_addr1]
+        self.output2 <<= self.mem[self.read_addr2]
+        self.mem[self.write_addr] <<= self.write_data
+
+        # build the actual simulation environment
+        self.sim_trace = pyrtl.SimulationTrace()
+
+    def test_mem_blocks_very_large(self):
+        ''' Tests support of very large memories (i.e. address width > 30 bits),
+            and that limbs are handled appropriately for bitwidths > 64 '''
+        sim = self.sim(tracer=self.sim_trace)
+
+        write_data = 0x20000000040000012  # 68 bits
+        input_signals = [[0, 1, 0xffffffff, write_data],
+                         [0xffffffff, 1, 0, write_data],
+                         [0, 0xffffffff, 0xf0000001, 6],
+                         [0xf0000001, 0xf0000001, 0, 0],
+                         [6, 0, 6, 7]]
+        for signals in input_signals:
+            sim.step({self.read_addr1: signals[0], self.read_addr2: signals[1],
+                      self.write_addr: signals[2], self.write_data: signals[3]})
+
+        output = six.StringIO()
+        correct_outp = ("--- Values in base 10 ---\n"
+                        "o1                    0 %d %d                    6                    0\n"
+                        "o2                    0                    0 %d                    6                    0\n"  # noqa
+                        % (write_data, write_data, write_data))
+        self.sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_outp)
+
 
 class RegisterDefaultsBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         self.i = pyrtl.Input(bitwidth=3)
         self.r1 = pyrtl.Register(name='r1', bitwidth=3)
         self.r2 = pyrtl.Register(name='r2', bitwidth=3)
@@ -611,15 +879,15 @@
         output = six.StringIO()
         sim_trace_a.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), expected_output)
 
     def test_function_RomBlock(self):
 
         def rom_data_function(add):
-            return int((add + 5)/2)
+            return int((add + 5) / 2)
 
         pyrtl.reset_working_block()
         self.bitwidth = 4
         self.addrwidth = 4
         self.output1 = pyrtl.Output(self.bitwidth, "o1")
         self.output2 = pyrtl.Output(self.bitwidth, "o2")
         self.read_addr1 = pyrtl.Input(self.addrwidth)
@@ -630,25 +898,25 @@
         self.output2 <<= self.rom[self.read_addr2]
         # build the actual simulation environment
         self.sim_trace = pyrtl.SimulationTrace()
         self.sim = self.sim(tracer=self.sim_trace)
 
         input_signals = {}
         for i in range(0, 5):
-            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2*i}
+            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2 * i}
             self.sim.step(input_signals[i])
 
         exp_out = self.generate_expected_output((("o1", lambda x: rom_data_function(x)),
-                                                 ("o2", lambda x: rom_data_function(2*x))), 6)
+                                                 ("o2", lambda x: rom_data_function(2 * x))), 6)
         self.compareIO(self.sim_trace, exp_out)
 
     def test_function_RomBlock_with_optimization(self):
 
         def rom_data_function(add):
-            return int((add + 5)/2)
+            return int((add + 5) / 2)
 
         pyrtl.reset_working_block()
         self.bitwidth = 4
         self.addrwidth = 4
         self.output1 = pyrtl.Output(self.bitwidth, "o1")
         self.output2 = pyrtl.Output(self.bitwidth, "o2")
 
@@ -663,36 +931,37 @@
         pyrtl.optimize()
         # build the actual simulation environment
         self.sim_trace = pyrtl.SimulationTrace()
         self.sim = self.sim(tracer=self.sim_trace)
 
         input_signals = {}
         for i in range(0, 5):
-            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2*i}
-            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2*i}
+            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2 * i}
+            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2 * i}
             self.sim.step(input_signals[i])
 
         # exp_out = self.generate_expected_output((("o1", lambda x: rom_data_function(x) - 1),
         exp_out = self.generate_expected_output((("o1", lambda x: rom_data_function(x)),
-                                                 ("o2", lambda x: rom_data_function(2*x))), 6)
+                                                 ("o2", lambda x: rom_data_function(2 * x))), 6)
         self.compareIO(self.sim_trace, exp_out)
 
-    @unittest.skip
     def test_rom_out_of_range_error(self):
         rom_data_array = [15, 13, 11, 9, 7, 5, 3]
         rom1 = pyrtl.RomBlock(bitwidth=4, addrwidth=3, romdata=rom_data_array)
         rom_add_1 = pyrtl.Input(3, "rom_in")
         rom_out_1 = pyrtl.Output(4, "rom_out_1")
         rom_out_1 <<= rom1[rom_add_1]
 
         sim_trace = pyrtl.SimulationTrace()
-        sim = self.sim(tracer=sim_trace)
-        sim.step({rom_add_1: 3})
-        with self.assertRaises(pyrtl.PyrtlError):
-            sim.step({rom_add_1: 7})
+        with self.assertRaises(pyrtl.PyrtlError) as ex:
+            self.sim(tracer=sim_trace)
+        self.assertEqual(
+            str(ex.exception),
+            "RomBlock index is invalid, consider using pad_with_zeros=True for defaults"
+        )
 
     def test_rom_val_map(self):
         def rom_data_function(add):
             return int((add + 5) / 2)
         dummy_in = pyrtl.Input(1, "dummy")
         self.bitwidth = 4
         self.addrwidth = 4
@@ -732,14 +1001,28 @@
     def setUp(self):
         pyrtl.reset_working_block()
 
     def test_empty_trace(self):
         with self.assertRaises(pyrtl.PyrtlError):
             self.sim_trace = pyrtl.SimulationTrace()
 
+    def test_empty_trace_after_untraceable_removed(self):
+        r = pyrtl.Register(2, 'r')
+        r.next <<= r + 1
+        sim = self.sim()
+        sim.step_multiple(provided_inputs={}, nsteps=10)
+        with self.assertRaises(pyrtl.PyrtlError) as ex:
+            sim.tracer.render_trace()
+        self.assertEquals(
+            str(ex.exception),
+            "Empty trace list. This may have occurred because "
+            "untraceable wires were removed prior to simulation, "
+            "if a CompiledSimulation was used."
+        )
+
     def test_invalid_base(self):
         self.in1 = pyrtl.Input(8, "in1")
         self.out = pyrtl.Output(8, "out")
         self.out <<= self.in1
         self.sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=self.sim_trace)
         for i in range(5):
@@ -766,13 +1049,14 @@
             raise Exception("You should be making unittests that are compatible with"
                             "both Fastsim and Simulation")
         for sim in sims:
             unit_name = "Test" + name + sim.__name__
             unittests[unit_name] = type(unit_name, (v,), {'sim': sim})
     g.update(unittests)
 
+
 sims = (pyrtl.CompiledSimulation,)
 make_unittests()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_transform.py` & `pyrtl-0.9.0/tests/test_transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,31 @@
         self.assertEquals(len([net for net in block.logic if net.op == netOp]), num)
 
     def num_wire_of_type(self, wiretype, num, block=None):
         block = pyrtl.working_block(block)
         self.assertEquals(len(block.wirevector_subset(wiretype)), num)
 
 
+class WireMemoryNameTestCases(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+
+    def name_wires(self, names, block=None):
+        block = pyrtl.working_block()
+        names = set(names.split(' '))
+        for n in names:
+            self.assertIn(n, block.wirevector_by_name)
+
+    def name_memories(self, names, block=None):
+        block = pyrtl.working_block()
+        names = set(names.split(' '))
+        for n in names:
+            self.assertIn(n, block.memblock_by_name)
+
+
 def insert_random_inversions(rate=0.5):
     """
     an example transform that can be used for testing
     """
 
     import random
 
@@ -53,67 +70,75 @@
         new_and_net = block.logic_subset('&').pop()
         for arg in new_and_net.args:
             self.assertIsNot(arg, a)
             self.assertIsNot(arg, b)
         self.assertIsNot(new_and_net.dests[0], o)
 
 
-class TestCopyBlock(NetWireNumTestCases):
+class TestCopyBlock(NetWireNumTestCases, WireMemoryNameTestCases):
     def num_memories(self, mems_expected, block):
         memories = set()
         for net in block.logic_subset('m@'):
             memories.add(net.op_param[1])  # location of the memories object
         self.assertEqual(mems_expected, len(memories))
 
     def test_blank(self):
         block = transform.copy_block()
         self.assert_num_net(0, block)
         self.assert_num_wires(0, block)
 
     def test_block(self):
-        a = pyrtl.Const(23)
-        b = pyrtl.Input(5)
-        o = pyrtl.Output(5)
+        a = pyrtl.Const(23, name='a')
+        b = pyrtl.Input(5, name='b')
+        o = pyrtl.Output(5, name='o')
         o <<= ~a & b
 
         old_block = pyrtl.working_block()
         old_block.sanity_check()
         self.assert_num_wires(5, old_block)
         self.assert_num_net(3, old_block)
 
+        self.name_wires('a b o', old_block)
+
         new_block = transform.copy_block()
         new_block.sanity_check()
         self.assert_num_wires(5, new_block)
-        self.assert_num_net(3, old_block)
+        self.assert_num_net(3, new_block)
+
+        self.name_wires('a b o', new_block)
 
     def test_copy_mem(self):
         ins = [pyrtl.Input(5) for i in range(4)]
         out = pyrtl.Output(5)
 
-        mem1 = pyrtl.MemBlock(5, 5)
-        mem2 = pyrtl.MemBlock(5, 5)
+        mem1 = pyrtl.MemBlock(5, 5, name='mem1')
+        mem2 = pyrtl.MemBlock(5, 5, name='mem2')
 
         mem1_o1 = mem1[ins[0]]
         mem1[ins[1]] <<= ins[2]
         mem2_o2 = mem2[ins[3]]
         out <<= mem1_o1 & mem2_o2
 
         old_block = pyrtl.working_block()
         old_block.sanity_check()
         self.num_net_of_type('m', 2, old_block)
         self.num_net_of_type('@', 1, old_block)
         self.num_net_of_type('&', 1, old_block)
         self.num_memories(2, old_block)
 
+        self.name_memories('mem1 mem2', old_block)
+
         new_block = transform.copy_block()
         self.num_net_of_type('m', 2, new_block)
         self.num_net_of_type('@', 1, new_block)
         self.num_net_of_type('&', 1, new_block)
         self.num_memories(2, new_block)
 
+        self.name_memories('mem1 mem2', new_block)
+
 
 class TestFastWireReplace(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def test_replace_multiple_wires(self):
         j, n = pyrtl.Input(8), pyrtl.Output(8)
@@ -135,23 +160,23 @@
 
     def test_replace_multiple_wires_2(self):
         j, n = pyrtl.Input(8), pyrtl.Output(8)
         o = pyrtl.WireVector()
         x, y, z = pyrtl.WireVector(8), pyrtl.WireVector(8), pyrtl.WireVector(8)
 
         o <<= j
-        l = ~ j
-        h = o & l
+        p = ~ j
+        h = o & p
         n <<= h
         block = pyrtl.working_block()
         src_nets, dst_nets = block.net_connections()
         transform.replace_wire_fast(o, x, x, src_nets, dst_nets)
-        transform.replace_wire_fast(l, z, z, src_nets, dst_nets)
+        transform.replace_wire_fast(p, z, z, src_nets, dst_nets)
         transform.replace_wire_fast(h, y, y, src_nets, dst_nets)
-        for old_wire in (o, h, l):
+        for old_wire in (o, h, p):
             self.assertNotIn(old_wire, src_nets)
             self.assertNotIn(old_wire, dst_nets)
             self.assertNotIn(old_wire, block.wirevector_set)
         block.sanity_check()
 
     def test_wire_used_in_multiple_places(self):
         j, k = pyrtl.Input(8), pyrtl.Input(8)
@@ -169,15 +194,14 @@
         for old_wire in (r,):
             self.assertNotIn(old_wire, src_nets)
             self.assertNotIn(old_wire, dst_nets)
             self.assertNotIn(old_wire, block.wirevector_set)
         block.sanity_check()
 
 
-
 # this code needs mocking from python 3's unittests to work
 """
 @mock.patch('transform_examples.pyrtl.probe')
 def test_probe(self, probe):
     # Note to readers, this is a rather contrived test
     # If you want to know how to probe a single wirevector, look at the
     # probe function in pyrtl core
@@ -189,7 +213,9 @@
     def probe_cond(wire):
         return wire is test_wire
 
     transform_examples.probe_wire_if(probe_cond)
     probe.assert_called_once_with(test_wire)
 """
 
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_core.py` & `pyrtl-0.9.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import print_function
 import unittest
+import six
 import pyrtl
 
 
 class TestBlock(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
@@ -72,22 +73,49 @@
 
         tempwire <<= inwire | inwire2
         tempwire2 <<= ~tempwire
         outwire <<= tempwire2 & inwire3
 
         block = pyrtl.working_block()
 
+        output = six.StringIO()
         i = 0
         for net in block:
             self.assertFalse(i > 100, "Too many iterations happened")
             i += 1
-            print(str(net))
+            print(str(net), file=output)
 
         for net in block.logic:
-            print(net)
+            print(net, file=output)
+
+    def test_no_memblocks(self):
+        block = pyrtl.working_block()
+        self.assertFalse(block.memblock_by_name)
+
+    def test_bad_memblock_name_strict(self):
+        block = pyrtl.working_block()
+        with self.assertRaises(pyrtl.PyrtlError):
+            _ = block.get_memblock_by_name('bad_mem', strict=True)
+
+    def test_bad_memblock_name_none(self):
+        block = pyrtl.working_block()
+        mem = block.get_memblock_by_name('bad_mem')
+        self.assertIsNone(mem)
+
+    def test_same_memblock_referenced_across_multiple_operators(self):
+        mem_name = 'mem'
+        mem = pyrtl.MemBlock(32, 5, mem_name)
+        x = mem[0]
+        mem[1] <<= 42
+        mem = pyrtl.working_block().get_memblock_by_name(mem_name)
+        for net in pyrtl.working_block().logic:
+            if net.op == 'm':
+                self.assertIs(net.op_param[1], mem)
+            if net.op == '@':
+                self.assertIs(net.op_param[1], mem)
 
 
 class TestSanityCheckNet(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def tearDown(self):
@@ -97,16 +125,18 @@
         with self.assertRaisesRegexp(pyrtl.PyrtlInternalError, exp_message):
             pyrtl.working_block().add_net(*args)
 
     @staticmethod
     def new_net(op='&', op_param=None, args=None, dests=None):
         if args is None or isinstance(args, int):
             args = tuple(pyrtl.Input(2) for i in range(args if isinstance(args, int) else 2))
-        if dests is None:
-            dests = (pyrtl.Output(2, 'out'),)
+        if dests is None or isinstance(dests, int):
+            def dest():
+                return pyrtl.Register(2) if op == 'r' else pyrtl.Output(2)
+            dests = tuple(dest() for i in range(dests if isinstance(dests, int) else 1))
         return pyrtl.LogicNet(op=op, op_param=op_param, args=args, dests=dests)
 
     def test_net_make_with_not_net(self):
         self.invalid_net("net must be of type LogicNet", None)
         self.invalid_net("net must be of type LogicNet", 1)
         self.invalid_net("net must be of type LogicNet", "hi")
         self.invalid_net("net must be of type LogicNet", pyrtl.Const(2))
@@ -221,18 +251,38 @@
                 self.bitwidth, self.addrwidth = bw, aw
 
         for op in 'm@':
             net = self.new_net(op=op, op_param=(1234, NotMem()),
                                args=tuple(pyrtl.Input(1) for i in range(1 if op == 'm' else 3)))
             self.invalid_net("mem op requires second operand of a memory type", net)
 
+    def test_net_dest_wrong_arity_or_type(self):
+        for op in 'w~&|^n+-*<>=cr':
+            net = self.new_net(op=op, args=1 if op in 'w~r' else 2, dests=2)
+            self.invalid_net("error, op only allowed 1 destination", net)
+        net = self.new_net(op='s', op_param=(1,), args=1, dests=2)
+        self.invalid_net("error, op only allowed 1 destination", net)
+        net = self.new_net(op='x', args=(pyrtl.Input(1), pyrtl.Input(2), pyrtl.Input(2)), dests=2)
+        self.invalid_net("error, op only allowed 1 destination", net)
+        net = self.new_net(op='m', op_param=(1234, pyrtl.MemBlock(1, 2)), args=1, dests=2)
+        self.invalid_net("error, op only allowed 1 destination", net)
+
+        net = self.new_net(op='@', op_param=(1234, pyrtl.MemBlock(2, 2)),
+                           args=tuple(pyrtl.Input(i) for i in (2, 2, 1)))
+        self.invalid_net("mem write dest should be empty tuple", net)
+
+        net = self.new_net(op='r', args=1, dests=(pyrtl.WireVector(2),))
+        self.invalid_net("error, dest of next op should be a Register", net)
+
     def test_net_dest_wrong_bitwidth(self):
-        for op in 'w~&|^nr':
-            net = self.new_net(op=op, args=1 if op in 'w~r' else 2, dests=(pyrtl.Output(3),))
+        for op in 'w~&|^n':
+            net = self.new_net(op=op, args=1 if op in 'w~' else 2, dests=(pyrtl.Output(3),))
             self.invalid_net("upper bits of destination unassigned", net)
+        net = self.new_net(op='r', args=1, dests=(pyrtl.Register(3),))
+        self.invalid_net("upper bits of destination unassigned", net)
         for op in '<>=':
             net = self.new_net(op=op, dests=(pyrtl.Output(2),))
             self.invalid_net("destination should be of bitwidth=1", net)
         for op in '+-':
             net = self.new_net(op=op, dests=(pyrtl.Output(4),))
             self.invalid_net("upper bits of destination unassigned", net)
         net = self.new_net(op='*', dests=(pyrtl.Output(5),))
@@ -241,17 +291,14 @@
         self.invalid_net("upper bits of mux output undefined", net)
         net = self.new_net(op='c', args=3, dests=(pyrtl.Output(7),))
         self.invalid_net("upper bits of concat output undefined", net)
         net = self.new_net(op='s', args=1, op_param=(1,))
         self.invalid_net("upper bits of select output undefined", net)
         net = self.new_net(op='m', op_param=(1234, pyrtl.MemBlock(3, 2)), args=1)
         self.invalid_net("mem read dest bitwidth mismatch", net)
-        net = self.new_net(op='@', op_param=(1234, pyrtl.MemBlock(2, 2)),
-                           args=tuple(pyrtl.Input(i) for i in (2, 2, 1)))
-        self.invalid_net("mem write dest should be empty tuple", net)
 
 
 class TestSetWorkingBlock(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         self.block_a = pyrtl.Block()
         self.block_b = pyrtl.Block()
@@ -551,48 +598,43 @@
         self.mem_write_address = pyrtl.Input(self.addrwidth, name='mem_write_address')
         self.mem_write_data = pyrtl.Input(self.bitwidth, name='mem_write_data')
 
     def tearDown(self):
         pyrtl.reset_working_block()
 
     def test_async_check_should_pass(self):
-        memory = pyrtl.MemBlock(
-                    bitwidth=self.bitwidth, 
-                    addrwidth=self.addrwidth,
-                    name='memory')
+        memory = pyrtl.MemBlock(bitwidth=self.bitwidth,
+                                addrwidth=self.addrwidth,
+                                name='memory')
         self.output1 <<= memory[self.mem_read_address1]
         memory[self.mem_write_address] <<= self.mem_write_data
         pyrtl.working_block().sanity_check()
 
     def test_async_check_should_pass_with_select(self):
-        memory = pyrtl.MemBlock(
-                    bitwidth=self.bitwidth, 
-                    addrwidth=self.addrwidth-1,
-                    name='memory')
+        memory = pyrtl.MemBlock(bitwidth=self.bitwidth,
+                                addrwidth=self.addrwidth - 1,
+                                name='memory')
         self.output1 <<= memory[self.mem_read_address1[0:-1]]
         pyrtl.working_block().sanity_check()
 
     def test_async_check_should_pass_with_cat(self):
-        memory = pyrtl.MemBlock(
-                    bitwidth=self.bitwidth, 
-                    addrwidth=self.addrwidth,
-                    name='memory')
+        memory = pyrtl.MemBlock(bitwidth=self.bitwidth,
+                                addrwidth=self.addrwidth,
+                                name='memory')
         addr = pyrtl.concat(self.mem_read_address1[0], self.mem_read_address2[0:-1])
         self.output1 <<= memory[addr]
         memory[self.mem_write_address] <<= self.mem_write_data
         pyrtl.working_block().sanity_check()
 
     def test_async_check_should_notpass_with_add(self):
-        memory = pyrtl.MemBlock(
-                    bitwidth=self.bitwidth, 
-                    addrwidth=self.addrwidth,
-                    name='memory')
+        memory = pyrtl.MemBlock(bitwidth=self.bitwidth,
+                                addrwidth=self.addrwidth,
+                                name='memory')
         addr = pyrtl.WireVector(self.bitwidth)
         addr <<= self.mem_read_address1 + self.mem_read_address2
         self.output1 <<= memory[addr]
-        print(pyrtl.working_block())
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.working_block().sanity_check()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_passes.py` & `pyrtl-0.9.0/tests/test_passes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import print_function, unicode_literals, absolute_import
 
 import unittest
-import io
+import six
 import operator
+import os
+import sys
 
 import pyrtl
-from pyrtl.wire import Const,  Output
+from pyrtl.wire import Const, Output
 from pyrtl.analysis import estimate
 
 from .test_transform import NetWireNumTestCases
 
 
 class TestSynthesis(unittest.TestCase):
     def setUp(self):
@@ -21,15 +23,15 @@
 
     def check_trace(self, correct_string):
         pyrtl.synthesize()
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
-        output = io.StringIO()
+        output = six.StringIO()
         sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_not_simulation(self):
         self.r.next <<= ~ self.r
         self.check_trace('r 07070707\n')
 
@@ -58,15 +60,15 @@
     def test_minus_simulation2(self):
         self.r.next <<= self.r - pyrtl.Const(3, bitwidth=self.bitwidth)
         self.check_trace('r 05274163\n')
 
     def test_const_nobitwidth_simulation(self):
         self.r.next <<= self.r - pyrtl.Const(1)
         self.check_trace('r 07654321\n')
-    
+
     def test_mux_simulation(self):
         self.r.next <<= pyrtl.mux(self.r, 4, 3, 1, 7, 2, 6, 0, 5)
         self.check_trace('r 04213756\n')
 
 
 class TestMultiplierSynthesis(unittest.TestCase):
     def setUp(self):
@@ -79,15 +81,15 @@
         pyrtl.synthesize()
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for a in range(16):
             for b in range(16):
                 sim.step({'a': a, 'b': b})
         result = sim_trace.trace['r']
-        self.assertEqual(result, [a*b for a in range(16) for b in range(16)])
+        self.assertEqual(result, [a * b for a in range(16) for b in range(16)])
 
     def test_chained_mul(self):
         ina, inb, inc = (
             pyrtl.Input(bitwidth=2, name='a'),
             pyrtl.Input(bitwidth=2, name='b'),
             pyrtl.Input(bitwidth=2, name='c'))
         self.output <<= ina * inb * inc
@@ -95,34 +97,34 @@
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for a in range(4):
             for b in range(4):
                 for c in range(4):
                     sim.step({'a': a, 'b': b, 'c': c})
         result = sim_trace.trace['r']
-        self.assertEqual(result, [a*b*c for a in range(4) for b in range(4) for c in range(4)])
+        self.assertEqual(result, [a * b * c for a in range(4) for b in range(4) for c in range(4)])
 
     def test_singlebit_mul(self):
         ina, inb = pyrtl.Input(bitwidth=1, name='a'), pyrtl.Input(bitwidth=3, name='b')
         self.output <<= ina * inb
         pyrtl.synthesize()
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for a in range(2):
             for b in range(8):
                 sim.step({'a': a, 'b': b})
         result = sim_trace.trace['r']
-        self.assertEqual(result, [a*b for a in range(2) for b in range(8)])
+        self.assertEqual(result, [a * b for a in range(2) for b in range(8)])
 
 
 class TestComparisonSynthesis(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         self.output = pyrtl.Output(name='r')
-    
+
     def check_op(self, op):
         ina, inb = pyrtl.Input(bitwidth=4, name='a'), pyrtl.Input(bitwidth=4, name='b')
         self.output <<= op(ina, inb)
         pyrtl.synthesize()
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for a in range(16):
@@ -170,14 +172,24 @@
         # should remove the middle wires but keep the input
         block = pyrtl.working_block()
         self.assert_num_net(5, block)
         self.assert_num_wires(6, block)
 
 
 class TestConstFolding(NetWireNumTestCases):
+    def setUp(self):
+        pyrtl.reset_working_block()
+        # Redirect stdout because we don't care to see the specific messages about
+        # wires being deemed useless by optimization sent to stdout.
+        f = open(os.devnull, 'w')
+        sys.stdout = f
+
+    def tearDown(self):
+        sys.stdout.close()
+        sys.stdout = sys.__stdout__
 
     def test_basic_one_var_op_1(self):
         constwire = pyrtl.Const(0, 1)
         outwire = pyrtl.Output()
 
         outwire <<= ~constwire
         pyrtl.synthesize()
@@ -499,44 +511,44 @@
         # to make sure that the timing matches
         # this is a subprocess to do the synth and timing
         block = pyrtl.working_block()
         timing = estimate.TimingAnalysis(block)
         timing_max_length = timing.max_length()
         if timing_val is not None:
             self.assertEqual(timing_max_length, timing_val)
-        critical_path = timing.critical_path()
+        critical_path = timing.critical_path(print_cp=False)
 
         pyrtl.synthesize()
         pyrtl.optimize()
 
         block = pyrtl.working_block()
         timing = estimate.TimingAnalysis(block)
         timing_max_length = timing.max_length()
         if opt_timing_val is not None:
             self.assertEqual(timing_max_length, opt_timing_val)
-        critical_path = timing.critical_path()
+        critical_path = timing.critical_path(print_cp=False)
 
         pyrtl.and_inverter_synth()
         pyrtl.optimize()
 
         block = pyrtl.working_block()
         timing = estimate.TimingAnalysis(block)
         timing_max_length = timing.max_length()
-        critical_path = timing.critical_path()
+        critical_path = timing.critical_path(print_cp=False)
         block = pyrtl.working_block()
         self.num_net_of_type('|', 0, block)
         self.num_net_of_type('^', 0, block)
 
         pyrtl.nand_synth()
         pyrtl.optimize()
 
         block = pyrtl.working_block()
         timing = estimate.TimingAnalysis(block)
         timing_max_length = timing.max_length()
-        critical_path = timing.critical_path()
+        critical_path = timing.critical_path(print_cp=False)
         block.sanity_check()
         self.num_net_of_type('|', 0, block)
         self.num_net_of_type('^', 0, block)
         self.num_net_of_type('&', 0, block)
 
     def test_const_folding_complex_1(self):
         output = pyrtl.Output(bitwidth=3, name='output')
@@ -563,20 +575,23 @@
         tempwire, tempwire2 = pyrtl.WireVector(1), pyrtl.WireVector(1)
         outwire = pyrtl.Output()
 
         tempwire <<= ~(inwire & tempwire2)
         tempwire2 <<= ~(inwire2 & tempwire)
         outwire <<= tempwire
 
+        output = six.StringIO()
+        sys.stdout = output
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.synthesize()
             pyrtl.optimize()
             block = pyrtl.working_block()
-            timing = estimate.TimingAnalysis(block)
-            timing_max_length = timing.max_length()
+            _timing = estimate.TimingAnalysis(block)
+        sys.stdout = sys.__stdout__
+        self.assertTrue(output.getvalue().startswith("Loop found:"))
 
     def test_wirevector_1(self):
         inwire = pyrtl.Input(bitwidth=1)
         tempwire0, tempwire1 = pyrtl.WireVector(bitwidth=1), pyrtl.WireVector(bitwidth=1)
         tempwire2 = pyrtl.WireVector(bitwidth=1)
         outwire = pyrtl.Output()
 
@@ -615,9 +630,61 @@
         memory = pyrtl.MemBlock(3, 3, asynchronous=True)
 
         memory[readAdd1 & readAdd2] <<= readData1 ^ readData2
         dataOut <<= memory[writeAdd1 | writeAdd2]
         self.everything_t_procedure()
 
 
+class TestConcatAndSelectSimplification(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+
+    def test_two_way_concat(self):
+        i = pyrtl.Const(0b1100)
+        j = pyrtl.Const(0b011, bitwidth=3)
+        k = pyrtl.Const(0b100110)
+        o = pyrtl.Output(13, 'o')
+        o <<= pyrtl.concat(i, j, k)
+
+        block = pyrtl.working_block()
+        concat_nets = list(block.logic_subset(op='c'))
+        self.assertEqual(len(concat_nets), 1)
+        self.assertEqual(concat_nets[0].args, (i, j, k))
+
+        pyrtl.passes.two_way_concat()
+
+        concat_nets = list(block.logic_subset(op='c'))
+        self.assertEqual(len(concat_nets), 2)
+        upper_concat = next(n for n in concat_nets if i is n.args[0])
+        lower_concat = next(n for n in concat_nets if k is n.args[1])
+        self.assertNotEqual(upper_concat, lower_concat)
+        self.assertEqual(upper_concat.args, (i, j))
+        self.assertEqual(lower_concat.args, (upper_concat.dests[0], k))
+
+        sim = pyrtl.Simulation()
+        sim.step({})
+        self.assertEqual(sim.inspect('o'), 0b1100011100110)
+
+    def test_one_bit_selects(self):
+        a = pyrtl.Const(0b101101001101)
+        b = pyrtl.Output(6, 'b')
+        b <<= a[::2]  # bits 0, 2, 4, 6, 8, and 10 of wire a
+
+        block = pyrtl.working_block()
+        select_nets = list(block.logic_subset(op='s'))
+        self.assertEqual(len(select_nets), 1)
+        self.assertEqual(tuple(select_nets[0].op_param), (0, 2, 4, 6, 8, 10))
+
+        pyrtl.passes.one_bit_selects()
+
+        select_nets = list(block.logic_subset(op='s'))
+        for net in select_nets:
+            indices = net.op_param
+            self.assertEqual(len(indices), 1)
+
+        sim = pyrtl.Simulation()
+        sim.step({})
+        self.assertEqual(sim.inspect('b'), 0b00011011)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_helperfuncs.py` & `pyrtl-0.9.0/tests/test_helperfuncs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import io
 import random
 import unittest
 import six
+import os
+import sys
 
 import pyrtl
 import pyrtl.corecircuits
 import pyrtl.helperfuncs
 from pyrtl.rtllib import testingutils as utils
 
 
@@ -65,110 +66,328 @@
 
 
 class TestNonCoreHelpers(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_log2(self):
-        self.assertEqual(pyrtl.log2(1),0)
-        self.assertEqual(pyrtl.log2(2),1)
-        self.assertEqual(pyrtl.log2(8),3)
-        self.assertEqual(pyrtl.log2(16),4)
+        self.assertEqual(pyrtl.log2(1), 0)
+        self.assertEqual(pyrtl.log2(2), 1)
+        self.assertEqual(pyrtl.log2(8), 3)
+        self.assertEqual(pyrtl.log2(16), 4)
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.log2(-1)
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.log2(1.5)
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.log2(0)
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.log2(7)
         with self.assertRaises(pyrtl.PyrtlError):
             pyrtl.log2(9)
 
     def test_truncate_function(self):
-        self.assertEqual(pyrtl.truncate(5,3),5)
-        self.assertEqual(pyrtl.truncate(9,3),1)
-        self.assertEqual(pyrtl.truncate(-1,3),7)
+        self.assertEqual(pyrtl.truncate(5, 3), 5)
+        self.assertEqual(pyrtl.truncate(9, 3), 1)
+        self.assertEqual(pyrtl.truncate(-1, 3), 7)
         with self.assertRaises(pyrtl.PyrtlError):
-            pyrtl.truncate(5,-1)
+            pyrtl.truncate(5, -1)
         with self.assertRaises(pyrtl.PyrtlError):
-            pyrtl.truncate(29,0)
+            pyrtl.truncate(29, 0)
 
     def test_val_to_signed_integer(self):
-        self.assertEqual(pyrtl.val_to_signed_integer(0b000,3), 0)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b001,3), 1)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b010,3), 2)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b011,3), 3)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b100,3), -4)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b101,3), -3)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b110,3), -2)
-        self.assertEqual(pyrtl.val_to_signed_integer(0b111,3), -1)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b000, 3), 0)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b001, 3), 1)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b010, 3), 2)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b011, 3), 3)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b100, 3), -4)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b101, 3), -3)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b110, 3), -2)
+        self.assertEqual(pyrtl.val_to_signed_integer(0b111, 3), -1)
+
+    def test_infer_val_and_bitwidth(self):
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(2, bitwidth=5), (2, 5))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(3), (3, 2))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(True), (1, 1))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(False), (0, 1))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth("5'd12"), (12, 5))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth("5'b10"), (2, 5))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth("5'b10"), (2, 5))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth("8'B 0110_1100"), (108, 8))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-3, bitwidth=5), (0b11101, 5))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(3, signed=True), (3, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-3, signed=True), (5, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-4, signed=True), (4, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-3, bitwidth=5, signed=True), (29, 5))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(3, bitwidth=2), (3, 2))
+
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(0), (0, 1))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(1), (1, 1))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(2), (2, 2))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(3), (3, 2))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(4), (4, 3))
+
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(0, signed=True), (0, 1))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(1, signed=True), (1, 2))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(2, signed=True), (2, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(3, signed=True), (3, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(4, signed=True), (4, 4))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-1, signed=True), (1, 1))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-2, signed=True), (2, 2))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-3, signed=True), (5, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-4, signed=True), (4, 3))
+        self.assertEqual(pyrtl.infer_val_and_bitwidth(-5, signed=True), (11, 4))
+
+        with self.assertRaises(pyrtl.PyrtlError):
+            pyrtl.infer_val_and_bitwidth(-3)
+        with self.assertRaises(pyrtl.PyrtlError):
+            pyrtl.infer_val_and_bitwidth(True, signed=True)
+        with self.assertRaises(pyrtl.PyrtlError):
+            pyrtl.infer_val_and_bitwidth(3, bitwidth=2, signed=True)
+
+
+class TestMatchBitpattern(unittest.TestCase):
+    def setUp(self):
+        random.seed(8492049)
+        pyrtl.reset_working_block()
+
+    def check_trace(self, correct_string):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = pyrtl.Simulation(tracer=sim_trace)
+        for i in range(8):
+            sim.step({})
+        output = six.StringIO()
+        sim_trace.print_trace(output, compact=True)
+        self.assertEqual(output.getvalue(), correct_string)
+
+    def test_pattern_type_or_length_mismatch(self):
+        instr = pyrtl.WireVector(name='instr', bitwidth=8)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, '000100010')
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, '0001000')
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, '0b00010001')
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, 'abcd0000')
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, 0b000100010)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, '')
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, None)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.match_bitpattern(instr, instr)
+
+    def test_match_bitwidth_does_simulation_correct(self):
+        r = pyrtl.Register(6, 'r')
+        r.next <<= r + 3
+        # 000000 -> 000011 -> 000110 -> 001001 -> 001100 -> 001111 -> 010010 -> 010101
+        a = pyrtl.match_bitpattern(r, '00_?0 ?1')
+        o = pyrtl.Output(name='o')
+        o <<= a
+        self.check_trace('o 01010000\nr 036912151821\n')
+
+    def test_match_bitwidth_simulates_no_ones_in_pattern(self):
+        r = pyrtl.Register(6, 'r')
+        r.next <<= r + 3
+        # 000000 -> 000011 -> 000110 -> 001001 -> 001100 -> 001111 -> 010010 -> 010101
+        a = pyrtl.match_bitpattern(r, '00??00')
+        o = pyrtl.Output(name='o')
+        o <<= a
+        self.check_trace('o 10001000\nr 036912151821\n')
+
+    def test_match_bitwidth_simulates_no_zeroes_in_pattern(self):
+        r = pyrtl.Register(6, 'r')
+        r.next <<= r + 3
+        # 000000 -> 000011 -> 000110 -> 001001 -> 001100 -> 001111 -> 010010 -> 010101
+        a = pyrtl.match_bitpattern(r, '?1??1?')
+        o = pyrtl.Output(name='o')
+        o <<= a
+        self.check_trace('o 00000010\nr 036912151821\n')
+
+    def test_match_bitwidth_simulates_only_wildcards(self):
+        r = pyrtl.Register(6, 'r')
+        r.next <<= r + 3
+        # 000000 -> 000011 -> 000110 -> 001001 -> 001100 -> 001111 -> 010010 -> 010101
+        a = pyrtl.match_bitpattern(r, '??????')
+        o = pyrtl.Output(name='o')
+        o <<= a
+        self.check_trace('o 11111111\nr 036912151821\n')
+
+
+class TestChop(unittest.TestCase):
+    def setUp(self):
+        random.seed(8492049)
+        pyrtl.reset_working_block()
+
+    def check_trace(self, correct_string):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = pyrtl.Simulation(tracer=sim_trace)
+        for i in range(8):
+            sim.step({})
+        output = six.StringIO()
+        sim_trace.print_trace(output, compact=True)
+        self.assertEqual(output.getvalue(), correct_string)
+
+    def test_fields_mismatch(self):
+        instr = pyrtl.WireVector(name='instr', bitwidth=32)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(instr, 10, 10, 10)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(instr, 10, 10, 14)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(instr, 33)
+
+    def test_wrong_input_types_fail(self):
+        instr = pyrtl.WireVector(name='instr', bitwidth=32)
+        x = pyrtl.WireVector(name='x', bitwidth=10)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(instr, x, 10, 12)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(instr, 10, x, 12)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(instr, x)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.chop(10, 5, 5)
+
+    def test_chop_does_simulation_correct(self):
+        r = pyrtl.Register(5, 'r')
+        r.next <<= r + 1
+        a, b, c = pyrtl.helperfuncs.chop(r, 2, 2, 1)
+        o = pyrtl.Output(name='o')
+        o <<= c
+        self.check_trace('o 01010101\nr 01234567\n')
 
 
 class TestBitField_Update(unittest.TestCase):
     def setUp(self):
         random.seed(8492049)
         pyrtl.reset_working_block()
 
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
-        output = io.StringIO()
+        output = six.StringIO()
         sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_field_too_big(self):
         a = pyrtl.WireVector(name='a', bitwidth=3)
         b = pyrtl.WireVector(name='b', bitwidth=3)
         with self.assertRaises(pyrtl.PyrtlError):
-            o = pyrtl.bitfield_update(a,1,2,b)
+            o = pyrtl.bitfield_update(a, 1, 2, b)
 
     def test_field_too_big_truncate(self):
         a = pyrtl.WireVector(name='a', bitwidth=3)
         b = pyrtl.WireVector(name='b', bitwidth=3)
-        o = pyrtl.bitfield_update(a,1,2,b,truncating=True)
+        o = pyrtl.bitfield_update(a, 1, 2, b, truncating=True)
 
     def test_no_bits_to_update(self):
         a = pyrtl.WireVector(name='a', bitwidth=3)
         b = pyrtl.WireVector(name='b', bitwidth=3)
         with self.assertRaises(pyrtl.PyrtlError):
-            o = pyrtl.bitfield_update(a,1,1,b,truncating=True)
+            o = pyrtl.bitfield_update(a, 1, 1, b, truncating=True)
 
-    def bitfield_update_checker(self, input_width, range_start, range_end, update_width, test_amt=20):
-        def ref(i,s,e,u):
-            mask = ((1<<(e))-1) - ((1<<s)-1)
-            return (i&~mask) | ((u<<s)&mask)
+    def bitfield_update_checker(self, input_width, range_start, range_end,
+                                update_width, test_amt=20):
+        def ref(i, s, e, u):
+            mask = ((1 << (e)) - 1) - ((1 << s) - 1)
+            return (i & ~mask) | ((u << s) & mask)
         inp, inp_vals = utils.an_input_and_vals(input_width, test_vals=test_amt, name='inp')
         upd, upd_vals = utils.an_input_and_vals(update_width, test_vals=test_amt, name='upd')
-        #inp_vals = [1,1,0,0]
-        #upd_vals = [0x7,0x6,0x7,0x6]
+        # inp_vals = [1,1,0,0]
+        # upd_vals = [0x7,0x6,0x7,0x6]
         out = pyrtl.Output(input_width, "out")
         bfu_out = pyrtl.bitfield_update(inp, range_start, range_end, upd)
         self.assertEqual(len(out), len(bfu_out))  # output should have width of input
         out <<= bfu_out
-        true_result = [ref(i,range_start,range_end,u) for i,u in zip(inp_vals, upd_vals)]
-        upd_result = utils.sim_and_ret_out(out, [inp,upd], [inp_vals,upd_vals])
+        true_result = [ref(i, range_start, range_end, u) for i, u in zip(inp_vals, upd_vals)]
+        upd_result = utils.sim_and_ret_out(out, [inp, upd], [inp_vals, upd_vals])
+        self.assertEqual(upd_result, true_result)
+
+    def test_bitfield(self):
+        self.bitfield_update_checker(10, 3, 6, 3)
+
+
+class TestBitField_Update_Set(unittest.TestCase):
+    def setUp(self):
+        random.seed(8492049)
+        pyrtl.reset_working_block()
+
+    def check_trace(self, correct_string):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = pyrtl.Simulation(tracer=sim_trace)
+        for i in range(8):
+            sim.step({})
+        output = six.StringIO()
+        sim_trace.print_trace(output, compact=True)
+        self.assertEqual(output.getvalue(), correct_string)
+
+    def test_field_too_big(self):
+        a = pyrtl.WireVector(name='a', bitwidth=3)
+        b = pyrtl.WireVector(name='b', bitwidth=3)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.bitfield_update_set(a, {(1, 2): b})
+
+    def test_field_too_big_truncate(self):
+        a = pyrtl.WireVector(name='a', bitwidth=3)
+        b = pyrtl.WireVector(name='b', bitwidth=3)
+        o = pyrtl.bitfield_update_set(a, {(1, 2): b}, truncating=True)
+
+    def test_no_bits_to_update(self):
+        a = pyrtl.WireVector(name='a', bitwidth=3)
+        b = pyrtl.WireVector(name='b', bitwidth=3)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.bitfield_update_set(a, {(1, 1): b}, truncating=True)
+
+    def test_overlapping_ranges(self):
+        a = pyrtl.WireVector(name='a', bitwidth=10)
+        b = pyrtl.WireVector(name='b', bitwidth=10)
+        c = pyrtl.WireVector(name='c', bitwidth=10)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.bitfield_update_set(a, {(1, 4): b, (3, 6): c}, truncating=True)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.bitfield_update_set(a, {(8, 10): b, (-1, None): c}, truncating=True)
+        with self.assertRaises(pyrtl.PyrtlError):
+            o = pyrtl.bitfield_update_set(a, {(None, 3): b, (0, 1): c}, truncating=True)
+
+    def bitfield_update_checker(self, input_width, range_start, range_end,
+                                update_width, test_amt=20):
+        def ref(i, s, e, u):
+            mask = ((1 << (e)) - 1) - ((1 << s) - 1)
+            return (i & ~mask) | ((u << s) & mask)
+        inp, inp_vals = utils.an_input_and_vals(input_width, test_vals=test_amt, name='inp')
+        upd, upd_vals = utils.an_input_and_vals(update_width, test_vals=test_amt, name='upd')
+        # inp_vals = [1,1,0,0]
+        # upd_vals = [0x7,0x6,0x7,0x6]
+        out = pyrtl.Output(input_width, "out")
+        bfu_out = pyrtl.bitfield_update_set(inp, {(range_start, range_end): upd})
+        self.assertEqual(len(out), len(bfu_out))  # output should have width of input
+        out <<= bfu_out
+        true_result = [ref(i, range_start, range_end, u) for i, u in zip(inp_vals, upd_vals)]
+        upd_result = utils.sim_and_ret_out(out, [inp, upd], [inp_vals, upd_vals])
         self.assertEqual(upd_result, true_result)
 
     def test_bitfield(self):
-        self.bitfield_update_checker(10,3,6,3)
+        self.bitfield_update_checker(10, 3, 6, 3)
 
 
 class TestAnyAll(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
-        output = io.StringIO()
+        output = six.StringIO()
         sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_any_only_on_1_bit_vectors(self):
         a = pyrtl.WireVector(name='a', bitwidth=3)
         b = pyrtl.WireVector(name='b', bitwidth=1)
         with self.assertRaises(pyrtl.PyrtlError):
@@ -235,15 +454,15 @@
         pyrtl.reset_working_block()
 
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
-        output = io.StringIO()
+        output = six.StringIO()
         sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_one_wirevector(self):
         r = pyrtl.Register(3, 'r')
         r.next <<= r + 1
         o = pyrtl.Output(name='o')
@@ -407,96 +626,109 @@
         x = pyrtl.probe(i)
         self.assertIs(x, i)
 
     def test_simple_probe_debug(self):
         pyrtl.set_debug_mode()
         i = pyrtl.Input(1)
         o = pyrtl.Output(1)
-        o <<= pyrtl.probe(i + 1)
+        output = six.StringIO()
+        sys.stdout = output
+        o <<= pyrtl.probe(i + 1, name="probe0")
+        sys.stdout = sys.__stdout__
+        self.assertTrue(output.getvalue().startswith("Probe: probe0"))
         pyrtl.set_debug_mode(False)
 
 
 class TestShiftSimulation(unittest.TestCase):
 
     def setUp(self):
         random.seed(8492049)
         pyrtl.reset_working_block()
 
     def shift_checker(self, shift_func, ref_func, input_width, shift_width, test_amt=20):
         inp, inp_vals = utils.an_input_and_vals(input_width, test_vals=test_amt, name='inp')
         shf, shf_vals = utils.an_input_and_vals(shift_width, test_vals=test_amt, name='shf')
         out = pyrtl.Output(input_width, "out")
-        shf_out = shift_func(inp,shf)
+        shf_out = shift_func(inp, shf)
         self.assertEqual(len(out), len(shf_out))  # output should have width of input
         out <<= shf_out
-        true_result = [ref_func(i,s) for i,s in zip(inp_vals, shf_vals)]
-        shift_result = utils.sim_and_ret_out(out, [inp,shf], [inp_vals,shf_vals])
+        true_result = [ref_func(i, s) for i, s in zip(inp_vals, shf_vals)]
+        shift_result = utils.sim_and_ret_out(out, [inp, shf], [inp_vals, shf_vals])
         self.assertEqual(shift_result, true_result)
 
     def sll_checker(self, input_width, shift_width):
-        mask = (1<<input_width)-1
-        ref = lambda i,s: (i<<s) & mask
+        mask = (1 << input_width) - 1
+
+        def ref(i, s):
+            return (i << s) & mask
+
         self.shift_checker(pyrtl.shift_left_logical, ref, input_width, shift_width)
 
     def sla_checker(self, input_width, shift_width):
-        mask = (1<<input_width)-1
-        ref = lambda i,s: (i<<s) & mask
+        mask = (1 << input_width) - 1
+
+        def ref(i, s):
+            return (i << s) & mask
+
         self.shift_checker(pyrtl.shift_left_arithmetic, ref, input_width, shift_width)
 
     def srl_checker(self, input_width, shift_width):
-        mask = (1<<input_width)-1
-        ref = lambda i,s: (i>>s) & mask
+        mask = (1 << input_width) - 1
+
+        def ref(i, s):
+            return (i >> s) & mask
+
         self.shift_checker(pyrtl.shift_right_logical, ref, input_width, shift_width)
 
     def sra_checker(self, input_width, shift_width):
         # a little more work is required to take the positive number and treat it
         # as a twos complement number for the purpose of testing the shifter
-        def ref(i,s):
-            mask = (1<<input_width)-1
-            if (i>>input_width-1) & 0x1 == 0x1:
-                return ((~mask|i)>>s) & mask  # negative number
+        def ref(i, s):
+            mask = (1 << input_width) - 1
+            if (i >> input_width - 1) & 0x1 == 0x1:
+                return ((~mask | i) >> s) & mask  # negative number
             else:
-                return (i>>s) & mask  # possitive number
+                return (i >> s) & mask  # positive number
         self.shift_checker(pyrtl.shift_right_arithmetic, ref, input_width, shift_width)
 
     def test_sll(self):
-        self.sll_checker(5,2)
+        self.sll_checker(5, 2)
 
     def test_sla(self):
-        self.sla_checker(5,2)
+        self.sla_checker(5, 2)
 
     def test_srl(self):
-        self.srl_checker(5,2)
+        self.srl_checker(5, 2)
 
     def test_sra(self):
-        self.sra_checker(5,2)
+        self.sra_checker(5, 2)
 
     def test_sll_big(self):
-        self.sll_checker(10,3)
+        self.sll_checker(10, 3)
 
     def test_sla_big(self):
-        self.sla_checker(10,3)
+        self.sla_checker(10, 3)
 
     def test_srl_big(self):
-        self.srl_checker(10,3)
+        self.srl_checker(10, 3)
 
     def test_sra_big(self):
-        self.sra_checker(10,3)
+        self.sra_checker(10, 3)
 
     def test_sll_over(self):
-        self.sll_checker(4,4)
+        self.sll_checker(4, 4)
 
     def test_sla_over(self):
-        self.sla_checker(4,4)
+        self.sla_checker(4, 4)
 
     def test_srl_over(self):
-        self.srl_checker(4,4)
+        self.srl_checker(4, 4)
 
     def test_sra_over(self):
-        self.sra_checker(4,4)
+        self.sra_checker(4, 4)
 
 
 class TestBasicMult(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def mult_t_base(self, len_a, len_b):
@@ -504,16 +736,16 @@
         a, b = pyrtl.Input(len_a, "a"), pyrtl.Input(len_b, "b")
         product = pyrtl.Output(name="product")
         product <<= pyrtl.corecircuits._basic_mult(a, b)
 
         self.assertEqual(len(product), len_a + len_b)
 
         # creating the testing values and the correct results
-        xvals = [int(random.uniform(0, 2**len_a-1)) for i in range(20)]
-        yvals = [int(random.uniform(0, 2**len_b-1)) for i in range(20)]
+        xvals = [int(random.uniform(0, 2 ** len_a - 1)) for i in range(20)]
+        yvals = [int(random.uniform(0, 2 ** len_b - 1)) for i in range(20)]
         true_result = [i * j for i, j in zip(xvals, yvals)]
 
         # Setting up and running the tests
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for cycle in range(len(xvals)):
             sim.step({a: xvals[cycle], b: yvals[cycle]})
@@ -608,14 +840,22 @@
         with self.assertRaises(self.RTLSampleException):
             sim.step({i: 0})
 
 
 class TestLoopDetection(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
+        # Redirect stdout because we don't care to see the specific messages about
+        # wires being deemed useless by optimization sent to stdout.
+        f = open(os.devnull, 'w')
+        sys.stdout = f
+
+    def tearDown(self):
+        sys.stdout.close()
+        sys.stdout = sys.__stdout__
 
     def assert_no_loop(self):
         self.assertEqual(pyrtl.find_loop(), None)
         pyrtl.synthesize()
         self.assertEqual(pyrtl.find_loop(), None)
         pyrtl.optimize()
         self.assertEqual(pyrtl.find_loop(), None)
@@ -720,7 +960,145 @@
 
     def test_no_loop_reg_1(self):
         reg = pyrtl.Register(8)
         in_w = pyrtl.Input(8)
         res = reg + in_w
         reg.next <<= res
         self.assert_no_loop()
+
+
+class TestBundle(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+
+    def test_create_bundle_from_tuples(self):
+        rformat = [
+            ("funct7", 7),
+            ("rs2", 5),
+            ("rs1", 5),
+            ("funct3", 3),
+            ("rd", 5),
+            ("opcode", 7),
+        ]
+        self.create_and_check_bundle(rformat)
+
+    def test_create_bundle_from_dict(self):
+        rformat = {
+            "funct7": 7,
+            "rs2": 5,
+            "rs1": 5,
+            "funct3": 3,
+            "rd": 5,
+            "opcode": 7
+        }
+        if six.PY2:
+            with self.assertRaises(pyrtl.PyrtlError) as ex:
+                self.create_and_check_bundle(rformat)
+            self.assertEqual(
+                str(ex.exception),
+                "For Python versions < 3.7, the dictionary used to instantiate "
+                "a Bundle must be explicitly ordered (i.e. OrderedDict)"
+            )
+        else:
+            self.create_and_check_bundle(rformat)
+
+    def test_create_bundle_from_class(self):
+        class RFormat:
+            funct7 = 7
+            rs2 = 5
+            rs1 = 5
+            funct3 = 3
+            rd = 5
+            opcode = 7
+        if six.PY2:
+            with self.assertRaises(pyrtl.PyrtlError) as ex:
+                self.create_and_check_bundle(RFormat)
+            self.assertEqual(
+                str(ex.exception),
+                "Passing a class as an argument to Bundle() is only "
+                "allowed for Python versions >= 3.7"
+            )
+        else:
+            self.create_and_check_bundle(RFormat)
+
+    def test_create_bundle_from_tuples_with_callable(self):
+        a = pyrtl.Input(1, 'a')
+        b = pyrtl.Input(2, 'b')
+
+        bundler = {
+            'a_not': (1, ~a),
+            'b_is_2': (1, b == 2),
+            'sum': (3, a + b)
+        }
+
+        if six.PY2:
+            with self.assertRaises(pyrtl.PyrtlError) as ex:
+                w = pyrtl.helperfuncs.Bundle(bundler)
+            self.assertEqual(
+                str(ex.exception),
+                "For Python versions < 3.7, the dictionary used to instantiate "
+                "a Bundle must be explicitly ordered (i.e. OrderedDict)"
+            )
+        else:
+            w = pyrtl.helperfuncs.Bundle(bundler)
+            self.assertTrue(isinstance(w, pyrtl.WireVector))
+            self.assertTrue(hasattr(w, 'a_not'))
+            self.assertTrue(hasattr(w, 'b_is_2'))
+            self.assertTrue(hasattr(w, 'sum'))
+            self.assertEqual(len(w.a_not), 1)
+            self.assertEqual(len(w.b_is_2), 1)
+            self.assertEqual(len(w.sum), 3)
+
+            pyrtl.probe(w.a_not, 'a_not_out')
+            pyrtl.probe(w.b_is_2, 'b_is_2_out')
+            pyrtl.probe(w.sum, 'sum_out')
+            sim = pyrtl.Simulation()
+            sim.step_multiple({
+                'a': '00001111',
+                'b': '01230123',
+            })
+            output = six.StringIO()
+            sim.tracer.print_trace(output, compact=True)
+            self.assertEqual(output.getvalue(),
+                             '         a 00001111\n'
+                             ' a_not_out 11110000\n'
+                             '         b 01230123\n'
+                             'b_is_2_out 00100010\n'
+                             '   sum_out 01231234\n')
+
+    def create_and_check_bundle(self, bundler):
+        w = pyrtl.helperfuncs.Bundle(bundler)
+        self.assertTrue(isinstance(w, pyrtl.WireVector))
+        self.assertTrue(hasattr(w, 'funct7'))
+        self.assertTrue(hasattr(w, 'rs2'))
+        self.assertTrue(hasattr(w, 'rs1'))
+        self.assertTrue(hasattr(w, 'funct3'))
+        self.assertTrue(hasattr(w, 'rd'))
+        self.assertTrue(hasattr(w, 'opcode'))
+        self.assertEqual(len(w), 32)
+        self.assertEqual(len(w.funct7), 7)
+        self.assertEqual(len(w.rs2), 5)
+        self.assertEqual(len(w.rs1), 5)
+        self.assertEqual(len(w.funct3), 3)
+        self.assertEqual(len(w.rd), 5)
+        self.assertEqual(len(w.opcode), 7)
+
+        r = pyrtl.Register(len(w))
+        r.next <<= w
+        y = r.as_bundle(bundler)
+        self.assertTrue(hasattr(y, 'funct7'))
+        self.assertTrue(hasattr(y, 'rs2'))
+        self.assertTrue(hasattr(y, 'rs1'))
+        self.assertTrue(hasattr(y, 'funct3'))
+        self.assertTrue(hasattr(y, 'rd'))
+        self.assertTrue(hasattr(y, 'opcode'))
+        self.assertEqual(len(y), 32)
+        self.assertEqual(len(y.funct7), 7)
+        self.assertEqual(len(y.rs2), 5)
+        self.assertEqual(len(y.rs1), 5)
+        self.assertEqual(len(y.funct3), 3)
+        self.assertEqual(len(y.rd), 5)
+        self.assertEqual(len(y.opcode), 7)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_memblock.py` & `pyrtl-0.9.0/tests/test_memblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def test_memblock_simple(self):
         self.output1 <<= self.memory[self.mem_read_address1]
         self.output2 <<= self.memory[self.mem_read_address2]
         self.memory[self.mem_write_address] <<= self.mem_write_data
         pyrtl.working_block().sanity_check()
 
     def test_memblock_assign_with_extention(self):
-        big_output = pyrtl.Output(self.bitwidth+1, "big_output")
+        big_output = pyrtl.Output(self.bitwidth + 1, "big_output")
         big_output <<= self.memory[self.mem_read_address1]
         self.output1 <<= 1
         self.output2 <<= 2
         self.memory[self.mem_write_address] <<= self.mem_write_data
         pyrtl.working_block().sanity_check()
 
     def test_memblock_with_write_enable_with_equalsign(self):
@@ -86,14 +86,24 @@
         lim_memory = pyrtl.MemBlock(bitwidth=self.bitwidth, addrwidth=self.addrwidth,
                                     name='lim_memory', max_write_ports=4)
         for i in range(lim_memory.max_write_ports):
             lim_memory[self.mem_write_address] <<= pyrtl.Const(6)
         with self.assertRaises(pyrtl.PyrtlError):
             lim_memory[self.mem_write_address] <<= pyrtl.Const(6)
 
+    def test_memblock_added_user_named(self):
+        mem_name = 'small_memory'
+        small_memory = pyrtl.MemBlock(bitwidth=self.bitwidth, addrwidth=self.addrwidth,
+                                      name=mem_name, max_read_ports=2, max_write_ports=1)
+        self.assertIs(pyrtl.working_block().get_memblock_by_name(mem_name), small_memory)
+
+    def test_memblock_added_default_named(self):
+        mem = pyrtl.MemBlock(32, 8)
+        self.assertIs(pyrtl.working_block().get_memblock_by_name(mem.name), mem)
+
 
 class MemIndexedTests(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def test_memindexed_name(self):
         self.mem = pyrtl.MemBlock(8, 8)
@@ -113,16 +123,16 @@
         z <<= x
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace, memory_value_map=self.mem_val_map)
         for i in range(5):
             sim.step({
                 a: i
             })
-            self.assertEqual(sim.inspect(y), 5-i)
-            self.assertEqual(sim.inspect(z), 5-i)
+            self.assertEqual(sim.inspect(y), 5 - i)
+            self.assertEqual(sim.inspect(z), 5 - i)
         self.assertEqual(self.mem.read_ports, 1)
 
     def test_write_memindexed_ilshift(self):
         self.mem1 = pyrtl.MemBlock(8, 8)
         self.mem2 = pyrtl.MemBlock(8, 8, asynchronous=True)
         self.mem_val_map = {self.mem1: {0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5}}
         addr1 = pyrtl.Input(3)
@@ -133,18 +143,18 @@
         out = pyrtl.Output(9, name='out')
         out <<= self.mem2[addr2]  # one behind addr1, so one behind x
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace, memory_value_map=self.mem_val_map)
         for i in range(5):
             sim.step({
                 addr1: i,
-                addr2: 0 if i == 0 else i-1,  # one behind addr1
-                inp: 5-i
+                addr2: 0 if i == 0 else i - 1,  # one behind addr1
+                inp: 5 - i
             })
-            self.assertEqual(sim.inspect(out), 0 if i ==0 else 5-(i-1))
+            self.assertEqual(sim.inspect(out), 0 if i == 0 else 5 - (i - 1))
         self.assertEqual(self.mem1.read_ports, 1)  # 2 b/c of the output read
         self.assertEqual(self.mem2.write_ports, 1)
 
     def test_read_memindexed_ior(self):
         self.mem = pyrtl.MemBlock(8, 8)
         self.mem_val_map = {self.mem: {0: 5, 1: 4, 2: 3, 3: 2, 4: 1, 5: 0}}
         decide = pyrtl.Input(1)
@@ -162,15 +172,15 @@
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace, memory_value_map=self.mem_val_map)
         for i in range(5):
             sim.step({
                 decide: i % 2,
                 ind: i
             })
-            if i ==0:
+            if i == 0:
                 y_exp, z_exp, w_exp = 0, 0, 5
             elif i == 1:
                 y_exp, z_exp, w_exp = 4, 4, 0
             elif i == 2:
                 y_exp, z_exp, w_exp = 0, 0, 3
             elif i == 3:
                 y_exp, z_exp, w_exp = 2, 2, 0
@@ -201,16 +211,16 @@
         out <<= self.mem2[addr2]  # one behind addr1, so one behind x
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace, memory_value_map=self.mem_val_map)
         for i in range(5):
             sim.step({
                 decide: i % 2,
                 addr1: i,
-                addr2: 0 if i == 0 else i-1,  # one behind addr1
-                inp: 5-i
+                addr2: 0 if i == 0 else i - 1,  # one behind addr1
+                inp: 5 - i
             })
             if (i == 0) | (i == 1) | (i == 3):
                 out_exp = 0
             elif i == 2:
                 out_exp = 4
             else:
                 out_exp = 2
@@ -318,15 +328,15 @@
         romf2 = pyrtl.RomBlock(5, 5, bad_func_2)
         for rom in (rom1, rom2, romf1, romf2):
             self.invalid_rom_read(rom, 0)
             self.invalid_rom_read(rom, 1)
 
     def test_value_out_of_range(self):
         def rom_func(address):
-            return 2 * (8-address) + 1
+            return 2 * (8 - address) + 1
 
         rom1 = pyrtl.RomBlock(3, 3, [15, 8, 7, 1])
         romf1 = pyrtl.RomBlock(3, 3, rom_func)
 
         for rom in (rom1, romf1):
             self.invalid_rom_read(rom, 0)
             self.invalid_rom_read(rom, 1)
```

### Comparing `pyrtl-0.8.7/tests/test_conditional.py` & `pyrtl-0.9.0/tests/test_conditional.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
         output = io.StringIO()
         sim_trace.print_trace(output, compact=True)
-        print(output.getvalue())
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_basic_true_condition(self):
         c = pyrtl.Const(1)
         r = pyrtl.Register(bitwidth=2, name='r')
         with pyrtl.conditional_assignment:
             with c:
@@ -135,21 +134,23 @@
             o |= c
 
     def test_error_on_non_boolean(self):
         c = pyrtl.Const(2)
         r = pyrtl.Register(bitwidth=2, name='r')
         with self.assertRaises(pyrtl.PyrtlError):
             with pyrtl.conditional_assignment:
-                with c: pass
+                with c:
+                    pass
 
     def test_error_on_non_boolean_with_register(self):
         r = pyrtl.Register(bitwidth=4, name='r')
         with self.assertRaises(pyrtl.PyrtlError):
             with pyrtl.conditional_assignment:
-                with r: pass
+                with r:
+                    pass
 
 
 # ---------------------------------------------------------------
 
 
 class TestMemConditionalBlock(unittest.TestCase):
     def setUp(self):
@@ -158,15 +159,14 @@
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
         output = io.StringIO()
         sim_trace.print_trace(output, compact=True)
-        print(output.getvalue())
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_basic_true_condition_memwrite(self):
         m = pyrtl.MemBlock(addrwidth=2, bitwidth=2, name='m')
         i = pyrtl.Register(bitwidth=2, name='i')
         o = pyrtl.WireVector(bitwidth=2, name='o')
         i.next <<= i + 1
@@ -178,15 +178,15 @@
 
     def test_basic_true_condition_memwrite_2(self):
         m = pyrtl.MemBlock(addrwidth=2, bitwidth=2, name='m')
         i = pyrtl.Register(bitwidth=2, name='i')
         o = pyrtl.WireVector(bitwidth=2, name='o')
         i.next <<= i + 1
         with pyrtl.conditional_assignment:
-            with m[i]!=0:
+            with m[i] != 0:
                 m[i] <<= i
         o <<= m[i]
         self.check_trace('i 01230123\no 00000123\n')
 
     def test_basic_true_condition_memread(self):
         m = pyrtl.MemBlock(addrwidth=2, bitwidth=3, name='m')
         i = pyrtl.Register(bitwidth=3, name='i')
@@ -231,15 +231,14 @@
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
         output = io.StringIO()
         sim_trace.print_trace(output, compact=True)
-        print(output.getvalue())
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_basic_condition_wire(self):
         i = pyrtl.Register(bitwidth=2, name='i')
         o = pyrtl.WireVector(bitwidth=2, name='o')
         i.next <<= i + 1
         with pyrtl.conditional_assignment:
@@ -250,15 +249,15 @@
         self.check_trace('i 01230123\no 11101110\n')
 
     def test_boolean_assignment_condition_wire(self):
         i = pyrtl.Register(bitwidth=2, name='i')
         o = pyrtl.WireVector(bitwidth=2, name='o')
         i.next <<= i + 1
         with pyrtl.conditional_assignment:
-            with i[0] == True:
+            with i[0]:
                 o |= 1
             with pyrtl.otherwise:
                 o |= 0
         self.check_trace('i 01230123\no 01010101\n')
 
     def test_nested_condition_wire(self):
         i = pyrtl.Register(bitwidth=2, name='i')
@@ -350,68 +349,71 @@
     def check_trace(self, correct_string):
         sim_trace = pyrtl.SimulationTrace()
         sim = pyrtl.Simulation(tracer=sim_trace)
         for i in range(8):
             sim.step({})
         output = io.StringIO()
         sim_trace.print_trace(output, compact=True)
-        print(output.getvalue())
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_basic_nested_non_exclusive_condition(self):
         i = pyrtl.Register(bitwidth=2, name='i')
         i.next <<= i + 1
         r1 = pyrtl.Register(bitwidth=3, name='r1')
         r2 = pyrtl.Register(bitwidth=3, name='r2')
         with pyrtl.conditional_assignment:
             with r1 < 3:
                 r1.next |= r1 + 1
-            with pyrtl.otherwise: pass
+            with pyrtl.otherwise:
+                pass
             with r2 < 3:
                 r2.next |= r2 + 1
         self.check_trace(' i 01230123\nr1 01233333\nr2 01233333\n')
 
     def test_one_deep_nested_non_exclusive_condition(self):
         i = pyrtl.Register(bitwidth=2, name='i')
         i.next <<= i + 1
         r1 = pyrtl.Register(bitwidth=3, name='r1')
         r2 = pyrtl.Register(bitwidth=3, name='r2')
         with pyrtl.conditional_assignment:
             with (i == 2) | (i == 3):
                 with r1 < 3:
                     r1.next |= r1 + 2
-                with pyrtl.otherwise: pass
+                with pyrtl.otherwise:
+                    pass
                 with r2 < 3:
                     r2.next |= r2 + 2
         self.check_trace(' i 01230123\nr1 00024444\nr2 00024444\n')
 
     def test_overlaping_assignments_in_non_exclusive_assignments(self):
         i = pyrtl.Register(bitwidth=2, name='i')
         i.next <<= i + 1
         r1 = pyrtl.Register(bitwidth=3, name='r1')
         r2 = pyrtl.Register(bitwidth=3, name='r2')
         with pyrtl.conditional_assignment:
             with r1 < 3:
                 r1.next |= r1 + 1
-            with pyrtl.otherwise: pass
+            with pyrtl.otherwise:
+                pass
             with r2 < 3:
                 with self.assertRaises(pyrtl.PyrtlError):
                     r1.next |= r2 + 1
 
     def test_other_overlaping_assignments_in_non_exclusive_assignments(self):
         i = pyrtl.Register(bitwidth=2, name='i')
         i.next <<= i + 1
         r1 = pyrtl.Register(bitwidth=3, name='r1')
         r2 = pyrtl.Register(bitwidth=3, name='r2')
         with pyrtl.conditional_assignment:
             with r1 < 3:
                 r1.next |= r1 + 1
-            with pyrtl.otherwise: pass
+            with pyrtl.otherwise:
+                pass
             with r2 < 3:
-                with i!=0:
+                with i != 0:
                     with self.assertRaises(pyrtl.PyrtlError):
                         r1.next |= r2 + 1
 
 # ---------------------------------------------------------------
 
 
 class TestSuperWireConditionalBlock(unittest.TestCase):
@@ -420,27 +422,27 @@
 
     def test_super_stress_test(self):
         allin = [pyrtl.Input(1, n) for n in 'abxyijkmzcd']
         a, b, x, y, i, j, k, m, z, c, d = allin
         allout = [pyrtl.Output(4, 'var' + str(index)) for index in range(5)]
         var0, var1, var2, var3, var4 = allout
 
-        """ 
+        """
          1  with a:  # a
          2  with b:  # not(a) and b
          3      with x:  # not(a) and b and x
          4      with otherwise:  # not(a) and b and not(x)
          5      with y:  # not(a) and b and y;  check(3,4)
          6          with i:  # not(a) and b and y and i;  check(3,4)
          7          with j:  # not(a) and b and y and not(i) and j;  check(3,4)
          8          with otherwise:  # not(a) and b and y and not(i) and not(j):  check(3,4)
          9          with k:  # not(a) and b and y and k;  check(3,4,6,7,8)
          8          with otherwise:  # not(a) and b and y and not(k):  check(?)
         10          with m:  # not(a) and b and y and m;  check(?)
-        11  with otherwise:  #not(a) and not(b)     
+        11  with otherwise:  #not(a) and not(b)
         12      with z: #not(a) and not(b) and z
         13  with c:  #c;  check(1,2,3,4,5,6,7,8,9,10,11,12)
         14  with d:  #not(c) and d;  check(1,2,3,4,5,6,7,8,9,10,11,12)
         """
 
         with pyrtl.conditional_assignment:
             with a:
@@ -517,9 +519,10 @@
                 t4 = 2
             self.assertEqual(v(var0), t0)
             self.assertEqual(v(var1), t1)
             self.assertEqual(v(var2), t2)
             self.assertEqual(v(var3), t3)
             self.assertEqual(v(var4), t4)
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_wire.py` & `pyrtl-0.9.0/tests/test_wire.py`

 * *Files 7% similar despite different names*

```diff
@@ -231,19 +231,31 @@
     def setUp(self):
         pyrtl.reset_working_block()
 
     def test_integers(self):
         self.check_const(1, 1, 1)
         self.check_const(5, 5, 3)
         self.check_const(1, 1, 5, bitwidth=5)
+        self.check_const(0, 0b0, 1)
+        self.check_const(0, 0b0, 1, signed=True)
+        self.check_const(1, 0b01, 2, signed=True)
+        self.check_const(2, 0b010, 3, signed=True)
+        self.check_const(3, 0b011, 3, signed=True)
+        self.check_const(4, 0b0100, 4, signed=True)
+        self.check_const(5, 0b0101, 4, signed=True)
 
     def test_neg_integers(self):
         self.check_const(-1, 0b11111, 5, bitwidth=5)
         self.check_const(-2, 0b110, 3, bitwidth=3)
         self.check_const(-5, 0b1011, 4, bitwidth=4)
+        self.check_const(-1, 0b1, 1, signed=True)
+        self.check_const(-2, 0b10, 2, signed=True)
+        self.check_const(-3, 0b101, 3, signed=True)
+        self.check_const(-4, 0b100, 3, signed=True)
+        self.check_const(-5, 0b1011, 4, signed=True)
 
     def test_too_big(self):
         self.assert_bad_const(5, 2)
 
     def test_invalid_bitwidth(self):
         self.assert_bad_const(1, 0)
         self.assert_bad_const(1, -1)
@@ -300,14 +312,26 @@
         self.assert_bad_const([])
 
     def test_assignment(self):
         with self.assertRaises(pyrtl.PyrtlError):
             c = pyrtl.Const(4)
             c <<= 3
 
+    def test_named(self):
+        block = pyrtl.working_block()
+        c = pyrtl.Const(20, name="archid")
+        self.assertIn("archid", block.wirevector_by_name)
+        self.assertIn(c, block.wirevector_set)
+        self.assertEqual(c.val, 20)
+        c.name = "vendorid"
+        self.assertNotIn("archid", block.wirevector_by_name)
+        self.assertIn("vendorid", block.wirevector_by_name)
+        self.assertIn(c, block.wirevector_set)
+        self.assertEqual(c.val, 20)
+
     def check_const(self, val_in, expected_val, expected_bitwidth, **kargs):
         c = pyrtl.Const(val_in, **kargs)
         self.assertEqual(c.val, expected_val)
         self.assertEqual(c.bitwidth, expected_bitwidth)
 
     def assert_bad_const(self, *args, **kwargs):
         with self.assertRaises(pyrtl.PyrtlError):
@@ -351,7 +375,11 @@
             call_stack = wire.init_call_stack
 
     def test_get_call_stack(self):
         pyrtl.set_debug_mode(True)
         wire = pyrtl.WireVector()
         call_stack = wire.init_call_stack
         self.assertIsInstance(call_stack, list)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_simulation.py` & `pyrtl-0.9.0/tests/test_simulation.py`

 * *Files 24% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     def test_print_trace_single_dig_notcompact(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") + self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
                 self.in1: i,
-                self.in2: 5-i
+                self.in2: 5 - i
             })
         correct_outp = ("      --- Values in base 10 ---\n"
                         "in1       0 1 2 3 4\n"
                         "in1_probe 0 1 2 3 4\n"
                         "in2       5 4 3 2 1\n"
                         "out       5 5 5 5 5\n")
         output = six.StringIO()
@@ -156,16 +156,16 @@
 
     def test_print_trace_base2(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") + self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
-                self.in1: 4*i,
-                self.in2: 4*(5 - i)
+                self.in1: 4 * i,
+                self.in2: 4 * (5 - i)
             })
         correct_outp = ("      --- Values in base 2 ---\n"
                         "in1           0   100  1000  1100 10000\n"
                         "in1_probe     0   100  1000  1100 10000\n"
                         "in2       10100 10000  1100  1000   100\n"
                         "out       10100 10100 10100 10100 10100\n")
         output = six.StringIO()
@@ -174,16 +174,16 @@
 
     def test_print_trace_base8(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") + self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
-                self.in1: 6*i,
-                self.in2: 6*(5 - i)
+                self.in1: 6 * i,
+                self.in2: 6 * (5 - i)
             })
         correct_outp = ("      --- Values in base 8 ---\n"
                         "in1        0  6 14 22 30\n"
                         "in1_probe  0  6 14 22 30\n"
                         "in2       36 30 22 14  6\n"
                         "out       36 36 36 36 36\n")
         output = six.StringIO()
@@ -192,16 +192,16 @@
 
     def test_print_trace_base16(self):
         self.out <<= pyrtl.probe(self.in1, "in1_probe") * self.in2
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(5):
             sim.step({
-                self.in1: 9*i,
-                self.in2: 9*(5 - i)
+                self.in1: 9 * i,
+                self.in2: 9 * (5 - i)
             })
         correct_outp = ("      --- Values in base 16 ---\n"
                         "in1         0   9  12  1b  24\n"
                         "in1_probe   0   9  12  1b  24\n"
                         "in2        2d  24  1b  12   9\n"
                         "out         0 144 1e6 1e6 144\n")
         output = six.StringIO()
@@ -256,28 +256,72 @@
         out2 = pyrtl.Output(16, "out3")
         out1 <<= in1 + in2
         out2 <<= in3 | truth
         sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=sim_trace)
         for i in range(10):
             sim.step({
-                'in1': 2*i,
-                'in2': 3*i,
-                'in3': 40 - 2*i
+                'in1': 2 * i,
+                'in2': 3 * i,
+                'in3': 40 - 2 * i
             })
         correct_outp = (" --- Values in base 10 ---\n"
                         "in1   0  2  4  6  8 10 12 14 16 18\n"
                         "in2   0  3  6  9 12 15 18 21 24 27\n"
                         "in3  40 38 36 34 32 30 28 26 24 22\n"
                         "out2  0  5 10 15 20 25 30 35 40 45\n"
                         "out3 41 39 37 35 33 31 29 27 25 23\n")
         output = six.StringIO()
         sim_trace.print_trace(output)
         self.assertEqual(output.getvalue(), correct_outp)
 
+    def test_consts_from_int_enums(self):
+        from enum import IntEnum
+
+        class MyEnum(IntEnum):
+            A = 0
+            B = 1
+            C = 3
+
+        i = pyrtl.Input(max(MyEnum).bit_length(), 'i')
+        o = pyrtl.Output(1, 'o')
+        with pyrtl.conditional_assignment:
+            with (i == MyEnum.A) | (i == MyEnum.B):
+                o |= 0
+            with pyrtl.otherwise:
+                o |= 1
+
+        trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=trace)
+
+        sim.step({'i': MyEnum.A})
+        self.assertEqual(sim.inspect(o), 0)
+        sim.step({'i': MyEnum.B})
+        self.assertEqual(sim.inspect(o), 0)
+        sim.step({'i': MyEnum.C})
+        self.assertEqual(sim.inspect(o), 1)
+
+    def test_named_consts(self):
+        in1 = pyrtl.Input(8, "in1")
+        c1 = pyrtl.Const(1, 1, "c1")
+        out1 = pyrtl.Output(16, "out1")
+        out1 <<= in1 + c1
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+        for i in range(10):
+            sim.step({
+                'in1': 2 * i,
+            })
+        correct_outp = (" --- Values in base 10 ---\n"
+                        "c1    1  1  1  1  1  1  1  1  1  1\n"
+                        "in1   0  2  4  6  8 10 12 14 16 18\n"
+                        "out1  1  3  5  7  9 11 13 15 17 19\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_outp)
 
 
 class SimInputValidationBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def test_input_out_of_bitwidth(self):
@@ -298,14 +342,414 @@
         c = pyrtl.Output()
         c <<= a + b
 
         with self.assertRaises(pyrtl.PyrtlError):
             sim_trace = pyrtl.SimulationTrace()
 
 
+class SimStepAccessInternalMemoryBase(unittest.TestCase):
+
+    def setUp(self):
+        pyrtl.reset_working_block()
+
+    def test_step_with_internal_memory(self):
+
+        def special_memory(read_addr, write_addr, data, wen):
+            mem = pyrtl.MemBlock(bitwidth=32, addrwidth=5, name='special_mem')
+            mem[write_addr] <<= pyrtl.MemBlock.EnabledWrite(data, wen & (write_addr > 0))
+            return mem[read_addr]
+
+        read_addr = pyrtl.Input(5, 'read_addr')
+        write_addr = pyrtl.Input(5, 'write_addr')
+        data = pyrtl.Input(32, 'data')
+        wen = pyrtl.Input(1, 'wen')
+        res = pyrtl.Output(32, 'res')
+
+        res <<= special_memory(read_addr, write_addr, data, wen)
+
+        # Can only access it after the `special_memory` block has been instantiated/called
+        special_mem = pyrtl.working_block().get_memblock_by_name('special_mem')
+
+        sim = self.sim(memory_value_map={
+            special_mem: {
+                0: 5,
+                1: 6,
+                2: 7,
+                3: 8,
+            }
+        })
+
+        inputs = {
+            'read_addr': '012012',
+            'write_addr': '012012',
+            'data': '890333',
+            'wen': '111000',
+        }
+        expected = {
+            'res': '567590',
+        }
+        # This should not fail
+        sim.step_multiple(inputs, expected)
+
+        # Let's check the memory contents too
+        mem_map = sim.inspect_mem(special_mem)
+        self.assertEqual(mem_map[0], 5)
+        self.assertEqual(mem_map[1], 9)
+        self.assertEqual(mem_map[2], 0)
+        self.assertEqual(mem_map[3], 8)
+
+
+class SimStepMultipleBase(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+        in1 = pyrtl.Input(4, "in1")
+        in2 = pyrtl.Input(4, "in2")
+        out1 = pyrtl.Output(4, "out1")
+        out1 <<= (in1 ^ in2) + pyrtl.Const(1)
+        out2 = pyrtl.Output(4, "out2")
+        out2 <<= in1 | in2
+        self.inputs = {
+            'in1': [0, 1, 3, 15, 14],
+            'in2': [6, 6, 6, 6, 6],
+        }
+
+    def test_step_multiple_nsteps_no_inputs(self):
+        pyrtl.reset_working_block()
+        a = pyrtl.Register(8)
+        b = pyrtl.Output(8, 'b')
+        a.next <<= a + 1
+        b <<= a
+
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+        sim.step_multiple(nsteps=5)
+
+        correct_output = ("--- Values in base 10 ---\n"
+                          "b 0 1 2 3 4\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_nsteps_gt_ninputs(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple(self.inputs, nsteps=6)
+        self.assertEqual(
+            str(error.exception),
+            'nsteps is specified but is greater than the '
+            'number of values supplied for each input'
+        )
+
+    def test_step_multiple_no_inputs(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple()
+        self.assertEqual(str(error.exception),
+                         'need to supply either input values '
+                         'or a number of steps to simulate')
+
+    def test_step_multiple_bad_nsteps1(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple({'in1': [], 'in2': []})
+        self.assertEqual(str(error.exception),
+                         'must simulate at least one step')
+
+    def test_step_multiple_bad_nsteps2(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple(self.inputs, nsteps=-1)
+        self.assertEqual(str(error.exception),
+                         'must simulate at least one step')
+
+    def test_step_multiple_no_values_for_each_step_of_input(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple({'in1': [0, 1, 3], 'in2': [1]})
+        self.assertEqual(str(error.exception),
+                         'must supply a value for each provided wire '
+                         'for each step of simulation')
+
+    def test_step_multiple_no_values_for_each_step_of_given_outputs(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        with self.assertRaises(pyrtl.PyrtlError) as error:
+            sim.step_multiple(self.inputs,
+                              {'out1': [7, 8, 6, 10, 9],
+                               'out2': [6, 7, 7, 15]})
+        self.assertEqual(str(error.exception),
+                         'any expected outputs must have a supplied value '
+                         'each step of simulation')
+
+    def test_step_multiple_no_expected_check(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        sim.step_multiple(self.inputs)
+
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1   0  1  3 15 14\n"
+                          "in2   6  6  6  6  6\n"
+                          "out1  7  8  6 10  9\n"
+                          "out2  6  7  7 15 14\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_no_errors(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 8, 6, 10, 9],
+            'out2': [6, 7, 7, 15, 14],
+        }
+        sim.step_multiple(self.inputs, expected)
+
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1   0  1  3 15 14\n"
+                          "in2   6  6  6  6  6\n"
+                          "out1  7  8  6 10  9\n"
+                          "out2  6  7  7 15 14\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_no_errors_nsteps_specified(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 8, 6, 10, 9],
+            'out2': [6, 7, 7, 15, 14],
+        }
+        sim.step_multiple(self.inputs, expected, nsteps=3)
+
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1  0 1 3\n"
+                          "in2  6 6 6\n"
+                          "out1 7 8 6\n"
+                          "out2 6 7 7\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_many_errors_report_only_first(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 9, 4, 10, 9],
+            'out2': [6, 2, 7, 8, 14],
+        }
+        output = six.StringIO()
+        sim.step_multiple(self.inputs, expected, file=output, stop_after_first_error=True)
+
+        # Test the output about unexpected values
+        correct_output = ("Unexpected output (stopped after step with first error):\n"
+                          " step       name expected   actual\n"
+                          "    1       out1        9        8\n"
+                          "    1       out2        2        7\n")
+        self.assertEqual(output.getvalue(), correct_output)
+
+        # Test that the trace stopped after the step with the first error
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1  0 1\n"
+                          "in2  6 6\n"
+                          "out1 7 8\n"
+                          "out2 6 7\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+    def test_step_multiple_many_errors_report_all(self):
+        sim_trace = pyrtl.SimulationTrace()
+        sim = self.sim(tracer=sim_trace)
+
+        expected = {
+            'out1': [7, 9, 4, 10, 9],
+            'out2': [6, 2, 7, 8, 14],
+        }
+        output = six.StringIO()
+        sim.step_multiple(self.inputs, expected, file=output)
+
+        # Test the output about unexpected values
+        correct_output = ("Unexpected output on one or more steps:\n"
+                          " step       name expected   actual\n"
+                          "    1       out1        9        8\n"
+                          "    1       out2        2        7\n"
+                          "    2       out1        4        6\n"
+                          "    3       out2        8       15\n")
+        self.assertEqual(output.getvalue(), correct_output)
+
+        # Test that the trace still produced all the steps
+        correct_output = (" --- Values in base 10 ---\n"
+                          "in1   0  1  3 15 14\n"
+                          "in2   6  6  6  6  6\n"
+                          "out1  7  8  6 10  9\n"
+                          "out2  6  7  7 15 14\n")
+        output = six.StringIO()
+        sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_output)
+
+
+class TestStepBundleBase(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+
+    def test_step_with_bundle_from_tuples(self):
+        rformat = [
+            ("funct7", 7),
+            ("rs2", 5),
+            ("rs1", 5),
+            ("funct3", 3),
+            ("rd", 5),
+            ("opcode", 7),
+        ]
+        self.step_with_bundle(rformat)
+
+    def test_step_with_bundle_from_dict(self):
+        rformat = {
+            "funct7": 7,
+            "rs2": 5,
+            "rs1": 5,
+            "funct3": 3,
+            "rd": 5,
+            "opcode": 7
+        }
+        if six.PY2:
+            with self.assertRaises(pyrtl.PyrtlError) as ex:
+                self.step_with_bundle(rformat)
+            self.assertEqual(
+                str(ex.exception),
+                "For Python versions < 3.7, the dictionary used to instantiate "
+                "a Bundle must be explicitly ordered (i.e. OrderedDict)"
+            )
+        else:
+            self.step_with_bundle(rformat)
+
+    def test_step_with_bundle_from_class(self):
+        class RFormat:
+            funct7 = 7
+            rs2 = 5
+            rs1 = 5
+            funct3 = 3
+            rd = 5
+            opcode = 7
+        if six.PY2:
+            with self.assertRaises(pyrtl.PyrtlError) as ex:
+                self.step_with_bundle(RFormat)
+            self.assertEqual(
+                str(ex.exception),
+                "Passing a class as an argument to Bundle() is only "
+                "allowed for Python versions >= 3.7"
+            )
+        else:
+            self.step_with_bundle(RFormat)
+
+    def step_with_bundle(self, obj):
+        w = pyrtl.Bundle(obj, "inst")
+        #     funct7   rs2   rs1 funct3    rd  opcode
+        # 0b 0000010 01100 01010    000 01011 0010011
+        w <<= 0b00000100110001010000010110010011
+        r = pyrtl.Register(len(w))
+        f7 = r.as_bundle(obj).funct7
+        r.next <<= w
+        y = r.as_bundle(obj)
+
+        sim = pyrtl.Simulation()
+        sim.step({})
+        assert sim.inspect(w.funct7) == 0b0000010
+        assert sim.inspect(w.rs2) == 0b01100
+        assert sim.inspect(w.rs1) == 0b01010
+        assert sim.inspect(w.funct3) == 0b000
+        assert sim.inspect(w.rd) == 0b01011
+        assert sim.inspect(w.opcode) == 0b0010011
+        assert sim.inspect(r) == 0
+
+        sim.step({})
+        assert sim.inspect(r) == 0b00000100110001010000010110010011
+        assert sim.inspect(f7) == 0b0000010
+        assert sim.inspect(y.funct7) == 0b0000010
+        assert sim.inspect(y.rs2) == 0b01100
+        assert sim.inspect(y.rs1) == 0b01010
+        assert sim.inspect(y.funct3) == 0b000
+        assert sim.inspect(y.rd) == 0b01011
+        assert sim.inspect(y.opcode) == 0b0010011
+
+    def test_bad_write_to_bundle(self):
+        w = pyrtl.WireVector(8, 'w')
+        x = w.as_bundle([('a', 2), ('b', 3), ('c', 3)])
+        with self.assertRaises(pyrtl.PyrtlError):
+            x <<= 0b10101110
+            _sim = pyrtl.Simulation()
+
+    # Highly experimental, but seems to work right now
+    def test_good_write_to_bundle(self):
+        x = pyrtl.Input(1, 'x')
+
+        def t1():
+            w = pyrtl.WireVector(8)
+            with pyrtl.conditional_assignment:
+                with x:
+                    w |= 0b00101100
+                with pyrtl.otherwise:
+                    w |= 0b10010011
+            return w
+
+        def t3():
+            w = pyrtl.WireVector(8)
+            with pyrtl.conditional_assignment:
+                with x:
+                    w |= 0b11111111
+                with pyrtl.otherwise:
+                    w |= 0b00000000
+            return w
+
+        class Array:
+            # Returning a function which returns a WireVector
+            thread1 = (8, t1)
+            # Returning a function with returns a Const with explicit size
+            thread2 = (8, lambda: pyrtl.Const(0b01100110, 8))
+            # Returning a WireVector
+            thread3 = (8, t3())
+            # Returning a Const without an explicit size
+            thread4 = (8, pyrtl.Const(0b00000011))
+            # Returning a literal
+            thread5 = (8, 0b01000011)
+
+        if six.PY3:
+            w = pyrtl.Bundle(Array, 'w')
+            sim = pyrtl.Simulation()
+            sim.step({'x': 1})
+            assert sim.inspect(w.thread1) == 0b00101100
+            assert sim.inspect(w.thread2) == 0b01100110
+            assert sim.inspect(w.thread3) == 0b11111111
+            assert sim.inspect(w.thread4) == 0b00000011
+            assert sim.inspect(w.thread5) == 0b01000011
+
+            sim.step({'x': 0})
+            assert sim.inspect(w.thread1) == 0b10010011
+            assert sim.inspect(w.thread2) == 0b01100110
+            assert sim.inspect(w.thread3) == 0b00000000
+            assert sim.inspect(w.thread4) == 0b00000011
+            assert sim.inspect(w.thread5) == 0b01000011
+
+
 class TraceWithAdderBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         bitwidth = 3
         self.r = pyrtl.Register(bitwidth=bitwidth, name='r')
         self.result = _basic_add(self.r, pyrtl.Const(1).zero_extended(bitwidth))
         self.r.next <<= self.result
@@ -318,18 +762,16 @@
 
         # step through 15 cycles
         for i in range(15):
             sim.step({})
 
         output = six.StringIO()
         sim_trace.print_trace(output, compact=True)
-        __IPYTHON__ = True
-        sim_trace.render_trace()  # want to make sure the code at least runs
-        __IPYTHON__ = False
-        sim_trace.render_trace()  # want to make sure the code at least runs
+        file = six.StringIO()
+        sim_trace.render_trace(file=file)  # want to make sure the code at least runs
         self.assertEqual(output.getvalue(), 'r 012345670123456\n')
         self.assertEqual(sim.inspect(self.r), 6)
 
 
 class SimulationVCDWithAdderBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
@@ -465,15 +907,15 @@
         input_signals = [[0, 1, 4, 5],
                          [4, 1, 0, 5],
                          [0, 4, 1, 6],
                          [1, 1, 0, 0],
                          [6, 0, 6, 7]]
         for signals in input_signals:
             sim.step({self.read_addr1: signals[0], self.read_addr2: signals[1],
-                           self.write_addr: signals[2], self.write_data: signals[3]})
+                      self.write_addr: signals[2], self.write_data: signals[3]})
 
         output = six.StringIO()
         self.sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), 'o1 05560\no2 00560\n')
 
     def test_simple2_memblock(self):
         sim = self.sim(tracer=self.sim_trace)
@@ -550,26 +992,69 @@
         mem_val_map = {self.mem1: {0: 0, 1: 1},
                        self.mem2: {0: 4, 1: 5}}
         self.sim_trace = pyrtl.SimulationTrace()
         sim = self.sim(tracer=self.sim_trace, memory_value_map=mem_val_map)
         for i in range(2, 8):
             sim.step({
                 self.read_addr1: i,
-                self.read_addr2: 8-i+1,
+                self.read_addr2: 8 - i + 1,
                 read_addr3: i,
                 self.write_addr: 0,
                 self.write_data: 0
             })
         output = six.StringIO()
         self.sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), 'o1 000000\n'
                                             'o2 000000\n'
                                             'o3 000000\n')
 
 
+class MemBlockLargeBase(unittest.TestCase):
+    def setUp(self):
+        pyrtl.reset_working_block()
+        self.bitwidth = 68
+        self.addrwidth = 32
+        self.output1 = pyrtl.Output(self.bitwidth, "o1")
+        self.output2 = pyrtl.Output(self.bitwidth, "o2")
+        self.read_addr1 = pyrtl.Input(self.addrwidth)
+        self.read_addr2 = pyrtl.Input(self.addrwidth)
+        self.write_addr = pyrtl.Input(self.addrwidth)
+        self.write_data = pyrtl.Input(self.bitwidth)
+        self.mem = pyrtl.MemBlock(bitwidth=self.bitwidth, addrwidth=self.addrwidth, name='mem')
+        self.output1 <<= self.mem[self.read_addr1]
+        self.output2 <<= self.mem[self.read_addr2]
+        self.mem[self.write_addr] <<= self.write_data
+
+        # build the actual simulation environment
+        self.sim_trace = pyrtl.SimulationTrace()
+
+    def test_mem_blocks_very_large(self):
+        ''' Tests support of very large memories (i.e. address width > 30 bits),
+            and that limbs are handled appropriately for bitwidths > 64 '''
+        sim = self.sim(tracer=self.sim_trace)
+
+        write_data = 0x20000000040000012  # 68 bits
+        input_signals = [[0, 1, 0xffffffff, write_data],
+                         [0xffffffff, 1, 0, write_data],
+                         [0, 0xffffffff, 0xf0000001, 6],
+                         [0xf0000001, 0xf0000001, 0, 0],
+                         [6, 0, 6, 7]]
+        for signals in input_signals:
+            sim.step({self.read_addr1: signals[0], self.read_addr2: signals[1],
+                      self.write_addr: signals[2], self.write_data: signals[3]})
+
+        output = six.StringIO()
+        correct_outp = ("--- Values in base 10 ---\n"
+                        "o1                    0 %d %d                    6                    0\n"
+                        "o2                    0                    0 %d                    6                    0\n"  # noqa
+                        % (write_data, write_data, write_data))
+        self.sim_trace.print_trace(output)
+        self.assertEqual(output.getvalue(), correct_outp)
+
+
 class RegisterDefaultsBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
         self.i = pyrtl.Input(bitwidth=3)
         self.r1 = pyrtl.Register(name='r1', bitwidth=3)
         self.r2 = pyrtl.Register(name='r2', bitwidth=3)
         self.o = pyrtl.Output(name='o', bitwidth=3)
@@ -586,21 +1071,24 @@
         sim_trace.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), correct_string)
 
     def test_default_value(self):
         self.check_trace(' o 55012345\nr1 50123456\nr2 55012345\n', default_value=5)
 
     def test_register_map(self):
-        self.check_trace(' o 36012345\nr1 60123456\nr2 36012345\n', register_value_map={self.r1: 6, self.r2: 3})
+        self.check_trace(' o 36012345\nr1 60123456\nr2 36012345\n',
+                         register_value_map={self.r1: 6, self.r2: 3})
 
     def test_partial_map(self):
-        self.check_trace(' o 06012345\nr1 60123456\nr2 06012345\n', register_value_map={self.r1: 6})
+        self.check_trace(' o 06012345\nr1 60123456\nr2 06012345\n',
+                         register_value_map={self.r1: 6})
 
     def test_map_and_default(self):
-        self.check_trace(' o 56012345\nr1 60123456\nr2 56012345\n', default_value=5, register_value_map={self.r1: 6})
+        self.check_trace(' o 56012345\nr1 60123456\nr2 56012345\n', default_value=5,
+                         register_value_map={self.r1: 6})
 
 
 class RomBlockSimBase(unittest.TestCase):
     def setUp(self):
         pyrtl.reset_working_block()
 
     def generate_expected_output(self, data_tuples, length):
@@ -620,15 +1108,15 @@
         output = six.StringIO()
         sim_trace_a.print_trace(output, compact=True)
         self.assertEqual(output.getvalue(), expected_output)
 
     def test_function_RomBlock(self):
 
         def rom_data_function(add):
-            return int((add + 5)/2)
+            return int((add + 5) / 2)
 
         pyrtl.reset_working_block()
         self.bitwidth = 4
         self.addrwidth = 4
         self.output1 = pyrtl.Output(self.bitwidth, "o1")
         self.output2 = pyrtl.Output(self.bitwidth, "o2")
         self.read_addr1 = pyrtl.Input(self.addrwidth)
@@ -639,25 +1127,25 @@
         self.output2 <<= self.rom[self.read_addr2]
         # build the actual simulation environment
         self.sim_trace = pyrtl.SimulationTrace()
         self.sim = self.sim(tracer=self.sim_trace)
 
         input_signals = {}
         for i in range(0, 5):
-            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2*i}
+            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2 * i}
             self.sim.step(input_signals[i])
 
         exp_out = self.generate_expected_output((("o1", lambda x: rom_data_function(x)),
-                                                 ("o2", lambda x: rom_data_function(2*x))), 6)
+                                                 ("o2", lambda x: rom_data_function(2 * x))), 6)
         self.compareIO(self.sim_trace, exp_out)
 
     def test_function_RomBlock_with_optimization(self):
 
         def rom_data_function(add):
-            return int((add + 5)/2)
+            return int((add + 5) / 2)
 
         pyrtl.reset_working_block()
         self.bitwidth = 4
         self.addrwidth = 4
         self.output1 = pyrtl.Output(self.bitwidth, "o1")
         self.output2 = pyrtl.Output(self.bitwidth, "o2")
 
@@ -672,21 +1160,21 @@
         pyrtl.optimize()
         # build the actual simulation environment
         self.sim_trace = pyrtl.SimulationTrace()
         self.sim = self.sim(tracer=self.sim_trace)
 
         input_signals = {}
         for i in range(0, 5):
-            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2*i}
-            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2*i}
+            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2 * i}
+            input_signals[i] = {self.read_addr1: i, self.read_addr2: 2 * i}
             self.sim.step(input_signals[i])
 
         # exp_out = self.generate_expected_output((("o1", lambda x: rom_data_function(x) - 1),
         exp_out = self.generate_expected_output((("o1", lambda x: rom_data_function(x)),
-                                                 ("o2", lambda x: rom_data_function(2*x))), 6)
+                                                 ("o2", lambda x: rom_data_function(2 * x))), 6)
         self.compareIO(self.sim_trace, exp_out)
 
     def test_rom_out_of_range_error(self):
         rom_data_array = [15, 13, 11, 9, 7, 5, 3]
         rom1 = pyrtl.RomBlock(bitwidth=4, addrwidth=3, romdata=rom_data_array)
         rom_add_1 = pyrtl.Input(3, "rom_in")
         rom_out_1 = pyrtl.Output(4, "rom_out_1")
@@ -800,14 +1288,15 @@
             raise Exception("You should be making unittests that are compatible with"
                             "both Fastsim and Simulation")
         for sim in sims:
             unit_name = "Test" + name + sim.__name__
             unittests[unit_name] = type(unit_name, (v,), {'sim': sim})
     g.update(unittests)
 
+
 # add compiledsim here if you want to unittest that as well
 sims = (pyrtl.Simulation, pyrtl.FastSimulation)
 make_unittests()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyrtl-0.8.7/tests/test_estimate.py` & `pyrtl-0.9.0/tests/test_estimate.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,62 +17,62 @@
         a = pyrtl.Const(2, 8)
         b = pyrtl.Const(85, 8)
         zero = pyrtl.Const(0, 1)
         reg = pyrtl.Register(8)
         mem = pyrtl.MemBlock(8, 8)
         out = pyrtl.Output(8)
         nota, aLSB, athenb, aORb, aANDb, aNANDb, \
-        aXORb, aequalsb, altb, agtb, aselectb, \
-        aplusb, bminusa, atimesb, memread = [pyrtl.Output() for i in range(15)]
+            aXORb, aequalsb, altb, agtb, aselectb, \
+            aplusb, bminusa, atimesb, memread = [pyrtl.Output() for i in range(15)]
         out <<= zero
         nota <<= ~a
         aLSB <<= a[0]
         athenb <<= pyrtl.concat(a, b)
         aORb <<= a | b
         aANDb <<= a & b
         aNANDb <<= a.nand(b)
         aXORb <<= a ^ b
-        aequalsb <<= a==b
+        aequalsb <<= a == b
         altb <<= a < b
         agtb <<= a > b
         aselectb <<= pyrtl.select(zero, a, b)
         reg.next <<= a
         aplusb <<= a + b
         bminusa <<= a - b
-        atimesb <<= a*b
+        atimesb <<= a * b
         memread <<= mem[0]
         mem[1] <<= a
         self.assertEquals(estimate.area_estimation(), (0.00734386752, 0.01879779717361501))
 
     def test_area_est_unchanged_with_rom(self):
         a = pyrtl.Const(2, 8)
         b = pyrtl.Const(85, 8)
         zero = pyrtl.Const(0, 1)
         reg = pyrtl.Register(8)
-        mem = pyrtl.RomBlock(8, 8, romdata=list(range(0,256)))
+        mem = pyrtl.RomBlock(8, 8, romdata=list(range(0, 256)))
         out = pyrtl.Output(8)
         nota, aLSB, athenb, aORb, aANDb, aNANDb, \
-        aXORb, aequalsb, altb, agtb, aselectb, \
-        aplusb, bminusa, atimesb, memread = [pyrtl.Output() for i in range(15)]
+            aXORb, aequalsb, altb, agtb, aselectb, \
+            aplusb, bminusa, atimesb, memread = [pyrtl.Output() for i in range(15)]
         out <<= zero
         nota <<= ~a
         aLSB <<= a[0]
         athenb <<= pyrtl.concat(a, b)
         aORb <<= a | b
         aANDb <<= a & b
         aNANDb <<= a.nand(b)
         aXORb <<= a ^ b
-        aequalsb <<= a==b
+        aequalsb <<= a == b
         altb <<= a < b
         agtb <<= a > b
         aselectb <<= pyrtl.select(zero, a, b)
         reg.next <<= a
         aplusb <<= a + b
         bminusa <<= a - b
-        atimesb <<= a*b
+        atimesb <<= a * b
         memread <<= mem[reg]
         self.assertEquals(estimate.area_estimation(), (0.00734386752, 0.001879779717361501))
 
 
 class TestTimingEstimate(unittest.TestCase):
 
     def setUp(self):
@@ -82,16 +82,16 @@
         a = pyrtl.Const(2, 8)
         b = pyrtl.Const(85, 8)
         zero = pyrtl.Const(0, 1)
         reg = pyrtl.Register(8)
         mem = pyrtl.MemBlock(8, 8)
         out = pyrtl.Output(8)
         nota, aLSB, athenb, aORb, aANDb, aNANDb, \
-        aXORb, aequalsb, altb, agtb, aselectb, \
-        aplusb, bminusa, atimesb, memread = [pyrtl.Output() for i in range(15)]
+            aXORb, aequalsb, altb, agtb, aselectb, \
+            aplusb, bminusa, atimesb, memread = [pyrtl.Output() for i in range(15)]
         out <<= zero
         nota <<= ~a
         aLSB <<= a[0]
         athenb <<= pyrtl.concat(a, b)
         aORb <<= a | b
         aANDb <<= a & b
         aNANDb <<= a.nand(b)
@@ -106,12 +106,12 @@
         atimesb <<= a * b
         memread <<= mem[0]
         mem[1] <<= a
         timing = estimate.TimingAnalysis()
         self.assertEqual(timing.max_freq(), 610.2770657878676)
         self.assertEquals(timing.max_length(), 1255.6000000000001)
 
+
 class TestYosysInterface(unittest.TestCase):
 
     def setUp(self):
         pyrtl.reset_working_block()
-
```

### Comparing `pyrtl-0.8.7/tests/test_examples.py` & `pyrtl-0.9.0/tests/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,13 +18,13 @@
     x = __file__
     for file in glob.iglob(os.path.dirname(__file__) + "/../examples/*.py"):
         yield example_t, os.path.realpath(file)
 
 
 # note that this function cannot start with "test"
 def example_t(file):
-    print("testing file: " + file)
+    # print("testing file: " + file)
     pyrtl.reset_working_block()
     try:
         output = subprocess.check_output(['python', file])
     except subprocess.CalledProcessError as e:
         raise e
```

### Comparing `pyrtl-0.8.7/README.md` & `pyrtl-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrtl-0.8.7/setup.py` & `pyrtl-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrtl',
-    version = '0.8.7', #VERSION
+    version = '0.9.0', #VERSION
     packages =  find_packages(),
     description = 'RTL-level Hardware Design and Simulation Toolkit',
     author =  'Timothy Sherwood, John Clow, and UCSBarchlab',
     author_email =  'sherwood@cs.ucsb.edu',
     url =  'http://ucsbarchlab.github.io/PyRTL/',
-    download_url = 'https://github.com/UCSBarchlab/PyRTL/tarball/0.8.7',  #VERSION
+    download_url = 'https://github.com/UCSBarchlab/PyRTL/tarball/0.9.0',  #VERSION
     install_requires =  ['six'],
     tests_require =  ['tox','nose'],
     extras_require =  {
         'blif parsing': ['pyparsing']
         },
     classifiers = [
         'Development Status :: 4 - Beta',
```

