# Comparing `tmp/apoplast-1.1.1.tar.gz` & `tmp/apoplast-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apoplast-1.1.1.tar", last modified: Sun Mar 31 22:19:14 2024, max compression
+gzip compressed data, was "apoplast-1.1.2.tar", last modified: Tue Apr  9 20:17:14 2024, max compression
```

## Comparing `apoplast-1.1.1.tar` & `apoplast-1.1.2.tar`

### file list

```diff
@@ -1,582 +1,604 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1024 2024-03-31 22:19:14.475580 apoplast-1.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      661 2024-03-31 22:19:07.000000 apoplast-1.1.1/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      550 2024-03-30 21:10:34.000000 apoplast-1.1.1/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 22:19:14.475580 apoplast-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.395581 apoplast-1.1.1/structures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.399581 apoplast-1.1.1/structures/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.419580 apoplast-1.1.1/structures/modules/apoplast/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.419580 apoplast-1.1.1/structures/modules/apoplast/-license/
--rwxrwxrwx   0 root         (0) root         (0)      427 2024-02-04 21:45:08.000000 apoplast-1.1.1/structures/modules/apoplast/-license/license.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.419580 apoplast-1.1.1/structures/modules/apoplast/-license/list/
--rwxrwxrwx   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 apoplast-1.1.1/structures/modules/apoplast/-license/list/gpl-3.0-standalone.html
--rwxrwxrwx   0 root         (0) root         (0)      112 2024-02-04 21:44:43.000000 apoplast-1.1.1/structures/modules/apoplast/-license/list/vegan.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-16 19:46:47.000000 apoplast-1.1.1/structures/modules/apoplast/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.419580 apoplast-1.1.1/structures/modules/apoplast/__itinerary/
--rwxrwxrwx   0 root         (0) root         (0)      371 2024-03-29 21:00:21.000000 apoplast-1.1.1/structures/modules/apoplast/__itinerary/apoplast.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.419580 apoplast-1.1.1/structures/modules/apoplast/__itinerary/book/
--rwxrwxrwx   0 root         (0) root         (0)      377 2023-11-16 22:44:34.000000 apoplast-1.1.1/structures/modules/apoplast/__itinerary/book/Vitamin B.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-11-16 20:32:46.000000 apoplast-1.1.1/structures/modules/apoplast/__itinerary/book/Vitamin K.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.423580 apoplast-1.1.1/structures/modules/apoplast/__status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.423580 apoplast-1.1.1/structures/modules/apoplast/__status/db/
--rwxrwxrwx   0 root         (0) root         (0)  6359047 2024-03-31 22:08:41.000000 apoplast-1.1.1/structures/modules/apoplast/__status/db/records.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/__status/db_API/
--rwxrwxrwx   0 root         (0) root         (0)    30367 2024-02-04 22:01:04.000000 apoplast-1.1.1/structures/modules/apoplast/__status/db_API/records.json
--rwxrwxrwx   0 root         (0) root         (0)     1311 2024-03-30 21:08:27.000000 apoplast-1.1.1/structures/modules/apoplast/__status/status.proc.py
--rwxrwxrwx   0 root         (0) root         (0)     1209 2024-03-30 21:08:29.000000 apoplast-1.1.1/structures/modules/apoplast/__status/status_API.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/_ellipses/
--rwxrwxrwx   0 root         (0) root         (0)      424 2024-03-30 22:53:59.000000 apoplast-1.1.1/structures/modules/apoplast/_ellipses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/_variables/
--rw-rw-r--   0 root         (0) root         (0)      632 2024-03-31 02:57:01.000000 apoplast-1.1.1/structures/modules/apoplast/_variables/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/affiliates_Amazon/
--rwxrwxrwx   0 root         (0) root         (0)      118 2024-02-04 18:06:33.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/affiliates_Amazon/affiliates.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      111 2024-03-31 01:44:52.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/clouds.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/
--rwxrwxrwx   0 root         (0) root         (0)     1036 2024-03-31 22:06:11.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/assertions/
--rwxrwxrwx   0 root         (0) root         (0)      429 2023-10-29 21:44:17.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/assertions/branded.py
--rwxrwxrwx   0 root         (0) root         (0)      264 2023-11-17 17:51:13.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/assertions/foundational.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/status/
--rwxrwxrwx   0 root         (0) root         (0)      419 2023-11-17 00:19:37.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/status/API_status_branded_1.py
--rwxrwxrwx   0 root         (0) root         (0)      465 2023-11-17 00:19:37.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/status/API_status_foundational_1.py
--rwxrwxrwx   0 root         (0) root         (0)      370 2023-11-16 23:17:45.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.427580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/
--rwxrwxrwx   0 root         (0) root         (0)     1009 2023-11-22 01:31:31.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/
--rwxrwxrwx   0 root         (0) root         (0)    37079 2023-12-09 20:38:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
--rwxrwxrwx   0 root         (0) root         (0)    37079 2023-11-22 01:40:03.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
--rwxrwxrwx   0 root         (0) root         (0)     7242 2023-10-19 22:27:22.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON
--rwxrwxrwx   0 root         (0) root         (0)     8522 2023-10-12 21:13:07.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON
--rwxrwxrwx   0 root         (0) root         (0)    33964 2023-11-22 01:38:38.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/problems/
--rwxrwxrwx   0 root         (0) root         (0)    17926 2023-09-25 16:28:17.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON
--rwxrwxrwx   0 root         (0) root         (0)      104 2023-11-26 02:04:47.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/problems/problems.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)    10678 2023-11-22 01:32:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON
--rwxrwxrwx   0 root         (0) root         (0)    10670 2023-10-24 03:17:57.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/foundational/
--rwxrwxrwx   0 root         (0) root         (0)   189146 2023-10-12 22:00:16.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
--rwxrwxrwx   0 root         (0) root         (0)      255 2023-11-17 18:04:07.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/mergers.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)       88 2023-11-22 01:27:20.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/priorities.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)      457 2023-12-09 23:06:15.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      614 2023-12-15 19:53:16.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/food.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.399581 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/foodNutrient/
--rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-22 04:54:08.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/foodNutrient/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/labelNutrient/
--rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-22 02:45:04.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/labelNutrient/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/
--rwxrwxrwx   0 root         (0) root         (0)     1783 2023-11-23 18:42:09.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      583 2023-11-22 00:01:06.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/
--rwxrwxrwx   0 root         (0) root         (0)     4126 2023-11-22 20:58:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1229 2023-11-22 20:47:39.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py
--rwxrwxrwx   0 root         (0) root         (0)      877 2023-11-22 20:23:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/
--rwxrwxrwx   0 root         (0) root         (0)      415 2023-11-22 20:49:55.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1374 2023-11-22 20:23:29.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/
--rwxrwxrwx   0 root         (0) root         (0)     5029 2024-01-08 21:02:44.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/
--rwxrwxrwx   0 root         (0) root         (0)     2606 2024-02-04 20:24:03.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1610 2023-12-09 20:39:39.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_2.py
--rwxrwxrwx   0 root         (0) root         (0)     1236 2023-12-17 01:49:13.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_2412474.py
--rwxrwxrwx   0 root         (0) root         (0)     1078 2023-12-17 00:42:09.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_3.py
--rwxrwxrwx   0 root         (0) root         (0)      812 2023-12-09 20:39:39.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/cautionary_ingredients/
--rwxrwxrwx   0 root         (0) root         (0)     3302 2023-12-15 23:15:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/energy/
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-11-26 00:02:13.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/energy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.431580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/essential_nutrients/
--rwxrwxrwx   0 root         (0) root         (0)     3116 2023-12-17 00:12:42.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/
--rwxrwxrwx   0 root         (0) root         (0)     4031 2023-11-26 01:50:19.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1231 2024-03-31 22:06:29.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/status_mass_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1159 2023-11-26 00:30:32.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/status_volume_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/
--rwxrwxrwx   0 root         (0) root         (0)     1427 2023-11-27 04:58:37.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/
--rwxrwxrwx   0 root         (0) root         (0)     1676 2023-11-26 01:00:29.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1875 2024-03-31 22:07:48.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1579 2023-11-26 01:00:16.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/
--rwxrwxrwx   0 root         (0) root         (0)     2077 2023-11-26 01:09:26.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/
--rwxrwxrwx   0 root         (0) root         (0)     1224 2023-11-26 01:10:07.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/
--rwxrwxrwx   0 root         (0) root         (0)     1494 2023-11-26 23:54:17.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/
--rwxrwxrwx   0 root         (0) root         (0)     1389 2024-03-29 23:33:34.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/
--rwxrwxrwx   0 root         (0) root         (0)      622 2023-11-26 02:01:26.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py
--rwxrwxrwx   0 root         (0) root         (0)      468 2023-11-22 04:50:10.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/label_nutrient.py
--rwxrwxrwx   0 root         (0) root         (0)      503 2023-11-26 00:52:57.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-11-22 20:45:42.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/
--rwxrwxrwx   0 root         (0) root         (0)      485 2023-11-26 01:53:47.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/
--rwxrwxrwx   0 root         (0) root         (0)     2092 2023-11-24 04:45:08.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py
--rwxrwxrwx   0 root         (0) root         (0)      687 2023-11-26 00:51:56.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-11-26 00:49:48.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/
--rwxrwxrwx   0 root         (0) root         (0)      863 2023-11-23 23:49:12.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/
--rwxrwxrwx   0 root         (0) root         (0)      575 2023-11-23 23:46:06.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1019 2023-11-23 23:47:00.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/goodness_certifications/
--rw-rw-r--   0 root         (0) root         (0)     1791 2024-03-31 18:10:18.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/goodness_certifications/certifications.py
--rwxrwxrwx   0 root         (0) root         (0)      641 2024-03-31 20:50:04.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/goodness_certifications/vegan.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/
--rwxrwxrwx   0 root         (0) root         (0)     1046 2024-03-31 02:07:55.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/NIH.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.435580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/
--rwxrwxrwx   0 root         (0) root         (0)     1137 2024-03-31 22:06:43.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1087 2023-10-25 01:29:58.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/assertions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/status/
--rwxrwxrwx   0 root         (0) root         (0)      392 2023-11-17 00:20:01.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/status/API_status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      316 2023-10-25 01:28:37.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/
--rwxrwxrwx   0 root         (0) root         (0)      848 2023-11-27 22:36:33.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/coated tablets/
--rwxrwxrwx   0 root         (0) root         (0)    44597 2023-10-13 17:10:19.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/other/
--rwxrwxrwx   0 root         (0) root         (0)    22180 2023-10-25 17:22:33.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder/
--rwxrwxrwx   0 root         (0) root         (0)     6430 2023-10-13 17:09:44.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON
--rwxrwxrwx   0 root         (0) root         (0)    72594 2023-10-25 01:46:01.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder packets/
--rwxrwxrwx   0 root         (0) root         (0)    57378 2023-10-13 17:05:59.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/tablets/
--rwxrwxrwx   0 root         (0) root         (0)    22710 2023-10-13 17:08:42.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON
--rwxrwxrwx   0 root         (0) root         (0)    43725 2023-10-13 17:08:08.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/vegan_capsules/
--rwxrwxrwx   0 root         (0) root         (0)     7107 2023-10-13 17:07:29.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.403581 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/
--rwxrwxrwx   0 root         (0) root         (0)       98 2023-11-27 03:46:15.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/
--rwxrwxrwx   0 root         (0) root         (0)     1152 2023-11-27 04:24:46.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      923 2023-11-27 04:25:24.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/servingSizeUnit/
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-11-27 04:49:39.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/servingSizeUnit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/
--rwxrwxrwx   0 root         (0) root         (0)     4087 2024-03-31 22:07:01.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.403581 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/_loop/
--rwxrwxrwx   0 root         (0) root         (0)      730 2023-11-27 22:52:02.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/
--rwxrwxrwx   0 root         (0) root         (0)     1580 2024-03-11 02:00:19.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py
--rwxrwxrwx   0 root         (0) root         (0)   136857 2024-03-31 22:08:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/other/
--rwxrwxrwx   0 root         (0) root         (0)   100726 2024-03-31 22:08:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON
--rwxrwxrwx   0 root         (0) root         (0)      762 2024-03-11 02:02:48.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/powder/
--rwxrwxrwx   0 root         (0) root         (0)    28773 2024-03-31 22:08:41.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON
--rwxrwxrwx   0 root         (0) root         (0)      748 2023-12-19 18:33:07.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/
--rwxrwxrwx   0 root         (0) root         (0)     2753 2023-12-15 23:31:38.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.439580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/essential_nutrients/
--rwxrwxrwx   0 root         (0) root         (0)     2583 2024-03-30 21:02:16.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      832 2023-11-27 20:26:53.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      281 2023-11-27 20:27:05.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients_priorities.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/
--rwxrwxrwx   0 root         (0) root         (0)      323 2023-11-27 04:41:57.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/amount/
--rwxrwxrwx   0 root         (0) root         (0)      676 2023-11-27 23:18:44.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      510 2023-11-22 19:45:00.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/amount/status_other_214893.py
--rwxrwxrwx   0 root         (0) root         (0)      512 2023-11-25 23:13:17.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/form.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.403581 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/
--rwxrwxrwx   0 root         (0) root         (0)     3759 2023-11-27 23:36:21.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 22:52:26.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1843 2023-11-27 23:35:48.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py
--rwxrwxrwx   0 root         (0) root         (0)     1711 2023-11-27 23:47:05.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/
--rwxrwxrwx   0 root         (0) root         (0)     3210 2023-11-27 23:13:13.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2023-11-27 23:17:35.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-11-22 18:01:32.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py
--rwxrwxrwx   0 root         (0) root         (0)      818 2023-11-22 19:42:51.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py
--rwxrwxrwx   0 root         (0) root         (0)      903 2023-11-22 19:46:12.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py
--rwxrwxrwx   0 root         (0) root         (0)     1333 2023-11-22 20:15:00.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py
--rwxrwxrwx   0 root         (0) root         (0)      701 2023-11-22 20:21:05.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py
--rwxrwxrwx   0 root         (0) root         (0)      725 2023-11-22 19:30:39.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/
--rwxrwxrwx   0 root         (0) root         (0)     4631 2024-03-11 02:07:04.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/
--rwxrwxrwx   0 root         (0) root         (0)     1687 2024-03-11 02:13:24.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.403581 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/mass/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 05:04:38.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/mass/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1514 2024-03-11 01:32:01.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/
--rwxrwxrwx   0 root         (0) root         (0)     1656 2024-03-30 21:01:47.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/
--rwxrwxrwx   0 root         (0) root         (0)      826 2024-03-11 02:03:57.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py
--rwxrwxrwx   0 root         (0) root         (0)      561 2023-11-27 05:48:16.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/
--rwxrwxrwx   0 root         (0) root         (0)     1116 2023-11-27 05:48:52.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      657 2023-11-27 05:50:29.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/
--rwxrwxrwx   0 root         (0) root         (0)      511 2023-11-27 18:44:30.000000 apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/
--rw-rw-r--   0 root         (0) root         (0)       44 2024-03-31 01:43:36.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/data_nodes.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.443580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/DB/
--rw-rw-r--   0 root         (0) root         (0)      436 2024-03-31 02:58:40.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/DB/connect.py
--rw-rw-r--   0 root         (0) root         (0)     1123 2024-03-31 03:51:14.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/DB/export.py
--rw-rw-r--   0 root         (0) root         (0)     1185 2024-03-31 03:17:06.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/DB/open.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/__itinerary/
--rw-rw-r--   0 root         (0) root         (0)      454 2024-03-31 01:44:39.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/__itinerary/itinerary.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/cautionary_ingredients/
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-31 03:53:00.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/cautionary_ingredients/cautionary_ingredients.1.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/essential_nutrients/
--rw-r--r--   0 root         (0) root         (0)     5140 2024-03-31 03:54:30.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/essential_nutrients/essential_nutrients.1.json
--rw-rw-r--   0 root         (0) root         (0)      481 2024-03-31 03:53:37.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/exports.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.407580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/_land/
--rw-rw-r--   0 root         (0) root         (0)      796 2024-03-31 03:43:31.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/_land/insert_document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/
--rw-rw-r--   0 root         (0) root         (0)        2 2024-03-31 03:51:33.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/export.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 02:55:12.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/insert_document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/essential_nutrients/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 03:51:29.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/essential_nutrients/export.py
--rw-rw-r--   0 root         (0) root         (0)     1424 2024-03-31 01:43:27.000000 apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/ingredients.S.HTML
--rw-rw-r--   0 root         (0) root         (0)       14 2024-03-31 22:10:20.000000 apoplast-1.1.1/structures/modules/apoplast/emojis.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/insure/
--rwxrwxrwx   0 root         (0) root         (0)     1085 2023-11-27 23:25:39.000000 apoplast-1.1.1/structures/modules/apoplast/insure/equalities.py
--rwxrwxrwx   0 root         (0) root         (0)      234 2023-11-22 18:56:47.000000 apoplast-1.1.1/structures/modules/apoplast/insure/equality.py
--rwxrwxrwx   0 root         (0) root         (0)      729 2023-11-27 01:34:09.000000 apoplast-1.1.1/structures/modules/apoplast/insure/override_print.py
--rwxrwxrwx   0 root         (0) root         (0)      374 2023-11-22 19:22:12.000000 apoplast-1.1.1/structures/modules/apoplast/insure/status_equalitites_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.407580 apoplast-1.1.1/structures/modules/apoplast/measures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/_interpret/
--rwxrwxrwx   0 root         (0) root         (0)       61 2023-10-24 19:09:48.000000 apoplast-1.1.1/structures/modules/apoplast/measures/_interpret/interpret.r.html
--rwxrwxrwx   0 root         (0) root         (0)      670 2023-11-22 03:00:29.000000 apoplast-1.1.1/structures/modules/apoplast/measures/_interpret/status_unit_kind.py
--rwxrwxrwx   0 root         (0) root         (0)     1678 2023-11-27 23:51:26.000000 apoplast-1.1.1/structures/modules/apoplast/measures/_interpret/unit_kind.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/biological_activity/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-22 02:29:15.000000 apoplast-1.1.1/structures/modules/apoplast/measures/biological_activity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/electric_current/
--rwxrwxrwx   0 root         (0) root         (0)       59 2024-02-26 21:23:18.000000 apoplast-1.1.1/structures/modules/apoplast/measures/electric_current/electric_current.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/energy/
--rwxrwxrwx   0 root         (0) root         (0)     1142 2023-11-18 02:03:26.000000 apoplast-1.1.1/structures/modules/apoplast/measures/energy/energy.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/energy/swap/
--rwxrwxrwx   0 root         (0) root         (0)     1174 2023-11-27 05:11:29.000000 apoplast-1.1.1/structures/modules/apoplast/measures/energy/swap/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      386 2023-11-22 03:06:00.000000 apoplast-1.1.1/structures/modules/apoplast/measures/energy/swap/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/length/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-11-18 02:08:27.000000 apoplast-1.1.1/structures/modules/apoplast/measures/length/length.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/mass/
--rwxrwxrwx   0 root         (0) root         (0)       95 2023-09-10 01:33:12.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass/e_note.py
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-10-24 23:00:23.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass/mass.r.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.447580 apoplast-1.1.1/structures/modules/apoplast/measures/mass/swap/
--rwxrwxrwx   0 root         (0) root         (0)     2329 2023-11-27 23:53:01.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass/swap/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1153 2023-11-21 20:24:21.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass/swap/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     2419 2023-10-25 22:32:32.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass/system international.r.html
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-10-24 19:13:36.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass/us customary.r.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/is_an_equivalent/
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-11-18 02:19:07.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      342 2023-11-18 02:17:02.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/is_an_equivalent/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      861 2023-11-18 02:32:14.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/jargon.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)     2242 2023-12-09 18:56:13.000000 apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/mass equivalents.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.407580 apoplast-1.1.1/structures/modules/apoplast/measures/number/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.407580 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/
--rwxrwxrwx   0 root         (0) root         (0)     2431 2024-02-26 20:25:18.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1428 2023-11-26 02:08:37.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      901 2023-11-21 19:30:34.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_2.py
--rwxrwxrwx   0 root         (0) root         (0)     1115 2023-11-21 19:30:34.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_3.py
--rwxrwxrwx   0 root         (0) root         (0)      470 2023-11-26 02:09:05.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_sci_note_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/fraction_point/
--rwxrwxrwx   0 root         (0) root         (0)      170 2023-12-10 03:06:16.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/fraction_point/fraction_point.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/integer/
--rwxrwxrwx   0 root         (0) root         (0)      560 2023-11-18 02:07:34.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/integer/status_string_is_integer.py
--rwxrwxrwx   0 root         (0) root         (0)      368 2023-11-18 02:05:23.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/integer/string_is_integer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/percentage/
--rwxrwxrwx   0 root         (0) root         (0)      951 2023-11-21 19:30:01.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/percentage/from_fraction.py
--rwxrwxrwx   0 root         (0) root         (0)      553 2023-11-18 02:34:50.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/percentage/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/
--rwxrwxrwx   0 root         (0) root         (0)     2211 2024-02-26 21:02:23.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/_status/
--rwxrwxrwx   0 root         (0) root         (0)     3224 2024-02-26 21:13:28.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py
--rwxrwxrwx   0 root         (0) root         (0)      612 2024-02-26 21:07:29.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/sci_note.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)      644 2024-02-26 21:07:36.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)     1342 2024-02-26 21:09:10.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note_2/
--rwxrwxrwx   0 root         (0) root         (0)      363 2024-03-29 23:32:14.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note_2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      936 2024-02-26 21:51:34.000000 apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note_2/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/temperature/
--rwxrwxrwx   0 root         (0) root         (0)       58 2023-10-24 22:59:09.000000 apoplast-1.1.1/structures/modules/apoplast/measures/temperature/temperature.r.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/volume/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/volume/swap/
--rwxrwxrwx   0 root         (0) root         (0)     2205 2023-11-18 04:45:15.000000 apoplast-1.1.1/structures/modules/apoplast/measures/volume/swap/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1666 2023-11-18 04:42:26.000000 apoplast-1.1.1/structures/modules/apoplast/measures/volume/swap/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      510 2023-10-19 17:30:50.000000 apoplast-1.1.1/structures/modules/apoplast/measures/volume/volume.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/measures/weight/
--rwxrwxrwx   0 root         (0) root         (0)      911 2023-11-18 02:37:48.000000 apoplast-1.1.1/structures/modules/apoplast/measures/weight/weight.r.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.451580 apoplast-1.1.1/structures/modules/apoplast/proposals/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/proposals/humans/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-16 03:24:46.000000 apoplast-1.1.1/structures/modules/apoplast/proposals/humans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/proposals/humans/_journal/
--rwxrwxrwx   0 root         (0) root         (0)      364 2023-11-18 01:10:16.000000 apoplast-1.1.1/structures/modules/apoplast/proposals/humans/_journal/vitamin e.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)      219 2023-11-18 02:14:35.000000 apoplast-1.1.1/structures/modules/apoplast/proposals/humans/people.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      207 2023-12-16 03:26:47.000000 apoplast-1.1.1/structures/modules/apoplast/proposals/proposals structure.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      958 2024-01-19 20:01:27.000000 apoplast-1.1.1/structures/modules/apoplast/proposals/proposals.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      200 2024-03-22 04:28:46.000000 apoplast-1.1.1/structures/modules/apoplast/room.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/
--rwxrwxrwx   0 root         (0) root         (0)      224 2023-11-17 23:54:21.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/FDA.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/
--rwxrwxrwx   0 root         (0) root         (0)      421 2023-11-22 20:41:38.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/journal.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-22 06:06:19.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/calcium.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/lipids/
--rwxrwxrwx   0 root         (0) root         (0)      216 2023-11-24 01:35:08.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/lipids/lipids.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/protein/
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-11-22 06:06:47.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/protein/protein.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)     1351 2023-11-18 00:49:44.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)      807 2023-11-18 00:12:47.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-11-24 01:36:24.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin c.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)     1298 2023-11-17 23:45:28.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-11-18 01:08:23.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin e.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/channel/
--rwxrwxrwx   0 root         (0) root         (0)      219 2023-11-16 23:54:05.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/channel/river.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      543 2024-02-04 19:20:12.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/forward channel.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      935 2023-11-24 02:38:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/structures.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.411580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/cautions/
--rwxrwxrwx   0 root         (0) root         (0)      102 2023-12-15 18:50:56.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.JSON
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-12-16 23:46:18.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/
--rwxrwxrwx   0 root         (0) root         (0)     3706 2023-11-25 18:53:45.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON
--rwxrwxrwx   0 root         (0) root         (0)     3955 2023-11-27 20:39:58.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON
--rwxrwxrwx   0 root         (0) root         (0)     3864 2023-12-15 19:16:15.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON
--rwxrwxrwx   0 root         (0) root         (0)     1643 2023-12-15 20:42:05.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/access.py
--rwxrwxrwx   0 root         (0) root         (0)      598 2023-12-15 20:11:06.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.411580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.455580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/list/
--rwxrwxrwx   0 root         (0) root         (0)      957 2024-03-11 03:50:37.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      425 2023-12-15 20:37:53.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/list/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek/
--rwxrwxrwx   0 root         (0) root         (0)     1040 2024-03-11 03:59:22.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1127 2024-03-11 03:56:08.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/
--rwxrwxrwx   0 root         (0) root         (0)      521 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/status_actual/
--rwxrwxrwx   0 root         (0) root         (0)      452 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.411580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/
--rwxrwxrwx   0 root         (0) root         (0)      994 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/
--rwxrwxrwx   0 root         (0) root         (0)     1160 2023-12-15 20:37:53.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/
--rwxrwxrwx   0 root         (0) root         (0)      735 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/
--rwxrwxrwx   0 root         (0) root         (0)      749 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-11-25 18:51:12.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/sculpt.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)      251 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.411580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/assertions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/assertions/one/
--rwxrwxrwx   0 root         (0) root         (0)      424 2023-12-15 22:29:15.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/assertions/one/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/assertions/recipe/
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/assertions/recipe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/assertions/
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/assertions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/
--rwxrwxrwx   0 root         (0) root         (0)     1030 2023-12-17 01:34:38.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      668 2023-12-17 01:36:56.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      603 2023-12-17 01:38:18.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/essential_is_story_1/
--rwxrwxrwx   0 root         (0) root         (0)      551 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      798 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      254 2023-11-23 22:33:02.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/grove.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/
--rwxrwxrwx   0 root         (0) root         (0)     4712 2024-03-31 22:07:23.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-11-26 03:02:03.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML
--rwxrwxrwx   0 root         (0) root         (0)     1055 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/measures/
--rwxrwxrwx   0 root         (0) root         (0)      222 2023-12-09 18:50:30.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/measures/measures.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/
--rwxrwxrwx   0 root         (0) root         (0)      176 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      164 2023-12-15 20:03:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/
--rwxrwxrwx   0 root         (0) root         (0)     2879 2023-12-17 01:45:25.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      542 2023-12-15 23:08:39.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-12-15 23:05:28.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py
--rwxrwxrwx   0 root         (0) root         (0)      696 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.459580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/print/
--rwxrwxrwx   0 root         (0) root         (0)     1424 2023-12-15 23:01:30.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/print/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek/
--rwxrwxrwx   0 root         (0) root         (0)     1235 2023-12-17 01:00:44.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      572 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_count/
--rwxrwxrwx   0 root         (0) root         (0)      469 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_count/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3891 2023-12-08 03:23:39.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON
--rwxrwxrwx   0 root         (0) root         (0)      833 2023-12-15 23:06:34.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/
--rwxrwxrwx   0 root         (0) root         (0)     1237 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      568 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/
--rwxrwxrwx   0 root         (0) root         (0)     1056 2023-12-17 00:41:11.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_uniter/
--rwxrwxrwx   0 root         (0) root         (0)      794 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      776 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/sort/
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/sort/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/
--rwxrwxrwx   0 root         (0) root         (0)      180 2023-11-23 19:14:43.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/grove prototype.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/
--rwxrwxrwx   0 root         (0) root         (0)     1903 2023-12-15 22:31:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/
--rwxrwxrwx   0 root         (0) root         (0)      918 2023-12-15 20:35:42.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      536 2023-12-15 20:35:49.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      624 2023-12-15 20:36:03.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py
--rwxrwxrwx   0 root         (0) root         (0)      966 2023-12-15 20:42:05.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/print/
--rwxrwxrwx   0 root         (0) root         (0)     1389 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/
--rwxrwxrwx   0 root         (0) root         (0)      719 2023-12-15 20:36:28.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      529 2023-12-15 20:36:38.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      615 2023-12-15 20:36:51.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/ingredient/
--rwxrwxrwx   0 root         (0) root         (0)      692 2023-11-24 00:44:01.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)     1012 2024-03-29 20:58:01.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/ingredient scan.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/
--rwxrwxrwx   0 root         (0) root         (0)     4982 2024-03-29 23:50:17.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-11-27 20:33:45.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/add_measured_ingredient.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.463580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/
--rwxrwxrwx   0 root         (0) root         (0)     1082 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/
--rwxrwxrwx   0 root         (0) root         (0)     2212 2024-03-29 23:53:03.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     2200 2024-03-29 23:53:32.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/
--rwxrwxrwx   0 root         (0) root         (0)     3932 2024-03-29 23:52:06.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/
--rwxrwxrwx   0 root         (0) root         (0)     1136 2023-12-15 23:10:16.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      375 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/measures.py
--rwxrwxrwx   0 root         (0) root         (0)      324 2023-12-15 23:11:21.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)      812 2023-12-15 23:12:52.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/calculate_portions/
--rwxrwxrwx   0 root         (0) root         (0)     3271 2024-03-30 21:01:29.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/cultivate/
--rwxrwxrwx   0 root         (0) root         (0)     1644 2023-12-17 01:39:47.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/cultivate/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3497 2024-03-29 23:49:19.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/land.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.415580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/aggregate/
--rwxrwxrwx   0 root         (0) root         (0)      439 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/aggregate/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      614 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/sums/
--rwxrwxrwx   0 root         (0) root         (0)     2794 2024-03-29 23:51:11.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/sums/status/
--rwxrwxrwx   0 root         (0) root         (0)      407 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/sums/status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/
--rwxrwxrwx   0 root         (0) root         (0)     2290 2023-12-15 20:50:14.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/courses/
--rwxrwxrwx   0 root         (0) root         (0)      551 2023-12-15 20:50:37.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py
--rwxrwxrwx   0 root         (0) root         (0)      950 2023-11-27 02:53:23.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)     2582 2024-03-30 00:06:40.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     2923 2024-03-30 00:05:43.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py
--rwxrwxrwx   0 root         (0) root         (0)     1039 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.415580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/
--rwxrwxrwx   0 root         (0) root         (0)     1313 2024-03-30 00:01:21.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1477 2024-03-30 00:13:11.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1475 2024-03-30 00:08:56.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/status_2.py
--rwxrwxrwx   0 root         (0) root         (0)     1319 2024-03-30 00:09:21.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/status_3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/multiply/
--rwxrwxrwx   0 root         (0) root         (0)      776 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/multiply/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1728 2023-12-15 20:03:33.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/multiply/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/selected_unit/
--rwxrwxrwx   0 root         (0) root         (0)      275 2023-11-26 22:20:49.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/selected_unit/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2023-12-15 19:52:46.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/names.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.467580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/
--rwxrwxrwx   0 root         (0) root         (0)     1200 2024-03-07 04:13:37.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.415580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/
--rwxrwxrwx   0 root         (0) root         (0)     1207 2023-12-16 05:02:53.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/
--rwxrwxrwx   0 root         (0) root         (0)     2315 2024-03-30 00:02:05.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py
--rwxrwxrwx   0 root         (0) root         (0)     6474 2024-03-30 00:18:21.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     3862 2024-03-30 00:17:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py
--rwxrwxrwx   0 root         (0) root         (0)     2473 2024-02-04 20:24:03.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/
--rwxrwxrwx   0 root         (0) root         (0)   215864 2024-03-31 22:08:37.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON
--rwxrwxrwx   0 root         (0) root         (0)     2506 2024-03-11 02:02:18.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/
--rwxrwxrwx   0 root         (0) root         (0)   131410 2024-03-31 22:08:36.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON
--rwxrwxrwx   0 root         (0) root         (0)     1863 2024-03-11 01:24:01.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/
--rwxrwxrwx   0 root         (0) root         (0)   127961 2024-03-31 22:08:37.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON
--rwxrwxrwx   0 root         (0) root         (0)     1755 2023-12-16 05:04:27.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py
--rwxrwxrwx   0 root         (0) root         (0)     1606 2023-12-16 05:04:52.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/assertions/
--rwxrwxrwx   0 root         (0) root         (0)     2844 2023-12-16 05:01:05.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.415580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/calculate/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/
--rwxrwxrwx   0 root         (0) root         (0)      471 2023-12-15 22:41:08.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/calculate/slice/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-09 18:24:24.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/calculate/slice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/cautionary_ingredients/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-16 04:48:59.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/cautionary_ingredients/formulate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/
--rwxrwxrwx   0 root         (0) root         (0)     3439 2024-03-07 04:11:50.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py
--rwxrwxrwx   0 root         (0) root         (0)     1876 2023-11-26 22:19:07.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML
--rwxrwxrwx   0 root         (0) root         (0)      968 2024-02-04 19:27:25.000000 apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/natures/
--rwxrwxrwx   0 root         (0) root         (0)      101 2023-11-17 21:50:38.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      371 2023-11-21 23:21:15.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/assertions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.471580 apoplast-1.1.1/structures/modules/apoplast/shows/natures/measured_ingredient/
--rwxrwxrwx   0 root         (0) root         (0)       84 2023-11-22 02:42:38.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/measured_ingredient/assertions.py
--rwxrwxrwx   0 root         (0) root         (0)      332 2024-03-29 20:56:02.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/nature.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/nature/
--rwxrwxrwx   0 root         (0) root         (0)     3867 2023-11-28 02:28:19.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/nature/nature.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-11-25 23:54:11.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/nature: form.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)      139 2023-11-28 02:28:25.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/pattern.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)      115 2023-11-16 20:19:44.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/pattern: measured ingredients.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-11-16 20:58:52.000000 apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/pattern: unmeasured ingredients.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)      843 2024-03-31 01:49:28.000000 apoplast-1.1.1/structures/modules/apoplast/shows/shows.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/
--rw-rw-r--   0 root         (0) root         (0)     1523 2024-03-31 02:20:59.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/grove.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/info/
--rw-rw-r--   0 root         (0) root         (0)       58 2024-03-31 02:19:44.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/info/info.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/measures/
--rw-rw-r--   0 root         (0) root         (0)       73 2024-03-31 02:21:06.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/measures/measures.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/natures/
--rw-rw-r--   0 root         (0) root         (0)       59 2024-03-31 02:21:27.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/natures/natures.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/unites/
--rw-rw-r--   0 root         (0) root         (0)     1508 2024-03-31 02:23:11.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/unites/unites.S.HTML
--rw-rw-r--   0 root         (0) root         (0)      131 2024-03-31 02:19:06.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/land.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/measures/
--rw-rw-r--   0 root         (0) root         (0)      459 2024-03-31 02:16:52.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/measures/measures.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/natures/
--rw-rw-r--   0 root         (0) root         (0)      412 2024-03-31 02:09:01.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/natures/natures.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/measured_ingredients/
--rw-rw-r--   0 root         (0) root         (0)      405 2024-03-31 01:56:16.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/measured_ingredients/measured_ingredients.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/measures/
--rw-rw-r--   0 root         (0) root         (0)     1018 2024-03-31 01:54:44.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/measures/measures.S.HTML
--rw-rw-r--   0 root         (0) root         (0)      426 2024-03-31 01:58:10.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/nature.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/unmeasured_ingredients/
--rw-rw-r--   0 root         (0) root         (0)      294 2024-03-31 01:56:52.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/unmeasured_ingredients/UI.S.HTML
--rw-rw-r--   0 root         (0) root         (0)      106 2024-03-31 01:57:56.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/shows.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast/shows_v2/treasure/
--rw-rw-r--   0 root         (0) root         (0)      232 2024-03-31 01:52:52.000000 apoplast-1.1.1/structures/modules/apoplast/shows_v2/treasure/treasure.S.HTML
--rwxrwxrwx   0 root         (0) root         (0)       63 2023-11-16 19:27:45.000000 apoplast-1.1.1/structures/modules/apoplast/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 22:19:14.475580 apoplast-1.1.1/structures/modules/apoplast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1024 2024-03-31 22:19:14.000000 apoplast-1.1.1/structures/modules/apoplast.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    28396 2024-03-31 22:19:14.000000 apoplast-1.1.1/structures/modules/apoplast.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-03-31 22:19:14.000000 apoplast-1.1.1/structures/modules/apoplast.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-03-31 22:19:14.000000 apoplast-1.1.1/structures/modules/apoplast.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2024-03-31 22:19:14.000000 apoplast-1.1.1/structures/modules/apoplast.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-09 20:17:14.238623 apoplast-1.1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      970 2024-04-09 20:16:05.000000 apoplast-1.1.2/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      550 2024-03-30 21:10:34.000000 apoplast-1.1.2/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:17:14.238623 apoplast-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.070625 apoplast-1.1.2/venues/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.070625 apoplast-1.1.2/venues/stages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.094624 apoplast-1.1.2/venues/stages/apoplast/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.094624 apoplast-1.1.2/venues/stages/apoplast/-license/
+-rwxrwxrwx   0 root         (0) root         (0)      427 2024-02-04 21:45:08.000000 apoplast-1.1.2/venues/stages/apoplast/-license/license.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.098624 apoplast-1.1.2/venues/stages/apoplast/-license/list/
+-rwxrwxrwx   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 apoplast-1.1.2/venues/stages/apoplast/-license/list/gpl-3.0-standalone.html
+-rwxrwxrwx   0 root         (0) root         (0)      112 2024-02-04 21:44:43.000000 apoplast-1.1.2/venues/stages/apoplast/-license/list/vegan.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       78 2024-04-08 03:43:18.000000 apoplast-1.1.2/venues/stages/apoplast/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.098624 apoplast-1.1.2/venues/stages/apoplast/__itinerary/
+-rwxrwxrwx   0 root         (0) root         (0)      595 2024-04-08 03:40:23.000000 apoplast-1.1.2/venues/stages/apoplast/__itinerary/apoplast.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.098624 apoplast-1.1.2/venues/stages/apoplast/__itinerary/book/
+-rwxrwxrwx   0 root         (0) root         (0)      405 2024-04-08 03:26:57.000000 apoplast-1.1.2/venues/stages/apoplast/__itinerary/book/Vitamin B.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       63 2024-04-08 03:27:04.000000 apoplast-1.1.2/venues/stages/apoplast/__itinerary/book/Vitamin K.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.098624 apoplast-1.1.2/venues/stages/apoplast/__status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.098624 apoplast-1.1.2/venues/stages/apoplast/__status/db/
+-rwxrwxrwx   0 root         (0) root         (0)  6494696 2024-04-09 20:16:48.000000 apoplast-1.1.2/venues/stages/apoplast/__status/db/records.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.106624 apoplast-1.1.2/venues/stages/apoplast/__status/db_API/
+-rwxrwxrwx   0 root         (0) root         (0)    30367 2024-02-04 22:01:04.000000 apoplast-1.1.2/venues/stages/apoplast/__status/db_API/records.json
+-rwxrwxrwx   0 root         (0) root         (0)     1265 2024-04-09 20:03:54.000000 apoplast-1.1.2/venues/stages/apoplast/__status/status.proc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1209 2024-03-30 21:08:29.000000 apoplast-1.1.2/venues/stages/apoplast/__status/status_API.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/_ellipses/
+-rwxrwxrwx   0 root         (0) root         (0)      424 2024-03-30 22:53:59.000000 apoplast-1.1.2/venues/stages/apoplast/_ellipses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.070625 apoplast-1.1.2/venues/stages/apoplast/_interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/_interfaces/clique/
+-rwxrwxrwx   0 root         (0) root         (0)      394 2024-04-09 15:54:03.000000 apoplast-1.1.2/venues/stages/apoplast/_interfaces/clique/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/_interfaces/clique/group/
+-rwxrwxrwx   0 root         (0) root         (0)      297 2024-04-08 03:41:14.000000 apoplast-1.1.2/venues/stages/apoplast/_interfaces/clique/group/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/_interfaces/sanic/
+-rwxrwxrwx   0 root         (0) root         (0)     1161 2024-04-08 04:51:52.000000 apoplast-1.1.2/venues/stages/apoplast/_interfaces/sanic/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2024-04-08 04:37:31.000000 apoplast-1.1.2/venues/stages/apoplast/_interfaces/sanic/off.py
+-rwxrwxrwx   0 root         (0) root         (0)      500 2024-04-08 04:45:34.000000 apoplast-1.1.2/venues/stages/apoplast/_interfaces/sanic/on.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/_variables/
+-rwxrwxrwx   0 root         (0) root         (0)     1238 2024-04-09 16:42:39.000000 apoplast-1.1.2/venues/stages/apoplast/_variables/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/clouds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/clouds/affiliates_Amazon/
+-rwxrwxrwx   0 root         (0) root         (0)      118 2024-02-04 18:06:33.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/affiliates_Amazon/affiliates.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      111 2024-03-31 01:44:52.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/clouds.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.110624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2024-03-31 22:06:11.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.114624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/
+-rwxrwxrwx   0 root         (0) root         (0)      429 2023-10-29 21:44:17.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/branded.py
+-rwxrwxrwx   0 root         (0) root         (0)      264 2023-11-17 17:51:13.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/foundational.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.114624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/
+-rwxrwxrwx   0 root         (0) root         (0)      419 2023-11-17 00:19:37.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/API_status_branded_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      465 2023-11-17 00:19:37.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/API_status_foundational_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      370 2023-11-16 23:17:45.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.114624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     1009 2023-11-22 01:31:31.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.118624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/
+-rwxrwxrwx   0 root         (0) root         (0)    37079 2023-12-09 20:38:41.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
+-rwxrwxrwx   0 root         (0) root         (0)    37079 2023-11-22 01:40:03.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     7242 2023-10-19 22:27:22.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     8522 2023-10-12 21:13:07.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON
+-rwxrwxrwx   0 root         (0) root         (0)    33964 2023-11-22 01:38:38.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.122624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/
+-rwxrwxrwx   0 root         (0) root         (0)    17926 2023-09-25 16:28:17.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON
+-rwxrwxrwx   0 root         (0) root         (0)      104 2023-11-26 02:04:47.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/problems.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)    10678 2023-11-22 01:32:41.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON
+-rwxrwxrwx   0 root         (0) root         (0)    10670 2023-10-24 03:17:57.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.122624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/foundational/
+-rwxrwxrwx   0 root         (0) root         (0)   189146 2023-10-12 22:00:16.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
+-rwxrwxrwx   0 root         (0) root         (0)      255 2023-11-17 18:04:07.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/mergers.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       88 2023-11-22 01:27:20.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/priorities.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      457 2023-12-09 23:06:15.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      614 2023-12-15 19:53:16.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/food.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.074625 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.126624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/foodNutrient/
+-rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-22 04:54:08.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/foodNutrient/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.126624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/labelNutrient/
+-rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-22 02:45:04.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/labelNutrient/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.126624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/
+-rwxrwxrwx   0 root         (0) root         (0)     1783 2023-11-23 18:42:09.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      583 2023-11-22 00:01:06.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/
+-rwxrwxrwx   0 root         (0) root         (0)     4126 2023-11-22 20:58:41.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1229 2023-11-22 20:47:39.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      877 2023-11-22 20:23:41.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/
+-rwxrwxrwx   0 root         (0) root         (0)      415 2023-11-22 20:49:55.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1374 2023-11-22 20:23:29.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-01-08 21:02:44.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/
+-rwxrwxrwx   0 root         (0) root         (0)     2606 2024-02-04 20:24:03.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1610 2023-12-09 20:39:39.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1236 2023-12-17 01:49:13.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2412474.py
+-rwxrwxrwx   0 root         (0) root         (0)     1078 2023-12-17 00:42:09.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_3.py
+-rwxrwxrwx   0 root         (0) root         (0)      812 2023-12-09 20:39:39.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-12-15 23:15:41.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/energy/
+-rwxrwxrwx   0 root         (0) root         (0)        4 2023-11-26 00:02:13.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/energy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.130624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/
+-rwxrwxrwx   0 root         (0) root         (0)     3116 2023-12-17 00:12:42.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.134624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/
+-rwxrwxrwx   0 root         (0) root         (0)     4031 2023-11-26 01:50:19.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1231 2024-03-31 22:06:29.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/status_mass_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1159 2023-11-26 00:30:32.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/status_volume_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.134624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/
+-rwxrwxrwx   0 root         (0) root         (0)     1427 2023-11-27 04:58:37.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.134624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/
+-rwxrwxrwx   0 root         (0) root         (0)     1676 2023-11-26 01:00:29.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1875 2024-03-31 22:07:48.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1579 2023-11-26 01:00:16.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.134624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/
+-rwxrwxrwx   0 root         (0) root         (0)     2077 2023-11-26 01:09:26.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.134624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/
+-rwxrwxrwx   0 root         (0) root         (0)     1224 2023-11-26 01:10:07.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.134624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/
+-rwxrwxrwx   0 root         (0) root         (0)     1494 2023-11-26 23:54:17.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.138624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/
+-rwxrwxrwx   0 root         (0) root         (0)     1389 2024-03-29 23:33:34.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.138624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/
+-rwxrwxrwx   0 root         (0) root         (0)      622 2023-11-26 02:01:26.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py
+-rwxrwxrwx   0 root         (0) root         (0)      468 2023-11-22 04:50:10.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/label_nutrient.py
+-rwxrwxrwx   0 root         (0) root         (0)      503 2023-11-26 00:52:57.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-11-22 20:45:42.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.138624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/
+-rwxrwxrwx   0 root         (0) root         (0)      485 2023-11-26 01:53:47.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.138624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/
+-rwxrwxrwx   0 root         (0) root         (0)     2092 2023-11-24 04:45:08.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      687 2023-11-26 00:51:56.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-11-26 00:49:48.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.138624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/
+-rwxrwxrwx   0 root         (0) root         (0)      863 2023-11-23 23:49:12.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.138624 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/
+-rwxrwxrwx   0 root         (0) root         (0)      575 2023-11-23 23:46:06.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1019 2023-11-23 23:47:00.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/goodness_certifications/
+-rwxrwxrwx   0 root         (0) root         (0)     1791 2024-03-31 18:10:18.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/goodness_certifications/certifications.py
+-rwxrwxrwx   0 root         (0) root         (0)      641 2024-03-31 20:50:04.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/goodness_certifications/vegan.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/
+-rwxrwxrwx   0 root         (0) root         (0)     1046 2024-03-31 02:07:55.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/NIH.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/
+-rwxrwxrwx   0 root         (0) root         (0)     1137 2024-03-31 22:06:43.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1087 2023-10-25 01:29:58.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/assertions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/status/
+-rwxrwxrwx   0 root         (0) root         (0)      392 2023-11-17 00:20:01.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/status/API_status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      316 2023-10-25 01:28:37.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/
+-rwxrwxrwx   0 root         (0) root         (0)      848 2023-11-27 22:36:33.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/
+-rwxrwxrwx   0 root         (0) root         (0)    44597 2023-10-13 17:10:19.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/other/
+-rwxrwxrwx   0 root         (0) root         (0)    22180 2023-10-25 17:22:33.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.142624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder/
+-rwxrwxrwx   0 root         (0) root         (0)     6430 2023-10-13 17:09:44.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON
+-rwxrwxrwx   0 root         (0) root         (0)    72594 2023-10-25 01:46:01.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.146624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/
+-rwxrwxrwx   0 root         (0) root         (0)    57378 2023-10-13 17:05:59.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.146624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/
+-rwxrwxrwx   0 root         (0) root         (0)    22710 2023-10-13 17:08:42.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON
+-rwxrwxrwx   0 root         (0) root         (0)    43725 2023-10-13 17:08:08.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.146624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/
+-rwxrwxrwx   0 root         (0) root         (0)     7107 2023-10-13 17:07:29.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.078625 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.146624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/
+-rwxrwxrwx   0 root         (0) root         (0)       98 2023-11-27 03:46:15.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-11-27 04:24:46.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      923 2023-11-27 04:25:24.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/servingSizeUnit/
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-11-27 04:49:39.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/servingSizeUnit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/
+-rwxrwxrwx   0 root         (0) root         (0)     4087 2024-03-31 22:07:01.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.078625 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/
+-rwxrwxrwx   0 root         (0) root         (0)      730 2023-11-27 22:52:02.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/
+-rwxrwxrwx   0 root         (0) root         (0)     1580 2024-03-11 02:00:19.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py
+-rwxrwxrwx   0 root         (0) root         (0)   136857 2024-04-09 20:16:48.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/
+-rwxrwxrwx   0 root         (0) root         (0)   100726 2024-04-09 20:16:48.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON
+-rwxrwxrwx   0 root         (0) root         (0)      762 2024-03-11 02:02:48.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/
+-rwxrwxrwx   0 root         (0) root         (0)    28773 2024-04-09 20:16:47.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON
+-rwxrwxrwx   0 root         (0) root         (0)      748 2023-12-19 18:33:07.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.150624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)     2753 2023-12-15 23:31:38.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.154624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2024-03-30 21:02:16.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      832 2023-11-27 20:26:53.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      281 2023-11-27 20:27:05.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients_priorities.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.154624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/
+-rwxrwxrwx   0 root         (0) root         (0)      323 2023-11-27 04:41:57.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.154624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/
+-rwxrwxrwx   0 root         (0) root         (0)      676 2023-11-27 23:18:44.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      510 2023-11-22 19:45:00.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/status_other_214893.py
+-rwxrwxrwx   0 root         (0) root         (0)      512 2023-11-25 23:13:17.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/form.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.078625 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.154624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/
+-rwxrwxrwx   0 root         (0) root         (0)     3759 2023-11-27 23:36:21.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 22:52:26.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1841 2024-04-09 20:04:26.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py
+-rwxrwxrwx   0 root         (0) root         (0)     1711 2023-11-27 23:47:05.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/
+-rwxrwxrwx   0 root         (0) root         (0)     3210 2023-11-27 23:13:13.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2023-11-27 23:17:35.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-11-22 18:01:32.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      818 2023-11-22 19:42:51.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py
+-rwxrwxrwx   0 root         (0) root         (0)      903 2023-11-22 19:46:12.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py
+-rwxrwxrwx   0 root         (0) root         (0)     1333 2023-11-22 20:15:00.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py
+-rwxrwxrwx   0 root         (0) root         (0)      701 2023-11-22 20:21:05.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py
+-rwxrwxrwx   0 root         (0) root         (0)      725 2023-11-22 19:30:39.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/
+-rwxrwxrwx   0 root         (0) root         (0)     4631 2024-03-11 02:07:04.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/
+-rwxrwxrwx   0 root         (0) root         (0)     1687 2024-03-11 02:13:24.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.078625 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/mass/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 05:04:38.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/mass/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1514 2024-03-11 01:32:01.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)     1656 2024-03-30 21:01:47.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/
+-rwxrwxrwx   0 root         (0) root         (0)      826 2024-03-11 02:03:57.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py
+-rwxrwxrwx   0 root         (0) root         (0)      561 2023-11-27 05:48:16.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.158624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/
+-rwxrwxrwx   0 root         (0) root         (0)     1116 2023-11-27 05:48:52.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      657 2023-11-27 05:50:29.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/
+-rwxrwxrwx   0 root         (0) root         (0)      511 2023-11-27 18:44:30.000000 apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/
+-rwxrwxrwx   0 root         (0) root         (0)      233 2024-04-09 15:54:11.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/clique.py
+-rwxrwxrwx   0 root         (0) root         (0)       96 2024-04-08 03:49:12.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/data_nodes.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/
+-rwxrwxrwx   0 root         (0) root         (0)      554 2024-04-09 16:42:34.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/connect.py
+-rwxrwxrwx   0 root         (0) root         (0)      632 2024-04-08 04:23:34.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/off.py
+-rwxrwxrwx   0 root         (0) root         (0)     2117 2024-04-09 20:12:27.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/on.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/saves/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:30:53.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/saves/dump.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 04:30:49.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/saves/export.py
+-rwxrwxrwx   0 root         (0) root         (0)     1701 2024-04-09 19:46:45.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/DB/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/__itinerary/
+-rwxrwxrwx   0 root         (0) root         (0)      454 2024-03-31 01:44:39.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/__itinerary/itinerary.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/cautionary_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)      118 2024-03-31 03:53:00.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/cautionary_ingredients/cautionary_ingredients.1.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/
+-rwxrwxrwx   0 root         (0) root         (0)     5140 2024-03-31 03:54:30.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/essential_nutrients.1.json
+-rwxrwxrwx   0 root         (0) root         (0)      481 2024-03-31 03:53:37.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/exports.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       35 2024-04-09 20:14:48.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/save.py
+-rwxrwxrwx   0 root         (0) root         (0)     1104 2024-04-09 19:46:23.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/clique.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.162624 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.166623 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/_land/
+-rwxrwxrwx   0 root         (0) root         (0)      796 2024-03-31 03:43:31.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/_land/insert_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.166623 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)      170 2024-04-08 03:47:20.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/cautionary_ingredients.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.166623 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/collection/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2024-03-31 03:51:33.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/collection/export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.166623 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/document/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 03:46:10.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/document/insert.py
+-rwxrwxrwx   0 root         (0) root         (0)       27 2024-04-08 03:47:50.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/collections.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.166623 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/essential_nutrients/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 03:51:29.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/essential_nutrients/export.py
+-rwxrwxrwx   0 root         (0) root         (0)     1523 2024-04-08 03:56:03.000000 apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/ingredients.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-03-31 22:10:20.000000 apoplast-1.1.2/venues/stages/apoplast/emojis.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.166623 apoplast-1.1.2/venues/stages/apoplast/insure/
+-rwxrwxrwx   0 root         (0) root         (0)     1085 2023-11-27 23:25:39.000000 apoplast-1.1.2/venues/stages/apoplast/insure/equalities.py
+-rwxrwxrwx   0 root         (0) root         (0)      234 2023-11-22 18:56:47.000000 apoplast-1.1.2/venues/stages/apoplast/insure/equality.py
+-rwxrwxrwx   0 root         (0) root         (0)      729 2023-11-27 01:34:09.000000 apoplast-1.1.2/venues/stages/apoplast/insure/override_print.py
+-rwxrwxrwx   0 root         (0) root         (0)      374 2023-11-22 19:22:12.000000 apoplast-1.1.2/venues/stages/apoplast/insure/status_equalitites_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.082625 apoplast-1.1.2/venues/stages/apoplast/measures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.170623 apoplast-1.1.2/venues/stages/apoplast/measures/_interpret/
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-10-24 19:09:48.000000 apoplast-1.1.2/venues/stages/apoplast/measures/_interpret/interpret.r.html
+-rwxrwxrwx   0 root         (0) root         (0)      670 2023-11-22 03:00:29.000000 apoplast-1.1.2/venues/stages/apoplast/measures/_interpret/status_unit_kind.py
+-rwxrwxrwx   0 root         (0) root         (0)     1678 2023-11-27 23:51:26.000000 apoplast-1.1.2/venues/stages/apoplast/measures/_interpret/unit_kind.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.170623 apoplast-1.1.2/venues/stages/apoplast/measures/biological_activity/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-22 02:29:15.000000 apoplast-1.1.2/venues/stages/apoplast/measures/biological_activity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.170623 apoplast-1.1.2/venues/stages/apoplast/measures/electric_current/
+-rwxrwxrwx   0 root         (0) root         (0)       59 2024-02-26 21:23:18.000000 apoplast-1.1.2/venues/stages/apoplast/measures/electric_current/electric_current.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.170623 apoplast-1.1.2/venues/stages/apoplast/measures/energy/
+-rwxrwxrwx   0 root         (0) root         (0)     1142 2023-11-18 02:03:26.000000 apoplast-1.1.2/venues/stages/apoplast/measures/energy/energy.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.170623 apoplast-1.1.2/venues/stages/apoplast/measures/energy/swap/
+-rwxrwxrwx   0 root         (0) root         (0)     1174 2023-11-27 05:11:29.000000 apoplast-1.1.2/venues/stages/apoplast/measures/energy/swap/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      386 2023-11-22 03:06:00.000000 apoplast-1.1.2/venues/stages/apoplast/measures/energy/swap/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.170623 apoplast-1.1.2/venues/stages/apoplast/measures/length/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-11-18 02:08:27.000000 apoplast-1.1.2/venues/stages/apoplast/measures/length/length.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/mass/
+-rwxrwxrwx   0 root         (0) root         (0)       95 2023-09-10 01:33:12.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass/e_note.py
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-10-24 23:00:23.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass/mass.r.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/mass/swap/
+-rwxrwxrwx   0 root         (0) root         (0)     2329 2023-11-27 23:53:01.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass/swap/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1153 2023-11-21 20:24:21.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass/swap/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     2419 2023-10-25 22:32:32.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass/system international.r.html
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-10-24 19:13:36.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass/us customary.r.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-11-18 02:19:07.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      342 2023-11-18 02:17:02.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      861 2023-11-18 02:32:14.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/jargon.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     2242 2023-12-09 18:56:13.000000 apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/mass equivalents.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.082625 apoplast-1.1.2/venues/stages/apoplast/measures/number/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.082625 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/
+-rwxrwxrwx   0 root         (0) root         (0)     2431 2024-02-26 20:25:18.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1428 2023-11-26 02:08:37.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      901 2023-11-21 19:30:34.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1115 2023-11-21 19:30:34.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_3.py
+-rwxrwxrwx   0 root         (0) root         (0)      470 2023-11-26 02:09:05.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_sci_note_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/number/fraction_point/
+-rwxrwxrwx   0 root         (0) root         (0)      170 2023-12-10 03:06:16.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/fraction_point/fraction_point.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.174623 apoplast-1.1.2/venues/stages/apoplast/measures/number/integer/
+-rwxrwxrwx   0 root         (0) root         (0)      560 2023-11-18 02:07:34.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/integer/status_string_is_integer.py
+-rwxrwxrwx   0 root         (0) root         (0)      368 2023-11-18 02:05:23.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/integer/string_is_integer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.178623 apoplast-1.1.2/venues/stages/apoplast/measures/number/percentage/
+-rwxrwxrwx   0 root         (0) root         (0)      951 2023-11-21 19:30:01.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/percentage/from_fraction.py
+-rwxrwxrwx   0 root         (0) root         (0)      553 2023-11-18 02:34:50.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/percentage/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.178623 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/
+-rwxrwxrwx   0 root         (0) root         (0)     2211 2024-02-26 21:02:23.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.178623 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/_status/
+-rwxrwxrwx   0 root         (0) root         (0)     3224 2024-02-26 21:13:28.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      612 2024-02-26 21:07:29.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/sci_note.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      644 2024-02-26 21:07:36.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     1342 2024-02-26 21:09:10.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.178623 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note_2/
+-rwxrwxrwx   0 root         (0) root         (0)      363 2024-03-29 23:32:14.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note_2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      936 2024-02-26 21:51:34.000000 apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note_2/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.178623 apoplast-1.1.2/venues/stages/apoplast/measures/temperature/
+-rwxrwxrwx   0 root         (0) root         (0)       58 2023-10-24 22:59:09.000000 apoplast-1.1.2/venues/stages/apoplast/measures/temperature/temperature.r.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.182623 apoplast-1.1.2/venues/stages/apoplast/measures/volume/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.182623 apoplast-1.1.2/venues/stages/apoplast/measures/volume/swap/
+-rwxrwxrwx   0 root         (0) root         (0)     2205 2023-11-18 04:45:15.000000 apoplast-1.1.2/venues/stages/apoplast/measures/volume/swap/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1666 2023-11-18 04:42:26.000000 apoplast-1.1.2/venues/stages/apoplast/measures/volume/swap/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      510 2023-10-19 17:30:50.000000 apoplast-1.1.2/venues/stages/apoplast/measures/volume/volume.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.182623 apoplast-1.1.2/venues/stages/apoplast/measures/weight/
+-rwxrwxrwx   0 root         (0) root         (0)      911 2023-11-18 02:37:48.000000 apoplast-1.1.2/venues/stages/apoplast/measures/weight/weight.r.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.182623 apoplast-1.1.2/venues/stages/apoplast/proposals/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.182623 apoplast-1.1.2/venues/stages/apoplast/proposals/humans/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-16 03:24:46.000000 apoplast-1.1.2/venues/stages/apoplast/proposals/humans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.182623 apoplast-1.1.2/venues/stages/apoplast/proposals/humans/_journal/
+-rwxrwxrwx   0 root         (0) root         (0)      364 2023-11-18 01:10:16.000000 apoplast-1.1.2/venues/stages/apoplast/proposals/humans/_journal/vitamin e.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      219 2023-11-18 02:14:35.000000 apoplast-1.1.2/venues/stages/apoplast/proposals/humans/people.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      207 2023-12-16 03:26:47.000000 apoplast-1.1.2/venues/stages/apoplast/proposals/proposals structure.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      958 2024-01-19 20:01:27.000000 apoplast-1.1.2/venues/stages/apoplast/proposals/proposals.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      338 2024-04-08 03:36:01.000000 apoplast-1.1.2/venues/stages/apoplast/room.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.186623 apoplast-1.1.2/venues/stages/apoplast/shows/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.186623 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/
+-rwxrwxrwx   0 root         (0) root         (0)      224 2023-11-17 23:54:21.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/FDA.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.186623 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/
+-rwxrwxrwx   0 root         (0) root         (0)      421 2023-11-22 20:41:38.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/journal.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.190623 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-11-22 06:06:19.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/calcium.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.190623 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/lipids/
+-rwxrwxrwx   0 root         (0) root         (0)      216 2023-11-24 01:35:08.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/lipids/lipids.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.190623 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/protein/
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-11-22 06:06:47.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/protein/protein.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2023-11-18 00:49:44.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      807 2023-11-18 00:12:47.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-11-24 01:36:24.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin c.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     1298 2023-11-17 23:45:28.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-11-18 01:08:23.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin e.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.190623 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/channel/
+-rwxrwxrwx   0 root         (0) root         (0)      219 2023-11-16 23:54:05.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/channel/river.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      543 2024-02-04 19:20:12.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/forward channel.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      935 2023-11-24 02:38:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/structures.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.190623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.086624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/
+-rwxrwxrwx   0 root         (0) root         (0)      102 2023-12-15 18:50:56.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.JSON
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-12-16 23:46:18.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/
+-rwxrwxrwx   0 root         (0) root         (0)     3706 2023-11-25 18:53:45.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     3955 2023-11-27 20:39:58.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     3864 2023-12-15 19:16:15.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     1643 2023-12-15 20:42:05.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/access.py
+-rwxrwxrwx   0 root         (0) root         (0)      598 2023-12-15 20:11:06.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.086624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/
+-rwxrwxrwx   0 root         (0) root         (0)      957 2024-03-11 03:50:37.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      425 2023-12-15 20:37:53.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/
+-rwxrwxrwx   0 root         (0) root         (0)     1040 2024-03-11 03:59:22.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1127 2024-03-11 03:56:08.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.194623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/
+-rwxrwxrwx   0 root         (0) root         (0)      521 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/status_actual/
+-rwxrwxrwx   0 root         (0) root         (0)      452 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.086624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/
+-rwxrwxrwx   0 root         (0) root         (0)      994 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/
+-rwxrwxrwx   0 root         (0) root         (0)     1160 2023-12-15 20:37:53.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/
+-rwxrwxrwx   0 root         (0) root         (0)      735 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/
+-rwxrwxrwx   0 root         (0) root         (0)      749 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-11-25 18:51:12.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/sculpt.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      251 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.086624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/assertions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.198623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/assertions/one/
+-rwxrwxrwx   0 root         (0) root         (0)      424 2023-12-15 22:29:15.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.202623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/assertions/recipe/
+-rwxrwxrwx   0 root         (0) root         (0)      504 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/assertions/recipe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.202623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.202623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.202623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/
+-rwxrwxrwx   0 root         (0) root         (0)     1030 2023-12-17 01:34:38.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      668 2023-12-17 01:36:56.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      603 2023-12-17 01:38:18.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.202623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/
+-rwxrwxrwx   0 root         (0) root         (0)      551 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      798 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      254 2023-11-23 22:33:02.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/grove.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.206623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/
+-rwxrwxrwx   0 root         (0) root         (0)     4712 2024-03-31 22:07:23.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-11-26 03:02:03.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     1055 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.206623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/measures/
+-rwxrwxrwx   0 root         (0) root         (0)      222 2023-12-09 18:50:30.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/measures/measures.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.206623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/
+-rwxrwxrwx   0 root         (0) root         (0)      176 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      164 2023-12-15 20:03:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.206623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/
+-rwxrwxrwx   0 root         (0) root         (0)     2879 2023-12-17 01:45:25.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      542 2023-12-15 23:08:39.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-12-15 23:05:28.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      696 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.206623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/print/
+-rwxrwxrwx   0 root         (0) root         (0)     1424 2023-12-15 23:01:30.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/print/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.206623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek/
+-rwxrwxrwx   0 root         (0) root         (0)     1235 2023-12-17 01:00:44.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      572 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/
+-rwxrwxrwx   0 root         (0) root         (0)      469 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3891 2023-12-08 03:23:39.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON
+-rwxrwxrwx   0 root         (0) root         (0)      833 2023-12-15 23:06:34.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/
+-rwxrwxrwx   0 root         (0) root         (0)     1237 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      568 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/
+-rwxrwxrwx   0 root         (0) root         (0)     1056 2023-12-17 00:41:11.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/
+-rwxrwxrwx   0 root         (0) root         (0)      794 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      776 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/sort/
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-11-23 19:14:43.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/grove prototype.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.210623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/
+-rwxrwxrwx   0 root         (0) root         (0)     1903 2023-12-15 22:31:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/
+-rwxrwxrwx   0 root         (0) root         (0)      918 2023-12-15 20:35:42.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      536 2023-12-15 20:35:49.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      624 2023-12-15 20:36:03.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py
+-rwxrwxrwx   0 root         (0) root         (0)      966 2023-12-15 20:42:05.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/
+-rwxrwxrwx   0 root         (0) root         (0)     1389 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/
+-rwxrwxrwx   0 root         (0) root         (0)      719 2023-12-15 20:36:28.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      529 2023-12-15 20:36:38.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      615 2023-12-15 20:36:51.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/ingredient/
+-rwxrwxrwx   0 root         (0) root         (0)      692 2023-11-24 00:44:01.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     1012 2024-03-29 20:58:01.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/ingredient scan.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/
+-rwxrwxrwx   0 root         (0) root         (0)     4982 2024-03-29 23:50:17.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-11-27 20:33:45.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/add_measured_ingredient.r.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/
+-rwxrwxrwx   0 root         (0) root         (0)     1082 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/
+-rwxrwxrwx   0 root         (0) root         (0)     2212 2024-03-29 23:53:03.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     2200 2024-03-29 23:53:32.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.214623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/
+-rwxrwxrwx   0 root         (0) root         (0)     3932 2024-03-29 23:52:06.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.218623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/
+-rwxrwxrwx   0 root         (0) root         (0)     1136 2023-12-15 23:10:16.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      375 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/measures.py
+-rwxrwxrwx   0 root         (0) root         (0)      324 2023-12-15 23:11:21.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)      812 2023-12-15 23:12:52.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.218623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/
+-rwxrwxrwx   0 root         (0) root         (0)     3271 2024-03-30 21:01:29.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.218623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/
+-rwxrwxrwx   0 root         (0) root         (0)     1644 2023-12-17 01:39:47.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3497 2024-03-29 23:49:19.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/land.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.090624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.218623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/
+-rwxrwxrwx   0 root         (0) root         (0)      439 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      614 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.218623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/
+-rwxrwxrwx   0 root         (0) root         (0)     2794 2024-03-29 23:51:11.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.218623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/status/
+-rwxrwxrwx   0 root         (0) root         (0)      407 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/status/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.222623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/
+-rwxrwxrwx   0 root         (0) root         (0)     2290 2023-12-15 20:50:14.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.222623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/
+-rwxrwxrwx   0 root         (0) root         (0)      551 2023-12-15 20:50:37.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py
+-rwxrwxrwx   0 root         (0) root         (0)      950 2023-11-27 02:53:23.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     2582 2024-03-30 00:06:40.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     2923 2024-03-30 00:05:43.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1039 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.090624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.222623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/
+-rwxrwxrwx   0 root         (0) root         (0)     1313 2024-03-30 00:01:21.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1477 2024-03-30 00:13:11.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2024-03-30 00:08:56.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1319 2024-03-30 00:09:21.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.222623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/
+-rwxrwxrwx   0 root         (0) root         (0)      776 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1728 2023-12-15 20:03:33.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.222623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/selected_unit/
+-rwxrwxrwx   0 root         (0) root         (0)      275 2023-11-26 22:20:49.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/selected_unit/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2023-12-15 19:52:46.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/names.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.222623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/
+-rwxrwxrwx   0 root         (0) root         (0)     1200 2024-03-07 04:13:37.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.090624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/
+-rwxrwxrwx   0 root         (0) root         (0)     1207 2023-12-16 05:02:53.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/
+-rwxrwxrwx   0 root         (0) root         (0)     2315 2024-03-30 00:02:05.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py
+-rwxrwxrwx   0 root         (0) root         (0)     6474 2024-03-30 00:18:21.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     3862 2024-03-30 00:17:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     2473 2024-02-04 20:24:03.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/
+-rwxrwxrwx   0 root         (0) root         (0)   215864 2024-04-09 20:16:43.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     2506 2024-03-11 02:02:18.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/
+-rwxrwxrwx   0 root         (0) root         (0)   131410 2024-04-09 20:16:42.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     1863 2024-03-11 01:24:01.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/
+-rwxrwxrwx   0 root         (0) root         (0)   127961 2024-04-09 20:16:43.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON
+-rwxrwxrwx   0 root         (0) root         (0)     1755 2023-12-16 05:04:27.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1606 2023-12-16 05:04:52.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/
+-rwxrwxrwx   0 root         (0) root         (0)     2844 2023-12-16 05:01:05.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.090624 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/
+-rwxrwxrwx   0 root         (0) root         (0)      471 2023-12-15 22:41:08.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/slice/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-09 18:24:24.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/slice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/cautionary_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-16 04:48:59.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/cautionary_ingredients/formulate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.226623 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/
+-rwxrwxrwx   0 root         (0) root         (0)     3439 2024-03-07 04:11:50.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py
+-rwxrwxrwx   0 root         (0) root         (0)     1876 2023-11-26 22:19:07.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      968 2024-02-04 19:27:25.000000 apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.230623 apoplast-1.1.2/venues/stages/apoplast/shows/natures/
+-rwxrwxrwx   0 root         (0) root         (0)      101 2023-11-17 21:50:38.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      371 2023-11-21 23:21:15.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/assertions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.230623 apoplast-1.1.2/venues/stages/apoplast/shows/natures/measured_ingredient/
+-rwxrwxrwx   0 root         (0) root         (0)       84 2023-11-22 02:42:38.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/measured_ingredient/assertions.py
+-rwxrwxrwx   0 root         (0) root         (0)      332 2024-03-29 20:56:02.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/nature.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.230623 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.230623 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/nature/
+-rwxrwxrwx   0 root         (0) root         (0)     3867 2023-11-28 02:28:19.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/nature/nature.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-11-25 23:54:11.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/nature: form.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      139 2023-11-28 02:28:25.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/pattern.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      115 2023-11-16 20:19:44.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/pattern: measured ingredients.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-11-16 20:58:52.000000 apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/pattern: unmeasured ingredients.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      843 2024-03-31 01:49:28.000000 apoplast-1.1.2/venues/stages/apoplast/shows/shows.s.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/
+-rwxrwxrwx   0 root         (0) root         (0)     1523 2024-03-31 02:20:59.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/grove.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/info/
+-rwxrwxrwx   0 root         (0) root         (0)       58 2024-03-31 02:19:44.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/info/info.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/measures/
+-rwxrwxrwx   0 root         (0) root         (0)       73 2024-03-31 02:21:06.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/measures/measures.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/natures/
+-rwxrwxrwx   0 root         (0) root         (0)       59 2024-03-31 02:21:27.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/natures/natures.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/unites/
+-rwxrwxrwx   0 root         (0) root         (0)     1508 2024-03-31 02:23:11.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/unites/unites.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      131 2024-03-31 02:19:06.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/land.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.234623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/measures/
+-rwxrwxrwx   0 root         (0) root         (0)      459 2024-03-31 02:16:52.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/measures/measures.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/natures/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2024-03-31 02:09:01.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/natures/natures.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/measured_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)      405 2024-03-31 01:56:16.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/measured_ingredients/measured_ingredients.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/measures/
+-rwxrwxrwx   0 root         (0) root         (0)     1018 2024-03-31 01:54:44.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/measures/measures.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      426 2024-03-31 01:58:10.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/nature.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/unmeasured_ingredients/
+-rwxrwxrwx   0 root         (0) root         (0)      294 2024-03-31 01:56:52.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/unmeasured_ingredients/UI.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)      106 2024-03-31 01:57:56.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/shows.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast/shows_v2/treasure/
+-rwxrwxrwx   0 root         (0) root         (0)      232 2024-03-31 01:52:52.000000 apoplast-1.1.2/venues/stages/apoplast/shows_v2/treasure/treasure.S.HTML
+-rwxrwxrwx   0 root         (0) root         (0)       63 2023-11-16 19:27:45.000000 apoplast-1.1.2/venues/stages/apoplast/status_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:17:14.238623 apoplast-1.1.2/venues/stages/apoplast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-09 20:17:14.000000 apoplast-1.1.2/venues/stages/apoplast.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    27469 2024-04-09 20:17:14.000000 apoplast-1.1.2/venues/stages/apoplast.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-09 20:17:14.000000 apoplast-1.1.2/venues/stages/apoplast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-09 20:17:14.000000 apoplast-1.1.2/venues/stages/apoplast.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       58 2024-04-09 20:17:14.000000 apoplast-1.1.2/venues/stages/apoplast.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2024-04-09 20:17:14.000000 apoplast-1.1.2/venues/stages/apoplast.egg-info/top_level.txt
```

### Comparing `apoplast-1.1.1/PKG-INFO` & `apoplast-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: apoplast
-Version: 1.1.1
+Version: 1.1.2
 Summary: The search for an abundant panacea of vivaciously invigorating utopian vegan absorbables.
 License: GPL 3.0 + vegan
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/modules_series_4/apoplast
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: ships
 Requires-Dist: sphene
+Requires-Dist: sanic
 Requires-Dist: pymongo
 Requires-Dist: pydash
 Requires-Dist: rich
 Requires-Dist: tinydb
 Requires-Dist: numpy
```

### Comparing `apoplast-1.1.1/readme.md` & `apoplast-1.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/-license/list/gpl-3.0-standalone.html` & `apoplast-1.1.2/venues/stages/apoplast/-license/list/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/__status/db/records.json` & `apoplast-1.1.2/venues/stages/apoplast/__status/db/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9917218543046358%*

 * *Differences: {"'_default'": "{'298': OrderedDict([('paths', []), ('alarms', []), ('stats', "*

 * *               "OrderedDict([('alarms', 0), ('empty', 0), ('checks', OrderedDict([('passes', 0), "*

 * *               "('alarms', 0)]))]))]), '299': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'status_1.py'), ('empty', False), ('parsed', True), ('stats', "*

 * *               "OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('passed', True), ('elapsed', [4 […]*

```diff
@@ -346074,14 +346074,2097 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 106
                 },
                 "empty": 2
             }
         },
+        "298": {
+            "alarms": [],
+            "paths": [],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "299": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "JSONDecodeError('Expecting value: line 1 column 1 (char 0)')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 81, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 10, in check_1",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py\", line 56, in beautifully",
+                                "    ingredients_DB_list = ingredients_DB_list_scan.retrieve (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py\", line 44, in retrieve",
+                                "    return ingredients_DB.all ()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 233, in all",
+                                "    return list(iter(self))",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 655, in __iter__",
+                                "    for doc_id, doc in self._read_table().items():",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 704, in _read_table",
+                                "    tables = self._storage.read()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/storages.py\", line 136, in read",
+                                "    return json.load(self._handle)",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 293, in load",
+                                "    return loads(fp.read(),",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 346, in loads",
+                                "    return _default_decoder.decode(s)",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 337, in decode",
+                                "    obj, end = self.raw_decode(s, idx=_w(s, 0).end())",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 355, in raw_decode",
+                                "    raise JSONDecodeError(\"Expecting value\", s, err.value) from None",
+                                "json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "shows/ingredient_scan/grove/seek/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 10, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_gram_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredient') at 126220100828848\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 36, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.measured_ingredients as measured_ingredients_builder",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py\", line 8, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.measured_ingredient as measured_ingredient_builder",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredient') at 126220100828848"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.serving_size.amount') at 134744757452656\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 7, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 34, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.serving_size.amount as serving_size_amount_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.serving_size.amount') at 134744757452656"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/amount/status_other_214893.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 12, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 12, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.1900057112798095e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0001240459969267249,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "insure/status_equalitites_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.0009794050019991118,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note/_status/status_multiples_of_3_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.8288002795306966e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_sci_note_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.007607817002281081,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002118079999490874,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.6236806790002447,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.0002669360001164023,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note_2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.415001502726227e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/integer/status_string_is_integer.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.0147998738102615e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/percentage/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "CHECK 1",
+                            "elapsed": [
+                                4.925800021737814e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "CHECK 2",
+                            "elapsed": [
+                                2.7032001526094973e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.6116002118214965e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/energy/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.2129973988048732e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass_equivalents/is_an_equivalent/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "fraction checks",
+                            "elapsed": [
+                                5.852599861100316e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "fraction checks, alternate spellings",
+                            "elapsed": [
+                                4.232900028000586e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "exceptions",
+                            "elapsed": [
+                                5.149995558895171e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/volume/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.185800157254562e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/_interpret/status_unit_kind.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00898989800043637,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.22124010599873145,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12220407600034378,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12409185300202807,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12527837800007546,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.29217209000125877,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.3027804470002593,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.2914310129999649,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.2109976870015089,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00015655199968023226,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "empty_aggregate_measures",
+                            "elapsed": [
+                                0.00012991399853490293,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00011407200145185925,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.255900057614781e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                4.4741002056980506e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/multiply/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.017438704999221954,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/aggregate/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0004166690014244523,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/sums/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0006215600005816668,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10045019899916952,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_cautionary_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.009877749002043856,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14911800399931963,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.034283213997696294,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0031975169986253604,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004684904997702688,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00742362500022864,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.008588029002567055,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.005613820001599379,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.0529997679404914e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.161998266587034e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.962003004038706e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.78300124895759e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005480609979713336,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.239000994246453e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.17488733800200862,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_count/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0006313270023383666,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.005235052998614265,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0008886489995347802,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003024308000021847,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_essentials_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003735393998795189,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_cautions_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.019996840001113014,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.010828276997926878,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_uniter/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.009449720997508848,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/essential_is_story_1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0007440599983965512,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/has_uniters/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "JSONDecodeError('Expecting value: line 1 column 1 (char 0)')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 81, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 10, in check_1",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py\", line 56, in beautifully",
+                                "    ingredients_DB_list = ingredients_DB_list_scan.retrieve (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py\", line 44, in retrieve",
+                                "    return ingredients_DB.all ()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 233, in all",
+                                "    return list(iter(self))",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 655, in __iter__",
+                                "    for doc_id, doc in self._read_table().items():",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 704, in _read_table",
+                                "    tables = self._storage.read()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/storages.py\", line 136, in read",
+                                "    return json.load(self._handle)",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 293, in load",
+                                "    return loads(fp.read(),",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 346, in loads",
+                                "    return _default_decoder.decode(s)",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 337, in decode",
+                                "    obj, end = self.raw_decode(s, idx=_w(s, 0).end())",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 355, in raw_decode",
+                                "    raise JSONDecodeError(\"Expecting value\", s, err.value) from None",
+                                "json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0007677879984839819,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04470212299929699,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/list/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005915699985052925,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "seek name",
+                            "elapsed": [
+                                0.0003102850023424253,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek region",
+                            "elapsed": [
+                                0.00026847499975701794,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek name 2",
+                            "elapsed": [
+                                0.0007342099997913465,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "__status/status_API.proc.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009412039980816189,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/examples/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00251054600084899,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0059693969997169916,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.02330098799939151,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004141170997172594,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002621547999297036,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.013958362997072982,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.019890921001206152,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.005189399002119899,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.013341146001039306,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10154857800080208,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.13422065299891983,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.031448851001186995,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2412474.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.032275874000333715,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0012452090013539419,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0009159639994322788,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01958814699901268,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.00032870600261958316,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.012386313999741105,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.00014035500134923495,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 3",
+                            "elapsed": [
+                                0.00015167500168900006,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 10, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 126220102926192"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07390455700078746,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_gram_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredient') at 126220100828848\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 36, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.measured_ingredients as measured_ingredients_builder",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py\", line 8, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.measured_ingredient as measured_ingredient_builder",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredient') at 126220100828848"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0024815819997456856,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_tablet_261967.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004252662998624146,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004723299000033876,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003447502000199165,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_220884.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0008357199985766783,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.serving_size.amount') at 134744757452656\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 7, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 34, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.serving_size.amount as serving_size_amount_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.serving_size.amount') at 134744757452656"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/amount/status_other_214893.py"
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 12, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 12, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01120925700161024,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/powder/status_mane_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11141103899717564,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/_loop/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.13597272299739416,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.013368987001740607,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0012384469991957303,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 7,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 98
+                },
+                "empty": 2
+            }
+        },
         "3": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
@@ -346480,14 +348563,6057 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 13
                 },
                 "empty": 0
             }
         },
+        "300": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredients') at 123406877407936\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 10, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 36, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.measured_ingredients as measured_ingredients_builder",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredients') at 123406877407936"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 134536586683840\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 134536586683840"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.319998308550566e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.7663001674227417e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "insure/status_equalitites_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.00110263700116775,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note/_status/status_multiples_of_3_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.31160005973652e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_sci_note_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.014506608000374399,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003639795999333728,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.5878364679992956,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.0003446729970164597,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note_2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1897001968463883e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/integer/status_string_is_integer.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.525499702547677e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/percentage/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "CHECK 1",
+                            "elapsed": [
+                                8.254600106738508e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "CHECK 2",
+                            "elapsed": [
+                                6.135199873824604e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.186599860782735e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/energy/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.248998837079853e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass_equivalents/is_an_equivalent/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "fraction checks",
+                            "elapsed": [
+                                5.601299926638603e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "fraction checks, alternate spellings",
+                            "elapsed": [
+                                4.289799835532904e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "exceptions",
+                            "elapsed": [
+                                3.8200232665985823e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/volume/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.914899833849631e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/_interpret/status_unit_kind.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0019711439999809954,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.28344162500070524,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.275488958999631,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.22031003500160296,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10933446399940294,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.25536541900146403,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.13325839299795916,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.15820186299970374,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14831542299725697,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00010502699660719372,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "empty_aggregate_measures",
+                            "elapsed": [
+                                9.621600111131556e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00014619699868489988,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.9134000214980915e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                4.682199869421311e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/multiply/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01203191400054493,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/aggregate/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04937717800203245,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/sums/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005291029992804397,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11864214999877731,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_cautionary_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07094176700047683,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.16378002599958563,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.029175703999499092,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0010772789973998442,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002057910998701118,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004690780999226263,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0030009780020918697,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.013367786999879172,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.863999492954463e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.011000318219885e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.30800093151629e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.243001164169982e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0006747970001015346,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.189976945985109e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.09317447699868353,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_count/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0011558949991012923,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0034294689976377413,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0013376559982134495,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002632261999679031,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_essentials_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0010101739972014911,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_cautions_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.001351815000816714,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0023589179982081987,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_uniter/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0008509120016242377,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/essential_is_story_1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009493780016782694,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/has_uniters/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005821029990329407,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0019019589999516029,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0024041830001806375,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/list/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0008625160007795785,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "seek name",
+                            "elapsed": [
+                                0.00012593900100910105,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek region",
+                            "elapsed": [
+                                8.671099931234494e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek name 2",
+                            "elapsed": [
+                                8.817699927021749e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "__status/status_API.proc.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00043844500032719225,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/examples/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0011317520002194215,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00705834399923333,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0015622310020262375,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.001001135999104008,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00168198200117331,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.010892812999372836,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01973770800032071,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.020742689997859998,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.06510610600162181,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.18837048699788284,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.20761121300165541,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.05217207799796597,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2412474.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07940081199922133,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003716635997989215,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0020311570006015245,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0003423039997869637,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0010041400018963031,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0023212160012917593,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0011781510002037976,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 3",
+                            "elapsed": [
+                                0.0009873259987216443,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredients') at 123406877407936\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 10, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 36, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.measured_ingredients as measured_ingredients_builder",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.measured_ingredients') at 123406877407936"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.933000698452815e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 134536586683840\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 134536586683840"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.008200662003218895,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_gram_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004793973999767331,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0038420269993366674,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_tablet_261967.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002755711000645533,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.006296936000580899,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.006461501998273889,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_220884.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004419860000780318,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.1350001487880945e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/amount/status_other_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004496200999710709,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0018617059977259487,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.007558798999525607,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/powder/status_mane_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.13569350100078736,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/_loop/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1205363179979031,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07748780099791475,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.007706926000537351,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 2,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 104
+                },
+                "empty": 2
+            }
+        },
+        "301": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "JSONDecodeError('Expecting value: line 1 column 1 (char 0)')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 81, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 20, in check_1",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py\", line 56, in beautifully",
+                                "    ingredients_DB_list = ingredients_DB_list_scan.retrieve (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py\", line 44, in retrieve",
+                                "    return ingredients_DB.all ()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 233, in all",
+                                "    return list(iter(self))",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 655, in __iter__",
+                                "    for doc_id, doc in self._read_table().items():",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 704, in _read_table",
+                                "    tables = self._storage.read()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/storages.py\", line 136, in read",
+                                "    return json.load(self._handle)",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 293, in load",
+                                "    return loads(fp.read(),",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 346, in loads",
+                                "    return _default_decoder.decode(s)",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 337, in decode",
+                                "    obj, end = self.raw_decode(s, idx=_w(s, 0).end())",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 355, in raw_decode",
+                                "    raise JSONDecodeError(\"Expecting value\", s, err.value) from None",
+                                "json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "shows/ingredient_scan/grove/seek_uniter/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.food_USDA.interpret.packageWeight.interpret') at 131309633140624\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 7, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py\", line 25, in <module>",
+                        "    import apoplast.clouds.food_USDA.interpret.packageWeight.interpret as interpreter",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.food_USDA.interpret.packageWeight.interpret') at 131309633140624"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/food_USDA/interpret/packageWeight/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 10, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.amount') at 133945520942976\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 33, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.amount as form_amount_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.amount') at 133945520942976"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 8, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_220884.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 8, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_270619.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 7, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/amount/status_other_214893.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.189976945985109e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.448099884437397e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "insure/status_equalitites_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.0012001280010736082,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note/_status/status_multiples_of_3_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.9124003049219027e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_sci_note_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01755214899822022,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00218731000131811,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.5335358230004204,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.00023403899831464514,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note_2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1218002327950671e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/integer/status_string_is_integer.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.826100045349449e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/percentage/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "CHECK 1",
+                            "elapsed": [
+                                7.69990001572296e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "CHECK 2",
+                            "elapsed": [
+                                5.7165001635439694e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.7985999369993806e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/energy/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.2999993234407157e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass_equivalents/is_an_equivalent/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "fraction checks",
+                            "elapsed": [
+                                6.794000000809319e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "fraction checks, alternate spellings",
+                            "elapsed": [
+                                4.2722000216599554e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "exceptions",
+                            "elapsed": [
+                                4.699977580457926e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/volume/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                9.657500049797818e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/_interpret/status_unit_kind.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.006225889999768697,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.13462581999920076,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1395056539986399,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1292041929991683,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.09079927099810448,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.24335247599810828,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.22433613699831767,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.24605201899976237,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.20527483499972732,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00014786400060984306,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "empty_aggregate_measures",
+                            "elapsed": [
+                                0.0001529319997644052,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00011703900236170739,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.042100044898689e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                5.404799958341755e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/multiply/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0379039819999889,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/aggregate/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004991977002646308,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/sums/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0004787760008184705,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.15209273700020276,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_cautionary_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04419971099923714,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.09228006100238417,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.039818108998588286,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.014163152998662554,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009329470012744423,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01572194300024421,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.016682912999385735,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003033385000890121,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.87100294069387e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.730999302817509e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.904999514110386e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.3349980337079614e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.007359383002039976,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.580004653893411e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.061334943002293585,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_count/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0006235170003492385,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0019493260006129276,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0030268360023910645,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.016049857000325574,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_essentials_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009364200013806112,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_cautions_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "JSONDecodeError('Expecting value: line 1 column 1 (char 0)')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 81, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 20, in check_1",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py\", line 56, in beautifully",
+                                "    ingredients_DB_list = ingredients_DB_list_scan.retrieve (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py\", line 44, in retrieve",
+                                "    return ingredients_DB.all ()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 233, in all",
+                                "    return list(iter(self))",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 655, in __iter__",
+                                "    for doc_id, doc in self._read_table().items():",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 704, in _read_table",
+                                "    tables = self._storage.read()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/storages.py\", line 136, in read",
+                                "    return json.load(self._handle)",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 293, in load",
+                                "    return loads(fp.read(),",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 346, in loads",
+                                "    return _default_decoder.decode(s)",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 337, in decode",
+                                "    obj, end = self.raw_decode(s, idx=_w(s, 0).end())",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 355, in raw_decode",
+                                "    raise JSONDecodeError(\"Expecting value\", s, err.value) from None",
+                                "json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+                            ],
+                            "passed": false
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0005771489995822776,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_uniter/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005689070021617226,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/essential_is_story_1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009729460034577642,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/has_uniters/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0004924080021737609,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0007743440000922419,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003643534000730142,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/list/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0006349190007313155,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "seek name",
+                            "elapsed": [
+                                0.00021917300182394683,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek region",
+                            "elapsed": [
+                                0.0001457799990021158,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek name 2",
+                            "elapsed": [
+                                0.0001466330031689722,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "__status/status_API.proc.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0007730380020802841,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/examples/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.005548434000957059,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0037707050032622647,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002635347998875659,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004701107001892524,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0144630330032669,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.008772297001996776,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.013637945001391927,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.010034989998530364,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0242443489987636,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07493310599966208,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.09215419800239033,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04183335000197985,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2412474.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.029291404000105103,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.food_USDA.interpret.packageWeight.interpret') at 131309633140624\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 7, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py\", line 25, in <module>",
+                        "    import apoplast.clouds.food_USDA.interpret.packageWeight.interpret as interpreter",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.food_USDA.interpret.packageWeight.interpret') at 131309633140624"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/food_USDA/interpret/packageWeight/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.048178348999499576,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0001785160020517651,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009903769969241694,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.00023988300017663278,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 3",
+                            "elapsed": [
+                                0.00011155199899803847,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 10, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 135837749819952"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0001444789995730389,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_gram_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004483991000597598,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0003907150021404959,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_tablet_261967.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0021206599994911812,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.amount') at 133945520942976\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 33, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.amount as form_amount_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.amount') at 133945520942976"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 8, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_220884.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 8, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_270619.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "ImportError(\"cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 7, in <module>",
+                        "ImportError: cannot import name 'nature' from 'apoplast.clouds.supp_NIH' (unknown location)"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/form/amount/status_other_214893.py"
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.014062703998206416,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0016975889993773308,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.021588949002762092,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/powder/status_mane_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12376321899864706,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/_loop/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.15373897600147757,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.030442923998634797,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0026501560023461934,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 8,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 96
+                },
+                "empty": 2
+            }
+        },
+        "302": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "JSONDecodeError('Expecting value: line 1 column 1 (char 0)')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 81, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 15, in check_1",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py\", line 51, in eloquently",
+                                "    \"grove\": grove_nurture.beautifully (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py\", line 56, in beautifully",
+                                "    ingredients_DB_list = ingredients_DB_list_scan.retrieve (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py\", line 44, in retrieve",
+                                "    return ingredients_DB.all ()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 233, in all",
+                                "    return list(iter(self))",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 655, in __iter__",
+                                "    for doc_id, doc in self._read_table().items():",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 704, in _read_table",
+                                "    tables = self._storage.read()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/storages.py\", line 136, in read",
+                                "    return json.load(self._handle)",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 293, in load",
+                                "    return loads(fp.read(),",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 346, in loads",
+                                "    return _default_decoder.decode(s)",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 337, in decode",
+                                "    obj, end = self.raw_decode(s, idx=_w(s, 0).end())",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 355, in raw_decode",
+                                "    raise JSONDecodeError(\"Expecting value\", s, err.value) from None",
+                                "json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.4600164983421564e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.000731064999854425,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "insure/status_equalitites_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.0010435939984745346,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note/_status/status_multiples_of_3_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.6751000152435154e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_sci_note_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.021654243999364553,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0019420850003371015,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.7101666939997813,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/decimal/reduce/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                0.0002762580006674398,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/sci_note_2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                9.840998245636001e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/integer/status_string_is_integer.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.9923000662820414e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/number/percentage/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "CHECK 1",
+                            "elapsed": [
+                                8.700699982000515e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "CHECK 2",
+                            "elapsed": [
+                                6.19469974481035e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.9188999178586528e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/energy/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.949000190710649e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/mass_equivalents/is_an_equivalent/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "fraction checks",
+                            "elapsed": [
+                                5.531199713004753e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "fraction checks, alternate spellings",
+                            "elapsed": [
+                                4.4338001316646114e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "exceptions",
+                            "elapsed": [
+                                4.760004230774939e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/volume/swap/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.436399831320159e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "measures/_interpret/status_unit_kind.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009478070023760665,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14537895600005868,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1425305489974562,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14043056000082288,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.09987540899965097,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.256302745998255,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.25807940199956647,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.2470184279991372,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.20850711399907595,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.844500189297833e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "empty_aggregate_measures",
+                            "elapsed": [
+                                8.680099927005358e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00013643000056617893,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/merge/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.0606999391457066e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                6.011000004946254e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/measures/multiply/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01993009699799586,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/aggregate/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00048479299948667176,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/measures/sums/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009224250024999492,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04054293199806125,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/build/status_cautionary_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.033118332001322415,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10234775599747081,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.024200995998398867,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/multiply_amount/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0012887420016340911,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004257484997651773,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.008003568997082766,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "JSONDecodeError('Expecting value: line 1 column 1 (char 0)')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 81, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 15, in check_1",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py\", line 51, in eloquently",
+                                "    \"grove\": grove_nurture.beautifully (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py\", line 56, in beautifully",
+                                "    ingredients_DB_list = ingredients_DB_list_scan.retrieve (",
+                                "  File \"/apoplast/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py\", line 44, in retrieve",
+                                "    return ingredients_DB.all ()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 233, in all",
+                                "    return list(iter(self))",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 655, in __iter__",
+                                "    for doc_id, doc in self._read_table().items():",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/table.py\", line 704, in _read_table",
+                                "    tables = self._storage.read()",
+                                "  File \"/apoplast/venues/stages_pip/tinydb/storages.py\", line 136, in read",
+                                "    return json.load(self._handle)",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 293, in load",
+                                "    return loads(fp.read(),",
+                                "  File \"/usr/lib/python3.10/json/__init__.py\", line 346, in loads",
+                                "    return _default_decoder.decode(s)",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 337, in decode",
+                                "    obj, end = self.raw_decode(s, idx=_w(s, 0).end())",
+                                "  File \"/usr/lib/python3.10/json/decoder.py\", line 355, in raw_decode",
+                                "    raise JSONDecodeError(\"Expecting value\", s, err.value) from None",
+                                "json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.010443268998642452,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.013000190956518e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.097001460148022e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.002999387215823e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.6150020100176334e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove_prototype/seek/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0046067939983913675,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.659990271553397e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1619308369990904,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_count/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.000916492997930618,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.006297782998444745,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0019163739998475648,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/erase_ingredient/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.015826689999812515,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_essentials_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.006819451999035664,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/nurture/status_cautions_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009663830023782793,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0004210169972793665,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek_uniter/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003038001999811968,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/essential_is_story_1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0004939840000588447,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/has_uniters/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.000803242000984028,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/grove/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.025564289000612916,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.001818262000597315,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/list/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.001429829000699101,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "seek name",
+                            "elapsed": [
+                                0.00023276600040844642,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek region",
+                            "elapsed": [
+                                0.00015139899915084243,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "seek name 2",
+                            "elapsed": [
+                                0.000496905002364656,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "shows/ingredient_scan/DB/scan/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "__status/status_API.proc.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005504549990291707,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/examples/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.002441075001115678,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0013674469992110971,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0041071550003835,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.007524202999775298,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0030020919984963257,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/form/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.007516986999689834,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.010194766997301485,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0066034980009135325,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04452830900117988,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12701346399990143,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_loop_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1442208890002803,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.042864757000643294,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2412474.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.042887984000117285,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/nature/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.003939725000236649,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.001000218002445763,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01637225599915837,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.0017948569984582718,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 2
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0008405209991906304,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 2",
+                            "elapsed": [
+                                0.00035492199822328985,
+                                "seconds"
+                            ],
+                            "passed": true
+                        },
+                        {
+                            "check": "check 3",
+                            "elapsed": [
+                                0.00025963100051740184,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 3
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.004361016999610001,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py"
+                },
+                {
+                    "alarm": "An exception occurred while scanning the path.",
+                    "exception": "_DeadlockError(\"deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/apoplast/venues/stages_pip/volts/processes/scan/process/keg/check.py\", line 54, in start",
+                        "    exec (",
+                        "  File \"<string>\", line 6, in <module>",
+                        "  File \"/apoplast/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py\", line 32, in <module>",
+                        "    import apoplast.clouds.supp_NIH.nature.form.unit as form_unit_calculator",
+                        "  File \"<frozen importlib._bootstrap>\", line 1024, in _find_and_load",
+                        "  File \"<frozen importlib._bootstrap>\", line 171, in __enter__",
+                        "  File \"<frozen importlib._bootstrap>\", line 116, in acquire",
+                        "_frozen_importlib._DeadlockError: deadlock detected by _ModuleLock('apoplast.clouds.supp_NIH.nature.form.unit') at 136384145129680"
+                    ],
+                    "parsed": false,
+                    "path": "clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.005789191000076244,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_gram_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.006431275996874319,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00568534199919668,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_tablet_261967.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0022430760000133887,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.005057703001511982,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0032348370004910976,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_220884.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0028621230012504384,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/unit/status_powder_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.301000444684178e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/amount/status_other_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "empty": true,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.01186166000115918,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0031790489992999937,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.012675303001742577,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/powder/status_mane_270619.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07461997300197254,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/_loop/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07476377100101672,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.041967663000832545,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0007953879976412281,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 2,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 103
+                },
+                "empty": 2
+            }
+        },
         "31": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `apoplast-1.1.1/structures/modules/apoplast/__status/db_API/records.json` & `apoplast-1.1.2/venues/stages/apoplast/__status/db_API/records.json`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/__status/status.proc.py` & `apoplast-1.1.2/venues/stages/apoplast/__status/status_API.proc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 
 
-'''
-	mongo connection strings
-		
-		DB: apoplast
-			
-			collection: 
-				cautionary_ingredients
-				essential_nutrients
-'''
 
 
 
 def add_paths_to_system (paths):
 	import pathlib
 	from os.path import dirname, join, normpath
 	import sys
@@ -32,31 +23,30 @@
 
 module_name = "apoplast"
 
 this_directory = pathlib.Path (__file__).parent.resolve ()
 structures = str (normpath (join (this_directory, "../../../../structures")))
 this_module = str (normpath (join (structures, f"modules/{ module_name }")))
 
-#glob_string = structures + '/modules/**/status_*.py'
 
 import sys
 if (len (sys.argv) >= 2):
 	glob_string = this_module + '/' + sys.argv [1]
 	db_directory = False
 else:
-	glob_string = this_module + '/**/status_*.py'
-	db_directory = normpath (join (this_directory, "db"))
+	glob_string = this_module + '/**/API_status_*.py'
+	db_directory = normpath (join (this_directory, "db_API"))
 
-print ("glob string:", glob_string)
+#glob_string = structures + '/modules/**/API_status_*.py'
 
 import volts
 scan = volts.start (
 	glob_string = glob_string,
 	simultaneous = True,
 	module_paths = [
 		normpath (join (structures, "modules")),
 		normpath (join (structures, "modules_pip"))
 	],
-	relative_path = this_module,
+	relative_path = normpath (join (structures, f"modules/{ module_name }")),
 	
 	db_directory = db_directory
 )
```

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/deliveries/one/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/food.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/food.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_2412474.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2412474.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_3.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/status_mass_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/form/status_volume_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/form/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/goodness_certifications/certifications.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/goodness_certifications/certifications.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/goodness_certifications/vegan.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/goodness_certifications/vegan.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/NIH.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/NIH.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/deliveries/one/assertions.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/assertions.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/form.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/form.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 '''
 	python3 insurance.py clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py
 '''
 
 import apoplast.clouds.supp_NIH.nature.form.serving_size.amount as serving_size_amount_calculator
 
-def check_1 ():
+import apoplast.clouds.supp_NIH.nature as supp_NIH_nature
+import apoplast.clouds.supp_NIH.examples as NIH_examples
 
-	import apoplast.clouds.supp_NIH.nature as supp_NIH_nature
-	import apoplast.clouds.supp_NIH.examples as NIH_examples
+def check_1 ():
 	supp_1 = NIH_examples.retrieve ("powder packets/multivitamin_246811.JSON")
 
 
 	net_contents = [
 		{
 			"order": 1,
 			"quantity": 5.29,
```

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/_mongo_exports/essential_nutrients/essential_nutrients.1.json` & `apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/essential_nutrients.1.json`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/collections/_land/insert_document.py` & `apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/collections/_land/insert_document.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/data_nodes/ingredients/ingredients.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/data_nodes/ingredients/ingredients.S.HTML`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,24 @@
 			
 			
 			collection: "cautionary_ingredients" [{
 				
 				
 			}]
 			
+			#
+			#	any ingredients
+			#	thorough
+			#
+			#
+			collection: "glossary" [{
+				
+				
+			}]
+			
 
 	<h2>itinerary</h2>
 	
 		#
 		#	the variables
 		#
 		from apoplast._variables import prepare_variables
```

### Comparing `apoplast-1.1.1/structures/modules/apoplast/insure/equalities.py` & `apoplast-1.1.2/venues/stages/apoplast/insure/equalities.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/insure/override_print.py` & `apoplast-1.1.2/venues/stages/apoplast/insure/override_print.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/_interpret/status_unit_kind.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/_interpret/status_unit_kind.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/_interpret/unit_kind.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/_interpret/unit_kind.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/energy/energy.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/measures/energy/energy.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/energy/swap/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/energy/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass/swap/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass/swap/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass/system international.r.html` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass/system international.r.html`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass/us customary.r.html` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass/us customary.r.html`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/jargon.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/jargon.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/mass_equivalents/mass equivalents.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/measures/mass_equivalents/mass equivalents.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/decimal/reduce/status_3.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/decimal/reduce/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/integer/status_string_is_integer.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/integer/status_string_is_integer.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/percentage/from_fraction.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/percentage/from_fraction.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/percentage/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/percentage/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/sci_note.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/sci_note.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/number/sci_note_2/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/number/sci_note_2/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/volume/swap/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/volume/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/volume/swap/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/measures/volume/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/measures/weight/weight.r.html` & `apoplast-1.1.2/venues/stages/apoplast/measures/weight/weight.r.html`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/proposals/proposals.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/proposals/proposals.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/forward channel.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/forward channel.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/forward_channel/structures.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/forward_channel/structures.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/access.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/access.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/path.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/path.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/assertions/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/print/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/print/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove/sort/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/ingredient scan.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/ingredient scan.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/cultivate/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/land.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/land.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/merge/status_3.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/multiply/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan/measures/multiply/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/nature/nature.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/nature/nature.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/natures/pattern/nature: form.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/natures/pattern/nature: form.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows/shows.s.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows/shows.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/grove.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/grove.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows_v2/land/grove/unites/unites.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows_v2/land/grove/unites/unites.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast/shows_v2/nature/measures/measures.S.HTML` & `apoplast-1.1.2/venues/stages/apoplast/shows_v2/nature/measures/measures.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-1.1.1/structures/modules/apoplast.egg-info/PKG-INFO` & `apoplast-1.1.2/venues/stages/apoplast.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: apoplast
-Version: 1.1.1
+Version: 1.1.2
 Summary: The search for an abundant panacea of vivaciously invigorating utopian vegan absorbables.
 License: GPL 3.0 + vegan
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/modules_series_4/apoplast
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: ships
 Requires-Dist: sphene
+Requires-Dist: sanic
 Requires-Dist: pymongo
 Requires-Dist: pydash
 Requires-Dist: rich
 Requires-Dist: tinydb
 Requires-Dist: numpy
```

