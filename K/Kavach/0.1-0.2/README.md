# Comparing `tmp/Kavach-0.1.tar.gz` & `tmp/Kavach-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kavach-0.1.tar", last modified: Tue Apr  9 17:00:44 2024, max compression
+gzip compressed data, was "Kavach-0.2.tar", last modified: Wed Apr 10 13:08:06 2024, max compression
```

## Comparing `Kavach-0.1.tar` & `Kavach-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-09 17:00:44.708003 Kavach-0.1/
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-09 17:00:44.705552 Kavach-0.1/Kavach/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       50 2024-04-08 09:32:22.000000 Kavach-0.1/Kavach/__init__.py
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-09 17:00:44.706576 Kavach-0.1/Kavach/data/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)    61101 2024-04-08 08:57:15.000000 Kavach-0.1/Kavach/data/logo.png
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     3002 2024-04-09 16:27:38.000000 Kavach-0.1/Kavach/gradio_app.py
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2013 2024-04-09 16:28:35.000000 Kavach-0.1/Kavach/utils.py
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-09 17:00:44.706450 Kavach-0.1/Kavach.egg-info/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-04-09 17:00:44.000000 Kavach-0.1/Kavach.egg-info/PKG-INFO
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      327 2024-04-09 17:00:44.000000 Kavach-0.1/Kavach.egg-info/SOURCES.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        1 2024-04-09 17:00:44.000000 Kavach-0.1/Kavach.egg-info/dependency_links.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       60 2024-04-09 17:00:44.000000 Kavach-0.1/Kavach.egg-info/entry_points.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       33 2024-04-09 17:00:44.000000 Kavach-0.1/Kavach.egg-info/requires.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       13 2024-04-09 17:00:44.000000 Kavach-0.1/Kavach.egg-info/top_level.txt
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       29 2024-04-09 16:26:05.000000 Kavach-0.1/MANIFEST.in
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-04-09 17:00:44.707812 Kavach-0.1/PKG-INFO
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2513 2024-04-08 09:16:45.000000 Kavach-0.1/README.md
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       38 2024-04-09 17:00:44.708159 Kavach-0.1/setup.cfg
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      427 2024-04-09 16:26:17.000000 Kavach-0.1/setup.py
-drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-09 17:00:44.707482 Kavach-0.1/tests/
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-08 09:17:41.000000 Kavach-0.1/tests/__init__.py
--rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     1739 2024-04-09 16:27:46.000000 Kavach-0.1/tests/test_utils.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.050175 Kavach-0.2/
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.047957 Kavach-0.2/Kavach/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       50 2024-04-08 09:32:22.000000 Kavach-0.2/Kavach/__init__.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.048804 Kavach-0.2/Kavach/data/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)    61101 2024-04-08 08:57:15.000000 Kavach-0.2/Kavach/data/logo.png
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     3076 2024-04-10 13:02:59.000000 Kavach-0.2/Kavach/gradio_app.py
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2013 2024-04-09 16:28:35.000000 Kavach-0.2/Kavach/utils.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.048694 Kavach-0.2/Kavach.egg-info/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/PKG-INFO
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      327 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/SOURCES.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        1 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/dependency_links.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       60 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/entry_points.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       33 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/requires.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       13 2024-04-10 13:08:06.000000 Kavach-0.2/Kavach.egg-info/top_level.txt
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       29 2024-04-09 16:26:05.000000 Kavach-0.2/MANIFEST.in
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      164 2024-04-10 13:08:06.049981 Kavach-0.2/PKG-INFO
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     2513 2024-04-08 09:16:45.000000 Kavach-0.2/README.md
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)       38 2024-04-10 13:08:06.050215 Kavach-0.2/setup.cfg
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)      427 2024-04-10 13:07:36.000000 Kavach-0.2/setup.py
+drwxr-xr-x   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-10 13:08:06.049764 Kavach-0.2/tests/
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)        0 2024-04-08 09:17:41.000000 Kavach-0.2/tests/__init__.py
+-rw-r--r--   0 rukaiyahhasan   (501) staff       (20)     1739 2024-04-09 16:27:46.000000 Kavach-0.2/tests/test_utils.py
```

### Comparing `Kavach-0.1/Kavach/data/logo.png` & `Kavach-0.2/Kavach/data/logo.png`

 * *Files identical despite different names*

### Comparing `Kavach-0.1/Kavach/gradio_app.py` & `Kavach-0.2/Kavach/gradio_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,17 +58,18 @@
                         "Ticket Channel",
                         "First Response Time",
                         "Time to Resolution",
                         "Customer Satisfaction Rating"], type="pandas", col_count=17)
             button = gr.Button("Export")
             csv = gr.File(interactive=False, visible=False)
 
-        button.click(export_csv, csv_display, csv)
+        button.click(export_csv, csv_output, csv)
         # csv_input.change(display_csv, inputs=csv_input, outputs=csv_display)
         csv_input.change(gradio_interface, inputs=csv_input, outputs=csv_output)
+        csv_input.change(modify_csv, inputs=csv_input, outputs=csv_output)
 
 # Launch the Gradio app
     demo.dependencies[0]["show_progress"] = "hidden"
     demo.launch(debug=True)
 
 def main():
     # Collect user input for columns to redact
```

### Comparing `Kavach-0.1/Kavach/utils.py` & `Kavach-0.2/Kavach/utils.py`

 * *Files identical despite different names*

### Comparing `Kavach-0.1/README.md` & `Kavach-0.2/README.md`

 * *Files identical despite different names*

### Comparing `Kavach-0.1/tests/test_utils.py` & `Kavach-0.2/tests/test_utils.py`

 * *Files identical despite different names*

