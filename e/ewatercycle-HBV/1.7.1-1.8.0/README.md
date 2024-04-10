# Comparing `tmp/ewatercycle_hbv-1.7.1.tar.gz` & `tmp/ewatercycle_hbv-1.8.0.tar.gz`

## Comparing `ewatercycle_hbv-1.7.1.tar` & `ewatercycle_hbv-1.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/plugin_guide.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.idea/.gitignore
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.idea/ewatercycle-hbv-numpy.iml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/conf.py
--rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/example_model_run_HBV.ipynb
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/make.bat
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/model.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/requirements.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/_images/model_layout.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/docs/_static/README.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/src/ewatercycle_HBV/__init__.py
--rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/src/ewatercycle_HBV/forcing.py
--rw-r--r--   0        0        0     9721 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/src/ewatercycle_HBV/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/tests/test_forcing.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/tests/test_model.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/LICENSE.txt
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/plugin_guide.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/.gitignore
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/ewatercycle-hbv-numpy.iml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/Makefile
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/conf.py
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/example_model_run_HBV.ipynb
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/make.bat
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/model.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/requirements.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/_images/model_layout.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/_static/README.rst
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/__init__.py
+-rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/forcing.py
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/tests/test_forcing.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/tests/test_model.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/PKG-INFO
```

### Comparing `ewatercycle_hbv-1.7.1/.readthedocs.yaml` & `ewatercycle_hbv-1.8.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/CHANGELOG.md` & `ewatercycle_hbv-1.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,8 +35,10 @@
 ### 1.6.0
   - now compatible with ewatercycle V2.1 `LumpedMakkinkForcing` which generates evaporation from era5/CMIP.
 #### 1.6.1
   - bug fix occuring when loading makkink data
 ### 1.7.0
   - new version of HBV bmi which adds snow 
 ### 1.7.1
-  - bug fix with definitions of state variable names
+  - bug fix with definitions of state variable names
+### 1.8.0
+- Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
```

### Comparing `ewatercycle_hbv-1.7.1/plugin_guide.md` & `ewatercycle_hbv-1.8.0/plugin_guide.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/.github/workflows/python-publish.yml` & `ewatercycle_hbv-1.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/.github/workflows/test.yml` & `ewatercycle_hbv-1.8.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/Makefile` & `ewatercycle_hbv-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/conf.py` & `ewatercycle_hbv-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/example_model_run_HBV.ipynb` & `ewatercycle_hbv-1.8.0/docs/example_model_run_HBV.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/index.rst` & `ewatercycle_hbv-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/make.bat` & `ewatercycle_hbv-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/model.rst` & `ewatercycle_hbv-1.8.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/_images/model_layout.png` & `ewatercycle_hbv-1.8.0/docs/_images/model_layout.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/docs/_static/README.rst` & `ewatercycle_hbv-1.8.0/docs/_static/README.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/src/ewatercycle_HBV/forcing.py` & `ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/forcing.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 import xarray as xr
 import numpy as np
 
 from ewatercycle.base.forcing import DefaultForcing
 
 
 RENAME_CAMELS = {'total_precipitation_sum':'pr',
-                 'potential_evaporation_sum':'pev',
+                 'potential_evaporation_sum':'evspsblpot',
                  'streamflow':'Q',
                  'temperature_2m_min':'tasmin',
                  'temperature_2m_max':'tasmax',
                  }
 
-REQUIRED_PARAMS = ["pr", "pev", "tasmean"]
+REQUIRED_PARAMS = ["pr", "evspsblpot", "tas"]
 class HBVForcing(DefaultForcing):
     """Container for HBV forcing data.
 
     Args:
         camels_file: .txt file that contains CAMELS forcing from https://hess.copernicus.org/articles/21/5293/2017/
         pr: Path to a NetCDF (.nc) file containing precipitation - ensure yourself that these already match start_time & end time
-        pev: Path to a NetCDF (.nc) file containing potential evaporation
+        evspsblpot: Path to a NetCDF (.nc) file containing potential evaporation
         alpha: float provided in camels dataset but not in the forcing file, instead in the model results.
-        test_data_bool: False by default, set True if instead of a camels file, a test files is passed for HBV including precipitation and evaporation contains columns: ["year", "month", "day", "pr", "pev"] seperated by a space
+        test_data_bool: False by default, set True if instead of a camels file, a test files is passed for HBV including precipitation and evaporation contains columns: ["year", "month", "day", "pr", "evspsblpot"] seperated by a space
 
     Examples:
 
         From existing forcing data:
 
         .. code-block:: python
 
@@ -51,88 +51,88 @@
         .. code-block:: python
 
             forcing = sources.HBVForcing(
                 directory='/home/davidhaasnoot/Code/Forcing/',
                 start_time='1997-08-01T00:00:00Z',
                 end_time='2000-08-31T00:00:00Z',
                 pr="precipitation_file.nc"
-                pev="potential_evaporation_file.nc"
+                evspsblpot="potential_evaporation_file.nc"
             )
 
         where :py:const:`precipitation_file` &  :py:const:`potential_evaporation_file` can be the same aslong as
-        they contain a  :py:const:`pr` &  :py:const:`pev` variable
+        they contain a  :py:const:`pr` &  :py:const:`evspsblpot` variable
 
         Inherited from base forcing:
             shape: Path to a shape file. Used for spatial selection.
             directory: Directory where forcing data files are stored.
             start_time: Start time of forcing in UTC and ISO format string e.g 'YYYY-MM-DDTHH:MM:SSZ'.
             end_time: End time of forcing in UTC and ISO format string e.g. 'YYYY-MM-DDTHH:MM:SSZ'.
 
     """
 
     # either a forcing file is supplied
     camels_file: Optional[str] = ".txt"
-    # or pr and pev are supplied seperately - can also be the same dataset
+    # or pr and evspsblpot are supplied seperately - can also be the same dataset
     pr: Optional[str] = ".nc"
-    pev: Optional[str] = ".nc"
-    tasmean: Optional[str] = ".nc"
+    evspsblpot: Optional[str] = ".nc"
+    tas: Optional[str] = ".nc"
     alpha: Optional[float] = 1.26 # varies per catchment, mostly 1.26?
     test_data_bool: bool = False # allows to use self.from_test_txt()
 
     def camels_txt_defined(self):
         """test whether user defined forcing file, used converting text forcing file to netcdf"""
         if len(self.camels_file) > 4:
             return True
         else:
             return False
 
     def forcing_nc_defined(self):
         """test whether user defined forcing file"""
-        if (len(self.pr) > 3) and (len(self.pev) > 3):
+        if (len(self.pr) > 3) and (len(self.evspsblpot) > 3):
             return True
         else:
             return False
 
     def from_test_txt(self) -> xr.Dataset:
         """Load forcing data from a txt file into an xarray dataset.
 
         Information:
-            Must contain ["year", "month", "day", "pr","Q", "pev"] in columns
+            Must contain ["year", "month", "day", "pr","Q", "evspsblpot"] in columns
 
             Will convert date to pandas.Timestamp()
 
-            pr (precipitation), Q (discharge), pev (potential evaportaion) - all im mm's
+            pr (precipitation), Q (discharge), evspsblpot (potential evaportaion) - all im mm's
 
         Returns:
             ds: xr.Dataset
                 Dataset with forcing data.
         """
         if self.directory is None or self.camels_file is None:
             self.file_not_found_error()
         fn = self.directory / self.camels_file
         forcing = np.loadtxt(fn, delimiter="	")
-        names = ["year", "month", "day", "pr","Q", "pev"]
+        names = ["year", "month", "day", "pr","Q", "evspsblpot"]
         df_in = pd.DataFrame(forcing, columns=names)
         df_in.index = df_in.apply(lambda x: pd.Timestamp(f'{int(x.year)}-{int(x.month)}-{int(x.day)}'), axis=1)
         df_in = df_in.drop(columns=["year", "month", "day"])
         df_in.index.name = "time"
         # test data has no snow but let's add in synthetic temperatures to ensure there's no snow:
-        df_in['tasmean'] = 25
+        df_in['tas'] = 25
 
         # TODO use netcdf-cf conventions
         ds = xr.Dataset(data_vars=df_in,
                         attrs={
                             "title": "HBV forcing data",
                             "history": "Created by ewatercycle_HBV.forcing.HBVForcing.to_xarray()",
                                 },
                         )
         ds, ds_name = self.crop_ds(ds, "test")
-        self.pev = ds_name
+        self.evspsblpot = ds_name
         self.pr = ds_name
-        self.tasmean = ds_name
+        self.tas = ds_name
 
         return ds
 
     def from_camels_txt(self) -> xr.Dataset:
         """Load forcing data from a txt file into an xarray dataset.
 
         Requirements:
@@ -198,70 +198,70 @@
         # add the data lines with catchment characteristics to the description
         attrs.update(data)
 
         ds = xr.Dataset(data_vars=df,
                         attrs=attrs,
                         )
         # Potential Evaporation conversion using srad & tasmin/maxs
-        ds['pev'] = calc_pet(ds['srad'],
+        ds['evspsblpot'] = calc_pet(ds['srad'],
                              ds["tasmin"].values,
                              ds["tasmax"].values,
                              ds["time.dayofyear"].values,
                              self.alpha,
                              ds.attrs['elevation(m)'],
                              ds.attrs['lat']
                              )
-        ds['tasmean'] = (ds["tasmin"] + ds["tasmax"]) / 2
+        ds['tas'] = (ds["tasmin"] + ds["tasmax"]) / 2
         ds, ds_name= self.crop_ds(ds, "CAMELS")
-        self.pev = ds_name
+        self.evspsblpot = ds_name
         self.pr = ds_name
-        self.tasmean = ds_name
+        self.tas = ds_name
         return ds
 
     def from_external_source(self):
         """Runs checks on externally provided forcing"""
-        if None in [self.directory, self.pr, self.pev]:
+        if None in [self.directory, self.pr, self.evspsblpot]:
             self.file_not_found_error()
 
         # often same file
-        if self.pr == self.pev == self.tasmean:
+        if self.pr == self.evspsblpot == self.tas:
             ds = xr.open_dataset(self.directory / self.pr)
 
             # make compatile with CARAVAN data style:
             if sum([key in ds.data_vars for key in RENAME_CAMELS.keys()]) == len(RENAME_CAMELS):
                 ds = ds.rename(RENAME_CAMELS)
                 ds = ds.rename_dims({'date': 'time'})
                 ds = ds.rename({'date': 'time'})
-                ds['tasmean'] = (ds["tasmin"] + ds["tasmax"]) / 2
+                ds['tas'] = (ds["tasmin"] + ds["tasmax"]) / 2
 
             ds, ds_name = self.crop_ds(ds, "external")
-            self.pev = ds_name
+            self.evspsblpot = ds_name
             self.pr = ds_name
-            self.tasmean = ds_name
+            self.tas = ds_name
             return ds
 
         else:
             # but can also seperate
             ds_pr = xr.open_dataset(self.directory / self.pr)
-            ds_pev = xr.open_dataset(self.directory / self.pev)
-            ds_tasmean = xr.open_dataset(self.directory / self.tasmean)
-            combined_data_vars = list(ds_pr.data_vars) + list(ds_pev.data_vars) + list(ds_tasmean.data_vars)
+            ds_evspsblpot = xr.open_dataset(self.directory / self.evspsblpot)
+            ds_tas = xr.open_dataset(self.directory / self.tas)
+            combined_data_vars = list(ds_pr.data_vars) + list(ds_evspsblpot.data_vars) + list(ds_tas.data_vars)
             if sum([param in combined_data_vars for param in REQUIRED_PARAMS]) != len(REQUIRED_PARAMS):
                 raise UserWarning(f"Supplied NetCDF files must contain {REQUIRED_PARAMS} respectively")
 
             ds_pr, ds_name_pr = self.crop_ds(ds_pr, "external")
             self.pr = ds_name_pr
 
-            ds_pev, ds_name_pev = self.crop_ds(ds_pev, "external")
-            self.pev = ds_name_pev
+            ds_evspsblpot, ds_name_evspsblpot = self.crop_ds(ds_evspsblpot, "external")
+            self.evspsblpot = ds_name_evspsblpot
 
-            ds_tasmean, ds_name_tasmean = self.crop_ds(ds_tasmean, "external")
-            self.tasmean = ds_name_tasmean
+            ds_tas, ds_name_tas = self.crop_ds(ds_tas, "external")
+            self.tas = ds_name_tas
 
-            return ds_pr, ds_pev, ds_tasmean
+            return ds_pr, ds_evspsblpot, ds_tas
 
     def crop_ds(self, ds: xr.Dataset, name: str):
         start = np.datetime64(self.start_time)
         end = np.datetime64(self.end_time)
         ds = ds.isel(time=(ds['time'].values >= start) & (ds['time'].values <= end))
 
         time = str(datetime.now())[:-10].replace(":", "_")
@@ -270,15 +270,15 @@
         out_dir = self.directory / ds_name
         if not out_dir.exists():
             ds.to_netcdf(out_dir)
 
         return ds, ds_name
 
     def file_not_found_error(self):
-        raise ValueError("Directory, camels_file or pr & pev values is not set correctly")
+        raise ValueError("Directory, camels_file or pr & evspsblpot values is not set correctly")
 
 def calc_pet(s_rad, t_min, t_max, doy, alpha, elev, lat) -> np.ndarray:
     """Calculates Potential Evaporation using Priestly–Taylor PET estimate, callibrated with longterm P-T trends from the camels data set (alpha).
 
     Parameters:
         s_rad: np.ndarray
             net radiation estimate in W/m^2. Function converts this to J/m^2/d
@@ -302,17 +302,19 @@
         pet: np.ndarray
             Array containing PET estimates in mm/day
 
     Reference:
         based on code from:
                 kratzert et al. 2022
                 `NeuralHydrology --- A Python library for Deep Learning research in hydrology,
-                Frederik Kratzert and Martin Gauch and Grey Nearing and Daniel Klotz <https://github.com/neuralhydrology/neuralhydrology/blob/master/neuralhydrology/datautils/pet.py>`_
+                Frederik Kratzert and Martin Gauch and Grey Nearing and Daniel Klotz
+                <https://github.com/neuralhydrology/neuralhydrology/blob/master/neuralhydrology/datautils/pet.py>`_
                 https://doi.org/10.21105/joss.04050
-        Who base on `allen et al. (1998) 'FOA 56' <https://appgeodb.nancy.inra.fr/biljou/pdf/Allen_FAO1998.pdf>`_ & `Newman et al (2015) <https://hess.copernicus.org/articles/21/5293/2017/>`_
+        Who base on `allen et al. (1998) 'FOA 56' <https://appgeodb.nancy.inra.fr/biljou/pdf/Allen_FAO1998.pdf>`_ &
+        `Newman et al (2015) <https://hess.copernicus.org/articles/21/5293/2017/>`_
 
     """
     G = 0
     LAMBDA = 2.45  # MJ/kg
 
     s_rad = s_rad * 0.0864  # conversion Wm-2 -> MJm-2day-1
     albedo = 0.23  # planetary albedo
```

### Comparing `ewatercycle_hbv-1.7.1/src/ewatercycle_HBV/model.py` & `ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,78 +65,86 @@
                 raise UserWarning("Ensure either a txt file with camels data or an(/set of) xarrays is defined")
 
             self._config["precipitation_file"] = str(
                 self.forcing.directory / self.forcing.pr
             )
 
             self._config["potential_evaporation_file"] = str(
-                self.forcing.directory / self.forcing.pev
+                self.forcing.directory / self.forcing.evspsblpot
             )
             self._config["mean_temperature_file"] = str(
-                self.forcing.directory / self.forcing.tasmean)
+                self.forcing.directory / self.forcing.tas)
 
+        elif type(self.forcing).__name__ == 'LumpedCaravanForcing':
+            self._config["precipitation_file"] = str(
+                self.forcing.directory / self.forcing['pr']
+            )
+
+            self._config["potential_evaporation_file"] = str(
+                self.forcing.directory / self.forcing['evspsblpot']
+            )
+
+            self._config["mean_temperature_file"] = str(
+                self.forcing.directory / self.forcing['tas']
+            )
 
         elif type(self.forcing).__name__ == 'GenericLumpedForcing':
-                raise UserWarning("Generic Lumped Forcing does not provide potential evaporation, which this model needs")
+                msg = "Generic Lumped Forcing does not provide potential evaporation, which this model needs"
+                raise UserWarning(msg)
 
         elif type(self.forcing).__name__ == 'LumpedMakkinkForcing':
-            temporary_pev_file = self.forcing.directory / self.forcing.filenames['evspsblpot'].replace('evspsblpot',
-                                                                                                       'pev_mm')
-            if not temporary_pev_file.is_file():
-                ds = xr.open_dataset(self.forcing.directory / self.forcing.filenames['evspsblpot'])
-                attributes = ds['evspsblpot'].attrs
-                attributes['units'] = 'mm'
-                ds = ds.rename({'evspsblpot': 'pev'})
-                ds['pev'] = ds['pev'] * 86400
-                ds['pev'].attrs = attributes
-                ds.to_netcdf(temporary_pev_file)
+            temporary_evspsblpot_file = (self.forcing.directory /
+                                         self.forcing.filenames['evspsblpot'].replace('evspsblpot',
+                                                                                  'evspsblpot_mm'))
+            if not temporary_evspsblpot_file.is_file():
+                ds = xr.open_dataset(self.forcing.directory /
+                                     self.forcing.filenames['evspsblpot'])
+                ds['evspsblpot'].attrs.update({'units':'mm'})
+                ds['evspsblpot'] = ds['evspsblpot'] * 86400
+                ds.to_netcdf(temporary_evspsblpot_file)
                 ds.close()
 
-            temporary_pr_file = self.forcing.directory / self.forcing.filenames['pr'].replace('pr', 'pr_mm')
+            temporary_pr_file = (self.forcing.directory /
+                                 self.forcing.filenames['pr'].replace('pr', 'pr_mm'))
             if not temporary_pr_file.is_file():
                 ds = xr.open_dataset(self.forcing.directory / self.forcing.filenames['pr'])
-                attributes = ds['pr'].attrs
-                attributes['units'] = 'mm'
+                ds['pr'].attrs.attrs.update({'units':'mm'})
                 ds['pr'] = ds['pr'] * 86400
-                ds['pr'].attrs = attributes
                 ds.to_netcdf(temporary_pr_file)
                 ds.close()
 
-            temporary_tasmean_file = self.forcing.directory / self.forcing.filenames['tas'].replace('tas', 'tasmean')
-            if not temporary_tasmean_file.is_file():
+            temporary_tas_file = (self.forcing.directory /
+                                  self.forcing.filenames['tas'].replace('tas', 'tas_deg'))
+            if not temporary_tas_file.is_file():
                 ds = xr.open_dataset(self.forcing.directory / self.forcing.filenames['tas'])
-                attributes = ds['tas'].attrs
-                ds['tasmean'] = ds['tas']
-                if ds['tasmean'].mean().values > 200: # adjust for kelvin units
-                    ds['tasmean'] -= 273.15
-                    attributes.update({'units':'degC'})
-                ds['tasmean'].attrs = attributes
-                ds.to_netcdf(temporary_tasmean_file)
+                if ds['tas'].mean().values > 200: # adjust for kelvin units
+                    ds['tas'] -= 273.15
+                    ds['tas'].attrs.update({'units':'degC'})
+                ds.to_netcdf(temporary_tas_file)
                 ds.close()
 
             self._config["precipitation_file"] = str(
                 temporary_pr_file
             )
             self._config["potential_evaporation_file"] = str(
-                temporary_pev_file
+                temporary_evspsblpot_file
             )
 
             self._config["mean_temperature_file"] = str(
-                temporary_tasmean_file
+                temporary_tas_file
             )
 
         for kwarg in kwargs:  # Write any kwargs to the config. - doesn't overwrite config?
             self._config[kwarg] = kwargs[kwarg]
 
         config_file = self._cfg_dir / "HBV_config.json"
 
         with config_file.open(mode="w") as f:
             f.write(json.dumps(self._config, indent=4))
 
-
         return config_file
 
     @property
     def parameters(self) -> ItemsView[str, Any]:
         """List the (initial!) parameters for this model.
 
         Exposed HBV parameters:
@@ -194,17 +202,17 @@
         ADDED: Remove created config files, especially useful for DA models
         """
 
         # remove bmi
         self._bmi.finalize()
         del self._bmi
 
+        config_file = self._cfg_dir / "HBV_config.json"
         try:
             # remove config file
-            config_file = self._cfg_dir / "HBV_config.json"
             config_file.unlink()
         except FileNotFoundError:
             warnings.warn(message=f'Config not found at {config_file}, removed by user?',category=UserWarning)
 
         try:
             # once empty, remove it
             self._cfg_dir.rmdir()
@@ -227,9 +235,9 @@
                 path.unlink()
             else:
                 pass
 
 class HBV(ContainerizedModel, HBVMethods):
     """The HBV eWaterCycle model, with the Container Registry docker image."""
     bmi_image: ContainerImage = ContainerImage(
-        "ghcr.io/daafip/hbv-bmi-grpc4bmi:v1.4.1"
+        "ghcr.io/daafip/hbv-bmi-grpc4bmi:v1.5.0"
     )
```

### Comparing `ewatercycle_hbv-1.7.1/.gitignore` & `ewatercycle_hbv-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/LICENSE.txt` & `ewatercycle_hbv-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/README.md` & `ewatercycle_hbv-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.7.1/pyproject.toml` & `ewatercycle_hbv-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = "src/ewatercycle_HBV/__init__.py"
 
 [project]
 name = "ewatercycle-HBV"
 description = "Implementation of HBV for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.7.1"
+version = "1.8.0"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `ewatercycle_hbv-1.7.1/PKG-INFO` & `ewatercycle_hbv-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ewatercycle-HBV
-Version: 1.7.1
+Version: 1.8.0
 Summary: Implementation of HBV for eWaterCycle
 Project-URL: homepage, https://github.com/Daafip/ewatercycle-hbv
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: ewatercycle,hydrology
 Classifier: Intended Audience :: Developers
```

