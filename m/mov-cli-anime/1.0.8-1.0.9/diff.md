# Comparing `tmp/mov-cli-anime-1.0.8.tar.gz` & `tmp/mov-cli-anime-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-anime-1.0.8.tar", last modified: Sat Mar 23 16:14:07 2024, max compression
+gzip compressed data, was "mov-cli-anime-1.0.9.tar", last modified: Mon Apr  8 22:04:12 2024, max compression
```

## Comparing `mov-cli-anime-1.0.8.tar` & `mov-cli-anime-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-23 16:14:07.934745 mov-cli-anime-1.0.8/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:26:30.000000 mov-cli-anime-1.0.8/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2883 2024-03-23 16:14:07.934745 mov-cli-anime-1.0.8/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      568 2024-03-14 17:40:35.000000 mov-cli-anime-1.0.8/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-23 16:14:07.931411 mov-cli-anime-1.0.8/mov_cli_anime/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      323 2024-03-23 16:13:58.000000 mov-cli-anime-1.0.8/mov_cli_anime/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-23 16:14:07.931411 mov-cli-anime-1.0.8/mov_cli_anime/anitaku/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 mov-cli-anime-1.0.8/mov_cli_anime/anitaku/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5227 2024-03-23 16:13:13.000000 mov-cli-anime-1.0.8/mov_cli_anime/anitaku/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-23 16:14:07.931411 mov-cli-anime-1.0.8/mov_cli_anime.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2883 2024-03-23 16:14:07.000000 mov-cli-anime-1.0.8/mov_cli_anime.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-03-23 16:14:07.000000 mov-cli-anime-1.0.8/mov_cli_anime.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-03-23 16:14:07.000000 mov-cli-anime-1.0.8/mov_cli_anime.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-03-23 16:14:07.000000 mov-cli-anime-1.0.8/mov_cli_anime.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-03-23 16:14:07.000000 mov-cli-anime-1.0.8/mov_cli_anime.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1325 2024-03-14 20:31:24.000000 mov-cli-anime-1.0.8/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-03-23 16:14:07.934745 mov-cli-anime-1.0.8/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.857237 mov-cli-anime-1.0.9/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:26:30.000000 mov-cli-anime-1.0.9/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-04-08 22:01:37.000000 mov-cli-anime-1.0.9/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/mov_cli_anime/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      323 2024-04-08 22:03:38.000000 mov-cli-anime-1.0.9/mov_cli_anime/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/mov_cli_anime/anitaku/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 mov-cli-anime-1.0.9/mov_cli_anime/anitaku/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5244 2024-04-08 22:02:12.000000 mov-cli-anime-1.0.9/mov_cli_anime/anitaku/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1324 2024-03-23 21:13:23.000000 mov-cli-anime-1.0.9/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-08 22:04:12.857237 mov-cli-anime-1.0.9/setup.cfg
```

### Comparing `mov-cli-anime-1.0.8/LICENSE` & `mov-cli-anime-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-anime-1.0.8/PKG-INFO` & `mov-cli-anime-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-anime
-Version: 1.0.8
+Version: 1.0.9
 Summary: A mov-cli v4 plugin for watching anime.
 Author-email: Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,30 +37,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.0.3
+Requires-Dist: mov-cli>=4.1.6
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-anime
   <sub>A mov-cli v4 plugin for watching anime.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
 
 </div>
 
-> [!Warning]
-> Currently work in progress.
+> [!NOTE]
+> Searching for maintainers
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-anime
```

### Comparing `mov-cli-anime-1.0.8/README.md` & `mov-cli-anime-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
   # mov-cli-anime
   <sub>A mov-cli v4 plugin for watching anime.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
 
 </div>
 
-> [!Warning]
-> Currently work in progress.
+> [!NOTE]
+> Searching for maintainers
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-anime
```

### Comparing `mov-cli-anime-1.0.8/mov_cli_anime/anitaku/scraper.py` & `mov-cli-anime-1.0.9/mov_cli_anime/anitaku/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 from mov_cli import Series, Movie, Metadata, MetadataType
 from mov_cli import ExtraMetadata
 
 __all__ = ("AnitakuScraper",)
 
 class AnitakuScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient) -> None:
-        self.base_url = "https://anitaku.to"
+        self.base_url = "https://anitaku.so"
         super().__init__(config, http_client)
 
     def search(self, query: str, limit: int = 20) -> List[Metadata]:
         query = query.replace(' ', '-')
         results = self.__results(query, limit)
         return results
 
     def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] = None, **kwargs) -> Series | Movie:
         if episode is None:
             episode = utils.EpisodeSelector()
 
-        req = self.http_client.get(self.base_url + f"/{metadata.id}-episode-{episode.episode}")
+        req = self.http_client.get(self.base_url + f"/{metadata.id}-episode-{episode.episode}", redirect = True)
         soup = self.soup(req)
 
         streamwish = soup.find("li", {"class": "streamwish"})
         dood = soup.find("li", {"class": "doodstream"})
 
         if streamwish:
             url = self.__streamwish(streamwish.find("a")["data-video"])
```

### Comparing `mov-cli-anime-1.0.8/mov_cli_anime.egg-info/PKG-INFO` & `mov-cli-anime-1.0.9/mov_cli_anime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-anime
-Version: 1.0.8
+Version: 1.0.9
 Summary: A mov-cli v4 plugin for watching anime.
 Author-email: Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,30 +37,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.0.3
+Requires-Dist: mov-cli>=4.1.6
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-anime
   <sub>A mov-cli v4 plugin for watching anime.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
 
 </div>
 
-> [!Warning]
-> Currently work in progress.
+> [!NOTE]
+> Searching for maintainers
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-anime
```

### Comparing `mov-cli-anime-1.0.8/pyproject.toml` & `mov-cli-anime-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'Programming Language :: Python :: 3.10',
 	'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     "requests",
     "importlib-metadata; python_version<'3.8'",
 
-    "mov-cli>=4.0.3"
+    "mov-cli>=4.1.6"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
@@ -44,8 +44,8 @@
 version = { attr = "mov_cli_anime.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["mov_cli_anime*"]
+include = ["mov_cli_anime*"]
```

