# Comparing `tmp/isubrip-2.5.2.tar.gz` & `tmp/isubrip-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isubrip-2.5.2.tar", max compression
+gzip compressed data, was "isubrip-2.5.3.tar", max compression
```

## Comparing `isubrip-2.5.2.tar` & `isubrip-2.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-12-16 12:00:50.413409 isubrip-2.5.2/isubrip/__init__.py
--rw-r--r--   0        0        0    21355 2024-01-06 19:28:37.458817 isubrip-2.5.2/isubrip/__main__.py
--rw-r--r--   0        0        0    13778 2023-12-16 12:00:50.414410 isubrip-2.5.2/isubrip/config.py
--rw-r--r--   0        0        0     1352 2024-01-06 19:28:37.458817 isubrip-2.5.2/isubrip/constants.py
--rw-r--r--   0        0        0     8178 2024-01-06 19:28:37.459820 isubrip-2.5.2/isubrip/data_structures.py
--rw-r--r--   0        0        0     1640 2023-12-16 12:00:50.416610 isubrip-2.5.2/isubrip/logger.py
--rw-r--r--   0        0        0      717 2023-12-16 12:00:50.416610 isubrip-2.5.2/isubrip/resources/default_config.toml
--rw-r--r--   0        0        0        0 2023-05-26 10:40:55.098754 isubrip-2.5.2/isubrip/scrapers/__init__.py
--rw-r--r--   0        0        0    16175 2024-01-06 19:28:37.460819 isubrip-2.5.2/isubrip/scrapers/appletv_scraper.py
--rw-r--r--   0        0        0     5723 2024-01-06 19:28:37.461821 isubrip-2.5.2/isubrip/scrapers/itunes_scraper.py
--rw-r--r--   0        0        0    21282 2024-01-06 19:28:37.461821 isubrip-2.5.2/isubrip/scrapers/scraper.py
--rw-r--r--   0        0        0        0 2023-05-24 22:34:46.568839 isubrip-2.5.2/isubrip/subtitle_formats/__init__.py
--rw-r--r--   0        0        0     1459 2023-12-16 12:00:50.419608 isubrip-2.5.2/isubrip/subtitle_formats/subrip.py
--rw-r--r--   0        0        0     7819 2023-12-16 12:00:50.419608 isubrip-2.5.2/isubrip/subtitle_formats/subtitles.py
--rw-r--r--   0        0        0    10165 2023-12-16 12:00:50.420609 isubrip-2.5.2/isubrip/subtitle_formats/webvtt.py
--rw-r--r--   0        0        0    16846 2024-01-06 19:28:37.463327 isubrip-2.5.2/isubrip/utils.py
--rw-r--r--   0        0        0     1093 2022-01-28 09:13:22.249000 isubrip-2.5.2/LICENSE
--rw-r--r--   0        0        0     2768 2024-01-06 19:28:37.463327 isubrip-2.5.2/pyproject.toml
--rw-r--r--   0        0        0     2913 2024-01-06 19:28:37.457819 isubrip-2.5.2/README.md
--rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 isubrip-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-16 16:42:50.118731 isubrip-2.5.3/isubrip/__init__.py
+-rw-r--r--   0        0        0    22220 2024-04-09 20:06:17.681572 isubrip-2.5.3/isubrip/__main__.py
+-rw-r--r--   0        0        0    14124 2024-04-09 20:06:17.681572 isubrip-2.5.3/isubrip/config.py
+-rw-r--r--   0        0        0     1858 2024-04-09 20:06:17.683080 isubrip-2.5.3/isubrip/constants.py
+-rw-r--r--   0        0        0     8355 2024-04-09 20:06:17.683080 isubrip-2.5.3/isubrip/data_structures.py
+-rw-r--r--   0        0        0     1640 2024-03-16 16:42:50.121730 isubrip-2.5.3/isubrip/logger.py
+-rw-r--r--   0        0        0      574 2024-04-09 20:06:17.684089 isubrip-2.5.3/isubrip/resources/default_config.toml
+-rw-r--r--   0        0        0        0 2023-05-26 10:40:55.098754 isubrip-2.5.3/isubrip/scrapers/__init__.py
+-rw-r--r--   0        0        0    16052 2024-04-09 20:06:17.685090 isubrip-2.5.3/isubrip/scrapers/appletv_scraper.py
+-rw-r--r--   0        0        0     6514 2024-04-09 20:06:17.685090 isubrip-2.5.3/isubrip/scrapers/itunes_scraper.py
+-rw-r--r--   0        0        0    25550 2024-04-09 20:06:17.686091 isubrip-2.5.3/isubrip/scrapers/scraper.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:34:46.568839 isubrip-2.5.3/isubrip/subtitle_formats/__init__.py
+-rw-r--r--   0        0        0     1406 2024-04-09 20:06:17.687091 isubrip-2.5.3/isubrip/subtitle_formats/subrip.py
+-rw-r--r--   0        0        0    10934 2024-04-09 20:06:17.687091 isubrip-2.5.3/isubrip/subtitle_formats/subtitles.py
+-rw-r--r--   0        0        0    10564 2024-04-09 20:06:17.688088 isubrip-2.5.3/isubrip/subtitle_formats/webvtt.py
+-rw-r--r--   0        0        0    19715 2024-04-09 20:06:17.688088 isubrip-2.5.3/isubrip/utils.py
+-rw-r--r--   0        0        0     1093 2022-01-28 09:13:22.249000 isubrip-2.5.3/LICENSE
+-rw-r--r--   0        0        0     2999 2024-04-09 20:06:17.690088 isubrip-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2899 2024-04-09 20:06:17.680573 isubrip-2.5.3/README.md
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 isubrip-2.5.3/PKG-INFO
```

### Comparing `isubrip-2.5.2/isubrip/__main__.py` & `isubrip-2.5.3/isubrip/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import atexit
 import logging
 from pathlib import Path
 import shutil
 import sys
 from typing import List
 
 import requests
@@ -21,131 +20,145 @@
     PACKAGE_VERSION,
     PREORDER_MESSAGE,
     TEMP_FOLDER_PATH,
     USER_CONFIG_FILE,
 )
 from isubrip.data_structures import (
     Episode,
-    MediaBase,
     MediaData,
     Movie,
     ScrapedMediaResponse,
     Season,
     Series,
     SubtitlesData,
     SubtitlesDownloadResults,
 )
 from isubrip.logger import CustomLogFileFormatter, CustomStdoutFormatter, logger
 from isubrip.scrapers.scraper import PlaylistLoadError, Scraper, ScraperError, ScraperFactory
 from isubrip.subtitle_formats.webvtt import Caption as WebVTTCaption
 from isubrip.utils import (
+    TempDirGenerator,
     download_subtitles_to_file,
-    generate_media_description,
+    format_media_description,
+    format_release_name,
+    format_subtitles_description,
     generate_non_conflicting_path,
-    generate_release_name,
     raise_for_status,
     single_to_list,
 )
 
 LOG_ROTATION_SIZE: int | None = None
 
 BASE_CONFIG_SETTINGS = [
     ConfigSetting(
         key="check-for-updates",
-        type=bool,
+        value_type=bool,
         category="general",
         required=False,
     ),
     ConfigSetting(
         key="log_rotation_size",
-        type=str,
+        value_type=str,
         category="general",
         required=False,
     ),
     ConfigSetting(
         key="add-release-year-to-series",
-        type=bool,
+        value_type=bool,
         category="downloads",
         required=False,
     ),
     ConfigSetting(
         key="folder",
-        type=str,
+        value_type=str,
         category="downloads",
         required=True,
         special_type=SpecialConfigType.EXISTING_FOLDER_PATH,
     ),
     ConfigSetting(
         key="languages",
-        type=List[str],
+        value_type=List[str],
         category="downloads",
         required=False,
     ),
     ConfigSetting(
         key="overwrite-existing",
-        type=bool,
+        value_type=bool,
         category="downloads",
         required=True,
     ),
     ConfigSetting(
         key="zip",
-        type=bool,
+        value_type=bool,
         category="downloads",
         required=False,
     ),
     ConfigSetting(
         key="fix-rtl",
-        type=bool,
+        value_type=bool,
         category="subtitles",
         required=True,
     ),
     ConfigSetting(
         key="rtl-languages",
-        type=List[str],
+        value_type=List[str],
         category="subtitles",
         required=False,
     ),
     ConfigSetting(
         key="remove-duplicates",
-        type=bool,
+        value_type=bool,
         category="subtitles",
         required=True,
     ),
     ConfigSetting(
         key="convert-to-srt",
-        type=bool,
+        value_type=bool,
         category="subtitles",
         required=False,
     ),
     ConfigSetting(
         key="subrip-alignment-conversion",
-        type=bool,
+        value_type=bool,
         category=("subtitles", "webvtt"),
         required=False,
     ),
     ConfigSetting(
         key="user-agent",
-        type=str,
+        value_type=str,
         category="scrapers",
         required=True,
     ),
+    ConfigSetting(
+        key="proxy",
+        value_type=str,
+        category="scrapers",
+        required=False,
+    ),
+    ConfigSetting(
+        key="verify-ssl",
+        value_type=bool,
+        category="scrapers",
+        required=False,
+    ),
 ]
 
 
 def main() -> None:
     try:
         # Assure at least one argument was passed
         if len(sys.argv) < 2:
             print_usage()
             exit(0)
 
-        create_required_folders()
         setup_loggers(stdout_loglevel=logging.INFO,
                       file_loglevel=logging.DEBUG)
 
+        generate_project_folders()
+
         cli_args = " ".join(sys.argv[1:])
         logger.debug(f"Used CLI Command: {PACKAGE_NAME} {cli_args}")
         logger.debug(f"Python version: {sys.version}")
         logger.debug(f"Package version: {PACKAGE_VERSION}")
         logger.debug(f"OS: {sys.platform}")
 
         config = generate_config()
@@ -162,66 +175,67 @@
         logger.debug(f"Stack trace: {ex}", exc_info=True)
         exit(1)
 
     finally:
         if log_rotation_size := LOG_ROTATION_SIZE:
             handle_log_rotation(log_rotation_size=log_rotation_size)
 
-        scraper_factory = ScraperFactory()
-
         # NOTE: This will only close scrapers that were initialized using the ScraperFactory.
-        for scraper in scraper_factory.get_initialized_scrapers():
+        for scraper in ScraperFactory.get_initialized_scrapers():
             scraper.close()
 
+        TempDirGenerator.cleanup()
+
 
 def download(urls: list[str], config: Config) -> None:
     """
     Download subtitles from a given URL.
 
     Args:
         urls (list[str]): A list of URLs to download subtitles from.
         config (Config): A config to use for downloading subtitles.
     """
-    scraper_factory = ScraperFactory()
-
     for url in urls:
         try:
             logger.info(f"Scraping '{url}'...")
 
-            scraper = scraper_factory.get_scraper_instance(url=url, config_data=config.data.get("scrapers"))
-            atexit.register(scraper.close)
+            scraper = ScraperFactory.get_scraper_instance(url=url,
+                                                          kwargs={"config_data": config.data.get("scrapers")},
+                                                          extract_scraper_config=True)
             scraper.config.check()  # Recheck config after scraper settings were loaded
 
             try:
+                logger.debug(f"Fetching '{url}'...")
                 scraper_response: ScrapedMediaResponse = scraper.get_data(url=url)
 
             except ScraperError as e:
                 logger.error(f"Error: {e}")
                 logger.debug("Debug information:", exc_info=True)
                 continue
 
-            media_data: List[MediaBase] = single_to_list(scraper_response.media_data)
-            playlist_scraper = scraper_factory.get_scraper_instance(scraper_id=scraper_response.playlist_scraper,
-                                                                    config_data=config.data.get("scrapers"))
+            media_data = scraper_response.media_data
+            playlist_scraper = ScraperFactory.get_scraper_instance(scraper_id=scraper_response.playlist_scraper,
+                                                                   kwargs={"config_data": config.data.get("scrapers")},
+                                                                   extract_scraper_config=True)
 
             if not media_data:
                 logger.error(f"Error: No supported media was found for {url}.")
                 continue
 
             for media_item in media_data:
                 try:
                     object_type_str = media_item.__class__.__name__.lower()
 
-                    logger.info(f"Found {object_type_str}: {generate_media_description(media_data=media_item)}")
+                    logger.info(f"Found {object_type_str}: {format_media_description(media_data=media_item)}")
                     download_media(scraper=playlist_scraper, media_item=media_item, config=config)
 
                 except Exception as e:
                     if len(media_data) > 1:
                         logger.warning(f"Error scraping media item "
-                                       f"'{generate_media_description(media_data=media_item)}': {e}\n"
+                                       f"'{format_media_description(media_data=media_item)}': {e}\n"
                                        f"Skipping to next media item...")
                         logger.debug("Debug information:", exc_info=True)
                         continue
 
                     raise
 
         except Exception as e:
@@ -238,22 +252,25 @@
         scraper (Scraper): A Scraper object to use for downloading subtitles.
         media_item (MediaData): A media data item to download subtitles for.
         config (Config): A config to use for downloading subtitles.
     """
     if isinstance(media_item, Series):
         for season in media_item.seasons:
             download_media(scraper=scraper, media_item=season, config=config)
-            return
 
-    if isinstance(media_item, Season):
+    elif isinstance(media_item, Season):
         for episode in media_item.episodes:
-            logger.info(f"{generate_media_description(media_data=episode)}:")
-            download_media(scraper=scraper, media_item=episode, config=config)
-            return
+            logger.info(f"{format_media_description(media_data=episode, shortened=True)}:")
+            download_media_item(scraper=scraper, media_item=episode, config=config)
+
+    elif isinstance(media_item, (Movie, Episode)):
+        download_media_item(scraper=scraper, media_item=media_item, config=config)
+
 
+def download_media_item(scraper: Scraper, media_item: Movie | Episode, config: Config) -> None:
     if media_item.playlist:
         download_subtitles_kwargs = {
             "download_path": Path(config.downloads["folder"]),
             "language_filter": config.downloads.get("languages"),
             "convert_to_srt": config.subtitles.get("convert-to-srt", False),
             "overwrite_existing": config.downloads.get("overwrite-existing", False),
             "zip_files": config.downloads.get("zip", False),
@@ -322,20 +339,20 @@
 
     except Exception as e:
         logger.warning(f"Update check failed: {e}")
         logger.debug(f"Stack trace: {e}", exc_info=True)
         return
 
 
-def create_required_folders() -> None:
+def generate_project_folders() -> None:
     if not DATA_FOLDER_PATH.is_dir():
         logger.debug(f"'{DATA_FOLDER_PATH}' directory could not be found and will be created.")
         LOG_FILES_PATH.mkdir(parents=True, exist_ok=True)
 
-    else:
+    else:  # LOG_FILES_PATH is inside DATA_FOLDER_PATH
         if not LOG_FILES_PATH.is_dir():
             logger.debug(f"'{LOG_FILES_PATH}' directory could not be found and will be created.")
             LOG_FILES_PATH.mkdir()
 
 
 def download_subtitles(scraper: Scraper, media_data: Movie | Episode, download_path: Path,
                        language_filter: list[str] | None = None, convert_to_srt: bool = False,
@@ -353,56 +370,54 @@
         overwrite_existing (bool, optional): Whether to overwrite existing subtitles. Defaults to True.
         zip_files (bool, optional): Whether to unite the subtitles into a single zip file
             (only if there are multiple subtitles).
 
     Returns:
         SubtitlesDownloadResults: A SubtitlesDownloadResults object containing the results of the download.
     """
-    temp_download_path = generate_media_path(base_path=TEMP_FOLDER_PATH,
-                                             media_data=media_data,
-                                             source=scraper.abbreviation)
-    atexit.register(shutil.rmtree, TEMP_FOLDER_PATH, ignore_errors=False, onerror=None)
+    temp_dir_name = generate_media_folder_name(media_data=media_data, source=scraper.abbreviation)
+    temp_download_path = TempDirGenerator.generate(directory_name=temp_dir_name)
 
     successful_downloads: list[SubtitlesData] = []
     failed_downloads: list[SubtitlesData] = []
     temp_downloads: list[Path] = []
 
     for subtitles_data in scraper.get_subtitles(main_playlist=media_data.playlist,  # type: ignore[arg-type]
                                                 language_filter=language_filter,
                                                 subrip_conversion=convert_to_srt):
-        language_data = f"{subtitles_data.language_name} ({subtitles_data.language_code})"
 
-        if subtitles_type := subtitles_data.special_type:
-            language_data += f" [{subtitles_type.value}]"
+        language_info = format_subtitles_description(language_code=subtitles_data.language_code,
+                                                     language_name=subtitles_data.language_name,
+                                                     special_type=subtitles_data.special_type)
 
         try:
             temp_downloads.append(download_subtitles_to_file(
                 media_data=media_data,
                 subtitles_data=subtitles_data,
                 output_path=temp_download_path,
                 source_abbreviation=scraper.abbreviation,
                 overwrite=overwrite_existing,
             ))
 
-            logger.info(f"{language_data} subtitles were successfully downloaded.")
+            logger.info(f"{language_info} subtitles were successfully downloaded.")
             successful_downloads.append(subtitles_data)
 
         except Exception as e:
-            logger.error(f"Error: Failed to download '{language_data}' subtitles: {e}")
+            logger.error(f"Error: Failed to download '{language_info}' subtitles: {e}")
             logger.debug("Stack trace:", exc_info=True)
             failed_downloads.append(subtitles_data)
             continue
 
     if not zip_files or len(temp_downloads) == 1:
         for file_path in temp_downloads:
             if overwrite_existing:
                 new_path = download_path / file_path.name
 
             else:
-                new_path = generate_non_conflicting_path(download_path / file_path.name)
+                new_path = generate_non_conflicting_path(file_path=download_path / file_path.name)
 
             # str conversion needed only for Python <= 3.8 - https://github.com/python/cpython/issues/76870
             shutil.move(src=str(file_path), dst=new_path)
 
     elif len(temp_downloads) > 0:
         archive_path = Path(shutil.make_archive(
             base_name=str(temp_download_path.parent / temp_download_path.name),
@@ -413,23 +428,20 @@
         file_name = generate_media_folder_name(media_data=media_data,
                                                source=scraper.abbreviation) + f".{ARCHIVE_FORMAT}"
 
         if overwrite_existing:
             destination_path = download_path / file_name
 
         else:
-            destination_path = generate_non_conflicting_path(download_path / file_name)
+            destination_path = generate_non_conflicting_path(file_path=download_path / file_name)
 
         shutil.move(src=str(archive_path), dst=destination_path)
 
-    shutil.rmtree(temp_download_path)
-    atexit.unregister(shutil.rmtree)
-
     return SubtitlesDownloadResults(
-        movie_data=media_data,
+        media_data=media_data,
         successful_subtitles=successful_downloads,
         failed_subtitles=failed_downloads,
         is_zip=zip_files,
     )
 
 
 def handle_log_rotation(log_rotation_size: int) -> None:
@@ -501,58 +513,62 @@
         media_data (Movie | Episode): A movie or episode data object.
         source (str | None, optional): Abbreviation of the source to use for file names. Defaults to None.
 
     Returns:
         str: A folder name for the media data.
     """
     if isinstance(media_data, Movie):
-        return generate_release_name(
+        return format_release_name(
             title=media_data.name,
             release_date=media_data.release_date,
             media_source=source,
         )
 
     # elif isinstance(media_data, Episode):
-    return generate_release_name(
+    return format_release_name(
         title=media_data.series_name,
         season_number=media_data.season_number,
         media_source=source,
     )
 
 
-def generate_media_path(base_path: Path, media_data: Movie | Episode, source: str | None = None) -> Path:
+def generate_temp_media_path(media_data: Movie | Episode, source: str | None = None) -> Path:
     """
-    Generate a temporary folder for downloading media data.
+    Generate a temporary directory for downloading media data.
 
     Args:
-        base_path (Path): A base path to generate the folder in.
         media_data (Movie | Episode): A movie or episode data object.
         source (str | None, optional): Abbreviation of the source to use for file names. Defaults to None.
 
     Returns:
         Path: A path to the temporary folder.
     """
     temp_folder_name = generate_media_folder_name(media_data=media_data, source=source)
-    path = generate_non_conflicting_path(base_path / temp_folder_name, has_extension=False)
-    path.mkdir(parents=True, exist_ok=True)
+    path = generate_non_conflicting_path(file_path=TEMP_FOLDER_PATH / temp_folder_name, has_extension=False)
 
-    return path
+    return TempDirGenerator.generate(directory_name=path.name)
 
 
 def update_settings(config: Config) -> None:
     """
     Update settings according to config.
 
     Args:
         config (Config): An instance of a config to set settings according to.
     """
     Scraper.subtitles_fix_rtl = config.subtitles["fix-rtl"]
-    Scraper.subtitles_fix_rtl_languages = config.subtitles.get("rtl-languages")
     Scraper.subtitles_remove_duplicates = config.subtitles["remove-duplicates"]
     Scraper.default_user_agent = config.scrapers.get("user-agent", default_user_agent())
+    Scraper.default_proxy = config.scrapers.get("proxy")
+    Scraper.default_verify_ssl = config.scrapers.get("verify-ssl", True)
+
+    if not Scraper.default_verify_ssl:
+        import urllib3
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
     WebVTTCaption.subrip_alignment_conversion = (
         config.subtitles.get("webvtt", {}).get("subrip-alignment-conversion", False)
     )
 
     if log_rotation := config.general.get("log-rotation-size"):
         global LOG_ROTATION_SIZE
         LOG_ROTATION_SIZE = log_rotation
@@ -576,15 +592,15 @@
     # Setup STDOUT logger
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setLevel(stdout_loglevel)
     stdout_handler.setFormatter(CustomStdoutFormatter())
     logger.addHandler(stdout_handler)
 
     # Setup logfile logger
-    logfile_path = generate_non_conflicting_path(LOG_FILES_PATH / LOG_FILE_NAME)
+    logfile_path = generate_non_conflicting_path(file_path=LOG_FILES_PATH / LOG_FILE_NAME)
     logfile_handler = logging.FileHandler(filename=logfile_path, encoding="utf-8")
     logfile_handler.setLevel(file_loglevel)
     logfile_handler.setFormatter(CustomLogFileFormatter())
     logger.addHandler(logfile_handler)
 
 
 if __name__ == "__main__":
```

### Comparing `isubrip-2.5.2/isubrip/config.py` & `isubrip-2.5.3/isubrip/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 
 class ConfigSetting(NamedTuple):
     """
     A NamedTuple representing a config setting.
 
     Attributes:
         key (str): Dictionary key used to access the setting.
-        type (type): Variable type of the value of the setting. Used for validation.
+        value_type (type): Variable type of the value of the setting. Used for validation.
         category (str | tuple[str, ...], optional): A category that the setting is under.
             Categories are used to group related settings' keys together in a sub-dictionary.
             A tuple can be used to nest categories (first item is the top-level category). Defaults to None.
         required (bool, optional): Whether the setting is required. Defaults to False.
         enum_type (type[Enum], optional): An Enum that the settings values will be converted to. Defaults to None.
         special_type (SpecialConfigType | list[SpecialConfigType], optional): A special property of the setting's value
             to validate, represented by a SpecialConfigType value. Defaults to None.
     """
     key: str
     # TODO: Use `types.UnionType` instead of `typing._UnionGenericAlias`, once minimum Python version >= 3.10.
     # TODO: Update 'InvalidConfigType' exception as well.
-    type: type | typing._UnionGenericAlias  # type: ignore[name-defined]  # noqa: SLF001
+    value_type: type | typing._UnionGenericAlias  # type: ignore[name-defined]
     category: str | tuple[str, ...] | None = None
     required: bool = False
     enum_type: Type[Enum] | None = None
     special_type: SpecialConfigType | list[SpecialConfigType] | None = None
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, ConfigSetting):
@@ -84,28 +84,40 @@
 
         if config_settings:
             self.add_settings(config_settings, check_config=False)
 
         if config_data:
             self._config_data = deepcopy(config_data)
 
+    def __contains__(self, item: Any) -> bool:
+        """
+        Allow checking if a key exists in the config using the 'in' operator.
+
+        Args:
+            item (Any): The key to check for.
+
+        Returns:
+            bool: True if the key exists in the config, False otherwise.
+        """
+        return item in self._config_data
+
     def __getattr__(self, key: str) -> Any:
         """
         Allow access to config settings using attributes.
 
         Args:
             key (str): Config key to get.
 
         Returns:
             Any: The corresponding value for the key in the config.
         """
         if self._config_data and key in self._config_data:
             return self._config_data[key]
 
-        raise AttributeError(f"Attribute \'{key}\' does not exist.")
+        raise AttributeError(f"Attribute '{key}' does not exist.")
 
     def __getitem__(self, key: str) -> Any:
         """
         Allow access to config settings using dict-like syntax.
 
         Args:
             key (str): Config key to get.
@@ -273,16 +285,16 @@
 
             if value is None:
                 if setting.required:
                     raise MissingRequiredConfigSettingError(setting_path=setting_path)
 
                 continue
 
-            if setting.enum_type is None and not check_type(value, setting.type):
-                raise InvalidConfigTypeError(setting_path=setting_path, value=value, expected_type=setting.type)
+            if setting.enum_type is None and not check_type(value, setting.value_type):
+                raise InvalidConfigTypeError(setting_path=setting_path, value=value, expected_type=setting.value_type)
 
             special_types = single_to_list(setting.special_type)
 
             if SpecialConfigType.EXISTING_FILE_PATH in special_types and not Path(value).is_file():
                 raise InvalidConfigFilePathError(setting_path=setting_path, value=value)
 
             if SpecialConfigType.EXISTING_FOLDER_PATH in special_types and not Path(value).is_dir():
@@ -321,15 +333,15 @@
             additional_note=f"Value can only be one of: {enum_options}.",
         )
 
 
 class InvalidConfigTypeError(InvalidConfigValueError):
     """An invalid config value type has been set."""
     def __init__(self, setting_path: str,
-                 expected_type: type | typing._UnionGenericAlias,  # type: ignore[name-defined] # noqa: SLF001
+                 expected_type: type | typing._UnionGenericAlias,  # type: ignore[name-defined]
                  value: Any):
         expected_type_str = expected_type.__name__ if hasattr(expected_type, '__name__') else str(expected_type)
         value_type_str = type(value).__name__ if hasattr(type(value), '__name__') else str(type(value))
 
         super().__init__(
             setting_path=setting_path,
             value=value,
```

### Comparing `isubrip-2.5.2/isubrip/constants.py` & `isubrip-2.5.3/isubrip/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import logging
 from pathlib import Path
 from tempfile import gettempdir
 
 # General
 PACKAGE_NAME = "isubrip"
-PACKAGE_VERSION = "2.5.2"
+PACKAGE_VERSION = "2.5.3"
 
 # Logging
 PREORDER_MESSAGE = ("'{movie_name}' is currently unavailable on {scraper_name}, "
                     "and will be available on {preorder_date}.")
 
 ANSI_COLORS = {
     logging.DEBUG: "\x1b[37;20m",  # Light Grey
@@ -37,7 +37,15 @@
 # Config Paths
 USER_CONFIG_FILE_NAME = "config.toml"
 USER_CONFIG_FILE = DATA_FOLDER_PATH / USER_CONFIG_FILE_NAME
 
 # Logging Paths
 LOG_FILES_PATH = DATA_FOLDER_PATH / "logs"
 LOG_FILE_NAME = f"{PACKAGE_NAME}_{dt.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.log"
+
+# Other
+TITLE_REPLACEMENT_STRINGS = {  # Replacements will be done by the order of the keys.
+    ": ": ".", ":": ".", " - ": "-", ", ": ".", ". ": ".", " ": ".", "|": ".", "/": ".", "…": ".",
+    "<": "", ">": "", "(": "", ")": "", '"': "", "?": "", "*": "",
+}
+WINDOWS_RESERVED_FILE_NAMES = ("CON", "PRN", "AUX", "NUL", "COM1", "COM2", "COM3", "COM4", "COM5", "COM6", "COM7",
+                               "COM8", "COM9", "LPT1", "LPT2", "LPT3", "LPT4", "LPT5", "LPT6", "LPT7", "LPT8", "LPT9")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `isubrip-2.5.2/isubrip/data_structures.py` & `isubrip-2.5.3/isubrip/data_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 
 class SubtitlesDownloadResults(NamedTuple):
     """
     A named tuple containing download results.
 
     Attributes:
-        movie_data (Movie): Movie data object.
+        media_data (Movie | Episode): An object containing metadata about the media the subtitles were downloaded for.
         successful_subtitles (list[SubtitlesData]): List of subtitles that were successfully downloaded.
         failed_subtitles (list[SubtitlesData]): List of subtitles that failed to download.
         is_zip (bool): Whether the subtitles were saved in a zip file.
     """
-    movie_data: Movie
+    media_data: Movie | Episode
     successful_subtitles: list[SubtitlesData]
     failed_subtitles: list[SubtitlesData]
     is_zip: bool
 
 
 class SubtitlesFormat(BaseModel):
     """
@@ -66,23 +66,25 @@
 
 class SubtitlesData(BaseModel):
     """
     An object containing subtitles data and metadata.
 
     Attributes:
         language_code (str): Language code of the language the subtitles are in.
-        language_name (str): Name of the language the subtitles are in.
+        language_name (str | None, optional): Name of the language the subtitles are in.
         subtitles_format (SubtitlesFormatType): Format of the subtitles.
         content (bytes): Content of the subtitles in binary format.
-        special_type (SubtitlesType | None): Type of the subtitles, if they're not regular. Defaults to None.
+        content_encoding (str): Encoding of subtitles content (ex. "utf-8").
+        special_type (SubtitlesType | None, optional): Type of the subtitles, if they're not regular. Defaults to None.
     """
     language_code: str
-    language_name: str
     subtitles_format: SubtitlesFormatType
     content: bytes
+    content_encoding: str
+    language_name: Optional[str] = None
     special_type: Union[SubtitlesType, None] = None
 
     class ConfigDict:
         str_strip_whitespace = True
 
 
 class MediaBase(BaseModel, ABC):
@@ -191,17 +193,17 @@
 
 
 class ScrapedMediaResponse(BaseModel, Generic[MediaData]):
     """
     An object containing scraped media data and metadata.
 
     Attributes:
-        media_data (Movie | list[Movie] | Episode | list[Episode] | Season | list[Season] | Series | list[Series]):
+        media_data (list[Movie] | list[Episode] | list[Season] | list[Series]):
             An object containing the scraped media data.
         metadata_scraper (str): ID of the scraper that was used to scrape metadata.
         playlist_scraper (str): ID of the scraper that should be used to parse and scrape the playlist.
         original_data (dict): Original raw data from the API that was used to extract media's data.
     """
-    media_data: Union[MediaData, List[MediaData]]
+    media_data: List[MediaData]
     metadata_scraper: str
     playlist_scraper: str
     original_data: dict
```

### Comparing `isubrip-2.5.2/isubrip/logger.py` & `isubrip-2.5.3/isubrip/logger.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.2/isubrip/scrapers/appletv_scraper.py` & `isubrip-2.5.3/isubrip/scrapers/appletv_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,41 +4,33 @@
 from enum import Enum
 import fnmatch
 import re
 from typing import Iterator
 
 from requests.exceptions import HTTPError
 
-from isubrip.data_structures import Episode, MediaData, Movie, ScrapedMediaResponse, Season, Series, SubtitlesData
+from isubrip.data_structures import Episode, Movie, ScrapedMediaResponse, Season, Series, SubtitlesData
 from isubrip.logger import logger
 from isubrip.scrapers.scraper import HLSScraper, ScraperError
 from isubrip.subtitle_formats.webvtt import WebVTTSubtitles
 from isubrip.utils import convert_epoch_to_datetime, parse_url_params, raise_for_status
 
 
 class AppleTVScraper(HLSScraper):
     """An Apple TV scraper."""
     id = "appletv"
     name = "Apple TV"
     abbreviation = "ATV"
-    url_regex = re.compile(r"(?P<base_url>https?://tv\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|episode|season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>umc\.cmc\.[a-z\d]{23,25}))(?:\?(?P<url_params>.*))?", flags=re.IGNORECASE)  # noqa: E501
+    url_regex = re.compile(r"(?i)(?P<base_url>https?://tv\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|episode|season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>umc\.cmc\.[a-z\d]{23,25}))(?:\?(?P<url_params>.*))?")
     subtitles_class = WebVTTSubtitles
     is_movie_scraper = True
     is_series_scraper = True
     uses_scrapers = ["itunes"]
-
-    _api_base_url = "https://tv.apple.com/api/uts/v3"
-    _api_base_params = {
-        "utscf": "OjAAAAAAAAA~",
-        "caller": "js",
-        "v": "66",
-        "pfm": "web",
-    }
-    _default_storefront = "US"  # Has to be uppercase
-    _storefronts_mapping = {
+    default_storefront = "US"
+    storefronts_mapping = {
         "AF": "143610", "AO": "143564", "AI": "143538", "AL": "143575", "AD": "143611", "AE": "143481", "AR": "143505",
         "AM": "143524", "AG": "143540", "AU": "143460", "AT": "143445", "AZ": "143568", "BE": "143446", "BJ": "143576",
         "BF": "143578", "BD": "143490", "BG": "143526", "BH": "143559", "BS": "143539", "BA": "143612", "BY": "143565",
         "BZ": "143555", "BM": "143542", "BO": "143556", "BR": "143503", "BB": "143541", "BN": "143560", "BT": "143577",
         "BW": "143525", "CF": "143623", "CA": "143455", "CH": "143459", "CL": "143483", "CN": "143465", "CI": "143527",
         "CM": "143574", "CD": "143613", "CG": "143582", "CO": "143501", "CV": "143580", "CR": "143495", "KY": "143544",
         "CY": "143557", "CZ": "143489", "DE": "143443", "DM": "143545", "DK": "143458", "DO": "143508", "DZ": "143563",
@@ -60,31 +52,38 @@
         "SE": "143456", "SZ": "143602", "SC": "143599", "TC": "143552", "TD": "143581", "TH": "143475", "TJ": "143603",
         "TM": "143604", "TO": "143608", "TT": "143551", "TN": "143536", "TR": "143480", "TW": "143470", "TZ": "143572",
         "UG": "143537", "UA": "143492", "UY": "143514", "US": "143441", "UZ": "143566", "VC": "143550", "VE": "143502",
         "VG": "143543", "VN": "143471", "VU": "143609", "WS": "143607", "XK": "143624", "YE": "143571", "ZA": "143472",
         "ZM": "143622", "ZW": "143605",
     }
 
+    _api_base_url = "https://tv.apple.com/api/uts/v3"
+    _api_base_params = {
+        "utscf": "OjAAAAAAAAA~",
+        "caller": "js",
+        "v": "66",
+        "pfm": "web",
+    }
+
     class Channel(Enum):
         """
         An Enum representing AppleTV channels.
         Value represents the channel ID as used by the API.
         """
         APPLE_TV_PLUS = "tvs.sbd.4000"
         DISNEY_PLUS = "tvs.sbd.1000216"
         ITUNES = "tvs.sbd.9001"
         HULU = "tvs.sbd.10000"
         MAX = "tvs.sbd.9050"
         NETFLIX = "tvs.sbd.9000"
         PRIME_VIDEO = "tvs.sbd.12962"
         STARZ = "tvs.sbd.1000308"
 
-    def __init__(self, config_data: dict | None = None):
-        super().__init__(config_data=config_data)
-        self._config_data = config_data
+    def __init__(self, user_agent: str | None = None, config_data: dict | None = None):
+        super().__init__(user_agent=user_agent, config_data=config_data)
         self._storefront_locale_mapping_cache: dict[str, str] = {}
 
     def _decide_locale(self, preferred_locales: str | list[str], default_locale: str, locales: list[str]) -> str:
         """
         Decide which locale to use.
 
         Args:
@@ -252,17 +251,14 @@
 
         for playable_data in mapped_playables[self.Channel.ITUNES.value]:
             return_data.append(self._extract_itunes_movie_data(playable_data))
 
         if len(return_data) > 1:
             logger.debug(f"{len(return_data)} iTunes playables were found for movie '{movie_id}'.")
 
-        else:
-            return_data = return_data[0]
-
         return ScrapedMediaResponse(
             media_data=return_data,
             metadata_scraper=self.id,
             playlist_scraper="itunes",
             original_data=data,
         )
 
@@ -310,32 +306,32 @@
 
     def get_season_data(self, storefront_id: str, season_id: str, show_id: str) -> ScrapedMediaResponse[Season]:
         raise NotImplementedError("Series scraping is not currently supported.")
 
     def get_show_data(self, storefront_id: str, show_id: str) -> ScrapedMediaResponse[Series]:
         raise NotImplementedError("Series scraping is not currently supported.")
 
-    def get_data(self, url: str) -> ScrapedMediaResponse[MediaData]:
-        regex_match = self.match_url(url, raise_error=True)
+    def get_data(self, url: str) -> ScrapedMediaResponse:
+        regex_match = self.match_url(url=url, raise_error=True)
         url_data = regex_match.groupdict()
 
         media_type = url_data["media_type"]
 
         if storefront_code := url_data.get("country_code"):
             storefront_code = storefront_code.upper()
 
         else:
-            storefront_code = self._default_storefront
+            storefront_code = self.default_storefront
 
         media_id = url_data["media_id"]
 
-        if storefront_code not in self._storefronts_mapping:
+        if storefront_code not in self.storefronts_mapping:
             raise ScraperError(f"ID mapping for storefront '{storefront_code}' could not be found.")
 
-        storefront_id = self._storefronts_mapping[storefront_code]
+        storefront_id = self.storefronts_mapping[storefront_code]
 
         if media_type == "movie":
             return self.get_movie_data(storefront_id=storefront_id, movie_id=media_id)
 
         if media_type == "episode":
             return self.get_episode_data(storefront_id=storefront_id, episode_id=media_id)
```

### Comparing `isubrip-2.5.2/isubrip/scrapers/itunes_scraper.py` & `isubrip-2.5.3/isubrip/scrapers/itunes_scraper.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,35 +6,43 @@
 import m3u8
 from requests.exceptions import HTTPError
 
 from isubrip.data_structures import SubtitlesData, SubtitlesFormatType
 from isubrip.logger import logger
 from isubrip.scrapers.scraper import HLSScraper, PlaylistLoadError, ScraperError, ScraperFactory
 from isubrip.subtitle_formats.webvtt import WebVTTSubtitles
-from isubrip.utils import raise_for_status
+from isubrip.utils import merge_dict_values, raise_for_status
 
 if TYPE_CHECKING:
     from isubrip.data_structures import Movie, ScrapedMediaResponse
 
 
 class ItunesScraper(HLSScraper):
     """An iTunes movie data scraper."""
     id = "itunes"
     name = "iTunes"
     abbreviation = "iT"
-    url_regex = re.compile(r"(?P<base_url>https?://itunes\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|tv-show|tv-season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>id\d{9,10}))(?:\?(?P<url_params>.*))?", flags=re.IGNORECASE)  # noqa: E501
+    url_regex = re.compile(r"(?i)(?P<base_url>https?://itunes\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|tv-show|tv-season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>id\d{9,10}))(?:\?(?P<url_params>.*))?")
     subtitles_class = WebVTTSubtitles
     is_movie_scraper = True
     uses_scrapers = ["appletv"]
 
-    def __init__(self, config_data: dict | None = None):
-        super().__init__(config_data=config_data)
-        self._appletv_scraper = ScraperFactory().get_scraper_instance(scraper_id="appletv",
-                                                                      config_data=self._config_data,
-                                                                      raise_error=True)
+    _subtitles_filters = {
+        HLSScraper.M3U8Attribute.GROUP_ID.value: ["subtitles_ak", "subtitles_vod-ak-amt.tv.apple.com"],
+        **HLSScraper._subtitles_filters,  # noqa: SLF001
+    }
+
+    def __init__(self,  user_agent: str | None = None, config_data: dict | None = None):
+        super().__init__(user_agent=user_agent, config_data=config_data)
+        self._appletv_scraper = ScraperFactory.get_scraper_instance(
+            scraper_id="appletv",
+            kwargs={"config_data": config_data},
+            extract_scraper_config=True,
+            raise_error=True,
+        )
 
     def get_data(self, url: str) -> ScrapedMediaResponse[Movie]:
         """
         Scrape iTunes to find info about a movie, and it's M3U8 main_playlist.
 
         Args:
             url (str): An iTunes store movie URL.
@@ -77,45 +85,58 @@
             logger.debug(f"iTunes URL: {url} redirected to an invalid Apple TV URL: '{redirect_location}'.")
             raise ScraperError("Redirect URL is not a valid Apple TV URL.")
 
         return self._appletv_scraper.get_data(redirect_location)
 
     def get_subtitles(self, main_playlist: str | list[str], language_filter: list[str] | str | None = None,
                       subrip_conversion: bool = False) -> Iterator[SubtitlesData]:
-        playlist_filters = {self.M3U8Attribute.LANGUAGE.value: language_filter} if language_filter else None
-        main_playlist_m3u8 = self.load_m3u8(main_playlist)
+        language_filters = {self.M3U8Attribute.LANGUAGE.value: language_filter} if language_filter else None
+        main_playlist_m3u8 = self.load_m3u8(url=main_playlist)
 
         if main_playlist_m3u8 is None:
             raise PlaylistLoadError("Could not load M3U8 playlist.")
 
+        playlist_filters = (merge_dict_values(self._subtitles_filters, language_filters)
+                            if language_filters
+                            else self._subtitles_filters)
+
         matched_media_items = self.get_media_playlists(main_playlist=main_playlist_m3u8,
                                                        playlist_filters=playlist_filters)
 
         for matched_media in matched_media_items:
+            language_name = matched_media.name.replace(' (forced)', '').strip()
+            language_code = matched_media.language
+            language_info_str = f"{language_name} ({language_code})"
+
             try:
                 m3u8_data = self._session.get(url=matched_media.absolute_uri)
                 matched_media_playlist = m3u8.loads(content=m3u8_data.text, uri=matched_media.absolute_uri)
-                subtitles = self.subtitles_class(language_code=matched_media.language)
-                for segment in self._download_segments_async(matched_media_playlist.segments):
-                    subtitles.append_subtitles(subtitles.loads(segment.decode("utf-8")))
+
+                subtitles_segments = self._download_segments(matched_media_playlist.segments)
+                subtitles = self.subtitles_class(data=subtitles_segments[0], language_code=language_code)
+
+                for segment in subtitles_segments[1:]:
+                    segment_subtitles_obj = self.subtitles_class(data=segment, language_code=language_code)
+                    segment_subtitles_obj.remove_head_blocks()
+                    subtitles.append_subtitles(segment_subtitles_obj)
 
                 subtitles.polish(
                     fix_rtl=self.subtitles_fix_rtl,
-                    rtl_languages=self.subtitles_fix_rtl_languages,
                     remove_duplicates=self.subtitles_remove_duplicates,
                 )
 
                 language_name = matched_media.name.replace(' (forced)', '').strip()
 
                 yield SubtitlesData(
-                    language_code=matched_media.language,
+                    language_code=language_code,
                     language_name=language_name,
                     subtitles_format=SubtitlesFormatType.SUBRIP if subrip_conversion else SubtitlesFormatType.WEBVTT,
                     content=subtitles.to_srt().dump() if subrip_conversion else subtitles.dump(),
+                    content_encoding=subtitles.encoding,
                     special_type=self.detect_subtitles_type(matched_media),
                 )
 
             except Exception as e:
-                logger.warning(f"Failed to download {matched_media.name} ({matched_media.language}) subtitles. "
+                logger.warning(f"Failed to download {language_info_str} subtitles. "
                                f"Skipping...")
                 logger.debug(e, exc_info=True)
                 continue
```

### Comparing `isubrip-2.5.2/isubrip/scrapers/scraper.py` & `isubrip-2.5.3/isubrip/scrapers/scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import asyncio
 from enum import Enum
 import importlib
 import inspect
 from pathlib import Path
 import re
 import sys
-from typing import TYPE_CHECKING, ClassVar, Iterator, List, Literal, Type, TypeVar, Union, overload
+from typing import TYPE_CHECKING, Any, ClassVar, Iterator, List, Literal, Type, TypeVar, Union, overload
 
-import aiohttp
+import httpx
 import m3u8
 from m3u8 import M3U8, Media, Segment, SegmentList
 import requests
 import requests.utils
 
 from isubrip.config import Config, ConfigSetting
 from isubrip.constants import PACKAGE_NAME, SCRAPER_MODULES_SUFFIX
@@ -33,66 +33,138 @@
 class Scraper(ABC, metaclass=SingletonMeta):
     """
     A base class for scrapers.
 
     Attributes:
         default_user_agent (str): [Class Attribute]
             Default user agent to use if no other user agent is specified when making requests.
+        default_proxy (str | None): [Class Attribute] Default proxy to use when making requests.
+        default_verify_ssl (bool): [Class Attribute] Whether to verify SSL certificates by default.
         subtitles_fix_rtl (bool): [Class Attribute] Whether to fix RTL from downloaded subtitles.
-        subtitles_fix_rtl_languages (list[str] | None): [Class Attribute]
             A list of languages to fix RTL on. If None, a default list will be used.
         subtitles_remove_duplicates (bool): [Class Attribute]
             Whether to remove duplicate lines from downloaded subtitles.
 
         id (str): [Class Attribute] ID of the scraper.
         name (str): [Class Attribute] Name of the scraper.
         abbreviation (str): [Class Attribute] Abbreviation of the scraper.
         url_regex (re.Pattern | list[re.Pattern]): [Class Attribute] A RegEx pattern to find URLs matching the service.
         subtitles_class (type[Subtitles]): [Class Attribute] Class of the subtitles format returned by the scraper.
         is_movie_scraper (bool): [Class Attribute] Whether the scraper is for movies.
         is_series_scraper (bool): [Class Attribute] Whether the scraper is for series.
         uses_scrapers (list[str]): [Class Attribute] A list of IDs for other scraper classes that this scraper uses.
             This assures that the config data for the other scrapers is passed as well.
         _session (requests.Session): A requests session to use for making requests.
+        _user_agent (str): A user agent to use when making requests.
+        _proxy (str | None): A proxy to use when making requests.
+        _verify_ssl (bool): Whether to verify SSL certificates when making requests.
         config (Config): A Config object containing the scraper's configuration.
     """
     default_user_agent: ClassVar[str] = requests.utils.default_user_agent()
+    default_proxy: ClassVar[str | None] = None
+    default_verify_ssl: ClassVar[bool] = True
     subtitles_fix_rtl: ClassVar[bool] = False
-    subtitles_fix_rtl_languages: ClassVar[list | None] = ["ar", "he"]
     subtitles_remove_duplicates: ClassVar[bool] = True
 
     id: ClassVar[str]
     name: ClassVar[str]
     abbreviation: ClassVar[str]
     url_regex: ClassVar[re.Pattern | list[re.Pattern]]
     subtitles_class: ClassVar[type[Subtitles]]
     is_movie_scraper: ClassVar[bool] = False
     is_series_scraper: ClassVar[bool] = False
     uses_scrapers: ClassVar[list[str]] = []
 
-    def __init__(self, config_data: dict | None = None):
+    def __init__(self, user_agent: str | None = None, proxy: str | None = None,
+                 verify_ssl: bool | None = None, config_data: dict | None = None):
         """
         Initialize a Scraper object.
 
         Args:
+            user_agent (str | None, optional): A user agent to use when making requests. Defaults to None.
+            proxy (str | None, optional): A proxy to use when making requests. Defaults to None.
+            verify_ssl (bool | None, optional): Whether to verify SSL certificates. Defaults to None.
             config_data (dict | None, optional): A dictionary containing scraper's configuration data. Defaults to None.
         """
         self._session = requests.Session()
-        self._config_data = config_data
         self.config = Config(config_data=config_data.get(self.id) if config_data else None)
 
+        # Add a "user-agent" setting by default to all scrapers
         self.config.add_settings([
             ConfigSetting(
                 key="user-agent",
-                type=str,
+                value_type=str,
                 required=False,
-            )],
+            ),
+            ConfigSetting(
+                key="proxy",
+                value_type=str,
+                required=False,
+            ),
+            ConfigSetting(
+                key="verify-ssl",
+                value_type=bool,
+                required=False,
+            ),
+        ],
             check_config=False)
 
-        self._session.headers.update({"User-Agent": self.config.get("user-agent") or self.default_user_agent})
+        self._user_agent: str
+        self._proxy: str | None
+        self._verify_ssl: bool
+
+        # User-Agent Configuration
+        if user_agent is not None:
+            self._user_agent = user_agent
+
+        elif "user-agent" in self.config:
+            self._user_agent = self.config["user-agent"]
+
+        else:
+            self._user_agent = self.default_user_agent
+
+        if self._user_agent != self.default_user_agent:
+            logger.debug(f"Initializing '{self.name}' scraper with user-agent: '{user_agent}'.")
+
+        # Proxy Configuration
+        if proxy is not None:
+            self._proxy = proxy
+
+        elif "proxy" in self.config:
+            self._proxy = self.config["proxy"]
+
+        else:
+            self._proxy = self.default_proxy
+
+        if self._proxy != self.default_proxy:
+            logger.debug(f"Initializing '{self.name}' scraper with proxy: '{proxy}'.")
+
+        # SSL Verification Configuration
+        if verify_ssl is not None:
+            self._verify_ssl = verify_ssl
+
+        elif "verify-ssl" in self.config:
+            self._verify_ssl = self.config["verify-ssl"]
+
+        else:
+            self._verify_ssl = self.default_verify_ssl
+
+        if self._verify_ssl != self.default_verify_ssl:
+            logger.debug(f"Initializing '{self.name}' scraper with SSL verification set to: '{verify_ssl}'.")
+
+        self._session.headers.update({"User-Agent": self._user_agent})
+
+        if self._proxy:
+            self._session.proxies.update({"http": self._proxy, "https": self._proxy})
+
+        self._session.verify = self._verify_ssl
+
+        if not self._verify_ssl:
+            import urllib3
+            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     @classmethod
     @overload
     def match_url(cls, url: str, raise_error: Literal[True] = ...) -> re.Match:
         ...
 
     @classmethod
@@ -111,21 +183,21 @@
 
         Returns:
             re.Match | None: A Match object if the URL matches the regex, None otherwise (if raise_error is False).
 
         Raises:
             ValueError: If the URL doesn't match the regex and raise_error is True.
         """
-        if isinstance(cls.url_regex, re.Pattern):
-            return re.fullmatch(pattern=cls.url_regex, string=url)
+        if isinstance(cls.url_regex, re.Pattern) and (match_result := re.fullmatch(pattern=cls.url_regex, string=url)):
+            return match_result
 
-        # isinstance(cls.url_regex, list):
-        for url_regex_item in cls.url_regex:
-            if result := re.fullmatch(pattern=url_regex_item, string=url):
-                return result
+        if isinstance(cls.url_regex, list):
+            for url_regex_item in cls.url_regex:
+                if result := re.fullmatch(pattern=url_regex_item, string=url):
+                    return result
 
         if raise_error:
             raise ValueError(f"URL '{url}' doesn't match the URL regex of {cls.name}.")
 
         return None
 
     def __enter__(self) -> Scraper:
@@ -166,31 +238,32 @@
             SubtitlesData: A SubtitlesData object for each subtitle found
                 in the main playlist (matching the filters, if given).
         """
 
 
 class AsyncScraper(Scraper, ABC):
     """A base class for scrapers that utilize async requests."""
-    def __init__(self, config_data: dict | None = None):
-        super().__init__(config_data)
-        self.async_session = aiohttp.ClientSession()
-        self.async_session.headers.update(self._session.headers)
+    def __init__(self,  user_agent: str | None = None, config_data: dict | None = None):
+        super().__init__(user_agent=user_agent, config_data=config_data)
+        self._async_session = httpx.AsyncClient(
+            headers={"User-Agent": self._user_agent},
+            proxy=(httpx.Proxy(url=self._proxy) if self._proxy else None),
+            verify=self._verify_ssl,
+        )
 
     def close(self) -> None:
-        asyncio.get_event_loop().run_until_complete(self._async_close())
+        asyncio.get_event_loop().run_until_complete(self._async_session.aclose())
         super().close()
 
     async def _async_close(self) -> None:
-        await self.async_session.close()
+        await self._async_session.aclose()
 
 
 class HLSScraper(AsyncScraper, ABC):
     """A base class for HLS (m3u8) scrapers."""
-    playlist_filters_config_category = "playlist-filters"
-
     class M3U8Attribute(Enum):
         """
         An enum representing all possible M3U8 attributes.
         Names / Keys represent M3U8 Media object attributes (should be converted to lowercase),
         and values represent the name of the key for config usage.
         """
         ASSOC_LANGUAGE = "assoc-language"
@@ -202,82 +275,103 @@
         GROUP_ID = "group-id"
         INSTREAM_ID = "instream-id"
         LANGUAGE = "language"
         NAME = "name"
         STABLE_RENDITION_ID = "stable-rendition-id"
         TYPE = "type"
 
-    def __init__(self, config_data: dict | None = None):
-        super().__init__(config_data)
+    _playlist_filters_config_category = "playlist-filters"
+    _subtitles_filters: dict[str, Any] = {
+        M3U8Attribute.TYPE.value: "SUBTITLES",
+    }
 
-        if self.config is None:
-            self.config = Config()
+    def __init__(self,  user_agent: str | None = None, config_data: dict | None = None):
+        super().__init__(user_agent=user_agent, config_data=config_data)
 
         # Add M3U8 filters settings
         self.config.add_settings([
             ConfigSetting(
-                category=self.playlist_filters_config_category,
+                category=self._playlist_filters_config_category,
                 key=m3u8_attribute.value,
-                type=Union[str, List[str]],
+                value_type=Union[str, List[str]],
                 required=False,
             ) for m3u8_attribute in self.M3U8Attribute],
             check_config=False)
 
-    def _download_segments_async(self, segments: SegmentList[Segment]) -> list[bytes]:
+    def _download_segments(self, segments: SegmentList[Segment]) -> list[bytes]:
         """
         Download M3U8 segments asynchronously.
 
         Args:
             segments (m3u8.SegmentList[m3u8.Segment]): List of segments to download.
 
         Returns:
             list[bytes]: List of downloaded segments.
         """
-        loop = asyncio.get_event_loop()
-        async_tasks = [loop.create_task(self._download_segment_async(segment.absolute_uri)) for segment in segments]
-        segments_bytes = loop.run_until_complete(asyncio.gather(*async_tasks))
+        return asyncio.get_event_loop().run_until_complete(self._download_segments_async(segments))
 
-        return list(segments_bytes)
+    async def _download_segments_async(self, segments: SegmentList[Segment]) -> list[bytes]:
+        """
+        Download M3U8 segments asynchronously.
+
+        Args:
+            segments (m3u8.SegmentList[m3u8.Segment]): List of segments to download.
+
+        Returns:
+            list[bytes]: List of downloaded segments.
+        """
+        async_tasks = [
+            self._download_segment_async(url=segment.absolute_uri)
+            for segment in segments
+        ]
+
+        return await asyncio.gather(*async_tasks)
 
     async def _download_segment_async(self, url: str) -> bytes:
         """
         Download an M3U8 segment asynchronously.
 
         Args:
             url (str): URL of the segment to download.
 
         Returns:
             bytes: Downloaded segment.
         """
-        async with self.async_session.get(url) as response:
-            segment: bytes = await response.read()
-
-        return segment
+        response = await self._async_session.get(url)
+        return response.content
 
-    def load_m3u8(self, url: str | list[str]) -> M3U8 | None:
+    def load_m3u8(self, url: str | list[str], headers: dict | None = None) -> M3U8 | None:
         """
         Load an M3U8 playlist from a URL to an M3U8 object.
         Multiple URLs can be given, in which case the first one that loads successfully will be returned.
         The method uses caching to avoid loading the same playlist multiple times.
 
         Args:
             url (str | list[str]): URL of the M3U8 playlist to load. Can also be a list of URLs (for redundancy).
+            headers (dict | None, optional): A dictionary of headers to use when making the request.
+                Defaults to None (results in using session's configured headers).
 
         Returns:
             m3u8.M3U8: An M3U8 object representing the playlist.
         """
+        _headers = headers or self._session.headers
+
         for url_item in single_to_list(url):
             try:
-                m3u8_data = self._session.get(url_item).text
-                return m3u8.loads(content=m3u8_data, uri=url_item)
+                response = self._session.get(url=url_item, headers=_headers)
 
             except Exception as e:
                 logger.debug(f"Failed to load M3U8 playlist '{url_item}': {e}")
                 continue
 
+            if not response.text:
+                raise PlaylistLoadError("Received empty response for playlist from server.")
+
+            return m3u8.loads(content=response.text, uri=url_item)
+
         return None
 
     @staticmethod
     def detect_subtitles_type(subtitles_media: Media) -> SubtitlesType | None:
         """
         Detect the subtitles type (Closed Captions, Forced, etc.) from an M3U8 Media object.
 
@@ -292,40 +386,31 @@
 
         if subtitles_media.characteristics is not None and "public.accessibility" in subtitles_media.characteristics:
             return SubtitlesType.CC
 
         return None
 
     def get_media_playlists(self, main_playlist: M3U8,
-                            playlist_filters: dict[str, str | list[str]] | None = None,
-                            include_default_filters: bool = True) -> list[Media]:
+                            playlist_filters: dict[str, str | list[str]] | None = None) -> list[Media]:
         """
         Find and yield playlists of media within an M3U8 main_playlist using optional filters.
 
         Args:
             main_playlist (m3u8.M3U8): An M3U8 object of the main main_playlist.
             playlist_filters (dict[str, str | list[str], optional):
                 A dictionary of filters to use when searching for subtitles.
-                Will be added to filters set by the config (unless `include_default_filters` is set to false).
-                Defaults to None.
-            include_default_filters (bool, optional): Whether to include the default filters set by the config or not.
-                Defaults to True.
+                Will be added to filters set by the config. Defaults to None.
 
         Returns:
             list[Media]: A list of  matching Media objects.
         """
         results = []
-        default_filters: dict | None = self.config.get(HLSScraper.playlist_filters_config_category)
-
-        if include_default_filters and default_filters:
-            if not playlist_filters:
-                playlist_filters = default_filters
-
-            else:
-                playlist_filters = merge_dict_values(default_filters, playlist_filters)
+        config_filters: dict | None = self.config.get(self._playlist_filters_config_category)
+        # Merge filtering dictionaries to a single dictionary
+        playlist_filters = merge_dict_values(*[item for item in (playlist_filters, config_filters) if item])
 
         for media in main_playlist.media:
             if not playlist_filters:
                 results.append(media)
                 continue
 
             is_valid = True
@@ -349,166 +434,183 @@
 
             if is_valid:
                 results.append(media)
 
         return results
 
 
-class ScraperFactory(metaclass=SingletonMeta):
-    def __init__(self) -> None:
-        self._scraper_classes_cache: list[type[Scraper]] | None = None
-        self._scraper_instances_cache: dict[type[Scraper], Scraper] = {}
-        self._currently_initializing: list[type[Scraper]] = []  # Used to prevent infinite recursion
+class ScraperFactory:
+    _scraper_classes_cache: list[type[Scraper]] | None = None
+    _scraper_instances_cache: dict[type[Scraper], Scraper] = {}
+    _currently_initializing: list[type[Scraper]] = []  # Used to prevent infinite recursion
 
-    def get_initialized_scrapers(self) -> list[Scraper]:
+    @classmethod
+    def get_initialized_scrapers(cls) -> list[Scraper]:
         """
         Get a list of all previously initialized scrapers.
 
         Returns:
             list[Scraper]: A list of initialized scrapers.
         """
-        return list(self._scraper_instances_cache.values())
+        return list(cls._scraper_instances_cache.values())
 
-    def get_scraper_classes(self) -> list[type[Scraper]]:
+    @classmethod
+    def get_scraper_classes(cls) -> list[type[Scraper]]:
         """
         Find all scraper classes in the scrapers directory.
 
         Returns:
             list[Scraper]: A Scraper subclass.
         """
-        if self._scraper_classes_cache is not None:
-            return self._scraper_classes_cache
+        if cls._scraper_classes_cache is not None:
+            return cls._scraper_classes_cache
 
-        self._scraper_classes_cache = []
+        cls._scraper_classes_cache = []
         scraper_modules_paths = Path(__file__).parent.glob(f"*{SCRAPER_MODULES_SUFFIX}.py")
 
         for scraper_module_path in scraper_modules_paths:
             sys.path.append(str(scraper_module_path))
 
             module = importlib.import_module(f"{PACKAGE_NAME}.scrapers.{scraper_module_path.stem}")
 
             # Find all 'Scraper' subclasses
             for _, obj in inspect.getmembers(module,
                                              predicate=lambda x: inspect.isclass(x) and issubclass(x, Scraper)):
                 # Skip object if it's an abstract or imported from another module
                 if not inspect.isabstract(obj) and obj.__module__ == module.__name__:
-                    self._scraper_classes_cache.append(obj)
+                    cls._scraper_classes_cache.append(obj)
 
-        return self._scraper_classes_cache
+        return cls._scraper_classes_cache
 
-    def _get_scraper_instance(self, scraper_class: type[ScraperT],
-                              scrapers_config_data: dict | None = None) -> ScraperT:
+    @classmethod
+    def _get_scraper_instance(cls, scraper_class: type[ScraperT], kwargs: dict | None = None,
+                              extract_scraper_config: bool = False) -> ScraperT:
         """
         Initialize and return a scraper instance.
 
         Args:
             scraper_class (type[ScraperT]): A scraper class to initialize.
-            scrapers_config_data (dict, optional): A dictionary containing scrapers config data to use
-                when creating a new scraper. Defaults to None.
+            kwargs (dict | None, optional): A dictionary containing parameters to pass to the scraper's constructor.
+                Defaults to None.
+            extract_scraper_config (bool, optional): Whether the passed 'config_data' (within kwargs)
+                is a main config dictionary, and scraper's config should be extracted from it. Defaults to False.
 
         Returns:
             Scraper: An instance of the given scraper class.
         """
         logger.debug(f"Initializing '{scraper_class.name}' scraper...")
+        kwargs = kwargs or {}
 
-        if scraper_class not in self._scraper_instances_cache:
+        if scraper_class not in cls._scraper_instances_cache:
             logger.debug(f"'{scraper_class.name}' scraper not found in cache, creating a new instance...")
 
-            if scraper_class in self._currently_initializing:
+            if scraper_class in cls._currently_initializing:
                 raise ScraperError(f"'{scraper_class.name}' scraper is already being initialized.\n"
                                    f"Make sure there are no circular dependencies between scrapers.")
 
-            self._currently_initializing.append(scraper_class)
+            cls._currently_initializing.append(scraper_class)
+
+            if extract_scraper_config:
+                if kwargs.get("config_data"):
+                    required_scrapers_ids = [scraper_class.id, *scraper_class.uses_scrapers]
+                    kwargs["config_data"] = (
+                        {scraper_id: kwargs["config_data"][scraper_id] for scraper_id in required_scrapers_ids
+                         if kwargs["config_data"].get(scraper_id)}
+                    )
 
-            # Set config data for the scraper and its dependencies, if any
-            if not scrapers_config_data:
-                config_data = None
-
-            else:
-                required_scrapers_ids = [scraper_class.id, *scraper_class.uses_scrapers]
-                config_data = \
-                    {scraper_id: scrapers_config_data[scraper_id] for scraper_id in required_scrapers_ids
-                     if scrapers_config_data.get(scraper_id)}
+                else:
+                    kwargs["config_data"] = None
 
-            self._scraper_instances_cache[scraper_class] = scraper_class(config_data=config_data)
-            self._currently_initializing.remove(scraper_class)
+            cls._scraper_instances_cache[scraper_class] = scraper_class(**kwargs)
+            cls._currently_initializing.remove(scraper_class)
 
         else:
             logger.debug(f"Cached '{scraper_class.name}' scraper instance found and will be used.")
 
-        return self._scraper_instances_cache[scraper_class]  # type: ignore[return-value]
+        return cls._scraper_instances_cache[scraper_class]  # type: ignore[return-value]
 
+    @classmethod
     @overload
-    def get_scraper_instance(self, scraper_class: type[ScraperT], scraper_id: str | None = ...,
-                             url: str | None = ..., config_data: dict | None = ...,
+    def get_scraper_instance(cls, scraper_class: type[ScraperT], scraper_id: str | None = ...,
+                             url: str | None = ..., kwargs: dict | None = ..., extract_scraper_config: bool = ...,
                              raise_error: Literal[True] = ...) -> ScraperT:
         ...
 
+    @classmethod
     @overload
-    def get_scraper_instance(self, scraper_class: type[ScraperT], scraper_id: str | None = ...,
-                             url: str | None = ..., config_data: dict | None = ...,
+    def get_scraper_instance(cls, scraper_class: type[ScraperT], scraper_id: str | None = ...,
+                             url: str | None = ..., kwargs: dict | None = ...,
+                             extract_scraper_config: bool = ...,
                              raise_error: Literal[False] = ...) -> ScraperT | None:
         ...
 
+    @classmethod
     @overload
-    def get_scraper_instance(self, scraper_class: None = ..., scraper_id: str | None = ...,
-                             url: str | None = ..., config_data: dict | None = ...,
+    def get_scraper_instance(cls, scraper_class: None = ..., scraper_id: str | None = ...,
+                             url: str | None = ..., kwargs: dict | None = ..., extract_scraper_config: bool = ...,
                              raise_error: Literal[True] = ...) -> Scraper:
         ...
 
+    @classmethod
     @overload
-    def get_scraper_instance(self, scraper_class: None = ..., scraper_id: str | None = ...,
-                             url: str | None = ..., config_data: dict | None = ...,
+    def get_scraper_instance(cls, scraper_class: None = ..., scraper_id: str | None = ...,
+                             url: str | None = ..., kwargs: dict | None = ..., extract_scraper_config: bool = ...,
                              raise_error: Literal[False] = ...) -> Scraper | None:
         ...
 
-    def get_scraper_instance(self, scraper_class: type[Scraper] | None = None, scraper_id: str | None = None,
-                             url: str | None = None, config_data: dict | None = None,
+    @classmethod
+    def get_scraper_instance(cls, scraper_class: type[Scraper] | None = None, scraper_id: str | None = None,
+                             url: str | None = None, kwargs: dict | None = None, extract_scraper_config: bool = False,
                              raise_error: bool = True) -> Scraper | None:
         """
         Find, initialize and return a scraper that matches the given URL or ID.
 
         Args:
             scraper_class (type[ScraperT] | None, optional): A scraper class to initialize. Defaults to None.
             scraper_id (str | None, optional): ID of a scraper to initialize. Defaults to None.
             url (str | None, optional): A URL to match a scraper for to initialize. Defaults to None.
-            config_data (dict, optional): A dictionary containing scrapers config data to use
-                when creating a new scraper. Defaults to None.
+            kwargs (dict | None, optional): A dictionary containing parameters to pass to the scraper's constructor.
+                Defaults to None.
+            extract_scraper_config (bool, optional): Whether the passed 'config_data' (within kwargs)
             raise_error (bool, optional): Whether to raise an error if no scraper was found. Defaults to False.
 
         Returns:
             ScraperT | Scraper | None: An instance of a scraper that matches the given URL or ID,
                 None otherwise (if raise_error is False).
 
         Raises:
             ValueError: If no scraper was found and raise_error is True.
         """
         if scraper_class:
-            return self._get_scraper_instance(scraper_class=scraper_class,
-                                              scrapers_config_data=config_data)
+            return cls._get_scraper_instance(scraper_class=scraper_class, kwargs=kwargs,
+                                             extract_scraper_config=extract_scraper_config)
 
         if not (scraper_id or url):
             raise ValueError("At least one of: 'scraper_class', 'scraper_id', or 'url' must be provided.")
 
         if scraper_id:
             logger.debug(f"Searching for a scraper object with ID '{scraper_id}'...")
-            for scraper in self.get_scraper_classes():
+            for scraper in cls.get_scraper_classes():
                 if scraper.id == scraper_id:
-                    return self._get_scraper_instance(scraper_class=scraper, scrapers_config_data=config_data)
+                    return cls._get_scraper_instance(scraper_class=scraper, kwargs=kwargs,
+                                                     extract_scraper_config=extract_scraper_config)
 
         elif url:
             logger.debug(f"Searching for a scraper object that matches URL '{url}'...")
-            for scraper in self.get_scraper_classes():
+            for scraper in cls.get_scraper_classes():
                 if scraper.match_url(url) is not None:
-                    return self._get_scraper_instance(scraper_class=scraper, scrapers_config_data=config_data)
+                    return cls._get_scraper_instance(scraper_class=scraper, kwargs=kwargs,
+                                                     extract_scraper_config=extract_scraper_config)
+
+        error_message = "No matching scraper was found."
 
         if raise_error:
-            raise ValueError(f"No matching scraper was found for URL '{url}'")
+            raise ValueError(error_message)
 
-        logger.debug("No matching scraper was found.")
+        logger.debug(error_message)
         return None
 
 
 class ScraperError(Exception):
     pass
```

### Comparing `isubrip-2.5.2/isubrip/subtitle_formats/subrip.py` & `isubrip-2.5.3/isubrip/subtitle_formats/subrip.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,20 +25,17 @@
         return self
 
 
 class SubRipSubtitles(Subtitles[SubRipCaptionBlock]):
     """An object representing a SubRip subtitles file."""
     format = SubtitlesFormatType.SUBRIP
 
-    def dumps(self) -> str:
+    def _dumps(self) -> str:
         subtitles_str = ""
-        count = 0
 
-        for block in self.blocks:
-            subtitles_str += f"{(count + 1)}\n{str(block)}\n\n"
-            count += 1
+        for i, block in enumerate(iterable=self.blocks, start=1):
+            subtitles_str += f"{i}\n{str(block)}\n\n"
 
         return subtitles_str.rstrip('\n')
 
-    @staticmethod
-    def loads(subtitles_data: str) -> SubRipSubtitles:
+    def _loads(self, data: str) -> None:
         raise NotImplementedError("SubRip subtitles loading is not supported.")
```

### Comparing `isubrip-2.5.2/isubrip/subtitle_formats/subtitles.py` & `isubrip-2.5.3/isubrip/subtitle_formats/subtitles.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,85 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from datetime import time
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypeVar
 
+from isubrip.logger import logger
+
 if TYPE_CHECKING:
-    from isubrip.data_structures import SubtitlesFormatType, SubtitlesType
+    from isubrip.data_structures import SubtitlesFormatType
     from isubrip.subtitle_formats.subrip import SubRipCaptionBlock, SubRipSubtitles
 
 RTL_CONTROL_CHARS = ('\u200e', '\u200f', '\u202a', '\u202b', '\u202c', '\u202d', '\u202e')
 RTL_CHAR = '\u202b'
-RTL_LANGUAGES = ["ar", "he"]
+RTL_LANGUAGES = ["ar", "he", "he-il"]
 
 SubtitlesT = TypeVar('SubtitlesT', bound='Subtitles')
 SubtitlesBlockT = TypeVar('SubtitlesBlockT', bound='SubtitlesBlock')
 
 
 class SubtitlesBlock(ABC):
-    """Abstract base class for subtitles blocks."""
+    """
+    Abstract base class for subtitles blocks.
+
+    Attributes:
+        modified (bool): Whether the block has been modified.
+    """
+
+    def __init__(self) -> None:
+        self.modified: bool = False
+
     @abstractmethod
     def __str__(self) -> str:
         pass
 
     @abstractmethod
     def __eq__(self, other: Any) -> bool:
         pass
 
 
 class SubtitlesCaptionBlock(SubtitlesBlock, ABC):
-    """A base class for subtitles caption blocks."""
+    """
+    A base class for subtitles caption blocks.
+
+    Attributes:
+        start_time (time): Start timestamp of the caption block.
+        end_time (time): End timestamp of the caption block.
+        payload (str): Caption block's payload.
+    """
 
     def __init__(self, start_time: time, end_time: time, payload: str):
         """
         Initialize a new SubtitlesCaptionBlock object.
 
         Args:
             start_time: Start timestamp of the caption block.
             end_time: End timestamp of the caption block.
-            payload: Caption block's payload (text).
+            payload: Caption block's payload.
         """
+        super().__init__()
         self.start_time = start_time
         self.end_time = end_time
         self.payload = payload
 
     def fix_rtl(self) -> None:
-        """Fix text direction to RTL."""
+        """Fix payload's text direction to RTL."""
+        previous_payload = self.payload
+
         # Remove previous RTL-related formatting
         for char in RTL_CONTROL_CHARS:
             self.payload = self.payload.replace(char, '')
 
         # Add RLM char at the start of every line
         self.payload = RTL_CHAR + self.payload.replace("\n", f"\n{RTL_CHAR}")
 
+        if self.payload != previous_payload:
+            self.modified = True
+
     @abstractmethod
     def to_srt(self) -> SubRipCaptionBlock:
         """
         Convert WebVTT caption block to SRT caption block.
 
         Returns:
             SubRipCaptionBlock: The caption block in SRT format.
@@ -64,154 +88,248 @@
 
 
 class Subtitles(Generic[SubtitlesBlockT], ABC):
     """
     An object representing subtitles, made out of blocks.
 
     Attributes:
+        _modified (bool): Whether the subtitles have been modified.
         format (SubtitlesFormatType): [Class Attribute] Format of the subtitles (contains name and file extension).
+        language_code (str): Language code of the subtitles.
         blocks (list[SubtitlesBlock]): A list of subtitles blocks that make up the subtitles.
-        language_code (str | None): Language code of the subtitles.
-        special_type (SubtitlesType | None): Special type of the subtitles (if any).
+        encoding (str): Encoding of the subtitles.
+        raw_data (bytes | None): Raw data of the subtitles.
     """
     format: ClassVar[SubtitlesFormatType]
 
-    def __init__(self, blocks: list[SubtitlesBlockT] | None = None,
-                 language_code: str | None = None, special_type: SubtitlesType | None = None):
+    def __init__(self, data: bytes | None, language_code: str, encoding: str = "utf-8"):
         """
         Initialize a new Subtitles object.
 
         Args:
-            blocks (list[SubtitlesBlock] | None, optional): A list of subtitles to initialize the object with.
-                Defaults to None.
-            language_code (str | None, optional): Language code of the subtitles. Defaults to None.
-            special_type (SubtitlesType | None, optional): Special type of the subtitles (if any). Defaults to None.
+            data (bytes | None): Raw data of the subtitles.
+            language_code (str): Language code of the subtitles.
+            encoding (str, optional): Encoding of the subtitles. Defaults to "utf-8".
         """
-        self.language_code = language_code
-        self.special_type = special_type
+        self._modified = False
+        self.raw_data = None
 
-        if blocks is None:
-            self.blocks = []
+        self.blocks: list[SubtitlesBlockT] = []
 
-        else:
-            self.blocks = blocks
+        self.language_code = language_code
+        self.encoding = encoding
+
+        if data:
+            self.raw_data = data
+            self._load(data=data)
 
     def __add__(self: SubtitlesT, obj: SubtitlesBlockT | SubtitlesT) -> SubtitlesT:
         """
         Add a new subtitles block, or append blocks from another subtitles object.
 
         Args:
             obj (SubtitlesBlock | Subtitles): A subtitles block or another subtitles object.
 
         Returns:
             Subtitles: The current subtitles object.
         """
         if isinstance(obj, SubtitlesBlock):
-            self.add_block(obj)
+            self.add_blocks(obj)
 
         elif isinstance(obj, self.__class__):
             self.append_subtitles(obj)
 
+        else:
+            logger.warning(f"Cannot add object of type '{type(obj)}' to '{type(self)}' object. Skipping...")
+
         return self
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self)) and self.blocks == other.blocks
 
     def __str__(self) -> str:
         return self.dumps()
 
+    def _dump(self) -> bytes:
+        """
+        Dump subtitles object to bytes representing the subtitles.
+
+        Returns:
+            bytes: The subtitles in a bytes object.
+        """
+        return self._dumps().encode(encoding=self.encoding)
+
     @abstractmethod
-    def dumps(self) -> str:
-        """Dump subtitles object to a string representing the subtitles."""
+    def _dumps(self) -> str:
+        """
+        Dump subtitles object to a string representing the subtitles.
+
+        Returns:
+            str: The subtitles in a string format.
+        """
+        ...
+
+    def _load(self, data: bytes) -> None:
+        """
+        Load and parse subtitles data from bytes.
+
+        Args:
+            data (bytes): Subtitles data to load.
+        """
+        parsed_data = data.decode(encoding=self.encoding)
+        self._loads(data=parsed_data)
 
-    @staticmethod
     @abstractmethod
-    def loads(subtitles_data: str) -> Subtitles:
-        pass
+    def _loads(self, data: str) -> None:
+        """
+        Load and parse subtitles data from a string.
 
-    def add_block(self: SubtitlesT, block: SubtitlesBlockT | list[SubtitlesBlockT]) -> SubtitlesT:
+        Args:
+            data (bytes): Subtitles data to load.
+        """
+        ...
+
+    def dump(self) -> bytes:
+        """
+        Dump subtitles to a bytes object representing the subtitles.
+        Returns the original raw subtitles data if they have not been modified, and raw data is available.
+
+        Returns:
+            bytes: The subtitles in a bytes object.
+        """
+        if self.raw_data is not None and not self.modified():
+            logger.debug("Returning original raw data as subtitles have not been modified.")
+            return self.raw_data
+
+        return self._dump()
+
+    def dumps(self) -> str:
+        """
+        Dump subtitles to a string representing the subtitles.
+        Returns the original raw subtitles data if they have not been modified, and raw data is available.
+
+        Returns:
+
+        """
+        if self.raw_data is not None and not self.modified():
+            logger.debug("Returning original raw data (decoded) as subtitles have not been modified.")
+            return self.raw_data.decode(encoding=self.encoding)
+
+        return self._dumps()
+
+    def add_blocks(self: SubtitlesT,
+                   blocks: SubtitlesBlockT | list[SubtitlesBlockT],
+                   set_modified: bool = True) -> SubtitlesT:
         """
         Add a new subtitles block to current subtitles.
 
         Args:
-            block (SubtitlesBlock | list[SubtitlesBlock]):
+            blocks (SubtitlesBlock | list[SubtitlesBlock]):
                 A block object or a list of block objects to append.
+            set_modified (bool, optional): Whether to set the subtitles as modified. Defaults to True.
 
         Returns:
             Subtitles: The current subtitles object.
         """
-        if isinstance(block, list):
-            self.blocks.extend(block)
+        if isinstance(blocks, list):
+            if not blocks:
+                return self
+
+            self.blocks.extend(blocks)
 
         else:
-            self.blocks.append(block)
+            self.blocks.append(blocks)
+
+        if set_modified:
+            self._modified = True
 
         return self
 
-    def append_subtitles(self: SubtitlesT, subtitles: SubtitlesT) -> SubtitlesT:
+    def append_subtitles(self: SubtitlesT,
+                         subtitles: SubtitlesT) -> SubtitlesT:
         """
-        Append an existing subtitles object.
+        Append subtitles to an existing subtitles object.
 
         Args:
             subtitles (Subtitles): Subtitles object to append to current subtitles.
 
         Returns:
             Subtitles: The current subtitles object.
         """
+        if not subtitles.blocks:
+            return self
+
         for block in subtitles.blocks:
-            self.add_block(block)
+            self.add_blocks(block)
 
         return self
 
-    def dump(self) -> bytes:
-        return self.dumps().encode(encoding="UTF-8")
-
-    def polish(self: SubtitlesT, fix_rtl: bool = False,
-               rtl_languages: list[str] | None = None, remove_duplicates: bool = False) -> SubtitlesT:
+    def polish(self: SubtitlesT,
+               fix_rtl: bool = False,
+               remove_duplicates: bool = True,
+               ) -> SubtitlesT:
         """
         Apply various fixes to subtitles.
 
         Args:
             fix_rtl (bool, optional): Whether to fix text direction of RTL languages. Defaults to False.
-            rtl_languages (list[str] | None, optional): Language code of the RTL language.
-                If not set, a default list of RTL languages will be used. Defaults to None.
-            remove_duplicates (bool, optional): Whether to remove duplicate captions. Defaults to False.
+            remove_duplicates (bool, optional): Whether to remove duplicate captions. Defaults to True.
 
         Returns:
             Subtitles: The current subtitles object.
         """
-        rtl_language = rtl_languages or RTL_LANGUAGES
+        fix_rtl = (fix_rtl and self.language_code in RTL_LANGUAGES)
+
+        if not any((
+                fix_rtl,
+                remove_duplicates,
+        )):
+            return self
+
         previous_block: SubtitlesBlockT | None = None
 
         for block in self.blocks:
-            if fix_rtl and isinstance(block, SubtitlesCaptionBlock) and \
-                    self.language_code in rtl_language:
+            if fix_rtl:
                 block.fix_rtl()
 
             if remove_duplicates and previous_block is not None and block == previous_block:
                 self.blocks.remove(previous_block)
+                self._modified = True
 
             previous_block = block
 
         return self
 
+    def modified(self) -> bool:
+        """
+        Check if the subtitles have been modified (by checking if any of its blocks have been modified).
+
+        Returns:
+            bool: True if the subtitles have been modified, False otherwise.
+        """
+        return self._modified or any(block.modified for block in self.blocks)
+
     def to_srt(self) -> SubRipSubtitles:
         """
         Convert subtitles to SRT format.
 
         Returns:
             SubRipSubtitles: The subtitles in SRT format.
         """
         from isubrip.subtitle_formats.subrip import SubRipSubtitles
 
-        return SubRipSubtitles(
-            blocks=[block.to_srt() for block in self.blocks if isinstance(block, SubtitlesCaptionBlock)],
+        subrip_subtitles = SubRipSubtitles(
+            data=None,
             language_code=self.language_code,
-            special_type=self.special_type,
+            encoding=self.encoding,
         )
+        subrip_blocks = [block.to_srt() for block in self.blocks if isinstance(block, SubtitlesCaptionBlock)]
+        subrip_subtitles.add_blocks(subrip_blocks)
+
+        return subrip_subtitles
 
 
 def split_timestamp(timestamp: str) -> tuple[time, time]:
     """
     Split a subtitles timestamp into start and end.
 
     Args:
```

### Comparing `isubrip-2.5.2/isubrip/subtitle_formats/webvtt.py` & `isubrip-2.5.3/isubrip/subtitle_formats/webvtt.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     def __init__(self, payload: str, inline: bool = False) -> None:
         """
         Initialize a new object representing a WebVTT comment block.
 
         Args:
             payload (str): Comment payload.
         """
+        super().__init__()
         self.payload = payload
         self.inline = inline
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self)) and self.inline == other.inline and self.payload == other.payload
 
     def __str__(self) -> str:
@@ -115,75 +116,72 @@
     def __init__(self, payload: str) -> None:
         """
         Initialize a new object representing a WebVTT style block.
 
         Args:
             payload (str): Style payload.
         """
+        super().__init__()
         self.payload = payload
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self)) and self.payload == other.payload
 
     def __str__(self) -> str:
-        return f"{self.header} {self.payload}"
+        return f"{self.header}\n{self.payload}"
 
 
 class Region(WebVTTBlock):
     """An object representing a WebVTT region block."""
     header = "REGION"
 
     def __init__(self, payload: str) -> None:
         """
         Initialize a new object representing a WebVTT region block.
 
         Args:
             payload (str): Region payload.
         """
+        super().__init__()
         self.payload = payload
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self)) and self.payload == other.payload
 
     def __str__(self) -> str:
         return f"{self.header} {self.payload}"
 
 
 class WebVTTSubtitles(Subtitles[WebVTTBlock]):
     """An object representing a WebVTT subtitles file."""
     format = SubtitlesFormatType.WEBVTT
 
-    def dumps(self) -> str:
+    def _dumps(self) -> str:
         """
         Dump subtitles to a string representing the subtitles in a WebVTT format.
 
         Returns:
             str: The subtitles in a string using a WebVTT format.
         """
         subtitles_str = "WEBVTT\n\n"
 
         for block in self.blocks:
             subtitles_str += str(block) + "\n\n"
 
         return subtitles_str.rstrip('\n')
 
-    @staticmethod
-    def loads(subtitles_data: str) -> WebVTTSubtitles:
+    def _loads(self, data: str) -> None:
         """
-        Load WebVTT subtitles from a string.
+        Load and parse WebVTT subtitles data from a string.
 
         Args:
-            subtitles_data (str): Subtitles data to load.
-
-        Returns:
-            WebVTTSubtitles: A WebVTTSubtitles object representing the subtitles.
+            data (bytes): Subtitles data to load.
         """
-        subtitles_obj = WebVTTSubtitles()
         prev_line: str = ""
-        lines_iterator = iter(subtitles_data.splitlines())
+        lines_iterator = iter(data.splitlines())
 
         for line in lines_iterator:
             # If the line is a timestamp
             if caption_block_regex := re.match(WEBVTT_CAPTION_BLOCK_REGEX, line):
                 # If previous line wasn't empty, add it as an identifier
                 if prev_line:
                     caption_identifier = prev_line
@@ -199,15 +197,15 @@
                     if not additional_line:
                         line = additional_line
                         break
 
                     caption_payload += additional_line + "\n"
 
                 caption_payload = caption_payload.rstrip("\n")
-                subtitles_obj.add_block(Caption(
+                self.blocks.append(Caption(
                     identifier=caption_identifier,
                     start_time=caption_timestamps[0],
                     end_time=caption_timestamps[1],
                     settings=caption_settings,
                     payload=caption_payload))
 
             elif comment_block_regex := re.match(WEBVTT_COMMENT_HEADER_REGEX, line):
@@ -221,42 +219,56 @@
                 for additional_line in lines_iterator:
                     if not additional_line:
                         line = additional_line
                         break
 
                     comment_payload += additional_line + "\n"
 
-                subtitles_obj.add_block(Comment(comment_payload.rstrip("\n"), inline=inline))
+                self.blocks.append(Comment(comment_payload.rstrip("\n"), inline=inline))
 
             elif line.rstrip(' \t') == Region.header:
                 region_payload = ""
 
                 for additional_line in lines_iterator:
                     if not additional_line:
                         line = additional_line
                         break
 
                     region_payload += additional_line + "\n"
 
-                subtitles_obj.add_block(Region(region_payload.rstrip("\n")))
+                self.blocks.append(Region(region_payload.rstrip("\n")))
 
             elif line.rstrip(' \t') == Style.header:
                 style_payload = ""
 
                 for additional_line in lines_iterator:
                     if not additional_line:
                         line = additional_line
                         break
 
                     style_payload += additional_line + "\n"
 
-                subtitles_obj.add_block(Region(style_payload.rstrip("\n")))
+                self.blocks.append(Style(style_payload.rstrip("\n")))
 
             prev_line = line
-        return subtitles_obj
+
+    def remove_head_blocks(self) -> None:
+        """
+        Remove all head blocks (Style / Region) from the subtitles.
+
+        NOTE:
+            Comment blocks are removed as well if they are before the first caption block (since they're probably
+            related to the head blocks).
+        """
+        for block in self.blocks:
+            if isinstance(block, Caption):
+                break
+
+            if isinstance(block, (Comment, Style, Region)):
+                self.blocks.remove(block)
 
 
 # --- Constants ---
 WEBVTT_PERCENTAGE_REGEX = r"\d{1,3}(?:\.\d+)?%"
 WEBVTT_CAPTION_TIMINGS_REGEX = \
     r"(?:[0-5]\d:)?[0-5]\d:[0-5]\d[\.,]\d{3}[ \t]+-->[ \t]+(?:[0-5]\d:)?[0-5]\d:[0-5]\d[\.,]\d{3}"
 
@@ -273,11 +285,11 @@
                                  f"(?:{WEBVTT_CAPTION_SETTING_POSITION_REGEX})|"
                                  f"(?:{WEBVTT_CAPTION_SETTING_REGION_REGEX})|"
                                  f"(?:{WEBVTT_CAPTION_SETTING_SIZE_REGEX})|"
                                  f"(?:{WEBVTT_CAPTION_SETTING_VERTICAL_REGEX})|"
                                  f"(?:[ \t]+)"
                                  ")*")
 
-WEBVTT_CAPTION_BLOCK_REGEX = rf"^({WEBVTT_CAPTION_TIMINGS_REGEX})[ \t]*({WEBVTT_CAPTION_SETTINGS_REGEX})?"
-WEBVTT_COMMENT_HEADER_REGEX = rf"^{Comment.header}(?:$|[ \t])(.+)?"
+WEBVTT_CAPTION_BLOCK_REGEX = re.compile(rf"^({WEBVTT_CAPTION_TIMINGS_REGEX})[ \t]*({WEBVTT_CAPTION_SETTINGS_REGEX})?")
+WEBVTT_COMMENT_HEADER_REGEX = re.compile(rf"^{Comment.header}(?:$|[ \t])(.+)?")
 
 WEBVTT_ALIGN_TOP_TAG = "{\\an8}"
```

### Comparing `isubrip-2.5.2/isubrip/utils.py` & `isubrip-2.5.3/isubrip/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from __future__ import annotations
 
 from abc import ABCMeta
 import datetime as dt
+from functools import lru_cache
 from pathlib import Path
 import re
+import secrets
+import shutil
 import sys
-from typing import TYPE_CHECKING, Any, Union, get_args, get_origin
+from typing import TYPE_CHECKING, Any, Type, Union, get_args, get_origin
 
+from isubrip.constants import TEMP_FOLDER_PATH, TITLE_REPLACEMENT_STRINGS, WINDOWS_RESERVED_FILE_NAMES
 from isubrip.data_structures import (
     Episode,
     MediaBase,
     Movie,
     Season,
     Series,
     SubtitlesData,
     SubtitlesFormatType,
     SubtitlesType,
 )
 from isubrip.logger import logger
 
 if TYPE_CHECKING:
     from os import PathLike
+    from types import TracebackType
 
     import requests
 
 
 class SingletonMeta(ABCMeta):
     """
     A metaclass that implements the Singleton pattern.
@@ -35,14 +40,69 @@
     def __call__(cls, *args: Any, **kwargs: Any) -> object:
         if cls._instances.get(cls) is None:
             cls._instances[cls] = super().__call__(*args, **kwargs)
 
         return cls._instances[cls]
 
 
+class TempDirGenerator:
+    """A class for generating temporary directories, and disposing them once the object is destroyed."""
+    _generated_temp_directories: list[Path] = []
+
+    def __exit__(self, exc_type: Type[BaseException] | None,
+                 exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+        self.cleanup()
+
+    @classmethod
+    def generate(cls, directory_name: str | None = None) -> Path:
+        """
+        Generate a temporary directory within 'TEMP_FOLDER_PATH'.
+
+        Args:
+            directory_name (str | None, optional): Name of the directory to generate.
+                If not specified, a random string will be generated. Defaults to None.
+
+        Returns:
+            Path: Path to the generated directory.
+        """
+        directory_name = directory_name or secrets.token_hex(5)
+        full_path = TEMP_FOLDER_PATH / directory_name
+
+        if full_path.is_dir():
+            if full_path in cls._generated_temp_directories:  # Generated by this class
+                logger.debug(f"Using previously generated temporary directory: '{full_path}'.")
+                return full_path
+
+            logger.debug(f"Temporary directory '{full_path}' already exists. "
+                         f"Emptying the directory from all contents...")
+            shutil.rmtree(full_path)
+            full_path.mkdir(parents=True)
+
+        else:
+            full_path.mkdir(parents=True)
+            logger.debug(f"Temporary directory has been generated: '{full_path}'")
+
+        cls._generated_temp_directories.append(full_path)
+        return full_path
+
+    @classmethod
+    def cleanup(cls) -> None:
+        """Remove all temporary directories generated by this object."""
+        for temp_directory in cls._generated_temp_directories:
+            logger.debug(f"Removing temporary directory: '{temp_directory}'")
+
+            try:
+                shutil.rmtree(temp_directory)
+
+            except Exception as e:
+                logger.debug(f"Failed to remove temporary directory '{temp_directory}': {e}")
+
+        cls._generated_temp_directories = []
+
+
 def check_type(value: Any, type_) -> bool:  # type: ignore[no-untyped-def]
     """
     Check if a value is of a certain type.
     Works with parameterized generics.
 
     Args:
         value (Any): Value to check.
@@ -117,48 +177,49 @@
     """
     output_path = Path(output_path)
 
     if not output_path.is_dir():
         raise ValueError(f"Invalid path: {output_path}")
 
     if isinstance(media_data, Movie):
-        file_name = generate_release_name(title=media_data.name,
-                                          release_date=media_data.release_date,
-                                          media_source=source_abbreviation,
-                                          language_code=subtitles_data.language_code,
-                                          subtitles_type=subtitles_data.special_type,
-                                          file_format=subtitles_data.subtitles_format)
+        file_name = format_release_name(title=media_data.name,
+                                        release_date=media_data.release_date,
+                                        media_source=source_abbreviation,
+                                        language_code=subtitles_data.language_code,
+                                        subtitles_type=subtitles_data.special_type,
+                                        file_format=subtitles_data.subtitles_format)
     else:  # isinstance(media_data, Episode):
-        file_name = generate_release_name(title=media_data.name,
-                                          release_date=media_data.release_date,
-                                          season_number=media_data.season_number,
-                                          episode_number=media_data.episode_number,
-                                          episode_name=media_data.episode_name,
-                                          media_source=source_abbreviation,
-                                          language_code=subtitles_data.language_code,
-                                          subtitles_type=subtitles_data.special_type,
-                                          file_format=subtitles_data.subtitles_format)
+        file_name = format_release_name(title=media_data.series_name,
+                                        release_date=media_data.release_date,
+                                        season_number=media_data.season_number,
+                                        episode_number=media_data.episode_number,
+                                        episode_name=media_data.episode_name,
+                                        media_source=source_abbreviation,
+                                        language_code=subtitles_data.language_code,
+                                        subtitles_type=subtitles_data.special_type,
+                                        file_format=subtitles_data.subtitles_format)
 
     file_path = output_path / file_name
 
     if file_path.exists() and not overwrite:
-        file_path = generate_non_conflicting_path(file_path)
+        file_path = generate_non_conflicting_path(file_path=file_path)
 
     with file_path.open('wb') as f:
         f.write(subtitles_data.content)
 
     return file_path
 
 
-def generate_media_description(media_data: MediaBase) -> str:
+def format_media_description(media_data: MediaBase, shortened: bool = False) -> str:
     """
     Generate a short description string of a media object.
 
     Args:
         media_data (MediaBase): An object containing media data.
+        shortened (bool, optional): Whether to generate a shortened description. Defaults to False.
 
     Returns:
         str: A short description string of the media object.
     """
     if isinstance(media_data, Movie):
         release_year = (
             media_data.release_date.year
@@ -184,83 +245,61 @@
 
         if media_data.id:
             description_str += f" (ID: {media_data.id})"
 
         return description_str
 
     if isinstance(media_data, Season):
-        description_str = f"{media_data.series_name} - Season {media_data.season_number:02d}"
+        if shortened:
+            description_str = f"Season {media_data.season_number:02d}"
+
+        else:
+            description_str = f"{media_data.series_name} - Season {media_data.season_number:02d}"
 
         if media_data.season_name:
             description_str += f" - {media_data.season_name}"
 
         if media_data.id:
             description_str += f" (ID: {media_data.id})"
 
         return description_str
 
     if isinstance(media_data, Episode):
-        description_str = f"{media_data.series_name} - S{media_data.season_number:02d}E{media_data.episode_number:02d}"
+        if shortened:
+            description_str = f"S{media_data.season_number:02d}E{media_data.episode_number:02d}"
+
+        else:
+            description_str = (f"{media_data.series_name} - "
+                               f"S{media_data.season_number:02d}E{media_data.episode_number:02d}")
 
         if media_data.episode_name:
             description_str += f" - {media_data.episode_name}"
 
         if media_data.id:
             description_str += f" (ID: {media_data.id})"
 
         return description_str
 
     raise ValueError(f"Unsupported media type: '{type(media_data)}'")
 
 
-def generate_non_conflicting_path(file_path: str | Path, has_extension: bool = True) -> Path:
+@lru_cache
+def format_release_name(title: str,
+                        release_date: dt.datetime | int | None = None,
+                        season_number: int | None = None,
+                        episode_number: int | None = None,
+                        episode_name: str | None = None,
+                        media_source: str | None = None,
+                        source_type: str | None = "WEB",
+                        additional_info: str | list[str] | None = None,
+                        language_code: str | None = None,
+                        subtitles_type: SubtitlesType | None = None,
+                        file_format: str | SubtitlesFormatType | None = None) -> str:
     """
-    Generate a non-conflicting path for a file.
-    If the file already exists, a number will be added to the end of the file name.
-
-    Args:
-        file_path (str | Path): Path to a file.
-        has_extension (bool, optional): Whether the name of the file includes file extension. Defaults to True.
-
-    Returns:
-        Path: A non-conflicting file path.
-    """
-    if isinstance(file_path, str):
-        file_path = Path(file_path)
-
-    if not file_path.exists():
-        return file_path
-
-    i = 1
-    while True:
-        if has_extension:
-            new_file_path = file_path.parent / f"{file_path.stem}-{i}{file_path.suffix}"
-
-        else:
-            new_file_path = file_path.parent / f"{file_path}-{i}"
-
-        if not new_file_path.exists():
-            return new_file_path
-
-        i += 1
-
-
-def generate_release_name(title: str,
-                          release_date: dt.datetime | int | None = None,
-                          season_number: int | None = None,
-                          episode_number: int | None = None,
-                          episode_name: str | None = None,
-                          media_source: str | None = None,
-                          source_type: str | None = "WEB",
-                          additional_info: str | list[str] | None = None,
-                          language_code: str | None = None,
-                          subtitles_type: SubtitlesType | None = None,
-                          file_format: str | SubtitlesFormatType | None = None) -> str:
-    """
-    Generate a release name.
+    Format a release name.
 
     Args:
         title (str): Media title.
         release_date (int | None, optional): Release date (datetime), or year (int) of the media. Defaults to None.
         season_number (int | None, optional): Season number. Defaults to None.
         episode_number (int | None, optional): Episode number. Defaults to None.
         episode_name (str | None, optional): Episode name. Defaults to None.
@@ -270,33 +309,30 @@
         language_code (str | None, optional): Language code. Defaults to None.
         subtitles_type (SubtitlesType | None, optional): Subtitles type. Defaults to None.
         file_format (SubtitlesFormat | str | None, optional): File format to use.  Defaults to None.
 
     Returns:
         str: Generated file name.
     """
-    file_name = standardize_title(title)
+    file_name = standardize_title(title).rstrip('.')
 
     if release_date is not None:
         if isinstance(release_date, dt.datetime):
             release_year = release_date.year
 
         else:
             release_year = release_date
 
         file_name += f".{release_year}"
 
-    if season_number is not None:
-        file_name += f".S{season_number:02}"
-
-    if episode_number is not None:
-        file_name += f".E{episode_number:02}"
+    if season_number is not None and episode_number is not None:
+        file_name += f".S{season_number:02}E{episode_number:02}"
 
     if episode_name is not None:
-        file_name += f".{standardize_title(episode_name)}"
+        file_name += f".{standardize_title(episode_name).rstrip('.')}"
 
     if media_source is not None:
         file_name += f".{media_source}"
 
     if source_type is not None:
         file_name += f".{source_type}"
 
@@ -317,38 +353,97 @@
             file_format = file_format.value.file_extension
 
         file_name += f".{file_format}"
 
     return file_name
 
 
+def format_subtitles_description(language_code: str, language_name: str | None = None,
+                                 special_type: SubtitlesType | None = None) -> str:
+    if language_name:
+        language_str = f"{language_name} ({language_code})"
+
+    else:
+        language_str = language_code
+
+    if special_type:
+        language_str += f" [{special_type.value}]"
+
+    return language_str
+
+
+def generate_non_conflicting_path(file_path: Path, has_extension: bool = True) -> Path:
+    """
+    Generate a non-conflicting path for a file.
+    If the file already exists, a number will be added to the end of the file name.
+
+    Args:
+        file_path (Path): Path to a file.
+        has_extension (bool, optional): Whether the name of the file includes file extension. Defaults to True.
+
+    Returns:
+        Path: A non-conflicting file path.
+    """
+    if isinstance(file_path, str):
+        file_path = Path(file_path)
+
+    if not file_path.exists():
+        return file_path
+
+    i = 1
+    while True:
+        if has_extension:
+            new_file_path = file_path.parent / f"{file_path.stem}-{i}{file_path.suffix}"
+
+        else:
+            new_file_path = file_path.parent / f"{file_path}-{i}"
+
+        if not new_file_path.exists():
+            return new_file_path
+
+        i += 1
+
+
 def merge_dict_values(*dictionaries: dict) -> dict:
     """
     A function for merging the values of multiple dictionaries using the same keys.
     If a key already exists, the value will be added to a list of values mapped to that key.
 
+    Note:
+        This function support only merging of lists, without any nesting.
+
     Args:
         *dictionaries (dict): Dictionaries to merge.
 
     Returns:
         dict: A merged dictionary.
     """
-    result: dict = {}
+    _dictionaries = [d for d in dictionaries if d]
 
-    for dict_ in dictionaries:
-        for key, value in dict_.items():
-            if key in result:
-                if isinstance(result[key], list) and value not in result[key]:
-                    result[key].append(value)
+    if len(_dictionaries) == 0:
+        return {}
 
-                elif isinstance(result[key], tuple) and value not in result[key]:
-                    result[key] = result[key] + (value,)
+    if len(_dictionaries) == 1:
+        return _dictionaries[0]
 
-                elif value != result[key]:
-                    result[key] = [result[key], value]
+    result: dict = {}
+
+    for _dict in _dictionaries:
+        for key, value in _dict.items():
+            if key in result:
+                if isinstance(result[key], list):
+                    if isinstance(value, list):
+                        result[key].extend(value)
+                    else:
+                        result[key].append(value)
+                else:
+                    if isinstance(value, list):
+                        result[key] = [result[key], *value]
+                    else:
+                        result[key] = [result[key], value]
             else:
                 result[key] = value
 
     return result
 
 
 def raise_for_status(response: requests.Response) -> None:
@@ -439,59 +534,37 @@
     # Support ',' character in timestamp's milliseconds (used in SubRip format).
     timestamp = timestamp.replace(',', '.')
 
     start_time, end_time = timestamp.split(" --> ")
     return dt.time.fromisoformat(start_time), dt.time.fromisoformat(end_time)
 
 
+@lru_cache
 def standardize_title(title: str) -> str:
     """
     Format movie title to a standardized title that can be used as a file name.
 
     Args:
         title (str): A movie title.
 
     Returns:
         str: The movie title, in a file-name-friendly format.
     """
-    windows_reserved_file_names = ("CON", "PRN", "AUX", "NUL", "COM1", "COM2", "COM3", "COM4",
-                                   "COM5", "COM6", "COM7", "COM8", "COM9", "LPT1", "LPT2",
-                                   "LPT3", "LPT4", "LPT5", "LPT6", "LPT7", "LPT8", "LPT9")
-
     title = title.strip()
 
-    # Replacements will be done in the same order of this list
-    replacement_pairs = [
-        (': ', '.'),
-        (':', '.'),
-        (' - ', '-'),
-        (', ', '.'),
-        ('. ', '.'),
-        (' ', '.'),
-        ('|', '.'),
-        ('/', '.'),
-        ('<', ''),
-        ('>', ''),
-        ('(', ''),
-        (')', ''),
-        ('"', ''),
-        ('?', ''),
-        ('*', ''),
-    ]
-
-    for pair in replacement_pairs:
-        title = title.replace(pair[0], pair[1])
+    for string, replacement_string in TITLE_REPLACEMENT_STRINGS.items():
+        title = title.replace(string, replacement_string)
 
     title = re.sub(r"\.+", ".", title)  # Replace multiple dots with a single dot
 
     # If running on Windows, rename Windows reserved names to allow file creation
     if sys.platform == 'win32':
         split_title = title.split('.')
 
-        if split_title[0].upper() in windows_reserved_file_names:
+        if split_title[0].upper() in WINDOWS_RESERVED_FILE_NAMES:
             if len(split_title) > 1:
                 return split_title[0] + split_title[1] + '.'.join(split_title[2:])
 
             if len(split_title) == 1:
                 return "_" + title
 
     return title
```

### Comparing `isubrip-2.5.2/LICENSE` & `isubrip-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.2/pyproject.toml` & `isubrip-2.5.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# --- Poetry ---
 [tool.poetry]
 name = "isubrip"
-version = "2.5.2"
+version = "2.5.3"
 description = "A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages."
 license = "MIT"
 authors = ["Michael Yochpaz"]
 readme = "README.md"
 homepage = "https://github.com/MichaelYochpaz/iSubRip"
 repository = "https://github.com/MichaelYochpaz/iSubRip"
 keywords = [
@@ -27,14 +26,15 @@
     "Operating System :: POSIX :: Linux",
     "Topic :: Utilities",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "isubrip" },
 ]
 include = [
     "isubrip/resources", "README.md", "LICENSE"
 ]
@@ -51,36 +51,44 @@
 
 [tool.poetry.urls]
 "Bug Reports" = "https://github.com/MichaelYochpaz/iSubRip/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
-aiohttp = "^3.9.1"
-m3u8 = "^4.0.0"
+httpx = {extras = ["http2"], version = "^0.27.0"}
+m3u8 = "^4.1.0"
 mergedeep = "^1.3.4"
-pydantic = "^2.5.2"
+pydantic = "^2.6.4"
 tomli = "^2.0.1"
 
+
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.9.0"
+ruff = "^0.3.5"
+types-requests = "^2.31.0.20240406"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry_bumpversion.file."isubrip/constants.py"]
 search = 'PACKAGE_VERSION = "{current_version}"'
 replace = 'PACKAGE_VERSION = "{new_version}"'
 
 [tool.poetry_bumpversion.file."README.md"]
 search = 'Latest version: {current_version}'
 replace = 'Latest version: {new_version}'
 
-# --- Ruff ---
+
 [tool.ruff]
 line-length = 120
 target-version = "py38"
+
+[tool.ruff.lint]
 select = [
     "ARG",
     "ASYNC",
     "B",
     "C4",
     "COM",
     "E",
@@ -90,41 +98,43 @@
     "INP",
     "ISC",
     "N",
     "PIE",
     "PGH",
     "PT",
     "PTH",
-    "Q002",
-    "Q003",
+    "Q",
     "RSE",
     "RET",
     "RUF",
     "S",
     "SIM",
     "SLF",
     "T20",
     "TCH",
     "TID",
     "TRY",
-#    "UP",
+    "UP",
 ]
 ignore = [
     "C416",
+    "Q000",
     "RUF010",
     "RUF012",
     "SIM108",
     "TD002",
     "TD003",
     "TRY003",
-#    "UP015",
 ]
 unfixable = ["ARG"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-sort-within-sections = true
+
+[tool.ruff.lint.pyupgrade]
+keep-runtime-typing = true
```

### Comparing `isubrip-2.5.2/README.md` & `isubrip-2.5.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.5.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.5.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
@@ -61,15 +61,15 @@
 convert-to-srt = true
 fix-rtl = true
 
 [subtitles.webvtt]
 subrip-alignment-conversion = true
 ```
 
-A complete config with all the available options and explanations for each configuration can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml).
+An example config with details and explanations for all available settings can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml).
 
 ## Logs
 A log file, containing debug information, will be created for each run on one of the following paths (according to OS):
 
 **Windows**: `%USERPROFILE%\.isubrip\logs`  
 **Linux / macOS**: `$HOME/.isubrip/logs`
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # iSubRip A Python package for scraping and downloading subtitles from AppleTV
-/ iTunes movie pages. Latest version: 2.5.2 ([changelog](https://github.com/
+/ iTunes movie pages. Latest version: 2.5.3 ([changelog](https://github.com/
 MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
@@ -22,16 +22,16 @@
 features. A config file will be looked for in one of the following paths
 (according to OS): **Windows**: `%USERPROFILE%\.isubrip\config.toml` **Linux /
 macOS**: `$HOME/.isubrip/config.toml` ### Examples: **Windows**: `C:
 \Users\Michael\.isubrip\config.toml` **Linux**: `/home/Michael/.isubrip/
 config.toml` **macOS**: `/Users/Michael/.isubrip/config.toml` --- ### Example
 Config: ```toml [downloads] folder = "C:\\Subtitles\\iTunes" languages = ["en-
 US", "fr-FR", "he"] zip = false [subtitles] convert-to-srt = true fix-rtl =
-true [subtitles.webvtt] subrip-alignment-conversion = true ``` A complete
-config with all the available options and explanations for each configuration
-can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/
-config.toml). ## Logs A log file, containing debug information, will be created
-for each run on one of the following paths (according to OS): **Windows**:
+true [subtitles.webvtt] subrip-alignment-conversion = true ``` An example
+config with details and explanations for all available settings can be found
+[here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml). ##
+Logs A log file, containing debug information, will be created for each run on
+one of the following paths (according to OS): **Windows**:
 `%USERPROFILE%\.isubrip\logs` **Linux / macOS**: `$HOME/.isubrip/logs` Log
 rotation (deletion of old files, once a certain amount of files is reached) can
 be configured in the config file using the `general.log-rotation-size` setting.
 The default log rotation value is `15`.
```

### Comparing `isubrip-2.5.2/PKG-INFO` & `isubrip-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.5.2
+Version: 2.5.3
 Summary: A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 License: MIT
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
 Author: Michael Yochpaz
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,28 +15,29 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: m3u8 (>=4.0.0,<5.0.0)
+Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
+Requires-Dist: m3u8 (>=4.1.0,<5.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Repository, https://github.com/MichaelYochpaz/iSubRip
 Description-Content-Type: text/markdown
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.5.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.5.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
@@ -93,15 +94,15 @@
 convert-to-srt = true
 fix-rtl = true
 
 [subtitles.webvtt]
 subrip-alignment-conversion = true
 ```
 
-A complete config with all the available options and explanations for each configuration can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml).
+An example config with details and explanations for all available settings can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml).
 
 ## Logs
 A log file, containing debug information, will be created for each run on one of the following paths (according to OS):
 
 **Windows**: `%USERPROFILE%\.isubrip\logs`  
 **Linux / macOS**: `$HOME/.isubrip/logs`
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.5.2 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.5.3 Summary: A Python package
 for scraping and downloading subtitles from AppleTV / iTunes movie pages. Home-
 page: https://github.com/MichaelYochpaz/iSubRip License: MIT Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Author: Michael
 Yochpaz Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: End Users/Desktop Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS Classifier: Operating System
 :: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Utilities Requires-Dist:
-aiohttp (>=3.9.1,<4.0.0) Requires-Dist: m3u8 (>=4.0.0,<5.0.0) Requires-Dist:
-mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pydantic (>=2.5.2,<3.0.0) Requires-
-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) Project-
-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues Project-URL:
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Utilities Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
+Requires-Dist: m3u8 (>=4.1.0,<5.0.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0) Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) Project-URL: Bug
+Reports, https://github.com/MichaelYochpaz/iSubRip/issues Project-URL:
 Repository, https://github.com/MichaelYochpaz/iSubRip Description-Content-Type:
 text/markdown # iSubRip A Python package for scraping and downloading subtitles
-from AppleTV / iTunes movie pages. Latest version: 2.5.2 ([changelog](https://
+from AppleTV / iTunes movie pages. Latest version: 2.5.3 ([changelog](https://
 github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
@@ -40,16 +41,16 @@
 features. A config file will be looked for in one of the following paths
 (according to OS): **Windows**: `%USERPROFILE%\.isubrip\config.toml` **Linux /
 macOS**: `$HOME/.isubrip/config.toml` ### Examples: **Windows**: `C:
 \Users\Michael\.isubrip\config.toml` **Linux**: `/home/Michael/.isubrip/
 config.toml` **macOS**: `/Users/Michael/.isubrip/config.toml` --- ### Example
 Config: ```toml [downloads] folder = "C:\\Subtitles\\iTunes" languages = ["en-
 US", "fr-FR", "he"] zip = false [subtitles] convert-to-srt = true fix-rtl =
-true [subtitles.webvtt] subrip-alignment-conversion = true ``` A complete
-config with all the available options and explanations for each configuration
-can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/
-config.toml). ## Logs A log file, containing debug information, will be created
-for each run on one of the following paths (according to OS): **Windows**:
+true [subtitles.webvtt] subrip-alignment-conversion = true ``` An example
+config with details and explanations for all available settings can be found
+[here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml). ##
+Logs A log file, containing debug information, will be created for each run on
+one of the following paths (according to OS): **Windows**:
 `%USERPROFILE%\.isubrip\logs` **Linux / macOS**: `$HOME/.isubrip/logs` Log
 rotation (deletion of old files, once a certain amount of files is reached) can
 be configured in the config file using the `general.log-rotation-size` setting.
 The default log rotation value is `15`.
```

