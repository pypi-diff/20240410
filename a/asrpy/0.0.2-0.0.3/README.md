# Comparing `tmp/asrpy-0.0.2.tar.gz` & `tmp/asrpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asrpy-0.0.2.tar", last modified: Mon Oct 24 10:59:30 2022, max compression
+gzip compressed data, was "asrpy-0.0.3.tar", last modified: Wed Apr 10 11:44:33 2024, max compression
```

## Comparing `asrpy-0.0.2.tar` & `asrpy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 10:59:30.000000 asrpy-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     3709 2022-10-24 10:59:30.000000 asrpy-0.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy/
--rw-r--r--   0 root         (0) root         (0)      309 2022-10-24 10:59:23.000000 asrpy-0.0.2/asrpy/asrpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34594 2022-10-24 10:59:23.000000 asrpy-0.0.2/asrpy/asrpy/asr.py
--rw-r--r--   0 root         (0) root         (0)    17618 2022-10-24 10:59:23.000000 asrpy-0.0.2/asrpy/asrpy/asr_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3709 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-10-24 10:59:30.000000 asrpy-0.0.2/asrpy/asrpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-24 10:59:30.000000 asrpy-0.0.2/setup.cfg
+drwxr-x---   0 guetlid95 (405022) agauksztulewicz (21258)        0 2024-04-10 11:44:33.416723 asrpy-0.0.3/
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)     3689 2024-04-10 11:44:33.413658 asrpy-0.0.3/PKG-INFO
+drwxr-x---   0 guetlid95 (405022) agauksztulewicz (21258)        0 2024-04-10 11:44:33.317623 asrpy-0.0.3/asrpy/
+drwxr-x---   0 guetlid95 (405022) agauksztulewicz (21258)        0 2024-04-10 11:44:33.348855 asrpy-0.0.3/asrpy/asrpy/
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)      309 2024-04-10 11:36:31.000000 asrpy-0.0.3/asrpy/asrpy/__init__.py
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)    34662 2024-04-10 11:36:31.000000 asrpy-0.0.3/asrpy/asrpy/asr.py
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)    17622 2024-04-10 11:36:31.000000 asrpy-0.0.3/asrpy/asrpy/asr_utils.py
+drwxr-x---   0 guetlid95 (405022) agauksztulewicz (21258)        0 2024-04-10 11:44:33.407507 asrpy-0.0.3/asrpy/asrpy.egg-info/
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)     3689 2024-04-10 11:44:32.000000 asrpy-0.0.3/asrpy/asrpy.egg-info/PKG-INFO
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)      241 2024-04-10 11:44:33.000000 asrpy-0.0.3/asrpy/asrpy.egg-info/SOURCES.txt
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)        1 2024-04-10 11:44:32.000000 asrpy-0.0.3/asrpy/asrpy.egg-info/dependency_links.txt
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)       16 2024-04-10 11:44:32.000000 asrpy-0.0.3/asrpy/asrpy.egg-info/requires.txt
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)        6 2024-04-10 11:44:32.000000 asrpy-0.0.3/asrpy/asrpy.egg-info/top_level.txt
+-rw-r-----   0 guetlid95 (405022) agauksztulewicz (21258)       38 2024-04-10 11:44:33.417887 asrpy-0.0.3/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `asrpy-0.0.2/PKG-INFO` & `asrpy-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: asrpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Artifact Subspace Reconstruction in Python.
 Home-page: https://github.com/DiGyt/asrpy
 Author: Dirk Gütlin
 Author-email: dirk.guetlin@gmail.com
 License: BSD-3
 Keywords: EEG MEG Signal Processing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 
 # ASRpy
 Artifact Subspace Reconstruction for Python
@@ -105,9 +104,7 @@
 twine upload dist/*
 -->
 
 
 
 
 
-
-
```

### Comparing `asrpy-0.0.2/asrpy/asrpy/asr.py` & `asrpy-0.0.3/asrpy/asrpy/asr.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,17 +751,17 @@
 
     # sort z scores into quantiles
     wz[np.isnan(wz)] = np.inf  # Nan to inf
     swz = np.sort(wz, axis=0)
 
     # determine which windows to remove
     if np.max(zthresholds) > 0:
-        mask1 = swz[-(np.int(max_bad_chans) + 1), :] > np.max(zthresholds)
+        mask1 = swz[-(int(max_bad_chans) + 1), :] > np.max(zthresholds)
     if np.min(zthresholds) < 0:
-        mask2 = (swz[1 + np.int(max_bad_chans - 1), :] < np.min(zthresholds))
+        mask2 = (swz[1 + int(max_bad_chans - 1), :] < np.min(zthresholds))
 
     # combine the two thresholds
     remove_mask = np.logical_or.reduce((mask1, mask2))
     removed_wins = np.where(remove_mask)
 
     # reconstruct the samples to remove
     sample_maskidx = []
@@ -780,9 +780,11 @@
     sample_mask2remove = np.unique(sample_maskidx)
     if sample_mask2remove.size:
         clean = np.delete(X, sample_mask2remove, 1)
         sample_mask = np.ones((1, ns), dtype=bool)
         sample_mask[0, sample_mask2remove] = False
     else:
         sample_mask = np.ones((1, ns), dtype=bool)
+        clean = X
+        print('Try calibrating ASR with cleaner data.')
 
     return clean, sample_mask
```

### Comparing `asrpy-0.0.2/asrpy/asrpy/asr_utils.py` & `asrpy-0.0.3/asrpy/asrpy/asr_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             1 / shape_range[b], np.sign(quants - 1 / 2) * (2 * quants - 1))
         zbounds.append(np.sign(quants - 1 / 2) * gam ** (1 / shape_range[b]))
         rescale.append(shape_range[b] / (2 * gamma(1 / shape_range[b])))
 
     # determine the quantile-dependent limits for the grid search
     # we can generally skip the tail below the lower quantile
     lower_min = np.min(quants)
-    # maximum width is the fit interval if all data is clean
+    # maximum width is the fit interval if all data is cleanT
     max_width = np.diff(quants)
     # minimum width of the fit interval, as fraction of data
     min_width = min_clean_fraction * max_width
 
     # Build quantile interval matrix
     cols = np.arange(lower_min,
                      lower_min + max_dropout_fraction + step_sizes[0] * 1e-9,
@@ -262,15 +262,15 @@
     # compute additive decomposition
     Qh = numf(np.concatenate((R[0] / 2, R[1:nr]), axis=None), A, order)
 
     # compute impulse response
     _, Ss = 2 * np.real(signal.freqz(Qh, A, worN=n, whole=True))
 
     hh = np.fft.ifft(
-        np.exp(np.fft.fft(Rwindow * np.fft.ifft(np.log(Ss, dtype=np.complex))))  # noqa
+        np.exp(np.fft.fft(Rwindow * np.fft.ifft(np.log(Ss, dtype=np.complex128))))  # noqa
     )
     B = np.real(numf(hh[0:nr], A, nb))
 
     return B, A
 
 
 def yulewalk_filter(X, sfreq, zi=None, ab=None, axis=-1):
```

### Comparing `asrpy-0.0.2/asrpy/asrpy.egg-info/PKG-INFO` & `asrpy-0.0.3/asrpy/asrpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: asrpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Artifact Subspace Reconstruction in Python.
 Home-page: https://github.com/DiGyt/asrpy
 Author: Dirk Gütlin
 Author-email: dirk.guetlin@gmail.com
 License: BSD-3
 Keywords: EEG MEG Signal Processing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 
 # ASRpy
 Artifact Subspace Reconstruction for Python
@@ -105,9 +104,7 @@
 twine upload dist/*
 -->
 
 
 
 
 
-
-
```

