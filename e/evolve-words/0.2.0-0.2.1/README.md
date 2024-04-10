# Comparing `tmp/evolve-words-0.2.0.tar.gz` & `tmp/evolve-words-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolve-words-0.2.0.tar", last modified: Wed Apr 10 08:50:28 2024, max compression
+gzip compressed data, was "evolve-words-0.2.1.tar", last modified: Wed Apr 10 11:22:43 2024, max compression
```

## Comparing `evolve-words-0.2.0.tar` & `evolve-words-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 08:50:28.321301 evolve-words-0.2.0/
--rw-r--r--   0 davep      (501) staff       (20)     3020 2024-04-10 08:50:28.321230 evolve-words-0.2.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     1667 2023-10-31 20:55:24.000000 evolve-words-0.2.0/README.md
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 08:50:28.320151 evolve-words-0.2.0/evolve_words/
--rw-r--r--   0 davep      (501) staff       (20)      508 2023-11-03 17:15:35.000000 evolve-words-0.2.0/evolve_words/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      222 2023-10-29 21:48:27.000000 evolve-words-0.2.0/evolve_words/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)    15319 2024-04-10 08:48:09.000000 evolve-words-0.2.0/evolve_words/app.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2023-10-31 20:30:32.000000 evolve-words-0.2.0/evolve_words/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 08:50:28.320950 evolve-words-0.2.0/evolve_words.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     3020 2024-04-10 08:50:28.000000 evolve-words-0.2.0/evolve_words.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      344 2024-04-10 08:50:28.000000 evolve-words-0.2.0/evolve_words.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-10 08:50:28.000000 evolve-words-0.2.0/evolve_words.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       59 2024-04-10 08:50:28.000000 evolve-words-0.2.0/evolve_words.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       39 2024-04-10 08:50:28.000000 evolve-words-0.2.0/evolve_words.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       13 2024-04-10 08:50:28.000000 evolve-words-0.2.0/evolve_words.egg-info/top_level.txt
--rw-r--r--   0 davep      (501) staff       (20)      124 2023-10-31 20:28:47.000000 evolve-words-0.2.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1545 2024-04-10 08:50:28.321608 evolve-words-0.2.0/setup.cfg
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 11:22:43.535212 evolve-words-0.2.1/
+-rw-r--r--   0 davep      (501) staff       (20)     3020 2024-04-10 11:22:43.535153 evolve-words-0.2.1/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     1667 2023-10-31 20:55:24.000000 evolve-words-0.2.1/README.md
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 11:22:43.534119 evolve-words-0.2.1/evolve_words/
+-rw-r--r--   0 davep      (501) staff       (20)      508 2024-04-10 11:22:06.000000 evolve-words-0.2.1/evolve_words/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      476 2024-04-10 11:20:04.000000 evolve-words-0.2.1/evolve_words/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)    15355 2024-04-10 11:20:04.000000 evolve-words-0.2.1/evolve_words/app.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2023-10-31 20:30:32.000000 evolve-words-0.2.1/evolve_words/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 11:22:43.534951 evolve-words-0.2.1/evolve_words.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     3020 2024-04-10 11:22:43.000000 evolve-words-0.2.1/evolve_words.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      344 2024-04-10 11:22:43.000000 evolve-words-0.2.1/evolve_words.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-10 11:22:43.000000 evolve-words-0.2.1/evolve_words.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       59 2024-04-10 11:22:43.000000 evolve-words-0.2.1/evolve_words.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       39 2024-04-10 11:22:43.000000 evolve-words-0.2.1/evolve_words.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       13 2024-04-10 11:22:43.000000 evolve-words-0.2.1/evolve_words.egg-info/top_level.txt
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-10-31 20:28:47.000000 evolve-words-0.2.1/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1545 2024-04-10 11:22:43.535487 evolve-words-0.2.1/setup.cfg
```

### Comparing `evolve-words-0.2.0/PKG-INFO` & `evolve-words-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolve-words
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple illustration of mutation aiding evolution
 Home-page: https://github.com/davep/evolve-words
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `evolve-words-0.2.0/README.md` & `evolve-words-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `evolve-words-0.2.0/evolve_words/app.py` & `evolve-words-0.2.1/evolve_words/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,19 @@
     DEFAULT_CSS = """
     IntInput {
         border: none;
         width: 1fr;
         max-width: 10;
         padding: 0;
         margin-top: 1;
-    }
+        height: 1;
 
-    IntInput:focus {
-        border: none;
+        &:focus {
+            border: none;
+        }
     }
     """
 
     def _validate_value(self, value: str) -> str:
         """Validate the value and ensure it's an integer input.
 
         Args:
@@ -276,18 +277,18 @@
         content-align: left middle;
     }
 
     VerticalScroll {
         border-top: panel cornflowerblue 70%;
         height: 1fr;
         background: $panel;
-    }
 
-    VerticalScroll:focus {
-        border-top: panel cornflowerblue;
+        &:focus {
+            border-top: panel cornflowerblue;
+        }
     }
 
     #counts {
         height: 1fr;
     }
 
     SizeCounts, PlotextPlot {
@@ -296,32 +297,32 @@
     }
 
     DataTable {
         background: $panel;
         border: solid cornflowerblue;
         color: $accent-lighten-2;
         height: 1fr;
-    }
 
-    DataTable > .datatable--header {
-        color: $accent-lighten-2;
+        &> .datatable--header {
+            color: $accent-lighten-2;
+        }
     }
 
     PlotextPlot {
         width: 3fr;
     }
 
     Log {
         border-top: panel cornflowerblue 70%;
         height: 1fr;
         background: $panel;
-    }
 
-    Log:focus {
-        border-top: panel cornflowerblue;
+        &:focus {
+            border-top: panel cornflowerblue;
+        }
     }
     """
 
     BINDINGS = [Binding("ctrl+q", "quit", "Quit")]
 
     ENABLE_COMMAND_PALETTE = False
```

### Comparing `evolve-words-0.2.0/evolve_words.egg-info/PKG-INFO` & `evolve-words-0.2.1/evolve_words.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolve-words
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple illustration of mutation aiding evolution
 Home-page: https://github.com/davep/evolve-words
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `evolve-words-0.2.0/setup.cfg` & `evolve-words-0.2.1/setup.cfg`

 * *Files identical despite different names*

