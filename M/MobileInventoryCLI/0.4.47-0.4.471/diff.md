# Comparing `tmp/MobileInventoryCLI-0.4.47.tar.gz` & `tmp/MobileInventoryCLI-0.4.471.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.47.tar", last modified: Tue Apr  9 14:33:23 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.471.tar", last modified: Tue Apr  9 14:53:31 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.47.tar` & `MobileInventoryCLI-0.4.471.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.336495 MobileInventoryCLI-0.4.47/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.336495 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   102988 2024-04-09 13:55:42.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-09 14:17:00.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    26852 2024-04-09 14:28:55.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-09 14:32:06.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-09 14:19:49.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5301 2024-04-09 14:31:46.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-09 14:32:11.000000 MobileInventoryCLI-0.4.47/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.716521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.719854 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.719854 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.719854 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   103215 2024-04-09 14:53:18.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    26852 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 14:53:28.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5301 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      714 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      714 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      820 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/setup.py
```

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,15 +876,15 @@
     Tax=Column(Float)
     TaxNote=Column(String)
 
     Note=Column(String)
     Size=Column(String)
     
     CaseCount=Column(Integer)
-
+    userUpdated=Column(Boolean)
     Shelf=Column(Integer)
     BackRoom=Column(Integer)
     Display_1=Column(Integer)
     Display_2=Column(Integer)
     Display_3=Column(Integer)
     Display_4=Column(Integer)
     Display_5=Column(Integer)
@@ -934,17 +934,18 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',DayLogDate=datetime.now(),DayLogId=None,CRV=0.0,Tax=0.0,TaxNote=''):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',DayLogDate=datetime.now(),DayLogId=None,CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False):
         if EntryId:
             self.EntryId=EntryId
+        self.userUpdated=userUpdated
         self.CRV=CRV
         self.Tax=Tax
         self.TaxNote=TaxNote
         self.Barcode=Barcode
         self.Code=Code
         self.Name=Name
         self.Price=Price
@@ -1237,14 +1238,15 @@
                     new.append(i)
             name='\n'.join(new)
         if num == None:
             num=''
         msg=f"""
 ============={Fore.green}{num}{Style.reset}============
 {Fore.cyan}DayLogId = {self.DayLogId}{Style.reset}
+{Fore.light_magenta}userUpdated = {self.userUpdated}{Style.reset}
 {Fore.cyan}DayLogDate = {self.DayLogDate}{Style.reset}
 {Fore.red}EntryId{Style.bold}={Fore.green_yellow}{self.EntryId}{Style.reset}
 {Fore.blue}Barcode{Style.reset} = {Fore.aquamarine_3}{self.Barcode}{Style.reset}
 {Fore.dark_goldenrod}Code/Shelf/Label{Style.reset} = {Fore.yellow}{self.Code}{Style.reset}
 {Fore.green_yellow}Name{Style.reset} = {Fore.cyan}{name}{Style.reset}
 {Fore.violet}Shelf{Style.reset} = {Fore.magenta}{self.Shelf}{Style.reset}
 {Fore.yellow_4b}BackRoom/Wall{Style.reset} = {Fore.orange_4b}{self.BackRoom}{Style.reset}
@@ -1289,14 +1291,15 @@
                 return name
         except Exception as e:
             return ''
 
     def __repr__(self):
         m= f"""
         {Style.bold}{Style.underline}{Fore.pale_green_1b}Daylog{Style.reset}(
+        {Fore.light_magenta}userUpdated = {self.userUpdated}{Style.reset},
         {Fore.cyan}DayLogId = {self.DayLogId}{Style.reset},
         {Fore.cyan}DayLogDate = {self.DayLogDate}{Style.reset},
         {Fore.hot_pink_2}{Style.bold}{Style.underline}EntryId{Style.reset}={self.EntryId}
         {Fore.violet}{Style.underline}Code{Style.reset}='{self.Code}',
         {Fore.orange_3}{Style.bold}Barcode{Style.reset}='{self.Barcode}',
         {Fore.orange_3}{Style.underline}UPCE from UPCA[if any]{Style.reset}='{self.upce2upca}',
         {Fore.green}{Style.bold}Price{Style.reset}=${self.Price},
```

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.47
+Version: 0.4.471
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.47/PKG-INFO` & `MobileInventoryCLI-0.4.471/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.47
+Version: 0.4.471
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.47/setup.py` & `MobileInventoryCLI-0.4.471/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.47'
+version='0.4.471'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

