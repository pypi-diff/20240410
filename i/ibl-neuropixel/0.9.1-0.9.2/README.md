# Comparing `tmp/ibl-neuropixel-0.9.1.tar.gz` & `tmp/ibl-neuropixel-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl-neuropixel-0.9.1.tar", last modified: Thu Feb  8 17:31:35 2024, max compression
+gzip compressed data, was "ibl-neuropixel-0.9.2.tar", last modified: Thu Feb  8 18:31:34 2024, max compression
```

## Comparing `ibl-neuropixel-0.9.1.tar` & `ibl-neuropixel-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:35.184793 ibl-neuropixel-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-08 17:31:35.184793 ibl-neuropixel-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 17:31:35.184793 ibl-neuropixel-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:35.180793 ibl-neuropixel-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:35.184793 ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-08 17:31:35.000000 ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-08 17:31:35.000000 ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 17:31:35.000000 ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-08 17:31:35.000000 ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-08 17:31:35.000000 ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:35.184793 ibl-neuropixel-0.9.1/src/ibldsp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/cadzow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/cuda_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/destripe_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/filter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/raw_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/spiketrains.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)    22018 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/ibldsp/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    36357 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/neuropixel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:35.184793 ibl-neuropixel-0.9.1/src/neurowaveforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/neurowaveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/neurowaveforms/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    34528 2024-02-08 17:31:28.000000 ibl-neuropixel-0.9.1/src/spikeglx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.212475 ibl-neuropixel-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-08 18:31:34.000000 ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/ibldsp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/cadzow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/cuda_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/destripe_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/filter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/raw_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/spiketrains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/ibldsp/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/neurodsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neurodsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36357 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neuropixel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:34.216475 ibl-neuropixel-0.9.2/src/neurowaveforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neurowaveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/neurowaveforms/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34528 2024-02-08 18:31:27.000000 ibl-neuropixel-0.9.2/src/spikeglx.py
```

### Comparing `ibl-neuropixel-0.9.1/LICENSE` & `ibl-neuropixel-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/PKG-INFO` & `ibl-neuropixel-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.9.1
+Version: 0.9.2
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibl-neuropixel-0.9.1/README.md` & `ibl-neuropixel-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/setup.py` & `ibl-neuropixel-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="0.9.1",
+    version="0.9.2",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
```

### Comparing `ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.9.1
+Version: 0.9.2
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibl-neuropixel-0.9.1/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl-neuropixel-0.9.2/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 src/ibldsp/fourier.py
 src/ibldsp/raw_metrics.py
 src/ibldsp/smooth.py
 src/ibldsp/spiketrains.py
 src/ibldsp/utils.py
 src/ibldsp/voltage.py
 src/ibldsp/waveforms.py
+src/neurodsp/__init__.py
 src/neurowaveforms/__init__.py
 src/neurowaveforms/model.py
```

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/cadzow.py` & `ibl-neuropixel-0.9.2/src/ibldsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/cuda_tools.py` & `ibl-neuropixel-0.9.2/src/ibldsp/cuda_tools.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/destripe_gpu.py` & `ibl-neuropixel-0.9.2/src/ibldsp/destripe_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/filter_gpu.py` & `ibl-neuropixel-0.9.2/src/ibldsp/filter_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/fourier.py` & `ibl-neuropixel-0.9.2/src/ibldsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/raw_metrics.py` & `ibl-neuropixel-0.9.2/src/ibldsp/raw_metrics.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/smooth.py` & `ibl-neuropixel-0.9.2/src/ibldsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/spiketrains.py` & `ibl-neuropixel-0.9.2/src/ibldsp/spiketrains.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/utils.py` & `ibl-neuropixel-0.9.2/src/ibldsp/utils.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/voltage.py` & `ibl-neuropixel-0.9.2/src/ibldsp/voltage.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/ibldsp/waveforms.py` & `ibl-neuropixel-0.9.2/src/ibldsp/waveforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -251,43 +251,42 @@
     x = x[order] + x_shift + 1
     ax.fill(y, x, 'k', aa=True)
     ax.set(xlim=[0, ns], ylim=[0, nc], xlabel='sample', ylabel='trace')
     plt.tight_layout()
     return ax
 
 
-def plot_peaktiptrough(df, arr, ax=None, nth_wav=0, plot_grey=True):
-    """
-    Plots the peak, tip and trough of a waveform to check the feature extraction
-    :param df:
-    :param arr:
-    :param ax:
-    :param nth_wav:
-    :param plot_grey:
-    :return:
-    """
+def plot_peaktiptrough(df, arr, ax, nth_wav=0, plot_grey=True, fs=30000):
+    # Time axix
+    nech, ntr = arr[nth_wav].shape
+    tscale = np.array([0, nech - 1]) / fs * 1e3
+
     if ax is None:
         fig, ax = plt.subplots()
     if plot_grey:
-        ax.plot(arr[nth_wav], c='gray', alpha=0.5)
+        ax.plot(tscale, arr[nth_wav], c='gray', alpha=0.5)
     # Peak channel
-    ax.plot(arr[nth_wav][:, int(df.iloc[nth_wav].peak_trace_idx)], marker=".", c='blue')
+    ax.plot(tscale, arr[nth_wav][:, int(df.iloc[nth_wav].peak_trace_idx)], marker=".", c='blue')
     # Peak point
-    ax.plot(df.iloc[nth_wav].peak_time_idx, df.iloc[nth_wav].peak_val, 'r*')
+    ax.plot(tscale[df.iloc[nth_wav].peak_time_idx], df.iloc[nth_wav].peak_val, 'r*')
     # Trough point
-    ax.plot(df.iloc[nth_wav].trough_time_idx, df.iloc[nth_wav].trough_val, 'g*')
+    ax.plot(tscale[df.iloc[nth_wav].trough_time_idx], df.iloc[nth_wav].trough_val, 'g*')
     # Tip point
-    ax.plot(df.iloc[nth_wav].tip_time_idx, df.iloc[nth_wav].tip_val, 'k*')
+    ax.plot(tscale[df.iloc[nth_wav].tip_time_idx], df.iloc[nth_wav].tip_val, 'k*')
     # Half peak points
-    ax.plot(df.iloc[nth_wav].half_peak_post_time_idx, df.iloc[nth_wav].half_peak_post_val, 'c*')
-    ax.plot(df.iloc[nth_wav].half_peak_pre_time_idx, df.iloc[nth_wav].half_peak_pre_val, 'c*')
+    ax.plot(tscale[df.iloc[nth_wav].half_peak_post_time_idx], df.iloc[nth_wav].half_peak_post_val, 'c*')
+    ax.plot(tscale[df.iloc[nth_wav].half_peak_pre_time_idx], df.iloc[nth_wav].half_peak_pre_val, 'c*')
     # Line for half peak boundary
-    ax.plot((0, arr.shape[1]), np.array((1, 1)) * df.iloc[nth_wav].peak_val / 2, '-k')
+    # ax.plot((0, arr.shape[1]), np.array((1, 1)) * df.iloc[nth_wav].peak_val / 2, '-k')
+    ax.plot((tscale[0], tscale[-1]), np.array((1, 1)) * df.iloc[nth_wav].peak_val / 2, '-k')
     # Recovery point
-    ax.plot(df.iloc[nth_wav].recovery_time_idx, df.iloc[nth_wav].recovery_val, 'y*')
+    ax.plot(tscale[df.iloc[nth_wav].recovery_time_idx], df.iloc[nth_wav].recovery_val, 'y*')
+    # Axis labels
+    ax.set_ylabel('(Volt)')
+    ax.set_xlabel('Time (ms)')
 
 
 def half_peak_point(arr_peak, df):
     '''
     Compute the two intersection points at halp-maximum peak
     :param: arr_peak: NxT waveform matrix : spikes x time, only the peak channel (inverted for positive wavs)
     :return: df with columns containing indices of intersection points and values, length of N wav
```

### Comparing `ibl-neuropixel-0.9.1/src/neuropixel.py` & `ibl-neuropixel-0.9.2/src/neuropixel.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/neurowaveforms/model.py` & `ibl-neuropixel-0.9.2/src/neurowaveforms/model.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.9.1/src/spikeglx.py` & `ibl-neuropixel-0.9.2/src/spikeglx.py`

 * *Files identical despite different names*

