# Comparing `tmp/PKNSETools-0.1.20240309.83.tar.gz` & `tmp/PKNSETools-0.1.20240410.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240309.83.tar", last modified: Sat Mar  9 08:23:19 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240410.84.tar", last modified: Wed Apr 10 20:29:58 2024, max compression
```

## Comparing `PKNSETools-0.1.20240309.83.tar` & `PKNSETools-0.1.20240410.84.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/
--rw-rw-rw-   0        0        0     2661 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-09 08:23:19.031908 PKNSETools-0.1.20240309.83/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3392 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    12458 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-03-09 08:23:13.000000 PKNSETools-0.1.20240309.83/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    60249 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    21951 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29930 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-03-09 08:23:19.000000 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-03-09 08:23:19.000000 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 08:23:19.000000 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-09 08:23:12.000000 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-03-09 08:23:19.000000 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-09 08:23:19.000000 PKNSETools-0.1.20240309.83/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/README.md
--rw-rw-rw-   0        0        0       86 2024-03-09 08:23:19.047516 PKNSETools-0.1.20240309.83/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-03-09 08:22:19.000000 PKNSETools-0.1.20240309.83/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:29:58.601948 PKNSETools-0.1.20240410.84/
+-rw-rw-rw-   0        0        0     2661 2024-04-10 20:29:58.601948 PKNSETools-0.1.20240410.84/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 20:29:58.586325 PKNSETools-0.1.20240410.84/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-04-10 20:29:58.586325 PKNSETools-0.1.20240410.84/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:29:58.586325 PKNSETools-0.1.20240410.84/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3392 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0     6446 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    12458 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-04-10 20:29:53.000000 PKNSETools-0.1.20240410.84/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:29:58.601948 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61965 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    21951 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29930 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:29:58.586325 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-04-10 20:29:58.000000 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-04-10 20:29:58.000000 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 20:29:58.000000 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 20:29:52.000000 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-04-10 20:29:58.000000 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 20:29:58.000000 PKNSETools-0.1.20240410.84/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-10 20:29:58.601948 PKNSETools-0.1.20240410.84/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-04-10 20:28:01.000000 PKNSETools-0.1.20240410.84/setup.py
```

### Comparing `PKNSETools-0.1.20240309.83/PKG-INFO` & `PKNSETools-0.1.20240410.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240309.83
+Version: 0.1.20240410.84
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240309.83.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240410.84.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240410.84/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240410.84/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240410.84/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240410.84/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKMultiProcessorClient.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240410.84/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
+from PKDevTools.classes.CookieHelper import CookieHelper
+from PKDevTools.classes import Archiver
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.Fetcher import fetcher
 from PKDevTools.classes.log import default_logger
 from PKNSETools.morningstartools.stock import Stock
 from PKDevTools.classes.Utils import random_user_agent
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 # This Class Handles Fetching of Stock Data over the internet from NSE/BSE
@@ -286,21 +288,55 @@
             )
             output.set_index("Stock", inplace=True)
             return output
         except Exception as e:
             pass
         return None
 
+    def refreshBobCapsTokens(self):
+        default_headers = {
+            "Accept-Encoding": "gzip, deflate, br, zstd",
+            "Accept-Language": "en-US,en;q=0.9",
+            "DNT": "1",
+            "Host": "www.barodaetrade.com",
+            "Referer": "https://www.barodaetrade.com/Markettracker/Dividend_Declared",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": random_user_agent()
+        }
+        cookieHelper = CookieHelper(download_folder=Archiver.get_user_outputs_dir(),
+                                                 baseCookieUrl="https://www.barodaetrade.com/Markettracker/Dividend_Declared",
+                                                 cookieStoreName="bobcaps",
+                                                 baseHtmlUrl="https://www.barodaetrade.com/Markettracker/Dividend_Declared",
+                                                 htmlStoreName="bobcaps")
+        self.session.headers.update(default_headers)
+        self.session.cookies.update(cookieHelper.cookies)
+
     def getCorporateActions(self):
-        dividends_dfs = pd.read_html("https://www.barodaetrade.com/Markettracker/Dividend_Declared")
-        bonus_dfs = pd.read_html("https://www.barodaetrade.com/Markettracker/Bonous_Issue")
-        stockSplit_dfs = pd.read_html("https://www.barodaetrade.com/Markettracker/Stock_Split")
-        dividends_df = dividends_dfs[1]
-        bonus_df = bonus_dfs[1]
-        stockSplit_df = stockSplit_dfs[1]
+        self.refreshBobCapsTokens()
+        dividends_df = pd.DataFrame([{"Company Name":""}])
+        bonus_df = pd.DataFrame([{"Company Name":""}])
+        stockSplit_df = pd.DataFrame([{"Company Name":""}])
+        try:
+            dividend_html = self.fetchURL("https://www.barodaetrade.com/Markettracker/Dividend_Declared")
+            dividends_dfs = pd.read_html(dividend_html.text)
+            dividends_df = dividends_dfs[1]
+        except:
+            pass
+        try:
+            bonus_html = self.fetchURL("https://www.barodaetrade.com/Markettracker/Bonous_Issue")
+            bonus_dfs = pd.read_html(bonus_html.text)
+            bonus_df = bonus_dfs[1]
+        except:
+            pass
+        try:
+            stockSplit_html = self.fetchURL("https://www.barodaetrade.com/Markettracker/Stock_Split")
+            stockSplit_dfs = pd.read_html(stockSplit_html.text)
+            stockSplit_df = stockSplit_dfs[1]
+        except:
+            pass
         dfs = [dividends_df,bonus_df,stockSplit_df]
         dateColumns = ["Record","Div.Date","Split","Announced"]
         for df in dfs:
             df.rename(
                     columns={
                         "Company Name": "Stock",
                         "Dividend Type": "Div.Type",
```

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240410.84/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240410.84/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240309.83
+Version: 0.1.20240410.84
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240309.83.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240410.84.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240309.83/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240410.84/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/README.md` & `PKNSETools-0.1.20240410.84/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240309.83/setup.py` & `PKNSETools-0.1.20240410.84/setup.py`

 * *Files identical despite different names*

