# Comparing `tmp/github_random_star-0.0.4.tar.gz` & `tmp/github_random_star-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_random_star-0.0.4.tar", max compression
+gzip compressed data, was "github_random_star-0.0.5.tar", max compression
```

## Comparing `github_random_star-0.0.4.tar` & `github_random_star-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1060 2024-02-24 14:08:01.013688 github_random_star-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     1927 2024-02-24 14:08:01.013688 github_random_star-0.0.4/README.md
--rw-r--r--   0        0        0      170 2024-02-24 14:08:01.013688 github_random_star-0.0.4/github_random_star/__init__.py
--rw-r--r--   0        0        0     5432 2024-02-24 14:08:01.013688 github_random_star-0.0.4/github_random_star/main.py
--rw-r--r--   0        0        0     1276 2024-02-24 14:08:01.013688 github_random_star-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 github_random_star-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-09 18:59:32.347862 github_random_star-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     2075 2024-04-09 18:59:32.347862 github_random_star-0.0.5/README.md
+-rw-r--r--   0        0        0      170 2024-04-09 18:59:32.347862 github_random_star-0.0.5/github_random_star/__init__.py
+-rw-r--r--   0        0        0     6916 2024-04-09 18:59:32.347862 github_random_star-0.0.5/github_random_star/main.py
+-rw-r--r--   0        0        0     1289 2024-04-09 18:59:32.347862 github_random_star-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 github_random_star-0.0.5/PKG-INFO
```

### Comparing `github_random_star-0.0.4/LICENSE.md` & `github_random_star-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `github_random_star-0.0.4/README.md` & `github_random_star-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,43 +14,39 @@
 
 ## Other
 
 Either install from [pypi](https://pypi.org/project/github-random-star) with `pip` or clone this repository and install requirements through [poetry](pyproject.toml) or the provided [requirements](requirements.txt) file.
 
 <details>
     <summary>If using poetry.</summary>
-    <code>
-    $ poetry shell<br>
-    $ poetry install
-    </code>
+    <code>$ poetry shell</code><br>
+    <code>$ poetry install</code>
 </details>
 <details>
     <summary> If using requirements.txt.</summary>
-    <code>
-    $ virtualenv -p python3.12 .venv<br>
-    $ source .venv/bin/activate<br>
-    $ pip install -r requirements.txt
-    </code>
+    <code>$ virtualenv -p python3.12 .venv</code><br>
+    <code>$ source .venv/bin/activate</code><br>
+    <code>$ pip install -r requirements.txt</code>
 </details>
 
 # Usage
 
 1. Setup GitHub API token as the `GITHUB_ACCESS_TOKEN` environment variable. _If this is not setup it will use the public access point with lower rates._
 2. Run the script through `gh-star <flags>`, `python github_random_star/main.py <flags>` or if using poetry `poetry run gh-star <flags>`
 
 ## Flags
 
-- `-a, --account` Username of the github account to retrieve the starred items from. `--account` is required or `GITHUB_ACCOUNT` environment variable needs to be set.
+- `-a, --account` Username of the GitHub account to retrieve the starred items from. `--account` is required or `GH_STAR_ACCOUNT` environment variable needs to be set.
 - `-t, --total` Total amount of random items to pick from. Defaults to 3.
-- `-r, --refresh` Whether to fetch new cached data or not. Will refetch all starred items.
-- `-m, --max-history` The amount of historic choices to cache. Defaults to 100.
+- `-r, --refresh` Whether to fetch new cached data or not. Will re fetch all starred items instead of using cache.
+- `-m, --max-history` The amount of historic choices to cache. Defaults to 100. Set to -1 to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable can be used to override this value.
 - `-i, --ignore` If to use a list of repositories to ignore. Defaults to true.
 
 ## Examples
 
-- `gh-star -a <username>`
-- `gh-star -a <username> -t 5`
-- `gh-star -a <username> -r -t 5`
+- `gh-star -a ddkasa`
+- `gh-star -a ddkasa -t 5`
+- `gh-star -a ddkasa -r -t 5`
 
 # License
 
 MIT. Look at the [LICENSE](LICENSE.md) for details.
```

### Comparing `github_random_star-0.0.4/github_random_star/main.py` & `github_random_star-0.0.5/github_random_star/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import json
 import logging as log
 import os
 import random
-import webbrowser
+import subprocess
 from datetime import datetime
-from functools import partial
 from pathlib import Path
-from threading import Timer
 from typing import NamedTuple, Optional
-import atexit
 
-import fire  # type: ignore [import-not-found]
-import httpx  # type: ignore [import-not-found]
+import fire
+import httpx
 
 USER_API_URL = "https://api.github.com/users/{user}/starred?page={page}&per_page=30"
 
 if os.name != "nt":
     CACHE_PATH = Path.home() / Path(".cache")
 else:
     env = os.getenv("APPDATA")
     if isinstance(env, str):
         CACHE_PATH = Path(env)
     else:
         CACHE_PATH = Path.home()
 
 CACHE_PATH = CACHE_PATH / Path("github_random_star/")
 
-
 CACHE_PATH.mkdir(parents=True, exist_ok=True)
 CACHE_FILE = CACHE_PATH / Path("cache.json")
 
 SELECTION_CACHE = CACHE_PATH / Path("selections.json")
 
 IGNORE_FILE = CACHE_PATH / Path("ignore.json")
 
@@ -41,15 +37,27 @@
 
 class StarredItem(NamedTuple):
     repo_id: int
     name: str
     url: str
 
 
-def retrieve_cache(account: str, refresh: bool) -> set[StarredItem]:
+def retrieve_cache(account: str, refresh: bool = False) -> set[StarredItem]:
+    """Retrieves data for choosing a random starred item from GitHub.
+
+    Args:
+        account: Github account the starred items will be retrieved from.
+        refresh: Weither or not to refresh the cache. Defaults to False.
+
+    Raises:
+        ConnectionError: If the outgoing request was not successful.
+
+    Returns:
+        set(StarredItem): Set of starred items from GitHub.
+    """
     if CACHE_FILE.exists() and not refresh:
         with CACHE_FILE.open("r", encoding="utf-8") as file:
             cache_data = json.load(file)
 
         log.info(
             "Cache last refreshed on the %s.",
             datetime.fromisoformat(cache_data["date"]).date().isoformat(),
@@ -100,14 +108,23 @@
         }
         json.dump(container, file)
 
     return data
 
 
 def extract_selection(path: Path) -> list[StarredItem]:
+    """Extracts selections from a JSON file.
+
+    Args:
+        path: Path to the JSON file.
+
+    Returns:
+        list(StarredItem): List of starred items from the JSON file. Needs to
+            stay a list in order to preserve order when keeping history.
+    """
     data = []
     if path.exists():
         with path.open("r", encoding="utf-8") as file:
             selections = json.load(file)
 
         data = [StarredItem(*item) for item in selections]
 
@@ -116,17 +133,29 @@
 
 def item_selection(
     starred_items: set[StarredItem],
     total: int,
     max_history: int = 100,
     ignore: bool = True,
 ) -> None:
-    selections = extract_selection(SELECTION_CACHE)
+    """Selection function where the user chooses a random starred item.
 
-    starred_items = starred_items - starred_items.intersection(selections)
+    Args:
+        starred_items: Set of starred items from GitHub.
+        total: Total of choices the user can pick from.
+        max_history: Maximum amount of items to keep in history.
+            Defaults to 100. Set to 0 to disable history or -1 to keep all.
+        ignore: Whether or not to ignore previously selected items.
+            Defaults to True.
+    """
+    og_len = len(starred_items)
+
+    if max_history != -1:
+        selections = extract_selection(SELECTION_CACHE)
+        starred_items = starred_items - starred_items.intersection(selections)
 
     if IGNORE_FILE.exists():
         if ignore:
             ignore_list = extract_selection(IGNORE_FILE)
             starred_items = starred_items - starred_items.intersection(ignore_list)
     else:
         with IGNORE_FILE.open("w", encoding="utf-8") as file:
@@ -151,43 +180,57 @@
 
         print(f"Select an item within the range of 1 and {total}")
 
     selected_item = StarredItem(*items[selection - 1])
 
     log.info("Opening %s", selected_item.url)
 
-    t = Timer(1, partial(webbrowser.get().open, selected_item.url))
-    atexit.register(t.cancel)
-    t.start()
+    subprocess.run(
+        ["python", "-m", "webbrowser", "-t", selected_item.url],
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+    )
 
     selections.insert(0, selected_item)
-    if len(selections) > max_history:
+    if len(selections) > max_history and max_history > 0:
         selections = selections[: -(len(selections) - max_history)]
 
+    if og_len == len(starred_items) and max_history == -1:
+        selections = []
+
     with SELECTION_CACHE.open("w", encoding="utf-8") as file:
         json.dump(selections, file)
 
 
 def main(
     account: Optional[str] = None,
     total: int = 3,
     refresh: bool = False,
-    max_history: int = 100,
+    max_history: Optional[int] = None,
     ignore: bool = True,
 ) -> None:
+    """Basic entrypoint for the CLI script.
+
+    Raises:
+        AccountMissingError: If the GitHub account was not provided through
+            flags or an environment variables.
+    """
     log.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
         level=log.INFO,
     )
 
     if account is None:
-        account = os.environ.get("GITHUB_ACCOUNT")
+        account = os.environ.get("GH_STAR_ACCOUNT")
         if account is None:
             raise AccountMissingError()
 
+    if max_history is None:
+        max_history = int(os.environ.get("GH_STAR_MAX_HISTORY", 100))
+
     starred_items = retrieve_cache(account, refresh)
 
     log.info("Total amount of starred items: %s", len(starred_items))
 
     item_selection(starred_items, total, max_history, ignore)
 
     log.info("Done!")
```

### Comparing `github_random_star-0.0.4/pyproject.toml` & `github_random_star-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "github-random-star"
-version = "0.0.4"
+version = "0.0.5"
 description = "Simple CLI tool to fetch a random starred items from a users GitHub profile."
 authors = ["David Kasakaitis <davidkasakaitis@proton.me>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "Topic :: Utilities",   
     "License :: OSI Approved :: MIT License",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Natural Language :: English",
     "Typing :: Typed",
     "Topic :: Software Development :: Version Control :: Git"
```

### Comparing `github_random_star-0.0.4/PKG-INFO` & `github_random_star-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: github-random-star
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple CLI tool to fetch a random starred items from a users GitHub profile.
 License: MIT
 Keywords: python,python3,cli,github,git
 Author: David Kasakaitis
 Author-email: davidkasakaitis@proton.me
 Requires-Python: >=3.12,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -42,44 +42,40 @@
 
 ## Other
 
 Either install from [pypi](https://pypi.org/project/github-random-star) with `pip` or clone this repository and install requirements through [poetry](pyproject.toml) or the provided [requirements](requirements.txt) file.
 
 <details>
     <summary>If using poetry.</summary>
-    <code>
-    $ poetry shell<br>
-    $ poetry install
-    </code>
+    <code>$ poetry shell</code><br>
+    <code>$ poetry install</code>
 </details>
 <details>
     <summary> If using requirements.txt.</summary>
-    <code>
-    $ virtualenv -p python3.12 .venv<br>
-    $ source .venv/bin/activate<br>
-    $ pip install -r requirements.txt
-    </code>
+    <code>$ virtualenv -p python3.12 .venv</code><br>
+    <code>$ source .venv/bin/activate</code><br>
+    <code>$ pip install -r requirements.txt</code>
 </details>
 
 # Usage
 
 1. Setup GitHub API token as the `GITHUB_ACCESS_TOKEN` environment variable. _If this is not setup it will use the public access point with lower rates._
 2. Run the script through `gh-star <flags>`, `python github_random_star/main.py <flags>` or if using poetry `poetry run gh-star <flags>`
 
 ## Flags
 
-- `-a, --account` Username of the github account to retrieve the starred items from. `--account` is required or `GITHUB_ACCOUNT` environment variable needs to be set.
+- `-a, --account` Username of the GitHub account to retrieve the starred items from. `--account` is required or `GH_STAR_ACCOUNT` environment variable needs to be set.
 - `-t, --total` Total amount of random items to pick from. Defaults to 3.
-- `-r, --refresh` Whether to fetch new cached data or not. Will refetch all starred items.
-- `-m, --max-history` The amount of historic choices to cache. Defaults to 100.
+- `-r, --refresh` Whether to fetch new cached data or not. Will re fetch all starred items instead of using cache.
+- `-m, --max-history` The amount of historic choices to cache. Defaults to 100. Set to -1 to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable can be used to override this value.
 - `-i, --ignore` If to use a list of repositories to ignore. Defaults to true.
 
 ## Examples
 
-- `gh-star -a <username>`
-- `gh-star -a <username> -t 5`
-- `gh-star -a <username> -r -t 5`
+- `gh-star -a ddkasa`
+- `gh-star -a ddkasa -t 5`
+- `gh-star -a ddkasa -r -t 5`
 
 # License
 
 MIT. Look at the [LICENSE](LICENSE.md) for details.
```

