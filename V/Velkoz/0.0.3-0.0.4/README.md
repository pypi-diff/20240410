# Comparing `tmp/Velkoz-0.0.3.tar.gz` & `tmp/Velkoz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.3.tar", last modified: Fri Mar 22 11:09:07 2024, max compression
+gzip compressed data, was "Velkoz-0.0.4.tar", last modified: Wed Apr 10 19:41:28 2024, max compression
```

## Comparing `Velkoz-0.0.3.tar` & `Velkoz-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 11:09:07.954409 Velkoz-0.0.3/
--rw-rw-rw-   0        0        0      670 2024-03-22 11:09:07.954409 Velkoz-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-22 11:09:07.886728 Velkoz-0.0.3/Velkoz/
--rw-rw-rw-   0        0        0      346 2024-03-21 19:18:50.000000 Velkoz-0.0.3/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 11:09:07.937705 Velkoz-0.0.3/Velkoz/eye/
--rw-rw-rw-   0        0        0      103 2024-03-21 19:18:34.000000 Velkoz-0.0.3/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-03-21 22:30:39.000000 Velkoz-0.0.3/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0        8 2024-03-18 23:45:29.000000 Velkoz-0.0.3/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7061 2024-03-21 22:30:39.000000 Velkoz-0.0.3/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1966 2024-03-21 00:27:14.000000 Velkoz-0.0.3/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     1159 2024-03-22 11:08:38.000000 Velkoz-0.0.3/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 11:09:07.950065 Velkoz-0.0.3/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.3/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.3/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-03-22 11:07:09.000000 Velkoz-0.0.3/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4529 2024-03-22 11:06:55.000000 Velkoz-0.0.3/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       18 2024-03-21 22:30:33.000000 Velkoz-0.0.3/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 11:07:44.000000 Velkoz-0.0.3/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.3/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     5448 2024-03-22 11:05:01.000000 Velkoz-0.0.3/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-03-22 11:09:07.950065 Velkoz-0.0.3/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      670 2024-03-22 11:09:07.000000 Velkoz-0.0.3/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-03-22 11:09:07.000000 Velkoz-0.0.3/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 11:09:07.000000 Velkoz-0.0.3/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-22 11:09:07.000000 Velkoz-0.0.3/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-22 11:09:07.000000 Velkoz-0.0.3/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 11:09:07.954409 Velkoz-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.600631 Velkoz-0.0.4/
+-rw-rw-rw-   0        0        0      670 2024-04-10 19:41:28.599632 Velkoz-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.554270 Velkoz-0.0.4/Velkoz/
+-rw-rw-rw-   0        0        0      346 2024-03-21 19:18:50.000000 Velkoz-0.0.4/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.589448 Velkoz-0.0.4/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.4/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.4/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.4/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.4/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-06 09:20:19.000000 Velkoz-0.0.4/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.4/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     1159 2024-04-10 19:41:05.000000 Velkoz-0.0.4/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.592616 Velkoz-0.0.4/Velkoz/supp/
+-rw-rw-rw-   0        0        0      129 2024-04-05 19:15:06.000000 Velkoz-0.0.4/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-04-10 19:31:43.000000 Velkoz-0.0.4/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0     1133 2024-04-10 19:40:41.000000 Velkoz-0.0.4/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      258 2024-04-05 19:15:09.000000 Velkoz-0.0.4/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1667 2024-04-05 19:15:09.000000 Velkoz-0.0.4/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.597633 Velkoz-0.0.4/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.4/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.4/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-10 19:40:42.000000 Velkoz-0.0.4/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4505 2024-04-06 09:36:14.000000 Velkoz-0.0.4/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.4/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.4/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.4/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     5364 2024-04-10 19:40:41.000000 Velkoz-0.0.4/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:41:28.598632 Velkoz-0.0.4/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      670 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 19:41:28.000000 Velkoz-0.0.4/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 19:41:28.600631 Velkoz-0.0.4/setup.cfg
```

### Comparing `Velkoz-0.0.3/PKG-INFO` & `Velkoz-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.3
+Version: 0.0.4
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `Velkoz-0.0.3/Velkoz/eye/account.py` & `Velkoz-0.0.4/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.3/Velkoz/eye/match.py` & `Velkoz-0.0.4/Velkoz/eye/match.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,23 +33,37 @@
         i = 0
         while (i<10):
             if self.participants[i] == puuid:
                 return i
             else: i += 1
         raise Exception ('Participant not found.')
 
-    def get_participant(self, index:int = 0, puuid:str = '\0'):
+
+    def _get_participant_by_riotId(self, riotId:str):
+        i = 0
+        while (i < 10):
+            riotName = self.infoDto['participants'][i].get('riotIdGameName', None)
+            tagline = self.infoDto['participants'][i].get('riotIdTagline', None)
+            if riotId == f'{riotName}#{tagline}': return i
+            else: i += 1
+        raise Exception ('Participant not found.')
+    
+
+    def get_participant(self, index:int = 0, puuid:str = '\0', riotId:str = '\0'):
         if puuid != '\0':
             i = self._get_participant_by_puuid(puuid)
+        
+        elif riotId != '\0':
+            i = self._get_participant_by_riotId(riotId)
+
         else:
+            #when index is provided 
             i = index
-
-        #when index is provided
-        if index < 0 or index > len(self.participants) + 1:
-            raise Exception ('That participant does not exist')
+            if index < 0 or index > len(self.participants) + 1:
+                raise Exception ('Invalid index')
 
         return Participant(self.infoDto['participants'][i])
     
 
 
 
 class Participant():
```

### Comparing `Velkoz-0.0.3/Velkoz/eye/summoner.py` & `Velkoz-0.0.4/Velkoz/eye/summoner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 class Summoner():
     
     def __init__(self, summonerDto:dict):
         self.summonerDto = summonerDto
         self.id = summonerDto['id']
         self.accountId = summonerDto['accountId']
         self.puuid = summonerDto['puuid']
-        self.name = summonerDto['name']
+        self.name = summonerDto.get('name', None)
         self.profileIcon = summonerDto['profileIconId']
         self.revisionDate = summonerDto['revisionDate']
         self.level = summonerDto['summonerLevel']
 
     def _save_summoner(self, author):
         print(f'Summoner saved with author {author}(actually did nothing)')
```

### Comparing `Velkoz-0.0.3/Velkoz/setup.py` & `Velkoz-0.0.4/Velkoz/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
```

### Comparing `Velkoz-0.0.3/Velkoz/tentacles/account.py` & `Velkoz-0.0.4/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.3/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.4/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.3/Velkoz/tentacles/common.py` & `Velkoz-0.0.4/Velkoz/tentacles/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,25 +91,25 @@
         request = RiotApiRequest(
             service=self,
             url=url,
             parameters=parameters
         )
         try:
             return request()
-        except requests.exceptions.HTTPError as errh:
-            return (f'HTTPError - {errh.args[0]}')
+        except Exception as error:
+            raise Exception (error)
     
     def _handle_error(
         self,
         error
     ):
         if error == 'Incorrect Parameters':
             return f'Detected error: {error}.'
         else:
-            return f'Raised exception: {error}'
+            raise Exception ('Raised exception: {error}')
 
 
 
 class RiotApiRequest(object):
     #This class needs error handling based on the riot api error codes
     def __init__(
         self,
```

### Comparing `Velkoz-0.0.3/Velkoz/tentacles/match.py` & `Velkoz-0.0.4/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.3/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.4/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.3/Velkoz/velkoz.py` & `Velkoz-0.0.4/Velkoz/velkoz.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,88 +9,53 @@
 from .eye import ( #dont forget the dots
     Summoner,
     Match,
     Participant,
     Account
         )
 
-service = RiotApiService(api_key)
+from .supp import ( #dont forget the dots
+    summoner as summ,
+    account as acc,
+    match as mat,
+    champion_mastery as mastery
+
+        ) 
+
+#CHANGE THIS
+#ERROR HANDLING FOR INVALID API_KEY
+
+def set_api_key(api_key:str):
+    global service
+    service = RiotApiService(api_key)
+
 
 def _initialize_service(api_key=api_key):
     return RiotApiService(api_key) # Service should be initiated in the needed file
 
 
-###############
-# Get Account #
-###############
-
 
-def _get_account_by_riotId(riotId:str, routing:str = 'europe'):
-    parameters = {'riotId': riotId, 'routing' : routing}
-    accountDto = AccountApi.get_account(service, parameters)
-    account = Account(accountDto)
-    return account
-
-def _get_account_by_parameters(parameters:dict):
-    accountDto = AccountApi.get_account(service, parameters)
-    account = Account(accountDto)
-    return account
 
+def _handle_missing_parameters(request:str):
 
+    raise Exception (f'Error fulfilling request {request}. Make sure you are passing the correct arguments')
 
-def _get_summonerDto_by_account(account:dict, region:str = 'euw1'):
-    parameters = {'puuid' : account['puuid'], 'region': region}
-    summonerDto = SummonerApi.get_summoner(service, parameters)
-    return summonerDto
-
-################
-# Get Summoner #
-################
-
-
-def _get_summoner_by_account(account:dict, region:str = 'euw1'):
-    parameters = {'puuid': account['puuid'], 'region' : region}
-    summonerDto = SummonerApi.get_summoner(service, parameters)
-    return Summoner(summonerDto)
-
-def _get_summoner_by_summonerName(summonerName:str, region:str = 'euw1'):
-    parameters = {'summonerName': summonerName, 'region': region}
-    summonerDto = SummonerApi.get_summoner(service,parameters)
-    return Summoner(summonerDto)
-
-def _get_summoner_by_summonerId(summonerId:str, region:str = 'euw1'):
-    parameters = {'summonerId': summonerId, 'region': region}
-    summonerDto = SummonerApi.get_summoner(service, parameters)
-    return Summoner(summonerDto)
-
-
-def _get_summoner_by_parameters(parameters):
-    summonerDto = SummonerApi.get_summoner(service, parameters)
-    return Summoner(summonerDto)
-
-
-#############
-# Get Match #
-#############
 
-def _get_matchDto_by_parameters(parameters:dict):
-    matchDto = MatchApi.get_matchDto(service, parameters)
-    return matchDto
 
 
+#for now only used in champion_mastery functions
+def _get_puuid(puuid:str, riotId:str, routing:str = 'europe'):
 
-#############
-
-def _request_on_summoner_by_riotId(riotId:str, routing:str = 'europe',region:str = 'euw1', request={'summonerLevel'}):
-    account = _get_account_by_riotId(riotId, routing) 
-    summonerDto = _get_summonerDto_by_account(account, region)
-    summoner = Summoner(summonerDto)
-    summoner_data = summoner.request({'data':request})
-    return summoner_data
-
+    if puuid != '\0':
+        return puuid
+    elif riotId != '\0':
+        account = get_account(riotId=riotId, routing=routing)
+        return account.puuid
+    else:
+        _handle_missing_parameters('_get_puuid')
 
 
 
 ############
 # Callable #
 ############
 
@@ -107,51 +72,51 @@
         parameters['riotId'] = riotId
     elif puuid != '\0':
         parameters['puuid'] = puuid
     else:
         raise Exception ('Error getting account. Please provide a riotId or puuid')
 
     parameters['routing'] = routing
-    account = _get_account_by_parameters(parameters)
+    account = acc._get_account_by_parameters(service, parameters)
     return account
 
 '''
 Function to get summoner
 Usage: Must be provided with a riotId, summonerName or summonerId. Having priority in the order they were mentioned here. Region parameter defualts to 'euw1', but should be changed if the summoner you are looking for is not from the euw server.
 '''
 def get_summoner(riotId:str = '\0', summonerName:str = '\0', summonerId:str = 0, region:str = 'euw1'):
     
     if riotId != '\0':
-        account = _get_account_by_riotId(riotId)
+        account = acc._get_account_by_riotId(service, riotId)
         parameters = {'puuid' : account.puuid}
 
     elif summonerName != '\0':
         parameters = {'summonerName': summonerName}
 
     elif summonerId != 0:
         parameters = {'summonerId' : summonerId}
 
     else:
         raise Exception ('Error getting summoner. Please provide a riotId, summonerName or summonerId')
 
     parameters['region'] = region
-    summoner = _get_summoner_by_parameters(parameters)
+    summoner = summ._get_summoner_by_parameters(service, parameters)
     return summoner
 
 
 
 '''
 Function to get a list of matches given a riotId or puuid
 needs more arguments, possibly use args to get the query
 returns an array with the match ids
 '''
 def get_match_list(riotId:str = '\0', puuid:str = '\0', routing:str = 'europe', count:int = 20):
     
     if riotId != '\0':
-        account = _get_account_by_riotId(riotId) 
+        account = acc._get_account_by_riotId(service, riotId) 
         parameters = {'puuid': account.puuid}
 
     elif puuid != '\0':
         parameters = {'puuid': puuid}
 
     parameters['routing'] = routing
     query = {'count' : count}
@@ -163,19 +128,57 @@
 Function to get a Match by a matchId
 Usage: Must be provided a matchId. Routing parameter is not necessary since it defaults to 'europe', but must be changed if the match is not from european servers.
 '''
 
 def get_match(matchId:str, routing:str = 'europe'):
 
     parameters = {'matchId' : matchId, 'routing': routing}
-    matchDto = _get_matchDto_by_parameters(parameters)
+    matchDto = _get_matchDto_by_parameters(service, parameters)
     match = Match(matchDto)
     return match
 
 
+####################
+# Champion Mastery #RGAPI-bdc5003a-3b45-4bc1-b6ec-f2dc5d4ae224
+####################
+
+def get_all_masteries(puuid:str = '\0', riotId:str = '\0', region = 'euw1', routing = 'europe'):
+    
+    new_puuid = _get_puuid(puuid, riotId, routing)
+
+    return mastery._get_all_masteries_by_puuid(service, new_puuid, region = region)
+
+
+def get_champion_mastery(puuid:str = '\0', riotId:str = '\0', championId:int = 1 ,region:str = 'euw1', routing:str = 'europe'):
+
+    new_puuid = _get_puuid(puuid, riotId, routing)
+
+
+    return mastery._get_champion_mastery(service=service, puuid = new_puuid, championId = championId,region = region)
+
+def get_top_masteries(puuid:str = '\0', riotId:str = '\0', region:str = 'euw1', routing:str = 'europe', **kwargs):
+
+    new_puuid = _get_puuid(puuid, riotId, routing)
+
+    query = {}
+    for key, value in kwargs.items():
+        query[key] = value
+
+    return mastery._get_top_masteries(service, puuid=puuid, query=query, region=region)
+
+
+def get_masteryscore(puuid:str='\0', riotId:str='\0',region:str='euw1', routing:str='europe'):
+
+    new_puuid = _get_puuid(puuid, riotId, routing)
+
+    return mastery._get_masteryscore(service, puuid=new_puuid, region=region)
+
+
+
+
 
 #############
 # DEBUGGING #
 #############
 
 if __name__ == '__main__':
     pass
```

### Comparing `Velkoz-0.0.3/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.4/Velkoz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.3
+Version: 0.0.4
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

