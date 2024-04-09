# Comparing `tmp/feagi_connector-0.0.3.tar.gz` & `tmp/feagi_connector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector-0.0.3.tar", last modified: Fri Apr  5 14:32:43 2024, max compression
+gzip compressed data, was "feagi_connector-0.0.4.tar", last modified: Tue Apr  9 17:16:10 2024, max compression
```

## Comparing `feagi_connector-0.0.3.tar` & `feagi_connector-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/feagi_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/PIL_retina.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/actuators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18257 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/feagi_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/pns_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/retina.py
--rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/feagi_connector/sensorimotor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/sensorimotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/testing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/feagi_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-05 14:32:43.194604 feagi_connector-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/feagi_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/PIL_retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/actuators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/feagi_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/pns_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/feagi_connector/sensorimotor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/sensorimotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/testing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/feagi_connector/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 17:16:00.000000 feagi_connector-0.0.4/feagi_connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/feagi_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 17:16:10.000000 feagi_connector-0.0.4/feagi_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 17:15:59.000000 feagi_connector-0.0.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-09 17:16:10.370454 feagi_connector-0.0.4/setup.cfg
```

### Comparing `feagi_connector-0.0.3/LICENSE` & `feagi_connector-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/PKG-INFO` & `feagi_connector-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.3
+Version: 0.0.4
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.3/README.md` & `feagi_connector-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/PIL_retina.py` & `feagi_connector-0.0.4/feagi_connector/PIL_retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/actuators.py` & `feagi_connector-0.0.4/feagi_connector/actuators.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/configuration.py` & `feagi_connector-0.0.4/feagi_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/feagi_interface.py` & `feagi_connector-0.0.4/feagi_connector/feagi_interface.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
+import os
+import json
+import socket
+import argparse
+import requests
+import threading
 import traceback
+from time import sleep
 from feagi_connector import router
 from feagi_connector import pns_gateway as pns
 from feagi_connector.version import __version__
-from time import sleep
-import requests
-import socket
-import threading
 
 
 
 def pub_initializer(ipu_address, bind=True):
     return router.Pub(address=ipu_address, bind=bind)
 
 
 def sub_initializer(opu_address, flags=router.zmq.NOBLOCK):
     return router.Sub(address=opu_address, flags=flags)
 
 
 def feagi_registration(feagi_auth_url, feagi_settings, agent_settings, capabilities,
-                       controller_version, magic_link=''):
+                       controller_version):
     host_info = router.app_host_info()
     runtime_data = {
         "host_network": {},
         "feagi_state": None
     }
     runtime_data["host_network"]["host_name"] = host_info["host_name"]
     runtime_data["host_network"]["ip_address"] = host_info["ip_address"]
     agent_settings['agent_ip'] = host_info["ip_address"]
 
     while runtime_data["feagi_state"] is None:
         print("\nAwaiting registration with FEAGI...")
         try:
             runtime_data["feagi_state"] = \
                 router.register_with_feagi(feagi_auth_url, feagi_settings, agent_settings,
-                                           capabilities, controller_version, __version__, magic_link)
+                                           capabilities, controller_version, __version__)
         except Exception as e:
             print("ERROR__: ", e, traceback.print_exc())
             pass
         sleep(1)
     print("\nversion: ", controller_version, "\n")
     print("\nagent version: ", __version__, "\n")
     return runtime_data["feagi_state"]
@@ -318,29 +321,28 @@
                 configuration.capabilities["position"][position_index]["z"] = \
                     float(control_data['robot_starting_position'][position_index][2])
         return configuration.capabilities["motor"]["power_coefficient"], \
                configuration.capabilities["position"]
 
 
 def connect_to_feagi(feagi_settings, runtime_data, agent_settings, capabilities, current_version,
-                     bind_flag=False, magic_link=''):
+                     bind_flag=False):
     print("Connecting to FEAGI resources...")
     feagi_auth_url = feagi_settings.pop('feagi_auth_url', None)
     runtime_data["feagi_state"] = feagi_registration(feagi_auth_url=feagi_auth_url,
                                                      feagi_settings=feagi_settings,
                                                      agent_settings=agent_settings,
                                                      capabilities=capabilities,
-                                                     controller_version=current_version,
-                                                     magic_link=magic_link)
+                                                     controller_version=current_version)
     api_address = runtime_data['feagi_state']["feagi_url"]
     router.global_api_address = api_address
     agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
-    if magic_link == '':
+    if 'magic_link' not in feagi_settings:
         if bind_flag:
             ipu_channel_address = "tcp://*:" + agent_data_port  # This is for godot to work due to
             # bind unable to use the dns.
         else:
             ipu_channel_address = feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
 
         print("IPU_channel_address=", ipu_channel_address)
@@ -387,7 +389,72 @@
 
 def mctl_neuron_update(feagi_power, id):
     z_depth = pns.full_list_dimension['o_mctl']['cortical_dimensions'][2]
     if id / z_depth == 0:
         return feagi_power / 100.0
     else:
         return feagi_power / z_depth
+
+def configuration_load(path='./'):
+    # NEW JSON UPDATE
+    f = open(path + 'configuration.json')
+    configuration = json.load(f)
+    feagi_settings = configuration["feagi_settings"]
+    agent_settings = configuration['agent_settings']
+    capabilities = configuration['capabilities']
+    feagi_settings['feagi_host'] = os.environ.get('FEAGI_HOST_INTERNAL', "127.0.0.1")
+    feagi_settings['feagi_api_port'] = os.environ.get('FEAGI_API_PORT', "8000")
+    message_to_feagi = {"data": {}}
+    f.close()
+    return feagi_settings, agent_settings, capabilities, message_to_feagi, configuration
+    # END JSON UPDATE
+
+def reading_parameters_to_confirm_communication(feagi_settings, configuration, path="."):
+    # Check if feagi_connector has arg
+    parser = argparse.ArgumentParser(description='enable to use magic link')
+    parser.add_argument('-magic_link', '--magic_link', help='to use magic link', required=False)
+    parser.add_argument('-magic-link', '--magic-link', help='to use magic link', required=False)
+    parser.add_argument('-magic', '--magic', help='to use magic link', required=False)
+    parser.add_argument('-ip', '--ip', help='to use feagi_ip', required=False)
+    parser.add_argument('-port', '--port', help='to use feagi_port', required=False)
+    args = vars(parser.parse_args())
+    if feagi_settings['feagi_url'] or args['magic'] or args['magic_link']:
+        if args['magic'] or args['magic_link']:
+            for arg in args:
+                if args[arg] is not None:
+                    feagi_settings['magic_link'] = args[arg]
+                    break
+            configuration['feagi_settings']['feagi_url'] = feagi_settings['magic_link']
+            with open(path+'configuration.json', 'w') as f:
+                json.dump(configuration, f)
+        else:
+            feagi_settings['magic_link'] = feagi_settings['feagi_url']
+        url_response = json.loads(requests.get(feagi_settings['magic_link']).text)
+        feagi_settings['feagi_dns'] = url_response['feagi_url']
+        feagi_settings['feagi_api_port'] = url_response['feagi_api_port']
+    else:
+        # # FEAGI REACHABLE CHECKER # #
+        feagi_flag = False
+        print("retrying...")
+        print("Waiting on FEAGI...")
+        if args['ip']:
+            feagi_settings['feagi_host'] = args['ip']
+        while not feagi_flag:
+            feagi_flag = is_FEAGI_reachable(os.environ.get('FEAGI_HOST_INTERNAL', feagi_settings["feagi_host"]),int(os.environ.get('FEAGI_OPU_PORT', "3000")))
+            sleep(2)
+    return feagi_settings, configuration
+
+def build_up_from_configuration(path="./"):
+    feagi_settings, agent_settings, capabilities, message_to_feagi, configuration = configuration_load(path)
+    default_capabilities = {}  # It will be generated in process_visual_stimuli. See the
+    # overwrite manual
+    default_capabilities = pns.create_runtime_default_list(default_capabilities, capabilities)
+
+    feagi_settings, configuration = reading_parameters_to_confirm_communication(feagi_settings, configuration,path)
+    return {
+        "feagi_settings": feagi_settings,
+        "agent_settings": agent_settings,
+        "default_capabilities": default_capabilities,
+        "message_to_feagi": message_to_feagi,
+        "capabilities": capabilities
+    }
+
```

### Comparing `feagi_connector-0.0.3/feagi_connector/pns_gateway.py` & `feagi_connector-0.0.4/feagi_connector/pns_gateway.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/retina.py` & `feagi_connector-0.0.4/feagi_connector/retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/router.py` & `feagi_connector-0.0.4/feagi_connector/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
 def feagi_listener(feagi_opu_channel):
     while True:
         data = fetch_feagi(feagi_opu_channel)
         if data is not None:
             pns.message_from_feagi = data
         sleep(0.001)  # hardcoded and max second that it can run up to
+        # print("inside router: ", pns.message_from_feagi['opu_data']['o__gaz'])
 
 
 def send_feagi(message_to_feagi, feagi_ipu_channel, agent_settings):
     """
     send data to FEAGI
     """
     if agent_settings['compression']:
@@ -179,15 +180,15 @@
     else:
         feagi_settings[
             'feagi_url'] = f"http://{feagi_settings['feagi_host']}:{feagi_settings['feagi_api_port']}"
     return feagi_settings
 
 
 def register_with_feagi(feagi_auth_url, feagi_settings, agent_settings, agent_capabilities,
-                        controller_version, agent_version, magic_link=''):
+                        controller_version, agent_version):
     """
     To trade information between FEAGI and Controller
 
     Controller                      <--     FEAGI(IPU/OPU socket info)
     Controller (Capabilities)       -->     FEAGI
     """
     network_endpoint = '/v1/network/network'
@@ -202,15 +203,15 @@
             feagi_settings = feagi_settings_from_composer(feagi_auth_url, feagi_settings)
             feagi_url = feagi_settings['feagi_url']
 
             print("feagiurl: ", feagi_url, " network endpoint: ", network_endpoint)
 
             network_output = requests.get(feagi_url + network_endpoint).json()
             # print(f"network_output ---- {network_output}")
-            if magic_link == '':
+            if 'magic_link' not in feagi_settings:
                 feagi_settings['feagi_opu_port'] = network_output['feagi_opu_port']
             if feagi_settings:
                 print("Data from FEAGI::", feagi_settings)
             else:
                 print("No feagi settings!")
 
             agent_registration_data = dict()
@@ -234,15 +235,15 @@
                     print("\n\n\n\nRegistration is complete....")
                     registration_complete = True
         except Exception as e:
             print("Registeration failed with FEAGI: ", e)
             # traceback.print_exc()
         sleep(2)
 
-    if magic_link == '':
+    if 'magic_link' not in feagi_settings:
         # feagi_settings['agent_state']['agent_ip'] = "127.0.0.1"
         print(f"Final Feagi Settings ---- {feagi_settings}")
         feagi_ip = feagi_settings['feagi_host']
         agent_data_port = feagi_settings['agent_state']['agent_data_port']
         print("feagi_ip:agent_data_port", feagi_ip, agent_data_port)
         # Transmit Controller Capabilities
         # address, bind = f"tcp://*:{agent_data_port}", True
```

### Comparing `feagi_connector-0.0.3/feagi_connector/sensors.py` & `feagi_connector-0.0.4/feagi_connector/sensors.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/testing_mode.py` & `feagi_connector-0.0.4/feagi_connector/testing_mode.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector/trainer.py` & `feagi_connector-0.0.4/feagi_connector/trainer.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/feagi_connector.egg-info/PKG-INFO` & `feagi_connector-0.0.4/feagi_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.3
+Version: 0.0.4
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.3/feagi_connector.egg-info/SOURCES.txt` & `feagi_connector-0.0.4/feagi_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.3/setup.cfg` & `feagi_connector-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector
-version = 0.0.3
+version = 0.0.4
 author = Neuraville Inc.
 author_email = info@feagi.org
 description = Feagi agent to work with general and simulation robots
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi-connector
 project_urls =
```

