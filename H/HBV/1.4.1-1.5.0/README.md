# Comparing `tmp/hbv-1.4.1.tar.gz` & `tmp/hbv-1.5.0.tar.gz`

## Comparing `hbv-1.4.1.tar` & `hbv-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.4.1/Dockerfile
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.4.1/MANIFEST.in
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/Forcing.txt
--rw-r--r--   0        0        0   525026 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/Forward model.ipynb
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/HBV_config.json
--rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/HBV_forcing.nc
--rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/Q_m_out_ref.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.4.1/docs/model_layout.png
--rw-r--r--   0        0        0    20165 2020-02-02 00:00:00.000000 hbv-1.4.1/src/HBV/HBV_bmi.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.4.1/src/HBV/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.4.1/src/HBV/utils.py
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 hbv-1.4.1/README.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 hbv-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 hbv-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 hbv-1.5.0/Dockerfile
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hbv-1.5.0/MANIFEST.in
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hbv-1.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    36937 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/Forcing.txt
+-rw-r--r--   0        0        0   525026 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/Forward model.ipynb
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/HBV_config.json
+-rw-r--r--   0        0        0    43177 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/HBV_forcing.nc
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/Q_m_out_ref.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 hbv-1.5.0/docs/model_layout.png
+-rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 hbv-1.5.0/src/HBV/HBV_bmi.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hbv-1.5.0/src/HBV/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hbv-1.5.0/src/HBV/utils.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hbv-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hbv-1.5.0/README.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hbv-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 hbv-1.5.0/PKG-INFO
```

### Comparing `hbv-1.4.1/Dockerfile` & `hbv-1.5.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/.github/workflows/python-publish.yml` & `hbv-1.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/docs/Forcing.txt` & `hbv-1.5.0/docs/Forcing.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/docs/Forward model.ipynb` & `hbv-1.5.0/docs/Forward model.ipynb`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/docs/HBV_forcing.nc` & `hbv-1.5.0/docs/HBV_forcing.nc`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/docs/Q_m_out_ref.txt` & `hbv-1.5.0/docs/Q_m_out_ref.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/docs/model_layout.png` & `hbv-1.5.0/docs/model_layout.png`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/src/HBV/HBV_bmi.py` & `hbv-1.5.0/src/HBV/HBV_bmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         """
         # open json files containing data
         self.config: dict[str, Any] = utils.read_config(config_file)
 
         # store forcing & obs
         self.P = utils.load_var(self.config["precipitation_file"], "pr")
 
-        self.EP = utils.load_var(self.config["potential_evaporation_file"], "pev")
+        self.EP = utils.load_var(self.config["potential_evaporation_file"], "evspsblpot")
 
-        self.Tmean = utils.load_var(self.config["mean_temperature_file"], "tasmean")
+        self.Tmean = utils.load_var(self.config["mean_temperature_file"], "tas")
 
         # set up times
         self.time = self.P['time'].astype("datetime64[s]")
         self.end_timestep = len(self.time.values)
         self.current_timestep = 0
 
         # time step size in seconds (to be able to do unit conversions) - change here to days
```

### Comparing `hbv-1.4.1/src/HBV/utils.py` & `hbv-1.5.0/src/HBV/utils.py`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/LICENSE.txt` & `hbv-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hbv-1.4.1/pyproject.toml` & `hbv-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "HBV"
 description = "Dev version for a HBV hydrological model using BMI for eWaterCycle."
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.4.1"
+version = "1.5.0"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 
 # Include here only the dependencies for the BMI Model
 # This is used to run the BmiModel inside the container
 dependencies = [
```

### Comparing `hbv-1.4.1/PKG-INFO` & `hbv-1.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: HBV
-Version: 1.4.1
+Version: 1.5.0
 Summary: Dev version for a HBV hydrological model using BMI for eWaterCycle.
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Requires-Dist: bmipy
 Requires-Dist: netcdf4
 Requires-Dist: numpy
@@ -16,14 +16,16 @@
 
 [![PyPI](https://img.shields.io/pypi/v/HBV)](https://pypi.org/project/HBV/)
 
 Basic Model Interface (BMI) HBV model intended for use with [eWaterCycle](https://github.com/eWaterCycle). See said repo for installation instructions. 
 
 HBV (Hydrologiska Byråns Vattenbalansavdelning) is a conceptual hydrological model. For more information on its history, see this [paper](https://hess.copernicus.org/articles/26/1371/2022/).
 
+_TODO: update to match snow reservoir_
+
 This current implementation is _without_ a snow reservoir, as shown below.
 (_Image from the course ENVM1502 - river basin Hydrology (Markus Hrachowitz)._) 
 ![model_layout.png](https://raw.githubusercontent.com/Daafip/HBV-bmi/main/docs/model_layout.png)
 
 Actual eWatercycle model wrapper can be found on [GitHub](https://github.com/Daafip/ewatercycle-hbv) with accompanying [documentation](https://ewatercycle-hbv.readthedocs.io/en/latest/)
 
 Feel free to fork/duplicate this repo and publish your own (better) version.
@@ -38,37 +40,15 @@
 
 Then HBV becomes available as one of the eWaterCycle models
 
 ```python
 from HBV import HBV
 
 model = HBV()
-
 ```
 
 Be aware of the non-intuitive [BMI](https://github.com/eWaterCycle/grpc4bmi) implementation as this package is designed to run in a [docker](https://github.com/Daafip/HBV-bmi/pkgs/container/hbv-bmi-grpc4bmi) container. 
 
 
 ## Changelog
 
-### v1.0.0 
-- working basic version after various [testing versions](https://test.pypi.org/project/HBV/)
-#### v1.0.1 - v1.0.3 
-- various bug fixes etc. (last time using live as a dev branch -> bad practice)
-### v1.1.0 
-- added support for updating memory vector on the fly for Data assimilation.
-#### V1.1.1
-- bug fix in `T_lag` value: can now only be set an integer larger than 1: otherwise makes no physical sense
-- bug fix where wrong types were given, warning messages cleaned up and code attempted to be made more readable
-### V1.2.0
-- pretty big issue with setting values fixed - won't affect most use but will cause issues for Data Assimilation
-- use opportunity to name all HBV packages/naming/images to 1.2.0 
-## V1.3.0
-- Change `Q_m` to `Q` in order to better integrate data assimilation & just makes more sense. 
-### v1.3.1
-- Fix bug in time indexing
-### v1.3.2
-- typo in update updating_dict_var_obj: was getting values wrong 
-## V1.4.0
-- adding snow reservoir
-### V1.4.1
-- bug fix in naming of values 
+See [CHANGELOG.md](https://github.com/Daafip/HBV-bmi/blob/main/CHANGELOD.md).
```

