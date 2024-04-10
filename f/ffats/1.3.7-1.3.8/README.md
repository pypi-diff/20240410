# Comparing `tmp/ffats-1.3.7.tar.gz` & `tmp/ffats-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffats-1.3.7.tar", last modified: Sat Apr  6 22:11:12 2024, max compression
+gzip compressed data, was "ffats-1.3.8.tar", last modified: Wed Apr 10 17:28:56 2024, max compression
```

## Comparing `ffats-1.3.7.tar` & `ffats-1.3.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      347 2024-04-06 21:16:24.000000 ffats-1.3.7/CMakeLists.txt
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/FFATS/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      166 2024-04-04 07:15:17.000000 ffats-1.3.7/FFATS/Base.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     7007 2024-04-04 07:31:13.000000 ffats-1.3.7/FFATS/Feature.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)    36472 2024-04-06 21:53:29.000000 ffats-1.3.7/FFATS/FeatureFunctionLib.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      785 2024-04-04 07:15:55.000000 ffats-1.3.7/FFATS/PreprocessLC.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      221 2024-04-04 07:01:49.000000 ffats-1.3.7/FFATS/__init__.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1945 2024-04-04 08:05:18.000000 ffats-1.3.7/FFATS/alignLC.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      157 2024-04-04 07:30:52.000000 ffats-1.3.7/FFATS/featureFunction.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      706 2024-04-04 07:15:38.000000 ffats-1.3.7/FFATS/import_lc_cluster.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      724 2024-04-04 07:15:42.000000 ffats-1.3.7/FFATS/import_lightcurve.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     6572 2024-04-04 07:37:28.000000 ffats-1.3.7/FFATS/lomb.py
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/FFATS/pybind11_CAR/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1975 2024-04-06 19:52:30.000000 ffats-1.3.7/FFATS/pybind11_CAR/fast_CAR.cpp
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)    11062 2024-04-06 19:33:32.000000 ffats-1.3.7/FFATS/test_library.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1079 2024-04-04 06:18:41.000000 ffats-1.3.7/LICENSE
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       64 2024-04-06 21:21:16.000000 ffats-1.3.7/MANIFEST.in
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-06 22:11:12.316820 ffats-1.3.7/PKG-INFO
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      581 2024-04-06 18:30:47.000000 ffats-1.3.7/README.rst
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/ffats.egg-info/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/PKG-INFO
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      521 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/SOURCES.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/dependency_links.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 20:10:00.000000 ffats-1.3.7/ffats.egg-info/not-zip-safe
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/requires.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       15 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/top_level.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      143 2024-04-06 21:50:16.000000 ffats-1.3.7/pyproject.toml
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 18:19:27.000000 ffats-1.3.7/requirements.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       38 2024-04-06 22:11:12.316820 ffats-1.3.7/setup.cfg
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     9421 2024-04-06 21:55:51.000000 ffats-1.3.7/setup.py
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      347 2024-04-06 21:16:24.000000 ffats-1.3.8/CMakeLists.txt
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/FFATS/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      166 2024-04-04 07:15:17.000000 ffats-1.3.8/FFATS/Base.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     7007 2024-04-04 07:31:13.000000 ffats-1.3.8/FFATS/Feature.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)    36484 2024-04-10 17:13:13.000000 ffats-1.3.8/FFATS/FeatureFunctionLib.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      785 2024-04-04 07:15:55.000000 ffats-1.3.8/FFATS/PreprocessLC.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      221 2024-04-04 07:01:49.000000 ffats-1.3.8/FFATS/__init__.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1945 2024-04-04 08:05:18.000000 ffats-1.3.8/FFATS/alignLC.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      157 2024-04-04 07:30:52.000000 ffats-1.3.8/FFATS/featureFunction.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      706 2024-04-04 07:15:38.000000 ffats-1.3.8/FFATS/import_lc_cluster.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      724 2024-04-04 07:15:42.000000 ffats-1.3.8/FFATS/import_lightcurve.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     6572 2024-04-04 07:37:28.000000 ffats-1.3.8/FFATS/lomb.py
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/FFATS/pybind11_CAR/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1975 2024-04-06 19:52:30.000000 ffats-1.3.8/FFATS/pybind11_CAR/fast_CAR.cpp
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)    10756 2024-04-10 17:17:51.000000 ffats-1.3.8/FFATS/test_library.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1079 2024-04-04 06:18:41.000000 ffats-1.3.8/LICENSE
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       64 2024-04-06 21:21:16.000000 ffats-1.3.8/MANIFEST.in
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-10 17:28:56.784040 ffats-1.3.8/PKG-INFO
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      581 2024-04-06 18:30:47.000000 ffats-1.3.8/README.rst
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/ffats.egg-info/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/PKG-INFO
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      521 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 20:10:00.000000 ffats-1.3.8/ffats.egg-info/not-zip-safe
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/requires.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       15 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/top_level.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      143 2024-04-06 21:50:16.000000 ffats-1.3.8/pyproject.toml
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 18:19:27.000000 ffats-1.3.8/requirements.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       38 2024-04-10 17:28:56.784040 ffats-1.3.8/setup.cfg
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     9421 2024-04-10 17:28:42.000000 ffats-1.3.8/setup.py
```

### Comparing `ffats-1.3.7/FFATS/Feature.py` & `ffats-1.3.8/FFATS/Feature.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/FeatureFunctionLib.py` & `ffats-1.3.8/FFATS/FeatureFunctionLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class Amplitude(Base):
     """Half the difference between the maximum and the minimum magnitude"""
 
     def __init__(self):
         self.Data = ['magnitude']
 
     def fit(self, data):
-        magnitude = data
+        magnitude = data[0]
         N = magnitude.shape[0]
         sorted_mag = np.sort(magnitude)
 
         return (np.median(sorted_mag[-int(math.ceil(0.05 * N)):]) -
                 np.median(sorted_mag[0:int(math.ceil(0.05 * N))])) / 2.0
 
 
@@ -85,15 +85,15 @@
 
     def __init__(self, lags=100):
         self.Data = ['magnitude']
         self.nlags = lags
 
     def fit(self, data):
 
-        magnitude = data
+        magnitude = data[0]
         AC = stattools.acf(magnitude, nlags=self.nlags)
         k = next((index for index, value in
                  enumerate(AC) if value < np.exp(-1)), None)
 
         while k is None:
             self.nlags = self.nlags + 100
             AC = stattools.acf(magnitude, nlags=self.nlags)
@@ -496,15 +496,15 @@
     of the median magnitude
     """
 
     def __init__(self):
         self.Data = ['magnitude']
 
     def fit(self, data):
-        magnitude = data
+        magnitude = data[0]
         median = np.median(magnitude)
         amplitude = (np.max(magnitude) - np.min(magnitude)) / 10
         n = magnitude.shape[0]
 
         count = np.sum(np.logical_and(magnitude < median + amplitude,
                                       magnitude > median - amplitude))
 
@@ -641,15 +641,15 @@
 
 class PercentDifferenceFluxPercentile(Base):
 
     def __init__(self):
         self.Data = ['magnitude']
 
     def fit(self, data):
-        magnitude = data
+        magnitude = data[0]
         median_data = np.median(magnitude)
 
         sorted_data = np.sort(magnitude)
         lc_length = len(sorted_data)
         F_5_index = int(math.ceil(0.05 * lc_length))
         F_95_index = int(math.ceil(0.95 * lc_length))
         F_5_95 = sorted_data[F_95_index] - sorted_data[F_5_index]
```

### Comparing `ffats-1.3.7/FFATS/PreprocessLC.py` & `ffats-1.3.8/FFATS/PreprocessLC.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/alignLC.py` & `ffats-1.3.8/FFATS/alignLC.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/import_lc_cluster.py` & `ffats-1.3.8/FFATS/import_lc_cluster.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/import_lightcurve.py` & `ffats-1.3.8/FFATS/import_lightcurve.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/lomb.py` & `ffats-1.3.8/FFATS/lomb.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/pybind11_CAR/fast_CAR.cpp` & `ffats-1.3.8/FFATS/pybind11_CAR/fast_CAR.cpp`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/FFATS/test_library.py` & `ffats-1.3.8/FFATS/test_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,47 +75,39 @@
     time_rw = np.array(range(0, N)) + 1 * np.random.uniform(size=N)
     data_rw = data_rw.squeeze()
     lc = np.array([data_rw, time_rw])
     return lc
 
 @pytest.fixture
 def sequence():
-    return range(1000)
+    return np.arange(1000).reshape(1, -1)
 
 
 def test_Amplitude(benchmark, sequence):
     a = FeatureSpace(featureList=['Amplitude'])
     a = benchmark(a.calculateFeature, sequence)
 
     # Exact value is 475 but I add some space for an error
     assert(a.result(method='array') >= 474.9 and a.result(method='array') <= 475.1)
 
 
 def test_Autocor(benchmark, periodic_lc):
     a = FeatureSpace(featureList=['Autocor_length'])
-    a = benchmark(a.calculateFeature, periodic_lc[:, 0])
+    a = benchmark(a.calculateFeature, periodic_lc)
 
     assert(a.result(method='array') == 1)
 
 
 def test_bench_Autocor(benchmark, white_noise):
     a = FeatureSpace(featureList=['Autocor_length'])
-    a = benchmark(a.calculateFeature, white_noise[:, 0])
+    a = benchmark(a.calculateFeature, white_noise)
 
     assert(a.result(method='array') == 1)
 
 
-@pytest.mark.skip('Automean was removed from the library')
-def test_Automean(benchmark, white_noise):
-    a = FeatureSpace(featureList=['Automean'] , Automean=[0,0])
-    a = benchmark(a.calculateFeature, white_noise[0])
-
-    assert(a.result(method='array') >= 0.043 and a.result(method='array') <= 0.046)
-
-
 @pytest.mark.skip('Invalid assertions')
 def test_B_R(benchmark, white_noise):
     a = FeatureSpace(featureList=['Q31_color'])
     a = benchmark(a.calculateFeature, white_noise)
 
     assert(a.result(method='array') >= 0.043 and a.result(method='array') <= 0.046)
 
@@ -258,15 +250,15 @@
     a = benchmark(a.calculateFeature, white_noise)
     assert (a.result(method='array') >=
             1.30 and a.result(method='array') <= 1.38)
 
 @pytest.mark.skip('No assertions')
 def test_Q31B_R(benchmark, white_noise):
     a = FeatureSpace(featureList=['Q31B_R'], Q31B_R = [aligned_second_data, aligned_data])
-    a = benchmark(a.calculateFeature, white_noise[0])
+    a = benchmark(a.calculateFeature, white_noise)
 
 
 def test_Rcs(benchmark, white_noise):
     a = FeatureSpace(featureList=['Rcs'])
     a = benchmark(a.calculateFeature, white_noise)
     assert (a.result(method='array') >= 0 and a.result(method='array') <= 0.1)
 
@@ -277,15 +269,15 @@
     assert (a.result(method='array') >= -
             0.1 and a.result(method='array') <= 0.1)
 
 
 @pytest.mark.skip('No assertions')
 def test_SlottedA(benchmark, white_noise):
     a = FeatureSpace(featureList=['SlottedA'], SlottedA = [mjd, 1])
-    a = benchmark(a.calculateFeature, white_noise[0])
+    a = benchmark(a.calculateFeature, white_noise)
 
 def test_SmallKurtosis(benchmark, white_noise):
     a = FeatureSpace(featureList=['SmallKurtosis'])
     a = benchmark(a.calculateFeature, white_noise)
     assert (a.result(method='array') >= -
             0.2 and a.result(method='array') <= 0.2)
```

### Comparing `ffats-1.3.7/LICENSE` & `ffats-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/PKG-INFO` & `ffats-1.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffats
-Version: 1.3.7
+Version: 1.3.8
 Summary: Library with compilation of features for time series
 Home-page: https://github.com/vBazilevich/FFATS
 Download-URL: https://github.com/vBazilevich/FFATS
 Author: Vladimir Bazilevich
 Author-email: bazilevichvl@gmail.com
 License: MIT licence
 Keywords: times series features,light curves
```

### Comparing `ffats-1.3.7/README.rst` & `ffats-1.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/ffats.egg-info/PKG-INFO` & `ffats-1.3.8/ffats.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffats
-Version: 1.3.7
+Version: 1.3.8
 Summary: Library with compilation of features for time series
 Home-page: https://github.com/vBazilevich/FFATS
 Download-URL: https://github.com/vBazilevich/FFATS
 Author: Vladimir Bazilevich
 Author-email: bazilevichvl@gmail.com
 License: MIT licence
 Keywords: times series features,light curves
```

### Comparing `ffats-1.3.7/ffats.egg-info/SOURCES.txt` & `ffats-1.3.8/ffats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffats-1.3.7/setup.py` & `ffats-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
 setup(
     name='ffats',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/development.html#single-sourcing-the-version
-    version='1.3.7',
+    version='1.3.8',
 
     description='Library with compilation of features for time series',
     long_description=readme(),
     # The project's main homepage.
     url='https://github.com/vBazilevich/FFATS',
 
     download_url = 'https://github.com/vBazilevich/FFATS',
```

