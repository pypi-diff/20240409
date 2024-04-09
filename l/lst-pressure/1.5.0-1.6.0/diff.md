# Comparing `tmp/lst-pressure-1.5.0.tar.gz` & `tmp/lst-pressure-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lst-pressure-1.5.0.tar", last modified: Fri Apr  5 13:18:44 2024, max compression
+gzip compressed data, was "lst-pressure-1.6.0.tar", last modified: Tue Apr  9 12:58:42 2024, max compression
```

## Comparing `lst-pressure-1.5.0.tar` & `lst-pressure-1.6.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/cli/apps/AppInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/cli/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/apps/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/cli/apps/aggregate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/apps/observables/
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/cli/apps/observables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/lst_pressure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lst/
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lst/LST.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/lst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lst/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/lst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lstcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendarDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/lstcalendar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lstindex/
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstindex/LSTIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstindex/LSTInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstindex/LSTIntervalType.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/lstindex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/observable/
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/observable/Observable.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/observable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/observation/
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/observation/Observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/observation/is_observable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/Sun.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/sun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/location_providers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/LocationProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/sun/location_providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/planets.json
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/normalize_intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/utils/normalize_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/utils/normalize_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/utils/time_conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/lstcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/lstcalendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendarDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/lstcalendar/test_LSTInterval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/observation/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/observation/test_Observation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/sun/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/sun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/sun/test_Sun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/test_lib_astral.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/test_lib_meerkat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/utils/test_normalize_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/utils/test_normalize_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/utils/test_time_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/cli/apps/AppInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/cli/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/apps/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/cli/apps/aggregate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/apps/observables/
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/cli/apps/observables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/lst_pressure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/lstpressure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lst/
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lst/LST.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lstcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendarDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lstcalendar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lstindex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstindex/LSTIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstindex/LSTInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstindex/LSTIntervalType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lstindex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/observable/
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/observable/Observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/observable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/observation/Observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/observation/is_observable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/Sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/location_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/LocationProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/location_providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/planets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/normalize_intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/utils/normalize_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/utils/normalize_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/utils/time_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/lstcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/tests/lstcalendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendarDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/lstcalendar/test_LSTInterval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/tests/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/observation/test_Observation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/tests/sun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/sun/test_Sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/test_lib_astral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/test_lib_meerkat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/utils/test_normalize_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/utils/test_normalize_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/utils/test_time_conversions.py
```

### Comparing `lst-pressure-1.5.0/LICENSE` & `lst-pressure-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/PKG-INFO` & `lst-pressure-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lst-pressure
-Version: 1.5.0
+Version: 1.6.0
 Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
 Home-page: https://github.com/ska-sa/lst-pressure
 Author: Zach Smith
 Author-email: zsmith@sarao.ac.za
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lst-pressure-1.5.0/README.md` & `lst-pressure-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/cli/__init__.py` & `lst-pressure-1.6.0/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,8 +94,8 @@
         parser.print_help()
         return
 
     # Otherwise execute the application
     app.parse(args).exe()
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/cli/apps/AppInterface.py` & `lst-pressure-1.6.0/cli/apps/AppInterface.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/cli/apps/aggregate/__init__.py` & `lst-pressure-1.6.0/cli/apps/aggregate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,8 +181,8 @@
     except Exception as e:
         raise e
 
 
 __all__ = ["parse_sql_query", "Aggregate", "execute_csvsql", "execute_csvlook"]
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/cli/apps/observables/__init__.py` & `lst-pressure-1.6.0/cli/apps/observables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 filter_mapping = {
     I.NIGHT.name: I.NIGHT,
     I.SUNRISE_SUNSET.name: I.SUNRISE_SUNSET,
     I.ALL_DAY.name: I.ALL_DAY,
     I.SUNSET_SUNRISE.name: I.SUNSET_SUNRISE,
     I.OBSERVATION_WINDOW.name: I.OBSERVATION_WINDOW,
+    I.DAY.name: I.DAY,
 }
 
 
 def kebab_to_snake(input_string):
     return re.sub(r"-", "_", input_string)
 
 
@@ -282,8 +283,8 @@
         if self.output:
             with open(self.output, "w") as f:
                 f.write(output_string)
         else:
             print(output_string)
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/conf/__init__.py` & `lst-pressure-1.6.0/conf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,8 @@
     def PY_ENV(self, value):
         self._py_env = value
 
 
 __all__ = ["Conf", "LogLevel"]
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/logger/__init__.py` & `lst-pressure-1.6.0/logger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 def error(*args, **kwargs):
     print("ERROR", *args, **kwargs, file=sys.stderr)
 
 
 __all__ = ["debug", "info", "warn", "error"]
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/lst_pressure.egg-info/PKG-INFO` & `lst-pressure-1.6.0/lst_pressure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lst-pressure
-Version: 1.5.0
+Version: 1.6.0
 Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
 Home-page: https://github.com/ska-sa/lst-pressure
 Author: Zach Smith
 Author-email: zsmith@sarao.ac.za
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lst-pressure-1.5.0/lst_pressure.egg-info/SOURCES.txt` & `lst-pressure-1.6.0/lst_pressure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/__init__.py` & `lst-pressure-1.6.0/lstpressure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     "Sun",
     "utils",
     "LSTConf",
     "LocationProviderType",
 ]
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/lstpressure/lst/LST.py` & `lst-pressure-1.6.0/lstpressure/lst/LST.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observables.py` & `lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observables.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observations.py` & `lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observations.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 def calculate_constraints(row) -> list[I]:
     constraints = []
     if row["night_obs"] == "Yes":
         constraints.append(I.NIGHT)
     elif row["avoid_sunrise_sunset"] == "Yes":
         constraints.append(I.SUNRISE_SUNSET)
         constraints.append(I.SUNSET_SUNRISE)
+        constraints.append(I.DAY)
 
     # If neither night_obs nor avoid_sunrise_sunset was selected
     if not constraints:
         constraints.append(I.ALL_DAY)
+        constraints.append(I.DAY)
 
     return constraints
 
 
 @track_total_runtime
 def calculate_observations(dataFrame, observation_filter) -> Tuple[Observation]:
     try:
```

### Comparing `lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendar.py` & `lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendar.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendarDate.py` & `lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendarDate.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/lstindex/LSTIndex.py` & `lst-pressure-1.6.0/lstpressure/lstindex/LSTIndex.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/lstindex/LSTInterval.py` & `lst-pressure-1.6.0/lstpressure/lstindex/LSTInterval.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     return (start, end)
 
 
 @decorate_all(track_total_runtime)
 class LSTInterval:
     def __init__(
         self,
-        start: float,
-        end: float,
+        start: float,  # lst start
+        end: float,  # lst end
         start_utc: datetime | float,
         end_utc: datetime | float,
         parent: Optional[Union[LSTCalendarDate, Observation]] = None,
         dt: Optional[datetime] = None,
         type: Optional[LSTIntervalType] = None,
         sun: Optional[Sun] = None,
         tomorrow_sun: Optional[Sun] = None,
```

### Comparing `lst-pressure-1.5.0/lstpressure/lstindex/LSTIntervalType.py` & `lst-pressure-1.6.0/lstpressure/lstindex/LSTIntervalType.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,12 @@
     SUNRISE_SUNSET : LSTIntervalType
         An interval type representing the period from sunrise to sunset.
     SUNSET_SUNRISE : LSTIntervalType
         An interval type representing the period from sunset to sunrise.
     """
 
     ALL_DAY = auto()
+    DAY = auto()
     NIGHT = auto()
     OBSERVATION_WINDOW = auto()
     SUNRISE_SUNSET = auto()
     SUNSET_SUNRISE = auto()
```

### Comparing `lst-pressure-1.5.0/lstpressure/observable/Observable.py` & `lst-pressure-1.6.0/lstpressure/observable/Observable.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/observation/Observation.py` & `lst-pressure-1.6.0/lstpressure/observation/Observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,23 @@
             The ending value of the LST window.
         utc_constraints : list[LSTInterval]
             The UTC constraints for the observation block represented as a list of LSTInterval values. Defaults to 0.
         """
         self.id = id
         self.lst_window_start = lst_window_start
         self.lst_window_end = lst_window_end
-        self.utc_constraints = (
-            utc_constraints
-            if utc_constraints and isinstance(utc_constraints, list)
-            else [utc_constraints]
+        self.utc_constraints = list(
+            filter(
+                lambda item: item,
+                (
+                    utc_constraints
+                    if utc_constraints and isinstance(utc_constraints, list)
+                    else [utc_constraints]
+                ),
+            )
         )
         self.proposal_id = proposal_id
         self._duration = duration if duration else 0
         self._cal: Optional[LSTCalendar] = None  # Reference to the calendar
         self._intervals = []
         self._intervals.append(
             LSTInterval(
```

### Comparing `lst-pressure-1.5.0/lstpressure/observation/is_observable.py` & `lst-pressure-1.6.0/lstpressure/observation/is_observable.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,23 +36,26 @@
         (Optional) The longitude for the observation in the format 'D:M:S'. Defaults to 21:26:38.0 (for ASTRAL provider).
 
     Returns
     -------
     bool
         True if the observation is observable within the specified parameters, False otherwise.
     """
-
     # TODO fix me. Some import problem
     from ..lstcalendar import LSTCalendar
 
     yyyymmdd_end = yyyymmdd_end if yyyymmdd_end else yyyymmdd_start
 
     # Create an LSTCalendar instance if not provided
     calendar = (
         lstCalendar
         if lstCalendar
         else LSTCalendar(
-            yyyymmdd_start, yyyymmdd_end, latitude=latitude, longitude=longitude, provider=provider
+            yyyymmdd_start,
+            yyyymmdd_end,
+            latitude=latitude,
+            longitude=longitude,
+            provider=provider,
         )
     )
 
     return bool(observation.observables(calendar))
```

### Comparing `lst-pressure-1.5.0/lstpressure/sun/Sun.py` & `lst-pressure-1.6.0/lstpressure/sun/Sun.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py` & `lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,33 +28,72 @@
         today_sun = Sun(today, latitude, longitude, provider=AstralProvider)
         today_sunrise_lst = today_sun.sunrise_lst
         today_sunrise_utc = today_sun.sunrise
         today_sunset_lst = today_sun.sunset_lst
         today_sunset_utc = today_sun.sunset
         today_dusk_lst = today_sun.dusk_lst
         today_dusk_utc = today_sun.dusk
+        today_dawn_lst = today_sun.dawn_lst
+        today_dawn_utc = today_sun.dawn
 
         tomorrow = today + timedelta(days=1)
         tomorrow_sun = Sun(tomorrow, latitude, longitude, provider=AstralProvider)
         tomorrow_dawn_lst = tomorrow_sun.dawn_lst
         tomorrow_dawn_utc = tomorrow_sun.dawn
         tomorrow_sunrise_lst = tomorrow_sun.sunrise_lst
         tomorrow_sunrise_utc = tomorrow_sun.sunrise
         tomorrow_sunset_lst = tomorrow_sun.sunset_lst
         tomorrow_sunset_utc = tomorrow_sun.sunset
+        tomorrow_dusk_utc = tomorrow_sun.dusk
+        tomorrow_dusk_lst = tomorrow_sun.dusk_lst
 
         result = []
 
         # ALL DAY
         result.append(
             LSTInterval(
-                0, 24, None, None, obj, today, LSTIntervalType.ALL_DAY, today_sun, tomorrow_sun
+                0,
+                24,
+                None,
+                None,
+                obj,
+                today,
+                LSTIntervalType.ALL_DAY,
+                today_sun,
+                tomorrow_sun,
             )
         )
 
+        # DAY
+        DAY = LSTInterval(
+            *normalize_interval(today_dawn_lst, today_dusk_lst),
+            today_dawn_utc.strftime("%H:%M"),
+            today_dusk_utc.strftime("%H:%M"),
+            obj,
+            today,
+            LSTIntervalType.DAY,
+            today_sun,
+            tomorrow_sun,
+        )
+        result.append(DAY)
+        if DAY.end > 24:
+            result.append(
+                LSTInterval(
+                    0,
+                    tomorrow_dusk_lst,
+                    today_dawn_utc.strftime("%H:%M"),
+                    today_dusk_utc.strftime("%H:%M"),
+                    obj,
+                    today,
+                    LSTIntervalType.DAY,
+                    today_sun,
+                    tomorrow_sun,
+                )
+            )
+
         # SUNRISE_SUNSET
         SUNRISE_SUNSET = LSTInterval(
             *normalize_interval(today_sunrise_lst, today_sunset_lst),
             today_sunrise_utc.strftime("%H:%M"),
             today_sunset_utc.strftime("%H:%M"),
             obj,
             today,
@@ -65,15 +104,15 @@
         result.append(SUNRISE_SUNSET)
         if SUNRISE_SUNSET.end > 24:
             result.append(
                 LSTInterval(
                     0,
                     tomorrow_sunset_lst,
                     today_sunrise_utc.strftime("%H:%M"),
-                    tomorrow_sunset_utc.strftime("%H:%M"),
+                    today_sunset_utc.strftime("%H:%M"),
                     obj,
                     today,
                     LSTIntervalType.SUNRISE_SUNSET,
                     today_sun,
                     tomorrow_sun,
                 )
             )
@@ -92,15 +131,15 @@
         result.append(SUNSET_SUNRISE)
 
         if SUNSET_SUNRISE.end > 24:
             result.append(
                 LSTInterval(
                     0,
                     tomorrow_sunrise_lst,
-                    0,
+                    today_sunset_utc.strftime("%H:%M"),
                     tomorrow_sunrise_utc.strftime("%H:%M"),
                     obj,
                     today,
                     LSTIntervalType.SUNSET_SUNRISE,
                     today_sun,
                     tomorrow_sun,
                 )
@@ -120,15 +159,15 @@
         result.append(NIGHT)
 
         if NIGHT.end > 24:
             result.append(
                 LSTInterval(
                     0,
                     tomorrow_dawn_lst,
-                    0,
+                    today_dusk_utc.strftime("%H:%M"),
                     tomorrow_dawn_utc.strftime("%H:%M"),
                     obj,
                     today,
                     LSTIntervalType.NIGHT,
                     today_sun,
                     tomorrow_sun,
                 )
```

### Comparing `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py` & `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py` & `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py` & `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,17 @@
             set_utc = DateTimeUtil.lst2ut(
                 sun_lst["lstSet"], AstroUtil.MKAT_POSITION["longitude"], date
             )
             rise_utc = DateTimeUtil.lst2ut(
                 sun_lst["lstRise"], AstroUtil.MKAT_POSITION["longitude"], date
             )
 
-            set_date = date.replace(hour=int(set_utc), minute=int((set_utc - int(set_utc)) * 60))
+            set_date = date.replace(
+                hour=int(set_utc), minute=int((set_utc - int(set_utc)) * 60)
+            )
             rise_date = date.replace(
                 hour=int(rise_utc), minute=int((rise_utc - int(rise_utc)) * 60)
             )
 
             return {
                 "dawn": None,
                 "dusk": None,
@@ -75,18 +77,53 @@
         tomorrow_sunset_utc = tomorrow_sun.sunset
 
         result = []
 
         # ALL DAY
         result.append(
             LSTInterval(
-                0, 24, None, None, obj, today, LSTIntervalType.ALL_DAY, today_sun, tomorrow_sun
+                0,
+                24,
+                None,
+                None,
+                obj,
+                today,
+                LSTIntervalType.ALL_DAY,
+                today_sun,
+                tomorrow_sun,
             )
         )
 
+        # DAY
+        DAY = LSTInterval(
+            *normalize_interval(today_sunrise_lst, today_sunset_lst),
+            today_sunrise_utc.strftime("%H:%M"),
+            today_sunset_utc.strftime("%H:%M"),
+            obj,
+            today,
+            LSTIntervalType.DAY,
+            today_sun,
+            tomorrow_sun,
+        )
+        result.append(DAY)
+        if DAY.end > 24:
+            result.append(
+                LSTInterval(
+                    0,
+                    tomorrow_sunset_lst,
+                    today_sunrise_utc.strftime("%H:%M"),
+                    today_sunset_utc.strftime("%H:%M"),
+                    obj,
+                    today,
+                    LSTIntervalType.DAY,
+                    today_sun,
+                    tomorrow_sun,
+                )
+            )
+
         # SUNRISE_SUNSET
         SUNRISE_SUNSET = LSTInterval(
             *normalize_interval(today_sunrise_lst, today_sunset_lst),
             today_sunrise_utc.strftime("%H:%M"),
             today_sunset_utc.strftime("%H:%M"),
             obj,
             today,
@@ -97,15 +134,15 @@
         result.append(SUNRISE_SUNSET)
         if SUNRISE_SUNSET.end > 24:
             result.append(
                 LSTInterval(
                     0,
                     tomorrow_sunset_lst,
                     today_sunrise_utc.strftime("%H:%M"),
-                    tomorrow_sunset_utc.strftime("%H:%M"),
+                    today_sunset_utc.strftime("%H:%M"),
                     obj,
                     today,
                     LSTIntervalType.SUNRISE_SUNSET,
                     today_sun,
                     tomorrow_sun,
                 )
             )
@@ -124,15 +161,15 @@
         result.append(SUNSET_SUNRISE)
 
         if SUNSET_SUNRISE.end > 24:
             result.append(
                 LSTInterval(
                     0,
                     tomorrow_sunrise_lst,
-                    0,
+                    today_sunset_utc.strftime("%H:%M"),
                     tomorrow_sunrise_utc.strftime("%H:%M"),
                     obj,
                     today,
                     LSTIntervalType.SUNSET_SUNRISE,
                     today_sun,
                     tomorrow_sun,
                 )
@@ -152,15 +189,15 @@
         result.append(NIGHT)
 
         if NIGHT.end > 24:
             result.append(
                 LSTInterval(
                     0,
                     tomorrow_sunrise_lst,
-                    0,
+                    today_sunset_utc.strftime("%H:%M"),
                     tomorrow_sunrise_utc.strftime("%H:%M"),
                     obj,
                     today,
                     LSTIntervalType.NIGHT,
                     today_sun,
                     tomorrow_sun,
                 )
@@ -172,17 +209,17 @@
 @track_total_runtime
 def calc_sun_rise_set(
     ra: float | str,
     dec: float | str,
     latitude: float | str,
     thresh_hold: float | str,
 ):
-    cos_h = -(AstroUtil.sind(thresh_hold) + AstroUtil.sind(latitude) * AstroUtil.sind(dec)) / (
-        AstroUtil.cosd(latitude) * AstroUtil.cosd(dec)
-    )
+    cos_h = -(
+        AstroUtil.sind(thresh_hold) + AstroUtil.sind(latitude) * AstroUtil.sind(dec)
+    ) / (AstroUtil.cosd(latitude) * AstroUtil.cosd(dec))
     obj = {
         "never_up": False,
         "circumpolar": False,
         "lstRise": 0,
         "lstSet": 0,
     }
     ha = AstroUtil.acosd(cos_h) / 15.0
```

### Comparing `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py` & `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/utils/normalize_coordinates.py` & `lst-pressure-1.6.0/lstpressure/utils/normalize_coordinates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/utils/normalize_date.py` & `lst-pressure-1.6.0/lstpressure/utils/normalize_date.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/lstpressure/utils/time_conversions.py` & `lst-pressure-1.6.0/lstpressure/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/perf/__init__.py` & `lst-pressure-1.6.0/perf/__init__.py`

 * *Files identical despite different names*

```diff
@@ -106,8 +106,8 @@
 
     return decorate
 
 
 __all__ = ["monitor_perf", "track_total_runtime", "decorate_all"]
 
 # Automatically added by katversion
-__version__ = '1.5.0'
+__version__ = '1.6.0'
```

### Comparing `lst-pressure-1.5.0/setup.py` & `lst-pressure-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendar.py` & `lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendar.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendarDate.py` & `lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendarDate.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/lstcalendar/test_LSTInterval.py` & `lst-pressure-1.6.0/tests/lstcalendar/test_LSTInterval.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/sun/test_Sun.py` & `lst-pressure-1.6.0/tests/sun/test_Sun.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/test_lib_astral.py` & `lst-pressure-1.6.0/tests/test_lib_meerkat.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     duration,
     dt_range,
     observables_count,
 ):
     assert is_observable(
         Observation("~", lst_window_start, lst_window_end, utc_constraints, duration),
         *dt_range,
-        provider=LocationProviderType.ASTRAL,
+        provider=LocationProviderType.MEERKAT,
     ) is bool(observables_count)
 
 
 @pytest.mark.parametrize(
     "lst_window_start, lst_window_end, utc_constraints, duration, dt_range, observables_count",
     tests,
 )
@@ -62,15 +62,18 @@
 ):
     assert (
         len(
             sorted(
                 Observation(
                     "~", lst_window_start, lst_window_end, utc_constraints, duration
                 ).observables(
-                    lstcalendar=LSTCalendar(*dt_range, provider=LocationProviderType.ASTRAL)
+                    lstcalendar=LSTCalendar(
+                        *dt_range,
+                        provider=LocationProviderType.MEERKAT,
+                    )
                 )
             )
         )
         == observables_count
     )
 
 
@@ -85,14 +88,14 @@
     duration,
     dt_range,
     observables_count,
 ):
     assert (
         len(
             sorted(
-                LSTCalendar(*dt_range, provider=LocationProviderType.ASTRAL).observables(
+                LSTCalendar(*dt_range, provider=LocationProviderType.MEERKAT).observables(
                     [Observation("~", lst_window_start, lst_window_end, utc_constraints, duration)]
                 )
             )
         )
         == observables_count
     )
```

### Comparing `lst-pressure-1.5.0/tests/test_lib_meerkat.py` & `lst-pressure-1.6.0/tests/test_lib_astral.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,19 +37,24 @@
     lst_window_start,
     lst_window_end,
     utc_constraints,
     duration,
     dt_range,
     observables_count,
 ):
-    assert is_observable(
-        Observation("~", lst_window_start, lst_window_end, utc_constraints, duration),
+    observation = Observation(
+        "~", lst_window_start, lst_window_end, utc_constraints, duration
+    )
+    o = is_observable(
+        observation,
         *dt_range,
-        provider=LocationProviderType.MEERKAT,
-    ) is bool(observables_count)
+        provider=LocationProviderType.ASTRAL,
+    )
+    observable = o
+    assert observable is bool(observables_count)
 
 
 @pytest.mark.parametrize(
     "lst_window_start, lst_window_end, utc_constraints, duration, dt_range, observables_count",
     tests,
 )
 def test_observation_observables(
@@ -63,16 +68,15 @@
     assert (
         len(
             sorted(
                 Observation(
                     "~", lst_window_start, lst_window_end, utc_constraints, duration
                 ).observables(
                     lstcalendar=LSTCalendar(
-                        *dt_range,
-                        provider=LocationProviderType.MEERKAT,
+                        *dt_range, provider=LocationProviderType.ASTRAL
                     )
                 )
             )
         )
         == observables_count
     )
 
@@ -85,17 +89,17 @@
     lst_window_start,
     lst_window_end,
     utc_constraints,
     duration,
     dt_range,
     observables_count,
 ):
-    assert (
-        len(
-            sorted(
-                LSTCalendar(*dt_range, provider=LocationProviderType.MEERKAT).observables(
-                    [Observation("~", lst_window_start, lst_window_end, utc_constraints, duration)]
-                )
-            )
-        )
-        == observables_count
+    cal = LSTCalendar(*dt_range, provider=LocationProviderType.ASTRAL)
+    observation = Observation(
+        "~",
+        lst_window_start,
+        lst_window_end,
+        utc_constraints,
+        duration,
     )
+    observables = cal.observables([observation])
+    assert len(sorted(observables)) == observables_count
```

### Comparing `lst-pressure-1.5.0/tests/utils/test_normalize_coordinates.py` & `lst-pressure-1.6.0/tests/utils/test_normalize_coordinates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/utils/test_normalize_dates.py` & `lst-pressure-1.6.0/tests/utils/test_normalize_dates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.5.0/tests/utils/test_time_conversions.py` & `lst-pressure-1.6.0/tests/utils/test_time_conversions.py`

 * *Files identical despite different names*

