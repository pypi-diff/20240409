# Comparing `tmp/unbirthday-1.0.tar.gz` & `tmp/unbirthday-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbirthday-1.0.tar", last modified: Tue Apr  9 06:23:14 2024, max compression
+gzip compressed data, was "unbirthday-1.0.1.tar", last modified: Tue Apr  9 07:09:52 2024, max compression
```

## Comparing `unbirthday-1.0.tar` & `unbirthday-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 06:23:14.504763 unbirthday-1.0/
--rw-rw-rw-   0        0        0     7978 2024-04-09 06:23:14.504763 unbirthday-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7878 2024-04-06 10:57:27.000000 unbirthday-1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 06:23:14.505766 unbirthday-1.0/setup.cfg
--rw-rw-rw-   0        0        0      344 2024-04-09 06:19:15.000000 unbirthday-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 06:23:14.488270 unbirthday-1.0/unbirthday/
--rw-rw-rw-   0        0        0      177 2024-04-09 06:02:18.000000 unbirthday-1.0/unbirthday/__init__.py
--rw-rw-rw-   0        0        0     6346 2024-04-05 22:59:31.000000 unbirthday-1.0/unbirthday/unbirthday.py
-drwxrwxrwx   0        0        0        0 2024-04-09 06:23:14.503765 unbirthday-1.0/unbirthday.egg-info/
--rw-rw-rw-   0        0        0     7978 2024-04-09 06:23:14.000000 unbirthday-1.0/unbirthday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-09 06:23:14.000000 unbirthday-1.0/unbirthday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 06:23:14.000000 unbirthday-1.0/unbirthday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 06:23:14.000000 unbirthday-1.0/unbirthday.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 07:09:52.226200 unbirthday-1.0.1/
+-rw-rw-rw-   0        0        0     7978 2024-04-09 07:09:52.226200 unbirthday-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7876 2024-04-09 07:05:19.000000 unbirthday-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 07:09:52.226200 unbirthday-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      346 2024-04-09 07:09:43.000000 unbirthday-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:09:52.210584 unbirthday-1.0.1/unbirthday/
+-rw-rw-rw-   0        0        0      177 2024-04-09 06:02:18.000000 unbirthday-1.0.1/unbirthday/__init__.py
+-rw-rw-rw-   0        0        0     6346 2024-04-05 22:59:31.000000 unbirthday-1.0.1/unbirthday/unbirthday.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:09:52.226200 unbirthday-1.0.1/unbirthday.egg-info/
+-rw-rw-rw-   0        0        0     7978 2024-04-09 07:09:52.000000 unbirthday-1.0.1/unbirthday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-09 07:09:52.000000 unbirthday-1.0.1/unbirthday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:09:52.000000 unbirthday-1.0.1/unbirthday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 07:09:52.000000 unbirthday-1.0.1/unbirthday.egg-info/top_level.txt
```

### Comparing `unbirthday-1.0/PKG-INFO` & `unbirthday-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: unbirthday
-Version: 1.0
-Description-Content-Type: text/markdown
-
 # Unbirthday (Calculator)
 
 ## Introduction
 
 Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday. This project is a tribute to the show *Alice's Wonderland Bakery (2022-2024)*.
 
 ## Inspiration
@@ -17,15 +12,19 @@
 
 By offering functions to calculate and manage unbirthdays, this project invites users to explore the whimsy of unbirthday celebrations in their own programming adventures. Whether you're curious about how many unbirthdays have passed since a certain date or eager to find out when your next unbirthday will be, the Unbirthday module adds a playful twist to date calculations.
 
 Join us in celebrating the spirit of Wonderland by incorporating a bit of unbirthday magic into your Python projects. Let's all savor the joy of everyday celebrations and the wonder of unexpected surprises. After all, as the Hatter famously said, "A very merry unbirthday to you!"
 
 ## Installation
 
-To use Unbirthday, download the `unbirthday.py` file and place it in your project directory.
+You can install the `unbirthday` module using pip:
+
+```bash
+pip install unbirthday
+```
 
 ## Usage
 
 You can import functions from the `unbirthday` module using the following syntax:
 
 ```python
 from unbirthday import add_ordinal_indicator, get_todays_date, years_passed, your_current_day_on_earth, calculate_unbirthday, find_startdate_unbirthday, find_enddate_unbirthday
@@ -215,8 +214,8 @@
   - **Systic**
   - [**Clay**](https://www.youtube.com/@DaClayCrew)
   - [**Ghosty**](https://discord.com/users/1056973970534051840)
   - [**Sam**](https://www.youtube.com/@ENHAPPIFY)
 
 **And to all of the Wonderland community**
 
-Thank you all for being part of this wonderful community!
+Thank you all for being part of this wonderful community!
```

### Comparing `unbirthday-1.0/README.md` & `unbirthday-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: unbirthday
+Version: 1.0.1
+Description-Content-Type: text/markdown
+
 # Unbirthday (Calculator)
 
 ## Introduction
 
 Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday. This project is a tribute to the show *Alice's Wonderland Bakery (2022-2024)*.
 
 ## Inspiration
@@ -12,15 +17,19 @@
 
 By offering functions to calculate and manage unbirthdays, this project invites users to explore the whimsy of unbirthday celebrations in their own programming adventures. Whether you're curious about how many unbirthdays have passed since a certain date or eager to find out when your next unbirthday will be, the Unbirthday module adds a playful twist to date calculations.
 
 Join us in celebrating the spirit of Wonderland by incorporating a bit of unbirthday magic into your Python projects. Let's all savor the joy of everyday celebrations and the wonder of unexpected surprises. After all, as the Hatter famously said, "A very merry unbirthday to you!"
 
 ## Installation
 
-To use Unbirthday, download the `unbirthday.py` file and place it in your project directory.
+You can install the `unbirthday` module using pip:
+
+```bash
+pip install unbirthday
+```
 
 ## Usage
 
 You can import functions from the `unbirthday` module using the following syntax:
 
 ```python
 from unbirthday import add_ordinal_indicator, get_todays_date, years_passed, your_current_day_on_earth, calculate_unbirthday, find_startdate_unbirthday, find_enddate_unbirthday
@@ -210,8 +219,8 @@
   - **Systic**
   - [**Clay**](https://www.youtube.com/@DaClayCrew)
   - [**Ghosty**](https://discord.com/users/1056973970534051840)
   - [**Sam**](https://www.youtube.com/@ENHAPPIFY)
 
 **And to all of the Wonderland community**
 
-Thank you all for being part of this wonderful community!
+Thank you all for being part of this wonderful community!
```

### Comparing `unbirthday-1.0/unbirthday/unbirthday.py` & `unbirthday-1.0.1/unbirthday/unbirthday.py`

 * *Files identical despite different names*

### Comparing `unbirthday-1.0/unbirthday.egg-info/PKG-INFO` & `unbirthday-1.0.1/unbirthday.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbirthday
-Version: 1.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # Unbirthday (Calculator)
 
 ## Introduction
 
 Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday. This project is a tribute to the show *Alice's Wonderland Bakery (2022-2024)*.
@@ -17,15 +17,19 @@
 
 By offering functions to calculate and manage unbirthdays, this project invites users to explore the whimsy of unbirthday celebrations in their own programming adventures. Whether you're curious about how many unbirthdays have passed since a certain date or eager to find out when your next unbirthday will be, the Unbirthday module adds a playful twist to date calculations.
 
 Join us in celebrating the spirit of Wonderland by incorporating a bit of unbirthday magic into your Python projects. Let's all savor the joy of everyday celebrations and the wonder of unexpected surprises. After all, as the Hatter famously said, "A very merry unbirthday to you!"
 
 ## Installation
 
-To use Unbirthday, download the `unbirthday.py` file and place it in your project directory.
+You can install the `unbirthday` module using pip:
+
+```bash
+pip install unbirthday
+```
 
 ## Usage
 
 You can import functions from the `unbirthday` module using the following syntax:
 
 ```python
 from unbirthday import add_ordinal_indicator, get_todays_date, years_passed, your_current_day_on_earth, calculate_unbirthday, find_startdate_unbirthday, find_enddate_unbirthday
```

