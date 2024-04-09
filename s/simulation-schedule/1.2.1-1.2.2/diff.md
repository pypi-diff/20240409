# Comparing `tmp/simulation-schedule-1.2.1.tar.gz` & `tmp/simulation-schedule-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation-schedule-1.2.1.tar", last modified: Mon Dec 11 10:58:05 2023, max compression
+gzip compressed data, was "simulation-schedule-1.2.2.tar", last modified: Tue Apr  9 17:29:36 2024, max compression
```

## Comparing `simulation-schedule-1.2.1.tar` & `simulation-schedule-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 emmettgreen   (504) staff       (20)        0 2023-12-11 10:58:05.617527 simulation-schedule-1.2.1/
--rw-r--r--   0 emmettgreen   (504) staff       (20)     2012 2023-12-11 09:09:23.000000 simulation-schedule-1.2.1/AUTHORS.rst
--rw-r--r--   0 emmettgreen   (504) staff       (20)     6542 2023-12-11 09:09:23.000000 simulation-schedule-1.2.1/HISTORY.rst
--rw-r--r--   0 emmettgreen   (504) staff       (20)     1099 2023-12-11 09:09:23.000000 simulation-schedule-1.2.1/LICENSE.txt
--rw-r--r--   0 emmettgreen   (504) staff       (20)      147 2023-12-11 09:09:23.000000 simulation-schedule-1.2.1/MANIFEST.in
--rw-r--r--   0 emmettgreen   (504) staff       (20)     3426 2023-12-11 10:58:05.617466 simulation-schedule-1.2.1/PKG-INFO
--rw-r--r--   0 emmettgreen   (504) staff       (20)     2288 2023-12-11 09:09:23.000000 simulation-schedule-1.2.1/README.rst
-drwxr-xr-x   0 emmettgreen   (504) staff       (20)        0 2023-12-11 10:58:05.616697 simulation-schedule-1.2.1/schedule/
--rw-r--r--   0 emmettgreen   (504) staff       (20)    33324 2023-12-11 10:35:59.000000 simulation-schedule-1.2.1/schedule/__init__.py
--rw-r--r--   0 emmettgreen   (504) staff       (20)        0 2023-12-11 09:09:24.000000 simulation-schedule-1.2.1/schedule/py.typed
--rw-r--r--   0 emmettgreen   (504) staff       (20)       93 2023-12-11 10:58:05.617730 simulation-schedule-1.2.1/setup.cfg
--rw-r--r--   0 emmettgreen   (504) staff       (20)     1667 2023-12-11 10:51:41.000000 simulation-schedule-1.2.1/setup.py
-drwxr-xr-x   0 emmettgreen   (504) staff       (20)        0 2023-12-11 10:58:05.617234 simulation-schedule-1.2.1/simulation_schedule.egg-info/
--rw-r--r--   0 emmettgreen   (504) staff       (20)     3426 2023-12-11 10:58:05.000000 simulation-schedule-1.2.1/simulation_schedule.egg-info/PKG-INFO
--rw-r--r--   0 emmettgreen   (504) staff       (20)      305 2023-12-11 10:58:05.000000 simulation-schedule-1.2.1/simulation_schedule.egg-info/SOURCES.txt
--rw-r--r--   0 emmettgreen   (504) staff       (20)        1 2023-12-11 10:58:05.000000 simulation-schedule-1.2.1/simulation_schedule.egg-info/dependency_links.txt
--rw-r--r--   0 emmettgreen   (504) staff       (20)        9 2023-12-11 10:58:05.000000 simulation-schedule-1.2.1/simulation_schedule.egg-info/top_level.txt
--rw-r--r--   0 emmettgreen   (504) staff       (20)    46579 2023-12-11 09:09:24.000000 simulation-schedule-1.2.1/test_schedule.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-09 17:29:36.887441 simulation-schedule-1.2.2/
+-rw-r--r--   0 ruben      (501) staff       (20)     2012 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/AUTHORS.rst
+-rw-r--r--   0 ruben      (501) staff       (20)     6542 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/HISTORY.rst
+-rw-r--r--   0 ruben      (501) staff       (20)     1099 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/LICENSE.txt
+-rw-r--r--   0 ruben      (501) staff       (20)      147 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/MANIFEST.in
+-rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-09 17:29:36.887382 simulation-schedule-1.2.2/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)     2288 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/README.rst
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-09 17:29:36.886548 simulation-schedule-1.2.2/schedule/
+-rw-r--r--   0 ruben      (501) staff       (20)    33413 2024-04-09 16:02:23.000000 simulation-schedule-1.2.2/schedule/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/schedule/py.typed
+-rw-r--r--   0 ruben      (501) staff       (20)       93 2024-04-09 17:29:36.887619 simulation-schedule-1.2.2/setup.cfg
+-rw-r--r--   0 ruben      (501) staff       (20)     1599 2024-04-09 17:29:10.000000 simulation-schedule-1.2.2/setup.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-09 17:29:36.887163 simulation-schedule-1.2.2/simulation_schedule.egg-info/
+-rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      305 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        1 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        9 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/top_level.txt
+-rw-r--r--   0 ruben      (501) staff       (20)    46579 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/test_schedule.py
```

### Comparing `simulation-schedule-1.2.1/AUTHORS.rst` & `simulation-schedule-1.2.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.1/HISTORY.rst` & `simulation-schedule-1.2.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.1/LICENSE.txt` & `simulation-schedule-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.1/PKG-INFO` & `simulation-schedule-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: simulation-schedule
-Version: 1.2.1
-Summary: This is a fork of the popular 'schedule' package, with the option to run the scheduler in non-realtime mode.
-Home-page: https://github.com/emmettgreen/schedule
-Download-URL: https://github.com/dbader/schedule/tarball/1.2.1
-Author: Daniel Bader, Ruben van Eldik
+Version: 1.2.2
+Summary: Job scheduling for humans.
+Home-page: https://github.com/dbader/schedule
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.2
+Author: Daniel Bader
+Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `simulation-schedule-1.2.1/README.rst` & `simulation-schedule-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.1/schedule/__init__.py` & `simulation-schedule-1.2.2/schedule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -827,15 +827,16 @@
             if (self.next_run - now).days >= 7:
                 self.next_run -= self.period
 
         # Calculations happen in the configured timezone, but to execute the schedule we
         # need to know the next_run time in the system time. So we convert back to naive local
         if self.at_time_zone is not None:
             self.next_run = self._normalize_preserve_timestamp(self.next_run)
-            self.next_run = self.next_run.astimezone().replace(tzinfo=None)
+            # This line has to be commented out so that timezones can be used properly
+            # self.next_run = self.next_run.astimezone().replace(tzinfo=None)
 
     # Usually when normalization of a timestamp causes the timestamp to change,
     # it preserves the moment in time and changes the local timestamp.
     # This method applies pytz normalization but preserves the local timestamp, in fact changing the moment in time.
     def _normalize_preserve_timestamp(
         self, input: datetime.datetime
     ) -> datetime.datetime:
```

### Comparing `simulation-schedule-1.2.1/setup.py` & `simulation-schedule-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 from setuptools import setup
 
 
-SCHEDULE_VERSION = "1.2.1"
+SCHEDULE_VERSION = "1.2.2"
 SCHEDULE_DOWNLOAD_URL = "https://github.com/dbader/schedule/tarball/" + SCHEDULE_VERSION
 
 
 def read_file(filename):
     """
     Read a utf8 encoded text file and return its contents.
     """
@@ -15,19 +15,20 @@
 
 
 setup(
     name="simulation-schedule",
     packages=["schedule"],
     package_data={"schedule": ["py.typed"]},
     version=SCHEDULE_VERSION,
-    description="This is a fork of the popular 'schedule' package, with the option to run the scheduler in non-realtime mode.",
+    description="Job scheduling for humans.",
     long_description=read_file("README.rst"),
     license="MIT",
-    author="Daniel Bader, Ruben van Eldik",
-    url="https://github.com/emmettgreen/schedule",
+    author="Daniel Bader",
+    author_email="mail@dbader.org",
+    url="https://github.com/dbader/schedule",
     download_url=SCHEDULE_DOWNLOAD_URL,
     keywords=[
         "schedule",
         "periodic",
         "jobs",
         "scheduling",
         "clockwork",
```

### Comparing `simulation-schedule-1.2.1/simulation_schedule.egg-info/PKG-INFO` & `simulation-schedule-1.2.2/simulation_schedule.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: simulation-schedule
-Version: 1.2.1
-Summary: This is a fork of the popular 'schedule' package, with the option to run the scheduler in non-realtime mode.
-Home-page: https://github.com/emmettgreen/schedule
-Download-URL: https://github.com/dbader/schedule/tarball/1.2.1
-Author: Daniel Bader, Ruben van Eldik
+Version: 1.2.2
+Summary: Job scheduling for humans.
+Home-page: https://github.com/dbader/schedule
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.2
+Author: Daniel Bader
+Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `simulation-schedule-1.2.1/test_schedule.py` & `simulation-schedule-1.2.2/test_schedule.py`

 * *Files identical despite different names*

