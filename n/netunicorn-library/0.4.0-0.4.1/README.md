# Comparing `tmp/netunicorn-library-0.4.0.tar.gz` & `tmp/netunicorn-library-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-library-0.4.0.tar", last modified: Sat Dec 23 03:43:20 2023, max compression
+gzip compressed data, was "netunicorn-library-0.4.1.tar", last modified: Tue Apr  9 20:56:08 2024, max compression
```

## Comparing `netunicorn-library-0.4.0.tar` & `netunicorn-library-0.4.1.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.859249 netunicorn-library-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-23 03:43:20.859249 netunicorn-library-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 03:43:20.859249 netunicorn-library-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.847249 netunicorn-library-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.843249 netunicorn-library-0.4.0/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.847249 netunicorn-library-0.4.0/src/netunicorn/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.847249 netunicorn-library-0.4.0/src/netunicorn/library/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.847249 netunicorn-library-0.4.0/src/netunicorn/library/pipelines/measurements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/pipelines/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/capture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/capture/tcpdump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/capture/tshark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/letsencrypt/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/letsencrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/letsencrypt/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/cloudflare/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/cloudflare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/cloudflare/speedtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/flent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/iperf3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/ndt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/arp/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/cve202141773/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/heartbleed/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/icmp/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/land/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/land/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/land/landattack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.851249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/log4j/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mail/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/scapy.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/tshark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/zeek.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/tasks_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/upload/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/upload/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/upload/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/utils/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.855249 netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2023-12-23 03:43:12.000000 netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 03:43:20.859249 netunicorn-library-0.4.0/src/netunicorn_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-23 03:43:20.000000 netunicorn-library-0.4.0/src/netunicorn_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2023-12-23 03:43:20.000000 netunicorn-library-0.4.0/src/netunicorn_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 03:43:20.000000 netunicorn-library-0.4.0/src/netunicorn_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-23 03:43:20.000000 netunicorn-library-0.4.0/src/netunicorn_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-23 03:43:20.000000 netunicorn-library-0.4.0/src/netunicorn_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.670771 netunicorn-library-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 20:56:08.670771 netunicorn-library-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:56:08.670771 netunicorn-library-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.654771 netunicorn-library-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.654771 netunicorn-library-0.4.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/pipelines/measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/pipelines/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/capture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/capture/tcpdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/capture/tshark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/letsencrypt/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/letsencrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/letsencrypt/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.658771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/cloudflare/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/cloudflare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/cloudflare/speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/flent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/iperf3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/ndt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/arp/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/cve202141773/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/heartbleed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/icmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/land/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/land/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/land/landattack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/log4j/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.662771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.666771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/scapy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/tshark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/zeek.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.666771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/tasks_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.666771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/upload/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/upload/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.666771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/utils/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.666771 netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-09 20:56:02.000000 netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:56:08.666771 netunicorn-library-0.4.1/src/netunicorn_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 20:56:08.000000 netunicorn-library-0.4.1/src/netunicorn_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-09 20:56:08.000000 netunicorn-library-0.4.1/src/netunicorn_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:56:08.000000 netunicorn-library-0.4.1/src/netunicorn_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 20:56:08.000000 netunicorn-library-0.4.1/src/netunicorn_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 20:56:08.000000 netunicorn-library-0.4.1/src/netunicorn_library.egg-info/top_level.txt
```

### Comparing `netunicorn-library-0.4.0/PKG-INFO` & `netunicorn-library-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-library
-Version: 0.4.0
+Version: 0.4.1
 Summary: netunicorn contrib library
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `netunicorn-library-0.4.0/pyproject.toml` & `netunicorn-library-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-library"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn contrib library"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py` & `netunicorn-library-0.4.1/src/netunicorn/library/pipelines/measurements/ookla_speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/basic.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/basic.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/capture/tcpdump.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/capture/tcpdump.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/capture/tshark.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/capture/tshark.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/flags.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/flags.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/letsencrypt/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/letsencrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/letsencrypt/tasks.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/letsencrypt/tasks.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/cloudflare/speedtest.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/cloudflare/speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/flent.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/flent.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/iperf3.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/iperf3.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/ndt.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/ndt.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/ookla_speedtest.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/ookla_speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/measurements/ping.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/measurements/ping.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/arp/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/land/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/land/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mail/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/scapy.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/scapy.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/preprocessing/zeek.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/preprocessing/zeek.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/__init__.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/qoe_youtube/watcher.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/qoe_youtube/watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/upload/fileio.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/upload/fileio.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/upload/webdav.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/upload/webdav.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/utils/sleep.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py` & `netunicorn-library-0.4.1/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.4.0/src/netunicorn_library.egg-info/PKG-INFO` & `netunicorn-library-0.4.1/src/netunicorn_library.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-library
-Version: 0.4.0
+Version: 0.4.1
 Summary: netunicorn contrib library
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `netunicorn-library-0.4.0/src/netunicorn_library.egg-info/SOURCES.txt` & `netunicorn-library-0.4.1/src/netunicorn_library.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 src/netunicorn/library/tasks/qoe_youtube/__init__.py
 src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
 src/netunicorn/library/tasks/qoe_youtube/watcher.py
 src/netunicorn/library/tasks/upload/__init__.py
 src/netunicorn/library/tasks/upload/fileio.py
 src/netunicorn/library/tasks/upload/webdav.py
 src/netunicorn/library/tasks/utils/__init__.py
+src/netunicorn/library/tasks/utils/network.py
 src/netunicorn/library/tasks/utils/sleep.py
 src/netunicorn/library/tasks/video_watchers/__init__.py
 src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
 src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
 src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
 src/netunicorn_library.egg-info/PKG-INFO
 src/netunicorn_library.egg-info/SOURCES.txt
```

