# Comparing `tmp/soundtools-0.1.3.5.tar.gz` & `tmp/soundtools-0.1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.1.3.5.tar", last modified: Wed Apr 10 02:26:46 2024, max compression
+gzip compressed data, was "soundtools-0.1.3.6.tar", last modified: Wed Apr 10 16:26:48 2024, max compression
```

## Comparing `soundtools-0.1.3.5.tar` & `soundtools-0.1.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:26:46.352314 soundtools-0.1.3.5/
--rw-rw-rw-   0        0        0      345 2024-04-10 02:26:46.351314 soundtools-0.1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 02:26:46.352314 soundtools-0.1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-04-10 02:26:04.000000 soundtools-0.1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:26:46.349316 soundtools-0.1.3.5/soundtools/
--rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.1.3.5/soundtools/__init__.py
--rw-rw-rw-   0        0        0    32110 2024-04-10 02:25:23.000000 soundtools-0.1.3.5/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:26:46.351314 soundtools-0.1.3.5/soundtools.egg-info/
--rw-rw-rw-   0        0        0      345 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 16:26:48.842104 soundtools-0.1.3.6/
+-rw-rw-rw-   0        0        0      345 2024-04-10 16:26:48.841104 soundtools-0.1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:26:48.842104 soundtools-0.1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-04-10 16:26:29.000000 soundtools-0.1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:26:48.829441 soundtools-0.1.3.6/soundtools/
+-rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.1.3.6/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    34888 2024-04-10 16:24:28.000000 soundtools-0.1.3.6/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:26:48.832441 soundtools-0.1.3.6/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-04-10 16:26:48.000000 soundtools-0.1.3.6/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-10 16:26:48.000000 soundtools-0.1.3.6/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:26:48.000000 soundtools-0.1.3.6/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 16:26:48.000000 soundtools-0.1.3.6/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.1.3.5/soundtools/soundtools.py` & `soundtools-0.1.3.6/soundtools/soundtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 and uses matplotlib to visualize the waves"""
 
 
 import pyaudio
 import numpy as np
 from typing import Callable, Iterable, Literal
 import scipy.io.wavfile as wf
-from scipy.signal import square
 import matplotlib.pyplot as plt
 import librosa.effects as effect
 from os.path import splitext
 from pydub.audio_segment import AudioSegment
 from soundfile import read as sfRead
 
 
@@ -48,16 +47,28 @@
         
         self.tau = 2*np.pi
         self.rev_pi = 1/np.pi
         self.two_oper_pi = 2/np.pi
         self.four_over_pi = 4/np.pi
         self.eight_over_pi_sqr = 8/np.pi**2
         
+        self.change_dtype(dtype)
+    
+    
+    def change_dtype(self, dtype):
         self.dtype = dtype
-        
+        if self.dtype == np.float32:
+            self.min_amp = -1
+            self.max_amp = 1
+        else:
+            i = np.iinfo(self.dtype)
+            self.min_amp = i.min
+            self.max_amp = i.max
+    
+    
     # caches the waves so if you had to generate a note multiple times its not gonna take long to execute
     # you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable
     # so this decorator will save a tuple of that numpy array in self.existed_notes and convert it back to a numpy array each time you want to use that wave
     def cache_wave(wave_type: str) -> SoundBuffer:
         """caches the waves so if you had to generate a note multiple times it's gonna use the cached wave. 
         you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable, 
         so this decorator will store the numpy array as a tuple in "self.existed_notes" and convert it back to a numpy array each time you want to use that wave
@@ -66,14 +77,16 @@
             def wrapper(self, freq:float, dur:float, vol: float):
                 name = f"{wave_type}|{freq}|{dur}|{vol}"
                 if name in self.existed_notes.keys():
                     self.total_cached += 1
                     return np.array(self.existed_notes[name], dtype=self.dtype)
                 
                 result: SoundBuffer = func(self, freq, dur, vol)
+                result[result > 1] = self.max_amp
+                result[result < -1] = self.min_amp
                 self.existed_notes[name] = self.array_to_tuple(result)
                 
                 return result
             return wrapper
         return decorator
 
     @cache_wave("sine")
@@ -97,16 +110,15 @@
             f = freq*h
             #-- break if the frequency is greater than 20,000 because human ear can' hear it and the arent many headphones that can play more than this anyways --#
             if f > 20_000:
                 break
             #-- adding the harmonics --#
             buf += np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h
         
-        # wave = ((self.four_over_pi)*vol*buf).astype(self.dtype)
-        wave = (vol*buf).astype(self.dtype)
+        wave = ((self.four_over_pi)*vol*buf).astype(self.dtype)
         return wave
     
     @cache_wave("tri")
     def triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a triangle wave based on the given frequency, duration and amplitude or volume\n
         a triangle wave is typically generated by adding every second odd harmonic (5, 9, 13...) to a fundamental frequency\n
         each harmonic is added with a less volume which causes the amplitude to change a bit so at the end the amplitude is multiplied by '8/pi^2' to fix it\n
@@ -409,14 +421,31 @@
                 width = 3
             case "float32":
                 width = 4
             case _:
                 return 4
         
         return width
+    
+    
+    def get_sampwidth_from_int(self, dtype: Literal[1, 2, 3, 4]) -> str:
+        if not (0 < dtype < 5):
+            raise f"Invalid data type {dtype}"
+        
+        match dtype:
+            case 1:
+                width = "uint8"
+            case 2:
+                width = "int16"
+            case 3:
+                width = "int24"
+            case 4:
+                width = "float32"
+        
+        return width
 
 
 class Music(Sounds, Export):
     """used for creating and playing sounds"""
     def __init__(self, middle_a=440, tempo=60, sample_rate=48000, tune=12) -> None:
         super().__init__(sample_rate)
         self.sample_rate: int = sample_rate
@@ -435,18 +464,49 @@
     # you have to use this function to initialize before playing any note.
     def init(self) -> None:
         super().__init__(self.sample_rate)
         self.SEMI_TONE: float = np.power(2, (1/self.TUNE)) # a semitone in a 12 equal temperament is 2 to the power of 1/12, that means in a 6 equal temperament system a semitone is 2^(1/6)
         self.generate_note_names()
         self.assign_middle_a()
         self.assign_frequencies()
+        self.init_output_stream()
+        self.init_input_stream()
+    
+    
+    def init_output_stream(self, samp_width:int|str="float32",
+                           n_channels:int|None=None,
+                           sample_rate:int|None=None) -> None:
+        
+        if not n_channels:
+            n_channels = self.channels
+        if not sample_rate:
+            sample_rate = self.sample_rate
         
-        self.stream = self.config_stream(samp_width="float32",
-                                         channels=self.channels,
-                                         sample_rate=self.sample_rate)
+        self.stream = self.config_stream(samp_width=samp_width,
+                                         channels=n_channels,
+                                         sample_rate=sample_rate)
+    
+    
+    def init_input_stream(self, samp_width: int|str="float32", n_channels: int=1, sample_rate: int|None=None, chunk:int=3200) -> None:
+        if not sample_rate:
+            sample_rate = self.sample_rate
+        
+        if type(samp_width) == str:
+            samp_width = self.get_sampwidth_from_str(dtype=samp_width)
+        
+        self.input_stream = self.AUDIO_OBJECT.open(format=self.AUDIO_OBJECT.get_format_from_width(samp_width),
+                                                   channels=n_channels,
+                                                   rate=sample_rate,
+                                                   input=True,
+                                                   frames_per_buffer=chunk)
+        
+        self.input_rate = sample_rate
+        self.input_chunk = chunk
+        self.input_dtype = self.get_sampwidth_from_int(samp_width)
+        self.input_channels = n_channels
     
     
     def config_stream(self, samp_width: int|str, channels: int, sample_rate: int) -> pyaudio.Stream:
         if type(samp_width) == str:
             samp_width = self.get_sampwidth_from_str(dtype=samp_width)
         
         return self.AUDIO_OBJECT.open(format=self.AUDIO_OBJECT.get_format_from_width(samp_width),
@@ -619,14 +679,28 @@
         
         buf = self.generate_note_buffer(notes[0], wave_type, duration, volume)
         for n in notes[1:]:
             buf += self.generate_note_buffer(n, wave_type, duration, volume)
         return (buf/len(notes))
     
     
+    def record(self, secs: float):
+        total_frames: bytes = bytes()
+        n_chunks = int(self.input_rate/self.input_chunk*secs)
+        
+        for _ in range(0, n_chunks):
+            data = self.input_stream.read(self.input_chunk)
+            total_frames += data
+        
+        self.input_stream.stop_stream()
+        
+        buf = np.frombuffer(total_frames, self.input_dtype)
+        return buf
+    
+    
     # creates a note buffer and plays it
     def play(self, note:str|float|int, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a note with the given arguments"""
         buf: bytes = self.generate_note_buffer(note, wave_type, duration, volume).tobytes()
     
         self.play_buffer(buf)
     
@@ -634,14 +708,15 @@
     # plays a buffer
     def play_buffer(self, wave: np.ndarray|bytes) -> None:
         """plays the given wave"""
         if type(wave) != bytes:
             wave = wave.tobytes()
         
         self.stream.write(wave)
+        self.stream.stop_stream()
     
     
     # created a chord sound buffer and plays it
     def play_chord(self, notes: Iterable, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a chord with the given arguments"""
         buf = self.generate_chord_buffer(notes, wave_type, duration, volume).tobytes()
         
@@ -697,10 +772,15 @@
         plt.xlim(0, duration)
         plt.colorbar()
         plt.show()
     
     
     def done(self) -> None:
         """will stop and close the stream and terminate the audio_object (basicly closes everything)"""
-        self.stream.stop_stream()
+        if not self.stream.is_stopped():
+            self.stream.stop_stream()
+        if not self.input_stream.is_stopped():
+            self.input_stream.stop_stream()
+        
         self.stream.close()
-        self.AUDIO_OBJECT.terminate()
+        self.input_stream.close()
+        self.AUDIO_OBJECT.terminate()
```

