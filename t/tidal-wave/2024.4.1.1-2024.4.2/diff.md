# Comparing `tmp/tidal-wave-2024.4.1.1.tar.gz` & `tmp/tidal-wave-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal-wave-2024.4.1.1.tar", last modified: Sun Apr  7 20:08:35 2024, max compression
+gzip compressed data, was "tidal-wave-2024.4.2.tar", last modified: Tue Apr  9 01:03:19 2024, max compression
```

## Comparing `tidal-wave-2024.4.1.1.tar` & `tidal-wave-2024.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40047 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:08:35.060119 tidal-wave-2024.4.1.1/tidal_wave/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/album.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/mix.py
--rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/requesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/tidal_wave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40047 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25953 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:03:19.914816 tidal-wave-2024.4.2/tidal_wave/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/requesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-09 01:02:55.000000 tidal-wave-2024.4.2/tidal_wave/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:03:19.918815 tidal-wave-2024.4.2/tidal_wave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 01:03:19.000000 tidal-wave-2024.4.2/tidal_wave.egg-info/top_level.txt
```

### Comparing `tidal-wave-2024.4.1.1/LICENSE` & `tidal-wave-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/PKG-INFO` & `tidal-wave-2024.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.4.1.1
+Version: 2024.4.2
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -232,14 +232,18 @@
 Requires-Dist: typer==0.12.1
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
+[![GNU/Linux amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml)
+[![macOS amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_x86.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_x86.yml)
+[![macOS aarch64 (Apple Silicon) Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_arm64.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_arm64.yml)
+[![Windows amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-windows.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-windows.yml)
 
 # tidal-wave &#x1F3B6; &#x1F30A;
 Waving at the [TIDAL](https://tidal.com) music service with [Python](https://www.python.org/). Runs on (at least) Windows, macOS, and GNU/Linux.
 
 >  TIDAL is an artist-first, fan-centered music streaming platform that delivers over 100 million songs in HiFi sound quality to the global music community. © 2024 TIDAL Music AS
 
 This project is inspired by [`qobuz-dl`](https://github.com/vitiko98/qobuz-dl), and, particularly, is a continuation of [`Tidal-Media-Downloader`](https://github.com/yaronzz/Tidal-Media-Downloader). **This project is intended for private use only: it is not intended for distribution of copyrighted content**.
@@ -264,20 +268,20 @@
 * Also because of the use of `requests`, very simple [`Cache-Control`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) request caching occurs via `CacheControl`
 
 ## Getting Started
 A [HiFi Plus](https://tidal.com/pricing) account is **required** in order to retrieve HiRes FLAC, Dolby Atmos, and Sony 360 Reality Audio tracks. Simply a [HiFi](https://tidal.com/pricing) plan is sufficient to retrieve in 16-bit, 44.1 kHz (i.e., lossless) or lower quality as well as videos. More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
 
 ### Requirements
  - As resources will be fetched from the World Wide Web, an Internet connection is required
- - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [`pyinstaller`](https://pyinstaller.org/en/stable/)-created [binary for GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_linux), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_macos_arm64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_macos_x86_64) build FFmpeg from source, so separate installation is unnecessary.
+ - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binary for Ubuntu GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_aarch64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_amd64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe) build FFmpeg from source, so separate installation is unnecessary.
    - Static builds of FFmpeg are available from [John Van Sickle](https://www.johnvansickle.com/ffmpeg/) for GNU/Linux, or most package managers feature `ffmpeg`.
    - For macOS, the [FFmpeg download page](http://ffmpeg.org/download.html#build-mac) links to [this download source](https://evermeet.cx/ffmpeg/); or there is always [Homebrew](https://formulae.brew.sh/formula/ffmpeg)
    - For Windows, the [FFmpeg download page](http://ffmpeg.org/download.html#build-windows) lists 2 resources; or [`chocolatey`](https://community.chocolatey.org/packages/ffmpeg) is an option
  - This is a Python package, so **to use it in the default manner** you will need [Python 3](https://www.python.org/downloads/), version 3.8 or newer, on your system.
-   - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); `pyapp`-compiled binaries; and [`pyinstaller`](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, and x86\_64 macOS are provided for download and use that *do not require Python to be installed*
+   - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); and [PyInstaller](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, x86\_64 macOS, and x86\_64 Windows are provided for download and use that *do not require Python to be installed*
  - Only a handful of Python libraries are dependencies:
    - [`backoff`](https://pypi.org/project/backoff/)
    - [`cachecontrol`](https://pypi.org/project/CacheControl/)
    - [`dataclass-wizard`](https://pypi.org/project/dataclass-wizard/)
    - [`ffmpeg-python`](https://pypi.org/project/ffmpeg-python/)
    - [`mutagen`](https://pypi.org/project/mutagen/)
    - [`m3u8`](https://pypi.org/project/m3u8/)
@@ -308,36 +312,22 @@
 ### `pip` Install from the Repository
 Alternatively, you can clone this repository; `cd` into it; and install from there:
 ```bash
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
-$ (.venv) pip install .  # or, pip install .[all]
+$ (.venv) pip install .
 ```
-### `Pyinstaller` executable
-This is the preferred release artifact, compiled with [`pyinstaller`](https://pyinstaller.org). It bundles Python 3.11, FFmpeg 6.1.1, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform (currently, GNU/Linux x86\_64; macOS x86\_64; or macOS arm64), giving it execute permissions, and running it.
+### PyInstaller executable
+These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_linux
-$ chmod +x ./tidal-wave_py311_FFmpeg6.1.1_linux
-# optionally, rename the binary because the name is descriptive, but unwieldy
-$ mv ./tidal-wave_py311_FFmpeg6.1.1_linux ./tidal-wave_linux
-$ ./tidal-wave_linux --help
-```
-### `pyapp` executable
-Download the Rust-compiled binary from [the Releases](https://github.com/ebb-earl-co/tidal-wave/releases/latest), and, on macOS or GNU/Linux, make it executable
-```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311.pyapp
-$ chmod +x ./tidal-wave_py311.pyapp
-$ ./tidal-wave_py311.pyapp --help
-```
-Or, on Windows, once the .exe file is downloaded, you might have to allow a security exception for an unknown developer, then:
-```powershell
-PS > Invoke-WebRequest https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_pyapp.exe
-PS > & "tidal-wave_py311_pyapp.exe" --help
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64
+$ chmod +x ./tidal-wave_ubuntu_amd64
+$ ./tidal-wave_ubuntu_amd64 --help
 ```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
@@ -441,15 +431,15 @@
 (.venv) $ tidal-wave https://listen.tidal.com/playlist/1b418bb8-90a7-4f87-901d-707993838346
 
 $ ls ~/Music/Playlists/New Arrivals [1b418bb8-90a7-4f87-901d-707993838346]/
 '001 - Dance Alone [CD].flac'
 '002 - Kissing Strangers [CD].flac'
 '003 - Sunday Service [CD].flac'
 ```
-If this is not the desired behavior, pass the `--no-flatten` flag. This flag instructs `tidal-wave` to leave the tracks and/or videos in the directory where they would be written if they had been passed to `tidal-wave` independently. E.g.
+If this is not the desired behavior, pass the `--no-flatten` flag. This flag instructs `tidal-wave` to leave the tracks and/or videos in the directory where they would have been written if they had been passed to `tidal-wave` independently. E.g.
 ```bash
 (.venv) $ tidal-wave https://listen.tidal.com/playlist/1b418bb8-90a7-4f87-901d-707993838346 --no-flatten
 
 $ ls ~/Music/
 'Sia/Dance Alone [343225498] [2024]/01 - Dance Alone [CD].flac'
 'USHER/COMING HOME [339249017] [2024]/05 - Kissing Strangers [CD].flac'
 'Latto/Sunday Service [344275657] [2024]/01 - Sunday Service [CD].flac'
```

### Comparing `tidal-wave-2024.4.1.1/README.md` & `tidal-wave-2024.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
+[![GNU/Linux amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml)
+[![macOS amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_x86.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_x86.yml)
+[![macOS aarch64 (Apple Silicon) Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_arm64.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_arm64.yml)
+[![Windows amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-windows.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-windows.yml)
 
 # tidal-wave &#x1F3B6; &#x1F30A;
 Waving at the [TIDAL](https://tidal.com) music service with [Python](https://www.python.org/). Runs on (at least) Windows, macOS, and GNU/Linux.
 
 >  TIDAL is an artist-first, fan-centered music streaming platform that delivers over 100 million songs in HiFi sound quality to the global music community. © 2024 TIDAL Music AS
 
 This project is inspired by [`qobuz-dl`](https://github.com/vitiko98/qobuz-dl), and, particularly, is a continuation of [`Tidal-Media-Downloader`](https://github.com/yaronzz/Tidal-Media-Downloader). **This project is intended for private use only: it is not intended for distribution of copyrighted content**.
@@ -31,20 +35,20 @@
 * Also because of the use of `requests`, very simple [`Cache-Control`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) request caching occurs via `CacheControl`
 
 ## Getting Started
 A [HiFi Plus](https://tidal.com/pricing) account is **required** in order to retrieve HiRes FLAC, Dolby Atmos, and Sony 360 Reality Audio tracks. Simply a [HiFi](https://tidal.com/pricing) plan is sufficient to retrieve in 16-bit, 44.1 kHz (i.e., lossless) or lower quality as well as videos. More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
 
 ### Requirements
  - As resources will be fetched from the World Wide Web, an Internet connection is required
- - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [`pyinstaller`](https://pyinstaller.org/en/stable/)-created [binary for GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_linux), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_macos_arm64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_macos_x86_64) build FFmpeg from source, so separate installation is unnecessary.
+ - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binary for Ubuntu GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_aarch64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_amd64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe) build FFmpeg from source, so separate installation is unnecessary.
    - Static builds of FFmpeg are available from [John Van Sickle](https://www.johnvansickle.com/ffmpeg/) for GNU/Linux, or most package managers feature `ffmpeg`.
    - For macOS, the [FFmpeg download page](http://ffmpeg.org/download.html#build-mac) links to [this download source](https://evermeet.cx/ffmpeg/); or there is always [Homebrew](https://formulae.brew.sh/formula/ffmpeg)
    - For Windows, the [FFmpeg download page](http://ffmpeg.org/download.html#build-windows) lists 2 resources; or [`chocolatey`](https://community.chocolatey.org/packages/ffmpeg) is an option
  - This is a Python package, so **to use it in the default manner** you will need [Python 3](https://www.python.org/downloads/), version 3.8 or newer, on your system.
-   - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); `pyapp`-compiled binaries; and [`pyinstaller`](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, and x86\_64 macOS are provided for download and use that *do not require Python to be installed*
+   - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); and [PyInstaller](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, x86\_64 macOS, and x86\_64 Windows are provided for download and use that *do not require Python to be installed*
  - Only a handful of Python libraries are dependencies:
    - [`backoff`](https://pypi.org/project/backoff/)
    - [`cachecontrol`](https://pypi.org/project/CacheControl/)
    - [`dataclass-wizard`](https://pypi.org/project/dataclass-wizard/)
    - [`ffmpeg-python`](https://pypi.org/project/ffmpeg-python/)
    - [`mutagen`](https://pypi.org/project/mutagen/)
    - [`m3u8`](https://pypi.org/project/m3u8/)
@@ -75,36 +79,22 @@
 ### `pip` Install from the Repository
 Alternatively, you can clone this repository; `cd` into it; and install from there:
 ```bash
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
-$ (.venv) pip install .  # or, pip install .[all]
+$ (.venv) pip install .
 ```
-### `Pyinstaller` executable
-This is the preferred release artifact, compiled with [`pyinstaller`](https://pyinstaller.org). It bundles Python 3.11, FFmpeg 6.1.1, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform (currently, GNU/Linux x86\_64; macOS x86\_64; or macOS arm64), giving it execute permissions, and running it.
+### PyInstaller executable
+These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_linux
-$ chmod +x ./tidal-wave_py311_FFmpeg6.1.1_linux
-# optionally, rename the binary because the name is descriptive, but unwieldy
-$ mv ./tidal-wave_py311_FFmpeg6.1.1_linux ./tidal-wave_linux
-$ ./tidal-wave_linux --help
-```
-### `pyapp` executable
-Download the Rust-compiled binary from [the Releases](https://github.com/ebb-earl-co/tidal-wave/releases/latest), and, on macOS or GNU/Linux, make it executable
-```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311.pyapp
-$ chmod +x ./tidal-wave_py311.pyapp
-$ ./tidal-wave_py311.pyapp --help
-```
-Or, on Windows, once the .exe file is downloaded, you might have to allow a security exception for an unknown developer, then:
-```powershell
-PS > Invoke-WebRequest https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_pyapp.exe
-PS > & "tidal-wave_py311_pyapp.exe" --help
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64
+$ chmod +x ./tidal-wave_ubuntu_amd64
+$ ./tidal-wave_ubuntu_amd64 --help
 ```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
@@ -208,15 +198,15 @@
 (.venv) $ tidal-wave https://listen.tidal.com/playlist/1b418bb8-90a7-4f87-901d-707993838346
 
 $ ls ~/Music/Playlists/New Arrivals [1b418bb8-90a7-4f87-901d-707993838346]/
 '001 - Dance Alone [CD].flac'
 '002 - Kissing Strangers [CD].flac'
 '003 - Sunday Service [CD].flac'
 ```
-If this is not the desired behavior, pass the `--no-flatten` flag. This flag instructs `tidal-wave` to leave the tracks and/or videos in the directory where they would be written if they had been passed to `tidal-wave` independently. E.g.
+If this is not the desired behavior, pass the `--no-flatten` flag. This flag instructs `tidal-wave` to leave the tracks and/or videos in the directory where they would have been written if they had been passed to `tidal-wave` independently. E.g.
 ```bash
 (.venv) $ tidal-wave https://listen.tidal.com/playlist/1b418bb8-90a7-4f87-901d-707993838346 --no-flatten
 
 $ ls ~/Music/
 'Sia/Dance Alone [343225498] [2024]/01 - Dance Alone [CD].flac'
 'USHER/COMING HOME [339249017] [2024]/05 - Kissing Strangers [CD].flac'
 'Latto/Sunday Service [344275657] [2024]/01 - Sunday Service [CD].flac'
```

### Comparing `tidal-wave-2024.4.1.1/pyproject.toml` & `tidal-wave-2024.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 [bdist_wheel]
 universal = 0  # Make the generated wheels have "py3" tag
 [project]
 name = "tidal-wave"
-version = "2024.4.1.1"
+version = "2024.4.2"
 description = "A tool to wave at the TIDAL music service."
 authors = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
 maintainers = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
```

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/album.py` & `tidal-wave-2024.4.2/tidal_wave/album.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/artist.py` & `tidal-wave-2024.4.2/tidal_wave/artist.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/dash.py` & `tidal-wave-2024.4.2/tidal_wave/dash.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/hls.py` & `tidal-wave-2024.4.2/tidal_wave/hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 "M3U8 file"
             )
 
         download_params: Dict[str, None] = {k: None for k in session.params}
         with session.get(url=url, params=download_params) as m3u8_response:
             try:
                 m3u8_response.raise_for_status()
-            except HTTPError as he:
+            except HTTPError:
                 raise TidalM3U8Exception(
                     f"Could not retrieve variant streams from manifest for "
                     f"video {vesrj.video_id}, video mode {vesrj.video_quality}"
                 )
             else:
                 em_three_you_ate: Optional[m3u8.M3U8] = m3u8.M3U8(
                     content=m3u8_response.text
```

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/login.py` & `tidal-wave-2024.4.2/tidal_wave/login.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/main.py` & `tidal-wave-2024.4.2/tidal_wave/main.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/media.py` & `tidal-wave-2024.4.2/tidal_wave/media.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/mix.py` & `tidal-wave-2024.4.2/tidal_wave/mix.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/models.py` & `tidal-wave-2024.4.2/tidal_wave/models.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/oauth.py` & `tidal-wave-2024.4.2/tidal_wave/oauth.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/playlist.py` & `tidal-wave-2024.4.2/tidal_wave/playlist.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/requesting.py` & `tidal-wave-2024.4.2/tidal_wave/requesting.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/track.py` & `tidal-wave-2024.4.2/tidal_wave/track.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/utils.py` & `tidal-wave-2024.4.2/tidal_wave/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,19 +123,19 @@
 
 def is_tidal_api_reachable(hostname: str = "api.tidal.com") -> bool:
     """Using stdlib 'socket' library, test if a few conditions are all
     met: whether the user has a connection to the larger Internet;
     whether the user can resolve the primary URL for this service,
     api.tidal.com, and whether api.tidal.com is responding to requests"""
     try:
-        s = closing(socket.create_connection((hostname, 80)))
+        _ = closing(socket.create_connection((hostname, 80)))
     except ConnectionRefusedError:
         logger.critical("It seems that 'api.tidal.com' is unreachable!")
         return False
-    except socket.gaierror as g:
+    except socket.gaierror:
         logger.critical(
             f"tidal-wave is unable to find the IP address of {hostname}: "
             "Please ensure that Internet connectivity is established, "
             "particularly DNS resolution"
         )
         return False
     except OSError as ose:
```

### Comparing `tidal-wave-2024.4.1.1/tidal_wave/video.py` & `tidal-wave-2024.4.2/tidal_wave/video.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.4.1.1/tidal_wave.egg-info/PKG-INFO` & `tidal-wave-2024.4.2/tidal_wave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.4.1.1
+Version: 2024.4.2
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -232,14 +232,18 @@
 Requires-Dist: typer==0.12.1
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
+[![GNU/Linux amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-linux.yml)
+[![macOS amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_x86.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_x86.yml)
+[![macOS aarch64 (Apple Silicon) Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_arm64.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-macos_arm64.yml)
+[![Windows amd64 Executable](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-windows.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/pyinstaller-windows.yml)
 
 # tidal-wave &#x1F3B6; &#x1F30A;
 Waving at the [TIDAL](https://tidal.com) music service with [Python](https://www.python.org/). Runs on (at least) Windows, macOS, and GNU/Linux.
 
 >  TIDAL is an artist-first, fan-centered music streaming platform that delivers over 100 million songs in HiFi sound quality to the global music community. © 2024 TIDAL Music AS
 
 This project is inspired by [`qobuz-dl`](https://github.com/vitiko98/qobuz-dl), and, particularly, is a continuation of [`Tidal-Media-Downloader`](https://github.com/yaronzz/Tidal-Media-Downloader). **This project is intended for private use only: it is not intended for distribution of copyrighted content**.
@@ -264,20 +268,20 @@
 * Also because of the use of `requests`, very simple [`Cache-Control`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) request caching occurs via `CacheControl`
 
 ## Getting Started
 A [HiFi Plus](https://tidal.com/pricing) account is **required** in order to retrieve HiRes FLAC, Dolby Atmos, and Sony 360 Reality Audio tracks. Simply a [HiFi](https://tidal.com/pricing) plan is sufficient to retrieve in 16-bit, 44.1 kHz (i.e., lossless) or lower quality as well as videos. More information on sound quality at [TIDAL's site here](https://tidal.com/sound-quality).
 
 ### Requirements
  - As resources will be fetched from the World Wide Web, an Internet connection is required
- - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [`pyinstaller`](https://pyinstaller.org/en/stable/)-created [binary for GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_linux), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_macos_arm64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_macos_x86_64) build FFmpeg from source, so separate installation is unnecessary.
+ - The venerable [FFmpeg](http://ffmpeg.org/download.html) is necessary for audio and video data manipulation. This project's [container image](https://github.com/ebb-earl-co/tidal-wave/blob/trunk/Dockerfile) as well as its [PyInstaller](https://pyinstaller.org/en/stable/)-created [binary for Ubuntu GNU/Linux](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64), [binary for Apple Silicon macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_aarch64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_macos_amd64), and [binary for x86\_64 macOS](https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe) build FFmpeg from source, so separate installation is unnecessary.
    - Static builds of FFmpeg are available from [John Van Sickle](https://www.johnvansickle.com/ffmpeg/) for GNU/Linux, or most package managers feature `ffmpeg`.
    - For macOS, the [FFmpeg download page](http://ffmpeg.org/download.html#build-mac) links to [this download source](https://evermeet.cx/ffmpeg/); or there is always [Homebrew](https://formulae.brew.sh/formula/ffmpeg)
    - For Windows, the [FFmpeg download page](http://ffmpeg.org/download.html#build-windows) lists 2 resources; or [`chocolatey`](https://community.chocolatey.org/packages/ffmpeg) is an option
  - This is a Python package, so **to use it in the default manner** you will need [Python 3](https://www.python.org/downloads/), version 3.8 or newer, on your system.
-   - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); `pyapp`-compiled binaries; and [`pyinstaller`](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, and x86\_64 macOS are provided for download and use that *do not require Python to be installed*
+   - *However*, as of December 2023, an [OCI container image](https://github.com/ebb-earl-co/tidal-wave/pkgs/container/tidal-wave); and [PyInstaller](https://pyinstaller.org/en/stable/)-created binaries for x86\_64 GNU/Linux, Apple Silicon macOS, x86\_64 macOS, and x86\_64 Windows are provided for download and use that *do not require Python to be installed*
  - Only a handful of Python libraries are dependencies:
    - [`backoff`](https://pypi.org/project/backoff/)
    - [`cachecontrol`](https://pypi.org/project/CacheControl/)
    - [`dataclass-wizard`](https://pypi.org/project/dataclass-wizard/)
    - [`ffmpeg-python`](https://pypi.org/project/ffmpeg-python/)
    - [`mutagen`](https://pypi.org/project/mutagen/)
    - [`m3u8`](https://pypi.org/project/m3u8/)
@@ -308,36 +312,22 @@
 ### `pip` Install from the Repository
 Alternatively, you can clone this repository; `cd` into it; and install from there:
 ```bash
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
-$ (.venv) pip install .  # or, pip install .[all]
+$ (.venv) pip install .
 ```
-### `Pyinstaller` executable
-This is the preferred release artifact, compiled with [`pyinstaller`](https://pyinstaller.org). It bundles Python 3.11, FFmpeg 6.1.1, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform (currently, GNU/Linux x86\_64; macOS x86\_64; or macOS arm64), giving it execute permissions, and running it.
+### PyInstaller executable
+These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_FFmpeg6.1.1_linux
-$ chmod +x ./tidal-wave_py311_FFmpeg6.1.1_linux
-# optionally, rename the binary because the name is descriptive, but unwieldy
-$ mv ./tidal-wave_py311_FFmpeg6.1.1_linux ./tidal-wave_linux
-$ ./tidal-wave_linux --help
-```
-### `pyapp` executable
-Download the Rust-compiled binary from [the Releases](https://github.com/ebb-earl-co/tidal-wave/releases/latest), and, on macOS or GNU/Linux, make it executable
-```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311.pyapp
-$ chmod +x ./tidal-wave_py311.pyapp
-$ ./tidal-wave_py311.pyapp --help
-```
-Or, on Windows, once the .exe file is downloaded, you might have to allow a security exception for an unknown developer, then:
-```powershell
-PS > Invoke-WebRequest https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_py311_pyapp.exe
-PS > & "tidal-wave_py311_pyapp.exe" --help
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_amd64
+$ chmod +x ./tidal-wave_ubuntu_amd64
+$ ./tidal-wave_ubuntu_amd64 --help
 ```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
@@ -441,15 +431,15 @@
 (.venv) $ tidal-wave https://listen.tidal.com/playlist/1b418bb8-90a7-4f87-901d-707993838346
 
 $ ls ~/Music/Playlists/New Arrivals [1b418bb8-90a7-4f87-901d-707993838346]/
 '001 - Dance Alone [CD].flac'
 '002 - Kissing Strangers [CD].flac'
 '003 - Sunday Service [CD].flac'
 ```
-If this is not the desired behavior, pass the `--no-flatten` flag. This flag instructs `tidal-wave` to leave the tracks and/or videos in the directory where they would be written if they had been passed to `tidal-wave` independently. E.g.
+If this is not the desired behavior, pass the `--no-flatten` flag. This flag instructs `tidal-wave` to leave the tracks and/or videos in the directory where they would have been written if they had been passed to `tidal-wave` independently. E.g.
 ```bash
 (.venv) $ tidal-wave https://listen.tidal.com/playlist/1b418bb8-90a7-4f87-901d-707993838346 --no-flatten
 
 $ ls ~/Music/
 'Sia/Dance Alone [343225498] [2024]/01 - Dance Alone [CD].flac'
 'USHER/COMING HOME [339249017] [2024]/05 - Kissing Strangers [CD].flac'
 'Latto/Sunday Service [344275657] [2024]/01 - Sunday Service [CD].flac'
```

### Comparing `tidal-wave-2024.4.1.1/tidal_wave.egg-info/SOURCES.txt` & `tidal-wave-2024.4.2/tidal_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

