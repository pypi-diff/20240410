# Comparing `tmp/Velkoz-0.0.4.tar.gz` & `tmp/Velkoz-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.4.tar", last modified: Wed Apr 10 19:41:28 2024, max compression
+gzip compressed data, was "Velkoz-0.0.41.tar", last modified: Wed Apr 10 19:46:14 2024, max compression
```

## Comparing `Velkoz-0.0.4.tar` & `Velkoz-0.0.41.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.600631 Velkoz-0.0.4/
--rw-rw-rw-   0        0        0      670 2024-04-10 19:41:28.599632 Velkoz-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.554270 Velkoz-0.0.4/Velkoz/
--rw-rw-rw-   0        0        0      346 2024-03-21 19:18:50.000000 Velkoz-0.0.4/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.589448 Velkoz-0.0.4/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.4/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.4/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.4/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.4/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-06 09:20:19.000000 Velkoz-0.0.4/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.4/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     1159 2024-04-10 19:41:05.000000 Velkoz-0.0.4/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.592616 Velkoz-0.0.4/Velkoz/supp/
--rw-rw-rw-   0        0        0      129 2024-04-05 19:15:06.000000 Velkoz-0.0.4/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      587 2024-04-10 19:31:43.000000 Velkoz-0.0.4/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0     1133 2024-04-10 19:40:41.000000 Velkoz-0.0.4/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      258 2024-04-05 19:15:09.000000 Velkoz-0.0.4/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1667 2024-04-05 19:15:09.000000 Velkoz-0.0.4/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.597633 Velkoz-0.0.4/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.4/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.4/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-10 19:40:42.000000 Velkoz-0.0.4/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4505 2024-04-06 09:36:14.000000 Velkoz-0.0.4/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.4/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.4/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.4/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     5364 2024-04-10 19:40:41.000000 Velkoz-0.0.4/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.598632 Velkoz-0.0.4/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      670 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 19:41:28.600631 Velkoz-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 19:46:14.818576 Velkoz-0.0.41/
+-rw-rw-rw-   0        0        0      671 2024-04-10 19:46:14.817573 Velkoz-0.0.41/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 19:46:14.767210 Velkoz-0.0.41/Velkoz/
+-rw-rw-rw-   0        0        0      346 2024-03-21 19:18:50.000000 Velkoz-0.0.41/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:46:14.799004 Velkoz-0.0.41/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.41/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.41/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.41/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.41/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-06 09:20:19.000000 Velkoz-0.0.41/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.41/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     1160 2024-04-10 19:45:49.000000 Velkoz-0.0.41/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:46:14.807557 Velkoz-0.0.41/Velkoz/supp/
+-rw-rw-rw-   0        0        0      129 2024-04-05 19:15:06.000000 Velkoz-0.0.41/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-04-10 19:45:34.000000 Velkoz-0.0.41/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0     1135 2024-04-10 19:45:27.000000 Velkoz-0.0.41/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      260 2024-04-10 19:45:19.000000 Velkoz-0.0.41/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1669 2024-04-10 19:45:11.000000 Velkoz-0.0.41/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:46:14.815576 Velkoz-0.0.41/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.41/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.41/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-10 19:40:42.000000 Velkoz-0.0.41/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4505 2024-04-06 09:36:14.000000 Velkoz-0.0.41/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.41/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.41/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.41/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     5364 2024-04-10 19:40:41.000000 Velkoz-0.0.41/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:46:14.816574 Velkoz-0.0.41/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      671 2024-04-10 19:46:14.000000 Velkoz-0.0.41/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2024-04-10 19:46:14.000000 Velkoz-0.0.41/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 19:46:14.000000 Velkoz-0.0.41/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 19:46:14.000000 Velkoz-0.0.41/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 19:46:14.000000 Velkoz-0.0.41/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 19:46:14.818576 Velkoz-0.0.41/setup.cfg
```

### Comparing `Velkoz-0.0.4/PKG-INFO` & `Velkoz-0.0.41/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.4
+Version: 0.0.41
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `Velkoz-0.0.4/Velkoz/eye/account.py` & `Velkoz-0.0.41/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/eye/champion_mastery.py` & `Velkoz-0.0.41/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/eye/match.py` & `Velkoz-0.0.41/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/eye/summoner.py` & `Velkoz-0.0.41/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/setup.py` & `Velkoz-0.0.41/Velkoz/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.4' 
+VERSION = '0.0.41' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
```

### Comparing `Velkoz-0.0.4/Velkoz/supp/account.py` & `Velkoz-0.0.41/Velkoz/supp/account.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from tentacles import (
+from .tentacles import (
     AccountApi
 
         )
 
-from eye import (
+from .eye import (
     Account
         )
 
 
 ###############
 # Get Account #
 ###############
```

### Comparing `Velkoz-0.0.4/Velkoz/supp/champion_mastery.py` & `Velkoz-0.0.41/Velkoz/supp/champion_mastery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-from tentacles import (ChampionMasteryApi)
+from .tentacles import (ChampionMasteryApi)
 
-from eye import (ChampionMastery)
+from .eye import (ChampionMastery)
 
 
 def _get_all_masteries_by_puuid(service, puuid:str, region:str = 'euw1'):
     parameters = {'puuid':puuid, 'region':region}
     championMasteryDto = ChampionMasteryApi.get_all_masteries(parameters)
     return championMasteryDto
```

### Comparing `Velkoz-0.0.4/Velkoz/supp/summoner.py` & `Velkoz-0.0.41/Velkoz/supp/summoner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # DO NOT FORGET THE DOTS!!!!!!
-from tentacles import (SummonerApi, RiotApiService, api_key) 
+from .tentacles import (SummonerApi, RiotApiService, api_key) 
 
-from eye import Summoner
+from .eye import Summoner
 
 #service = RiotApiService(api_key)
 
 
 def _get_summonerDto_by_account(service, account:dict, region:str = 'euw1'):
     parameters = {'puuid' : account['puuid'], 'region': region}
     summonerDto = SummonerApi.get_summoner(service, parameters)
```

### Comparing `Velkoz-0.0.4/Velkoz/tentacles/account.py` & `Velkoz-0.0.41/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.41/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/tentacles/common.py` & `Velkoz-0.0.41/Velkoz/tentacles/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/tentacles/match.py` & `Velkoz-0.0.41/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.41/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz/velkoz.py` & `Velkoz-0.0.41/Velkoz/velkoz.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.4/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.41/Velkoz.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.4
+Version: 0.0.41
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `Velkoz-0.0.4/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.0.41/Velkoz.egg-info/SOURCES.txt`

 * *Files identical despite different names*
