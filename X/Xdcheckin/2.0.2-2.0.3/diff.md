# Comparing `tmp/Xdcheckin-2.0.2.tar.gz` & `tmp/Xdcheckin-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xdcheckin-2.0.2.tar", last modified: Sat Apr  6 04:04:23 2024, max compression
+gzip compressed data, was "Xdcheckin-2.0.3.tar", last modified: Tue Apr  9 02:48:56 2024, max compression
```

## Comparing `Xdcheckin-2.0.2.tar` & `Xdcheckin-2.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.175032 Xdcheckin-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.179033 Xdcheckin-2.0.2/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.179033 Xdcheckin-2.0.2/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.179033 Xdcheckin-2.0.2/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/util/chaoxing_captcha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.769287 Xdcheckin-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-09 02:48:56.000000 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 02:48:56.000000 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 02:48:56.000000 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 02:48:56.000000 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 02:48:56.000000 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 02:48:56.000000 Xdcheckin-2.0.3/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.773287 Xdcheckin-2.0.3/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.773287 Xdcheckin-2.0.3/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33281 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.773287 Xdcheckin-2.0.3/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:56.777287 Xdcheckin-2.0.3/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-09 02:48:50.000000 Xdcheckin-2.0.3/src/xdcheckin/util/chaoxing_captcha.py
```

### Comparing `Xdcheckin-2.0.2/LICENSE` & `Xdcheckin-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/PKG-INFO` & `Xdcheckin-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.2
+Version: 2.0.3
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `Xdcheckin-2.0.2/README.md` & `Xdcheckin-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/pyproject.toml` & `Xdcheckin-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 5864 6368 6563 6b69 6e22 0d0a 7665   "Xdcheckin"..ve
-00000080: 7273 696f 6e20 3d20 2232 2e30 2e32 220d  rsion = "2.0.2".
+00000080: 7273 696f 6e20 3d20 2232 2e30 2e33 220d  rsion = "2.0.3".
 00000090: 0a61 7574 686f 7273 203d 205b 0d0a 097b  .authors = [...{
 000000a0: 6e61 6d65 203d 2022 5061 6972 6d61 6e22  name = "Pairman"
 000000b0: 2c20 656d 6169 6c20 3d20 2270 6169 726d  , email = "pairm
 000000c0: 616e 786c 7240 676d 6169 6c2e 636f 6d22  anxlr@gmail.com"
 000000d0: 7d0d 0a5d 0d0a 7265 6164 6d65 203d 2022  }..]..readme = "
 000000e0: 5245 4144 4d45 2e6d 6422 0d0a 6465 7363  README.md"..desc
 000000f0: 7269 7074 696f 6e20 3d20 2243 6861 6f78  ription = "Chaox
```

### Comparing `Xdcheckin-2.0.2/src/Xdcheckin.egg-info/PKG-INFO` & `Xdcheckin-2.0.3/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.2
+Version: 2.0.3
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `Xdcheckin-2.0.2/src/Xdcheckin.egg-info/SOURCES.txt` & `Xdcheckin-2.0.3/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/core/chaoxing.py` & `Xdcheckin-2.0.3/src/xdcheckin/core/chaoxing.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 			"User-Agent": "Mozilla/5.0 (Linux; Android 10; K) Apple"
 				      "WebKit/537.36 (KHTML, like Gecko) Chrome"
 				      "/120.0.0.0 Mobile Safari/537.36 com.chao"
 				      "xing.mobile/ChaoXingStudy_3_6.1.0_androi"
 				      "d_phone_906_100"
 		},
 		"requests_cache_enabled": True,
-		"chaoxing_course_get_activities_courses_limit": 36,
+		"chaoxing_course_get_activities_courses_limit": 32,
 		"chaoxing_course_get_activities_workers": 16,
 		"chaoxing_checkin_location_address_override_maxlen": 0,
 		"chaoxing_checkin_location_randomness": True
 	}
 
 	def __init__(
 		self, username: str = "", password: str = "", cookies = None,
@@ -846,15 +846,15 @@
 				"params": params
 			}
 		except Exception as e:
 			if type(e) is AssertionError:
 				match = search(r"validate_([0-9A-Fa-f]{32})", str(e))
 				if match:
 					params["enc2"] = match.group(1)
-				msg = f"Checkin failure. {dumps(params), str(e)}"
+				msg = f"Checkin failure. {params, str(e)}"
 			else:
 				msg = str(e)
 			return False, {
 				"msg": msg,
 				"params": params
 			}
 
@@ -869,15 +869,15 @@
 		"""
 		try:
 			thread_analysis = Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			presign = self.checkin_do_presign(activity = activity, course = {"class_id": str(info["clazzId"])})
-			assert presign[0], f"Presign failure. {dumps(activity), dumps(presign)}"
+			assert presign[0], f"Presign failure. {activity, presign}"
 			if presign[0] == 2:
 				return True, {
 					"msg": "Checkin success. (Already checked in.)",
 					"params": "",
 					"captcha": ""
 				}
 			location_new = {
@@ -915,15 +915,15 @@
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			course, location_new = {"class_id": str(info["clazzId"])}, {}
 			thread_location = Thread(target = _get_location)
 			thread_location.start()
 			presign = self.checkin_do_presign(activity = activity, course = course)
-			assert presign[0], f"Presign failure. {dumps(activity), dumps(presign)}"
+			assert presign[0], f"Presign failure. {activity, presign}"
 			if presign[0] == 2:
 				return True, {
 					"msg": "Checkin success. (Already checked in.)",
 					"params": "",
 					"captcha": ""
 				}
 			location_new = {
```

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/core/locations.py` & `Xdcheckin-2.0.3/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/core/xidian.py` & `Xdcheckin-2.0.3/src/xdcheckin/core/xidian.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/server.py` & `Xdcheckin-2.0.3/src/xdcheckin/server/server.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/activity.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/activity.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/classroom.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/curriculum.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/curriculum.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,15 @@
             let bgn = timetable[v.period_begin - 1].slice(0, 5);
             let end = timetable[v.period_end - 1].slice(6, 11);
             td.appendChild(document.createTextNode(`${v.day}  ` +
                 `${bgn}-${end}`));
 
         });
         td = tr.appendChild(newElement("td"));
-        if (!with_live)
+        if (!lesson.livestreams)
             lesson.locations.forEach((v, i) => {
                 if (i)
                     td.appendChild(newElement("br"));
                 td.appendChild(document.createTextNode(v));
             });
         else
             lesson.livestreams.forEach((v, i) => {
```

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/g_classroom_urls.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/location.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/login.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/misc.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/player.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/style.css` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/style.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+body {
+	touch-action: manipulation;
+}
+
+#xdcheckin-title-div {
+	font-family: sans-serif;
+	font-weight: bold;
+	font-size:48px;
+}
+
 div {
 	font-size:22px;
 	font-family: sans-serif;
 }
 .div-center {
 	justify-content: center;
 	align-items: center;
@@ -44,13 +54,7 @@
 }
 .captcha-input {
 	justify-content: center;
 	align-items: center;
 	display: flex;
 	width: 70%;
 }
-
-#xdcheckin-title-div {
-	font-family: sans-serif;
-	font-weight: bold;
-	font-size:48px;
-}
```

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/static/util.js` & `Xdcheckin-2.0.3/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/server/templates/index.html` & `Xdcheckin-2.0.3/src/xdcheckin/server/templates/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!DOCTYPE html>
-<html>
+<html lang="en">
 	<title>Xdcheckin</title>
 
 	<meta charset="UTF-8">
-	<meta name="viewport" content="initial-scale=0.7, user-scalable=no">
-	<link rel="shortcut icon" href="#"/>
-	<link rel="stylesheet" href="static/style.css"/>
-	<link rel="stylesheet" href="https://g.alicdn.com/apsara-media-box/imp-web-player/2.20.2/skins/default/aliplayer-min.css"/>
+	<meta name="viewport" content="initial-scale=0.7">
+	<link rel="shortcut icon" href="#">
+	<link rel="stylesheet" href="static/style.css">
+	<link rel="stylesheet" href="https://g.alicdn.com/apsara-media-box/imp-web-player/2.20.2/skins/default/aliplayer-min.css">
 	<script src="https://g.alicdn.com/apsara-media-box/imp-web-player/2.20.2/aliplayer-h5-min.js"></script>
 	<script src="static/g_classroom_urls.js"></script>
 	<script src="static/g_locations.js"></script>
 	<script src="static/global.js"></script>
 	<script src="static/util.js"></script>
 	<script src="static/misc.js"></script>
 	<script src="static/login.js"></script>
@@ -34,27 +34,27 @@
 					getActivities().then(hideOtherLists('activities-list-div'));
 				else
 					displayTag('activities-list-div');
 			" style="display: none">Activities</button>
 		</div>
 		<div id="activities-checkin-captcha-div" style="display: none">
 			<div id="activities-checkin-captcha-container-div" class="captcha-container-div">
-				<img id="activities-checkin-captcha-img" class="captcha-img" src="">
-				<img id="activities-checkin-captcha-small-img" class="captcha-small-img" src="">
+				<img id="activities-checkin-captcha-img" class="captcha-img" alt="activities-checkin-captcha-img" src=",">
+				<img id="activities-checkin-captcha-small-img" class="captcha-small-img" alt="activities-checkin-captcha-small-img" src=",">
 			</div>
 			<div class="div-center">
 				<input id="activities-checkin-captcha-input" class="captcha-input" type="range" min="0" max="320" step="1" value="0">
 				&emsp;
 				<button id="activities-checkin-captcha-button">Verify</button>
 			</div>
 		</div>
 		<div id="ids-login-captcha-div" style="display: none">
 			<div id="ids-login-captcha-container-div" class="captcha-container-div">
-				<img id="ids-login-captcha-img" class="captcha-img" src="">
-				<img id="ids-login-captcha-small-img" class="captcha-small-img" src="">
+				<img id="ids-login-captcha-img" class="captcha-img" alt="ids-login-captcha-img" src=",">
+				<img id="ids-login-captcha-small-img" class="captcha-small-img" alt="ids-login-captcha-small-img" src=",">
 			</div>
 			<div class="div-center">
 				<input id="ids-login-captcha-input" class="captcha-input" type="range" min="0" max="280" step="1" value="0">
 				&emsp;
 				<button id="ids-login-captcha-button">Verify</button>
 			</div>
 		</div>
@@ -85,16 +85,16 @@
 				chaoxingCheckinQrcodeWrapper(g_players[0].tag, 1, 'player0-scanresult-div');
 				onclickCooldown(this.id);
 			" style="display: none">Scan</button>
 		</div>
 		<div id="player0-div"></div>
 		<div id="player0-checkin-captcha-div" style="display: none">
 			<div id="player0-checkin-captcha-container-div" class="captcha-container-div">
-				<img id="player0-checkin-captcha-img" class="captcha-img" src="">
-				<img id="player0-checkin-captcha-small-img" class="captcha-small-img" src="">
+				<img id="player0-checkin-captcha-img" class="captcha-img" alt="player0-checkin-captcha-img" src=",">
+				<img id="player0-checkin-captcha-small-img" class="captcha-small-img" alt="player0-checkin-captcha-small-img" src=",">
 			</div>
 			<div class="div-center">
 				<input id="player0-checkin-captcha-input" class="captcha-input" type="range" min="0" max="320" step="1" value="0">
 				&emsp;
 				<button id="player0-checkin-captcha-button">Verify</button>
 			</div>
 		</div>
@@ -141,36 +141,36 @@
 			" style="display: none">Scan</button>
 		</div>
 		<div id="camera-div" style="display: none">
 			<video id="camera-video" width="640" height="480" autoplay></video>
 		</div>
 		<div id="camera-checkin-captcha-div" style="display: none">
 			<div id="camera-checkin-captcha-container-div" class="captcha-container-div">
-				<img id="camera-checkin-captcha-img" class="captcha-img" src="">
-				<img id="camera-checkin-captcha-small-img" class="captcha-small-img" src="">
+				<img id="camera-checkin-captcha-img" class="captcha-img" alt="camera-checkin-captcha-img" src=",">
+				<img id="camera-checkin-captcha-small-img" class="captcha-small-img" alt="camera-checkin-captcha-small-img" src=",">
 			</div>
 			<div class="div-center">
 				<input id="camera-checkin-captcha-input" class="captcha-input" type="range" min="0" max="320" step="1" value="0">
 				&emsp;
 				<button id="camera-checkin-captcha-button">Verify</button>
 			</div>
 		</div>
 		<div id="camera-scanresult-div" class="scanresult-div" style="display: none"></div>
 
 		<div id="footer-div" class="div-center">
 			<a id="footer-link-a" href="https://github.com/Pairman/Xdcheckin">Xdcheckin</a>
 			&emsp;(C) 2024 Pairman
 		</div>
-	</body>
 
-	<script>
-		checkEula();
-		xdcheckinCheckUpdates();
-		if (localStorage.getItem("username"))
-			promptLogin(auto = true);
-		listLocations();
-		listClassrooms();
-		resizePlayers().then(enablePlayers);
-		window.onresize = resizePlayers;
-		enableCamera();
-	</script>
+		<script>
+			checkEula();
+			xdcheckinCheckUpdates();
+			if (localStorage.getItem("username"))
+				promptLogin(auto = true);
+			listLocations();
+			listClassrooms();
+			resizePlayers().then(enablePlayers);
+			window.onresize = resizePlayers;
+			enableCamera();
+		</script>
+	</body>
 </html>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 Login Logout Curriculum Location Activities
-[Image][Image]
+[activities-checkin-captcha-img][activities-checkin-captcha-small-img]
 [Unknown INPUT type]  Verify
-[Image][Image]
+[ids-login-captcha-img][ids-login-captcha-small-img]
 [Unknown INPUT type]  Verify
 Xdcheckin
  
 Classroom Play All Stop All
 
 PPPPTTVViiddeeoo   Play Stop Unmute Mute Scan
-[Image][Image]
+[player0-checkin-captcha-img][player0-checkin-captcha-small-img]
 [Unknown INPUT type]  Verify
 TTeeaacchheerrTTrraacckk   Play Stop Unmute Mute
 TTeeaacchheerrFFuullll   Play Stop Unmute Mute
 SSttuuddeennttFFuullll   Play Stop Unmute Mute
 CCaammeerraa   On Off Scan
-[Image][Image]
+[camera-checkin-captcha-img][camera-checkin-captcha-small-img]
 [Unknown INPUT type]  Verify
 _X_d_c_h_e_c_k_i_n  (C) 2024 Pairman
```

### Comparing `Xdcheckin-2.0.2/src/xdcheckin/util/chaoxing_captcha.py` & `Xdcheckin-2.0.3/src/xdcheckin/util/chaoxing_captcha.py`

 * *Files identical despite different names*

