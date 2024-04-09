# Comparing `tmp/pyweatherfr-2.0.4.tar.gz` & `tmp/pyweatherfr-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-2.0.4.tar", last modified: Sun Apr  7 12:27:08 2024, max compression
+gzip compressed data, was "pyweatherfr-3.0.0.tar", last modified: Tue Apr  9 18:19:18 2024, max compression
```

## Comparing `pyweatherfr-2.0.4.tar` & `pyweatherfr-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    36004 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36888 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:19:17.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/setup.py
```

### Comparing `pyweatherfr-2.0.4/LICENSE.txt` & `pyweatherfr-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.4/PKG-INFO` & `pyweatherfr-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.4
+Version: 3.0.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.4/README.md` & `pyweatherfr-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 exemple : ``pyweatherfr -n Grenoble`` affiche les données météo pour Grenoble 
 
 pyweatherfr \[TOWN\] -j [INT(0-3)]
 
 exemple : ``pyweatherfr Grenoble -j 1`` affiche les prévisions météo détaillées pour Grenoble à J+1
 
-pyweatherfr -p \[CODE_POSTAL\]
+exemple : ``pyweatherfr Grenoble -j -2`` affiche les données météo détaillées pour Grenoble à J-2
 
-exemple : ``pyweatherfr -p  38700`` affiche les prévisions météo pour le code postal 38700
+exemple : ``pyweatherfr 38700`` affiche les prévisions météo pour le code postal 38700
 
 pyweatherfr -g \[COORDONNEES_GPS\]
 
 exemple : `` pyweatherfr -g 45 5`` affiche les prévisions météo pour les coordonnées GPS (latitude : 45 et longitude : 5)
 
 
 ## Autres options
```

### Comparing `pyweatherfr-2.0.4/pyweatherfr/args.py` & `pyweatherfr-3.0.0/pyweatherfr/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,41 +41,33 @@
     )
     my_group = my_parser.add_mutually_exclusive_group()
     my_group.add_argument(
         "town",
         metavar="VILLE",
         type=str,
         nargs="?",
-        help="affichage des données météo par nom de ville -si absent, la VILLE est déduite de l'ip-",
+        help="affichage des données météo par nom de ville ou code postal -si absent, la VILLE est déduite de l'ip-",
     )
     my_parser.add_argument(
         "-n",
         "--now",
         action="store_true",
         help="affichage des données météo détaillées actuelles",
     )    
     my_parser.add_argument(
         "-j",
         "--jour",
         metavar="JOUR",
         action="store",
         type=int,
-        default=-1,
-        choices=range(0, 4),
-        help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ...)",
+        default=1000,
+        choices=range(-100, 4),
+        help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ..., -1 pour J-1, ...)",
     ) 
     my_group.add_argument(
-        "-p",
-        "--post",
-        action="store",
-        metavar="CODE_POSTAL",
-        type=str,
-        help="affichage des données météo par CODE_POSTAL",
-    )  
-    my_group.add_argument(
         "-g",
         "--gps",
         metavar=("LATITUDE", "LONGITUDE"),
         action="store",
         nargs=2,
         type=str,
         help="affichage des données météo par coordonnées GPS",
```

### Comparing `pyweatherfr-2.0.4/pyweatherfr/pyweatherfr.py` & `pyweatherfr-3.0.0/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,53 +104,58 @@
     doublon_cp = False
 
     vjson = recuperation_data_villes()
 
     if compute_args().search:
         search_town(vjson)
     elif compute_args().town:
-        url = obtain_url_and_town()
-    elif compute_args().post:
         url, doublon_cp = obtain_url_and_town_from_cp(vjson)
     elif compute_args().gps:
         is_gps = True
         url = obtain_url_and_town_from_gps()
     else:
         url = obtain_url_and_town_from_ip()
 
     print_debug(
         "recherche prévision depuis http://prevision-meteo.ch/services/json/" + url
     )
     r = requests.get("http://prevision-meteo.ch/services/json/" + url)
-    if r.json().get("errors"):
-        display_error(r)
+    try:
+        if r.json().get("errors"):
+            display_error(r)
+    except Exception:
+        print(r)        
     if is_gps:
         infos = "(" + url + ")"
         city = "."
     else:
         infos = obtain_info_town(vjson, url, r)
+        try:
+            city = r.json().get("city_info").get("name")
+        except Exception:
+            print(r)  
         city = r.json().get("city_info").get("name")
     if compute_args().now:
         previsions_courantes(r, infos, city)
-    elif compute_args().jour == -1:
+    elif compute_args().jour == 1000:
         previsions_generiques(r, infos, city)
     else:
         previsions_detaillees(r, infos, city)
     if incomplete_data == True:
         print(
             my_colored(
                 "attention : données incomplètes, vous pouvez essayer une autre ville pour plus de précision",
                 "yellow",
             )
         )
     if doublon_cp:
         print(
             my_colored(
                 'attention : il existe plusieurs villes associées au code postal. Si besoin, jouez "pyweather -s '
-                + compute_args().post
+                + compute_args().town
                 + '"'
                 + " pour trouver la ville souhaitée ",
                 "yellow",
             )
         )
 
 
@@ -259,33 +264,33 @@
                 ]
             )
 
     if compute_args().nocolor:
         headers = [
             "date",
             "temps",
-            "température (ressenties)",
+            "température (ressentie)",
             "précipitations",
             "vent (rafales)",
-            "direction",
+            "direction vent",
             "pression",
             "humidité",
-            "soleil / nuage"
+            "durée soleil / couverture nuage"
         ]
     else:
         headers = [
             "date",
             "temps",
-            "température (ressenties)",
+            "température (ressentie)",
             "précipitations",
             "vent (rafales)",
-            "direction",
+            "direction vent",
             "pression",
             "humidité",
-            "soleil / nuage",            
+            "durée soleil / couverture nuage",            
             "warnings",
         ]
 
     if data != []:
         if compute_args().condensate:
             table = columnar(data, no_borders=True, wrap_max=0)
         else:
@@ -388,15 +393,15 @@
     current_weather, emojiweather = traduction(current_weather_code)
     data = []
     direction = calculer_direction(current_wind_direction_10m)
 
     if compute_args().nocolor:
         data.append(
             [
-                "température",
+                "température (ressentie)",
                 f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",
             ]
         )
         data.append(["humidité", f"{current_relative_humidity_2m:.1f}%"])
         data.append(["precipitation", f"{current_precipitation:.1f}mm"])
         data.append(["pression", f"{current_surface_pressure:.1f}Hp"])
         data.append(
@@ -408,15 +413,15 @@
         )
         data.append(["temps", current_weather])
 
     else:
         if current_temperature_2m >= WARNING_WARM or current_apparent_temperature >= WARNING_WARM:
             data.append(
                 [
-                    "température",
+                    "température (ressentie)",
                     f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",
                     WARM,
                 ]
             )
         else:
             data.append(
                 [
@@ -542,19 +547,19 @@
                     direction,
                     duree
                 ]
             )
             headers = [
                 "date",
                 "temps",
-                "température",
+                "température (ressentie)",
                 "précipitations",
                 "vent (rafales)",
                 "direction",
-                "pluie/soleil"
+                "durée pluie / soleil"
             ]
         else:
             data2.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
@@ -570,19 +575,19 @@
                     duree,
                     warning,
                 ]
             )
             headers = [
                 "date",
                 "temps",
-                "température",
+                "température (ressentie)",
                 "précipitations",
                 "vent (rafales)",
-                "direction",
-                "pluie/soleil",
+                "direction vent",
+                "durée pluie / soleil",
                 "warning",
             ]
 
     if data2 != []:
         if compute_args().condensate:
             table = columnar(data2, no_borders=True, wrap_max=0)
         else:
@@ -663,15 +668,15 @@
 
 
 def display_error(r):
     print(my_colored("erreur : pas de données trouvées", "red"))
     print_debug(r.json().get("errors")[0].get("code"))
     print_debug(r.json().get("errors")[0].get("text"))
     print_debug(r.json().get("errors")[0].get("description"))
-    if compute_args().town or compute_args().post:
+    if compute_args().town:
         print(
             my_colored(
                 "essayez de trouver un paramètre correct avec \"pyweatherfr -s '"
                 + compute_args().town
                 + "'\"",
                 "yellow",
             )
@@ -728,58 +733,58 @@
     )
     url = "lat=" + compute_args().gps[0] + "lng=" + compute_args().gps[1]
     print_debug("URL : " + url)
     return url
 
 
 def obtain_url_and_town_from_cp(vjson):
-    post = compute_args().post.zfill(5)
-    print_debug("CODE_POSTAL : " + str(post))
-    print_debug(
-        "recherche de la VILLE et de l'URL depuis https://www.prevision-meteo.ch/services/json/list-cities"
-    )
-    i = 0
-    try:
-        trouve = False
-        doublon = False
-        while True:
-            if (
-                vjson.get(str(i)).get("country") is not None
-                and vjson.get(str(i)).get("country") == "FRA"
-            ):
-                if str(post) == vjson.get(str(i)).get("npa"):
-                    if not trouve:
-                        url = vjson.get(str(i)).get("url")
-                        print_debug("URL : " + url)
-                    if trouve:
-                        doublon = True
-                    trouve = True
-            i = i + 1
-    except Exception:
-        if not trouve:
-            print(
-                my_colored(
-                    "erreur : pas de ville trouvée avec le code postal " + str(post),
-                    "red",
+    town = compute_args().town
+    doublon = False
+    if town.isnumeric():
+        post = town
+        print_debug("CODE_POSTAL : " + str(post))
+        print_debug(
+            "recherche de la VILLE et de l'URL depuis https://www.prevision-meteo.ch/services/json/list-cities"
+        )
+        i = 0
+        try:
+            trouve = False
+            while True:
+                if (
+                    vjson.get(str(i)).get("country") is not None
+                    and vjson.get(str(i)).get("country") == "FRA"
+                ):
+                    if str(post) == vjson.get(str(i)).get("npa"):
+                        if not trouve:
+                            url = vjson.get(str(i)).get("url")
+                            print_debug("URL : " + url)
+                        if trouve:
+                            doublon = True
+                        trouve = True
+                i = i + 1
+        except Exception:
+            if not trouve:
+                print(
+                    my_colored(
+                        "erreur : pas de ville trouvée avec le code postal " + str(post),
+                        "red",
+                    )
                 )
-            )
-            print(
-                my_colored(
-                    "essayez avec un autre code postal, ou avec le code postal principal de la ville",
-                    "yellow",
+                print(
+                    my_colored(
+                        "essayez avec un autre code postal, ou avec le code postal principal de la ville ou encore le nom de la ville",
+                        "yellow",
+                    )
                 )
-            )
-            sys.exit(1)
-    return url, doublon
-
-
-def obtain_url_and_town():
-    url = unidecode.unidecode(compute_args().town.lower()).replace(" ", "-")
-    print_debug("URL : " + url)
-    return url
+                sys.exit(1)
+        return url, doublon
+    else:
+        url = unidecode.unidecode(town.lower()).replace(" ", "-")
+        print_debug("URL : " + url)
+        return url, doublon
 
 
 def search_town(vjson):
     search = compute_args().search
     print_debug(
         "recherche de la ville depuis https://www.prevision-meteo.ch/services/json/list-cities"
     )
@@ -808,15 +813,15 @@
                         my_colored(
                             "pour "
                             + name
                             + " ("
                             + npa
                             + "), exécutez 'pyweatherfr "
                             + url
-                            + "' or 'pyweatherfr -p "
+                            + "' or 'pyweatherfr  "
                             + npa
                             + "'",
                             "yellow",
                         )
                     )
             i = i + 1
     except Exception:
@@ -908,14 +913,15 @@
             "wind_direction_10m_dominant",
             "weather_code",
             "snowfall_sum",
             "precipitation_hours",
             "sunshine_duration"
         ],
     }
+    print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
 
     # Process daily data. The order of variables needs to be the same as requested.
     daily = response.Daily()
@@ -977,14 +983,15 @@
         "start_date": (datetime.datetime.now() + datetime.timedelta(days=day)).strftime(
             "%Y-%m-%d"
         ),
         "end_date": (
             datetime.datetime.now() + datetime.timedelta(days=day + 1)
         ).strftime("%Y-%m-%d"),
     }
+    print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
 
     # Process daily data. The order of variables needs to be the same as requested.
     hourly = response.Hourly()
@@ -1037,14 +1044,15 @@
             "weather_code",
             "pressure_msl",
             "wind_speed_10m",
             "wind_direction_10m",
             "wind_gusts_10m",
         ],
     }
+    print_debug("appel api meteo france "+url+"?"+'&'.join([f'{key}={",".join(value) if isinstance(value, list) else value}' for key, value in params.items()]))
     responses = openmeteo.weather_api(url, params=params)
 
     response = responses[0]
 
     current = response.Current()
     current_temperature_2m = current.Variables(0).Value()
     current_relative_humidity_2m = current.Variables(1).Value()
```

### Comparing `pyweatherfr-2.0.4/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-3.0.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.4
+Version: 3.0.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.4/setup.py` & `pyweatherfr-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="2.0.4",
+    version="3.0.0",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

