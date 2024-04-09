# Comparing `tmp/audiotimer-0.3.1.tar.gz` & `tmp/audiotimer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiotimer-0.3.1.tar", last modified: Fri Jan 12 13:12:21 2024, max compression
+gzip compressed data, was "audiotimer-0.4.0.tar", last modified: Tue Apr  9 23:00:59 2024, max compression
```

## Comparing `audiotimer-0.3.1.tar` & `audiotimer-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 ranch      (501) staff       (20)        0 2024-01-12 13:12:21.100322 audiotimer-0.3.1/
--rw-r--r--   0 ranch      (501) staff       (20)      923 2024-01-12 13:12:21.100128 audiotimer-0.3.1/PKG-INFO
--rw-r--r--   0 ranch      (501) staff       (20)      739 2024-01-12 12:57:20.000000 audiotimer-0.3.1/README.md
-drwxr-xr-x   0 ranch      (501) staff       (20)        0 2024-01-12 13:12:21.099116 audiotimer-0.3.1/audiotimer/
--rw-r--r--   0 ranch      (501) staff       (20)        0 2024-01-04 21:15:05.000000 audiotimer-0.3.1/audiotimer/__init__.py
--rw-r--r--   0 ranch      (501) staff       (20)     4832 2024-01-12 13:07:14.000000 audiotimer-0.3.1/audiotimer/__main__.py
--rw-r--r--   0 ranch      (501) staff       (20)      825 2024-01-12 12:37:26.000000 audiotimer-0.3.1/audiotimer/flags.py
-drwxr-xr-x   0 ranch      (501) staff       (20)        0 2024-01-12 13:12:21.099896 audiotimer-0.3.1/audiotimer.egg-info/
--rw-r--r--   0 ranch      (501) staff       (20)      923 2024-01-12 13:12:21.000000 audiotimer-0.3.1/audiotimer.egg-info/PKG-INFO
--rw-r--r--   0 ranch      (501) staff       (20)      290 2024-01-12 13:12:21.000000 audiotimer-0.3.1/audiotimer.egg-info/SOURCES.txt
--rw-r--r--   0 ranch      (501) staff       (20)        1 2024-01-12 13:12:21.000000 audiotimer-0.3.1/audiotimer.egg-info/dependency_links.txt
--rw-r--r--   0 ranch      (501) staff       (20)       56 2024-01-12 13:12:21.000000 audiotimer-0.3.1/audiotimer.egg-info/entry_points.txt
--rw-r--r--   0 ranch      (501) staff       (20)       44 2024-01-12 13:12:21.000000 audiotimer-0.3.1/audiotimer.egg-info/requires.txt
--rw-r--r--   0 ranch      (501) staff       (20)       11 2024-01-12 13:12:21.000000 audiotimer-0.3.1/audiotimer.egg-info/top_level.txt
--rw-r--r--   0 ranch      (501) staff       (20)       38 2024-01-12 13:12:21.100361 audiotimer-0.3.1/setup.cfg
--rw-r--r--   0 ranch      (501) staff       (20)      605 2024-01-12 13:12:17.000000 audiotimer-0.3.1/setup.py
+drwxr-xr-x   0 andreasranch   (501) staff       (20)        0 2024-04-09 23:00:59.478520 audiotimer-0.4.0/
+-rw-r--r--   0 andreasranch   (501) staff       (20)     1250 2024-04-09 23:00:59.478409 audiotimer-0.4.0/PKG-INFO
+-rw-r--r--   0 andreasranch   (501) staff       (20)     1082 2024-04-09 19:57:31.000000 audiotimer-0.4.0/README.md
+drwxr-xr-x   0 andreasranch   (501) staff       (20)        0 2024-04-09 23:00:59.477592 audiotimer-0.4.0/audiotimer/
+-rw-r--r--   0 andreasranch   (501) staff       (20)        0 2024-04-09 19:38:59.000000 audiotimer-0.4.0/audiotimer/__init__.py
+-rw-r--r--   0 andreasranch   (501) staff       (20)     5995 2024-04-09 22:37:20.000000 audiotimer-0.4.0/audiotimer/__main__.py
+-rw-r--r--   0 andreasranch   (501) staff       (20)      825 2024-04-09 21:54:50.000000 audiotimer-0.4.0/audiotimer/flags.py
+-rw-r--r--   0 andreasranch   (501) staff       (20)     2060 2024-04-09 22:41:04.000000 audiotimer-0.4.0/audiotimer/helpers.py
+-rw-r--r--   0 andreasranch   (501) staff       (20)     2231 2024-04-09 22:40:18.000000 audiotimer-0.4.0/audiotimer/slack_ping.py
+drwxr-xr-x   0 andreasranch   (501) staff       (20)        0 2024-04-09 23:00:59.478273 audiotimer-0.4.0/audiotimer.egg-info/
+-rw-r--r--   0 andreasranch   (501) staff       (20)     1250 2024-04-09 23:00:59.000000 audiotimer-0.4.0/audiotimer.egg-info/PKG-INFO
+-rw-r--r--   0 andreasranch   (501) staff       (20)      337 2024-04-09 23:00:59.000000 audiotimer-0.4.0/audiotimer.egg-info/SOURCES.txt
+-rw-r--r--   0 andreasranch   (501) staff       (20)        1 2024-04-09 23:00:59.000000 audiotimer-0.4.0/audiotimer.egg-info/dependency_links.txt
+-rw-r--r--   0 andreasranch   (501) staff       (20)       57 2024-04-09 23:00:59.000000 audiotimer-0.4.0/audiotimer.egg-info/entry_points.txt
+-rw-r--r--   0 andreasranch   (501) staff       (20)     5737 2024-04-09 23:00:59.000000 audiotimer-0.4.0/audiotimer.egg-info/requires.txt
+-rw-r--r--   0 andreasranch   (501) staff       (20)       11 2024-04-09 23:00:59.000000 audiotimer-0.4.0/audiotimer.egg-info/top_level.txt
+-rw-r--r--   0 andreasranch   (501) staff       (20)       38 2024-04-09 23:00:59.478563 audiotimer-0.4.0/setup.cfg
+-rw-r--r--   0 andreasranch   (501) staff       (20)     1186 2024-04-09 22:59:00.000000 audiotimer-0.4.0/setup.py
```

### Comparing `audiotimer-0.3.1/PKG-INFO` & `audiotimer-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: audiotimer
-Version: 0.3.1
+Version: 0.4.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.26.3
-Requires-Dist: PyAudio>=0.2.14
-Requires-Dist: pynput>=1.7.6
 
 # Audio timer
 Github: https://github.com/ARanch/audiotimer
 
 This small program starts listening for an audio input on the system microphone. When a set audio level threshold is reached, a timer is started. When the audio level is reduced below the threshold, the timer is stopped after a short countdown, and the timespan is logged.
 
 `python -m pip install audiotimer`
 
 install requirements:
 `pip install -r requirements.txt`
 
+Note: on Mac OS you need [Portaudio](https://www.portaudio.com/) installed, otherwise you will get the error `ERROR: Failed building wheel for PyAudio`. Install it using:
+`brew install portaudio` before installing requirements.
+
 
 run using: 
-`python audiotimer`
+`python -m audiotimer`
 
 see -h flag for run-time options.
 
+Eample usage:
+Run using a treshold of "50" and a buffertime of 30 seconds:
+`python -m audiotimer -t 50 -b 30`
+
 ## Use case
 The program is intended to be used as a way of testing the battery life of battery powered loudspeakers. Set the speaker to play a pink noise at a certain level, and leave a laptop with the speaker to listen for when it dies out. 
+
+
```

### Comparing `audiotimer-0.3.1/README.md` & `audiotimer-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 This small program starts listening for an audio input on the system microphone. When a set audio level threshold is reached, a timer is started. When the audio level is reduced below the threshold, the timer is stopped after a short countdown, and the timespan is logged.
 
 `python -m pip install audiotimer`
 
 install requirements:
 `pip install -r requirements.txt`
 
+Note: on Mac OS you need [Portaudio](https://www.portaudio.com/) installed, otherwise you will get the error `ERROR: Failed building wheel for PyAudio`. Install it using:
+`brew install portaudio` before installing requirements.
+
 
 run using: 
-`python audiotimer`
+`python -m audiotimer`
 
 see -h flag for run-time options.
 
+Eample usage:
+Run using a treshold of "50" and a buffertime of 30 seconds:
+`python -m audiotimer -t 50 -b 30`
+
 ## Use case
 The program is intended to be used as a way of testing the battery life of battery powered loudspeakers. Set the speaker to play a pink noise at a certain level, and leave a laptop with the speaker to listen for when it dies out.
```

### Comparing `audiotimer-0.3.1/audiotimer/__main__.py` & `audiotimer-0.4.0/audiotimer/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 def main():
     import pyaudio
     import numpy as np
     import time
+    import math
     from pynput import keyboard
-    from .flags import args # . notation ensures import from local package
+    from slack_ping import Slack
+
+
+
+    # TODO: make more elegant? 
+    if __name__ == "__main__":
+        # import default flag values when run as script
+        from flags import args
+        from slack_ping import Slack
+        from helpers import time_stamp, Configuration
+    else:
+        # import flag values when run as module
+        from .flags import args # . notation ensures import from local package
+        from .slack_ping import Slack
+        from .helpers import time_stamp, Configuration
+
+    # import message client for Slack.
+    slack = Slack() 
 
+    # config = Configuration()
     # Constants
     FORMAT = pyaudio.paInt16
     CHANNELS = 1
     RATE = 44100
     CHUNK = 1024
     THRESHOLD = args.threshold  # Audio level threshold for detecting sound. Defaults to 1000.
     MAX_LEVEL = 32768  # Max level for 16-bit audio
@@ -21,24 +40,25 @@
     # Initialize PyAudio
     p = pyaudio.PyAudio()
 
     # Open stream for audio input
     stream = p.open(format=FORMAT, channels=CHANNELS, rate=RATE, input=True, frames_per_buffer=CHUNK)
 
     print("Listening for audio... Press 'q' to quit early.")
+    test_note = input("Add a note to the test measurement:")
+    slack.post_message(f'Test started at {time_stamp()}')
 
     def on_press(key):
         try:
             # Stop the listener if 'q' is pressed
             if key.char == 'q':
                 return False
         except AttributeError:
             pass
 
-    import math
 
     def create_volume_bar(level, max_level, bar_length, threshold):
         """Create a graphical representation of the volume level with logarithmic scaling."""
         # check that level is non negative (can happen on windows 11)
         if level < 0:
             level = 0
         # Apply logarithmic scaling
@@ -84,32 +104,35 @@
                 if audio_detected and current_level < THRESHOLD:
                     if buffer_start is None:
                         buffer_start = time.time()  # Start buffer timer
                     else:
                         remaining_time = BUFFER_TIME - (time.time() - buffer_start)
                         if remaining_time <= 0:
                             end_time = time.time()
+                            end_time_stamp = time_stamp() 
                             break
                         countdown_msg = f" - Countdown: {int(remaining_time)}s"
                 else:
                     countdown_msg = ""
 
                 print(f"Volume: [{volume_bar}] {countdown_msg}", end='\r')
 
             # Check if the current audio level exceeds the threshold
             if current_level > THRESHOLD:
                 if not start_time:
                     print("\nAudio detected. Starting timer...")
                     start_time = time.time()
+                    start_time_stamp = time_stamp()
                 audio_detected = True
                 buffer_start = None  # Reset buffer timer
 
             # Check for keypress to quit early
             if not listener.running and start_time:
                 end_time = time.time()
+                end_time_stamp = time_stamp()
                 break
     except KeyboardInterrupt:
         end_time = time.time()
     except RuntimeError as e:
         print(e)
     finally:
         # Close the audio stream and terminate PyAudio
@@ -120,16 +143,27 @@
     # Calculate and print the duration if audio was detected
     if start_time:
         duration = end_time - start_time
         hours, remainder = divmod(duration, 3600)
         minutes, seconds = divmod(remainder, 60)
         formatted_duration = f"{int(hours)}h:{int(minutes):02d}m:{int(seconds):02d}s"
         print(f"\nDuration: {formatted_duration}")
+        slack.post_message(
+            f"Battery test ended at {end_time_stamp}\n"
+            f"Duration was: {formatted_duration}\n"
+            f"Test note: {test_note}"
+            )
+
 
         # Write the duration to a file
         with open("duration.txt", "w") as file:
-            file.write(f"Duration: {formatted_duration}")
+            file.write(
+                f"Duration: {formatted_duration}\n"
+                f"Start time: {start_time_stamp}\n"
+                f"End time: {end_time_stamp}\nq"
+                f"Note: {test_note}"
+                )
     else:
         print("No audio detected.")
 
 if __name__=="__main__":
     main()
```

### Comparing `audiotimer-0.3.1/audiotimer/flags.py` & `audiotimer-0.4.0/audiotimer/flags.py`

 * *Files identical despite different names*

### Comparing `audiotimer-0.3.1/audiotimer.egg-info/PKG-INFO` & `audiotimer-0.4.0/audiotimer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: audiotimer
-Version: 0.3.1
+Version: 0.4.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.26.3
-Requires-Dist: PyAudio>=0.2.14
-Requires-Dist: pynput>=1.7.6
 
 # Audio timer
 Github: https://github.com/ARanch/audiotimer
 
 This small program starts listening for an audio input on the system microphone. When a set audio level threshold is reached, a timer is started. When the audio level is reduced below the threshold, the timer is stopped after a short countdown, and the timespan is logged.
 
 `python -m pip install audiotimer`
 
 install requirements:
 `pip install -r requirements.txt`
 
+Note: on Mac OS you need [Portaudio](https://www.portaudio.com/) installed, otherwise you will get the error `ERROR: Failed building wheel for PyAudio`. Install it using:
+`brew install portaudio` before installing requirements.
+
 
 run using: 
-`python audiotimer`
+`python -m audiotimer`
 
 see -h flag for run-time options.
 
+Eample usage:
+Run using a treshold of "50" and a buffertime of 30 seconds:
+`python -m audiotimer -t 50 -b 30`
+
 ## Use case
 The program is intended to be used as a way of testing the battery life of battery powered loudspeakers. Set the speaker to play a pink noise at a certain level, and leave a laptop with the speaker to listen for when it dies out. 
+
+
```

