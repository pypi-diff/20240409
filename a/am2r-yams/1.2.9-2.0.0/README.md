# Comparing `tmp/am2r_yams-1.2.9.tar.gz` & `tmp/am2r_yams-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "am2r_yams-1.2.9.tar", last modified: Sun Jan 28 20:09:22 2024, max compression
+gzip compressed data, was "am2r_yams-2.0.0.tar", last modified: Tue Apr  9 18:54:00 2024, max compression
```

## Comparing `am2r_yams-1.2.9.tar` & `am2r_yams-2.0.0.tar`

### file list

```diff
@@ -1,1020 +1,1097 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.605903 am2r_yams-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-28 20:09:22.605903 am2r_yams-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.441902 am2r_yams-1.2.9/am2r_yams/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.445902 am2r_yams-1.2.9/am2r_yams/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/__pyinstaller/hook-am2r_yams.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.453902 am2r_yams-1.2.9/am2r_yams/yams/
--rwxr--r--   0 runner    (1001) docker     (127)   204800 2021-09-19 09:20:24.000000 am2r_yams-1.2.9/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
--rwxr--r--   0 runner    (1001) docker     (127)    42496 2022-06-15 03:36:02.000000 am2r_yams-1.2.9/am2r_yams/yams/Macross.Json.Extensions.dll
--rwxr--r--   0 runner    (1001) docker     (127)    27528 2020-10-19 18:40:26.000000 am2r_yams-1.2.9/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (127)     6656 2023-12-07 09:32:36.000000 am2r_yams-1.2.9/am2r_yams/yams/NaturalSort.Extension.dll
--rwxr--r--   0 runner    (1001) docker     (127)     6656 2021-03-13 10:51:42.000000 am2r_yams-1.2.9/am2r_yams/yams/PropertyChanged.dll
--rwxr--r--   0 runner    (1001) docker     (127)  2087936 2024-01-01 03:46:38.000000 am2r_yams-1.2.9/am2r_yams/yams/SixLabors.ImageSharp.dll
--rwxr--r--   0 runner    (1001) docker     (127)   173432 2021-10-22 20:57:42.000000 am2r_yams-1.2.9/am2r_yams/yams/System.Drawing.Common.dll
--rw-r--r--   0 runner    (1001) docker     (127)   947200 2024-01-28 20:09:14.000000 am2r_yams-1.2.9/am2r_yams/yams/UndertaleModLib.dll
--rw-r--r--   0 runner    (1001) docker     (127)   330863 2024-01-28 20:09:13.000000 am2r_yams-1.2.9/am2r_yams/yams/UndertaleModLib.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-01-28 20:09:16.000000 am2r_yams-1.2.9/am2r_yams/yams/YAMS-LIB.deps.json
--rw-r--r--   0 runner    (1001) docker     (127)   276480 2024-01-28 20:09:16.000000 am2r_yams-1.2.9/am2r_yams/yams/YAMS-LIB.dll
--rw-r--r--   0 runner    (1001) docker     (127)    27932 2024-01-28 20:09:16.000000 am2r_yams-1.2.9/am2r_yams/yams/YAMS-LIB.pdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.429902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.429902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.429902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.453902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (127)   419720 2021-10-22 20:57:34.000000 am2r_yams-1.2.9/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.429902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.429902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.453902 am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (127)    52104 2020-10-19 18:52:12.000000 am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (127)   436600 2021-10-22 20:58:02.000000 am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.453902 am2r_yams-1.2.9/am2r_yams/yams/sprites/
--rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/Attribution.md
--rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/LICENSE-GRAPHICS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.461902 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearBulletHell.png
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearPipeHub.png
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearSave.png
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearTotem.png
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPRightExterior.png
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPRobotHome.png
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorArachnus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorBlue.png
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorBomb.png
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorGenesis.png
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorGuardian.png
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorLocked.png
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorMissile.png
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorPBomb.png
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorQueen.png
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorScrew.png
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSerris.png
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSpider.png
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSuper.png
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTempLocked.png
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTester.png
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTorizo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.429902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.461902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.461902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.465902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.465902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.465902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.469902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.473902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.473902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.473902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.477902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.477902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.477902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveJump/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.477902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.481902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.481902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.481902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.481902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.485902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.485902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.485902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_8.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.485902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.489902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.489902 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.493902 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.493902 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.493902 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIMissileNormal.png
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIMissileNormalGreen.png
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIMissileSelected.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIPBombNormal.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIPBombNormalGreen.png
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIPBombSelected.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUISMissileNormal.png
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUISMissileNormalGreen.png
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUISMissileSelected.png
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newA4Doors.png
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newA4Doors2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.497902 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/sDisconnected.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/sMapHint.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.497902 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/skippy_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadP.png
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadPClaw.png
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadPFang.png
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpHideout.png
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.497902 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.433902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.433902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.497902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.497902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/default/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/default/sItemRDV_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/default/sItemRDV_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/default/sItemRDV_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/default/sItemRDV_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.433902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.501902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.501902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.501902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/energyPart/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.505902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.505902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.509902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.509902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.513902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.513902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.513902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spaceJump/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.517902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.521902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.525902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.525902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.529902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/wideBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.437902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.437902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.529902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.529902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.529902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.533902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.533902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.537902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.537902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.537902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.537902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.541902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.545902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.545902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.545902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.545902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.549902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.549902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.549902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.553902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.553902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.557902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.557902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.557902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.561902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.561902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.561902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.565902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.441902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.565902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.565902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.565902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.569902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.569902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.569902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.569902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.569902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.573902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.573902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.573902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.573902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.577902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.577902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.581902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_21.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_22.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_23.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.581902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.581902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.581902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.585903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.585903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.589902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.589902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.593902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.593902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.593902 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.597903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.597903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.597903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.597903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.601903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.601903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.601903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.605903 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.605903 am2r_yams-1.2.9/am2r_yams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    70566 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-28 20:09:22.000000 am2r_yams-1.2.9/am2r_yams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:09:22.605903 am2r_yams-1.2.9/am2r_yams_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/am2r_yams_tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-28 20:08:58.000000 am2r_yams-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-28 20:09:22.605903 am2r_yams-1.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.391579 am2r_yams-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 18:54:00.391579 am2r_yams-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.203578 am2r_yams-2.0.0/am2r_yams/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.203578 am2r_yams-2.0.0/am2r_yams/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/__pyinstaller/hook-am2r_yams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/
+-rwxr--r--   0 runner    (1001) docker     (127)   204800 2021-09-19 09:20:24.000000 am2r_yams-2.0.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    42496 2022-06-15 03:36:02.000000 am2r_yams-2.0.0/am2r_yams/yams/Macross.Json.Extensions.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    27528 2020-10-19 18:40:26.000000 am2r_yams-2.0.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (127)     6656 2023-12-07 09:32:36.000000 am2r_yams-2.0.0/am2r_yams/yams/NaturalSort.Extension.dll
+-rwxr--r--   0 runner    (1001) docker     (127)     6656 2021-03-13 10:51:42.000000 am2r_yams-2.0.0/am2r_yams/yams/PropertyChanged.dll
+-rwxr--r--   0 runner    (1001) docker     (127)  2088448 2024-03-05 05:20:28.000000 am2r_yams-2.0.0/am2r_yams/yams/SixLabors.ImageSharp.dll
+-rwxr--r--   0 runner    (1001) docker     (127)   173432 2021-10-22 20:57:42.000000 am2r_yams-2.0.0/am2r_yams/yams/System.Drawing.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   947200 2024-04-09 18:53:54.000000 am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   330863 2024-04-09 18:53:53.000000 am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-09 18:53:57.000000 am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.deps.json
+-rw-r--r--   0 runner    (1001) docker     (127)   278016 2024-04-09 18:53:57.000000 am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    28044 2024-04-09 18:53:57.000000 am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.pdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (127)   419720 2021-10-22 20:57:34.000000 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (127)    52104 2020-10-19 18:52:12.000000 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (127)   436600 2021-10-22 20:58:02.000000 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/sprites/
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/Attribution.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/LICENSE-GRAPHICS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.223578 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearBulletHell.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearPipeHub.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearSave.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearTotem.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPRightExterior.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPRobotHome.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorArachnus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorBlue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorBomb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorGenesis.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorGuardian.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorLocked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorMissile.png
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorQueen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorScrew.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSerris.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSpider.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSuper.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTempLocked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTester.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTorizo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.191578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.227578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.227578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.227578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.231578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.231578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.231578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.235578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.235578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.235578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.239578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.239578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.239578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.243578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.243578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.251578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_8.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.251578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.255578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.255578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.255578 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.259579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.259579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileNormal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileNormalGreen.png
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileSelected.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombNormal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombNormalGreen.png
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombSelected.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileNormal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileNormalGreen.png
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileSelected.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newA4Doors.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newA4Doors2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/sDisconnected.png
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/sMapHint.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadP.png
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadPClaw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadPFang.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpHideout.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.195578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.191578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.195578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.271579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.271579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.275579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.275579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.279579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.283579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.283579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.287579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.287579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.287579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.291579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.295579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_17.png
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_18.png
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.299579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_17.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_18.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_20.png
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.299579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_17.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_18.png
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_20.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.303579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.303579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_8.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.199578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.199578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.311579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.311579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.315579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.315579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.315579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.319579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_17.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_18.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_20.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_21.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_22.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_23.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.323579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.323579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.327579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.327579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.327579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.331579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.331579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.331579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.335579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.335579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.339579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.339579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.339579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.343579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.203578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.363579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_17.png
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_18.png
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_20.png
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_21.png
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_22.png
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_23.png
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.367579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.367579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.367579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.371579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.371579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.371579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.375579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_7.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.383579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.383579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.383579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_11.png
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_13.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_9.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_4.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_6.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    76644 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:53:59.000000 am2r_yams-2.0.0/am2r_yams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams_tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 18:54:00.391579 am2r_yams-2.0.0/setup.cfg
```

### Comparing `am2r_yams-1.2.9/PKG-INFO` & `am2r_yams-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 1.2.9
+Version: 2.0.0
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `am2r_yams-1.2.9/README.md` & `am2r_yams-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/wrapper.py` & `am2r_yams-2.0.0/am2r_yams/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         # Patch data.win
         progress_update("Patching data file...", 0.6)
         self.csharp_patcher.Main(input_data_win, output_data_win, json_file)
 
         # Move temp dir to output dir and get rid of it. Also delete original data.win
         # Also delete the json if we're on a race seed.
-        if patch_data.get("configuration_identifier", {}).get("contains_spoiler", False):
+        if not patch_data.get("configuration_identifier", {}).get("contains_spoiler", False):
             input_data_win_path.parent.joinpath("yams-data.json").unlink()
         input_data_win_path.unlink()
         progress_update("Moving to output directory...", 0.8)
         shutil.copytree(tempdir.name, output_path, dirs_exist_ok=True)
         shutil.rmtree(tempdir.name)
 
         progress_update("Exporting finished!", 1)
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/ICSharpCode.SharpZipLib.dll` & `am2r_yams-2.0.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/Macross.Json.Extensions.dll` & `am2r_yams-2.0.0/am2r_yams/yams/Macross.Json.Extensions.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-2.0.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/NaturalSort.Extension.dll` & `am2r_yams-2.0.0/am2r_yams/yams/NaturalSort.Extension.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/PropertyChanged.dll` & `am2r_yams-2.0.0/am2r_yams/yams/PropertyChanged.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/SixLabors.ImageSharp.dll` & `am2r_yams-2.0.0/am2r_yams/yams/SixLabors.ImageSharp.dll`

 * *Files 18% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xc84bc16f
+	             Time stamp: 0xf9e6da3b
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x001fd200
+	              Code Size: 0x001fd400
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x001f78a6
+	        Entry Point RVA: 0x001f79d2
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00200000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -29,94 +29,94 @@
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x00204000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x001fefd2
+	            Checksum (0): 0x0020bfa2
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x001f7853 [0x0000004f]
+	     Import Table: 0x001f797f [0x0000004f]
 	   Resource Table: 0x00200000 [0x000004b8]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x00202000 [0x0000000c]
-	            Debug: 0x001f7778 [0x00000054]
+	            Debug: 0x001f78a4 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x001fd1e0
+	   Virtual Size: 0x001fd308
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x001fd200
+	  Raw Data Size: 0x001fd400
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x000004b8
 	Virtual Address: 0x00200000
 	  Raw Data Size: 0x00000600
-	   Raw Data Ptr: 0x001fd400
+	   Raw Data Ptr: 0x001fd600
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x00202000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x001fda00
+	   Raw Data Ptr: 0x001fdc00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x000d5834 [0x00121ec4]
+	         Metadata: 0x000d5840 [0x00121fe4]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
-	   Strong Name at: 0x001f76f8 [0x00000080]
+	   Strong Name at: 0x001f7824 [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 34 A7 B6 3B 51 04 0B BE 26 5A 41 A6 C4 65 6C 74
-	 34 31 B2 EB 2C 34 0C AB 84 FC BD C5 1C D7 28 DC
-	 38 76 E7 12 E0 E2 B0 11 07 B5 F2 FA 79 2B 91 1A
-	 03 23 52 FE 3F 56 02 AD 75 7F 87 F1 39 68 9A 26
-	 04 31 F9 FC E5 5F C8 16 9C A5 0A 99 50 A7 50 0B
-	 06 BE 74 86 64 DA 24 32 2A 21 A5 17 78 D4 10 8A
-	 06 EF 45 DE 92 83 3E 3C EB 47 A9 7C 24 D5 EE E0
-	 E7 80 DE 49 CA E8 B9 BF 56 12 D0 65 8A 17 23 83
+	 E9 2D D9 38 5C 7F 4F AA 4C 8F 45 5B E7 4A 38 3F
+	 7E 47 C5 E2 1D BB 99 89 30 1E BD 10 6C FD 5F F3
+	 DD C8 BD 14 CC E9 57 DD F0 40 3B 24 CE ED 0F 42
+	 F2 92 65 0A 89 46 28 53 9B 0D BE E6 07 63 2E 93
+	 7C B4 E1 D3 40 43 90 87 46 71 3C 4B AC A5 B5 46
+	 9B 07 E6 D3 AC AE 93 03 EE 09 14 4F 84 55 FB 96
+	 14 68 47 5D 7E BF FA EB FF D9 58 F0 E2 0E EF EA
+	 73 CD B1 5E 66 2D 14 F7 F3 CE DF 35 12 1F 73 82
 
 Public key:
 	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
 	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
 	 01 47 E6 FE 67 66 71 5E EC 6C FE D6 1F 1E 7D CD
 	 BF 69 74 8A 3E 35 5C 67 E9 D8 DF D9 53 AC AB 1D
 	 5E 01 2B A3 4B 23 30 81 66 FD C6 1E E1 D0 39 0D
@@ -127,41 +127,41 @@
 	 4B 0E 9A 51 71 E6 BB 13 84 B6 D2 F7 D5 4D FA 97
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x000be390 [779044 == 0x000be324]
-	    Strings: 0x000be390 - 0x000f0460 [205008 == 0x000320d0]
-	       Blob: 0x000fb960 - 0x00121ec4 [157028 == 0x00026564]
-	User string: 0x000f0460 - 0x000fb950 [46320 == 0x0000b4f0]
-	       GUID: 0x000fb950 - 0x000fb960 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x000be420 [779188 == 0x000be3b4]
+	    Strings: 0x000be420 - 0x000f0594 [205172 == 0x00032174]
+	       Blob: 0x000fba94 - 0x00121fe4 [157008 == 0x00026550]
+	User string: 0x000f0594 - 0x000fba84 [46320 == 0x0000b4f0]
+	       GUID: 0x000fba84 - 0x000fba94 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at d3b28)
-Table TypeRef: 256 records (10 bytes, at d3b34)
-Table TypeDef: 1591 records (18 bytes, at d4534)
-Table Field: 6611 records (10 bytes, at db512)
-Table Method: 12250 records (18 bytes, at eb750)
-Table Param: 17803 records (8 bytes, at 1214a4)
-Table InterfaceImpl: 611 records (4 bytes, at 1440fc)
-Table MemberRef: 4302 records (12 bytes, at 144a88)
-Table Constant: 2187 records (10 bytes, at 151430)
-Table CustomAttribute: 12265 records (12 bytes, at 15699e)
-Table DeclSecurity: 1 records (8 bytes, at 17a88a)
-Table ClassLayout: 80 records (8 bytes, at 17a892)
-Table FieldLayoutt: 49 records (6 bytes, at 17ab12)
-Table StandaloneSig: 2103 records (4 bytes, at 17ac38)
-Table EventMap: 1 records (4 bytes, at 17cd14)
-Table Event: 3 records (8 bytes, at 17cd18)
-Table PropertyMap: 702 records (4 bytes, at 17cd30)
-Table Property: 2358 records (10 bytes, at 17d828)
-Table MethodSemantics: 3023 records (6 bytes, at 183444)
-Table MethodImpl: 102 records (6 bytes, at 187b1e)
-Table TypeSpec: 1297 records (4 bytes, at 187d82)
-Table FieldRVA: 348 records (6 bytes, at 1891c6)
-Table Assembly: 1 records (28 bytes, at 1899ee)
-Table AssemblyRef: 16 records (28 bytes, at 189a0a)
-Table NestedClass: 465 records (4 bytes, at 189bca)
-Table GenericParam: 1102 records (10 bytes, at 18a30e)
-Table MethodSpec: 2077 records (6 bytes, at 18ce1a)
-Table GenericParamConstraint: 1982 records (4 bytes, at 18fec8)
+Table Module: 1 records (12 bytes, at d3b34)
+Table TypeRef: 256 records (10 bytes, at d3b40)
+Table TypeDef: 1591 records (18 bytes, at d4540)
+Table Field: 6613 records (10 bytes, at db51e)
+Table Method: 12252 records (18 bytes, at eb770)
+Table Param: 17805 records (8 bytes, at 1214e8)
+Table InterfaceImpl: 611 records (4 bytes, at 144150)
+Table MemberRef: 4304 records (12 bytes, at 144adc)
+Table Constant: 2187 records (10 bytes, at 15149c)
+Table CustomAttribute: 12268 records (12 bytes, at 156a0a)
+Table DeclSecurity: 1 records (8 bytes, at 17a91a)
+Table ClassLayout: 80 records (8 bytes, at 17a922)
+Table FieldLayoutt: 49 records (6 bytes, at 17aba2)
+Table StandaloneSig: 2102 records (4 bytes, at 17acc8)
+Table EventMap: 1 records (4 bytes, at 17cda0)
+Table Event: 3 records (8 bytes, at 17cda4)
+Table PropertyMap: 702 records (4 bytes, at 17cdbc)
+Table Property: 2359 records (10 bytes, at 17d8b4)
+Table MethodSemantics: 3025 records (6 bytes, at 1834da)
+Table MethodImpl: 102 records (6 bytes, at 187bc0)
+Table TypeSpec: 1297 records (4 bytes, at 187e24)
+Table FieldRVA: 348 records (6 bytes, at 189268)
+Table Assembly: 1 records (28 bytes, at 189a90)
+Table AssemblyRef: 16 records (28 bytes, at 189aac)
+Table NestedClass: 465 records (4 bytes, at 189c6c)
+Table GenericParam: 1102 records (10 bytes, at 18a3b0)
+Table MethodSpec: 2076 records (6 bytes, at 18cebc)
+Table GenericParamConstraint: 1982 records (4 bytes, at 18ff64)
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/System.Drawing.Common.dll` & `am2r_yams-2.0.0/am2r_yams/yams/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/UndertaleModLib.dll` & `am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.dll`

 * *Files 6% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xe268f1a6
+	             Time stamp: 0xd06ab7c2
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2102
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x000e6c00
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x000e8b2e
+	        Entry Point RVA: 0x000e8ade
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00000000
 
 
 NT Header:
 	   Image Base (0x400000): 0x00400000
 	Section Alignment (8192): 0x00002000
@@ -41,31 +41,31 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000e8ad4 [0x00000057]
+	     Import Table: 0x000e8a8c [0x0000004f]
 	   Resource Table: 0x000ea000 [0x000003b4]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x000ec000 [0x0000000c]
-	            Debug: 0x000d1ea0 [0x00000054]
+	            Debug: 0x000d1e54 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000e6b34
+	   Virtual Size: 0x000e6ae4
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x000e6c00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
@@ -92,58 +92,58 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0005bfe0 [0x00075ec0]
+	         Metadata: 0x0005bf94 [0x00075ec0]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0005bbe4 [0x00000018]
+	     Resources at: 0x0005bb98 [0x00000018]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x0002ae80 [175636 == 0x0002ae14]
-	    Strings: 0x0002ae80 - 0x0003b5dc [67420 == 0x0001075c]
-	       Blob: 0x0006e484 - 0x00075ec0 [31292 == 0x00007a3c]
-	User string: 0x0003b5dc - 0x0006e474 [208536 == 0x00032e98]
-	       GUID: 0x0006e474 - 0x0006e484 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x0002ae88 [175644 == 0x0002ae1c]
+	    Strings: 0x0002ae88 - 0x0003b5e4 [67420 == 0x0001075c]
+	       Blob: 0x0006e48c - 0x00075ec0 [31284 == 0x00007a34]
+	User string: 0x0003b5e4 - 0x0006e47c [208536 == 0x00032e98]
+	       GUID: 0x0006e47c - 0x0006e48c [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at 5a2d4)
-Table TypeRef: 206 records (10 bytes, at 5a2e0)
-Table TypeDef: 437 records (18 bytes, at 5aaec)
-Table Field: 2714 records (8 bytes, at 5c9a6)
-Table Method: 3582 records (16 bytes, at 61e76)
-Table Param: 2600 records (8 bytes, at 6fe56)
-Table InterfaceImpl: 394 records (4 bytes, at 74f96)
-Table MemberRef: 1671 records (8 bytes, at 755be)
-Table Constant: 1122 records (6 bytes, at 789f6)
-Table CustomAttribute: 2309 records (8 bytes, at 7a442)
-Table DeclSecurity: 1 records (6 bytes, at 7ec6a)
-Table ClassLayout: 14 records (8 bytes, at 7ec70)
-Table StandaloneSig: 357 records (2 bytes, at 7ece0)
-Table EventMap: 84 records (4 bytes, at 7efaa)
-Table Event: 84 records (8 bytes, at 7f0fa)
-Table PropertyMap: 171 records (4 bytes, at 7f39a)
-Table Property: 931 records (8 bytes, at 7f646)
-Table MethodSemantics: 1846 records (6 bytes, at 8135e)
-Table MethodImpl: 4 records (6 bytes, at 83ea2)
-Table TypeSpec: 502 records (2 bytes, at 83eba)
-Table FieldRVA: 26 records (6 bytes, at 842a6)
-Table Assembly: 1 records (26 bytes, at 84342)
-Table AssemblyRef: 18 records (24 bytes, at 8435c)
-Table ManifestResource: 1 records (14 bytes, at 8450c)
-Table NestedClass: 220 records (4 bytes, at 8451a)
-Table GenericParam: 31 records (10 bytes, at 8488a)
-Table MethodSpec: 394 records (4 bytes, at 849c0)
-Table GenericParamConstraint: 30 records (4 bytes, at 84fe8)
+Table Module: 1 records (12 bytes, at 5a288)
+Table TypeRef: 206 records (10 bytes, at 5a294)
+Table TypeDef: 437 records (18 bytes, at 5aaa0)
+Table Field: 2714 records (8 bytes, at 5c95a)
+Table Method: 3582 records (16 bytes, at 61e2a)
+Table Param: 2600 records (8 bytes, at 6fe0a)
+Table InterfaceImpl: 394 records (4 bytes, at 74f4a)
+Table MemberRef: 1672 records (8 bytes, at 75572)
+Table Constant: 1122 records (6 bytes, at 789b2)
+Table CustomAttribute: 2309 records (8 bytes, at 7a3fe)
+Table DeclSecurity: 1 records (6 bytes, at 7ec26)
+Table ClassLayout: 14 records (8 bytes, at 7ec2c)
+Table StandaloneSig: 357 records (2 bytes, at 7ec9c)
+Table EventMap: 84 records (4 bytes, at 7ef66)
+Table Event: 84 records (8 bytes, at 7f0b6)
+Table PropertyMap: 171 records (4 bytes, at 7f356)
+Table Property: 931 records (8 bytes, at 7f602)
+Table MethodSemantics: 1846 records (6 bytes, at 8131a)
+Table MethodImpl: 4 records (6 bytes, at 83e5e)
+Table TypeSpec: 502 records (2 bytes, at 83e76)
+Table FieldRVA: 26 records (6 bytes, at 84262)
+Table Assembly: 1 records (26 bytes, at 842fe)
+Table AssemblyRef: 18 records (24 bytes, at 84318)
+Table ManifestResource: 1 records (14 bytes, at 844c8)
+Table NestedClass: 220 records (4 bytes, at 844d6)
+Table GenericParam: 31 records (10 bytes, at 84846)
+Table MethodSpec: 394 records (4 bytes, at 8497c)
+Table GenericParamConstraint: 30 records (4 bytes, at 84fa4)
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/UndertaleModLib.xml` & `am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.xml`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/YAMS-LIB.deps.json` & `am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.deps.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9423076923076924%*

 * *Differences: {"'libraries'": "{'YAMS-LIB/2.0.0': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), 'SixLabors.ImageSharp/3.1.3': OrderedDict([('type', 'package'), "*

 * *                "('serviceable', True), ('sha512', "*

 * *                "'sha512-wybtaqZQ1ZRZ4ZeU+9h+PaSeV14nyiGKIy7qRbDfSHzHq4ybqyOcjoifeaYbiKLO1u+PVxLBuy7MF/DMmwwbfg=='), "*

 * *                "('path', 'sixlabors.imagesharp/3.1.3'), ('hashPath', "*

 * *                "'sixlabors.imagesharp.3.1.3.nupkg.sha512')]), delete:  […]*

```diff
@@ -46,34 +46,34 @@
         "SharpZipLib/1.3.3": {
             "hashPath": "sharpziplib.1.3.3.nupkg.sha512",
             "path": "sharpziplib/1.3.3",
             "serviceable": true,
             "sha512": "sha512-N8+hwhsKZm25tDJfWpBSW7EGhH/R7EMuiX+KJ4C4u+fCWVc1lJ5zg1u3S1RPPVYgTqhx/C3hxrqUpi6RwK5+Tg==",
             "type": "package"
         },
-        "SixLabors.ImageSharp/3.1.2": {
-            "hashPath": "sixlabors.imagesharp.3.1.2.nupkg.sha512",
-            "path": "sixlabors.imagesharp/3.1.2",
+        "SixLabors.ImageSharp/3.1.3": {
+            "hashPath": "sixlabors.imagesharp.3.1.3.nupkg.sha512",
+            "path": "sixlabors.imagesharp/3.1.3",
             "serviceable": true,
-            "sha512": "sha512-PYdR6GUI+gW6LBaAQKTik0Ai8oLpFAz3a/KrVusxoTg3kf7F3cuIqKMhJGsuQcmDHCF+iD81Pyn4cexyHrb1ZA==",
+            "sha512": "sha512-wybtaqZQ1ZRZ4ZeU+9h+PaSeV14nyiGKIy7qRbDfSHzHq4ybqyOcjoifeaYbiKLO1u+PVxLBuy7MF/DMmwwbfg==",
             "type": "package"
         },
         "System.Drawing.Common/5.0.3": {
             "hashPath": "system.drawing.common.5.0.3.nupkg.sha512",
             "path": "system.drawing.common/5.0.3",
             "serviceable": true,
             "sha512": "sha512-rEQZuslijqdsO0pkJn7LtGBaMc//YVA8de0meGihkg9oLPaN+w+/Pb5d71lgp0YjPoKgBKNMvdq0IPnoW4PEng==",
             "type": "package"
         },
         "UndertaleModLib/1.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
-        "YAMS-LIB/1.2.9": {
+        "YAMS-LIB/2.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         }
     },
     "runtimeTarget": {
         "name": ".NETCoreApp,Version=v6.0",
@@ -130,19 +130,19 @@
                 "runtime": {
                     "lib/netstandard2.1/ICSharpCode.SharpZipLib.dll": {
                         "assemblyVersion": "1.3.3.11",
                         "fileVersion": "1.3.3.11"
                     }
                 }
             },
-            "SixLabors.ImageSharp/3.1.2": {
+            "SixLabors.ImageSharp/3.1.3": {
                 "runtime": {
                     "lib/net6.0/SixLabors.ImageSharp.dll": {
                         "assemblyVersion": "3.0.0.0",
-                        "fileVersion": "3.1.2.0"
+                        "fileVersion": "3.1.3.0"
                     }
                 }
             },
             "System.Drawing.Common/5.0.3": {
                 "dependencies": {
                     "Microsoft.Win32.SystemEvents": "5.0.0"
                 },
@@ -174,19 +174,19 @@
                     "SharpZipLib": "1.3.3",
                     "System.Drawing.Common": "5.0.3"
                 },
                 "runtime": {
                     "UndertaleModLib.dll": {}
                 }
             },
-            "YAMS-LIB/1.2.9": {
+            "YAMS-LIB/2.0.0": {
                 "dependencies": {
                     "Macross.Json.Extensions": "3.0.0",
                     "NaturalSort.Extension": "4.2.0",
-                    "SixLabors.ImageSharp": "3.1.2",
+                    "SixLabors.ImageSharp": "3.1.3",
                     "UndertaleModLib": "1.0.0"
                 },
                 "runtime": {
                     "YAMS-LIB.dll": {}
                 }
             }
         }
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/YAMS-LIB.dll` & `am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.dll`

 * *Files 2% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xb0226ddc
+	             Time stamp: 0xc5330f13
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x00043000
+	              Code Size: 0x00043600
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x00044f16
+	        Entry Point RVA: 0x0004556a
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00046000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -41,66 +41,66 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x00044ec4 [0x0000004f]
+	     Import Table: 0x00045518 [0x0000004f]
 	   Resource Table: 0x00046000 [0x00000370]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x00048000 [0x0000000c]
-	            Debug: 0x00044dec [0x00000054]
+	            Debug: 0x00045440 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00042f48
+	   Virtual Size: 0x00043598
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x00043000
+	  Raw Data Size: 0x00043600
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x00000370
 	Virtual Address: 0x00046000
 	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x00043200
+	   Raw Data Ptr: 0x00043800
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x00048000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x00043600
+	   Raw Data Ptr: 0x00043c00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0000eb90 [0x0003625c]
+	         Metadata: 0x0000ec0c [0x00036834]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
@@ -111,30 +111,30 @@
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
 	Tables (#~): 0x0000006c - 0x00002b58 [10988 == 0x00002aec]
 	    Strings: 0x00002b58 - 0x00004d98 [8768 == 0x00002240]
-	       Blob: 0x00033ec8 - 0x0003625c [9108 == 0x00002394]
-	User string: 0x00004d98 - 0x00033eb8 [192800 == 0x0002f120]
-	       GUID: 0x00033eb8 - 0x00033ec8 [16 == 0x00000010]
+	       Blob: 0x000344ac - 0x00036834 [9096 == 0x00002388]
+	User string: 0x00004d98 - 0x0003449c [194308 == 0x0002f704]
+	       GUID: 0x0003449c - 0x000344ac [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at ce60)
-Table TypeRef: 130 records (6 bytes, at ce6a)
-Table TypeDef: 42 records (14 bytes, at d176)
-Table Field: 262 records (6 bytes, at d3c2)
-Table Method: 94 records (14 bytes, at d9e6)
-Table Param: 100 records (6 bytes, at df0a)
-Table MemberRef: 350 records (6 bytes, at e162)
-Table Constant: 143 records (6 bytes, at e996)
-Table CustomAttribute: 412 records (6 bytes, at ecf0)
-Table ClassLayout: 1 records (8 bytes, at f698)
-Table StandaloneSig: 18 records (2 bytes, at f6a0)
-Table TypeSpec: 66 records (2 bytes, at f6c4)
-Table FieldRVA: 1 records (6 bytes, at f748)
-Table Assembly: 1 records (22 bytes, at f74e)
-Table AssemblyRef: 11 records (20 bytes, at f764)
-Table NestedClass: 9 records (4 bytes, at f840)
-Table GenericParam: 2 records (8 bytes, at f864)
-Table MethodSpec: 26 records (4 bytes, at f874)
-Table GenericParamConstraint: 2 records (4 bytes, at f8dc)
+Table Module: 1 records (10 bytes, at cedc)
+Table TypeRef: 130 records (6 bytes, at cee6)
+Table TypeDef: 42 records (14 bytes, at d1f2)
+Table Field: 262 records (6 bytes, at d43e)
+Table Method: 94 records (14 bytes, at da62)
+Table Param: 100 records (6 bytes, at df86)
+Table MemberRef: 350 records (6 bytes, at e1de)
+Table Constant: 143 records (6 bytes, at ea12)
+Table CustomAttribute: 412 records (6 bytes, at ed6c)
+Table ClassLayout: 1 records (8 bytes, at f714)
+Table StandaloneSig: 18 records (2 bytes, at f71c)
+Table TypeSpec: 66 records (2 bytes, at f740)
+Table FieldRVA: 1 records (6 bytes, at f7c4)
+Table Assembly: 1 records (22 bytes, at f7ca)
+Table AssemblyRef: 11 records (20 bytes, at f7e0)
+Table NestedClass: 9 records (4 bytes, at f8bc)
+Table GenericParam: 2 records (8 bytes, at f8e0)
+Table MethodSpec: 26 records (4 bytes, at f8f0)
+Table GenericParamConstraint: 2 records (4 bytes, at f958)
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/YAMS-LIB.pdb` & `am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.pdb`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 00000000: 4253 4a42 0100 0100 0000 0000 0c00 0000  BSJB............
 00000010: 5044 4220 7631 2e30 0000 0000 0000 0600  PDB v1.0........
 00000020: 7c00 0000 6c00 0000 2350 6462 0000 0000  |...l...#Pdb....
-00000030: e800 0000 a00f 0000 237e 0000 8810 0000  ........#~......
+00000030: e800 0000 b80f 0000 237e 0000 a010 0000  ........#~......
 00000040: 0408 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
-00000050: 8c18 0000 0400 0000 2355 5300 9018 0000  ........#US.....
-00000060: 7000 0000 2347 5549 4400 0000 0019 0000  p...#GUID.......
-00000070: 1c54 0000 2342 6c6f 6200 0000 4bc1 9499  .T..#Blob...K...
-00000080: 0af5 2b4e 8b83 efc4 7a88 5ecc 66ed 89bc  ..+N....z.^.f...
+00000050: a418 0000 0400 0000 2355 5300 a818 0000  ........#US.....
+00000060: 7000 0000 2347 5549 4400 0000 1819 0000  p...#GUID.......
+00000070: 7454 0000 2342 6c6f 6200 0000 dcd1 0daf  tT..#Blob.......
+00000080: a09b 2341 afa0 4650 144a 6c0f ebc5 43e5  ..#A..FP.Jl...C.
 00000090: 0000 0000 579d 0228 091e 0000 0100 0000  ....W..(........
 000000a0: 8200 0000 2a00 0000 0601 0000 5e00 0000  ....*.......^...
 000000b0: 6400 0000 5e01 0000 8f00 0000 9c01 0000  d...^...........
 000000c0: 0100 0000 1200 0000 4200 0000 0100 0000  ........B.......
 000000d0: 0100 0000 0b00 0000 0900 0000 0200 0000  ................
 000000e0: 1a00 0000 0200 0000 0000 0000 0200 0001  ................
 000000f0: 0000 0000 0000 bf00 0000 0000 0000 8400  ................
-00000100: 0e00 0000 5e00 0000 8600 0000 b600 0000  ....^...........
+00000100: 0e00 0000 5e00 0000 8700 0000 b700 0000  ....^...........
 00000110: 0800 0000 1900 0000 0f00 0000 2e00 0100  ................
 00000120: 3800 0200 6d00 0100 7700 0200 a800 0100  8...m...w.......
 00000130: b300 0200 ee00 0100 fb00 0200 2d01 0100  ............-...
 00000140: 3a01 0200 7701 0100 8601 0200 c001 0100  :...w...........
 00000150: cf01 0200 0602 0100 1502 0200 5002 0100  ............P...
 00000160: 5f02 0200 8b02 0100 9602 0200 c502 0100  _...............
 00000170: d002 0200 1f03 0100 3003 0200 f103 0100  ........0.......
 00000180: 0204 0200 0705 0100 1805 0200 0000 0000  ................
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0100 d32d 0100 652e 0100 712e 0200 7d2e  ...-..e...q...}.
-000001b0: 0200 242f 0200 2b2f 0200 552f 0200 6b2f  ..$/..+/..U/..k/
-000001c0: 0200 812f 0200 8d2f 0200 992f 0200 a52f  .../.../.../.../
-000001d0: 0200 af2f 0300 f72f 0000 0000 0a00 b830  .../.../.......0
-000001e0: 0a00 e731 0000 0000 0a00 e34a 0a00 ea4a  ...1.......J...J
-000001f0: 0b00 204b 0000 0000 0b00 a64b 0b00 ae4b  .. K.......K...K
-00000200: 0b00 b64b 0000 0000 0000 0000 0b00 d24b  ...K...........K
-00000210: 0b00 da4b 0b00 e74b 0b00 f94b 0400 014c  ...K...K...K...L
-00000220: 0400 434c 0400 ee4c 0000 0000 0500 004d  ..CL...L.......M
-00000230: 0000 0000 0600 ca4f 0000 0000 0700 3151  .......O......1Q
-00000240: 0000 0000 0800 af51 0000 0000 0900 d851  .......Q.......Q
-00000250: 0000 0000 0000 0000 0200 2452 0000 0000  ..........$R....
-00000260: 0000 0000 0a00 2b52 0a00 3352 0a00 3b52  ......+R..3R..;R
-00000270: 0a00 4352 0a00 4b52 0a00 5352 0a00 5b52  ..CR..KR..SR..[R
-00000280: 0a00 6352 0a00 6b52 0a00 7352 0a00 7c52  ..cR..kR..sR..|R
-00000290: 0a00 8452 0a00 8c52 0a00 9552 0a00 9d52  ...R...R...R...R
-000002a0: 0a00 a552 0a00 ad52 0a00 b552 0a00 bd52  ...R...R...R...R
-000002b0: 0a00 c552 0a00 cd52 0000 0000 0a00 d552  ...R...R.......R
-000002c0: 0a00 8853 0a00 c153 0a00 ce53 0a00 d653  ...S...S...S...S
-000002d0: 0000 0000 0a00 de53 0000 0000 0a00 e553  .......S.......S
-000002e0: 0a00 ed53 0a00 f553 0a00 fd53 0000 0000  ...S...S...S....
-000002f0: 0a00 0554 0000 0000 0000 0000 0500 0d54  ...T...........T
-00000300: 0500 1454 0600 0300 0100 0100 0000 0000  ...T............
+000001a0: 0100 d22d 0100 642e 0100 702e 0200 7c2e  ...-..d...p...|.
+000001b0: 0200 232f 0200 2a2f 0200 542f 0200 6a2f  ..#/..*/..T/..j/
+000001c0: 0200 802f 0200 8c2f 0200 982f 0200 a42f  .../.../.../.../
+000001d0: 0200 ae2f 0300 f62f 0000 0000 0a00 b730  .../.../.......0
+000001e0: 0a00 0632 0000 0000 0a00 394b 0a00 404b  ...2......9K..@K
+000001f0: 0b00 764b 0000 0000 0b00 fc4b 0b00 044c  ..vK.......K...L
+00000200: 0b00 0c4c 0000 0000 0000 0000 0b00 284c  ...L..........(L
+00000210: 0b00 304c 0b00 3d4c 0b00 4f4c 0400 574c  ..0L..=L..OL..WL
+00000220: 0400 994c 0400 444d 0000 0000 0500 564d  ...L..DM......VM
+00000230: 0000 0000 0600 2050 0000 0000 0700 8751  ...... P.......Q
+00000240: 0000 0000 0800 0552 0000 0000 0900 2e52  .......R.......R
+00000250: 0000 0000 0000 0000 0200 7a52 0000 0000  ..........zR....
+00000260: 0000 0000 0a00 8152 0a00 8952 0a00 9152  .......R...R...R
+00000270: 0a00 9952 0a00 a152 0a00 a952 0a00 b152  ...R...R...R...R
+00000280: 0a00 b952 0a00 c152 0a00 c952 0a00 d252  ...R...R...R...R
+00000290: 0a00 da52 0a00 e252 0a00 eb52 0a00 f352  ...R...R...R...R
+000002a0: 0a00 fb52 0a00 0353 0a00 0b53 0a00 1353  ...R...S...S...S
+000002b0: 0a00 1b53 0a00 2353 0000 0000 0a00 2b53  ...S..#S......+S
+000002c0: 0a00 de53 0a00 1754 0a00 2454 0a00 2c54  ...S...T..$T..,T
+000002d0: 0000 0000 0a00 3454 0000 0000 0a00 3b54  ......4T......;T
+000002e0: 0a00 4354 0a00 4b54 0a00 5354 0000 0000  ..CT..KT..ST....
+000002f0: 0a00 5b54 0000 0000 0000 0000 0500 6354  ..[T..........cT
+00000300: 0500 6a54 0600 0300 0100 0100 0000 0000  ..jT............
 00000310: 0700 0000 0700 0300 0100 0100 0000 0000  ................
 00000320: 0800 0000 0800 0300 0100 0100 0000 0000  ................
 00000330: 0900 0000 0900 0500 0100 0100 0000 0000  ................
 00000340: 1500 0000 0a00 0500 0100 0100 0000 0000  ................
 00000350: 0d00 0000 0b00 0500 0100 0100 0000 0000  ................
 00000360: 8500 0000 0c00 0500 0200 0100 0000 0000  ................
 00000370: 2700 0000 0d00 0500 0300 0100 0000 0000  '...............
@@ -61,1686 +61,1693 @@
 000003c0: 4a00 0000 1200 0500 0500 0100 0000 0000  J...............
 000003d0: d000 0000 1300 0700 0900 0100 0000 0000  ................
 000003e0: 8901 0000 1300 0700 0a00 0100 c900 0000  ................
 000003f0: 5900 0000 1300 0700 0c00 0100 4b01 0000  Y...........K...
 00000400: 3300 0000 1300 0700 0d00 0100 5001 0000  3...........P...
 00000410: 2e00 0000 1500 0900 0e00 0100 0000 0000  ................
 00000420: 6900 0000 1600 0900 0f00 0100 0000 0000  i...............
-00000430: 209c 0000 1600 0900 3d00 0900 2700 0000   .......=...'...
+00000430: 999c 0000 1600 0900 3d00 0900 2700 0000  ........=...'...
 00000440: 2a00 0000 1600 0900 3e00 0900 3001 0000  *.......>...0...
 00000450: 4400 0000 1600 0900 3f00 0900 7401 0000  D.......?...t...
 00000460: 0102 0000 1600 0900 4200 0900 3802 0000  ........B...8...
 00000470: 4000 0000 1600 0900 4300 0900 3503 0000  @.......C...5...
-00000480: 4000 0000 1600 0900 4400 0900 2e2f 0000  @.......D..../..
-00000490: 2000 0000 1600 0900 4500 0900 b42f 0000   .......E..../..
-000004a0: 2000 0000 1600 0900 4600 0900 3c30 0000   .......F...<0..
-000004b0: 2000 0000 1600 0900 4700 0900 a730 0000   .......G....0..
-000004c0: 4500 0000 1600 0900 4800 0900 c635 0000  E.......H....5..
-000004d0: 4b00 0000 1600 0900 4900 0900 6537 0000  K.......I...e7..
-000004e0: 2300 0000 1600 0900 4a00 0900 173a 0000  #.......J....:..
-000004f0: 2300 0000 1600 0900 4b00 0900 a23b 0000  #.......K....;..
-00000500: 2600 0000 1600 0900 4c00 0900 1b3c 0000  &.......L....<..
-00000510: 4500 0000 1600 0900 4d00 0900 f43c 0000  E.......M....<..
-00000520: 4500 0000 1600 0900 4e00 0900 983e 0000  E.......N....>..
-00000530: 2900 0000 1600 0900 4f00 0900 b842 0000  ).......O....B..
-00000540: c401 0000 1600 0900 5000 0900 c442 0000  ........P....B..
-00000550: a601 0000 1600 0900 5500 0900 a845 0000  ........U....E..
-00000560: 2900 0000 1600 0900 5600 0900 1c46 0000  ).......V....F..
-00000570: 2900 0000 1600 0900 5700 0900 9b47 0000  ).......W....G..
-00000580: 890e 0000 1600 0900 6400 0900 9b5f 0000  ........d...._..
-00000590: 2900 0000 1600 0900 6500 0900 8b62 0000  ).......e....b..
-000005a0: 2900 0000 1600 0900 6600 0900 9664 0000  ).......f....d..
-000005b0: 2900 0000 1600 0900 6700 0900 7d65 0000  ).......g...}e..
-000005c0: 2900 0000 1600 0900 6800 0900 4066 0000  ).......h...@f..
-000005d0: 2900 0000 1600 0900 6900 0900 1b6c 0000  ).......i....l..
-000005e0: 2900 0000 1600 0900 6a00 0900 976d 0000  ).......j....m..
-000005f0: 3409 0000 1600 0900 6c00 0900 b36d 0000  4.......l....m..
-00000600: 1809 0000 1600 0900 6d00 0900 b76d 0000  ........m....m..
-00000610: c108 0000 1600 0900 7300 0900 d870 0000  ........s....p..
-00000620: 3700 0000 1600 0900 7400 0900 8f7e 0000  7.......t....~..
-00000630: 5707 0000 1600 0900 7600 0900 ab7e 0000  W.......v....~..
-00000640: 3b07 0000 1600 0900 7900 0900 ca82 0000  ;.......y.......
-00000650: 2200 0000 1600 0900 7a00 0900 b589 0000  ".......z.......
-00000660: 2300 0000 1600 0900 7b00 0900 0e8a 0000  #.......{.......
-00000670: 8b00 0000 1600 0900 7c00 0900 598a 0000  ........|...Y...
-00000680: 2900 0000 1600 0900 7d00 0900 aa8a 0000  ).......}.......
-00000690: 5e00 0000 1600 0900 7e00 0900 568c 0000  ^.......~...V...
-000006a0: 4a00 0000 1600 0900 7f00 0900 fe8c 0000  J...............
-000006b0: 3600 0000 1600 0900 8000 0900 0c8e 0000  6...............
-000006c0: 3600 0000 1600 0900 8100 0900 a08e 0000  6...............
-000006d0: 4a00 0000 1600 0900 8200 0900 3d8f 0000  J...........=...
-000006e0: 2900 0000 1600 0900 8300 0900 5994 0000  )...........Y...
-000006f0: 0d01 0000 1600 0900 8400 0900 9094 0000  ................
-00000700: a200 0000 1600 0900 8500 0900 dd9b 0000  ................
-00000710: 4200 0000 1800 0900 8600 0900 0000 0000  B...............
-00000720: 0b00 0000 1900 0900 8600 0900 0000 0000  ................
-00000730: 8a00 0000 1a00 0b00 8900 0900 0000 0000  ................
-00000740: 3e00 0000 1c00 0b00 8900 0900 0000 0000  >...............
-00000750: 1200 0000 1d00 0b00 8900 0900 0000 0000  ................
-00000760: 0e00 0000 1e00 0b00 8900 0900 0000 0000  ................
-00000770: 3e00 0000 2100 0b00 8900 0900 0000 0000  >...!...........
-00000780: 1200 0000 2200 0b00 8900 0900 0000 0000  ...."...........
-00000790: 1d00 0000 2300 0b00 8900 0900 0000 0000  ....#...........
-000007a0: 2800 0000 2400 0b00 8900 0900 0000 0000  (...$...........
-000007b0: 1200 0000 2500 0e00 8900 0900 0000 0000  ....%...........
-000007c0: b600 0000 2600 0e00 8900 0900 0000 0000  ....&...........
-000007d0: 5906 0000 2700 0e00 8a00 0900 0000 0000  Y...'...........
-000007e0: 1100 0000 2900 1100 8a00 0900 0000 0000  ....)...........
-000007f0: 210b 0000 2900 1100 8c00 0900 0e01 0000  !...)...........
-00000800: f609 0000 2900 1100 8e00 0900 2a01 0000  ....).......*...
-00000810: da09 0000 2900 1100 8f00 0900 3e01 0000  ....).......>...
-00000820: 7309 0000 2900 1100 9000 0900 5801 0000  s...).......X...
-00000830: 3c09 0000 2900 1100 9100 0900 6001 0000  <...).......`...
-00000840: 3409 0000 2900 1100 9800 0900 4403 0000  4...).......D...
-00000850: 8000 0000 2900 1100 9900 0900 5308 0000  ....).......S...
-00000860: fa00 0000 2900 1100 9a00 0900 1c09 0000  ....)...........
-00000870: 1800 0000 2900 1100 9b00 0900 6909 0000  ....).......i...
-00000880: e200 0000 2b00 1500 9c00 0900 0000 0000  ....+...........
-00000890: 9003 0000 2b00 1500 a600 0900 1500 0000  ....+...........
-000008a0: 7000 0000 2d00 1500 a800 0900 0000 0000  p...-...........
-000008b0: d601 0000 2d00 1500 ad00 0900 1d00 0000  ....-...........
-000008c0: dd00 0000 2d00 1500 ae00 0900 4800 0000  ....-.......H...
-000008d0: 9600 0000 2f00 1900 af00 0900 0000 0000  ..../...........
-000008e0: 2200 0000 3100 1900 af00 0900 0000 0000  "...1...........
-000008f0: 6901 0000 3400 0500 b000 0900 0000 0000  i...4...........
-00000900: 1d00 0000 3700 0900 b000 0900 0000 0000  ....7...........
-00000910: 0200 0000 3800 0900 b000 0900 0000 0000  ....8...........
-00000920: 1d00 0000 3900 0900 b000 0900 0000 0000  ....9...........
-00000930: 1a00 0000 3a00 0900 b000 0900 0000 0000  ....:...........
-00000940: 1a00 0000 3b00 0900 b000 0900 0000 0000  ....;...........
-00000950: 1a00 0000 3c00 0900 b000 0900 0000 0000  ....<...........
-00000960: 1d00 0000 3d00 0900 b000 0900 0000 0000  ....=...........
-00000970: 1d00 0000 3e00 0900 b000 0900 0000 0000  ....>...........
-00000980: 1d00 0000 3f00 0900 b000 0900 0000 0000  ....?...........
-00000990: 1d00 0000 4000 0900 b000 0900 0000 0000  ....@...........
-000009a0: 4300 0000 4100 0900 b000 0900 0000 0000  C...A...........
-000009b0: 5a00 0000 4200 0900 b000 0900 0000 0000  Z...B...........
-000009c0: 5a00 0000 4300 0900 b000 0900 0000 0000  Z...C...........
-000009d0: 4300 0000 4400 0900 b000 0900 0000 0000  C...D...........
-000009e0: 1600 0000 4500 0900 b000 0900 0000 0000  ....E...........
-000009f0: 1b00 0000 4600 0900 b000 0900 0000 0000  ....F...........
-00000a00: 1b00 0000 4700 0900 b000 0900 0000 0000  ....G...........
-00000a10: 1b00 0000 4800 0900 b000 0900 0000 0000  ....H...........
-00000a20: 1b00 0000 4900 0900 b000 0900 0000 0000  ....I...........
-00000a30: 3300 0000 4a00 0900 b000 0900 0000 0000  3...J...........
-00000a40: 1b00 0000 4b00 0900 b000 0900 0000 0000  ....K...........
-00000a50: 1b00 0000 4d00 0900 b000 0900 0000 0000  ....M...........
-00000a60: b802 0000 4d00 0900 b000 0900 0b00 0000  ....M...........
-00000a70: 0b00 0000 4d00 0900 b100 0900 2e00 0000  ....M...........
-00000a80: 7c02 0000 4d00 0900 b200 0900 3200 0000  |...M.......2...
-00000a90: 7802 0000 4e00 0900 b500 0900 0000 0000  x...N...........
-00000aa0: ae00 0000 4e00 0900 b600 0900 4300 0000  ....N.......C...
-00000ab0: 3c00 0000 4f00 0900 b700 0900 0000 0000  <...O...........
-00000ac0: 7200 0000 5000 0900 b700 0900 0000 0000  r...P...........
-00000ad0: 1d00 0000 5100 0900 b700 0900 0000 0000  ....Q...........
-00000ae0: 1d00 0000 5300 0900 b700 0900 0000 0000  ....S...........
-00000af0: 2400 0000 5500 0900 b700 0900 0000 0000  $...U...........
-00000b00: 3900 0000 5600 0900 b700 0900 0000 0000  9...V...........
-00000b10: 3100 0000 5700 0900 b700 0900 0000 0000  1...W...........
-00000b20: 3900 0000 5800 0900 b700 0900 0000 0000  9...X...........
-00000b30: 3100 0000 5a00 0900 b700 0900 0000 0000  1...Z...........
-00000b40: 4000 0000 5d00 1100 b700 0900 0000 0000  @...]...........
-00000b50: 1b00 0000 5e00 1100 b700 0900 0000 0000  ....^...........
-00000b60: 6100 0000 0000 0000 b806 0000 0000 b806  a...............
-00000b70: 0000 0000 b806 0000 0000 0100 0000 0000  ................
-00000b80: 5f07 0000 0100 b004 0000 0200 1103 0000  _...............
-00000b90: 0300 9706 0000 0000 e202 0000 0400 4802  ..............H.
-00000ba0: 0000 0500 3b02 0000 0900 0f02 0000 0a00  ....;...........
-00000bb0: 3202 0000 0000 4307 0000 0000 0100 0000  2.....C.........
-00000bc0: 0100 cd04 0000 0200 a402 0000 0300 8002  ................
-00000bd0: 0000 0400 9e03 0000 0500 0006 0000 0600  ................
-00000be0: 2104 0000 0700 c301 0000 0800 e906 0000  !...............
-00000bf0: 0900 5003 0000 0a00 c103 0000 0b00 7a06  ..P...........z.
-00000c00: 0000 0c00 c106 0000 0d00 ea03 0000 0e00  ................
-00000c10: d603 0000 0f00 4200 0000 1000 5200 0000  ......B.....R...
-00000c20: 1100 2f00 0000 1200 d005 0000 1300 5005  ../...........P.
-00000c30: 0000 1400 0204 0000 1500 7c01 0000 1600  ..........|.....
-00000c40: 0803 0000 1700 8801 0000 1800 5006 0000  ............P...
-00000c50: 1900 3506 0000 1a00 2106 0000 1b00 6606  ..5.....!.....f.
-00000c60: 0000 1c00 3304 0000 1d00 d806 0000 1e00  ....3...........
-00000c70: f006 0000 1f00 0207 0000 2000 8706 0000  .......... .....
-00000c80: 2100 b301 0000 2200 a301 0000 2300 9804  !.....".....#...
-00000c90: 0000 2400 ba04 0000 2500 8504 0000 2600  ..$.....%.....&.
-00000ca0: 3007 0000 2700 1407 0000 2800 5c05 0000  0...'.....(.\...
-00000cb0: 2900 0401 0000 2a00 b004 0000 2b00 1103  ).....*.....+...
-00000cc0: 0000 2c00 b203 0000 2d00 1306 0000 2e00  ..,.....-.......
-00000cd0: ad04 0000 3000 b704 0000 3100 1100 0000  ....0.....1.....
-00000ce0: 3200 0302 0000 3300 f601 0000 3400 b704  2.....3.....4...
-00000cf0: 0000 3500 b704 0000 3700 6907 0000 3800  ..5.....7.i...8.
-00000d00: 6907 0000 3a00 a102 0000 3c00 2702 0000  i...:.....<.'...
-00000d10: 3d00 e501 0000 3e00 1e02 0000 3f00 1e02  =.....>.....?...
-00000d20: 0000 4000 1e02 0000 4200 d100 0000 4400  ..@.....B.....D.
-00000d30: d100 0000 4500 1e02 0000 4700 0603 0000  ....E.....G.....
-00000d40: 4800 0e04 0000 4900 9402 0000 4a00 cf03  H.....I.....J...
-00000d50: 0000 4b00 0c06 0000 4c00 6303 0000 4d00  ..K.....L.c...M.
-00000d60: 7602 0000 4e00 7602 0000 4f00 bd05 0000  v...N.v...O.....
-00000d70: 5000 7705 0000 5100 a705 0000 5200 9105  P.w...Q.....R...
-00000d80: 0000 5300 6905 0000 5400 d804 0000 5500  ..S.i...T.....U.
-00000d90: 1005 0000 5600 6c01 0000 5700 5f01 0000  ....V.l...W._...
-00000da0: 5800 2903 0000 5900 3d01 0000 5a00 3803  X.)...Y.=...Z.8.
-00000db0: 0000 5b00 4c01 0000 5e00 e501 0000 6300  ..[.L...^.....c.
-00000dc0: e501 0000 6400 e501 0000 6500 e501 0000  ....d.....e.....
-00000dd0: 6600 e501 0000 6700 e501 0000 6900 2403  f.....g.....i.$.
-00000de0: 0000 6a00 f807 0000 6d00 c807 0000 6e00  ..j.....m.....n.
-00000df0: a207 0000 6f00 b807 0000 7000 d607 0000  ....o.....p.....
-00000e00: 7100 ea07 0000 7200 8007 0000 7300 9407  q.....r.....s...
-00000e10: 0000 7400 3d07 0000 7600 5d02 0000 7700  ..t.=...v.]...w.
-00000e20: 4504 0000 7b00 2f05 0000 7c00 9501 0000  E...{./...|.....
-00000e30: 7d00 2b01 0000 7e00 3d07 0000 7f00 1e02  }.+...~.=.......
-00000e40: 0000 8000 5402 0000 8100 f204 0000 8200  ....T...........
-00000e50: 0603 0000 8300 f204 0000 8400 f204 0000  ................
-00000e60: 8500 f204 0000 8600 f204 0000 8700 1e02  ................
-00000e70: 0000 8900 7b02 0000 8a00 f204 0000 8b00  ....{...........
-00000e80: ad04 0000 0000 0100 0000 0100 ea01 0000  ................
-00000e90: 0200 b704 0000 0000 a402 0000 0000 7904  ..............y.
-00000ea0: 0000 0100 2107 0000 0500 1c01 0000 0600  ....!...........
-00000eb0: 7607 0000 0a00 1f01 0000 0b00 4b03 0000  v...........K...
-00000ec0: 0c00 f204 0000 0d00 3805 0000 0e00 d202  ........8.......
-00000ed0: 0000 0f00 8004 0000 1000 4505 0000 1100  ..........E.....
-00000ee0: fd04 0000 1200 1b05 0000 1300 b806 0000  ................
-00000ef0: 1600 e501 0000 1900 b302 0000 1b00 1902  ................
-00000f00: 0000 1c00 dc05 0000 0000 5d04 0000 0100  ..........].....
-00000f10: be02 0000 0200 2100 0000 0300 4c07 0000  ......!.....L...
-00000f20: 0400 f502 0000 0500 9e06 0000 0600 1104  ................
-00000f30: 0000 0700 e404 0000 0800 9003 0000 0900  ................
-00000f40: f305 0000 0b00 5402 0000 0c00 fb00 0000  ......T.........
-00000f50: 0000 4c04 0000 0100 6802 0000 0200 d501  ..L.....h.......
-00000f60: 0000 0300 8503 0000 0400 e905 0000 0600  ................
-00000f70: 9b02 0000 0b00 2501 0000 0000 c301 0000  ......%.........
-00000f80: 0200 7204 0000 0300 ec02 0000 0400 0100  ..r.............
-00000f90: 0000 0500 7b03 0000 0600 1b03 0000 0000  ....{...........
-00000fa0: b306 0000 0200 3f07 8b00 b34a ba00 b94a  ......?....J...J
-00000fb0: a100 bf4a eb00 c54a 7700 cb4a 6300 d14a  ...J...Jw..Jc..J
-00000fc0: d800 d74a 6d03 dd4a 0000 0000 0100 4f2e  ...Jm..J......O.
-00000fd0: 0200 0000 0100 ff2e 0400 0000 0100 9f30  ...............0
-00000fe0: 0600 0000 0100 a831 0800 0000 0100 804b  .......1.......K
-00000ff0: 0a00 0000 0100 254c 0c00 0000 0d00 0000  ......%L........
-00001000: 0100 a94f 0f00 0000 1000 0000 0100 0d51  ...O...........Q
-00001010: 1200 0000 1300 0000 1400 0000 0100 bc51  ...............Q
-00001020: 1600 0000 1700 0000 1800 0000 2700 0500  ............'...
-00001030: 9306 2700 0600 bc07 2700 0700 e309 6301  ..'.....'.....c.
-00001040: 0400 9106 8301 0400 9106 9601 0300 5103  ..............Q.
-00001050: a301 0400 9106 b601 0300 2304 c301 0400  ..........#.....
-00001060: 9106 d601 0300 3905 e301 0400 9106 6302  ......9.......c.
-00001070: 0400 9106 8302 0400 9106 a302 0400 9106  ................
-00001080: 4303 0400 9106 0000 0043 5324 3c3e 385f  C........CS$<>8_
-00001090: 5f6c 6f63 616c 7330 0043 5324 3c3e 385f  _locals0.CS$<>8_
-000010a0: 5f6c 6f63 616c 7331 0072 6f6f 6d4e 616d  _locals1.roomNam
-000010b0: 6548 7564 4343 0077 6174 6572 5475 7262  eHudCC.waterTurb
-000010c0: 696e 6544 6f6f 7243 4300 7468 6f74 684c  ineDoorCC.thothL
-000010d0: 6566 7444 6f6f 7243 4300 7468 6f74 6852  eftDoorCC.thothR
-000010e0: 6967 6874 446f 6f72 4343 0050 6970 6549  ightDoorCC.PipeI
-000010f0: 6e44 6570 7468 7355 7070 6572 4944 0050  nDepthsUpperID.P
-00001100: 6970 6549 6e44 6570 7468 734c 6f77 6572  ipeInDepthsLower
-00001110: 4944 0054 686f 7468 4272 6964 6765 4c65  ID.ThothBridgeLe
-00001120: 6674 446f 6f72 4944 0041 3257 6174 6572  ftDoorID.A2Water
-00001130: 5475 7262 696e 654c 6566 7444 6f6f 7249  TurbineLeftDoorI
-00001140: 4400 5468 6f74 6842 7269 6467 6552 6967  D.ThothBridgeRig
-00001150: 6874 446f 6f72 4944 0064 6f6f 7249 4400  htDoorID.doorID.
-00001160: 5069 7065 496e 5761 7465 7266 616c 6c73  PipeInWaterfalls
-00001170: 4944 0050 6970 6549 6e48 6964 656f 7574  ID.PipeInHideout
-00001180: 4944 0072 6f6f 6d44 6174 6100 6f43 6f6e  ID.roomData.oCon
-00001190: 7472 6f6c 4e65 7477 6f72 6b52 6563 6569  trolNetworkRecei
-000011a0: 7665 6400 6964 0066 6f75 6e64 0063 6f6f  ved.id.found.coo
-000011b0: 7264 0063 6f6c 6c69 7369 6f6e 436f 6465  rd.collisionCode
-000011c0: 546f 4265 0064 6570 7468 7350 6970 6543  ToBe.depthsPipeC
-000011d0: 6f64 6500 7761 7465 7266 616c 6c73 5069  ode.waterfallsPi
-000011e0: 7065 436f 6465 006e 6573 7450 6970 6543  peCode.nestPipeC
-000011f0: 6f64 6500 6869 6465 6f75 7450 6970 6543  ode.hideoutPipeC
-00001200: 6f64 6500 6472 6177 4775 6943 6f64 6500  ode.drawGuiCode.
-00001210: 6c61 6242 6c6f 636b 436f 6465 0063 6f6c  labBlockCode.col
-00001220: 6c69 7369 6f6e 436f 6465 006c 6f61 6447  lisionCode.loadG
-00001230: 6c6f 6261 6c73 436f 6465 0073 6176 6547  lobalsCode.saveG
-00001240: 6c6f 6261 6c73 436f 6465 0063 6861 7261  lobalsCode.chara
-00001250: 6374 6572 5661 7273 436f 6465 0073 7346  cterVarsCode.ssF
-00001260: 4744 6573 7472 6f79 436f 6465 0063 6f64  GDestroyCode.cod
-00001270: 6500 7465 7874 7572 6550 6167 6500 6134  e.texturePage.a4
-00001280: 5061 6765 3249 6d61 6765 0061 3450 6167  Page2Image.a4Pag
-00001290: 6549 6d61 6765 006d 7573 6963 4669 6c65  eImage.musicFile
-000012a0: 0074 696c 6500 636f 6465 4e61 6d65 0073  .tile.codeName.s
-000012b0: 7072 6974 654e 616d 6500 6f72 6967 4e61  priteName.origNa
-000012c0: 6d65 006f 7269 6753 6f6e 674e 616d 6500  me.origSongName.
-000012d0: 6e65 7753 6f6e 674e 616d 6500 726f 6f6d  newSongName.room
-000012e0: 4e61 6d65 0070 6963 6b75 704e 616d 6500  Name.pickupName.
-000012f0: 4453 4d61 7043 6f6f 7264 526f 6f6d 6e61  DSMapCoordRoomna
-00001300: 6d65 0070 6970 6500 7769 7364 6f6d 5365  me.pipe.wisdomSe
-00001310: 7074 6f67 6743 7265 6174 6500 6372 6561  ptoggCreate.crea
-00001320: 7465 0076 616c 7565 0062 6700 6f57 6973  te.value.bg.oWis
-00001330: 646f 6d53 6570 746f 6767 006c 6566 7446  domSeptogg.leftF
-00001340: 6163 696e 6700 726f 6f6d 4e61 6d65 4453  acing.roomNameDS
-00001350: 4d61 7053 7472 696e 6700 6973 5265 7365  MapString.isRese
-00001360: 6172 6368 4861 7463 6800 6d75 7369 6350  archHatch.musicP
-00001370: 6174 6800 6669 6c65 5061 7468 0072 6f6f  ath.filePath.roo
-00001380: 6d4e 616d 6548 7564 4472 6177 4775 6900  mNameHudDrawGui.
-00001390: 6c61 6242 6c6f 636b 0061 7267 734c 6f63  labBlock.argsLoc
-000013a0: 616c 0070 6167 6549 7465 6d00 6974 656d  al.pageItem.item
-000013b0: 0064 6570 7468 7350 6970 6552 6f6f 6d00  .depthsPipeRoom.
-000013c0: 7761 7465 7266 616c 6c73 5069 7065 526f  waterfallsPipeRo
-000013d0: 6f6d 0072 6f6f 6d00 646f 6f72 5361 6d75  om.room.doorSamu
-000013e0: 7343 6f6c 6c69 7369 6f6e 0063 6f6c 6c69  sCollision.colli
-000013f0: 7369 6f6e 0070 6167 6544 696d 656e 7369  sion.pageDimensi
-00001400: 6f6e 0065 7874 656e 7369 6f6e 0073 7346  on.extension.ssF
-00001410: 4741 6374 696f 6e00 726f 6f6d 4875 6441  GAction.roomHudA
-00001420: 6374 696f 6e00 7769 7364 6f6d 5365 7074  ction.wisdomSept
-00001430: 6f67 6741 6374 696f 6e00 6f43 6f6e 7472  oggAction.oContr
-00001440: 6f6c 4163 7469 6f6e 0076 6172 446f 6f72  olAction.varDoor
-00001450: 4163 7469 6f6e 0061 6374 696f 6e00 6135  Action.action.a5
-00001460: 4163 7469 7661 7465 436f 6e64 6974 696f  ActivateConditio
-00001470: 6e00 656d 7042 6174 7465 7279 4365 6c6c  n.empBatteryCell
-00001480: 436f 6e64 6974 696f 6e00 7363 7244 4e41  Condition.scrDNA
-00001490: 5370 6177 6e00 676f 0072 6f6f 6d4e 616d  Spawn.go.roomNam
-000014a0: 6548 7564 5374 6570 0077 6973 646f 6d53  eHudStep.wisdomS
-000014b0: 6570 746f 6767 5374 6570 0073 7562 7363  eptoggStep.subsc
-000014c0: 7265 656e 4d65 6e75 5374 6570 0070 6963  reenMenuStep.pic
-000014d0: 6b75 7000 6473 4d61 7043 6f72 6442 7569  kup.dsMapCordBui
-000014e0: 6c64 6572 0072 6f6f 6d4e 616d 6544 534d  lder.roomNameDSM
-000014f0: 6170 4275 696c 6465 7200 7375 6244 6972  apBuilder.subDir
-00001500: 0061 3544 6f6f 7200 646f 6f72 0061 6c72  .a5Door.door.alr
-00001510: 6561 6479 4164 6465 6450 426f 6d62 7300  eadyAddedPBombs.
-00001520: 616c 7265 6164 7941 6464 6564 4d69 7373  alreadyAddedMiss
-00001530: 696c 6573 0066 7300 6c6f 6361 6c73 006d  iles.fs.locals.m
-00001540: 7300 616c 7265 6164 7941 6464 6564 5375  s.alreadyAddedSu
-00001550: 7065 7273 0073 6565 644f 626a 6563 7400  pers.seedObject.
-00001560: 736f 6c69 644f 626a 6563 7400 726f 6f6d  solidObject.room
-00001570: 4875 644f 626a 6563 7400 6761 6d65 4f62  HudObject.gameOb
-00001580: 6a65 6374 0077 6174 6572 5475 7262 696e  ject.waterTurbin
-00001590: 654f 626a 6563 7400 7069 7065 4f62 6a65  eObject.pipeObje
-000015a0: 6374 0072 6573 6561 7263 6848 6174 6368  ct.researchHatch
-000015b0: 4f62 6a65 6374 0067 6d4f 626a 6563 7400  Object.gmObject.
-000015c0: 6973 476f 746f 4f62 6a65 6374 0064 6f6f  isGotoObject.doo
-000015d0: 724f 626a 6563 7400 656e 656d 794f 626a  rObject.enemyObj
-000015e0: 6563 7400 6574 616e 6b53 6e69 7070 6574  ect.etankSnippet
-000015f0: 0070 6970 6542 4754 696c 6573 6574 0064  .pipeBGTileset.d
-00001600: 6570 7468 7345 6e74 7261 6e63 6550 6970  epthsEntrancePip
-00001610: 6554 696c 6573 6574 0077 6174 6572 6661  eTileset.waterfa
-00001620: 6c6c 7350 6970 6554 696c 6573 6574 0064  llsPipeTileset.d
-00001630: 6570 7468 7345 7869 7450 6970 6554 696c  epthsExitPipeTil
-00001640: 6573 6574 0068 6964 656f 7574 5069 7065  eset.hideoutPipe
-00001650: 5469 6c65 7365 7400 646f 6f72 5469 6c65  Tileset.doorTile
-00001660: 7365 7400 6d6f 7669 6e67 4f66 6673 6574  set.movingOffset
-00001670: 0073 7346 4745 7665 6e74 0072 6f6f 6d48  .ssFGEvent.roomH
-00001680: 7564 4576 656e 7400 7769 7364 6f6d 5365  udEvent.wisdomSe
-00001690: 7074 6f67 6745 7665 6e74 006f 436f 6e74  ptoggEvent.oCont
-000016a0: 726f 6c45 7665 6e74 0070 426f 6d62 4368  rolEvent.pBombCh
-000016b0: 6172 6163 7465 7245 7665 6e74 0073 7570  aracterEvent.sup
-000016c0: 6572 4d69 7373 696c 6543 6861 7261 6374  erMissileCharact
-000016d0: 6572 4576 656e 7400 6d69 7373 696c 6543  erEvent.missileC
-000016e0: 6861 7261 6374 6572 4576 656e 7400 6554  haracterEvent.eT
-000016f0: 616e 6b43 6861 7261 6374 6572 4576 656e  ankCharacterEven
-00001700: 7400 7661 7244 6f6f 7245 7665 6e74 0069  t.varDoorEvent.i
-00001710: 7465 6d73 5377 6170 5363 7269 7074 0073  temsSwapScript.s
-00001720: 6372 6970 7400 726f 6f6d 4e61 6d65 4875  cript.roomNameHu
-00001730: 6452 6f6f 6d53 7461 7274 006c 6973 7400  dRoomStart.list.
-00001740: 636f 6465 5465 7874 006e 6577 446f 6f72  codeText.newDoor
-00001750: 5265 706c 6163 656d 656e 7454 6578 7400  ReplacementText.
-00001760: 7375 6273 6372 6565 6e4d 6973 6344 6177  subscreenMiscDaw
-00001770: 0073 7344 7261 7700 7375 6263 7265 656e  .ssDraw.subcreen
-00001780: 426f 6f74 7344 7261 7700 7375 6273 6372  BootsDraw.subscr
-00001790: 6565 6e53 7569 7444 7261 7700 6472 6177  eenSuitDraw.draw
-000017a0: 456e 6449 6e64 6578 0064 6f6f 7245 7665  EndIndex.doorEve
-000017b0: 6e74 496e 6465 7800 6472 6177 5374 6172  ntIndex.drawStar
-000017c0: 7449 6e64 6578 006b 6579 0061 7373 656d  tIndex.key.assem
-000017d0: 626c 7900 726f 6f6d 4e61 6d65 4875 6444  bly.roomNameHudD
-000017e0: 6573 7472 6f79 0063 6f64 6545 6e74 7279  estroy.codeEntry
-000017f0: 0074 6578 7475 7265 456e 7472 7900 646f  .textureEntry.do
-00001800: 6f72 456e 7472 7900 6c6f 636b 6564 5042  orEntry.lockedPB
-00001810: 6f6d 6251 7561 6e74 6974 7900 7042 6f6d  ombQuantity.pBom
-00001820: 6251 7561 6e74 6974 7900 6c6f 636b 6564  bQuantity.locked
-00001830: 4d69 7373 696c 6551 7561 6e74 6974 7900  MissileQuantity.
-00001840: 6d69 7373 696c 6551 7561 6e74 6974 7900  missileQuantity.
-00001850: 6669 6e61 6c51 7561 6e74 6974 7900 6c6f  finalQuantity.lo
-00001860: 636b 6564 5375 7065 7251 7561 6e74 6974  ckedSuperQuantit
-00001870: 7900 7375 7065 7251 7561 6e74 6974 7900  y.superQuantity.
-00001880: 7175 616e 7469 7479 0000 0000 0000 0000  quantity........
-00001890: 0fd0 2988 b811 1342 878b 770e 8597 ac16  ..)....B..w.....
-000018a0: f862 513f c607 d311 9053 00c0 4fa3 02a1  .bQ?.....S..O...
-000018b0: 1b57 8a0e 2669 6e46 b4ad 8ab0 4611 f5fe  .W..&inF....F...
-000018c0: bc74 2e93 a9db 7844 8d46 0f32 a7ba b3d3  .t....xD.F.2....
-000018d0: 5605 11cc 91a0 384d 9fec 25ab 9a35 1a6a  V.....8M..%..5.j
-000018e0: 05ec feb5 d08c 834a 96da 4662 84bb 4bd8  .......J..Fb..K.
-000018f0: 0847 4d7e 6e09 5c4c aeda cb10 ba6a 740d  .GM~n.\L.....jt.
-00001900: 0004 686f 6d65 0672 756e 6e65 7204 776f  ..home.runner.wo
-00001910: 726b 0459 414d 5308 5941 4d53 2d4c 4942  rk.YAMS.YAMS-LIB
-00001920: 0d45 7863 6570 7469 6f6e 732e 6373 092f  .Exceptions.cs./
-00001930: 0001 060d 1212 1720 2045 cf63 12b5 33a2  .......  E.c..3.
-00001940: 5dfc 4dce b431 5040 06cb b9c4 4b95 8487  ].M..1P@....K...
-00001950: 2f00 aa0c 69ad 7c7b 7913 4578 7465 6e73  /...i.|{y.Extens
-00001960: 696f 6e4d 6574 686f 6473 2e63 7309 2f00  ionMethods.cs./.
-00001970: 0106 0d12 1217 5920 8e60 29b7 ed9a 0b1a  ......Y .`).....
-00001980: 1a46 f770 be95 760e ea0e 8ec0 45b2 e613  .F.p..v.....E...
-00001990: b318 395a 43ae 57f7 0f4d 7573 6963 5368  ..9ZC.W..MusicSh
-000019a0: 7566 666c 652e 6373 0a2f 0001 060d 1212  uffle.cs./......
-000019b0: 1780 9820 3c0a 97ef 3aba 9a95 23f6 7f5c  ... <...:...#..\
-000019c0: 7a9b 8254 fac4 f5de dc3e 0a75 a15d d33b  z..T.....>.u.].;
-000019d0: dcc7 45e4 0770 6174 6368 6573 1141 6464  ..E..patches.Add
-000019e0: 496e 4761 6d65 4869 6e74 732e 6373 0c2f  InGameHints.cs./
-000019f0: 0001 060d 1212 1780 d480 dc20 6e02 69a1  ........... n.i.
-00001a00: 68e9 d66f e7cc 3811 95b7 b370 bf14 88e1  h..o..8....p....
-00001a10: e2a0 5b53 5d2c f554 b77d acd2 1044 6f6f  ..[S],.T.}...Doo
-00001a20: 724c 6f63 6b52 616e 646f 2e63 730c 2f00  rLockRando.cs./.
-00001a30: 0106 0d12 1217 80d4 811c 2036 f08f a89d  .......... 6....
-00001a40: edf4 9ff1 a97a ba4d a182 4fae 5fd8 d698  .....z.M..O._...
-00001a50: f8ef ca26 269f d9e7 76e9 4b03 716f 6c17  ...&&...v.K.qol.
-00001a60: 4469 7370 6c61 7952 6f6f 6d4e 616d 654f  DisplayRoomNameO
-00001a70: 6e48 5544 2e63 730e 2f00 0106 0d12 1217  nHUD.cs./.......
-00001a80: 80d4 815b 815f 204d 230e 0556 3847 6697  ...[._ M#..V8Gf.
-00001a90: 0043 bc2d 019d cbc8 eff9 18c3 6186 d3f1  .C.-........a...
-00001aa0: 6fc8 9a1b fbec 8518 4469 7370 6c61 7952  o.......DisplayR
-00001ab0: 6f6f 6d4e 616d 6573 4f6e 4d61 702e 6373  oomNamesOnMap.cs
-00001ac0: 0e2f 0001 060d 1212 1780 d481 5b81 a720  ./..........[.. 
-00001ad0: 9919 2851 d6ab de16 69e2 2683 bb64 d446  ..(Q....i.&..d.F
-00001ae0: ec54 5d2c 3782 f134 153b 566c d5e2 b53d  .T],7..4.;Vl...=
-00001af0: 1552 6f6f 6d46 6561 7475 7265 4d61 7054  .RoomFeatureMapT
-00001b00: 6578 742e 6373 0e2f 0001 060d 1212 1780  ext.cs./........
-00001b10: d481 5b81 f020 c482 530a 0a87 6a5c fe69  ..[.. ..S...j\.i
-00001b20: 192a 2c85 e5cc b9d5 9e17 e194 a1d4 dce7  .*,.............
-00001b30: ab23 4c0e d7c7 1953 686f 7746 756c 6c79  .#L....ShowFully
-00001b40: 556e 6578 706c 6f72 6564 4d61 702e 6373  UnexploredMap.cs
-00001b50: 0e2f 0001 060d 1212 1780 d481 5b82 3620  ./..........[.6 
-00001b60: 4b38 9777 782b b256 ca61 3817 dbbd b9b4  K8.wx+.V.a8.....
-00001b70: eecc 3d52 c65a 60a4 aa48 c276 683a d2af  ..=R.Z`..H.vh:..
-00001b80: 0a50 726f 6772 616d 2e63 730a 2f00 0106  .Program.cs./...
-00001b90: 0d12 1217 8280 20f1 dcd0 8ba4 e324 8cd4  ...... ......$..
-00001ba0: 20fd 33c3 6a3f 4a62 93ed 43b0 db7f 9c6c   .3.j?Jb..C....l
-00001bb0: 89f9 4190 708c f60d 5365 6564 4f62 6a65  ..A.p...SeedObje
-00001bc0: 6374 2e63 730a 2f00 0106 0d12 1217 82b7  ct.cs./.........
-00001bd0: 20a5 b494 9139 481b 9251 1e7e e0ce e117   ....9H..Q.~....
-00001be0: effa 872f f3db 1e04 f297 e646 7c22 8262  .../.......F|".b
-00001bf0: 6203 6f62 6a07 5265 6c65 6173 6506 6e65  b.obj.Release.ne
-00001c00: 7436 2e30 1a59 414d 532d 4c49 422e 476c  t6.0.YAMS-LIB.Gl
-00001c10: 6f62 616c 5573 696e 6773 2e67 2e63 7310  obalUsings.g.cs.
-00001c20: 2f00 0106 0d12 1217 82f1 82f5 82fd 8304  /...............
-00001c30: 20ad db14 3f8c 43b9 5f1b b73a 0cba 7c79   ...?.C._..:..|y
-00001c40: 3281 935c 4ab8 ccab bdf6 b04d 3e0f 809e  2..\J......M>...
-00001c50: 0e70 1f01 0000 d3d7 57b0 492c 2dc9 d74d  .p......W.I,-..M
-00001c60: 4fcd 4b2d 4a2c 494d d1b7 e34a cfc9 4f4a  O.K-J,IM...J..OJ
-00001c70: cc51 282d cecc 4b57 8070 acac 822b 8b4b  .Q(-..KW.p...+.K
-00001c80: 5273 adf1 49ea 39e7 e7e4 a426 9764 e6e7  Rs..I.9....&.d..
-00001c90: 15eb b983 0ccc 4cc6 afc1 d31f bfbc 4f66  ......L.......Of
-00001ca0: 5e21 7e15 7ea9 257a 1e25 2505 f855 8564  ^!~.~.%z.%%..U.d
-00001cb0: 14a5 26a6 0025 8854 a617 9258 9c5d 6ccd  ..&..%.T...X.]l.
-00001cc0: 0500 2e2e 4e45 5443 6f72 6541 7070 2c56  ....NETCoreApp,V
-00001cd0: 6572 7369 6f6e 3d76 362e 302e 4173 7365  ersion=v6.0.Asse
-00001ce0: 6d62 6c79 4174 7472 6962 7574 6573 2e63  mblyAttributes.c
-00001cf0: 7310 2f00 0106 0d12 1217 82f1 82f5 82fd  s./.............
-00001d00: 83c2 2078 97e5 953c b5cd 5131 509b 3504  .. x...<..Q1P.5.
-00001d10: 2186 34c2 4b9c e7a6 8b98 4ffb 5a16 686e  !.4.K.....O.Z.hn
-00001d20: b5af 5c80 c900 0000 002f 2f20 3c61 7574  ..\......// <aut
-00001d30: 6f67 656e 6572 6174 6564 202f 3e0d 0a75  ogenerated />..u
-00001d40: 7369 6e67 2053 7973 7465 6d3b 0d0a 7573  sing System;..us
-00001d50: 696e 6720 5379 7374 656d 2e52 6566 6c65  ing System.Refle
-00001d60: 6374 696f 6e3b 0d0a 5b61 7373 656d 626c  ction;..[assembl
-00001d70: 793a 2067 6c6f 6261 6c3a 3a53 7973 7465  y: global::Syste
-00001d80: 6d2e 5275 6e74 696d 652e 5665 7273 696f  m.Runtime.Versio
-00001d90: 6e69 6e67 2e54 6172 6765 7446 7261 6d65  ning.TargetFrame
-00001da0: 776f 726b 4174 7472 6962 7574 6528 222e  workAttribute(".
-00001db0: 4e45 5443 6f72 6541 7070 2c56 6572 7369  NETCoreApp,Versi
-00001dc0: 6f6e 3d76 362e 3022 2c20 4672 616d 6577  on=v6.0", Framew
-00001dd0: 6f72 6b44 6973 706c 6179 4e61 6d65 203d  orkDisplayName =
-00001de0: 2022 2e4e 4554 2036 2e30 2229 5d0a 1859   ".NET 6.0")]..Y
-00001df0: 414d 532d 4c49 422e 4173 7365 6d62 6c79  AMS-LIB.Assembly
-00001e00: 496e 666f 2e63 7310 2f00 0106 0d12 1217  Info.cs./.......
-00001e10: 82f1 82f5 82fd 84ee 200b 2c44 55bc ee11  ........ .,DU...
-00001e20: a2b3 77c5 872b ed97 9494 a179 00d4 e354  ..w..+.....y...T
-00001e30: a7c1 be13 d5ab 2a1c 2481 56d2 0300 00ad  ......*.$.V.....
-00001e40: 93df 4bc3 3010 c7df fb57 1c3e 29b2 d675  ..K.0....W.>)..u
-00001e50: 3f3a 9d08 db60 3270 20db 5044 7cb8 b697  ?:...`2p .PD|...
-00001e60: 3690 2692 a48e fef7 a6d3 8d8d a114 b67b  6.&............{
-00001e70: cbdd e5f3 bdbb 5c82 a075 56f3 8200 eeb1  ......\..uV.....
-00001e80: b4aa 9591 248d 96d2 87da 57db 2ae7 0612  ....$.....W.*...
-00001e90: 9512 acd1 c02e 0e71 0508 5629 e1bb cc6d  .......q..V)...m
-00001ea0: f224 4799 9171 7eb0 f53d c605 4181 1524  .$G..q~..=..A..$
-00001eb0: 581a 022e 13a5 3525 1662 caf1 8b2b 0d28  X.....5%.b...+.(
-00001ec0: 5358 7321 9c07 8432 1638 dbc2 6c4e 3fc2  SXs!...2.8..lN?.
-00001ed0: 0ea4 69a7 ec6f aa0d 8ecb 3df3 4cbc d270  ..i..o....=.L..p
-00001ee0: 99c1 b232 968a e1c1 c95f 1013 ae0d aee4  ...2....._......
-00001ef0: d0f3 ded1 182a 6251 dd1d 87fd d16f 6ca2  .....*bQ.....ol.
-00001f00: 8a4f 94d5 c85a cde3 d2d2 e5c5 db68 be6c  .O...Z.......h.l
-00001f10: 3dcd c617 571f 4d11 92f1 ac74 fd3a ef1e  =...W.M....t.:..
-00001f20: 6841 82d0 5063 ced4 3dca 0b69 7348 69fb  hA..Pc..=..isHi.
-00001f30: a17f ebdf 34a6 cc24 53ba d8d4 82e2 0fdc  ....4..$S.......
-00001f40: f5a0 8351 38e8 f559 1452 afdb 6fb3 68d0  ...Q8..Y.R..o.h.
-00001f50: 4efa 0c19 85d4 c110 23ea 4631 76fa 8d55  N.......#.F1v..U
-00001f60: 9fb5 4acb c49e 32c6 15b7 824e 01fc 3bbb  ..J...2....N..;.
-00001f70: 7a39 1ff7 3f49 bdc5 f3e5 b8e4 2285 57cd  z9..?I......".W.
-00001f80: 2d4d dc4a 4f35 6605 490b 8970 8abe e77d  -M.JO5f.I..p...}
-00001f90: 0301 0b81 277b 2264 6f63 756d 656e 7473  ....'{"documents
-00001fa0: 223a 7b22 2f68 6f6d 652f 7275 6e6e 6572  ":{"/home/runner
-00001fb0: 2f77 6f72 6b2f 5941 4d53 2f59 414d 532f  /work/YAMS/YAMS/
-00001fc0: 2a22 3a22 6874 7470 733a 2f2f 7261 772e  *":"https://raw.
-00001fd0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00001fe0: 742e 636f 6d2f 7261 6e64 6f76 616e 6961  t.com/randovania
-00001ff0: 2f59 414d 532f 3833 6137 3238 3536 6637  /YAMS/83a72856f7
-00002000: 3265 3534 3631 6637 3831 6336 6661 6665  2e5461f781c6fafe
-00002010: 3265 3361 3261 3765 3437 6261 3336 2f2a  2e3a2a7e47ba36/*
-00002020: 222c 222f 686f 6d65 2f72 756e 6e65 722f  ","/home/runner/
-00002030: 776f 726b 2f59 414d 532f 5941 4d53 2f55  work/YAMS/YAMS/U
-00002040: 6e64 6572 7461 6c65 4d6f 6454 6f6f 6c2f  ndertaleModTool/
-00002050: 2a22 3a22 6874 7470 733a 2f2f 7261 772e  *":"https://raw.
-00002060: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00002070: 742e 636f 6d2f 6b72 7a79 732d 682f 556e  t.com/krzys-h/Un
-00002080: 6465 7274 616c 654d 6f64 546f 6f6c 2f32  dertaleModTool/2
-00002090: 6630 6536 3665 3039 3130 3439 3764 3531  f0e66e0910497d51
-000020a0: 3263 3138 6234 3439 6637 3566 3437 3461  2c18b449f75f474a
-000020b0: 3334 3235 6630 372f 2a22 7d7d 8225 7665  3425f07/*"}}.%ve
-000020c0: 7273 696f 6e00 3200 636f 6d70 696c 6572  rsion.2.compiler
-000020d0: 2d76 6572 7369 6f6e 0034 2e38 2e30 2d37  -version.4.8.0-7
-000020e0: 2e32 3335 3732 2e31 2b37 6237 3539 3831  .23572.1+7b75981
-000020f0: 6366 3362 6435 3230 6238 3665 6334 6564  cf3bd520b86ec4ed
-00002100: 3030 6563 3135 3663 3862 6334 3865 3465  00ec156c8bc48e4e
-00002110: 6200 6c61 6e67 7561 6765 0043 2300 736f  b.language.C#.so
-00002120: 7572 6365 2d66 696c 652d 636f 756e 7400  urce-file-count.
-00002130: 3134 006f 7574 7075 742d 6b69 6e64 0044  14.output-kind.D
-00002140: 796e 616d 6963 616c 6c79 4c69 6e6b 6564  ynamicallyLinked
-00002150: 4c69 6272 6172 7900 6f70 7469 6d69 7a61  Library.optimiza
-00002160: 7469 6f6e 0072 656c 6561 7365 0070 6c61  tion.release.pla
-00002170: 7466 6f72 6d00 416e 7943 7075 0072 756e  tform.AnyCpu.run
-00002180: 7469 6d65 2d76 6572 7369 6f6e 0038 2e30  time-version.8.0
-00002190: 2e31 2b62 6635 6532 3739 6439 3233 3962  .1+bf5e279d9239b
-000021a0: 6665 6635 6262 3162 3864 3632 3132 6631  fef5bb1b8d6212f1
-000021b0: 6239 3731 6334 3334 3630 3600 6c61 6e67  b971c434606.lang
-000021c0: 7561 6765 2d76 6572 7369 6f6e 0070 7265  uage-version.pre
-000021d0: 7669 6577 006e 756c 6c61 626c 6500 456e  view.nullable.En
-000021e0: 6162 6c65 0064 6566 696e 6500 5452 4143  able.define.TRAC
-000021f0: 452c 5245 4c45 4153 452c 4e45 542c 4e45  E,RELEASE,NET,NE
-00002200: 5436 5f30 2c4e 4554 434f 5245 4150 502c  T6_0,NETCOREAPP,
-00002210: 4e45 5435 5f30 5f4f 525f 4752 4541 5445  NET5_0_OR_GREATE
-00002220: 522c 4e45 5436 5f30 5f4f 525f 4752 4541  R,NET6_0_OR_GREA
-00002230: 5445 522c 4e45 5443 4f52 4541 5050 315f  TER,NETCOREAPP1_
-00002240: 305f 4f52 5f47 5245 4154 4552 2c4e 4554  0_OR_GREATER,NET
-00002250: 434f 5245 4150 5031 5f31 5f4f 525f 4752  COREAPP1_1_OR_GR
-00002260: 4541 5445 522c 4e45 5443 4f52 4541 5050  EATER,NETCOREAPP
-00002270: 325f 305f 4f52 5f47 5245 4154 4552 2c4e  2_0_OR_GREATER,N
-00002280: 4554 434f 5245 4150 5032 5f31 5f4f 525f  ETCOREAPP2_1_OR_
-00002290: 4752 4541 5445 522c 4e45 5443 4f52 4541  GREATER,NETCOREA
-000022a0: 5050 325f 325f 4f52 5f47 5245 4154 4552  PP2_2_OR_GREATER
-000022b0: 2c4e 4554 434f 5245 4150 5033 5f30 5f4f  ,NETCOREAPP3_0_O
-000022c0: 525f 4752 4541 5445 522c 4e45 5443 4f52  R_GREATER,NETCOR
-000022d0: 4541 5050 335f 315f 4f52 5f47 5245 4154  EAPP3_1_OR_GREAT
-000022e0: 4552 00a3 ee49 4353 6861 7270 436f 6465  ER...ICSharpCode
-000022f0: 2e53 6861 7270 5a69 704c 6962 2e64 6c6c  .SharpZipLib.dll
-00002300: 0000 016c 9904 9800 8003 0087 d282 16a4  ...l............
-00002310: 95d1 4abd 3f1f c402 13b4 ed4d 6163 726f  ..J.?......Macro
-00002320: 7373 2e4a 736f 6e2e 4578 7465 6e73 696f  ss.Json.Extensio
-00002330: 6e73 2e64 6c6c 0000 0155 c478 ba00 0001  ns.dll...U.x....
-00002340: 00b2 09ba d9ca d5dc 4e93 a42a 22b1 17ec  ........N..*"...
-00002350: 344d 6963 726f 736f 6674 2e43 5368 6172  4Microsoft.CShar
-00002360: 702e 646c 6c00 0001 91d0 e9ab 0080 0000  p.dll...........
-00002370: 847c 1edb f757 d540 be4e 6263 2977 646d  .|...W.@.Nbc)wdm
-00002380: 4d69 6372 6f73 6f66 742e 5669 7375 616c  Microsoft.Visual
-00002390: 4261 7369 632e 436f 7265 2e64 6c6c 0000  Basic.Core.dll..
-000023a0: 01d9 c8d2 a900 2001 00dd 6120 0279 6494  ...... ...a .yd.
-000023b0: 4b8a b0cb 44c4 86c6 624d 6963 726f 736f  K...D...bMicroso
-000023c0: 6674 2e56 6973 7561 6c42 6173 6963 2e64  ft.VisualBasic.d
-000023d0: 6c6c 0000 019a f527 8700 8000 0004 e09a  ll.....'........
-000023e0: 55d8 5175 4f80 ed40 596e 37bf 7d4d 6963  U.QuO..@Yn7.}Mic
-000023f0: 726f 736f 6674 2e57 696e 3332 2e50 7269  rosoft.Win32.Pri
-00002400: 6d69 7469 7665 732e 646c 6c00 0001 097a  mitives.dll....z
-00002410: c3d5 0080 0000 c646 6217 f0e4 8f43 ac21  .......Fb....C.!
-00002420: 64cf 2cfa a161 4d69 6372 6f73 6f66 742e  d.,..aMicrosoft.
-00002430: 5769 6e33 322e 5265 6769 7374 7279 2e64  Win32.Registry.d
-00002440: 6c6c 0000 01c2 00bc 8c00 a000 00b5 9185  ll..............
-00002450: 8107 e7cc 45b1 9ec7 f905 1350 416d 7363  ....E......PAmsc
-00002460: 6f72 6c69 622e 646c 6c00 0001 e816 0b95  orlib.dll.......
-00002470: 0020 0100 3460 7cd4 1bf5 744b bd05 a18d  . ..4`|...tK....
-00002480: 8491 838e 4e61 7475 7261 6c53 6f72 742e  ....NaturalSort.
-00002490: 4578 7465 6e73 696f 6e2e 646c 6c00 0001  Extension.dll...
-000024a0: f2df 7ed4 0080 0000 9283 2462 453e 0f40  ..~.......$bE>.@
-000024b0: b403 4bfc c383 cfba 6e65 7473 7461 6e64  ..K.....netstand
-000024c0: 6172 642e 646c 6c00 0001 7426 75aa 00c0  ard.dll...t&u...
-000024d0: 0100 a89e adf7 ffbb 3444 a75d 0c03 0288  ........4D.]....
-000024e0: e443 5072 6f70 6572 7479 4368 616e 6765  .CPropertyChange
-000024f0: 642e 646c 6c00 0001 8b5a 978a 0080 0000  d.dll....Z......
-00002500: 3174 ff35 d3a6 344c 90ea 21b0 de57 7fe0  1t.5..4L..!..W..
-00002510: 5369 784c 6162 6f72 732e 496d 6167 6553  SixLabors.ImageS
-00002520: 6861 7270 2e64 6c6c 0000 016f c14b c800  harp.dll...o.K..
-00002530: 4020 0026 2592 e899 d38e 4f9d c75f e567  @ .&%.....O.._.g
-00002540: 7258 8953 7973 7465 6d2e 4170 7043 6f6e  rX.System.AppCon
-00002550: 7465 7874 2e64 6c6c 0000 0189 0042 d700  text.dll.....B..
-00002560: 8000 00f3 77d7 0309 562e 4aa1 edb9 3a8d  ....w...V.J...:.
-00002570: 7d51 9a53 7973 7465 6d2e 4275 6666 6572  }Q.System.Buffer
-00002580: 732e 646c 6c00 0001 7390 4c81 0080 0000  s.dll...s.L.....
-00002590: f330 8b8f 7193 904c 9a3f 555c 754c a71d  .0..q..L.?U\uL..
-000025a0: 5379 7374 656d 2e43 6f6c 6c65 6374 696f  System.Collectio
-000025b0: 6e73 2e43 6f6e 6375 7272 656e 742e 646c  ns.Concurrent.dl
-000025c0: 6c00 0001 fe8f 5bc9 00a0 0000 15ac 643a  l.....[.......d:
-000025d0: 157c 6c45 b351 ea60 8312 c278 5379 7374  .|lE.Q.`...xSyst
-000025e0: 656d 2e43 6f6c 6c65 6374 696f 6e73 2e64  em.Collections.d
-000025f0: 6c6c 0000 0106 b6f9 bd00 0001 00f0 00e8  ll..............
-00002600: 6f21 312c 4986 7f21 cbbe 20a1 e553 7973  o!1,I..!.. ..Sys
-00002610: 7465 6d2e 436f 6c6c 6563 7469 6f6e 732e  tem.Collections.
-00002620: 496d 6d75 7461 626c 652e 646c 6c00 0001  Immutable.dll...
-00002630: 258a 3da9 0040 0100 5fd2 d324 4295 e342  %.=..@.._..$B..B
-00002640: a117 f482 0163 ac2b 5379 7374 656d 2e43  .....c.+System.C
-00002650: 6f6c 6c65 6374 696f 6e73 2e4e 6f6e 4765  ollections.NonGe
-00002660: 6e65 7269 632e 646c 6c00 0001 dfed 5ba4  neric.dll.....[.
-00002670: 00a0 0000 0192 9215 b917 e34f 8388 06c5  ...........O....
-00002680: 2f1a c689 5379 7374 656d 2e43 6f6c 6c65  /...System.Colle
-00002690: 6374 696f 6e73 2e53 7065 6369 616c 697a  ctions.Specializ
-000026a0: 6564 2e64 6c6c 0000 01ae 911e 8000 a000  ed.dll..........
-000026b0: 008a 1bec 37cf 318f 4bb9 a81c af1f 50f8  ....7.1.K.....P.
-000026c0: 7a53 7973 7465 6d2e 436f 6d70 6f6e 656e  zSystem.Componen
-000026d0: 744d 6f64 656c 2e41 6e6e 6f74 6174 696f  tModel.Annotatio
-000026e0: 6e73 2e64 6c6c 0000 01cf 803a ee00 c000  ns.dll.....:....
-000026f0: 00ae 3486 ae94 0c7e 4eb8 8438 411d ceea  ..4....~N..8A...
-00002700: f653 7973 7465 6d2e 436f 6d70 6f6e 656e  .System.Componen
-00002710: 744d 6f64 656c 2e44 6174 6141 6e6e 6f74  tModel.DataAnnot
-00002720: 6174 696f 6e73 2e64 6c6c 0000 0122 f4ef  ations.dll..."..
-00002730: b600 8000 0012 bc50 61c6 a6b2 4db9 bdf6  .......Pa...M...
-00002740: 5cd7 f45d 8953 7973 7465 6d2e 436f 6d70  \..].System.Comp
-00002750: 6f6e 656e 744d 6f64 656c 2e64 6c6c 0000  onentModel.dll..
-00002760: 018e 581b 9900 8000 0070 f30e 9e6b 3528  ..X......p...k5(
-00002770: 4590 0e0f 551f a272 ba53 7973 7465 6d2e  E...U..r.System.
-00002780: 436f 6d70 6f6e 656e 744d 6f64 656c 2e45  ComponentModel.E
-00002790: 7665 6e74 4261 7365 6441 7379 6e63 2e64  ventBasedAsync.d
-000027a0: 6c6c 0000 01a7 0575 8700 8000 0092 5580  ll.....u......U.
-000027b0: d711 aba2 4785 002b e48b f753 df53 7973  ....G..+...S.Sys
-000027c0: 7465 6d2e 436f 6d70 6f6e 656e 744d 6f64  tem.ComponentMod
-000027d0: 656c 2e50 7269 6d69 7469 7665 732e 646c  el.Primitives.dl
-000027e0: 6c00 0001 407a 69d3 00a0 0000 11e1 1041  l...@zi........A
-000027f0: 8eb8 c640 b66d d089 85bf e10c 5379 7374  ...@.m......Syst
-00002800: 656d 2e43 6f6d 706f 6e65 6e74 4d6f 6465  em.ComponentMode
-00002810: 6c2e 5479 7065 436f 6e76 6572 7465 722e  l.TypeConverter.
-00002820: 646c 6c00 0001 3fd5 e5d4 00c0 0100 f072  dll...?........r
-00002830: 3cdc 4e2e 0348 a1f9 6f05 6409 62f4 5379  <.N..H..o.d.b.Sy
-00002840: 7374 656d 2e43 6f6e 6669 6775 7261 7469  stem.Configurati
-00002850: 6f6e 2e64 6c6c 0000 0117 4f5e a700 8000  on.dll....O^....
-00002860: 008f 1bad f913 e271 449f 8fcd 27df 70ae  .......qD...'.p.
-00002870: 4053 7973 7465 6d2e 436f 6e73 6f6c 652e  @System.Console.
-00002880: 646c 6c00 0001 5c17 f7a2 00a0 0000 2d00  dll...\.......-.
-00002890: 8a7b c3ce 344a 98a6 3bd8 2f5d 5e3d 5379  .{..4J..;./]^=Sy
-000028a0: 7374 656d 2e43 6f72 652e 646c 6c00 0001  stem.Core.dll...
-000028b0: 9fc2 93ff 00a0 0000 d76f e7ec 69c7 e043  .........o..i..C
-000028c0: 83ea 106f 205d f9f9 5379 7374 656d 2e44  ...o ]..System.D
-000028d0: 6174 612e 436f 6d6d 6f6e 2e64 6c6c 0000  ata.Common.dll..
-000028e0: 01bf c165 b500 8002 00cb 497c 2393 3d25  ...e......I|#.=%
-000028f0: 4581 9757 6989 cbc5 c653 7973 7465 6d2e  E..Wi....System.
-00002900: 4461 7461 2e44 6174 6153 6574 4578 7465  Data.DataSetExte
-00002910: 6e73 696f 6e73 2e64 6c6c 0000 0134 bfab  nsions.dll...4..
-00002920: c300 8000 0066 7e45 b888 3111 4d82 18db  .....f~E..1.M...
-00002930: 2655 cc35 9d53 7973 7465 6d2e 4461 7461  &U.5.System.Data
-00002940: 2e64 6c6c 0000 018e d59c db00 a000 00e3  .dll............
-00002950: c8c3 a86e daeb 4eb5 35ab 5644 dd40 9d53  ...n..N.5.VD.@.S
-00002960: 7973 7465 6d2e 4469 6167 6e6f 7374 6963  ystem.Diagnostic
-00002970: 732e 436f 6e74 7261 6374 732e 646c 6c00  s.Contracts.dll.
-00002980: 0001 0d60 1680 0080 0000 fa9d c34f 6c6a  ...`.........Olj
-00002990: 8947 b3b7 f0df c330 f853 5379 7374 656d  .G.....0.SSystem
-000029a0: 2e44 6961 676e 6f73 7469 6373 2e44 6562  .Diagnostics.Deb
-000029b0: 7567 2e64 6c6c 0000 0176 4e5a 9000 8000  ug.dll...vNZ....
-000029c0: 004b 1885 263b 3a9d 43a5 fd92 572e 5f8e  .K..&;:.C...W._.
-000029d0: 1253 7973 7465 6d2e 4469 6167 6e6f 7374  .System.Diagnost
-000029e0: 6963 732e 4469 6167 6e6f 7374 6963 536f  ics.DiagnosticSo
-000029f0: 7572 6365 2e64 6c6c 0000 012b 9bab d000  urce.dll...+....
-00002a00: c000 0021 6bc9 c501 92ba 4796 971e ebca  ...!k.....G.....
-00002a10: 98f4 b253 7973 7465 6d2e 4469 6167 6e6f  ...System.Diagno
-00002a20: 7374 6963 732e 4669 6c65 5665 7273 696f  stics.FileVersio
-00002a30: 6e49 6e66 6f2e 646c 6c00 0001 2e01 d09f  nInfo.dll.......
-00002a40: 0080 0000 19d3 1884 f386 db43 8b43 ad1c  ...........C.C..
-00002a50: 785d 6985 5379 7374 656d 2e44 6961 676e  x]i.System.Diagn
-00002a60: 6f73 7469 6373 2e50 726f 6365 7373 2e64  ostics.Process.d
-00002a70: 6c6c 0000 014c 6f42 e100 c000 001b eeee  ll...LoB........
-00002a80: 27ad c857 4591 8cb3 6a9b bd5c 7853 7973  '..WE...j..\xSys
-00002a90: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
-00002aa0: 5374 6163 6b54 7261 6365 2e64 6c6c 0000  StackTrace.dll..
-00002ab0: 01de 729e c800 a000 0042 b2fe 6ba7 7572  ..r......B..k.ur
-00002ac0: 419c 76dc 601c 0cb2 8453 7973 7465 6d2e  A.v.`....System.
-00002ad0: 4469 6167 6e6f 7374 6963 732e 5465 7874  Diagnostics.Text
-00002ae0: 5772 6974 6572 5472 6163 654c 6973 7465  WriterTraceListe
-00002af0: 6e65 722e 646c 6c00 0001 1d78 61f8 0080  ner.dll....xa...
-00002b00: 0000 7e92 bdbf b6ef 8346 a6f8 c568 6ff4  ..~......F...ho.
-00002b10: 2b8e 5379 7374 656d 2e44 6961 676e 6f73  +.System.Diagnos
-00002b20: 7469 6373 2e54 6f6f 6c73 2e64 6c6c 0000  tics.Tools.dll..
-00002b30: 01f3 b145 9c00 8000 0007 0bd7 840a ca5f  ...E..........._
-00002b40: 42a8 9058 5cde d118 6e53 7973 7465 6d2e  B..X\...nSystem.
-00002b50: 4469 6167 6e6f 7374 6963 732e 5472 6163  Diagnostics.Trac
-00002b60: 6553 6f75 7263 652e 646c 6c00 0001 a95b  eSource.dll....[
-00002b70: 9ec2 00a0 0000 4266 01a7 524e aa4f 9adf  ......Bf..RN.O..
-00002b80: 87b9 1f74 4cb6 5379 7374 656d 2e44 6961  ...tL.System.Dia
-00002b90: 676e 6f73 7469 6373 2e54 7261 6369 6e67  gnostics.Tracing
-00002ba0: 2e64 6c6c 0000 0109 a6c6 fc00 a000 0063  .dll...........c
-00002bb0: 7534 7c00 7a4a 4fb7 c94d 447c 9a77 9653  u4|.zJO..MD|.w.S
-00002bc0: 7973 7465 6d2e 646c 6c00 0001 7f6b 82fc  ystem.dll....k..
-00002bd0: 0000 0100 d720 4800 f750 f943 b07d 731e  ..... H..P.C.}s.
-00002be0: b9bb 49af 5379 7374 656d 2e44 7261 7769  ..I.System.Drawi
-00002bf0: 6e67 2e43 6f6d 6d6f 6e2e 646c 6c00 0001  ng.Common.dll...
-00002c00: 218d 42d5 0020 0200 0843 fec0 6a78 bb46  !.B.. ...C..jx.F
-00002c10: 9f62 dc8a c5b5 5abc 5379 7374 656d 2e44  .b....Z.System.D
-00002c20: 7261 7769 6e67 2e64 6c6c 0000 0132 8a8b  rawing.dll...2..
-00002c30: ce00 8000 00e5 90db 8f3d 81e3 4cb7 a9c5  .........=..L...
-00002c40: 133a 6614 0653 7973 7465 6d2e 4472 6177  .:f..System.Draw
-00002c50: 696e 672e 5072 696d 6974 6976 6573 2e64  ing.Primitives.d
-00002c60: 6c6c 0000 011f 8c68 b300 c000 001d d0fb  ll.....h........
-00002c70: 4c9a 7940 45ae 2b9b 0cb0 2967 9553 7973  L.y@E.+...)g.Sys
-00002c80: 7465 6d2e 4479 6e61 6d69 632e 5275 6e74  tem.Dynamic.Runt
-00002c90: 696d 652e 646c 6c00 0001 9b33 a19d 0080  ime.dll....3....
-00002ca0: 0000 099e 3f8c f188 2a45 b61a be23 a15f  ....?...*E...#._
-00002cb0: 8e27 5379 7374 656d 2e46 6f72 6d61 7473  .'System.Formats
-00002cc0: 2e41 736e 312e 646c 6c00 0001 e249 aac6  .Asn1.dll....I..
-00002cd0: 00a0 0000 9595 b6ea 2025 5e42 9f2d e8b6  ........ %^B.-..
-00002ce0: 2563 4d74 5379 7374 656d 2e47 6c6f 6261  %cMtSystem.Globa
-00002cf0: 6c69 7a61 7469 6f6e 2e43 616c 656e 6461  lization.Calenda
-00002d00: 7273 2e64 6c6c 0000 0126 a597 9a00 8000  rs.dll...&......
-00002d10: 00bc cbe8 2ac5 3fe2 499a 5723 8e30 7fa2  ....*.?.I.W#.0..
-00002d20: eb53 7973 7465 6d2e 476c 6f62 616c 697a  .System.Globaliz
-00002d30: 6174 696f 6e2e 646c 6c00 0001 cf5f ff90  ation.dll...._..
-00002d40: 0080 0000 38dd 4bf4 e502 ca46 aa62 9fe8  ....8.K....F.b..
-00002d50: 5d24 4789 5379 7374 656d 2e47 6c6f 6261  ]$G.System.Globa
-00002d60: 6c69 7a61 7469 6f6e 2e45 7874 656e 7369  lization.Extensi
-00002d70: 6f6e 732e 646c 6c00 0001 ffd1 a7d5 0080  ons.dll.........
-00002d80: 0000 20a3 ea29 f7b1 f942 ab10 5fd8 d0da  .. ..)...B.._...
-00002d90: ff89 5379 7374 656d 2e49 4f2e 436f 6d70  ..System.IO.Comp
-00002da0: 7265 7373 696f 6e2e 4272 6f74 6c69 2e64  ression.Brotli.d
-00002db0: 6c6c 0000 0158 58f3 de00 8000 0083 5eb3  ll...XX.......^.
-00002dc0: fc8d 9e09 4fbc 04f0 20cd d695 b353 7973  ....O... ....Sys
-00002dd0: 7465 6d2e 494f 2e43 6f6d 7072 6573 7369  tem.IO.Compressi
-00002de0: 6f6e 2e64 6c6c 0000 015e 490f cc00 a000  on.dll...^I.....
-00002df0: 005f 59c8 75f7 c490 4094 9d70 52a4 3579  ._Y.u...@..pR.5y
-00002e00: 6c53 7973 7465 6d2e 494f 2e43 6f6d 7072  lSystem.IO.Compr
-00002e10: 6573 7369 6f6e 2e46 696c 6553 7973 7465  ession.FileSyste
-00002e20: 6d2e 646c 6c00 0001 a0dc 41aa 0080 0000  m.dll.....A.....
-00002e30: 4062 8cca aa5f 3c48 bff6 503c 69e8 70a5  @b..._<H..P<i.p.
-00002e40: 5379 7374 656d 2e49 4f2e 436f 6d70 7265  System.IO.Compre
-00002e50: 7373 696f 6e2e 5a69 7046 696c 652e 646c  ssion.ZipFile.dl
-00002e60: 6c00 0001 c27b 83d4 0080 0000 dff4 40cc  l....{........@.
-00002e70: 6507 9c4f 948b 50b6 efcf b9ed 5379 7374  e..O..P.....Syst
-00002e80: 656d 2e49 4f2e 646c 6c00 0001 3496 8cec  em.IO.dll...4...
-00002e90: 0080 0000 0875 2e81 fd7e 0243 ad06 bdec  .....u...~.C....
-00002ea0: 29cc 2360 5379 7374 656d 2e49 4f2e 4669  ).#`System.IO.Fi
-00002eb0: 6c65 5379 7374 656d 2e41 6363 6573 7343  leSystem.AccessC
-00002ec0: 6f6e 7472 6f6c 2e64 6c6c 0000 01fe cec7  ontrol.dll......
-00002ed0: f400 a000 0095 d9aa d4f3 7110 4384 90de  ..........q.C...
-00002ee0: a7ab 8f50 2e53 7973 7465 6d2e 494f 2e46  ...P.System.IO.F
-00002ef0: 696c 6553 7973 7465 6d2e 646c 6c00 0001  ileSystem.dll...
-00002f00: 7953 7cd7 0080 0000 57e9 5221 2ce4 0444  yS|.....W.R!,..D
-00002f10: a794 ec0c 9c9e a409 5379 7374 656d 2e49  ........System.I
-00002f20: 4f2e 4669 6c65 5379 7374 656d 2e44 7269  O.FileSystem.Dri
-00002f30: 7665 496e 666f 2e64 6c6c 0000 014d 58d8  veInfo.dll...MX.
-00002f40: a600 8000 00e6 1289 5a9b 1ba7 45bb aae5  ........Z...E...
-00002f50: c8be 2862 0953 7973 7465 6d2e 494f 2e46  ..(b.System.IO.F
-00002f60: 696c 6553 7973 7465 6d2e 5072 696d 6974  ileSystem.Primit
-00002f70: 6976 6573 2e64 6c6c 0000 01a7 0ef2 f000  ives.dll........
-00002f80: 8000 0060 12c9 96e6 62e4 4d9b 1959 b08e  ...`....b.M..Y..
-00002f90: 040c 2253 7973 7465 6d2e 494f 2e46 696c  .."System.IO.Fil
-00002fa0: 6553 7973 7465 6d2e 5761 7463 6865 722e  eSystem.Watcher.
-00002fb0: 646c 6c00 0001 796e 34a8 00a0 0000 0d3e  dll...yn4......>
-00002fc0: 50ca f48b 774b 91fb 2967 4f0b 3a38 5379  P...wK..)gO.:8Sy
-00002fd0: 7374 656d 2e49 4f2e 4973 6f6c 6174 6564  stem.IO.Isolated
-00002fe0: 5374 6f72 6167 652e 646c 6c00 0001 ca38  Storage.dll....8
-00002ff0: ecf4 00a0 0000 8f0a f0fe ee42 4441 8218  ...........BDA..
-00003000: e4ee a372 435b 5379 7374 656d 2e49 4f2e  ...rC[System.IO.
-00003010: 4d65 6d6f 7279 4d61 7070 6564 4669 6c65  MemoryMappedFile
-00003020: 732e 646c 6c00 0001 5855 eda0 0080 0000  s.dll...XU......
-00003030: bd62 a1b3 c5f4 0f4e 9b27 47ca 2a73 6180  .b.....N.'G.*sa.
-00003040: 5379 7374 656d 2e49 4f2e 5069 7065 732e  System.IO.Pipes.
-00003050: 4163 6365 7373 436f 6e74 726f 6c2e 646c  AccessControl.dl
-00003060: 6c00 0001 bab8 84bb 0080 0000 3ceb bc81  l...........<...
-00003070: faea 7948 b53b c997 375e 1a81 5379 7374  ..yH.;..7^..Syst
-00003080: 656d 2e49 4f2e 5069 7065 732e 646c 6c00  em.IO.Pipes.dll.
-00003090: 0001 5474 81ae 00a0 0000 7378 db8c 2210  ..Tt......sx..".
-000030a0: fd4b ad05 e9c2 e8b7 e87b 5379 7374 656d  .K.......{System
-000030b0: 2e49 4f2e 556e 6d61 6e61 6765 644d 656d  .IO.UnmanagedMem
-000030c0: 6f72 7953 7472 6561 6d2e 646c 6c00 0001  oryStream.dll...
-000030d0: 4069 d4e0 0080 0000 d41c 571f ea58 a444  @i........W..X.D
-000030e0: 8eb0 6ecb c478 e011 5379 7374 656d 2e4c  ..n..x..System.L
-000030f0: 696e 712e 646c 6c00 0001 32cf 0994 00c0  inq.dll...2.....
-00003100: 0000 33a0 d1ab 6d0d 294d 905c c78f b059  ..3...m.)M.\...Y
-00003110: 7785 5379 7374 656d 2e4c 696e 712e 4578  w.System.Linq.Ex
-00003120: 7072 6573 7369 6f6e 732e 646c 6c00 0001  pressions.dll...
-00003130: 002d 14bd 0040 0100 d08c 373c a5b9 df4c  .-...@....7<...L
-00003140: bfa9 da0c 7221 6f9e 5379 7374 656d 2e4c  ....r!o.System.L
-00003150: 696e 712e 5061 7261 6c6c 656c 2e64 6c6c  inq.Parallel.dll
-00003160: 0000 01fb f43e 9e00 c000 003d 4799 a20e  .....>.....=G...
-00003170: 7ed3 4c86 f7ed f0e0 9c6c 7853 7973 7465  ~.L......lxSyste
-00003180: 6d2e 4c69 6e71 2e51 7565 7279 6162 6c65  m.Linq.Queryable
-00003190: 2e64 6c6c 0000 011f 760b 8600 c000 00ae  .dll....v.......
-000031a0: 7b1d f1d8 11c6 4fae 0116 aea1 cdaa 4d53  {.....O.......MS
-000031b0: 7973 7465 6d2e 4d65 6d6f 7279 2e64 6c6c  ystem.Memory.dll
-000031c0: 0000 016f 05a0 ea00 e000 0072 a6b3 0123  ...o.......r...#
-000031d0: da0a 4d9a da50 9b59 d336 af53 7973 7465  ..M..P.Y.6.Syste
-000031e0: 6d2e 4e65 742e 646c 6c00 0001 43f9 eabe  m.Net.dll...C...
-000031f0: 0080 0000 c9d8 dc65 0efd 7840 b56b 2909  .......e..x@.k).
-00003200: dd5d 9e81 5379 7374 656d 2e4e 6574 2e48  .]..System.Net.H
-00003210: 7474 702e 646c 6c00 0001 dae1 e39c 0020  ttp.dll........ 
-00003220: 0100 5b44 6dce e120 8549 9629 96cd 6adf  ..[Dm.. .I.)..j.
-00003230: b501 5379 7374 656d 2e4e 6574 2e48 7474  ..System.Net.Htt
-00003240: 702e 4a73 6f6e 2e64 6c6c 0000 0169 b5d8  p.Json.dll...i..
-00003250: 9800 8000 0030 8217 8bc1 955d 4d8a 0431  .....0.....]M..1
-00003260: db06 16a8 3853 7973 7465 6d2e 4e65 742e  ....8System.Net.
-00003270: 4874 7470 4c69 7374 656e 6572 2e64 6c6c  HttpListener.dll
-00003280: 0000 01c6 1187 8f00 a000 006c fde1 fa82  ...........l....
-00003290: 68ed 47b3 046a 68ef eda5 7753 7973 7465  h.G..jh...wSyste
-000032a0: 6d2e 4e65 742e 4d61 696c 2e64 6c6c 0000  m.Net.Mail.dll..
-000032b0: 0180 e023 d000 c000 00e7 4861 e834 943a  ...#......Ha.4.:
-000032c0: 4f9d d546 0351 f8de 1353 7973 7465 6d2e  O..F.Q...System.
-000032d0: 4e65 742e 4e61 6d65 5265 736f 6c75 7469  Net.NameResoluti
-000032e0: 6f6e 2e64 6c6c 0000 01c4 01d6 be00 8000  on.dll..........
-000032f0: 00fa d9ed f7b1 f204 44b0 d725 23cf 14a0  ........D..%#...
-00003300: 8c53 7973 7465 6d2e 4e65 742e 4e65 7477  .System.Net.Netw
-00003310: 6f72 6b49 6e66 6f72 6d61 7469 6f6e 2e64  orkInformation.d
-00003320: 6c6c 0000 011a 8961 ed00 c000 0065 5a4d  ll.....a.....eZM
-00003330: 6224 e22e 4e98 c5db 7538 6719 bc53 7973  b$..N...u8g..Sys
-00003340: 7465 6d2e 4e65 742e 5069 6e67 2e64 6c6c  tem.Net.Ping.dll
-00003350: 0000 01d1 651e 8400 8000 00ec 6e76 04b0  ....e.......nv..
-00003360: f9fd 4daf 8f93 d837 9031 fe53 7973 7465  ..M....7.1.Syste
-00003370: 6d2e 4e65 742e 5072 696d 6974 6976 6573  m.Net.Primitives
-00003380: 2e64 6c6c 0000 014e 59b2 8f00 c000 0051  .dll...NY......Q
-00003390: 5f32 bdbd 2228 458f 3dc9 bb72 09eb 6953  _2.."(E.=..r..iS
-000033a0: 7973 7465 6d2e 4e65 742e 5265 7175 6573  ystem.Net.Reques
-000033b0: 7473 2e64 6c6c 0000 013e 7429 8500 e000  ts.dll...>t)....
-000033c0: 005a 6f4c 449b c19e 4c87 0f1d eb1a d6dc  .ZoLD...L.......
-000033d0: b153 7973 7465 6d2e 4e65 742e 5365 6375  .System.Net.Secu
-000033e0: 7269 7479 2e64 6c6c 0000 0143 a011 e200  rity.dll...C....
-000033f0: 0001 00b1 787c f276 548f 4e86 36a2 afc4  ....x|.vT.N.6...
-00003400: 0c39 a253 7973 7465 6d2e 4e65 742e 5365  .9.System.Net.Se
-00003410: 7276 6963 6550 6f69 6e74 2e64 6c6c 0000  rvicePoint.dll..
-00003420: 019f b132 8e00 8000 00ba 9a58 1bdb 8c92  ...2.......X....
-00003430: 46ac c2d1 d921 8aa6 6a53 7973 7465 6d2e  F....!..jSystem.
-00003440: 4e65 742e 536f 636b 6574 732e 646c 6c00  Net.Sockets.dll.
-00003450: 0001 d990 26d0 0000 0100 629c e5d5 2d79  ....&.....b...-y
-00003460: 124c b4cd a08a 27b5 d3ed 5379 7374 656d  .L....'...System
-00003470: 2e4e 6574 2e57 6562 436c 6965 6e74 2e64  .Net.WebClient.d
-00003480: 6c6c 0000 01a7 6b96 d900 a000 006a f69f  ll....k......j..
-00003490: 190b 922e 439b a994 0260 4b11 be53 7973  ....C....`K..Sys
-000034a0: 7465 6d2e 4e65 742e 5765 6248 6561 6465  tem.Net.WebHeade
-000034b0: 7243 6f6c 6c65 6374 696f 6e2e 646c 6c00  rCollection.dll.
-000034c0: 0001 94da 15fd 0080 0000 5211 b004 db9d  ..........R.....
-000034d0: a74a b41c 0bf7 896c e0ca 5379 7374 656d  .J.....l..System
-000034e0: 2e4e 6574 2e57 6562 5072 6f78 792e 646c  .Net.WebProxy.dl
-000034f0: 6c00 0001 673c 8bfc 0080 0000 c312 3fb1  l...g<........?.
-00003500: f4a8 e34c 85e7 34e8 a755 39a3 5379 7374  ...L..4..U9.Syst
-00003510: 656d 2e4e 6574 2e57 6562 536f 636b 6574  em.Net.WebSocket
-00003520: 732e 436c 6965 6e74 2e64 6c6c 0000 0164  s.Client.dll...d
-00003530: 0f7a ae00 8000 00a5 0ddd 9f18 2c4d 41a2  .z..........,MA.
-00003540: 8786 b5b6 b350 c353 7973 7465 6d2e 4e65  .....P.System.Ne
-00003550: 742e 5765 6253 6f63 6b65 7473 2e64 6c6c  t.WebSockets.dll
-00003560: 0000 011f e0d9 c600 a000 0012 3e15 8249  ............>..I
-00003570: 6e65 4aa7 1578 3ec1 9bb1 5353 7973 7465  neJ..x>...SSyste
-00003580: 6d2e 4e75 6d65 7269 6373 2e64 6c6c 0000  m.Numerics.dll..
-00003590: 01a4 7f79 ad00 8000 00c9 48e6 0556 56c7  ...y......H..VV.
-000035a0: 469e 45a6 b779 a3d3 6253 7973 7465 6d2e  F.E..y..bSystem.
-000035b0: 4e75 6d65 7269 6373 2e56 6563 746f 7273  Numerics.Vectors
-000035c0: 2e64 6c6c 0000 016e 49c6 9200 c000 0027  .dll...nI......'
-000035d0: 240e f79e abc9 42b5 6aeb 7120 50bc 7353  $.....B.j.q P.sS
-000035e0: 7973 7465 6d2e 4f62 6a65 6374 4d6f 6465  ystem.ObjectMode
-000035f0: 6c2e 646c 6c00 0001 e694 81ba 00c0 0000  l.dll...........
-00003600: ead3 6238 ab32 bb4c a1f8 6674 1e45 44f1  ..b8.2.L..ft.ED.
-00003610: 5379 7374 656d 2e52 6566 6c65 6374 696f  System.Reflectio
-00003620: 6e2e 4469 7370 6174 6368 5072 6f78 792e  n.DispatchProxy.
-00003630: 646c 6c00 0001 6f18 67af 0080 0000 f03e  dll...o.g......>
-00003640: a54f 1d57 5c4a bc3c 4e0e 342c 59d7 5379  .O.W\J.<N.4,Y.Sy
-00003650: 7374 656d 2e52 6566 6c65 6374 696f 6e2e  stem.Reflection.
-00003660: 646c 6c00 0001 47c3 2c96 0080 0000 239d  dll...G.,.....#.
-00003670: 2ee3 d160 444a b4c5 d800 1271 d86b 5379  ...`DJ.....q.kSy
-00003680: 7374 656d 2e52 6566 6c65 6374 696f 6e2e  stem.Reflection.
-00003690: 456d 6974 2e64 6c6c 0000 01b7 56b4 8000  Emit.dll....V...
-000036a0: e000 00e8 e1a6 3e2d b322 4f95 4afa edde  ......>-."O.J...
-000036b0: 6f9e f353 7973 7465 6d2e 5265 666c 6563  o..System.Reflec
-000036c0: 7469 6f6e 2e45 6d69 742e 494c 4765 6e65  tion.Emit.ILGene
-000036d0: 7261 7469 6f6e 2e64 6c6c 0000 0103 a0c8  ration.dll......
-000036e0: e900 a000 0033 0eb4 e590 27fe 4d9f 723a  .....3....'.M.r:
-000036f0: ab2f c745 3a53 7973 7465 6d2e 5265 666c  ./.E:System.Refl
-00003700: 6563 7469 6f6e 2e45 6d69 742e 4c69 6768  ection.Emit.Ligh
-00003710: 7477 6569 6768 742e 646c 6c00 0001 3ae1  tweight.dll...:.
-00003720: 1097 0080 0000 78a0 3ce2 2b89 7a49 9e60  ......x.<.+.zI.`
-00003730: 8b82 2eb4 043a 5379 7374 656d 2e52 6566  .....:System.Ref
-00003740: 6c65 6374 696f 6e2e 4578 7465 6e73 696f  lection.Extensio
-00003750: 6e73 2e64 6c6c 0000 01ab d82e 9700 8000  ns.dll..........
-00003760: 003d 4b2b 7b68 2d8e 4792 ef1b 1ac6 9d83  .=K+{h-.G.......
-00003770: 9b53 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
-00003780: 6f6e 2e4d 6574 6164 6174 612e 646c 6c00  on.Metadata.dll.
-00003790: 0001 2373 afd6 0020 0200 5415 befe 330e  ..#s... ..T...3.
-000037a0: 1448 a1cb c61d ee8c f9ce 5379 7374 656d  .H........System
-000037b0: 2e52 6566 6c65 6374 696f 6e2e 5072 696d  .Reflection.Prim
-000037c0: 6974 6976 6573 2e64 6c6c 0000 0196 d10b  itives.dll......
-000037d0: c200 a000 0086 8d69 edcb 01c8 4ea6 5987  .......i....N.Y.
-000037e0: 31e3 1149 2653 7973 7465 6d2e 5265 666c  1..I&System.Refl
-000037f0: 6563 7469 6f6e 2e54 7970 6545 7874 656e  ection.TypeExten
-00003800: 7369 6f6e 732e 646c 6c00 0001 f2aa c4f8  sions.dll.......
-00003810: 0080 0000 1f75 8f9e 6f4a 5744 a08f d1e5  .....u..oJWD....
-00003820: e63a 25d9 5379 7374 656d 2e52 6573 6f75  .:%.System.Resou
-00003830: 7263 6573 2e52 6561 6465 722e 646c 6c00  rces.Reader.dll.
-00003840: 0001 ba00 4fb8 0080 0000 1ae6 1cff 8e10  ....O...........
-00003850: 124c ba07 d9d5 baac a67c 5379 7374 656d  .L.......|System
-00003860: 2e52 6573 6f75 7263 6573 2e52 6573 6f75  .Resources.Resou
-00003870: 7263 654d 616e 6167 6572 2e64 6c6c 0000  rceManager.dll..
-00003880: 0199 4f3a e700 8000 0035 4a78 a4fa 9730  ..O:.....5Jx...0
-00003890: 48b3 8d73 43b4 f9c7 0753 7973 7465 6d2e  H..sC....System.
-000038a0: 5265 736f 7572 6365 732e 5772 6974 6572  Resources.Writer
-000038b0: 2e64 6c6c 0000 010c 189b dd00 8000 008b  .dll............
-000038c0: a44d eaed 62f5 4c9b f034 e00d 1fa2 2253  .M..b.L..4...."S
-000038d0: 7973 7465 6d2e 5275 6e74 696d 652e 436f  ystem.Runtime.Co
-000038e0: 6d70 696c 6572 5365 7276 6963 6573 2e55  mpilerServices.U
-000038f0: 6e73 6166 652e 646c 6c00 0001 b18c d9af  nsafe.dll.......
-00003900: 0080 0000 aefe a9de f1c6 5b48 abf8 0d87  ..........[H....
-00003910: 7820 fd9e 5379 7374 656d 2e52 756e 7469  x ..System.Runti
-00003920: 6d65 2e43 6f6d 7069 6c65 7253 6572 7669  me.CompilerServi
-00003930: 6365 732e 5669 7375 616c 432e 646c 6c00  ces.VisualC.dll.
-00003940: 0001 45bd e8ce 0080 0000 f30c 2748 19e5  ..E.........'H..
-00003950: 1947 b304 b2a7 1bee 157c 5379 7374 656d  .G.......|System
-00003960: 2e52 756e 7469 6d65 2e64 6c6c 0000 0116  .Runtime.dll....
-00003970: d16a 8300 8007 0098 bfdf 9864 345b 43a3  .j.........d4[C.
-00003980: 81bb 4c30 1700 1c53 7973 7465 6d2e 5275  ..L0...System.Ru
-00003990: 6e74 696d 652e 4578 7465 6e73 696f 6e73  ntime.Extensions
-000039a0: 2e64 6c6c 0000 0162 ae55 b100 8000 003c  .dll...b.U.....<
-000039b0: b181 0e50 54dc 4481 5bf0 895b 1b12 7553  ...PT.D.[..[..uS
-000039c0: 7973 7465 6d2e 5275 6e74 696d 652e 4861  ystem.Runtime.Ha
-000039d0: 6e64 6c65 732e 646c 6c00 0001 32ed 24c9  ndles.dll...2.$.
-000039e0: 0080 0000 a7e0 c37f 3023 be45 a736 903c  ........0#.E.6.<
-000039f0: 9881 8850 5379 7374 656d 2e52 756e 7469  ...PSystem.Runti
-00003a00: 6d65 2e49 6e74 6572 6f70 5365 7276 6963  me.InteropServic
-00003a10: 6573 2e64 6c6c 0000 0161 1506 ad00 4001  es.dll...a....@.
-00003a20: 0011 07d1 1e55 3202 4f81 5913 18d4 d4d3  .....U2.O.Y.....
-00003a30: 8953 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
-00003a40: 496e 7465 726f 7053 6572 7669 6365 732e  InteropServices.
-00003a50: 5275 6e74 696d 6549 6e66 6f72 6d61 7469  RuntimeInformati
-00003a60: 6f6e 2e64 6c6c 0000 0190 8044 9f00 8000  on.dll.....D....
-00003a70: 00b0 2e5f 0cea c2bd 4cad 9856 9143 d9be  ..._....L..V.C..
-00003a80: 8a53 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
-00003a90: 496e 7472 696e 7369 6373 2e64 6c6c 0000  Intrinsics.dll..
-00003aa0: 0193 f213 b200 c002 00fd 0b54 dd6d 5415  ...........T.mT.
-00003ab0: 4080 90fb b224 74fe ce53 7973 7465 6d2e  @....$t..System.
-00003ac0: 5275 6e74 696d 652e 4c6f 6164 6572 2e64  Runtime.Loader.d
-00003ad0: 6c6c 0000 0117 a796 a700 8000 00b2 45b3  ll............E.
-00003ae0: ab4e b292 4aab 7ad2 c8e1 c402 0e53 7973  .N..J.z......Sys
-00003af0: 7465 6d2e 5275 6e74 696d 652e 4e75 6d65  tem.Runtime.Nume
-00003b00: 7269 6373 2e64 6c6c 0000 01eb 1af2 8300  rics.dll........
-00003b10: a000 001d a599 8948 3f3a 47b5 4a16 fbe0  .......H?:G.J...
-00003b20: 64ec a353 7973 7465 6d2e 5275 6e74 696d  d..System.Runtim
-00003b30: 652e 5365 7269 616c 697a 6174 696f 6e2e  e.Serialization.
-00003b40: 646c 6c00 0001 8c37 e6ed 0080 0000 91b6  dll....7........
-00003b50: e794 8700 cf4c b0a9 359e fe13 a80c 5379  .....L..5.....Sy
-00003b60: 7374 656d 2e52 756e 7469 6d65 2e53 6572  stem.Runtime.Ser
-00003b70: 6961 6c69 7a61 7469 6f6e 2e46 6f72 6d61  ialization.Forma
-00003b80: 7474 6572 732e 646c 6c00 0001 ee53 3a97  tters.dll....S:.
-00003b90: 00a0 0000 9a1c 8065 7120 024a bff7 1113  .......eq .J....
-00003ba0: 69a5 7ad6 5379 7374 656d 2e52 756e 7469  i.z.System.Runti
-00003bb0: 6d65 2e53 6572 6961 6c69 7a61 7469 6f6e  me.Serialization
-00003bc0: 2e4a 736f 6e2e 646c 6c00 0001 5828 6bf9  .Json.dll...X(k.
-00003bd0: 0080 0000 8c3a 3f80 1cd6 a746 b54a 42f9  .....:?....F.JB.
-00003be0: fb1e 0507 5379 7374 656d 2e52 756e 7469  ....System.Runti
-00003bf0: 6d65 2e53 6572 6961 6c69 7a61 7469 6f6e  me.Serialization
-00003c00: 2e50 7269 6d69 7469 7665 732e 646c 6c00  .Primitives.dll.
-00003c10: 0001 4ea6 3e80 0080 0000 761a 5da5 1bc1  ..N.>.....v.]...
-00003c20: e74f 9c28 ae49 fa16 eb2a 5379 7374 656d  .O.(.I...*System
-00003c30: 2e52 756e 7469 6d65 2e53 6572 6961 6c69  .Runtime.Seriali
-00003c40: 7a61 7469 6f6e 2e58 6d6c 2e64 6c6c 0000  zation.Xml.dll..
-00003c50: 0172 75a0 c400 c000 006c 6576 9350 f831  .ru......lev.P.1
-00003c60: 4695 8ce5 dcb1 5114 ff53 7973 7465 6d2e  F.....Q..System.
-00003c70: 5365 6375 7269 7479 2e41 6363 6573 7343  Security.AccessC
-00003c80: 6f6e 7472 6f6c 2e64 6c6c 0000 01c7 c248  ontrol.dll.....H
-00003c90: f100 e000 0045 a216 9be0 4ec6 488f df9c  .....E....N.H...
-00003ca0: 06f0 cac6 b453 7973 7465 6d2e 5365 6375  .....System.Secu
-00003cb0: 7269 7479 2e43 6c61 696d 732e 646c 6c00  rity.Claims.dll.
-00003cc0: 0001 c549 89fc 00c0 0000 34bf a082 4a91  ...I......4...J.
-00003cd0: 914f 9a87 ccc3 a3d7 5e2c 5379 7374 656d  .O......^,System
-00003ce0: 2e53 6563 7572 6974 792e 4372 7970 746f  .Security.Crypto
-00003cf0: 6772 6170 6879 2e41 6c67 6f72 6974 686d  graphy.Algorithm
-00003d00: 732e 646c 6c00 0001 7314 f5c7 0000 0100  s.dll...s.......
-00003d10: abb4 ea41 672c 0446 9ae6 3057 1b90 d6d6  ...Ag,.F..0W....
-00003d20: 5379 7374 656d 2e53 6563 7572 6974 792e  System.Security.
-00003d30: 4372 7970 746f 6772 6170 6879 2e43 6e67  Cryptography.Cng
-00003d40: 2e64 6c6c 0000 01db c47b ad00 c000 00f9  .dll.....{......
-00003d50: 38b0 b695 ebd5 4093 c165 e932 411f 5c53  8.....@..e.2A.\S
-00003d60: 7973 7465 6d2e 5365 6375 7269 7479 2e43  ystem.Security.C
-00003d70: 7279 7074 6f67 7261 7068 792e 4373 702e  ryptography.Csp.
-00003d80: 646c 6c00 0001 334f 7ca6 00a0 0000 d1e9  dll...3O|.......
-00003d90: 39fa 959d b645 890d e759 0a73 a8d9 5379  9....E...Y.s..Sy
-00003da0: 7374 656d 2e53 6563 7572 6974 792e 4372  stem.Security.Cr
-00003db0: 7970 746f 6772 6170 6879 2e45 6e63 6f64  yptography.Encod
-00003dc0: 696e 672e 646c 6c00 0001 5d0b e3f4 00a0  ing.dll...].....
-00003dd0: 0000 45a9 088f 07e1 c446 a214 9c6c b288  ..E......F...l..
-00003de0: 89bd 5379 7374 656d 2e53 6563 7572 6974  ..System.Securit
-00003df0: 792e 4372 7970 746f 6772 6170 6879 2e4f  y.Cryptography.O
-00003e00: 7065 6e53 736c 2e64 6c6c 0000 01d7 53a9  penSsl.dll....S.
-00003e10: e800 8000 007e 3973 abae 085d 499a ca2c  .....~9s...]I..,
-00003e20: 00c9 08aa 5353 7973 7465 6d2e 5365 6375  ....SSystem.Secu
-00003e30: 7269 7479 2e43 7279 7074 6f67 7261 7068  rity.Cryptograph
-00003e40: 792e 5072 696d 6974 6976 6573 2e64 6c6c  y.Primitives.dll
-00003e50: 0000 01f6 9b73 f200 a000 00bc 443b d78b  .....s......D;..
-00003e60: 30e2 4d81 4b0b 88b3 6952 3a53 7973 7465  0.M.K...iR:Syste
-00003e70: 6d2e 5365 6375 7269 7479 2e43 7279 7074  m.Security.Crypt
-00003e80: 6f67 7261 7068 792e 5835 3039 4365 7274  ography.X509Cert
-00003e90: 6966 6963 6174 6573 2e64 6c6c 0000 012f  ificates.dll.../
-00003ea0: 6dd8 c500 e000 0078 0c36 f87f 97a9 49b7  m......x.6....I.
-00003eb0: b9b9 524c bea3 7e53 7973 7465 6d2e 5365  ..RL..~System.Se
-00003ec0: 6375 7269 7479 2e64 6c6c 0000 01aa 2377  curity.dll....#w
-00003ed0: cb00 8000 00b7 dfd9 5176 6172 44a2 0584  ........QvarD...
-00003ee0: 3db5 b833 1153 7973 7465 6d2e 5365 6375  =..3.System.Secu
-00003ef0: 7269 7479 2e50 7269 6e63 6970 616c 2e64  rity.Principal.d
-00003f00: 6c6c 0000 0101 1449 d400 8000 0074 05a8  ll.....I.....t..
-00003f10: a8ed d97b 479e ff72 b99b 713d fa53 7973  ...{G..r..q=.Sys
-00003f20: 7465 6d2e 5365 6375 7269 7479 2e50 7269  tem.Security.Pri
-00003f30: 6e63 6970 616c 2e57 696e 646f 7773 2e64  ncipal.Windows.d
-00003f40: 6c6c 0000 01dc 9ed4 ab00 a000 0080 1fa3  ll..............
-00003f50: 571f e82f 49b3 7ca4 f021 d5bc 5453 7973  W../I.|..!..TSys
-00003f60: 7465 6d2e 5365 6375 7269 7479 2e53 6563  tem.Security.Sec
-00003f70: 7572 6553 7472 696e 672e 646c 6c00 0001  ureString.dll...
-00003f80: a89e 0e9d 0080 0000 6088 0a2d 4b88 704d  ........`..-K.pM
-00003f90: bc75 58a4 0dd6 50a3 5379 7374 656d 2e53  .uX...P.System.S
-00003fa0: 6572 7669 6365 4d6f 6465 6c2e 5765 622e  erviceModel.Web.
-00003fb0: 646c 6c00 0001 b2a6 d9e9 0080 0000 a74f  dll............O
-00003fc0: bdf0 830b 7342 b796 3d76 aa7c 96ec 5379  ....sB..=v.|..Sy
-00003fd0: 7374 656d 2e53 6572 7669 6365 5072 6f63  stem.ServiceProc
-00003fe0: 6573 732e 646c 6c00 0001 5859 7b96 0080  ess.dll...XY{...
-00003ff0: 0000 4ab0 e099 1765 7b49 b7ba 4674 5ceb  ..J....e{I..Ft\.
-00004000: 209d 5379 7374 656d 2e54 6578 742e 456e   .System.Text.En
-00004010: 636f 6469 6e67 2e43 6f64 6550 6167 6573  coding.CodePages
-00004020: 2e64 6c6c 0000 01f9 c988 8c00 8000 0078  .dll...........x
-00004030: 27e6 61f7 adb2 4394 2b9a a7cc 467f e253  '.a...C.+...F..S
-00004040: 7973 7465 6d2e 5465 7874 2e45 6e63 6f64  ystem.Text.Encod
-00004050: 696e 672e 646c 6c00 0001 5682 deec 0080  ing.dll...V.....
-00004060: 0000 e7b3 8f81 9565 de43 b014 87b5 d014  .......e.C......
-00004070: 597b 5379 7374 656d 2e54 6578 742e 456e  Y{System.Text.En
-00004080: 636f 6469 6e67 2e45 7874 656e 7369 6f6e  coding.Extension
-00004090: 732e 646c 6c00 0001 1d9a 87fe 00a0 0000  s.dll...........
-000040a0: ac74 1900 4b7c 7444 8dbf 1fb8 c369 885d  .t..K|tD.....i.]
-000040b0: 5379 7374 656d 2e54 6578 742e 456e 636f  System.Text.Enco
-000040c0: 6469 6e67 732e 5765 622e 646c 6c00 0001  dings.Web.dll...
-000040d0: d474 bd99 00a0 0000 d9b9 ad28 c987 5942  .t.........(..YB
-000040e0: bd65 eedc c872 9636 5379 7374 656d 2e54  .e...r.6System.T
-000040f0: 6578 742e 4a73 6f6e 2e64 6c6c 0000 016f  ext.Json.dll...o
-00004100: d647 d300 2001 0071 c840 fe70 c582 4c9a  .G.. ..q.@.p..L.
-00004110: 4422 d442 2534 fb53 7973 7465 6d2e 5465  D".B%4.System.Te
-00004120: 7874 2e52 6567 756c 6172 4578 7072 6573  xt.RegularExpres
-00004130: 7369 6f6e 732e 646c 6c00 0001 5ba3 88d3  sions.dll...[...
-00004140: 00c0 0000 1e98 62f2 782d 4943 b298 6bb5  ......b.x-IC..k.
-00004150: 201d fa42 5379 7374 656d 2e54 6872 6561   ..BSystem.Threa
-00004160: 6469 6e67 2e43 6861 6e6e 656c 732e 646c  ding.Channels.dl
-00004170: 6c00 0001 293c c68b 0080 0000 debb 5031  l...)<........P1
-00004180: facc b643 87ac e080 c51b 428b 5379 7374  ...C......B.Syst
-00004190: 656d 2e54 6872 6561 6469 6e67 2e64 6c6c  em.Threading.dll
-000041a0: 0000 01e3 b550 8c00 c000 00fb 8355 3df9  .....P.......U=.
-000041b0: 907a 49b6 f68e 9302 3c10 2053 7973 7465  .zI.....<. Syste
-000041c0: 6d2e 5468 7265 6164 696e 672e 4f76 6572  m.Threading.Over
-000041d0: 6c61 7070 6564 2e64 6c6c 0000 01e7 fa52  lapped.dll.....R
-000041e0: d400 8000 0085 5870 af36 c609 4c81 5b0f  ......Xp.6..L.[.
-000041f0: 5f77 6dfb 5d53 7973 7465 6d2e 5468 7265  _wm.]System.Thre
-00004200: 6164 696e 672e 5461 736b 732e 4461 7461  ading.Tasks.Data
-00004210: 666c 6f77 2e64 6c6c 0000 019f 91ad b800  flow.dll........
-00004220: c000 0084 65c6 e353 0f28 45ab b6af ec19  ....e..S.(E.....
-00004230: 36ec ca53 7973 7465 6d2e 5468 7265 6164  6..System.Thread
-00004240: 696e 672e 5461 736b 732e 646c 6c00 0001  ing.Tasks.dll...
-00004250: e93d c3e7 0080 0000 b2c6 707b a68f 654c  .=........p{..eL
-00004260: 9553 331f e298 58fd 5379 7374 656d 2e54  .S3...X.System.T
-00004270: 6872 6561 6469 6e67 2e54 6173 6b73 2e45  hreading.Tasks.E
-00004280: 7874 656e 7369 6f6e 732e 646c 6c00 0001  xtensions.dll...
-00004290: de4a de85 0080 0000 f58b 9c26 9cdd 034f  .J.........&...O
-000042a0: a6c4 ef23 824b 3be3 5379 7374 656d 2e54  ...#.K;.System.T
-000042b0: 6872 6561 6469 6e67 2e54 6173 6b73 2e50  hreading.Tasks.P
-000042c0: 6172 616c 6c65 6c2e 646c 6c00 0001 b2a4  arallel.dll.....
-000042d0: 7ff3 0080 0000 25f6 7953 1072 8645 a233  ......%.yS.r.E.3
-000042e0: a10e e3ee cc25 5379 7374 656d 2e54 6872  .....%System.Thr
-000042f0: 6561 6469 6e67 2e54 6872 6561 642e 646c  eading.Thread.dl
-00004300: 6c00 0001 e9a4 90a1 00a0 0000 f65d 3dde  l............]=.
-00004310: 45d1 064f a0f5 69c3 80a0 8fc1 5379 7374  E..O..i.....Syst
-00004320: 656d 2e54 6872 6561 6469 6e67 2e54 6872  em.Threading.Thr
-00004330: 6561 6450 6f6f 6c2e 646c 6c00 0001 6a4d  eadPool.dll...jM
-00004340: de81 0080 0000 dd2b 5f60 8fe3 7342 a6d5  .......+_`..sB..
-00004350: 47e2 7534 978b 5379 7374 656d 2e54 6872  G.u4..System.Thr
-00004360: 6561 6469 6e67 2e54 696d 6572 2e64 6c6c  eading.Timer.dll
-00004370: 0000 0131 5870 ef00 8000 00d1 389c 58ea  ...1Xp......8.X.
-00004380: 9ae1 4b93 2a4a 50be 5568 b453 7973 7465  ..K.*JP.Uh.Syste
-00004390: 6d2e 5472 616e 7361 6374 696f 6e73 2e64  m.Transactions.d
-000043a0: 6c6c 0000 01a9 f534 e400 8000 002e a551  ll.....4.......Q
-000043b0: da36 8436 4c83 e031 eea3 65ec 2553 7973  .6.6L..1..e.%Sys
-000043c0: 7465 6d2e 5472 616e 7361 6374 696f 6e73  tem.Transactions
-000043d0: 2e4c 6f63 616c 2e64 6c6c 0000 01ee d65f  .Local.dll....._
-000043e0: a900 a000 00db 13e2 954e a38c 4f8b f4f6  .........N..O...
-000043f0: 4a10 767a fe53 7973 7465 6d2e 5661 6c75  J.vz.System.Valu
-00004400: 6554 7570 6c65 2e64 6c6c 0000 015d 3017  eTuple.dll...]0.
-00004410: ab00 8000 00c3 d6d5 4e7d a5ad 4482 499c  ........N}..D.I.
-00004420: 4733 a87e c353 7973 7465 6d2e 5765 622e  G3.~.System.Web.
-00004430: 646c 6c00 0001 0c94 a4b9 0080 0000 8c53  dll............S
-00004440: f813 2625 304b 97d3 a54f f1dc 69b1 5379  ..&%0K...O..i.Sy
-00004450: 7374 656d 2e57 6562 2e48 7474 7055 7469  stem.Web.HttpUti
-00004460: 6c69 7479 2e64 6c6c 0000 01a0 f880 ff00  lity.dll........
-00004470: 8000 00b4 54d9 6960 a3b1 4c8b 5301 16d0  ....T.i`..L.S...
-00004480: 5c69 0453 7973 7465 6d2e 5769 6e64 6f77  \i.System.Window
-00004490: 732e 646c 6c00 0001 5d3d 42bd 0080 0000  s.dll...]=B.....
-000044a0: f3b7 5fad 14d7 9641 bc27 4140 126f 3ed7  .._....A.'A@.o>.
-000044b0: 5379 7374 656d 2e58 6d6c 2e64 6c6c 0000  System.Xml.dll..
-000044c0: 016d 12f6 cf00 a000 00c6 a96f 4641 7c05  .m.........oFA|.
-000044d0: 4397 1b28 6599 83c0 ac53 7973 7465 6d2e  C..(e....System.
-000044e0: 586d 6c2e 4c69 6e71 2e64 6c6c 0000 01c6  Xml.Linq.dll....
-000044f0: d85c ac00 8000 0009 7f13 0fbc e673 4fa4  .\...........sO.
-00004500: 7ea7 a403 0599 3953 7973 7465 6d2e 586d  ~.....9System.Xm
-00004510: 6c2e 5265 6164 6572 5772 6974 6572 2e64  l.ReaderWriter.d
-00004520: 6c6c 0000 01f2 6997 c900 0002 00a8 f2db  ll....i.........
-00004530: 1842 568a 4491 1625 e858 413a 0153 7973  .BV.D..%.XA:.Sys
-00004540: 7465 6d2e 586d 6c2e 5365 7269 616c 697a  tem.Xml.Serializ
-00004550: 6174 696f 6e2e 646c 6c00 0001 e06d b088  ation.dll....m..
-00004560: 0080 0000 430a d75f 9f2a f445 8f5e da9b  ....C.._.*.E.^..
-00004570: f225 c9f3 5379 7374 656d 2e58 6d6c 2e58  .%..System.Xml.X
-00004580: 446f 6375 6d65 6e74 2e64 6c6c 0000 0171  Document.dll...q
-00004590: 032d 8f00 c000 00d3 3e1c e284 2262 49ac  .-......>..."bI.
-000045a0: 0d55 4d66 98f6 0753 7973 7465 6d2e 586d  .UMf...System.Xm
-000045b0: 6c2e 586d 6c44 6f63 756d 656e 742e 646c  l.XmlDocument.dl
-000045c0: 6c00 0001 7a80 57ea 0080 0000 3d03 0ef9  l...z.W.....=...
-000045d0: 441d d44c 81f1 0bf8 39ed aec1 5379 7374  D..L....9...Syst
-000045e0: 656d 2e58 6d6c 2e58 6d6c 5365 7269 616c  em.Xml.XmlSerial
-000045f0: 697a 6572 2e64 6c6c 0000 01d9 9d66 d200  izer.dll.....f..
-00004600: 0001 00da 5853 909f 5ad6 4f95 948e 719d  ....XS..Z.O...q.
-00004610: f238 c053 7973 7465 6d2e 586d 6c2e 5850  .8.System.Xml.XP
-00004620: 6174 682e 646c 6c00 0001 fbf4 20ba 0080  ath.dll..... ...
-00004630: 0000 495b eca5 e2ff 334b a02f 0feb ff7f  ..I[....3K./....
-00004640: e1ae 5379 7374 656d 2e58 6d6c 2e58 5061  ..System.Xml.XPa
-00004650: 7468 2e58 446f 6375 6d65 6e74 2e64 6c6c  th.XDocument.dll
-00004660: 0000 0195 7872 b200 8000 001a ce48 b261  ....xr.......H.a
-00004670: 236d 40b5 a4c8 a88c cdf4 fa55 6e64 6572  #m@........Under
-00004680: 7461 6c65 4d6f 644c 6962 2e64 6c6c 0000  taleModLib.dll..
-00004690: 0162 f29a e300 2003 00c1 84c3 596d 761f  .b.... .....Ymv.
-000046a0: 4997 6ebf 23e5 75fd e757 696e 646f 7773  I.n.#.u..Windows
-000046b0: 4261 7365 2e64 6c6c 0000 014a a478 b800  Base.dll...J.x..
-000046c0: 8000 00d9 f093 acde 50cf 4a98 0af9 7eb7  ........P.J...~.
-000046d0: cb19 ad0b 0000 0024 0505 0600 0104 0006  .......$........
-000046e0: 5379 7374 656d 1a53 7973 7465 6d2e 436f  System.System.Co
-000046f0: 6c6c 6563 7469 6f6e 732e 4765 6e65 7269  llections.Generi
-00004700: 6309 5379 7374 656d 2e49 4f0b 5379 7374  c.System.IO.Syst
-00004710: 656d 2e4c 696e 710f 5379 7374 656d 2e4e  em.Linq.System.N
-00004720: 6574 2e48 7474 7010 5379 7374 656d 2e54  et.Http.System.T
-00004730: 6872 6561 6469 6e67 1653 7973 7465 6d2e  hreading.System.
-00004740: 5468 7265 6164 696e 672e 5461 736b 7315  Threading.Tasks.
-00004750: 01ad df01 ade6 01ae 0101 ae0b 01ae 1701  ................
-00004760: ae27 01ae 380b 0000 000d 0a0b 0700 0104  .'..8...........
-00004770: 750b 0000 0014 0f0b 0800 0104 7510 0000  u...........u...
-00004780: 0018 1009 0a00 2c02 000a 0001 0279 0f55  ......,......y.U
-00004790: 6e64 6572 7461 6c65 4d6f 644c 6962 1a55  ndertaleModLib.U
-000047a0: 6e64 6572 7461 6c65 4d6f 644c 6962 2e44  ndertaleModLib.D
-000047b0: 6563 6f6d 7069 6c65 7216 556e 6465 7274  ecompiler.Undert
-000047c0: 616c 654d 6f64 4c69 622e 4d6f 6465 6c73  aleModLib.Models
-000047d0: 1153 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
-000047e0: 6f6e 1c53 7973 7465 6d2e 5275 6e74 696d  on.System.Runtim
-000047f0: 652e 5365 7269 616c 697a 6174 696f 6e24  e.Serialization$
-00004800: 01ad df01 ade6 01ae 0101 ae0b 01ae 1701  ................
-00004810: ae27 01ae 3801 ae8e 01ae 9e01 aeb9 01ae  .'..8...........
-00004820: d001 aee2 0600 0000 3417 0929 0100 003c  ........4..)...<
-00004830: 1c09 0d00 2602 0009 0011 0408 0300 0702  ....&...........
-00004840: 0801 006a 0479 5500 3c04 7909 0022 0200  ...j.yU.<.y.."..
-00004850: 0c00 0102 7915 0200 003c 2a09 0d00 2b02  ....y....<*...+.
-00004860: 000d 0022 0200 0c00 0102 7915 0200 003c  ..."......y....<
-00004870: 3109 0d00 2a02 000d 0022 0200 0c00 0102  1...*...."......
-00004880: 790b 0000 0024 3809 0c00 0102 790b 0300  y....$8.....y...
-00004890: 0025 3d09 340b 0402 000b 0300 0024 4e09  .%=.4........$N.
-000048a0: 3409 0402 0009 0400 0000 0d05 185e 0947  4............^.G
-000048b0: 0500 005f 6809 2700 1b02 0010 0037 0400  ..._h.'......7..
-000048c0: 0600 1d02 000c 004c 0200 0600 3802 001b  .......L....8...
-000048d0: 0014 0200 0700 1d02 000c 001a 0200 0700  ................
-000048e0: 1e02 0010 0022 0400 0700 5f02 0024 001b  ....."...._..$..
-000048f0: 0200 1000 0102 7980 8606 0000 1909 0908  ......y.........
-00004900: 0007 0208 0100 3c06 7907 006f 0600 2400  ......<.y..o..$.
-00004910: 5902 081b 0069 0479 2400 5302 081b 001b  Y....i.y$.S.....
-00004920: 062c 0e00 0002 000d 005f 0300 2b02 7715  .,......._..+.w.
-00004930: 0000 0400 027f 2606 0009 0832 0700 0002  ......&....2....
-00004940: 0023 0033 1c00 3b04 7719 0059 0208 2400  .#.3..;.w..Y..$.
-00004950: 027b 4a0b 0000 0e00 1c0e 5b0e 0000 0200  .{J.......[.....
-00004960: 0d00 5f05 002b 0477 1c00 1b02 0009 001b  .._..+.w........
-00004970: 0208 0900 0004 0002 791e 0600 010c 4b1f  ........y.....K.
-00004980: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
-00004990: 6373 2e43 6f64 6541 6e61 6c79 7369 7318  cs.CodeAnalysis.
-000049a0: 01ad df01 ade6 01ae 0101 ae0b 01ae 1701  ................
-000049b0: ae27 01ae 3801 b07f 1507 0000 461a 0910  .'..8.......F...
-000049c0: 0015 0200 0300 0a00 2c06 003d 0455 1453  ........,..=.U.S
-000049d0: 7973 7465 6d2e 476c 6f62 616c 697a 6174  ystem.Globalizat
-000049e0: 696f 6e10 5379 7374 656d 2e54 6578 742e  ion.System.Text.
-000049f0: 4a73 6f6e 154e 6174 7572 616c 536f 7274  Json.NaturalSort
-00004a00: 2e45 7874 656e 7369 6f6e 1453 6978 4c61  .Extension.SixLa
-00004a10: 626f 7273 2e49 6d61 6765 5368 6172 7020  bors.ImageSharp 
-00004a20: 5369 784c 6162 6f72 732e 496d 6167 6553  SixLabors.ImageS
-00004a30: 6861 7270 2e46 6f72 6d61 7473 2e50 6e67  harp.Formats.Png
-00004a40: 2153 6978 4c61 626f 7273 2e49 6d61 6765  !SixLabors.Image
-00004a50: 5368 6172 702e 5069 7865 6c46 6f72 6d61  Sharp.PixelForma
-00004a60: 7473 1f53 6978 4c61 626f 7273 2e49 6d61  ts.SixLabors.Ima
-00004a70: 6765 5368 6172 702e 5072 6f63 6573 7369  geSharp.Processi
-00004a80: 6e67 1059 414d 535f 4c49 422e 7061 7463  ng.YAMS_LIB.patc
-00004a90: 6865 7314 5941 4d53 5f4c 4942 2e70 6174  hes.YAMS_LIB.pat
-00004aa0: 6368 6573 2e71 6f6c 3e01 addf 01ad e601  ches.qol>.......
-00004ab0: ae01 01ae 0b01 ae17 01ae 2701 ae38 01b0  ..........'..8..
-00004ac0: ce01 aed0 01b0 e301 b0f4 01b1 0a01 b11f  ................
-00004ad0: 01b1 4001 b162 01ae 8e01 ae9e 01ae b901  ..@..b..........
-00004ae0: b182 01b1 9303 1c98 ca08 0000 0006 003a  ...............:
-00004af0: 2d09 0a00 5c04 000d 001d 0e00 0a00 3104  -...\.........1.
-00004b00: 0e0d 001e 047b 0f00 0102 7902 0000 0b00  .....{....y.....
-00004b10: 0001 0025 0400 0a00 3d02 0010 0057 0600  ...%....=....W..
-00004b20: 1a00 4002 000c 004e 0080 820b 0037 08bf  ..@....N.....7..
-00004b30: 7f0b 0011 0400 0700 0d00 2607 0016 001e  ..........&.....
-00004b40: 0700 4502 3d15 0049 0200 0b00 4902 0020  ..E.=..I....I.. 
-00004b50: 002b 0200 1500 635c 001f 0024 020e 0700  .+....c\...$....
-00004b60: 2c04 7b12 0060 0200 1d00 0102 7902 0000  ,.{..`......y...
-00004b70: 0b00 0001 0000 0700 6008 0826 004e 0200  ........`..&.N..
-00004b80: 2700 8084 0200 1900 5302 0021 004a 0200  '.......S..!.J..
-00004b90: 2200 6402 0014 0024 020e 0700 2904 7b0e  ".d....$....).{.
-00004ba0: 0039 0200 1d00 0102 7902 0000 0b00 0001  .9......y.......
-00004bb0: 0062 0400 2600 5002 0027 0080 8902 0019  .b..&.P..'......
-00004bc0: 0055 0200 2100 4c02 0022 0068 0200 1400  .U..!.L..".h....
-00004bd0: 2402 0e07 002a 047b 0e00 3a02 001d 0001  $....*.{..:.....
-00004be0: 0279 0200 000b 0000 0100 7222 7939 0078  .y........r"y9.x
-00004bf0: 0200 3900 7802 0039 007e 0200 3900 6b02  ..9.x..9.~..9.k.
-00004c00: 0039 0080 a602 0054 0080 a602 0054 0080  .9.....T.....T..
-00004c10: a602 0054 0080 a602 0054 0080 a602 0054  ...T.....T.....T
-00004c20: 0080 a602 0054 0080 a602 0054 0181 3604  .....T.....T..6.
-00004c30: 0054 0181 2204 0054 0181 1204 0054 0181  .T.."..T.....T..
-00004c40: 0e04 0054 0080 a508 0049 0080 a702 0049  ...T.....I.....I
-00004c50: 0080 a102 0049 0080 a302 0049 0080 a502  .....I.....I....
-00004c60: 0049 0080 9f02 0049 0080 a802 0049 0080  .I.....I.....I..
-00004c70: aa02 0049 0080 a402 0049 0075 0600 4400  ...I.....I.u..D.
-00004c80: 7802 0044 0076 0200 4400 7602 0044 007b  x..D.v..D.v..D.{
-00004c90: 0200 4400 80a2 0600 4900 80a0 0200 4900  ..D.....I.....I.
-00004ca0: 80a2 0200 4900 80a2 0200 4900 809f 0200  ....I.....I.....
-00004cb0: 4900 809c 0200 4900 809e 0200 4900 809d  I.....I.....I...
-00004cc0: 0200 4900 80a4 0200 4900 809e 0200 4900  ..I.....I.....I.
-00004cd0: 80a0 0200 4900 80a0 0200 4900 809e 0200  ....I.....I.....
-00004ce0: 4900 809e 0200 4900 809f 0200 4900 809d  I.....I.....I...
-00004cf0: 0200 4900 80a4 0200 4900 809d 0200 4900  ..I.....I.....I.
-00004d00: 809d 0200 4900 809d 0200 4900 80a6 0200  ....I.....I.....
-00004d10: 4900 80a6 0200 4900 80a5 0200 4900 80ab  I.....I.....I...
-00004d20: 0200 4900 80a8 0200 4900 80aa 0200 4900  ..I.....I.....I.
-00004d30: 809e 0200 4900 3206 001f 0080 9902 0049  ....I.2........I
-00004d40: 0080 9902 0049 0080 9902 0049 0080 9902  .....I.....I....
-00004d50: 0049 0080 9902 0049 0080 9902 0049 0080  .I.....I.....I..
-00004d60: 9902 0049 0080 9902 0049 0080 9902 0049  ...I.....I.....I
-00004d70: 0506 1600 7d04 060e 006f 0406 0c00 6f04  ....}....o....o.
-00004d80: 060c 006f 0406 0c00 6f04 060c 006f 0406  ...o....o....o..
-00004d90: 0c00 6f04 060a 006f 0406 0c00 6f05 060c  ..o....o....o...
-00004da0: 006f 0406 0e00 6f04 060c 006f 0406 0c00  .o....o....o....
-00004db0: 6f05 060c 007d 0506 0e00 7d00 390e 001f  o....}....}.9...
-00004dc0: 0067 0200 2500 3904 001f 0067 0200 2500  .g..%.9....g..%.
-00004dd0: 8095 0400 490a 0604 0081 1137 0618 008a  ....I......7....
-00004de0: 6604 0672 006f 0406 0c00 6f04 060c 006f  f..r.o....o....o
-00004df0: 0406 0c00 6f00 2f0c 000b 002f 0200 0b05  ....o./..../....
-00004e00: 0606 007f 0023 1200 0b00 2d06 000b 0032  .....#....-....2
-00004e10: 0200 0b00 3202 000b 0036 0200 0b00 3302  ....2....6....3.
-00004e20: 000b 0034 0200 0b00 3302 000b 0035 0200  ...4....3....5..
-00004e30: 0b00 3002 000b 0032 0200 0b00 3402 000b  ..0....2....4...
-00004e40: 0031 0200 0b00 3202 000b 002a 0200 0b00  .1....2....*....
-00004e50: 2e02 000b 0030 0200 0b00 3102 000b 0030  .....0....1....0
-00004e60: 0200 0b00 3002 000b 002c 0200 0b00 3002  ....0....,....0.
-00004e70: 000b 002e 0200 0b00 2f02 000b 002f 0200  ......../..../..
-00004e80: 0b00 2e02 000b 0036 0200 0b00 2e02 000b  .......6........
-00004e90: 0031 0200 0b00 3102 000b 002e 0200 0b00  .1....1.........
-00004ea0: 2d02 000b 002f 0200 0b00 2e02 000b 002b  -..../.........+
-00004eb0: 0600 0b00 3102 000b 002e 0200 0b00 3002  ....1.........0.
-00004ec0: 000b 002c 0200 0b00 3102 000b 002e 0200  ...,....1.......
-00004ed0: 0b00 2e02 000b 002e 0200 0b00 3302 000b  ............3...
-00004ee0: 002f 0200 0b00 2f02 000b 002f 0200 0b00  ./..../..../....
-00004ef0: 2d02 000b 0030 0200 0b00 2f02 000b 002f  -....0..../..../
-00004f00: 0200 0b00 2f02 000b 0037 0200 0b00 3502  ..../....7....5.
-00004f10: 000b 0031 0200 0b00 3302 000b 0032 0200  ...1....3....2..
-00004f20: 0b00 3202 000b 002f 0200 0b00 2c02 000b  ..2..../....,...
-00004f30: 002f 0800 0b00 3202 000b 002a 0200 0b00  ./....2....*....
-00004f40: 2f02 000b 0030 0200 0b00 3002 000b 002e  /....0....0.....
-00004f50: 0200 0b00 3102 000b 002f 0200 0b00 2e02  ....1..../......
-00004f60: 000b 0031 0200 0b00 3102 000b 002e 0200  ...1....1.......
-00004f70: 0b00 3202 000b 002d 0200 0b00 2908 000b  ..2....-....)...
-00004f80: 002f 1e00 0d00 2b04 7621 0000 0200 2a00  ./....+.v!....*.
-00004f90: 2509 005f 0477 1700 027d 600b 0000 0b00  %.._.w...}`.....
-00004fa0: 0001 0030 0e11 0d00 6004 7640 0000 0200  ...0....`.v@....
-00004fb0: 2a00 2509 0060 0477 1700 027d 600b 0000  *.%..`.w...}`...
-00004fc0: 0b00 0001 002d 0e11 0d00 8081 044e 4200  .....-.......NB.
-00004fd0: 0002 0016 004d 0900 5304 7717 0002 7d38  .....M..S.w...}8
-00004fe0: 0b00 000e 0023 0e39 0d00 3404 4423 0000  .....#.9..4.D#..
-00004ff0: 0200 1100 5707 003c 0477 1200 5502 002c  ....W..<.w..U..,
-00005000: 0000 0600 027b 2e08 0068 1043 1600 8082  .....{...h.C....
-00005010: 0400 1f00 6702 0025 0504 0800 4400 8081  ....g..%....D...
-00005020: 0c00 2100 5502 000b 0025 0200 1000 3702  ..!.U....%....7.
-00005030: 000c 005c 0200 0700 3102 0008 004f 0200  ...\....1....O..
-00005040: 0700 2402 0008 0034 0200 0e00 3002 0007  ..$....4....0...
-00005050: 007d 0200 2200 7402 000c 0023 0200 1100  .}..".t....#....
-00005060: 3502 000c 003c 0200 0700 2f02 0009 0035  5....<..../....5
-00005070: 0200 0700 2402 0008 0034 0200 0e00 2e02  ....$....4......
-00005080: 0007 0027 0200 1000 5804 0017 0034 0600  ...'....X....4..
-00005090: 1b00 3502 001c 005a 0600 1500 5602 0010  ..5....Z....V...
-000050a0: 0180 d202 0025 0181 ca08 0025 0080 8708  .....%.....%....
-000050b0: 001f 0059 0600 1f00 5306 0015 005e 0200  ...Y....S....^..
-000050c0: 0a00 5802 001f 0055 0600 1f00 808f 0600  ..X....U........
-000050d0: 2500 8088 0200 2502 80a6 0600 2502 80a6  %.....%.....%...
-000050e0: 0a00 2500 770a 0025 0080 8704 0025 0080  ..%.w..%.....%..
-000050f0: 9d06 0025 005c 0600 1f00 5a02 001f 0047  ...%.\....Z....G
-00005100: 0600 1700 8089 0200 1200 8081 0200 1200  ................
-00005110: 8083 0200 1200 7e02 0012 0060 0232 2a00  ......~....`.2*.
-00005120: 0002 000c 0061 0700 4704 7722 0047 0200  .....a..G.w".G..
-00005130: 2200 0006 0002 7b24 0801 809a 0e55 2500  ".....{$.....U%.
-00005140: 6706 0025 0058 0600 1f00 8084 0200 2500  g..%.X........%.
-00005150: 7306 001f 0073 0200 1f00 7302 001f 006e  s....s....s....n
-00005160: 0200 1f00 7302 001f 004e 0638 1b00 0002  ....s....N.8....
-00005170: 000f 005b 0700 3c04 771c 0000 0600 027d  ...[..<.w......}
-00005180: 2a08 0080 a60c 4f1f 0e12 0200 2501 8104  *.....O.....%...
-00005190: 1e00 2511 1204 0025 002d 2800 1200 6700  ..%....%.-(...g.
-000051a0: 5c25 0180 da06 251f 0068 0400 1f00 7606  \%....%..h....v.
-000051b0: 0025 007d 0200 2500 7402 0025 0080 9c06  .%.}..%.t..%....
-000051c0: 001f 0080 9702 001f 0080 9702 001f 005e  ...............^
-000051d0: 0600 2500 6002 0025 055d 0638 6600 0002  ..%.`..%.].8f...
-000051e0: 000f 005b 0700 330e 771c 0000 0600 0273  ...[..3.w......s
-000051f0: 2a08 0080 8f14 4f1f 0181 1a06 0025 0380  *.....O......%..
-00005200: e208 0025 0071 0e00 2500 3702 0007 0056  ...%.q..%.7....V
-00005210: 0200 1c02 6c02 000c 0024 0600 1100 4502  ....l....$....E.
-00005220: 0020 0056 0200 0700 2a02 0009 0049 0200  . .V....*....I..
-00005230: 0700 2002 000c 0028 0200 0e00 2402 0007  .. ....(....$...
-00005240: 0781 220c 0007 0180 f612 382b 0000 0200  ..".......8+....
-00005250: 0f00 5b07 0053 0677 1f00 0006 0002 7b2a  ..[..S.w......{*
-00005260: 0800 6a0e 4f25 0029 0600 0700 5d02 3017  ..j.O%.)....].0.
-00005270: 0000 0200 0b00 6307 002e 0477 0f00 3100  ......c....w..1.
-00005280: 5e2f 0000 0600 027d 4508 0480 900a 5731  ^/.....}E.....W1
-00005290: 0480 860a 0031 0025 0c00 0700 1d02 301b  .....1.%......0.
-000052a0: 0000 0200 0b00 6307 002e 0477 0f00 2d00  ......c....w..-.
-000052b0: 5e2f 0000 0600 027d 4508 0480 880a 5731  ^/.....}E.....W1
-000052c0: 047e 0a00 3109 808a 1000 1f00 5d16 0025  .~..1.......]..%
-000052d0: 005d 0200 2500 6006 0025 0080 9d06 0025  .]..%.`..%.....%
-000052e0: 004e 0600 1f00 5506 381b 0000 0200 0f00  .N....U.8.......
-000052f0: 5b07 007b 0477 2200 0006 0002 7d2a 0800  [..{.w".....}*..
-00005300: 808c 0c4f 2501 7406 0025 1780 9e08 0025  ...O%.t..%.....%
-00005310: 007a 3400 2200 7c02 0022 0021 0200 1100  .z4.".|..".!....
-00005320: 2202 0011 0906 0200 7809 0614 007b 005c  ".......x....{.\
-00005330: 1800 1f00 8080 0800 2200 2402 0011 003a  ........".$....:
-00005340: 0200 1500 808b 0200 3700 4706 0017 0048  ........7.G....H
-00005350: 0200 2d00 4802 002d 0048 0200 2a00 4602  ..-.H..-.H..*.F.
-00005360: 0029 0046 0200 2c00 4602 002c 0046 0200  .).F..,.F..,.F..
-00005370: 2900 4402 0027 0046 0800 1700 0b02 0a07  ).D..'.F........
-00005380: 0000 0500 3304 7f07 0035 0200 2800 1a02  ....3....5..(...
-00005390: 0009 002b 0400 0700 4d02 0049 0043 0200  ...+....M..I.C..
-000053a0: 1d00 1802 0011 0023 0200 0d00 4f02 0007  .......#....O...
-000053b0: 0017 0200 0900 4302 0007 001b 0200 0e00  ......C.........
-000053c0: 1c02 0007 002e 0400 0700 5502 0049 001b  ..........U..I..
-000053d0: 0200 1100 2602 000d 002f 0200 0700 1a02  ....&..../......
-000053e0: 0009 0029 0200 0700 1a02 000c 001b 0200  ...)............
-000053f0: 0e00 1f02 0007 001b 0200 1100 034b 3006  .............K0.
-00005400: 0008 006d 0c0e 5a3e 5d12 004e 1e00 2500  ...m..Z>]..N..%.
-00005410: 4e02 0025 0030 0600 0700 4802 001c 5d46  N..%.0....H...]F
-00005420: 0200 0c00 1d80 bc00 1100 7102 0037 0181  ..........q..7..
-00005430: 7a06 0012 0181 7a04 0012 0465 0830 3300  z.....z....e.03.
-00005440: 0002 000b 0063 0700 3b0c 7722 0000 0600  .....c..;.w"....
-00005450: 0275 2208 0465 1406 3b00 0002 000b 0063  .u"..e..;......c
-00005460: 0700 620c 7722 0000 0600 0275 2208 0047  ..b.w".....u"..G
-00005470: 1457 1700 4202 0012 0047 0200 1200 8092  .W..B....G......
-00005480: 0200 2500 8092 0200 2501 6802 0025 005f  ..%.....%.h..%._
-00005490: 0400 1500 7102 0011 006f 0200 1100 8088  ....q....o......
-000054a0: 0200 1101 809e 0200 1100 808c 0400 1000  ................
-000054b0: 6d02 0025 0021 0600 1000 4106 0815 005c  m..%.!....A....\
-000054c0: 0200 1700 5c02 0017 005a 0200 1700 5b02  ....\....Z....[.
-000054d0: 0017 004e 0200 1700 4802 0017 0050 0200  ...N....H....P..
-000054e0: 1700 5c02 002f 0055 0200 2f00 5602 0030  ..\../.U../.V..0
-000054f0: 0055 0200 2f00 5502 002f 0056 0200 3000  .U../.U../.V..0.
-00005500: 5602 0030 0056 0200 3000 5602 002c 0052  V..0.V..0.V..,.R
-00005510: 0400 2900 4902 0029 0052 0200 2900 7a04  ..).I..).R..).z.
-00005520: 0022 0065 0200 0c00 2102 0011 0070 0200  .".e....!....p..
-00005530: 2a00 6802 000f 003e 0600 1500 6002 002f  *.h....>....`../
-00005540: 0058 0200 2e00 5a02 0030 0059 0200 2f00  .X....Z..0.Y../.
-00005550: 5a02 0030 0059 0200 2f00 5a02 0030 005a  Z..0.Y../.Z..0.Z
-00005560: 0200 3000 4f06 0029 0046 0200 2900 4f02  ..0.O..).F..).O.
-00005570: 0029 0045 0400 1000 7704 0022 0063 0200  .).E....w..".c..
-00005580: 0c00 1e02 0011 006e 0200 2a00 5d06 0030  .......n..*.]..0
-00005590: 0040 0800 1700 5d02 002d 0056 0200 2d00  .@....]..-.V..-.
-000055a0: 5702 002e 0057 0200 2d00 5602 002d 0057  W....W..-.V..-.W
-000055b0: 0200 2e00 5702 002e 0058 0200 2e00 5708  ....W....X....W.
-000055c0: 0038 0056 0200 3800 5e02 0032 0050 0400  .8.V..8.^..2.P..
-000055d0: 2700 4702 0027 0050 0200 2700 4804 0011  '.G..'.P..'.H...
-000055e0: 0079 0400 2200 6502 000c 0020 0200 1100  .y..".e.... ....
-000055f0: 7102 0028 0044 0600 1700 6202 0030 005a  q..(.D....b..0.Z
-00005600: 0200 2f00 5c02 0031 005b 0200 3000 5c02  ../.\..1.[..0.\.
-00005610: 0031 005b 0200 3000 5c02 0031 005c 0200  .1.[..0.\..1.\..
-00005620: 3100 5f08 0038 005f 0200 3800 5f02 0038  1._..8._..8._..8
-00005630: 005f 0200 3800 6f02 0043 0055 0400 2a00  ._..8.o..C.U..*.
-00005640: 4c02 002a 0055 0200 2a00 7d04 0022 0067  L..*.U..*.}..".g
-00005650: 0200 0c00 2402 0011 0079 0200 2b00 4904  ....$....y..+.I.
-00005660: 0011 0080 8808 0025 0080 8802 0025 0180  .......%.....%..
-00005670: 9404 0025 0080 8806 0025 0080 8802 0025  ...%.....%.....%
-00005680: 0080 8802 0025 0080 8802 0025 0080 8802  .....%.....%....
-00005690: 0025 0080 8604 0025 0080 8602 0025 0080  .%.....%.....%..
-000056a0: 8602 0025 0080 8802 0025 0181 9208 7925  ...%.....%....y%
-000056b0: 0181 9204 0025 0181 9204 0025 0181 9204  .....%.....%....
-000056c0: 0025 0281 7008 001f 003b 0a00 1500 4302  .%..p....;....C.
-000056d0: 0007 0010 0200 0900 1002 0009 0014 0200  ................
-000056e0: 0c00 1402 000c 0033 0200 2400 4102 001c  .......3..$.A...
-000056f0: 0031 0200 0700 5602 001c 006e 0200 0c00  .1....V....n....
-00005700: 1e02 0011 0025 0200 0900 2302 000d 0b06  .....%....#.....
-00005710: 0200 8088 0b06 1800 808a 007b 1c00 2502  ...........{..%.
-00005720: 8098 0600 4b00 4a0a 0015 0063 0200 1100  ....K.J....c....
-00005730: 6f06 0010 005b 0600 2500 5b02 0025 0180  o....[..%.[..%..
-00005740: 9406 0025 0181 2a0e 000c 006c 0a00 1200  ...%..*....l....
-00005750: 8080 0200 1200 5402 0012 0069 0200 1200  ......T....i....
-00005760: 4e02 0012 0060 0200 1200 6702 0012 0051  N....`....g....Q
-00005770: 0600 1502 8156 0200 1000 4c06 0015 0068  .....V....L....h
-00005780: 0200 100b 1208 0012 084e 1800 1208 4e12  .........N....N.
-00005790: 0012 0a4e 1200 120b 121a 0012 084e 1800  ...N.........N..
-000057a0: 1208 4e12 0012 0a4e 1200 120a 121a 0012  ..N....N........
-000057b0: 084e 1600 1208 4e12 0012 0a4e 1200 1200  .N....N....N....
-000057c0: 521a 0015 0080 9502 0011 0180 b602 0011  R...............
-000057d0: 0181 2408 0011 095a 0800 1100 5914 0010  ..$....Z....Y...
-000057e0: 0281 280e 000c 003b 0a00 0c00 6a06 000c  ..(....;....j...
-000057f0: 007f 0600 2400 8083 0200 2a01 812a 0600  ....$.....*..*..
-00005800: 0c01 80cc 0800 0c00 6404 0017 0862 0200  ........d....b..
-00005810: 1200 6712 0012 006e 0400 1708 6c02 0012  ..g....n....l...
-00005820: 0071 1200 1200 6404 0017 085e 0200 1200  .q....d....^....
-00005830: 6712 0012 0065 0400 1708 5e02 0012 0064  g....e....^....d
-00005840: 1200 1200 4e06 000c 0181 1002 0025 0080  ....N........%..
-00005850: a304 0025 0f80 9e02 0025 007d 2400 0c00  ...%.....%.}$...
-00005860: 80af 0200 1f00 80be 0200 2500 3702 000d  ..........%.7...
-00005870: 0061 0408 1200 8093 0200 2c00 8094 0200  .a........,.....
-00005880: 2c02 814a 0879 0c1e 5a0a 0012 0181 003e  ,..J.y..Z......>
-00005890: 0012 007a 0800 2500 5a06 0017 004e 0200  ...z..%.Z....N..
-000058a0: 1200 5902 0017 0047 0200 1205 6504 304b  ..Y....G....e.0K
-000058b0: 0000 0200 0b00 6307 004f 0e77 2200 0006  ......c..O.w"...
-000058c0: 0002 7322 0800 4f14 571b 000c 023e 1100  ..s"..O.W....>..
-000058d0: 0002 0012 0055 0700 6004 4632 0000 0200  .....U..`.F2....
-000058e0: 1b00 4307 004c 0477 1500 027d 420b 0000  ..C..L.w...}B...
-000058f0: 0b00 0001 0002 7d67 0b00 000b 0000 0100  ......}g........
-00005900: 4b14 4912 0052 0200 1200 4c06 0012 0053  K.I..R....L....S
-00005910: 0200 1201 80da 023e 3500 0002 0012 0055  .......>5......U
-00005920: 0700 4006 7710 0002 7b30 0b00 000b 0000  ..@.w...{0......
-00005930: 0100 4a0e 4912 0051 0200 1200 7502 0025  ..J.I..Q....u..%
-00005940: 005b 0600 1700 4902 0012 004f 0200 1202  .[....I....O....
-00005950: 8096 0240 3500 0002 0013 0053 0700 3c08  ...@5......S..<.
-00005960: 7710 0002 7932 0b00 000b 0000 0100 5a10  w...y2........Z.
-00005970: 4717 0048 0200 1200 4e02 0012 0465 0230  G..H....N....e.0
-00005980: 3300 0002 000b 0063 0700 4f0c 7722 0000  3......c..O.w"..
-00005990: 0600 0275 2208 004c 1457 1200 5202 0012  ...u"..L.W..R...
-000059a0: 0280 9602 4035 0000 0200 1300 5307 0045  ....@5......S..E
-000059b0: 0877 1000 0279 320b 0000 0b00 0001 004f  .w...y2........O
-000059c0: 1047 1200 5502 0012 0180 d602 4035 0000  .G..U.......@5..
-000059d0: 0200 1300 5307 0048 0677 1000 027b 320b  ....S..H.w...{2.
-000059e0: 0000 0b00 0001 004d 1047 1200 5402 0012  .......M.G..T...
-000059f0: 0765 0230 809c 0000 0200 0b00 6307 0055  .e.0........c..U
-00005a00: 1277 2200 0006 0002 6f22 0800 4a1c 5712  .w".....o"..J.W.
-00005a10: 0050 0200 1206 6504 3080 8a00 0002 000b  .P....e.0.......
-00005a20: 0063 0700 5110 7722 0000 0600 0271 2208  .c..Q.w".....q".
-00005a30: 0055 1857 1700 4702 0012 004f 0200 1200  .U.W..G....O....
-00005a40: 4706 0012 004f 0200 1200 808c 0230 2b00  G....O.......0+.
-00005a50: 0002 000b 0063 0700 5604 7722 0000 0600  .....c..V.w"....
-00005a60: 027d 2208 0047 0c57 1200 4f02 0012 0047  .}"..G.W..O....G
-00005a70: 0600 1200 4f02 0012 0047 0600 1200 4f02  ....O....G....O.
-00005a80: 0012 0858 0600 1208 5a12 0012 085a 1200  ...X....Z....Z..
-00005a90: 1212 5a12 0012 085a 2800 1200 80a8 1600  ..Z....Z(.......
-00005aa0: 7e00 6606 0025 0065 0200 1f00 5f02 001f  ~.f..%.e...._...
-00005ab0: 0065 0600 2500 8083 0400 1f00 3f06 000c  .e..%.......?...
-00005ac0: 004e 0200 1504 80f6 0200 1010 80a6 0e00  .N..............
-00005ad0: 1f00 6e22 0025 0780 a202 001f 2780 aa10  ..n".%......'...
-00005ae0: 0025 0780 a250 001f 0067 1000 1f08 8092  .%...P...g......
-00005af0: 0200 1f01 80a6 1200 2500 3408 0007 0052  ........%.4....R
-00005b00: 0200 1c2d 4e02 000c 0021 5c00 1100 7b02  ...-N....!\...{.
-00005b10: 0037 0034 0400 0700 5202 001c 324e 0200  .7.4....R...2N..
-00005b20: 0c00 2166 0011 007b 0200 3700 4304 0015  ..!f...{..7.C...
-00005b30: 0080 8002 0011 002d 0200 1100 3702 0010  .......-....7...
-00005b40: 0043 0400 1500 2d02 0011 0074 0200 1100  .C....-....t....
-00005b50: 7102 0011 0d44 0200 1100 80a1 2000 7d04  q....D...... .}.
-00005b60: 6002 0010 0052 1000 1500 3402 0011 007b  `....R....4....{
-00005b70: 0200 1000 6e04 302b 0000 0200 0b00 6307  ....n.0+......c.
-00005b80: 003e 0477 2200 0006 0002 7d22 0800 400c  .>.w".....}"..@.
-00005b90: 5724 0044 0200 2400 8081 0600 4a00 809c  W$.D..$.....J...
-00005ba0: 0200 3c00 4206 000c 0064 0200 2508 1202  ..<.B....d..%...
-00005bb0: 001f 0022 1600 0300 2002 0003 0020 0200  ...".... .... ..
-00005bc0: 0300 4802 000c 0018 0254 0d00 0005 001d  ..H......T......
-00005bd0: 003f 1c00 1d04 7704 000d 0200 0400 0080  .?....w.........
-00005be0: b600 5806 103f 0180 e802 0080 8500 0604  ..X..?..........
-00005bf0: 0005 0019 0600 0700 7c04 0017 0027 0408  ........|....'..
-00005c00: 0700 7606 7917 0021 0080 ee07 0061 04bf  ..v.y..!.....a..
-00005c10: 133f 001c 0200 0300 0602 0005 0017 0600  .?..............
-00005c20: 0700 8084 0400 1700 2504 0807 007e 0679  ........%....~.y
-00005c30: 1700 1f00 80fe 0700 6304 bf03 3f00 1a02  ........c...?...
-00005c40: 0003 0006 0200 0500 1708 0007 0076 0400  .............v..
-00005c50: 1700 2500 80ee 0700 7004 bf13 1700 1f00  ..%.....p.......
-00005c60: 80e2 0700 5d04 bf1f 3f00 1a02 0003 0006  ....]...?.......
-00005c70: 0200 0500 0004 0023 0e0e 1c00 4702 7312  .......#....G.s.
-00005c80: 0006 0200 0500 5c06 003f 0006 0200 0500  ......\..?......
-00005c90: 6404 003f 0006 0200 0500 6604 003f 0006  d..?......f..?..
-00005ca0: 0200 0500 6204 003f 0006 0200 0500 5e04  ....b..?......^.
-00005cb0: 003f 0006 0200 0500 5c04 003f 0006 0200  .?......\..?....
-00005cc0: 0500 6404 003f 0006 0200 0500 1204 0005  ..d..?..........
-00005cd0: 0054 0026 1200 1204 5b08 005a 0026 1200  .T.&....[..Z.&..
-00005ce0: 0604 5b05 006a 0400 3f00 0602 0005 0068  ..[..j..?......h
-00005cf0: 0400 3f00 0602 0005 0060 0400 3f00 0602  ..?......`..?...
-00005d00: 0005 0012 0400 0500 5200 2612 0012 045b  ........R.&....[
-00005d10: 0800 5600 2612 0006 045b 0500 5c0a 003f  ..V.&....[..\..?
-00005d20: 0006 0200 0500 5c04 003f 0006 0200 0500  ......\..?......
-00005d30: 5c04 003f 0006 0200 0500 5c04 003f 0006  \..?......\..?..
-00005d40: 0200 0500 5c04 003f 0006 0200 0500 5c04  ....\..?......\.
-00005d50: 003f 0006 0200 0500 6a04 003f 0006 0200  .?......j..?....
-00005d60: 0200 6b04 003f 0006 0200 0200 8081 0400  ..k..?..........
-00005d70: 3300 0602 0002 0028 0800 0600 6b04 7153  3......(....k.qS
-00005d80: 0002 beef 460e 0000 0e00 7181 1a33 1c00  ....F.....q..3..
-00005d90: 5f04 0812 0074 0679 1c00 6104 0812 006a  _....t.y..a....j
-00005da0: 0679 1c00 5b04 0812 007f 0879 3c00 7902  .y..[......y<.y.
-00005db0: 003c 0880 9006 0025 0061 1200 252d 7e04  .<.....%.a..%-~.
-00005dc0: 001f 0056 6200 1f01 7a02 0025 003a 0800  ...Vb...z..%.:..
-00005dd0: 1000 6606 001f 004a 0600 1901 822e 0200  ..f....J........
-00005de0: 80a0 0081 0f04 002a 0182 4a02 0080 a000  .......*..J.....
-00005df0: 811e 0400 2a01 8220 0200 80a0 0081 0004  ....*.. ........
-00005e00: 002a 0049 0200 1900 4f02 0019 005d 0200  .*.I....O....]..
-00005e10: 1900 6002 0019 005d 0200 1900 808f 0200  ..`....]........
-00005e20: 1915 5602 0019 0080 892c 0019 0066 0200  ..V......,...f..
-00005e30: 1900 5302 0019 0081 7402 0068 155a 0200  ..S.....t..h.Z..
-00005e40: 1929 6c2c 0068 0056 5400 1900 5402 0019  .)l,.h.VT...T...
-00005e50: 0054 0200 1900 5602 0019 0056 0200 1900  .T....V....V....
-00005e60: 5a02 0019 0080 aa02 0019 0080 a802 0019  Z...............
-00005e70: 0080 9d02 0019 0080 a902 0019 0080 9602  ................
-00005e80: 0019 0080 b702 0019 0080 b602 0019 006a  ...............j
-00005e90: 0200 1900 1806 6a0d 0000 0500 2800 291c  ......j.....(.).
-00005ea0: 0046 0477 1400 4302 0023 0055 0200 1c00  .F.w..C..#.U....
-00005eb0: 6a04 0857 0044 0879 2301 813e 0200 80c4  j..W.D.y#..>....
-00005ec0: 0047 0600 2543 0402 0080 cb00 0d04 360c  .G..%C........6.
-00005ed0: 002b 020c 3e01 6002 7f48 0031 040c 3e01  .+..>.`..H.1..>.
-00005ee0: 6c02 7f48 0026 0475 3e01 5602 7f48 0026  l..H.&.u>.V..H.&
-00005ef0: 0459 1600 2e00 540c 0047 0245 0c00 3502  .Y....T..G.E..5.
-00005f00: 080c 004b 0202 0c00 4c02 000c 0038 0202  ...K....L....8..
-00005f10: 0c06 0602 750c 0037 0e08 0c00 3802 060c  ....u..7....8...
-00005f20: 0031 0275 0c00 3d04 630c 0606 0220 0c06  .1.u..=.c.... ..
-00005f30: 060e 100c 004c 0e6f 0c00 3302 7b0c 0034  .....L.o..3.{..4
-00005f40: 0202 0c00 3602 040c 0036 0200 0c00 3502  ....6....6....5.
-00005f50: 060c 0051 045d 3e00 4f04 003e 004c 0400  ...Q.]>.O..>.L..
-00005f60: 3e00 5204 003e 004f 0400 3e00 4a04 003e  >.R..>.O..>.J..>
-00005f70: 0049 0400 3b00 5502 383b 0014 0269 0900  .I..;.U.8;...i..
-00005f80: 4902 6322 0000 0400 3304 6f09 0002 bf5b  I.c"....3.o....[
-00005f90: 5c0e 0000 0e07 6480 ae1d 1207 6e12 0012  \.....d.....n...
-00005fa0: 0760 1200 1207 8090 1600 8099 004a 1600  .`...........J..
-00005fb0: 0d00 4402 000d 0049 0200 0d00 5b02 000e  ..D....I....[...
-00005fc0: 1364 0200 80a1 0026 2c00 0d00 5d00 4e12  .d.....&,...].N.
-00005fd0: 004d 0473 3500 0002 0013 0053 0700 5504  .M.s5......S..U.
-00005fe0: 770a 0002 7d32 0b00 000b 0000 0100 0c0a  w...}2..........
-00005ff0: 0411 0000 0200 1200 5507 0060 0446 3200  ........U..`.F2.
-00006000: 0002 001b 0043 0701 4804 7715 0002 7d42  .....C..H.w...}B
-00006010: 0b00 000b 0000 0100 027d 670b 0000 0b00  .........}g.....
-00006020: 0001 0150 1249 2500 7306 0025 0073 0200  ...P.I%.s..%.s..
-00006030: 2500 7302 0025 0027 0a00 0d00 5f00 5012  %.s..%.'...._.P.
-00006040: 045d 0669 4300 0002 000f 005b 0700 760c  .].iC......[..v.
-00006050: 771c 0000 0600 0275 2a08 002c 1206 2300  w......u*..,..#.
-00006060: 0005 000f 005b 0700 6604 5842 0000 0200  .....[..f.XB....
-00006070: 2400 3109 0024 0477 0900 5004 0017 0002  $.1..$.w..P.....
-00006080: 7954 0b00 000b 0000 0100 0006 0002 7d4f  yT............}O
-00006090: 0b00 0a16 5904 0000 0200 7e04 7f4c 0003  ....Y.....~..L..
-000060a0: 7d2c 0600 0700 6f06 0028 0c5f 0d00 5004  },....o..(._..P.
-000060b0: 0812 0238 0679 2500 2a0a 000d 0066 0056  ...8.y%.*....f.V
-000060c0: 1200 6f08 7d45 0000 0200 1c00 4107 0043  ..o.}E......A..C
-000060d0: 0477 1a00 027d 440b 0000 0b00 0001 2980  .w...}D.......).
-000060e0: 940a 3525 0037 5800 1500 4e02 6230 0000  ..5%.7X...N.b0..
-000060f0: 0200 2400 3109 0017 0677 0b03 6404 0817  ..$.1....w..d...
-00006100: 0018 0e79 0e00 5e00 3211 0002 6922 0b00  ...y..^.2...i"..
-00006110: 000b 0000 0100 6820 0645 0000 0200 2400  ......h .E....$.
-00006120: 3109 002d 0477 1601 4204 0817 0002 794c  1..-.w..B.....yL
-00006130: 0b00 000b 0000 0100 7814 0645 0000 0200  ........x..E....
-00006140: 2400 3107 0142 0477 1500 027d 540b 0000  $.1..B.w...}T...
-00006150: 0b00 0001 0067 0e06 4500 0002 0024 0031  .....g..E....$.1
-00006160: 0900 2e04 7716 0142 0408 1700 0279 4c0b  ....w..B.....yL.
-00006170: 0000 0b00 0001 006c 1606 4500 0002 0024  .......l..E....$
-00006180: 0031 0900 1706 770b 0464 0408 1700 1810  .1....w..d......
-00006190: 790e 005e 0032 1100 0267 220b 0000 0b00  y..^.2...g".....
-000061a0: 0001 0080 8b22 251f 004e 0638 1b00 0002  ....."%..N.8....
-000061b0: 000f 005b 0700 8086 0477 2200 0006 0002  ...[.....w".....
-000061c0: 7d2a 0800 80f8 0c4f 1f02 2406 0025 0124  }*.....O..$..%.$
-000061d0: 0600 2500 809e 0800 1f00 7506 001f 0029  ..%.......u....)
-000061e0: 0600 0d00 6300 5412 0080 a606 2d1f 0043  ....c.T.....-..C
-000061f0: 0600 1000 2606 000d 0059 004e 1201 80cc  ....&....Y.N....
-00006200: 0433 1f00 2508 000d 005b 004c 1200 6006  .3..%....[.L..`.
-00006210: 351f 004c 0400 0c0b 80b2 0400 1f00 4e1a  5..L..........N.
-00006220: 000c 004e 0400 0c1b 8098 0400 1f00 523a  ...N..........R:
-00006230: 000c 0281 f404 001f 0281 f408 001f 005c  ...............\
-00006240: 0800 1f01 8116 0400 1f0e 80a2 0600 2501  ..............%.
-00006250: 80ba 1e00 2500 2808 000d 0061 0052 121b  ....%.(....a.R..
-00006260: 809e 042f 2500 283c 000d 005f 0052 1200  .../%.(<..._.R..
-00006270: 6e06 2f1f 0076 0600 2500 8084 0400 2508  n./..v..%.....%.
-00006280: 1206 001f 0041 1600 1000 808f 0600 5206  .....A........R.
-00006290: 8096 0600 80b2 0032 1200 0d00 7500 6612  .......2....u.f.
-000062a0: 003b 0a1b 1000 160a 2a0d 0000 0500 0800  .;......*.......
-000062b0: 6909 000c 0436 1100 0005 0013 0053 0700  i....6.......S..
-000062c0: 1004 580c 0000 0500 2400 3109 0026 0477  ..X.....$.1..&.w
-000062d0: 1300 8090 0400 8086 0002 7954 0e00 000b  ..........yT....
-000062e0: 0000 0100 027d 570e 0000 0b00 0001 0002  .....}W.........
-000062f0: 7d63 0e00 000e 0042 1c5d 1000 3306 000f  }c.....B.]..3...
-00006300: 0181 0808 0035 080a 0c00 1904 0614 006a  .....5.........j
-00006310: 270a 0c00 3404 0a54 000c 1f0a 0e00 1906  '...4..T........
-00006320: 0a46 0025 040a 1200 1f14 0a0e 0019 030a  .F.%............
-00006330: 2c00 1f15 0a0c 001f 2954 3000 1f00 7758  ,.......)T0...wX
-00006340: 0022 0037 0200 0700 2b02 000e 004c 0200  .".7....+....L..
-00006350: 0700 3802 001c 0014 0200 0800 1d02 000e  ..8.............
-00006360: 0028 0200 0800 1e02 0011 8113 0a02 0083  .(..............
-00006370: 8200 2982 2800 1100 4c02 0020 003b 0200  ..).(...L.. .;..
-00006380: 0700 3002 0009 0034 0200 0700 2002 0009  ..0....4.... ...
-00006390: 002a 0200 0e00 2902 0007 0038 080e 0d00  .*....)....8....
-000063a0: 3104 7b27 0001 0279 0200 000b 0000 0100  1.{'...y........
-000063b0: 0102 7905 0980 1a06 0005 0981 1a06 0005  ..y.............
-000063c0: 0982 1a06 0005 0983 1a06 0005 0984 1a06  ................
-000063d0: 0005 0985 1a06 0005 0986 1a06 0005 0800  ................
-000063e0: 0400 0006 0000 0035 1405 3509 0000 0014  .......5..5.....
-000063f0: 0052 822e 0d20 0080 8702 0012 002b 0400  .R... .......+..
-00006400: 0600 2902 000c 003b 0200 1b00 0102 7902  ..)....;......y.
-00006410: 0000 0900 0001 0000 0900 0001 0001 0000  ................
-00006420: 1a00 0000 5f1b 050b 0059 0800 0b00 5508  ...._....Y....U.
-00006430: 000b 0051 0800 0b00 5f10 0025 5379 7374  ...Q...._..%Syst
-00006440: 656d 2e43 6f6d 706f 6e65 6e74 4d6f 6465  em.ComponentMode
-00006450: 6c2e 4461 7461 416e 6e6f 7461 7469 6f6e  l.DataAnnotation
-00006460: 731e 5379 7374 656d 2e54 6578 742e 4a73  s.System.Text.Js
-00006470: 6f6e 2e53 6572 6961 6c69 7a61 7469 6f6e  on.Serialization
-00006480: 2501 addf 01ad e601 ae01 01ae 0b01 ae17  %...............
-00006490: 01ae 2701 ae38 01c0 004b 3b01 aee2 01b0  ..'..8...K;.....
-000064a0: e301 c000 4b61 0700 0000 5680 da05 0700  ....Ka....V.....
-000064b0: 0000 2e81 1005 1b00 0000 1d81 3705 0b00  ............7...
-000064c0: 2408 000b 0028 0800 0b00 2608 000b 001d  $....(....&.....
-000064d0: 1200 0700 0000 2482 2905 0c00 0000 2682  ......$.).....&.
-000064e0: 3305 0b00 3208 0011 0000 001f 823e 050b  3...2........>..
-000064f0: 001e 0800 0b00 3d08 0007 0000 0018 8255  ......=........U
-00006500: 0523 0000 0069 0c09 2100 80a8 0400 2100  .#...i..!.....!.
-00006510: 80bc 0400 3100 808f 0400 2100 8085 0600  ....1.....!.....
-00006520: 2100 0102 791d 01ad df01 ade6 01ae 0101  !...y...........
-00006530: ae0b 01ae 1701 ae27 01ae 3801 ae8e 01ae  .......'..8.....
-00006540: 9e03 1c80 a90a 0000 5f1c 0921 005f 0200  ........_..!._..
-00006550: 2114 1204 001b 0612 2c00 2107 1210 0021  !.......,.!....!
-00006560: 0412 1200 2106 120c 0021 1d12 0e00 2117  ....!....!....!.
-00006570: 123e 0082 2800 4134 0012 005b 0600 3400  .>..(.A4...[..4.
-00006580: 6e02 001b 005c 0400 3700 6f02 001b 005c  n....\..7.o....\
-00006590: 0400 3400 6f02 001b 005c 0400 3700 6f02  ..4.o....\..7.o.
-000065a0: 001b 005b 0400 3400 6e02 001b 005c 0400  ...[..4.n....\..
-000065b0: 3700 6f02 001b 005c 0400 3700 6f02 001b  7.o....\..7.o...
-000065c0: 0080 870a 0021 0080 8706 0021 0080 8706  .....!.....!....
-000065d0: 0021 0080 8706 0021 0080 8706 0021 0080  .!.....!.....!..
-000065e0: 8706 0021 0080 8706 0021 0001 0279 1100  ...!.....!...y..
-000065f0: 0000 3780 be09 0800 3e02 0008 0001 0279  ..7.....>......y
-00006600: 82a7 0b00 004d 0c09 110e 1206 0010 0050  .....M.........P
-00006610: 1e02 2100 5002 0021 0032 067f 1200 0c02  ..!.P..!.2......
-00006620: 2a0c 0000 0200 0800 6906 0052 0420 2f00  *.......i..R. /.
-00006630: 0002 0008 0069 0600 1f04 7706 0002 7d1c  .....i....w...}.
-00006640: 0a00 0009 0000 0100 027d 790a 0000 0900  .........}y.....
-00006650: 0001 0013 105d 0800 1906 0006 0014 0248  .....].........H
-00006660: 0d00 0005 0017 004b 1c00 1304 7703 000c  .......K....w...
-00006670: 022a 0c00 0005 0008 0069 0800 1004 2c0d  .*.......i....,.
-00006680: 0000 0500 0e00 5d08 0020 0477 0e00 4c04  ......].. .w..L.
-00006690: 001d 0050 0200 1d00 2602 000d 0080 9004  ...P....&.......
-000066a0: 0838 012a 0679 4200 5506 0838 002b 0679  .8.*.yB.U..8.+.y
-000066b0: 0400 1102 0007 0080 fe06 0862 0080 ed04  ...........b....
-000066c0: 0053 001b 0200 0e00 0d06 7903 001e 0200  .S........y.....
-000066d0: 0c00 7304 086a 0016 0200 0d00 1902 0009  ..s..j..........
-000066e0: 0036 0679 1300 4402 0013 0042 0200 1328  .6.y..D....B...(
-000066f0: 0404 0080 9d00 1704 360c 003b 0202 3800  ........6..;..8.
-00006700: 3b02 0a38 003b 0273 3800 2d02 0a0c 002d  ;..8.;.s8.-....-
-00006710: 0279 0c00 2d02 7d0c 002d 0204 0c00 2d02  .y..-.}..-....-.
-00006720: 000c 002d 027b 0c00 2d02 020c 002d 0204  ...-.{..-....-..
-00006730: 0c00 2d02 7f0c 002d 020e 0c00 2d02 7d0c  ..-....-....-.}.
-00006740: 002d 0204 0c00 2d02 000c 002d 027d 0c00  .-....-....-.}..
-00006750: 2d02 000c 002d 0202 0c00 2d02 7d0c 002d  -....-....-.}..-
-00006760: 0206 0c00 2d02 730c 002d 0200 0c00 2d02  ....-.s..-....-.
-00006770: 000c 002d 0210 0c00 2d02 020c 002d 027f  ...-....-....-..
-00006780: 0c00 2d02 040c 002d 027b 0c00 2d02 0c0c  ..-....-.{..-...
-00006790: 002d 0269 0c03 80b2 0210 5f00 5d08 7f4c  .-.i......_.]..L
-000067a0: 005e 024f 5200 0004 0061 066f 1600 2f04  .^.OR....a.o../.
-000067b0: 080c 0031 0200 0a00 0c02 0002 0012 0408  ...1............
-000067c0: 1300 0d02 0010 0061 0871 1600 1404 080e  .......a.q......
-000067d0: 0024 0408 1300 0d02 0010 0061 0871 1c00  .$.........a.q..
-000067e0: 2204 0819 0012 0200 1300 2202 0010 0080  ".........".....
-000067f0: 9602 0054 0080 9e02 0030 000d 022a 0700  ...T.....0...*..
-00006800: 0002 0008 0069 0900 1802 770f 0002 7f1c  .....i....w.....
-00006810: 0b00 000e 0061 0855 1c00 4a04 0813 002c  .....a.U..J....,
-00006820: 0200 1900 1202 0013 0017 0200 0c00 6202  ..............b.
-00006830: 0840 0000 0200 2002 0215 0062 027f 4000  .@.... ....b..@.
-00006840: 3108 710b 002c 0208 0900 0002 0032 0202  1.q..,.......2..
-00006850: 0b00 2b02 7f09 0000 0200 2304 0009 002c  ..+.......#....,
-00006860: 0479 0e00 1102 0004 0006 0200 0200 02be  .y..............
-00006870: f728 0d00 0009 0000 0100 0a81 1051 0400  .(...........Q..
-00006880: 0600 1602 0002 beed 060d 0000 0900 0001  ................
-00006890: 000b 811a 5d04 0043 0208 3800 02be df32  ....]..C..8....2
-000068a0: 0e00 000e 0001 8126 3720 01ad df01 ade6  .......&7 ......
-000068b0: 01ae 0101 ae0b 01ae 1701 ae27 01ae 3801  ...........'..8.
-000068c0: ae8e 01ae 9e01 aeb9 031c 8135 0c00 0039  ...........5...9
-000068d0: 0c09 0600 1602 520d 0000 0200 1c00 411c  ......R.......A.
-000068e0: 0065 0277 5400 027f 440b 0000 0e00 3d04  .e.wT...D.....=.
-000068f0: 3507 0071 0400 1d0d 0a02 004c 0077 1c00  5..q.......L.w..
-00006900: 1d00 5e02 000b 0075 0200 1e05 0a02 000c  ..^....u........
-00006910: 0075 0c00 1e09 0a02 000c 0071 1400 1e22  .u.........q..."
-00006920: 0a02 000c 001f 4600 0c00 2402 000c 0024  ......F...$....$
-00006930: 0200 0d00 2602 000d 0021 0200 0d00 8087  ....&....!......
-00006940: 0600 3000 2602 000d 0080 9202 001b 0033  ..0.&..........3
-00006950: 0400 0d00 3a02 0007 0025 0200 0800 3302  ....:....%....3.
-00006960: 0007 001e 0200 0800 2802 000e 0027 0200  ........(....'..
-00006970: 0700 2f04 000d 0036 0200 0700 2a02 0008  ../....6....*...
-00006980: 002f 0200 0700 1e02 0008 0028 0200 0e00  ./.........(....
-00006990: 2702 0007 002f 0400 0d00 3602 0007 0027  '..../....6....'
-000069a0: 0200 0900 2f02 0007 001e 0200 0800 2802  ..../.........(.
-000069b0: 000e 0027 0200 0700 2f04 000d 0036 0200  ...'..../....6..
-000069c0: 0700 2c02 0009 002f 0200 0700 1e02 0008  ..,..../........
-000069d0: 0028 0200 0e00 2702 0007 002f 0400 0d00  .(....'..../....
-000069e0: 3602 0007 002a 0200 0900 2f02 0007 001f  6....*..../.....
-000069f0: 0200 0900 2802 000e 0027 0200 0700 0102  ....(....'......
-00006a00: 790b 5379 7374 656d 2e54 6578 7423 01ad  y.System.Text#..
-00006a10: df01 ade6 01ae 0101 ae0b 01ae 1701 ae27  ...............'
-00006a20: 01ae 3801 c000 5101 01ae 8e01 ae9e 01ae  ..8...Q.........
-00006a30: b97d 0d00 005a 0c09 0b00 1602 560d 0000  .}...Z......V...
-00006a40: 0500 1e00 3d18 0011 0430 0e00 0005 0010  ....=....0......
-00006a50: 0059 0900 8084 0477 808d 0002 7d2c 0e00  .Y.....w....},..
-00006a60: 000e 0002 7d14 0e00 000e 0038 0e31 0700  ....}......8.1..
-00006a70: 5602 0017 110a 0200 2100 6e24 001d 0048  V.......!.n$...H
-00006a80: 0200 0b00 2102 000c 0046 0200 1c00 3702  ....!....F....7.
-00006a90: 0006 0024 0200 0700 3002 0007 001b 0200  ...$....0.......
-00006aa0: 0800 2202 000d 0021 0200 0700 0102 790c  .."....!......y.
-00006ab0: 0000 0080 a30a 0921 0001 0279 1b01 addf  .......!...y....
-00006ac0: 01ad e601 ae01 01ae 0b01 ae17 01ae 2701  ..............'.
-00006ad0: ae38 01ae 8e01 ae9e 4b0e 0000 4d0a 0912  .8......K...M...
-00006ae0: 005d 0600 2100 5f02 0021 002b 0600 0d00  .]..!._..!.+....
-00006af0: 5d04 0811 1412 0279 2107 1a2c 0021 0080  ]......y!..,.!..
-00006b00: af12 0021 0080 af02 0021 0080 8904 001b  ...!.....!......
-00006b10: 0080 a304 0021 2a0a 0400 1b0d 0a5a 001b  .....!*......Z..
-00006b20: 0001 1c79 0600 0000 1a61 2307 0000 0001  ...y.....a#.....
-00006b30: 809f 4907 0000 0018 84e1 3107 0000 0018  ..I.......1.....
-00006b40: 84f1 4907 0000 0017 84f2 4907 0000 0017  ..I.......I.....
-00006b50: 84f3 3307 0000 0018 850d 5107 0000 0018  ..3.......Q.....
-00006b60: 850e 5107 0000 0018 850f 5107 0000 0018  ..Q.......Q.....
-00006b70: 8510 5108 0000 0180 aa86 e83f 0700 0002  ..Q........?....
-00006b80: 6686 f740 0700 0002 6687 0e40 0800 0001  f..@....f..@....
-00006b90: 80a6 8718 4007 0000 0035 8aad 4007 0000  ....@....5..@...
-00006ba0: 0030 8ad3 7307 0000 0036 8af0 6a07 0000  .0..s....6..j...
-00006bb0: 0030 8b22 5707 0000 0030 8b32 7107 0f00  .0."W....0.2q...
-00006bc0: 0040 8b3c 7107 0000 002f 8b43 7107 0000  .@.<q..../.Cq...
-00006bd0: 0034 8b4e 7180 b110 0000 2151 2709 0000  .4.Nq.....!Q'...
-00006be0: 0200 0d00 5f04 001d 0477 0700 0004 0002  ...._....w......
-00006bf0: 7d26 0600 1b0a 0a09 0000 0500 0f00 5b04  }&............[.
-00006c00: 0000 0700 3404 770d 0056 0200 2e00 2404  ....4.w..V....$.
-00006c10: 000d 0041 0200 1d00 2d02 001d 000e 0408  ...A....-.......
-00006c20: 0700 2002 0013 0027 0200 1400 2104 0013  .. ....'....!...
-00006c30: 0080 8304 084f 002e 0871 1a00 6d00 5e3b  .....O...q..m.^;
-00006c40: 0017 0423 0d00 1702 000d 004e 0200 1800  ...#.......N....
-00006c50: 4302 0007 0022 0200 0f00 2202 000f 005c  C...."...."....\
-00006c60: 0200 2c00 6002 002c 0025 0200 0d00 2602  ..,.`..,.%....&.
-00006c70: 0011 001e 0200 1b00 6602 0022 0000 0400  ........f.."....
-00006c80: 0241 2a09 0001 4447 3811 0000 4380 9e0d  .A*...DG8...C...
-00006c90: 0600 5d02 2e3b 0000 0200 0a00 6507 0019  ..]..;......e...
-00006ca0: 0477 0900 6a00 342c 0002 7d6d 0a00 0009  .w..j.4,..}m....
-00006cb0: 0000 0100 100a 5908 003e 0208 1100 0c04  ......Y..>......
-00006cc0: 790c 0000 0406 80fd 0d71 0001 0a79 0700  y........q...y..
-00006cd0: 0000 4286 da52 0700 0000 428a b452 0600  ..B..R....B..R..
-00006ce0: 0000 316d 2c07 0000 006a 8085 2507 0000  ..1m,....j..%...
-00006cf0: 004a 8088 2507 0000 006e 8091 2607 0000  .J..%....n..&...
-00006d00: 004d 8094 2607 0000 006c 822f 2606 0000  .M..&....l./&...
-00006d10: 0034 253f 0712 0000 6780 9f44            .4%?....g..D
+00000480: 4000 0000 1600 0900 4400 0900 702f 0000  @.......D...p/..
+00000490: 2000 0000 1600 0900 4500 0900 f62f 0000   .......E..../..
+000004a0: 2000 0000 1600 0900 4600 0900 7e30 0000   .......F...~0..
+000004b0: 2000 0000 1600 0900 4700 0900 e930 0000   .......G....0..
+000004c0: 4500 0000 1600 0900 4800 0900 0836 0000  E.......H....6..
+000004d0: 4b00 0000 1600 0900 4900 0900 a737 0000  K.......I....7..
+000004e0: 2300 0000 1600 0900 4a00 0900 593a 0000  #.......J...Y:..
+000004f0: 2300 0000 1600 0900 4b00 0900 e43b 0000  #.......K....;..
+00000500: 2600 0000 1600 0900 4c00 0900 5d3c 0000  &.......L...]<..
+00000510: 4500 0000 1600 0900 4d00 0900 363d 0000  E.......M...6=..
+00000520: 4500 0000 1600 0900 4e00 0900 da3e 0000  E.......N....>..
+00000530: 2900 0000 1600 0900 4f00 0900 fa42 0000  ).......O....B..
+00000540: c401 0000 1600 0900 5000 0900 0643 0000  ........P....C..
+00000550: a601 0000 1600 0900 5500 0900 ea45 0000  ........U....E..
+00000560: 2900 0000 1600 0900 5600 0900 5e46 0000  ).......V...^F..
+00000570: 6000 0000 1600 0900 5700 0900 6546 0000  `.......W...eF..
+00000580: 5900 0000 1600 0900 5800 0900 1448 0000  Y.......X....H..
+00000590: 890e 0000 1600 0900 6500 0900 1460 0000  ........e....`..
+000005a0: 2900 0000 1600 0900 6600 0900 0463 0000  ).......f....c..
+000005b0: 2900 0000 1600 0900 6700 0900 0f65 0000  ).......g....e..
+000005c0: 2900 0000 1600 0900 6800 0900 f665 0000  ).......h....e..
+000005d0: 2900 0000 1600 0900 6900 0900 b966 0000  ).......i....f..
+000005e0: 2900 0000 1600 0900 6a00 0900 946c 0000  ).......j....l..
+000005f0: 2900 0000 1600 0900 6b00 0900 106e 0000  ).......k....n..
+00000600: 3409 0000 1600 0900 6d00 0900 2c6e 0000  4.......m...,n..
+00000610: 1809 0000 1600 0900 6e00 0900 306e 0000  ........n...0n..
+00000620: c108 0000 1600 0900 7400 0900 5171 0000  ........t...Qq..
+00000630: 3700 0000 1600 0900 7500 0900 087f 0000  7.......u.......
+00000640: 5707 0000 1600 0900 7700 0900 247f 0000  W.......w...$...
+00000650: 3b07 0000 1600 0900 7a00 0900 4383 0000  ;.......z...C...
+00000660: 2200 0000 1600 0900 7b00 0900 2e8a 0000  ".......{.......
+00000670: 2300 0000 1600 0900 7c00 0900 878a 0000  #.......|.......
+00000680: 8b00 0000 1600 0900 7d00 0900 d28a 0000  ........}.......
+00000690: 2900 0000 1600 0900 7e00 0900 238b 0000  ).......~...#...
+000006a0: 5e00 0000 1600 0900 7f00 0900 cf8c 0000  ^...............
+000006b0: 4a00 0000 1600 0900 8000 0900 778d 0000  J...........w...
+000006c0: 3600 0000 1600 0900 8100 0900 858e 0000  6...............
+000006d0: 3600 0000 1600 0900 8200 0900 198f 0000  6...............
+000006e0: 4a00 0000 1600 0900 8300 0900 b68f 0000  J...............
+000006f0: 2900 0000 1600 0900 8400 0900 d294 0000  )...............
+00000700: 0d01 0000 1600 0900 8500 0900 0995 0000  ................
+00000710: a200 0000 1600 0900 8600 0900 569c 0000  ............V...
+00000720: 4200 0000 1800 0900 8700 0900 0000 0000  B...............
+00000730: 0b00 0000 1900 0900 8700 0900 0000 0000  ................
+00000740: 8a00 0000 1a00 0b00 8a00 0900 0000 0000  ................
+00000750: 3e00 0000 1c00 0b00 8a00 0900 0000 0000  >...............
+00000760: 1200 0000 1d00 0b00 8a00 0900 0000 0000  ................
+00000770: 0e00 0000 1e00 0b00 8a00 0900 0000 0000  ................
+00000780: 3e00 0000 2100 0b00 8a00 0900 0000 0000  >...!...........
+00000790: 1200 0000 2200 0b00 8a00 0900 0000 0000  ...."...........
+000007a0: 1d00 0000 2300 0b00 8a00 0900 0000 0000  ....#...........
+000007b0: 2800 0000 2400 0b00 8a00 0900 0000 0000  (...$...........
+000007c0: 1200 0000 2500 0e00 8a00 0900 0000 0000  ....%...........
+000007d0: b600 0000 2600 0e00 8a00 0900 0000 0000  ....&...........
+000007e0: 5906 0000 2700 0e00 8b00 0900 0000 0000  Y...'...........
+000007f0: 1100 0000 2900 1100 8b00 0900 0000 0000  ....)...........
+00000800: 210b 0000 2900 1100 8d00 0900 0e01 0000  !...)...........
+00000810: f609 0000 2900 1100 8f00 0900 2a01 0000  ....).......*...
+00000820: da09 0000 2900 1100 9000 0900 3e01 0000  ....).......>...
+00000830: 7309 0000 2900 1100 9100 0900 5801 0000  s...).......X...
+00000840: 3c09 0000 2900 1100 9200 0900 6001 0000  <...).......`...
+00000850: 3409 0000 2900 1100 9900 0900 4403 0000  4...).......D...
+00000860: 8000 0000 2900 1100 9a00 0900 5308 0000  ....).......S...
+00000870: fa00 0000 2900 1100 9b00 0900 1c09 0000  ....)...........
+00000880: 1800 0000 2900 1100 9c00 0900 6909 0000  ....).......i...
+00000890: e200 0000 2b00 1500 9d00 0900 0000 0000  ....+...........
+000008a0: 9003 0000 2b00 1500 a700 0900 1500 0000  ....+...........
+000008b0: 7000 0000 2d00 1500 a900 0900 0000 0000  p...-...........
+000008c0: d601 0000 2d00 1500 ae00 0900 1d00 0000  ....-...........
+000008d0: dd00 0000 2d00 1500 af00 0900 4800 0000  ....-.......H...
+000008e0: 9600 0000 2f00 1900 b000 0900 0000 0000  ..../...........
+000008f0: 2200 0000 3100 1900 b000 0900 0000 0000  "...1...........
+00000900: 6901 0000 3400 0500 b100 0900 0000 0000  i...4...........
+00000910: 1d00 0000 3700 0900 b100 0900 0000 0000  ....7...........
+00000920: 0200 0000 3800 0900 b100 0900 0000 0000  ....8...........
+00000930: 1d00 0000 3900 0900 b100 0900 0000 0000  ....9...........
+00000940: 1a00 0000 3a00 0900 b100 0900 0000 0000  ....:...........
+00000950: 1a00 0000 3b00 0900 b100 0900 0000 0000  ....;...........
+00000960: 1a00 0000 3c00 0900 b100 0900 0000 0000  ....<...........
+00000970: 1d00 0000 3d00 0900 b100 0900 0000 0000  ....=...........
+00000980: 1d00 0000 3e00 0900 b100 0900 0000 0000  ....>...........
+00000990: 1d00 0000 3f00 0900 b100 0900 0000 0000  ....?...........
+000009a0: 1d00 0000 4000 0900 b100 0900 0000 0000  ....@...........
+000009b0: 4300 0000 4100 0900 b100 0900 0000 0000  C...A...........
+000009c0: 5a00 0000 4200 0900 b100 0900 0000 0000  Z...B...........
+000009d0: 5a00 0000 4300 0900 b100 0900 0000 0000  Z...C...........
+000009e0: 4300 0000 4400 0900 b100 0900 0000 0000  C...D...........
+000009f0: 1600 0000 4500 0900 b100 0900 0000 0000  ....E...........
+00000a00: 1b00 0000 4600 0900 b100 0900 0000 0000  ....F...........
+00000a10: 1b00 0000 4700 0900 b100 0900 0000 0000  ....G...........
+00000a20: 1b00 0000 4800 0900 b100 0900 0000 0000  ....H...........
+00000a30: 1b00 0000 4900 0900 b100 0900 0000 0000  ....I...........
+00000a40: 3300 0000 4a00 0900 b100 0900 0000 0000  3...J...........
+00000a50: 1b00 0000 4b00 0900 b100 0900 0000 0000  ....K...........
+00000a60: 1b00 0000 4d00 0900 b100 0900 0000 0000  ....M...........
+00000a70: b802 0000 4d00 0900 b100 0900 0b00 0000  ....M...........
+00000a80: 0b00 0000 4d00 0900 b200 0900 2e00 0000  ....M...........
+00000a90: 7c02 0000 4d00 0900 b300 0900 3200 0000  |...M.......2...
+00000aa0: 7802 0000 4e00 0900 b600 0900 0000 0000  x...N...........
+00000ab0: ae00 0000 4e00 0900 b700 0900 4300 0000  ....N.......C...
+00000ac0: 3c00 0000 4f00 0900 b800 0900 0000 0000  <...O...........
+00000ad0: 7200 0000 5000 0900 b800 0900 0000 0000  r...P...........
+00000ae0: 1d00 0000 5100 0900 b800 0900 0000 0000  ....Q...........
+00000af0: 1d00 0000 5300 0900 b800 0900 0000 0000  ....S...........
+00000b00: 2400 0000 5500 0900 b800 0900 0000 0000  $...U...........
+00000b10: 3900 0000 5600 0900 b800 0900 0000 0000  9...V...........
+00000b20: 3100 0000 5700 0900 b800 0900 0000 0000  1...W...........
+00000b30: 3900 0000 5800 0900 b800 0900 0000 0000  9...X...........
+00000b40: 3100 0000 5a00 0900 b800 0900 0000 0000  1...Z...........
+00000b50: 4000 0000 5d00 1100 b800 0900 0000 0000  @...]...........
+00000b60: 1b00 0000 5e00 1100 b800 0900 0000 0000  ....^...........
+00000b70: 6100 0000 0000 0000 b806 0000 0000 b806  a...............
+00000b80: 0000 0000 b806 0000 0000 0100 0000 0000  ................
+00000b90: 5f07 0000 0100 b004 0000 0200 1103 0000  _...............
+00000ba0: 0300 9706 0000 0000 e202 0000 0400 4802  ..............H.
+00000bb0: 0000 0500 3b02 0000 0900 0f02 0000 0a00  ....;...........
+00000bc0: 3202 0000 0000 4307 0000 0000 0100 0000  2.....C.........
+00000bd0: 0100 cd04 0000 0200 a402 0000 0300 8002  ................
+00000be0: 0000 0400 9e03 0000 0500 0006 0000 0600  ................
+00000bf0: 2104 0000 0700 c301 0000 0800 e906 0000  !...............
+00000c00: 0900 5003 0000 0a00 c103 0000 0b00 7a06  ..P...........z.
+00000c10: 0000 0c00 c106 0000 0d00 ea03 0000 0e00  ................
+00000c20: d603 0000 0f00 4200 0000 1000 5200 0000  ......B.....R...
+00000c30: 1100 2f00 0000 1200 d005 0000 1300 5005  ../...........P.
+00000c40: 0000 1400 0204 0000 1500 7c01 0000 1600  ..........|.....
+00000c50: 0803 0000 1700 8801 0000 1800 5006 0000  ............P...
+00000c60: 1900 3506 0000 1a00 2106 0000 1b00 6606  ..5.....!.....f.
+00000c70: 0000 1c00 3304 0000 1d00 d806 0000 1e00  ....3...........
+00000c80: f006 0000 1f00 0207 0000 2000 8706 0000  .......... .....
+00000c90: 2100 b301 0000 2200 a301 0000 2300 9804  !.....".....#...
+00000ca0: 0000 2400 ba04 0000 2500 8504 0000 2600  ..$.....%.....&.
+00000cb0: 3007 0000 2700 1407 0000 2800 5c05 0000  0...'.....(.\...
+00000cc0: 2900 0401 0000 2a00 b004 0000 2b00 1103  ).....*.....+...
+00000cd0: 0000 2c00 b203 0000 2d00 1306 0000 2e00  ..,.....-.......
+00000ce0: ad04 0000 3000 b704 0000 3100 1100 0000  ....0.....1.....
+00000cf0: 3200 0302 0000 3300 f601 0000 3400 b704  2.....3.....4...
+00000d00: 0000 3500 b704 0000 3700 6907 0000 3800  ..5.....7.i...8.
+00000d10: 6907 0000 3a00 a102 0000 3c00 2702 0000  i...:.....<.'...
+00000d20: 3d00 e501 0000 3e00 1e02 0000 3f00 1e02  =.....>.....?...
+00000d30: 0000 4000 1e02 0000 4200 d100 0000 4400  ..@.....B.....D.
+00000d40: d100 0000 4500 1e02 0000 4700 0603 0000  ....E.....G.....
+00000d50: 4800 0e04 0000 4900 9402 0000 4a00 cf03  H.....I.....J...
+00000d60: 0000 4b00 0c06 0000 4c00 6303 0000 4d00  ..K.....L.c...M.
+00000d70: 7602 0000 4e00 7602 0000 4f00 5f07 0000  v...N.v...O._...
+00000d80: 5000 bd05 0000 5100 7705 0000 5200 a705  P.....Q.w...R...
+00000d90: 0000 5300 9105 0000 5400 6905 0000 5500  ..S.....T.i...U.
+00000da0: d804 0000 5600 1005 0000 5700 6c01 0000  ....V.....W.l...
+00000db0: 5800 5f01 0000 5900 2903 0000 5a00 3d01  X._...Y.)...Z.=.
+00000dc0: 0000 5b00 3803 0000 5c00 4c01 0000 5f00  ..[.8...\.L..._.
+00000dd0: e501 0000 6400 e501 0000 6500 e501 0000  ....d.....e.....
+00000de0: 6600 e501 0000 6700 e501 0000 6800 e501  f.....g.....h...
+00000df0: 0000 6a00 2403 0000 6b00 f807 0000 6e00  ..j.$...k.....n.
+00000e00: c807 0000 6f00 a207 0000 7000 b807 0000  ....o.....p.....
+00000e10: 7100 d607 0000 7200 ea07 0000 7300 8007  q.....r.....s...
+00000e20: 0000 7400 9407 0000 7500 3d07 0000 7700  ..t.....u.=...w.
+00000e30: 5d02 0000 7800 4504 0000 7c00 2f05 0000  ]...x.E...|./...
+00000e40: 7d00 9501 0000 7e00 2b01 0000 7f00 3d07  }.....~.+.....=.
+00000e50: 0000 8000 1e02 0000 8100 5402 0000 8200  ..........T.....
+00000e60: f204 0000 8300 0603 0000 8400 f204 0000  ................
+00000e70: 8500 f204 0000 8600 f204 0000 8700 f204  ................
+00000e80: 0000 8800 1e02 0000 8a00 7b02 0000 8b00  ..........{.....
+00000e90: f204 0000 8c00 ad04 0000 0000 0100 0000  ................
+00000ea0: 0100 ea01 0000 0200 b704 0000 0000 a402  ................
+00000eb0: 0000 0000 7904 0000 0100 2107 0000 0500  ....y.....!.....
+00000ec0: 1c01 0000 0600 7607 0000 0a00 1f01 0000  ......v.........
+00000ed0: 0b00 4b03 0000 0c00 f204 0000 0d00 3805  ..K...........8.
+00000ee0: 0000 0e00 d202 0000 0f00 8004 0000 1000  ................
+00000ef0: 4505 0000 1100 fd04 0000 1200 1b05 0000  E...............
+00000f00: 1300 b806 0000 1600 e501 0000 1900 b302  ................
+00000f10: 0000 1b00 1902 0000 1c00 dc05 0000 0000  ................
+00000f20: 5d04 0000 0100 be02 0000 0200 2100 0000  ]...........!...
+00000f30: 0300 4c07 0000 0400 f502 0000 0500 9e06  ..L.............
+00000f40: 0000 0600 1104 0000 0700 e404 0000 0800  ................
+00000f50: 9003 0000 0900 f305 0000 0b00 5402 0000  ............T...
+00000f60: 0c00 fb00 0000 0000 4c04 0000 0100 6802  ........L.....h.
+00000f70: 0000 0200 d501 0000 0300 8503 0000 0400  ................
+00000f80: e905 0000 0600 9b02 0000 0b00 2501 0000  ............%...
+00000f90: 0000 c301 0000 0200 7204 0000 0300 ec02  ........r.......
+00000fa0: 0000 0400 0100 0000 0500 7b03 0000 0600  ..........{.....
+00000fb0: 1b03 0000 0000 b306 0000 0200 3f07 8b00  ............?...
+00000fc0: 094b ba00 0f4b a100 154b eb00 1b4b 7700  .K...K...K...Kw.
+00000fd0: 214b 6300 274b d800 2d4b 6d03 334b 0000  !Kc.'K..-Km.3K..
+00000fe0: 0000 0100 4e2e 0200 0000 0100 fe2e 0400  ....N...........
+00000ff0: 0000 0100 9e30 0600 0000 0100 c431 0800  .....0.......1..
+00001000: 0000 0100 d64b 0a00 0000 0100 7b4c 0c00  .....K......{L..
+00001010: 0000 0d00 0000 0100 ff4f 0f00 0000 1000  .........O......
+00001020: 0000 0100 6351 1200 0000 1300 0000 1400  ....cQ..........
+00001030: 0000 0100 1252 1600 0000 1700 0000 1800  .....R..........
+00001040: 0000 2700 0500 9206 2700 0600 bb07 2700  ..'.....'.....'.
+00001050: 0700 e209 6301 0400 9006 8301 0400 9006  ....c...........
+00001060: 9601 0300 5103 a301 0400 9006 b601 0300  ....Q...........
+00001070: 2304 c301 0400 9006 d601 0300 3905 e301  #...........9...
+00001080: 0400 9006 6302 0400 9006 8302 0400 9006  ....c...........
+00001090: a302 0400 9006 4303 0400 9006 0000 0000  ......C.........
+000010a0: 0043 5324 3c3e 385f 5f6c 6f63 616c 7330  .CS$<>8__locals0
+000010b0: 0043 5324 3c3e 385f 5f6c 6f63 616c 7331  .CS$<>8__locals1
+000010c0: 0072 6f6f 6d4e 616d 6548 7564 4343 0077  .roomNameHudCC.w
+000010d0: 6174 6572 5475 7262 696e 6544 6f6f 7243  aterTurbineDoorC
+000010e0: 4300 7468 6f74 684c 6566 7444 6f6f 7243  C.thothLeftDoorC
+000010f0: 4300 7468 6f74 6852 6967 6874 446f 6f72  C.thothRightDoor
+00001100: 4343 0050 6970 6549 6e44 6570 7468 7355  CC.PipeInDepthsU
+00001110: 7070 6572 4944 0050 6970 6549 6e44 6570  pperID.PipeInDep
+00001120: 7468 734c 6f77 6572 4944 0054 686f 7468  thsLowerID.Thoth
+00001130: 4272 6964 6765 4c65 6674 446f 6f72 4944  BridgeLeftDoorID
+00001140: 0041 3257 6174 6572 5475 7262 696e 654c  .A2WaterTurbineL
+00001150: 6566 7444 6f6f 7249 4400 5468 6f74 6842  eftDoorID.ThothB
+00001160: 7269 6467 6552 6967 6874 446f 6f72 4944  ridgeRightDoorID
+00001170: 0064 6f6f 7249 4400 5069 7065 496e 5761  .doorID.PipeInWa
+00001180: 7465 7266 616c 6c73 4944 0050 6970 6549  terfallsID.PipeI
+00001190: 6e48 6964 656f 7574 4944 0072 6f6f 6d44  nHideoutID.roomD
+000011a0: 6174 6100 6f43 6f6e 7472 6f6c 4e65 7477  ata.oControlNetw
+000011b0: 6f72 6b52 6563 6569 7665 6400 6964 0066  orkReceived.id.f
+000011c0: 6f75 6e64 0063 6f6f 7264 0063 6f6c 6c69  ound.coord.colli
+000011d0: 7369 6f6e 436f 6465 546f 4265 0064 6570  sionCodeToBe.dep
+000011e0: 7468 7350 6970 6543 6f64 6500 7761 7465  thsPipeCode.wate
+000011f0: 7266 616c 6c73 5069 7065 436f 6465 006e  rfallsPipeCode.n
+00001200: 6573 7450 6970 6543 6f64 6500 6869 6465  estPipeCode.hide
+00001210: 6f75 7450 6970 6543 6f64 6500 6472 6177  outPipeCode.draw
+00001220: 4775 6943 6f64 6500 6c61 6242 6c6f 636b  GuiCode.labBlock
+00001230: 436f 6465 0063 6f6c 6c69 7369 6f6e 436f  Code.collisionCo
+00001240: 6465 006c 6f61 6447 6c6f 6261 6c73 436f  de.loadGlobalsCo
+00001250: 6465 0073 6176 6547 6c6f 6261 6c73 436f  de.saveGlobalsCo
+00001260: 6465 0063 6861 7261 6374 6572 5661 7273  de.characterVars
+00001270: 436f 6465 0073 7346 4744 6573 7472 6f79  Code.ssFGDestroy
+00001280: 436f 6465 0063 6f64 6500 7465 7874 7572  Code.code.textur
+00001290: 6550 6167 6500 6134 5061 6765 3249 6d61  ePage.a4Page2Ima
+000012a0: 6765 0061 3450 6167 6549 6d61 6765 006d  ge.a4PageImage.m
+000012b0: 7573 6963 4669 6c65 0074 696c 6500 636f  usicFile.tile.co
+000012c0: 6465 4e61 6d65 0073 7072 6974 654e 616d  deName.spriteNam
+000012d0: 6500 6f72 6967 4e61 6d65 006f 7269 6753  e.origName.origS
+000012e0: 6f6e 674e 616d 6500 6e65 7753 6f6e 674e  ongName.newSongN
+000012f0: 616d 6500 726f 6f6d 4e61 6d65 0070 6963  ame.roomName.pic
+00001300: 6b75 704e 616d 6500 4453 4d61 7043 6f6f  kupName.DSMapCoo
+00001310: 7264 526f 6f6d 6e61 6d65 0070 6970 6500  rdRoomname.pipe.
+00001320: 7769 7364 6f6d 5365 7074 6f67 6743 7265  wisdomSeptoggCre
+00001330: 6174 6500 6372 6561 7465 0076 616c 7565  ate.create.value
+00001340: 0062 6700 6f57 6973 646f 6d53 6570 746f  .bg.oWisdomSepto
+00001350: 6767 006c 6566 7446 6163 696e 6700 726f  gg.leftFacing.ro
+00001360: 6f6d 4e61 6d65 4453 4d61 7053 7472 696e  omNameDSMapStrin
+00001370: 6700 6973 5265 7365 6172 6368 4861 7463  g.isResearchHatc
+00001380: 6800 6d75 7369 6350 6174 6800 6669 6c65  h.musicPath.file
+00001390: 5061 7468 0072 6f6f 6d4e 616d 6548 7564  Path.roomNameHud
+000013a0: 4472 6177 4775 6900 6c61 6242 6c6f 636b  DrawGui.labBlock
+000013b0: 0061 7267 734c 6f63 616c 0070 6167 6549  .argsLocal.pageI
+000013c0: 7465 6d00 6974 656d 0064 6570 7468 7350  tem.item.depthsP
+000013d0: 6970 6552 6f6f 6d00 7761 7465 7266 616c  ipeRoom.waterfal
+000013e0: 6c73 5069 7065 526f 6f6d 0072 6f6f 6d00  lsPipeRoom.room.
+000013f0: 646f 6f72 5361 6d75 7343 6f6c 6c69 7369  doorSamusCollisi
+00001400: 6f6e 0063 6f6c 6c69 7369 6f6e 0070 6167  on.collision.pag
+00001410: 6544 696d 656e 7369 6f6e 0065 7874 656e  eDimension.exten
+00001420: 7369 6f6e 0073 7346 4741 6374 696f 6e00  sion.ssFGAction.
+00001430: 726f 6f6d 4875 6441 6374 696f 6e00 7769  roomHudAction.wi
+00001440: 7364 6f6d 5365 7074 6f67 6741 6374 696f  sdomSeptoggActio
+00001450: 6e00 6f43 6f6e 7472 6f6c 4163 7469 6f6e  n.oControlAction
+00001460: 0076 6172 446f 6f72 4163 7469 6f6e 0061  .varDoorAction.a
+00001470: 6374 696f 6e00 6135 4163 7469 7661 7465  ction.a5Activate
+00001480: 436f 6e64 6974 696f 6e00 656d 7042 6174  Condition.empBat
+00001490: 7465 7279 4365 6c6c 436f 6e64 6974 696f  teryCellConditio
+000014a0: 6e00 7363 7244 4e41 5370 6177 6e00 676f  n.scrDNASpawn.go
+000014b0: 0072 6f6f 6d4e 616d 6548 7564 5374 6570  .roomNameHudStep
+000014c0: 0077 6973 646f 6d53 6570 746f 6767 5374  .wisdomSeptoggSt
+000014d0: 6570 0073 7562 7363 7265 656e 4d65 6e75  ep.subscreenMenu
+000014e0: 5374 6570 0070 6963 6b75 7000 6473 4d61  Step.pickup.dsMa
+000014f0: 7043 6f72 6442 7569 6c64 6572 0072 6f6f  pCordBuilder.roo
+00001500: 6d4e 616d 6544 534d 6170 4275 696c 6465  mNameDSMapBuilde
+00001510: 7200 7375 6244 6972 0061 3544 6f6f 7200  r.subDir.a5Door.
+00001520: 646f 6f72 0061 6c72 6561 6479 4164 6465  door.alreadyAdde
+00001530: 6450 426f 6d62 7300 616c 7265 6164 7941  dPBombs.alreadyA
+00001540: 6464 6564 4d69 7373 696c 6573 0066 7300  ddedMissiles.fs.
+00001550: 6c6f 6361 6c73 006d 7300 616c 7265 6164  locals.ms.alread
+00001560: 7941 6464 6564 5375 7065 7273 0073 6565  yAddedSupers.see
+00001570: 644f 626a 6563 7400 736f 6c69 644f 626a  dObject.solidObj
+00001580: 6563 7400 726f 6f6d 4875 644f 626a 6563  ect.roomHudObjec
+00001590: 7400 6761 6d65 4f62 6a65 6374 0077 6174  t.gameObject.wat
+000015a0: 6572 5475 7262 696e 654f 626a 6563 7400  erTurbineObject.
+000015b0: 7069 7065 4f62 6a65 6374 0072 6573 6561  pipeObject.resea
+000015c0: 7263 6848 6174 6368 4f62 6a65 6374 0067  rchHatchObject.g
+000015d0: 6d4f 626a 6563 7400 6973 476f 746f 4f62  mObject.isGotoOb
+000015e0: 6a65 6374 0064 6f6f 724f 626a 6563 7400  ject.doorObject.
+000015f0: 656e 656d 794f 626a 6563 7400 6574 616e  enemyObject.etan
+00001600: 6b53 6e69 7070 6574 0070 6970 6542 4754  kSnippet.pipeBGT
+00001610: 696c 6573 6574 0064 6570 7468 7345 6e74  ileset.depthsEnt
+00001620: 7261 6e63 6550 6970 6554 696c 6573 6574  rancePipeTileset
+00001630: 0077 6174 6572 6661 6c6c 7350 6970 6554  .waterfallsPipeT
+00001640: 696c 6573 6574 0064 6570 7468 7345 7869  ileset.depthsExi
+00001650: 7450 6970 6554 696c 6573 6574 0068 6964  tPipeTileset.hid
+00001660: 656f 7574 5069 7065 5469 6c65 7365 7400  eoutPipeTileset.
+00001670: 646f 6f72 5469 6c65 7365 7400 6d6f 7669  doorTileset.movi
+00001680: 6e67 4f66 6673 6574 0073 7346 4745 7665  ngOffset.ssFGEve
+00001690: 6e74 0072 6f6f 6d48 7564 4576 656e 7400  nt.roomHudEvent.
+000016a0: 7769 7364 6f6d 5365 7074 6f67 6745 7665  wisdomSeptoggEve
+000016b0: 6e74 006f 436f 6e74 726f 6c45 7665 6e74  nt.oControlEvent
+000016c0: 0070 426f 6d62 4368 6172 6163 7465 7245  .pBombCharacterE
+000016d0: 7665 6e74 0073 7570 6572 4d69 7373 696c  vent.superMissil
+000016e0: 6543 6861 7261 6374 6572 4576 656e 7400  eCharacterEvent.
+000016f0: 6d69 7373 696c 6543 6861 7261 6374 6572  missileCharacter
+00001700: 4576 656e 7400 6554 616e 6b43 6861 7261  Event.eTankChara
+00001710: 6374 6572 4576 656e 7400 7661 7244 6f6f  cterEvent.varDoo
+00001720: 7245 7665 6e74 0069 7465 6d73 5377 6170  rEvent.itemsSwap
+00001730: 5363 7269 7074 0073 6372 6970 7400 726f  Script.script.ro
+00001740: 6f6d 4e61 6d65 4875 6452 6f6f 6d53 7461  omNameHudRoomSta
+00001750: 7274 006c 6973 7400 636f 6465 5465 7874  rt.list.codeText
+00001760: 006e 6577 446f 6f72 5265 706c 6163 656d  .newDoorReplacem
+00001770: 656e 7454 6578 7400 7375 6273 6372 6565  entText.subscree
+00001780: 6e4d 6973 6344 6177 0073 7344 7261 7700  nMiscDaw.ssDraw.
+00001790: 7375 6263 7265 656e 426f 6f74 7344 7261  subcreenBootsDra
+000017a0: 7700 7375 6273 6372 6565 6e53 7569 7444  w.subscreenSuitD
+000017b0: 7261 7700 6472 6177 456e 6449 6e64 6578  raw.drawEndIndex
+000017c0: 0064 6f6f 7245 7665 6e74 496e 6465 7800  .doorEventIndex.
+000017d0: 6472 6177 5374 6172 7449 6e64 6578 006b  drawStartIndex.k
+000017e0: 6579 0061 7373 656d 626c 7900 726f 6f6d  ey.assembly.room
+000017f0: 4e61 6d65 4875 6444 6573 7472 6f79 0063  NameHudDestroy.c
+00001800: 6f64 6545 6e74 7279 0074 6578 7475 7265  odeEntry.texture
+00001810: 456e 7472 7900 646f 6f72 456e 7472 7900  Entry.doorEntry.
+00001820: 6c6f 636b 6564 5042 6f6d 6251 7561 6e74  lockedPBombQuant
+00001830: 6974 7900 7042 6f6d 6251 7561 6e74 6974  ity.pBombQuantit
+00001840: 7900 6c6f 636b 6564 4d69 7373 696c 6551  y.lockedMissileQ
+00001850: 7561 6e74 6974 7900 6d69 7373 696c 6551  uantity.missileQ
+00001860: 7561 6e74 6974 7900 6669 6e61 6c51 7561  uantity.finalQua
+00001870: 6e74 6974 7900 6c6f 636b 6564 5375 7065  ntity.lockedSupe
+00001880: 7251 7561 6e74 6974 7900 7375 7065 7251  rQuantity.superQ
+00001890: 7561 6e74 6974 7900 7175 616e 7469 7479  uantity.quantity
+000018a0: 0000 0000 0000 0000 0fd0 2988 b811 1342  ..........)....B
+000018b0: 878b 770e 8597 ac16 f862 513f c607 d311  ..w......bQ?....
+000018c0: 9053 00c0 4fa3 02a1 1b57 8a0e 2669 6e46  .S..O....W..&inF
+000018d0: b4ad 8ab0 4611 f5fe bc74 2e93 a9db 7844  ....F....t....xD
+000018e0: 8d46 0f32 a7ba b3d3 5605 11cc 91a0 384d  .F.2....V.....8M
+000018f0: 9fec 25ab 9a35 1a6a 05ec feb5 d08c 834a  ..%..5.j.......J
+00001900: 96da 4662 84bb 4bd8 0847 4d7e 6e09 5c4c  ..Fb..K..GM~n.\L
+00001910: aeda cb10 ba6a 740d 0004 686f 6d65 0672  .....jt...home.r
+00001920: 756e 6e65 7204 776f 726b 0459 414d 5308  unner.work.YAMS.
+00001930: 5941 4d53 2d4c 4942 0d45 7863 6570 7469  YAMS-LIB.Excepti
+00001940: 6f6e 732e 6373 092f 0001 060d 1212 1720  ons.cs./....... 
+00001950: 2045 cf63 12b5 33a2 5dfc 4dce b431 5040   E.c..3.].M..1P@
+00001960: 06cb b9c4 4b95 8487 2f00 aa0c 69ad 7c7b  ....K.../...i.|{
+00001970: 7913 4578 7465 6e73 696f 6e4d 6574 686f  y.ExtensionMetho
+00001980: 6473 2e63 7309 2f00 0106 0d12 1217 5920  ds.cs./.......Y 
+00001990: 8e60 29b7 ed9a 0b1a 1a46 f770 be95 760e  .`)......F.p..v.
+000019a0: ea0e 8ec0 45b2 e613 b318 395a 43ae 57f7  ....E.....9ZC.W.
+000019b0: 0f4d 7573 6963 5368 7566 666c 652e 6373  .MusicShuffle.cs
+000019c0: 0a2f 0001 060d 1212 1780 9820 3c0a 97ef  ./......... <...
+000019d0: 3aba 9a95 23f6 7f5c 7a9b 8254 fac4 f5de  :...#..\z..T....
+000019e0: dc3e 0a75 a15d d33b dcc7 45e4 0770 6174  .>.u.].;..E..pat
+000019f0: 6368 6573 1141 6464 496e 4761 6d65 4869  ches.AddInGameHi
+00001a00: 6e74 732e 6373 0c2f 0001 060d 1212 1780  nts.cs./........
+00001a10: d480 dc20 6e02 69a1 68e9 d66f e7cc 3811  ... n.i.h..o..8.
+00001a20: 95b7 b370 bf14 88e1 e2a0 5b53 5d2c f554  ...p......[S],.T
+00001a30: b77d acd2 1044 6f6f 724c 6f63 6b52 616e  .}...DoorLockRan
+00001a40: 646f 2e63 730c 2f00 0106 0d12 1217 80d4  do.cs./.........
+00001a50: 811c 2036 f08f a89d edf4 9ff1 a97a ba4d  .. 6.........z.M
+00001a60: a182 4fae 5fd8 d698 f8ef ca26 269f d9e7  ..O._......&&...
+00001a70: 76e9 4b03 716f 6c17 4469 7370 6c61 7952  v.K.qol.DisplayR
+00001a80: 6f6f 6d4e 616d 654f 6e48 5544 2e63 730e  oomNameOnHUD.cs.
+00001a90: 2f00 0106 0d12 1217 80d4 815b 815f 204d  /..........[._ M
+00001aa0: 230e 0556 3847 6697 0043 bc2d 019d cbc8  #..V8Gf..C.-....
+00001ab0: eff9 18c3 6186 d3f1 6fc8 9a1b fbec 8518  ....a...o.......
+00001ac0: 4469 7370 6c61 7952 6f6f 6d4e 616d 6573  DisplayRoomNames
+00001ad0: 4f6e 4d61 702e 6373 0e2f 0001 060d 1212  OnMap.cs./......
+00001ae0: 1780 d481 5b81 a720 9919 2851 d6ab de16  ....[.. ..(Q....
+00001af0: 69e2 2683 bb64 d446 ec54 5d2c 3782 f134  i.&..d.F.T],7..4
+00001b00: 153b 566c d5e2 b53d 1552 6f6f 6d46 6561  .;Vl...=.RoomFea
+00001b10: 7475 7265 4d61 7054 6578 742e 6373 0e2f  tureMapText.cs./
+00001b20: 0001 060d 1212 1780 d481 5b81 f020 c482  ..........[.. ..
+00001b30: 530a 0a87 6a5c fe69 192a 2c85 e5cc b9d5  S...j\.i.*,.....
+00001b40: 9e17 e194 a1d4 dce7 ab23 4c0e d7c7 1953  .........#L....S
+00001b50: 686f 7746 756c 6c79 556e 6578 706c 6f72  howFullyUnexplor
+00001b60: 6564 4d61 702e 6373 0e2f 0001 060d 1212  edMap.cs./......
+00001b70: 1780 d481 5b82 3620 4b38 9777 782b b256  ....[.6 K8.wx+.V
+00001b80: ca61 3817 dbbd b9b4 eecc 3d52 c65a 60a4  .a8.......=R.Z`.
+00001b90: aa48 c276 683a d2af 0a50 726f 6772 616d  .H.vh:...Program
+00001ba0: 2e63 730a 2f00 0106 0d12 1217 8280 202a  .cs./......... *
+00001bb0: 7b45 233b 47c3 fd8b 03e3 3133 4937 757c  {E#;G.....13I7u|
+00001bc0: 23a8 c280 fd1b 2fe8 3035 636b 029c 5f0d  #...../.05ck.._.
+00001bd0: 5365 6564 4f62 6a65 6374 2e63 730a 2f00  SeedObject.cs./.
+00001be0: 0106 0d12 1217 82b7 2012 f3e2 9746 8561  ........ ....F.a
+00001bf0: ed04 11ae e932 879d 7ff7 9962 301b 17e8  .....2.....b0...
+00001c00: a26d 6886 ae28 9ac7 b303 6f62 6a07 5265  .mh..(....obj.Re
+00001c10: 6c65 6173 6506 6e65 7436 2e30 1a59 414d  lease.net6.0.YAM
+00001c20: 532d 4c49 422e 476c 6f62 616c 5573 696e  S-LIB.GlobalUsin
+00001c30: 6773 2e67 2e63 7310 2f00 0106 0d12 1217  gs.g.cs./.......
+00001c40: 82f1 82f5 82fd 8304 20ad db14 3f8c 43b9  ........ ...?.C.
+00001c50: 5f1b b73a 0cba 7c79 3281 935c 4ab8 ccab  _..:..|y2..\J...
+00001c60: bdf6 b04d 3e0f 809e 0e70 1f01 0000 d3d7  ...M>....p......
+00001c70: 57b0 492c 2dc9 d74d 4fcd 4b2d 4a2c 494d  W.I,-..MO.K-J,IM
+00001c80: d1b7 e34a cfc9 4f4a cc51 282d cecc 4b57  ...J..OJ.Q(-..KW
+00001c90: 8070 acac 822b 8b4b 5273 adf1 49ea 39e7  .p...+.KRs..I.9.
+00001ca0: e7e4 a426 9764 e6e7 15eb b983 0ccc 4cc6  ...&.d........L.
+00001cb0: afc1 d31f bfbc 4f66 5e21 7e15 7ea9 257a  ......Of^!~.~.%z
+00001cc0: 1e25 2505 f855 8564 14a5 26a6 0025 8854  .%%..U.d..&..%.T
+00001cd0: a617 9258 9c5d 6ccd 0500 2e2e 4e45 5443  ...X.]l.....NETC
+00001ce0: 6f72 6541 7070 2c56 6572 7369 6f6e 3d76  oreApp,Version=v
+00001cf0: 362e 302e 4173 7365 6d62 6c79 4174 7472  6.0.AssemblyAttr
+00001d00: 6962 7574 6573 2e63 7310 2f00 0106 0d12  ibutes.cs./.....
+00001d10: 1217 82f1 82f5 82fd 83c2 2078 97e5 953c  .......... x...<
+00001d20: b5cd 5131 509b 3504 2186 34c2 4b9c e7a6  ..Q1P.5.!.4.K...
+00001d30: 8b98 4ffb 5a16 686e b5af 5c80 c900 0000  ..O.Z.hn..\.....
+00001d40: 002f 2f20 3c61 7574 6f67 656e 6572 6174  .// <autogenerat
+00001d50: 6564 202f 3e0d 0a75 7369 6e67 2053 7973  ed />..using Sys
+00001d60: 7465 6d3b 0d0a 7573 696e 6720 5379 7374  tem;..using Syst
+00001d70: 656d 2e52 6566 6c65 6374 696f 6e3b 0d0a  em.Reflection;..
+00001d80: 5b61 7373 656d 626c 793a 2067 6c6f 6261  [assembly: globa
+00001d90: 6c3a 3a53 7973 7465 6d2e 5275 6e74 696d  l::System.Runtim
+00001da0: 652e 5665 7273 696f 6e69 6e67 2e54 6172  e.Versioning.Tar
+00001db0: 6765 7446 7261 6d65 776f 726b 4174 7472  getFrameworkAttr
+00001dc0: 6962 7574 6528 222e 4e45 5443 6f72 6541  ibute(".NETCoreA
+00001dd0: 7070 2c56 6572 7369 6f6e 3d76 362e 3022  pp,Version=v6.0"
+00001de0: 2c20 4672 616d 6577 6f72 6b44 6973 706c  , FrameworkDispl
+00001df0: 6179 4e61 6d65 203d 2022 2e4e 4554 2036  ayName = ".NET 6
+00001e00: 2e30 2229 5d0a 1859 414d 532d 4c49 422e  .0")]..YAMS-LIB.
+00001e10: 4173 7365 6d62 6c79 496e 666f 2e63 7310  AssemblyInfo.cs.
+00001e20: 2f00 0106 0d12 1217 82f1 82f5 82fd 84ee  /...............
+00001e30: 20df ad83 a128 f3da 9288 bb66 1a3f 00fa   ....(.....f.?..
+00001e40: 22d4 d442 6a1f ccfc f315 ebf2 1ba1 dc9b  "..Bj...........
+00001e50: 3081 55d2 0300 00ad 935d 6bc2 3014 86ef  0.U......]k.0...
+00001e60: fb2b 0e5e 6d0c dbfa 55dd 1c83 2a38 8409  .+.^m...U...*8..
+00001e70: 4365 638c 5da4 e949 1b48 9391 a493 fefb  Cec.]..I.H......
+00001e80: a56e 8a22 1b05 4dae f29e 93e7 7ce4 2408  .n."..M.....|.$.
+00001e90: da17 5d5e 10c0 3d29 ad6a 6728 5113 8be9  ..]^..=).jg(Q...
+00001ea0: 43ad d56b 9d73 0354 a508 1b62 606f 87a4  C..k.s.T...b`o..
+00001eb0: 0202 5629 e13b cf9d f334 2732 43e3 74b0  ..V).;...4'2C.t.
+00001ec0: f53d c605 4241 2aa0 a434 085c 52a5 3552  .=..BA*..4.\R.5R
+00001ed0: 0b09 e6e4 8b2b 0d44 a6b0 e142 3805 8432  .....+.D...B8..2
+00001ee0: 1638 dbc1 6c8e 3f81 1d48 e33e b2bf cd36  .8..l.?..H.>...6
+00001ef0: 384d f7c2 3df1 4ac3 6506 abca 582c c647  8M..=.J.e...X,.G
+00001f00: 277f 894c b832 b892 63cf 7b27 c660 9188  '..L.2..c.{'.`..
+00001f10: eaee d4ec c7bf b6a9 2a3e 89ac 626b 354f  ........*>..bk5O
+00001f20: 4a8b 57ad b778 b16a 3fcd 27ad eb8f a608  J.W..x.j?.'.....
+00001f30: c978 56ba 7a9d 7a00 5aa2 4062 b031 67e6  .xV.z.z.Z.@b.1g.
+00001f40: 1ee5 05b5 39a6 74fd b0de 8d29 73c9 942e  ....9.t....)s...
+00001f50: b6b9 10f1 07ee 868d c2b0 774b 0743 32ec  ..........wK.C2.
+00001f60: 7669 27c1 5ec2 fa69 d2a7 bd68 1075 fa2c  vi'.^..i...h.u.,
+00001f70: 1ab1 348c 58f3 dc9f b54a 4b6a cf69 e39a  ..4.X....JKj.i..
+00001f80: 5b81 e700 feed 5d3d 9c8f 879f a49e e2c5  [.....]=........
+00001f90: 6a52 7291 c2ab e616 a76e a467 9a64 054a  jRr......n.g.d.J
+00001fa0: 0b54 b888 bee7 7d03 010b 8127 7b22 646f  .T....}....'{"do
+00001fb0: 6375 6d65 6e74 7322 3a7b 222f 686f 6d65  cuments":{"/home
+00001fc0: 2f72 756e 6e65 722f 776f 726b 2f59 414d  /runner/work/YAM
+00001fd0: 532f 5941 4d53 2f2a 223a 2268 7474 7073  S/YAMS/*":"https
+00001fe0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00001ff0: 7263 6f6e 7465 6e74 2e63 6f6d 2f72 616e  rcontent.com/ran
+00002000: 646f 7661 6e69 612f 5941 4d53 2f66 3830  dovania/YAMS/f80
+00002010: 3033 3963 3537 6137 3232 6331 6265 3362  039c57a722c1be3b
+00002020: 6634 6462 3463 3336 3536 3134 6636 3866  f4db4c365614f68f
+00002030: 6430 3666 652f 2a22 2c22 2f68 6f6d 652f  d06fe/*","/home/
+00002040: 7275 6e6e 6572 2f77 6f72 6b2f 5941 4d53  runner/work/YAMS
+00002050: 2f59 414d 532f 556e 6465 7274 616c 654d  /YAMS/UndertaleM
+00002060: 6f64 546f 6f6c 2f2a 223a 2268 7474 7073  odTool/*":"https
+00002070: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002080: 7263 6f6e 7465 6e74 2e63 6f6d 2f6b 727a  rcontent.com/krz
+00002090: 7973 2d68 2f55 6e64 6572 7461 6c65 4d6f  ys-h/UndertaleMo
+000020a0: 6454 6f6f 6c2f 3266 3065 3636 6530 3931  dTool/2f0e66e091
+000020b0: 3034 3937 6435 3132 6331 3862 3434 3966  0497d512c18b449f
+000020c0: 3735 6634 3734 6133 3432 3566 3037 2f2a  75f474a3425f07/*
+000020d0: 227d 7d82 2576 6572 7369 6f6e 0032 0063  "}}.%version.2.c
+000020e0: 6f6d 7069 6c65 722d 7665 7273 696f 6e00  ompiler-version.
+000020f0: 342e 392e 322d 332e 3234 3132 392e 362b  4.9.2-3.24129.6+
+00002100: 3939 3334 6662 3965 3335 3237 6531 6330  9934fb9e3527e1c0
+00002110: 6335 3133 3134 6535 3764 3461 6162 3330  c51314e57d4aab30
+00002120: 6639 3765 3866 3965 006c 616e 6775 6167  f97e8f9e.languag
+00002130: 6500 4323 0073 6f75 7263 652d 6669 6c65  e.C#.source-file
+00002140: 2d63 6f75 6e74 0031 3400 6f75 7470 7574  -count.14.output
+00002150: 2d6b 696e 6400 4479 6e61 6d69 6361 6c6c  -kind.Dynamicall
+00002160: 794c 696e 6b65 644c 6962 7261 7279 006f  yLinkedLibrary.o
+00002170: 7074 696d 697a 6174 696f 6e00 7265 6c65  ptimization.rele
+00002180: 6173 6500 706c 6174 666f 726d 0041 6e79  ase.platform.Any
+00002190: 4370 7500 7275 6e74 696d 652d 7665 7273  Cpu.runtime-vers
+000021a0: 696f 6e00 382e 302e 342b 3264 3765 6561  ion.8.0.4+2d7eea
+000021b0: 3235 3239 3634 6536 3962 6539 3463 6239  252964e69be94cb9
+000021c0: 6338 3437 6233 3731 6232 3365 3464 6434  c847b371b23e4dd4
+000021d0: 3730 006c 616e 6775 6167 652d 7665 7273  70.language-vers
+000021e0: 696f 6e00 7072 6576 6965 7700 6e75 6c6c  ion.preview.null
+000021f0: 6162 6c65 0045 6e61 626c 6500 6465 6669  able.Enable.defi
+00002200: 6e65 0054 5241 4345 2c52 454c 4541 5345  ne.TRACE,RELEASE
+00002210: 2c4e 4554 2c4e 4554 365f 302c 4e45 5443  ,NET,NET6_0,NETC
+00002220: 4f52 4541 5050 2c4e 4554 355f 305f 4f52  OREAPP,NET5_0_OR
+00002230: 5f47 5245 4154 4552 2c4e 4554 365f 305f  _GREATER,NET6_0_
+00002240: 4f52 5f47 5245 4154 4552 2c4e 4554 434f  OR_GREATER,NETCO
+00002250: 5245 4150 5031 5f30 5f4f 525f 4752 4541  REAPP1_0_OR_GREA
+00002260: 5445 522c 4e45 5443 4f52 4541 5050 315f  TER,NETCOREAPP1_
+00002270: 315f 4f52 5f47 5245 4154 4552 2c4e 4554  1_OR_GREATER,NET
+00002280: 434f 5245 4150 5032 5f30 5f4f 525f 4752  COREAPP2_0_OR_GR
+00002290: 4541 5445 522c 4e45 5443 4f52 4541 5050  EATER,NETCOREAPP
+000022a0: 325f 315f 4f52 5f47 5245 4154 4552 2c4e  2_1_OR_GREATER,N
+000022b0: 4554 434f 5245 4150 5032 5f32 5f4f 525f  ETCOREAPP2_2_OR_
+000022c0: 4752 4541 5445 522c 4e45 5443 4f52 4541  GREATER,NETCOREA
+000022d0: 5050 335f 305f 4f52 5f47 5245 4154 4552  PP3_0_OR_GREATER
+000022e0: 2c4e 4554 434f 5245 4150 5033 5f31 5f4f  ,NETCOREAPP3_1_O
+000022f0: 525f 4752 4541 5445 5200 a3ee 4943 5368  R_GREATER...ICSh
+00002300: 6172 7043 6f64 652e 5368 6172 705a 6970  arpCode.SharpZip
+00002310: 4c69 622e 646c 6c00 0001 6c99 0498 0080  Lib.dll...l.....
+00002320: 0300 87d2 8216 a495 d14a bd3f 1fc4 0213  .........J.?....
+00002330: b4ed 4d61 6372 6f73 732e 4a73 6f6e 2e45  ..Macross.Json.E
+00002340: 7874 656e 7369 6f6e 732e 646c 6c00 0001  xtensions.dll...
+00002350: 55c4 78ba 0000 0100 b209 bad9 cad5 dc4e  U.x............N
+00002360: 93a4 2a22 b117 ec34 4d69 6372 6f73 6f66  ..*"...4Microsof
+00002370: 742e 4353 6861 7270 2e64 6c6c 0000 0190  t.CSharp.dll....
+00002380: b7f7 da00 8000 0002 bf51 7cd8 89f6 45b8  .........Q|...E.
+00002390: 47ae 7603 9cc9 7e4d 6963 726f 736f 6674  G.v...~Microsoft
+000023a0: 2e56 6973 7561 6c42 6173 6963 2e43 6f72  .VisualBasic.Cor
+000023b0: 652e 646c 6c00 0001 6e94 3ef3 0020 0100  e.dll...n.>.. ..
+000023c0: 983f ef31 cb95 e040 93e1 3811 4ec5 0bcc  .?.1...@..8.N...
+000023d0: 4d69 6372 6f73 6f66 742e 5669 7375 616c  Microsoft.Visual
+000023e0: 4261 7369 632e 646c 6c00 0001 8f74 36d1  Basic.dll....t6.
+000023f0: 0080 0000 7bea d8d1 1ca5 d94b 8712 ee81  ....{......K....
+00002400: 3606 02cc 4d69 6372 6f73 6f66 742e 5769  6...Microsoft.Wi
+00002410: 6e33 322e 5072 696d 6974 6976 6573 2e64  n32.Primitives.d
+00002420: 6c6c 0000 01f5 4741 c300 8000 0044 f9d4  ll....GA.....D..
+00002430: b63a 8a03 438f 7881 b159 9916 d14d 6963  .:..C.x..Y...Mic
+00002440: 726f 736f 6674 2e57 696e 3332 2e52 6567  rosoft.Win32.Reg
+00002450: 6973 7472 792e 646c 6c00 0001 9d29 82c8  istry.dll....)..
+00002460: 00a0 0000 bd1d 9739 d520 7b43 a590 a101  .......9. {C....
+00002470: 09e1 b68f 6d73 636f 726c 6962 2e64 6c6c  ....mscorlib.dll
+00002480: 0000 01f6 672c f100 2001 00f2 341a e430  ....g,.. ...4..0
+00002490: b193 42af 3ebd 2e47 ab2e c34e 6174 7572  ..B.>..G...Natur
+000024a0: 616c 536f 7274 2e45 7874 656e 7369 6f6e  alSort.Extension
+000024b0: 2e64 6c6c 0000 01f2 df7e d400 8000 0092  .dll.....~......
+000024c0: 8324 6245 3e0f 40b4 034b fcc3 83cf ba6e  .$bE>.@..K.....n
+000024d0: 6574 7374 616e 6461 7264 2e64 6c6c 0000  etstandard.dll..
+000024e0: 0183 5935 8600 c001 004d d526 eda7 899a  ..Y5.....M.&....
+000024f0: 45bb a1d3 9579 1289 4850 726f 7065 7274  E....y..HPropert
+00002500: 7943 6861 6e67 6564 2e64 6c6c 0000 018b  yChanged.dll....
+00002510: 5a97 8a00 8000 0031 74ff 35d3 a634 4c90  Z......1t.5..4L.
+00002520: ea21 b0de 577f e053 6978 4c61 626f 7273  .!..W..SixLabors
+00002530: 2e49 6d61 6765 5368 6172 702e 646c 6c00  .ImageSharp.dll.
+00002540: 0001 3bda e6f9 0040 2000 0d43 ee7e 03cb  ..;....@ ..C.~..
+00002550: 7a4b a41a 0502 1378 bc82 5379 7374 656d  zK.....x..System
+00002560: 2e41 7070 436f 6e74 6578 742e 646c 6c00  .AppContext.dll.
+00002570: 0001 5098 5dd5 0080 0000 63b3 c130 39ef  ..P.].....c..09.
+00002580: eb4c 8d73 af89 a38c c3cb 5379 7374 656d  .L.s......System
+00002590: 2e42 7566 6665 7273 2e64 6c6c 0000 01cc  .Buffers.dll....
+000025a0: 49bb cd00 8000 0042 aa23 a17c 823a 48b8  I......B.#.|.:H.
+000025b0: 39e2 e40c d420 3753 7973 7465 6d2e 436f  9.... 7System.Co
+000025c0: 6c6c 6563 7469 6f6e 732e 436f 6e63 7572  llections.Concur
+000025d0: 7265 6e74 2e64 6c6c 0000 01f1 5ece c700  rent.dll....^...
+000025e0: a000 0047 f8cf ca22 bc5c 47b4 e052 51ce  ...G...".\G..RQ.
+000025f0: a1bb 8153 7973 7465 6d2e 436f 6c6c 6563  ...System.Collec
+00002600: 7469 6f6e 732e 646c 6c00 0001 cedb 82d9  tions.dll.......
+00002610: 0000 0100 b000 adf5 0126 b64c 8413 26e1  .........&.L..&.
+00002620: 61d7 722a 5379 7374 656d 2e43 6f6c 6c65  a.r*System.Colle
+00002630: 6374 696f 6e73 2e49 6d6d 7574 6162 6c65  ctions.Immutable
+00002640: 2e64 6c6c 0000 0133 269d aa00 4001 004d  .dll...3&...@..M
+00002650: c8e5 f4d7 ff63 469f d6d7 2ccf a9a8 1953  .....cF...,....S
+00002660: 7973 7465 6d2e 436f 6c6c 6563 7469 6f6e  ystem.Collection
+00002670: 732e 4e6f 6e47 656e 6572 6963 2e64 6c6c  s.NonGeneric.dll
+00002680: 0000 012a 5464 fd00 a000 00f7 dcc2 7db8  ...*Td........}.
+00002690: 0995 4e98 9f40 a313 58e5 1153 7973 7465  ..N..@..X..Syste
+000026a0: 6d2e 436f 6c6c 6563 7469 6f6e 732e 5370  m.Collections.Sp
+000026b0: 6563 6961 6c69 7a65 642e 646c 6c00 0001  ecialized.dll...
+000026c0: 91bc fbf7 00a0 0000 b976 b1fe e642 864a  .........v...B.J
+000026d0: acc6 f46b 96a4 548a 5379 7374 656d 2e43  ...k..T.System.C
+000026e0: 6f6d 706f 6e65 6e74 4d6f 6465 6c2e 416e  omponentModel.An
+000026f0: 6e6f 7461 7469 6f6e 732e 646c 6c00 0001  notations.dll...
+00002700: aceb 1ef6 00c0 0000 bea9 50cc e4f4 234f  ..........P...#O
+00002710: 9689 0316 8081 bd8b 5379 7374 656d 2e43  ........System.C
+00002720: 6f6d 706f 6e65 6e74 4d6f 6465 6c2e 4461  omponentModel.Da
+00002730: 7461 416e 6e6f 7461 7469 6f6e 732e 646c  taAnnotations.dl
+00002740: 6c00 0001 d2ba b0b0 0080 0000 c6be 8af3  l...............
+00002750: aa01 8f43 99c0 220a 479a aa58 5379 7374  ...C..".G..XSyst
+00002760: 656d 2e43 6f6d 706f 6e65 6e74 4d6f 6465  em.ComponentMode
+00002770: 6c2e 646c 6c00 0001 c0d2 c885 0080 0000  l.dll...........
+00002780: 6640 632d 1669 ef4a a2d7 eab7 2fc3 0c04  f@c-.i.J..../...
+00002790: 5379 7374 656d 2e43 6f6d 706f 6e65 6e74  System.Component
+000027a0: 4d6f 6465 6c2e 4576 656e 7442 6173 6564  Model.EventBased
+000027b0: 4173 796e 632e 646c 6c00 0001 aa5d 0bed  Async.dll....]..
+000027c0: 0080 0000 fab9 dd69 d926 cb40 bc36 979f  .......i.&.@.6..
+000027d0: e336 231c 5379 7374 656d 2e43 6f6d 706f  .6#.System.Compo
+000027e0: 6e65 6e74 4d6f 6465 6c2e 5072 696d 6974  nentModel.Primit
+000027f0: 6976 6573 2e64 6c6c 0000 0103 3edb a600  ives.dll....>...
+00002800: a000 00e1 4a5f 190e 79ec 45b5 de71 ac2d  ....J_..y.E..q.-
+00002810: d94e e653 7973 7465 6d2e 436f 6d70 6f6e  .N.System.Compon
+00002820: 656e 744d 6f64 656c 2e54 7970 6543 6f6e  entModel.TypeCon
+00002830: 7665 7274 6572 2e64 6c6c 0000 013f 357a  verter.dll...?5z
+00002840: 9800 c001 0039 bdca 3079 46df 48b3 8afc  .....9..0yF.H...
+00002850: 551d 0595 5653 7973 7465 6d2e 436f 6e66  U...VSystem.Conf
+00002860: 6967 7572 6174 696f 6e2e 646c 6c00 0001  iguration.dll...
+00002870: 5d23 b8c5 0080 0000 cdb2 fba9 39b5 694f  ]#..........9.iO
+00002880: 9ffe cc67 fd11 7312 5379 7374 656d 2e43  ...g..s.System.C
+00002890: 6f6e 736f 6c65 2e64 6c6c 0000 0179 a1c9  onsole.dll...y..
+000028a0: fa00 a000 00fd 414e a49a f577 49b5 9667  ......AN...wI..g
+000028b0: 9571 3761 be53 7973 7465 6d2e 436f 7265  .q7a.System.Core
+000028c0: 2e64 6c6c 0000 01a8 7b0e db00 a000 006e  .dll....{......n
+000028d0: cb5c 54b5 1a70 428d 9cd8 594b 5afd 9853  .\T..pB...YKZ..S
+000028e0: 7973 7465 6d2e 4461 7461 2e43 6f6d 6d6f  ystem.Data.Commo
+000028f0: 6e2e 646c 6c00 0001 5b42 f8ee 0080 0200  n.dll...[B......
+00002900: 0a63 3114 0b2d 0d45 a9d1 b116 3456 9dc4  .c1..-.E....4V..
+00002910: 5379 7374 656d 2e44 6174 612e 4461 7461  System.Data.Data
+00002920: 5365 7445 7874 656e 7369 6f6e 732e 646c  SetExtensions.dl
+00002930: 6c00 0001 8b62 4ed2 0080 0000 bfd8 8565  l....bN........e
+00002940: 95bb 3447 bb37 e1e4 37c1 9911 5379 7374  ..4G.7..7...Syst
+00002950: 656d 2e44 6174 612e 646c 6c00 0001 1985  em.Data.dll.....
+00002960: 12f0 00a0 0000 934e 3b58 88a9 764b b006  .......N;X..vK..
+00002970: 8803 8996 db4a 5379 7374 656d 2e44 6961  .....JSystem.Dia
+00002980: 676e 6f73 7469 6373 2e43 6f6e 7472 6163  gnostics.Contrac
+00002990: 7473 2e64 6c6c 0000 01f0 e969 8a00 8000  ts.dll.....i....
+000029a0: 00c0 61cf ba60 0f2d 4598 094c 7855 1b61  ..a..`.-E..LxU.a
+000029b0: f853 7973 7465 6d2e 4469 6167 6e6f 7374  .System.Diagnost
+000029c0: 6963 732e 4465 6275 672e 646c 6c00 0001  ics.Debug.dll...
+000029d0: 4015 a8cb 0080 0000 932a 7b58 53a6 3a47  @........*{XS.:G
+000029e0: 926a be96 c1f3 3482 5379 7374 656d 2e44  .j....4.System.D
+000029f0: 6961 676e 6f73 7469 6373 2e44 6961 676e  iagnostics.Diagn
+00002a00: 6f73 7469 6353 6f75 7263 652e 646c 6c00  osticSource.dll.
+00002a10: 0001 48de 52f8 00c0 0000 1cf1 f85e 3aaa  ..H.R........^:.
+00002a20: 4b43 a27d 312e 15b5 2a76 5379 7374 656d  KC.}1...*vSystem
+00002a30: 2e44 6961 676e 6f73 7469 6373 2e46 696c  .Diagnostics.Fil
+00002a40: 6556 6572 7369 6f6e 496e 666f 2e64 6c6c  eVersionInfo.dll
+00002a50: 0000 0129 c5bb 9300 8000 0070 e8bb f93f  ...).......p...?
+00002a60: 4286 42bc b28e 02e9 c4fc 7a53 7973 7465  B.B.......zSyste
+00002a70: 6d2e 4469 6167 6e6f 7374 6963 732e 5072  m.Diagnostics.Pr
+00002a80: 6f63 6573 732e 646c 6c00 0001 0a9a dd82  ocess.dll.......
+00002a90: 00c0 0000 8775 042f 74d1 3745 baf2 b029  .....u./t.7E...)
+00002aa0: 3aec 958c 5379 7374 656d 2e44 6961 676e  :...System.Diagn
+00002ab0: 6f73 7469 6373 2e53 7461 636b 5472 6163  ostics.StackTrac
+00002ac0: 652e 646c 6c00 0001 a52a 0df2 00a0 0000  e.dll....*......
+00002ad0: 8768 db59 3fc1 404e 95de 4fa4 7b7e bc7d  .h.Y?.@N..O.{~.}
+00002ae0: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
+00002af0: 6373 2e54 6578 7457 7269 7465 7254 7261  cs.TextWriterTra
+00002b00: 6365 4c69 7374 656e 6572 2e64 6c6c 0000  ceListener.dll..
+00002b10: 0193 2a55 d200 8000 0002 b86f f9c7 507e  ..*U.......o..P~
+00002b20: 4b8e 1a2e 05fa b72a 9453 7973 7465 6d2e  K......*.System.
+00002b30: 4469 6167 6e6f 7374 6963 732e 546f 6f6c  Diagnostics.Tool
+00002b40: 732e 646c 6c00 0001 117a d2ba 0080 0000  s.dll....z......
+00002b50: 0d25 cefc 5cdb 6948 8945 ba1c 3e3c 5343  .%..\.iH.E..><SC
+00002b60: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
+00002b70: 6373 2e54 7261 6365 536f 7572 6365 2e64  cs.TraceSource.d
+00002b80: 6c6c 0000 0102 2358 f700 a000 009a 7fe2  ll....#X........
+00002b90: 801c 1e53 4394 133e 6eea 056d c753 7973  ...SC..>n..m.Sys
+00002ba0: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
+00002bb0: 5472 6163 696e 672e 646c 6c00 0001 dd66  Tracing.dll....f
+00002bc0: 14d9 00a0 0000 5f8b 559e e617 4441 8b85  ......_.U...DA..
+00002bd0: 844c adc7 ae45 5379 7374 656d 2e64 6c6c  .L...ESystem.dll
+00002be0: 0000 01e4 f024 f900 0001 00b5 4281 cb66  .....$......B..f
+00002bf0: 7d19 4d85 c7af f759 5cd7 b453 7973 7465  }.M....Y\..Syste
+00002c00: 6d2e 4472 6177 696e 672e 436f 6d6d 6f6e  m.Drawing.Common
+00002c10: 2e64 6c6c 0000 0121 8d42 d500 2002 0008  .dll...!.B.. ...
+00002c20: 43fe c06a 78bb 469f 62dc 8ac5 b55a bc53  C..jx.F.b....Z.S
+00002c30: 7973 7465 6d2e 4472 6177 696e 672e 646c  ystem.Drawing.dl
+00002c40: 6c00 0001 950e c9f9 0080 0000 01c6 7517  l.............u.
+00002c50: b781 9545 8c15 b804 af68 b533 5379 7374  ...E.....h.3Syst
+00002c60: 656d 2e44 7261 7769 6e67 2e50 7269 6d69  em.Drawing.Primi
+00002c70: 7469 7665 732e 646c 6c00 0001 45b3 c2ab  tives.dll...E...
+00002c80: 00c0 0000 355a d266 3dff 9741 b81c bb16  ....5Z.f=..A....
+00002c90: e2f8 3ad7 5379 7374 656d 2e44 796e 616d  ..:.System.Dynam
+00002ca0: 6963 2e52 756e 7469 6d65 2e64 6c6c 0000  ic.Runtime.dll..
+00002cb0: 01b9 c1b9 ce00 8000 006f 0d16 6f04 e818  .........o..o...
+00002cc0: 43ac 1e99 260a 1b43 7053 7973 7465 6d2e  C...&..CpSystem.
+00002cd0: 466f 726d 6174 732e 4173 6e31 2e64 6c6c  Formats.Asn1.dll
+00002ce0: 0000 010c e173 de00 a000 007c e231 9758  .....s.....|.1.X
+00002cf0: 5b77 419b 52e7 b44b 2509 0153 7973 7465  [wA.R..K%..Syste
+00002d00: 6d2e 476c 6f62 616c 697a 6174 696f 6e2e  m.Globalization.
+00002d10: 4361 6c65 6e64 6172 732e 646c 6c00 0001  Calendars.dll...
+00002d20: 87a2 cdf5 0080 0000 1d48 e933 e32a ec4c  .........H.3.*.L
+00002d30: 8881 bf0d 2fcb 0df1 5379 7374 656d 2e47  ..../...System.G
+00002d40: 6c6f 6261 6c69 7a61 7469 6f6e 2e64 6c6c  lobalization.dll
+00002d50: 0000 016c 3098 a200 8000 006f 416e 0f43  ...l0......oAn.C
+00002d60: bf18 438e 564a 0101 b0d5 7753 7973 7465  ..C.VJ....wSyste
+00002d70: 6d2e 476c 6f62 616c 697a 6174 696f 6e2e  m.Globalization.
+00002d80: 4578 7465 6e73 696f 6e73 2e64 6c6c 0000  Extensions.dll..
+00002d90: 01bc 0f66 ea00 8000 008e 5987 3774 e153  ...f......Y.7t.S
+00002da0: 439f cade 4d3a 9536 9b53 7973 7465 6d2e  C...M:.6.System.
+00002db0: 494f 2e43 6f6d 7072 6573 7369 6f6e 2e42  IO.Compression.B
+00002dc0: 726f 746c 692e 646c 6c00 0001 b86f adfe  rotli.dll....o..
+00002dd0: 0080 0000 faaf 58e7 26e4 a448 818b 16d6  ......X.&..H....
+00002de0: e8d6 3163 5379 7374 656d 2e49 4f2e 436f  ..1cSystem.IO.Co
+00002df0: 6d70 7265 7373 696f 6e2e 646c 6c00 0001  mpression.dll...
+00002e00: 138f 71b8 00a0 0000 1ae9 9681 2081 a049  ..q......... ..I
+00002e10: b6f1 f5bf a087 327e 5379 7374 656d 2e49  ......2~System.I
+00002e20: 4f2e 436f 6d70 7265 7373 696f 6e2e 4669  O.Compression.Fi
+00002e30: 6c65 5379 7374 656d 2e64 6c6c 0000 0120  leSystem.dll... 
+00002e40: 31e3 ef00 8000 00d7 4240 8e69 d733 4795  1.......B@.i.3G.
+00002e50: 7160 5402 d9a2 7753 7973 7465 6d2e 494f  q`T...wSystem.IO
+00002e60: 2e43 6f6d 7072 6573 7369 6f6e 2e5a 6970  .Compression.Zip
+00002e70: 4669 6c65 2e64 6c6c 0000 01fd 9d13 f900  File.dll........
+00002e80: 8000 0061 9000 02b8 be32 4a90 ee5a 3708  ...a.....2J..Z7.
+00002e90: 9487 8b53 7973 7465 6d2e 494f 2e64 6c6c  ...System.IO.dll
+00002ea0: 0000 018e 03f1 aa00 8000 00ef 2112 2b55  ............!.+U
+00002eb0: ec28 42a4 c946 5d8d b924 5a53 7973 7465  .(B..F]..$ZSyste
+00002ec0: 6d2e 494f 2e46 696c 6553 7973 7465 6d2e  m.IO.FileSystem.
+00002ed0: 4163 6365 7373 436f 6e74 726f 6c2e 646c  AccessControl.dl
+00002ee0: 6c00 0001 bcd9 4ba3 00a0 0000 1f12 af19  l.....K.........
+00002ef0: 095e ae42 ba6d 366b d407 6820 5379 7374  .^.B.m6k..h Syst
+00002f00: 656d 2e49 4f2e 4669 6c65 5379 7374 656d  em.IO.FileSystem
+00002f10: 2e64 6c6c 0000 0128 52e6 fc00 8000 0019  .dll...(R.......
+00002f20: ba4d 2471 e2f7 4f99 820f 2811 c9b9 9d53  .M$q..O...(....S
+00002f30: 7973 7465 6d2e 494f 2e46 696c 6553 7973  ystem.IO.FileSys
+00002f40: 7465 6d2e 4472 6976 6549 6e66 6f2e 646c  tem.DriveInfo.dl
+00002f50: 6c00 0001 b4e5 138e 0080 0000 4555 1c03  l...........EU..
+00002f60: 2359 7446 9923 cf08 f4da e719 5379 7374  #YtF.#......Syst
+00002f70: 656d 2e49 4f2e 4669 6c65 5379 7374 656d  em.IO.FileSystem
+00002f80: 2e50 7269 6d69 7469 7665 732e 646c 6c00  .Primitives.dll.
+00002f90: 0001 a311 45cd 0080 0000 c81b 3339 252b  ....E.......39%+
+00002fa0: 4f42 9747 3780 2bde 2e69 5379 7374 656d  OB.G7.+..iSystem
+00002fb0: 2e49 4f2e 4669 6c65 5379 7374 656d 2e57  .IO.FileSystem.W
+00002fc0: 6174 6368 6572 2e64 6c6c 0000 010d d21b  atcher.dll......
+00002fd0: 8200 a000 00c8 b49a 4425 88fb 44a1 4117  ........D%..D.A.
+00002fe0: 3b8e 1b16 7b53 7973 7465 6d2e 494f 2e49  ;...{System.IO.I
+00002ff0: 736f 6c61 7465 6453 746f 7261 6765 2e64  solatedStorage.d
+00003000: 6c6c 0000 01f2 acc3 a000 a000 006e b8b5  ll...........n..
+00003010: 85a4 92b6 41a1 ccd4 2499 fe3a 5153 7973  ....A...$..:QSys
+00003020: 7465 6d2e 494f 2e4d 656d 6f72 794d 6170  tem.IO.MemoryMap
+00003030: 7065 6446 696c 6573 2e64 6c6c 0000 0166  pedFiles.dll...f
+00003040: 1d17 8e00 8000 003f 928a 0869 d4cc 459f  .......?...i..E.
+00003050: 62d0 4060 df4f 3153 7973 7465 6d2e 494f  b.@`.O1System.IO
+00003060: 2e50 6970 6573 2e41 6363 6573 7343 6f6e  .Pipes.AccessCon
+00003070: 7472 6f6c 2e64 6c6c 0000 01f2 e4e0 9e00  trol.dll........
+00003080: 8000 00ac 0361 4155 c9f3 4680 8e62 74e6  .....aAU..F..bt.
+00003090: 3d7e 4d53 7973 7465 6d2e 494f 2e50 6970  =~MSystem.IO.Pip
+000030a0: 6573 2e64 6c6c 0000 01f8 690c ce00 a000  es.dll....i.....
+000030b0: 00cf 7a29 ebb4 8bb9 4dbe 51ab e2c7 4f19  ..z)....M.Q...O.
+000030c0: d153 7973 7465 6d2e 494f 2e55 6e6d 616e  .System.IO.Unman
+000030d0: 6167 6564 4d65 6d6f 7279 5374 7265 616d  agedMemoryStream
+000030e0: 2e64 6c6c 0000 0138 5620 f000 8000 0088  .dll...8V ......
+000030f0: 1146 331a d1bb 4cae 182e 7e42 b5a2 f753  .F3...L...~B...S
+00003100: 7973 7465 6d2e 4c69 6e71 2e64 6c6c 0000  ystem.Linq.dll..
+00003110: 010b cc1a 8300 c000 009b 25e8 7f7a 3c9b  ..........%..z<.
+00003120: 4190 2cad 9f56 5c9f 7253 7973 7465 6d2e  A.,..V\.rSystem.
+00003130: 4c69 6e71 2e45 7870 7265 7373 696f 6e73  Linq.Expressions
+00003140: 2e64 6c6c 0000 0179 6685 b300 4001 000c  .dll...yf...@...
+00003150: fa9f fe83 250c 41bf 5392 459f c189 8153  ....%.A.S.E....S
+00003160: 7973 7465 6d2e 4c69 6e71 2e50 6172 616c  ystem.Linq.Paral
+00003170: 6c65 6c2e 646c 6c00 0001 4455 84a1 00c0  lel.dll...DU....
+00003180: 0000 689a 81a1 bac8 354f b65e 96f2 1fbd  ..h.....5O.^....
+00003190: 972f 5379 7374 656d 2e4c 696e 712e 5175  ./System.Linq.Qu
+000031a0: 6572 7961 626c 652e 646c 6c00 0001 62e9  eryable.dll...b.
+000031b0: f2c2 00c0 0000 02af 4034 c6c2 784f 9f1b  ........@4..xO..
+000031c0: 3cdc c7bc 2ab4 5379 7374 656d 2e4d 656d  <...*.System.Mem
+000031d0: 6f72 792e 646c 6c00 0001 8953 afd7 00e0  ory.dll....S....
+000031e0: 0000 35a6 bb5f aeb4 c94c 8682 07fc 22b2  ..5.._...L....".
+000031f0: a65c 5379 7374 656d 2e4e 6574 2e64 6c6c  .\System.Net.dll
+00003200: 0000 0169 4722 ea00 8000 0049 da92 7cb9  ...iG".....I..|.
+00003210: 905c 49b7 a800 ae87 db5a c653 7973 7465  .\I......Z.Syste
+00003220: 6d2e 4e65 742e 4874 7470 2e64 6c6c 0000  m.Net.Http.dll..
+00003230: 01c1 110c b700 2001 0022 e637 a280 8f3f  ...... ..".7...?
+00003240: 41a6 e29f fee3 0ee1 3953 7973 7465 6d2e  A.......9System.
+00003250: 4e65 742e 4874 7470 2e4a 736f 6e2e 646c  Net.Http.Json.dl
+00003260: 6c00 0001 8cdc 6188 0080 0000 b28b 7b2e  l.....a.......{.
+00003270: 85f2 da46 9863 b96f fd8e 4d7b 5379 7374  ...F.c.o..M{Syst
+00003280: 656d 2e4e 6574 2e48 7474 704c 6973 7465  em.Net.HttpListe
+00003290: 6e65 722e 646c 6c00 0001 e0d3 4b83 00a0  ner.dll.....K...
+000032a0: 0000 6aa0 267d 15e2 3e4b a13e 031e 8e40  ..j.&}..>K.>...@
+000032b0: 295f 5379 7374 656d 2e4e 6574 2e4d 6169  )_System.Net.Mai
+000032c0: 6c2e 646c 6c00 0001 d5c6 74ea 00c0 0000  l.dll.....t.....
+000032d0: 2d6c 5c70 7991 9d47 8d95 287f cc03 ccf0  -l\py..G..(.....
+000032e0: 5379 7374 656d 2e4e 6574 2e4e 616d 6552  System.Net.NameR
+000032f0: 6573 6f6c 7574 696f 6e2e 646c 6c00 0001  esolution.dll...
+00003300: cd77 b08f 0080 0000 8417 f30f 81a3 7d4c  .w............}L
+00003310: 8312 cbf4 47f9 6bf6 5379 7374 656d 2e4e  ....G.k.System.N
+00003320: 6574 2e4e 6574 776f 726b 496e 666f 726d  et.NetworkInform
+00003330: 6174 696f 6e2e 646c 6c00 0001 2e75 60cf  ation.dll....u`.
+00003340: 00c0 0000 53a1 aa29 6d30 e84b 9209 cd2e  ....S..)m0.K....
+00003350: d2a4 10a4 5379 7374 656d 2e4e 6574 2e50  ....System.Net.P
+00003360: 696e 672e 646c 6c00 0001 4786 7ffd 0080  ing.dll...G.....
+00003370: 0000 c487 da6a 9c62 e44d 879c 7e40 a009  .....j.b.M..~@..
+00003380: 9db8 5379 7374 656d 2e4e 6574 2e50 7269  ..System.Net.Pri
+00003390: 6d69 7469 7665 732e 646c 6c00 0001 4b76  mitives.dll...Kv
+000033a0: 99e7 00c0 0000 ab76 7ebe 969d 0f48 b49f  .......v~....H..
+000033b0: 5c16 75da 6273 5379 7374 656d 2e4e 6574  \.u.bsSystem.Net
+000033c0: 2e52 6571 7565 7374 732e 646c 6c00 0001  .Requests.dll...
+000033d0: 7dbc 9ccf 00e0 0000 b116 128b 1810 c64d  }..............M
+000033e0: 9ab5 450c a275 649d 5379 7374 656d 2e4e  ..E..ud.System.N
+000033f0: 6574 2e53 6563 7572 6974 792e 646c 6c00  et.Security.dll.
+00003400: 0001 566c 68e0 0000 0100 9197 e28a d4b4  ..Vlh...........
+00003410: 3848 905f c725 6100 1c2d 5379 7374 656d  8H._.%a..-System
+00003420: 2e4e 6574 2e53 6572 7669 6365 506f 696e  .Net.ServicePoin
+00003430: 742e 646c 6c00 0001 80ea 6586 0080 0000  t.dll.....e.....
+00003440: 814c 94a2 4d3e 5349 9b40 34d3 f36c 40b5  .L..M>SI.@4..l@.
+00003450: 5379 7374 656d 2e4e 6574 2e53 6f63 6b65  System.Net.Socke
+00003460: 7473 2e64 6c6c 0000 0137 00ad 8700 0001  ts.dll...7......
+00003470: 00c0 7863 7bff 41e1 459e de56 f210 5af7  ..xc{.A.E..V..Z.
+00003480: 1153 7973 7465 6d2e 4e65 742e 5765 6243  .System.Net.WebC
+00003490: 6c69 656e 742e 646c 6c00 0001 e853 72f3  lient.dll....Sr.
+000034a0: 00a0 0000 deb3 5eab 571b 8e4d 9630 997c  ......^.W..M.0.|
+000034b0: 941e 7aae 5379 7374 656d 2e4e 6574 2e57  ..z.System.Net.W
+000034c0: 6562 4865 6164 6572 436f 6c6c 6563 7469  ebHeaderCollecti
+000034d0: 6f6e 2e64 6c6c 0000 0153 c4ac 9f00 8000  on.dll...S......
+000034e0: 0007 563e cf35 6910 4983 042e 0c7b 0bed  ..V>.5i.I....{..
+000034f0: 7853 7973 7465 6d2e 4e65 742e 5765 6250  xSystem.Net.WebP
+00003500: 726f 7879 2e64 6c6c 0000 010a 45d2 c000  roxy.dll....E...
+00003510: 8000 0057 028c 0931 68be 48ae b5ff e2fb  ...W...1h.H.....
+00003520: 9106 3d53 7973 7465 6d2e 4e65 742e 5765  ..=System.Net.We
+00003530: 6253 6f63 6b65 7473 2e43 6c69 656e 742e  bSockets.Client.
+00003540: 646c 6c00 0001 66f1 8abb 0080 0000 fdc2  dll...f.........
+00003550: 24b7 c698 9e49 8b17 951d 2a30 f029 5379  $....I....*0.)Sy
+00003560: 7374 656d 2e4e 6574 2e57 6562 536f 636b  stem.Net.WebSock
+00003570: 6574 732e 646c 6c00 0001 8211 728b 00a0  ets.dll.....r...
+00003580: 0000 5665 8daf b779 aa48 9a1f 9d64 da3e  ..Ve...y.H...d.>
+00003590: e4e1 5379 7374 656d 2e4e 756d 6572 6963  ..System.Numeric
+000035a0: 732e 646c 6c00 0001 2969 11bc 0080 0000  s.dll...)i......
+000035b0: 35ef 3669 8a2b 3c40 994c 6412 532d 2f69  5.6i.+<@.Ld.S-/i
+000035c0: 5379 7374 656d 2e4e 756d 6572 6963 732e  System.Numerics.
+000035d0: 5665 6374 6f72 732e 646c 6c00 0001 c9c0  Vectors.dll.....
+000035e0: 82a2 00c0 0000 292c 7b98 41a8 304f 9df6  ......),{.A.0O..
+000035f0: ae3f 29ab 22c6 5379 7374 656d 2e4f 626a  .?).".System.Obj
+00003600: 6563 744d 6f64 656c 2e64 6c6c 0000 0180  ectModel.dll....
+00003610: f76d db00 c000 00f6 7968 42e3 076c 498b  .m......yhB..lI.
+00003620: f691 900a 1377 a453 7973 7465 6d2e 5265  .....w.System.Re
+00003630: 666c 6563 7469 6f6e 2e44 6973 7061 7463  flection.Dispatc
+00003640: 6850 726f 7879 2e64 6c6c 0000 0101 ded8  hProxy.dll......
+00003650: d900 8000 009f 1e13 9798 c643 43a9 dd5a  ...........CC..Z
+00003660: 15f9 da8e 9f53 7973 7465 6d2e 5265 666c  .....System.Refl
+00003670: 6563 7469 6f6e 2e64 6c6c 0000 015f 54f1  ection.dll..._T.
+00003680: af00 8000 00a4 4fbb 49d5 bb9f 4c81 a888  ......O.I...L...
+00003690: 584d f5f8 b053 7973 7465 6d2e 5265 666c  XM...System.Refl
+000036a0: 6563 7469 6f6e 2e45 6d69 742e 646c 6c00  ection.Emit.dll.
+000036b0: 0001 f656 c9d1 00e0 0000 527c f24b 230b  ...V......R|.K#.
+000036c0: 914c 9ee8 9e48 bc69 e433 5379 7374 656d  .L...H.i.3System
+000036d0: 2e52 6566 6c65 6374 696f 6e2e 456d 6974  .Reflection.Emit
+000036e0: 2e49 4c47 656e 6572 6174 696f 6e2e 646c  .ILGeneration.dl
+000036f0: 6c00 0001 d0cc 528a 00a0 0000 6a47 2ce2  l.....R.....jG,.
+00003700: f0c7 4044 b96e 5e8e c09d ff84 5379 7374  ..@D.n^.....Syst
+00003710: 656d 2e52 6566 6c65 6374 696f 6e2e 456d  em.Reflection.Em
+00003720: 6974 2e4c 6967 6874 7765 6967 6874 2e64  it.Lightweight.d
+00003730: 6c6c 0000 0181 9008 9900 8000 008e ab92  ll..............
+00003740: f552 6a17 42ba 3cfa ef67 d7be dc53 7973  .Rj.B.<..g...Sys
+00003750: 7465 6d2e 5265 666c 6563 7469 6f6e 2e45  tem.Reflection.E
+00003760: 7874 656e 7369 6f6e 732e 646c 6c00 0001  xtensions.dll...
+00003770: 8e2f 0290 0080 0000 ed7c 7ac1 3b68 d340  ./.......|z.;h.@
+00003780: b1e9 1cd5 f9b5 a0cc 5379 7374 656d 2e52  ........System.R
+00003790: 6566 6c65 6374 696f 6e2e 4d65 7461 6461  eflection.Metada
+000037a0: 7461 2e64 6c6c 0000 01e1 cfc8 ce00 2002  ta.dll........ .
+000037b0: 004b 198d c8c8 0be1 4685 8caa 2893 dc56  .K......F...(..V
+000037c0: e453 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
+000037d0: 6f6e 2e50 7269 6d69 7469 7665 732e 646c  on.Primitives.dl
+000037e0: 6c00 0001 cdf7 acf2 00a0 0000 0ff8 60a3  l.............`.
+000037f0: fd8e 844a 9269 4a45 e940 0c3d 5379 7374  ...J.iJE.@.=Syst
+00003800: 656d 2e52 6566 6c65 6374 696f 6e2e 5479  em.Reflection.Ty
+00003810: 7065 4578 7465 6e73 696f 6e73 2e64 6c6c  peExtensions.dll
+00003820: 0000 0179 2bdb cf00 8000 0052 ac92 ba89  ...y+......R....
+00003830: 813e 48b7 dac0 4645 c4d3 2053 7973 7465  .>H...FE.. Syste
+00003840: 6d2e 5265 736f 7572 6365 732e 5265 6164  m.Resources.Read
+00003850: 6572 2e64 6c6c 0000 0134 22d6 a600 8000  er.dll...4".....
+00003860: 0055 f605 bbbe f6ea 4aac 94f1 ba2e 9835  .U......J......5
+00003870: 0953 7973 7465 6d2e 5265 736f 7572 6365  .System.Resource
+00003880: 732e 5265 736f 7572 6365 4d61 6e61 6765  s.ResourceManage
+00003890: 722e 646c 6c00 0001 497b a9b6 0080 0000  r.dll...I{......
+000038a0: c99d 9a68 6639 2544 978b fcc9 2efa 581c  ...hf9%D......X.
+000038b0: 5379 7374 656d 2e52 6573 6f75 7263 6573  System.Resources
+000038c0: 2e57 7269 7465 722e 646c 6c00 0001 40b3  .Writer.dll...@.
+000038d0: 3aca 0080 0000 8d42 0f61 dada 6349 8d3a  :......B.a..cI.:
+000038e0: 4d16 18c6 2e42 5379 7374 656d 2e52 756e  M....BSystem.Run
+000038f0: 7469 6d65 2e43 6f6d 7069 6c65 7253 6572  time.CompilerSer
+00003900: 7669 6365 732e 556e 7361 6665 2e64 6c6c  vices.Unsafe.dll
+00003910: 0000 014a a3ce 8900 8000 00d9 87bf 498f  ...J..........I.
+00003920: 333c 4ab3 c9c2 7112 71fb 2253 7973 7465  3<J...q.q."Syste
+00003930: 6d2e 5275 6e74 696d 652e 436f 6d70 696c  m.Runtime.Compil
+00003940: 6572 5365 7276 6963 6573 2e56 6973 7561  erServices.Visua
+00003950: 6c43 2e64 6c6c 0000 0178 9010 e900 8000  lC.dll...x......
+00003960: 009d 8b55 682d a38d 41b9 94a5 a6fe 901d  ...Uh-..A.......
+00003970: 5453 7973 7465 6d2e 5275 6e74 696d 652e  TSystem.Runtime.
+00003980: 646c 6c00 0001 7175 28ad 0080 0700 0d93  dll...qu(.......
+00003990: ab77 873d d44b 8b9d b4da c495 304b 5379  .w.=.K......0KSy
+000039a0: 7374 656d 2e52 756e 7469 6d65 2e45 7874  stem.Runtime.Ext
+000039b0: 656e 7369 6f6e 732e 646c 6c00 0001 a750  ensions.dll....P
+000039c0: 82dc 0080 0000 d170 e615 7b65 e84d b7e5  .......p..{e.M..
+000039d0: a725 5c80 f9b4 5379 7374 656d 2e52 756e  .%\...System.Run
+000039e0: 7469 6d65 2e48 616e 646c 6573 2e64 6c6c  time.Handles.dll
+000039f0: 0000 0138 1582 c400 8000 008d 99e5 04f6  ...8............
+00003a00: 51c7 4698 58d9 08e6 8f9b 3653 7973 7465  Q.F.X.....6Syste
+00003a10: 6d2e 5275 6e74 696d 652e 496e 7465 726f  m.Runtime.Intero
+00003a20: 7053 6572 7669 6365 732e 646c 6c00 0001  pServices.dll...
+00003a30: d565 85a4 0040 0100 f7ab 7f09 2004 4c49  .e...@...... .LI
+00003a40: 857f 4cf8 65f8 c0da 5379 7374 656d 2e52  ..L.e...System.R
+00003a50: 756e 7469 6d65 2e49 6e74 6572 6f70 5365  untime.InteropSe
+00003a60: 7276 6963 6573 2e52 756e 7469 6d65 496e  rvices.RuntimeIn
+00003a70: 666f 726d 6174 696f 6e2e 646c 6c00 0001  formation.dll...
+00003a80: 81bb 82fb 0080 0000 a762 3fa2 4ed0 bd4e  .........b?.N..N
+00003a90: bace e9cf ee64 0873 5379 7374 656d 2e52  .....d.sSystem.R
+00003aa0: 756e 7469 6d65 2e49 6e74 7269 6e73 6963  untime.Intrinsic
+00003ab0: 732e 646c 6c00 0001 cba4 f89f 00c0 0200  s.dll...........
+00003ac0: 488f 960c c488 4c4b 987d 2735 dbb1 a1f1  H.....LK.}'5....
+00003ad0: 5379 7374 656d 2e52 756e 7469 6d65 2e4c  System.Runtime.L
+00003ae0: 6f61 6465 722e 646c 6c00 0001 2e5c 20ac  oader.dll....\ .
+00003af0: 0080 0000 3fb5 afb0 5ca1 9846 ae12 d8b1  ....?...\..F....
+00003b00: e15f dfcc 5379 7374 656d 2e52 756e 7469  ._..System.Runti
+00003b10: 6d65 2e4e 756d 6572 6963 732e 646c 6c00  me.Numerics.dll.
+00003b20: 0001 a11a 1fb6 00a0 0000 e7b0 b739 037c  .............9.|
+00003b30: 1c40 97b3 8a49 3691 f51c 5379 7374 656d  .@...I6...System
+00003b40: 2e52 756e 7469 6d65 2e53 6572 6961 6c69  .Runtime.Seriali
+00003b50: 7a61 7469 6f6e 2e64 6c6c 0000 01b8 b010  zation.dll......
+00003b60: 9600 8000 0054 2c81 23e9 9d4b 458c 404d  .....T,.#..KE.@M
+00003b70: 0077 edc4 7253 7973 7465 6d2e 5275 6e74  .w..rSystem.Runt
+00003b80: 696d 652e 5365 7269 616c 697a 6174 696f  ime.Serializatio
+00003b90: 6e2e 466f 726d 6174 7465 7273 2e64 6c6c  n.Formatters.dll
+00003ba0: 0000 0192 2056 8e00 a000 0083 5794 72d6  .... V......W.r.
+00003bb0: 41b6 4c82 1cf6 84be 27cf 0153 7973 7465  A.L.....'..Syste
+00003bc0: 6d2e 5275 6e74 696d 652e 5365 7269 616c  m.Runtime.Serial
+00003bd0: 697a 6174 696f 6e2e 4a73 6f6e 2e64 6c6c  ization.Json.dll
+00003be0: 0000 018c d031 8900 8000 00b6 67d3 b931  .....1......g..1
+00003bf0: c09b 43b3 578b cbd6 8d9f 8253 7973 7465  ..C.W......Syste
+00003c00: 6d2e 5275 6e74 696d 652e 5365 7269 616c  m.Runtime.Serial
+00003c10: 697a 6174 696f 6e2e 5072 696d 6974 6976  ization.Primitiv
+00003c20: 6573 2e64 6c6c 0000 013a 616c cb00 8000  es.dll...:al....
+00003c30: 00c9 5960 56e5 ab6d 4782 bc64 c985 77c5  ..Y`V..mG..d..w.
+00003c40: 1a53 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+00003c50: 5365 7269 616c 697a 6174 696f 6e2e 586d  Serialization.Xm
+00003c60: 6c2e 646c 6c00 0001 a1a1 9085 00c0 0000  l.dll...........
+00003c70: e6cd 651f e244 0e4a 82e7 012e 7c72 34d5  ..e..D.J....|r4.
+00003c80: 5379 7374 656d 2e53 6563 7572 6974 792e  System.Security.
+00003c90: 4163 6365 7373 436f 6e74 726f 6c2e 646c  AccessControl.dl
+00003ca0: 6c00 0001 99f6 7c8d 00e0 0000 d3af 763b  l.....|.......v;
+00003cb0: 7d6b 5545 b122 fce8 b29a 5de2 5379 7374  }kUE."....].Syst
+00003cc0: 656d 2e53 6563 7572 6974 792e 436c 6169  em.Security.Clai
+00003cd0: 6d73 2e64 6c6c 0000 01e1 2d2d ab00 c000  ms.dll....--....
+00003ce0: 00be 69ff e59e d6e6 469f c937 4300 23ff  ..i.....F..7C.#.
+00003cf0: c553 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
+00003d00: 2e43 7279 7074 6f67 7261 7068 792e 416c  .Cryptography.Al
+00003d10: 676f 7269 7468 6d73 2e64 6c6c 0000 015b  gorithms.dll...[
+00003d20: fd04 ff00 0001 00aa c5b2 e3d3 1d84 4c96  ..............L.
+00003d30: dfb4 7da7 1778 8753 7973 7465 6d2e 5365  ..}..x.System.Se
+00003d40: 6375 7269 7479 2e43 7279 7074 6f67 7261  curity.Cryptogra
+00003d50: 7068 792e 436e 672e 646c 6c00 0001 8f28  phy.Cng.dll....(
+00003d60: 0ad7 00c0 0000 d298 a01f 2fe0 5543 8976  ........../.UC.v
+00003d70: 52e2 5091 8de8 5379 7374 656d 2e53 6563  R.P...System.Sec
+00003d80: 7572 6974 792e 4372 7970 746f 6772 6170  urity.Cryptograp
+00003d90: 6879 2e43 7370 2e64 6c6c 0000 01ed 734a  hy.Csp.dll....sJ
+00003da0: f200 a000 00eb a654 e4a0 6d13 4e95 ce4c  .......T..m.N..L
+00003db0: 14c7 c45b 2653 7973 7465 6d2e 5365 6375  ...[&System.Secu
+00003dc0: 7269 7479 2e43 7279 7074 6f67 7261 7068  rity.Cryptograph
+00003dd0: 792e 456e 636f 6469 6e67 2e64 6c6c 0000  y.Encoding.dll..
+00003de0: 010e 8f8f 8a00 a000 00f6 17ee 262b 286a  ............&+(j
+00003df0: 4cb9 8642 5164 1057 7f53 7973 7465 6d2e  L..BQd.W.System.
+00003e00: 5365 6375 7269 7479 2e43 7279 7074 6f67  Security.Cryptog
+00003e10: 7261 7068 792e 4f70 656e 5373 6c2e 646c  raphy.OpenSsl.dl
+00003e20: 6c00 0001 9604 9284 0080 0000 5dde 4b76  l...........].Kv
+00003e30: 6cb0 0847 932b 7d1c 1c47 2337 5379 7374  l..G.+}..G#7Syst
+00003e40: 656d 2e53 6563 7572 6974 792e 4372 7970  em.Security.Cryp
+00003e50: 746f 6772 6170 6879 2e50 7269 6d69 7469  tography.Primiti
+00003e60: 7665 732e 646c 6c00 0001 e13d bdfb 00a0  ves.dll....=....
+00003e70: 0000 4c85 6a80 de12 e146 8f26 662d 29a1  ..L.j....F.&f-).
+00003e80: cf72 5379 7374 656d 2e53 6563 7572 6974  .rSystem.Securit
+00003e90: 792e 4372 7970 746f 6772 6170 6879 2e58  y.Cryptography.X
+00003ea0: 3530 3943 6572 7469 6669 6361 7465 732e  509Certificates.
+00003eb0: 646c 6c00 0001 3611 e28c 00e0 0000 2cc4  dll...6.......,.
+00003ec0: 8139 49ee 4a42 858d 9f79 ac14 765a 5379  .9I.JB...y..vZSy
+00003ed0: 7374 656d 2e53 6563 7572 6974 792e 646c  stem.Security.dl
+00003ee0: 6c00 0001 a18e 3cc0 0080 0000 9a70 982e  l.....<......p..
+00003ef0: d660 fc4b 9e4b 680a 1f99 096b 5379 7374  .`.K.Kh....kSyst
+00003f00: 656d 2e53 6563 7572 6974 792e 5072 696e  em.Security.Prin
+00003f10: 6369 7061 6c2e 646c 6c00 0001 ce84 a6f5  cipal.dll.......
+00003f20: 0080 0000 0b19 49df 1dd2 ca46 a390 779c  ......I....F..w.
+00003f30: 21f5 c8b9 5379 7374 656d 2e53 6563 7572  !...System.Secur
+00003f40: 6974 792e 5072 696e 6369 7061 6c2e 5769  ity.Principal.Wi
+00003f50: 6e64 6f77 732e 646c 6c00 0001 8fa7 319a  ndows.dll.....1.
+00003f60: 00a0 0000 3616 512f ef9d 3b4d 988f 54cc  ....6.Q/..;M..T.
+00003f70: 9e5f f773 5379 7374 656d 2e53 6563 7572  ._.sSystem.Secur
+00003f80: 6974 792e 5365 6375 7265 5374 7269 6e67  ity.SecureString
+00003f90: 2e64 6c6c 0000 018c 3d6d 9100 8000 00f5  .dll....=m......
+00003fa0: acbb 5b1e 9fe9 4192 1956 8761 5f22 7353  ..[...A..V.a_"sS
+00003fb0: 7973 7465 6d2e 5365 7276 6963 654d 6f64  ystem.ServiceMod
+00003fc0: 656c 2e57 6562 2e64 6c6c 0000 0181 bc59  el.Web.dll.....Y
+00003fd0: 8100 8000 006c 718c 60be 7f6a 4f9c 2955  .....lq.`..jO.)U
+00003fe0: 3771 adfc 8253 7973 7465 6d2e 5365 7276  7q...System.Serv
+00003ff0: 6963 6550 726f 6365 7373 2e64 6c6c 0000  iceProcess.dll..
+00004000: 01e9 2f6f f200 8000 00d4 b2f3 44da ec85  ../o........D...
+00004010: 409e a8c7 816f 1db3 4153 7973 7465 6d2e  @....o..ASystem.
+00004020: 5465 7874 2e45 6e63 6f64 696e 672e 436f  Text.Encoding.Co
+00004030: 6465 5061 6765 732e 646c 6c00 0001 feb9  dePages.dll.....
+00004040: 9d8e 0080 0000 037a 5569 ae0e e443 8765  .......zUi...C.e
+00004050: 8705 843a 7edf 5379 7374 656d 2e54 6578  ...:~.System.Tex
+00004060: 742e 456e 636f 6469 6e67 2e64 6c6c 0000  t.Encoding.dll..
+00004070: 0158 6be3 9500 8000 0022 a70d 7812 0793  .Xk......"..x...
+00004080: 4796 b2e4 c83c ad55 9b53 7973 7465 6d2e  G....<.U.System.
+00004090: 5465 7874 2e45 6e63 6f64 696e 672e 4578  Text.Encoding.Ex
+000040a0: 7465 6e73 696f 6e73 2e64 6c6c 0000 01c1  tensions.dll....
+000040b0: 13c6 f600 a000 0003 7df2 d761 28b8 4ea1  ........}..a(.N.
+000040c0: cf20 2c9c 5962 6153 7973 7465 6d2e 5465  . ,.YbaSystem.Te
+000040d0: 7874 2e45 6e63 6f64 696e 6773 2e57 6562  xt.Encodings.Web
+000040e0: 2e64 6c6c 0000 0111 9cf3 a600 a000 001a  .dll............
+000040f0: c151 246d 819f 4cb5 514f 56ff 0acb 3453  .Q$m..L.QOV...4S
+00004100: 7973 7465 6d2e 5465 7874 2e4a 736f 6e2e  ystem.Text.Json.
+00004110: 646c 6c00 0001 4cd4 79b6 0020 0100 53c3  dll...L.y.. ..S.
+00004120: 6f06 8841 234a 8654 6e3d b7f8 e206 5379  o..A#J.Tn=....Sy
+00004130: 7374 656d 2e54 6578 742e 5265 6775 6c61  stem.Text.Regula
+00004140: 7245 7870 7265 7373 696f 6e73 2e64 6c6c  rExpressions.dll
+00004150: 0000 01e2 f476 ce00 c000 0016 55f0 0e63  .....v......U..c
+00004160: b68c 4aba 1dc1 4637 1ecc 9b53 7973 7465  ..J...F7...Syste
+00004170: 6d2e 5468 7265 6164 696e 672e 4368 616e  m.Threading.Chan
+00004180: 6e65 6c73 2e64 6c6c 0000 017b e800 d100  nels.dll...{....
+00004190: 8000 00f4 d815 180c 8909 4f8b 8acc 09b4  ..........O.....
+000041a0: be7c e953 7973 7465 6d2e 5468 7265 6164  .|.System.Thread
+000041b0: 696e 672e 646c 6c00 0001 7eda efd8 00c0  ing.dll...~.....
+000041c0: 0000 ba90 d4c9 03af 8c4e a674 8fa0 9b0e  .........N.t....
+000041d0: 8992 5379 7374 656d 2e54 6872 6561 6469  ..System.Threadi
+000041e0: 6e67 2e4f 7665 726c 6170 7065 642e 646c  ng.Overlapped.dl
+000041f0: 6c00 0001 9ebc 1e9f 0080 0000 efe3 07b6  l...............
+00004200: 0430 3a40 a003 ca72 22b3 526a 5379 7374  .0:@...r".RjSyst
+00004210: 656d 2e54 6872 6561 6469 6e67 2e54 6173  em.Threading.Tas
+00004220: 6b73 2e44 6174 6166 6c6f 772e 646c 6c00  ks.Dataflow.dll.
+00004230: 0001 ff2c cea4 00c0 0000 f7ba 8f1e 2c70  ...,..........,p
+00004240: b140 8eed 9f18 4db3 40a5 5379 7374 656d  .@....M.@.System
+00004250: 2e54 6872 6561 6469 6e67 2e54 6173 6b73  .Threading.Tasks
+00004260: 2e64 6c6c 0000 0140 df01 a400 8000 00fa  .dll...@........
+00004270: 28ef 588c 8118 47b2 2337 a936 9c91 2753  (.X...G.#7.6..'S
+00004280: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
+00004290: 5461 736b 732e 4578 7465 6e73 696f 6e73  Tasks.Extensions
+000042a0: 2e64 6c6c 0000 0191 5532 9900 8000 0041  .dll....U2.....A
+000042b0: 1f28 12e2 cd8a 4fb0 93c1 d645 df73 b753  .(....O....E.s.S
+000042c0: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
+000042d0: 5461 736b 732e 5061 7261 6c6c 656c 2e64  Tasks.Parallel.d
+000042e0: 6c6c 0000 0131 36c3 8700 8000 004d e835  ll...16......M.5
+000042f0: 6a82 6bb9 45bd 968b fe87 76b8 f253 7973  j.k.E.....v..Sys
+00004300: 7465 6d2e 5468 7265 6164 696e 672e 5468  tem.Threading.Th
+00004310: 7265 6164 2e64 6c6c 0000 010b 44cc 8700  read.dll....D...
+00004320: a000 00a4 3128 3113 e9e6 46ac a103 6512  ....1(1...F...e.
+00004330: 137d 7153 7973 7465 6d2e 5468 7265 6164  .}qSystem.Thread
+00004340: 696e 672e 5468 7265 6164 506f 6f6c 2e64  ing.ThreadPool.d
+00004350: 6c6c 0000 019e c281 8a00 8000 0053 7182  ll...........Sq.
+00004360: b26d 3157 4fa0 116d 753c fd45 5b53 7973  .m1WO..mu<.E[Sys
+00004370: 7465 6d2e 5468 7265 6164 696e 672e 5469  tem.Threading.Ti
+00004380: 6d65 722e 646c 6c00 0001 c998 5cf7 0080  mer.dll.....\...
+00004390: 0000 464e 2ff3 c91d 8543 8890 fdd8 1882  ..FN/....C......
+000043a0: 173e 5379 7374 656d 2e54 7261 6e73 6163  .>System.Transac
+000043b0: 7469 6f6e 732e 646c 6c00 0001 bea6 e5ab  tions.dll.......
+000043c0: 0080 0000 1182 f39b 052c ae47 b79c d357  .........,.G...W
+000043d0: 6de6 7782 5379 7374 656d 2e54 7261 6e73  m.w.System.Trans
+000043e0: 6163 7469 6f6e 732e 4c6f 6361 6c2e 646c  actions.Local.dl
+000043f0: 6c00 0001 cdb6 888a 00a0 0000 5bdf 7329  l...........[.s)
+00004400: 3e0a a24c a45d edfd d4d8 a082 5379 7374  >..L.]......Syst
+00004410: 656d 2e56 616c 7565 5475 706c 652e 646c  em.ValueTuple.dl
+00004420: 6c00 0001 9417 34e1 0080 0000 94bc d2cd  l.....4.........
+00004430: 5615 a346 925a 4d80 38bc e760 5379 7374  V..F.ZM.8..`Syst
+00004440: 656d 2e57 6562 2e64 6c6c 0000 018a c4d9  em.Web.dll......
+00004450: dd00 8000 00e8 2ee7 53a8 6764 4a8f 6182  ........S.gdJ.a.
+00004460: a82e 4370 df53 7973 7465 6d2e 5765 622e  ..Cp.System.Web.
+00004470: 4874 7470 5574 696c 6974 792e 646c 6c00  HttpUtility.dll.
+00004480: 0001 8f3c c496 0080 0000 2760 77c5 5658  ...<......'`w.VX
+00004490: 9e4a be87 c59b 6653 02d3 5379 7374 656d  .J....fS..System
+000044a0: 2e57 696e 646f 7773 2e64 6c6c 0000 0108  .Windows.dll....
+000044b0: f7bc 8c00 8000 00c0 dc39 85a7 7b45 4ca6  .........9..{EL.
+000044c0: fb4a 37b4 8d9a c553 7973 7465 6d2e 586d  .J7....System.Xm
+000044d0: 6c2e 646c 6c00 0001 408e e8a8 00a0 0000  l.dll...@.......
+000044e0: 9ce2 023c db5e 8b42 8f3c 057e 6888 6a54  ...<.^.B.<.~h.jT
+000044f0: 5379 7374 656d 2e58 6d6c 2e4c 696e 712e  System.Xml.Linq.
+00004500: 646c 6c00 0001 cdb3 e28c 0080 0000 20f6  dll........... .
+00004510: 7c16 85bf cb4d 9464 97c0 60a2 2372 5379  |....M.d..`.#rSy
+00004520: 7374 656d 2e58 6d6c 2e52 6561 6465 7257  stem.Xml.ReaderW
+00004530: 7269 7465 722e 646c 6c00 0001 583d bdec  riter.dll...X=..
+00004540: 0000 0200 ef11 ece4 c0a5 d847 bd14 d15f  ...........G..._
+00004550: c89e cacd 5379 7374 656d 2e58 6d6c 2e53  ....System.Xml.S
+00004560: 6572 6961 6c69 7a61 7469 6f6e 2e64 6c6c  erialization.dll
+00004570: 0000 0101 8a97 9200 8000 001a ace4 b35e  ...............^
+00004580: 2752 48b9 95ee 2d62 2557 3a53 7973 7465  'RH...-b%W:Syste
+00004590: 6d2e 586d 6c2e 5844 6f63 756d 656e 742e  m.Xml.XDocument.
+000045a0: 646c 6c00 0001 1a39 06f7 00c0 0000 7030  dll....9......p0
+000045b0: b0a8 e4ca 8649 9f8f f2ae e4dd 05bd 5379  .....I........Sy
+000045c0: 7374 656d 2e58 6d6c 2e58 6d6c 446f 6375  stem.Xml.XmlDocu
+000045d0: 6d65 6e74 2e64 6c6c 0000 011b 6fa6 c900  ment.dll....o...
+000045e0: 8000 0056 f158 4291 b078 4bbe 1fe5 33ef  ...V.XB..xK...3.
+000045f0: 377e 6053 7973 7465 6d2e 586d 6c2e 586d  7~`System.Xml.Xm
+00004600: 6c53 6572 6961 6c69 7a65 722e 646c 6c00  lSerializer.dll.
+00004610: 0001 a302 b0ac 0000 0100 342b 816c 87dc  ..........4+.l..
+00004620: c343 ad58 88da 4e88 0d26 5379 7374 656d  .C.X..N..&System
+00004630: 2e58 6d6c 2e58 5061 7468 2e64 6c6c 0000  .Xml.XPath.dll..
+00004640: 01bb c47b bf00 8000 00ea 6700 93ec 22ea  ...{......g...".
+00004650: 4eaf 11e1 0419 57cf a253 7973 7465 6d2e  N.....W..System.
+00004660: 586d 6c2e 5850 6174 682e 5844 6f63 756d  Xml.XPath.XDocum
+00004670: 656e 742e 646c 6c00 0001 53b3 9cc7 0080  ent.dll...S.....
+00004680: 0000 ba04 e243 f288 1d4a a7db 0681 3656  .....C...J....6V
+00004690: 9948 556e 6465 7274 616c 654d 6f64 4c69  .HUndertaleModLi
+000046a0: 622e 646c 6c00 0001 62f2 9ae3 0020 0300  b.dll...b.... ..
+000046b0: c184 c359 6d76 1f49 976e bf23 e575 fde7  ...Ymv.I.n.#.u..
+000046c0: 5769 6e64 6f77 7342 6173 652e 646c 6c00  WindowsBase.dll.
+000046d0: 0001 15f4 31ad 0080 0000 e603 b5c3 1541  ....1..........A
+000046e0: 6344 856e 88a6 29fa 8eae 0b00 0000 2405  cD.n..).......$.
+000046f0: 0506 0001 0400 0653 7973 7465 6d1a 5379  .......System.Sy
+00004700: 7374 656d 2e43 6f6c 6c65 6374 696f 6e73  stem.Collections
+00004710: 2e47 656e 6572 6963 0953 7973 7465 6d2e  .Generic.System.
+00004720: 494f 0b53 7973 7465 6d2e 4c69 6e71 0f53  IO.System.Linq.S
+00004730: 7973 7465 6d2e 4e65 742e 4874 7470 1053  ystem.Net.Http.S
+00004740: 7973 7465 6d2e 5468 7265 6164 696e 6716  ystem.Threading.
+00004750: 5379 7374 656d 2e54 6872 6561 6469 6e67  System.Threading
+00004760: 2e54 6173 6b73 1501 adde 01ad e501 ae00  .Tasks..........
+00004770: 01ae 0a01 ae16 01ae 2601 ae37 0b00 0000  ........&..7....
+00004780: 0d0a 0b07 0001 0475 0b00 0000 140f 0b08  .......u........
+00004790: 0001 0475 1000 0000 1810 090a 002c 0200  ...u.........,..
+000047a0: 0a00 0102 790f 556e 6465 7274 616c 654d  ....y.UndertaleM
+000047b0: 6f64 4c69 621a 556e 6465 7274 616c 654d  odLib.UndertaleM
+000047c0: 6f64 4c69 622e 4465 636f 6d70 696c 6572  odLib.Decompiler
+000047d0: 1655 6e64 6572 7461 6c65 4d6f 644c 6962  .UndertaleModLib
+000047e0: 2e4d 6f64 656c 7311 5379 7374 656d 2e52  .Models.System.R
+000047f0: 6566 6c65 6374 696f 6e1c 5379 7374 656d  eflection.System
+00004800: 2e52 756e 7469 6d65 2e53 6572 6961 6c69  .Runtime.Seriali
+00004810: 7a61 7469 6f6e 2401 adde 01ad e501 ae00  zation$.........
+00004820: 01ae 0a01 ae16 01ae 2601 ae37 01ae 8d01  ........&..7....
+00004830: ae9d 01ae b801 aecf 01ae e106 0000 0034  ...............4
+00004840: 1709 2901 0000 3c1c 090d 0026 0200 0900  ..)...<....&....
+00004850: 1104 0803 0007 0208 0100 6a04 7955 003c  ..........j.yU.<
+00004860: 0479 0900 2202 000c 0001 0279 1502 0000  .y.."......y....
+00004870: 3c2a 090d 002b 0200 0d00 2202 000c 0001  <*...+....".....
+00004880: 0279 1502 0000 3c31 090d 002a 0200 0d00  .y....<1...*....
+00004890: 2202 000c 0001 0279 0b00 0000 2438 090c  "......y....$8..
+000048a0: 0001 0279 0b03 0000 253d 0934 0b04 0200  ...y....%=.4....
+000048b0: 0b03 0000 244e 0934 0904 0200 0904 0000  ....$N.4........
+000048c0: 000d 0518 5e09 4705 0000 5f68 0927 001b  ....^.G..._h.'..
+000048d0: 0200 1000 3704 0006 001d 0200 0c00 4c02  ....7.........L.
+000048e0: 0006 0038 0200 1b00 1402 0007 001d 0200  ...8............
+000048f0: 0c00 1a02 0007 001e 0200 1000 2204 0007  ............"...
+00004900: 005f 0200 2400 1b02 0010 0001 0279 8086  ._..$........y..
+00004910: 0600 0019 0909 0800 0702 0801 003c 0679  .............<.y
+00004920: 0700 6f06 0024 0059 0208 1b00 6904 7924  ..o..$.Y....i.y$
+00004930: 0053 0208 1b00 1b06 2c0e 0000 0200 0d00  .S......,.......
+00004940: 5f03 002b 0277 1500 0004 0002 7f26 0600  _..+.w.......&..
+00004950: 0908 3207 0000 0200 2300 331c 003b 0477  ..2.....#.3..;.w
+00004960: 1900 5902 0824 0002 7b4a 0b00 000e 001c  ..Y..$..{J......
+00004970: 0e5b 0e00 0002 000d 005f 0500 2b04 771c  .[......._..+.w.
+00004980: 001b 0200 0900 1b02 0809 0000 0400 0279  ...............y
+00004990: 1e06 0001 0c4b 1f53 7973 7465 6d2e 4469  .....K.System.Di
+000049a0: 6167 6e6f 7374 6963 732e 436f 6465 416e  agnostics.CodeAn
+000049b0: 616c 7973 6973 1801 adde 01ad e501 ae00  alysis..........
+000049c0: 01ae 0a01 ae16 01ae 2601 ae37 01b0 7e15  ........&..7..~.
+000049d0: 0700 0046 1b09 1000 1502 0003 000a 002c  ...F...........,
+000049e0: 0600 3d04 551c 5379 7374 656d 2e43 6f6d  ..=.U.System.Com
+000049f0: 706f 6e65 6e74 4d6f 6465 6c2e 4465 7369  ponentModel.Desi
+00004a00: 676e 1453 7973 7465 6d2e 476c 6f62 616c  gn.System.Global
+00004a10: 697a 6174 696f 6e10 5379 7374 656d 2e54  ization.System.T
+00004a20: 6578 742e 4a73 6f6e 154e 6174 7572 616c  ext.Json.Natural
+00004a30: 536f 7274 2e45 7874 656e 7369 6f6e 1453  Sort.Extension.S
+00004a40: 6978 4c61 626f 7273 2e49 6d61 6765 5368  ixLabors.ImageSh
+00004a50: 6172 7020 5369 784c 6162 6f72 732e 496d  arp SixLabors.Im
+00004a60: 6167 6553 6861 7270 2e46 6f72 6d61 7473  ageSharp.Formats
+00004a70: 2e50 6e67 2153 6978 4c61 626f 7273 2e49  .Png!SixLabors.I
+00004a80: 6d61 6765 5368 6172 702e 5069 7865 6c46  mageSharp.PixelF
+00004a90: 6f72 6d61 7473 1f53 6978 4c61 626f 7273  ormats.SixLabors
+00004aa0: 2e49 6d61 6765 5368 6172 702e 5072 6f63  .ImageSharp.Proc
+00004ab0: 6573 7369 6e67 1059 414d 535f 4c49 422e  essing.YAMS_LIB.
+00004ac0: 7061 7463 6865 7314 5941 4d53 5f4c 4942  patches.YAMS_LIB
+00004ad0: 2e70 6174 6368 6573 2e71 6f6c 4101 adde  .patches.qolA...
+00004ae0: 01ad e501 ae00 01ae 0a01 ae16 01ae 2601  ..............&.
+00004af0: ae37 01b0 cd01 b0ea 01ae cf01 b0ff 01b1  .7..............
+00004b00: 1001 b126 01b1 3b01 b15c 01b1 7e01 ae8d  ...&..;..\..~...
+00004b10: 01ae 9d01 aeb8 01b1 9e01 b1af 031c 9901  ................
+00004b20: 0800 0000 0600 3a2e 090a 005c 0400 0d00  ......:....\....
+00004b30: 1d0e 000a 0031 040e 0d00 1e04 7b0f 0001  .....1......{...
+00004b40: 0279 0200 000b 0000 0100 2504 000a 003d  .y........%....=
+00004b50: 0200 1000 5706 001a 0040 0200 0c00 4e00  ....W....@....N.
+00004b60: 8082 0b00 3708 bf7f 0b00 1104 0007 000d  ....7...........
+00004b70: 0026 0700 1600 1e07 0045 023d 1500 4902  .&.......E.=..I.
+00004b80: 000b 0049 0200 2000 2b02 0015 0063 5c00  ...I.. .+....c\.
+00004b90: 1f00 2402 0e07 002c 047b 1200 6002 001d  ..$....,.{..`...
+00004ba0: 0001 0279 0200 000b 0000 0100 0007 0060  ...y...........`
+00004bb0: 0808 2600 4e02 0027 0080 8402 0019 0053  ..&.N..'.......S
+00004bc0: 0200 2100 4a02 0022 0064 0200 1400 2402  ..!.J..".d....$.
+00004bd0: 0e07 0029 047b 0e00 3902 001d 0001 0279  ...).{..9......y
+00004be0: 0200 000b 0000 0100 6204 0026 0050 0200  ........b..&.P..
+00004bf0: 2700 8089 0200 1900 5502 0021 004c 0200  '.......U..!.L..
+00004c00: 2200 6802 0014 0024 020e 0700 2a04 7b0e  ".h....$....*.{.
+00004c10: 003a 0200 1d00 0102 7902 0000 0b00 0001  .:......y.......
+00004c20: 0072 2279 3900 7802 0039 0078 0200 3900  .r"y9.x..9.x..9.
+00004c30: 7e02 0039 006b 0200 3900 80a6 0200 5400  ~..9.k..9.....T.
+00004c40: 80a6 0200 5400 80a6 0200 5400 80a6 0200  ....T.....T.....
+00004c50: 5400 80a6 0200 5400 80a6 0200 5400 80a6  T.....T.....T...
+00004c60: 0200 5401 8136 0400 5401 8122 0400 5401  ..T..6..T.."..T.
+00004c70: 8112 0400 5401 810e 0400 5400 80a5 0800  ....T.....T.....
+00004c80: 4900 80a7 0200 4900 80a1 0200 4900 80a3  I.....I.....I...
+00004c90: 0200 4900 80a5 0200 4900 809f 0200 4900  ..I.....I.....I.
+00004ca0: 80a8 0200 4900 80aa 0200 4900 80a4 0200  ....I.....I.....
+00004cb0: 4900 7506 0044 0078 0200 4400 7602 0044  I.u..D.x..D.v..D
+00004cc0: 0076 0200 4400 7b02 0044 0080 a206 0049  .v..D.{..D.....I
+00004cd0: 0080 a002 0049 0080 a202 0049 0080 a202  .....I.....I....
+00004ce0: 0049 0080 9f02 0049 0080 9c02 0049 0080  .I.....I.....I..
+00004cf0: 9e02 0049 0080 9d02 0049 0080 a402 0049  ...I.....I.....I
+00004d00: 0080 9e02 0049 0080 a002 0049 0080 a002  .....I.....I....
+00004d10: 0049 0080 9e02 0049 0080 9e02 0049 0080  .I.....I.....I..
+00004d20: 9f02 0049 0080 9d02 0049 0080 a402 0049  ...I.....I.....I
+00004d30: 0080 9d02 0049 0080 9d02 0049 0080 9d02  .....I.....I....
+00004d40: 0049 0080 a602 0049 0080 a602 0049 0080  .I.....I.....I..
+00004d50: a502 0049 0080 ab02 0049 0080 a802 0049  ...I.....I.....I
+00004d60: 0080 aa02 0049 0080 9e02 0049 0032 0600  .....I.....I.2..
+00004d70: 1f00 8099 0200 4900 8099 0200 4900 8099  ......I.....I...
+00004d80: 0200 4900 8099 0200 4900 8099 0200 4900  ..I.....I.....I.
+00004d90: 8099 0200 4900 8099 0200 4900 8099 0200  ....I.....I.....
+00004da0: 4900 8099 0200 4905 0616 007d 0406 0e00  I.....I....}....
+00004db0: 6f04 060c 006f 0406 0c00 6f04 060c 006f  o....o....o....o
+00004dc0: 0406 0c00 6f04 060c 006f 0406 0a00 6f04  ....o....o....o.
+00004dd0: 060c 006f 0506 0c00 6f04 060e 006f 0406  ...o....o....o..
+00004de0: 0c00 6f04 060c 006f 0506 0c00 7d05 060e  ..o....o....}...
+00004df0: 007d 0039 0e00 1f00 6702 0025 0039 0400  .}.9....g..%.9..
+00004e00: 1f00 6702 0025 0080 9504 0049 0a06 0400  ..g..%.....I....
+00004e10: 8111 3706 1800 8a66 0406 7200 6f04 060c  ..7....f..r.o...
+00004e20: 006f 0406 0c00 6f04 060c 006f 002f 0c00  .o....o....o./..
+00004e30: 0b00 2f02 000b 0506 0600 7f00 2312 000b  ../.........#...
+00004e40: 002d 0600 0b00 3202 000b 0032 0200 0b00  .-....2....2....
+00004e50: 3602 000b 0033 0200 0b00 3402 000b 0033  6....3....4....3
+00004e60: 0200 0b00 3502 000b 0030 0200 0b00 3202  ....5....0....2.
+00004e70: 000b 0034 0200 0b00 3102 000b 0032 0200  ...4....1....2..
+00004e80: 0b00 2a02 000b 002e 0200 0b00 3002 000b  ..*.........0...
+00004e90: 0031 0200 0b00 3002 000b 0030 0200 0b00  .1....0....0....
+00004ea0: 2c02 000b 0030 0200 0b00 2e02 000b 002f  ,....0........./
+00004eb0: 0200 0b00 2f02 000b 002e 0200 0b00 3602  ..../.........6.
+00004ec0: 000b 002e 0200 0b00 3102 000b 0031 0200  ........1....1..
+00004ed0: 0b00 2e02 000b 002d 0200 0b00 2f02 000b  .......-..../...
+00004ee0: 002e 0200 0b00 2b06 000b 0031 0200 0b00  ......+....1....
+00004ef0: 2e02 000b 0030 0200 0b00 2c02 000b 0031  .....0....,....1
+00004f00: 0200 0b00 2e02 000b 002e 0200 0b00 2e02  ................
+00004f10: 000b 0033 0200 0b00 2f02 000b 002f 0200  ...3..../..../..
+00004f20: 0b00 2f02 000b 002d 0200 0b00 3002 000b  ../....-....0...
+00004f30: 002f 0200 0b00 2f02 000b 002f 0200 0b00  ./..../..../....
+00004f40: 3702 000b 0035 0200 0b00 3102 000b 0033  7....5....1....3
+00004f50: 0200 0b00 3202 000b 0032 0200 0b00 2f02  ....2....2..../.
+00004f60: 000b 002c 0200 0b00 2f08 000b 0032 0200  ...,..../....2..
+00004f70: 0b00 2a02 000b 002a 0200 0b00 2f02 000b  ..*....*..../...
+00004f80: 0030 0200 0b00 3002 000b 0030 0200 0b00  .0....0....0....
+00004f90: 3402 000b 002e 0200 0b00 3602 000b 0032  4.........6....2
+00004fa0: 0200 0b00 3102 000b 002f 0200 0b00 2e02  ....1..../......
+00004fb0: 000b 0031 0200 0b00 3102 000b 002e 0200  ...1....1.......
+00004fc0: 0b00 3202 000b 002e 0200 0b00 2d02 000b  ..2.........-...
+00004fd0: 0029 0800 0b00 2f1e 000d 002b 0476 2100  .)..../....+.v!.
+00004fe0: 0002 002a 0025 0900 5f04 7717 0002 7d60  ...*.%.._.w...}`
+00004ff0: 0b00 000b 0000 0100 300e 110d 0060 0476  ........0....`.v
+00005000: 4000 0002 002a 0025 0900 6004 7717 0002  @....*.%..`.w...
+00005010: 7d60 0b00 000b 0000 0100 2d0e 110d 0080  }`........-.....
+00005020: 8104 4e42 0000 0200 1600 4d09 0053 0477  ..NB......M..S.w
+00005030: 1700 027d 380b 0000 0e00 230e 390d 0034  ...}8.....#.9..4
+00005040: 0444 2300 0002 0011 0057 0700 3c04 7712  .D#......W..<.w.
+00005050: 0055 0200 2c00 0006 0002 7b2e 0800 6810  .U..,.....{...h.
+00005060: 4316 0080 8204 001f 0067 0200 2505 0408  C........g..%...
+00005070: 0044 0080 810c 0021 0055 0200 0b00 2502  .D.....!.U....%.
+00005080: 0010 0037 0200 0c00 5c02 0007 0031 0200  ...7....\....1..
+00005090: 0800 4f02 0007 0024 0200 0800 3402 000e  ..O....$....4...
+000050a0: 0030 0200 0700 7d02 0022 0074 0200 0c00  .0....}..".t....
+000050b0: 2302 0011 0035 0200 0c00 3c02 0007 002f  #....5....<..../
+000050c0: 0200 0900 3502 0007 0024 0200 0800 3402  ....5....$....4.
+000050d0: 000e 002e 0200 0700 2702 0010 0058 0400  ........'....X..
+000050e0: 1700 3406 001b 0035 0200 1c00 5a06 0015  ..4....5....Z...
+000050f0: 0056 0200 1001 80d2 0200 2501 81ca 0800  .V........%.....
+00005100: 2500 8087 0800 1f00 5906 001f 0053 0600  %.......Y....S..
+00005110: 1500 5e02 000a 0058 0200 1f00 5506 001f  ..^....X....U...
+00005120: 0080 8f06 0025 0080 8802 0025 0280 a606  .....%.....%....
+00005130: 0025 0280 a60a 0025 0077 0a00 2500 8087  .%.....%.w..%...
+00005140: 0400 2500 809d 0600 2500 5c06 001f 005a  ..%.....%.\....Z
+00005150: 0200 1f00 4706 0017 0080 8902 0012 0080  ....G...........
+00005160: 8102 0012 0080 8302 0012 007e 0200 1200  ...........~....
+00005170: 6002 322a 0000 0200 0c00 6107 0047 0477  `.2*......a..G.w
+00005180: 2200 4702 0022 0000 0600 027b 2408 0180  ".G..".....{$...
+00005190: 9a0e 5525 0067 0600 2500 5806 001f 0080  ..U%.g..%.X.....
+000051a0: 8402 0025 0073 0600 1f00 7302 001f 0073  ...%.s....s....s
+000051b0: 0200 1f00 6e02 001f 0073 0200 1f00 4e06  ....n....s....N.
+000051c0: 381b 0000 0200 0f00 5b07 003c 0477 1c00  8.......[..<.w..
+000051d0: 0006 0002 7d2a 0800 80a6 0c4f 1f0e 1202  ....}*.....O....
+000051e0: 0025 0181 041e 0025 1112 0400 2500 2d28  .%.....%....%.-(
+000051f0: 0012 0067 005c 2501 80da 0625 1f00 6804  ...g.\%....%..h.
+00005200: 001f 0076 0600 2500 7d02 0025 0074 0200  ...v..%.}..%.t..
+00005210: 2500 809c 0600 1f00 8097 0200 1f00 8097  %...............
+00005220: 0200 1f00 5e06 0025 0060 0200 2505 5d06  ....^..%.`..%.].
+00005230: 3866 0000 0200 0f00 5b07 0033 0e77 1c00  8f......[..3.w..
+00005240: 0006 0002 732a 0800 808f 144f 1f01 811a  ....s*.....O....
+00005250: 0600 2503 80e2 0800 2500 710e 0025 0037  ..%.....%.q..%.7
+00005260: 0200 0700 5602 001c 026c 0200 0c00 2406  ....V....l....$.
+00005270: 0011 0045 0200 2000 5602 0007 002a 0200  ...E.. .V....*..
+00005280: 0900 4902 0007 0020 0200 0c00 2802 000e  ..I.... ....(...
+00005290: 0024 0200 0707 8122 0c00 0701 80f6 1238  .$.....".......8
+000052a0: 2b00 0002 000f 005b 0700 5306 771f 0000  +......[..S.w...
+000052b0: 0600 027b 2a08 006a 0e4f 2500 2906 0007  ...{*..j.O%.)...
+000052c0: 005d 0230 1700 0002 000b 0063 0700 2e04  .].0.......c....
+000052d0: 770f 0031 005e 2f00 0006 0002 7d45 0804  w..1.^/.....}E..
+000052e0: 8090 0a57 3104 8086 0a00 3100 250c 0007  ...W1.....1.%...
+000052f0: 001d 0230 1b00 0002 000b 0063 0700 2e04  ...0.......c....
+00005300: 770f 002d 005e 2f00 0006 0002 7d45 0804  w..-.^/.....}E..
+00005310: 8088 0a57 3104 7e0a 0031 0980 8a10 001f  ...W1.~..1......
+00005320: 005d 1600 2500 5d02 0025 0060 0600 2500  .]..%.]..%.`..%.
+00005330: 809d 0600 2500 4e06 001f 0055 0638 1b00  ....%.N....U.8..
+00005340: 0002 000f 005b 0700 7b04 7722 0000 0600  .....[..{.w"....
+00005350: 027d 2a08 0080 8c0c 4f25 0174 0600 2517  .}*.....O%.t..%.
+00005360: 809e 0800 2500 7a34 0022 007c 0200 2200  ....%.z4.".|..".
+00005370: 2102 0011 0022 0200 1109 0602 0078 0906  !....".......x..
+00005380: 1400 7b00 5c18 001f 0080 8008 0022 0024  ..{.\........".$
+00005390: 0200 1100 3a02 0015 0080 8b02 0037 0047  ....:........7.G
+000053a0: 0600 1700 4802 002d 0048 0200 2d00 4802  ....H..-.H..-.H.
+000053b0: 002a 0046 0200 2900 4602 002c 0046 0200  .*.F..).F..,.F..
+000053c0: 2c00 4602 0029 0044 0200 2700 4608 0017  ,.F..).D..'.F...
+000053d0: 000b 020a 0700 0005 0033 047f 0700 3502  .........3....5.
+000053e0: 0028 001a 0200 0900 2b04 0007 004d 0200  .(......+....M..
+000053f0: 4900 4302 001d 0018 0200 1100 2302 000d  I.C.........#...
+00005400: 004f 0200 0700 1702 0009 0043 0200 0700  .O.........C....
+00005410: 1b02 000e 001c 0200 0700 2e04 0007 0055  ...............U
+00005420: 0200 4900 1b02 0011 0026 0200 0d00 2f02  ..I......&..../.
+00005430: 0007 001a 0200 0900 2902 0007 001a 0200  ........).......
+00005440: 0c00 1b02 000e 001f 0200 0700 1b02 0011  ................
+00005450: 0003 4b30 0600 0800 6d0c 0e5a 3e5d 1200  ..K0....m..Z>]..
+00005460: 4e1e 0025 004e 0200 2500 3006 0007 0048  N..%.N..%.0....H
+00005470: 0200 1c5d 4602 000c 001d 80bc 0011 0071  ...]F..........q
+00005480: 0200 3701 817a 0600 1201 817a 0400 1204  ..7..z.....z....
+00005490: 6508 3033 0000 0200 0b00 6307 003b 0c77  e.03......c..;.w
+000054a0: 2200 0006 0002 7522 0804 6514 063b 0000  ".....u"..e..;..
+000054b0: 0200 0b00 6307 0029 0c77 1400 5302 0012  ....c..).w..S...
+000054c0: 031a 0200 1308 120e 0812 0000 0205 0a18  ................
+000054d0: 000c 0000 0600 024b 1a08 0047 4a57 1700  .......K...GJW..
+000054e0: 4202 0012 0047 0200 1200 8092 0200 2500  B....G........%.
+000054f0: 8092 0200 2501 6802 0025 005f 0400 1500  ....%.h..%._....
+00005500: 7102 0011 006f 0200 1100 8088 0200 1101  q....o..........
+00005510: 809e 0200 1100 808c 0400 1000 6d02 0025  ............m..%
+00005520: 0021 0600 1000 4106 0815 005c 0200 1700  .!....A....\....
+00005530: 5c02 0017 005a 0200 1700 5b02 0017 004e  \....Z....[....N
+00005540: 0200 1700 4802 0017 0050 0200 1700 5c02  ....H....P....\.
+00005550: 002f 0055 0200 2f00 5602 0030 0055 0200  ./.U../.V..0.U..
+00005560: 2f00 5502 002f 0056 0200 3000 5602 0030  /.U../.V..0.V..0
+00005570: 0056 0200 3000 5602 002c 0052 0400 2900  .V..0.V..,.R..).
+00005580: 4902 0029 0052 0200 2900 7a04 0022 0065  I..).R..).z..".e
+00005590: 0200 0c00 2102 0011 0070 0200 2a00 6802  ....!....p..*.h.
+000055a0: 000f 003e 0600 1500 6002 002f 0058 0200  ...>....`../.X..
+000055b0: 2e00 5a02 0030 0059 0200 2f00 5a02 0030  ..Z..0.Y../.Z..0
+000055c0: 0059 0200 2f00 5a02 0030 005a 0200 3000  .Y../.Z..0.Z..0.
+000055d0: 4f06 0029 0046 0200 2900 4f02 0029 0045  O..).F..).O..).E
+000055e0: 0400 1000 7704 0022 0063 0200 0c00 1e02  ....w..".c......
+000055f0: 0011 006e 0200 2a00 5d06 0030 0040 0800  ...n..*.]..0.@..
+00005600: 1700 5d02 002d 0056 0200 2d00 5702 002e  ..]..-.V..-.W...
+00005610: 0057 0200 2d00 5602 002d 0057 0200 2e00  .W..-.V..-.W....
+00005620: 5702 002e 0058 0200 2e00 5708 0038 0056  W....X....W..8.V
+00005630: 0200 3800 5e02 0032 0050 0400 2700 4702  ..8.^..2.P..'.G.
+00005640: 0027 0050 0200 2700 4804 0011 0079 0400  .'.P..'.H....y..
+00005650: 2200 6502 000c 0020 0200 1100 7102 0028  ".e.... ....q..(
+00005660: 0044 0600 1700 6202 0030 005a 0200 2f00  .D....b..0.Z../.
+00005670: 5c02 0031 005b 0200 3000 5c02 0031 005b  \..1.[..0.\..1.[
+00005680: 0200 3000 5c02 0031 005c 0200 3100 5f08  ..0.\..1.\..1._.
+00005690: 0038 005f 0200 3800 5f02 0038 005f 0200  .8._..8._..8._..
+000056a0: 3800 6f02 0043 0055 0400 2a00 4c02 002a  8.o..C.U..*.L..*
+000056b0: 0055 0200 2a00 7d04 0022 0067 0200 0c00  .U..*.}..".g....
+000056c0: 2402 0011 0079 0200 2b00 4904 0011 0080  $....y..+.I.....
+000056d0: 8808 0025 0080 8802 0025 0180 9404 0025  ...%.....%.....%
+000056e0: 0080 8806 0025 0080 8802 0025 0080 8802  .....%.....%....
+000056f0: 0025 0080 8802 0025 0080 8802 0025 0080  .%.....%.....%..
+00005700: 8604 0025 0080 8602 0025 0080 8602 0025  ...%.....%.....%
+00005710: 0080 8802 0025 0181 9208 7925 0181 9204  .....%....y%....
+00005720: 0025 0181 9204 0025 0181 9204 0025 0281  .%.....%.....%..
+00005730: 7008 001f 003b 0a00 1500 4302 0007 0010  p....;....C.....
+00005740: 0200 0900 1002 0009 0014 0200 0c00 1402  ................
+00005750: 000c 0033 0200 2400 4102 001c 0031 0200  ...3..$.A....1..
+00005760: 0700 5602 001c 006e 0200 0c00 1e02 0011  ..V....n........
+00005770: 0025 0200 0900 2302 000d 0b06 0200 8088  .%....#.........
+00005780: 0b06 1800 808a 007b 1c00 2502 8098 0600  .......{..%.....
+00005790: 4b00 4a0a 0015 0063 0200 1100 6f06 0010  K.J....c....o...
+000057a0: 005b 0600 2500 5b02 0025 0180 9406 0025  .[..%.[..%.....%
+000057b0: 0181 2a0e 000c 006c 0a00 1200 8080 0200  ..*....l........
+000057c0: 1200 5402 0012 0069 0200 1200 4e02 0012  ..T....i....N...
+000057d0: 0060 0200 1200 6702 0012 0051 0600 1502  .`....g....Q....
+000057e0: 8156 0200 1000 4c06 0015 0068 0200 100b  .V....L....h....
+000057f0: 1208 0012 084e 1800 1208 4e12 0012 0a4e  .....N....N....N
+00005800: 1200 120b 121a 0012 084e 1800 1208 4e12  .........N....N.
+00005810: 0012 0a4e 1200 120a 121a 0012 084e 1600  ...N.........N..
+00005820: 1208 4e12 0012 0a4e 1200 1200 521a 0015  ..N....N....R...
+00005830: 0080 9502 0011 0180 b602 0011 0181 2408  ..............$.
+00005840: 0011 095a 0800 1100 5914 0010 0281 280e  ...Z....Y.....(.
+00005850: 000c 003b 0a00 0c00 6a06 000c 007f 0600  ...;....j.......
+00005860: 2400 8083 0200 2a01 812a 0600 0c01 80cc  $.....*..*......
+00005870: 0800 0c00 6404 0017 0862 0200 1200 6712  ....d....b....g.
+00005880: 0012 006e 0400 1708 6c02 0012 0071 1200  ...n....l....q..
+00005890: 1200 6404 0017 085e 0200 1200 6712 0012  ..d....^....g...
+000058a0: 0065 0400 1708 5e02 0012 0064 1200 1200  .e....^....d....
+000058b0: 4e06 000c 0181 1002 0025 0080 a304 0025  N........%.....%
+000058c0: 0f80 9e02 0025 007d 2400 0c00 80af 0200  .....%.}$.......
+000058d0: 1f00 80be 0200 2500 3702 000d 0061 0408  ......%.7....a..
+000058e0: 1200 8093 0200 2c00 8094 0200 2c02 814a  ......,.....,..J
+000058f0: 0879 0c1e 5a0a 0012 0181 003e 0012 007a  .y..Z......>...z
+00005900: 0800 2500 5a06 0017 004e 0200 1200 5902  ..%.Z....N....Y.
+00005910: 0017 0047 0200 1205 6504 304b 0000 0200  ...G....e.0K....
+00005920: 0b00 6307 004f 0e77 2200 0006 0002 7322  ..c..O.w".....s"
+00005930: 0800 4f14 571b 000c 023e 1100 0002 0012  ..O.W....>......
+00005940: 0055 0700 6004 4632 0000 0200 1b00 4307  .U..`.F2......C.
+00005950: 004c 0477 1500 027d 420b 0000 0b00 0001  .L.w...}B.......
+00005960: 0002 7d67 0b00 000b 0000 0100 4b14 4912  ..}g........K.I.
+00005970: 0052 0200 1200 4c06 0012 0053 0200 1201  .R....L....S....
+00005980: 80da 023e 3500 0002 0012 0055 0700 4006  ...>5......U..@.
+00005990: 7710 0002 7b30 0b00 000b 0000 0100 4a0e  w...{0........J.
+000059a0: 4912 0051 0200 1200 7502 0025 005b 0600  I..Q....u..%.[..
+000059b0: 1700 4902 0012 004f 0200 1202 8096 0240  ..I....O.......@
+000059c0: 3500 0002 0013 0053 0700 3c08 7710 0002  5......S..<.w...
+000059d0: 7932 0b00 000b 0000 0100 5a10 4717 0048  y2........Z.G..H
+000059e0: 0200 1200 4e02 0012 0465 0230 3300 0002  ....N....e.03...
+000059f0: 000b 0063 0700 4f0c 7722 0000 0600 0275  ...c..O.w".....u
+00005a00: 2208 004c 1457 1200 5202 0012 0280 9602  "..L.W..R.......
+00005a10: 4035 0000 0200 1300 5307 0045 0877 1000  @5......S..E.w..
+00005a20: 0279 320b 0000 0b00 0001 004f 1047 1200  .y2........O.G..
+00005a30: 5502 0012 0180 d602 4035 0000 0200 1300  U.......@5......
+00005a40: 5307 0048 0677 1000 027b 320b 0000 0b00  S..H.w...{2.....
+00005a50: 0001 004d 1047 1200 5402 0012 0765 0230  ...M.G..T....e.0
+00005a60: 809c 0000 0200 0b00 6307 0055 1277 2200  ........c..U.w".
+00005a70: 0006 0002 6f22 0800 4a1c 5712 0050 0200  ....o"..J.W..P..
+00005a80: 1206 6504 3080 8a00 0002 000b 0063 0700  ..e.0........c..
+00005a90: 5110 7722 0000 0600 0271 2208 0055 1857  Q.w".....q"..U.W
+00005aa0: 1700 4702 0012 004f 0200 1200 4706 0012  ..G....O....G...
+00005ab0: 004f 0200 1200 808c 0230 2b00 0002 000b  .O.......0+.....
+00005ac0: 0063 0700 5604 7722 0000 0600 027d 2208  .c..V.w".....}".
+00005ad0: 0047 0c57 1200 4f02 0012 0047 0600 1200  .G.W..O....G....
+00005ae0: 4f02 0012 0047 0600 1200 4f02 0012 0858  O....G....O....X
+00005af0: 0600 1208 5a12 0012 085a 1200 1212 5a12  ....Z....Z....Z.
+00005b00: 0012 085a 2800 1200 80a8 1600 7e00 6606  ...Z(.......~.f.
+00005b10: 0025 0065 0200 1f00 5f02 001f 0065 0600  .%.e...._....e..
+00005b20: 2500 8083 0400 1f00 3f06 000c 004e 0200  %.......?....N..
+00005b30: 1504 80f6 0200 1010 80a6 0e00 1f00 6e22  ..............n"
+00005b40: 0025 0780 a202 001f 2780 aa10 0025 0780  .%......'....%..
+00005b50: a250 001f 0067 1000 1f08 8092 0200 1f01  .P...g..........
+00005b60: 80a6 1200 2500 3408 0007 0052 0200 1c2d  ....%.4....R...-
+00005b70: 4e02 000c 0021 5c00 1100 7b02 0037 0034  N....!\...{..7.4
+00005b80: 0400 0700 5202 001c 324e 0200 0c00 2166  ....R...2N....!f
+00005b90: 0011 007b 0200 3700 4304 0015 0080 8002  ...{..7.C.......
+00005ba0: 0011 002d 0200 1100 3702 0010 0043 0400  ...-....7....C..
+00005bb0: 1500 2d02 0011 0074 0200 1100 7102 0011  ..-....t....q...
+00005bc0: 0d44 0200 1100 80a1 2000 7d04 6002 0010  .D...... .}.`...
+00005bd0: 0052 1000 1500 3402 0011 007b 0200 1000  .R....4....{....
+00005be0: 6e04 302b 0000 0200 0b00 6307 003e 0477  n.0+......c..>.w
+00005bf0: 2200 0006 0002 7d22 0800 400c 5724 0044  ".....}"..@.W$.D
+00005c00: 0200 2400 8081 0600 4a00 809c 0200 3c00  ..$.....J.....<.
+00005c10: 4206 000c 0064 0200 2508 1202 001f 0022  B....d..%......"
+00005c20: 1600 0300 2002 0003 0020 0200 0300 4802  .... .... ....H.
+00005c30: 000c 0018 0254 0d00 0005 001d 003f 1c00  .....T.......?..
+00005c40: 1d04 7704 000d 0200 0400 0080 b600 5806  ..w...........X.
+00005c50: 103f 0180 e802 0080 8500 0604 0005 0019  .?..............
+00005c60: 0600 0700 7c04 0017 0027 0408 0700 7606  ....|....'....v.
+00005c70: 7917 0021 0080 ee07 0061 04bf 133f 001c  y..!.....a...?..
+00005c80: 0200 0300 0602 0005 0017 0600 0700 8084  ................
+00005c90: 0400 1700 2504 0807 007e 0679 1700 1f00  ....%....~.y....
+00005ca0: 80fe 0700 6304 bf03 3f00 1a02 0003 0006  ....c...?.......
+00005cb0: 0200 0500 1708 0007 0076 0400 1700 2500  .........v....%.
+00005cc0: 80ee 0700 7004 bf13 1700 1f00 80e2 0700  ....p...........
+00005cd0: 5d04 bf1f 3f00 1a02 0003 0006 0200 0500  ]...?...........
+00005ce0: 0004 0023 0e0e 1c00 4702 7312 0006 0200  ...#....G.s.....
+00005cf0: 0500 5c06 003f 0006 0200 0500 6404 003f  ..\..?......d..?
+00005d00: 0006 0200 0500 6604 003f 0006 0200 0500  ......f..?......
+00005d10: 6204 003f 0006 0200 0500 5e04 003f 0006  b..?......^..?..
+00005d20: 0200 0500 5c04 003f 0006 0200 0500 6404  ....\..?......d.
+00005d30: 003f 0006 0200 0500 1204 0005 0054 0026  .?...........T.&
+00005d40: 1200 1204 5b08 005a 0026 1200 0604 5b05  ....[..Z.&....[.
+00005d50: 006a 0400 3f00 0602 0005 0068 0400 3f00  .j..?......h..?.
+00005d60: 0602 0005 0060 0400 3f00 0602 0005 0012  .....`..?.......
+00005d70: 0400 0500 5200 2612 0012 045b 0800 5600  ....R.&....[..V.
+00005d80: 2612 0006 045b 0500 5c0a 003f 0006 0200  &....[..\..?....
+00005d90: 0500 5c04 003f 0006 0200 0500 5c04 003f  ..\..?......\..?
+00005da0: 0006 0200 0500 5c04 003f 0006 0200 0500  ......\..?......
+00005db0: 5c04 003f 0006 0200 0500 5c04 003f 0006  \..?......\..?..
+00005dc0: 0200 0500 6a04 003f 0006 0200 0200 6b04  ....j..?......k.
+00005dd0: 003f 0006 0200 0200 8081 0400 3300 0602  .?..........3...
+00005de0: 0002 0028 0800 0600 6b04 7153 0002 beef  ...(....k.qS....
+00005df0: 460e 0000 0e00 7181 1a33 1c00 5f04 0812  F.....q..3.._...
+00005e00: 0074 0679 1c00 6104 0812 006a 0679 1c00  .t.y..a....j.y..
+00005e10: 5b04 0812 007f 0879 3c00 7902 003c 0880  [......y<.y..<..
+00005e20: 9006 0025 0061 1200 252d 7e04 001f 0056  ...%.a..%-~....V
+00005e30: 6200 1f01 7a02 0025 003a 0800 1000 6606  b...z..%.:....f.
+00005e40: 001f 004a 0600 1901 822e 0200 80a0 0081  ...J............
+00005e50: 0f04 002a 0182 4a02 0080 a000 811e 0400  ...*..J.........
+00005e60: 2a01 8220 0200 80a0 0081 0004 002a 0049  *.. .........*.I
+00005e70: 0200 1900 4f02 0019 005d 0200 1900 6002  ....O....]....`.
+00005e80: 0019 005d 0200 1900 808f 0200 1917 5602  ...]..........V.
+00005e90: 0019 0080 8930 0019 0066 0200 1900 5302  .....0...f....S.
+00005ea0: 0019 0081 7402 0068 175a 0200 192b 6c30  ....t..h.Z...+l0
+00005eb0: 0068 0056 5800 1900 5402 0019 0054 0200  .h.VX...T....T..
+00005ec0: 1900 5602 0019 0056 0200 1900 5a02 0019  ..V....V....Z...
+00005ed0: 0080 aa02 0019 0080 a802 0019 0080 9d02  ................
+00005ee0: 0019 0080 a902 0019 0080 9602 0019 0080  ................
+00005ef0: d902 0019 0080 d802 0019 006a 0200 1900  ...........j....
+00005f00: 1806 6a0d 0000 0500 2800 291c 0046 0477  ..j.....(.)..F.w
+00005f10: 1400 4302 0023 0055 0200 1c00 6a04 0857  ..C..#.U....j..W
+00005f20: 0044 0879 2301 813e 0200 80c4 0047 0600  .D.y#..>.....G..
+00005f30: 2543 0402 0080 cb00 0d04 360c 002b 020c  %C........6..+..
+00005f40: 3e01 8088 027f 4800 3104 0c3e 0180 9402  >.....H.1..>....
+00005f50: 7f48 0026 0475 3e01 7e02 7f48 0026 0459  .H.&.u>.~..H.&.Y
+00005f60: 1600 2e00 540c 0047 0245 0c00 3502 080c  ....T..G.E..5...
+00005f70: 004b 0202 0c00 4c02 000c 0038 0202 0c06  .K....L....8....
+00005f80: 0602 750c 0037 0e08 0c00 3802 060c 0031  ..u..7....8....1
+00005f90: 0275 0c00 3d04 630c 0606 0220 0c06 060e  .u..=.c.... ....
+00005fa0: 100c 004c 0e6f 0c00 3302 7b0c 0034 0202  ...L.o..3.{..4..
+00005fb0: 0c00 3602 040c 0036 0200 0c00 3502 060c  ..6....6....5...
+00005fc0: 0051 045d 3e00 4f04 003e 004c 0400 3e00  .Q.]>.O..>.L..>.
+00005fd0: 5204 003e 004f 0400 3e00 4a04 003e 0049  R..>.O..>.J..>.I
+00005fe0: 0400 3b00 5502 383b 0014 0269 0900 4902  ..;.U.8;...i..I.
+00005ff0: 6322 0000 0400 3304 6f09 0002 bf5b 5c0e  c"....3.o....[\.
+00006000: 0000 0e07 6480 ae1d 1207 6e12 0012 0760  ....d.....n....`
+00006010: 1200 1207 8090 1600 8099 004a 1600 0d00  ...........J....
+00006020: 4402 000d 0049 0200 0d00 5b02 000e 1364  D....I....[....d
+00006030: 0200 80a1 0026 2c00 0d00 5d00 4e12 004d  .....&,...].N..M
+00006040: 0473 3500 0002 0013 0053 0700 5504 770a  .s5......S..U.w.
+00006050: 0002 7d32 0b00 000b 0000 0100 0c0a 0411  ..}2............
+00006060: 0000 0200 1200 5507 0060 0446 3200 0002  ......U..`.F2...
+00006070: 001b 0043 0701 4804 7715 0002 7d42 0b00  ...C..H.w...}B..
+00006080: 000b 0000 0100 027d 670b 0000 0b00 0001  .......}g.......
+00006090: 0150 1249 2500 7306 0025 0073 0200 2500  .P.I%.s..%.s..%.
+000060a0: 7302 0025 0027 0a00 0d00 5f00 5012 045d  s..%.'...._.P..]
+000060b0: 0669 4300 0002 000f 005b 0700 760c 771c  .iC......[..v.w.
+000060c0: 0000 0600 0275 2a08 002c 1206 2300 0005  .....u*..,..#...
+000060d0: 000f 005b 0700 6604 5842 0000 0200 2400  ...[..f.XB....$.
+000060e0: 3109 0024 0477 0900 5004 0017 0002 7954  1..$.w..P.....yT
+000060f0: 0b00 000b 0000 0100 0006 0002 7d4f 0b00  ............}O..
+00006100: 0a16 5904 0000 0200 7e04 7f4c 0003 7d2c  ..Y.....~..L..},
+00006110: 0600 0700 6f06 0028 0c5f 0d00 5004 0812  ....o..(._..P...
+00006120: 0238 0679 2500 2a0a 000d 0066 0056 1200  .8.y%.*....f.V..
+00006130: 6f08 7d45 0000 0200 1c00 4107 0043 0477  o.}E......A..C.w
+00006140: 1a00 027d 440b 0000 0b00 0001 2980 940a  ...}D.......)...
+00006150: 3525 0037 5800 1500 4e02 6230 0000 0200  5%.7X...N.b0....
+00006160: 2400 3109 0017 0677 0b03 6404 0817 0018  $.1....w..d.....
+00006170: 0e79 0e00 5e00 3211 0002 6922 0b00 000b  .y..^.2...i"....
+00006180: 0000 0100 6820 0645 0000 0200 2400 3109  ....h .E....$.1.
+00006190: 002d 0477 1601 4204 0817 0002 794c 0b00  .-.w..B.....yL..
+000061a0: 000b 0000 0100 7814 0645 0000 0200 2400  ......x..E....$.
+000061b0: 3107 0142 0477 1500 027d 540b 0000 0b00  1..B.w...}T.....
+000061c0: 0001 0067 0e06 4500 0002 0024 0031 0900  ...g..E....$.1..
+000061d0: 2e04 7716 0142 0408 1700 0279 4c0b 0000  ..w..B.....yL...
+000061e0: 0b00 0001 006c 1606 4500 0002 0024 0031  .....l..E....$.1
+000061f0: 0900 1706 770b 0464 0408 1700 1810 790e  ....w..d......y.
+00006200: 005e 0032 1100 0267 220b 0000 0b00 0001  .^.2...g".......
+00006210: 0080 8b22 251f 004e 0638 1b00 0002 000f  ..."%..N.8......
+00006220: 005b 0700 8086 0477 2200 0006 0002 7d2a  .[.....w".....}*
+00006230: 0800 80f8 0c4f 1f02 2406 0025 0124 0600  .....O..$..%.$..
+00006240: 2500 809e 0800 1f00 7506 001f 0029 0600  %.......u....)..
+00006250: 0d00 6300 5412 0080 a606 2d1f 0043 0600  ..c.T.....-..C..
+00006260: 1000 2606 000d 0059 004e 1201 80cc 0433  ..&....Y.N.....3
+00006270: 1f00 2508 000d 005b 004c 1200 6006 351f  ..%....[.L..`.5.
+00006280: 004c 0400 0c0b 80b2 0400 1f00 4e1a 000c  .L..........N...
+00006290: 004e 0400 0c1b 8098 0400 1f00 523a 000c  .N..........R:..
+000062a0: 0281 f404 001f 0281 f408 001f 005c 0800  .............\..
+000062b0: 1f01 8116 0400 1f0e 80a2 0600 2501 80ba  ............%...
+000062c0: 1e00 2500 2808 000d 0061 0052 121b 809e  ..%.(....a.R....
+000062d0: 042f 2500 283c 000d 005f 0052 1200 6e06  ./%.(<..._.R..n.
+000062e0: 2f1f 0076 0600 2500 8084 0400 2508 1206  /..v..%.....%...
+000062f0: 001f 0041 1600 1000 808f 0600 5206 8096  ...A........R...
+00006300: 0600 80b2 0032 1200 0d00 7500 6612 003b  .....2....u.f..;
+00006310: 0a1b 1000 160a 2a0d 0000 0500 0800 6909  ......*.......i.
+00006320: 000c 0436 1100 0005 0013 0053 0700 1004  ...6.......S....
+00006330: 580c 0000 0500 2400 3109 0026 0477 1300  X.....$.1..&.w..
+00006340: 8090 0400 8086 0002 7954 0e00 000b 0000  ........yT......
+00006350: 0100 027d 570e 0000 0b00 0001 0002 7d63  ...}W.........}c
+00006360: 0e00 000e 0042 1c5d 1000 3306 000f 0181  .....B.]..3.....
+00006370: 0808 0035 080a 0c00 1904 0614 006a 270a  ...5.........j'.
+00006380: 0c00 3404 0a54 000c 1f0a 0e00 1906 0a46  ..4..T.........F
+00006390: 0025 040a 1200 1f14 0a0e 0019 030a 2c00  .%............,.
+000063a0: 1f15 0a0c 001f 2954 3000 1f00 7758 0022  ......)T0...wX."
+000063b0: 0037 0200 0700 2b02 000e 004c 0200 0700  .7....+....L....
+000063c0: 3802 001c 0014 0200 0800 1d02 000e 0028  8..............(
+000063d0: 0200 0800 1e02 0011 8113 0a02 0083 8200  ................
+000063e0: 2982 2800 1100 4c02 0020 003b 0200 0700  ).(...L.. .;....
+000063f0: 3002 0009 0034 0200 0700 2002 0009 002a  0....4.... ....*
+00006400: 0200 0e00 2902 0007 0038 080e 0d00 3104  ....)....8....1.
+00006410: 7b27 0001 0279 0200 000b 0000 0100 0102  {'...y..........
+00006420: 7905 0980 1a06 0005 0981 1a06 0005 0982  y...............
+00006430: 1a06 0005 0983 1a06 0005 0984 1a06 0005  ................
+00006440: 0985 1a06 0005 0986 1a06 0005 0800 0400  ................
+00006450: 0006 0000 0035 1505 3509 0000 0014 0052  .....5..5......R
+00006460: 8235 0d20 0080 8702 0012 002b 0400 0600  .5. .......+....
+00006470: 2902 000c 003b 0200 1b00 0102 7902 0000  )....;......y...
+00006480: 0900 0001 0000 0900 0001 0001 0000 1a00  ................
+00006490: 0000 5f1b 050b 0059 0800 0b00 5508 000b  .._....Y....U...
+000064a0: 0051 0800 0b00 5f10 0025 5379 7374 656d  .Q...._..%System
+000064b0: 2e43 6f6d 706f 6e65 6e74 4d6f 6465 6c2e  .ComponentModel.
+000064c0: 4461 7461 416e 6e6f 7461 7469 6f6e 731e  DataAnnotations.
+000064d0: 5379 7374 656d 2e54 6578 742e 4a73 6f6e  System.Text.Json
+000064e0: 2e53 6572 6961 6c69 7a61 7469 6f6e 2501  .Serialization%.
+000064f0: adde 01ad e501 ae00 01ae 0a01 ae16 01ae  ................
+00006500: 2601 ae37 01c0 004b 9101 aee1 01b0 ff01  &..7...K........
+00006510: c000 4bb7 0700 0000 5680 da05 0700 0000  ..K.....V.......
+00006520: 2e81 1005 1b00 0000 1d81 3705 0b00 2408  ..........7...$.
+00006530: 000b 0028 0800 0b00 2608 000b 001d 1200  ...(....&.......
+00006540: 0700 0000 2482 2905 0c00 0000 2682 3305  ....$.).....&.3.
+00006550: 0b00 3208 0011 0000 001f 823e 050b 001e  ..2........>....
+00006560: 0800 0b00 3d08 0007 0000 0018 8255 0523  ....=........U.#
+00006570: 0000 0069 0c09 2100 80a8 0400 2100 80bc  ...i..!.....!...
+00006580: 0400 3100 808f 0400 2100 8085 0600 2100  ..1.....!.....!.
+00006590: 0102 791d 01ad de01 ade5 01ae 0001 ae0a  ..y.............
+000065a0: 01ae 1601 ae26 01ae 3701 ae8d 01ae 9d03  .....&..7.......
+000065b0: 1c80 a90a 0000 5f1c 0921 005f 0200 2114  ......_..!._..!.
+000065c0: 1204 001b 0612 2c00 2107 1210 0021 0412  ......,.!....!..
+000065d0: 1200 2106 120c 0021 1d12 0e00 2117 123e  ..!....!....!..>
+000065e0: 0082 2800 4134 0012 005b 0600 3400 6e02  ..(.A4...[..4.n.
+000065f0: 001b 005c 0400 3700 6f02 001b 005c 0400  ...\..7.o....\..
+00006600: 3400 6f02 001b 005c 0400 3700 6f02 001b  4.o....\..7.o...
+00006610: 005b 0400 3400 6e02 001b 005c 0400 3700  .[..4.n....\..7.
+00006620: 6f02 001b 005c 0400 3700 6f02 001b 0080  o....\..7.o.....
+00006630: 870a 0021 0080 8706 0021 0080 8706 0021  ...!.....!.....!
+00006640: 0080 8706 0021 0080 8706 0021 0080 8706  .....!.....!....
+00006650: 0021 0080 8706 0021 0001 0279 1100 0000  .!.....!...y....
+00006660: 3780 be09 0800 3e02 0008 0001 0279 82a7  7.....>......y..
+00006670: 0b00 004d 0c09 110e 1206 0010 0050 1e02  ...M.........P..
+00006680: 2100 5002 0021 0032 067f 1200 0c02 2a0c  !.P..!.2......*.
+00006690: 0000 0200 0800 6906 0052 0420 2f00 0002  ......i..R. /...
+000066a0: 0008 0069 0600 1f04 7706 0002 7d1c 0a00  ...i....w...}...
+000066b0: 0009 0000 0100 027d 790a 0000 0900 0001  .......}y.......
+000066c0: 0013 105d 0800 1906 0006 0014 0248 0d00  ...].........H..
+000066d0: 0005 0017 004b 1c00 1304 7703 000c 022a  .....K....w....*
+000066e0: 0c00 0005 0008 0069 0800 1004 2c0d 0000  .......i....,...
+000066f0: 0500 0e00 5d08 0020 0477 0e00 4c04 001d  ....].. .w..L...
+00006700: 0050 0200 1d00 2602 000d 0080 9004 0838  .P....&........8
+00006710: 012a 0679 4200 5506 0838 002b 0679 0400  .*.yB.U..8.+.y..
+00006720: 1102 0007 0080 fe06 0862 0080 ed04 0053  .........b.....S
+00006730: 001b 0200 0e00 0d06 7903 001e 0200 0c00  ........y.......
+00006740: 7304 086a 0016 0200 0d00 1902 0009 0036  s..j...........6
+00006750: 0679 1300 4402 0013 0042 0200 1328 0404  .y..D....B...(..
+00006760: 0080 9d00 1704 360c 003b 0202 3800 3b02  ......6..;..8.;.
+00006770: 0a38 003b 0273 3800 2d02 0a0c 002d 0279  .8.;.s8.-....-.y
+00006780: 0c00 2d02 7d0c 002d 0204 0c00 2d02 000c  ..-.}..-....-...
+00006790: 002d 027b 0c00 2d02 020c 002d 0204 0c00  .-.{..-....-....
+000067a0: 2d02 7f0c 002d 020e 0c00 2d02 7d0c 002d  -....-....-.}..-
+000067b0: 0204 0c00 2d02 000c 002d 027d 0c00 2d02  ....-....-.}..-.
+000067c0: 000c 002d 0202 0c00 2d02 7d0c 002d 0206  ...-....-.}..-..
+000067d0: 0c00 2d02 730c 002d 0200 0c00 2d02 000c  ..-.s..-....-...
+000067e0: 002d 0210 0c00 2d02 020c 002d 027f 0c00  .-....-....-....
+000067f0: 2d02 040c 002d 027b 0c00 2d02 0c0c 002d  -....-.{..-....-
+00006800: 0269 0c03 80b2 0210 5f00 5d08 7f4c 005e  .i......_.]..L.^
+00006810: 024f 5200 0004 0061 066f 1600 2f04 080c  .OR....a.o../...
+00006820: 0031 0200 0a00 0c02 0002 0012 0408 1300  .1..............
+00006830: 0d02 0010 0061 0871 1600 1404 080e 0024  .....a.q.......$
+00006840: 0408 1300 0d02 0010 0061 0871 1c00 2204  .........a.q..".
+00006850: 0819 0012 0200 1300 2202 0010 0080 9602  ........".......
+00006860: 0054 0080 9e02 0030 000d 022a 0700 0002  .T.....0...*....
+00006870: 0008 0069 0900 1802 770f 0002 7f1c 0b00  ...i....w.......
+00006880: 000e 0061 0855 1c00 4a04 0813 002c 0200  ...a.U..J....,..
+00006890: 1900 1202 0013 0017 0200 0c00 6202 0840  ............b..@
+000068a0: 0000 0200 2002 0215 0062 027f 4000 3108  .... ....b..@.1.
+000068b0: 710b 002c 0208 0900 0002 0032 0202 0b00  q..,.......2....
+000068c0: 2b02 7f09 0000 0200 2304 0009 002c 0479  +.......#....,.y
+000068d0: 0e00 1102 0004 0006 0200 0200 02be f728  ...............(
+000068e0: 0d00 0009 0000 0100 0a81 1051 0400 0600  ...........Q....
+000068f0: 1602 0002 beed 060d 0000 0900 0001 000b  ................
+00006900: 811a 5d04 0043 0208 3800 02be df32 0e00  ..]..C..8....2..
+00006910: 000e 0001 8126 3720 01ad de01 ade5 01ae  .....&7 ........
+00006920: 0001 ae0a 01ae 1601 ae26 01ae 3701 ae8d  .........&..7...
+00006930: 01ae 9d01 aeb8 031c 8135 0c00 0039 0c09  .........5...9..
+00006940: 0600 1602 520d 0000 0200 1c00 411c 0065  ....R.......A..e
+00006950: 0277 5400 027f 440b 0000 0e00 3d04 3507  .wT...D.....=.5.
+00006960: 0071 0400 1d0d 0a02 004c 0077 1c00 1d00  .q.......L.w....
+00006970: 5e02 000b 0075 0200 1e05 0a02 000c 0075  ^....u.........u
+00006980: 0c00 1e09 0a02 000c 0071 1400 1e22 0a02  .........q..."..
+00006990: 000c 001f 4600 0c00 2402 000c 0024 0200  ....F...$....$..
+000069a0: 0d00 2602 000d 0021 0200 0d00 8087 0600  ..&....!........
+000069b0: 3000 2602 000d 0080 9202 001b 0033 0400  0.&..........3..
+000069c0: 0d00 3a02 0007 0025 0200 0800 3302 0007  ..:....%....3...
+000069d0: 001e 0200 0800 2802 000e 0027 0200 0700  ......(....'....
+000069e0: 2f04 000d 0036 0200 0700 2a02 0008 002f  /....6....*..../
+000069f0: 0200 0700 1e02 0008 0028 0200 0e00 2702  .........(....'.
+00006a00: 0007 002f 0400 0d00 3602 0007 0027 0200  .../....6....'..
+00006a10: 0900 2f02 0007 001e 0200 0800 2802 000e  ../.........(...
+00006a20: 0027 0200 0700 2f04 000d 0036 0200 0700  .'..../....6....
+00006a30: 2c02 0009 002f 0200 0700 1e02 0008 0028  ,..../.........(
+00006a40: 0200 0e00 2702 0007 002f 0400 0d00 3602  ....'..../....6.
+00006a50: 0007 002a 0200 0900 2f02 0007 001f 0200  ...*..../.......
+00006a60: 0900 2802 000e 0027 0200 0700 0102 790b  ..(....'......y.
+00006a70: 5379 7374 656d 2e54 6578 7423 01ad de01  System.Text#....
+00006a80: ade5 01ae 0001 ae0a 01ae 1601 ae26 01ae  .............&..
+00006a90: 3701 c000 5157 01ae 8d01 ae9d 01ae b87d  7...QW.........}
+00006aa0: 0d00 005a 0c09 0b00 1602 560d 0000 0500  ...Z......V.....
+00006ab0: 1e00 3d18 0011 0430 0e00 0005 0010 0059  ..=....0.......Y
+00006ac0: 0900 8084 0477 808d 0002 7d2c 0e00 000e  .....w....},....
+00006ad0: 0002 7d14 0e00 000e 0038 0e31 0700 5602  ..}......8.1..V.
+00006ae0: 0017 110a 0200 2100 6e24 001d 0048 0200  ......!.n$...H..
+00006af0: 0b00 2102 000c 0046 0200 1c00 3702 0006  ..!....F....7...
+00006b00: 0024 0200 0700 3002 0007 001b 0200 0800  .$....0.........
+00006b10: 2202 000d 0021 0200 0700 0102 790c 0000  "....!......y...
+00006b20: 0080 a30a 0921 0001 0279 1b01 adde 01ad  .....!...y......
+00006b30: e501 ae00 01ae 0a01 ae16 01ae 2601 ae37  ............&..7
+00006b40: 01ae 8d01 ae9d 4b0e 0000 4d0a 0912 005d  ......K...M....]
+00006b50: 0600 2100 5f02 0021 002b 0600 0d00 5d04  ..!._..!.+....].
+00006b60: 0811 1412 0279 2107 1a2c 0021 0080 af12  .....y!..,.!....
+00006b70: 0021 0080 af02 0021 0080 8904 001b 0080  .!.....!........
+00006b80: a304 0021 2a0a 0400 1b0d 0a5a 001b 0001  ...!*......Z....
+00006b90: 1c79 0600 0000 1a61 2307 0000 0001 80a0  .y.....a#.......
+00006ba0: 4907 0000 0018 8503 3107 0000 0018 8513  I.......1.......
+00006bb0: 4907 0000 0017 8514 4907 0000 0017 8515  I.......I.......
+00006bc0: 3307 0000 0018 852f 5107 0000 0018 8530  3....../Q......0
+00006bd0: 5107 0000 0018 8531 5107 0000 0018 8532  Q......1Q......2
+00006be0: 5108 0000 0180 aa87 0a3f 0700 0002 6687  Q........?....f.
+00006bf0: 1940 0700 0002 6687 3040 0800 0001 80a6  .@....f.0@......
+00006c00: 873a 4007 0000 0035 8ad5 4007 0000 0030  .:@....5..@....0
+00006c10: 8afb 7307 0000 0036 8b18 6a07 0000 0030  ..s....6..j....0
+00006c20: 8b4a 5707 0000 0030 8b5a 7107 0f00 0040  .JW....0.Zq....@
+00006c30: 8b64 7107 0000 002f 8b6b 7107 0000 0034  .dq..../.kq....4
+00006c40: 8b76 7180 b110 0000 2152 2709 0000 0200  .vq.....!R'.....
+00006c50: 0d00 5f04 001d 0477 0700 0004 0002 7d26  .._....w......}&
+00006c60: 0600 1b0a 0a09 0000 0500 0f00 5b04 0000  ............[...
+00006c70: 0700 3404 770d 0056 0200 2e00 2404 000d  ..4.w..V....$...
+00006c80: 0041 0200 1d00 2d02 001d 000e 0408 0700  .A....-.........
+00006c90: 2002 0013 0027 0200 1400 2104 0013 0080   ....'....!.....
+00006ca0: 8304 084f 002e 0871 1a00 6d00 5e3b 0017  ...O...q..m.^;..
+00006cb0: 0423 0d00 1702 000d 004e 0200 1800 4302  .#.......N....C.
+00006cc0: 0007 0022 0200 0f00 2202 000f 005c 0200  ..."...."....\..
+00006cd0: 2c00 6002 002c 0025 0200 0d00 2602 0011  ,.`..,.%....&...
+00006ce0: 001e 0200 1b00 6602 0022 0000 0400 0241  ......f..".....A
+00006cf0: 2a09 0001 4447 3811 0000 4380 9f0d 0600  *...DG8...C.....
+00006d00: 5d02 2e3b 0000 0200 0a00 6507 0019 0477  ]..;......e....w
+00006d10: 0900 6a00 342c 0002 7d6d 0a00 0009 0000  ..j.4,..}m......
+00006d20: 0100 100a 5908 003e 0208 1100 0c04 790c  ....Y..>......y.
+00006d30: 0000 0406 80fe 0d71 0001 0a79 0700 0000  .......q...y....
+00006d40: 4286 fc52 0700 0000 428a dc52 0600 0000  B..R....B..R....
+00006d50: 316e 2c07 0000 006a 8086 2507 0000 004a  1n,....j..%....J
+00006d60: 8089 2507 0000 006e 8092 2607 0000 004d  ..%....n..&....M
+00006d70: 8095 2607 0000 006c 8236 2606 0000 0034  ..&....l.6&....4
+00006d80: 253f 0712 0000 6780 9f44 0000            %?....g..D..
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/Attribution.md` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/Attribution.md`

 * *Files 20% similar despite different names*

```diff
@@ -23,57 +23,64 @@
 - The Speed Booster Upgrade sprites were (`items/speedboosterUpgrade`) were made by BastionB56 and modified
   by [Miepee](https://github.com/Miepee)
 
 Offworld items
 - The RDV item sprite (`offworld items/default`) was made by [Miepee](https://github.com/Miepee). It's a modification of the Unknown sprite by [AbyssalCreature](https://github.com/AbyssalCreature) and the [Randovania logo](https://github.com/randovania/randovania/tree/main/tools/icons) by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
 
 Dread items:
-- The Cross Bomb (`offworld items/dread/crossBombs`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
-- The Diffusion Beam (`offworld items/dread/diffusionBeam`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
-- The Energy Part (`offworld items/dread/energyPart`) sprites were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Flash Shift (`offworld items/dread/flashShift`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature)
-- The Grapple Beam (`offworld items/dread/grappleBeam`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature)
-- The Ice Missiles (`offworld items/dread/iceMissiles`) sprites were made by [Shale](https://cohost.org/RaffiTheOwl), modified from the Missile Launcher sprites by ShirtyScarab554
+- The Cross Bomb sprites (`offworld items/dread/crossBombs`) were made by [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
+- The Diffusion Beam sprites (`offworld items/dread/diffusionBeam`) were made by [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
+- The Energy Part sprites (`offworld items/dread/energyPart`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and [radzo73](https://github.com/radzo73)
+- The Energy Tank sprites (`offworld items/dread/energyTank`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and [radzo73](https://github.com/radzo73)
+- The Flash Shift sprites (`offworld items/dread/flashShift`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Grapple Beam sprites (`offworld items/dread/grappleBeam`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Ice Missiles sprites (`offworld items/dread/iceMissiles`) were made by [Shale](https://cohost.org/RaffiTheOwl), modified from the Missile Launcher sprites by ShirtyScarab554
+- The Missile Tank sprites (`offworld items/dread/missileTank`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and Samario
+- The Missile Tank+ sprites (`offworld items/dread/missileTankPlus`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and Samario
 - The Morph Ball sprites (`offworld items/dread/morphBall`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
-- The Phantom Cloak (`offworld items/dread/phantomCloak`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature)
-- The Pulse Radar (`offworld items/dread/pulseRadar`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature)
-- The Space Jump(`offworld items/dread/spaceJump`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Missile Tank sprites (`offworld items/dread/missileTank`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and Samario
+- The Power Bomb Launcher sprites (`offworld items/dread/pbLauncher`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and Samario
+- The Power Bomb Tank sprites (`offworld items/dread/pbTank`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), ShirtyScarab554 and Samario
+- The Phantom Cloak sprites (`offworld items/dread/phantomCloak`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Pulse Radar sprites (`offworld items/dread/pulseRadar`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Space Jump sprites (`offworld items/dread/spaceJump`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Speed Booster sprites (`offworld items/dread/speedBooster`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Spider Magnet sprites (`offworld items/dread/spiderMagnet`) were made by [AbyssalCreature](https://github.com/AbyssalCreature), modified from the Spin Boost sprites by ShirtyScarab554
 - The Spin Boost sprites (`offworld items/dread/spinBoost`) were made by ShirtyScarab554
 - The Storm Missile sprites (`offworld items/dread/stormMissiles`) were made by [Shale](https://cohost.org/RaffiTheOwl), modified from the Missile Launcher sprites by ShirtyScarab554
-- The Wide Beam (`offworld items/dread/wideBeam`) sprites were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Varia Suit sprites (`offworld items/dread/variaSuit`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Wide Beam sprites (`offworld items/dread/wideBeam`) were made by [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
 
 Echoes items:
-- The Amber translator sprites (`offworld items/primes/echoes/amber`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Annihilator sprites (`offworld items/primes/echoes/annihilator`) were made by JKMaxx and [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
+- The Amber translator sprites (`offworld items/primes/echoes/amber`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia), [AbyssalCreature](https://github.com/AbyssalCreature) and [Uncle Reggie](https://www.threads.net/@unclereggiegames)
+- The Annihilator sprites (`offworld items/primes/echoes/annihilator`) were made by JKMaxx, [LaKompetenzia](https://www.twitch.tv/ilakompetenzia), [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
 - The Beam Ammo sprites (`offworld items/primes/echoes/beamAmmo`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Cannon Ball sprites (`offworld items/primes/echoes/cannonBall`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Cobalt translator sprites (`offworld items/primes/echoes/cobalt`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Dark Agon Key sprites (`offworld items/primes/echoes/darkAgon`) were made by [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q)
+- The Cobalt translator sprites (`offworld items/primes/echoes/cobalt`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia), [AbyssalCreature](https://github.com/AbyssalCreature) and [Uncle Reggie](https://www.threads.net/@unclereggiegames)
+- The Dark Agon Key sprites (`offworld items/primes/echoes/darkAgon`) were made by [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Dark Beam Ammo sprites (`offworld items/primes/echoes/darkAmmo`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Dark Beam sprites (`offworld items/primes/echoes/darkBeam`) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
-- The Dark Burst sprites (`offworld items/primes/echoes/darkBurst`) were made by [JeffGainsNGames](https://www.youtube.com/@jeffgainsngames)
+- The Dark Burst sprites (`offworld items/primes/echoes/darkBurst`) were made by [JeffGainsNGames](https://www.youtube.com/@jeffgainsngames), [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
 - The Dark Suit sprites (`offworld items/primes/echoes/darkSuit`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Dark Torvus Key sprites (`offworld items/primes/echoes/darkTorvus`) were made by [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q)
+- The Dark Torvus Key sprites (`offworld items/primes/echoes/darkTorvus`) were made by [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Dark Visor sprites (`offworld items/primes/echoes/darkVisor`) were made by [JeffGainsNGames](https://www.youtube.com/@jeffgainsngames)
 - The Echo Visor sprites (`offworld items/primes/echoes/echoVisor`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Emerald Translator sprites (`offworld items/primes/echoes/emerald`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Ing Hive Key sprites (`offworld items/primes/echoes/ingHive`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
+- The Emerald Translator sprites (`offworld items/primes/echoes/emerald`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Ing Hive Key sprites (`offworld items/primes/echoes/ingHive`) were made by [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Light Beam Ammo sprites (`offworld items/primes/echoes/lightAmmo`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Light Beam sprites (`offworld items/primes/echoes/lightBeam`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Light Suit sprites (`offworld items/primes/echoes/lightSuit`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Power Bomb Launcher (`offworld items/primes/echoes/powerBombLauncher`) sprites were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
+- The Power Bomb Launcher sprites (`offworld items/primes/echoes/powerBombLauncher`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Progressive Suit sprites (`offworld items/primes/echoes/progressiveSuit`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Screw Attack sprites (`offworld items/primes/echoes/screwAttack`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Seeker Missile sprites (`offworld items/primes/echoes/seekers`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Sky Temple Key sprites (`offworld items/primes/echoes/skyTempleKey`) were made [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q)
+- The Sky Temple Key sprites (`offworld items/primes/echoes/skyTempleKey`) were made [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Sonic Boom sprites (`offworld items/primes/echoes/sonicBoom`) were made by [Schwartz Ghandi](https://www.youtube.com/channel/UCTm7a6JWDeTiHkWa8xR9W-Q), [AbyssalCreature](https://github.com/AbyssalCreature) and ShirtyScarab554
-- The Super Missile sprites (`offworld items/primes/echoes/superMissile`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
-- The Violet translator sprites (`offworld items/primes/echoes/violet`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
+- The Super Missile sprites (`offworld items/primes/echoes/superMissile`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
+- The Violet translator sprites (`offworld items/primes/echoes/violet`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
 
 
 Prime items:
 - The Artifact sprites (`offworld items/primes/prime1/artifact` as well as the suffixes) were made by [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Bomb sprites (`offworld items/primes/prime1/bombs`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Boost Ball sprites (`offworld items/primes/prime1/boostBall`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Combat Visor sprites (`offworld items/primes/prime1/combatVisor`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
@@ -82,15 +89,15 @@
 - The Gravity Suit sprites (`offworld items/primes/prime1/gravity`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Ice Beam sprites (`offworld items/primes/prime1/iceBeam`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
 - The Ice Spreader sprites (`offworld items/primes/prime1/iceSpreader`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Morph Ball sprites (`offworld items/primes/prime1/morphBall`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Phazon Suit sprites (`offworld items/primes/prime1/phazonSuit`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Plasma Beam sprites (`offworld items/primes/prime1/plasmaBeam`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
 - The Power Beam sprites (`offworld items/primes/prime1/powerBeam`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
-- The Power Bomb Launcher (`offworld items/primes/prime1/powerBombLauncher`) sprites were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
+- The Power Bomb Launcher sprites (`offworld items/primes/prime1/powerBombLauncher`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Scan Visor sprites (`offworld items/primes/prime1/scanVisor`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
 - The Super Missile sprites (`offworld items/primes/prime1/superMissile`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The Thermal Visor sprites (`offworld items/primes/prime1/thermalVisor`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
 - The Varia Suit sprites (`offworld items/primes/prime1/varia`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia)
 - The Wave Beam sprites (`offworld items/primes/prime1/waveBeam`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
 - The Wave Buster sprites (`offworld items/primes/prime1/waveBuster`) were made by [LaKompetenzia](https://www.twitch.tv/ilakompetenzia) and [AbyssalCreature](https://github.com/AbyssalCreature)
 - The X-Ray sprites (`offworld items/primes/prime1/xrayVisor`) were made by [Uncle Reggie](https://www.threads.net/@unclereggiegames)
```

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/LICENSE-GRAPHICS` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/LICENSE-GRAPHICS`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearBulletHell.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearBulletHell.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearPipeHub.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearPipeHub.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearSave.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearSave.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPNearTotem.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearTotem.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPRightExterior.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPRightExterior.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorA5EMPRobotHome.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPRobotHome.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorAnim_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorArachnus.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorArachnus.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorBlue.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorBlue.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorBomb.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPA1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPA2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPA3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorGenesis.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorGenesis.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorGuardian.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorGuardian.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorIceBeam.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorIceBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorLocked.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorLocked.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorMissile.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorPBomb.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorQueen.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorQueen.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorScrew.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorScrew.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSerris.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSerris.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSpider.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSpider.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorSuper.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSuper.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTempLocked.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTempLocked.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTester.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTester.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTorizo.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTorizo.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/items/unknown/sItemUnknown_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/bg_MapBottom2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bg_MapBottom2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIMissileSelected.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileSelected.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUIPBombSelected.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombSelected.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/hud/sGUISMissileSelected.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileSelected.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newA4Doors.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newA4Doors.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/newA4Doors2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newA4Doors2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadP.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadP.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpHideout.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpHideout.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_11.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_13.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_14.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_15.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_16.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_11.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_13.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_14.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_15.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_16.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_17.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_17.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_18.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_18.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_19.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_19.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_0.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_11.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_12.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_13.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_14.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_15.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_16.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_17.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_17.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_18.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_18.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_19.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_19.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_20.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_20.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_21.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_21.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_22.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_22.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_23.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_23.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_10.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_8.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_9.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_1.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_2.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_3.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_4.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_5.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_6.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_7.png` & `am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/am2r_yams.egg-info/PKG-INFO` & `am2r_yams-2.0.0/am2r_yams.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 1.2.9
+Version: 2.0.0
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `am2r_yams-1.2.9/am2r_yams.egg-info/SOURCES.txt` & `am2r_yams-2.0.0/am2r_yams.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -301,14 +301,19 @@
 am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_1.png
 am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_2.png
 am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_3.png
 am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_1.png
 am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_2.png
 am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_4.png
+am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_1.png
+am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_2.png
+am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_0.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_1.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_2.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_3.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_5.png
 am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_6.png
@@ -337,14 +342,30 @@
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_3.png
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_5.png
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_6.png
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_7.png
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_8.png
 am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_9.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_0.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_1.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_2.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_4.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_5.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_6.png
+am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_7.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_0.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_1.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_2.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_4.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_5.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_6.png
+am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_7.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_1.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_10.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_11.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_12.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_13.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_14.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_15.png
@@ -353,14 +374,38 @@
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_3.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_5.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_6.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_7.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_8.png
 am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_9.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_0.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_1.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_10.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_11.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_12.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_13.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_14.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_15.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_2.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_4.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_5.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_6.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_7.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_8.png
+am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_9.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_0.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_1.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_2.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_4.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_5.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_6.png
+am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_7.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_0.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_1.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_2.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_3.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_5.png
 am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_6.png
@@ -444,14 +489,23 @@
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_3.png
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_4.png
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_5.png
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_6.png
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_7.png
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_8.png
 am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_9.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_0.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_1.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_2.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_3.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_4.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_5.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_6.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_7.png
+am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_8.png
 am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_0.png
 am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_1.png
 am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_2.png
 am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_3.png
@@ -478,20 +532,20 @@
 am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_9.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_6.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_0.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_10.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_11.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_12.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_13.png
-am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_14.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_7.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_8.png
@@ -500,21 +554,38 @@
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_4.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_0.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_1.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_10.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_11.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_12.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_13.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_14.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_15.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_16.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_17.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_18.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_19.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_2.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_20.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_21.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_22.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_23.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_7.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_8.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_9.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_10.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_11.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_12.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_13.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_14.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_15.png
@@ -523,20 +594,20 @@
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_7.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_8.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_9.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_0.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_10.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_11.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_12.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_13.png
-am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_14.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_7.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_8.png
@@ -555,20 +626,20 @@
 am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_6.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_0.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_10.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_11.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_12.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_13.png
-am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_14.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_7.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_8.png
@@ -621,20 +692,20 @@
 am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_4.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_0.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_10.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_11.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_12.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_13.png
-am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_14.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_7.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_8.png
@@ -647,18 +718,18 @@
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_7.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_8.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_9.png
+am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_0.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_3.png
-am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_1.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_2.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_3.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_4.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_5.png
 am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_6.png
 am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_0.png
```

### Comparing `am2r_yams-1.2.9/am2r_yams_tests/test_meta.py` & `am2r_yams-2.0.0/am2r_yams_tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `am2r_yams-1.2.9/setup.cfg` & `am2r_yams-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = am2r_yams
-version = 1.2.9
+version = 2.0.0
 description = An open source randomizer patcher for AM2R.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Miepee/YAMS
 author = Miepee
 license_files = 
 	LICENSE
```

