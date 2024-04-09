# Comparing `tmp/esp-matter-mfg-tool-1.0.0.tar.gz` & `tmp/esp-matter-mfg-tool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esp-matter-mfg-tool-1.0.0.tar", last modified: Wed Feb 14 15:57:58 2024, max compression
+gzip compressed data, was "esp-matter-mfg-tool-1.0.1.tar", last modified: Tue Apr  9 07:10:38 2024, max compression
```

## Comparing `esp-matter-mfg-tool-1.0.0.tar` & `esp-matter-mfg-tool-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:58.777979 esp-matter-mfg-tool-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-14 15:57:58.777979 esp-matter-mfg-tool-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:58.773979 esp-matter-mfg-tool-1.0.0/deps/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/deps/Base38.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/deps/generate_setup_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/deps/mfg_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    38554 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/deps/nvs_partition_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/deps/spake2p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:58.777979 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-14 15:57:58.000000 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-14 15:57:58.000000 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 15:57:58.000000 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-14 15:57:58.000000 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-14 15:57:58.000000 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-14 15:57:58.000000 esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 15:57:58.777979 esp-matter-mfg-tool-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:58.777979 esp-matter-mfg-tool-1.0.0/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/sources/chip_nvs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34939 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/sources/mfg_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-02-14 15:57:44.000000 esp-matter-mfg-tool-1.0.0/sources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:38.240497 esp-matter-mfg-tool-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-09 07:10:38.240497 esp-matter-mfg-tool-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:38.236497 esp-matter-mfg-tool-1.0.1/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/deps/Base38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/deps/generate_setup_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/deps/mfg_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38554 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/deps/nvs_partition_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/deps/spake2p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:38.240497 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-09 07:10:38.000000 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 07:10:38.000000 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:10:38.000000 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 07:10:38.000000 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 07:10:38.000000 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 07:10:38.000000 esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:10:38.240497 esp-matter-mfg-tool-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:38.236497 esp-matter-mfg-tool-1.0.1/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/sources/chip_nvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36194 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/sources/mfg_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-04-09 07:10:23.000000 esp-matter-mfg-tool-1.0.1/sources/utils.py
```

### Comparing `esp-matter-mfg-tool-1.0.0/PKG-INFO` & `esp-matter-mfg-tool-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-matter-mfg-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python utility which helps to generate matter manufacturing partitions
 Home-page: https://github.com/espressif/esp-matter-tools/tree/main/mfg_tool
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp-matter-tools/tree/main/mfg_tool/README.md
 Project-URL: Source, https://github.com/espressif/esp-matter-tools/tree/main/mfg_tool
```

### Comparing `esp-matter-mfg-tool-1.0.0/README.md` & `esp-matter-mfg-tool-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `esp-matter-mfg-tool-1.0.0/deps/Base38.py` & `esp-matter-mfg-tool-1.0.1/deps/Base38.py`

 * *Files identical despite different names*

### Comparing `esp-matter-mfg-tool-1.0.0/deps/generate_setup_payload.py` & `esp-matter-mfg-tool-1.0.1/deps/generate_setup_payload.py`

 * *Files identical despite different names*

### Comparing `esp-matter-mfg-tool-1.0.0/deps/mfg_gen.py` & `esp-matter-mfg-tool-1.0.1/deps/mfg_gen.py`

 * *Files identical despite different names*

### Comparing `esp-matter-mfg-tool-1.0.0/deps/nvs_partition_gen.py` & `esp-matter-mfg-tool-1.0.1/deps/nvs_partition_gen.py`

 * *Files identical despite different names*

### Comparing `esp-matter-mfg-tool-1.0.0/deps/spake2p.py` & `esp-matter-mfg-tool-1.0.1/deps/spake2p.py`

 * *Files identical despite different names*

### Comparing `esp-matter-mfg-tool-1.0.0/esp_matter_mfg_tool.egg-info/PKG-INFO` & `esp-matter-mfg-tool-1.0.1/esp_matter_mfg_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-matter-mfg-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python utility which helps to generate matter manufacturing partitions
 Home-page: https://github.com/espressif/esp-matter-tools/tree/main/mfg_tool
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp-matter-tools/tree/main/mfg_tool/README.md
 Project-URL: Source, https://github.com/espressif/esp-matter-tools/tree/main/mfg_tool
```

### Comparing `esp-matter-mfg-tool-1.0.0/setup.py` & `esp-matter-mfg-tool-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     print(
         "Package setuptools is missing from your Python installation. "
         "Please see the installation section in the esp-matter-mfg-tool "
         "documentation for instructions on how to install it."
     )
     exit(1)
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 long_description = """
 ====================
 esp-matter-mfg-tool
 ====================
 The python utility helps to generate the matter manufacturing partitions.
```

### Comparing `esp-matter-mfg-tool-1.0.0/sources/chip_nvs.py` & `esp-matter-mfg-tool-1.0.1/sources/chip_nvs.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,14 @@
             'value': None,
         },
         'salt': {
             'type': 'data',
             'encoding': 'string',
             'value': None,
         },
-        'verifier': {
-            'type': 'data',
-            'encoding': 'string',
-            'value': None,
-        },
     }
 }
 
 
 def get_dict(key, type, encoding, value):
     return {
         key: {
```

### Comparing `esp-matter-mfg-tool-1.0.0/sources/mfg_tool.py` & `esp-matter-mfg-tool-1.0.1/sources/mfg_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,25 +85,31 @@
 
 
 def generate_passcodes(args):
     iter_count_max = 10000
     salt_len_max = 32
     with open(OUT_FILE['pin_csv'], 'w', newline='') as f:
         writer = csv.writer(f)
-        writer.writerow(["Index", "PIN Code", "Iteration Count", "Salt", "Verifier"])
+        if args.enable_dynamic_passcode:
+            writer.writerow(["Index", "Iteration Count", "Salt"])
+        else:
+            writer.writerow(["Index", "PIN Code", "Iteration Count", "Salt", "Verifier"])
         for i in range(0, args.count):
-            if args.passcode:
-                passcode = args.passcode
-            else:
-                passcode = random.randint(1, 99999998)
-                if passcode in INVALID_PASSCODES:
-                    passcode -= 1
             salt = os.urandom(salt_len_max)
-            verifier = generate_verifier(passcode, salt, iter_count_max)
-            writer.writerow([i, passcode, iter_count_max, base64.b64encode(salt).decode('utf-8'), base64.b64encode(verifier).decode('utf-8')])
+            if args.enable_dynamic_passcode:
+                writer.writerow([i, iter_count_max, base64.b64encode(salt).decode('utf-8')])
+            else:
+                if args.passcode:
+                    passcode = args.passcode
+                else:
+                    passcode = random.randint(1, 99999998)
+                    if passcode in INVALID_PASSCODES:
+                        passcode -= 1
+                verifier = generate_verifier(passcode, salt, iter_count_max)
+                writer.writerow([i, passcode, iter_count_max, base64.b64encode(salt).decode('utf-8'), base64.b64encode(verifier).decode('utf-8')])
 
 
 def generate_discriminators(args):
     discriminators = list()
 
     # If discriminator is provided, use it
     if args.discriminator:
@@ -173,15 +179,15 @@
     ])
 
     execute_cmd(cmd)
     logging.info('Generated PAI certificate: {}'.format(out_cert))
     logging.info('Generated PAI private key: {}'.format(out_key))
 
 
-def generate_dac(iteration, args, discriminator, passcode, ca_key, ca_cert):
+def generate_dac(iteration, args, ca_key, ca_cert):
     out_key_pem = os.sep.join([OUT_DIR['top'], UUIDs[iteration], 'internal', 'DAC_key.pem'])
     out_private_key_der = out_key_pem.replace('key.pem', 'key.der')
     out_cert_pem = out_key_pem.replace('key.pem', 'cert.pem')
     out_cert_der = out_key_pem.replace('key.pem', 'cert.der')
     out_private_key_bin = out_key_pem.replace('key.pem', 'private_key.bin')
     out_public_key_bin = out_key_pem.replace('key.pem', 'public_key.bin')
     cmd = [
@@ -326,21 +332,21 @@
     with open(OUT_FILE['pin_disc_csv'], 'r') as csvf:
         pin_disc_dict = csv.DictReader(csvf)
 
         for row in pin_disc_dict:
             chip_factory_update('discriminator', row['Discriminator'])
             chip_factory_update('iteration-count', row['Iteration Count'])
             chip_factory_update('salt', row['Salt'])
-            chip_factory_update('verifier', row['Verifier'])
+            if not args.enable_dynamic_passcode:
+                chip_factory_update('verifier', row['Verifier'])
             if args.paa or args.pai:
                 if args.dac_key is not None and args.dac_cert is not None:
                     dacs = use_dac_from_args(args)
                 else:
-                    dacs = generate_dac(int(row['Index']), args, int(row['Discriminator']),
-                                        int(row['PIN Code']), PAI['key_pem'], PAI['cert_pem'])
+                    dacs = generate_dac(int(row['Index']), args, PAI['key_pem'], PAI['cert_pem'])
 
                 if not args.dac_in_secure_cert:
                     chip_factory_update('dac-cert', os.path.abspath(dacs[0]))
                     chip_factory_update('dac-key', os.path.abspath(dacs[1]))
                     chip_factory_update('dac-pub-key', os.path.abspath(dacs[2]))
                     chip_factory_update('pai-cert', os.path.abspath(PAI['cert_der']))
                 else:
@@ -382,15 +388,16 @@
             if (args.csv is not None and args.mcsv is not None):
                 overwrite_values_in_mcsv(args, int(row['Index']))
 
             mcsv_row_data = chip_get_values_as_csv()
             append_chip_mcsv_row(mcsv_row_data)
 
             # Generate onboarding data
-            generate_onboarding_data(args, int(row['Index']), int(chip_factory_get_val('discriminator')), int(row['PIN Code']))
+            if not args.enable_dynamic_passcode:
+                generate_onboarding_data(args, int(row['Index']), int(chip_factory_get_val('discriminator')), int(row['PIN Code']))
         if args.paa or args.pai:
             logging.info("Generated CSV of Common Name and DAC: {}".format(OUT_FILE['cn_dac_csv']))
 
 
 def organize_output_files(suffix, args):
     for i in range(len(UUIDs)):
         dest_path = os.sep.join([OUT_DIR['top'], UUIDs[i]])
@@ -423,30 +430,37 @@
 def generate_summary(args):
     master_csv = os.sep.join([OUT_DIR['stage'], 'master.csv'])
     summary_csv = os.sep.join([OUT_DIR['top'], 'summary-{}.csv'.format(datetime.now().strftime("%Y-%m-%d-%H-%M-%S"))])
 
     summary_csv_data = ''
     with open(master_csv, 'r') as mcsvf:
         summary_lines = mcsvf.read().splitlines()
-        summary_csv_data += summary_lines[0] + ',pincode,qrcode,manualcode\n'
+        summary_csv_data += summary_lines[0]
+        if not args.enable_dynamic_passcode:
+            summary_csv_data += ',pincode,qrcode,manualcode\n'
+        else:
+            summary_csv_data += '\n'
         with open(OUT_FILE['pin_disc_csv'], 'r') as pdcsvf:
             pin_disc_dict = csv.DictReader(pdcsvf)
             for row in pin_disc_dict:
-                pincode = row['PIN Code']
-                discriminator = row['Discriminator']
-                payloads = SetupPayload(int(discriminator), int(pincode), 1 << args.discovery_mode, CommissioningFlow(args.commissioning_flow),
-                                        args.vendor_id, args.product_id)
-                qrcode = payloads.generate_qrcode()
-                manualcode = payloads.generate_manualcode()
-                # ToDo: remove this if qrcode tool can handle the standard manual code format
-                if args.commissioning_flow == CommissioningFlow.Standard:
-                    manualcode = manualcode[:4] + '-' + manualcode[4:7] + '-' + manualcode[7:]
+                if not args.enable_dynamic_passcode:
+                    pincode = row['PIN Code']
+                    discriminator = row['Discriminator']
+                    payloads = SetupPayload(int(discriminator), int(pincode), 1 << args.discovery_mode, CommissioningFlow(args.commissioning_flow),
+                                            args.vendor_id, args.product_id)
+                    qrcode = payloads.generate_qrcode()
+                    manualcode = payloads.generate_manualcode()
+                    # ToDo: remove this if qrcode tool can handle the standard manual code format
+                    if args.commissioning_flow == CommissioningFlow.Standard:
+                        manualcode = manualcode[:4] + '-' + manualcode[4:7] + '-' + manualcode[7:]
+                    else:
+                        manualcode = '"' + manualcode[:4] + '-' + manualcode[4:7] + '-' + manualcode[7:11] + '\n' + manualcode[11:15] + '-' + manualcode[15:18] + '-' + manualcode[18:20] + '-' + manualcode[20:21] + '"'
+                    summary_csv_data += summary_lines[1 + int(row['Index'])] + ',' + pincode + ',' + qrcode + ',' + manualcode + '\n'
                 else:
-                    manualcode = '"' + manualcode[:4] + '-' + manualcode[4:7] + '-' + manualcode[7:11] + '\n' + manualcode[11:15] + '-' + manualcode[15:18] + '-' + manualcode[18:20] + '-' + manualcode[20:21] + '"'
-                summary_csv_data += summary_lines[1 + int(row['Index'])] + ',' + pincode + ',' + qrcode + ',' + manualcode + '\n'
+                    summary_csv_data += summary_lines[1 + int(row['Index'])] + '\n'
 
     with open(summary_csv, 'w') as scsvf:
         scsvf.write(summary_csv_data)
 
 def generate_partitions(suffix, size, encrypt):
     partition_args = SimpleNamespace(fileid = None,
                                      version = 2,
@@ -517,14 +531,19 @@
                                  help='The discriminator for pairing. Randomly generated if not specified.')
     g_commissioning.add_argument('-cf', '--commissioning-flow', type=any_base_int, default=0,
                                  help='Device commissioning flow, 0:Standard, 1:User-Intent, 2:Custom. \
                                           Default is 0.', choices=[0, 1, 2])
     g_commissioning.add_argument('-dm', '--discovery-mode', type=any_base_int, default=1,
                                  help='Commissionable device discovery networking technology. \
                                           0:WiFi-SoftAP, 1:BLE, 2:On-network. Default is BLE.', choices=[0, 1, 2])
+    g_commissioning.add_argument('--enable-dynamic-passcode', action="store_true", required=False,
+                                 help='Enable dynamic passcode. If enabling this option, the generated binaries will \
+                                         not include the spake2p verifier. so this option should work with a custom \
+                                         CommissionableDataProvider which can generate random passcode and \
+                                         corresponding verifier')
 
     g_dac = parser.add_argument_group('Device attestation credential options')
     g_dac.add_argument('--dac-in-secure-cert', action="store_true", required=False,
                         help='Store DAC in secure cert partition. By default, DAC is stored in nvs factory partition.')
     g_dac.add_argument('-lt', '--lifetime', default=4294967295, type=any_base_int,
                        help='Lifetime of the generated certificate. Default is 4294967295 if not specified, \
                               this indicate that certificate does not have well defined expiration date.')
@@ -616,14 +635,17 @@
     # Add certificates and keys
     if (args.paa or args.pai) and (not args.dac_in_secure_cert):
         chip_factory_append('dac-cert', 'file', 'binary', None)
         chip_factory_append('dac-key', 'file', 'binary', None)
         chip_factory_append('dac-pub-key', 'file', 'binary', None)
         chip_factory_append('pai-cert', 'file', 'binary', None)
 
+    if not args.enable_dynamic_passcode:
+        chip_factory_append('verifier', 'data', 'string', None)
+
     # Add certificate declaration
     if args.cert_dclrn:
         chip_factory_append('cert-dclrn','file','binary', os.path.relpath(args.cert_dclrn))
 
     # Add the Keys in csv files
     if args.csv is not None:
         chip_nvs_map_append_config_csv(args.csv)
```

### Comparing `esp-matter-mfg-tool-1.0.0/sources/utils.py` & `esp-matter-mfg-tool-1.0.1/sources/utils.py`

 * *Files identical despite different names*

