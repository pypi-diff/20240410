# Comparing `tmp/fissure-engine-1.0.2.tar.gz` & `tmp/fissure-engine-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissure-engine-1.0.2.tar", last modified: Fri Apr  5 16:44:50 2024, max compression
+gzip compressed data, was "fissure-engine-1.0.3.tar", last modified: Wed Apr 10 21:10:59 2024, max compression
```

## Comparing `fissure-engine-1.0.2.tar` & `fissure-engine-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 16:44:50.602913 fissure-engine-1.0.2/
--rw-rw-rw-   0        0        0      485 2024-04-05 16:44:50.601912 fissure-engine-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 16:44:50.594914 fissure-engine-1.0.2/fissure_engine/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:22:54.000000 fissure-engine-1.0.2/fissure_engine/__init__.py
--rw-rw-rw-   0        0        0    75962 2024-03-27 20:54:24.000000 fissure-engine-1.0.2/fissure_engine/common.py
--rw-rw-rw-   0        0        0    17669 2024-04-05 16:44:15.000000 fissure-engine-1.0.2/fissure_engine/fissure_engine.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:44:50.600913 fissure-engine-1.0.2/fissure_engine.egg-info/
--rw-rw-rw-   0        0        0      485 2024-04-05 16:44:50.000000 fissure-engine-1.0.2/fissure_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-05 16:44:50.000000 fissure-engine-1.0.2/fissure_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:44:50.000000 fissure-engine-1.0.2/fissure_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-05 16:44:50.000000 fissure-engine-1.0.2/fissure_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 16:44:50.000000 fissure-engine-1.0.2/fissure_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 16:44:50.602913 fissure-engine-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      749 2024-04-05 16:44:46.000000 fissure-engine-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:10:59.436918 fissure-engine-1.0.3/
+-rw-rw-rw-   0        0        0      485 2024-04-10 21:10:59.435920 fissure-engine-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 21:10:59.428388 fissure-engine-1.0.3/fissure_engine/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:22:54.000000 fissure-engine-1.0.3/fissure_engine/__init__.py
+-rw-rw-rw-   0        0        0    75962 2024-03-27 20:54:24.000000 fissure-engine-1.0.3/fissure_engine/common.py
+-rw-rw-rw-   0        0        0    17876 2024-04-10 21:09:47.000000 fissure-engine-1.0.3/fissure_engine/fissure_engine.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:10:59.434920 fissure-engine-1.0.3/fissure_engine.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 21:10:59.436918 fissure-engine-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-04-10 21:09:47.000000 fissure-engine-1.0.3/setup.py
```

### Comparing `fissure-engine-1.0.2/fissure_engine/common.py` & `fissure-engine-1.0.3/fissure_engine/common.py`

 * *Files identical despite different names*

### Comparing `fissure-engine-1.0.2/fissure_engine/fissure_engine.py` & `fissure-engine-1.0.3/fissure_engine/fissure_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
             field_formats (list): List of tuples. Each tuple contains a field name and a format string.
             display_type (str): Type of display for the expiry field.
             emoji_dict (dict): A dictionary mapping fissure type short identifiers and eras to emojis.
 
         Returns:
             dict: A dictionary where each key is a field name and the corresponding value is a list of all values for that field from the list of Fissures, formatted according to the format string.
         """
-
         preprocess_functions = {
             "{era}": lambda
                 fissure: f"{get_fissure_type_identifier(fissure.fissure_type, emoji_dict)} {emoji_dict.get(fissure.era, '') if emoji_dict else ''} {fissure.era}",
             "{expiry}": lambda fissure: self.format_time_remaining(fissure.expiry, display_type)
         }
 
         def preprocess_format_string(format_string, fissure):
@@ -146,27 +145,29 @@
 
         # Sort fissures by fissure type in the order of normal, steel path, void storms
         sorted_fissures = sorted(fissures, key=lambda f: (f.fissure_type != self.FISSURE_TYPE_NORMAL,
                                                           f.fissure_type == self.FISSURE_TYPE_STEEL_PATH,
                                                           f.fissure_type == self.FISSURE_TYPE_VOID_STORMS))
 
         result = {}
-        for field_name, format_string in field_formats:
-            result[field_name] = []
-            prev_fissure_type = None
-
-            for fissure in sorted_fissures:
-                if fissure.fissure_type != prev_fissure_type:
-                    if prev_fissure_type is not None:
-                        for field in result.values():
-                            field.append("")
-                    prev_fissure_type = fissure.fissure_type
+        for field_name, _ in field_formats:
+            result[field_name] = [[]]  # Initialize with a list that contains an empty list for the first fissure type
+
+        prev_fissure_type = None
+
+        for fissure in sorted_fissures:
+            if fissure.fissure_type != prev_fissure_type:
+                if prev_fissure_type is not None:
+                    for field in result.values():
+                        field.append([])  # Start a new list for the new fissure type
+                prev_fissure_type = fissure.fissure_type
 
+            for field_name, format_string in field_formats:
                 formatted_value = preprocess_format_string(format_string, fissure).format(**fissure.__dict__)
-                result[field_name].append(formatted_value)
+                result[field_name][-1].append(formatted_value)  # Append to the last list for the current fissure type
 
         return result
 
     @staticmethod
     def parse_fissure(type, data, data2="N/A"):
         if isinstance(fissure_parser[type][data], str) or isinstance(fissure_parser[type][data], int):
             return fissure_parser[type][data]
@@ -358,15 +359,15 @@
         get_emoji = (lambda x: emoji_dict.get(x, x)) if emoji_dict else (lambda x: x)
 
         expiries = []
 
         # Find the soonest expiry and append it to expiries list
         try:
             soonest_expiry = min(last_expiries[fissure_type].items(), key=lambda x: x[1])
-            next_reset_string = (f"Next reset is {soonest_expiry[0]} "
+            next_reset_string = (f"Next reset: {soonest_expiry[0]} "
                                  f"{self.format_time_remaining(soonest_expiry[1], display_type=display_type)}")
         except ValueError:
             next_reset_string = "No fissures found."
 
         expiries.append(next_reset_string)
 
         expiries += [f"{get_emoji(era)} {self.format_time_remaining(expiry, display_type=display_type)}"
```

### Comparing `fissure-engine-1.0.2/setup.py` & `fissure-engine-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'Engine for getting fissure information in Warframe.'
 LONG_DESCRIPTION = 'Engine for getting the current fissures for Warframe in a dictionary object.'
 
 
 setup(
     name='fissure-engine',
     version=VERSION,
```

