# Comparing `tmp/ncmlistdownloader-1.0.0.240407b1.tar.gz` & `tmp/ncmlistdownloader-1.0.0.240408a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240407b1.tar", last modified: Sun Apr  7 14:49:27 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.0.240408a1.tar", last modified: Mon Apr  8 14:54:12 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240407b1.tar` & `ncmlistdownloader-1.0.0.240408a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.439933 ncmlistdownloader-1.0.0.240407b1/
--rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240407b1/LICENSE
--rw-rw-rw-   0        0        0     1398 2024-04-07 14:49:27.437933 ncmlistdownloader-1.0.0.240407b1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.396888 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1531 2024-04-07 14:32:39.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.421545 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     1785 2024-04-02 10:13:15.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.424890 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.427070 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.431026 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     1660 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.433701 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     6091 2024-04-07 14:32:56.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.436349 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1398 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 14:49:27.439933 ncmlistdownloader-1.0.0.240407b1/setup.cfg
--rw-rw-rw-   0        0        0     1700 2024-04-07 14:33:40.000000 ncmlistdownloader-1.0.0.240407b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.226579 ncmlistdownloader-1.0.0.240408a1/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240408a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-08 14:54:12.226579 ncmlistdownloader-1.0.0.240408a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.191360 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1264 2024-04-08 14:52:37.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.209135 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2137 2024-04-08 14:53:36.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.215050 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.217043 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.219038 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     1660 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.221507 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     6146 2024-04-08 14:41:40.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:54:12.225440 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-08 14:54:12.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2024-04-08 14:54:12.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:54:12.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-08 14:54:12.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-08 14:54:12.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-08 14:54:12.000000 ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:54:12.226579 ncmlistdownloader-1.0.0.240408a1/setup.cfg
+-rw-rw-rw-   0        0        0     1700 2024-04-08 14:53:57.000000 ncmlistdownloader-1.0.0.240408a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240407b1/LICENSE` & `ncmlistdownloader-1.0.0.240408a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/PKG-INFO` & `ncmlistdownloader-1.0.0.240408a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240407b1
+Version: 1.0.0.240408a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 '''
 ncmlistdownloader/__init__.py
-Core.Ver.1.0.0.240407b1
+Core.Ver.1.0.0.240408a1
 Author: CooooldWind_
 '''
+from pathlib import Path
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common import *
+from ncmlistdownloader.common.global_args import *
 
 def main():
-    print("163ListDownloader CMD Ver.")
-    print("Core.Ver.1.0.0.240407b1 / Made by CooooldWind_")
-    print("Warning: It's an Beta Version. It may has a lot of bugs.")
-    print("If you met them, click the links below:")
-    print("Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues")
-    print("GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues")
+    for i in CMD_START_WORDS:
+        print(i)
+    print('Core.Ver.1.0.0.240408a1')
     id = str(input("ID: "))
     p = Playlist(id)
     p.get_info()
     p.get_detail_info()
     print("Playlist info-reading succeed.")
     d = str(input("Dir: "))
     if d == '':
-        d = '%USERPROFILE%/Downloads/ncmlistdownloader/'
+        d = str(Path.home()) + '/Downloads/ncmld_downloads/'
     fnf = str(input("Filename format: "))
     if fnf == '':
         fnf = '$title$ - $artist$'
     if d[-1] != '/' and d[-1] != '\\':
         d += '/'
     d = d.replace('\\', '/')
     auto_mkdir(d)
     for i in p.track:
         i.filename_format = d + fnf
+    p.get_detail_info()
+    for i in p.track:
         music_filename = i.song_download()
         if music_filename == -1:
-            print(i.title + 'cannot download.')
+            print(i.title + ' cannot download.')
             continue
-        cover_filename = i.cover_download()
-        lyric_filename = i.lyric_get()
-        i.attribute_write(music_filename)
-        i.cover_write(music_filename, cover_filename)
-        i.lyric_write(music_filename, lyric_filename)
-        print(i.title + 'Succeed.')
-    print('Succeed.')
+        i.cover_download()
+        i.lyric_get()
+        i.attribute_write()
+        i.cover_write()
+        i.lyric_write()
+        print(i.title + ' succeed.')
+    print('Succeed. Files at:', d)
```

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/global_args.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 list_downloader/global_args.py
-Core.Ver.1.0.0.240328a1
+Core.Ver.1.0.0.240408a1
 Author: CooooldWind_, 是青旨啊
 '''
 FUNC_F_PART = [
   "00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7",
   "b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280",
   "104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932",
   "575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b",
@@ -36,7 +36,15 @@
 FUNC_F = json_file['FUNC_F']
 SEC_KEY = json_file['SEC_KEY']
 PLAYLIST_API = json_file['PLAYLIST_API']
 SONG_INFO_API = json_file['SONG_INFO_API']
 SONG_FILE_API = json_file['SONG_FILE_API']
 SONG_FILE_API_2 = json_file['SONG_FILE_API_2']
 LYRIC_API = json_file['LYRIC_API']
+CMD_START_WORDS = [
+    "163ListDownloader CMD Ver.",
+    "Made by CooooldWind_",
+    "Warning: It's an Alpha Version. It may has a lot of bugs.",
+    "If you met them, click the links below:",
+    "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
+    "GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues",
+]
```

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader/song/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/Song/__init__.py
-Core.Ver.1.0.0.240407b1
+Core.Ver.1.0.0.240408a1
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -44,25 +44,42 @@
             'id': str(str(self.id)),
             'lv': -1,
             'tv': -1,
         }
         self.raw_info = {}
         self.processed_info = {}
         self.url_info = {}
+        self.filename_info = {}
         self.filename_format = '$title$ - $artist$'
 
     def __str__(self):
         '''
         返回存有歌曲信息的字符串。
         ----------
         无参数。
         如果直接`print`这个类就是调用这个函数了。
         '''
         return str(self.processed_info)
     
+    def get_formated_filename(self, suffix):
+        format_info = self.processed_info
+        format_info.update({
+            'filename': self.filename_format,
+            'artist': self.artist_str,
+            'album': self.album,
+            'id': self.id,
+            'title': self.title,
+            })
+        formated = format(**format_info) + '.' + suffix
+        if formated.rfind('/') != -1:
+            formated = formated[:formated.rfind('/') + 1] + clean(formated[formated.rfind('/') + 1:])
+        else:
+            formated = clean(formated)
+        return formated
+
     def get_info(self):
         '''
         获取歌曲信息
         ----------
         无参数。
         '''
         self.raw_info = NeteaseParams(
@@ -73,47 +90,36 @@
         for i in self.raw_info['ar']:
             self.artist.append(i['name'])
         self.artist_str = artist_turn_str(self.artist)
         self.processed_info = {
             'album': self.album,
             'title': self.title,
             'artist': self.artist,
-            'id': self.id
+            'id': self.id,
         }
         self.url_info.update({
             'album_pic': self.raw_info['al']['picUrl'],
             'song_file': SONG_FILE_API + self.id,
         })
+        self.filename_info.update({
+            'song': self.get_formated_filename('mp3'),
+            'pic': self.get_formated_filename('jpg'),
+            'lyric': self.get_formated_filename('lrc'),
+        })
         return self.raw_info
     
     def multi_get_info(self):
         '''
         获取歌曲信息（多线程用）
         ----------
         无参数。
         '''
         with threading.Semaphore(8):
             self.get_info()
 
-    def get_formated_filename(self, suffix):
-        format_info = self.processed_info
-        format_info.update({
-            'filename': self.filename_format,
-            'artist': self.artist_str,
-            'album': self.album,
-            'id': self.id,
-            'title': self.title,
-            })
-        formated = format(**format_info) + '.' + suffix
-        if formated.rfind('/') != -1:
-            formated = formated[:formated.rfind('/') + 1] + clean(formated[formated.rfind('/') + 1:])
-        else:
-            formated = clean(formated)
-        return formated
-
     def song_download(self):
         filename = self.get_formated_filename('mp3')
         file_origin = OriginFile(self.url_info['song_file'])
         if file_origin.total_size <= 0:
             return -1
         file_origin.single_thread_start(filename = filename)
         return filename
@@ -141,38 +147,32 @@
         往文件里面写入歌曲信息
         ----------
         参数: 
         1. `filename`: 文件名，字符串，仅mp3/flac格式
         '''
         filename_ready = self.get_formated_filename('mp3')
         if filename == 'No filename':
-            filename = filename_ready
+            filename = self.filename_info['song']
         attribute_write(filename = filename, info = self.processed_info)
 
-    def cover_write(self, filename = 'No filename', cover_filename = 'No filename'):
+    def cover_write(self, filename = 'No filename', cover_filename = 'No cover_filename'):
         '''
         专辑封面写入
         ----------
         参数: 
         1. `filename`: 文件名，字符串，仅mp3/flac格式
         2. `cover_filename`: 封面的文件名, 字符串, 仅jpg格式
         '''
-
-        filename_ready = self.get_formated_filename('mp3')
         if filename == 'No filename':
-            filename = filename_ready
-
-        cover_filename_ready = self.get_formated_filename('jpg')
+            filename = self.filename_info['song']
         if cover_filename == 'No cover_filename':
-            cover_filename = cover_filename_ready
+            cover_filename = self.filename_info['pic']
         cover_write(filename = filename, cover_filename = cover_filename)
 
-    def lyric_write(self, filename = 'No filename', lyric_filename = 'No filename'):
-        filename_ready = self.get_formated_filename('mp3')
+    def lyric_write(self, filename = 'No filename', lyric_filename = 'No lyric_filename'):
         if filename == 'No filename':
-            filename = filename_ready
-        lyric_filename_ready = self.get_formated_filename('lrc')
+            filename = self.filename_info['song']
         if lyric_filename == 'No lyric_filename':
-            lyric_filename = lyric_filename_ready
+            lyric_filename = self.filename_info['lyric']
         lyric_write(filename = filename, lyric_filename = lyric_filename)
```

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240407b1
+Version: 1.0.0.240408a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.0.240408a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240407b1/setup.py` & `ncmlistdownloader-1.0.0.240408a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        # 'Development Status :: 3 - Alpha',
-        'Development Status :: 4 - Beta',
+        'Development Status :: 3 - Alpha',
+        # 'Development Status :: 4 - Beta',
         # 开发的目标用户
         'Intended Audience :: Customer Service',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         # 属于什么类型
         'Topic :: Communications :: File Sharing',
         'Topic :: Internet',
@@ -25,15 +25,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240407b1",
+    version = "1.0.0.240408a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

