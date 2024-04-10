# Comparing `tmp/pricedisplay-0.5.1.tar.gz` & `tmp/pricedisplay-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pricedisplay-0.5.1.tar", max compression
+gzip compressed data, was "pricedisplay-0.5.2.tar", max compression
```

## Comparing `pricedisplay-0.5.1.tar` & `pricedisplay-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35148 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/LICENSE.md
--rw-r--r--   0        0        0     1924 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/README.md
--rw-r--r--   0        0        0       29 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/__init__.py
--rw-r--r--   0        0        0       65 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/__main__.py
--rw-r--r--   0        0        0     8357 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/application.py
--rw-r--r--   0        0        0      175 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/config.migrate
--rw-r--r--   0        0        0     3292 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/config.template
--rw-r--r--   0        0        0    11531 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/configparser.py
--rw-r--r--   0        0        0     8075 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/datahandler.py
--rw-r--r--   0        0        0     1217 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/exceptions.py
--rw-r--r--   0        0        0    29390 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pricedisplay/graphics.py
--rw-r--r--   0        0        0      795 2024-01-05 15:13:06.298821 pricedisplay-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2959 1970-01-01 00:00:00.000000 pricedisplay-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/LICENSE.md
+-rw-r--r--   0        0        0     1924 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/README.md
+-rw-r--r--   0        0        0       29 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/__main__.py
+-rw-r--r--   0        0        0     8357 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/application.py
+-rw-r--r--   0        0        0      175 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/config.migrate
+-rw-r--r--   0        0        0     3292 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/config.template
+-rw-r--r--   0        0        0    11531 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/configparser.py
+-rw-r--r--   0        0        0     8075 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/datahandler.py
+-rw-r--r--   0        0        0     1217 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/exceptions.py
+-rw-r--r--   0        0        0    29483 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pricedisplay/graphics.py
+-rw-r--r--   0        0        0      795 2024-04-10 10:20:12.690641 pricedisplay-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2959 1970-01-01 00:00:00.000000 pricedisplay-0.5.2/PKG-INFO
```

### Comparing `pricedisplay-0.5.1/LICENSE.md` & `pricedisplay-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/README.md` & `pricedisplay-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/pricedisplay/application.py` & `pricedisplay-0.5.2/pricedisplay/application.py`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/pricedisplay/config.template` & `pricedisplay-0.5.2/pricedisplay/config.template`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/pricedisplay/configparser.py` & `pricedisplay-0.5.2/pricedisplay/configparser.py`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/pricedisplay/datahandler.py` & `pricedisplay-0.5.2/pricedisplay/datahandler.py`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/pricedisplay/exceptions.py` & `pricedisplay-0.5.2/pricedisplay/exceptions.py`

 * *Files identical despite different names*

### Comparing `pricedisplay-0.5.1/pricedisplay/graphics.py` & `pricedisplay-0.5.2/pricedisplay/graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import math
 import sparklines
 import warnings
 
 from .exceptions import MissingOptionError
 from .exceptions import CollectionSizeError, WindowSizeError, WindowPositionError
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 class Point:
 	"""Represents a point on the terminal screen."""
 	
 	y = 0
 	x = 0
 	pos = ( 0,0 )
@@ -163,20 +163,25 @@
 	
 	def _CurrentHourIndex( self, hoursInDay ):
 		"""Takes into account the daylight saving time change, when finding the index for the current hour."""
 		
 		now = datetime.datetime.now()
 		utc = datetime.datetime.utcnow()
 		
-		timezone = ( now.hour - utc.hour ) % 24
-		offset = timezone - self._normalTimezone
-		delta = hoursInDay - 24
+		# account for dst change
+		if hoursInDay != 24:
+			timezone = ( now.hour - utc.hour ) % 24
+			offset = timezone - self._normalTimezone
+		
+			delta = hoursInDay - 24
+			index = now.hour + (abs(delta) + delta)/2 - offset
+			index = int( index )
 		
-		index = now.hour + (abs(delta) + delta)/2 - offset
-		index = int( index )
+		else:
+			index = int( now.hour )
 		
 		return index
 	
 	def _PriceToColor( self, price ):
 		"""Finds a curses color pair based on the given price (low, medium, high)."""
 		
 		if price == None:
```

### Comparing `pricedisplay-0.5.1/pyproject.toml` & `pricedisplay-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pricedisplay"
-version = "0.5.1"
+version = "0.5.2"
 authors = ["Lumi"]
 description = "Terminal display for the Finnish power price."
 readme = "README.md"
 license = "LICENSE.md"
 repository = "https://github.com/YukiNeko-hime/pricedisplay"
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `pricedisplay-0.5.1/PKG-INFO` & `pricedisplay-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pricedisplay
-Version: 0.5.1
+Version: 0.5.2
 Summary: Terminal display for the Finnish power price.
 Home-page: https://github.com/YukiNeko-hime/pricedisplay
 License: LICENSE.md
 Author: Lumi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
```

