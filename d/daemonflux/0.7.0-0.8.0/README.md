# Comparing `tmp/daemonflux-0.7.0.tar.gz` & `tmp/daemonflux-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daemonflux-0.7.0.tar", last modified: Thu Jun  1 12:50:51 2023, max compression
+gzip compressed data, was "daemonflux-0.8.0.tar", last modified: Wed Apr 10 13:35:29 2024, max compression
```

## Comparing `daemonflux-0.7.0.tar` & `daemonflux-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-01 12:50:26.000000 daemonflux-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 12:50:51.821183 daemonflux-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-01 12:50:26.000000 daemonflux-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-01 12:50:26.000000 daemonflux-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 12:50:51.821183 daemonflux-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.817183 daemonflux-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/src/daemonflux/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 12:50:26.000000 daemonflux-0.7.0/src/daemonflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26884 2023-06-01 12:50:26.000000 daemonflux-0.7.0/src/daemonflux/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-01 12:50:26.000000 daemonflux-0.7.0/src/daemonflux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/src/daemonflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-01 12:50:26.000000 daemonflux-0.7.0/tests/test_daemonflux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 13:35:09.000000 daemonflux-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-10 13:35:29.227994 daemonflux-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-10 13:35:09.000000 daemonflux-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 13:35:09.000000 daemonflux-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-10 13:35:29.227994 daemonflux-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/src/daemonflux/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 13:35:09.000000 daemonflux-0.8.0/src/daemonflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28411 2024-04-10 13:35:09.000000 daemonflux-0.8.0/src/daemonflux/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-10 13:35:09.000000 daemonflux-0.8.0/src/daemonflux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/src/daemonflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-04-10 13:35:09.000000 daemonflux-0.8.0/tests/test_daemonflux.py
```

### Comparing `daemonflux-0.7.0/LICENSE` & `daemonflux-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daemonflux-0.7.0/PKG-INFO` & `daemonflux-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.7.0
+Version: 0.8.0
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy>=1.8.0
+Requires-Dist: rich
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: examples
-License-File: LICENSE
+Requires-Dist: matplotlib; extra == "examples"
 
 # daemonflux: DAta-drivEn and MuOn-calibrated Neutrino flux
 
 Daemonflux is a tabulated/splined version of the an atmospheric flux model calibrated on muon spectrometer data. For the details about how daemonflux is built and calibrated to muon data [the following publication](https://inspirehep.net/literature/2637710).
 
 ```
 @article{Yanez:2023lsy,
@@ -88,10 +93,14 @@
 - muon neutrinos: `numuflux`, `numuratio`, `numu`, `antinumu`, `flavorratio`
 - electron neutrinos: `nueflux`, `nueratio`, `nue`, `antinue`, `flavorratio`
 
 Those titled XXXflux are the sum of particle and antiparticle fluxes `numuflux = numu + antinumu`, the ratio is `numuratio = numu/antinumu`, and the is defined as `flavorratio = (numu + antinumu)/(nue + antinue)`.
 
 The `total_` quantities, such as `total_muflux`, represent the total flux, which includes both conventional and prompt atmospheric fluxes. However, unlike the conventional flux, the prompt flux is not calibrated using the daemonflux method, as surface muons are not sensitive to prompt fluxes. As a result, the prompt component does not include correction parameters or errors. It is important to note, however, that the conventional part of the flux remains calibrated, so the total_ flux is simply the sum of the calibrated conventional and uncalibrated prompt fluxes.
 
+## Using parameter correlations represented by the covariance matrix
+
+The parameters of the model are correlated. These correlations are drdetermined from the data we have used for the fit. The errors are already computed taking the covariance matrix into account when using the `error` method. If daemonflux is used in a fit with free floating parameters, one can include these correlations by adding the chi2 as additional penalty term. The chi2 for the current combination of parameters can be obtained by calling `flux.chi2({dictionary of modified parameters})`.
+
 ## LICENSE
 
 [BSD 3-Clause License](LICENSE)
```

### Comparing `daemonflux-0.7.0/README.md` & `daemonflux-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -63,10 +63,14 @@
 - muon neutrinos: `numuflux`, `numuratio`, `numu`, `antinumu`, `flavorratio`
 - electron neutrinos: `nueflux`, `nueratio`, `nue`, `antinue`, `flavorratio`
 
 Those titled XXXflux are the sum of particle and antiparticle fluxes `numuflux = numu + antinumu`, the ratio is `numuratio = numu/antinumu`, and the is defined as `flavorratio = (numu + antinumu)/(nue + antinue)`.
 
 The `total_` quantities, such as `total_muflux`, represent the total flux, which includes both conventional and prompt atmospheric fluxes. However, unlike the conventional flux, the prompt flux is not calibrated using the daemonflux method, as surface muons are not sensitive to prompt fluxes. As a result, the prompt component does not include correction parameters or errors. It is important to note, however, that the conventional part of the flux remains calibrated, so the total_ flux is simply the sum of the calibrated conventional and uncalibrated prompt fluxes.
 
+## Using parameter correlations represented by the covariance matrix
+
+The parameters of the model are correlated. These correlations are drdetermined from the data we have used for the fit. The errors are already computed taking the covariance matrix into account when using the `error` method. If daemonflux is used in a fit with free floating parameters, one can include these correlations by adding the chi2 as additional penalty term. The chi2 for the current combination of parameters can be obtained by calling `flux.chi2({dictionary of modified parameters})`.
+
 ## LICENSE
 
 [BSD 3-Clause License](LICENSE)
```

### Comparing `daemonflux-0.7.0/setup.cfg` & `daemonflux-0.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = daemonflux
-version = 0.7.0
+version = 0.8.0
 author = Anatoli Fedynitch
 maintainer_email = afedynitch@gmail.com
 description = Tabulated representation of a muon-calibrated muon and neutrino flux model
 license = BSD 3-Clause License
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mceq-project/daemonflux
```

### Comparing `daemonflux-0.7.0/src/daemonflux/__init__.py` & `daemonflux-0.8.0/src/daemonflux/__init__.py`

 * *Files identical despite different names*

### Comparing `daemonflux-0.7.0/src/daemonflux/flux.py` & `daemonflux-0.8.0/src/daemonflux/flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         Covariance matrix of parameters.
     """
 
     def __init__(
         self, known_parameters: List[str], values: np.ndarray, cov: np.ndarray
     ):
         self.known_parameters = known_parameters
+        self._n_non_gsf = len([p for p in known_parameters if "GSF" not in p])
         self.values = values
+        self._unmodified_values = np.copy(values)
         self.cov = cov
 
     @property
     def invcov(self) -> np.ndarray:
         """Inverse of the covariance matrix of parameters.
 
         Returns
@@ -67,15 +69,15 @@
             Dictionary of modified parameters
 
         Returns
         -------
         numpy.ndarray
             Chi-square value associated with params
         """
-        return np.sum(grid_cov(self.values, self.invcov))
+        return np.sum(grid_cov(self.values - self._unmodified_values, self.invcov))
 
     def __iter__(self) -> Generator[Tuple[str, float], None, None]:
         """Iterate over the parameters.
 
         Yields
         ------
         str
@@ -103,23 +105,24 @@
     """
 
     _default_url = (
         "https://github.com/mceq-project/daemonflux/releases/download/prerelease/"
     )
     _default_spl_file = "daemonsplines_{location}_{rev}.pkl"
     _default_cal_file = "daemonsplines_calibration_{cset}_{rev}.pkl"
-    _revision = "202303_1"
+    _revision = "202303_2"
 
     def __init__(
         self,
         location="generic",
         spl_file=None,
         cal_file=None,
         calibration_set="default",
         use_calibration=True,
+        uncorrelated_hadr_errors=False,
         exclude=[],
         keep_old_revisions=False,
         debug=1,
     ) -> None:
         """
         Initialize the Flux instance.
 
@@ -129,25 +132,33 @@
             Location to be used, default is "generic".
         spl_file : str, optional
             Path to the spline file.
         cal_file : str, optional
             Path to the calibration file.
         use_calibration : bool, optional
             Flag indicating whether to use calibration, default is True.
+        uncorrelated_hadr_errors: bool, optional
+            Flag indicating whether to use uncorrelated hadronic errors
+            (during calibration), default is False.
         calibration_set : str, optional
             Calibration set to be used. Default is "default". Optional is "with_deis".
         exclude : list, optional
             A list of parameters to be excluded, default is an empty list.
         keep_old_revisions : bool, optional
             Flag indicating whether to keep old spline file revisions, default is False.
         debug : int, optional
             Debug level, default is 1.
         """
         self.exclude = exclude
         self._debug = debug
+        self._uncorrelated_hadr_errors = uncorrelated_hadr_errors
+
+        # Define location or spl_file
+        assert location or spl_file, "Either location or spl_file must be defined."
+
         spl_file = (
             spl_file
             if spl_file
             else _cached_data_dir(
                 self._default_url
                 + self._default_spl_file.format(location=location, rev=self._revision)
             )
@@ -207,15 +218,14 @@
                 continue
             if k.startswith("total_"):
                 continue
             known_parameters.append(k)
 
         if cal_file is None:
             print("No calibration used.")
-
             params = Parameters(
                 known_parameters,
                 np.zeros(len(known_parameters)),
                 cov,
             )
             assert params.cov.shape == (len(known_parameters),) * 2, (
                 f"covariance shape {params.cov.shape} is not consistent"
@@ -270,14 +280,19 @@
                         + " "
                         + str(pj)
                         + " incorrectly sorted."
                     )
 
             params = Parameters(known_parameters, np.asarray(param_values), cov)
 
+        if self._uncorrelated_hadr_errors:
+            params.cov[: params._n_non_gsf, : params._n_non_gsf] = np.diag(
+                np.ones(params._n_non_gsf)
+            )
+
         # If multiple locations inside the spline file, create a FluxEntry for each
         self.supported_fluxes = []
         for exp in self._fl_spl:
             subflux = _FluxEntry(
                 exp,
                 self._fl_spl[exp],
                 self._jac_spl[exp],
@@ -427,14 +442,30 @@
         return self._get_flux_instance(exp).error(
             grid,
             zenith_deg,
             quantity,
             only_hadronic,
         )
 
+    def chi2(self, params={}, exp=""):
+        """
+        Returns the chi-square value of the parameters.
+
+        Parameters
+        ----------
+        params: dict
+            Dictionary of modified parameters
+
+        Returns
+        -------
+        float
+            Chi-square value associated with params
+        """
+        return self._get_flux_instance(exp).chi2(params)
+
     def __getitem__(self, exp_label):
         if exp_label not in self.supported_fluxes:
             raise KeyError("Supported fluxes are", self.supported_fluxes)
         return self.__getattribute__(exp_label)
 
 
 class _FluxEntry(Flux):
@@ -796,7 +827,24 @@
         # handle the case where the zenith angle is a single value or an array
         if not is_iterable(zenith_deg) and float(zenith_deg) in self._zenith_deg_arr:
             return self._error_from_spl(
                 grid, format_angle(zenith_deg), quantity, only_hadronic
             )
         else:
             return self._error_from_interp(grid, zenith_deg, quantity, only_hadronic)
+
+    def chi2(self, params={}):
+        """
+        Returns the chi-square value of the parameters.
+
+        Parameters
+        ----------
+        params: dict
+            Dictionary of modified parameters
+
+        Returns
+        -------
+        numpy.ndarray
+            Chi-square value associated with params
+        """
+        with self._temporary_parameters(params):
+            return self._params.chi2
```

### Comparing `daemonflux-0.7.0/src/daemonflux/utils.py` & `daemonflux-0.8.0/src/daemonflux/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,31 +38,31 @@
     -------
     str
         The formatted angle as a string.
     """
     return "{:4.4f}".format(float(ang))
 
 
-def grid_cov(jac: np.ndarray, cov: np.ndarray) -> np.ndarray:
+def grid_cov(jac: np.ndarray, invcov: np.ndarray) -> np.ndarray:
     """
-    Calculate the covariance of the grid.
+    Chi2 matrix expression.
 
     Parameters
     ----------
     jac : np.ndarray
         The Jacobian matrix.
-    cov : np.ndarray
-        The covariance matrix.
+    invcov : np.ndarray
+        The inverse of the covariance matrix.
 
     Returns
     -------
     np.ndarray
-        The covariance of the grid.
+
     """
-    return np.dot(jac, np.dot(cov, jac.T))
+    return np.dot(jac, np.dot(invcov, jac.T))
 
 
 def is_iterable(arg) -> bool:
     """
     Check if an argument is iterable.
 
     Parameters
```

### Comparing `daemonflux-0.7.0/src/daemonflux.egg-info/PKG-INFO` & `daemonflux-0.8.0/src/daemonflux.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.7.0
+Version: 0.8.0
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy>=1.8.0
+Requires-Dist: rich
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: examples
-License-File: LICENSE
+Requires-Dist: matplotlib; extra == "examples"
 
 # daemonflux: DAta-drivEn and MuOn-calibrated Neutrino flux
 
 Daemonflux is a tabulated/splined version of the an atmospheric flux model calibrated on muon spectrometer data. For the details about how daemonflux is built and calibrated to muon data [the following publication](https://inspirehep.net/literature/2637710).
 
 ```
 @article{Yanez:2023lsy,
@@ -88,10 +93,14 @@
 - muon neutrinos: `numuflux`, `numuratio`, `numu`, `antinumu`, `flavorratio`
 - electron neutrinos: `nueflux`, `nueratio`, `nue`, `antinue`, `flavorratio`
 
 Those titled XXXflux are the sum of particle and antiparticle fluxes `numuflux = numu + antinumu`, the ratio is `numuratio = numu/antinumu`, and the is defined as `flavorratio = (numu + antinumu)/(nue + antinue)`.
 
 The `total_` quantities, such as `total_muflux`, represent the total flux, which includes both conventional and prompt atmospheric fluxes. However, unlike the conventional flux, the prompt flux is not calibrated using the daemonflux method, as surface muons are not sensitive to prompt fluxes. As a result, the prompt component does not include correction parameters or errors. It is important to note, however, that the conventional part of the flux remains calibrated, so the total_ flux is simply the sum of the calibrated conventional and uncalibrated prompt fluxes.
 
+## Using parameter correlations represented by the covariance matrix
+
+The parameters of the model are correlated. These correlations are drdetermined from the data we have used for the fit. The errors are already computed taking the covariance matrix into account when using the `error` method. If daemonflux is used in a fit with free floating parameters, one can include these correlations by adding the chi2 as additional penalty term. The chi2 for the current combination of parameters can be obtained by calling `flux.chi2({dictionary of modified parameters})`.
+
 ## LICENSE
 
 [BSD 3-Clause License](LICENSE)
```

### Comparing `daemonflux-0.7.0/tests/test_daemonflux.py` & `daemonflux-0.8.0/tests/test_daemonflux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import numpy.testing as npt
 import pytest
+import pathlib
 
 from daemonflux.flux import Flux, Parameters, _FluxEntry
 from daemonflux.utils import format_angle, grid_cov, is_iterable, rearrange_covariance
 
 
 def test_format_angle():
     tests = [
@@ -40,17 +41,18 @@
     expected_errors = np.array([1.0, 1.0])
     npt.assert_allclose(errors, expected_errors, rtol=1e-6, atol=1e-6)
     known_parameters = ["param1", "param2"]
 
 
 def test_parameters_chi2():
     known_parameters = ["p1", "p2"]
-    values = np.array([1, 2])
+    values = np.zeros(2)
     cov = np.array([[1.0, 0.5], [0.5, 1.0]])
     params = Parameters(known_parameters, values, cov)
+    params.values = np.array([1, 2])
     chi2 = params.chi2
     expected_chi2 = 4
     npt.assert_allclose(chi2, expected_chi2, rtol=1e-6, atol=1e-6)
 
 
 def test_parameters_class():
     known_parameters = ["param1", "param2"]
@@ -87,15 +89,17 @@
     cov = np.array([[1, 2, 3, 4], [2, 5, 6, 7], [3, 6, 8, 9], [4, 7, 9, 10]])
     expected = np.array([[10, 9, 7, 4], [9, 8, 6, 3], [7, 6, 5, 2], [4, 3, 2, 1]])
 
     assert np.allclose(rearrange_covariance(original_order, new_order, cov), expected)
 
 
 def test_interpolation_domain():
-    zenith_test_dataset = np.array([0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100], dtype=float)
+    zenith_test_dataset = np.array(
+        [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100], dtype=float
+    )
     mock_spl = dict(
         [(format_angle(z), {"numuflux": [], "muflux": []}) for z in zenith_test_dataset]
     )
     known_parameters = ["p1", "p2"]
     values = np.array([1, 2])
     cov = np.array([[1.0, 0.5], [0.5, 1.0]])
     params = Parameters(known_parameters, values, cov)
@@ -132,43 +136,38 @@
         entry._interpolation_domain(np.array([50.0, 45.0]))
     except ValueError as e:
         assert str(e) == "Requested angles must be sorted in ascending order."
 
 
 @pytest.fixture(scope="session")
 def test_flux_calibrated():
-    import pathlib
-
     basep = pathlib.Path(__file__).parent.absolute()
     return Flux(
         "",
         spl_file=basep / "test_daemonsplines_generic_202303_1.pkl",
         cal_file=basep / "test_calibration_default_202303_1.pkl",
         use_calibration=True,
         debug=1,
     )
 
 
 @pytest.fixture(scope="session")
 def test_flux_not_calibrated():
-    import pathlib
-
     basep = pathlib.Path(__file__).parent.absolute()
     return Flux(
         "",
         spl_file=basep / "test_daemonsplines_generic_202303_1.pkl",
         cal_file=basep / "test_calibration_default_202303_1.pkl",
         use_calibration=False,
         debug=1,
     )
 
 
 # Generate updated numbers for this test by running the following:
 def test_Flux(test_flux_calibrated, test_flux_not_calibrated):
-
     egrid = np.logspace(0, 8)
 
     assert np.allclose(
         np.sum(test_flux_calibrated.flux(egrid, "0.0000", "numuflux")), 0.795157
     )
     assert np.allclose(
         np.sum(test_flux_calibrated.flux(egrid, "18.1949", "numuflux")), 0.813709
@@ -351,18 +350,45 @@
     url_generic_spl = (
         test_flux_calibrated._default_url
         + test_flux_calibrated._default_spl_file.format(
             location="generic", rev=test_flux_calibrated._revision
         )
         + ".zip"
     )
+    assert test_flux_calibrated._revision == "202303_2"
     assert request.urlopen(url_generic_spl).status in [200, 302]
-    
+
     for cal_set in ["default", "with_deis"]:
+
         url_cal = (
             test_flux_calibrated._default_url
             + test_flux_calibrated._default_cal_file.format(
                 cset=cal_set, rev=test_flux_calibrated._revision
             )
             + ".zip"
         )
         assert request.urlopen(url_cal).status in [200, 302]
+
+
+def test_chi2(test_flux_calibrated, test_flux_not_calibrated):
+    assert test_flux_calibrated.chi2() == test_flux_not_calibrated.chi2() == 0.0
+    params = test_flux_calibrated.params.known_parameters[:3]
+    values = np.array([1, 2, 3])
+    param_dict = dict(zip(params, values))
+    assert test_flux_calibrated.chi2(param_dict) > 0
+    assert test_flux_not_calibrated.chi2(param_dict)
+
+
+def test_uncorrelated_errors():
+    basep = pathlib.Path(__file__).parent.absolute()
+    fl = Flux(
+        "",
+        spl_file=basep / "test_daemonsplines_generic_202303_1.pkl",
+        cal_file=basep / "test_calibration_default_202303_1.pkl",
+        use_calibration=False,
+        uncorrelated_hadr_errors=True,
+        debug=1,
+    )
+    assert np.allclose(
+        fl.params.cov[: fl.params._n_non_gsf, : fl.params._n_non_gsf],
+        np.diag(np.ones(fl.params._n_non_gsf)),
+    )
```

