# Comparing `tmp/pyetho-1.2.tar.gz` & `tmp/pyetho-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetho-1.2.tar", last modified: Mon Mar 11 08:58:05 2024, max compression
+gzip compressed data, was "pyetho-2.0.tar", last modified: Wed Apr 10 06:29:32 2024, max compression
```

## Comparing `pyetho-1.2.tar` & `pyetho-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 08:58:05.004748 pyetho-1.2/
--rw-rw-rw-   0        0        0     5491 2024-03-11 08:58:05.004748 pyetho-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2024-03-11 08:36:12.000000 pyetho-1.2/README.md
--rw-rw-rw-   0        0        0      108 2023-08-26 06:59:26.000000 pyetho-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      794 2024-03-11 08:58:05.007901 pyetho-1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 08:58:04.981011 pyetho-1.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 08:58:04.987040 pyetho-1.2/src/etho/
--rw-rw-rw-   0        0        0        0 2023-08-26 06:44:15.000000 pyetho-1.2/src/etho/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:58:04.989347 pyetho-1.2/src/etho/data/
--rw-rw-rw-   0        0        0  3328676 2024-02-26 07:10:46.000000 pyetho-1.2/src/etho/data/etho.pkl
--rw-rw-rw-   0        0        0    34254 2024-03-11 08:51:10.000000 pyetho-1.2/src/etho/pyetho.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:58:05.003233 pyetho-1.2/src/pyetho.egg-info/
--rw-rw-rw-   0        0        0     5491 2024-03-11 08:58:04.000000 pyetho-1.2/src/pyetho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-03-11 08:58:04.000000 pyetho-1.2/src/pyetho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 08:58:04.000000 pyetho-1.2/src/pyetho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-11 08:58:04.000000 pyetho-1.2/src/pyetho.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:29:32.198241 pyetho-2.0/
+-rw-rw-rw-   0        0        0     5584 2024-04-10 06:29:32.198241 pyetho-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5062 2024-04-10 06:20:42.000000 pyetho-2.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-08-26 06:59:26.000000 pyetho-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      794 2024-04-10 06:29:32.200337 pyetho-2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 06:29:32.100850 pyetho-2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 06:29:32.105469 pyetho-2.0/src/etho/
+-rw-rw-rw-   0        0        0        0 2023-08-26 06:44:15.000000 pyetho-2.0/src/etho/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:29:32.155172 pyetho-2.0/src/etho/data/
+-rw-rw-rw-   0        0        0  3328676 2024-02-26 07:10:46.000000 pyetho-2.0/src/etho/data/etho.pkl
+-rw-rw-rw-   0        0        0    34222 2024-03-30 05:36:25.000000 pyetho-2.0/src/etho/pyetho.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:29:32.197243 pyetho-2.0/src/pyetho.egg-info/
+-rw-rw-rw-   0        0        0     5584 2024-04-10 06:29:32.000000 pyetho-2.0/src/pyetho.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-10 06:29:32.000000 pyetho-2.0/src/pyetho.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:29:32.000000 pyetho-2.0/src/pyetho.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 06:29:32.000000 pyetho-2.0/src/pyetho.egg-info/top_level.txt
```

### Comparing `pyetho-1.2/PKG-INFO` & `pyetho-2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetho
-Version: 1.2
+Version: 2.0
 Summary: Exploration of World Languages
 Home-page: https://github.com/i18nsolutionspy/Pyetho
 Author: SathishKumar paramasivam Et al.
 Author-email: i18nsolutionspy@gmail.com
 Project-URL: Bug Tracker, https://github.com/i18nsolutionspy/Pyetho/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,18 +16,21 @@
   <img src="https://raw.githubusercontent.com/i18nsolutionspy/Ethnologue/632e1a61f13aaf91e2e93766ef9d6bc91cceb1e4/logo.svg"><br>
 </div>
 
 ## Pyetho: A library for Python to all the country languages in the world
 This is a Language and Country Information Package. In order to know the details of all the languages in the world, **i18n Solutions Salem**, have developed this package based on the interest of integrating the languages of the world to python developers.
 
 
-> Developers : Bhuvaneshwara Ragavendra.S <bhuvaneshwararagavendra@gmail.com> Roseline Santhiya.M <rosekevin30@gmail.com> Archana.K.T <archanakt.cse@gmail.com> Vinoth Kumar <vinobe000@gmail.com>
+>Developers : Bhuvaneshwara Ragavendra.S <bhuvaneshwararagavendra@gmail.com> Roseline Santhiya.M <rosekevin30@gmail.com> Archana.K.T <archanakt.cse@gmail.com>
 
+>Version 1.0 Developer: Vinoth Kumar <vinobe000@gmail.com>
 
-> Contributors : Varsha A, JayaShree S, Kaviya V, Abinaya V, Janani S, Karthika P, Anandhi P, Hemalatha R, Sri Sakthi Priya T, Nidha Basreen M, Anu R, Megala V, Mogana Priya S
+>version 2.0 Contributors : Arthi G
+
+>Version 1.0 Contributors : Varsha A, JayaShree S, Kaviya V, Abinaya V, Janani S, Karthika P, Anandhi P, Hemalatha R, Sri Sakthi Priya T, Nidha Basreen M, Anu R, Megala V, Mogana Priya S
 
 
 
 Installation
 ============
 ```python
 pip install pyetho
@@ -49,19 +52,19 @@
 -> Retrieve details about countries and their attributes such as continent, area, commencement year, and more.
 
 -> Access language-specific information, including summaries, language codes, populations, and families.
 
 -> Explore language families and their associated languages across various countries.
 
 ```python
-1        
+1
 country_list()
 Get a list of all country names in the dataset.
 
-2        
+2
 country_summary(country_name="India")
 Get a summary of the specified country.
 
 3
 country_officialname(country_name="India")
 Get the official name of the specified country.
 
@@ -176,7 +179,9 @@
 https://www.ethnologue.com/
 
 https://www.worldometers.info/
 
 https://www.worlddata.info/
 
 https://www.wikipedia.org/
+
+https://www.officeholidays.com/
```

### Comparing `pyetho-1.2/README.md` & `pyetho-2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,21 @@
   <img src="https://raw.githubusercontent.com/i18nsolutionspy/Ethnologue/632e1a61f13aaf91e2e93766ef9d6bc91cceb1e4/logo.svg"><br>
 </div>
 
 ## Pyetho: A library for Python to all the country languages in the world
 This is a Language and Country Information Package. In order to know the details of all the languages in the world, **i18n Solutions Salem**, have developed this package based on the interest of integrating the languages of the world to python developers.
 
 
-> Developers : Bhuvaneshwara Ragavendra.S <bhuvaneshwararagavendra@gmail.com> Roseline Santhiya.M <rosekevin30@gmail.com> Archana.K.T <archanakt.cse@gmail.com> Vinoth Kumar <vinobe000@gmail.com>
+>Developers : Bhuvaneshwara Ragavendra.S <bhuvaneshwararagavendra@gmail.com> Roseline Santhiya.M <rosekevin30@gmail.com> Archana.K.T <archanakt.cse@gmail.com>
 
+>Version 1.0 Developer: Vinoth Kumar <vinobe000@gmail.com>
 
-> Contributors : Varsha A, JayaShree S, Kaviya V, Abinaya V, Janani S, Karthika P, Anandhi P, Hemalatha R, Sri Sakthi Priya T, Nidha Basreen M, Anu R, Megala V, Mogana Priya S
+>version 2.0 Contributors : Arthi G
+
+>Version 1.0 Contributors : Varsha A, JayaShree S, Kaviya V, Abinaya V, Janani S, Karthika P, Anandhi P, Hemalatha R, Sri Sakthi Priya T, Nidha Basreen M, Anu R, Megala V, Mogana Priya S
 
 
 
 Installation
 ============
 ```python
 pip install pyetho
@@ -35,19 +38,19 @@
 -> Retrieve details about countries and their attributes such as continent, area, commencement year, and more.
 
 -> Access language-specific information, including summaries, language codes, populations, and families.
 
 -> Explore language families and their associated languages across various countries.
 
 ```python
-1        
+1
 country_list()
 Get a list of all country names in the dataset.
 
-2        
+2
 country_summary(country_name="India")
 Get a summary of the specified country.
 
 3
 country_officialname(country_name="India")
 Get the official name of the specified country.
 
@@ -161,8 +164,10 @@
 ==========
 https://www.ethnologue.com/
 
 https://www.worldometers.info/
 
 https://www.worlddata.info/
 
-https://www.wikipedia.org/
+https://www.wikipedia.org/
+
+https://www.officeholidays.com/
```

### Comparing `pyetho-1.2/setup.cfg` & `pyetho-2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7965 7468 6f0d 0a76 6572 7369   = pyetho..versi
-00000020: 6f6e 203d 2031 2e32 0d0a 6175 7468 6f72  on = 1.2..author
+00000020: 6f6e 203d 2032 2e30 0d0a 6175 7468 6f72  on = 2.0..author
 00000030: 203d 2053 6174 6869 7368 4b75 6d61 7220   = SathishKumar 
 00000040: 7061 7261 6d61 7369 7661 6d20 4574 2061  paramasivam Et a
 00000050: 6c2e 0d0a 6175 7468 6f72 5f65 6d61 696c  l...author_email
 00000060: 203d 2069 3138 6e73 6f6c 7574 696f 6e73   = i18nsolutions
 00000070: 7079 4067 6d61 696c 2e63 6f6d 0d0a 6465  py@gmail.com..de
 00000080: 7363 7269 7074 696f 6e20 3d20 4578 706c  scription = Expl
 00000090: 6f72 6174 696f 6e20 6f66 2057 6f72 6c64  oration of World
```

### Comparing `pyetho-1.2/src/etho/data/etho.pkl` & `pyetho-2.0/src/etho/data/etho.pkl`

 * *Files identical despite different names*

### Comparing `pyetho-1.2/src/etho/pyetho.py` & `pyetho-2.0/src/etho/pyetho.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json	  
 import os
 import pandas as pd
 import pickle
 module_path = os.path.dirname(__file__)
 with open(os.path.join(module_path,"data","etho.pkl"),"rb") as x:
     data=(pickle.load(x))
     #@staticmethod
@@ -10,15 +9,15 @@
          """
         Get a list of all country names in the dataset.
 
         Returns:
         list: A list of country names.
 
         Examples
-        --------        
+        --------
         >>> pyetho.country_list()
         ['Afghanistan',
         'Albania',
         'Algeria',
         'Andorra',
         'Angola',
         'Antigua_and_Barbuda',
@@ -46,15 +45,15 @@
         country_name : str, optional
             The name of the country will be given to retrieve the summary. Default choice is "India".
 
         Returns:
         str: A summary of the specified country will be returned in a string format.
 
         Examples
-        --------        
+        --------
         >>> pyetho.country_summary('Sri_Lanka')
         'Sri Lanka is a country in Asia that is home to 22,156,000 people. It is also home to 5 living indigenous languages. Two of these, Sinhala and Tamil, are the official languages of the country. In addition, 2 living non-indigenous languages are established within the country. In formal education, 2 indigenous languages are used as languages of instruction.'
         
         >>> pyetho.country_summary('China')
         'China is a country in Asia that is home to 1,412,600,000 people. It is also home to 281 living indigenous languages. One of these, Mandarin Chinese, is the official language of the country. Others—Central Tibetan, Kyrgyz, and Uyghur—are official languages in parts of the country. China was also home to 2 indigenous languages that are now extinct. In addition, 25 living non-indigenous languages are established within the country. In formal education, 7 indigenous languages are used as languages of instruction.'
 
         """
```

### Comparing `pyetho-1.2/src/pyetho.egg-info/PKG-INFO` & `pyetho-2.0/src/pyetho.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetho
-Version: 1.2
+Version: 2.0
 Summary: Exploration of World Languages
 Home-page: https://github.com/i18nsolutionspy/Pyetho
 Author: SathishKumar paramasivam Et al.
 Author-email: i18nsolutionspy@gmail.com
 Project-URL: Bug Tracker, https://github.com/i18nsolutionspy/Pyetho/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,18 +16,21 @@
   <img src="https://raw.githubusercontent.com/i18nsolutionspy/Ethnologue/632e1a61f13aaf91e2e93766ef9d6bc91cceb1e4/logo.svg"><br>
 </div>
 
 ## Pyetho: A library for Python to all the country languages in the world
 This is a Language and Country Information Package. In order to know the details of all the languages in the world, **i18n Solutions Salem**, have developed this package based on the interest of integrating the languages of the world to python developers.
 
 
-> Developers : Bhuvaneshwara Ragavendra.S <bhuvaneshwararagavendra@gmail.com> Roseline Santhiya.M <rosekevin30@gmail.com> Archana.K.T <archanakt.cse@gmail.com> Vinoth Kumar <vinobe000@gmail.com>
+>Developers : Bhuvaneshwara Ragavendra.S <bhuvaneshwararagavendra@gmail.com> Roseline Santhiya.M <rosekevin30@gmail.com> Archana.K.T <archanakt.cse@gmail.com>
 
+>Version 1.0 Developer: Vinoth Kumar <vinobe000@gmail.com>
 
-> Contributors : Varsha A, JayaShree S, Kaviya V, Abinaya V, Janani S, Karthika P, Anandhi P, Hemalatha R, Sri Sakthi Priya T, Nidha Basreen M, Anu R, Megala V, Mogana Priya S
+>version 2.0 Contributors : Arthi G
+
+>Version 1.0 Contributors : Varsha A, JayaShree S, Kaviya V, Abinaya V, Janani S, Karthika P, Anandhi P, Hemalatha R, Sri Sakthi Priya T, Nidha Basreen M, Anu R, Megala V, Mogana Priya S
 
 
 
 Installation
 ============
 ```python
 pip install pyetho
@@ -49,19 +52,19 @@
 -> Retrieve details about countries and their attributes such as continent, area, commencement year, and more.
 
 -> Access language-specific information, including summaries, language codes, populations, and families.
 
 -> Explore language families and their associated languages across various countries.
 
 ```python
-1        
+1
 country_list()
 Get a list of all country names in the dataset.
 
-2        
+2
 country_summary(country_name="India")
 Get a summary of the specified country.
 
 3
 country_officialname(country_name="India")
 Get the official name of the specified country.
 
@@ -176,7 +179,9 @@
 https://www.ethnologue.com/
 
 https://www.worldometers.info/
 
 https://www.worlddata.info/
 
 https://www.wikipedia.org/
+
+https://www.officeholidays.com/
```

