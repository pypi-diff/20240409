# Comparing `tmp/kivy_garden_invisible_magnet-0.1.0.tar.gz` & `tmp/kivy_garden_invisible_magnet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_garden_invisible_magnet-0.1.0.tar", max compression
+gzip compressed data, was "kivy_garden_invisible_magnet-0.1.1.tar", max compression
```

## Comparing `kivy_garden_invisible_magnet-0.1.0.tar` & `kivy_garden_invisible_magnet-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      733 2024-04-07 21:06:21.244653 kivy_garden_invisible_magnet-0.1.0/README.md
--rw-r--r--   0        0        0      414 2024-04-07 21:09:08.250433 kivy_garden_invisible_magnet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      157 2024-04-07 19:53:11.791446 kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/__init__.py
--rw-r--r--   0        0        0      985 2024-04-07 20:34:32.330110 kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_install.py
--rw-r--r--   0        0        0      892 2024-04-07 19:53:11.791446 kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_main.py
--rw-r--r--   0        0        0     3380 2024-04-07 19:53:11.791446 kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_pos_and_size.py
--rw-r--r--   0        0        0     2059 2024-04-07 19:53:11.795446 kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_pos_only.py
--rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 kivy_garden_invisible_magnet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      733 2024-04-07 21:06:21.244653 kivy_garden_invisible_magnet-0.1.1/README.md
+-rw-r--r--   0        0        0      432 2024-04-09 05:10:45.792393 kivy_garden_invisible_magnet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2024-04-09 02:00:10.645579 kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/__init__.py
+-rw-r--r--   0        0        0     1792 2024-04-09 01:59:34.770953 kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_install.py
+-rw-r--r--   0        0        0      864 2024-04-08 09:30:05.079785 kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_main.py
+-rw-r--r--   0        0        0     3380 2024-04-07 19:53:11.791446 kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_pos_and_size.py
+-rw-r--r--   0        0        0     2059 2024-04-07 19:53:11.795446 kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_pos_only.py
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 kivy_garden_invisible_magnet-0.1.1/PKG-INFO
```

### Comparing `kivy_garden_invisible_magnet-0.1.0/README.md` & `kivy_garden_invisible_magnet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_main.py` & `kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     magnetize(widget, speed=speed)
     widget._unmagnetize = unmagnetize
 
 
 def unmagnetize(widget):
     widget = widget.__self__
     if not is_magnetized(widget):
-        raise ValueError('Not magnetized')
+        return
     widget._unmagnetize(widget)
     del widget._unmagnetize
```

### Comparing `kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_pos_and_size.py` & `kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_pos_and_size.py`

 * *Files identical despite different names*

### Comparing `kivy_garden_invisible_magnet-0.1.0/src/kivy_garden/invisible_magnet/_pos_only.py` & `kivy_garden_invisible_magnet-0.1.1/src/kivy_garden/invisible_magnet/_pos_only.py`

 * *Files identical despite different names*

### Comparing `kivy_garden_invisible_magnet-0.1.0/PKG-INFO` & `kivy_garden_invisible_magnet-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-garden-invisible-magnet
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Nattōsai Mitō
 Author-email: flow4re2c@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

