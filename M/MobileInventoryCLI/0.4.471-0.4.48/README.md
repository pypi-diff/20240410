# Comparing `tmp/MobileInventoryCLI-0.4.471.tar.gz` & `tmp/MobileInventoryCLI-0.4.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.471.tar", last modified: Tue Apr  9 14:53:31 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.48.tar", last modified: Tue Apr  9 17:38:09 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.471.tar` & `MobileInventoryCLI-0.4.48.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.716521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.719854 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.719854 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.719854 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   103215 2024-04-09 14:53:18.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.723188 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    26852 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 14:53:28.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5301 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-09 14:33:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      714 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      714 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-09 14:53:31.726521 MobileInventoryCLI-0.4.471/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      820 2024-04-09 14:53:31.000000 MobileInventoryCLI-0.4.471/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.716735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.716735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   103952 2024-04-09 17:36:29.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.720069 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28296 2024-04-09 17:20:02.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-09 17:38:02.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      903 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-09 17:21:27.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.723402 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-09 14:53:40.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-09 17:38:09.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-09 17:38:09.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-09 17:38:09.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-09 17:38:09.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-09 17:38:09.000000 MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      713 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-09 17:38:09.726735 MobileInventoryCLI-0.4.48/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      819 2024-04-09 17:38:09.000000 MobileInventoryCLI-0.4.48/setup.py
```

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -782,58 +782,60 @@
         except Exception as e:
             return ''
 
     def __repr__(self):
         total_value=self.total_value(CaseMode=False)
         total_value_case=self.total_value()
         m= f"""
-{Style.bold}{Style.underline}{Fore.pale_green_1b}Entry{Style.reset}(
-{Fore.light_magenta}UserUpdated={self.userUpdated}{Style.reset},
-{Fore.hot_pink_2}{Style.bold}{Style.underline}EntryId{Style.reset}={self.EntryId}
-{Fore.violet}{Style.underline}Code{Style.reset}='{self.Code}',
-{Fore.orange_3}{Style.bold}Barcode{Style.reset}='{self.Barcode}',
-{Fore.orange_3}{Style.underline}UPCE from UPCA[if any]{Style.reset}='{self.upce2upca}',
-{Fore.green}{Style.bold}Price{Style.reset}=${self.Price},
-{Fore.green}{Style.bold}CRV{Style.reset}=${self.CRV},
-{Fore.green}{Style.bold}Tax{Style.reset}=${self.Tax},
-{Fore.green}{Style.bold}TaxNote{Style.reset}='{self.TaxNote}',
-{Fore.red}Name{Style.reset}='{self.Name}',
-{Fore.tan}Note{Style.reset}='{self.Note}',
-{Fore.grey_50}ALT_Barcode{Style.reset}={Fore.grey_70}{self.ALT_Barcode}{Style.reset}
-{Fore.grey_50}DUP_Barcode{Style.reset}={Fore.grey_70}{self.DUP_Barcode}{Style.reset}
-{Fore.grey_50}CaseID_BR{Style.reset}={Fore.grey_70}{self.CaseID_BR}{Style.reset}
-{Fore.grey_50}CaseID_LD{Style.reset}={Fore.grey_70}{self.CaseID_LD}{Style.reset}
-{Fore.grey_50}CaseID_6W{Style.reset}={Fore.grey_70}{self.CaseID_6W}{Style.reset}
-{Fore.grey_50}Tags{Style.reset}={Fore.grey_70}{self.Tags}{Style.reset}
-{Fore.grey_50}Facings{Style.reset}={Fore.grey_70}{self.Facings}{Style.reset}
-{Fore.pale_green_1b}Timestamp{Style.reset}='{datetime.fromtimestamp(self.Timestamp).strftime('%D@%H:%M:%S')}',
-{Fore.deep_pink_3b}Shelf{Style.reset}={self.Shelf},
-{Fore.light_steel_blue}BackRoom{Style.reset}={self.BackRoom},
-{Fore.cyan}Display_1{Style.reset}={self.Display_1},
-{Fore.cyan}Display_2{Style.reset}={self.Display_2},
-{Fore.cyan}Display_3{Style.reset}={self.Display_3},
-{Fore.cyan}Display_4{Style.reset}={self.Display_4},
-{Fore.cyan}Display_5{Style.reset}={self.Display_5},
-{Fore.cyan}Display_6{Style.reset}={self.Display_6},
-{Fore.cyan}SBX_WTR_DSPLY{Style.reset}={Fore.pale_green_1b}{self.SBX_WTR_DSPLY}{Style.reset}
-{Fore.cyan}SBX_CHP_DSPLY{Style.reset}={Fore.pale_green_1b}{self.SBX_CHP_DSPLY}{Style.reset}
-{Fore.cyan}SBX_WTR_KLR{Style.reset}={Fore.pale_green_1b}{self.SBX_WTR_KLR}{Style.reset}
-{Fore.violet}FLRL_CHP_DSPLY{Style.reset}={Fore.green_yellow}{self.FLRL_CHP_DSPLY}{Style.reset}
-{Fore.violet}FLRL_WTR_DSPLY{Style.reset}={Fore.green_yellow}{self.FLRL_WTR_DSPLY}{Style.reset}
-{Fore.grey_50}WD_DSPLY{Style.reset}={self.WD_DSPLY}{Style.reset}
-{Fore.grey_50}CHKSTND_SPLY{Style.reset}={self.CHKSTND_SPLY}{Style.reset}
-{Fore.light_salmon_3a}Stock_Total{Style.reset}={self.Stock_Total},
-{Fore.magenta_3c}InList{Style.reset}={self.InList}
-{Fore.indian_red_1b}{Style.bold}{Style.underline}{Style.blink}ListQty{Style.reset}={self.ListQty}
-{Fore.misty_rose_3}Location{Style.reset}={self.Location}
-{Fore.sky_blue_2}CaseCount{Style.reset}={self.CaseCount}
-{Fore.sky_blue_2}Size{Style.reset}={self.Size}
-{Fore.tan}Image[{Fore.dark_goldenrod}Exists:{Fore.deep_pink_3b}{self.imageExists()}{Style.reset}{Fore.tan}]{Style.reset}={self.Image}
-{Fore.medium_violet_red}Total Product Handled/To Be Handled Value: {Fore.spring_green_3a}{total_value}{Style.reset}
-{Fore.medium_violet_red}Total Product Handled/To Be Handled Value*CaseCount: {Fore.spring_green_3a}{total_value_case}{Style.reset}"""
+        {Style.bold}{Style.underline}{Fore.pale_green_1b}Entry{Style.reset}(
+        {Fore.light_magenta}UserUpdated={self.userUpdated}{Style.reset},
+        {Fore.hot_pink_2}{Style.bold}{Style.underline}EntryId{Style.reset}={self.EntryId}
+        {Fore.violet}{Style.underline}Code{Style.reset}='{self.Code}',
+        {Fore.orange_3}{Style.bold}Barcode{Style.reset}='{self.Barcode}',
+        {Fore.orange_3}{Style.underline}UPCE from UPCA[if any]{Style.reset}='{self.upce2upca}',
+        {Fore.green}{Style.bold}Price{Style.reset}=${self.Price},
+        {Fore.green}{Style.bold}CRV{Style.reset}=${self.CRV},
+        {Fore.green}{Style.bold}Tax{Style.reset}=${self.Tax},
+        {Fore.green}{Style.bold}TaxNote{Style.reset}='{self.TaxNote}',
+        {Fore.red}Name{Style.reset}='{self.Name}',
+        {Fore.tan}Note{Style.reset}='{self.Note}',
+        {Fore.grey_50}ALT_Barcode{Style.reset}={Fore.grey_70}{self.ALT_Barcode}{Style.reset}
+        {Fore.grey_50}DUP_Barcode{Style.reset}={Fore.grey_70}{self.DUP_Barcode}{Style.reset}
+        {Fore.grey_50}CaseID_BR{Style.reset}={Fore.grey_70}{self.CaseID_BR}{Style.reset}
+        {Fore.grey_50}CaseID_LD{Style.reset}={Fore.grey_70}{self.CaseID_LD}{Style.reset}
+        {Fore.grey_50}CaseID_6W{Style.reset}={Fore.grey_70}{self.CaseID_6W}{Style.reset}
+        {Fore.grey_50}Tags{Style.reset}={Fore.grey_70}{self.Tags}{Style.reset}
+        {Fore.grey_50}Facings{Style.reset}={Fore.grey_70}{self.Facings}{Style.reset}
+        {Fore.pale_green_1b}Timestamp{Style.reset}='{datetime.fromtimestamp(self.Timestamp).strftime('%D@%H:%M:%S')}',
+        {Fore.deep_pink_3b}Shelf{Style.reset}={self.Shelf},
+        {Fore.light_steel_blue}BackRoom{Style.reset}={self.BackRoom},
+        {Fore.cyan}Display_1{Style.reset}={self.Display_1},
+        {Fore.cyan}Display_2{Style.reset}={self.Display_2},
+        {Fore.cyan}Display_3{Style.reset}={self.Display_3},
+        {Fore.cyan}Display_4{Style.reset}={self.Display_4},
+        {Fore.cyan}Display_5{Style.reset}={self.Display_5},
+        {Fore.cyan}Display_6{Style.reset}={self.Display_6},
+        {Fore.cyan}SBX_WTR_DSPLY{Style.reset}={Fore.pale_green_1b}{self.SBX_WTR_DSPLY}{Style.reset}
+        {Fore.cyan}SBX_CHP_DSPLY{Style.reset}={Fore.pale_green_1b}{self.SBX_CHP_DSPLY}{Style.reset}
+        {Fore.cyan}SBX_WTR_KLR{Style.reset}={Fore.pale_green_1b}{self.SBX_WTR_KLR}{Style.reset}
+        {Fore.violet}FLRL_CHP_DSPLY{Style.reset}={Fore.green_yellow}{self.FLRL_CHP_DSPLY}{Style.reset}
+        {Fore.violet}FLRL_WTR_DSPLY{Style.reset}={Fore.green_yellow}{self.FLRL_WTR_DSPLY}{Style.reset}
+        {Fore.grey_50}WD_DSPLY{Style.reset}={self.WD_DSPLY}{Style.reset}
+        {Fore.grey_50}CHKSTND_SPLY{Style.reset}={self.CHKSTND_SPLY}{Style.reset}
+        {Fore.light_salmon_3a}Stock_Total{Style.reset}={self.Stock_Total},
+        {Fore.magenta_3c}InList{Style.reset}={self.InList}
+        {Fore.indian_red_1b}{Style.bold}{Style.underline}{Style.blink}ListQty{Style.reset}={self.ListQty}
+        {Fore.misty_rose_3}Location{Style.reset}={self.Location}
+        {Fore.sky_blue_2}CaseCount{Style.reset}={self.CaseCount}
+        {Fore.sky_blue_2}Size{Style.reset}={self.Size}
+        {Fore.tan}Image[{Fore.dark_goldenrod}Exists:{Fore.deep_pink_3b}{self.imageExists()}{Style.reset}{Fore.tan}]{Style.reset}={self.Image}
+        {Fore.slate_blue_1}{Style.underline}{'-'*5}{Style.reset}{Style.bold} Short Data {Style.reset}{Fore.slate_blue_1}{Style.underline}{'-'*5}{Style.reset}
+        {Fore.light_yellow}{self.Name} ({Fore.light_magenta}{self.Barcode}[{Fore.spring_green_3a}UPC{Style.reset}{Fore.light_magenta}]:{Fore.light_red}{self.Code}[{Fore.orange_red_1}SHELF/TAG/CIC]{Fore.light_red}){Style.reset}
+        {Fore.medium_violet_red}Total Product Handled/To Be Handled Value: {Fore.spring_green_3a}{total_value}{Style.reset}
+        {Fore.medium_violet_red}Total Product Handled/To Be Handled Value*CaseCount: {Fore.spring_green_3a}{total_value_case}{Style.reset}"""
         if self.imageExists():
             m+=f"""
         {Fore.green}Image {Fore.orange_3}{Style.bold}{Style.underline}ABSOLUTE{Style.reset}{Style.reset}={Path(self.Image).absolute()}"""
 
         m+="""
         )
         """
```

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 3% similar despite different names*

```diff
@@ -611,14 +611,40 @@
 					print(f"{Fore.green}{num+1}{Style.reset}/{Fore.red}{ct}{Style.reset}")
 					r.InList=True
 					if num % 100 == 0:
 						session.commit()
 				session.commit()
 				session.flush()
 			return True
+		elif args[0].lower() in ['set_all_userUpdated_1','sau1']:
+			with Session(self.engine) as session:
+				result=session.query(Entry).all()
+				ct=len(result)
+				for num,r in enumerate(result):
+					print(f"{Fore.green}{num+1}{Style.reset}/{Fore.red}{ct}{Style.reset}")
+					r.userUpdated=True
+					if num % 100 == 0:
+						session.commit()
+				session.commit()
+				session.flush()
+			return True
+		elif args[0].lower() in ['list_all_userUpdated_1','lau1']:
+			with Session(self.engine) as session:
+				result=session.query(Entry).filter(Entry.userUpdated==True).all()
+				ct=len(result)
+				for num,r in enumerate(result):
+					print(f"{Fore.green}{num}{Style.reset}/{Fore.red}{ct}{Style.reset} -> {r}")	
+			return True
+		elif args[0].lower() in ['list_all_userUpdated_0','lau0']:
+			with Session(self.engine) as session:
+				result=session.query(Entry).filter(Entry.userUpdated==False).all()
+				ct=len(result)
+				for num,r in enumerate(result):
+					print(f"{Fore.green}{num}{Style.reset}/{Fore.red}{ct}{Style.reset} -> {r}")	
+			return True
 		elif args[0].lower() in ['ts','touchstamp']:
 			self.ts=TouchStampC(engine=self.engine,parent=self)
 		elif args[0].lower() in ['import_csv']:
 			def import_csv_lcl(codefile,self):
 				codefile_path=Path(codefile)
 				if codefile_path.exists() and codefile_path.is_file():	
 					with Session(self.engine) as session:
@@ -658,14 +684,26 @@
 					r.InList=False
 					r.ListQty=0
 					if num % 100 == 0:
 						session.commit()
 				session.commit()
 				session.flush()
 			return True
+		elif args[0].lower() in ['set_all_userUpdated_0','sau0']:
+			with Session(self.engine) as session:
+				result=session.query(Entry).all()
+				ct=len(result)
+				for num,r in enumerate(result):
+					print(f"{Fore.green}{num+1}{Style.reset}/{Fore.red}{ct}{Style.reset}")
+					r.userUpdated=False
+					if num % 100 == 0:
+						session.commit()
+				session.commit()
+				session.flush()
+			return True
 		elif args[0].lower() in ['export_list','el']:
 			ExportListCSV(parent=self,engine=self.engine)
 		elif args[0].lower() in ['ie','item_editor','itm_edt']:
 			editor=EntrySet(engine=self.engine,parent=self)
 		elif args[0].lower() in ['ni','new_item']:
 			while True:
 				try:
```

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,12 +32,16 @@
 {Fore.green}location|geo|lctn|ln|l,$code{Style.reset}-{Fore.cyan}print location finding data for $code{Style.reset}
 {Fore.green}smle-e{Style.reset}-{Fore.cyan}save list items as png{Style.reset}
 {Fore.green}ni|new_item{Style.reset}-{Fore.cyan}create new Entry Item{Style.reset}
 {Fore.green}le-img{Style.reset}-{Fore.cyan}export list items as png{Style.reset}
 {Fore.green}smle,s|search|?{Style.reset} - {Fore.cyan}calls a prompt to search for InList==True with CODE|BARCODE instead of direct search waits for b for back, q for quit, for next CODE|BARCODE{Style.reset}
 {Fore.green}sai0|set_all_inlist_0{Style.reset} - {Fore.cyan}set all Entry's to InList=False{Style.reset}
 {Fore.green}sai1|set_all_inlist_1{Style.reset} - {Fore.cyan}set all Entry's to InList=True{Style.reset}
+{Fore.green}sau0|set_all_userUpdated_0{Style.reset} - {Fore.cyan}set all Entry's to userUpdated=False{Style.reset}
+{Fore.green}sau1|set_all_userUpdated_1{Style.reset} - {Fore.cyan}set all Entry's to userUpdated=True{Style.reset}
+{Fore.green}lau0|list_all_userUpdated_0{Style.reset} - {Fore.cyan}list all Entry's with userUpdated=False{Style.reset}
+{Fore.green}lau1|list_all_userUpdated_1{Style.reset} - {Fore.cyan}list all Entry's with userUpdated=True{Style.reset}
 {Fore.green}import_csv{Style.reset} - {Fore.cyan}Import CSV data, must have Barcode,Code,Name headers and if other Entry Fields are specified, then those will be used too, icluding valid image paths.{Style.reset}
 {Fore.green}ie|item_editor|itm_edt{Style.reset}-{Fore.cyan}Use the Item Editor,auto-scaling for new fields when new fields are added!{Style.reset}
 {Fore.green}export_list_field|elf{Style.reset}-{Fore.cyan}Export specified field to QREncoded Img from Entry.InList==True{Style.reset}
 {Fore.green}total_entries|te|count_all|cta{Style.reset}-{Fore.cyan}count all Entry's{Style.reset}
 {Fore.green}qsl|quick_show_list{Style.reset}-{Fore.cyan}Briefly display list contents{Style.reset}
```

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.471
+Version: 0.4.48
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.471/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.48/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.471/PKG-INFO` & `MobileInventoryCLI-0.4.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.471
+Version: 0.4.48
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.471/setup.py` & `MobileInventoryCLI-0.4.48/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.471'
+version='0.4.48'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

