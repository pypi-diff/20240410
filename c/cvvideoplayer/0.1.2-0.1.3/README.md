# Comparing `tmp/cvvideoplayer-0.1.2.tar.gz` & `tmp/cvvideoplayer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvvideoplayer-0.1.2.tar", last modified: Wed Apr  3 19:16:34 2024, max compression
+gzip compressed data, was "cvvideoplayer-0.1.3.tar", last modified: Wed Apr 10 15:03:22 2024, max compression
```

## Comparing `cvvideoplayer-0.1.2.tar` & `cvvideoplayer-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.563959 cvvideoplayer-0.1.2/
--rw-rw-rw-   0        0        0     1067 2024-03-17 19:44:52.000000 cvvideoplayer-0.1.2/License.txt
--rw-rw-rw-   0        0        0      727 2024-04-03 19:16:34.562738 cvvideoplayer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4900 2024-04-03 18:20:34.000000 cvvideoplayer-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.529934 cvvideoplayer-0.1.2/cvvideoplayer/
--rw-rw-rw-   0        0        0      187 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.545668 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/
--rw-rw-rw-   0        0        0      303 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/__init__.py
--rw-rw-rw-   0        0        0     4127 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_bbox_plotter.py
--rw-rw-rw-   0        0        0     2606 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_frame_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.552248 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
--rw-rw-rw-   0        0        0     1868 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py
--rw-rw-rw-   0        0        0     1108 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
--rw-rw-rw-   0        0        0     1387 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/detections_csv_plotter.py
--rw-rw-rw-   0        0        0     3363 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_reader.py
--rw-rw-rw-   0        0        0     1404 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/recorder.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.559695 cvvideoplayer-0.1.2/cvvideoplayer/utils/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/__init__.py
--rw-rw-rw-   0        0        0      863 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/bbox_utils.py
--rw-rw-rw-   0        0        0     2233 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/drawing_utils.py
--rw-rw-rw-   0        0        0     3277 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/video_player_utils.py
--rw-rw-rw-   0        0        0     3012 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/windows_vk_dict.py
--rw-rw-rw-   0        0        0    12573 2024-04-03 19:08:49.000000 cvvideoplayer-0.1.2/cvvideoplayer/video_player.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.538570 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/
--rw-rw-rw-   0        0        0      727 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 19:16:34.563959 cvvideoplayer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-04-03 19:16:26.000000 cvvideoplayer-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.561692 cvvideoplayer-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-03-18 19:35:21.000000 cvvideoplayer-0.1.2/tests/test_video_player_basic_functionality.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.404600 cvvideoplayer-0.1.3/
+-rw-rw-rw-   0        0        0     1067 2024-03-17 19:44:52.000000 cvvideoplayer-0.1.3/License.txt
+-rw-rw-rw-   0        0        0      727 2024-04-10 15:03:22.402371 cvvideoplayer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4979 2024-04-10 14:54:37.000000 cvvideoplayer-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.350108 cvvideoplayer-0.1.3/cvvideoplayer/
+-rw-rw-rw-   0        0        0      202 2024-04-10 14:54:37.000000 cvvideoplayer-0.1.3/cvvideoplayer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.372202 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/
+-rw-rw-rw-   0        0        0      303 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/__init__.py
+-rw-rw-rw-   0        0        0     4127 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_bbox_plotter.py
+-rw-rw-rw-   0        0        0     2606 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_frame_editor.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.383983 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
+-rw-rw-rw-   0        0        0     2373 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
+-rw-rw-rw-   0        0        0     1868 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py
+-rw-rw-rw-   0        0        0     1108 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
+-rw-rw-rw-   0        0        0     1387 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/detections_csv_plotter.py
+-rw-rw-rw-   0        0        0     3363 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_reader.py
+-rw-rw-rw-   0        0        0     1404 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/recorder.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.397074 cvvideoplayer-0.1.3/cvvideoplayer/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/__init__.py
+-rw-rw-rw-   0        0        0      863 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/bbox_utils.py
+-rw-rw-rw-   0        0        0     2233 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/drawing_utils.py
+-rw-rw-rw-   0        0        0     3277 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/video_player_utils.py
+-rw-rw-rw-   0        0        0     3012 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/windows_vk_dict.py
+-rw-rw-rw-   0        0        0    13039 2024-04-06 17:07:18.000000 cvvideoplayer-0.1.3/cvvideoplayer/video_player.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.361073 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/
+-rw-rw-rw-   0        0        0      727 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 15:03:22.404600 cvvideoplayer-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      931 2024-04-10 14:56:05.000000 cvvideoplayer-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.400279 cvvideoplayer-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-18 19:35:21.000000 cvvideoplayer-0.1.3/tests/test_video_player_basic_functionality.py
```

### Comparing `cvvideoplayer-0.1.2/License.txt` & `cvvideoplayer-0.1.3/License.txt`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/PKG-INFO` & `cvvideoplayer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvvideoplayer
-Version: 0.1.2
+Version: 0.1.3
 Summary: moduler multi purpose video player for python
 Author: Daniel Tomer
 Author-email: danieltomer1@gmail.com
 Project-URL: Homepage, https://github.com/danieltomer1/CVVideoPlayer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `cvvideoplayer-0.1.2/README.md` & `cvvideoplayer-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<div align="center"><img src="assets/logo.png" width="150"></div>
+<div align="center"><img src="assets/logo.jpeg" width="250"></div>
 
 ## Introduction
 CV video player is a Python-based customizable video player that helps computer vision practitioners
 to develop, analyze, and debug their video-related algorithms and models.
 
 
 ## Installation
@@ -30,28 +30,27 @@
         pass
 
     @abc.abstractmethod
     def __len__(self) -> int:
         pass
 ```
 
-A ready-to-use LocalFrameReader is already implemented and can be used to read 
+A ready-to-use `LocalFrameReader` is already implemented and can be used to read 
 any local video file or folder containing the frames as images 
 (as long as there is a number in the name of the image files indicating their order).
 
 </details>
 
 
 <details>
-<summary>FrameEditor class</summary>
+<summary>BaseFrameEditor class</summary>
 
-You can add any number of FrameEditors for the player to apply using
-the VideoPlayer method "add_frame_editor". A FrameEditor is a class
-that needs to inherit BaseFrameEditor and implement 
-the following abstract methods:
+You can add any number of frame editores for the player to apply using
+the VideoPlayer method `add_frame_editor`. A frame editor is an instance of a class
+that inherit `BaseFrameEditor` and implements the following abstract methods:
 
 ```python
 class BaseFrameEditor(ABC):
     @property
     @abstractmethod
     def edit_after_resize(self) -> bool:
         """
@@ -77,43 +76,45 @@
 
 </details>
 
 
 <details>
 <summary>KeyFunction dataclass</summary>
 
-A KeyFunction defines a mapping between a key and a function with an added description of the
-function's purpose. You can add a new KeyFunction in two ways:
-- Using the video player's method "register_key_function"
-- Using a FrameEditors property "key_functions_to_register" which returns 
+A `KeyFunction` defines a mapping between a key and a function with an added description of the
+function's purpose. You can add a new `KeyFunction` in two ways:
+- Using the video player's method `register_key_function`
+- Using a FrameEditors property `key_functions_to_register` which returns 
 a list of KeyFunctions that will be registered once the FrameEditor is added 
 to the player
 
 ### default key functions:
 These are used by the player and cannot be overwritten:
 - "space bar": Play/Pause video
 - "right": Next frame
 - "left": Previous frame
 - "ctrl+right": 10 frames forward
 - "ctrl+left": 10 frames back
 - "ctrl+shift+right": 50 frames forward
 - "ctrl+shift+left": 50 frames back
-- "+": Increase frame size
-- "-": Decrease frame size
+- "+": Double play speed
+- "-": half play speed
+- "ctrl++": Increase frame size
+- "ctrl+-": Decrease frame size
 
 </details>
 
 <details>
 <summary>Recorder class</summary>
 
-The recorder class is an object that can be used to record whatever is being
+The Recorder class can be used to record whatever is being
 played in the video player. By default, the video will be saved in an "outputs" folder
-which will be created in the CWD.
+which will be automatically created in the CWD.
 
-To use the recorder:
+To use the Recorder:
 ```python
 from cvvideoplayer import VideoPlayer, Recorder
 video_player = VideoPlayer(
     recorder=Recorder(),
     **other_video_player_kwargs
 )
 ```
@@ -144,8 +145,8 @@
 In this example, we initiate a very basic video player that will play "example_video.mp4" with added basic
 frame editors:
 - Frame number printer (disable/enable with **ctrl+f**): Prints the current frame number and original frame resolution in the top left corner
 - Histogram Equalizer (disable/enable with **ctrl+h**): Preforms histogram equalization on the image
 - Frame Normalizer: Allows the user to print the current frame's intensities histogram and also
 set a dynamic range for the image (see printed keymap at runtime for the used keyboard shortcuts).
 
-Check out the run_video_player.py which also uses the DetectionsCsvPlotter to plot precalculated detection
+Check out the `run_video_player.py` which also uses the DetectionsCsvPlotter to plot precalculated detection
```

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_bbox_plotter.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_bbox_plotter.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_frame_editor.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_frame_editor.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/detections_csv_plotter.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/detections_csv_plotter.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/frame_reader.py` & `cvvideoplayer-0.1.3/cvvideoplayer/frame_reader.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/recorder.py` & `cvvideoplayer-0.1.3/cvvideoplayer/recorder.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/utils/bbox_utils.py` & `cvvideoplayer-0.1.3/cvvideoplayer/utils/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/utils/drawing_utils.py` & `cvvideoplayer-0.1.3/cvvideoplayer/utils/drawing_utils.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/utils/video_player_utils.py` & `cvvideoplayer-0.1.3/cvvideoplayer/utils/video_player_utils.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/utils/windows_vk_dict.py` & `cvvideoplayer-0.1.3/cvvideoplayer/utils/windows_vk_dict.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer/video_player.py` & `cvvideoplayer-0.1.3/cvvideoplayer/video_player.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         for key, key_function in self._keymap.items():
             if key_function.description:
                 print(f"{key}: {key_function.description}")
         print("***********************************")
 
     def _play_continuously(self) -> None:
         while self._ui_queue.empty() and self._play:
-            self._next_frame(self._play_speed)
+            self._next_frame(self._play_speed) if self._play_speed > 0 else self._prev_frame(-self._play_speed)
             self._show_current_frame()
 
     def _resize_frame(self, frame) -> np.ndarray:
         width, height = get_screen_adjusted_frame_size(
             screen_size=self._screen_size,
             frame_width=frame.shape[1],
             frame_height=frame.shape[0],
@@ -252,38 +252,50 @@
     def _change_frame_resize_factor(self, change_by: float) -> None:
         self._resize_factor = max(0.1, min(1.0, self._resize_factor + change_by))
 
     def _play_pause(self):
         self._play = not self._play
         self._play_continuously()
 
-    def _double_play_speed(self) -> None:
-        self._play_speed = min(16, self._play_speed * 2)
+    def _increase_play_speed(self) -> None:
+        if self._play_speed == -1:
+            self._play_speed = 1
+        elif self._play_speed < -1:
+            self._play_speed = min(-1, self._play_speed // 2)
+        else:
+            self._play_speed = min(16, self._play_speed * 2)
+
         self._play = True
         self._play_continuously()
 
-    def _half_play_speed(self) -> None:
-        self._play_speed = max(1, self._play_speed // 2)
+    def _decrease_play_speed(self) -> None:
+        if self._play_speed == 1:
+            self._play_speed = -1
+        elif self._play_speed > 1:
+            self._play_speed = max(1, self._play_speed // 2)
+        else:
+            self._play_speed = max(-16, self._play_speed * 2)
+
         self._play = True
         self._play_continuously()
 
     def _add_default_key_functions(self) -> None:
         default_key_functions = [
             KeyFunction("space", func=lambda: self._play_pause(), description="Play/Pause video"),
             KeyFunction("right", func=lambda: self._next_frame(1), description="Next frame"),
             KeyFunction("left", func=lambda: self._prev_frame(1), description="Previous frame"),
             KeyFunction("ctrl+right", func=lambda: self._next_frame(10), description="10 frames forward"),
             KeyFunction("ctrl+left", func=lambda: self._prev_frame(10), description="10 frames back"),
             KeyFunction("ctrl+shift+right", func=lambda: self._next_frame(50), description="50 frames forward"),
             KeyFunction("ctrl+shift+left", func=lambda: self._prev_frame(50), description="50 frames back"),
             KeyFunction("ctrl++", func=lambda: self._change_frame_resize_factor(0.1), description="Increase frame size"),
             KeyFunction("ctrl+-", lambda: self._change_frame_resize_factor(-0.1), description="Decrease frame size"),
-            KeyFunction("+", lambda: self._double_play_speed(), description="Double play speed"),
-            KeyFunction("shift++", lambda: self._double_play_speed(), description=""),
-            KeyFunction("-", lambda: self._half_play_speed(), description="Half play speed"),
+            KeyFunction("+", lambda: self._increase_play_speed(), description="Increase play speed"),
+            KeyFunction("shift++", lambda: self._increase_play_speed(), description=""),
+            KeyFunction("-", lambda: self._decrease_play_speed(), description="Decrease play speed"),
         ]
 
         for key_function in default_key_functions:
             self.register_key_function(key_function)
 
     def _handle_keyboard_press(self, key_without_modifiers) -> None:
         if (
```

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer.egg-info/PKG-INFO` & `cvvideoplayer-0.1.3/cvvideoplayer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvvideoplayer
-Version: 0.1.2
+Version: 0.1.3
 Summary: moduler multi purpose video player for python
 Author: Daniel Tomer
 Author-email: danieltomer1@gmail.com
 Project-URL: Homepage, https://github.com/danieltomer1/CVVideoPlayer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `cvvideoplayer-0.1.2/cvvideoplayer.egg-info/SOURCES.txt` & `cvvideoplayer-0.1.3/cvvideoplayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.2/setup.py` & `cvvideoplayer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cvvideoplayer",
-    version="0.1.2",
+    version="0.1.3",
     author="Daniel Tomer",
     author_email="danieltomer1@gmail.com",
     description="moduler multi purpose video player for python",
     long_description=(
         "CV video player is a Python-based customizable video player that helps"
         " computer vision practitioners to develop, analyze and debug their video"
         " related algorithms and model."
```

