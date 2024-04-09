# Comparing `tmp/salure_helpers_datev-1.0.5.tar.gz` & `tmp/salure_helpers_datev-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_datev-1.0.5.tar", last modified: Mon Apr  8 15:23:57 2024, max compression
+gzip compressed data, was "dist/salure_helpers_datev-1.0.6.tar", last modified: Mon Apr  8 15:29:49 2024, max compression
```

## Comparing `salure_helpers_datev-1.0.5.tar` & `salure_helpers_datev-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      259 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev.py
--rw-rw-rw-   0 root         (0) root         (0)    83624 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas.py
--rw-rw-rw-   0 root         (0) root         (0)    32802 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     5621 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/salure_helpers/datev/datev_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/
--rw-r--r--   0 root         (0) root         (0)      259 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/salure_helpers_datev.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:23:57.000000 salure_helpers_datev-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-08 15:23:40.000000 salure_helpers_datev-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:29:49.000000 salure_helpers_datev-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-08 15:29:49.000000 salure_helpers_datev-1.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:29:49.000000 salure_helpers_datev-1.0.6/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:29:49.000000 salure_helpers_datev-1.0.6/salure_helpers/datev/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-08 15:29:36.000000 salure_helpers_datev-1.0.6/salure_helpers/datev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-08 15:29:36.000000 salure_helpers_datev-1.0.6/salure_helpers/datev/datev.py
+-rw-rw-rw-   0 root         (0) root         (0)    83640 2024-04-08 15:29:36.000000 salure_helpers_datev-1.0.6/salure_helpers/datev/datev_lodas.py
+-rw-rw-rw-   0 root         (0) root         (0)    32802 2024-04-08 15:29:36.000000 salure_helpers_datev-1.0.6/salure_helpers/datev/datev_lodas_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     5621 2024-04-08 15:29:36.000000 salure_helpers_datev-1.0.6/salure_helpers/datev/datev_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:29:49.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-08 15:29:48.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-08 15:29:48.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:29:48.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:29:48.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-08 15:29:48.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-08 15:29:48.000000 salure_helpers_datev-1.0.6/salure_helpers_datev.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:29:49.000000 salure_helpers_datev-1.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-08 15:29:36.000000 salure_helpers_datev-1.0.6/setup.py
```

### Comparing `salure_helpers_datev-1.0.5/salure_helpers/datev/datev.py` & `salure_helpers_datev-1.0.6/salure_helpers/datev/datev.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas.py` & `salure_helpers_datev-1.0.6/salure_helpers/datev/datev_lodas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1204,15 +1204,15 @@
             if field not in df.columns:
                 raise KeyError(f'Column {field} is required. Required columns are: {tuple(required_fields)}')
 
         template_description = [f"309;u_lod_bwd_buchung_standard;{'pnr_betriebliche#bwd' if use_alternative_employee_number else 'pnr#bwd'};abrechnung_zeitraum#bwd;bs_wert_butab#bwd;bs_nr#bwd;kostenstelle#bwd;la_eigene#bwd;abw_lohnfaktor#bwd;\n"]
 
         body = []
         for _, row in df.iterrows():
-            body.append(
+            formatted_string = (
                 f"309;"
                 f"{row['employee_id']};"
                 f"{row['booking_date'] if 'booking_date' in row.keys() else ''};"
                 f"{row['value'] if 'value' in row.keys() else ''};"
                 f"{row['declaration_type'] if 'declaration_type' in row.keys() else ''};"
                 f"{row['costcenter'] if 'costcenter' in row.keys() else ''};"
                 f"{row['wage_component'] if 'wage_component' in row.keys() else ''};"
@@ -1240,15 +1240,15 @@
             if field not in df.columns:
                 raise KeyError(f'Column {field} is required. Required columns are: {tuple(required_fields)}')
 
         template_description = [f"1300;u_lod_psd_vermoegensbildung;{'pnr_betriebliche#psd' if use_alternative_employee_number else 'pnr#psd'};vwl_1_netto_abz_1#psd;vwl_ag_anteil_la_1#psd;vwl_ag_anteil_betrag_1#psd;lastschrift1_kz#psd;\n"]
 
         body = []
         for _, row in df.iterrows():
-            body.append(
+            formatted_string = (
                 f"1300;"
                 f"{row['employee_id']};"
                 f"{row['vwl_saving_formation'] if 'vwl_saving_formation' in row.keys() else ''};"
                 f"{row['vwl_wage_component'] if 'vwl_wage_component' in row.keys() else ''};"
                 f"{row['vwl_amount'] if 'vwl_amount' in row.keys() else ''};"
                 f"{row['vwl_direct_debit'] if 'vwl_direct_debit' in row.keys() else ''};\n"
             )
```

### Comparing `salure_helpers_datev-1.0.5/salure_helpers/datev/datev_lodas_mapping.py` & `salure_helpers_datev-1.0.6/salure_helpers/datev/datev_lodas_mapping.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_datev-1.0.5/salure_helpers/datev/datev_mapping.py` & `salure_helpers_datev-1.0.6/salure_helpers/datev/datev_mapping.py`

 * *Files identical despite different names*

