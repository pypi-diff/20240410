# Comparing `tmp/utils2p-1.0.0.tar.gz` & `tmp/utils2p-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils2p-1.0.0.tar", last modified: Mon Oct 23 11:52:25 2023, max compression
+gzip compressed data, was "utils2p-1.0.1.tar", last modified: Wed Apr 10 09:36:27 2024, max compression
```

## Comparing `utils2p-1.0.0.tar` & `utils2p-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-10-23 11:52:25.801575 utils2p-1.0.0/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     1103 2023-10-16 14:20:41.000000 utils2p-1.0.0/LICENSE
--rw-r--r--   0 phelps   (253699) upramdya (11350)     2087 2023-10-23 11:52:25.801575 utils2p-1.0.0/PKG-INFO
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     1685 2023-10-16 14:20:41.000000 utils2p-1.0.0/README.rst
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       38 2023-10-23 11:52:25.801575 utils2p-1.0.0/setup.cfg
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     1216 2023-10-23 11:50:14.000000 utils2p-1.0.0/setup.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-10-23 11:52:25.801575 utils2p-1.0.0/tests/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     8411 2023-10-16 14:20:41.000000 utils2p-1.0.0/tests/test_external_tifffile.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)    21010 2023-10-16 14:20:41.000000 utils2p-1.0.0/tests/test_main.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)    17973 2023-10-16 14:20:41.000000 utils2p-1.0.0/tests/test_synchronization.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-10-23 11:52:25.801575 utils2p-1.0.0/utils2p/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)      112 2023-10-23 11:51:05.000000 utils2p-1.0.0/utils2p/__init__.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-10-23 11:52:25.801575 utils2p-1.0.0/utils2p/external/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)        0 2023-10-16 14:20:41.000000 utils2p-1.0.0/utils2p/external/__init__.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-10-23 11:52:25.801575 utils2p-1.0.0/utils2p/external/tifffile/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)      281 2023-10-16 14:20:41.000000 utils2p-1.0.0/utils2p/external/tifffile/__init__.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)    29817 2023-10-16 14:20:41.000000 utils2p-1.0.0/utils2p/external/tifffile/tifffile.c
--rw-rw-r--   0 phelps   (253699) upramdya (11350)   236992 2023-10-16 14:20:41.000000 utils2p-1.0.0/utils2p/external/tifffile/tifffile.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)    45158 2023-10-16 14:20:41.000000 utils2p-1.0.0/utils2p/main.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)    43769 2023-10-16 14:20:41.000000 utils2p-1.0.0/utils2p/synchronization.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-10-23 11:52:25.801575 utils2p-1.0.0/utils2p.egg-info/
--rw-r--r--   0 phelps   (253699) upramdya (11350)     2087 2023-10-23 11:52:25.000000 utils2p-1.0.0/utils2p.egg-info/PKG-INFO
--rw-rw-r--   0 phelps   (253699) upramdya (11350)      467 2023-10-23 11:52:25.000000 utils2p-1.0.0/utils2p.egg-info/SOURCES.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)        1 2023-10-23 11:52:25.000000 utils2p-1.0.0/utils2p.egg-info/dependency_links.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       24 2023-10-23 11:52:25.000000 utils2p-1.0.0/utils2p.egg-info/requires.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)        8 2023-10-23 11:52:25.000000 utils2p-1.0.0/utils2p.egg-info/top_level.txt
+drwxr-xr-x   0 azcorra    (502) staff       (20)        0 2024-04-10 09:36:27.516348 utils2p-1.0.1/
+-rw-r--r--   0 azcorra    (502) staff       (20)     1103 2024-04-10 09:24:08.000000 utils2p-1.0.1/LICENSE
+-rw-r--r--   0 azcorra    (502) staff       (20)     2087 2024-04-10 09:36:27.516115 utils2p-1.0.1/PKG-INFO
+-rw-r--r--   0 azcorra    (502) staff       (20)     1685 2024-04-10 09:24:08.000000 utils2p-1.0.1/README.rst
+-rw-r--r--   0 azcorra    (502) staff       (20)       38 2024-04-10 09:36:27.516409 utils2p-1.0.1/setup.cfg
+-rw-r--r--   0 azcorra    (502) staff       (20)     1216 2024-04-10 09:35:24.000000 utils2p-1.0.1/setup.py
+drwxr-xr-x   0 azcorra    (502) staff       (20)        0 2024-04-10 09:36:27.514402 utils2p-1.0.1/tests/
+-rw-r--r--   0 azcorra    (502) staff       (20)     8411 2024-04-10 09:24:08.000000 utils2p-1.0.1/tests/test_external_tifffile.py
+-rw-r--r--   0 azcorra    (502) staff       (20)    21004 2024-04-10 09:24:08.000000 utils2p-1.0.1/tests/test_main.py
+-rw-r--r--   0 azcorra    (502) staff       (20)    17973 2024-04-10 09:24:08.000000 utils2p-1.0.1/tests/test_synchronization.py
+drwxr-xr-x   0 azcorra    (502) staff       (20)        0 2024-04-10 09:36:27.514763 utils2p-1.0.1/utils2p/
+-rw-r--r--   0 azcorra    (502) staff       (20)      112 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/__init__.py
+drwxr-xr-x   0 azcorra    (502) staff       (20)        0 2024-04-10 09:36:27.515495 utils2p-1.0.1/utils2p/external/
+-rw-r--r--   0 azcorra    (502) staff       (20)        0 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/external/__init__.py
+drwxr-xr-x   0 azcorra    (502) staff       (20)        0 2024-04-10 09:36:27.515828 utils2p-1.0.1/utils2p/external/tifffile/
+-rw-r--r--   0 azcorra    (502) staff       (20)      281 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/external/tifffile/__init__.py
+-rw-r--r--   0 azcorra    (502) staff       (20)    29817 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/external/tifffile/tifffile.c
+-rw-r--r--   0 azcorra    (502) staff       (20)   236992 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/external/tifffile/tifffile.py
+-rw-r--r--   0 azcorra    (502) staff       (20)    45158 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/main.py
+-rw-r--r--   0 azcorra    (502) staff       (20)    43748 2024-04-10 09:24:08.000000 utils2p-1.0.1/utils2p/synchronization.py
+drwxr-xr-x   0 azcorra    (502) staff       (20)        0 2024-04-10 09:36:27.515387 utils2p-1.0.1/utils2p.egg-info/
+-rw-r--r--   0 azcorra    (502) staff       (20)     2087 2024-04-10 09:36:27.000000 utils2p-1.0.1/utils2p.egg-info/PKG-INFO
+-rw-r--r--   0 azcorra    (502) staff       (20)      467 2024-04-10 09:36:27.000000 utils2p-1.0.1/utils2p.egg-info/SOURCES.txt
+-rw-r--r--   0 azcorra    (502) staff       (20)        1 2024-04-10 09:36:27.000000 utils2p-1.0.1/utils2p.egg-info/dependency_links.txt
+-rw-r--r--   0 azcorra    (502) staff       (20)       24 2024-04-10 09:36:27.000000 utils2p-1.0.1/utils2p.egg-info/requires.txt
+-rw-r--r--   0 azcorra    (502) staff       (20)        8 2024-04-10 09:36:27.000000 utils2p-1.0.1/utils2p.egg-info/top_level.txt
```

### Comparing `utils2p-1.0.0/LICENSE` & `utils2p-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/PKG-INFO` & `utils2p-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils2p
-Version: 1.0.0
+Version: 1.0.1
 Summary: Basic utility functions for 2 photon image data generated using ThorImage and ThorSync.
 Home-page: https://github.com/NeLy-EPFL/utils2p
 Author: Florian Aymanns
 Author-email: florian.aymanns@epfl.ch
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `utils2p-1.0.0/README.rst` & `utils2p-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/setup.py` & `utils2p-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     sources=["utils2p/external/tifffile/tifffile.c"],
     include_dirs=[np.get_include()],
 )
 
 
 setup(
     name="utils2p",
-    version="1.0.0",
+    version="1.0.1",
     packages=["utils2p", "utils2p.external", "utils2p.external.tifffile"],
     author="Florian Aymanns",
     author_email="florian.aymanns@epfl.ch",
     description="Basic utility functions for 2 photon image data generated using ThorImage and ThorSync.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/NeLy-EPFL/utils2p",
```

### Comparing `utils2p-1.0.0/tests/test_external_tifffile.py` & `utils2p-1.0.1/tests/test_external_tifffile.py`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/tests/test_main.py` & `utils2p-1.0.1/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,16 +563,16 @@
     default_exp_dir.joinpath("Untitled_001/Image_0001_0001.raw").unlink()
     with pytest.raises(FileNotFoundError):
         utils2p.find_raw_file(directory)
 
 
 def test_load_optical_flow(tmpdir):
     n_timepoints = 10
-    opt_flow_data = np.zeros((n_timepoints, 5), dtype=np.int)
-    opt_flow_data[:, 4] = np.arange(n_timepoints, dtype=np.int)
+    opt_flow_data = np.zeros((n_timepoints, 5), dtype=int)
+    opt_flow_data[:, 4] = np.arange(n_timepoints, dtype=int)
     opt_flow_data[1, 0] = -1
     opt_flow_data[3, 1] = 1
     opt_flow_data[6, 2] = 2
     opt_flow_data[9, 3] = -3
 
     file_name = os.path.join(tmpdir, "OpFlow.txt")
     np.savetxt(file_name, opt_flow_data, delimiter=",")
```

### Comparing `utils2p-1.0.0/tests/test_synchronization.py` & `utils2p-1.0.1/tests/test_synchronization.py`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/utils2p/external/tifffile/tifffile.c` & `utils2p-1.0.1/utils2p/external/tifffile/tifffile.c`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/utils2p/external/tifffile/tifffile.py` & `utils2p-1.0.1/utils2p/external/tifffile/tifffile.py`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/utils2p/main.py` & `utils2p-1.0.1/utils2p/main.py`

 * *Files identical despite different names*

### Comparing `utils2p-1.0.0/utils2p/synchronization.py` & `utils2p-1.0.1/utils2p/synchronization.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
     first_camera_used = sorted(list(capture_info["Frame Counts"].keys()))[0]
     for i, (start, stop) in enumerate(
             zip(rising_edges[:last_tick], rising_edges[1:last_tick + 1])):
         if capture_info["Frame Counts"][first_camera_used][str(current_frame +
                                                                1)] <= i:
             current_frame += 1
         processed_line[start:stop] = current_frame
-    return processed_line.astype(np.int)
+    return processed_line.astype(int)
 
 
 def process_frame_counter(line, metadata=None, steps_per_frame=None):
     """
     Converts the frame counter line to an array with frame numbers for each
     time point.
 
@@ -510,24 +510,24 @@
 
     processed_frame_counter = np.ones_like(line) * np.nan
     rising_edges = edges(line, (0, np.inf))[0]
 
     # Case of one frame/volume only
     if len(rising_edges) <= steps_per_frame:
         processed_frame_counter[rising_edges[0]:] = 0
-        return processed_frame_counter.astype(np.int)
+        return processed_frame_counter.astype(int)
 
     for i, index in enumerate(
             range(0,
                   len(rising_edges) - steps_per_frame, steps_per_frame)):
         processed_frame_counter[
             rising_edges[index]:rising_edges[index + steps_per_frame]] = i
     processed_frame_counter[rising_edges[-1 * steps_per_frame]:] = (
         processed_frame_counter[rising_edges[-1 * steps_per_frame] - 1] + 1)
-    return processed_frame_counter.astype(np.int)
+    return processed_frame_counter.astype(int)
 
 
 def process_stimulus_line(line):
     """
     This function converts the stimulus line to an array with
     0s and 1s for stimulus off and on respectively. The raw
     stimulus line can contain values larger than 1.
@@ -555,15 +555,15 @@
     >>> processed_stimulus_line = utils2p.synchronization.process_stimulus_line(stimulus_line)
     >>> set(processed_stimulus_line)
     {0, 1}
     """
     processed_stimulus_line = np.zeros_like(line)
     indices = np.where(line > 0)
     processed_stimulus_line[indices] = 1
-    return processed_stimulus_line.astype(np.int)
+    return processed_stimulus_line.astype(int)
 
 
 def process_optical_flow_line(line):
     """
     This function converts the optical flow line
     into a step function. The value corresponds
     to the index of optical flow value at this
@@ -606,15 +606,15 @@
     """
     processed_optical_flow_line = np.ones_like(line) * np.nan
     rising_edges = edges(line, (0, np.inf))[0]
     for i in range(0, len(rising_edges) - 1):
         processed_optical_flow_line[rising_edges[i]:rising_edges[i + 1]] = i
     processed_optical_flow_line[rising_edges[-1]:] = (
         processed_optical_flow_line[rising_edges[-1] - 1] + 1)
-    return processed_optical_flow_line.astype(np.int)
+    return processed_optical_flow_line.astype(int)
 
 
 def crop_lines(mask, lines):
     """
     This function crops all lines based on a binary signal/mask.
     The 'Capture On' line of the h5 file can be used as a mask.
 
@@ -710,29 +710,29 @@
                               1,                    1,                    1,
                               1,                    1,                    1])
     """
     thor_sync_indices = edges(cam_line)[0]
     if not cam_line[0] < 0:
         thor_sync_indices = np.append(np.array([0]), thor_sync_indices)
 
-    indices_2p = np.ones(len(beh_indices), dtype=np.int) * np.nan
+    indices_2p = np.ones(len(beh_indices), dtype=int) * np.nan
 
     first_frame_of_cam_line = np.min(cam_line[np.where(cam_line >= 0)])
 
     for i, frame_num in enumerate(beh_indices):
 
         # This is necessary for cropped lines that don't start at 0
         frame_num = frame_num - first_frame_of_cam_line
         if frame_num < 0:
             raise ValueError(f"{frame_num + first_frame_of_cam_line} is smaller than first frame in cam_line ({first_frame_of_cam_line})")
 
         thor_sync_index = thor_sync_indices[frame_num]
         indices_2p[i] = frame_counter[thor_sync_index]
 
-    return indices_2p.astype(np.int)
+    return indices_2p.astype(int)
 
 
 def reduce_during_2p_frame(frame_counter, values, function):
     """
     Reduces all values occurring during the acquisition of a
     2-photon frame to a single value using the `function`
     given by the user.
```

### Comparing `utils2p-1.0.0/utils2p.egg-info/PKG-INFO` & `utils2p-1.0.1/utils2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils2p
-Version: 1.0.0
+Version: 1.0.1
 Summary: Basic utility functions for 2 photon image data generated using ThorImage and ThorSync.
 Home-page: https://github.com/NeLy-EPFL/utils2p
 Author: Florian Aymanns
 Author-email: florian.aymanns@epfl.ch
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
```

