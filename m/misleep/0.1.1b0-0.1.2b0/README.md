# Comparing `tmp/misleep-0.1.1b0.tar.gz` & `tmp/misleep-0.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.1.1b0.tar", last modified: Wed Apr  3 09:04:05 2024, max compression
+gzip compressed data, was "misleep-0.1.2b0.tar", last modified: Tue Apr  9 10:20:00 2024, max compression
```

## Comparing `misleep-0.1.1b0.tar` & `misleep-0.1.2b0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.724379 misleep-0.1.1b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.1b0/LICENSE
--rw-rw-rw-   0        0        0     1132 2024-04-03 09:04:05.723214 misleep-0.1.1b0/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-03-05 06:34:51.000000 misleep-0.1.1b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.697214 misleep-0.1.1b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.1b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.1b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      510 2024-04-03 08:56:33.000000 misleep-0.1.1b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.702214 misleep-0.1.1b0/misleep/gui/
--rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.1b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.1b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.1b0/misleep/gui/label_dialog.py
--rw-rw-rw-   0        0        0    52166 2024-04-03 08:56:06.000000 misleep-0.1.1b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.705213 misleep-0.1.1b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.1b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.1b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      473 2024-04-02 10:20:22.000000 misleep-0.1.1b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     4092 2024-04-01 13:45:14.000000 misleep-0.1.1b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.1b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.709214 misleep-0.1.1b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.1b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    23842 2024-04-03 02:14:41.000000 misleep-0.1.1b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     4468 2024-03-31 07:18:43.000000 misleep-0.1.1b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.1b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.711214 misleep-0.1.1b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.1b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.1b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     5908 2024-04-03 09:01:34.000000 misleep-0.1.1b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.713214 misleep-0.1.1b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.1b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.1b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.1b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.718213 misleep-0.1.1b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.1b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.1b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/utils/only4gui.py
--rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.1b0/misleep/utils/others.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.719214 misleep-0.1.1b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.1b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.1b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.1b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.699214 misleep-0.1.1b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     1132 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1340 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:04:05.724379 misleep-0.1.1b0/setup.cfg
--rw-rw-rw-   0        0        0     2057 2024-04-03 09:04:01.000000 misleep-0.1.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.722214 misleep-0.1.1b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.1b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.1b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.1b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.1b0/test/test_show.py
--rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.1b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.1b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.1b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.233956 misleep-0.1.2b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.2b0/LICENSE
+-rw-rw-rw-   0        0        0     1132 2024-04-09 10:20:00.233956 misleep-0.1.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2024-03-05 06:34:51.000000 misleep-0.1.2b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.208956 misleep-0.1.2b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.2b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.2b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      507 2024-04-09 10:19:29.000000 misleep-0.1.2b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.217957 misleep-0.1.2b0/misleep/gui/
+-rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.2b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.2b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.2b0/misleep/gui/label_dialog.py
+-rw-rw-rw-   0        0        0    52174 2024-04-09 10:15:25.000000 misleep-0.1.2b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.220956 misleep-0.1.2b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.2b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.2b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      473 2024-04-08 05:55:10.000000 misleep-0.1.2b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-08 05:54:04.000000 misleep-0.1.2b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.2b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.223956 misleep-0.1.2b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.2b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    23842 2024-04-08 05:30:54.000000 misleep-0.1.2b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-08 05:30:56.000000 misleep-0.1.2b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.2b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.224957 misleep-0.1.2b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.2b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.2b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     4431 2024-04-08 12:27:01.000000 misleep-0.1.2b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.226956 misleep-0.1.2b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.2b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.2b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.2b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.227956 misleep-0.1.2b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.2b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.2b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/utils/only4gui.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.2b0/misleep/utils/others.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.229956 misleep-0.1.2b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.2b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.2b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.2b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.211957 misleep-0.1.2b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     1132 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1340 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:20:00.233956 misleep-0.1.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     2057 2024-04-09 10:19:18.000000 misleep-0.1.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.232957 misleep-0.1.2b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.2b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.2b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.2b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.2b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.2b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.2b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.2b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.1.1b0/LICENSE` & `misleep-0.1.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/PKG-INFO` & `misleep-0.1.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.1b0
+Version: 0.1.2b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.1.1b0/misleep/gui/about.py` & `misleep-0.1.2b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/label_dialog.py` & `misleep-0.1.2b0/misleep/gui/label_dialog.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/main_window.py` & `misleep-0.1.2b0/misleep/gui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 import copy
 import datetime
 import configparser
 import json
 
 import numpy as np
-from PyQt5.QtCore import QCoreApplication, Qt, QStringListModel
+from PyQt5.QtCore import QCoreApplication, Qt, QStringListModel, QTimer
 from PyQt5.QtGui import QKeySequence
 from PyQt5.QtWidgets import QMainWindow, QFileDialog, QMessageBox, QAction, QShortcut
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
 from misleep.preprocessing.spectral import spectrogram
 from misleep.io.base import MiData, MiAnnotation
@@ -76,20 +76,14 @@
         }
         self.current_spectrogram_idx = 0
         self.spectrogram_percentile = 99.7
         self.show_midata = None
         self.epoch_length = 5
         self.ac_time = None
 
-        # Default marker label and start_end label for label dialog
-        # self.marker_label = ['Injection', 'Pat', 'Add water', 'label', 'label']
-        # self.start_end_label = ['Spindle', 'Slow wave activity', 'start_end_label']
-        # self.marker_label = json.loads(self.config['gui']['MARKERS'])
-        # self.start_end_label = json.loads(self.config['gui']['STARTEND'])
-
         # Signal area figure
         self.signal_figure = plt.figure()
         self.signal_ax = self.signal_figure.subplots()
         self.signal_figure.set_tight_layout(True)
         self.signal_figure.tight_layout(h_pad=0, w_pad=0)
         self.signal_figure.subplots_adjust(hspace=0)  # Adjust subplots
         self.signal_canvas = FigureCanvas(self.signal_figure)
@@ -113,23 +107,27 @@
             self.current_sec, color="gray", alpha=0.8
         )
 
         # Initial params for widgets
         self.channel_slm = QStringListModel()
 
         # Initial about dialog and spec window
-        self.about_dialog = about_dialog(version=json.loads(self.config['gui']['version']),
-                                         update_time=json.loads(self.config['gui']['updatetime']))
+        self.about_dialog = about_dialog(version=self.config['gui']['version'],
+                                         update_time=self.config['gui']['updatetime'])
         self.spec_window = SpecWindow()
         # Initial label dialog
         self.label_dialog = label_dialog(config=self.config)
 
         # Check wheher operation done and saved or not
         self.is_saved = True
 
+        # Timer to auto save annotations
+        self.save_timer = QTimer()
+        self.save_timer.timeout.connect(self.auto_save)
+
         self.init_qt()
 
     def init_qt(self):
         """Initial actions for qt widgets"""
         # Set triggers for toolBars
         self.AboutBar.actionTriggered[QAction].connect(self.about_bar_dispatcher)
         self.LoadBar.actionTriggered[QAction].connect(self.load_bar_dispatcher)
@@ -370,14 +368,17 @@
         self.SignalArea.setWidget(self.signal_canvas)
         self.HypnoArea.setWidget(self.hypo_canvas)
 
         self.redraw_all(second=0)
         self.clear_refresh(clf=False)
         self.change_Bts_status(False)
 
+        # save timer start, 5 mins
+        self.save_timer.start(60*5*1000)
+
     def reset_sec_limit(self):
         """When show duration changes, change the limitation of 
         ScrollerBar, DateTimeEdit, SecondSpin
         """
         self.ScrollerBar.setRange(0, self.total_seconds-self.show_duration)
         self.SecondSpin.setRange(0, self.total_seconds-self.show_duration)
 
@@ -562,15 +563,15 @@
                 ) : int(
                     (self.current_sec + self.show_duration)
                     * self.midata.sf[self.current_spectrogram_idx]
                 )
             ],
             sf=self.midata.sf[self.current_spectrogram_idx],
             step=1,
-            window=1,
+            window=5,
             norm=True,
         )
         cmap = plt.cm.get_cmap("jet")
 
         self.signal_ax[0].set_xticks([])
         self.signal_ax[0].set_ylim(0, 30)
         self.signal_ax[0].set_ylabel(
@@ -1117,29 +1118,29 @@
         signal_data = self.midata.signals[channel][
             int(self.start_end[0]*self.midata.sf[channel]) : 
             int(self.start_end[1]*self.midata.sf[channel])
         ]
         
         freq, psd = spectrum(signal=signal_data,
                              sf=self.midata.sf[channel],
-                             relative=False)
+                             relative=True)
         
         f, t, Sxx = spectrogram(signal=signal_data,
                                 sf=self.midata.sf[channel],
                                 step=1, window=5, norm=True)
 
         bandPower = band_power(psd=psd, freq=freq, 
                                bands=[[0.5, 4, 'delta'], [4, 9, 'theta']])
         
         ratio = bandPower['delta'] / bandPower['theta']
         
         self.spec_window.show_(spectrum=[psd, freq], 
                                spectrogram=[f, t, Sxx],
                                percentile_=self.spectrogram_percentile,
-                               ratio=ratio)
+                               ratio=ratio, start_end=self.start_end)
         
         self.spec_window.activateWindow()
         self.spec_window.setWindowState(
                 self.spec_window.windowState() & ~Qt.WindowMinimized | Qt.WindowActive)
         self.spec_window.showNormal()
 
     def set_show_duration(self, type_="Combo"):
@@ -1273,14 +1274,20 @@
         save_thread = SaveThread(file=[self.mianno, self.midata], 
                                  file_path=self.anno_path)
         saved = save_thread.save_anno()
         if saved:
             self.is_saved = True
             QMessageBox.about(self, "Info", "Annotation saved")
         save_thread.quit()
+    
+    def auto_save(self):
+        """Auto save every 5 mins"""
+        if not self.is_saved:
+            self.save_anno()
+        self.save_timer.start(5*60*1000)
 
     def save_config(self, config_dict):
         """Save config"""
         for key, value in config_dict.items():
             self.config.set('gui', key, value)
         save_thread = SaveThread(file=self.config, 
                                  file_path='./misleep/config.ini')
```

### Comparing `misleep-0.1.1b0/misleep/gui/resources/entire_logo.png` & `misleep-0.1.2b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/resources/logo.png` & `misleep-0.1.2b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/resources/misleep.py` & `misleep-0.1.2b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/thread.py` & `misleep-0.1.2b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/uis/about_ui.py` & `misleep-0.1.2b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.1.2b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.1.2b0/misleep/gui/uis/main_window_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file './misleep/gui/uis/main_window.ui'
+# Form implementation generated from reading ui file 'misleep/gui/uis/main_window.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
@@ -386,8 +386,8 @@
         self.AboutBar.setWindowTitle(_translate("MiSleep", "toolBar"))
         self.actionLoad_Data.setText(_translate("MiSleep", "Load Data"))
         self.actionLoad_Annotation.setText(_translate("MiSleep", "Load Annotation"))
         self.actionShow.setText(_translate("MiSleep", "Show"))
         self.actionSave_data.setText(_translate("MiSleep", "Save Data"))
         self.actionSave_Annotation.setText(_translate("MiSleep", "Save Annotation"))
         self.actionAbout.setText(_translate("MiSleep", "About"))
-from misleep.gui.resources import misleep
+from misleep.gui.resources import misleep
```

### Comparing `misleep-0.1.1b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.1.2b0/misleep/gui/uis/spec_window_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file './misleep/gui/uis/spec_window.ui'
+# Form implementation generated from reading ui file 'misleep/gui/uis/spec_window.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_spec_window(object):
     def setupUi(self, spec_window):
         spec_window.setObjectName("spec_window")
-        spec_window.resize(860, 600)
-        spec_window.setMinimumSize(QtCore.QSize(860, 600))
+        spec_window.resize(932, 900)
+        spec_window.setMinimumSize(QtCore.QSize(860, 800))
         icon = QtGui.QIcon()
         icon.addPixmap(QtGui.QPixmap(":/logo/logo.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         spec_window.setWindowIcon(icon)
         self.centralwidget = QtWidgets.QWidget(spec_window)
         self.centralwidget.setObjectName("centralwidget")
         self.gridLayout = QtWidgets.QGridLayout(self.centralwidget)
         self.gridLayout.setObjectName("gridLayout")
@@ -33,28 +33,28 @@
         self.DeltaThetaRatioLabel = QtWidgets.QLabel(self.groupBox)
         self.DeltaThetaRatioLabel.setObjectName("DeltaThetaRatioLabel")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.DeltaThetaRatioLabel)
         self.SpectrumScrollArea = QtWidgets.QScrollArea(self.groupBox)
         self.SpectrumScrollArea.setWidgetResizable(True)
         self.SpectrumScrollArea.setObjectName("SpectrumScrollArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 820, 214))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 892, 364))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
         self.SpectrumScrollArea.setWidget(self.scrollAreaWidgetContents)
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.SpanningRole, self.SpectrumScrollArea)
         self.gridLayout.addWidget(self.groupBox, 0, 0, 1, 1)
         self.groupBox_2 = QtWidgets.QGroupBox(self.centralwidget)
         self.groupBox_2.setObjectName("groupBox_2")
         self.formLayout_2 = QtWidgets.QFormLayout(self.groupBox_2)
         self.formLayout_2.setObjectName("formLayout_2")
         self.SpectrogramScrollArea = QtWidgets.QScrollArea(self.groupBox_2)
         self.SpectrogramScrollArea.setWidgetResizable(True)
         self.SpectrogramScrollArea.setObjectName("SpectrogramScrollArea")
         self.scrollAreaWidgetContents_2 = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents_2.setGeometry(QtCore.QRect(0, 0, 820, 214))
+        self.scrollAreaWidgetContents_2.setGeometry(QtCore.QRect(0, 0, 892, 364))
         self.scrollAreaWidgetContents_2.setObjectName("scrollAreaWidgetContents_2")
         self.SpectrogramScrollArea.setWidget(self.scrollAreaWidgetContents_2)
         self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.SpanningRole, self.SpectrogramScrollArea)
         self.SpectrogramSaveBt = QtWidgets.QPushButton(self.groupBox_2)
         self.SpectrogramSaveBt.setObjectName("SpectrogramSaveBt")
         self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.SpectrogramSaveBt)
         self.gridLayout.addWidget(self.groupBox_2, 1, 0, 1, 1)
```

### Comparing `misleep-0.1.1b0/misleep/gui/utils.py` & `misleep-0.1.2b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/io/annotation_io.py` & `misleep-0.1.2b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/io/base.py` & `misleep-0.1.2b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/io/signal_io.py` & `misleep-0.1.2b0/misleep/io/signal_io.py`

 * *Files 23% similar despite different names*

```diff
@@ -84,44 +84,15 @@
     
         except Exception:
             # If old version misleep data
             signals = raw_data
             channels = [f'ch{each + 1}' for each in range(raw_data.shape[0])]
             sf = [305. for _ in range(raw_data.shape[0])]
             time = datetime.datetime.now().strftime("%Y%m%d-%H:%M:%S")
-            return MiData(signals=signals, channels=channels, sf=sf, time=time)
-
-        
-    
-    # raw_data = list(loadmat(data_path).values())[-1]
-    # try:
-    #     # Whether save with python, because python has no 'cell' type
-    #     _ = raw_data['save']
-    #     channels = list(raw_data['channels'][0, 0])
-    #     channels = [each.strip() for each in channels]
-    #     sf = list(raw_data['sf'][0, 0][0].astype(float))
-    #     signals = [raw_data[each][0, 0][0] for each in channels]
-    #     time = raw_data['time'][0, 0][0]
-
-    #     return MiData(signals=signals, channels=channels, sf=sf, time=time)
-    # except Exception:
-    #     try:
-    #         channels = [item for each in raw_data['channels'][0][0][0] for item in each]
-    #         channels = [each.strip() for each in channels]
-    #         sf = list(raw_data['sf'][0, 0][0].astype(float))
-    #         signals = [raw_data[each][0, 0][0] for each in channels]
-    #         time = raw_data['time'][0, 0][0]
-    #         return MiData(signals=signals, channels=channels, sf=sf, time=time)
-    #     except Exception:
-    #         # If matlab data is not a struct, or have no channel field, will arise this
-    #         signals = raw_data
-    #         channels = [f'ch{each + 1}' for each in range(raw_data.shape[0])]
-    #         sf = [305. for _ in range(raw_data.shape[0])]
-    #         time = datetime.datetime.now().strftime("%Y%m%d-%H:%M:%S")
-    #         return MiData(signals=signals, channels=channels, sf=sf, time=time)       
+            return MiData(signals=signals, channels=channels, sf=sf, time=time)  
 
 
 def write_mat(signals, channels, sf, time, mat_file=None):
     """
     Write data to .mat file
 
     Parameters
```

### Comparing `misleep-0.1.1b0/misleep/preprocessing/spectral.py` & `misleep-0.1.2b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/utils/annotation.py` & `misleep-0.1.2b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/utils/only4gui.py` & `misleep-0.1.2b0/misleep/utils/only4gui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/utils/signals.py` & `misleep-0.1.2b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/viz/hypnogram.py` & `misleep-0.1.2b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/viz/signals.py` & `misleep-0.1.2b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep/viz/spectral.py` & `misleep-0.1.2b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/misleep.egg-info/PKG-INFO` & `misleep-0.1.2b0/misleep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.1b0
+Version: 0.1.2b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.1.1b0/misleep.egg-info/SOURCES.txt` & `misleep-0.1.2b0/misleep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/setup.py` & `misleep-0.1.2b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.1.1 Beta"
+VERSION = "0.1.2 Beta"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
```

### Comparing `misleep-0.1.1b0/test/test_midata.py` & `misleep-0.1.2b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/test/test_signal_io.py` & `misleep-0.1.2b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/test/test_signals_viz.py` & `misleep-0.1.2b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.1b0/test/test_spectral_viz.py` & `misleep-0.1.2b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

