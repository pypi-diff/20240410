# Comparing `tmp/limexhub-0.1.6.tar.gz` & `tmp/limexhub-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limexhub-0.1.6.tar", last modified: Tue Apr  9 16:06:46 2024, max compression
+gzip compressed data, was "limexhub-0.1.7.tar", last modified: Wed Apr 10 10:27:41 2024, max compression
```

## Comparing `limexhub-0.1.6.tar` & `limexhub-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 16:06:46.304426 limexhub-0.1.6/
--rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.6/LICENSE
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 16:06:46.304313 limexhub-0.1.6/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.6/README.md
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 16:06:46.303541 limexhub-0.1.6/limexhub/
--rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.6/limexhub/__init__.py
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2944 2024-04-09 16:06:37.000000 limexhub-0.1.6/limexhub/restapi.py
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 16:06:46.304150 limexhub-0.1.6/limexhub.egg-info/
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/SOURCES.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/dependency_links.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/requires.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/top_level.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-09 16:06:46.304468 limexhub-0.1.6/setup.cfg
--rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-09 14:38:32.000000 limexhub-0.1.6/setup.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-10 10:27:41.579256 limexhub-0.1.7/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.7/LICENSE
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-10 10:27:41.579122 limexhub-0.1.7/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.7/README.md
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-10 10:27:41.578172 limexhub-0.1.7/limexhub/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.7/limexhub/__init__.py
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     3372 2024-04-10 10:26:49.000000 limexhub-0.1.7/limexhub/restapi.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-10 10:27:41.578937 limexhub-0.1.7/limexhub.egg-info/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-10 10:27:41.000000 limexhub-0.1.7/limexhub.egg-info/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-10 10:27:41.000000 limexhub-0.1.7/limexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-10 10:27:41.000000 limexhub-0.1.7/limexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-10 10:27:41.000000 limexhub-0.1.7/limexhub.egg-info/requires.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-10 10:27:41.000000 limexhub-0.1.7/limexhub.egg-info/top_level.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-10 10:27:41.579298 limexhub-0.1.7/setup.cfg
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-10 10:26:58.000000 limexhub-0.1.7/setup.py
```

### Comparing `limexhub-0.1.6/LICENSE` & `limexhub-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.6/PKG-INFO` & `limexhub-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple API wrapper for Limex DataHub
 Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `limexhub-0.1.6/README.md` & `limexhub-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.6/limexhub/restapi.py` & `limexhub-0.1.7/limexhub/restapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 import pandas as pd
 from typing import Optional,Dict
+from datetime import datetime
+
  
 class RestAPI:
     def __init__(self, base_url="https://hub.limex.com/v1", token=None):
         self.base_url = base_url
         self.token = token
  
     def _get(self, endpoint, params: Dict):
@@ -14,58 +16,58 @@
         return response.json()
 
     def instruments(self, assets=None):
         endpoint = "instruments"
         params = {'assets': assets}
         return pd.DataFrame(self._get(endpoint, params=params))
    
-    def candles(self, symbol, from_date, timeframe):
+    def candles(self, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d'), timeframe=3):
         endpoint = "candles"
-        params = {'symbol': symbol, 'from': from_date, 'timeframe': timeframe}
+        params = {'symbol': symbol, 'from': from_date, 'to': to_date, 'timeframe': timeframe}
         res = pd.DataFrame(self._get(endpoint, params=params))
         if timeframe>=3:
             res['ts'] = pd.to_datetime(res['ts'], utc=True).dt.date
         else:
             res['ts'] = pd.to_datetime(res['ts'], utc=True)
-        return res
+        return res.sort_values(by=['ts'])
    
-    def fundamental(self, symbol, to_date, from_date, fields):
+    def fundamental(self, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d'), fields='ebitda'):
         endpoint = "fundamental"
-        params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'fields': fields}
+        params = {'symbol': symbol, 'from': from_date,'to': to_date, 'fields': fields}
         res = pd.DataFrame(self._get(endpoint, params=params))
         res['date'] = pd.to_datetime(res['date'], utc=True).dt.date
         return res
    
-    def news(self, symbol, to_date, from_date):
+    def news(self, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d')):
         endpoint = "news"
-        params = {'symbol': symbol, 'to': to_date, 'from': from_date}
+        params = {'symbol': symbol, 'from': from_date,'to': to_date}
         res = pd.DataFrame(self._get(endpoint, params=params))
         res['created'] = pd.to_datetime(res['created'], utc=True)
         return res
    
-    def events(self, symbol, to_date, from_date, event_type):
+    def events(self, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d'), event_type='dividends'):
         endpoint = "events"
-        params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'type': event_type}
+        params = {'symbol': symbol, 'from': from_date, 'to': to_date,'type': event_type}
         res = pd.DataFrame(self._get(endpoint, params=params))
         res['buy_date'] = pd.to_datetime(res['buy_date'], utc=True).dt.date
         return res
    
-    def signals(self, vendor, model, symbol, from_date):
+    def signals(self, vendor, model, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d')):
         endpoint = "signals"
-        params = {'vendor': vendor, 'model': model, 'symbol': symbol, 'from': from_date}
+        params = {'vendor': vendor, 'model': model, 'symbol': symbol, 'from': from_date,'to': to_date}
         res = pd.DataFrame(self._get(endpoint, params=params))
         res['trade_date'] = pd.to_datetime(res['trade_date'], utc=True).dt.date
         return res
  
-    def models(self, vendor):
+    def models(self, vendor='boosted'):
         endpoint = "models"
         params = {'vendor': vendor}
         return self._get(endpoint, params=params)
 
-    def altercandles(self, symbol, to_date, from_date, timeframe):
+    def candles(self, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d'), timeframe=3):
         endpoint = "altercandles"
         params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'timeframe': timeframe}
         res = pd.DataFrame(self._get(endpoint, params=params))
         if timeframe>=3:
             res['ts'] = pd.to_datetime(res['ts'], utc=True).dt.date
         else:
             res['ts'] = pd.to_datetime(res['ts'], utc=True)
```

### Comparing `limexhub-0.1.6/limexhub.egg-info/PKG-INFO` & `limexhub-0.1.7/limexhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple API wrapper for Limex DataHub
 Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `limexhub-0.1.6/setup.py` & `limexhub-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='limexhub',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     include_package_data=True,
     description='A simple API wrapper for Limex DataHub',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Limex-com/limexhub-python',
     author='V.Arbuzov',
```

