# Comparing `tmp/servizio_anon-0.2.1.tar.gz` & `tmp/servizio_anon-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servizio_anon-0.2.1.tar", last modified: Thu Mar 21 12:13:05 2024, max compression
+gzip compressed data, was "servizio_anon-0.5.0.tar", last modified: Tue Apr  9 16:02:38 2024, max compression
```

## Comparing `servizio_anon-0.2.1.tar` & `servizio_anon-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 12:13:05.959340 servizio_anon-0.2.1/
--rw-rw-rw-   0        0        0      906 2024-01-05 15:41:49.000000 servizio_anon-0.2.1/LICENSE.md
--rw-rw-rw-   0        0        0      787 2024-03-21 12:13:05.957346 servizio_anon-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-02 11:37:53.000000 servizio_anon-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 12:13:05.941389 servizio_anon-0.2.1/servizio_anon/
--rw-rw-rw-   0        0        0        0 2023-12-30 15:32:18.000000 servizio_anon-0.2.1/servizio_anon/__init__.py
--rw-rw-rw-   0        0        0     2964 2024-03-21 12:09:28.000000 servizio_anon-0.2.1/servizio_anon/servizio_anon.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:13:05.955352 servizio_anon-0.2.1/servizio_anon.egg-info/
--rw-rw-rw-   0        0        0      787 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 12:13:05.959340 servizio_anon-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      974 2024-03-21 12:09:57.000000 servizio_anon-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:02:38.369994 servizio_anon-0.5.0/
+-rw-rw-rw-   0        0        0      906 2024-01-05 15:41:49.000000 servizio_anon-0.5.0/LICENSE.md
+-rw-rw-rw-   0        0        0      787 2024-04-09 16:02:38.367993 servizio_anon-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-02 11:37:53.000000 servizio_anon-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:02:38.349995 servizio_anon-0.5.0/servizio_anon/
+-rw-rw-rw-   0        0        0        0 2023-12-30 15:32:18.000000 servizio_anon-0.5.0/servizio_anon/__init__.py
+-rw-rw-rw-   0        0        0     4073 2024-04-09 15:58:11.000000 servizio_anon-0.5.0/servizio_anon/servizio_anon.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:02:38.365995 servizio_anon-0.5.0/servizio_anon.egg-info/
+-rw-rw-rw-   0        0        0      787 2024-04-09 16:02:38.000000 servizio_anon-0.5.0/servizio_anon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-09 16:02:38.000000 servizio_anon-0.5.0/servizio_anon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:02:38.000000 servizio_anon-0.5.0/servizio_anon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2024-04-09 16:02:38.000000 servizio_anon-0.5.0/servizio_anon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 16:02:38.000000 servizio_anon-0.5.0/servizio_anon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:02:38.369994 servizio_anon-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      974 2024-04-09 16:02:20.000000 servizio_anon-0.5.0/setup.py
```

### Comparing `servizio_anon-0.2.1/LICENSE.md` & `servizio_anon-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `servizio_anon-0.2.1/PKG-INFO` & `servizio_anon-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servizio_anon
-Version: 0.2.1
+Version: 0.5.0
 Summary: Aggiornamento automatico di documenti GateNLP mediante Presidio
 Home-page: https://github.com/RafVale/anon_testo
 Author: Raffaele Valendino
 Author-email: raffaele.valendino@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `servizio_anon-0.2.1/servizio_anon/servizio_anon.py` & `servizio_anon-0.5.0/servizio_anon/servizio_anon.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,79 @@
+import copy
 
-def updateAnnotazioni(gatenlpOriginale:dict, risultatoAnalisi:list):
+def updateAnnotazioni(gatenlpOriginale:dict, risultatoAnalisi:list, sovrascriviAnnotazioni):
 #REQUIRES: Valid GateNLP and a List which contains the results of an analysis run by Presidio
 #MODIFIES: input GateNLP
-#EFFECTS: Returns a new GateNLP with updated annotations found via Presidio
-    annotazioni = gatenlpOriginale['annotation_sets']["entities"]["annotations"]
-    nextID = gatenlpOriginale['annotation_sets']["entities"]["next_annid"]
+#EFFECTS: Returns a new GateNLP with updated annotations found via Presidio inside an annotation field
+
+    if sovrascriviAnnotazioni == False:
+        if "presidio_entities" not in (gatenlpOriginale["annotation_sets"].keys()):
+            gatenlpOriginale["annotation_sets"]["presidio_entities"] = {}
+            gatenlpOriginale["annotation_sets"]["presidio_entities"]["name"] = "presidio_entities"
+            gatenlpOriginale["annotation_sets"]["presidio_entities"]["annotations"] = copy.deepcopy(gatenlpOriginale['annotation_sets']["entities"]["annotations"])
+            gatenlpOriginale["annotation_sets"]["presidio_entities"]["next_annid"] = copy.deepcopy(gatenlpOriginale["annotation_sets"]["entities"]["next_annid"])
+
+        nextID = gatenlpOriginale['annotation_sets']["presidio_entities"]["next_annid"]
+        annotazioni = gatenlpOriginale['annotation_sets']["presidio_entities"]["annotations"]
+    
+    else:
+        nextID = gatenlpOriginale['annotation_sets']["entities"]["next_annid"]
+        annotazioni = gatenlpOriginale['annotation_sets']["entities"]["annotations"]
 
     # Mappiamo le entità per rinominarle
     entity_type_mapping = {
         'PERSON': 'persona_presidio',
         'LOCATION': 'indirizzo',
         'ORGANIZATION': 'persona_presidio',
         'IT_FISCAL_CODE':'codice_fiscale',
         'IT_VAT_CODE':'partita_iva',
         'LIST':'lista'
     }
 
-
     for nuovaAnnotazione in risultatoAnalisi:
         flagPresenza = False
 
         for annotazioneOriginale in annotazioni:
             if annotazioneOriginale["start"] == nuovaAnnotazione.start and annotazioneOriginale["end"] == nuovaAnnotazione.end:
                 print("La seguente annotazione non è stata inserita in quanto doppione:")
                 print(nuovaAnnotazione)
                 flagPresenza = True,
                 break
         
         if flagPresenza == False:
             mapped_entity_type = entity_type_mapping.get(nuovaAnnotazione.entity_type)
-
+            
             if (mapped_entity_type) == 'lista':
                 mapped_entity_type = 'persona_presidio'
                 for annotazioneOriginale in annotazioni:
                     if annotazioneOriginale["features"]["title"] == gatenlpOriginale["text"][nuovaAnnotazione.start:nuovaAnnotazione.end]:
                         mapped_entity_type = annotazioneOriginale["features"]["ner"]["type"]
                         break
 
             testoAnnotazione = {"type": "Word",
                                 "start": nuovaAnnotazione.start,
                                 "end": nuovaAnnotazione.end,
                                 "id": nextID,
                                 "features": {
-                                "title": gatenlpOriginale["text"][nuovaAnnotazione.start:nuovaAnnotazione.end],
-                                "url": "",
-                                "ner": {
-                                    "type": mapped_entity_type,
-                                    "normalized_text": gatenlpOriginale["text"][nuovaAnnotazione.start:nuovaAnnotazione.end],
-                                },
-                                "entity_registry": {
-                                    "er_name": None,
-                                    "entity_type": None,
-                                    "entity_id": None
+                                    "title": gatenlpOriginale["text"][nuovaAnnotazione.start:nuovaAnnotazione.end],
+                                    "url": "",
+                                    "ner": {
+                                        "type": mapped_entity_type,
+                                        "normalized_text": gatenlpOriginale["text"][nuovaAnnotazione.start:nuovaAnnotazione.end],
+                                    },
+                                    "entity_registry": {
+                                        "er_name": None,
+                                        "entity_type": None,
+                                        "entity_id": None
                                     }
                                 },
                             }
             annotazioni.append(testoAnnotazione)
             nextID += 1
-    
-    gatenlpOriginale['annotation_sets']["entities"]["next_annid"] = nextID
+
+    if sovrascriviAnnotazioni == False:
+        gatenlpOriginale['annotation_sets']["presidio_entities"]["next_annid"] = nextID
+        
+    else:
+        gatenlpOriginale['annotation_sets']["entities"]["next_annid"] = nextID
+
     return gatenlpOriginale
```

### Comparing `servizio_anon-0.2.1/servizio_anon.egg-info/PKG-INFO` & `servizio_anon-0.5.0/servizio_anon.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servizio_anon
-Version: 0.2.1
+Version: 0.5.0
 Summary: Aggiornamento automatico di documenti GateNLP mediante Presidio
 Home-page: https://github.com/RafVale/anon_testo
 Author: Raffaele Valendino
 Author-email: raffaele.valendino@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `servizio_anon-0.2.1/setup.py` & `servizio_anon-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='servizio_anon',
-    version='0.2.1',    
+    version='0.5.0',    
     description='Aggiornamento automatico di documenti GateNLP mediante Presidio',
     url='https://github.com/RafVale/anon_testo',
     author='Raffaele Valendino',
     author_email='raffaele.valendino@gmail.com',
     license='MIT',
     packages=['servizio_anon'],
     install_requires=['spacy <= 3.2.0',
```

