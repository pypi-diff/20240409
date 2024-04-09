# Comparing `tmp/SdcStatsBot-0.2.1.tar.gz` & `tmp/SdcStatsBot-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SdcStatsBot-0.2.1.tar", last modified: Tue Apr  9 10:02:10 2024, max compression
+gzip compressed data, was "SdcStatsBot-0.2.4.tar", last modified: Tue Apr  9 10:44:21 2024, max compression
```

## Comparing `SdcStatsBot-0.2.1.tar` & `SdcStatsBot-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:10.790381 SdcStatsBot-0.2.1/
--rw-rw-rw-   0        0        0      344 2024-04-09 10:02:10.790381 SdcStatsBot-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:10.725384 SdcStatsBot-0.2.1/SDcStatsBot/
--rw-rw-rw-   0        0        0       26 2024-04-09 09:32:35.000000 SdcStatsBot-0.2.1/SDcStatsBot/__init__.py
--rw-rw-rw-   0        0        0     1395 2024-04-09 09:58:20.000000 SdcStatsBot-0.2.1/SDcStatsBot/client.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:02:10.743881 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 10:02:10.000000 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-09 10:02:10.000000 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:02:10.000000 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-09 10:02:10.000000 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2024-04-09 10:02:10.000000 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 10:02:10.000000 SdcStatsBot-0.2.1/SdcStatsBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:02:10.795379 SdcStatsBot-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      671 2024-04-09 10:01:00.000000 SdcStatsBot-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:44:21.830501 SdcStatsBot-0.2.4/
+-rw-rw-rw-   0        0        0      344 2024-04-09 10:44:21.831506 SdcStatsBot-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 10:44:21.821576 SdcStatsBot-0.2.4/SDcStatsBot/
+-rw-rw-rw-   0        0        0       26 2024-04-09 09:32:35.000000 SdcStatsBot-0.2.4/SDcStatsBot/__init__.py
+-rw-rw-rw-   0        0        0     2072 2024-04-09 10:39:02.000000 SdcStatsBot-0.2.4/SDcStatsBot/client.py
+-rw-rw-rw-   0        0        0       32 2024-04-09 10:30:59.000000 SdcStatsBot-0.2.4/SDcStatsBot/interval.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:44:21.829079 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:44:21.832505 SdcStatsBot-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-04-09 10:44:05.000000 SdcStatsBot-0.2.4/setup.py
```

