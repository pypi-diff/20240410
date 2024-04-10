# Comparing `tmp/accmt-0.0.8.tar.gz` & `tmp/accmt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-0.0.8.tar", last modified: Tue Apr  9 04:35:00 2024, max compression
+gzip compressed data, was "accmt-0.0.9.tar", last modified: Wed Apr 10 06:54:47 2024, max compression
```

## Comparing `accmt-0.0.8.tar` & `accmt-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.198601 accmt-0.0.8/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    12238 2024-04-09 04:35:00.196594 accmt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11517 2024-04-09 02:52:21.000000 accmt-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      837 2024-04-09 04:35:00.200597 accmt-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.142363 accmt-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.167593 accmt-0.0.8/src/accmt/
--rw-rw-rw-   0        0        0       96 2024-04-09 02:00:37.000000 accmt-0.0.8/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    23923 2024-04-09 04:33:12.000000 accmt-0.0.8/src/accmt/accmt.py
--rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-0.0.8/src/accmt/collate_fns.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.8/src/accmt/config.py
-drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.195594 accmt-0.0.8/src/accmt.egg-info/
--rw-rw-rw-   0        0        0    12238 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.353626 accmt-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    12238 2024-04-10 06:54:47.351626 accmt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11517 2024-04-09 02:52:21.000000 accmt-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      837 2024-04-10 06:54:47.356627 accmt-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.299448 accmt-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.320440 accmt-0.0.9/src/accmt/
+-rw-rw-rw-   0        0        0       96 2024-04-09 02:00:37.000000 accmt-0.0.9/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    23935 2024-04-10 06:51:48.000000 accmt-0.0.9/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-0.0.9/src/accmt/collate_fns.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.9/src/accmt/config.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.349629 accmt-0.0.9/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0    12238 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-0.0.8/LICENSE` & `accmt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-0.0.8/PKG-INFO` & `accmt-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/MartinPC-uls/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/MartinPC-uls/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `accmt-0.0.8/README.md` & `accmt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `accmt-0.0.8/setup.cfg` & `accmt-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 302e 302e 380d 0a61 7574 686f  n = 0.0.8..autho
+00000020: 6e20 3d20 302e 302e 390d 0a61 7574 686f  n = 0.0.9..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
```

### Comparing `accmt-0.0.8/src/accmt/accmt.py` & `accmt-0.0.9/src/accmt/accmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             raise AttributeError("'self.model' needs to be declared in the AcceleratorModule class.")
         
         cfg = read(self.hps_config)
         hps = cfg["hps"]
         optim = hps["optim"]
         schlr = hps["scheduler"] if "scheduler" in hps else None
 
-        if self.model_path is not None:
+        if self.model_path is None:
             self.model_path = cfg["version"]
 
         if self.model_saving:
             os.makedirs(self.model_path, exist_ok=True)
 
         best_train_loss = float("inf")
         best_valid_loss = float("inf")
@@ -330,15 +330,15 @@
                           "Using 'log_every' from HPS config file.")
 
         model, train_dataloader, val_dataloader, optimizer, scheduler = self.accelerator.prepare(
             model, train_dataloader, val_dataloader, optimizer, scheduler
         )
         if scheduler:
             self.accelerator.register_for_checkpointing(scheduler)
-        self.accelerator.init_trackers(cfg["version"])
+        self.accelerator.init_trackers(self.model_path.split("/")[-1])
 
         if self.resume:
             if os.path.exists(self.checkpoint):
                 self.accelerator.load_state(self.checkpoint)
             else:
                 raise FileNotFoundError(f"{self.checkpoint} was not found.")
```

### Comparing `accmt-0.0.8/src/accmt/collate_fns.py` & `accmt-0.0.9/src/accmt/collate_fns.py`

 * *Files identical despite different names*

### Comparing `accmt-0.0.8/src/accmt.egg-info/PKG-INFO` & `accmt-0.0.9/src/accmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/MartinPC-uls/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/MartinPC-uls/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

