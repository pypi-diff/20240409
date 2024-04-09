# Comparing `tmp/aiosu-2.2.2.tar.gz` & `tmp/aiosu-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosu-2.2.2.tar", max compression
+gzip compressed data, was "aiosu-2.3.0.tar", max compression
```

## Comparing `aiosu-2.2.2.tar` & `aiosu-2.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35149 2024-03-03 10:17:09.133109 aiosu-2.2.2/LICENSE
--rw-r--r--   0        0        0     3862 2024-03-03 10:17:09.133109 aiosu-2.2.2/README.rst
--rw-r--r--   0        0        0      682 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/__init__.py
--rw-r--r--   0        0        0     2292 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/events.py
--rw-r--r--   0        0        0     1053 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/exceptions.py
--rw-r--r--   0        0        0     2394 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/helpers.py
--rw-r--r--   0        0        0      655 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/__init__.py
--rw-r--r--   0        0        0     2705 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/artist.py
--rw-r--r--   0        0        0      407 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/backgrounds.py
--rw-r--r--   0        0        0     1335 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/base.py
--rw-r--r--   0        0        0    19824 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/beatmap.py
--rw-r--r--   0        0        0     2202 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/changelog.py
--rw-r--r--   0        0        0     1742 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/chat.py
--rw-r--r--   0        0        0     1762 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/comment.py
--rw-r--r--   0        0        0     3620 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/common.py
--rw-r--r--   0        0        0     1822 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/event.py
--rw-r--r--   0        0        0      104 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/files/__init__.py
--rw-r--r--   0        0        0     2798 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/files/replay.py
--rw-r--r--   0        0        0     1697 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/forum.py
--rw-r--r--   0        0        0     1903 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/gamemode.py
--rw-r--r--   0        0        0      764 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/kudosu.py
--rw-r--r--   0        0        0     6354 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/lazer.py
--rw-r--r--   0        0        0      133 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/legacy/__init__.py
--rw-r--r--   0        0        0     3442 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/legacy/match.py
--rw-r--r--   0        0        0      272 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/legacy/replay.py
--rw-r--r--   0        0        0     6425 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/mods.py
--rw-r--r--   0        0        0     4874 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/multiplayer.py
--rw-r--r--   0        0        0     1111 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/news.py
--rw-r--r--   0        0        0     1959 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/oauthtoken.py
--rw-r--r--   0        0        0      840 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/performance.py
--rw-r--r--   0        0        0      693 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/rankings.py
--rw-r--r--   0        0        0     1491 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/scopes.py
--rw-r--r--   0        0        0     7893 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/score.py
--rw-r--r--   0        0        0      590 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/search.py
--rw-r--r--   0        0        0      511 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/spotlight.py
--rw-r--r--   0        0        0    10766 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/user.py
--rw-r--r--   0        0        0      386 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/models/wiki.py
--rw-r--r--   0        0        0        0 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/py.typed
--rw-r--r--   0        0        0      218 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/utils/__init__.py
--rw-r--r--   0        0        0     8721 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/utils/accuracy.py
--rw-r--r--   0        0        0     2824 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/utils/auth.py
--rw-r--r--   0        0        0     7976 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/utils/binary.py
--rw-r--r--   0        0        0    22058 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/utils/performance.py
--rw-r--r--   0        0        0     6230 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/utils/replay.py
--rw-r--r--   0        0        0       98 2024-03-03 10:17:09.133109 aiosu-2.2.2/aiosu/v1/__init__.py
--rw-r--r--   0        0        0    18341 2024-03-03 10:17:09.137109 aiosu-2.2.2/aiosu/v1/client.py
--rw-r--r--   0        0        0      146 2024-03-03 10:17:09.137109 aiosu-2.2.2/aiosu/v2/__init__.py
--rw-r--r--   0        0        0   104188 2024-03-03 10:17:09.137109 aiosu-2.2.2/aiosu/v2/client.py
--rw-r--r--   0        0        0     7792 2024-03-03 10:17:09.137109 aiosu-2.2.2/aiosu/v2/clientstorage.py
--rw-r--r--   0        0        0       95 2024-03-03 10:17:09.137109 aiosu-2.2.2/aiosu/v2/repository/__init__.py
--rw-r--r--   0        0        0     1906 2024-03-03 10:17:09.137109 aiosu-2.2.2/aiosu/v2/repository/oauthtoken.py
--rw-r--r--   0        0        0     2028 2024-03-03 10:17:09.137109 aiosu-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 aiosu-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 07:06:41.745397 aiosu-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3862 2024-04-09 07:06:41.745397 aiosu-2.3.0/README.rst
+-rw-r--r--   0        0        0      682 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/__init__.py
+-rw-r--r--   0        0        0     2292 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/events.py
+-rw-r--r--   0        0        0     1053 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/exceptions.py
+-rw-r--r--   0        0        0     3286 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/helpers.py
+-rw-r--r--   0        0        0      655 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/__init__.py
+-rw-r--r--   0        0        0     2717 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/artist.py
+-rw-r--r--   0        0        0      407 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/backgrounds.py
+-rw-r--r--   0        0        0     1335 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/base.py
+-rw-r--r--   0        0        0    19824 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/beatmap.py
+-rw-r--r--   0        0        0     2202 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/changelog.py
+-rw-r--r--   0        0        0     1742 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/chat.py
+-rw-r--r--   0        0        0     1762 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/comment.py
+-rw-r--r--   0        0        0     3620 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/common.py
+-rw-r--r--   0        0        0     1822 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/event.py
+-rw-r--r--   0        0        0      104 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/files/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/files/replay.py
+-rw-r--r--   0        0        0     1697 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/forum.py
+-rw-r--r--   0        0        0     1903 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/gamemode.py
+-rw-r--r--   0        0        0      764 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/kudosu.py
+-rw-r--r--   0        0        0     6354 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/lazer.py
+-rw-r--r--   0        0        0      133 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/legacy/__init__.py
+-rw-r--r--   0        0        0     3442 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/legacy/match.py
+-rw-r--r--   0        0        0      272 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/legacy/replay.py
+-rw-r--r--   0        0        0     6425 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/mods.py
+-rw-r--r--   0        0        0     4874 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/multiplayer.py
+-rw-r--r--   0        0        0     1111 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/news.py
+-rw-r--r--   0        0        0     1959 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/oauthtoken.py
+-rw-r--r--   0        0        0      840 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/performance.py
+-rw-r--r--   0        0        0      693 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/rankings.py
+-rw-r--r--   0        0        0     1491 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/scopes.py
+-rw-r--r--   0        0        0     7893 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/score.py
+-rw-r--r--   0        0        0      590 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/search.py
+-rw-r--r--   0        0        0      511 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/spotlight.py
+-rw-r--r--   0        0        0    10766 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/user.py
+-rw-r--r--   0        0        0      386 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/wiki.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/py.typed
+-rw-r--r--   0        0        0      218 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/__init__.py
+-rw-r--r--   0        0        0     8721 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/accuracy.py
+-rw-r--r--   0        0        0     2824 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/auth.py
+-rw-r--r--   0        0        0     7976 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/binary.py
+-rw-r--r--   0        0        0    22058 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/performance.py
+-rw-r--r--   0        0        0     6230 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/replay.py
+-rw-r--r--   0        0        0       98 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v1/__init__.py
+-rw-r--r--   0        0        0    18341 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v1/client.py
+-rw-r--r--   0        0        0      146 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/__init__.py
+-rw-r--r--   0        0        0   104324 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/client.py
+-rw-r--r--   0        0        0     7792 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/clientstorage.py
+-rw-r--r--   0        0        0       95 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/repository/__init__.py
+-rw-r--r--   0        0        0     1906 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/repository/oauthtoken.py
+-rw-r--r--   0        0        0     2028 2024-04-09 07:06:41.749397 aiosu-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 aiosu-2.3.0/PKG-INFO
```

### Comparing `aiosu-2.2.2/LICENSE` & `aiosu-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/README.rst` & `aiosu-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/__init__.py` & `aiosu-2.3.0/aiosu/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/events.py` & `aiosu-2.3.0/aiosu/events.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/exceptions.py` & `aiosu-2.3.0/aiosu/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/__init__.py` & `aiosu-2.3.0/aiosu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/artist.py` & `aiosu-2.3.0/aiosu/models/artist.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from .beatmap import Beatmapset
 from .common import CursorModel
 
 __all__ = (
     "Artist",
     "ArtistAlbum",
     "ArtistLabel",
-    "ArtistResponse",
     "ArtistSearch",
     "ArtistSortType",
     "ArtistTrack",
+    "ArtistTracksResponse",
 )
 
 ArtistSortType = Literal[
     "album_asc",
     "album_desc",
     "artist_asc",
     "artist_desc",
@@ -112,12 +112,12 @@
     preview_url: str = Field(alias="preview")
     album: Optional[ArtistAlbum] = None
     album_id: Optional[int] = None
     updated_at: Optional[datetime] = None
     version: Optional[str] = None
 
 
-class ArtistResponse(CursorModel):
+class ArtistTracksResponse(CursorModel):
     """Artist response model."""
 
     artist_tracks: list[ArtistTrack]
     search: Optional[ArtistSearch] = None
```

### Comparing `aiosu-2.2.2/aiosu/models/base.py` & `aiosu-2.3.0/aiosu/models/base.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/beatmap.py` & `aiosu-2.3.0/aiosu/models/beatmap.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/changelog.py` & `aiosu-2.3.0/aiosu/models/changelog.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/chat.py` & `aiosu-2.3.0/aiosu/models/chat.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/comment.py` & `aiosu-2.3.0/aiosu/models/comment.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/common.py` & `aiosu-2.3.0/aiosu/models/common.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/event.py` & `aiosu-2.3.0/aiosu/models/event.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/files/replay.py` & `aiosu-2.3.0/aiosu/models/files/replay.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/forum.py` & `aiosu-2.3.0/aiosu/models/forum.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/gamemode.py` & `aiosu-2.3.0/aiosu/models/gamemode.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/kudosu.py` & `aiosu-2.3.0/aiosu/models/kudosu.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/lazer.py` & `aiosu-2.3.0/aiosu/models/lazer.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/legacy/match.py` & `aiosu-2.3.0/aiosu/models/legacy/match.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/mods.py` & `aiosu-2.3.0/aiosu/models/mods.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/multiplayer.py` & `aiosu-2.3.0/aiosu/models/multiplayer.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/news.py` & `aiosu-2.3.0/aiosu/models/news.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/oauthtoken.py` & `aiosu-2.3.0/aiosu/models/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/performance.py` & `aiosu-2.3.0/aiosu/models/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/rankings.py` & `aiosu-2.3.0/aiosu/models/rankings.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/scopes.py` & `aiosu-2.3.0/aiosu/models/scopes.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/score.py` & `aiosu-2.3.0/aiosu/models/score.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/search.py` & `aiosu-2.3.0/aiosu/models/search.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/models/user.py` & `aiosu-2.3.0/aiosu/models/user.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/utils/accuracy.py` & `aiosu-2.3.0/aiosu/utils/accuracy.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/utils/auth.py` & `aiosu-2.3.0/aiosu/utils/auth.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/utils/binary.py` & `aiosu-2.3.0/aiosu/utils/binary.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/utils/performance.py` & `aiosu-2.3.0/aiosu/utils/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/utils/replay.py` & `aiosu-2.3.0/aiosu/utils/replay.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/v1/client.py` & `aiosu-2.3.0/aiosu/v1/client.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/v2/client.py` & `aiosu-2.3.0/aiosu/v2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 from aiolimiter import AsyncLimiter
 
 from ..events import ClientUpdateEvent
 from ..events import Eventable
 from ..exceptions import APIException
 from ..exceptions import RefreshTokenExpiredError
 from ..helpers import add_param
+from ..helpers import add_range
 from ..helpers import append_param
 from ..helpers import from_list
-from ..models import ArtistResponse
+from ..models import ArtistTracksResponse
 from ..models import Beatmap
 from ..models import BeatmapDifficultyAttributes
 from ..models import BeatmapPack
 from ..models import BeatmapPacksResponse
 from ..models import BeatmapPackType
 from ..models import Beatmapset
 from ..models import BeatmapsetDiscussionPostResponse
@@ -341,15 +342,14 @@
         if self._session is None:
             self._session = aiohttp.ClientSession(headers=await self._get_headers())
 
         async with self._limiter:
             async with self._session.request(request_type, *args, **kwargs) as resp:
                 if resp.status == 204:
                     return
-
                 body = await resp.read()
                 content_type = get_content_type(resp.headers.get("content-type", ""))
                 if resp.status != 200:
                     json = {}
                     if content_type == "application/json":
                         json = orjson.loads(body)
                     raise APIException(resp.status, json.get("error", ""))
@@ -404,61 +404,61 @@
                     )
 
         await self._process_event(
             ClientUpdateEvent(client=self, old_token=old_token, new_token=new_token),
         )
 
     @prepare_token
-    async def get_featured_artists(self, **kwargs: Any) -> ArtistResponse:
-        r"""Gets the current featured artists.
+    async def get_featured_tracks(self, **kwargs: Any) -> ArtistTracksResponse:
+        r"""Query tracks from featured artists.
 
         :param \**kwargs:
             See below
 
         :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the number of featured artists to return.
             * *album* (``str``) --
                 Optional, the album to filter by.
             * *artist* (``str``) --
                 Optional, the artist to filter by.
             * *genre* (``int``) --
                 Optional, the genre ID to filter by.
-            * *length* (``list[int]``) --
+            * *length* (``tuple[int, int]``) --
                 Optional, the length range to filter by.
-            * *bpm* (``list[int]``) --
+            * *bpm* (``tuple[int, int]``) --
                 Optional, The BPM range to filter by.
             * *query* (``str``) --
                 Optional, the search query to filter by.
             * *is_default_sort* (``bool``) --
                 Optional, whether to sort by the default sort.
             * *sort* (``str``) --
                 Optional, the sort to use.
+            * *exclusive_only* (``bool``) --
+                Optional, whether to only get osu! exclusive tracks.
 
         :raises APIException: Contains status code and error message
-        :return: Featured artist response object
-        :rtype: aiosu.models.artist.ArtistResponse
+        :return: Featured artist tracks response object
+        :rtype: aiosu.models.artist.ArtistTracksResponse
         """
         url = f"{self.base_url}/beatmaps/artists/tracks"
         params: dict[str, object] = {}
-        add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="album")
         add_param(params, kwargs, key="artist")
         add_param(params, kwargs, key="genre")
-        add_param(params, kwargs, key="length")
-        add_param(params, kwargs, key="bpm")
+        add_range(params, kwargs, key="length")
+        add_range(params, kwargs, key="bpm")
         add_param(params, kwargs, key="query")
         add_param(params, kwargs, key="is_default_sort", converter=to_lower_str)
         add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="exclusive_only", converter=to_lower_str)
         add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url)
-        resp = ArtistResponse.model_validate(json)
+        json = await self._request("GET", url, params=params)
+        resp = ArtistTracksResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_featured_artists, **kwargs)
+            resp.next = partial(self.get_featured_tracks, **kwargs)
         return resp
 
     @prepare_token
     async def get_seasonal_backgrounds(self) -> SeasonalBackgroundSet:
         r"""Gets the current seasonal background set.
 
         :raises APIException: Contains status code and error message
@@ -820,15 +820,15 @@
         :raises APIException: Contains status code and error message
         :raises RefreshTokenExpiredError: If the client refresh token has expired
         :return: List of user data objects
         :rtype: list[aiosu.models.user.User]
         """
         url = f"{self.base_url}/api/v2/users"
         params: dict[str, object] = {
-            "ids": user_ids,
+            "ids[]": user_ids,
         }
         json = await self._request("GET", url, params=params)
         return from_list(User.model_validate, json.get("users", []))
 
     @prepare_token
     @check_token
     @requires_scope(Scopes.PUBLIC)
@@ -1684,15 +1684,15 @@
         """
         url = f"{self.base_url}/api/v2/beatmapsets/discussions/posts"
         params: dict[str, object] = {}
         add_param(params, kwargs, key="beatmapset_discussion_id")
         add_param(params, kwargs, key="limit")
         add_param(params, kwargs, key="page")
         add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="types")
+        add_param(params, kwargs, key="types[]")
         add_param(params, kwargs, key="user", param_name="user_id")
         add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
         add_param(params, kwargs, key="cursor_string")
         json = await self._request("GET", url, params=params)
         resp = BeatmapsetDiscussionPostResponse.model_validate(json)
         if resp.cursor_string:
             kwargs["cursor_string"] = resp.cursor_string
@@ -2250,15 +2250,15 @@
             See below
 
         :Keyword Arguments:
             * *message* (``str``) --
                 Required if type is ``ANNOUNCE``, the message to send in the PM
             * *target_id* (``int``) --
                 Only used if if type is ``PM``, the ID of the user to send a PM to
-            * *target_ids* (``List[int]``) --
+            * *target_ids* (``list[int]``) --
                 Only used if type is ``ANNOUNCE``, the IDs of the users to send a PM to
             * *channel_name* (``str``) --
                 Only used if type is ``ANNOUNCE``, the name of the channel
             * *channel_description* (``str``) --
                 Only used if type is ``ANNOUNCE``, the description of the channel
 
         :raises ValueError: If missing required parameters
```

### Comparing `aiosu-2.2.2/aiosu/v2/clientstorage.py` & `aiosu-2.3.0/aiosu/v2/clientstorage.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/aiosu/v2/repository/oauthtoken.py` & `aiosu-2.3.0/aiosu/v2/repository/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.2.2/pyproject.toml` & `aiosu-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 profile = "black"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.poetry]
 name = "aiosu"
-version = "2.2.2"
+version = "2.3.0"
 description = "Simple and fast osu! API v1 and v2 library"
 authors = ["Nice Aesthetics <nice@aesth.dev>"]
 license = "GPLv3+"
 readme = "README.rst"
 repository = "https://github.com/NiceAesth/aiosu"
 documentation = "https://aiosu.readthedocs.io/"
 keywords = ["osu!", "osu", "api"]
@@ -54,15 +54,15 @@
 pytest-asyncio = "^0.23.5"
 pytest-mock = "^3.10.0"
 mypy = "^1.0"
 toml = "^0.10.2"
 types-toml = "^0.10.8.1"
 sphinx = "^7.0.0"
 furo = "^2024.0.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 black = { version = "^24.0.0", allow-prereleases = true }
 pre-commit = "^3.2.2"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-asyncio", "pytest-mock", "toml", "types-toml"]
 docs = ["Sphinx", "furo", "toml"]
```

### Comparing `aiosu-2.2.2/PKG-INFO` & `aiosu-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosu
-Version: 2.2.2
+Version: 2.3.0
 Summary: Simple and fast osu! API v1 and v2 library
 Home-page: https://github.com/NiceAesth/aiosu
 License: GPLv3+
 Keywords: osu!,osu,api
 Author: Nice Aesthetics
 Author-email: nice@aesth.dev
 Requires-Python: >=3.9,<4.0
```

