# Comparing `tmp/fedpredict-0.0.4.4.tar.gz` & `tmp/fedpredict-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedpredict-0.0.4.4.tar", last modified: Thu Feb 15 21:55:56 2024, max compression
+gzip compressed data, was "fedpredict-0.0.7.tar", last modified: Mon Apr  8 23:20:16 2024, max compression
```

## Comparing `fedpredict-0.0.4.4.tar` & `fedpredict-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:55:56.036399 fedpredict-0.0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-15 21:55:56.036399 fedpredict-0.0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:55:56.032399 fedpredict-0.0.4.4/fedpredict/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41973 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/fedpredict.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/test_fedpredict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:55:56.036399 fedpredict-0.0.4.4/fedpredict/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:55:56.036399 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/fedkd.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/fedpsarsification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/parameters_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/compression_methods/sparsification.py
--rw-r--r--   0 runner    (1001) docker     (127)    34698 2024-02-15 21:55:53.000000 fedpredict-0.0.4.4/fedpredict/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:55:56.036399 fedpredict-0.0.4.4/fedpredict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-15 21:55:55.000000 fedpredict-0.0.4.4/fedpredict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-15 21:55:55.000000 fedpredict-0.0.4.4/fedpredict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 21:55:55.000000 fedpredict-0.0.4.4/fedpredict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-15 21:55:55.000000 fedpredict-0.0.4.4/fedpredict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 21:55:56.036399 fedpredict-0.0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-15 21:55:55.000000 fedpredict-0.0.4.4/setup.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-08 23:20:16.853944 fedpredict-0.0.7/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1519 2024-02-23 16:53:31.000000 fedpredict-0.0.7/LICENSE
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     5623 2024-04-08 23:20:16.853944 fedpredict-0.0.7/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4632 2024-03-15 14:46:59.000000 fedpredict-0.0.7/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-08 23:20:16.849944 fedpredict-0.0.7/fedpredict/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      761 2024-03-14 20:01:23.000000 fedpredict-0.0.7/fedpredict/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4229 2024-03-10 16:55:29.000000 fedpredict-0.0.7/fedpredict/fedpredict.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    43298 2024-03-10 18:30:58.000000 fedpredict-0.0.7/fedpredict/fedpredict_core.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    17513 2024-03-17 23:49:58.000000 fedpredict-0.0.7/fedpredict/fedpredict_torch.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-08 23:20:16.853944 fedpredict-0.0.7/fedpredict/utils/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2024-02-23 16:53:31.000000 fedpredict-0.0.7/fedpredict/utils/__init__.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-08 23:20:16.853944 fedpredict-0.0.7/fedpredict/utils/compression_methods/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      458 2024-02-29 21:14:11.000000 fedpredict-0.0.7/fedpredict/utils/compression_methods/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3257 2024-02-29 20:29:40.000000 fedpredict-0.0.7/fedpredict/utils/compression_methods/fedkd.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      599 2024-02-23 16:53:31.000000 fedpredict-0.0.7/fedpredict/utils/compression_methods/fedpsarsification.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6369 2024-02-23 16:53:31.000000 fedpredict-0.0.7/fedpredict/utils/compression_methods/parameters_svd.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6076 2024-02-29 20:23:10.000000 fedpredict-0.0.7/fedpredict/utils/compression_methods/quantization.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    15775 2024-02-23 16:53:31.000000 fedpredict-0.0.7/fedpredict/utils/compression_methods/sparsification.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    34669 2024-02-29 20:31:34.000000 fedpredict-0.0.7/fedpredict/utils/utils.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-08 23:20:16.853944 fedpredict-0.0.7/fedpredict.egg-info/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     5623 2024-04-08 23:20:16.000000 fedpredict-0.0.7/fedpredict.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      690 2024-04-08 23:20:16.000000 fedpredict-0.0.7/fedpredict.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2024-04-08 23:20:16.000000 fedpredict-0.0.7/fedpredict.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      138 2024-04-08 23:20:16.000000 fedpredict-0.0.7/fedpredict.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       11 2024-04-08 23:20:16.000000 fedpredict-0.0.7/fedpredict.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1014 2024-03-01 19:02:05.000000 fedpredict-0.0.7/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       38 2024-04-08 23:20:16.853944 fedpredict-0.0.7/setup.cfg
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       69 2024-03-01 13:54:09.000000 fedpredict-0.0.7/setup.py
```

### Comparing `fedpredict-0.0.4.4/fedpredict/fedpredict.py` & `fedpredict-0.0.7/fedpredict/fedpredict_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import sys
 import copy
 import numpy as np
-from utils.compression_methods.parameters_svd import parameter_svd_write, inverse_parameter_svd_reading, if_reduces_size
-from utils.compression_methods.sparsification import sparse_crs_top_k, to_dense, sparse_matrix, get_not_zero_values
-from utils.compression_methods.fedkd import fedkd_compression
+from .utils.compression_methods.parameters_svd import parameter_svd_write, inverse_parameter_svd_reading, if_reduces_size
+from .utils.compression_methods.sparsification import sparse_crs_top_k, to_dense, sparse_matrix, get_not_zero_values
+from .utils.compression_methods.fedkd import fedkd_compression
 import os
 
 import math
-import torch
-
-from flwr.common import (
-    EvaluateIns,
-    EvaluateRes,
-    FitIns,
-    FitRes,
-    MetricsAggregationFn,
-    NDArrays,
-    Parameters,
-    Scalar,
-    ndarrays_to_parameters,
-    parameters_to_ndarrays,
-)
 
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 
+try:
+    import flwr
+    from flwr.common import (
+        EvaluateIns,
+        ndarrays_to_parameters,
+    )
+except ImportError:
+    _has_flwr = False
+else:
+    _has_flwr = True
+
 NDArray = npt.NDArray[Any]
 NDArrayInt = npt.NDArray[np.int_]
 NDArrayFloat = npt.NDArray[np.float_]
 NDArrays = List[NDArray]
 
 
 class CKA(object):
@@ -72,61 +69,401 @@
     def kernel_CKA(self, X, Y, sigma=None):
         hsic = self.kernel_HSIC(X, Y, sigma)
         var1 = np.sqrt(self.kernel_HSIC(X, X, sigma))
         var2 = np.sqrt(self.kernel_HSIC(Y, Y, sigma))
 
         return hsic / (var1 * var2)
 
+# ===========================================================================================
+
+# FedPredict server
+
+def get_size(parameter):
+    try:
+        return parameter.nbytes
+    except Exception as e:
+        print("get_size")
+        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
+
+
+def fedpredict_server(parameters: np.array, client_evaluate_list: List[Tuple], fedpredict_clients_metrics: Dict,
+                      server_round: int, num_rounds: int, model_shape: List, compression_method=None,
+                      df: float=0, fl_framework=None):
+    """
+
+    Args:
+        parameters: list[np.array], required
+            List of numpy arrays
+        client_evaluate_list: list[tuple], required
+            List of clients' tuples
+        fedpredict_clients_metrics: dict, required
+            Dict of clients' metrics.
+        server_round: int, required
+        num_rounds: int, required
+        df: float, optional. Default=0
+            Layers' similarity difference. It is used when compression_method uses the "dls" technique.
+        model_shape: list, optional
+        compression_method: None, 'dls_compredict', 'dls', 'compredict', 'sparsification', 'fedkd', 'fedper'. Default=None
+        fl_framework: None, 'flwr'. Default='flwr'
+            Method for compressing the global model parameters before sending to thee clients
+
+    Returns: list[tuple]
+
+    """
+    try:
+
+        client_evaluate_list_fedpredict = []
+        accuracy = 0
+        size_of_parameters = []
+
+        # Reuse previously compressed parameters
+        previously_reduced_parameters = {}
+        print("compression technique: ", compression_method)
+        if compression_method in ["fedkd", "compredict", "dls_compredict"]:
+            layers_compression_range = layer_compression_range(model_shape)
+        fedkd = None
+        for client_tuple in client_evaluate_list:
+            client = client_tuple[0]
+            client_id = str(client.cid)
+            config = copy.copy(client_tuple[1].config)
+            client_config = fedpredict_clients_metrics[str(client.cid)]
+            nt = client_config['nt']
+            if nt != 0 and nt in previously_reduced_parameters:
+                process_parameters = False
+            else:
+                process_parameters = True
+
+            if compression_method is None:
+                process_parameters = True
+            config['nt'] = nt
+            config['metrics'] = client_config
+            config['last_global_accuracy'] = accuracy
+            config['total_server_rounds'] = num_rounds
+            M = [i for i in range(len(parameters))]
+            parameters_to_send = None
+            if nt == 0 and compression_method not in ["fedkd", None]:
+                config['M'] = []
+                config['decompress'] = False
+                config['layers_fraction'] = 0
+                if fl_framework is None:
+                    config['parameters'] = np.array([])
+                    client_evaluate_list_fedpredict.append((client, config))
+                elif fl_framework == 'flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(np.array([])), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
+                continue
+            elif compression_method == 'fedkd':
+                if fedkd is None:
+                    parameters_to_send = parameters_to_send if parameters_to_send is not None else parameters
+                    print("dentro 1: ", type(parameters_to_send[0]), len(parameters_to_send[0]))
+                    parameters_to_send, layers_fraction = fedkd_compression(
+                        fedpredict_clients_metrics[str(client_id)]['round_of_last_fit'], layers_compression_range,
+                        num_rounds, client_id, server_round, len(M), parameters_to_send)
+                    fedkd = parameters_to_send
+                else:
+                    parameters_to_send = fedkd
+                config['decompress'] = True
+                config['M'] = M
+                config['layers_fraction'] = layers_fraction
+                if fl_framework is None:
+                    config['parameters'] = parameters_to_send
+                    client_evaluate_list_fedpredict.append((client, config))
+                elif fl_framework =='flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
+                continue
+            elif compression_method == 'sparsification':
+                k = 0.3
+
+                t, k_values = sparse_crs_top_k([np.abs(i) for i in parameters], k)
+                parameters_to_send = t
+                # print("contar2")
+                # print([len(i[i == 0]) for i in parameters_to_send])
+                config['decompress'] = False
+                config['M'] = M
+                config['layers_fraction'] = 1
+                if fl_framework is None:
+                    config['parameters'] = parameters_to_send
+                    client_evaluate_list_fedpredict.append((client, config))
+                elif fl_framework == 'flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
+                continue
+
+            elif compression_method is None:
+                config['M'] = [i for i in range(len(parameters))]
+                config['decompress'] = False
+                config['layers_fraction'] = 1
+                if fl_framework is None:
+                    config['parameters'] = parameters
+                    client_evaluate_list_fedpredict.append((client, config))
+                elif fl_framework == 'flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
+                continue
+
+            parameters_to_send = None
+
+            print("Tamanho parametros antes: ", sum([i.nbytes for i in parameters]))
+
+            if process_parameters:
+                if "dls" in compression_method:
+                    parameters_to_send, M = dls(fedpredict_clients_metrics[client_id]['first_round'],
+                                                parameters, server_round, nt, num_rounds, df, size_of_parameters)
+                    print("Tamanho parametros als: ", sum(i.nbytes for i in parameters_to_send))
+                elif "per" in compression_method:
+                    parameters_to_send, M = per(fedpredict_clients_metrics[client_id]['first_round'],
+                                                parameters)
+                    print("Tamanho parametros per: ", sum(i.nbytes for i in parameters_to_send),
+                          len(parameters_to_send), len(M))
+                layers_fraction = []
+                if 'compredict' in compression_method:
+                    parameters_to_send = parameters_to_send if parameters_to_send is not None else parameters
+                    parameters_to_send, layers_fraction = compredict(
+                        fedpredict_clients_metrics[str(client_id)]['round_of_last_fit'], layers_compression_range,
+                        num_rounds, server_round, len(M), parameters_to_send)
+                    config['decompress'] = True
+                    pass
+                else:
+                    config['decompress'] = False
+                    print("nao igual")
+                # config['decompress'] = False
+                print("Novos parametros para nt: ", nt)
+                decompress = config['decompress']
+                previously_reduced_parameters[nt] = [copy.deepcopy(parameters_to_send), M, layers_fraction, decompress]
+
+            else:
+                print("Reutilizou parametros de nt: ", nt)
+                parameters_to_send, M, layers_fraction, decompress = previously_reduced_parameters[nt]
+
+            parameters_to_send = [np.array(i) for i in parameters_to_send]
+            print("Tamanho parametros compredict: ", sum(i.nbytes for i in parameters_to_send))
+            for i in range(1, len(parameters)):
+                size_of_parameters.append(get_size(parameters[i]))
+            fedpredict_clients_metrics[str(client.cid)]['acc_bytes_rate'] = size_of_parameters
+            config['M'] = M
+            config['decompress'] = decompress
+            config['layers_fraction'] = layers_fraction
+            if fl_framework is None:
+                config['parameters'] = parameters_to_send
+                client_evaluate_list_fedpredict.append((client, config))
+            elif fl_framework == 'flwr':
+                if _has_flwr:
+                    evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
+                    client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                else:
+                    raise ImportError("Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
+
+        return client_evaluate_list_fedpredict
+
+    except Exception as e:
+        print("fedpredict server")
+        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
+
+
+def compredict(round_of_last_fit, layers_comppression_range, num_rounds, server_round, M, parameter):
+
+    try:
+
+        nt = server_round - round_of_last_fit
+        layers_fraction = []
+        if round_of_last_fit >= 1:
+            n_components_list = []
+            for i in range(M):
+                # if i % 2 == 0:
+                layer = parameter[i]
+                if len(layer.shape) >= 2:
+
+                    compression_range = layers_comppression_range[i]
+                    if compression_range > 0:
+                        n_components = fedpredict_core_compredict(server_round, num_rounds, nt, layer,
+                                                                  compression_range)
+                    else:
+                        n_components = None
+                else:
+                    n_components = None
+
+                if n_components is None:
+                    layers_fraction.append(1)
+                else:
+                    layers_fraction.append(n_components / layer.shape[-1])
+
+                n_components_list.append(n_components)
+
+            print("Vetor de componentes: ", n_components_list)
+
+            parameter = parameter_svd_write(parameter, n_components_list)
+
+            # print("Client: ", client_id, " round: ", server_round, " nt: ", nt, " norm: ", np.mean(gradient_norm), " camadas: ", M, " todos: ", gradient_norm)
+            print("modelo compredict: ", [i.shape for i in parameter])
+
+        else:
+            new_parameter = []
+            for param in parameter:
+                new_parameter.append(param)
+                new_parameter.append(np.array([]))
+                new_parameter.append(np.array([]))
+
+            parameter = new_parameter
+
+            layers_fraction = [1] * len(parameter)
+
+        return parameter, layers_fraction
+
+    except Exception as e:
+        print("compredict")
+        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
+
+
+def layer_compression_range(model_shape):
+    try:
+
+        layers_range = []
+        for shape in model_shape:
+
+            layer_range = 0
+            if len(shape) >= 2:
+                shape = shape[-2:]
+
+                col = shape[1]
+                for n_components in range(1, col + 1):
+                    if if_reduces_size(shape, n_components):
+                        layer_range = n_components
+                    else:
+                        break
+
+            layers_range.append(layer_range)
+
+        return layers_range
+
+    except Exception as e:
+        print("layer compression range")
+        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
+
+
+def dls(first_round, parameters,
+        server_round, nt, num_rounds, df, size_of_layers):
+    try:
+        M = [i for i in range(len(parameters))]
+        n_layers = len(parameters) / 2
+
+        # return parameters, M
+
+        size_list = []
+        for i in range(len(parameters)):
+            tamanho = get_size(parameters[i])
+            size_list.append(tamanho)
+        if first_round != -1:
+            # baixo-cima
+            M = fedpredict_core_layer_selection(t=server_round, T=num_rounds, nt=nt, n_layers=n_layers,
+                                                size_per_layer=size_of_layers, df=df)
+            new_parameters = []
+            for i in range(len(parameters)):
+                if i in M:
+                    new_parameters.append(parameters[i])
+            parameters = new_parameters
+
+        size_list = []
+        for i in range(len(parameters)):
+            tamanho = parameters[i].nbytes
+            size_list.append(tamanho)
+
+        return parameters, M
+
+    except Exception as e:
+        print("dls")
+        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
+
+def per(first_round, parameters):
+    try:
+        M = [i for i in range(len(parameters))]
+        n_layers = len(parameters) / 2
+
+        size_list = []
+        for i in range(len(parameters)):
+            tamanho = get_size(parameters[i])
+            size_list.append(tamanho)
+        if first_round != -1:
+            # baixo-cima
+            M = [i for i in range(len(parameters))][:-2]
+            new_parameters = []
+            for i in range(len(parameters)):
+                if i in M:
+                    new_parameters.append(parameters[i])
+            parameters = new_parameters
+
+        size_list = []
+        for i in range(len(parameters)):
+            tamanho = parameters[i].nbytes
+            size_list.append(tamanho)
+
+        return parameters, M
+
+    except Exception as e:
+        print("per")
+        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
+
 
 def fedpredict_core(t, T, nt):
     try:
 
         # 9
         if nt == 0:
             global_model_weight = 0
         elif nt == t:
             global_model_weight = 1
         else:
             update_level = 1 / nt
             evolution_level = t / T
-            eq1 = (-update_level - evolution_level)  # v1 pior
+            eq1 = (-update_level - evolution_level)
             eq2 = round(np.exp(eq1), 6)
             global_model_weight = eq2
 
         local_model_weights = 1 - global_model_weight
 
-        print("rodada: ", t, " rounds sem fit: ", nt, "\npeso global: ", global_model_weight, " peso local: ",
-              local_model_weights)
+        # print("rodada: ", t, " rounds sem fit: ", nt, "\npeso global: ", global_model_weight, " peso local: ",
+        #       local_model_weights)
 
         return local_model_weights, global_model_weight
 
     except Exception as e:
         print("fedpredict core")
         print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
 
 
-def fedpredict_dynamic_core(t, T, nt, local_client_information, current_proportion):
+def fedpredict_dynamic_core(t, T, nt, similarity, fraction_of_classes):
     try:
-
-        # 9
-        similarity = local_client_information['similarity']
-        imbalance_level = local_client_information['imbalance_level']
-        fraction_of_classes = local_client_information['fraction_of_classes']
         print("fedpredict_dynamic_core rodada: ", t, "local classes: ", similarity)
         similarity = float(np.round(similarity, 1))
 
         if nt == 0:
             global_model_weight = 0
-        elif nt == t or (fraction_of_classes == 1 and imbalance_level <= 10):
+        elif nt == t or (fraction_of_classes == 1):
             global_model_weight = 1
         elif similarity != 1:
             global_model_weight = 1
         else:
             update_level = 1 / nt
-            evolution_level = t / int(100)
+            evolution_level = t / int(T)
             eq1 = (-update_level - evolution_level) * similarity
             eq2 = round(np.exp(eq1), 6)
             global_model_weight = eq2
             # global_model_weight = 0
 
         local_model_weights = 1 - global_model_weight
 
@@ -368,15 +705,15 @@
             Dict of clients' metrics.
         server_round: int, required
         num_rounds: int, required
         df: float, optional. Default=0
             Layers' similarity difference. It is used when compression_method uses the "dls" technique.
         model_shape: list, optional
         compression_method: None, 'dls_compredict', 'dls', 'compredict', 'sparsification', 'fedkd', 'fedper'. Default=None
-        fl_framework: None, 'flower'. Default='flower'
+        fl_framework: None, 'flwr'. Default='flwr'
             Method for compressing the global model parameters before sending to thee clients
 
     Returns: list[tuple]
 
     """
     try:
 
@@ -412,17 +749,21 @@
             if nt == 0 and compression_method not in ["fedkd", None]:
                 config['M'] = []
                 config['decompress'] = False
                 config['layers_fraction'] = 0
                 if fl_framework is None:
                     config['parameters'] = np.array([])
                     client_evaluate_list_fedpredict.append((client, config))
-                elif fl_framework == 'flower':
-                    evaluate_ins = EvaluateIns(ndarrays_to_parameters(np.array([])), config)
-                    client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                elif fl_framework == 'flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(np.array([])), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
                 continue
             elif compression_method == 'fedkd':
                 if fedkd is None:
                     parameters_to_send = parameters_to_send if parameters_to_send is not None else parameters
                     print("dentro 1: ", type(parameters_to_send[0]), len(parameters_to_send[0]))
                     parameters_to_send, layers_fraction = fedkd_compression(
                         fedpredict_clients_metrics[str(client_id)]['round_of_last_fit'], layers_compression_range,
@@ -432,46 +773,58 @@
                     parameters_to_send = fedkd
                 config['decompress'] = True
                 config['M'] = M
                 config['layers_fraction'] = layers_fraction
                 if fl_framework is None:
                     config['parameters'] = parameters_to_send
                     client_evaluate_list_fedpredict.append((client, config))
-                else:
-                    evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
-                    client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                elif fl_framework =='flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
                 continue
             elif compression_method == 'sparsification':
                 k = 0.3
 
                 t, k_values = sparse_crs_top_k([np.abs(i) for i in parameters], k)
                 parameters_to_send = t
                 # print("contar2")
                 # print([len(i[i == 0]) for i in parameters_to_send])
                 config['decompress'] = False
                 config['M'] = M
                 config['layers_fraction'] = 1
                 if fl_framework is None:
                     config['parameters'] = parameters_to_send
                     client_evaluate_list_fedpredict.append((client, config))
-                elif fl_framework == 'flower':
-                    evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
-                    client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                elif fl_framework == 'flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
                 continue
 
             elif compression_method is None:
                 config['M'] = [i for i in range(len(parameters))]
                 config['decompress'] = False
                 config['layers_fraction'] = 1
                 if fl_framework is None:
                     config['parameters'] = parameters
                     client_evaluate_list_fedpredict.append((client, config))
-                elif fl_framework == 'flower':
-                    evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters), config)
-                    client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                elif fl_framework == 'flwr':
+                    if _has_flwr:
+                        evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters), config)
+                        client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                    else:
+                        raise ImportError(
+                            "Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
                 continue
 
             parameters_to_send = None
 
             print("Tamanho parametros antes: ", sum([i.nbytes for i in parameters]))
 
             if process_parameters:
@@ -511,19 +864,20 @@
             fedpredict_clients_metrics[str(client.cid)]['acc_bytes_rate'] = size_of_parameters
             config['M'] = M
             config['decompress'] = decompress
             config['layers_fraction'] = layers_fraction
             if fl_framework is None:
                 config['parameters'] = parameters_to_send
                 client_evaluate_list_fedpredict.append((client, config))
-            elif fl_framework == 'flower':
-                evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
-                # print("Evaluate enviar: ", client_id, [i.shape for i in parameters_to_ndarrays(parameters_to_send)])
-                # print("enviar referencia: ", len(parameters), len(parameters_to_ndarrays(parameters_to_send)))
-                client_evaluate_list_fedpredict.append((client, evaluate_ins))
+            elif fl_framework == 'flwr':
+                if _has_flwr:
+                    evaluate_ins = EvaluateIns(ndarrays_to_parameters(parameters_to_send), config)
+                    client_evaluate_list_fedpredict.append((client, evaluate_ins))
+                else:
+                    raise ImportError("Flower is required. Digit: 'pip install fedpredict[flwr]' or 'pip install fedpredict[full]'")
 
         return client_evaluate_list_fedpredict
 
     except Exception as e:
         print("fedpredict server")
         print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
 
@@ -615,20 +969,15 @@
         n_layers = len(parameters) / 2
 
         # return parameters, M
 
         size_list = []
         for i in range(len(parameters)):
             tamanho = get_size(parameters[i])
-            # print("inicio camada: ", i, " tamanho: ", tamanho, " shape: ", parameters[i].shape)
             size_list.append(tamanho)
-        # print("Tamanho total parametros original: ", sum(size_list), sys.getsizeof(fl.common.ndarrays_to_parameters(parameters)))
-
-        # print("quantidade de camadas: ", len(parameters), [i.shape for i in parameters], " comment: ", comment)
-        # print("layer selection evaluate: ", self.compression, self.comment)
         if first_round != -1:
             # baixo-cima
             M = fedpredict_core_layer_selection(t=server_round, T=num_rounds, nt=nt, n_layers=n_layers,
                                                 size_per_layer=size_of_layers, df=df)
             new_parameters = []
             for i in range(len(parameters)):
                 if i in M:
@@ -653,20 +1002,15 @@
     try:
         M = [i for i in range(len(parameters))]
         n_layers = len(parameters) / 2
 
         size_list = []
         for i in range(len(parameters)):
             tamanho = get_size(parameters[i])
-            # print("inicio camada: ", i, " tamanho: ", tamanho, " shape: ", parameters[i].shape)
             size_list.append(tamanho)
-        # print("Tamanho total parametros original: ", sum(size_list), sys.getsizeof(fl.common.ndarrays_to_parameters(parameters)))
-
-        # print("quantidade de camadas: ", len(parameters), [i.shape for i in parameters], " comment: ", comment)
-        # print("layer selection evaluate: ", self.compression, self.comment)
         if first_round != -1:
             # baixo-cima
             M = [i for i in range(len(parameters))][:-2]
             new_parameters = []
             for i in range(len(parameters)):
                 if i in M:
                     new_parameters.append(parameters[i])
@@ -678,290 +1022,7 @@
             size_list.append(tamanho)
 
         return parameters, M
 
     except Exception as e:
         print("per")
         print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-
-# ===========================================================================================
-
-# FedPredict client
-
-def fedpredict_client_weight_prediction(output: torch.Tensor, t: int, current_proportion: np.array, s: float, framework='torch') -> np.array:
-    """
-        This function gives more weight to the predominant classes in the current dataset. This function is part of
-        FedPredict-Dynamic
-    Args:
-        output: torch.Tensor, required
-            The output of the model after applying 'softmax' activation function.
-        t: int, required
-            The current server round
-        current_proportion:  np.array, required
-            The classes proportion in the current training data
-        s: float, required
-            The similarity between the previous and current dataset. Note that s \in [0, 1]
-        framework: str, optional. Default='torch'
-
-    Returns:
-        np.array containing the weighted predictions
-
-    """
-
-    try:
-        if s != 1 and t > 10:
-            if framework == 'torch':
-                output = torch.multiply(output, torch.from_numpy(current_proportion * (1 - s)))
-            else:
-                raise ValueError('Framework not found')
-
-        return output
-
-    except Exception as e:
-        print("FedPredict client weight prediction")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-def fedpredict_client(local_model: torch.nn.Module, global_parameters: NDArrays,
-                      current_proportion: List[float], t: int, T: int, nt: int, M: List,
-                      local_client_information: Dict, filename: str='', knowledge_distillation=False,
-                      decompress=False, dynamic=False) -> torch.nn.Module:
-    """
-        FedPredict v.1 presented in https://ieeexplore.ieee.org/abstract/document/10257293
-        This method combines global and local parameters, providing both generalization and personalization.
-        It also prevents drop in the accuracy when new/untrained clients are evaluated
-
-        FedPredict v.3 (FedPredict-Dynamic)
-        This method combines global and local parameters, providing both generalization and personalization.
-        Differently from v.1, it takes into account the similarity between last and current dataset to weight the
-        combination and provide support for heterogeneous and non-stationary/dynamic data.
-        It also prevents drop in the accuracy when new/untrained clients are evaluated
-       Args:
-           local_model: torch.nn.Module, required
-           global_parameters: list[np.array], required
-           current_proportion: list[float], required
-           t: int, required
-           T: int, required
-           nt: int, required
-           M: list, required
-           local_client_information: dict, required
-           filename: str, optional. Default=''
-           knowledge_distillation: bool, optional. Default=False
-               If the model has knowledge distillation, then set True, to indicate that the global model parameters have
-               to be combined with the student model
-           decompress: bool, optional. Default=False
-               Whether or not to decompress global model parameters in case a previous compression was applied. Only set
-               True if using "FedPredict_server" and compressing the shared parameters.
-            dynamic: bool, optional. Default=False
-                If True, it uses the FedPredict dynamic. If False, it uses the traditional FedPredict.
-
-       Returns: torch.nn.Module
-           The combined model
-
-       """
-
-    try:
-
-        if not dynamic:
-
-            return fedpredict_client_traditional(local_model=local_model, global_parameters=global_parameters, t=t, T=T,
-                                                 nt=nt, M=M, filename=filename,
-                                                 knowledge_distillation=knowledge_distillation, decompress=decompress)
-
-        else:
-
-            return fedpredict_dynamic_client(local_model=local_model, global_parameters=global_parameters,
-                                             current_proportion=current_proportion,
-                                             t=t, T=T, nt=nt, M=M, local_client_information=local_client_information,
-                                             filename=filename,  knowledge_distillation=knowledge_distillation)
-
-    except Exception as e:
-        print("FedPredict client")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-
-def fedpredict_client_traditional(local_model: torch.nn.Module, global_parameters: NDArrays,
-                                  t: int, T: int, nt: int, M: List,
-                                  filename: str='', knowledge_distillation=False,
-                                  decompress=False) -> torch.nn.Module:
-    """
-        FedPredict v.1 presented in https://ieeexplore.ieee.org/abstract/document/10257293
-        This method combines global and local parameters, providing both generalization and personalization.
-        It also prevents drop in the accuracy when new/untrained clients are evaluated
-        Args:
-            local_model: torch.nn.Module, required
-            global_parameters: list[np.array], required
-            t: int, required
-            T: int, required
-            nt: int, required
-            M: list, required
-            filename: str, optional. Default=''
-            knowledge_distillation: bool, optional. Default=False
-                If the model has knowledge distillation, then set True, to indicate that the global model parameters have
-                to be combined with the student model
-            decompress: bool, optional. Default=False
-               Whether or not to decompress global model parameters in case a previous compression was applied. Only set
-               True if using "FedPredict_server" and compressing the shared parameters.
-
-        Returns: torch.nn.Module
-            The combined model
-
-        """
-    # Using 'torch.load'
-    try:
-        if knowledge_distillation:
-            model_shape = [i.detach().cpu().numpy().shape for i in local_model.student.parameters()]
-        else:
-            model_shape = [i.detach().cpu().numpy().shape for i in local_model.parameters()]
-        print("comprimido: ", len(model_shape))
-        global_parameters = decompress_global_parameters(global_parameters, model_shape, M, decompress)
-        print("shape modelo: ", model_shape)
-        print("descomprimido: ", [i.shape for i in global_parameters])
-        print("M: ", M)
-        # parameters = [Parameter(torch.Tensor(i.tolist())) for i in global_parameters]
-
-        if len(global_parameters) != len(M):
-            print("diferente", len(global_parameters), len(M))
-            raise Exception("Lenght of parameters is different from M")
-
-        if os.path.exists(filename):
-            # Load local parameters to 'self.model'
-            print("existe modelo local")
-            local_model.load_state_dict(torch.load(filename))
-            local_model = fedpredict_combine_models(global_parameters, local_model, t, T, nt, M)
-        else:
-            if not knowledge_distillation:
-                for old_param, new_param in zip(local_model.parameters(), global_parameters):
-                    old_param.data = new_param.data.clone()
-            else:
-                local_model.new_client = True
-                for old_param, new_param in zip(local_model.student.parameters(), global_parameters):
-                    old_param.data = new_param.data.clone()
-
-        return local_model
-
-    except Exception as e:
-        print("FedPredict client traditional")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-
-def fedpredict_dynamic_client(local_model: torch.nn.Module, global_parameters: NDArrays,
-                              current_proportion: List[float], t: int, T: int, nt: int, M:List,
-                              local_client_information: Dict, filename: str='', knowledge_distillation=False,
-                              decompress=False) -> torch.nn.Module:
-    """
-
-    Args:
-        local_model: torch.nn.Module, required
-        global_parameters: list[np.array], required
-        current_proportion: list[float], required
-        t: int, required
-        T: int, required
-        nt: int, required
-        M: list, required
-        local_client_information: dict, required
-        filename: str, optional. Default=''
-        knowledge_distillation: bool, optional. Default=False
-            If the model has knowledge distillation, then set True, to indicate that the global model parameters have
-            to be combined with the student model
-        decompress: bool, optional. Default=False
-           Whether or not to decompress global model parameters in case a previous compression was applied. Only set
-               True if using "FedPredict_server" and compressing the shared parameters.
-
-    Returns: torch.nn.Module
-        The combined model
-
-    """
-    # Using 'torch.load'
-    try:
-
-        if knowledge_distillation:
-            model_shape = [i.detach().cpu().numpy().shape for i in local_model.student.parameters()]
-        else:
-            model_shape = [i.detach().cpu().numpy().shape for i in local_model.parameters()]
-        global_parameters = decompress_global_parameters(global_parameters, model_shape, M, decompress)
-
-        if len(global_parameters) != len(M):
-            # print("diferente", len(parameters), len(M))
-            raise Exception("Lenght of parameters is different from M")
-
-        if os.path.exists(filename):
-            # Load local parameters to 'self.model'
-            # print("existe modelo local")
-            local_model.load_state_dict(torch.load(filename))
-            local_model = fedpredict_dynamic_combine_models(global_parameters, local_model, t, T, nt, M,
-                                                            local_client_information, current_proportion)
-        else:
-            # print("usar modelo global: ", cid)
-            if knowledge_distillation is None:
-                for old_param, new_param in zip(local_model.parameters(), global_parameters):
-                    old_param.data = new_param.data.clone()
-            else:
-                local_model.new_client = True
-                for old_param, new_param in zip(local_model.student.parameters(), global_parameters):
-                    old_param.data = new_param.data.clone()
-
-        return local_model
-
-    except Exception as e:
-        print("FedPredict dynamic client")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-
-def decompress_global_parameters(compressed_global_model_gradients, model_shape, M, decompress):
-    try:
-        if decompress and len(compressed_global_model_gradients) > 0:
-            decompressed_gradients = inverse_parameter_svd_reading(compressed_global_model_gradients, model_shape,
-                                                                   len(M))
-            parameters = [torch.Tensor(i.tolist()) for i in decompressed_gradients]
-        else:
-            parameters = [torch.Tensor(i.tolist()) for i in compressed_global_model_gradients]
-
-        return parameters
-
-    except Exception as e:
-        print("decompress global parameters")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-
-def fedpredict_combine_models(global_parameters, model, t, T, nt, M):
-    try:
-
-        local_model_weights, global_model_weight = fedpredict_core(t, T, nt)
-        count = 0
-        for new_param, old_param in zip(global_parameters, model.parameters()):
-            if count in M:
-                if new_param.shape == old_param.shape:
-                    old_param.data = (
-                            global_model_weight * new_param.data.clone() + local_model_weights * old_param.data.clone())
-                else:
-                    print("Não combinou, CNN student: ", new_param.shape, " CNN 3 proto: ", old_param.shape)
-            count += 1
-
-        return model
-
-    except Exception as e:
-        print("FedPredict combine models")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
-
-
-def fedpredict_dynamic_combine_models(global_parameters, model, t, T, nt, M, local_client_information,
-                                      current_proportion):
-    try:
-
-        local_model_weights, global_model_weight = fedpredict_dynamic_core(t, T, nt, local_client_information,
-                                                                           current_proportion)
-        count = 0
-        for new_param, old_param in zip(global_parameters, model.parameters()):
-            if count in M:
-                if new_param.shape == old_param.shape:
-                    old_param.data = (
-                            global_model_weight * new_param.data.clone() + local_model_weights * old_param.data.clone())
-                else:
-                    print("Não combinou, CNN student: ", new_param.shape, " CNN 3 proto: ", old_param.shape)
-            count += 1
-
-        return model
-
-    except Exception as e:
-        print("FedPredict dynamic combine models")
-        print('Error on line {}'.format(sys.exc_info()[-1].tb_lineno), type(e).__name__, e)
```

### Comparing `fedpredict-0.0.4.4/fedpredict/utils/compression_methods/fedkd.py` & `fedpredict-0.0.7/fedpredict/utils/compression_methods/fedkd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from utils.compression_methods.parameters_svd import parameter_svd_write, inverse_parameter_svd_reading, if_reduces_size
+from fedpredict.utils.compression_methods.parameters_svd import parameter_svd_write, inverse_parameter_svd_reading, if_reduces_size
 import numpy as np
 
 def fedkd_compression_core(parameters, energy):
     try:
         for i in range(0, len(parameters), 3):
             u = parameters[i]
             v = parameters[i + 1]
```

### Comparing `fedpredict-0.0.4.4/fedpredict/utils/compression_methods/fedpsarsification.py` & `fedpredict-0.0.7/fedpredict/utils/compression_methods/fedpsarsification.py`

 * *Files identical despite different names*

### Comparing `fedpredict-0.0.4.4/fedpredict/utils/compression_methods/parameters_svd.py` & `fedpredict-0.0.7/fedpredict/utils/compression_methods/parameters_svd.py`

 * *Files identical despite different names*

### Comparing `fedpredict-0.0.4.4/fedpredict/utils/compression_methods/quantization.py` & `fedpredict-0.0.7/fedpredict/utils/compression_methods/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 # from bitstring import BitArray
 import sys
-import flwr
 
 
 def quantize_linear_symmetric(value, bits):
     qmin = -2**(bits - 1)
     qmax = 2**(bits - 1) - 1
     scale = max(abs(qmin), abs(qmax)) / max(abs(np.min(value)), abs(np.max(value)))
     value = np.round(value * scale)
```

### Comparing `fedpredict-0.0.4.4/fedpredict/utils/compression_methods/sparsification.py` & `fedpredict-0.0.7/fedpredict/utils/compression_methods/sparsification.py`

 * *Files identical despite different names*

### Comparing `fedpredict-0.0.4.4/fedpredict/utils/utils.py` & `fedpredict-0.0.7/fedpredict/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import sys
 import copy
 import numpy as np
 from sklearn.metrics.pairwise import cosine_similarity, euclidean_distances
-from utils.compression_methods.parameters_svd import parameter_svd_write, inverse_parameter_svd_reading, if_reduces_size
-from utils.compression_methods.sparsification import client_model_non_zero_indexes, client_specific_top_k_parameters
-from utils.compression_methods.sparsification import sparse_crs_top_k, to_dense, sparse_matrix, get_not_zero_values
-from utils.compression_methods.fedkd import fedkd_compression
+from fedpredict.utils.compression_methods.parameters_svd import parameter_svd_write, inverse_parameter_svd_reading, if_reduces_size
+from fedpredict.utils.compression_methods.sparsification import client_model_non_zero_indexes, client_specific_top_k_parameters
+from fedpredict.utils.compression_methods.sparsification import sparse_crs_top_k, to_dense, sparse_matrix, get_not_zero_values
+from fedpredict.utils.compression_methods.fedkd import fedkd_compression
 import os
 from scipy.stats import entropy
-import scipy.stats as st
-# from torch_cka import CKA
-import pandas as pd
 
 import math
 import torch
 import numpy as np
 
 
 class CKA(object):
```

### Comparing `fedpredict-0.0.4.4/fedpredict.egg-info/SOURCES.txt` & `fedpredict-0.0.7/fedpredict.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+LICENSE
 README.md
+pyproject.toml
 setup.py
 fedpredict/__init__.py
 fedpredict/fedpredict.py
-fedpredict/test_fedpredict.py
+fedpredict/fedpredict_core.py
+fedpredict/fedpredict_torch.py
 fedpredict.egg-info/PKG-INFO
 fedpredict.egg-info/SOURCES.txt
 fedpredict.egg-info/dependency_links.txt
+fedpredict.egg-info/requires.txt
 fedpredict.egg-info/top_level.txt
 fedpredict/utils/__init__.py
 fedpredict/utils/utils.py
 fedpredict/utils/compression_methods/__init__.py
 fedpredict/utils/compression_methods/fedkd.py
 fedpredict/utils/compression_methods/fedpsarsification.py
 fedpredict/utils/compression_methods/parameters_svd.py
```

