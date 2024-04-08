# Comparing `tmp/pyvene-0.1.0.tar.gz` & `tmp/pyvene-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvene-0.1.0.tar", last modified: Fri Apr  5 00:18:40 2024, max compression
+gzip compressed data, was "pyvene-0.1.1.tar", last modified: Mon Apr  8 22:27:57 2024, max compression
```

## Comparing `pyvene-0.1.0.tar` & `pyvene-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 00:18:36.000000 pyvene-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:18:36.000000 pyvene-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-05 00:18:40.549513 pyvene-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-05 00:18:36.000000 pyvene-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/data_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/data_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16588 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/data_generators/causal_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.545513 pyvene-0.1.0/pyvene/models/backpack_gpt2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/backpack_gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/basic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/blip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_blip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/configuration_intervenable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt2/modelings_intervenable_gpt2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gpt_neo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gpt_neox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/gru/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gru/modelings_gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/gru/modelings_intervenable_gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    74237 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/intervenable_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/intervenable_modelcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/intervention_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/interventions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/llama/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/llama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/llama/modelings_intervenable_llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mistral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mistral/modellings_intervenable_mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene/models/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mlp/modelings_intervenable_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/mlp/modelings_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-05 00:18:36.000000 pyvene-0.1.0/pyvene/models/modeling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:18:40.549513 pyvene-0.1.0/pyvene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 00:18:40.000000 pyvene-0.1.0/pyvene.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-04-05 00:18:36.000000 pyvene-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:18:40.553513 pyvene-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-05 00:18:36.000000 pyvene-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.315974 pyvene-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 22:27:53.000000 pyvene-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 22:27:53.000000 pyvene-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-08 22:27:57.311974 pyvene-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-08 22:27:53.000000 pyvene-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.307974 pyvene-0.1.1/pyvene/
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.307974 pyvene-0.1.1/pyvene/data_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/data_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16588 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/data_generators/causal_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.307974 pyvene-0.1.1/pyvene/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.307974 pyvene-0.1.1/pyvene/models/backpack_gpt2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/backpack_gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/basic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/blip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/blip/modelings_blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/blip/modelings_blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/blip/modelings_intervenable_blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/blip/modelings_intervenable_blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/configuration_intervenable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gpt2/modelings_intervenable_gpt2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/gpt_neo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gpt_neo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/gpt_neox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gpt_neox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/gru/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gru/modelings_gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/gru/modelings_intervenable_gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74237 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/intervenable_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/intervenable_modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/intervention_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/interventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/llama/modelings_intervenable_llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/mistral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/mistral/modellings_intervenable_mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene/models/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/mlp/modelings_intervenable_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/mlp/modelings_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-08 22:27:53.000000 pyvene-0.1.1/pyvene/models/modeling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:27:57.311974 pyvene-0.1.1/pyvene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-08 22:27:57.000000 pyvene-0.1.1/pyvene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-08 22:27:57.000000 pyvene-0.1.1/pyvene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:27:57.000000 pyvene-0.1.1/pyvene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 22:27:57.000000 pyvene-0.1.1/pyvene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 22:27:57.000000 pyvene-0.1.1/pyvene.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      217 2024-04-08 22:27:53.000000 pyvene-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:27:57.315974 pyvene-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-08 22:27:53.000000 pyvene-0.1.1/setup.py
```

### Comparing `pyvene-0.1.0/LICENSE` & `pyvene-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/PKG-INFO` & `pyvene-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvene
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use Activation Intervention to Interpret Causal Mechanism of Model
 Home-page: https://github.com/stanfordnlp/pyvene
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: transformers>=4.38.1
 Requires-Dist: datasets>=2.16.1
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: matplotlib>=3.7.4
-Requires-Dist: seaborn>=0.13.1
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub==0.20.3
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: fsspec>=2023.6.0
 Requires-Dist: accelerate>=0.26.1
 Requires-Dist: sentencepiece>=0.1.96
```

### Comparing `pyvene-0.1.0/README.md` & `pyvene-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/__init__.py` & `pyvene-0.1.1/pyvene/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/data_generators/causal_model.py` & `pyvene-0.1.1/pyvene/data_generators/causal_model.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py` & `pyvene-0.1.1/pyvene/models/backpack_gpt2/modelings_backpack_gpt2.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py` & `pyvene-0.1.1/pyvene/models/backpack_gpt2/modelings_intervenable_backpack_gpt2.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/basic_utils.py` & `pyvene-0.1.1/pyvene/models/basic_utils.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/blip/modelings_blip.py` & `pyvene-0.1.1/pyvene/models/blip/modelings_blip.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/blip/modelings_blip_itm.py` & `pyvene-0.1.1/pyvene/models/blip/modelings_blip_itm.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip.py` & `pyvene-0.1.1/pyvene/models/blip/modelings_intervenable_blip.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/blip/modelings_intervenable_blip_itm.py` & `pyvene-0.1.1/pyvene/models/blip/modelings_intervenable_blip_itm.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/configuration_intervenable_model.py` & `pyvene-0.1.1/pyvene/models/configuration_intervenable_model.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/constants.py` & `pyvene-0.1.1/pyvene/models/constants.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/gpt2/modelings_intervenable_gpt2.py` & `pyvene-0.1.1/pyvene/models/gpt2/modelings_intervenable_gpt2.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py` & `pyvene-0.1.1/pyvene/models/gpt_neo/modelings_intervenable_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py` & `pyvene-0.1.1/pyvene/models/gpt_neox/modelings_intervenable_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/gru/modelings_gru.py` & `pyvene-0.1.1/pyvene/models/gru/modelings_gru.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/gru/modelings_intervenable_gru.py` & `pyvene-0.1.1/pyvene/models/gru/modelings_intervenable_gru.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/intervenable_base.py` & `pyvene-0.1.1/pyvene/models/intervenable_base.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/intervenable_modelcard.py` & `pyvene-0.1.1/pyvene/models/intervenable_modelcard.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/intervention_utils.py` & `pyvene-0.1.1/pyvene/models/intervention_utils.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/interventions.py` & `pyvene-0.1.1/pyvene/models/interventions.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/layers.py` & `pyvene-0.1.1/pyvene/models/layers.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/llama/modelings_intervenable_llama.py` & `pyvene-0.1.1/pyvene/models/llama/modelings_intervenable_llama.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/mistral/modellings_intervenable_mistral.py` & `pyvene-0.1.1/pyvene/models/mistral/modellings_intervenable_mistral.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/mlp/modelings_intervenable_mlp.py` & `pyvene-0.1.1/pyvene/models/mlp/modelings_intervenable_mlp.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/mlp/modelings_mlp.py` & `pyvene-0.1.1/pyvene/models/mlp/modelings_mlp.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene/models/modeling_utils.py` & `pyvene-0.1.1/pyvene/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/pyvene.egg-info/PKG-INFO` & `pyvene-0.1.1/pyvene.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvene
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use Activation Intervention to Interpret Causal Mechanism of Model
 Home-page: https://github.com/stanfordnlp/pyvene
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: transformers>=4.38.1
 Requires-Dist: datasets>=2.16.1
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: matplotlib>=3.7.4
-Requires-Dist: seaborn>=0.13.1
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub==0.20.3
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: fsspec>=2023.6.0
 Requires-Dist: accelerate>=0.26.1
 Requires-Dist: sentencepiece>=0.1.96
```

### Comparing `pyvene-0.1.0/pyvene.egg-info/SOURCES.txt` & `pyvene-0.1.1/pyvene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvene-0.1.0/setup.py` & `pyvene-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyvene",
-    version="0.1.0",
+    version="0.1.1",
     description="Use Activation Intervention to Interpret Causal Mechanism of Model",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/stanfordnlp/pyvene",
     author="Zhengxuan Wu",
     author_email="wuzhengx@stanford.edu",
     license="Apache License 2.0",
```

