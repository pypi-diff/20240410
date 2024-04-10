# Comparing `tmp/soundtools-0.1.3.4.tar.gz` & `tmp/soundtools-0.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.1.3.4.tar", last modified: Wed Apr 10 02:12:37 2024, max compression
+gzip compressed data, was "soundtools-0.1.3.5.tar", last modified: Wed Apr 10 02:26:46 2024, max compression
```

## Comparing `soundtools-0.1.3.4.tar` & `soundtools-0.1.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:12:37.192314 soundtools-0.1.3.4/
--rw-rw-rw-   0        0        0      345 2024-04-10 02:12:37.192314 soundtools-0.1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 02:12:37.192314 soundtools-0.1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-04-10 02:11:55.000000 soundtools-0.1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:12:37.181316 soundtools-0.1.3.4/soundtools/
--rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.1.3.4/soundtools/__init__.py
--rw-rw-rw-   0        0        0    32118 2024-04-10 02:11:43.000000 soundtools-0.1.3.4/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:12:37.191314 soundtools-0.1.3.4/soundtools.egg-info/
--rw-rw-rw-   0        0        0      345 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 02:12:37.000000 soundtools-0.1.3.4/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 02:26:46.352314 soundtools-0.1.3.5/
+-rw-rw-rw-   0        0        0      345 2024-04-10 02:26:46.351314 soundtools-0.1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:26:46.352314 soundtools-0.1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-04-10 02:26:04.000000 soundtools-0.1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:26:46.349316 soundtools-0.1.3.5/soundtools/
+-rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.1.3.5/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    32110 2024-04-10 02:25:23.000000 soundtools-0.1.3.5/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:26:46.351314 soundtools-0.1.3.5/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 02:26:46.000000 soundtools-0.1.3.5/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.1.3.4/soundtools/soundtools.py` & `soundtools-0.1.3.5/soundtools/soundtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
         """Iterates recursivelly."""
         try:
             return tuple(self.array_to_tuple(_) for _ in np_array)
         except TypeError:
             return np_array
 
 
-class Export(Sounds):
+class Export:
     def __init__(self) -> None:
         pass
     
     # converts a float32 array to an int type
     def float2pcm(self, sig: np.ndarray, dtype: Literal["int32", "int16", "uint8"]="int16") -> SoundBuffer:
         """gets a float dtype array as input, converts it to int and returns the converted array"""
```

