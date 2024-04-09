# Comparing `tmp/spotidex-0.0.4.tar.gz` & `tmp/spotidex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotidex-0.0.4.tar", last modified: Sun Apr  7 09:29:00 2024, max compression
+gzip compressed data, was "spotidex-0.0.5.tar", max compression
```

## Comparing `spotidex-0.0.4.tar` & `spotidex-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.420750 spotidex-0.0.4/
--rw-rw-rw-   0        0        0     1110 2024-04-06 09:42:27.000000 spotidex-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1129 2024-04-07 09:29:00.417519 spotidex-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-06 09:42:27.000000 spotidex-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 09:29:00.420750 spotidex-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-07 09:27:38.000000 spotidex-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.295922 spotidex-0.0.4/spotidex/
--rw-rw-rw-   0        0        0      121 2024-04-07 04:09:46.000000 spotidex-0.0.4/spotidex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.356891 spotidex-0.0.4/spotidex/cli/
--rw-rw-rw-   0        0        0      616 2024-04-07 04:09:10.000000 spotidex-0.0.4/spotidex/cli/SpotidexApp.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:04:49.000000 spotidex-0.0.4/spotidex/cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.362395 spotidex-0.0.4/spotidex/cli/app_screens/
--rw-rw-rw-   0        0        0     6871 2024-04-07 04:25:26.000000 spotidex-0.0.4/spotidex/cli/app_screens/DownloadInterface.py
--rw-rw-rw-   0        0        0     4675 2024-04-06 10:26:15.000000 spotidex-0.0.4/spotidex/cli/app_screens/MainMenuInterface.py
--rw-rw-rw-   0        0        0     4360 2024-04-06 19:29:28.000000 spotidex-0.0.4/spotidex/cli/app_screens/SearchInterface.py
--rw-rw-rw-   0        0        0     4025 2024-04-06 10:25:55.000000 spotidex-0.0.4/spotidex/cli/app_screens/SelectDownloadInterface.py
--rw-rw-rw-   0        0        0     2430 2024-04-06 10:26:19.000000 spotidex-0.0.4/spotidex/cli/app_screens/SettingsInterface.py
--rw-rw-rw-   0        0        0        0 2024-03-25 10:54:48.000000 spotidex-0.0.4/spotidex/cli/app_screens/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.378943 spotidex-0.0.4/spotidex/cli/custom_widgets/
--rw-rw-rw-   0        0        0     4510 2024-04-06 08:18:54.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/AppInterface.py
--rw-rw-rw-   0        0        0     1409 2024-04-06 10:25:36.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadPathSelector.py
--rw-rw-rw-   0        0        0     1694 2024-03-26 11:07:37.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadQualitySelection.py
--rw-rw-rw-   0        0        0     1933 2024-03-26 10:25:59.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/MetadataCheckBox.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:19:37.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.404431 spotidex-0.0.4/spotidex/cli/popup_screens/
--rw-rw-rw-   0        0        0     4303 2024-04-06 09:28:28.000000 spotidex-0.0.4/spotidex/cli/popup_screens/DownloadPathPopup.py
--rw-rw-rw-   0        0        0     1126 2023-12-20 02:51:25.000000 spotidex-0.0.4/spotidex/cli/popup_screens/ExitScreenPopup.py
--rw-rw-rw-   0        0        0     1210 2024-03-26 12:20:40.000000 spotidex-0.0.4/spotidex/cli/popup_screens/GoBackSettingsPopup.py
--rw-rw-rw-   0        0        0     1389 2024-03-22 13:06:57.000000 spotidex-0.0.4/spotidex/cli/popup_screens/NetworkErrorPopup.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:19:46.000000 spotidex-0.0.4/spotidex/cli/popup_screens/__init__.py
--rw-rw-rw-   0        0        0     3880 2024-04-06 12:55:51.000000 spotidex-0.0.4/spotidex/cli/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.412477 spotidex-0.0.4/spotidex/src/
--rw-rw-rw-   0        0        0        0 2024-04-06 10:22:02.000000 spotidex-0.0.4/spotidex/src/__init__.py
--rw-rw-rw-   0        0        0     3043 2024-04-07 05:31:37.000000 spotidex-0.0.4/spotidex/src/content.py
--rw-rw-rw-   0        0        0     6703 2024-04-07 06:26:09.000000 spotidex-0.0.4/spotidex/src/download.py
--rw-rw-rw-   0        0        0     1049 2023-12-06 02:16:07.000000 spotidex-0.0.4/spotidex/src/static.py
--rw-rw-rw-   0        0        0     5954 2024-04-07 06:30:44.000000 spotidex-0.0.4/spotidex/src/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.350367 spotidex-0.0.4/spotidex.egg-info/
--rw-rw-rw-   0        0        0     1129 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/top_level.txt
+-rw-r--r--   0        0        0      532 2024-04-09 17:06:57.148329 spotidex-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      499 2024-04-06 09:42:27.400268 spotidex-0.0.5/README.md
+-rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-0.0.5/spotidex/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-0.0.5/spotidex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-0.0.5/spotidex/cli/app_screens/__init__.py
+-rw-r--r--   0        0        0     6871 2024-04-07 04:25:26.776169 spotidex-0.0.5/spotidex/cli/app_screens/DownloadInterface.py
+-rw-r--r--   0        0        0     4675 2024-04-06 10:26:15.321454 spotidex-0.0.5/spotidex/cli/app_screens/MainMenuInterface.py
+-rw-r--r--   0        0        0     4576 2024-04-09 17:31:03.911736 spotidex-0.0.5/spotidex/cli/app_screens/SearchInterface.py
+-rw-r--r--   0        0        0     4025 2024-04-06 10:25:55.937694 spotidex-0.0.5/spotidex/cli/app_screens/SelectDownloadInterface.py
+-rw-r--r--   0        0        0     2430 2024-04-06 10:26:19.911279 spotidex-0.0.5/spotidex/cli/app_screens/SettingsInterface.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-0.0.5/spotidex/cli/custom_widgets/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
+-rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
+-rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
+-rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
+-rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
+-rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
+-rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
+-rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-0.0.5/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
+-rw-r--r--   0        0        0     4510 2024-04-06 08:18:54.195763 spotidex-0.0.5/spotidex/cli/custom_widgets/AppInterface.py
+-rw-r--r--   0        0        0     1409 2024-04-06 10:25:36.360967 spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadPathSelector.py
+-rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadQualitySelection.py
+-rw-r--r--   0        0        0     1933 2024-03-26 10:25:59.101131 spotidex-0.0.5/spotidex/cli/custom_widgets/MetadataCheckBox.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-0.0.5/spotidex/cli/popup_screens/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
+-rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-0.0.5/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
+-rw-r--r--   0        0        0     4303 2024-04-06 09:28:28.087939 spotidex-0.0.5/spotidex/cli/popup_screens/DownloadPathPopup.py
+-rw-r--r--   0        0        0     1135 2024-04-09 16:48:01.830808 spotidex-0.0.5/spotidex/cli/popup_screens/ExitScreenPopup.py
+-rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-0.0.5/spotidex/cli/popup_screens/GoBackSettingsPopup.py
+-rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-0.0.5/spotidex/cli/popup_screens/NetworkErrorPopup.py
+-rw-r--r--   0        0        0      616 2024-04-07 04:09:10.420863 spotidex-0.0.5/spotidex/cli/SpotidexApp.py
+-rw-r--r--   0        0        0     4196 2024-04-09 16:52:32.143307 spotidex-0.0.5/spotidex/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-0.0.5/spotidex/src/__init__.py
+-rw-r--r--   0        0        0     3043 2024-04-07 05:31:37.359930 spotidex-0.0.5/spotidex/src/content.py
+-rw-r--r--   0        0        0     6712 2024-04-09 17:18:55.031801 spotidex-0.0.5/spotidex/src/download.py
+-rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-0.0.5/spotidex/src/static.py
+-rw-r--r--   0        0        0     5950 2024-04-09 17:11:57.735948 spotidex-0.0.5/spotidex/src/utils.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 spotidex-0.0.5/PKG-INFO
```

### Comparing `spotidex-0.0.4/PKG-INFO` & `spotidex-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-Metadata-Version: 2.1
-Name: spotidex
-Version: 0.0.4
-Author: libin-codes
-Author-email: libinlalu000@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: mutagen==1.47.0
-Requires-Dist: Requests==2.31.0
-Requires-Dist: rich==13.7.1
-Requires-Dist: spotipy==2.23.0
-Requires-Dist: textual==0.55.1
-Requires-Dist: tqdm==4.66.1
-Requires-Dist: yt_dlp==2024.3.10
-Requires-Dist: ytmusicapi==1.3.2
-
-# spotidex
-
-[![PyPI - Version](https://img.shields.io/pypi/v/spotidex.svg)](https://pypi.org/project/spotidex)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotidex.svg)](https://pypi.org/project/spotidex)
-
------
-
-**Table of Contents**
-
-- [Installation](#installation)
-- [License](#license)
-
-## Installation
-
-```console
-pip install spotidex
-```
-
-## License
-
-`spotidex` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+Metadata-Version: 2.1
+Name: spotidex
+Version: 0.0.5
+Summary: Spotify Downloader TUI
+License: MIT
+Author: Libin Lalu
+Author-email: libinlalu000@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: mutagen (==1.47.0)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: rich (==13.7.1)
+Requires-Dist: spotipy (==2.23.0)
+Requires-Dist: textual (==0.56.4)
+Requires-Dist: tqdm (==4.66.1)
+Requires-Dist: yt-dlp (==2024.3.10)
+Requires-Dist: ytmusicapi (==1.3.2)
+Description-Content-Type: text/markdown
+
+# spotidex
+
+[![PyPI - Version](https://img.shields.io/pypi/v/spotidex.svg)](https://pypi.org/project/spotidex)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotidex.svg)](https://pypi.org/project/spotidex)
+
+-----
+
+**Table of Contents**
+
+- [Installation](#installation)
+- [License](#license)
+
+## Installation
+
+```console
+pip install spotidex
+```
+
+## License
+
+`spotidex` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
```

### Comparing `spotidex-0.0.4/spotidex/cli/SpotidexApp.py` & `spotidex-0.0.5/spotidex/cli/SpotidexApp.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/app_screens/DownloadInterface.py` & `spotidex-0.0.5/spotidex/cli/app_screens/DownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/app_screens/MainMenuInterface.py` & `spotidex-0.0.5/spotidex/cli/app_screens/MainMenuInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/app_screens/SearchInterface.py` & `spotidex-0.0.5/spotidex/cli/app_screens/SearchInterface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from textual.widgets import Input, Button, Label
 from textual.screen import Screen
 from textual.containers import Horizontal
 
 from spotidex.cli.custom_widgets.AppInterface import AppInterface
 from spotidex.cli.app_screens.MainMenuInterface import MainMenuInterface
-from spotidex.cli.utils import input_validator,app_description
+from spotidex.cli.utils import input_validator, app_description
 from spotidex.cli.utils import get_link_details
 
 from textual.worker import Worker, get_current_worker
 from textual import work
 
 CSS = """
 Search {
@@ -41,75 +41,84 @@
 }
 
 #search-input:blur{
     border:tall black
 }
 """
 
+
 class Search(Screen):
     DEFAULT_CSS = CSS
+
     def compose(self):
         yield AppInterface(
             Horizontal(
                 Input(
                     id="search-input",
                     placeholder="PASTE YOUR SPOTIFY LINK HERE",
                 ),
                 Button("SEARCH", "success", id="search-button", disabled=True),
             ),
             Label(app_description, id="app-description", shrink=True),
             id="search-interface",
         )
-    
+
     @work(exclusive=True, thread=True)
     def get_link_info(self):
         self.app.query_one("LoadingIndicator").styles.background = "#1c1c1c"
         try:
             self.app.link_details = get_link_details(self.app.spotify_link)
         except Exception as spotidex_error:
             if spotidex_error.message == "NetworkError":
-                self.app.notify("Network Connection Error",title="SPOTIDEX",severity="error")
+                self.app.notify(
+                    "Please check you internet connection and try again",
+                    title="Network Error",
+                    severity="error",
+                )
             elif spotidex_error.message == "InvalidSpotifyLink":
-                self.app.notify("Invalid Spotify Link",title="SPOTIDEX",severity="error")
+                self.app.notify(
+                    "The link provided is not valid, please check the link and try again",
+                    title="INVALID LINK",
+                    severity="error",
+                )
             get_current_worker().cancel()
         self.app.query_one("#interface").loading = False
         self.app.query_one("#exit-button").disabled = False
-        self.app.query_one("#interface").styles.padding = (2,3,0,3)
-        
-        
+        self.app.query_one("#interface").styles.padding = (2, 3, 0, 3)
+
     def on_worker_state_changed(self, event: Worker.StateChanged) -> None:
         if str(event.state) == "WorkerState.CANCELLED":
-            self.query_one('#search-input').visible = True
-            self.query_one('#app-description').visible = True
-            self.query_one('#search-button').visible = True
+            self.query_one("#search-input").visible = True
+            self.query_one("#app-description").visible = True
+            self.query_one("#search-button").visible = True
         elif str(event.state) == "WorkerState.SUCCESS":
             self.app.push_screen(MainMenuInterface())
-            self.query_one('#search-input').visible = True
-            self.query_one('#app-description').visible = True
-            self.query_one('#search-button').visible = True
+            self.query_one("#search-input").visible = True
+            self.query_one("#app-description").visible = True
+            self.query_one("#search-button").visible = True
             self.query_one("#search-button").disabled = True
-            
+
     def on_mount(self):
         self.app.query_one("#nav-label").update("[bold]HOME")
         self.query_one("#app-description").border_title = "ABOUT SPOTIDEX"
         self.app.query_one("#back-button").disabled = True
-        
+
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "search-button":
             self.app.query_one("#interface").styles.padding = 0
             self.app.spotify_link = self.query_one("#search-input").value
             self.app.query_one("#interface").loading = True
             self.app.query_one("#exit-button").disabled = True
-            self.query_one('#search-input').visible = False
-            self.query_one('#app-description').visible = False
-            self.query_one('#search-button').visible = False
+            self.query_one("#search-input").visible = False
+            self.query_one("#app-description").visible = False
+            self.query_one("#search-button").visible = False
             self.get_link_info()
-        
+
     def on_input_changed(self, event: Input.Changed):
         if input_validator(event.input.value):
-            self.app.query_one("#search-input",Input).styles.border = ("tall","green")
+            self.app.query_one("#search-input", Input).styles.border = ("tall", "green")
             self.app.query_one("#search-button").disabled = False
         elif event.input.value == "":
-            self.app.query_one("#search-input",Input).styles.border = ("tall","black")
+            self.app.query_one("#search-input", Input).styles.border = ("tall", "black")
         else:
-            self.app.query_one("#search-input",Input).styles.border = ("tall","red")
+            self.app.query_one("#search-input", Input).styles.border = ("tall", "red")
             self.app.query_one("#search-button").disabled = True
```

### Comparing `spotidex-0.0.4/spotidex/cli/app_screens/SelectDownloadInterface.py` & `spotidex-0.0.5/spotidex/cli/app_screens/SelectDownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/app_screens/SettingsInterface.py` & `spotidex-0.0.5/spotidex/cli/app_screens/SettingsInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/custom_widgets/AppInterface.py` & `spotidex-0.0.5/spotidex/cli/custom_widgets/AppInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadPathSelector.py` & `spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadPathSelector.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadQualitySelection.py` & `spotidex-0.0.5/spotidex/cli/custom_widgets/DownloadQualitySelection.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/custom_widgets/MetadataCheckBox.py` & `spotidex-0.0.5/spotidex/cli/custom_widgets/MetadataCheckBox.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/popup_screens/DownloadPathPopup.py` & `spotidex-0.0.5/spotidex/cli/popup_screens/DownloadPathPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/popup_screens/ExitScreenPopup.py` & `spotidex-0.0.5/spotidex/cli/popup_screens/ExitScreenPopup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,10 +44,10 @@
             Button("YES", id="yes-exit-button",variant='success'),
             Button("NO", variant="error", id="exit-no-button"),
             id="exit-dialog-box",
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "yes-exit-button":
-            exit()
+            self.app.exit()
         else:
             self.dismiss()
```

### Comparing `spotidex-0.0.4/spotidex/cli/popup_screens/GoBackSettingsPopup.py` & `spotidex-0.0.5/spotidex/cli/popup_screens/GoBackSettingsPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/cli/popup_screens/NetworkErrorPopup.py` & `spotidex-0.0.5/spotidex/cli/popup_screens/NetworkErrorPopup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,10 +55,10 @@
             Button("RETRY", id="retry-button",variant='warning'),
             Button("EXIT", variant="error", id="exit-button"),
             id="network-error-dialog-box",
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "exit-button":
-            exit()
+            self.app.exit()
         else:
             self.dismiss("retry")
```

### Comparing `spotidex-0.0.4/spotidex/cli/utils.py` & `spotidex-0.0.5/spotidex/cli/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,19 +87,22 @@
     if ("spotify" in value)
     and (any(keyword in value for keyword in ["track", "playlist", "album"]))
     else False
 )
 
 def get_data_drive_path():
     if os.name == 'nt':  # Windows
+        system_drive = os.environ['SYSTEMDRIVE'] if 'SYSTEMDRIVE' in os.environ else 'C:'
         drives = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
-        available_drives = [drive + ':\\' for drive in drives if os.path.exists(drive + ':\\')]
+        available_drives = [drive + ':\\' for drive in drives if os.path.exists(drive + ':\\') and drive + ':' != system_drive]
         return available_drives[0] if available_drives else None
     else:  # Unix-like systems
-        return '/'
+        # Filter out root directory ('/') from mounted drives
+        mounted_drives = [root for root, dirs, files in os.walk('/') if dirs or files]
+        return mounted_drives[0] if mounted_drives else None
 
 def get_downloads_folder():
     # Get the user's home directory
     home_dir = os.path.expanduser("~")
     
     # Operating system specific logic to get the Downloads folder
     if os.name == 'posix':  # Unix-like OS (Linux, macOS)
```

### Comparing `spotidex-0.0.4/spotidex/src/content.py` & `spotidex-0.0.5/spotidex/src/content.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/src/download.py` & `spotidex-0.0.5/spotidex/src/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         except SpotifyException:
             raise SpotidexError("InvalidSpotifyLink")
         except (ConnectionError,ReadTimeout):
             raise SpotidexError("NetworkError")
 
         
         track_artist = ",".join([artist["name"] for artist in data["artists"]])
-        query = f"{data["name"]} song by {track_artist} official lyrics "
+        query = data["name"]+f" song by {track_artist} official lyrics "
         file_name = get_valid_name(download_path,data["name"]+".mp3")
     
         with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
             options = {
                 "format": "bestaudio/best",
                 "outtmpl": str(download_path)+'\\'+file_name,
                 "quiet": True,
@@ -105,15 +105,15 @@
 
             if metadata:
                 add_metadata(data, Path(downloaded_path + ".mp3").resolve())
 
             if self.total_tracks == None:
                 progress_hook(self, {"status": "downloaded"}, custom_hook)
                 for file_path in Path(temp_folder).iterdir():
-                    shutil.move(file_path, download_path)
+                    shutil.move(str(file_path), str(download_path))
                 progress_hook(self, {"status": "transfered"}, custom_hook)
     
     def download_playlist(
         self,
         link,
         custom_hook=None,
         download_path=Path.cwd(),
```

### Comparing `spotidex-0.0.4/spotidex/src/static.py` & `spotidex-0.0.5/spotidex/src/static.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.4/spotidex/src/utils.py` & `spotidex-0.0.5/spotidex/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,9 +176,9 @@
     if os_name in ["linux", "darwin"]:
         ffmpeg_path.chmod(ffmpeg_path.stat().st_mode | stat.S_IEXEC)
 
 def get_valid_name(path, name):
     name, i = re.sub(r"[^\w\d(),.\-\[\] ]", "", name), 1
     add_mp3 = ".mp3" if ".mp3" in name else ""
     while Path(path, name).exists():
-        name, i = name.removesuffix(".mp3").split(" (")[0] + f" ({i})" + add_mp3, i + 1
-    return name.removesuffix(".mp3")
+        name, i = name.replace('.mp3',"").split(" (")[0] + f" ({i})" + add_mp3, i + 1
+    return name.replace('.mp3',"")
```

