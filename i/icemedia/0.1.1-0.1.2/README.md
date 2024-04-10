# Comparing `tmp/icemedia-0.1.1.tar.gz` & `tmp/icemedia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icemedia-0.1.1.tar", last modified: Sat Apr  6 04:26:03 2024, max compression
+gzip compressed data, was "icemedia-0.1.2.tar", last modified: Wed Apr 10 06:20:26 2024, max compression
```

## Comparing `icemedia-0.1.1.tar` & `icemedia-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 04:26:03.610958 icemedia-0.1.1/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    26526 2024-04-05 18:14:06.000000 icemedia-0.1.1/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7315 2024-04-06 04:26:03.610958 icemedia-0.1.1/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6759 2024-04-06 04:20:23.000000 icemedia-0.1.1/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 04:26:03.606958 icemedia-0.1.1/icemedia/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-05 18:15:47.000000 icemedia-0.1.1/icemedia/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9471 2024-04-06 04:20:24.000000 icemedia-0.1.1/icemedia/iceflow.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    43774 2024-04-06 04:20:24.000000 icemedia-0.1.1/icemedia/iceflow_server.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     7016 2024-04-05 23:26:04.000000 icemedia-0.1.1/icemedia/jack_client_subprocess.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    36598 2024-04-06 00:15:25.000000 icemedia-0.1.1/icemedia/jack_tools.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    20536 2024-04-06 01:31:32.000000 icemedia-0.1.1/icemedia/jsonrpyc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    24337 2024-04-06 02:27:57.000000 icemedia-0.1.1/icemedia/python_mpv_jsonipc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    22471 2024-04-06 04:15:27.000000 icemedia-0.1.1/icemedia/sound_player.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 04:26:03.610958 icemedia-0.1.1/icemedia.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7315 2024-04-06 04:26:03.000000 icemedia-0.1.1/icemedia.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      477 2024-04-06 04:26:03.000000 icemedia-0.1.1/icemedia.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 04:26:03.000000 icemedia-0.1.1/icemedia.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-04-06 04:26:03.000000 icemedia-0.1.1/icemedia.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2024-04-06 04:26:03.000000 icemedia-0.1.1/icemedia.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 04:26:03.610958 icemedia-0.1.1/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2024-04-06 04:23:34.000000 icemedia-0.1.1/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 04:26:03.610958 icemedia-0.1.1/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 icemedia-0.1.1/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3037 2024-04-06 01:34:27.000000 icemedia-0.1.1/tests/testGstStability.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      938 2024-04-06 01:34:27.000000 icemedia-0.1.1/tests/testJack.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2024-04-06 02:25:55.000000 icemedia-0.1.1/tests/test_sound_player.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    26526 2024-04-05 18:14:06.000000 icemedia-0.1.2/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8772 2024-04-10 06:20:26.063933 icemedia-0.1.2/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8216 2024-04-06 20:31:46.000000 icemedia-0.1.2/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/icemedia/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-05 18:15:47.000000 icemedia-0.1.2/icemedia/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9616 2024-04-10 05:25:46.000000 icemedia-0.1.2/icemedia/iceflow.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    43774 2024-04-06 04:20:24.000000 icemedia-0.1.2/icemedia/iceflow_server.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7016 2024-04-05 23:26:04.000000 icemedia-0.1.2/icemedia/jack_client_subprocess.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    36703 2024-04-10 05:33:55.000000 icemedia-0.1.2/icemedia/jack_tools.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    20538 2024-04-10 05:33:09.000000 icemedia-0.1.2/icemedia/jsonrpyc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    24337 2024-04-06 02:27:57.000000 icemedia-0.1.2/icemedia/python_mpv_jsonipc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    22470 2024-04-06 20:31:46.000000 icemedia-0.1.2/icemedia/sound_player.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/icemedia.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8772 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      477 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-10 06:20:26.063933 icemedia-0.1.2/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2024-04-10 05:37:18.000000 icemedia-0.1.2/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 icemedia-0.1.2/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3037 2024-04-06 01:34:27.000000 icemedia-0.1.2/tests/testGstStability.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      938 2024-04-06 01:34:27.000000 icemedia-0.1.2/tests/testJack.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2024-04-06 02:25:55.000000 icemedia-0.1.2/tests/test_sound_player.py
```

### Comparing `icemedia-0.1.1/LICENSE` & `icemedia-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.1/PKG-INFO` & `icemedia-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icemedia
-Version: 0.1.1
+Version: 0.1.2
 Summary: A GStreamer wrapper with JACK connection management
 Home-page: https://github.com/EternityForest/iceflow
 Author: Daniel Dunn
 Author-email: dannydunn@eternityforest.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -21,40 +21,47 @@
 ## Install
 
 ```
 pip install icemedia
 ```
 
 
-## iceflow.sound_player
+## icemedia.sound_player
 
+### Example
+```python
+import icemedia.sound_player
+
+testmedia = "YourAudioFileHere.mp3"
 
-### iceflow.sound_player.sound
+icemedia.sound_player.play_sound(testmedia)
+time.sleep(3)
+```
 
-The iceflow.sound_player.sound uses MPV to play sounds
+The icemedia.sound_player.sound uses MPV to play sounds, so it supports almost any file.
 
 
-#### iceflow.sound_player.sound.preload(filename,output="@auto")
+#### icemedia.sound_player.preload(filename,output="@auto")
 Spins up a paused player for that filename and player. Garbage collecting old cache entries is handled for you.
 Will be used when sound.play is called for the same filename and output.
 
 
-#### iceflow.sound_player.sound.fade_to(self,file,length=1.0, block=False, detach=True, handle="PRIMARY",**kwargs):
+#### icemedia.sound_player.fade_to(self,file,length=1.0, block=False, detach=True, handle="PRIMARY",**kwargs):
 
 Fades the current sound on a given channel to the file. **kwargs aare equivalent to those on playSound.
 
 Passing none for the file allows you to fade to silence, and if no sound is playing. it will fade FROM silence.
 
 Block will block till the fade ends. Detach lets you keep the faded copy attached to the handle(Which makes it end when a new sound plays,
 so it only makes sense if fading to silence).
 
 Fading is perceptually linear.
 
 
-#### iceflow.sound_player.sound.play(filename,handle="PRIMARY",volume=1,start=0,end=-0.0001, output=None,fs=False,extraPaths=\[\])
+#### icemedia.sound_player.play(filename,handle="PRIMARY",volume=1,start=0,end=-0.0001, output=None,fs=False,extraPaths=\[\])
 
 The handle parameter lets you name the new sound instance to
 stop it later or set volume.
 
 If you try to play a sound under the same handle as a
 stil-playing sound, the old one will be stopped. Defaults to PRIMARY.
 
@@ -65,70 +72,106 @@
 other players.
 
 
 Output is a jack client or port if JACK is running.  Currently only the default
 outout works on non-jack systems.
 
 
-#### iceflow.sound_player.sound.stop(handle="PRIMARY")
+#### icemedia.sound_player.stop(handle="PRIMARY")
 
 Stop a sound by handle.
 
-#### iceflow.sound_player.sound.stop_all()
+#### icemedia.sound_player.stop_all()
 
 Stop all currently playing sounds.
 
-#### iceflow.sound_player.sound.is_playing(handle="PRIMARY")
+#### icemedia.sound_player.is_playing(handle="PRIMARY")
 
 Return true if a sound with handle handle is playing. Note that the
 sound might finish before you actually get around to doing anything with
 the value. If using the dummy backend because a backend is not
 installed, result is undefined, but will not be an error, and will be a
 boolean value. If a sound is paused, will return True anyway.
 
-#### iceflow.sound_player.sound.setvol(vol,handle="PRIMARY")
+#### icemedia.sound_player.setvol(vol,handle="PRIMARY")
 
 Set the volume of a sound. Volume goes from 0 to 1.
 
-#### iceflow.sound_player.sound.pause(handle="PRIMARY")
+#### icemedia.sound_player.pause(handle="PRIMARY")
 
 Pause a sound. Does nothing if already paused.
 
-#### iceflow.sound_player.sound.resume(handle="PRIMARY")
+#### icemedia.sound_player.resume(handle="PRIMARY")
 
 Resume a paused a sound. Does nothing if not paused.
 
 
-## iceflow.jack module
+## icemedia.jack module
 
 This submodule requires pyjack, and of course Jack.
 
-### iceflow.jack.start_managing()
+
+### Example
+This uses both JACK and GStreamer
+
+```python
+import time
+import icemedia.jack_tools
+import icemedia.iceflow
+
+"Only works if your device names match, may need to change Built-in Audio Analog Stereo to something else"
+
+icemedia.jack_tools.start_managing()
+
+
+class Player(icemedia.iceflow.GstreamerPipeline):
+    def __init__(self):
+        icemedia.iceflow.GstreamerPipeline.__init__(self, realtime=False)
+        self.src = self.add_element("audiotestsrc")
+        self.sink = self.add_element("jackaudiosink", client_name="JackTest", connect=0)
+
+p = Player()
+p.start()
+
+print("You should hear noise")
+aw = icemedia.jack_tools.Airwire("JackTest", "Built-in Audio Analog Stereo")
+aw.connect()
+time.sleep(1)
+print("No more noise")
+aw.disconnect()
+
+del aw
+gc.collect()
+time.sleep(1)
+```
+
+### icemedia.jack.start_managing()
 
 Call this to try to connect to the JACK server.  None of the other commands will work until you do this.
 
 
-### iceflow.jack.Airwire(from,to)
+### icemedia.jack.Airwire(from,to)
 Return an Airwire object. This is a declaration that you want to connect two clients or ports and keep them connected.
 If you try to connect a client to a single port, all outputs get mixed down. Likewise a port to a client duplicates to all inputs.
 
 They start in the dis_connected state.
 
 
-### iceflow.jack.Airwire.connect()
+### icemedia.jack.Airwire.connect()
 Connect and stay connected. Even if a client dissapears and comes back. Deleting the Airwire will disconnect.
 Note that manually disconnecting may not be undone, to prevent annoyance.
 
-### iceflow.jack.Airwire.disconnect()
+### icemedia.jack.Airwire.disconnect()
 Disconnect.
 
 
 ### Message Bus activity
 
-This submodule posts the following messages to the scullery
+This submodule posts the following messages to the [Scullery](https://github.com/EternityForest/scullery) message bus.
+
 #### /system/jack/newport
  A PortInfo object with a .name, isInput, and isOutput property gets posted here whenever a new port is added to JACK.
 
 #### /system/jack/delport
  A PortInfo object gets posted here whenever a port is unregistered.
 
 #### system/jack/started
@@ -136,14 +179,28 @@
 
 #### sullery.jack.start_managing()
 Start the worker thread and enable management functions
 
 
 ## icemedia.iceflow module
 
+This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.  
+You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.  
+
+To do this on debian-based systems, try these packages on apt, you only 
+need the plugins you actually want to use. GStreamer also will use any LADSPA plugins it finds.
+
+ - python3-gi
+ - python3-gst-1.0
+ - gstreamer1.0-plugins-good
+ - gstreamer1.0-plugins-bad
+ - gstreamer1.0-plugins-ugly
+
+
+### Noise Window
 
 This example shows a window full of noise
 
 ```python
 import time
 import icemedia.iceflow
```

### Comparing `icemedia-0.1.1/README.md` & `icemedia-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,40 +5,47 @@
 ## Install
 
 ```
 pip install icemedia
 ```
 
 
-## iceflow.sound_player
+## icemedia.sound_player
 
+### Example
+```python
+import icemedia.sound_player
+
+testmedia = "YourAudioFileHere.mp3"
 
-### iceflow.sound_player.sound
+icemedia.sound_player.play_sound(testmedia)
+time.sleep(3)
+```
 
-The iceflow.sound_player.sound uses MPV to play sounds
+The icemedia.sound_player.sound uses MPV to play sounds, so it supports almost any file.
 
 
-#### iceflow.sound_player.sound.preload(filename,output="@auto")
+#### icemedia.sound_player.preload(filename,output="@auto")
 Spins up a paused player for that filename and player. Garbage collecting old cache entries is handled for you.
 Will be used when sound.play is called for the same filename and output.
 
 
-#### iceflow.sound_player.sound.fade_to(self,file,length=1.0, block=False, detach=True, handle="PRIMARY",**kwargs):
+#### icemedia.sound_player.fade_to(self,file,length=1.0, block=False, detach=True, handle="PRIMARY",**kwargs):
 
 Fades the current sound on a given channel to the file. **kwargs aare equivalent to those on playSound.
 
 Passing none for the file allows you to fade to silence, and if no sound is playing. it will fade FROM silence.
 
 Block will block till the fade ends. Detach lets you keep the faded copy attached to the handle(Which makes it end when a new sound plays,
 so it only makes sense if fading to silence).
 
 Fading is perceptually linear.
 
 
-#### iceflow.sound_player.sound.play(filename,handle="PRIMARY",volume=1,start=0,end=-0.0001, output=None,fs=False,extraPaths=\[\])
+#### icemedia.sound_player.play(filename,handle="PRIMARY",volume=1,start=0,end=-0.0001, output=None,fs=False,extraPaths=\[\])
 
 The handle parameter lets you name the new sound instance to
 stop it later or set volume.
 
 If you try to play a sound under the same handle as a
 stil-playing sound, the old one will be stopped. Defaults to PRIMARY.
 
@@ -49,70 +56,106 @@
 other players.
 
 
 Output is a jack client or port if JACK is running.  Currently only the default
 outout works on non-jack systems.
 
 
-#### iceflow.sound_player.sound.stop(handle="PRIMARY")
+#### icemedia.sound_player.stop(handle="PRIMARY")
 
 Stop a sound by handle.
 
-#### iceflow.sound_player.sound.stop_all()
+#### icemedia.sound_player.stop_all()
 
 Stop all currently playing sounds.
 
-#### iceflow.sound_player.sound.is_playing(handle="PRIMARY")
+#### icemedia.sound_player.is_playing(handle="PRIMARY")
 
 Return true if a sound with handle handle is playing. Note that the
 sound might finish before you actually get around to doing anything with
 the value. If using the dummy backend because a backend is not
 installed, result is undefined, but will not be an error, and will be a
 boolean value. If a sound is paused, will return True anyway.
 
-#### iceflow.sound_player.sound.setvol(vol,handle="PRIMARY")
+#### icemedia.sound_player.setvol(vol,handle="PRIMARY")
 
 Set the volume of a sound. Volume goes from 0 to 1.
 
-#### iceflow.sound_player.sound.pause(handle="PRIMARY")
+#### icemedia.sound_player.pause(handle="PRIMARY")
 
 Pause a sound. Does nothing if already paused.
 
-#### iceflow.sound_player.sound.resume(handle="PRIMARY")
+#### icemedia.sound_player.resume(handle="PRIMARY")
 
 Resume a paused a sound. Does nothing if not paused.
 
 
-## iceflow.jack module
+## icemedia.jack module
 
 This submodule requires pyjack, and of course Jack.
 
-### iceflow.jack.start_managing()
+
+### Example
+This uses both JACK and GStreamer
+
+```python
+import time
+import icemedia.jack_tools
+import icemedia.iceflow
+
+"Only works if your device names match, may need to change Built-in Audio Analog Stereo to something else"
+
+icemedia.jack_tools.start_managing()
+
+
+class Player(icemedia.iceflow.GstreamerPipeline):
+    def __init__(self):
+        icemedia.iceflow.GstreamerPipeline.__init__(self, realtime=False)
+        self.src = self.add_element("audiotestsrc")
+        self.sink = self.add_element("jackaudiosink", client_name="JackTest", connect=0)
+
+p = Player()
+p.start()
+
+print("You should hear noise")
+aw = icemedia.jack_tools.Airwire("JackTest", "Built-in Audio Analog Stereo")
+aw.connect()
+time.sleep(1)
+print("No more noise")
+aw.disconnect()
+
+del aw
+gc.collect()
+time.sleep(1)
+```
+
+### icemedia.jack.start_managing()
 
 Call this to try to connect to the JACK server.  None of the other commands will work until you do this.
 
 
-### iceflow.jack.Airwire(from,to)
+### icemedia.jack.Airwire(from,to)
 Return an Airwire object. This is a declaration that you want to connect two clients or ports and keep them connected.
 If you try to connect a client to a single port, all outputs get mixed down. Likewise a port to a client duplicates to all inputs.
 
 They start in the dis_connected state.
 
 
-### iceflow.jack.Airwire.connect()
+### icemedia.jack.Airwire.connect()
 Connect and stay connected. Even if a client dissapears and comes back. Deleting the Airwire will disconnect.
 Note that manually disconnecting may not be undone, to prevent annoyance.
 
-### iceflow.jack.Airwire.disconnect()
+### icemedia.jack.Airwire.disconnect()
 Disconnect.
 
 
 ### Message Bus activity
 
-This submodule posts the following messages to the scullery
+This submodule posts the following messages to the [Scullery](https://github.com/EternityForest/scullery) message bus.
+
 #### /system/jack/newport
  A PortInfo object with a .name, isInput, and isOutput property gets posted here whenever a new port is added to JACK.
 
 #### /system/jack/delport
  A PortInfo object gets posted here whenever a port is unregistered.
 
 #### system/jack/started
@@ -120,14 +163,28 @@
 
 #### sullery.jack.start_managing()
 Start the worker thread and enable management functions
 
 
 ## icemedia.iceflow module
 
+This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.  
+You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.  
+
+To do this on debian-based systems, try these packages on apt, you only 
+need the plugins you actually want to use. GStreamer also will use any LADSPA plugins it finds.
+
+ - python3-gi
+ - python3-gst-1.0
+ - gstreamer1.0-plugins-good
+ - gstreamer1.0-plugins-bad
+ - gstreamer1.0-plugins-ugly
+
+
+### Noise Window
 
 This example shows a window full of noise
 
 ```python
 import time
 import icemedia.iceflow
```

### Comparing `icemedia-0.1.1/icemedia/iceflow.py` & `icemedia-0.1.2/icemedia/iceflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,19 @@
                 env=env,
             )
         else:
             # TODO nobody seems to know why this sometimes OSErrors
             for i in range(5):
                 try:
                     self.worker = Popen(
-                        ["python3", f], stdout=PIPE, stdin=PIPE, stderr=STDOUT, env=env
+                        [sys.executable or "python3", f],
+                        stdout=PIPE,
+                        stdin=PIPE,
+                        stderr=STDOUT,
+                        env=env,
                     )
                     self.worker.stdin.flush()
                     break
                 except OSError:
                     if i == 4:
                         raise
                     else:
@@ -179,15 +183,15 @@
 
     def cleanup_popen(self):
         self.worker.terminate()
         self.worker.kill()
         close_fds(self.worker)
         try:
             self.rpc.stdin.close()
-        except:
+        except Exception:
             pass
 
     def __del__(self):
         self.cleanup_popen()
         workers.do(self.worker.wait)
 
     def add_element(self, element_name: str, *a, **k):
@@ -288,25 +292,25 @@
             self.rpc_call("stop", block=0.01, timeout=10)
             self.worker.terminate()
             time.sleep(0.5)
             self.worker.kill()
             close_fds(self.worker)
             try:
                 self.rpc.stdin.close()
-            except:
+            except Exception:
                 pass
 
         except Exception:
             self.worker.terminate()
             time.sleep(0.5)
             self.worker.kill()
             close_fds(self.worker)
             try:
                 self.rpc.stdin.close()
-            except:
+            except Exception:
                 pass
             workers.do(self.worker.wait)
 
         self.rpc = None
 
     def add_jack_mixer_send_elements(self, *a, **k):
         a, b = self.rpc_call(
```

### Comparing `icemedia-0.1.1/icemedia/iceflow_server.py` & `icemedia-0.1.2/icemedia/iceflow_server.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.1/icemedia/jack_client_subprocess.py` & `icemedia-0.1.2/icemedia/jack_client_subprocess.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.1/icemedia/jack_tools.py` & `icemedia-0.1.2/icemedia/jack_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 
 
 import weakref
 import threading
 import functools
 import os
 import time
-import threading
 import traceback
 import sys
-import weakref
 from .jsonrpyc import RPC
 from subprocess import PIPE, STDOUT, Popen
 
 
 def close_fds(p: Popen):
     try:
         p.stdin.close()
@@ -98,15 +96,15 @@
             "isAudio": self.isAudio,
             "aliases": self.aliases,
         }
 
 
 class JackClientProxy:
     def __getattr__(self, attr):
-        if self.ended or not self.worker.poll() is None:
+        if self.ended or self.worker.poll() is not None:
             raise RuntimeError("This process is already dead")
         check_exclude()
 
         def f(*a, timeout=10, **k):
             try:
                 # Can't serialize ports
                 a = [i.name if isinstance(i, PortInfo) else i for i in a]
@@ -129,26 +127,28 @@
 
         return f
 
     def get_all_connections(self, *a, **k):
         check_exclude()
 
         a = [i.name if isinstance(i, PortInfo) else i for i in a]
-        x = self.rpc.call("get_all_connections", args=a, kwargs=k, block=0.001)
+        x = self.rpc.call(
+            "get_all_connections", args=a, kwargs=k, block=0.001, timeout=25
+        )
         x = [PortInfo(**i) for i in x]
         return x
 
     def get_ports(self, *a, **k):
         check_exclude()
 
-        if self.ended or not self.worker.poll() is None:
+        if self.ended or self.worker.poll() is not None:
             raise RuntimeError("This process is already dead")
         try:
             a = [i.name if isinstance(i, PortInfo) else i for i in a]
-            x = self.rpc.call("get_ports", args=a, kwargs=k, block=0.001)
+            x = self.rpc.call("get_ports", args=a, kwargs=k, block=0.001, timeout=25)
             x = [PortInfo(**i) for i in x]
             return x
 
         except TimeoutError:
             print(traceback.format_exc())
             self.worker.terminate()
             self.worker.kill()
@@ -259,18 +259,18 @@
         workers.do(handle_jack_event)
 
     def close(self):
         if self.ended:
             return
 
         self.ended = True
-        if not self.worker.poll() is None:
+        if self.worker.poll() is not None:
             return
         try:
-            x = self.rpc.call("close")
+            x = self.rpc.call("close", timeout=15)
             self.rpc.stopFlag = True
         except Exception:
             self.rpc.stopFlag = True
             self.worker.terminate()
             self.worker.kill()
             close_fds(self.worker)
             workers.do(self.worker.wait)
@@ -298,20 +298,24 @@
                 stdout=PIPE,
                 stdin=PIPE,
                 stderr=STDOUT,
                 env=env,
             )
         else:
             self.worker = Popen(
-                ["python3", f], stdout=PIPE, stdin=PIPE, stderr=STDOUT, env=env
+                [sys.executable or "python3", f],
+                stdout=PIPE,
+                stdin=PIPE,
+                stderr=STDOUT,
+                env=env,
             )
         self.rpc = RPC(
             target=self, stdin=self.worker.stdout, stdout=self.worker.stdin, daemon=True
         )
-        self.rpc.call("init")
+        self.rpc.call("init", timeout=15)
 
     def print(self, s):
         print(s)
 
 
 def handle_jack_event():
     with jackEventHandlingQueueLock:
@@ -488,15 +492,15 @@
             # Don't disconnect if this airwire has been taken over by a new connection between the ports
             x = None
             try:
                 x = latestAirWireForGivenPair[self.tupleid]
             except KeyError:
                 pass
 
-            if x and not x is self:
+            if x and x is not self:
                 return
 
         try:
             if lock.acquire(timeout=10):
                 try:
                     if is_connected(self.orig, self.to):
                         disconnect(self.orig, self.to)
@@ -640,15 +644,15 @@
             # Don't disconnect if this airwire has been taken over by a new connection between the ports
             x = None
             try:
                 x = latestAirWireForGivenPair[self.tupleid]
             except KeyError:
                 pass
 
-            if x and not x is self:
+            if x and x is not self:
                 return
 
         if portsListLock.acquire(timeout=10):
             try:
                 outPorts = sorted(
                     [
                         portsList[i]
@@ -745,15 +749,15 @@
             # Don't disconnect if this airwire has been taken over by a new connection between the ports
             x = None
             try:
                 x = latestAirWireForGivenPair[self.tupleid]
             except KeyError:
                 pass
 
-            if x and not x is self:
+            if x and x is not self:
                 return
 
         if lock.acquire(timeout=10):
             try:
                 if t.endswith("*"):
                     t = t[:-1]
 
@@ -796,15 +800,15 @@
         f = "jdgdsjfgkldsf"
         t = "dsfjgjdsfjgkl"
     if force_combining:
         return CombiningAirwire(f, t)
     elif f == None or t == None:
         return MonoAirwire(None, None)
     elif ":" in f:
-        if not ":" in t:
+        if ":" not in t:
             return CombiningAirwire(f, t)
         return MonoAirwire(f, t)
     else:
         return MultichannelAirwire(f, t)
 
 
 ############################################################################
@@ -904,15 +908,14 @@
 postedCheck = True
 
 firstConnect = False
 
 
 def _checkJackClient(err=True):
     global _jackclient, realConnections, postedCheck, firstConnect
-    import jack
 
     if lock.acquire(timeout=10):
         try:
             t = _jackclient.get_ports()
 
             if not t:
                 if firstConnect:
@@ -1010,17 +1013,17 @@
         try:
             if not _jackclient:
                 return []
             ports = []
             x = _jackclient.get_ports(*a, **k)
             for i in x:
                 for j in i.aliases:
-                    if not j in ports:
+                    if j not in ports:
                         ports.append(j)
-                if not i.name in ports:
+                if i.name not in ports:
                     ports.append(i.name)
             return ports
         finally:
             lock.release()
     else:
         pass
```

### Comparing `icemedia-0.1.1/icemedia/jsonrpyc.py` & `icemedia-0.1.2/icemedia/jsonrpyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
 
     def call(
         self: RPC,
         method: str,
         args: tuple[Any] = (),
         kwargs: dict | None = None,
         callback: Callable | None = None,
-        block: int = 0,
+        block: float = 0,
         timeout: float = 0,
     ) -> None:
         """
         Performs an actual remote procedure call by writing a request representation (a string) to
         the output stream. The remote RPC instance uses *method* to route to the actual method to
         call with *args* and *kwargs*. When *callback* is set, it will be called with the result of
         the remote call. When *block* is larger than *0*, the calling thread is blocked until the
```

### Comparing `icemedia-0.1.1/icemedia/python_mpv_jsonipc.py` & `icemedia-0.1.2/icemedia/python_mpv_jsonipc.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.1/icemedia/sound_player.py` & `icemedia-0.1.2/icemedia/sound_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,15 +505,15 @@
         "Return true if a sound is playing on channel"
         try:
             return self.runningSounds[channel].is_playing(refresh)
         except KeyError:
             return False
 
     def wait(self, channel="PRIMARY"):
-        "Block until any sound playing on a channel is finished"
+        "Block until any sound playing on a channel is playing"
         try:
             self.runningSounds[channel].wait()
         except KeyError:
             return False
 
     def set_volume(self, vol, channel="PRIMARY", final=True):
         "Return true if a sound is playing on channel"
```

### Comparing `icemedia-0.1.1/icemedia.egg-info/PKG-INFO` & `icemedia-0.1.2/icemedia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icemedia
-Version: 0.1.1
+Version: 0.1.2
 Summary: A GStreamer wrapper with JACK connection management
 Home-page: https://github.com/EternityForest/iceflow
 Author: Daniel Dunn
 Author-email: dannydunn@eternityforest.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -21,40 +21,47 @@
 ## Install
 
 ```
 pip install icemedia
 ```
 
 
-## iceflow.sound_player
+## icemedia.sound_player
 
+### Example
+```python
+import icemedia.sound_player
+
+testmedia = "YourAudioFileHere.mp3"
 
-### iceflow.sound_player.sound
+icemedia.sound_player.play_sound(testmedia)
+time.sleep(3)
+```
 
-The iceflow.sound_player.sound uses MPV to play sounds
+The icemedia.sound_player.sound uses MPV to play sounds, so it supports almost any file.
 
 
-#### iceflow.sound_player.sound.preload(filename,output="@auto")
+#### icemedia.sound_player.preload(filename,output="@auto")
 Spins up a paused player for that filename and player. Garbage collecting old cache entries is handled for you.
 Will be used when sound.play is called for the same filename and output.
 
 
-#### iceflow.sound_player.sound.fade_to(self,file,length=1.0, block=False, detach=True, handle="PRIMARY",**kwargs):
+#### icemedia.sound_player.fade_to(self,file,length=1.0, block=False, detach=True, handle="PRIMARY",**kwargs):
 
 Fades the current sound on a given channel to the file. **kwargs aare equivalent to those on playSound.
 
 Passing none for the file allows you to fade to silence, and if no sound is playing. it will fade FROM silence.
 
 Block will block till the fade ends. Detach lets you keep the faded copy attached to the handle(Which makes it end when a new sound plays,
 so it only makes sense if fading to silence).
 
 Fading is perceptually linear.
 
 
-#### iceflow.sound_player.sound.play(filename,handle="PRIMARY",volume=1,start=0,end=-0.0001, output=None,fs=False,extraPaths=\[\])
+#### icemedia.sound_player.play(filename,handle="PRIMARY",volume=1,start=0,end=-0.0001, output=None,fs=False,extraPaths=\[\])
 
 The handle parameter lets you name the new sound instance to
 stop it later or set volume.
 
 If you try to play a sound under the same handle as a
 stil-playing sound, the old one will be stopped. Defaults to PRIMARY.
 
@@ -65,70 +72,106 @@
 other players.
 
 
 Output is a jack client or port if JACK is running.  Currently only the default
 outout works on non-jack systems.
 
 
-#### iceflow.sound_player.sound.stop(handle="PRIMARY")
+#### icemedia.sound_player.stop(handle="PRIMARY")
 
 Stop a sound by handle.
 
-#### iceflow.sound_player.sound.stop_all()
+#### icemedia.sound_player.stop_all()
 
 Stop all currently playing sounds.
 
-#### iceflow.sound_player.sound.is_playing(handle="PRIMARY")
+#### icemedia.sound_player.is_playing(handle="PRIMARY")
 
 Return true if a sound with handle handle is playing. Note that the
 sound might finish before you actually get around to doing anything with
 the value. If using the dummy backend because a backend is not
 installed, result is undefined, but will not be an error, and will be a
 boolean value. If a sound is paused, will return True anyway.
 
-#### iceflow.sound_player.sound.setvol(vol,handle="PRIMARY")
+#### icemedia.sound_player.setvol(vol,handle="PRIMARY")
 
 Set the volume of a sound. Volume goes from 0 to 1.
 
-#### iceflow.sound_player.sound.pause(handle="PRIMARY")
+#### icemedia.sound_player.pause(handle="PRIMARY")
 
 Pause a sound. Does nothing if already paused.
 
-#### iceflow.sound_player.sound.resume(handle="PRIMARY")
+#### icemedia.sound_player.resume(handle="PRIMARY")
 
 Resume a paused a sound. Does nothing if not paused.
 
 
-## iceflow.jack module
+## icemedia.jack module
 
 This submodule requires pyjack, and of course Jack.
 
-### iceflow.jack.start_managing()
+
+### Example
+This uses both JACK and GStreamer
+
+```python
+import time
+import icemedia.jack_tools
+import icemedia.iceflow
+
+"Only works if your device names match, may need to change Built-in Audio Analog Stereo to something else"
+
+icemedia.jack_tools.start_managing()
+
+
+class Player(icemedia.iceflow.GstreamerPipeline):
+    def __init__(self):
+        icemedia.iceflow.GstreamerPipeline.__init__(self, realtime=False)
+        self.src = self.add_element("audiotestsrc")
+        self.sink = self.add_element("jackaudiosink", client_name="JackTest", connect=0)
+
+p = Player()
+p.start()
+
+print("You should hear noise")
+aw = icemedia.jack_tools.Airwire("JackTest", "Built-in Audio Analog Stereo")
+aw.connect()
+time.sleep(1)
+print("No more noise")
+aw.disconnect()
+
+del aw
+gc.collect()
+time.sleep(1)
+```
+
+### icemedia.jack.start_managing()
 
 Call this to try to connect to the JACK server.  None of the other commands will work until you do this.
 
 
-### iceflow.jack.Airwire(from,to)
+### icemedia.jack.Airwire(from,to)
 Return an Airwire object. This is a declaration that you want to connect two clients or ports and keep them connected.
 If you try to connect a client to a single port, all outputs get mixed down. Likewise a port to a client duplicates to all inputs.
 
 They start in the dis_connected state.
 
 
-### iceflow.jack.Airwire.connect()
+### icemedia.jack.Airwire.connect()
 Connect and stay connected. Even if a client dissapears and comes back. Deleting the Airwire will disconnect.
 Note that manually disconnecting may not be undone, to prevent annoyance.
 
-### iceflow.jack.Airwire.disconnect()
+### icemedia.jack.Airwire.disconnect()
 Disconnect.
 
 
 ### Message Bus activity
 
-This submodule posts the following messages to the scullery
+This submodule posts the following messages to the [Scullery](https://github.com/EternityForest/scullery) message bus.
+
 #### /system/jack/newport
  A PortInfo object with a .name, isInput, and isOutput property gets posted here whenever a new port is added to JACK.
 
 #### /system/jack/delport
  A PortInfo object gets posted here whenever a port is unregistered.
 
 #### system/jack/started
@@ -136,14 +179,28 @@
 
 #### sullery.jack.start_managing()
 Start the worker thread and enable management functions
 
 
 ## icemedia.iceflow module
 
+This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.  
+You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.  
+
+To do this on debian-based systems, try these packages on apt, you only 
+need the plugins you actually want to use. GStreamer also will use any LADSPA plugins it finds.
+
+ - python3-gi
+ - python3-gst-1.0
+ - gstreamer1.0-plugins-good
+ - gstreamer1.0-plugins-bad
+ - gstreamer1.0-plugins-ugly
+
+
+### Noise Window
 
 This example shows a window full of noise
 
 ```python
 import time
 import icemedia.iceflow
```

### Comparing `icemedia-0.1.1/setup.py` & `icemedia-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="icemedia",
-    version="0.1.1",
+    version="0.1.2",
     author="Daniel Dunn",
     author_email="dannydunn@eternityforest.com",
     description="A GStreamer wrapper with JACK connection management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EternityForest/iceflow",
     packages=setuptools.find_packages(),
```

### Comparing `icemedia-0.1.1/tests/testGstStability.py` & `icemedia-0.1.2/tests/testGstStability.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.1/tests/testJack.py` & `icemedia-0.1.2/tests/testJack.py`

 * *Files identical despite different names*

