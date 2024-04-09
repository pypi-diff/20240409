# Comparing `tmp/gamdl-2.1.3.tar.gz` & `tmp/gamdl-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.3.tar` & `gamdl-2.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1137 2024-04-09 09:56:05.135619 gamdl-2.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-09 09:56:05.135619 gamdl-2.1.3/.gitignore
--rw-r--r--   0        0        0    11240 2024-04-09 09:56:05.135619 gamdl-2.1.3/README.md
--rw-r--r--   0        0        0       22 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26304 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/cli.py
--rw-r--r--   0        0        0     5544 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/constants.py
--rw-r--r--   0        0        0    12570 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader.py
--rw-r--r--   0        0        0    10356 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2121 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13741 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3691 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      801 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-09 09:56:05.135619 gamdl-2.1.3/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-09 09:56:05.135619 gamdl-2.1.3/requirements.txt
--rw-r--r--   0        0        0    11715 1970-01-01 00:00:00.000000 gamdl-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-09 10:17:10.546515 gamdl-2.1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-09 10:17:10.546515 gamdl-2.1.4/.gitignore
+-rw-r--r--   0        0        0    11240 2024-04-09 10:17:10.546515 gamdl-2.1.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26303 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/cli.py
+-rw-r--r--   0        0        0     5544 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/constants.py
+-rw-r--r--   0        0        0    12570 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/downloader.py
+-rw-r--r--   0        0        0    10356 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2121 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13741 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3691 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      801 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-09 10:17:10.546515 gamdl-2.1.4/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-09 10:17:10.546515 gamdl-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-09 10:17:10.546515 gamdl-2.1.4/requirements.txt
+-rw-r--r--   0        0        0    11715 1970-01-01 00:00:00.000000 gamdl-2.1.4/PKG-INFO
```

### Comparing `gamdl-2.1.3/.github/workflows/main.yml` & `gamdl-2.1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/README.md` & `gamdl-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/apple_music_api.py` & `gamdl-2.1.4/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/cli.py` & `gamdl-2.1.4/gamdl/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
                             )
                             logger.debug("Getting decryption key")
                             decryption_key = downloader_song_legacy.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
                         else:
                             stream_info = downloader_song.get_stream_info(track)
-                            if not stream_info.stream_url or not stream_info.codec:
+                            if not stream_info.stream_url or not stream_info.pssh:
                                 logger.warning(
                                     f"({queue_progress}) Song is not downloadable or is not"
                                     " available in the chosen codec, skipping"
                                 )
                                 continue
                             logger.debug("Getting decryption key")
                             decryption_key = downloader.get_decryption_key(
```

### Comparing `gamdl-2.1.3/gamdl/constants.py` & `gamdl-2.1.4/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/downloader.py` & `gamdl-2.1.4/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/downloader_music_video.py` & `gamdl-2.1.4/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/downloader_post.py` & `gamdl-2.1.4/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/downloader_song.py` & `gamdl-2.1.4/gamdl/downloader_song.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/downloader_song_legacy.py` & `gamdl-2.1.4/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/enums.py` & `gamdl-2.1.4/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/hardcoded_wvd.py` & `gamdl-2.1.4/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/gamdl/itunes_api.py` & `gamdl-2.1.4/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/pyproject.toml` & `gamdl-2.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.3/PKG-INFO` & `gamdl-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.3
+Version: 2.1.4
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
```

