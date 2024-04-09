# Comparing `tmp/MobileInventoryCLI-0.4.46.tar.gz` & `tmp/MobileInventoryCLI-0.4.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.46.tar", last modified: Thu Apr  4 19:02:13 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.47.tar", last modified: Tue Apr  9 14:33:23 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.46.tar` & `MobileInventoryCLI-0.4.47.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.931988 MobileInventoryCLI-0.4.46/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.918655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.921988 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.921988 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.921988 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-04 18:57:55.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.925321 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-04 18:58:55.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      599 2024-04-04 19:00:27.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.928655 MobileInventoryCLI-0.4.46/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-04 17:57:33.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:13.931988 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 19:02:13.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-04 19:02:13.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-04 19:02:13.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-04 19:02:13.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-04 19:02:13.000000 MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-04 19:02:13.931988 MobileInventoryCLI-0.4.46/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-04 19:02:13.931988 MobileInventoryCLI-0.4.46/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      810 2024-04-04 19:02:13.000000 MobileInventoryCLI-0.4.46/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.336495 MobileInventoryCLI-0.4.47/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.336495 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   102988 2024-04-09 13:55:42.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-09 14:17:00.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.339828 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    26852 2024-04-09 14:28:55.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-09 14:32:06.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-09 14:19:49.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5301 2024-04-09 14:31:46.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.343161 MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-04 19:02:21.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 14:33:23.000000 MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-09 14:33:23.346495 MobileInventoryCLI-0.4.47/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-09 14:32:11.000000 MobileInventoryCLI-0.4.47/setup.py
```

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
     Display_3=Column(Integer)
     Display_4=Column(Integer)
     Display_5=Column(Integer)
     Display_6=Column(Integer)
     InList=Column(Boolean)
     Stock_Total=Column(Integer)
     Location=Column(String)
+    userUpdated=Column(Boolean)
     ListQty=Column(Float)
     upce2upca=Column(String)
     Image=Column(String)
     EntryId=Column(Integer,primary_key=True)
     Timestamp=Column(Float)
 
     ALT_Barcode=Column(String)
@@ -342,18 +343,19 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote=''):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False):
         if EntryId:
             self.EntryId=EntryId
         self.CRV=CRV
+        self.userUpdated=userUpdated
         self.Tax=Tax
         self.TaxNote=TaxNote
         self.Barcode=Barcode
         self.Code=Code
         self.Name=Name
         self.Price=Price
         self.Note=Note
@@ -723,15 +725,17 @@
                     new.append(i)
             name='\n'.join(new)
         if num == None:
             num=''
         total_value=self.total_value(CaseMode=False)
         total_value_case=self.total_value()
         msg=f"""
+
 ============={Fore.green}{num}{Style.reset}============
+{Fore.light_magenta}UserUpdated={self.userUpdated}{Style.reset}
 {Fore.red}EntryId{Style.bold}={Fore.green_yellow}{self.EntryId}{Style.reset}
 {Fore.blue}Barcode{Style.reset} = {Fore.aquamarine_3}{self.Barcode}{Style.reset}
 {Fore.dark_goldenrod}Code/Shelf/Label{Style.reset} = {Fore.yellow}{self.Code}{Style.reset}
 {Fore.green_yellow}Name{Style.reset} = {Fore.cyan}{name}{Style.reset}
 {Fore.violet}Shelf{Style.reset} = {Fore.magenta}{self.Shelf}{Style.reset}
 {Fore.yellow_4b}BackRoom/Wall{Style.reset} = {Fore.orange_4b}{self.BackRoom}{Style.reset}
 {Fore.slate_blue_1}Display_1{Style.reset} = {Fore.medium_purple_3b}{self.Display_1}{Style.reset}
@@ -779,14 +783,15 @@
             return ''
 
     def __repr__(self):
         total_value=self.total_value(CaseMode=False)
         total_value_case=self.total_value()
         m= f"""
 {Style.bold}{Style.underline}{Fore.pale_green_1b}Entry{Style.reset}(
+{Fore.light_magenta}UserUpdated={self.userUpdated}{Style.reset},
 {Fore.hot_pink_2}{Style.bold}{Style.underline}EntryId{Style.reset}={self.EntryId}
 {Fore.violet}{Style.underline}Code{Style.reset}='{self.Code}',
 {Fore.orange_3}{Style.bold}Barcode{Style.reset}='{self.Barcode}',
 {Fore.orange_3}{Style.underline}UPCE from UPCA[if any]{Style.reset}='{self.upce2upca}',
 {Fore.green}{Style.bold}Price{Style.reset}=${self.Price},
 {Fore.green}{Style.bold}CRV{Style.reset}=${self.CRV},
 {Fore.green}{Style.bold}Tax{Style.reset}=${self.Tax},
@@ -1670,14 +1675,15 @@
         if code and field and value:
             print(code,field,value)
             if field not in self.valid_field_names:
                 raise Exception(f"InvalidField '{field}:{self.valid_field_names}'")
             if field in ['Timestamp',]:
                 raise Exception(f"Field not supported for changes yet!")
 
+
             with Session(self.engine) as session:
                 ext=code.lower().split('.')[0]
                 cd=code.lower().split('.')[-1]
                 
                 #result=session.query()
                 if ext in ['b']:
                     try:
@@ -2022,14 +2028,16 @@
                 if value not in ['True','False','1','0']:
                     raise Exception(f"Not a Boolean: {['True','False','1','0']}")
                 value=bool(eval(value))
             setattr(entry,field,value)
             #as item was changed, log it in InList==True
             if field != 'InList':
                 setattr(entry,"InList",True)
+            if field != 'userUpdated':
+                setattr(entry,'userUpdated',True)
             session.commit()
             session.flush()
             session.refresh(entry)
             print(entry)
         else:
             print(entry)
             print(f"{Fore.dark_goldenrod}{Style.underline}Nothing was changed!{Style.reset}")
```

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,23 @@
 												dt["Price"]=item.Price
 												dt["Image"]=n
 												dt["Note"]=json.dumps({'Note':item.Note,'MeasurementUnit':item.MeasurementUnit})
 												dt["Size"]=f"SIZE:{dt.get('Size')}|Unit:{dt.get('SizeUnit')}"
 												if item.Tags:
 													dt["Tags"]=json.dumps(item.Tags.split(","))
 												entry=Entry(**dt)
+
+												check=session.query(Entry).filter(Entry.Barcode==entry.Barcode,Entry.Code==entry.Code).first()
+												print(check)
+												if check:
+													setattr(check,'InList',True)
+													session.commit()
+													print("A Duplicate was found added to InList==True for review!")
+												
+												#for now all duplicates will be added
 												session.add(entry)
 												if num % 100 == 0:
 													session.commit()
 												print(f'{num+1}/{len(results)}')
 											session.commit()
 									print("done importing")
 								else:
```

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,14 +351,42 @@
 				        'CHKSTND_SPLY':0,
 						})
 					session.commit()
 					session.flush()
 					print(result)
 			print("-"*10)
 			return True
+		elif args[0].lower() in ["total_entries","te","count_all",'cta']:
+			print("-"*10)
+			with Session(self.engine) as session:
+					result=session.query(Entry).all()
+					ct=len(result)
+					bcode=Fore.light_yellow
+					ccode=Fore.dark_goldenrod
+					ncode=Fore.light_red
+					cur=Fore.cyan
+					total=Fore.medium_violet_red
+					line=f"{cur}Current/{total}Total -> {bcode}Barcode | {ccode}Code | {ncode}Name{Style.reset}"
+					for num,item in enumerate(result):
+						line=f"{cur}{num}/{total}{ct} -> {bcode}{item.Barcode} | {ccode}{item.Code} | {ncode}{item.Name}{Style.reset}"
+						print(line)
+		elif args[0].lower() in ["qsl","quick_show_list",]:
+			print("-"*10)
+			with Session(self.engine) as session:
+					result=session.query(Entry).filter(Entry.InList==True).all()
+					ct=len(result)
+					bcode=Fore.light_yellow
+					ccode=Fore.dark_goldenrod
+					ncode=Fore.light_red
+					cur=Fore.cyan
+					total=Fore.medium_violet_red
+					line=f"{cur}Current/{total}Total -> {bcode}Barcode | {ccode}Code | {ncode}Name{Style.reset}"
+					for num,item in enumerate(result):
+						line=f"{cur}{num}/{total}{ct} -> {bcode}{item.Barcode} | {ccode}{item.Code} | {ncode}{item.Name}{Style.reset}"
+						print(line)
 		elif args[0].lower() in ["clear_all_img","cam","clrallimg"]:
 			print("-"*10)
 			with Session(self.engine) as session:
 					result=session.query(Entry).all()
 					for num,item in enumerate(result):
 						print(f"{Fore.red}{num} - clearing img field -> {item}")
 						if Path(item.Image).exists():
```

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,10 @@
 {Fore.green}ni|new_item{Style.reset}-{Fore.cyan}create new Entry Item{Style.reset}
 {Fore.green}le-img{Style.reset}-{Fore.cyan}export list items as png{Style.reset}
 {Fore.green}smle,s|search|?{Style.reset} - {Fore.cyan}calls a prompt to search for InList==True with CODE|BARCODE instead of direct search waits for b for back, q for quit, for next CODE|BARCODE{Style.reset}
 {Fore.green}sai0|set_all_inlist_0{Style.reset} - {Fore.cyan}set all Entry's to InList=False{Style.reset}
 {Fore.green}sai1|set_all_inlist_1{Style.reset} - {Fore.cyan}set all Entry's to InList=True{Style.reset}
 {Fore.green}import_csv{Style.reset} - {Fore.cyan}Import CSV data, must have Barcode,Code,Name headers and if other Entry Fields are specified, then those will be used too, icluding valid image paths.{Style.reset}
 {Fore.green}ie|item_editor|itm_edt{Style.reset}-{Fore.cyan}Use the Item Editor,auto-scaling for new fields when new fields are added!{Style.reset}
-{Fore.green}export_list_field|elf{Style.reset}-{Fore.cyan}Export specified field to QREncoded Img from Entry.InList==True{Style.reset}
+{Fore.green}export_list_field|elf{Style.reset}-{Fore.cyan}Export specified field to QREncoded Img from Entry.InList==True{Style.reset}
+{Fore.green}total_entries|te|count_all|cta{Style.reset}-{Fore.cyan}count all Entry's{Style.reset}
+{Fore.green}qsl|quick_show_list{Style.reset}-{Fore.cyan}Briefly display list contents{Style.reset}
```

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.46
+Version: 0.4.47
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+Requires-Dist: cython
 Requires-Dist: pint
 Requires-Dist: pyupc-ean
 Requires-Dist: openpyxl
 Requires-Dist: plyer
 Requires-Dist: colored
 Requires-Dist: numpy
 Requires-Dist: pandas
```

### Comparing `MobileInventoryCLI-0.4.46/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.47/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.46/PKG-INFO` & `MobileInventoryCLI-0.4.47/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.46
+Version: 0.4.47
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+Requires-Dist: cython
 Requires-Dist: pint
 Requires-Dist: pyupc-ean
 Requires-Dist: openpyxl
 Requires-Dist: plyer
 Requires-Dist: colored
 Requires-Dist: numpy
 Requires-Dist: pandas
```

### Comparing `MobileInventoryCLI-0.4.46/setup.py` & `MobileInventoryCLI-0.4.47/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.46'
+version='0.4.47'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
 
           ],
       packages=find_packages(),
       python_requires='>=3.6',
-      install_requires=['pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder'],
+      install_requires=['cython','pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder'],
       package_data={
         '':["*.config","*.txt","*.README","*.TTF"],
         }
       )
```

