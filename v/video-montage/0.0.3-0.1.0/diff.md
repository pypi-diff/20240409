# Comparing `tmp/video_montage-0.0.3.tar.gz` & `tmp/video_montage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/video_montage-0.0.3.tar", last modified: Fri Oct 20 07:26:49 2023, max compression
+gzip compressed data, was "dist/video_montage-0.1.0.tar", last modified: Tue Apr  9 04:22:19 2024, max compression
```

## Comparing `video_montage-0.0.3.tar` & `video_montage-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-20 07:26:49.000000 video_montage-0.0.3/
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1066 2023-10-08 00:04:31.000000 video_montage-0.0.3/LICENSE
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     4386 2023-10-20 07:26:49.000000 video_montage-0.0.3/PKG-INFO
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     3860 2023-10-20 07:23:49.000000 video_montage-0.0.3/README.md
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       38 2023-10-20 07:26:49.000000 video_montage-0.0.3/setup.cfg
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1102 2023-10-20 07:26:08.000000 video_montage-0.0.3/setup.py
-drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage/
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-08 01:07:02.000000 video_montage-0.0.3/video_montage/__init__.py
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1638 2023-10-20 07:12:26.000000 video_montage-0.0.3/video_montage/utils.py
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     3046 2023-10-20 07:12:26.000000 video_montage-0.0.3/video_montage/video_grid_montage.py
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1601 2023-10-20 07:12:26.000000 video_montage-0.0.3/video_montage/video_sequence_montage.py
-drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     4386 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/PKG-INFO
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      375 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/SOURCES.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)        1 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/dependency_links.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      145 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/entry_points.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       30 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/requires.txt
--rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       14 2023-10-20 07:26:49.000000 video_montage-0.0.3/video_montage.egg-info/top_level.txt
+drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2024-04-09 04:22:19.000000 video_montage-0.1.0/
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1066 2023-10-08 00:04:31.000000 video_montage-0.1.0/LICENSE
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     4386 2024-04-09 04:22:19.000000 video_montage-0.1.0/PKG-INFO
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     3860 2023-10-20 07:23:49.000000 video_montage-0.1.0/README.md
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       38 2024-04-09 04:22:19.000000 video_montage-0.1.0/setup.cfg
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1102 2024-04-09 04:21:41.000000 video_montage-0.1.0/setup.py
+drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage/
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)        0 2023-10-08 01:07:02.000000 video_montage-0.1.0/video_montage/__init__.py
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1715 2024-04-09 04:13:55.000000 video_montage-0.1.0/video_montage/utils.py
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     3285 2024-04-09 04:18:28.000000 video_montage-0.1.0/video_montage/video_grid_montage.py
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     1840 2024-04-09 04:19:29.000000 video_montage-0.1.0/video_montage/video_sequence_montage.py
+drwxrwxr-x   0 tylerlum  (1000) tylerlum  (1000)        0 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)     4386 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/PKG-INFO
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      375 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/SOURCES.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)        1 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/dependency_links.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)      145 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/entry_points.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       30 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/requires.txt
+-rw-rw-r--   0 tylerlum  (1000) tylerlum  (1000)       14 2024-04-09 04:22:19.000000 video_montage-0.1.0/video_montage.egg-info/top_level.txt
```

### Comparing `video_montage-0.0.3/LICENSE` & `video_montage-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video_montage-0.0.3/PKG-INFO` & `video_montage-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video_montage
-Version: 0.0.3
+Version: 0.1.0
 Summary: Easily create a video montage (either a sequence or a grid of videos)
 Home-page: https://github.com/tylerlum/video_montage
 Author: Tyler Lum
 Author-email: tylergwlum@gmail.com
 License: UNKNOWN
 Keywords: python,video,montage,grid,sequence
 Platform: UNKNOWN
```

### Comparing `video_montage-0.0.3/README.md` & `video_montage-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `video_montage-0.0.3/setup.py` & `video_montage-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.0.3"
+VERSION = "0.1.0"
 DESCRIPTION = "Easily create a video montage (either a sequence or a grid of videos)"
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="video_montage",
     version=VERSION,
```

### Comparing `video_montage-0.0.3/video_montage/utils.py` & `video_montage-0.1.0/video_montage/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 def create_video_clips(
     input_video_folders_path: pathlib.Path, max_n_videos: Optional[int] = None
 ) -> List[mp.VideoFileClip]:
     VIDEO_EXTENSIONS = ["*.mp4", "*.webm", "*.avi", "*.mov", "*.mkv", "*.gif"]
 
     video_file_paths = sum(
         [
-            list(input_video_folders_path.glob(video_extension))
+            sorted(
+                list(input_video_folders_path.glob(video_extension)),
+                key=lambda x: x.name,
+            )
             for video_extension in VIDEO_EXTENSIONS
         ],
         [],
     )
 
     max_n_videos = max_n_videos if max_n_videos is not None else len(video_file_paths)
     selected_video_file_paths = video_file_paths[:max_n_videos]
```

### Comparing `video_montage-0.0.3/video_montage/video_grid_montage.py` & `video_montage-0.1.0/video_montage/video_grid_montage.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 import math
 from video_montage.utils import create_video_clips, datetime_str, overlay_text_on_clip
 
 
 class ArgumentParser(Tap):
     input_video_folder_path: pathlib.Path
     output_video_folder_path: pathlib.Path = pathlib.Path(".")
-    output_video_filename: str = f"{datetime_str()}_video_grid_montage.mp4"
+    output_video_filename: Optional[str] = None
     max_n_videos: Optional[int] = None
     max_duration_seconds: Optional[int] = None
     fps: Optional[int] = None
     num_per_row: Optional[int] = None
     overlay_filename: bool = False
 
+    @property
+    def output_video_filepath(self) -> pathlib.Path:
+        if self.output_video_filename is None:
+            filename = f"{self.input_video_folder_path.name}_{datetime_str()}_video_grid_montage.mp4"
+        else:
+            filename = self.output_video_filename
+        return self.output_video_folder_path / filename
+
 
 def trim_video_clips(
     video_clips: List[mp.VideoFileClip], max_duration_seconds: Optional[int] = None
 ) -> List[mp.VideoFileClip]:
     shortest_duration_seconds = min([video_clip.duration for video_clip in video_clips])
     montage_duration_seconds = (
         min(shortest_duration_seconds, max_duration_seconds)
@@ -77,17 +85,16 @@
     ]
     assert len(video_clips) == num_slots, f"{len(video_clips)} != {num_slots}"
 
     video_grid = mp.clips_array(
         [video_clips[i * num_per_row : (i + 1) * num_per_row] for i in range(num_rows)]
     )
 
-    output_filepath = args.output_video_folder_path / args.output_video_filename
     fps = args.fps if args.fps is not None else video_clips[0].fps
     video_grid.write_videofile(
-        str(output_filepath),
+        str(args.output_video_filepath),
         fps=fps,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `video_montage-0.0.3/video_montage/video_sequence_montage.py` & `video_montage-0.1.0/video_montage/video_sequence_montage.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,27 @@
 import pathlib
 from video_montage.utils import create_video_clips, datetime_str, overlay_text_on_clip
 
 
 class ArgumentParser(Tap):
     input_video_folder_path: pathlib.Path
     output_video_folder_path: pathlib.Path = pathlib.Path(".")
-    output_video_filename: str = f"{datetime_str()}_video_sequence_montage.mp4"
+    output_video_filename: Optional[str] = None
     max_n_videos: Optional[int] = None
     fps: Optional[int] = None
     overlay_filename: bool = False
 
+    @property
+    def output_video_filepath(self) -> pathlib.Path:
+        if self.output_video_filename is None:
+            filename = f"{self.input_video_folder_path.name}_{datetime_str()}_video_sequence_montage.mp4"
+        else:
+            filename = self.output_video_filename
+        return self.output_video_folder_path / filename
+
 
 def main() -> None:
     args: ArgumentParser = ArgumentParser().parse_args()
     assert (
         args.input_video_folder_path.exists()
     ), f"Input video folder path {args.input_video_folder_path} does not exist."
 
@@ -34,17 +42,16 @@
                 clip=video_clip, text=pathlib.Path(video_clip.filename).name
             )
             for video_clip in video_clips
         ]
 
     video_sequence = mp.concatenate_videoclips(video_clips, method="compose")
 
-    output_filepath = args.output_video_folder_path / args.output_video_filename
     fps = args.fps if args.fps is not None else video_clips[0].fps
     video_sequence.write_videofile(
-        str(output_filepath),
+        str(args.output_video_filepath),
         fps=fps,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `video_montage-0.0.3/video_montage.egg-info/PKG-INFO` & `video_montage-0.1.0/video_montage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-montage
-Version: 0.0.3
+Version: 0.1.0
 Summary: Easily create a video montage (either a sequence or a grid of videos)
 Home-page: https://github.com/tylerlum/video_montage
 Author: Tyler Lum
 Author-email: tylergwlum@gmail.com
 License: UNKNOWN
 Keywords: python,video,montage,grid,sequence
 Platform: UNKNOWN
```

