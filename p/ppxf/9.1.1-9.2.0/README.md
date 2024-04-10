# Comparing `tmp/ppxf-9.1.1.tar.gz` & `tmp/ppxf-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppxf-9.1.1.tar", last modified: Thu Jan 18 19:03:09 2024, max compression
+gzip compressed data, was "ppxf-9.2.0.tar", last modified: Wed Apr 10 18:10:38 2024, max compression
```

## Comparing `ppxf-9.1.1.tar` & `ppxf-9.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 19:03:09.468234 ppxf-9.1.1/
--rw-rw-rw-   0        0        0   108240 2024-01-18 19:03:09.468234 ppxf-9.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-18 19:03:09.389220 ppxf-9.1.1/ppxf/
--rw-rw-rw-   0        0        0    35226 2024-01-18 19:02:14.000000 ppxf-9.1.1/ppxf/CHANGELOG.rst
--rw-rw-rw-   0        0        0      388 2024-01-05 17:54:47.000000 ppxf-9.1.1/ppxf/LICENSE.txt
--rw-rw-rw-   0        0        0     3058 2023-11-10 19:40:33.000000 ppxf-9.1.1/ppxf/README.rst
--rw-rw-rw-   0        0        0       22 2024-01-18 17:30:36.000000 ppxf-9.1.1/ppxf/__init__.py
--rw-rw-rw-   0        0        0    39684 2023-11-26 15:49:05.000000 ppxf-9.1.1/ppxf/capfit.py
-drwxrwxrwx   0        0        0        0 2024-01-18 19:03:09.436600 ppxf-9.1.1/ppxf/examples/
--rw-rw-rw-   0        0        0    34077 2022-06-10 10:29:46.000000 ppxf-9.1.1/ppxf/examples/FILTER.RES.info.txt
--rw-rw-rw-   0        0        0  2964767 2022-06-10 10:29:28.000000 ppxf-9.1.1/ppxf/examples/FILTER.RES.txt
--rw-rw-rw-   0        0        0       35 2020-11-26 15:46:13.000000 ppxf-9.1.1/ppxf/examples/__init__.py
--rw-rw-rw-   0        0        0    12485 2024-01-04 17:27:50.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_gas_sdss_tied.py
--rw-rw-rw-   0        0        0    11175 2024-01-04 17:30:59.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_kinematics_sauron.py
--rw-rw-rw-   0        0        0    10742 2024-01-04 17:32:46.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_kinematics_sdss.py
--rw-rw-rw-   0        0        0     8641 2024-01-04 17:34:27.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_montecarlo_simulation.py
--rw-rw-rw-   0        0        0    14025 2024-01-18 18:49:08.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_population_gas_sdss.py
--rw-rw-rw-   0        0        0    10799 2024-01-18 18:53:20.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_population_photometry.py
--rw-rw-rw-   0        0        0     6523 2024-01-04 17:53:58.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_sky_and_symmetric_losvd.py
--rw-rw-rw-   0        0        0     7237 2024-01-04 17:56:15.000000 ppxf-9.1.1/ppxf/examples/ppxf_example_two_components.py
--rw-rw-rw-   0        0        0    12828 2024-01-05 19:07:01.000000 ppxf-9.1.1/ppxf/examples/ppxf_python_reference_output.txt
--rw-rw-rw-   0        0        0   133034 2023-12-07 18:27:28.000000 ppxf-9.1.1/ppxf/ppxf.py
--rw-rw-rw-   0        0        0    46976 2024-01-18 17:27:57.000000 ppxf-9.1.1/ppxf/ppxf_util.py
-drwxrwxrwx   0        0        0        0 2024-01-18 19:03:09.452222 ppxf-9.1.1/ppxf/spectra/
--rw-rw-rw-   0        0        0   172800 2011-10-17 22:16:00.000000 ppxf-9.1.1/ppxf/spectra/NGC3073_SDSS_DR8.fits
--rw-rw-rw-   0        0        0   172800 2011-10-17 14:22:36.000000 ppxf-9.1.1/ppxf/spectra/NGC3522_SDSS_DR8.fits
--rw-rw-rw-   0        0        0     5760 2004-12-28 23:44:02.000000 ppxf-9.1.1/ppxf/spectra/NGC4550_SAURON.fits
--rw-rw-rw-   0        0        0   604800 2015-10-12 18:45:25.000000 ppxf-9.1.1/ppxf/spectra/NGC4636_SDSS_DR12.fits
--rw-rw-rw-   0        0        0   155520 2021-03-19 16:06:44.000000 ppxf-9.1.1/ppxf/spectra/legac_M19_56670_v3.0.fits
-drwxrwxrwx   0        0        0        0 2024-01-18 19:03:09.468234 ppxf-9.1.1/ppxf/sps_models/
--rw-rw-rw-   0        0        0   462791 2023-09-23 18:39:50.000000 ppxf-9.1.1/ppxf/sps_models/Vazdekis2012_ssp_mass_Padova00_UN_baseFe_v10.0.txt
--rw-rw-rw-   0        0        0  1063839 2018-04-13 12:44:27.000000 ppxf-9.1.1/ppxf/sps_models/Vazdekis2012_ssp_phot_Padova00_UN_v10.0.txt
--rw-rw-rw-   0        0        0    47415 2018-04-13 12:44:36.000000 ppxf-9.1.1/ppxf/sps_models/Vazdekis2012_ssp_sdss_miuscat_UN1.30_v9.txt
--rw-rw-rw-   0        0        0    19722 2023-10-10 17:43:44.000000 ppxf-9.1.1/ppxf/sps_models/spectra_sun_vega.npz
--rw-rw-rw-   0        0        0    14665 2024-01-18 18:59:47.000000 ppxf-9.1.1/ppxf/sps_util.py
-drwxrwxrwx   0        0        0        0 2024-01-18 19:03:09.468234 ppxf-9.1.1/ppxf.egg-info/
--rw-rw-rw-   0        0        0   108240 2024-01-18 19:03:09.000000 ppxf-9.1.1/ppxf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1231 2024-01-18 19:03:09.000000 ppxf-9.1.1/ppxf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 19:03:09.000000 ppxf-9.1.1/ppxf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-01-18 19:03:09.000000 ppxf-9.1.1/ppxf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-18 19:03:09.000000 ppxf-9.1.1/ppxf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-01-18 19:03:09.000000 ppxf-9.1.1/ppxf.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-01-18 19:03:09.468234 ppxf-9.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-11-12 09:26:58.000000 ppxf-9.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:10:38.569325 ppxf-9.2.0/
+-rw-rw-rw-   0        0        0   109093 2024-04-10 18:10:38.569325 ppxf-9.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 18:10:38.143747 ppxf-9.2.0/ppxf/
+-rw-rw-rw-   0        0        0    36062 2024-04-10 17:47:24.000000 ppxf-9.2.0/ppxf/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      388 2024-01-05 17:54:47.000000 ppxf-9.2.0/ppxf/LICENSE.txt
+-rw-rw-rw-   0        0        0     3058 2023-11-10 19:40:33.000000 ppxf-9.2.0/ppxf/README.rst
+-rw-rw-rw-   0        0        0       22 2024-04-10 18:09:49.000000 ppxf-9.2.0/ppxf/__init__.py
+-rw-rw-rw-   0        0        0    39781 2024-01-31 18:05:35.000000 ppxf-9.2.0/ppxf/capfit.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:10:38.340506 ppxf-9.2.0/ppxf/examples/
+-rw-rw-rw-   0        0        0    34077 2022-06-10 10:29:46.000000 ppxf-9.2.0/ppxf/examples/FILTER.RES.info.txt
+-rw-rw-rw-   0        0        0  2964767 2022-06-10 10:29:28.000000 ppxf-9.2.0/ppxf/examples/FILTER.RES.txt
+-rw-rw-rw-   0        0        0       35 2020-11-26 15:46:13.000000 ppxf-9.2.0/ppxf/examples/__init__.py
+-rw-rw-rw-   0        0        0    12485 2024-01-04 17:27:50.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_gas_sdss_tied.py
+-rw-rw-rw-   0        0        0    11175 2024-01-04 17:30:59.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_kinematics_sauron.py
+-rw-rw-rw-   0        0        0    10742 2024-01-04 17:32:46.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_kinematics_sdss.py
+-rw-rw-rw-   0        0        0     8742 2024-03-16 11:15:46.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_montecarlo_simulation.py
+-rw-rw-rw-   0        0        0    14107 2024-02-08 18:01:10.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_population_gas_sdss.py
+-rw-rw-rw-   0        0        0    10881 2024-02-08 17:59:57.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_population_photometry.py
+-rw-rw-rw-   0        0        0     6523 2024-01-04 17:53:58.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_sky_and_symmetric_losvd.py
+-rw-rw-rw-   0        0        0     7237 2024-01-04 17:56:15.000000 ppxf-9.2.0/ppxf/examples/ppxf_example_two_components.py
+-rw-rw-rw-   0        0        0    12827 2024-04-10 18:08:16.000000 ppxf-9.2.0/ppxf/examples/ppxf_python_reference_output.txt
+-rw-rw-rw-   0        0        0   133311 2024-04-10 17:37:02.000000 ppxf-9.2.0/ppxf/ppxf.py
+-rw-rw-rw-   0        0        0    48330 2024-03-21 17:07:37.000000 ppxf-9.2.0/ppxf/ppxf_util.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:10:38.356507 ppxf-9.2.0/ppxf/spectra/
+-rw-rw-rw-   0        0        0   172800 2011-10-17 22:16:00.000000 ppxf-9.2.0/ppxf/spectra/NGC3073_SDSS_DR8.fits
+-rw-rw-rw-   0        0        0   172800 2011-10-17 14:22:36.000000 ppxf-9.2.0/ppxf/spectra/NGC3522_SDSS_DR8.fits
+-rw-rw-rw-   0        0        0     5760 2004-12-28 23:44:02.000000 ppxf-9.2.0/ppxf/spectra/NGC4550_SAURON.fits
+-rw-rw-rw-   0        0        0   604800 2015-10-12 18:45:25.000000 ppxf-9.2.0/ppxf/spectra/NGC4636_SDSS_DR12.fits
+-rw-rw-rw-   0        0        0   155520 2021-03-19 16:06:44.000000 ppxf-9.2.0/ppxf/spectra/legac_M19_56670_v3.0.fits
+drwxrwxrwx   0        0        0        0 2024-04-10 18:10:38.544584 ppxf-9.2.0/ppxf/sps_models/
+-rw-rw-rw-   0        0        0   462791 2023-09-23 18:39:50.000000 ppxf-9.2.0/ppxf/sps_models/Vazdekis2012_ssp_mass_Padova00_UN_baseFe_v10.0.txt
+-rw-rw-rw-   0        0        0  1063839 2018-04-13 12:44:27.000000 ppxf-9.2.0/ppxf/sps_models/Vazdekis2012_ssp_phot_Padova00_UN_v10.0.txt
+-rw-rw-rw-   0        0        0    47415 2018-04-13 12:44:36.000000 ppxf-9.2.0/ppxf/sps_models/Vazdekis2012_ssp_sdss_miuscat_UN1.30_v9.txt
+-rw-rw-rw-   0        0        0    19722 2023-10-10 17:43:44.000000 ppxf-9.2.0/ppxf/sps_models/spectra_sun_vega.npz
+-rw-rw-rw-   0        0        0    14734 2024-01-22 11:26:26.000000 ppxf-9.2.0/ppxf/sps_util.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:10:38.553032 ppxf-9.2.0/ppxf.egg-info/
+-rw-rw-rw-   0        0        0   109093 2024-04-10 18:10:37.000000 ppxf-9.2.0/ppxf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1231 2024-04-10 18:10:37.000000 ppxf-9.2.0/ppxf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 18:10:37.000000 ppxf-9.2.0/ppxf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-10 18:10:37.000000 ppxf-9.2.0/ppxf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 18:10:37.000000 ppxf-9.2.0/ppxf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 18:10:37.000000 ppxf-9.2.0/ppxf.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-10 18:10:38.569325 ppxf-9.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-11-12 09:26:58.000000 ppxf-9.2.0/setup.py
```

### Comparing `ppxf-9.1.1/PKG-INFO` & `ppxf-9.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppxf
-Version: 9.1.1
+Version: 9.2.0
 Summary: pPXF: Full Spectrum and SED Fitting of Galactic and Stellar Spectra
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -1468,22 +1468,39 @@
 redistribute the code.
 
 ###########################################################################
 
 Changelog
 ---------
 
+V9.2.0: MC, Oxford, 10 April 2024
++++++++++++++++++++++++++++++++++
+
+- **Improved** ``sps_util.synthetic_photometry``: Accepts input wavelengths
+  that are not evenly spaced.
+- **Added** ``ppxf_util.mag_spectrum``: A new function to get the apparent
+  magnitude from a spectrum in any photometric band, at any redshift, in either
+  the AB or Vega magnitude system.
+- **Improved** ``ppxf``: Now considers the given ``goodpixels`` when checking
+  that the ``templates`` cover the full ``galaxy`` spectrum, if both ``lam``
+  and ``lam_temp`` are provided.
+- **Fixed** ``ppxf``: Avoids new ``SyntaxWarning`` in Matplotlib LaTeX string
+  in the latest Python 3.12.
+- **Fixed** ``ppxf``: Avoid program stop when passing an input covariance
+  matrix while fitting for gas emission lines. Thanks to Jackson ODonnell
+  (ucsc.edu) for the report.
+
 V9.1.1: MC, Oxford, 18 January 2024
 +++++++++++++++++++++++++++++++++++
 
 - **Improved** ``sps_util.mass_to_light``: Now it can calculate the stellar
   mass-to-light ratio (``M*/L``) for any stellar population synthesis (SPS)
   model, any filter, and any redshift, using the output weights from ``pPXF``.
   No need for pre-computed tables anymore.
-- **Added** ``ppxf_util.solar_mag``: A new function to get the absolute solar
+- **Added** ``ppxf_util.mag_sun``: A new function to get the absolute solar
   magnitude in any photometric band, at any redshift, in either the AB or Vega
   magnitude system.
 
 V9.0.2: MC, Oxford, 30 November 2023
 ++++++++++++++++++++++++++++++++++++
 
 - ``ppxf``: Fixed bug in the automatic truncation of the template wavelength,
```

### Comparing `ppxf-9.1.1/ppxf/CHANGELOG.rst` & `ppxf-9.2.0/ppxf/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 
 Changelog
 ---------
 
+V9.2.0: MC, Oxford, 10 April 2024
++++++++++++++++++++++++++++++++++
+
+- **Improved** ``sps_util.synthetic_photometry``: Accepts input wavelengths
+  that are not evenly spaced.
+- **Added** ``ppxf_util.mag_spectrum``: A new function to get the apparent
+  magnitude from a spectrum in any photometric band, at any redshift, in either
+  the AB or Vega magnitude system.
+- **Improved** ``ppxf``: Now considers the given ``goodpixels`` when checking
+  that the ``templates`` cover the full ``galaxy`` spectrum, if both ``lam``
+  and ``lam_temp`` are provided.
+- **Fixed** ``ppxf``: Avoids new ``SyntaxWarning`` in Matplotlib LaTeX string
+  in the latest Python 3.12.
+- **Fixed** ``ppxf``: Avoid program stop when passing an input covariance
+  matrix while fitting for gas emission lines. Thanks to Jackson ODonnell
+  (ucsc.edu) for the report.
+
 V9.1.1: MC, Oxford, 18 January 2024
 +++++++++++++++++++++++++++++++++++
 
 - **Improved** ``sps_util.mass_to_light``: Now it can calculate the stellar
   mass-to-light ratio (``M*/L``) for any stellar population synthesis (SPS)
   model, any filter, and any redshift, using the output weights from ``pPXF``.
   No need for pre-computed tables anymore.
-- **Added** ``ppxf_util.solar_mag``: A new function to get the absolute solar
+- **Added** ``ppxf_util.mag_sun``: A new function to get the absolute solar
   magnitude in any photometric band, at any redshift, in either the AB or Vega
   magnitude system.
 
 V9.0.2: MC, Oxford, 30 November 2023
 ++++++++++++++++++++++++++++++++++++
 
 - ``ppxf``: Fixed bug in the automatic truncation of the template wavelength,
```

### Comparing `ppxf-9.1.1/ppxf/README.rst` & `ppxf-9.2.0/ppxf/README.rst`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/capfit.py` & `ppxf-9.2.0/ppxf/capfit.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
     find a vector x which solves::
 
           Minimize      || A @ x - b ||
           Subject to    bounds[0] <= x <= bounds[1]
 
     This function implements an improved and faster version of the
     BVLS algorithm by Lawson & Hanson (1995) and Stark & Parker (1995),
-    which both generalize the L&H active-set NNLS algorithm (23.10).
+    which both generalize the L&H95 active-set NNLS algorithm (23.10).
     
     This implementation is described in Section 3.2.3 of the paper
     `Cappellari (2023) <https://ui.adsabs.harvard.edu/abs/2023MNRAS.526.3273C>`_.
 
     It allows for an initial value for x, which can dramatically speed up
     convergence when a good guess is available. I also included an
     initialization phase, given as Algorithm 3 of `Cappellari (2023)`_.
@@ -577,14 +577,16 @@
         }
 
     Calling Sequence
     ----------------
 
     .. code-block:: python
 
+        from ppxf.capfit import capfit
+
         res = capfit(func, p1, A_eq=None, A_ineq=None, abs_step=None, b_eq=None,
                      b_ineq=None, bounds=(-np.inf, np.inf), diff_step=1e-4,
                      fixed=None, ftol=1e-4, linear_method='cvxopt',
                      max_nfev=None, rcond=None, tied=None, verbose=0,
                      x_scale='jac', xtol=1e-4, args=(), kwargs={})
 
         print(f"solution: {res.x}")
@@ -849,15 +851,15 @@
             resid = func(p, *args, **kwargs)
             assert np.all(np.isfinite(resid)), \
                 "The fitting function returned infinite residuals"
             return resid
 
         p1, p1_err = self.optimize(call, p0[free], A_eq, b_eq, A_ineq, b_ineq, bounds[:, free])
 
-        self.x = tie(p1)
+        self.x = tie(p1)   # Return both free and tied/fixed variables
         self.x_err = np.zeros_like(self.x)
         self.x_err[free] = p1_err
 
 ################################################################################
 
     def optimize(self, call, p1, A_eq, b_eq, A_ineq, b_ineq, bounds):
         """
@@ -870,15 +872,15 @@
         dd = linalg.norm(J1, axis=0)
         mx = np.max(dd)
         eps = np.finfo(float).eps
         dd[dd < eps*max(1, mx)] = 1  # As More'+80
         lam = 0.01*mx**2  # 0.01*max(diag(J1.T @ J1))
 
         if self.verbose == 2:
-            print(f"\nStart lambda: {lam:#.4g}  chi2: {chi2(f1):#.4g}\nStart p_free:" + fprint(p1))
+            print(f"\nStart lambda: {lam:#.4g}  chi2: {chi2(f1):#.4g}\nStart p[free]:" + fprint(p1))
 
         while True:
 
             if self.x_scale == 'jac':
                 dd = np.maximum(dd, linalg.norm(J1, axis=0))
             else:
                 dd = np.ones_like(p1)/self.x_scale
@@ -910,15 +912,15 @@
 
             if status != -1:
                 if actred > 0:
                     p1, f1 = p2, f2
                 if self.verbose:
                     print(f"\n{self.message}\nFinal iter: {self.njev}  "
                           f"Func calls: {self.nfev}  chi2: {chi2(f1):#.4g}  "
-                          f"Status: {status}\nFinal p:" + fprint(p1) + "\n")
+                          f"Status: {status}\nFinal p[free]:" + fprint(p1) + "\n")
                 break
 
             # Algorithm (5.2.7) of Fletcher (1987)
             # Algorithm 4.1 in Nocedal & Wright (2006)
             if ratio < 0.25:
                 lam *= 4
             elif ratio > 0.75:
@@ -991,12 +993,12 @@
                 status = 4
             else:
                 self.message = "Terminating on small step (xtol)"
                 status = 3
 
         if self.verbose == 2:
             print(f"\niter: {self.njev}  lambda: {lam:#.4g}  chi2: {chi2(f):#.4g}"
-                  f"  ratio: {actred/prered:#.4g}\np_free:" + fprint(p) + "\nh:" + fprint(h))
+                  f"  ratio: {actred/prered:#.4g}\np[free]:" + fprint(p) + "\ndp:" + fprint(h))
 
         return status
 
 ################################################################################
```

### Comparing `ppxf-9.1.1/ppxf/examples/FILTER.RES.info.txt` & `ppxf-9.2.0/ppxf/examples/FILTER.RES.info.txt`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/FILTER.RES.txt` & `ppxf-9.2.0/ppxf/examples/FILTER.RES.txt`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_gas_sdss_tied.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_gas_sdss_tied.py`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_kinematics_sauron.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_kinematics_sauron.py`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_kinematics_sdss.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_kinematics_sdss.py`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_montecarlo_simulation.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_montecarlo_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 #       example unchanged from any directory. MC, Oxford, 17 April 2018
 #   V2.1.4: Dropped legacy Python 2.7 support. MC, Oxford, 10 May 2018
 #   V4.0.3: Fixed clock DeprecationWarning in Python 3.7.
 #       MC, Oxford, 27 September 2018
 #   V4.1.0: Use E-Miles spectral library. MC, Oxford, 16 March 2022
 #   V4.2.0: Use the new `sps_util` instead of `miles_util`. 
 #       MC, Oxford, 12 November 2023
+#   V4.2.1: Use updated random generator default_rng. 
+#       MC, Oxford, 16 March 2024
 #
 ##############################################################################
 
 from time import perf_counter as clock
 from pathlib import Path
 from urllib import request
 
@@ -62,18 +64,20 @@
 
 from ppxf.ppxf import ppxf, rebin
 import ppxf.ppxf_util as util
 import ppxf.sps_util as lib
 
 #----------------------------------------------------------------------------
 
-def ppxf_example_simulation():
+def ppxf_example_simulation(seed=123):
 
     ppxf_dir = Path(util.__file__).parent
 
+    rng = np.random.default_rng(seed)  # For reproducible results
+
     lam_range_temp = [3500, 7500]
     sps_name = 'emiles'
     velscale = 35   # km/s
 
     # Read SPS models file from my GitHub if not already in the ppxf package dir.
     # The SPS model files are also available here https://github.com/micappe/ppxf_data
     basename = f"spectra_{sps_name}_9.0.npz"
@@ -101,15 +105,15 @@
     star = rebin(starNew, factor)        # Make sure that the observed spectrum is the integral over the pixels
 
     h3 = 0.1       # Adopted G-H parameters of the LOSVD
     h4 = 0.1
     sn = 30.        # Adopted S/N of the Monte Carlo simulation
     m = 300        # Number of realizations of the simulation
     moments = 4
-    velV = np.random.rand(m)  # velocity in *pixels* [=V(km/s)/velScale]
+    velV = rng.uniform(size=m)      # velocity in *pixels* [=V(km/s)/velScale]
     sigmaV = np.linspace(0.5, 4, m) # Range of sigma in *pixels* [=sigma(km/s)/velScale]
 
     result = np.zeros((m, moments)) # This will store the results
     t = clock()
 
     for j, (vel, sigma) in enumerate(zip(velV, sigmaV)):
 
@@ -122,16 +126,16 @@
         h3poly = w*(2.*w2 - 3.)/np.sqrt(3.)             # H3(y)
         h4poly = (w2*(4.*w2 - 12.) + 3.)/np.sqrt(24.)   # H4(y)
         losvd = gauss *(1. + h3*h3poly + h4*h4poly)
 
         galaxy = signal.fftconvolve(starNew, losvd, mode="same") # Convolve the oversampled spectrum
         galaxy = rebin(galaxy, factor) # Integrate spectrum into original spectral pixels
         noise = galaxy/sn        # 1sigma error spectrum
-        galaxy = np.random.normal(galaxy, noise) # Add noise to the galaxy spectrum
-        start = np.array([vel + np.random.uniform(-1, 1), sigma*np.random.uniform(0.8, 1.2)])*velscale  # Convert to km/s
+        galaxy = rng.normal(galaxy, noise) # Add noise to the galaxy spectrum
+        start = np.array([vel + rng.uniform(-1, 1), sigma*rng.uniform(0.8, 1.2)])*velscale  # Convert to km/s
 
         pp = ppxf(star, galaxy, noise, velscale, start,
                   goodpixels=np.arange(dx, galaxy.size - dx),
                   plot=False, moments=moments, bias=0.1)
         result[j,:] = pp.sol
 
     print('Calculation time: %.2f s' % (clock()-t))
@@ -182,9 +186,8 @@
     plt.tight_layout()
     plt.pause(5)
 
 #----------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
-    np.random.seed(123)  # For reprodcible results
     ppxf_example_simulation()
```

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_population_gas_sdss.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_population_gas_sdss.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,16 @@
     #
     noise = np.full_like(galaxy, 0.0163)  # Assume constant noise per pixel here
 
     # The velocity step was already chosen by the SDSS pipeline,
     # and we convert it below to km/s
     #
     c = 299792.458  # speed of light in km/s
-    velscale = c*np.log(wave[1]/wave[0])  # eq.(8) of Cappellari (2017)
+    d_ln_lam = np.log(wave[-1]/wave[0])/(wave.size - 1)  # Average ln_lam step
+    velscale = c*d_ln_lam                   # eq. (8) of Cappellari (2017)
     FWHM_gal = 2.76  # SDSS has an approximate instrumental resolution FWHM of 2.76A.
 
     #------------------- Setup stellar templates -----------------------
 
     # pPXF can be used with any set of SPS population templates. However, I am
     # currently providing (with permission) ready-to-use template files for
     # three SPS. One can just uncomment one of the three models below. The
```

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_population_photometry.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_population_photometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
                             2.93e-17, 2.30e-17, 1.30e-17, 7.83e-18, 3.49e-18])  # fluxes in erg/cm^2/s/A
     phot_noise = np.full_like(phot_galaxy, np.max(phot_galaxy)*0.03)  # 1sigma uncertainties of 3%
 
     # ------------------- Setup spectral templates -----------------------------
 
     # The velocity step was already chosen by the SDSS pipeline and I convert it to km/s
     c = 299792.458  # speed of light in km/s
-    velscale = c*np.log(wave[1]/wave[0])  # eq.(8) of Cappellari (2017)
+    d_ln_lam = np.log(wave[-1]/wave[0])/(wave.size - 1)  # Average ln_lam step
+    velscale = c*d_ln_lam                   # eq. (8) of Cappellari (2017)
     FWHM_gal = 2.76  # SDSS has an approximate instrumental resolution FWHM of 2.76A.
 
     # Read SPS model file from my GitHub if not already in the ppxf package dir.
     # The SPS model files are also available here https://github.com/micappe/ppxf_data
     basename = f"spectra_{sps_name}_9.0.npz"
     filename = ppxf_dir / 'sps_models' / basename
     if not filename.is_file():
```

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_sky_and_symmetric_losvd.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_sky_and_symmetric_losvd.py`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_example_two_components.py` & `ppxf-9.2.0/ppxf/examples/ppxf_example_two_components.py`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/examples/ppxf_python_reference_output.txt` & `ppxf-9.2.0/ppxf/examples/ppxf_python_reference_output.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Reference expected output of the pPXF 9.1.0 examples (5 January 2024).
-# Python 3.11 using NumPy 1.26, SciPy 1.11, Matplotlib 3.8
+# Reference expected output of the pPXF 9.2.0 examples (10 April 2024).
+# Python 3.12 using NumPy 1.26, SciPy 1.13, Matplotlib 3.8
 ###############################################################################
 
 
 >>> runfile('ppxf_example_kinematics_sauron.py')
 
   Best Fit:       Vel     sigma        h3        h4
  comp.  0:        33       111     0.028     0.066
```

### Comparing `ppxf-9.1.1/ppxf/ppxf.py` & `ppxf-9.2.0/ppxf/ppxf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1976,18 +1976,18 @@
             self.templates_full = self.templates.copy()
             self.lam_temp_full = self.lam_temp.copy()
             if bounds is None:
                 vlim = np.array([2900, -2900])  # Default bounds: 2e3 as nonlinear_fit() +900 for 3sigma
             else:
                 vlim = [np.array(b[0]) - s[0] for b, s in zip(bounds, start)]
                 vlim = np.array([np.max(vlim) + 900, np.min(vlim) - 900])
-            lam_range = self.lam[[0, -1]]/np.exp(vlim/c)   # Use eq.(5c) of Cappellari (2023)
+            lam_range = self.lam[self.goodpixels][[0, -1]]/np.exp(vlim/c)   # Use eq.(5c) of Cappellari (2023)
             assert (self.lam_temp[0] <= lam_range[0]) and (self.lam_temp[-1] >= lam_range[1]), \
                 "The `templates` must cover the full wavelength range of the " \
-                "`galaxy` for the adopted velocity starting guess"
+                "`galaxy[goodpixels]` spectrum for the adopted velocity starting guess"
             ok = (self.lam_temp > lam_range[0]) & (self.lam_temp < lam_range[1])
             self.templates = self.templates[ok, :]
             self.lam_temp = self.lam_temp[ok]
             self.npix_temp = self.templates.shape[0]
             lam_temp_min = np.mean(self.lam_temp[:self.velscale_ratio])
             self.vsyst = c*np.log(lam_temp_min/self.lam[0])/self.velscale
         elif self.templates.shape[0]/self.velscale_ratio > 2*self.galaxy.shape[0]:
@@ -2475,15 +2475,15 @@
                 phot_bestfit = self.phot_bestfit*phot_x
                 phot_noise = self.phot_noise*phot_x
                 if self.lam_temp is not None:
                     bestfit_full = self.bestfit_full*x_full
                     if self.gas_any:
                         gas_bestfit_full = self.gas_bestfit_full*x_full
         else:
-            plt.ylabel("Relative Flux ($f_\lambda$)")
+            plt.ylabel(r"Relative Flux ($f_\lambda$)")
             galaxy = self.galaxy
             bestfit = self.bestfit
             if self.gas_any:
                 gas_bestfit = self.gas_bestfit
                 gas_bestfit_templates= self.gas_bestfit_templates
             if phot:
                 phot_galaxy = self.phot_galaxy
@@ -2665,15 +2665,20 @@
 
         if self.gas_any:
             gas = self.gas_component
             spectra = self.matrix[: , npoly : npoly + self.ntemp]   # Remove polynomials & sky
             weights = self.weights[: self.ntemp]                    # Remove sky weights
             integ = abs(spectra[: , gas].sum(0))
             self.gas_flux = integ*weights[gas]
-            design_matrix = spectra[:, gas]/self.noise[: , None]
+            if self.noise.ndim == 2:
+                # input NOISE is a npix*npix covariance matrix
+                design_matrix = self.noise @ spectra[:, gas]
+            else:
+                # input NOISE is a 1sigma error vector
+                design_matrix = spectra[:, gas]/self.noise[: , None]
             self.gas_flux_error = integ*cov_err(design_matrix)[1]
             self.gas_bestfit_templates = spectra[:, gas]*weights[gas]
             self.gas_bestfit = self.gas_bestfit_templates.sum(1)
             if self.gas_any_zero:
                 self.gas_flux[self.gas_zero_template] = np.nan
                 self.gas_flux_error[self.gas_zero_template] = np.nan
```

### Comparing `ppxf-9.1.1/ppxf/ppxf_util.py` & `ppxf-9.2.0/ppxf/ppxf_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ###############################################################################
 
-    Copyright (C) 2001-2023, Michele Cappellari
+    Copyright (C) 2001-2024, Michele Cappellari
     E-mail: michele.cappellari_at_physics.ox.ac.uk
 
     This software is provided as is without any warranty whatsoever.
     Permission to use, for non-commercial purposes is granted.
     Permission to modify for personal or internal use is granted,
     provided this copyright and disclaimer are included unchanged
     at the beginning of the file. All other rights are reserved.
@@ -806,15 +806,15 @@
     conv_temp = rebin(conv_temp[:npix*velscale_ratio, :], velscale_ratio)
 
     return conv_temp.squeeze()
 
 ###############################################################################
 # MODIFICATION HISTORY:
 #   V1.0.0: Written. Michele Cappellari, Oxford, 15 March 2022
-#   V1.1.0: Moved from, miles_util to ppxf_util and request spectra as input.
+#   V1.1.0: Moved from, sps_util to ppxf_util and request spectra as input.
 #       MC, Oxford, 4 April 2022
 
 class synthetic_photometry:
     """
     Purpose
     -------
 
@@ -829,19 +829,19 @@
     density is not adjusted for cosmological effects. The user is expected to
     explicitly account for the factor `(1 + z)` when needed.
 
     Input Parameters
     ----------------
 
     spectra : array_like of shape (n_pixels, n_spectra) or (n_pixels, ...)
-        Logarithmically-sampled spectra arranged as columns.
-        Fluxes must be proportional to `ergs/(s cm^2 A)` units.
+        Single spectrum vector or multiple spectra arranged as columns of an
+        array. Fluxes must be proportional to `ergs/(s cm^2 A)` units.
     lam_spec : array_like of shape (n_pixels,)
-        Logarithmically-sampled restframe wavelength in Angstrom for every
-        pixel of `spectra`.
+        Restframe wavelength in Angstrom for every pixel of `spectra`. This can
+        be non-uniformly sampled.
     redshift : float
         Approximate redshift of the galaxy under study.
     bands : string array_like of shape (n_bands,)
         String identifying the filter. The matching is done using partial
         string matching with the file FILTER.RES.txt.
         For example, if the filter in the file is "Johnson B-band", one can
         use "B-band" as long as it does not match other filters in the file.
@@ -879,24 +879,19 @@
     """
     def __init__(self, spectra, lam_spec, bands,
                  redshift=0, filters_file=None, quiet=False):
 
         assert len(lam_spec) == len(spectra), \
             "`lam_spec`  must have the same number of elements as `spectra.shape[0]`"
 
-        bands = np.atleast_1d(bands)
-        ln_lam_spec = np.log(lam_spec)
-        d_ln_lam = np.diff(ln_lam_spec)
-        d_ln_lam_mean = np.diff(ln_lam_spec[[0, -1]])/(lam_spec.size - 1)
-        assert np.allclose(d_ln_lam, d_ln_lam_mean), "`lam_spec` must be logarithmically sampled"
-
         if filters_file is None:
             ppxf_dir = Path(__file__).parent  # path of current file
             filters_file = ppxf_dir / 'examples' / 'FILTER.RES.txt'
 
+        bands = np.atleast_1d(bands)
         lam_eff, flux = np.empty((2, len(bands), *spectra.shape[1:]))
         lam_piv = np.empty(len(bands))
         ok = np.empty(len(bands), dtype=bool)
         for j, band in enumerate(bands):
             lam_eff[j], lam_piv[j], flux[j], ok[j] = synthetic_photometry_one_band(
                 spectra, lam_spec, band, redshift, filters_file)
             if not quiet:
@@ -923,25 +918,24 @@
 
     """
     lam_resp, response = read_filter(band, filters_file)
     lam_resp /= 1 + redshift
     lam_in_fwhm = lam_resp[response > 0.5*np.max(response)]  # I want FWHM fully covered
     ok = np.all((lam_in_fwhm >= lam_spec[0]) & (lam_in_fwhm <= lam_spec[-1]))
 
-    # The spectrum is logarithmically sampled. Use the following:
-    # Integrate[f[lam], lam] = Integrate[lam*f[lam], ln_lam]
     if ok:
         fil = np.interp(lam_spec, lam_resp, response, left=0, right=0)
-        filam2 = fil*lam_spec**2
-        filam3 = filam2*lam_spec
-        int1 = filam2.sum()             # Integrate[S[lam]*lam, lam]
-        int2 = filam3.sum()             # Integrate[S[lam]*lam^2, lam]
-        int3 = (spectra.T @ filam2).T   # Integrate[g[lam]*S[lam]*lam, lam]
-        int4 = (spectra.T @ filam3).T   # Integrate[g[lam]*S[lam]*lam^2, lam]
-        int5 = fil.sum()                # Integrate[S[lam]/lam, lam]
+        fdlam = fil*np.gradient(lam_spec)  
+        filam2 = fdlam*lam_spec
+        filam3 = filam2*lam_spec      
+        int1 = filam2.sum()                 # Integrate[S[lam]*lam, lam]
+        int2 = filam3.sum()                 # Integrate[S[lam]*lam^2, lam]
+        int3 = (spectra.T @ filam2).T       # Integrate[g[lam]*S[lam]*lam, lam]
+        int4 = (spectra.T @ filam3).T       # Integrate[g[lam]*S[lam]*lam^2, lam]
+        int5 = (fdlam/lam_spec).sum()       # Integrate[S[lam]/lam, lam]
         flux = int3/int1
         with np.errstate(invalid='ignore'):
             lam_eff = np.where(int3 > 0, int4/int3, int2/int1)
         lam_piv = np.sqrt(int1/int5)
     else:
         lam_eff = flux = np.full(spectra.shape[1:], np.nan)
         lam_piv = np.nan
@@ -958,23 +952,23 @@
     response values. Subsequent rows contain the response function wavelength
     in Angstrom and the response function value, in the second and third column
     respectively. The absolute normalization of the response function is
     irrelevant.
 
     FILE FORMAT EXAMPLE:
 
-          3 Johnson B-band ...
+          4 Johnson B-band ...
         1   3000   0
-        2   4000   0.5
-        3   5000   0
-          4 Johnson V-band ...
-        1   4000   0
+        2   3500   0.5
+        3   4000   0.3
+        4   4500   0
+          3 Johnson V-band ...
+        1   4500   0
         2   5000   0.5
-        3   6000   0.5
-        4   7000   0
+        3   5500   0
     """
     lines = []
     with open(filters_file) as f:
         for ln in f:
             if band in ln:
                 for j in range(int(ln.split()[0])):
                     lines.append(next(f))
@@ -985,44 +979,84 @@
 
     j, lam, resp = np.array([ln.split() for ln in lines], float).T
 
     return lam, resp
 
 ###############################################################################
 
-def solar_mag(bands, redshift=0, system='AB'):
+def mag_sun(bands, redshift=0, system='AB', quiet=True):
     """
     Computes the absolute magnitude of the Sun in the AB or Vega magnitude
     system in the given set of bands, optionally shifted to the given redshift.
     
     NB: The (1 + z) dimming factor is *not* applied.
 
     """        
-    ppxf_dir = Path(__file__).parent  # path of current file
+    ppxf_dir = Path(__file__).parent        # path of current file
     filename = ppxf_dir / 'sps_models' / 'spectra_sun_vega.npz'
-    a = np.load(filename)   # Spectrum in cgs/A at 10pc
+    a = np.load(filename)                   # Spectra in erg/s/cm2/A at 10pc
     flux_sun, lam = a["flux_sun"], a["lam"]
 
     if system == 'AB':
-        c_as = 299792458e+10                        # speed of light in A/s
-        flux_ref = 3631e-23*c_as/lam**2             # AB flux in cgs/A
+        c_as = 299792458e+10                # speed of light in A/s
+        flux_ref = 3631e-23*c_as/lam**2     # AB flux in erg/s/cm2/A
     elif system == 'Vega':
         flux_ref = a["flux_vega"]
 
-    velscale = 1000  # Don't need high resolution for photometry
     flux = np.column_stack([flux_sun, flux_ref])
-    flux_new, ln_lam, velscale = log_rebin(lam, flux, velscale)
-
-    p = synthetic_photometry(flux_new, np.exp(ln_lam), bands, redshift=redshift, quiet=True)
+    p = synthetic_photometry(flux, lam, bands, redshift=redshift, quiet=quiet)
     sun_mag = -2.5*np.log10(np.divide(*p.flux.T))
 
     return sun_mag
 
 ###############################################################################
 
+def mag_spectrum(spectrum, lam, bands='SDSS/r', redshift=0, system='AB', quiet=True):
+    """
+    Computes the apparent magnitude from a spectrum in erg/s/cm2/A, in the AB
+    or Vega magnitude system in the given set of bands, optionally shifted to
+    the given redshift.
+
+    Input Parameters
+    ----------------
+
+    spectrum: array_like with shape (n_pixels,)
+        Spectrum flux density in erg/s/cm2/A.
+    lam: array_like with shape (n_pixels,)
+        Wavelength in Angstrom of every pixel in the spectrum.
+    bands: string or array_like of strings with shape (n_bands,)
+        Bands for which one wants to compute the magnitude.
+
+    Output Parameters
+    -----------------
+
+    mag: array_like with shape (n_bands,)
+        Apparent magnitude in each of the input bands. If the redshift is
+        nonzero, the spectrum is red-shifted to the desired redshift before
+        computing the magnitude. However, no cosmological dimming of the
+        spectrum is performed.
+    """        
+    p2 = synthetic_photometry(spectrum, lam, bands, redshift=redshift, quiet=quiet)
+
+    if system == 'AB':
+        c_as = 299792458e+10                # speed of light in A/s
+        flux = 3631e-23*c_as/lam**2         # AB flux in erg/s/cm2/A
+    elif system == 'Vega':
+        ppxf_dir = Path(__file__).parent    # path of current file
+        filename = ppxf_dir / 'sps_models' / 'spectra_sun_vega.npz'
+        a = np.load(filename)               # Spectra in erg/s/cm2/A at 10pc
+        flux, lam = a["flux_vega"], a["lam"]
+
+    p1 = synthetic_photometry(flux, lam, bands, redshift=redshift, quiet=quiet)
+    mag = -2.5*np.log10(p2.flux/p1.flux)
+
+    return mag
+
+##############################################################################
+
 def varsmooth(x, y, sig_x, xout=None, oversample=1):
     """    
     Fast and accurate convolution with a Gaussian of variable width.
 
     This function performs an accurate Fourier convolution of a vector or the
     columns of an array with a Gaussian kernel that has a varying or constant
     standard deviation (sigma) per pixel. The convolution is done using fast
```

### Comparing `ppxf-9.1.1/ppxf/spectra/NGC3073_SDSS_DR8.fits` & `ppxf-9.2.0/ppxf/spectra/NGC3073_SDSS_DR8.fits`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/spectra/NGC3522_SDSS_DR8.fits` & `ppxf-9.2.0/ppxf/spectra/NGC3522_SDSS_DR8.fits`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/spectra/NGC4550_SAURON.fits` & `ppxf-9.2.0/ppxf/spectra/NGC4550_SAURON.fits`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/spectra/NGC4636_SDSS_DR12.fits` & `ppxf-9.2.0/ppxf/spectra/NGC4636_SDSS_DR12.fits`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/spectra/legac_M19_56670_v3.0.fits` & `ppxf-9.2.0/ppxf/spectra/legac_M19_56670_v3.0.fits`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/sps_models/Vazdekis2012_ssp_mass_Padova00_UN_baseFe_v10.0.txt` & `ppxf-9.2.0/ppxf/sps_models/Vazdekis2012_ssp_mass_Padova00_UN_baseFe_v10.0.txt`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/sps_models/Vazdekis2012_ssp_phot_Padova00_UN_v10.0.txt` & `ppxf-9.2.0/ppxf/sps_models/Vazdekis2012_ssp_phot_Padova00_UN_v10.0.txt`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/sps_models/Vazdekis2012_ssp_sdss_miuscat_UN1.30_v9.txt` & `ppxf-9.2.0/ppxf/sps_models/Vazdekis2012_ssp_sdss_miuscat_UN1.30_v9.txt`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/sps_models/spectra_sun_vega.npz` & `ppxf-9.2.0/ppxf/sps_models/spectra_sun_vega.npz`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/ppxf/sps_util.py` & `ppxf-9.2.0/ppxf/sps_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ###############################################################################
 #
-# Copyright (C) 2016-2023, Michele Cappellari
+# Copyright (C) 2016-2024, Michele Cappellari
 # E-mail: michele.cappellari_at_physics.ox.ac.uk
 #
 # This software is provided as is without any warranty whatsoever.
 # Permission to use, for non-commercial purposes is granted.
 # Permission to modify for personal or internal use is granted,
 # provided this copyright and disclaimer are included unchanged
 # at the beginning of the file. All other rights are reserved.
@@ -29,20 +29,25 @@
     Input Parameters
     ----------------
 
     filename:
         Name of a Numpy np.savez() file containing the following arrays for a
         given SPS models library, like FSPS, Miles, GALEXEV, BPASS,...
 
-        1. templates[npixels, n_ages, n_metals] in erg/cm^2/s/A
-        2. lam[npixels] in Angstroms in common to all the spectra (can be non-uniform)
-        3. fwhm[npixels] or scalar in Angstroms, for the instrumental line-spread function
-        4. ages[n_ages] for the spectra along the 2nd dimension
-        5. metals[n_metals] for the spectra along the 3nd dimension
-        6. masses[n_ages, n_metals] mass of living stars + remnants for each SPS
+        1. templates[npixels, n_ages, n_metals] SPS spectra in units of L_Sun/A
+           (solar luminosities per Angstrom)
+        2. lam[npixels] Wavelength in Angstroms in common to all the spectra
+           (can be non-uniform)
+        3. fwhm[npixels] vector or scalar in Angstroms, for the instrumental
+           line-spread function at every wavelength
+        4. ages[n_ages] for the SPS spectra along the 2nd dimension. These are
+           typically logarithmically spaced, but other choices are possible.
+        5. metals[n_metals] for the SPS spectra along the 3nd dimension
+        6. masses[n_ages, n_metals] mass in solar masses of living stars +
+           remnants for each SPS
 
         This file can be created with a command like::
 
             np.savez_compressed(filename, templates=templates, masses=masses, 
                                 lam=lam, ages=ages, metals=metals, fwhm=fwhm)
 
     velscale:
@@ -57,19 +62,19 @@
         If ``FWHM_gal=None`` (default), no convolution is performed.
 
     Optional Keywords
     -----------------
 
     age_range: array_like with shape (2,)
         ``[age_min, age_max]`` optional age range (inclusive) in Gyr for the 
-        MILES models. This can be useful e.g. to limit the age of the templates 
+        SPS models. This can be useful e.g. to limit the age of the templates 
         to be younger than the age of the Universe at a given redshift.
     metal_range: array_like with shape (2,)
         ``[metal_min, metal_max]`` optional metallicity [M/H] range (inclusive) 
-        for the MILES models (e.g.`` metal_range = [0, np.inf]`` to select only
+        for the SPS models (e.g.`` metal_range = [0, np.inf]`` to select only
         the spectra with Solar metallicity and above).
     norm_range: array_like with shape (2,)
         A two-elements vector specifying the wavelength range in Angstroms 
         within which to compute the templates normalization
         (e.g. ``norm_range=[5070, 5950]`` for the FWHM of the V-band). In this
         case, the output weights will represent light weights.
 
@@ -95,15 +100,15 @@
         However, when using regularization in ``ppxf`` the results will not
         be identical. In fact, enforcing smoothness to the light-weights is
         not quite the same as enforcing it to the mass-weights.
     wave_range: array_like with shape (2,)
         A two-elements vector specifying the wavelength range in Angstroms for
         which to extract the stellar templates. Restricting the wavelength
         range of the templates to the range of the galaxy data is useful to
-        save some computational time. By default ``wave_range=[3541, 1e4]``
+        save some computational time. By default ``wave_range=None``
 
     Output Parameters
     -----------------
 
     Stored as attributes of the ``sps_lib`` class:
 
     .ages_grid: array_like with shape (n_ages, n_metals)
@@ -290,17 +295,15 @@
         dist = (10*units.pc).to('cm').value        
         p1.flux /= 4*np.pi*dist**2            # convert luminosity to observed flux/cm^2 at 10pc
         p1.flux *= constants.L_sun.to('erg/s').value  # spectra are in units of Lsun
 
         ppxf_dir = Path(__file__).parent  # path of current file
         filename = ppxf_dir / 'sps_models' / 'spectra_sun_vega.npz'
         a = np.load(filename)   # Spectrum in cgs/A at 10pc
-        velscale = 1000         # Don't need high resolution for photometry
-        flux_sun, ln_lam, velscale = util.log_rebin(a["lam"], a["flux_sun"], velscale)
-        p2 = util.synthetic_photometry(flux_sun, np.exp(ln_lam), band, 
+        p2 = util.synthetic_photometry(a["flux_sun"], a["lam"], band, 
                                        redshift=redshift, quiet=True) 
 
         mass_weights = weights/self.flux    # Revert possible templates normalization
         lum = p1.flux/p2.flux               # Lum in solar luminosities
         mlpop = np.sum(mass_weights*self.mass_no_gas_grid)/np.sum(weights*lum)
 
         if not quiet:
```

### Comparing `ppxf-9.1.1/ppxf.egg-info/PKG-INFO` & `ppxf-9.2.0/ppxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppxf
-Version: 9.1.1
+Version: 9.2.0
 Summary: pPXF: Full Spectrum and SED Fitting of Galactic and Stellar Spectra
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -1468,22 +1468,39 @@
 redistribute the code.
 
 ###########################################################################
 
 Changelog
 ---------
 
+V9.2.0: MC, Oxford, 10 April 2024
++++++++++++++++++++++++++++++++++
+
+- **Improved** ``sps_util.synthetic_photometry``: Accepts input wavelengths
+  that are not evenly spaced.
+- **Added** ``ppxf_util.mag_spectrum``: A new function to get the apparent
+  magnitude from a spectrum in any photometric band, at any redshift, in either
+  the AB or Vega magnitude system.
+- **Improved** ``ppxf``: Now considers the given ``goodpixels`` when checking
+  that the ``templates`` cover the full ``galaxy`` spectrum, if both ``lam``
+  and ``lam_temp`` are provided.
+- **Fixed** ``ppxf``: Avoids new ``SyntaxWarning`` in Matplotlib LaTeX string
+  in the latest Python 3.12.
+- **Fixed** ``ppxf``: Avoid program stop when passing an input covariance
+  matrix while fitting for gas emission lines. Thanks to Jackson ODonnell
+  (ucsc.edu) for the report.
+
 V9.1.1: MC, Oxford, 18 January 2024
 +++++++++++++++++++++++++++++++++++
 
 - **Improved** ``sps_util.mass_to_light``: Now it can calculate the stellar
   mass-to-light ratio (``M*/L``) for any stellar population synthesis (SPS)
   model, any filter, and any redshift, using the output weights from ``pPXF``.
   No need for pre-computed tables anymore.
-- **Added** ``ppxf_util.solar_mag``: A new function to get the absolute solar
+- **Added** ``ppxf_util.mag_sun``: A new function to get the absolute solar
   magnitude in any photometric band, at any redshift, in either the AB or Vega
   magnitude system.
 
 V9.0.2: MC, Oxford, 30 November 2023
 ++++++++++++++++++++++++++++++++++++
 
 - ``ppxf``: Fixed bug in the automatic truncation of the template wavelength,
```

### Comparing `ppxf-9.1.1/ppxf.egg-info/SOURCES.txt` & `ppxf-9.2.0/ppxf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppxf-9.1.1/setup.py` & `ppxf-9.2.0/setup.py`

 * *Files identical despite different names*

