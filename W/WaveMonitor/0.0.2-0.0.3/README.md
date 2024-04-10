# Comparing `tmp/WaveMonitor-0.0.2.tar.gz` & `tmp/WaveMonitor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveMonitor-0.0.2.tar", last modified: Tue Mar 12 08:35:55 2024, max compression
+gzip compressed data, was "WaveMonitor-0.0.3.tar", last modified: Wed Apr 10 16:08:11 2024, max compression
```

## Comparing `WaveMonitor-0.0.2.tar` & `WaveMonitor-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 08:35:55.785329 WaveMonitor-0.0.2/
--rw-rw-rw-   0        0        0     1066 2024-01-29 11:15:32.000000 WaveMonitor-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       12 2024-02-08 08:53:23.000000 WaveMonitor-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2042 2024-03-12 08:35:55.784318 WaveMonitor-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1468 2024-03-12 08:10:36.000000 WaveMonitor-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 08:35:55.783317 WaveMonitor-0.0.2/WaveMonitor.egg-info/
--rw-rw-rw-   0        0        0     2042 2024-03-12 08:35:55.000000 WaveMonitor-0.0.2/WaveMonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-03-12 08:35:55.000000 WaveMonitor-0.0.2/WaveMonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 08:35:55.000000 WaveMonitor-0.0.2/WaveMonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-03-12 08:35:55.000000 WaveMonitor-0.0.2/WaveMonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-12 08:35:55.000000 WaveMonitor-0.0.2/WaveMonitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-12 08:35:55.781317 WaveMonitor-0.0.2/assets/
--rw-rw-rw-   0        0        0    11131 2024-02-08 08:53:23.000000 WaveMonitor-0.0.2/assets/icon.png
--rw-rw-rw-   0        0        0    36100 2024-03-12 08:05:54.000000 WaveMonitor-0.0.2/assets/snapshot.png
--rw-rw-rw-   0        0        0    10884 2024-03-12 08:04:40.000000 WaveMonitor-0.0.2/assets/style.qss
--rw-rw-rw-   0        0        0    19261 2024-02-08 09:18:55.000000 WaveMonitor-0.0.2/assets/style2.qss
--rw-rw-rw-   0        0        0      640 2024-03-12 08:35:27.000000 WaveMonitor-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 08:35:55.785329 WaveMonitor-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 16:08:11.118450 WaveMonitor-0.0.3/
+-rw-rw-rw-   0        0        0     1066 2024-01-29 11:15:32.000000 WaveMonitor-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       12 2024-02-08 08:53:23.000000 WaveMonitor-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2069 2024-04-10 16:08:11.118450 WaveMonitor-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1495 2024-04-10 16:00:48.000000 WaveMonitor-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 16:08:11.102841 WaveMonitor-0.0.3/WaveMonitor.egg-info/
+-rw-rw-rw-   0        0        0     2069 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-10 16:08:11.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 16:08:11.102841 WaveMonitor-0.0.3/assets/
+-rw-rw-rw-   0        0        0    11131 2024-02-08 08:53:23.000000 WaveMonitor-0.0.3/assets/icon.png
+-rw-rw-rw-   0        0        0    36100 2024-03-12 08:05:54.000000 WaveMonitor-0.0.3/assets/snapshot.png
+-rw-rw-rw-   0        0        0    10884 2024-03-12 08:04:40.000000 WaveMonitor-0.0.3/assets/style.qss
+-rw-rw-rw-   0        0        0    19261 2024-02-08 09:18:55.000000 WaveMonitor-0.0.3/assets/style2.qss
+-rw-rw-rw-   0        0        0      640 2024-04-10 15:48:57.000000 WaveMonitor-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:08:11.118450 WaveMonitor-0.0.3/setup.cfg
```

### Comparing `WaveMonitor-0.0.2/LICENSE` & `WaveMonitor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.2/PKG-INFO` & `WaveMonitor-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveMonitor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple GUI for monitoring waveforms.
 Author-email: Qiujv <qiujv@outlook.com>
 Project-URL: Homepage, https://github.com/Qiujv/WaveMonitor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -25,15 +25,15 @@
 The `WaveMonitor` class is the main interface. It provides methods for adding and removing waveforms from the plot, clearing the plot, and etc.
 
 In GUI, right click to show the menu. Keyboard shortcuts are also supported.
 
 # Installation
 
 ```bash
-pip install wave_monitor
+pip install WaveMonitor
 ```
 
 or install from source.
 
 ```bash
 pip install git+https://github.com/Qiujv/WaveMonitor.git
 ```
@@ -42,27 +42,28 @@
 Avoid calling `clear` if you only want to update the plot. It is more efficient to update the plot with `add_wfm`.
 
 ```python
 from wave_monitor import WaveMonitor
 import numpy as np
 
 monitor = WaveMonitor()
-monitor.find_or_run_monitor_window()
 monitor.autoscale()
 # monitor.clear()
 
 t = np.linspace(0, 1, 1_000_001)  # 1m pts ~= 1ms for 1GSa/s.
-n = 20  # Okay with 20.
+n = 20
 i_waves = [np.cos(2 * np.pi * f * t) for f in range(1, n + 1)]
 q_waves = [np.sin(2 * np.pi * f * t) for f in range(1, n + 1)]
 
 for i, (i_wave, q_wave) in enumerate(zip(i_waves, q_waves)):
-    monitor.add_wfm(f"wave_{i%15}", t, [i_wave, q_wave])
+    monitor.add_wfm(f"wave_{i}", t, [i_wave, q_wave])
 monitor.autoscale()
 
+monitor.add_wfm("wave_1", t, [i_waves[-1], q_waves[-1]])  # Replaces previous wfm.
+
 monitor.remove_wfm("wave_10")
 
 ```
 
 # Thanks
 
 This project is derived from [WaveViewer](https://github.com/kahojyun/wave-viewer).
```

### Comparing `WaveMonitor-0.0.2/README.md` & `WaveMonitor-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 The `WaveMonitor` class is the main interface. It provides methods for adding and removing waveforms from the plot, clearing the plot, and etc.
 
 In GUI, right click to show the menu. Keyboard shortcuts are also supported.
 
 # Installation
 
 ```bash
-pip install wave_monitor
+pip install WaveMonitor
 ```
 
 or install from source.
 
 ```bash
 pip install git+https://github.com/Qiujv/WaveMonitor.git
 ```
@@ -24,27 +24,28 @@
 Avoid calling `clear` if you only want to update the plot. It is more efficient to update the plot with `add_wfm`.
 
 ```python
 from wave_monitor import WaveMonitor
 import numpy as np
 
 monitor = WaveMonitor()
-monitor.find_or_run_monitor_window()
 monitor.autoscale()
 # monitor.clear()
 
 t = np.linspace(0, 1, 1_000_001)  # 1m pts ~= 1ms for 1GSa/s.
-n = 20  # Okay with 20.
+n = 20
 i_waves = [np.cos(2 * np.pi * f * t) for f in range(1, n + 1)]
 q_waves = [np.sin(2 * np.pi * f * t) for f in range(1, n + 1)]
 
 for i, (i_wave, q_wave) in enumerate(zip(i_waves, q_waves)):
-    monitor.add_wfm(f"wave_{i%15}", t, [i_wave, q_wave])
+    monitor.add_wfm(f"wave_{i}", t, [i_wave, q_wave])
 monitor.autoscale()
 
+monitor.add_wfm("wave_1", t, [i_waves[-1], q_waves[-1]])  # Replaces previous wfm.
+
 monitor.remove_wfm("wave_10")
 
 ```
 
 # Thanks
 
 This project is derived from [WaveViewer](https://github.com/kahojyun/wave-viewer).
```

### Comparing `WaveMonitor-0.0.2/WaveMonitor.egg-info/PKG-INFO` & `WaveMonitor-0.0.3/WaveMonitor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaveMonitor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple GUI for monitoring waveforms.
 Author-email: Qiujv <qiujv@outlook.com>
 Project-URL: Homepage, https://github.com/Qiujv/WaveMonitor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -25,15 +25,15 @@
 The `WaveMonitor` class is the main interface. It provides methods for adding and removing waveforms from the plot, clearing the plot, and etc.
 
 In GUI, right click to show the menu. Keyboard shortcuts are also supported.
 
 # Installation
 
 ```bash
-pip install wave_monitor
+pip install WaveMonitor
 ```
 
 or install from source.
 
 ```bash
 pip install git+https://github.com/Qiujv/WaveMonitor.git
 ```
@@ -42,27 +42,28 @@
 Avoid calling `clear` if you only want to update the plot. It is more efficient to update the plot with `add_wfm`.
 
 ```python
 from wave_monitor import WaveMonitor
 import numpy as np
 
 monitor = WaveMonitor()
-monitor.find_or_run_monitor_window()
 monitor.autoscale()
 # monitor.clear()
 
 t = np.linspace(0, 1, 1_000_001)  # 1m pts ~= 1ms for 1GSa/s.
-n = 20  # Okay with 20.
+n = 20
 i_waves = [np.cos(2 * np.pi * f * t) for f in range(1, n + 1)]
 q_waves = [np.sin(2 * np.pi * f * t) for f in range(1, n + 1)]
 
 for i, (i_wave, q_wave) in enumerate(zip(i_waves, q_waves)):
-    monitor.add_wfm(f"wave_{i%15}", t, [i_wave, q_wave])
+    monitor.add_wfm(f"wave_{i}", t, [i_wave, q_wave])
 monitor.autoscale()
 
+monitor.add_wfm("wave_1", t, [i_waves[-1], q_waves[-1]])  # Replaces previous wfm.
+
 monitor.remove_wfm("wave_10")
 
 ```
 
 # Thanks
 
 This project is derived from [WaveViewer](https://github.com/kahojyun/wave-viewer).
```

### Comparing `WaveMonitor-0.0.2/assets/icon.png` & `WaveMonitor-0.0.3/assets/icon.png`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.2/assets/snapshot.png` & `WaveMonitor-0.0.3/assets/snapshot.png`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.2/assets/style.qss` & `WaveMonitor-0.0.3/assets/style.qss`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.2/assets/style2.qss` & `WaveMonitor-0.0.3/assets/style2.qss`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.2/pyproject.toml` & `WaveMonitor-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "WaveMonitor"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
     "msgpack",
     "msgpack_numpy",
     "numpy",
     "pyqtgraph",
     "PySide6",
 ]
```

