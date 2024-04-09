# Comparing `tmp/gamdl-2.1.tar.gz` & `tmp/gamdl-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.tar` & `gamdl-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1137 2024-04-08 21:27:20.588555 gamdl-2.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-08 21:27:20.588555 gamdl-2.1/.gitignore
--rw-r--r--   0        0        0    11148 2024-04-08 21:27:20.588555 gamdl-2.1/README.md
--rw-r--r--   0        0        0       20 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26458 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/cli.py
--rw-r--r--   0        0        0     5522 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/constants.py
--rw-r--r--   0        0        0    12570 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader.py
--rw-r--r--   0        0        0    10356 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2121 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13662 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3691 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      801 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-08 21:27:20.592555 gamdl-2.1/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-08 21:27:20.592555 gamdl-2.1/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-08 21:27:20.592555 gamdl-2.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-08 21:27:20.592555 gamdl-2.1/requirements.txt
--rw-r--r--   0        0        0    11621 1970-01-01 00:00:00.000000 gamdl-2.1/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-08 22:51:22.523302 gamdl-2.1.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-08 22:51:22.523302 gamdl-2.1.1/.gitignore
+-rw-r--r--   0        0        0    11148 2024-04-08 22:51:22.523302 gamdl-2.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26458 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/cli.py
+-rw-r--r--   0        0        0     5522 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/constants.py
+-rw-r--r--   0        0        0    12570 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader.py
+-rw-r--r--   0        0        0    10356 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2121 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13710 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3691 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      801 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-08 22:51:22.523302 gamdl-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-08 22:51:22.523302 gamdl-2.1.1/requirements.txt
+-rw-r--r--   0        0        0    11623 1970-01-01 00:00:00.000000 gamdl-2.1.1/PKG-INFO
```

### Comparing `gamdl-2.1/.github/workflows/main.yml` & `gamdl-2.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/README.md` & `gamdl-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/apple_music_api.py` & `gamdl-2.1.1/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/cli.py` & `gamdl-2.1.1/gamdl/cli.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/constants.py` & `gamdl-2.1.1/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/downloader.py` & `gamdl-2.1.1/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/downloader_music_video.py` & `gamdl-2.1.1/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/downloader_post.py` & `gamdl-2.1.1/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/downloader_song.py` & `gamdl-2.1.1/gamdl/downloader_song.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import base64
 import datetime
 import json
 import re
 import subprocess
 from pathlib import Path
 from xml.dom import minidom
@@ -320,15 +322,16 @@
     def remux_ffmpeg(
         self,
         decrypted_path: Path,
         remuxed_path: Path,
         codec: str,
     ):
         use_mp4_format = any(
-            codec.startswith(possible_codec) for possible_codec in self.MP4_FORMAT_CODECS
+            codec.startswith(possible_codec)
+            for possible_codec in self.MP4_FORMAT_CODECS
         )
         subprocess.run(
             [
                 self.downloader.ffmpeg_path_full,
                 "-loglevel",
                 "error",
                 "-y",
```

### Comparing `gamdl-2.1/gamdl/downloader_song_legacy.py` & `gamdl-2.1.1/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/enums.py` & `gamdl-2.1.1/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/hardcoded_wvd.py` & `gamdl-2.1.1/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/gamdl/itunes_api.py` & `gamdl-2.1.1/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/pyproject.toml` & `gamdl-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1/PKG-INFO` & `gamdl-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1
+Version: 2.1.1
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
```

