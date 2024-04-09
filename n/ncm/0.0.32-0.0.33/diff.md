# Comparing `tmp/ncm-0.0.32.tar.gz` & `tmp/ncm-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.32.tar", last modified: Wed Apr  3 22:07:45 2024, max compression
+gzip compressed data, was "ncm-0.0.33.tar", last modified: Tue Apr  9 15:51:41 2024, max compression
```

## Comparing `ncm-0.0.32.tar` & `ncm-0.0.33.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-03 22:07:45.461346 ncm-0.0.32/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.32/LICENSE
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-03 22:07:45.460346 ncm-0.0.32/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.32/README.md
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-03 22:07:45.459346 ncm-0.0.32/ncm/
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.32/ncm/__init__.py
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   150635 2024-04-03 21:55:00.000000 ncm-0.0.32/ncm/ncm.py
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-03 22:07:45.460346 ncm-0.0.32/ncm.egg-info/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/requires.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/top_level.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-03 22:07:45.461346 ncm-0.0.32/setup.cfg
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      602 2024-04-03 21:56:14.000000 ncm-0.0.32/setup.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-09 15:51:41.222190 ncm-0.0.33/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.33/LICENSE
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-09 15:51:41.221190 ncm-0.0.33/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.33/README.md
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-09 15:51:41.221190 ncm-0.0.33/ncm/
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.33/ncm/__init__.py
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   148254 2024-04-08 23:21:43.000000 ncm-0.0.33/ncm/ncm.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-09 15:51:41.221190 ncm-0.0.33/ncm.egg-info/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/requires.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/top_level.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-09 15:51:41.222190 ncm-0.0.33/setup.cfg
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      602 2024-04-09 15:49:48.000000 ncm-0.0.33/setup.py
```

### Comparing `ncm-0.0.32/LICENSE` & `ncm-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.32/PKG-INFO` & `ncm-0.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.32
+Version: 0.0.33
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.32/README.md` & `ncm-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.32/ncm/ncm.py` & `ncm-0.0.33/ncm/ncm.py`

 * *Files 6% similar despite different names*

```diff
@@ -2180,14 +2180,16 @@
         return results
 
 
     def __parse_kwargs(self, kwargs, allowed_params):
         """
         Checks for invalid parameters and missing API Keys, and handles "filter" fields
         """
+        if 'search' in kwargs:
+            return self.__parse_search_kwargs(kwargs, allowed_params)
 
         bad_params = {k: v for (k, v) in kwargs.items() if
                       k not in allowed_params if ("search" not in k and "filter" not in k and "sort" not in k)}
         if len(bad_params) > 0:
             raise ValueError("Invalid parameters: {}".format(bad_params))
 
         if 'Authorization' not in self.session.headers:
@@ -2290,21 +2292,15 @@
                           'last_name',
                           'last_name__ne',
                           'pending_email',
                           'fields',
                           'limit',
                           'sort']
 
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
+        params = self.__parse_kwargs(kwargs, allowed_params)
         return self.__get_json(get_url, call_type, params=params)
 
     def create_user(self, email, first_name, last_name, **kwargs):
         """
         Creates a user.
         :param email: Email address
         :type email: str
@@ -2413,24 +2409,17 @@
                           'hardware_series',
                           'hardware_series_key',
                           'mac_address',
                           'serial_number',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
-
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_subscriptions(self, **kwargs):
         """
         Returns subscriptions with details.
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
         :return: A list of subscriptions with details.
@@ -2455,21 +2444,76 @@
                           'start_time__ne',
                           'tenant',
                           'type',
                           'fields',
                           'limit',
                           'sort']
 
-        if kwargs.get('search'):
-            params = self.__parse_search_kwargs(kwargs, allowed_params)
-        else:
-            params = self.__parse_kwargs(kwargs, allowed_params)
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
+    
+    def regrade(self, subscription_id, mac_or_serial_number=None):
+        """ 
+        Applies a subscription to an asset.
+        :param subscription_id: ID of the subscription to apply. (see https://developer.cradlepoint.com/ for list of subscriptions)
+        :param asset_id: ID of the asset to apply the subscription to. If not provided, the MAC address must be provided. Can also be a list
+        :param mac: MAC address of the asset to apply the subscription to. If not provided, the asset_id must be provided. Can also be a list.
+        """
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        call_type = 'Subscription'
+        post_url = f'{self.base_url}/asset_endpoints/regrade'
+
+        payload = {
+            "atomic:operations": []
+        }
+        mac_or_serial_number = mac_or_serial_number if isinstance(mac_or_serial_number, list) else [mac_or_serial_number]
+        for smac in mac_or_serial_number:
+            data = {
+                "op": "add",
+                "data": {
+                    "type": "regrades",
+                    "attributes": {
+                        "action": "UPGRADE",
+                        "subscription_type": subscription_id
+                    }
+                }
+            }
+            if len(smac) == 17:
+                data['data']['attributes']['mac_address'] = smac.replace(':','')
+            elif len(smac) == 12:
+                data['data']['attributes']['mac_address'] = smac
+            else:
+                data['data']['attributes']['serial_number'] = smac
+            payload.append(data)
+
+        ncm = self.session.post(post_url, json=payload)
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
+    def get_regrades(self, **kwargs):
+        """
+        Returns regrade jobs with details.
+        :param kwargs: A set of zero or more allowed parameters
+          in the allowed_params list.
+        :return: A list of regrades with details.
+        """
+        call_type = 'Subscription'
+        get_url = f'{self.base_url}/asset_endpoints/regrade'
+
+        allowed_params = ["id", 
+                    "action_id", 
+                    "mac_address", 
+                    "created_at", 
+                    "action", 
+                    "subcription_type", 
+                    "status", 
+                    "error_code"]
+
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_networks(self, **kwargs):
         """
         Returns information about your private cellular networks.
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
         :return: A list of PCNs with details.
@@ -2498,24 +2542,17 @@
                           'updated_at__lte',
                           'updated_at__gt',
                           'updated_at__gte',
                           'updated_at__ne',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
-
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_network(self, network_id, **kwargs):
         """
         Returns information about a private cellular network.
         :param network_id: ID of the private_cellular_networks record
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -2530,24 +2567,17 @@
                           'mobility_gateway_virtual_ip',
                           'state',
                           'status',
                           'tac',
                           'created_at',
                           'updated_at',
                           'fields']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def update_private_cellular_network(self, id=None, name=None, **kwargs):
         """
         Make changes to a private cellular network.
         :param id: PCN network ID. Specify either this or name.
         :type id: str
         :param name: PCN network name
@@ -2676,24 +2706,17 @@
                           'status',
                           'type',
                           'updated_at',
                           'url',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_core(self, core_id, **kwargs):
         """
         Returns information about a private cellular core.
         :param core_id: ID of the private_cellular_cores record
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -2709,24 +2732,17 @@
                           'router',
                           'status',
                           'type',
                           'updated_at',
                           'url',
                           'fields',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_radios(self, **kwargs):
         """
         Returns information about a private cellular radio.
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
         :return: A list of Cellular APs with details.
@@ -2761,24 +2777,17 @@
                           'tdd_mode',
                           'tx_power',
                           'type',
                           'updated_at',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_radio(self, id, **kwargs):
         """
         Returns information about a private cellular radio.
         :param id: ID of the private_cellular_radios record
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -2814,24 +2823,17 @@
                           'tdd_mode',
                           'tx_power',
                           'type',
                           'updated_at',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def update_private_cellular_radio(self, id=None, name=None, **kwargs):
         """
         Updates a Cellular AP's data.
         :param id: ID of the private_cellular_radio record. Must specify this or name.
         :type id: str
         :param name: Name of the Cellular AP. Must specify this or id.
@@ -2940,24 +2942,17 @@
                           'updated_at__lte',
                           'updated_at__gt',
                           'updated_at__gte',
                           'updated_at__ne',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_radio_group(self, group_id, **kwargs):
         """
         Returns information about a private cellular core.
         :param group_id: ID of the private_cellular_radio_groups record
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -3128,24 +3123,17 @@
                           'state_updated_at__gt',
                           'state_updated_at__gte',
                           'state_updated_at__ne',
                           'type',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_sim(self, id, **kwargs):
         """
         Returns information about a private cellular core.
         :param sim_id: ID of the private_cellular_sims record
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -3163,24 +3151,17 @@
                           'network',
                           'state',
                           'state_updated_at',
                           'type',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def update_private_cellular_sim(self, id=None, iccid=None, imsi=None, **kwargs):
         """
         Updates a SIM's data.
         :param id: ID of the private_cellular_sim record. Must specify ID, ICCID, or IMSI.
         :type id: str
         :param iccid: ICCID. Must specify ID, ICCID, or IMSI.
@@ -3255,24 +3236,17 @@
                           'operating_tx_power',
                           's1_status',
                           'time_synchronization',
                           'type',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_private_cellular_radio_status(self, status_id, **kwargs):
         """
         Returns information about a private cellular core.
         :param status_id: ID of the private_cellular_radio_statuses resource
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -3296,24 +3270,17 @@
                           'operating_tx_power',
                           's1_status',
                           'time_synchronization',
                           'type',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
 
     def get_public_sim_mgmt_assets(self, **kwargs):
         """
         Returns information about SIM asset resources in your NetCloud Manager account.
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
@@ -3328,24 +3295,17 @@
                           'device_status',
                           'iccid',
                           'is_licensed'
                           'type',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def get_public_sim_mgmt_rate_plans(self, **kwargs):
         """
         Returns information about rate plan resources associated with the SIM assets in your NetCloud Manager account.
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
         :return: Rate plans for SIM assets.
@@ -3355,24 +3315,17 @@
 
         allowed_params = ['carrier',
                           'name',
                           'status',
                           'fields',
                           'limit',
                           'sort']
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
 
-        results = self.__get_json(get_url, call_type, params=params)
-        return results
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
 
     def get_exchange_sites(self, **kwargs):
         """
         Returns exchange sites.
         :param kwargs: A set of zero or more allowed parameters
         in the allowed_params list.
@@ -3388,25 +3341,16 @@
 
         allowed_params = ['exchange_network',
                         'name',
                         'fields',
                         'limit',
                         'sort']
 
-        params = None
-        if "search" not in kwargs.keys():
-            params = self.__parse_kwargs(kwargs, allowed_params)
-        else:
-            if kwargs['search']:
-                params = self.__parse_search_kwargs(kwargs, allowed_params)
-            else:
-                params = self.__parse_kwargs(kwargs, allowed_params)
-
-        response = self.__get_json(get_url, call_type, params=params)
-        return response
+        params = self.__parse_kwargs(kwargs, allowed_params)
+        return self.__get_json(get_url, call_type, params=params)
 
     def create_exchange_site(self, name, exchange_network_id, router_id, local_domain=None, primary_dns=None, secondary_dns=None, lan_as_dns=False):
         """
         Creates an exchange site.
         :param name: Name of the exchange site.
         :type name: str
         :param primary_dns: Primary DNS of the exchange site.
@@ -3540,21 +3484,15 @@
                           'name',
                           'id',
                           'fields',
                           'limit',
                           'sort']
 
         if kwargs:
-            if "search" not in kwargs.keys():
-                params = self.__parse_kwargs(kwargs, allowed_params)
-            else:
-                if kwargs['search']:
-                    params = self.__parse_search_kwargs(kwargs, allowed_params)
-                else:
-                    params = self.__parse_kwargs(kwargs, allowed_params)
+            params = self.__parse_kwargs(kwargs, allowed_params)
 
         if exchange_site:
             params['filter[exchange_site]'] = exchange_site
         elif exchange_network:
             params['filter[exchange_network]'] = exchange_network
 
         response = self.__get_json(get_url, call_type, params=params)
```

### Comparing `ncm-0.0.32/ncm.egg-info/PKG-INFO` & `ncm-0.0.33/ncm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.32
+Version: 0.0.33
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.32/setup.py` & `ncm-0.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.32",
+    version="0.0.33",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
```

