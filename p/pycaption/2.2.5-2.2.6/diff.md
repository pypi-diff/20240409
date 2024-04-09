# Comparing `tmp/pycaption-2.2.5.tar.gz` & `tmp/pycaption-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaption-2.2.5.tar", last modified: Tue Feb 20 12:05:08 2024, max compression
+gzip compressed data, was "pycaption-2.2.6.tar", last modified: Tue Apr  9 09:48:24 2024, max compression
```

## Comparing `pycaption-2.2.5.tar` & `pycaption-2.2.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.326975 pycaption-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-02-20 12:04:52.000000 pycaption-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-20 12:04:52.000000 pycaption-2.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-20 12:05:08.326975 pycaption-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-20 12:04:52.000000 pycaption-2.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.314975 pycaption-2.2.5/pycaption/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.318975 pycaption-2.2.5/pycaption/dfxp/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/dfxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/dfxp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/dfxp/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/english.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/sami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.318975 pycaption-2.2.5/pycaption/scc/
--rw-r--r--   0 runner    (1001) docker     (127)    25323 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/scc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27884 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/scc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27806 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/scc/specialized_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/scc/state_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/scc/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-02-20 12:04:52.000000 pycaption-2.2.5/pycaption/webvtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.322975 pycaption-2.2.5/pycaption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-20 12:05:08.000000 pycaption-2.2.5/pycaption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-20 12:05:08.000000 pycaption-2.2.5/pycaption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 12:05:08.000000 pycaption-2.2.5/pycaption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-20 12:05:08.000000 pycaption-2.2.5/pycaption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-20 12:05:08.000000 pycaption-2.2.5/pycaption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 12:05:08.326975 pycaption-2.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-20 12:04:52.000000 pycaption-2.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.322975 pycaption-2.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:05:08.322975 pycaption-2.2.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/sami.py
--rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/translated_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/fixtures/webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_dfxp_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_dfxp_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_microdvd_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_sami.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_sami_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    24072 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_scc_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_scc_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_srt_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-02-20 12:04:52.000000 pycaption-2.2.5/tests/test_webvtt_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.950192 pycaption-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-09 09:48:12.000000 pycaption-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 09:48:12.000000 pycaption-2.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-09 09:48:24.946191 pycaption-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 09:48:12.000000 pycaption-2.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.938192 pycaption-2.2.6/pycaption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.942191 pycaption-2.2.6/pycaption/dfxp/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/dfxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/dfxp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/dfxp/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/english.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/sami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.942191 pycaption-2.2.6/pycaption/scc/
+-rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27793 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/specialized_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/state_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/scc/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-04-09 09:48:12.000000 pycaption-2.2.6/pycaption/webvtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.946191 pycaption-2.2.6/pycaption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 09:48:24.000000 pycaption-2.2.6/pycaption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:48:24.950192 pycaption-2.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 09:48:12.000000 pycaption-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.946191 pycaption-2.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:24.946191 pycaption-2.2.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/translated_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/fixtures/webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_dfxp_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_dfxp_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_microdvd_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_sami_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22989 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_scc_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_scc_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_srt_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-09 09:48:12.000000 pycaption-2.2.6/tests/test_webvtt_conversion.py
```

### Comparing `pycaption-2.2.5/LICENSE` & `pycaption-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/PKG-INFO` & `pycaption-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.5
+Version: 2.2.6
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.5/README.rst` & `pycaption-2.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/__init__.py` & `pycaption-2.2.6/pycaption/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/base.py` & `pycaption-2.2.6/pycaption/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/dfxp/base.py` & `pycaption-2.2.6/pycaption/dfxp/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/dfxp/extras.py` & `pycaption-2.2.6/pycaption/dfxp/extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/english.pickle` & `pycaption-2.2.6/pycaption/english.pickle`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/exceptions.py` & `pycaption-2.2.6/pycaption/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/geometry.py` & `pycaption-2.2.6/pycaption/geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/microdvd.py` & `pycaption-2.2.6/pycaption/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/sami.py` & `pycaption-2.2.6/pycaption/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/scc/__init__.py` & `pycaption-2.2.6/pycaption/scc/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,19 +77,19 @@
  dictionary. This is legacy logic, that I didn't know how to handle, and
  just carried over when implementing positioning.
 """
 
 import math
 import re
 import textwrap
-from collections import deque
+from collections import deque, defaultdict
 from copy import deepcopy
 
 from pycaption.base import (
-    BaseReader, BaseWriter, CaptionSet, CaptionNode,
+    BaseReader, BaseWriter, CaptionSet
 )
 from pycaption.exceptions import CaptionReadNoCaptions, InvalidInputError, \
     CaptionReadTimingError, CaptionLineLengthError
 from .constants import (
     HEADER, COMMANDS, SPECIAL_CHARS, EXTENDED_CHARS, CHARACTERS,
     MICROSECONDS_PER_CODEWORD, CHARACTER_TO_CODE,
     SPECIAL_OR_EXTENDED_CHAR_TO_CODE, PAC_BYTES_TO_POSITIONING_MAP,
@@ -228,24 +228,32 @@
             self._translate_line(line)
 
         self._flush_implicit_buffers(self.buffer_dict.active_key)
 
         captions = CaptionSet({lang: self.caption_stash.get_all()})
 
         # check captions for incorrect lengths
-        lines = []
+        lines_too_long = defaultdict(list)
         for caption in self.caption_stash._collection:
+            caption_start = caption.to_real_caption().format_start()
             caption_text = "".join(caption.to_real_caption().get_text_nodes())
-            lines.extend(caption_text.split("\n"))
-        lines_too_long = [line for line in lines if len(line) > 32]
-
-        if bool(lines_too_long):
-            msg = ""
-            for line in lines_too_long:
-                msg += line + f" - Length { len(line)}" + "\n"
+            text_too_long = [line for line in caption_text.split("\n") if len(line) > 32]
+            if caption_start in lines_too_long:
+                lines_too_long[caption_start] = text_too_long
+            else:
+                lines_too_long[caption_start].extend(text_too_long)
+
+        msg = ""
+        if bool(lines_too_long.keys()):
+            for key in lines_too_long:
+                if lines_too_long[key]:
+                    msg += f"around {key} - "
+                    for line in lines_too_long[key]:
+                        msg += line + f" - Length { len(line)}" + "\n"
+        if len(msg):
             raise CaptionLineLengthError(
                 f"32 character limit for caption cue in scc file.\n"
                 f"Lines longer than 32:\n"
                 f"{msg}"
             )
 
         for cap in captions.get_captions(lang):
@@ -297,35 +305,29 @@
         # split line in timestamp and words
         r = re.compile(r"([0-9:;]*)([\s\t]*)((.)*)")
         parts = r.findall(line.lower())
 
         self.time_translator.start_at(parts[0][0])
 
         # loop through each word
-        words = [word.strip() for word in parts[0][2].split(' ') if len(word) == 4]
-
-        for idx, word in enumerate(words):
-            self._translate_word(word, words, idx)
+        for word in parts[0][2].split(' '):
+            # ignore empty results or invalid commands
+            word = word.strip()
+            if len(word) == 4:
+                self._translate_word(word)
 
-    @staticmethod
-    def get_command(commands, idx):
-        try:
-            return commands[idx]
-        except IndexError:
-            return None
-
-    def _translate_word(self, word, words, idx):
-        if self._skip_double_command(word, words, idx):
+    def _translate_word(self, word):
+        if self._handle_double_command(word):
             # count frames for timing
             self.time_translator.increment_frames()
             return
         # first check if word is a command
         # TODO - check that all the positioning commands are here, or use
         # some other strategy to determine if the word is a command.
-        if word in COMMANDS or _is_pac_command(word) or word in PAC_TAB_OFFSET_COMMANDS:
+        if word in COMMANDS or _is_pac_command(word):
             self._translate_command(word)
 
         # second, check if word is a special character
         elif word in SPECIAL_CHARS:
             self._translate_special_char(word)
 
         elif word in EXTENDED_CHARS:
@@ -334,47 +336,39 @@
         # third, try to convert word into 2 characters
         else:
             self._translate_characters(word)
 
         # count frames for timing only after processing a command
         self.time_translator.increment_frames()
 
-    def _skip_double_command(self, word, words, idx):
+    def _handle_double_command(self, word):
         # If the caption is to be broadcast, each of the commands are doubled
         # up for redundancy in case the signal is garbled in transmission.
         # The decoder is programmed to ignore a second command when it is the
         # same as the first.
         # Also like codes, Special Characters are always doubled up,
         # with only one member of each pair being displayed.
-        next_command = self.get_command(words, idx + 1)
-        second_next = self.get_command(words, idx + 2)
-
         if word in COMMANDS or _is_pac_command(word) or word in SPECIAL_CHARS or word in EXTENDED_CHARS:
-            # skip duplicates, execute the last occurrence if not a positioning command
-            if word == self.last_command and not _is_pac_command(word):
+            if word == self.last_command:
                 self.last_command = ''
                 return True
-            # skip consecutive positioning commands, execute the last one
-            elif _is_pac_command(word) and _is_pac_command(next_command):
+            # Fix for the <position> <tab offset> <position> <tab offset>
+            # repetition
+            elif _is_pac_command(word) and word in self.last_command:
                 self.last_command = ''
                 return True
-            # Fix for the <position> <tab offset> <position> <tab offset> repetition
-            # execute the last positioning command
-            elif _is_pac_command(word) and next_command in PAC_TAB_OFFSET_COMMANDS and _is_pac_command(second_next):
-                self.last_command = ''
-                return True
-            # execute offset commands only if previous command is PAC and next is not PAC
             elif word in PAC_TAB_OFFSET_COMMANDS:
-                if _is_pac_command(self.last_command) and not _is_pac_command(next_command):
-                    self.last_command = word
+                if _is_pac_command(self.last_command):
+                    self.last_command += f" {word}"
                     return False
                 else:
                     return True
-            self.last_command = word
-            return False
+
+        self.last_command = word
+        return False
 
     def _translate_special_char(self, word):
         self.buffer.add_chars(SPECIAL_CHARS[word])
 
     def _translate_extended_char(self, word):
         self.buffer.remove_ascii_duplicate(EXTENDED_CHARS[word])
```

### Comparing `pycaption-2.2.5/pycaption/scc/constants.py` & `pycaption-2.2.6/pycaption/scc/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from itertools import product
-from collections import defaultdict
 
 COMMANDS = {
     '9420': '',
     '9429': '',
     '9425': '',
     '9426': '',
     '94a7': '',
@@ -983,16 +982,14 @@
 
 # Time to transmit a single codeword = 1 second / 29.97
 MICROSECONDS_PER_CODEWORD = 1000.0 * 1000.0 / (30.0 * 1000.0 / 1001.0)
 
 
 HEADER = 'Scenarist_SCC V1.0'
 
-UNHANDLED_COMMANDS = ["9120", "91ae", "912f", "91a1"]
-
 # taken from
 # http://www.theneitherworld.com/mcpoodle/SCC_TOOLS/DOCS/CC_CHARS.HTML
 INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION = {
     '¡': ["!", "i"],   # inverted exclamation mark
      '¤': ["C"],  # currency
      '¥': ["Y"],  # yen
      '¦': ["-"],  # broken bar
```

### Comparing `pycaption-2.2.5/pycaption/scc/specialized_collections.py` & `pycaption-2.2.6/pycaption/scc/specialized_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from ..base import CaptionList, Caption, CaptionNode
 from ..geometry import (
     UnitEnum, Size, Layout, Point, Alignment,
     VerticalAlignmentEnum, HorizontalAlignmentEnum
 )
 from .constants import (
     PAC_BYTES_TO_POSITIONING_MAP, COMMANDS, PAC_TAB_OFFSET_COMMANDS,
-    MICROSECONDS_PER_CODEWORD, UNHANDLED_COMMANDS,
-    INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION
+    MICROSECONDS_PER_CODEWORD, INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION
 )
 
 PopOnCue = collections.namedtuple("PopOnCue", "buffer, start, end")
 
 
 class PreCaption:
     """
@@ -339,17 +338,18 @@
         """Given a command determines whether to turn italics on or off,
         or to set the positioning
 
         This is mostly used to convert from the legacy-style commands
 
         :type command: str
         """
-        if command not in UNHANDLED_COMMANDS:
-            self._update_positioning(command)
+        self._update_positioning(command)
+
         text = COMMANDS.get(command, '')
+
         if 'italic' in text:
             if 'end' not in text:
                 self._collection.append(
                     _InstructionNode.create_italics_style(
                         self._position_tracer.get_current_position())
                 )
             else:
```

### Comparing `pycaption-2.2.5/pycaption/scc/state_machines.py` & `pycaption-2.2.6/pycaption/scc/state_machines.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/scc/translator.py` & `pycaption-2.2.6/pycaption/scc/translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/srt.py` & `pycaption-2.2.6/pycaption/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/transcript.py` & `pycaption-2.2.6/pycaption/transcript.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption/webvtt.py` & `pycaption-2.2.6/pycaption/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/pycaption.egg-info/PKG-INFO` & `pycaption-2.2.6/pycaption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.5
+Version: 2.2.6
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.5/pycaption.egg-info/SOURCES.txt` & `pycaption-2.2.6/pycaption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/setup.py` & `pycaption-2.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 transcript_dependencies = [
     'nltk'
 ]
 
 setup(
     name='pycaption',
-    version='2.2.5',
+    version='2.2.6',
     description='Closed caption converter',
     long_description=open(README_PATH).read(),
     author='Joe Norton',
     author_email='joey@nortoncrew.com',
     project_urls={
         'Source': 'https://github.com/pbs/pycaption',
         'Documentation': 'https://pycaption.readthedocs.io/',
```

### Comparing `pycaption-2.2.5/tests/conftest.py` & `pycaption-2.2.6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,14 @@
     sample_scc_empty, sample_scc_roll_up_ru2, sample_no_positioning_at_all_scc,
     sample_scc_no_explicit_end_to_last_caption, sample_scc_flashing_cue,
     sample_scc_eoc_first_command, sample_scc_with_extended_characters,
     sample_scc_with_ampersand_character, sample_scc_multiple_formats,
     sample_scc_duplicate_tab_offset, sample_scc_duplicate_special_characters,
     sample_scc_tab_offset, sample_scc_with_unknown_commands,
     sample_scc_special_and_extended_characters,
-    sample_scc_with_consecutive_pac_commands,
-    sample_scc_special_and_extended_characters,
     sample_scc_with_line_too_long
 )
 from tests.fixtures.srt import (  # noqa: F401
     sample_srt, sample_srt_ascii, sample_srt_numeric, sample_srt_empty,
     sample_srt_blank_lines, sample_srt_trailing_blanks,
     samples_srt_same_time, sample_srt_empty_cue_output,
     sample_srt_timestamps_without_microseconds,
```

### Comparing `pycaption-2.2.5/tests/fixtures/dfxp.py` & `pycaption-2.2.6/tests/fixtures/dfxp.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,18 +916,18 @@
    <region tts:displayAlign="before" tts:origin="40% 5%" tts:textAlign="left" xml:id="r1"/>
    <region tts:displayAlign="before" tts:origin="70% 23%" tts:textAlign="left" xml:id="r2"/>
    <region tts:displayAlign="before" tts:origin="20% 47%" tts:textAlign="left" xml:id="r3"/>
    <region tts:displayAlign="before" tts:origin="20% 89%" tts:textAlign="left" xml:id="r4"/>
    <region tts:displayAlign="before" tts:origin="40% 53%" tts:textAlign="left" xml:id="r5"/>
    <region tts:displayAlign="before" tts:origin="70% 17%" tts:textAlign="left" xml:id="r6"/>
    <region tts:displayAlign="before" tts:origin="20% 35%" tts:textAlign="left" xml:id="r7"/>
-   <region tts:displayAlign="before" tts:origin="25% 83%" tts:textAlign="left" xml:id="r8"/>
+   <region tts:displayAlign="before" tts:origin="20% 83%" tts:textAlign="left" xml:id="r8"/>
    <region tts:displayAlign="before" tts:origin="70% 11%" tts:textAlign="left" xml:id="r9"/>
    <region tts:displayAlign="before" tts:origin="40% 41%" tts:textAlign="left" xml:id="r10"/>
-   <region tts:displayAlign="before" tts:origin="25% 71%" tts:textAlign="left" xml:id="r11"/>
+   <region tts:displayAlign="before" tts:origin="20% 71%" tts:textAlign="left" xml:id="r11"/>
   </layout>
  </head>
  <body>
   <div region="bottom" xml:lang="en-US">
    <p begin="00:00:01.134" end="00:00:03.136" region="r0" style="default">
     abab
    </p>
```

### Comparing `pycaption-2.2.5/tests/fixtures/microdvd.py` & `pycaption-2.2.6/tests/fixtures/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/fixtures/sami.py` & `pycaption-2.2.6/tests/fixtures/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/fixtures/scc.py` & `pycaption-2.2.6/tests/fixtures/scc.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,41 +21,14 @@
 00:01:55;22 9420 942f 6162 e364 94f4 8080 6162 e364
 
 00:01:59;14 9420 942f 94ae
 """
 
 
 @pytest.fixture(scope="session")
-def sample_scc_with_consecutive_pac_commands():
-    return """\
-Scenarist_SCC V1.0
-
-00:00:00;15	942c
-
-00:11:45;10	9420 94d0 94ce 5b20 cec1 5252 c154 4f52 205d 9470 946e cd4f cecb 45d9 d320 4c4f d645 2054 c849 cec7 d320 54c8 c154 2046 4cd9 ae80 942c 8080 8080 942f
-
-00:11:47;28	9420 9454 9723 d9c1 d9a1 94f4 9723 5b20 c84f 4f54 49ce c720 5d80 942c 8080 8080 942f
-
-00:11:50;08	9420 94d0 94ce 45d3 d045 4349 c14c 4cd9 2049 4620 54c8 45d9 a752 4520 54c8 4520 4fce 45d3 9470 946e 57c8 4f20 c745 5420 544f 2046 4cd9 2054 c845 cdae 942c 8080 8080 942f
-
-00:11:54;06	942c
-
-00:23:00;13	9420 1370 136e 5b20 43c8 494c c420 5d80 94d0 94ce c745 4f52 c745 20cd c1c4 4520 c120 cdc1 43c8 49ce 4580 9470 946e 464f 5220 c84f 5749 4520 544f 942c 8080 8080 942f
-
-00:23:02;04	9420 91d0 91ce 544f 2046 49ce c420 43d5 5249 4fd5 d320 c745 4f52 c745 9170 916e c1ce c420 c849 d320 4652 4945 cec4 d380 92d0 92ce 45d6 4552 d920 c4c1 d920 4fce 4c49 ce45 2c80 942c 8080 8080 942f
-
-00:23:05;00	9420 9152 91ae d357 49ce c720 c2d9 20d0 c2d3 cb49 c4d3 ae4f 52c7 9170 916e 544f 20d0 4cc1 d920 46d5 ce20 c7c1 cd45 d320 c1ce c420 57c1 5443 c880 92d0 9723 91ae d94f d552 2046 c1d6 4f52 4954 4520 d649 c445 4fd3 ae80 942c 8080 8080 942f
-
-
-00:23:05;00	9420 9152 91ae d357 49ce c720 c2d9 20d0 c2d3 cb49 c4d3 ae4f 52c7 9170 916e 544f 20d0 4cc1 d920 46d5 ce20 c7c1 cd45 d320 c1ce c420 57c1 5443 c880 92d0 9723 91ae d94f d552 2046 c1d6 4f52 4954 4520 d649 c445 4fd3 ae80 942c 8080 8080 942f
-
-"""
-
-
-@pytest.fixture(scope="session")
 def scc_that_generates_webvtt_with_proper_newlines():
     return """\
 Scenarist_SCC V1.0
 
 00:21:29;23    9420 9452 6161 94f4 97a2 6262 942c 942f
 """
 
@@ -458,15 +431,15 @@
 @pytest.fixture(scope="session")
 def sample_scc_with_line_too_long():
     return """\
 Scenarist_SCC V1.0
 
 00:00:00;03	942c
 
-00:00:01;45	9420 91f4 cb45 4c4c d920 4ac1 cd45 d3ba 20c8 eff7 9254 f468 e520 7368 eff7d3ba 20c8 eff7 9254 f468 e520 7368 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 eff7 2073 f461 f2f4 e564 942c 8080 8080 942f
+00:00:01;45	9420 91f4 cb45 4c4c d920 4ac1 cd45 d3ba 20c8 eff7 9254 f468 e520 7368 eff7 2073 f461 f2f4 e564 942c 8080 8080 942f
 
 00:00:02;55	9420 91e0 9723 f761 7320 4361 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 ec20 c4e5 6ee9 73ef 6e2c 2061 20e6 f2e9 e56e 6480 9240 9723 efe6 20ef 75f2 732c 20f7 6173 2064 efe9 6e67 206d 7920 43c4 73ae 942c 8080 8080 942f
 
 00:00:06;57	9420 94e0 c16e 6420 68e5 2073 61e9 642c 2049 20e3 616e 2064 ef20 6120 54d6 2073 68ef f7ae 942c 8080 8080 942f
 
 00:00:08;58	9420 9452 4920 ea75 73f4 20f7 616e f4e5 6420 ef6e e520 7368 eff7 2c80 94f2 ea75 73f4 20f4 ef20 6861 76e5 2061 7320 6120 ece9 f4f4 ece5 942c 8080 8080 942f
 """
```

### Comparing `pycaption-2.2.5/tests/fixtures/srt.py` & `pycaption-2.2.6/tests/fixtures/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/fixtures/translated_scc.py` & `pycaption-2.2.6/tests/fixtures/translated_scc.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/fixtures/webvtt.py` & `pycaption-2.2.6/tests/fixtures/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/mixins.py` & `pycaption-2.2.6/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_base.py` & `pycaption-2.2.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_dfxp.py` & `pycaption-2.2.6/tests/test_dfxp.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_dfxp_conversion.py` & `pycaption-2.2.6/tests/test_dfxp_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_dfxp_extras.py` & `pycaption-2.2.6/tests/test_dfxp_extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_functions.py` & `pycaption-2.2.6/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_geometry.py` & `pycaption-2.2.6/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_microdvd.py` & `pycaption-2.2.6/tests/test_microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_microdvd_conversion.py` & `pycaption-2.2.6/tests/test_microdvd_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_sami.py` & `pycaption-2.2.6/tests/test_sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_sami_conversion.py` & `pycaption-2.2.6/tests/test_sami_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_scc.py` & `pycaption-2.2.6/tests/test_scc.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,18 +73,18 @@
             ((40.0, UnitEnum.PERCENT), (5.0, UnitEnum.PERCENT)),
             ((70.0, UnitEnum.PERCENT), (23.0, UnitEnum.PERCENT)),
             ((20.0, UnitEnum.PERCENT), (47.0, UnitEnum.PERCENT)),
             ((20.0, UnitEnum.PERCENT), (89.0, UnitEnum.PERCENT)),
             ((40.0, UnitEnum.PERCENT), (53.0, UnitEnum.PERCENT)),
             ((70.0, UnitEnum.PERCENT), (17.0, UnitEnum.PERCENT)),
             ((20.0, UnitEnum.PERCENT), (35.0, UnitEnum.PERCENT)),
-            ((25.0, UnitEnum.PERCENT), (83.0, UnitEnum.PERCENT)),
+            ((20.0, UnitEnum.PERCENT), (83.0, UnitEnum.PERCENT)),
             ((70.0, UnitEnum.PERCENT), (11.0, UnitEnum.PERCENT)),
             ((40.0, UnitEnum.PERCENT), (41.0, UnitEnum.PERCENT)),
-            ((25.0, UnitEnum.PERCENT), (71.0, UnitEnum.PERCENT))
+            ((20.0, UnitEnum.PERCENT), (71.0, UnitEnum.PERCENT))
         ]
 
         actual_positioning = [
             caption_.layout_info.origin.serialized()
             for caption_ in captions.get_captions('en-US')
         ]
 
@@ -240,54 +240,23 @@
     def test_flashing_cue(self, sample_scc_flashing_cue):
         with pytest.raises(CaptionReadTimingError) as exc_info:
             SCCReader().read(sample_scc_flashing_cue)
 
         assert exc_info.value.args[0].startswith(
             "Unsupported cue duration around 00:00:20.433")
 
-    def test_skip_first_pac_command(self, sample_scc_with_consecutive_pac_commands):
-        caption_set = SCCReader().read(sample_scc_with_consecutive_pac_commands)
-        caption = caption_set.get_captions('en-US')
-        actual_lines = [
-            node.content
-            for cap_ in caption
-            for node in cap_.nodes
-            if node.type_ == CaptionNode.TEXT
-        ]
-        expected_lines = [
-            '[ NARRATOR ]',
-             'MONKEYS LOVE THINGS THAT FLY.',
-             'YAY!',
-             '[ HOOTING ]',
-             "ESPECIALLY IF THEY'RE THE ONES",
-             'WHO GET TO FLY THEM.',
-             '[ CHILD ]',
-             'GEORGE MADE A MACHINE',
-             'FOR HOWIE TO',
-             'TO FIND CURIOUS GEORGE',
-             'AND HIS FRIENDS',
-             'EVERY DAY ONLINE,',
-             'SWING BY PBSKIDS.ORG',
-             'TO PLAY FUN GAMES AND WATCH',
-             'YOUR FAVORITE VIDEOS.',
-             'SWING BY PBSKIDS.ORG',
-             'TO PLAY FUN GAMES AND WATCH',
-             'YOUR FAVORITE VIDEOS.'
-        ]
-        # is not breaking the lines
-        assert expected_lines == actual_lines
-
     def test_line_too_long(self, sample_scc_with_line_too_long):
         with pytest.raises(CaptionLineLengthError) as exc_info:
             SCCReader().read(sample_scc_with_line_too_long)
 
         assert exc_info.value.args[0].startswith(
             "32 character limit for caption cue in scc file.")
-        assert ("was Cal l l l l l l l l l l l l l l l l l l l l l l l l l l l l Denison, a friend - Length 81"
-                in exc_info.value.args[0].split("\n"))
+        str_to_check = ("around 00:00:05.900 - was Cal l l l l l l l l l l l l l l l l l l l l l l l l l l l l "
+                        "Denison, a friend - Length 81")
+        assert str_to_check in exc_info.value.args[0].split("\n")
 
 
 class TestCoverageOnly:
     """In order to refactor safely, we need coverage of 95% or more.
      This class includes tests that ensure that at the very least, we don't
      break anything that was working, OR fix anything whose faulty behavior
       was accepted.
@@ -373,14 +342,15 @@
             (21800000.0, 34900000.0),
             (34900000.0, 36400000.0),
             (36400000.0, 44266666.666666664),
             (44266666.666666664, 44866666.666666664),
         ]
 
         actual_timings = [(c_.start, c_.end) for c_ in captions]
+
         assert expected_timings == actual_timings
 
     def test_freeze_colon_spec_time(self, sample_scc_pop_on):
         # Coverage doesn't mean we test that functionality, so assert that
         # all the timing specs that previously had coverage, will actually
         # remain unchanged.
         scc1 = SCCReader().read(sample_scc_pop_on)
@@ -611,8 +581,8 @@
         # TODO First caption should be ignored because it doesn't start with
         #  a pop/roll/paint on command
         caption_set = SCCReader().read(sample_scc_eoc_first_command)
 
         # just one caption, first EOC disappears
         num_captions = len(caption_set.get_captions('en-US'))
 
-        assert num_captions == 1
+        assert num_captions == 2
```

### Comparing `pycaption-2.2.5/tests/test_scc_conversion.py` & `pycaption-2.2.6/tests/test_scc_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_scc_translator.py` & `pycaption-2.2.6/tests/test_scc_translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_srt.py` & `pycaption-2.2.6/tests/test_srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_srt_conversion.py` & `pycaption-2.2.6/tests/test_srt_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_webvtt.py` & `pycaption-2.2.6/tests/test_webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.5/tests/test_webvtt_conversion.py` & `pycaption-2.2.6/tests/test_webvtt_conversion.py`

 * *Files identical despite different names*

