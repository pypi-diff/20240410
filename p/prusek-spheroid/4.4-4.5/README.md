# Comparing `tmp/prusek_spheroid-4.4.tar.gz` & `tmp/prusek_spheroid-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-4.4.tar", last modified: Tue Apr  9 19:07:49 2024, max compression
+gzip compressed data, was "prusek_spheroid-4.5.tar", last modified: Wed Apr 10 08:01:27 2024, max compression
```

## Comparing `prusek_spheroid-4.4.tar` & `prusek_spheroid-4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:07:49.047781 prusek_spheroid-4.4/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-09 19:07:49.047565 prusek_spheroid-4.4/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.4/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:07:49.046564 prusek_spheroid-4.4/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.4/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-4.4/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12428 2024-04-06 18:03:18.000000 prusek_spheroid-4.4/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.4/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.4/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.4/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.4/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.4/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.4/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.4/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.4/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-09 19:07:49.047362 prusek_spheroid-4.4/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-09 19:07:49.000000 prusek_spheroid-4.4/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-09 19:07:49.047827 prusek_spheroid-4.4/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-09 19:07:39.000000 prusek_spheroid-4.4/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 08:01:27.590856 prusek_spheroid-4.5/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 08:01:27.590522 prusek_spheroid-4.5/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.5/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 08:01:27.589001 prusek_spheroid-4.5/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.5/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51479 2024-04-10 07:58:49.000000 prusek_spheroid-4.5/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12428 2024-04-06 18:03:18.000000 prusek_spheroid-4.5/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.5/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.5/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.5/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.5/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.5/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.5/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.5/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.5/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 08:01:27.590294 prusek_spheroid-4.5/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 08:01:27.000000 prusek_spheroid-4.5/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-10 08:01:27.000000 prusek_spheroid-4.5/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-10 08:01:27.000000 prusek_spheroid-4.5/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-10 08:01:27.000000 prusek_spheroid-4.5/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-10 08:01:27.000000 prusek_spheroid-4.5/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-10 08:01:27.590901 prusek_spheroid-4.5/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-10 08:01:18.000000 prusek_spheroid-4.5/setup.py
```

### Comparing `prusek_spheroid-4.4/PKG-INFO` & `prusek_spheroid-4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.4
+Version: 4.5
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-4.4/README.md` & `prusek_spheroid-4.5/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-4.5/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/GUI.py` & `prusek_spheroid-4.5/prusek_spheroid/GUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -596,26 +596,47 @@
         print("Spheroid properties calculated and saved.")
 
 
 class SpheroidSegmentationGUI:
     def __init__(self, selection_dialog):
         self.selection_dialog = selection_dialog
         self.dialog = tk.Toplevel(selection_dialog.root)
-        self.dialog.title("Spheroid Quantification")
+        self.dialog.title("Spheroid Segmentation")
 
-        back_button = tk.Button(self.dialog, text="Back", command=self.go_back)
+        self.canvas = tk.Canvas(self.dialog)
+        self.scrollbar = tk.Scrollbar(self.dialog, orient="vertical", command=self.canvas.yview)
+        self.scrollable_frame = ttk.Frame(self.canvas)
+
+        self.scrollable_frame.bind(
+            "<Configure>",
+            lambda e: self.canvas.configure(
+                scrollregion=self.canvas.bbox("all")
+            )
+        )
+
+        # Step 3: Create a window in the canvas for your scrollable_frame
+        self.canvas.create_window((0, 0), window=self.scrollable_frame, anchor="nw")
+
+        # Step 4: Configure the canvas to use the scrollbar
+        self.canvas.configure(yscrollcommand=self.scrollbar.set)
+
+        # Packing the canvas and scrollbar to the dialog
+        self.canvas.pack(side="left", fill="both", expand=True)
+        self.scrollbar.pack(side="right", fill="y")
+
+        back_button = tk.Button(self.scrollable_frame, text="Back", command=self.go_back)
         back_button.pack(anchor='nw', padx=10, pady=5)
         self.loaded_parameters = None
         self.loaded_method = None
 
         # Adresní sekce
-        self.address_section_label = tk.Label(self.dialog, text="Address Settings", font=("Helvetica", 12, "bold"))
+        self.address_section_label = tk.Label(self.scrollable_frame, text="Address Settings", font=("Helvetica", 12, "bold"))
         self.address_section_label.pack()
 
-        self.notebook = ttk.Notebook(self.dialog)
+        self.notebook = ttk.Notebook(self.scrollable_frame)
         self.coco_tab = ttk.Frame(self.notebook)  # První záložka pro COCO
         self.mask_tab = ttk.Frame(self.notebook)  # Druhá záložka pro masky
 
         self.notebook.add(self.coco_tab, text='Load COCO Annotations')
         self.notebook.add(self.mask_tab, text='Load MASK Annotations')
         self.notebook.pack(expand=True, fill='both')
 
@@ -653,89 +674,89 @@
         self.images_address_label = tk.Label(self.mask_tab, text="Images Directory: Not selected")
         self.images_address_label.pack()
 
         self.masks_annotation_path = tk.StringVar()
         self.image_dataset_path = tk.StringVar()
 
         # File Dialog pro výsledné segmentované obrázky (změna na askdirectory)
-        self.dataset_address_button = tk.Button(self.dialog,
+        self.dataset_address_button = tk.Button(self.scrollable_frame,
                                                 text="Dataset of all images address (folder of images you want to segment)",
                                                 command=lambda: browse_directory(self.dataset_path,
                                                                                  "Selected dataset path",
                                                                                  self.dataset_address_label))
         self.dataset_address_button.pack(side=tk.TOP)
 
         self.dataset_path = tk.StringVar()
 
         # Indikátor pro vyplnění adresy
-        self.dataset_address_label = tk.Label(self.dialog, text="Dataset Directory: Not selected")
+        self.dataset_address_label = tk.Label(self.scrollable_frame, text="Dataset Directory: Not selected")
         self.dataset_address_label.pack()
 
         # File Dialog pro výsledné segmentované obrázky (změna na askdirectory)
-        self.output_address_button = tk.Button(self.dialog,
+        self.output_address_button = tk.Button(self.scrollable_frame,
                                                text="Output address (folder where to save the output)",
                                                command=lambda: browse_directory(self.output_path,
                                                                                 "Selected output path",
                                                                                 self.output_address_label))
         self.output_address_button.pack(side=tk.TOP)
 
         self.output_path = tk.StringVar()
 
         # Indikátor pro vyplnění adresy
-        self.output_address_label = tk.Label(self.dialog, text="Output Directory: Not selected")
+        self.output_address_label = tk.Label(self.scrollable_frame, text="Output Directory: Not selected")
         self.output_address_label.pack()
 
         # Oddělovací čára mezi adresní a metody sekce
-        self.address_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
+        self.address_separator = tk.Frame(self.scrollable_frame, height=2, bd=1, relief=tk.SUNKEN)
         self.address_separator.pack(fill=tk.X, padx=5, pady=5)
 
         # Metodická sekce
-        self.method_section_label = tk.Label(self.dialog, text="Method Settings", font=("Helvetica", 12, "bold"))
+        self.method_section_label = tk.Label(self.scrollable_frame, text="Method Settings", font=("Helvetica", 12, "bold"))
         self.method_section_label.pack()
 
         # Textbox pro název projektu
-        self.project_name_label = tk.Label(self.dialog, text="Project Name:")
+        self.project_name_label = tk.Label(self.scrollable_frame, text="Project Name:")
         self.project_name_label.pack()
-        self.project_name_entry = tk.Entry(self.dialog)
+        self.project_name_entry = tk.Entry(self.scrollable_frame)
         self.project_name_entry.pack()
 
         # Tlačítko pro načtení parametrů z JSON souboru
-        self.load_parameters_button = tk.Button(self.dialog,
+        self.load_parameters_button = tk.Button(self.scrollable_frame,
                                                 text="I already know the parameters (load JSON file with parameters)",
                                                 command=self.load_and_run_parameters)
         self.load_parameters_button.pack()
 
         # Create a frame to contain the label and button
-        self.parameters_frame = tk.Frame(self.dialog)
+        self.parameters_frame = tk.Frame(self.scrollable_frame)
         self.parameters_frame.pack()
 
         # Initially disable the "Parameters loaded" label and the "Cancel" button
         self.parameters_loaded_label = tk.Label(self.parameters_frame, text="Parameters loaded", state=tk.DISABLED)
         self.parameters_loaded_label.pack(side=tk.LEFT)
 
         self.cancel_button = tk.Button(self.parameters_frame, text="Cancel", command=self.cancel_parameters_loaded,
                                        state=tk.DISABLED)
         self.cancel_button.pack(side=tk.LEFT)
 
         # Checkboxy pro výběr metod
-        self.methods_frame = tk.Frame(self.dialog)
+        self.methods_frame = tk.Frame(self.scrollable_frame)
         self.methods_frame.pack()
         self.method_labels = ["Sauvola", "Niblack", "Gaussian"]
 
         self.methods_checkboxes = []
 
         for i, method_label in enumerate(self.method_labels):
             method_var = tk.IntVar()
             method_checkbox = tk.Checkbutton(self.methods_frame, text=method_label, variable=method_var)
             method_checkbox.grid(row=0, column=i, padx=5, pady=5)
 
             self.methods_checkboxes.append((method_checkbox, method_var))
 
         # Textová pole pro zadání parametrů
-        self.parameters_frame = tk.Frame(self.dialog)
+        self.parameters_frame = tk.Frame(self.scrollable_frame)
         self.parameters_frame.pack()
         self.learning_rate_label = tk.Label(self.parameters_frame, text="Learning Rate:")
         self.learning_rate_label.grid(row=0, column=0, padx=5, pady=5)
         self.learning_rate_entry = tk.Entry(self.parameters_frame)
         self.learning_rate_entry.grid(row=0, column=1, padx=5, pady=5)
 
         self.iterations_label = tk.Label(self.parameters_frame, text="Number of Iterations:")
@@ -750,24 +771,24 @@
 
         # Přednastavení hodnot parametrů
         self.learning_rate_entry.insert(0, "0.01")
         self.iterations_entry.insert(0, "50")
         self.batch_size_entry.insert(0, "10")
 
         # Oddělovací čára mezi adresní a metody sekce
-        self.method_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
+        self.method_separator = tk.Frame(self.scrollable_frame, height=2, bd=1, relief=tk.SUNKEN)
         self.method_separator.pack(fill=tk.X, padx=5, pady=5)
 
         # Hole Finding Settings Section
-        self.hole_finding_section_label = tk.Label(self.dialog, text="Hole Finding Settings",
+        self.hole_finding_section_label = tk.Label(self.scrollable_frame, text="Hole Finding Settings",
                                                    font=("Helvetica", 12, "bold"))
         self.hole_finding_section_label.pack()
 
         # Frame for the checkboxes
-        self.hole_finding_frame = tk.Frame(self.dialog)
+        self.hole_finding_frame = tk.Frame(self.scrollable_frame)
         self.hole_finding_frame.pack()
 
         # Variables for the checkboxes
         self.detect_outer_var = tk.IntVar(value=0)
         self.detect_all_var = tk.IntVar(value=0)
         self.view_select_var = tk.IntVar(value=0)
 
@@ -796,21 +817,21 @@
                                                    command=lambda: update_hole_finding_checkboxes(self.view_select_var))
 
         self.detect_outer_checkbox.pack(anchor='w')  # Aligns to the west (left) of the frame
         self.detect_all_checkbox.pack(anchor='w')  # Consistent with the first checkbox
         self.view_select_checkbox.pack(anchor='w')
 
         # Oddělovací čára mezi adresní a metody sekce
-        self.settings_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
+        self.settings_separator = tk.Frame(self.scrollable_frame, height=2, bd=1, relief=tk.SUNKEN)
         self.settings_separator.pack(fill=tk.X, padx=5, pady=5)
 
-        self.other_section_label = tk.Label(self.dialog, text="Other Settings", font=("Helvetica", 12, "bold"))
+        self.other_section_label = tk.Label(self.scrollable_frame, text="Other Settings", font=("Helvetica", 12, "bold"))
         self.other_section_label.pack()
 
-        checkbox_frame = tk.Frame(self.dialog)
+        checkbox_frame = tk.Frame(self.scrollable_frame)
         checkbox_frame.pack()
 
         self.detect_corrupted_var = tk.BooleanVar()
         self.checkbox_detect_corrupted = tk.Checkbutton(checkbox_frame, text="Detect and discard corrupted images",
                                                         variable=self.detect_corrupted_var, onvalue=True,
                                                         offvalue=False)
         self.checkbox_detect_corrupted.pack(side=tk.LEFT)
@@ -826,15 +847,15 @@
         self.calculate_contours_var = tk.BooleanVar()
         self.checkbox_calculate_contours = tk.Checkbutton(checkbox_frame, text="Calculate spheroid properties",
                                                           variable=self.calculate_contours_var,
                                                           onvalue=True, offvalue=False)
         self.checkbox_calculate_contours.pack(side=tk.LEFT)
 
         # Tlačítko pro spuštění
-        self.run_button = tk.Button(self.dialog, text="Run", command=self.run_method)
+        self.run_button = tk.Button(self.scrollable_frame, text="Run", command=self.run_method)
         self.run_button.pack()
 
         self.dialog.protocol("WM_DELETE_WINDOW", self.on_close)
         self.stop_event = threading.Event()
 
     def go_back(self):
         self.dialog.destroy()
```

### Comparing `prusek_spheroid-4.4/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-4.5/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-4.5/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/conversion.py` & `prusek_spheroid-4.5/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/file_management.py` & `prusek_spheroid-4.5/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/image_processing.py` & `prusek_spheroid-4.5/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/merge_directories.py` & `prusek_spheroid-4.5/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/methods.py` & `prusek_spheroid-4.5/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/metrics.py` & `prusek_spheroid-4.5/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-4.5/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-4.5/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.4
+Version: 4.5
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-4.4/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-4.5/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.4/setup.py` & `prusek_spheroid-4.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="4.4",
+    version="4.5",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

