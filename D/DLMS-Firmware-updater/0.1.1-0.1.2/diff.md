# Comparing `tmp/DLMS_Firmware_updater-0.1.1.tar.gz` & `tmp/DLMS_Firmware_updater-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_Firmware_updater-0.1.1.tar", last modified: Mon Apr  8 13:06:36 2024, max compression
+gzip compressed data, was "DLMS_Firmware_updater-0.1.2.tar", last modified: Tue Apr  9 05:35:59 2024, max compression
```

## Comparing `DLMS_Firmware_updater-0.1.1.tar` & `DLMS_Firmware_updater-0.1.2.tar`

### file list

```diff
@@ -1,288 +1,156 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.842413 DLMS_Firmware_updater-0.1.1/
--rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      569 2024-04-08 13:06:36.841413 DLMS_Firmware_updater-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.1.1/README.md
--rw-rw-rw-   0        0        0     1115 2024-04-08 13:06:32.000000 DLMS_Firmware_updater-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 13:06:36.842413 DLMS_Firmware_updater-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.226420 DLMS_Firmware_updater-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.250412 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.252413 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Firmwares/
--rw-rw-rw-   0        0        0  2737171 2024-01-16 06:35:27.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Firmwares/firmwares.dat
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.185310 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.181316 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.303445 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/
--rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.14.typ
--rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.16.typ
--rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.26.typ
--rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.39.typ
--rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.43.typ
--rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.45.typ
--rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.46.typ
--rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.48.typ
--rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.49.typ
--rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.53.typ
--rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.54.typ
--rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.1.0.typ
--rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.2.0.typ
--rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.0.typ
--rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.30.typ
--rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.7.typ
--rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.9.typ
--rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.4.0.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.182309 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.345411 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/
--rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.20.typ
--rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.26.typ
--rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.39.typ
--rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.41.typ
--rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.43.typ
--rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.45.typ
--rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.48.typ
--rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.49.typ
--rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.53.typ
--rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.1.0.typ
--rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.2.0.typ
--rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.0.typ
--rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.30.typ
--rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.5.typ
--rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.7.typ
--rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.183308 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.384413 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/
--rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.16.typ
--rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.26.typ
--rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.39.typ
--rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.43.typ
--rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.45.typ
--rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.48.typ
--rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.49.typ
--rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.1.0.typ
--rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.2.0.typ
--rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.0.typ
--rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.30.typ
--rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.7.typ
--rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.184308 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.420415 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/
--rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.20.typ
--rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.26.typ
--rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.39.typ
--rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.43.typ
--rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.45.typ
--rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.48.typ
--rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.49.typ
--rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.1.0.typ
--rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.2.0.typ
--rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.0.typ
--rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.30.typ
--rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.7.typ
--rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.225414 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.443413 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.0.typ
--rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.15.typ
--rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.16.typ
--rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.17.typ
--rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.5.0.typ
--rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.5.3.typ
--rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.5.7.typ
--rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.6.1.typ
--rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.467442 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.0.typ
--rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.10.typ
--rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.12.typ
--rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.15.typ
--rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.16.typ
--rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.17.typ
--rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.5.0.typ
--rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.5.7.typ
--rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.485414 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.0.typ
--rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.15.typ
--rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.16.typ
--rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.17.typ
--rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.5.0.typ
--rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.5.7.typ
--rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.504443 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.0.typ
--rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.15.typ
--rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.16.typ
--rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.17.typ
--rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.5.0.typ
--rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.5.7.typ
--rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.526413 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.0.typ
--rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.12.typ
--rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.15.typ
--rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.16.typ
--rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.17.typ
--rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.5.0.typ
--rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.5.7.typ
--rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.6.2.typ
--rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/__init__.py
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/config.toml
--rw-rw-rw-   0        0        0     2987 2024-04-08 08:43:51.000000 DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.538414 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/
--rw-rw-rw-   0        0        0      569 2024-04-08 13:06:35.000000 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12355 2024-04-08 13:06:36.000000 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:06:35.000000 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-08 13:06:35.000000 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-04-08 13:06:35.000000 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-08 13:06:35.000000 DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.545414 DLMS_Firmware_updater-0.1.1/test/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.547413 DLMS_Firmware_updater-0.1.1/test/Firmwares/
--rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.1.1/test/Firmwares/firmwares.dat
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.233446 DLMS_Firmware_updater-0.1.1/test/Types/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.229414 DLMS_Firmware_updater-0.1.1/test/Types/101/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.595413 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/
--rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.14.typ
--rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.16.typ
--rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.26.typ
--rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.39.typ
--rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.43.typ
--rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.45.typ
--rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.46.typ
--rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.48.typ
--rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.49.typ
--rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.53.typ
--rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/0.0.54.typ
--rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.1.0.typ
--rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.2.0.typ
--rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.3.0.typ
--rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.3.30.typ
--rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.3.7.typ
--rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.3.9.typ
--rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.4.0.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.230412 DLMS_Firmware_updater-0.1.1/test/Types/102/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.640414 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/
--rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.20.typ
--rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.26.typ
--rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.39.typ
--rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.41.typ
--rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.43.typ
--rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.45.typ
--rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.48.typ
--rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.49.typ
--rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/0.0.53.typ
--rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.1.0.typ
--rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.2.0.typ
--rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.3.0.typ
--rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.3.30.typ
--rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.3.5.typ
--rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.3.7.typ
--rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/102/09054d324d5f33/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.231413 DLMS_Firmware_updater-0.1.1/test/Types/103/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.676412 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/
--rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.16.typ
--rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.26.typ
--rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.39.typ
--rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.43.typ
--rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.45.typ
--rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.48.typ
--rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.49.typ
--rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.1.0.typ
--rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.2.0.typ
--rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.3.0.typ
--rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.3.30.typ
--rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.3.7.typ
--rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/103/09064d324d5f3153/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.232412 DLMS_Firmware_updater-0.1.1/test/Types/104/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.716413 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/
--rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.20.typ
--rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.26.typ
--rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.39.typ
--rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.43.typ
--rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.45.typ
--rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.48.typ
--rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.49.typ
--rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.1.0.typ
--rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.2.0.typ
--rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.3.0.typ
--rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.3.30.typ
--rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.3.7.typ
--rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/104/09064d324d5f3353/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.719413 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.743413 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ
--rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ
--rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ
--rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ
--rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ
--rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ
--rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ
--rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ
--rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.769414 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ
--rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ
--rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ
--rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ
--rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ
--rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ
--rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ
--rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ
--rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.790414 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
--rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
--rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
--rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
--rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
--rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
--rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.816413 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
--rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
--rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
--rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
--rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
--rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
--rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-08 13:06:36.839414 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
--rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
--rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
--rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
--rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
--rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
--rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
--rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.1/test/Types/KPZ/image_transfer_1.typ
--rw-rw-rw-   0        0        0    24980 2024-04-05 12:32:20.000000 DLMS_Firmware_updater-0.1.1/test/client_log.txt
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.1.1/test/config.toml
--rw-rw-rw-   0        0        0      129 2024-04-08 11:48:52.000000 DLMS_Firmware_updater-0.1.1/test/test_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.494382 DLMS_Firmware_updater-0.1.2/
+-rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      569 2024-04-09 05:35:59.494382 DLMS_Firmware_updater-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1115 2024-04-09 05:35:54.000000 DLMS_Firmware_updater-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:35:59.494382 DLMS_Firmware_updater-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.100016 DLMS_Firmware_updater-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.165417 DLMS_Firmware_updater-0.1.2/src/DLMSFirmwareUpdater/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.1.2/src/DLMSFirmwareUpdater/__init__.py
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.1.2/src/DLMSFirmwareUpdater/config.toml
+-rw-rw-rw-   0        0        0     2968 2024-04-09 05:14:35.000000 DLMS_Firmware_updater-0.1.2/src/DLMSFirmwareUpdater/main.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.181384 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-04-09 05:35:58.000000 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5345 2024-04-09 05:35:59.000000 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:35:58.000000 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-09 05:35:58.000000 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-04-09 05:35:58.000000 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 05:35:58.000000 DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.192384 DLMS_Firmware_updater-0.1.2/test/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.195385 DLMS_Firmware_updater-0.1.2/test/Firmwares/
+-rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.1.2/test/Firmwares/firmwares.dat
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.108013 DLMS_Firmware_updater-0.1.2/test/Types/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.104047 DLMS_Firmware_updater-0.1.2/test/Types/101/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.252386 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/
+-rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.14.typ
+-rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.16.typ
+-rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.26.typ
+-rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.39.typ
+-rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.43.typ
+-rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.45.typ
+-rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.46.typ
+-rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.48.typ
+-rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.49.typ
+-rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.53.typ
+-rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.54.typ
+-rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.1.0.typ
+-rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.2.0.typ
+-rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.0.typ
+-rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.30.typ
+-rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.7.typ
+-rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.9.typ
+-rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.4.0.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.105016 DLMS_Firmware_updater-0.1.2/test/Types/102/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.297383 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/
+-rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.20.typ
+-rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.26.typ
+-rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.39.typ
+-rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.41.typ
+-rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.43.typ
+-rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.45.typ
+-rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.48.typ
+-rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.49.typ
+-rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.53.typ
+-rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.1.0.typ
+-rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.2.0.typ
+-rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.0.typ
+-rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.30.typ
+-rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.5.typ
+-rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.7.typ
+-rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.106047 DLMS_Firmware_updater-0.1.2/test/Types/103/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.336382 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/
+-rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.16.typ
+-rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.26.typ
+-rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.39.typ
+-rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.43.typ
+-rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.45.typ
+-rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.48.typ
+-rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.49.typ
+-rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.1.0.typ
+-rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.2.0.typ
+-rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.0.typ
+-rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.30.typ
+-rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.7.typ
+-rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.107015 DLMS_Firmware_updater-0.1.2/test/Types/104/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.378383 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/
+-rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.20.typ
+-rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.26.typ
+-rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.39.typ
+-rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.43.typ
+-rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.45.typ
+-rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.48.typ
+-rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.49.typ
+-rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.1.0.typ
+-rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.2.0.typ
+-rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.0.typ
+-rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.30.typ
+-rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.7.typ
+-rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.380383 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.405383 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.0.typ
+-rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.15.typ
+-rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.16.typ
+-rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.17.typ
+-rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.5.0.typ
+-rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.5.3.typ
+-rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.5.7.typ
+-rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.6.1.typ
+-rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.429383 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.0.typ
+-rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.10.typ
+-rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.12.typ
+-rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.15.typ
+-rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.16.typ
+-rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.17.typ
+-rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.5.0.typ
+-rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.5.7.typ
+-rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.450383 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
+-rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
+-rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
+-rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
+-rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
+-rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
+-rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.470383 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
+-rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
+-rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
+-rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
+-rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
+-rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
+-rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:59.491382 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
+-rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
+-rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
+-rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
+-rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
+-rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
+-rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
+-rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.2/test/Types/KPZ/image_transfer_1.typ
+-rw-rw-rw-   0        0        0    24980 2024-04-05 12:32:20.000000 DLMS_Firmware_updater-0.1.2/test/client_log.txt
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.1.2/test/config.toml
+-rw-rw-rw-   0        0        0      129 2024-04-08 11:48:52.000000 DLMS_Firmware_updater-0.1.2/test/test_updater.py
```

### Comparing `DLMS_Firmware_updater-0.1.1/PKG-INFO` & `DLMS_Firmware_updater-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_Firmware_updater
-Version: 0.1.1
+Version: 0.1.2
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.1.1/pyproject.toml` & `DLMS_Firmware_updater-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [tool.setuptools.package-data]
 DLMSFirmwareUpdater = ["*.toml", "*.dat", "*.typ"]
 #exclude = ["test*", "dummy"]  # alternatively: `exclude = ["additional*"]`
 #namespaces = false
 
 [project]
 name = "DLMS_Firmware_updater"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS_SPODES_client == 0.7.2",
     "pyinstaller >= 6.2",
     "build >= 1.2.1"
```

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.14.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.14.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.26.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.39.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.43.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.45.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.46.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.46.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.48.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.49.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.53.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/0.0.54.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/0.0.54.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.1.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.1.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.2.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.2.5.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.30.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.3.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/101/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/101/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.20.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.26.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.39.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.41.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.41.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.43.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.45.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.48.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.49.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/0.0.53.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.1.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.1.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.2.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.2.5.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.30.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.5.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/102/09054d324d5f33/1.3.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/102/09054d324d5f33/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.26.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.39.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.43.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.45.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.48.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.49.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/0.0.53.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.1.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.1.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.2.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.2.5.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.30.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/103/09064d324d5f3153/1.3.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/103/09064d324d5f3153/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.20.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.26.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.39.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.43.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.45.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.48.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.49.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/0.0.53.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.1.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.1.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.2.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.2.5.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.30.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/104/09064d324d5f3353/1.3.9.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/104/09064d324d5f3353/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.15.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.17.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.4.22.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.5.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.5.3.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.5.3.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.5.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.6.1.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.6.1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f31/1.6.2.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f31/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.10.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.10.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.12.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.15.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.17.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.4.22.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.5.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.5.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09054d324d5f33/1.6.2.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09054d324d5f33/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.15.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.17.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.4.22.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.5.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.5.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3153/1.6.2.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3153/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.15.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.17.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.4.22.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.5.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.5.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3353/1.6.2.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3353/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.12.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.15.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.16.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.17.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.4.22.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.5.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.5.7.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/Types/KPZ/09064d324d5f3354/1.6.2.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/09064d324d5f3354/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/config.toml` & `DLMS_Firmware_updater-0.1.2/src/DLMSFirmwareUpdater/config.toml`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMSFirmwareUpdater/main.py` & `DLMS_Firmware_updater-0.1.2/src/DLMSFirmwareUpdater/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,12 +89,12 @@
         while results:
             time.sleep(3)
             for res in results:
                 res: Result
                 if res.complete:
                     results.remove(res)
                     c.log(logL.INFO, F"Для {res.client} обновление: {'Удачно' if res.value else 'Неудачно'}")
-                    file.write(F"{res.client} {'OK' if res.value else 'NOK'}")
+                    file.write(F"{res.client} {res.value}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DLMS_Firmware_updater-0.1.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO` & `DLMS_Firmware_updater-0.1.2/src/DLMS_Firmware_updater.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-Firmware-updater
-Version: 0.1.1
+Version: 0.1.2
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.1.1/test/Firmwares/firmwares.dat` & `DLMS_Firmware_updater-0.1.2/test/Firmwares/firmwares.dat`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/test/Types/101/09054d324d5f31/1.1.0.typ` & `DLMS_Firmware_updater-0.1.2/test/Types/KPZ/image_transfer_1.typ`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 <?xml version="1.0" encoding="cp1251"?>
 <Objects version="3.0.0">
   <dlms_ver>6</dlms_ver>
   <country>7</country>
   <country_ver>3.0</country_ver>
-  <manufacturer>101</manufacturer>
-  <server_ver>1.1.0</server_ver>
+  <manufacturer>KPZ</manufacturer>
   <object name="Ñîåäèíåíèå òèïà &quot;Êîíôèãóðàòîð&quot;" ln="0.0.40.0.3.255">
-    <version>1</version>
     <class_id>15</class_id>
     <!--Ñïèñîê îáúåêòîâ: Ñòðóêòóðà[16]-->
     <attribute index="2">0110020412000f110109060000280000ff0202010902030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f0716030002030f0816030002030f09160300010402020f01160102020f02160102020f03160102020f0416010204120017110109060000160000ff0202010902030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f0716030002030f0816030002030f0916030001000204120017110109060001160000ff0202010902030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f0716030002030f0816030002030f0916030001000204120017110109060002160000ff0202010902030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f0716030002030f0816030002030f09160300010002041200011100090600002a0000ff0202010202030f0116010002030f0216030001000204120001110009060000600100ff0202010202030f0116010002030f0216030001000204120001110009060000600102ff0202010202030f0116010002030f0216030001000204120001110009060000600106ff0202010202030f0116010002030f0216030001000204120001110009060000600103ff0202010202030f0116010002030f0216030001000204120001110009060000600101ff0202010202030f0116010002030f0216030001000204120001110009060000806400ff0202010202030f0116010002030f021603000100020412002d110009060000190400ff0202010402030f0116010002030f0216030002030f0316030002030f041603000100020412002f110109060000190600ff0202010802030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f0716030002030f081603000100020412000f110109060000280003ff0202010902030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f0716030002030f0816030002030f09160300010402020f01160102020f02160102020f03160102020f04160102041200121100090600002c0000ff0202010702030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f07160300010402020f01160102020f02160102020f03160102020f04160102041200121100090600002c0080ff0202010702030f0116010002030f0216030002030f0316030002030f0416030002030f0516030002030f0616030002030f07160300010402020f01160102020f02160102020f03160102020f041601</attribute>
     <!--Èäåíòèôèêàòîð ïàðòíåðà: {Êîíôèãóðàòîð, 1}-->
     <attribute index="3">02020f30120001</attribute>
     <!--Èìÿ êîíòåêñòà ïðèëîæåíèÿ: {2, 16, 756, 5, 8, 1, 1}-->
     <attribute index="4">090760857405080101</attribute>
```

### Comparing `DLMS_Firmware_updater-0.1.1/test/client_log.txt` & `DLMS_Firmware_updater-0.1.2/test/client_log.txt`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.1/test/config.toml` & `DLMS_Firmware_updater-0.1.2/test/config.toml`

 * *Files identical despite different names*

