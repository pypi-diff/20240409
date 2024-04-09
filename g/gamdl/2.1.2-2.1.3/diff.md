# Comparing `tmp/gamdl-2.1.2.tar.gz` & `tmp/gamdl-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.2.tar` & `gamdl-2.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1137 2024-04-09 00:09:03.183159 gamdl-2.1.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-09 00:09:03.183159 gamdl-2.1.2/.gitignore
--rw-r--r--   0        0        0    11148 2024-04-09 00:09:03.183159 gamdl-2.1.2/README.md
--rw-r--r--   0        0        0       22 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26235 2024-04-09 00:09:03.183159 gamdl-2.1.2/gamdl/cli.py
--rw-r--r--   0        0        0     5522 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/constants.py
--rw-r--r--   0        0        0    12570 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader.py
--rw-r--r--   0        0        0    10356 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2121 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13741 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3691 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      801 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-09 00:09:03.187159 gamdl-2.1.2/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-09 00:09:03.187159 gamdl-2.1.2/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-09 00:09:03.187159 gamdl-2.1.2/requirements.txt
--rw-r--r--   0        0        0    11623 1970-01-01 00:00:00.000000 gamdl-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-09 09:56:05.135619 gamdl-2.1.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-09 09:56:05.135619 gamdl-2.1.3/.gitignore
+-rw-r--r--   0        0        0    11240 2024-04-09 09:56:05.135619 gamdl-2.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26304 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/cli.py
+-rw-r--r--   0        0        0     5544 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/constants.py
+-rw-r--r--   0        0        0    12570 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader.py
+-rw-r--r--   0        0        0    10356 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2121 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13741 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3691 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      801 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-09 09:56:05.135619 gamdl-2.1.3/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-09 09:56:05.135619 gamdl-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-09 09:56:05.135619 gamdl-2.1.3/requirements.txt
+-rw-r--r--   0        0        0    11715 1970-01-01 00:00:00.000000 gamdl-2.1.3/PKG-INFO
```

### Comparing `gamdl-2.1.2/.github/workflows/main.yml` & `gamdl-2.1.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/README.md` & `gamdl-2.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     * Binaries can be obtained from here: https://www.bento4.com/downloads/.
  
 ## Installation
 1. Install the package `gamdl` using pip
     ```bash
     pip install gamdl
     ```
-2. Place your cookies in the same directory you will run the script from and name it as `cookies.txt`
+2. Place your cookies in the same directory you will run gamdl from and name it as `cookies.txt`
 
 ## Usage
 * Download a song
     ```bash
     gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1626265761?i=1626265765"
     ```
 * Download an album
@@ -140,16 +140,18 @@
 * `aac-he`
 * `aac-binaural`
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
 * `alac`
 * `atmos`
+* `ask`
+    * When using this option, the script will ask you which **non-legacy** codec to use.
 
-**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be decrypted  when using non-legacy codecs.**
+**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
 * `h264-best` (with AAC 256kbps, up to 1080p)
 * `h265-best` (With AAC 256kpbs, up to 2160p)
 * `ask`
     * When using this option, the script will ask you which audio and video codec to use.
```

### Comparing `gamdl-2.1.2/gamdl/apple_music_api.py` & `gamdl-2.1.3/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/cli.py` & `gamdl-2.1.3/gamdl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,14 +415,19 @@
             logger.warn(
                 X_NOT_FOUND_STRING.format("mp4decrypt", mp4decrypt_path)
                 + ", music videos will not be downloaded"
             )
             skip_mv = True
         else:
             skip_mv = False
+        if codec_song not in LEGACY_CODECS:
+            logger.warn(
+                "You have chosen a non-legacy codec. Support for non-legacy codecs are not guaranteed, "
+                "as most of the songs cannot be downloaded when using non-legacy codecs."
+            )
     error_count = 0
     if read_urls_as_txt:
         urls = [url.strip() for url in Path(urls[0]).read_text().splitlines()]
     for url_index, url in enumerate(urls, start=1):
         url_progress = f"URL {url_index}/{len(urls)}"
         try:
             url_info = downloader.get_url_info(url)
@@ -473,47 +478,41 @@
                     if synced_lyrics_only:
                         pass
                     elif final_path.exists() and not overwrite:
                         logger.warning(
                             f'({queue_progress}) Song already exists at "{final_path}", skipping'
                         )
                     else:
-                        if codec_song in (
-                            SongCodec.AAC_LEGACY,
-                            SongCodec.AAC_HE_LEGACY,
-                        ):
+                        if codec_song in LEGACY_CODECS:
                             logger.debug("Getting stream info")
                             stream_info = downloader_song_legacy.get_stream_info(
                                 webplayback
                             )
                             logger.debug("Getting decryption key")
                             decryption_key = downloader_song_legacy.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
                         else:
                             stream_info = downloader_song.get_stream_info(track)
-                            if not stream_info.stream_url:
+                            if not stream_info.stream_url or not stream_info.codec:
                                 logger.warning(
                                     f"({queue_progress}) Song is not downloadable or is not"
                                     " available in the chosen codec, skipping"
                                 )
                                 continue
                             logger.debug("Getting decryption key")
                             decryption_key = downloader.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
                         encrypted_path = downloader_song.get_encrypted_path(track["id"])
                         decrypted_path = downloader_song.get_decrypted_path(track["id"])
                         remuxed_path = downloader_song.get_remuxed_path(track["id"])
                         logger.debug(f"Downloading to {encrypted_path}")
                         downloader.download(encrypted_path, stream_info.stream_url)
-                        if codec_song in (
-                            SongCodec.AAC_LEGACY,
-                            SongCodec.AAC_HE_LEGACY,
-                        ):
+                        if codec_song in LEGACY_CODECS:
                             logger.debug(f"Remuxing/Decrypting to {remuxed_path}")
                             downloader_song_legacy.remux(
                                 encrypted_path,
                                 decrypted_path,
                                 remuxed_path,
                                 decryption_key,
                             )
```

### Comparing `gamdl-2.1.2/gamdl/constants.py` & `gamdl-2.1.3/gamdl/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,8 +214,11 @@
     "no_config_file",
     "version",
     "help",
 )
 
 X_NOT_FOUND_STRING = '{} not found at "{}"'
 
-AMP_API_HOSTNAME = "https://amp-api.music.apple.com"
+LEGACY_CODECS = [
+    SongCodec.AAC_LEGACY,
+    SongCodec.AAC_HE_LEGACY,
+]
```

### Comparing `gamdl-2.1.2/gamdl/downloader.py` & `gamdl-2.1.3/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/downloader_music_video.py` & `gamdl-2.1.3/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/downloader_post.py` & `gamdl-2.1.3/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/downloader_song.py` & `gamdl-2.1.3/gamdl/downloader_song.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/downloader_song_legacy.py` & `gamdl-2.1.3/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/enums.py` & `gamdl-2.1.3/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/hardcoded_wvd.py` & `gamdl-2.1.3/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/gamdl/itunes_api.py` & `gamdl-2.1.3/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/pyproject.toml` & `gamdl-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.2/PKG-INFO` & `gamdl-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.2
+Version: 2.1.3
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
@@ -42,15 +42,15 @@
     * Binaries can be obtained from here: https://www.bento4.com/downloads/.
  
 ## Installation
 1. Install the package `gamdl` using pip
     ```bash
     pip install gamdl
     ```
-2. Place your cookies in the same directory you will run the script from and name it as `cookies.txt`
+2. Place your cookies in the same directory you will run gamdl from and name it as `cookies.txt`
 
 ## Usage
 * Download a song
     ```bash
     gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1626265761?i=1626265765"
     ```
 * Download an album
@@ -157,16 +157,18 @@
 * `aac-he`
 * `aac-binaural`
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
 * `alac`
 * `atmos`
+* `ask`
+    * When using this option, the script will ask you which **non-legacy** codec to use.
 
-**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be decrypted  when using non-legacy codecs.**
+**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
 * `h264-best` (with AAC 256kbps, up to 1080p)
 * `h265-best` (With AAC 256kpbs, up to 2160p)
 * `ask`
     * When using this option, the script will ask you which audio and video codec to use.
```

