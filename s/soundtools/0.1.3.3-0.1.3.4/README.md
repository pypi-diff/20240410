# Comparing `tmp/soundtools-0.1.3.3.tar.gz` & `tmp/soundtools-0.1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.1.3.3.tar", last modified: Sun Apr  7 11:01:02 2024, max compression
+gzip compressed data, was "soundtools-0.1.3.4.tar", last modified: Wed Apr 10 02:12:37 2024, max compression
```

## Comparing `soundtools-0.1.3.3.tar` & `soundtools-0.1.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 11:01:02.167465 soundtools-0.1.3.3/
--rw-rw-rw-   0        0        0      345 2024-04-07 11:01:02.166467 soundtools-0.1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 11:01:02.167465 soundtools-0.1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-04-07 10:59:35.000000 soundtools-0.1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:01:02.142823 soundtools-0.1.3.3/soundtools/
--rw-rw-rw-   0        0        0       25 2024-04-06 19:22:41.000000 soundtools-0.1.3.3/soundtools/__init__.py
--rw-rw-rw-   0        0        0    31839 2024-04-07 10:59:06.000000 soundtools-0.1.3.3/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:01:02.166467 soundtools-0.1.3.3/soundtools.egg-info/
--rw-rw-rw-   0        0        0      345 2024-04-07 11:01:02.000000 soundtools-0.1.3.3/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-07 11:01:02.000000 soundtools-0.1.3.3/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 11:01:02.000000 soundtools-0.1.3.3/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 11:01:02.000000 soundtools-0.1.3.3/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 02:12:37.192314 soundtools-0.1.3.4/
+-rw-rw-rw-   0        0        0      345 2024-04-10 02:12:37.192314 soundtools-0.1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:12:37.192314 soundtools-0.1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-04-10 02:11:55.000000 soundtools-0.1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:12:37.181316 soundtools-0.1.3.4/soundtools/
+-rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.1.3.4/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    32118 2024-04-10 02:11:43.000000 soundtools-0.1.3.4/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:12:37.191314 soundtools-0.1.3.4/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.1.3.3/soundtools/soundtools.py` & `soundtools-0.1.3.4/soundtools/soundtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
 this package is used to create, play and save sound files
-it has some basic sound waves although you can add your own and you can modify the package.
+it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
-uses scipy.io.wavfile to read wav files because the wave module can read the float32 bit wav files
-and finally uses matplotlib to visualize the waves"""
+and uses matplotlib to visualize the waves"""
 
 
 import pyaudio
 import numpy as np
 from typing import Callable, Iterable, Literal
 import scipy.io.wavfile as wf
+from scipy.signal import square
 import matplotlib.pyplot as plt
 import librosa.effects as effect
 from os.path import splitext
 from pydub.audio_segment import AudioSegment
 from soundfile import read as sfRead
 
 
@@ -97,15 +97,16 @@
             f = freq*h
             #-- break if the frequency is greater than 20,000 because human ear can' hear it and the arent many headphones that can play more than this anyways --#
             if f > 20_000:
                 break
             #-- adding the harmonics --#
             buf += np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h
         
-        wave = ((self.four_over_pi)*vol*buf).astype(self.dtype)
+        # wave = ((self.four_over_pi)*vol*buf).astype(self.dtype)
+        wave = (vol*buf).astype(self.dtype)
         return wave
     
     @cache_wave("tri")
     def triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a triangle wave based on the given frequency, duration and amplitude or volume\n
         a triangle wave is typically generated by adding every second odd harmonic (5, 9, 13...) to a fundamental frequency\n
         each harmonic is added with a less volume which causes the amplitude to change a bit so at the end the amplitude is multiplied by '8/pi^2' to fix it\n
@@ -171,40 +172,40 @@
                 break
             buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**smoothness)
         
         wave = (vol * -self.two_oper_pi * buf).astype(self.dtype)
         return wave
     
     @cache_wave("revsmoothsaw")
-    def smooth_saw_wave(self, freq:float, dur:float, vol: float, smoothness: float=1.25) -> SoundBuffer:
+    def rev_smooth_saw_wave(self, freq:float, dur:float, vol: float, smoothness: float=1.25) -> SoundBuffer:
         """creates a wave like reversed saw wave but without the sharp points"""
         buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
         for h in range(2, 1000):
             f = freq*h
             if f > 20000:
                 break
             buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**smoothness)
         
         wave = (vol * self.two_oper_pi * buf).astype(self.dtype)
         return wave
     
     @cache_wave("wavy")
-    def wavy_wave(self, freq:float, dur:float, vol: float, wavyness: int=10) -> SoundBuffer:
+    def wavy_wave(self, freq:float, dur:float, vol: float, wavyness: int=1.25) -> SoundBuffer:
         buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
         for h in range(2, 1000):
             f = freq*h
             if f > 20000:
                 break
             buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**wavyness)
         
         wave = (vol * -self.two_oper_pi * buf).astype(self.dtype)
         return wave
     
     @cache_wave("revwavy")
-    def wavy_wave(self, freq:float, dur:float, vol: float, wavyness: int=10) -> SoundBuffer:
+    def rev_wavy_wave(self, freq:float, dur:float, vol: float, wavyness: int=1.25) -> SoundBuffer:
         buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
         for h in range(2, 1000):
             f = freq*h
             if f > 20000:
                 break
             buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**wavyness)
         
@@ -250,23 +251,33 @@
                 break
             buf += (-1)**h * (np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h)
         
         wave = (vol * (0.5 - self.rev_pi*buf)).astype(self.dtype)
         return wave
     
     
-    def array_to_tuple(self, np_array) -> tuple:
+    def fade_in_out(self, buffer: SoundBuffer, fadein_len:int = 1500, fadeout_len:int = 1500) -> SoundBuffer:
+        fadein = ((1 - np.cos(np.linspace(0, np.pi, fadein_len))) * 0.5).astype(buffer.dtype)
+        fadeout = np.flip(fadein)
+        
+        buffer[:fadein_len] *= fadein
+        buffer[-fadeout_len:] *= fadeout
+        
+        return buffer
+    
+    
+    def array_to_tuple(self, np_array: SoundBuffer) -> tuple:
         """Iterates recursivelly."""
         try:
             return tuple(self.array_to_tuple(_) for _ in np_array)
         except TypeError:
             return np_array
 
 
-class Export:
+class Export(Sounds):
     def __init__(self) -> None:
         pass
     
     # converts a float32 array to an int type
     def float2pcm(self, sig: np.ndarray, dtype: Literal["int32", "int16", "uint8"]="int16") -> SoundBuffer:
         """gets a float dtype array as input, converts it to int and returns the converted array"""
         
@@ -310,18 +321,15 @@
                 audio_format = 2
             elif dtype == "int24":
                 audio_format = 3
             elif dtype == np.float32 or dtype == "float32":
                 audio_format = 4
             else:
                 raise ValueError(f"Incorrect dtype: {dtype}\nvalid options are: \"uint8, int16, int24, float32\"")
-                
-        
-        if not sample_rate:
-            sample_rate = self.default_sample_rate
+            
         
         with open(f"{file_name}.erfan", "wb") as f:
             f.write(sample_rate.to_bytes(4, "little"))
             f.write(audio_format.to_bytes(2, "little"))
             f.write(channels.to_bytes(2, "little"))
             
             if type(buffer) == np.ndarray:
```

