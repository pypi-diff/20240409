# Comparing `tmp/gamdl-2.1.1.tar.gz` & `tmp/gamdl-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.1.tar` & `gamdl-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1137 2024-04-08 22:51:22.523302 gamdl-2.1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-08 22:51:22.523302 gamdl-2.1.1/.gitignore
--rw-r--r--   0        0        0    11148 2024-04-08 22:51:22.523302 gamdl-2.1.1/README.md
--rw-r--r--   0        0        0       22 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26458 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/cli.py
--rw-r--r--   0        0        0     5522 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/constants.py
--rw-r--r--   0        0        0    12570 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader.py
--rw-r--r--   0        0        0    10356 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2121 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13710 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3691 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      801 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-08 22:51:22.523302 gamdl-2.1.1/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-08 22:51:22.523302 gamdl-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-08 22:51:22.523302 gamdl-2.1.1/requirements.txt
--rw-r--r--   0        0        0    11623 1970-01-01 00:00:00.000000 gamdl-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-09 00:09:03.183159 gamdl-2.1.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-09 00:09:03.183159 gamdl-2.1.2/.gitignore
+-rw-r--r--   0        0        0    11148 2024-04-09 00:09:03.183159 gamdl-2.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26235 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/cli.py
+-rw-r--r--   0        0        0     5522 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/constants.py
+-rw-r--r--   0        0        0    12570 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader.py
+-rw-r--r--   0        0        0    10356 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2121 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13741 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3691 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      801 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-09 00:09:03.187159 gamdl-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-09 00:09:03.187159 gamdl-2.1.2/requirements.txt
+-rw-r--r--   0        0        0    11623 1970-01-01 00:00:00.000000 gamdl-2.1.2/PKG-INFO
```

### Comparing `gamdl-2.1.1/.github/workflows/main.yml` & `gamdl-2.1.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/README.md` & `gamdl-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/apple_music_api.py` & `gamdl-2.1.2/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/cli.py` & `gamdl-2.1.2/gamdl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,22 +487,18 @@
                             )
                             logger.debug("Getting decryption key")
                             decryption_key = downloader_song_legacy.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
                         else:
                             stream_info = downloader_song.get_stream_info(track)
-                            if not stream_info.pssh:
+                            if not stream_info.stream_url:
                                 logger.warning(
-                                    f"({queue_progress}) Song does not contain Widevine DRM, skipping"
-                                )
-                                continue
-                            elif not stream_info.stream_url:
-                                logger.warning(
-                                    f"({queue_progress}) Song is not available with the selected codec, skipping"
+                                    f"({queue_progress}) Song is not downloadable or is not"
+                                    " available in the chosen codec, skipping"
                                 )
                                 continue
                             logger.debug("Getting decryption key")
                             decryption_key = downloader.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
                         encrypted_path = downloader_song.get_encrypted_path(track["id"])
```

### Comparing `gamdl-2.1.1/gamdl/constants.py` & `gamdl-2.1.2/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/downloader.py` & `gamdl-2.1.2/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/downloader_music_video.py` & `gamdl-2.1.2/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/downloader_post.py` & `gamdl-2.1.2/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/downloader_song.py` & `gamdl-2.1.2/gamdl/downloader_song.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 session_data
                 for session_data in m3u8_data["session_data"]
                 if session_data["data_id"] == "com.apple.hls.AudioSessionKeyInfo"
             ),
             None,
         )
         if not drm_info_raw:
-            raise Exception("DRM info not found")
+            return None
         return json.loads(base64.b64decode(drm_info_raw["value"]).decode("utf-8"))
 
     def get_asset_infos(self, m3u8_data: dict) -> dict:
         return json.loads(
             base64.b64decode(
                 next(
                     session_data
@@ -110,14 +110,16 @@
         return self._get_stream_info(m3u8_url)
 
     def _get_stream_info(self, m3u8_url: str) -> StreamInfo:
         stream_info = StreamInfo()
         m3u8_obj = m3u8.load(m3u8_url)
         m3u8_data = m3u8_obj.data
         drm_infos = self.get_drm_infos(m3u8_data)
+        if not drm_infos:
+            return stream_info
         asset_infos = self.get_asset_infos(m3u8_data)
         if self.codec == SongCodec.ASK:
             playlist = self.get_playlist_from_user(m3u8_data)
         else:
             playlist = self.get_playlist_from_codec(m3u8_data)
         if playlist is None:
             return stream_info
```

### Comparing `gamdl-2.1.1/gamdl/downloader_song_legacy.py` & `gamdl-2.1.2/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/enums.py` & `gamdl-2.1.2/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/hardcoded_wvd.py` & `gamdl-2.1.2/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/gamdl/itunes_api.py` & `gamdl-2.1.2/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/pyproject.toml` & `gamdl-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.1/PKG-INFO` & `gamdl-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.1
+Version: 2.1.2
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
```

