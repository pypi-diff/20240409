# Comparing `tmp/gamdl-2.0.tar.gz` & `tmp/gamdl-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.0.tar` & `gamdl-2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1137 2024-04-08 18:49:22.867913 gamdl-2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-08 18:49:22.867913 gamdl-2.0/.gitignore
--rw-r--r--   0        0        0    11148 2024-04-08 18:49:22.867913 gamdl-2.0/README.md
--rw-r--r--   0        0        0       20 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26206 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/cli.py
--rw-r--r--   0        0        0     5522 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/constants.py
--rw-r--r--   0        0        0    12570 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader.py
--rw-r--r--   0        0        0     9847 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2121 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13316 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3691 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      801 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/itunes_api.py
--rw-r--r--   0        0        0      347 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-08 18:49:22.867913 gamdl-2.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-08 18:49:22.867913 gamdl-2.0/requirements.txt
--rw-r--r--   0        0        0    11621 1970-01-01 00:00:00.000000 gamdl-2.0/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-08 21:27:20.588555 gamdl-2.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-08 21:27:20.588555 gamdl-2.1/.gitignore
+-rw-r--r--   0        0        0    11148 2024-04-08 21:27:20.588555 gamdl-2.1/README.md
+-rw-r--r--   0        0        0       20 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26458 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/cli.py
+-rw-r--r--   0        0        0     5522 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/constants.py
+-rw-r--r--   0        0        0    12570 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader.py
+-rw-r--r--   0        0        0    10356 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2121 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13662 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3691 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      801 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-08 21:27:20.588555 gamdl-2.1/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-08 21:27:20.592555 gamdl-2.1/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-08 21:27:20.592555 gamdl-2.1/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-08 21:27:20.592555 gamdl-2.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-08 21:27:20.592555 gamdl-2.1/requirements.txt
+-rw-r--r--   0        0        0    11621 1970-01-01 00:00:00.000000 gamdl-2.1/PKG-INFO
```

### Comparing `gamdl-2.0/.github/workflows/main.yml` & `gamdl-2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/README.md` & `gamdl-2.1/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/apple_music_api.py` & `gamdl-2.1/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/cli.py` & `gamdl-2.1/gamdl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,19 @@
                             )
                         else:
                             logger.debug(f"Decrypting to {decrypted_path}")
                             downloader_song.decrypt(
                                 encrypted_path, decrypted_path, decryption_key
                             )
                             logger.debug(f"Remuxing to {final_path}")
-                            downloader_song.remux(decrypted_path, remuxed_path)
+                            downloader_song.remux(
+                                decrypted_path,
+                                remuxed_path,
+                                stream_info.codec,
+                            )
                         logger.debug("Applying tags")
                         downloader.apply_tags(remuxed_path, tags, cover_url)
                         logger.debug(f"Moving to {final_path}")
                         downloader.move_to_output_path(remuxed_path, final_path)
                     if no_synced_lyrics or not lyrics.synced:
                         pass
                     elif lyrics_synced_path.exists() and not overwrite:
@@ -631,14 +635,16 @@
                             decrypted_path_audio,
                         )
                         logger.debug(f"Remuxing to {remuxed_path}")
                         downloader_music_video.remux(
                             decrypted_path_video,
                             decrypted_path_audio,
                             remuxed_path,
+                            stream_info_video.codec,
+                            stream_info_audio.codec,
                         )
                         logger.debug("Applying tags")
                         downloader.apply_tags(remuxed_path, tags, cover_url)
                         logger.debug(f"Moving to {final_path}")
                         downloader.move_to_output_path(remuxed_path, final_path)
                     if not save_cover:
                         pass
```

### Comparing `gamdl-2.0/gamdl/constants.py` & `gamdl-2.1/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/downloader.py` & `gamdl-2.1/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/downloader_music_video.py` & `gamdl-2.1/gamdl/downloader_music_video.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import subprocess
 import urllib.parse
 from pathlib import Path
 
 import click
 import m3u8
 from tabulate import tabulate
@@ -9,14 +10,16 @@
 from .constants import MUSIC_VIDEO_CODEC_MAP
 from .downloader import Downloader
 from .enums import MusicVideoCodec, RemuxMode
 from .models import StreamInfo
 
 
 class DownloaderMusicVideo:
+    MP4_FORMAT_CODECS = ["hvc1", "ec-3"]
+
     def __init__(
         self,
         downloader: Downloader,
         codec: MusicVideoCodec = MusicVideoCodec.H264_BEST,
     ):
         self.downloader = downloader
         self.codec = codec
@@ -29,18 +32,18 @@
         query = urllib.parse.parse_qs(url_parts.query, keep_blank_values=True)
         query.update({"aec": "HD", "dsid": "1"})
         stream_url_master_new = url_parts._replace(
             query=urllib.parse.urlencode(query, doseq=True)
         ).geturl()
         return m3u8.load(stream_url_master_new).data
 
-    def get_stream_url_video(
+    def get_playlist_video(
         self,
         playlists: list[dict],
-    ):
+    ) -> dict:
         playlists_filtered = [
             playlist
             for playlist in playlists
             if playlist["stream_info"]["codecs"].startswith(
                 MUSIC_VIDEO_CODEC_MAP[self.codec]
             )
         ]
@@ -49,20 +52,20 @@
                 playlist
                 for playlist in playlists
                 if playlist["stream_info"]["codecs"].startswith(
                     MUSIC_VIDEO_CODEC_MAP[MusicVideoCodec.H264_BEST]
                 )
             ]
         playlists_filtered.sort(key=lambda x: x["stream_info"]["bandwidth"])
-        return playlists_filtered[-1]["uri"]
+        return playlists_filtered[-1]
 
-    def get_stream_url_video_from_user(
+    def get_playlist_video_from_user(
         self,
         playlists: list[dict],
-    ):
+    ) -> dict:
         table = [
             [
                 i,
                 playlist["stream_info"]["codecs"],
                 playlist["stream_info"]["resolution"],
                 playlist["stream_info"]["bandwidth"],
             ]
@@ -72,34 +75,34 @@
         try:
             choice = (
                 click.prompt("Choose a video codec", type=click.IntRange(1, len(table)))
                 - 1
             )
         except click.exceptions.Abort:
             raise KeyboardInterrupt()
-        return playlists[choice]["uri"]
+        return playlists[choice]
 
-    def get_stream_url_audio(
+    def get_playlist_audio(
         self,
         playlists: list[dict],
-    ) -> str:
+    ) -> dict:
         stream_url = next(
             (
                 playlist
                 for playlist in playlists
                 if playlist["group_id"] == "audio-stereo-256"
             ),
             None,
-        )["uri"]
+        )
         return stream_url
 
-    def get_stream_url_audio_from_user(
+    def get_playlist_audio_from_user(
         self,
         playlists: list[dict],
-    ):
+    ) -> dict:
         table = [
             [
                 i,
                 playlist["group_id"],
             ]
             for i, playlist in enumerate(playlists, 1)
         ]
@@ -109,50 +112,48 @@
                 click.prompt(
                     "Choose an audio codec", type=click.IntRange(1, len(table))
                 )
                 - 1
             )
         except click.exceptions.Abort:
             raise KeyboardInterrupt()
-        return playlists[choice]["uri"]
+        return playlists[choice]
 
     def get_pssh(self, m3u8_data: dict):
         return next(
             (
                 key
                 for key in m3u8_data["keys"]
                 if key["keyformat"] == "urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed"
             ),
             None,
         )["uri"]
 
     def get_stream_info_video(self, m3u8_master_data: dict) -> StreamInfo:
         stream_info = StreamInfo()
         if self.codec != MusicVideoCodec.ASK:
-            stream_info.stream_url = self.get_stream_url_video(
-                m3u8_master_data["playlists"]
-            )
+            playlist = self.get_playlist_video(m3u8_master_data["playlists"])
         else:
-            stream_info.stream_url = self.get_stream_url_video_from_user(
-                m3u8_master_data["playlists"]
-            )
+            playlist = self.get_playlist_video_from_user(m3u8_master_data["playlists"])
+        stream_info.stream_url = playlist["uri"]
+        stream_info.codec = playlist["stream_info"]["codecs"]
         m3u8_data = m3u8.load(stream_info.stream_url).data
         stream_info.pssh = self.get_pssh(m3u8_data)
         return stream_info
 
     def get_stream_info_audio(self, m3u8_master_data: dict) -> StreamInfo:
         stream_info = StreamInfo()
         if self.codec != MusicVideoCodec.ASK:
-            stream_info.stream_url = self.get_stream_url_audio(
-                m3u8_master_data["media"]
-            )
+            playlist = self.get_playlist_audio(m3u8_master_data["media"])
         else:
-            stream_info.stream_url = self.get_stream_url_audio_from_user(
-                m3u8_master_data["media"]
-            )
+            playlist = self.get_playlist_audio_from_user(m3u8_master_data["media"])
+        stream_info.stream_url = playlist["uri"]
+        stream_info.codec = re.search(r"_([^_]+)\.m3u8", stream_info.stream_url).group(
+            1
+        )
         m3u8_data = m3u8.load(stream_info.stream_url).data
         stream_info.pssh = self.get_pssh(m3u8_data)
         return stream_info
 
     def get_music_video_id_alt(self, metadata: dict) -> str:
         return metadata["attributes"]["url"].split("/")[-1].split("?")[0]
 
@@ -251,52 +252,61 @@
         )
 
     def remux_ffmpeg(
         self,
         decrypted_path_video: Path,
         decrypte_path_audio: Path,
         fixed_path: Path,
+        codec_video: str,
+        codec_audio: str,
     ):
+        use_mp4_flag = any(
+            codec_video.startswith(codec) for codec in self.MP4_FORMAT_CODECS
+        ) or any(codec_audio.startswith(codec) for codec in self.MP4_FORMAT_CODECS)
         subprocess.run(
             [
                 self.downloader.ffmpeg_path_full,
                 "-loglevel",
                 "error",
                 "-y",
                 "-i",
                 decrypted_path_video,
                 "-i",
                 decrypte_path_audio,
                 "-movflags",
                 "+faststart",
                 "-f",
-                "mp4",
+                "mp4" if use_mp4_flag else "ipod",
                 "-c",
                 "copy",
                 "-c:s",
                 "mov_text",
                 fixed_path,
             ],
             check=True,
         )
 
     def remux(
         self,
         decrypted_path_video: Path,
         decrypted_path_audio: Path,
         remuxed_path: Path,
+        codec_video: str,
+        codec_audio: str,
     ):
         if self.downloader.remux_mode == RemuxMode.MP4BOX:
             self.remux_mp4box(
                 decrypted_path_audio,
                 decrypted_path_video,
                 remuxed_path,
             )
         elif self.downloader.remux_mode == RemuxMode.FFMPEG:
             self.remux_ffmpeg(
                 decrypted_path_video,
                 decrypted_path_audio,
                 remuxed_path,
+                codec_video,
+                codec_audio,
             )
 
     def get_cover_path(self, final_path: Path) -> Path:
         return final_path.with_suffix(f".{self.downloader.cover_format.value}")
```

### Comparing `gamdl-2.0/gamdl/downloader_post.py` & `gamdl-2.1/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/downloader_song.py` & `gamdl-2.1/gamdl/downloader_song.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .downloader import Downloader
 from .enums import RemuxMode, SongCodec, SyncedLyricsFormat
 from .models import Lyrics, StreamInfo
 
 
 class DownloaderSong:
     DEFAULT_DECRYPTION_KEY = "32b8ade1769e26b1ffb8986352793fc6"
+    MP4_FORMAT_CODECS = ["ec-3"]
 
     def __init__(
         self,
         downloader: Downloader,
         codec: SongCodec = SongCodec.AAC_LEGACY,
         synced_lyrics_format: SyncedLyricsFormat = SyncedLyricsFormat.LRC,
     ):
@@ -119,14 +120,15 @@
         if playlist is None:
             return stream_info
         stream_info.stream_url = m3u8_obj.base_uri + playlist["uri"]
         variant_id = playlist["stream_info"]["stable_variant_id"]
         drm_ids = asset_infos[variant_id]["AUDIO-SESSION-KEY-IDS"]
         pssh = self.get_pssh(drm_infos, drm_ids)
         stream_info.pssh = pssh
+        stream_info.codec = playlist["stream_info"]["codecs"]
         return stream_info
 
     @staticmethod
     def parse_datetime_obj_from_timestamp_ttml(
         timestamp_ttml: str,
     ) -> datetime.datetime:
         mins_secs_ms = re.findall(r"\d+", timestamp_ttml)
@@ -290,46 +292,56 @@
                 "--key",
                 f"00000000000000000000000000000000:{self.DEFAULT_DECRYPTION_KEY}",
                 decrypted_path,
             ],
             check=True,
         )
 
-    def remux(self, decrypted_path: Path, remuxed_path: Path) -> None:
+    def remux(self, decrypted_path: Path, remuxed_path: Path, codec: str):
         if self.downloader.remux_mode == RemuxMode.MP4BOX:
             self.remux_mp4box(decrypted_path, remuxed_path)
         elif self.downloader.remux_mode == RemuxMode.FFMPEG:
-            self.remux_ffmpeg(decrypted_path, remuxed_path)
+            self.remux_ffmpeg(decrypted_path, remuxed_path, codec)
 
-    def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path) -> None:
+    def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path):
         subprocess.run(
             [
                 self.downloader.mp4box_path_full,
                 "-quiet",
                 "-add",
                 decrypted_path,
                 "-itags",
                 "artist=placeholder",
                 "-new",
                 remuxed_path,
             ],
             check=True,
         )
 
-    def remux_ffmpeg(self, decrypted_path: Path, remuxed_path: Path) -> None:
+    def remux_ffmpeg(
+        self,
+        decrypted_path: Path,
+        remuxed_path: Path,
+        codec: str,
+    ):
+        use_mp4_format = any(
+            codec.startswith(possible_codec) for possible_codec in self.MP4_FORMAT_CODECS
+        )
         subprocess.run(
             [
                 self.downloader.ffmpeg_path_full,
                 "-loglevel",
                 "error",
                 "-y",
                 "-i",
                 decrypted_path,
                 "-c",
                 "copy",
+                "-f",
+                "mp4" if use_mp4_format else "ipod",
                 "-movflags",
                 "+faststart",
                 remuxed_path,
             ],
             check=True,
         )
```

### Comparing `gamdl-2.0/gamdl/downloader_song_legacy.py` & `gamdl-2.1/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/enums.py` & `gamdl-2.1/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/hardcoded_wvd.py` & `gamdl-2.1/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/gamdl/itunes_api.py` & `gamdl-2.1/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/pyproject.toml` & `gamdl-2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.0/PKG-INFO` & `gamdl-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.0
+Version: 2.1
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
```

