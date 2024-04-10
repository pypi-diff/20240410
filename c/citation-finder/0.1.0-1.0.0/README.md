# Comparing `tmp/citation_finder-0.1.0.tar.gz` & `tmp/citation_finder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_finder-0.1.0.tar", max compression
+gzip compressed data, was "citation_finder-1.0.0.tar", max compression
```

## Comparing `citation_finder-0.1.0.tar` & `citation_finder-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       63 2023-11-28 14:33:25.496513 citation_finder-0.1.0/README.md
--rw-r--r--   0        0        0     4719 2023-11-28 14:33:25.496513 citation_finder-0.1.0/citation_finder.py
--rw-r--r--   0        0        0      341 2023-11-28 14:33:25.500512 citation_finder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 citation_finder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2957 2024-04-10 11:44:59.520431 citation_finder-1.0.0/README.md
+-rw-r--r--   0        0        0     4603 2024-04-10 11:49:29.965937 citation_finder-1.0.0/citation_finder.py
+-rw-r--r--   0        0        0      341 2024-04-10 11:52:20.166647 citation_finder-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3455 1970-01-01 00:00:00.000000 citation_finder-1.0.0/PKG-INFO
```

### Comparing `citation_finder-0.1.0/citation_finder.py` & `citation_finder-1.0.0/citation_finder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,122 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import re
 import pandas as pd
 import dhlab as dh
+import datetime
 
 def findone(regex, s):
     res = re.findall(regex,s)
     try:
         r = res[0]
     except:
         r = "itj no"
     return r
 
 #### Bygge korpus
-# corpus = dh.Corpus(doctype="digibok", subject = "språkvitenskap", limit = 1000,from_year=1950)
+#### corpus = dh.Corpus(doctype="digibok", subject = "språkvitenskap", limit = 1000, from_year=1950)
 
-#### Finne konkordanser med årstall mellom 1900 og 2020
+#### Finne konkordanser med årstall mellom 1000 og 2023
 
-def citation_finder(corpus, yearspan = (1900,2020), get_concs: bool = False):
+
+curr_year = datetime.datetime.today().year
+
+
+def citation_finder(corpus, yearspan=(1000,curr_year), conc_limit=4000, get_concs=False):
+    """Finds citations in text using regular expressions"""
 
     tall = list(range(yearspan[0],yearspan[1]))
 
     tallOR = ' OR '.join([str(x) for x in tall])
 
-    tallconc = dh.Concordance(corpus, tallOR, limit=4000)
+    tallconc = dh.Concordance(corpus, tallOR, limit=conc_limit)
 
     concs = tallconc.frame
     concs.concordance = concs.concordance.apply(lambda x:x.replace('<b>', '').replace('</b>', '').replace('...', ''))
-
-    books1 = concs[['urn', 'concordance']]
+    concs1 = concs[['urn', 'concordance']]
 
     #### Regex1
     #### finner alle konkordanser med parentes (eller semikolon) med årstall.
 
     regex1 = r'[\(;].*?\D\d{4}\D.*?[\);]'
 
-    books1['parentes'] = books1.concordance.apply(lambda x: findone(regex1, x))
+    concs1['parentes'] = concs1.concordance.apply(lambda x: findone(regex1, x))
 
-    books2 = books1[books1['parentes'] != 'itj no']
-    books2 = books2[['urn', 'concordance']]
+    concs2 = concs1[concs1['parentes'] != 'itj no']
+    concs2 = concs2[['urn', 'concordance']]
 
+    #### Navn i parentes
     #### Regex2
-    #### finner alle konkordanser som har tallkonstruksjoner med årstall og potensielt sidetall før sluttparentes (eller semikolon).
-    #### books3 er en dataramme med disse resultatene. Den er grunnlaget for å finne de to forskjellige typene siteringer med navn og
-    #### årstall inne i parentes, og med navn utenfor parentes.
+    #### finner alle konkordanser med navn, årstall og potensielt sidetall før sluttparentes (eller semikolon). Navnet kan følges av "et
+    #### al." eller "m.fl.".
 
-    regex2 = r'\[?\s*\d{4}\s*[a-zæøå]?\s*\.?\s*\]?(?:\s*[,-;:/\)\s]\s*(?:[ps]\s*\.?)?\[?\s*\d{1,4}\s*[a-zæøå]?\s*\.?\s*\]?)*\s*[\);]'
+    regex2 = r'(?:[A-ZÀ-Ž](?:[A-zÀ-ž-]+|\s*\.)\s*,?\s*)+(?:\s*(?:et\s*al\.?|m(?:ed|\s*\.?)\s*fl(?:ei?re?|\s*\.?))\s*)?,?\s*\[?\s*\d{4}\s*[a-zæøå]?\s*\.?\s*\]?(?:\s*[,;:/\)\s]\s*(?:[PpSs]\s*\.?)?\[?\s*\d{1,4}\s*[a-zæøå]?\s*\.?\s*\]?(?:\s*[,-]\s*\d{1,4}\s*[a-zæøå]?\s*\.?)?)*\s*[\);]'
 
-    books2['årstall + sidetall'] = books2.concordance.apply(lambda x: findone(regex2, x))
+    concs2['navn i parentes'] = concs2.concordance.apply(lambda x: findone(regex2, x))
 
-    books3 = books2[books2['årstall + sidetall'] != 'itj no']
-    books3 = books3[['urn', 'concordance']]
-
-    #### Navn i parentes
-    #### Regex3
-    #### finner alle konkordanser med navn, årstall og potensielt sidetall før sluttparentes (eller semikolon). Navnet kan følge "og/and/&"
-    #### eller følges av "et al.".
-
-    regex3 = r'(?:og|and|&)?(?:[A-ZÆØÅ](?:[A-ZÆØÅa-zæøå-]+|\s*\.)\s*,?\s*)+(?:\s*et\sal\.\s*)?,?\s*\[?\s*\d{4}\s*[a-zæøå]?\s*\.?\s*\]?(?:\s*[,-;:/\)\s]\s*(?:[ps]\s*\.?)?\[?\s*\d{1,4}\s*[a-zæøå]?\s*\.?\s*\]?)*\s*[\);]'
-
-    books3['navn i parentes'] = books3.concordance.apply(lambda x: findone(regex3, x))
+    concs3 = concs2[concs2['navn i parentes'] != 'itj no']
+    concs3 = concs3[['urn', 'concordance']]
 
     if get_concs:
-        return books3
+        return concs3
 
-    books4 = books3[books3['navn i parentes'] != 'itj no']
-    books4 = books4[['urn', 'concordance']]
-
-    #### Regex4
+    #### Regex3
     #### finner alle treff i alle konkordanser som macther parenteser (eller semikolon) som består av minst én bokstav, årstall og hva som
-    #### helst annet. Antakelsen er at vi allerede har filtrert ut parentes-konstruksjoner som ligner på siteringer med navn, årstall og
+    #### helst annet. Antakelsen er at vi allerede har filtrert på parentes-konstruksjoner som ligner på siteringer med navn, årstall og
     #### sidetall og at alle parenteser med minimum én bokstav og et årstall derfor er siteringer.
 
-    regex4 = r'(?<=[\(;])[^(;\d]*?[A-ZÆØÅa-zæøå][^(;]*?\d{4}[^);]*?(?=[\);])'
+    regex3 = r'(?<=[\(;])[^(;\d]*?[A-zÀ-ž-][^(;]*?\d{4}[^);]*?(?=[\);])'
 
     match = []
 
-    for i in books4.values:
-        m = re.findall(regex4, i[1])
+    for i in concs3.values:
+        m = re.findall(regex3, i[1])
         if m != []:
             match.append((i[0],m))
 
     match_df = pd.DataFrame(match)
     match_explode = match_df.explode(column=1)
 
     #### Navn utenfor parentes
-    #### Regex5
-    #### tar utgangspunkt i books3 og finner alle konkordanser med navn utenfor parentes (eller semikolon) med årstall inni.
-
-    regex5 = '(?:[A-ZÆØÅ](?:[A-ZÆØÅa-zæøå-]+|\s*\.)\s*,?\s*)+[\(;]\s*\d{4}\D'
-
-    books3['navn u/parentes'] = books3.concordance.apply(lambda x: findone(regex5, x))
-
-    books5 = books3[books3['navn u/parentes'] != 'itj no']
-    books5 = books5[['urn', 'concordance']]
-
-    #### Regex6
+    #### Regex4
     #### finner alle treff i alle konkordanser som macther navn utenfor parentes (eller semikolon) som består av et årstall og hva som helst
     #### annet. Navnekonstruksjonene kan bestå av flere navn etter hverandre, potensielt skilt av komma eller "og/and/&", eller etterfulgt
-    #### av "et al.".
+    #### av "et al." eller "m.fl.".
 
-    regex6 = r'(?:(?:[A-ZÆØÅ](?:[A-ZÆØÅa-zæøå-]+|\s*\.)\s*,?\s*)+(?:og|and|&)\s*)?(?:[A-ZÆØÅ](?:[A-ZÆØÅa-zæøå-]+|\s*\.)\s*,?\s*)+(?:\s*et\sal\.)?\s*\(\s*\d{4}\D[^)]*?\)'
+    regex4 = r'(?:(?:[A-ZÀ-Ž](?:[A-zÀ-ž-]+|\s*\.)\s*,?\s*)+(?:og|and|&)\s*)?(?:[A-ZÀ-Ž](?:[A-zÀ-ž-]+|\s*\.)\s*,?\s*)+(?:\s*(?:et\s*al\.?|m(?:ed|\s*\.?)\s*fl(?:ei?re?|\s*\.?))\s*)?\s*\(\s*\d{4}\s+(?:\)|[^-–—)][^)]*?\))'
 
     matchu = []
 
-    for i in books5.values:
-        mu = re.findall(regex6, i[1])
+    for i in concs2.values:
+        mu = re.findall(regex4, i[1])
         if mu != []:
             matchu.append((i[0],mu))
 
     matchu_df = pd.DataFrame(matchu)
     matchu_explode = matchu_df.explode(column=1)
 
-    ### match_sorted
-    # setter sammen datarammene med siteringer for navn i og utenfor parentes, og sorterer på URN.
-
-    match_concat = pd.concat([match_explode, matchu_explode], ignore_index=True)
-    match_sorted = match_concat.sort_values(by=0, ignore_index=True)
-
-    return match_sorted
+    #### NOU, Stortingsmelding og Proposisjon
+    #### Regex5
+    #### finner alle treff i alle konkordanser som matcher NOU-er, stortingsmeldinger eller proposisjoner.
 
+    regex5 = r'(?:(?:NOU|nou)\s*\(?\s*\d{4}\s*:\s*\d{1,4}|(?:St\s*\.?\s*)?Meld\s*\.?\s*(?:St\s*\.?\s*)?(?:nr\s*\.?\s*)?\d{1,3}\s*\(?\s*\d{4}\s*-\s*\d{4}\s*\)?|Prop\s*\.?\s*\d{1,3}\s*[A-ZÆØÅ]\s*\(?\s*\d{4}\s*-\s*\d{4}\s*\)?)(?:\s*[,(]?\s*[PpSs]\s*\.?\s*\d{1,4})?'
 
+    matchn = []
 
+    for i in concs1.values:
+        mn = re.findall(regex5, i[1])
+        if mn != []:
+            matchn.append((i[0],mn))
 
+    matchn_df = pd.DataFrame(matchn)
+    matchn_explode = matchn_df.explode(column=1)
 
+    #### match_sorted
+    #### setter sammen datarammene med siteringer for navn i parentes, navn utenfor parentes og NOU-er, stortingsmeldinger og proposisjoner,
+    #### og sorterer på URN.
 
+    match_concat = pd.concat([match_explode, matchu_explode, matchn_explode], axis=0, ignore_index=True)
+    match_sorted = match_concat.sort_values(by=0, ignore_index=True)
 
+    return match_sorted
```

