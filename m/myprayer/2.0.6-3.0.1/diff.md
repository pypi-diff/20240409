# Comparing `tmp/myprayer-2.0.6.tar.gz` & `tmp/myprayer-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myprayer-2.0.6.tar", max compression
+gzip compressed data, was "myprayer-3.0.1.tar", max compression
```

## Comparing `myprayer-2.0.6.tar` & `myprayer-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-2.0.6/LICENSE
--rw-r--r--   0        0        0     5975 2024-03-23 05:28:17.103974 myprayer-2.0.6/README.md
--rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-2.0.6/myprayer/__init__.py
--rw-r--r--   0        0        0     8662 2024-04-02 02:10:18.540660 myprayer-2.0.6/myprayer/api/client.py
--rw-r--r--   0        0        0     2672 2023-12-31 14:42:40.793978 myprayer-2.0.6/myprayer/api/day.py
--rw-r--r--   0        0        0      732 2023-10-14 01:43:01.057210 myprayer-2.0.6/myprayer/api/exceptions.py
--rw-r--r--   0        0        0      571 2023-10-17 21:43:15.204557 myprayer-2.0.6/myprayer/api/location_types.py
--rw-r--r--   0        0        0      669 2023-11-11 17:45:03.278715 myprayer-2.0.6/myprayer/api/method.py
--rw-r--r--   0        0        0     1983 2023-10-18 20:42:45.215200 myprayer-2.0.6/myprayer/api/month.py
--rw-r--r--   0        0        0      416 2023-11-26 16:42:45.935655 myprayer-2.0.6/myprayer/api/prayer.py
--rw-r--r--   0        0        0     5387 2024-03-22 21:23:48.888843 myprayer-2.0.6/myprayer/cli/config.py
--rw-r--r--   0        0        0     2689 2024-01-13 20:29:26.231274 myprayer-2.0.6/myprayer/cli/constants.py
--rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-2.0.6/myprayer/cli/enums.py
--rwxr-xr-x   0        0        0    11756 2024-04-02 01:55:35.084447 myprayer-2.0.6/myprayer/cli/main.py
--rw-r--r--   0        0        0     3420 2024-01-07 14:51:48.788896 myprayer-2.0.6/myprayer/cli/output.py
--rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-2.0.6/myprayer/cli/utils.py
--rw-r--r--   0        0        0      527 2024-04-02 02:12:18.170257 myprayer-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 myprayer-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-3.0.1/LICENSE
+-rw-r--r--   0        0        0     6123 2024-04-09 04:24:47.948029 myprayer-3.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-3.0.1/myprayer/__init__.py
+-rw-r--r--   0        0        0     5112 2024-04-09 04:05:59.536272 myprayer-3.0.1/myprayer/cli/config.py
+-rw-r--r--   0        0        0     2689 2024-04-09 03:00:44.536541 myprayer-3.0.1/myprayer/cli/constants.py
+-rw-r--r--   0        0        0     1995 2024-04-09 04:05:52.042947 myprayer-3.0.1/myprayer/cli/day.py
+-rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-3.0.1/myprayer/cli/enums.py
+-rwxr-xr-x   0        0        0    12521 2024-04-09 04:22:32.499778 myprayer-3.0.1/myprayer/cli/main.py
+-rw-r--r--   0        0        0     3420 2024-04-09 02:47:58.627693 myprayer-3.0.1/myprayer/cli/output.py
+-rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-3.0.1/myprayer/cli/utils.py
+-rw-r--r--   0        0        0      559 2024-04-09 04:22:40.026341 myprayer-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7101 1970-01-01 00:00:00.000000 myprayer-3.0.1/PKG-INFO
```

### Comparing `myprayer-2.0.6/LICENSE` & `myprayer-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.6/README.md` & `myprayer-3.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 ## Dependencies
 
 - Python 3.8+
 - [Typer](https://github.com/tiangolo/typer) - CLI app framework
 - [Inquirer.py](https://github.com/magmax/python-inquirer) - user prompts
 - [Rich](https://github.com/willmcgugan/rich) - output formatting
 - [Requests](https://docs.python-requests.org/en/latest/) - HTTP client
+- [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
+- [geopy](https://geopy.readthedocs.io/en/stable/) - Geocoding library
+- [tzlocal](https://pypi.org/project/tzlocal/) - Local timezone
+- [pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
+
 
 ### Install
 
 ```bash
 pip install myprayer
 ```
 
@@ -108,24 +113,21 @@
         "Fajr",
         "Dhuhr",
         "Asr",
         "Maghrib",
         "Isha"
     ],
     "location": { // Default location used if no location is provided in command
-        "type": "city",
-        "city": "Cairo",
-        "country": "Egypt",
-        "state": null
+        "latitude": 30,
+        "longitude": 31,
     }
 }
 ```
 
 
 ## Credits
-- [Aladhan API](https://aladhan.com/) - for prayer time data
-- [aladhan-api](https://pypi.org/project/aladhan-api/) - i drew inspiration from this project
+- [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
 
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `myprayer-2.0.6/myprayer/api/day.py` & `myprayer-3.0.1/myprayer/cli/day.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 from datetime import datetime, timedelta
 
-from myprayer.api.prayer import Prayer
+import tzlocal
+
+tz = tzlocal.get_localzone()
+
+
+class Prayer:
+    def __init__(self, name: str, time: datetime) -> None:
+        self.name = name
+        self.time = time
+
+    def has_passed(self) -> bool:
+        return datetime.now(tz) > self.time
+
+    def time_left(self) -> timedelta:
+        return self.time - datetime.now(tz)
+
+    def __str__(self) -> str:
+        return f"{self.name}: {self.time.strftime('%H:%M')}"
 
 
 class Day:
     """Represents a single day with prayer times.
 
     Attributes:
         day (int): The day number in the month
@@ -27,54 +44,22 @@
         >>> print(day.prayers[0].name)
         Fajr
 
         >>> day.get_prayer("fajr").__str__()
         Fajr: 05:20
     """
 
-    day: int
-    month: int
-    year: int
     data: dict
     prayers: list[Prayer]
 
-    def __init__(
-        self, day: int, month: int, year: int, data: dict, skip: list[str] = []
-    ):
-        if day not in range(1, 32):
-            raise ValueError("Day must be in range 1 to 31")
-        if month not in range(1, 13):
-            raise ValueError("Month must be in range 1 to 12")
-
-        self.data: dict = data
-        self.day: int = day
-        self.month: int = month
-        self.year: int = year
-        self.date: datetime = datetime(year, month, day)
-        self.prayers: list[Prayer] = []
-        self.skip: list[str] = skip
+    def __init__(self, date: datetime, prayers: list[Prayer], skip: list[str] = []):
 
-        timings = data["timings"]
-        day_passed = False
-        last_prayer = None
-        for prayer, time in timings.items():
-            if prayer in self.skip:
-                continue
-            prayer_time = datetime.strptime(time[:5], "%H:%M").replace(
-                day=self.day,
-                month=self.month,
-                year=self.year,
-            )
-            if last_prayer and (prayer_time - last_prayer).total_seconds() < 0:
-                day_passed = True
-
-            if day_passed:
-                prayer_time += timedelta(days=1)
-            self.prayers += [Prayer(prayer, prayer_time)]
-            last_prayer = prayer_time
+        self.date: datetime = date
+        self.prayers: list[Prayer] = prayers
+        self.skip: list[str] = skip
 
     def get_next_prayer(self) -> Prayer | None:
         for prayer in self.prayers:
             if not prayer.has_passed():
                 return prayer
 
     def get_prayer(self, name: str) -> Prayer | None:
```

### Comparing `myprayer-2.0.6/myprayer/cli/config.py` & `myprayer-3.0.1/myprayer/cli/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from enum import Enum
 from pathlib import Path
 from typing import Literal, Optional
 
 from pydantic import BaseModel, validator
 
-from myprayer.api.location_types import Address, City, Coordinates
 from myprayer.cli.constants import CALCULATION_METHODS, DEFAULT_PRAYERS
 from myprayer.cli.enums import OutType, TimeFormat
 
 
 class LocationType(str, Enum):
     city = "city"
     coordinates = "coordinates"
@@ -20,15 +19,15 @@
     type: Literal["city"]
     city: str
     country: str
     state: Optional[str] = None
 
 
 class CoordinatesModel(BaseModel):
-    type: Literal["coordinates"]
+    # type: Literal["coordinates"]
     latitude: float
     longitude: float
 
 
 class AddressModel(BaseModel):
     type: Literal["address"]
     address: str
@@ -45,30 +44,39 @@
     @validator("method")
     def method_is_valid(cls, v):
         if v not in CALCULATION_METHODS.values():
             raise ValueError(f"Invalid method: {v}")
         return v
 
 
+class Coordinates:
+    latitude: float
+    longitude: float
+
+    def __init__(self, latitude: float, longitude: float):
+        self.latitude = latitude
+        self.longitude = longitude
+
+
 # Create dataclass for config that has default values and can be loaded from file
 class Config:
-    location: City | Coordinates | Address
+    location: Coordinates
     time_format: TimeFormat = TimeFormat.twelve
     out_type: OutType = OutType.table
     method: int = 5
     next: bool = True
     prayers: list[str] = DEFAULT_PRAYERS
     is_error: bool = False
     error: Optional[str] = None
 
     def __init__(
         self,
         config_file: Path,
     ):
-        self.location = City("Cairo", "Egypt")
+        self.location = Coordinates(latitude=30, longitude=31)
         self.time_format = TimeFormat.twelve
         self.out_type = OutType.table
         self.method = 5
         self.next = True
         self.prayers = DEFAULT_PRAYERS
         self.is_error = False
         self.error = None
@@ -86,43 +94,50 @@
             try:
                 ConfigModel(**data)
             except Exception:
                 self.is_error = True
                 self.error = "Invalid config file structure"
                 return
 
-            location_type: str = data["location"]["type"]
-            if location_type == "city":
-                self.location = City(
-                    data["location"]["city"],
-                    data["location"]["country"],
-                    data["location"]["state"] if "state" in data["location"] else None,
-                )
-            elif location_type == "coordinates":
+            # location_type: str = data["location"]["type"]
+            # if location_type == "city":
+            #     self.location = City(
+            #         data["location"]["city"],
+            #         data["location"]["country"],
+            #         data["location"]["state"] if "state" in data["location"] else None,
+            #     )
+
+            try:
                 self.location = Coordinates(
-                    data["location"]["latitude"],
-                    data["location"]["longitude"],
-                )
-            elif location_type == "address":
-                self.location = Address(
-                    data["location"]["address"],
+                    latitude=data["location"]["latitude"],
+                    longitude=data["location"]["longitude"],
                 )
+            except KeyError:
+                self.is_error = True
+                self.error = "Invalid location data"
+                return
+            # elif location_type == "address":
+            #     self.location = Address(
+            #         data["location"]["address"],
+            #     )
 
             self.time_format = TimeFormat(data["time_format"])
             self.out_type = OutType(data["print_type"])
             self.method = data["method"]
             self.next = data["show_next"]
             self.prayers = data["prayers"]
         else:
             self.is_error = True
-            self.error = "Config file not found, please run `myprayer config` to create one."
+            self.error = (
+                "Config file not found, please run `myprayer config` to create one."
+            )
 
     def update(
         self,
-        location: Optional[City | Coordinates | Address],
+        location: Optional[Coordinates],
         time_format: Optional[TimeFormat] = None,
         out_type: Optional[OutType] = None,
         method: Optional[int] = None,
         next: Optional[bool] = None,
         prayers: Optional[list[str]] = None,
     ):
         if location is not None:
@@ -145,28 +160,14 @@
             "time_format": self.time_format.value,
             "print_type": self.out_type.value,
             "method": self.method,
             "show_next": self.next,
             "prayers": self.prayers,
         }
 
-        if isinstance(self.location, City):
-            config_data["location"] = {
-                "type": "city",
-                "city": self.location.city,
-                "country": self.location.country,
-                "state": self.location.state,
-            }
-        elif isinstance(self.location, Coordinates):
-            config_data["location"] = {
-                "type": "coordinates",
-                "latitude": self.location.latitude,
-                "longitude": self.location.longitude,
-            }
-        elif isinstance(self.location, Address):
-            config_data["location"] = {
-                "type": "address",
-                "address": self.location.address,
-            }
+        config_data["location"] = {
+            "latitude": self.location.latitude,
+            "longitude": self.location.longitude,
+        }
 
         with open(config_file, "w") as f:
             json.dump(config_data, f, indent=4)
```

### Comparing `myprayer-2.0.6/myprayer/cli/constants.py` & `myprayer-3.0.1/myprayer/cli/constants.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.6/myprayer/cli/enums.py` & `myprayer-3.0.1/myprayer/cli/enums.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.6/myprayer/cli/main.py` & `myprayer-3.0.1/myprayer/cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,58 @@
 #!/usr/bin/env python
 
 __author__ = "Youssef Aswad"
-__version__ = "2.0.5"
+__version__ = "3.0.1"
 
 import json
 from datetime import datetime
 
 import inquirer
 import typer
+import tzlocal
+from adhanpy.calculation import CalculationMethod
+from adhanpy.PrayerTimes import PrayerTimes
+from geopy import Nominatim
 from rich import print as rprint
 from rich.prompt import FloatPrompt, Prompt
 from rich.table import Table
 
-from myprayer.api.client import Client
-from myprayer.api.location_types import Address, City, Coordinates
 from myprayer.cli import utils
-from myprayer.cli.config import Config
+from myprayer.cli.config import Config, Coordinates
 from myprayer.cli.constants import (
     APP_NAME,
-    CACHE_DIR,
     CALCULATION_METHODS,
     CONFIG_FILE,
     LOCATION_TYPES,
     PRAYERS,
     TIME_FORMATS,
 )
+from myprayer.cli.day import Day, Prayer
 from myprayer.cli.enums import NextOutType, OutType, TimeFormat
 from myprayer.cli.output import DayOutput
 from myprayer.cli.utils import format_time_left
 
-
 app = typer.Typer(name=APP_NAME, pretty_exceptions_enable=False, help="MyPrayer CLI.")
 
 
 # TODO: Add option to display date in output
 # TODO: Emphasize next prayer in waybar output <span font_weight="bold">...</span>
 
 # Load config
 CONFIG = Config(CONFIG_FILE)
+SKIP = [prayer for prayer in PRAYERS if prayer not in CONFIG.prayers]
+# get current timezone
+tz = tzlocal.get_localzone()
 
 
-def get_client(city, country, address, latitude, longitude, method, force):
-    cache = None if force else CACHE_DIR
-    skip = [prayer for prayer in PRAYERS if prayer not in CONFIG.prayers]
-
-    location = None
-    if not any([city, country, address, latitude, longitude]):
-        if not CONFIG.location:
-            typer.echo(message="No location given.", err=True)
-            exit(1)
-    else:
-        if city and country:
-            location = City(city, country)
-        elif address:
-            location = Address(address)
-        elif latitude and longitude:
-            location = Coordinates(latitude, longitude)
-        else:
-            typer.echo(message="Invalid location.", err=True)
-            exit(1)
-
-    # if no location is given, use the one from config
-    location = location or CONFIG.location
+def get_coordinates(address: str):
+    nom = Nominatim(user_agent="myprayer")
+    location = nom.geocode(address)
 
-    return Client(location, method, skip=skip, cache_dir=cache)
+    return location.latitude, location.longitude  # type: ignore
 
 
 @app.command(name="list", help="List prayer times.")
 def list_prayers(
     city: str = typer.Option(
         None,
         "--city",
@@ -124,15 +109,15 @@
     year: int = typer.Option(
         None,
         "--year",
         "-y",
         help="Year",
         show_default="Current year",  # type: ignore
     ),
-    method: int = typer.Option(
+    method: CalculationMethod = typer.Option(
         CONFIG.method,
         "--method",
         "-M",
         help="Calculation method.",
         show_default=f"{utils.get_key(CALCULATION_METHODS, CONFIG.method)}",  # type: ignore
     ),
     time_format: TimeFormat = typer.Option(
@@ -155,21 +140,48 @@
     ),
     force: bool = typer.Option(False, "--force", "-f", help="Force update cache."),
 ):
     if CONFIG.is_error:
         typer.echo(message=f"[ERROR] {CONFIG.error}", err=True)
         exit(1)
 
-    client = get_client(city, country, address, latitude, longitude, method, force)
+    # client = get_client(city, country, address, latitude, longitude, method, force)
 
-    today = datetime.today()
+    if city and country:
+        latitude, longitude = get_coordinates(f"{city}, {country}")
+    elif address:
+        latitude, longitude = get_coordinates(address)
+    elif latitude and longitude:
+        pass
+    else:
+        latitude, longitude = CONFIG.location.latitude, CONFIG.location.longitude
+
+    today = datetime.today().replace(tzinfo=tz)
     day = day or today.day
     month = month or today.month
     year = year or today.year
-    day_data = client.get_day(day, month, year)
+    date = datetime(year, month, day)
+    # day_data = client.get_day(day, month, year)
+    prayer_times = PrayerTimes(
+        (latitude, longitude),
+        date,
+        CalculationMethod.EGYPTIAN,
+    )
+
+    print(date)
+    prayers = [
+        Prayer("Fajr", prayer_times.fajr.astimezone(tz)),
+        Prayer("Sunrise", prayer_times.sunrise.astimezone(tz)),
+        Prayer("Dhuhr", prayer_times.dhuhr.astimezone(tz)),
+        Prayer("Asr", prayer_times.asr.astimezone(tz)),
+        Prayer("Maghrib", prayer_times.maghrib.astimezone(tz)),
+        Prayer("Isha", prayer_times.isha.astimezone(tz)),
+    ]
+
+    day_data = Day(date, prayers, SKIP)
 
     output = DayOutput(day_data, time_format, next)
 
     if out_type == OutType.table:
         rprint(output.table())
     elif out_type == OutType.pretty:
         rprint(output.pretty())
@@ -212,15 +224,15 @@
     longitude: float = typer.Option(
         None,
         "--longitude",
         "-lon",
         help="Longitude.",
         show_default=False,
     ),
-    method: int = typer.Option(
+    method: CalculationMethod = typer.Option(
         CONFIG.method,
         "--method",
         "-M",
         help="Calculation method.",
         show_default=f"{utils.get_key(CALCULATION_METHODS, CONFIG.method)}",  # type: ignore
     ),
     out_type: NextOutType = typer.Option(
@@ -231,17 +243,46 @@
     ),
     force: bool = typer.Option(False, "--force", "-f", help="Force update cache."),
 ):
     if CONFIG.is_error:
         typer.echo(message=f"[ERROR] {CONFIG.error}", err=True)
         exit(1)
 
-    client = get_client(city, country, address, latitude, longitude, method, force)
+    if city and country:
+        latitude, longitude = get_coordinates(f"{city}, {country}")
+    elif address:
+        latitude, longitude = get_coordinates(address)
+    elif latitude and longitude:
+        pass
+    else:
+        latitude, longitude = CONFIG.location.latitude, CONFIG.location.longitude
+
+    today = datetime.today().replace(tzinfo=tz)
+    # day_data = client.get_day(day, month, year)
+    prayer_times = PrayerTimes(
+        (latitude, longitude),
+        today,
+        method,
+    )
+
+    prayers = [
+        Prayer("Fajr", prayer_times.fajr),
+        Prayer("Sunrise", prayer_times.sunrise),
+        Prayer("Dhuhr", prayer_times.dhuhr),
+        Prayer("Asr", prayer_times.asr),
+        Prayer("Maghrib", prayer_times.maghrib),
+        Prayer("Isha", prayer_times.isha),
+    ]
 
-    next_prayer = client.get_next_prayer()
+    next_prayer = None
+    day_data = Day(today, prayers, SKIP)
+    for prayer in day_data.prayers:
+        if not prayer.has_passed():
+            next_prayer = prayer
+            break
 
     if next_prayer is not None:
         time_left = format_time_left(next_prayer.time_left(), out_type)  # type: ignore
         if out_type == OutType.table:
             table = Table(show_header=True, header_style="bold magenta")
             table.add_column("Prayer")
             table.add_column("Time Left")
@@ -254,18 +295,14 @@
         elif out_type == OutType.json:
             out_json = {
                 "next": next_prayer.name,
                 "time_left": time_left,
             }
             print(json.dumps(out_json, indent=4))
         elif out_type == NextOutType.waybar:
-            day_data = client.get_day(
-                next_prayer.time.day, next_prayer.time.month, next_prayer.time.year
-            )
-
             tooltip_date = day_data.date.strftime("%A, %B %d")
             tooltip_data = "\n".join(
                 [
                     f"{prayer.name}: {prayer.time.strftime(TIME_FORMATS[CONFIG.time_format])}"
                     for prayer in day_data.prayers
                 ]
             )
@@ -291,63 +328,49 @@
             choices=LOCATION_TYPES,
             default=type(CONFIG.location).__name__,  # type: ignore
         ),
     ]
     loc_type_choice = inquirer.prompt(loc_type_question)
     loc_type: str = loc_type_choice["type"]  # type: ignore
 
-    location = None
+    latitude = 30
+    longitude = 31
     if loc_type == "City":
         city: str = Prompt.ask(
             "City",
-            default=(
-                CONFIG.location.city if isinstance(CONFIG.location, City) else None
-            ),  # type: ignore
         )
         country: str = Prompt.ask(
             "Country",
-            default=(
-                CONFIG.location.country if isinstance(CONFIG.location, City) else None
-            ),  # type: ignore
         )
         state: str = Prompt.ask(
             "State",
             default=None,  # type: ignore
         )
-        location = City(city, country, state)
+        location = f"{city}, {country}, {state}" if state else f"{city}, {country}"
+        latitude, longitude = get_coordinates(location)
 
     elif loc_type == "Coordinates":
         latitude: float = FloatPrompt.ask(
             "Latitude",
             default=(
-                CONFIG.location.latitude
-                if isinstance(CONFIG.location, Coordinates)
-                else None
+                CONFIG.location.latitude if CONFIG.location.latitude else None
             ),  # type: ignore
         )
         longitude: float = FloatPrompt.ask(
             "Longitude",
             default=(
-                CONFIG.location.longitude
-                if isinstance(CONFIG.location, Coordinates)
-                else None
+                CONFIG.location.longitude if CONFIG.location.longitude else None
             ),  # type: ignore
         )
-        location = Coordinates(latitude, longitude)
 
     elif loc_type == "Address":
         address: str = Prompt.ask(
             "Address",
-            default=(
-                CONFIG.location.address
-                if isinstance(CONFIG.location, Address)
-                else None
-            ),  # type: ignore
         )
-        location = Address(address)
+        latitude, longitude = get_coordinates(address)
 
     # city: str = Prompt.ask(
     #     "City",
     #     default=CONFIG.city,
     #     show_default=True if CONFIG.city else False,
     # )
     #
@@ -359,21 +382,22 @@
     # )
 
     # Prompt for calculation method
     method_question = [
         inquirer.List(
             "method",
             message="Select a calculation method:",
-            choices=CALCULATION_METHODS,
-            default=utils.get_key(CALCULATION_METHODS, CONFIG.method),  # type: ignore
+            choices=CalculationMethod.__members__.keys(),
+            default=utils.get_key(CalculationMethod.__members__, CalculationMethod(CONFIG.method)),  # type: ignore
         ),
     ]
-    method_choice = inquirer.prompt(method_question)
-    method: int = CALCULATION_METHODS[method_choice["method"]]  # type: ignore
+    
 
+    method_choice = inquirer.prompt(method_question)
+    method: int = CalculationMethod[method_choice["method"]].value  # type: ignore
     # Prompt for time format
     time_format: str = Prompt.ask(
         "Time format",
         choices=[TimeFormat.twelve, TimeFormat.twenty_four],
         default=TimeFormat.twelve.value,
     )
 
@@ -397,15 +421,15 @@
     prayers_choice = inquirer.prompt(prayers_question)
     prayers: list[str] = prayers_choice["prayers"]  # type: ignore
 
     # Prompt for next prayer option
     next = typer.confirm("Show next prayer?", default=True)
 
     CONFIG.update(
-        location=location,
+        location=Coordinates(latitude, longitude),
         time_format=TimeFormat(time_format),
         out_type=OutType(print_type),
         method=method,
         next=next,
         prayers=prayers,
     )
     CONFIG.save(CONFIG_FILE)
```

### Comparing `myprayer-2.0.6/myprayer/cli/output.py` & `myprayer-3.0.1/myprayer/cli/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rich.table import Table
 
-from myprayer.api.day import Day
 from myprayer.cli.constants import TIME_FORMATS
 from myprayer.cli.enums import OutType, TimeFormat
 from myprayer.cli.utils import format_time_left
+from myprayer.cli.day import Day
 
 
 class DayOutput:
     day: Day
     time_format: TimeFormat
     show_next: bool
```

### Comparing `myprayer-2.0.6/myprayer/cli/utils.py` & `myprayer-3.0.1/myprayer/cli/utils.py`

 * *Files identical despite different names*

### Comparing `myprayer-2.0.6/PKG-INFO` & `myprayer-3.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: myprayer
-Version: 2.0.6
+Version: 3.0.1
 Summary: A CLI tool to get prayer times
 Home-page: https://github.com/YoussefAswad/myprayer
 License: MIT
 Author: Youssef Aswad
 Author-email: youssefaswad@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: adhanpy (>=1.0.5,<2.0.0)
+Requires-Dist: geopy (>=2.4.1,<3.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: tzlocal (>=5.2,<6.0)
 Project-URL: Repository, https://github.com/YoussefAswad/myprayer
 Description-Content-Type: text/markdown
 
 # MyPrayer
 
 [![PyPI version](https://badge.fury.io/py/myprayer.svg)](https://badge.fury.io/py/myprayer)
 
@@ -39,14 +41,19 @@
 ## Dependencies
 
 - Python 3.8+
 - [Typer](https://github.com/tiangolo/typer) - CLI app framework
 - [Inquirer.py](https://github.com/magmax/python-inquirer) - user prompts
 - [Rich](https://github.com/willmcgugan/rich) - output formatting
 - [Requests](https://docs.python-requests.org/en/latest/) - HTTP client
+- [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
+- [geopy](https://geopy.readthedocs.io/en/stable/) - Geocoding library
+- [tzlocal](https://pypi.org/project/tzlocal/) - Local timezone
+- [pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
+
 
 ### Install
 
 ```bash
 pip install myprayer
 ```
 
@@ -132,25 +139,22 @@
         "Fajr",
         "Dhuhr",
         "Asr",
         "Maghrib",
         "Isha"
     ],
     "location": { // Default location used if no location is provided in command
-        "type": "city",
-        "city": "Cairo",
-        "country": "Egypt",
-        "state": null
+        "latitude": 30,
+        "longitude": 31,
     }
 }
 ```
 
 
 ## Credits
-- [Aladhan API](https://aladhan.com/) - for prayer time data
-- [aladhan-api](https://pypi.org/project/aladhan-api/) - i drew inspiration from this project
+- [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
 
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

