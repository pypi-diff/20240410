# Comparing `tmp/misleep-0.1.2b0.tar.gz` & `tmp/misleep-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.1.2b0.tar", last modified: Tue Apr  9 10:20:00 2024, max compression
+gzip compressed data, was "misleep-0.1.3b0.tar", last modified: Wed Apr 10 04:05:33 2024, max compression
```

## Comparing `misleep-0.1.2b0.tar` & `misleep-0.1.3b0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.233956 misleep-0.1.2b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.2b0/LICENSE
--rw-rw-rw-   0        0        0     1132 2024-04-09 10:20:00.233956 misleep-0.1.2b0/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-03-05 06:34:51.000000 misleep-0.1.2b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.208956 misleep-0.1.2b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.2b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.2b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      507 2024-04-09 10:19:29.000000 misleep-0.1.2b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.217957 misleep-0.1.2b0/misleep/gui/
--rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.2b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.2b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.2b0/misleep/gui/label_dialog.py
--rw-rw-rw-   0        0        0    52174 2024-04-09 10:15:25.000000 misleep-0.1.2b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.220956 misleep-0.1.2b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.2b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.2b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      473 2024-04-08 05:55:10.000000 misleep-0.1.2b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-08 05:54:04.000000 misleep-0.1.2b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.2b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.223956 misleep-0.1.2b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.2b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    23842 2024-04-08 05:30:54.000000 misleep-0.1.2b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-08 05:30:56.000000 misleep-0.1.2b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.2b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.224957 misleep-0.1.2b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.2b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.2b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     4431 2024-04-08 12:27:01.000000 misleep-0.1.2b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.226956 misleep-0.1.2b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.2b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.2b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.2b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.227956 misleep-0.1.2b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.2b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.2b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/utils/only4gui.py
--rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.2b0/misleep/utils/others.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.229956 misleep-0.1.2b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.2b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.2b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.2b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.2b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.211957 misleep-0.1.2b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     1132 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1340 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 10:20:00.000000 misleep-0.1.2b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:20:00.233956 misleep-0.1.2b0/setup.cfg
--rw-rw-rw-   0        0        0     2057 2024-04-09 10:19:18.000000 misleep-0.1.2b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:20:00.232957 misleep-0.1.2b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.2b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.2b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.2b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.2b0/test/test_show.py
--rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.2b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.2b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.2b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:33.010472 misleep-0.1.3b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.3b0/LICENSE
+-rw-rw-rw-   0        0        0     2920 2024-04-10 04:05:33.009591 misleep-0.1.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2024-04-10 04:00:34.000000 misleep-0.1.3b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:32.986740 misleep-0.1.3b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.3b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.3b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      507 2024-04-10 03:45:37.000000 misleep-0.1.3b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:32.993740 misleep-0.1.3b0/misleep/gui/
+-rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.3b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.3b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.3b0/misleep/gui/label_dialog.py
+-rw-rw-rw-   0        0        0    52563 2024-04-10 03:38:55.000000 misleep-0.1.3b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:32.996590 misleep-0.1.3b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.3b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.3b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      473 2024-04-08 05:55:10.000000 misleep-0.1.3b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-08 05:54:04.000000 misleep-0.1.3b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.3b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:32.998590 misleep-0.1.3b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.3b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    23842 2024-04-08 05:30:54.000000 misleep-0.1.3b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-08 05:30:56.000000 misleep-0.1.3b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.3b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:33.000590 misleep-0.1.3b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.3b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.3b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     4431 2024-04-08 12:27:01.000000 misleep-0.1.3b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:33.001591 misleep-0.1.3b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.3b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.3b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.3b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:33.003590 misleep-0.1.3b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.3b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.3b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/utils/only4gui.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.3b0/misleep/utils/others.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:33.005590 misleep-0.1.3b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.3b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.3b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.3b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.3b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:32.988740 misleep-0.1.3b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     2920 2024-04-10 04:05:32.000000 misleep-0.1.3b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1340 2024-04-10 04:05:32.000000 misleep-0.1.3b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 04:05:32.000000 misleep-0.1.3b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-10 04:05:32.000000 misleep-0.1.3b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 04:05:32.000000 misleep-0.1.3b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 04:05:33.010472 misleep-0.1.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     2125 2024-04-10 04:05:25.000000 misleep-0.1.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:05:33.008591 misleep-0.1.3b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.3b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.3b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.3b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.3b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.3b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.3b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.3b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.1.2b0/LICENSE` & `misleep-0.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/about.py` & `misleep-0.1.3b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/label_dialog.py` & `misleep-0.1.3b0/misleep/gui/label_dialog.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/main_window.py` & `misleep-0.1.3b0/misleep/gui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,24 @@
             )
             self.signal_ax[i + 1].xaxis.set_ticks([])
             self.signal_ax[i + 1].yaxis.set_ticks([])
             self.signal_ax[i + 1].set_ylabel(
                 f"{self.midata.channels[each]}\n\n{y_lim:.2e}"
             )
 
+            if self.show_duration < 300:
+                for pos_ in range(0, self.show_duration, 5):
+                    self.signal_ax[i + 1].axvline(
+                        pos_ * self.midata.sf[each],
+                        color="green",
+                        linestyle="--",
+                        linewidth=1,
+                        alpha=0.5
+                    )
+
             # plot label
             for state in sleep_state:
                 self.signal_ax[i + 1].fill_between(
                     range(
                         int(state[0] * self.midata.sf[each]),
                         int((state[1] + 1) * self.midata.sf[each]),
                     ),
```

### Comparing `misleep-0.1.2b0/misleep/gui/resources/entire_logo.png` & `misleep-0.1.3b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/resources/logo.png` & `misleep-0.1.3b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/resources/misleep.py` & `misleep-0.1.3b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/spec_window.py` & `misleep-0.1.3b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/thread.py` & `misleep-0.1.3b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/uis/about_ui.py` & `misleep-0.1.3b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.1.3b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.1.3b0/misleep/gui/uis/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.1.3b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/gui/utils.py` & `misleep-0.1.3b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/io/annotation_io.py` & `misleep-0.1.3b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/io/base.py` & `misleep-0.1.3b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/io/signal_io.py` & `misleep-0.1.3b0/misleep/io/signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/preprocessing/spectral.py` & `misleep-0.1.3b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/utils/annotation.py` & `misleep-0.1.3b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/utils/only4gui.py` & `misleep-0.1.3b0/misleep/utils/only4gui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/utils/signals.py` & `misleep-0.1.3b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/viz/hypnogram.py` & `misleep-0.1.3b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/viz/signals.py` & `misleep-0.1.3b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep/viz/spectral.py` & `misleep-0.1.3b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/misleep.egg-info/SOURCES.txt` & `misleep-0.1.3b0/misleep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/setup.py` & `misleep-0.1.3b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.1.2 Beta"
+VERSION = "0.1.3 Beta"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
@@ -59,20 +59,22 @@
 if __name__ == "__main__":
     setup(
         name=DISTNAME,
         author=MAINTAINER,
         author_email=MAINTAINER_EMAIL,
         maintainer=MAINTAINER,
         maintainer_email=MAINTAINER_EMAIL,
+        long_description_content_type = 'text/markdown',
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         license=LICENSE,
         url=URL,
         version=VERSION,
         download_url=DOWNLOAD_URL,
         install_requires=INSTALL_REQUIRES,
         data_files=DATA_FILES,
         include_package_data=True,
         packages=find_packages(),
         package_dir={'misleep': 'misleep'},
         classifiers=CLASSIFIERS,
+        
     )
```

### Comparing `misleep-0.1.2b0/test/test_midata.py` & `misleep-0.1.3b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/test/test_signal_io.py` & `misleep-0.1.3b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/test/test_signals_viz.py` & `misleep-0.1.3b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.2b0/test/test_spectral_viz.py` & `misleep-0.1.3b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

