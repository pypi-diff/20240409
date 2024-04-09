# Comparing `tmp/timetree-exporter-0.1.0.tar.gz` & `tmp/timetree-exporter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetree-exporter-0.1.0.tar", last modified: Sat Apr  6 09:00:24 2024, max compression
+gzip compressed data, was "timetree-exporter-0.2.0.tar", last modified: Tue Apr  9 15:12:59 2024, max compression
```

## Comparing `timetree-exporter-0.1.0.tar` & `timetree-exporter-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.723033 timetree-exporter-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.719032 timetree-exporter-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.719032 timetree-exporter-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/.github/workflows/release-please.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.719032 timetree-exporter-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-06 09:00:24.723033 timetree-exporter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.715032 timetree-exporter-0.1.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.719032 timetree-exporter-0.1.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/assets/images/copy-response.png
--rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/assets/images/prepare-for-signin.png
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.719032 timetree-exporter-0.1.0/responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/responses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:00:24.723033 timetree-exporter-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.723033 timetree-exporter-0.1.0/timetree_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/timetree_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/timetree_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/timetree_exporter/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/timetree_exporter/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-06 09:00:20.000000 timetree-exporter-0.1.0/timetree_exporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:00:24.723033 timetree-exporter-0.1.0/timetree_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-06 09:00:24.000000 timetree-exporter-0.1.0/timetree_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-06 09:00:24.000000 timetree-exporter-0.1.0/timetree_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:00:24.000000 timetree-exporter-0.1.0/timetree_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-06 09:00:24.000000 timetree-exporter-0.1.0/timetree_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:00:24.000000 timetree-exporter-0.1.0/timetree_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 09:00:24.000000 timetree-exporter-0.1.0/timetree_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.593331 timetree-exporter-0.2.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/assets/images/copy-response.png
+-rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/assets/images/prepare-for-signin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/responses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/timetree_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/timetree_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/top_level.txt
```

### Comparing `timetree-exporter-0.1.0/.github/workflows/pylint.yml` & `timetree-exporter-0.2.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.1.0/.github/workflows/python-publish.yml` & `timetree-exporter-0.2.0/.github/workflows/python-publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `timetree-exporter-0.1.0/LICENSE` & `timetree-exporter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.1.0/PKG-INFO` & `timetree-exporter-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
 Project-URL: Changelog, https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
@@ -73,15 +73,15 @@
 
 # Roadmap of the properties mapping to iCal
 - [ ] **ID**
 - [ ] **Primary ID**
 - [ ] **Calendar ID**
 - [x] **UUID**
 - [ ] **Category**
-- [ ] **Type**
+- [x] **Type**
 - [ ] **Author ID**
 - [ ] **Author Type**
 - [x] **Title**
 - [x] **All Day**
 - [x] **Start At**
 - [x] **Start Timezone**
 - [x] **End At**
@@ -93,15 +93,15 @@
 - [x] **URL**
 - [x] **Note**
 - [ ] **Lunar**
 - [ ] **Attendees**
 - [x] **Recurrences**
 - [ ] **Recurring UUID**
 - [x] **Alerts**
-- [ ] **Parent ID**
+- [x] **Parent ID**
 - [ ] **Link Object ID**
 - [ ] **Link Object ID String**
 - [ ] **Row Order**
 - [ ] **Attachment**
 - [ ] **Like Count**
 - [ ] **Files**
 - [ ] **Deactivated At**
```

### Comparing `timetree-exporter-0.1.0/README.md` & `timetree-exporter-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 # Roadmap of the properties mapping to iCal
 - [ ] **ID**
 - [ ] **Primary ID**
 - [ ] **Calendar ID**
 - [x] **UUID**
 - [ ] **Category**
-- [ ] **Type**
+- [x] **Type**
 - [ ] **Author ID**
 - [ ] **Author Type**
 - [x] **Title**
 - [x] **All Day**
 - [x] **Start At**
 - [x] **Start Timezone**
 - [x] **End At**
@@ -75,15 +75,15 @@
 - [x] **URL**
 - [x] **Note**
 - [ ] **Lunar**
 - [ ] **Attendees**
 - [x] **Recurrences**
 - [ ] **Recurring UUID**
 - [x] **Alerts**
-- [ ] **Parent ID**
+- [x] **Parent ID**
 - [ ] **Link Object ID**
 - [ ] **Link Object ID String**
 - [ ] **Row Order**
 - [ ] **Attachment**
 - [ ] **Like Count**
 - [ ] **Files**
 - [ ] **Deactivated At**
```

### Comparing `timetree-exporter-0.1.0/assets/images/copy-response.png` & `timetree-exporter-0.2.0/assets/images/copy-response.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.1.0/assets/images/prepare-for-signin.png` & `timetree-exporter-0.2.0/assets/images/prepare-for-signin.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.1.0/pyproject.toml` & `timetree-exporter-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.1.0/responses/README.md` & `timetree-exporter-0.2.0/responses/README.md`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.1.0/timetree_exporter/__main__.py` & `timetree-exporter-0.2.0/timetree_exporter/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,12 +46,14 @@
         continue
 
     # Add events to calendar
     for event in events:
         time_tree_event = TimeTreeEvent.from_dict(event)
         formatter = ICalEventFormatter(time_tree_event)
         iCalEvent = formatter.to_ical()
+        if iCalEvent is None:
+            continue
         cal.add_component(iCalEvent)
 
 # Write calendar to file
 with open(args.output, "wb") as f:  # Path Traversal Vulnerability if on a server
     f.write(cal.to_ical())
```

### Comparing `timetree-exporter-0.1.0/timetree_exporter/event.py` & `timetree-exporter-0.2.0/timetree_exporter/event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module provides the TimeTreeEvent class for representing TimeTree events."""
 
+import dataclasses
+
 
 class TimeTreeEvent:
     """TimeTree event class"""
 
     # pylint: disable=too-many-instance-attributes
 
     def __init__(
@@ -20,14 +22,16 @@
         end_at: int,
         all_day: bool,
         start_timezone: str,
         end_timezone: str,
         location_lat: str,
         location_lon: str,
         location: str,
+        parent_id: str,
+        event_type: int,
     ):
         # pylint: disable=too-many-arguments
         # pylint: disable=too-many-locals
         self.uuid = uuid
         self.title = title
         self.created_at = created_at
         self.updated_at = updated_at
@@ -39,14 +43,16 @@
         self.start_at = start_at
         self.start_timezone = start_timezone
         self.end_at = end_at
         self.end_timezone = end_timezone
         self.all_day = all_day
         self.alerts = alerts
         self.recurrences = recurrences
+        self.parent_id = parent_id
+        self.event_type = event_type
 
     @classmethod
     def from_dict(cls, event_data: dict):
         """Create TimeTreeEvent object from JSON data"""
         return cls(
             uuid=event_data.get("uuid"),
             title=event_data.get("title"),
@@ -60,11 +66,21 @@
             start_at=event_data.get("start_at"),
             start_timezone=event_data.get("start_timezone"),
             end_at=event_data.get("end_at"),
             end_timezone=event_data.get("end_timezone"),
             all_day=event_data.get("all_day"),
             alerts=event_data.get("alerts"),
             recurrences=event_data.get("recurrences"),
+            parent_id=event_data.get("parent_id"),
+            event_type=event_data.get("type"),
         )
 
     def __str__(self):
         return self.title
+
+
+@dataclasses.dataclass
+class TimeTreeEventType(enumerate):
+    """TimeTree event type enumeration"""
+
+    NORMAL = 0
+    BIRTHDAY = 1
```

### Comparing `timetree-exporter-0.1.0/timetree_exporter/formatter.py` & `timetree-exporter-0.2.0/timetree_exporter/formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """
 
 from datetime import datetime, timedelta
 from icalendar import Event, vRecur, vDate, vDatetime, vGeo
 from icalendar.prop import vDDDLists
 from icalendar.parser import Contentline
 from dateutil import tz
-from timetree_exporter.event import TimeTreeEvent
+from timetree_exporter.event import TimeTreeEvent, TimeTreeEventType
+from timetree_exporter.utils import convert_timestamp_to_datetime
 
 
 class ICalEventFormatter:
     """
     Class for formatting TimeTree events into iCalendar format.
     """
 
@@ -29,25 +30,25 @@
         """Return the title of the event."""
         return self.time_tree_event.title
 
     @property
     def created(self):
         """Return the creation time of the event."""
         return vDatetime(
-            datetime.fromtimestamp(
-                self.time_tree_event.created_at / 1000, tz.gettz("UTC")
+            convert_timestamp_to_datetime(
+                self.time_tree_event.created_at / 1000, tz.tzutc()
             )
         )
 
     @property
     def last_modify(self):
         """Return the last modification time of the event."""
         return vDatetime(
-            datetime.fromtimestamp(
-                self.time_tree_event.updated_at / 1000, tz.gettz("UTC")
+            convert_timestamp_to_datetime(
+                self.time_tree_event.updated_at / 1000, tz.tzutc()
             )
         )
 
     @property
     def description(self):
         """Return the note of the event."""
         return self.time_tree_event.note if self.time_tree_event.note != "" else None
@@ -74,32 +75,37 @@
         )
 
     @property
     def url(self):
         """Return the URL of the event."""
         return self.time_tree_event.url if self.time_tree_event.url != "" else None
 
+    @property
+    def related_to(self):
+        """Return the parent ID of the event."""
+        return self.time_tree_event.parent_id
+
     def get_datetime(self, is_start_time):
         """Return the start or end time of the event."""
         if is_start_time:
             time = self.time_tree_event.start_at
             timezone = self.time_tree_event.start_timezone
         else:
             time = self.time_tree_event.end_at
             timezone = self.time_tree_event.end_timezone
 
         if self.time_tree_event.all_day:
             return vDate(
-                datetime.fromtimestamp(
+                convert_timestamp_to_datetime(
                     time / 1000,
                     tz.gettz(timezone),
                 )
             )
         return vDatetime(
-            datetime.fromtimestamp(
+            convert_timestamp_to_datetime(
                 time / 1000,
                 tz.gettz(timezone),
             )
         )
 
     @property
     def dtstart(self):
@@ -133,32 +139,40 @@
             elif name.lower() == "exdate" or name.lower() == "rdate":
                 event.add(name, vDDDLists.from_ical(value), parameters)
             else:
                 raise ValueError(f"Unknown recurrence type: {name}")
 
     def to_ical(self) -> Event:
         """Return the iCal event."""
+        if (
+            self.time_tree_event.event_type == TimeTreeEventType.BIRTHDAY
+        ):  # Skip if event is a birthday
+            return None
+
         event = Event()
 
         event.add("uid", self.uid)
         event.add("summary", self.summary)
-        event.add("dtstamp", datetime.now(tz.tzutc()))
+        # event.add("dtstamp", datetime.now(tz.tzutc()))
+        event.add("dtstamp", datetime.fromtimestamp(0, tz.tzutc()))
         event.add("created", self.created)
         event.add("last-modify", self.last_modify)
         event.add("dtstart", self.dtstart)
         event.add("dtend", self.dtend)
 
         if self.location:
             event.add("location", self.location)
         if self.geo:
             event.add("geo", self.geo)
         if self.url:
             event.add("url", self.url)
         if self.description:
             event.add("description", self.description)
+        if self.related_to:
+            event.add("related-to", self.related_to)
 
         for alert in self.alerts:
             event.add_component(alert)
 
         self.add_recurrences(event)
 
         return event
```

### Comparing `timetree-exporter-0.1.0/timetree_exporter.egg-info/PKG-INFO` & `timetree-exporter-0.2.0/timetree_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
 Project-URL: Changelog, https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
@@ -73,15 +73,15 @@
 
 # Roadmap of the properties mapping to iCal
 - [ ] **ID**
 - [ ] **Primary ID**
 - [ ] **Calendar ID**
 - [x] **UUID**
 - [ ] **Category**
-- [ ] **Type**
+- [x] **Type**
 - [ ] **Author ID**
 - [ ] **Author Type**
 - [x] **Title**
 - [x] **All Day**
 - [x] **Start At**
 - [x] **Start Timezone**
 - [x] **End At**
@@ -93,15 +93,15 @@
 - [x] **URL**
 - [x] **Note**
 - [ ] **Lunar**
 - [ ] **Attendees**
 - [x] **Recurrences**
 - [ ] **Recurring UUID**
 - [x] **Alerts**
-- [ ] **Parent ID**
+- [x] **Parent ID**
 - [ ] **Link Object ID**
 - [ ] **Link Object ID String**
 - [ ] **Row Order**
 - [ ] **Attachment**
 - [ ] **Like Count**
 - [ ] **Files**
 - [ ] **Deactivated At**
```

### Comparing `timetree-exporter-0.1.0/timetree_exporter.egg-info/SOURCES.txt` & `timetree-exporter-0.2.0/timetree_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

