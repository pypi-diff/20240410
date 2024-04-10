# Comparing `tmp/xlandsat-0.4.0.tar.gz` & `tmp/xlandsat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlandsat-0.4.0.tar", last modified: Fri Sep 29 12:51:25 2023, max compression
+gzip compressed data, was "xlandsat-0.5.0.tar", last modified: Wed Apr 10 12:12:20 2024, max compression
```

## Comparing `xlandsat-0.4.0.tar` & `xlandsat-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 12:51:25.651076 xlandsat-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-09-29 12:51:10.000000 xlandsat-0.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-29 12:51:10.000000 xlandsat-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-09-29 12:51:10.000000 xlandsat-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-09-29 12:51:25.651076 xlandsat-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2023-09-29 12:51:10.000000 xlandsat-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-09-29 12:51:10.000000 xlandsat-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-09-29 12:51:25.655076 xlandsat-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 12:51:25.651076 xlandsat-0.4.0/xlandsat/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/_enhancement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    21007 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/_pansharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    10184 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 12:51:25.651076 xlandsat-0.4.0/xlandsat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2023-09-29 12:51:10.000000 xlandsat-0.4.0/xlandsat/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 12:51:25.651076 xlandsat-0.4.0/xlandsat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 12:51:25.000000 xlandsat-0.4.0/xlandsat.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:20.337389 xlandsat-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 12:11:58.000000 xlandsat-0.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-10 12:11:58.000000 xlandsat-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 12:11:58.000000 xlandsat-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-10 12:12:20.337389 xlandsat-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-10 12:11:58.000000 xlandsat-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-10 12:11:58.000000 xlandsat-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:12:20.337389 xlandsat-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:20.337389 xlandsat-0.5.0/xlandsat/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/_enhancement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21727 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/_pansharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 12:12:20.000000 xlandsat-0.5.0/xlandsat/_version_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:20.337389 xlandsat-0.5.0/xlandsat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-10 12:11:58.000000 xlandsat-0.5.0/xlandsat/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:20.337389 xlandsat-0.5.0/xlandsat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-10 12:12:20.000000 xlandsat-0.5.0/xlandsat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-10 12:12:20.000000 xlandsat-0.5.0/xlandsat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:12:20.000000 xlandsat-0.5.0/xlandsat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 12:12:20.000000 xlandsat-0.5.0/xlandsat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 12:12:20.000000 xlandsat-0.5.0/xlandsat.egg-info/top_level.txt
```

### Comparing `xlandsat-0.4.0/LICENSE.txt` & `xlandsat-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xlandsat-0.4.0/PKG-INFO` & `xlandsat-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: xlandsat
-Version: 0.4.0
-Summary: Load Landsat remote sensing images into xarray
-Home-page: https://github.com/compgeolab/xlandsat
-Author: Leonardo Uieda
-Author-email: leouieda@gmail.com
+Version: 0.5.0
+Summary: Analyze Landsat remote sensing images using xarray
+Author-email: Leonardo Uieda <leo@uieda.com>
 License: MIT License
 Project-URL: Documentation, https://www.compgeolab.org/xlandsat
-Project-URL: Release Notes, https://github.com/compgeolab/xlandsat/releases
+Project-URL: Changelog, https://www.compgeolab.org/xlandsat/latest/changes.html
 Project-URL: Bug Tracker, https://github.com/compgeolab/xlandsat/issues
 Project-URL: Source Code, https://github.com/compgeolab/xlandsat
-Keywords: xarray,remote-sensing,landsat
-Platform: any
-Classifier: Development Status :: 3 - Alpha
+Keywords: xarray,remote sensing,satellite,landsat
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+License-File: AUTHORS.md
 Requires-Dist: numpy>=1.19
 Requires-Dist: scipy>=1.5
 Requires-Dist: xarray>=0.16
 Requires-Dist: scikit-image>=0.18
 Requires-Dist: pooch>=1.3.0
 
 <img src="https://github.com/compgeolab/xlandsat/raw/main/doc/_static/banner.jpg" alt="xlandsat">
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: xlandsat Version: 0.4.0 Summary: Load Landsat
-remote sensing images into xarray Home-page: https://github.com/compgeolab/
-xlandsat Author: Leonardo Uieda Author-email: leouieda@gmail.com License: MIT
-License Project-URL: Documentation, https://www.compgeolab.org/xlandsat
-Project-URL: Release Notes, https://github.com/compgeolab/xlandsat/releases
-Project-URL: Bug Tracker, https://github.com/compgeolab/xlandsat/issues
-Project-URL: Source Code, https://github.com/compgeolab/xlandsat Keywords:
-xarray,remote-sensing,landsat Platform: any Classifier: Development Status :: 3
-- Alpha Classifier: Intended Audience :: Science/Research Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Natural Language :: English Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Software
-Development :: Libraries Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.txt Requires-Dist: numpy>=1.19 Requires-
-Dist: scipy>=1.5 Requires-Dist: xarray>=0.16 Requires-Dist: scikit-image>=0.18
-Requires-Dist: pooch>=1.3.0[xlandsat]
+Metadata-Version: 2.1 Name: xlandsat Version: 0.5.0 Summary: Analyze Landsat
+remote sensing images using xarray Author-email: Leonardo Uieda
+uieda.com> License: MIT License Project-URL: Documentation, https://
+www.compgeolab.org/xlandsat Project-URL: Changelog, https://www.compgeolab.org/
+xlandsat/latest/changes.html Project-URL: Bug Tracker, https://github.com/
+compgeolab/xlandsat/issues Project-URL: Source Code, https://github.com/
+compgeolab/xlandsat Keywords: xarray,remote sensing,satellite,landsat
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Developers Classifier: Intended Audience :: Education Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE.txt License-File: AUTHORS.md Requires-Dist: numpy>=1.19
+Requires-Dist: scipy>=1.5 Requires-Dist: xarray>=0.16 Requires-Dist: scikit-
+image>=0.18 Requires-Dist: pooch>=1.3.0[xlandsat]
               AAnnaallyyzzee LLaannddssaatt rreemmoottee sseennssiinngg iimmaaggeess uussiinngg xxaarrrraayy
    _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_l_a_t_e_s_t_) â¢ _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg_ _(_h_o_w_ _y_o_u_ _c_a_n_ _h_e_l_p_) â¢ _CC_oo_mm_pp_GG_ee_oo_LL_aa_bb
  _[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _P_y_P_I_]_[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _c_o_n_d_a_-_f_o_r_g_e_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _s_t_a_t_u_s_]
              _[_C_o_m_p_a_t_i_b_l_e_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_._]_[_D_O_I_ _u_s_e_d_ _f_o_r_ _c_i_t_a_t_i_o_n_s_]
 ## About **xlandsat** is Python library for loading and analyzing Landsat
 scenes downloaded from [USGS EarthExplorer](https://earthexplorer.usgs.gov)
 with the power of [xarray](https://xarray.dev/). We take care of reading the
```

### Comparing `xlandsat-0.4.0/README.md` & `xlandsat-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `xlandsat-0.4.0/xlandsat/_composite.py` & `xlandsat-0.5.0/xlandsat/_composite.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 Generate and manipulate composites.
 """
 import numpy as np
 import skimage.exposure
 import xarray as xr
 
 
-def composite(scene, bands=("red", "green", "blue"), rescale_to=None):
+def composite(scene, bands=("red", "green", "blue"), rescale_to=None, dtype="uint8"):
     """
     Create a composite using the given bands.
 
     The composite will be an RGBA array if NaNs are present in any band (with
     transparency of the NaN pixels set to full), or RGB is no NaNs are present.
-    The RGB(A) array is encoded as unsigned 8-bit integers for easier plotting
-    with matplotlib and smaller memory footprint.
+    The RGB(A) array is encoded using the given dtype for easier plotting with
+    matplotlib.
 
     Optionally rescale each band to the given range for improved contrast.
 
     Parameters
     ----------
     scene : :class:`xarray.Dataset`
         A Landsat scene, as read with :func:`xlandsat.load_scene`.
@@ -28,14 +28,19 @@
         A list of variable names from the scene that will be used as the
         composite's red, green, and blue channels, respectively.
     rescale_to : None or list
         If not None, then should be a list/tuple with the minimum and maximum
         reflectance ranges to use for rescaling. The same values are used for
         each band. Bands are rescaled separately. Example: ``rescale_to=[0,
         0.5]``. Default is None.
+    dtype : str or numpy dtype
+        The type of the output array. Will determine the range of values in the
+        composite. Float types will result in [-1, 1] range outputs. Default is
+        ``"uint8"`` meaning outputs in [0, 255] range and a smaller memory
+        footprint. Use a float type for higher radiometric precision.
 
     Returns
     -------
     composite : :class:`xarray.DataArray`
         The composite as a 3D ``DataArray`` of type uint8. The first 2
         dimensions are the same as the scene with the ``"channel"`` added as
         third dimension. Metadata from the scene is copied to the composite.
@@ -50,30 +55,34 @@
 
     """
     nrows, ncols = scene[bands[0]].shape
     if np.any((np.isnan(scene[b]) for b in bands)):
         ndim = 4
     else:
         ndim = 3
-    composite = np.empty((nrows, ncols, ndim), dtype="uint8")
+    composite = np.empty((nrows, ncols, ndim), dtype=dtype)
     for i, band in enumerate(bands):
         if rescale_to is None:
             in_range = (np.nanmin(scene[band].values), np.nanmax(scene[band].values))
         else:
             in_range = tuple(rescale_to)
         composite[:, :, i] = skimage.exposure.rescale_intensity(
             scene[band].values,
-            out_range="uint8",
+            out_range=dtype,
             in_range=in_range,
         )
     if ndim == 4:
+        if np.dtype(dtype) == np.uint8:
+            vmax = 255
+        else:
+            vmax = 1
         composite[:, :, 3] = np.where(
             np.any([np.isnan(scene[b]) for b in bands], axis=0),
             0,
-            255,
+            vmax,
         )
     long_name = (
         ", ".join(f"{scene[b].attrs['long_name']}" for b in bands) + " composite"
     )
     name = f"composite_{'_'.join(bands)}"
     coordinates = {"channel": ["red", "green", "blue", "alpha"][:ndim]}
     coordinates.update(scene.coords)
```

### Comparing `xlandsat-0.4.0/xlandsat/_enhancement.py` & `xlandsat-0.5.0/xlandsat/_enhancement.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) 2022 The xlandsat developers.
 # Distributed under the terms of the MIT License.
 # SPDX-License-Identifier: MIT
 """
 Operations to enhance composites. Basically wrappers for skimage.exposure.
 """
+import numpy as np
 import skimage.color
 import skimage.exposure
 
 
 def equalize_histogram(composite, kernel_size=None, clip_limit=0.01):
     """
     Adaptive histogram equalization for a composite
@@ -36,31 +37,79 @@
     clip_limit : float
         Clipping limit, normalized between 0 and 1 (higher values give more
         contrast).
 
     Returns
     -------
     equalized_composite : :class:`xarray.DataArray`
-        The composite after equalization, scaled back to unsigned 8-bit integer
-        range.
+        The composite after equalization, scaled back to the range of the
+        original composite.
 
     Notes
     -----
 
     This function first converts the composite from the RGB color space to the
     `HSV color space <https://en.wikipedia.org/wiki/HSL_and_HSV>`__. Then, it
     applies :func:`skimage.exposure.equalize_adapthist` to the values
     (intensity) channel. Finally, the composite is converted back into the RGB
     color space.
     """
     result = composite.copy(deep=True)
-    hsv = skimage.color.rgb2hsv(result.values[:, :, :3])
+    # Make sure the input is in the 0-255 range for the color space transform
+    hsv = skimage.color.rgb2hsv(
+        skimage.exposure.rescale_intensity(result.values[:, :, :3], out_range="uint8")
+    )
     hsv[:, :, 2] = skimage.exposure.equalize_adapthist(
         hsv[:, :, 2],
         kernel_size=kernel_size,
         clip_limit=clip_limit,
     )
     result.values[:, :, :3] = skimage.exposure.rescale_intensity(
         skimage.color.hsv2rgb(hsv),
-        out_range="uint8",
+        out_range=str(composite.values.dtype),
     )
     return result
+
+
+def adjust_l1_colors(composite, percentile=0.1):
+    """
+    Adjust the colors in an RGB composite from Level 1 data
+
+    Corrects the balance of the red, green, and blue bands in an RGB (true
+    color) composite made from Level 1 data (without atmospheric correction).
+    This is **not as accurate as atmospheric correction** but can lead to nicer
+    images in places where the atmospheric correction causes artifacts.
+
+    **Do not use the output for calculating indices.**
+
+    Parameters
+    ----------
+    composite : :class:`xarray.DataArray`
+        A composite, as generated by :func:`xlandsat.composite`.
+    percentile : float
+        The percentile range to use for the intensity rescaling. Will use the
+        ``percentile`` as the lower bound and ``100 - percentile`` for the
+        upper bound. Default is 0.1%.
+
+    Returns
+    -------
+    adjusted_composite : :class:`xarray.DataArray`
+        The composite after color adjustment, scaled back to the range of the
+        original composite.
+
+    Notes
+    -----
+
+    The correction raises each channel to the power of 1/2.2 (inverse of the
+    sRGB gamma function) and then rescales the transformed intensity to the
+    given percentile range.
+    """
+    output = composite.copy()
+    for i, channel in enumerate(["red", "green", "blue"]):
+        scaled = composite.sel(channel=channel).values ** (1 / 2.2)
+        vmin, vmax = np.percentile(scaled, (percentile, 100 - percentile))
+        output.values[:, :, i] = skimage.exposure.rescale_intensity(
+            scaled,
+            in_range=(vmin, vmax),
+            out_range=str(composite.values.dtype),
+        )
+    return output
```

### Comparing `xlandsat-0.4.0/xlandsat/_interpolation.py` & `xlandsat-0.5.0/xlandsat/_interpolation.py`

 * *Files identical despite different names*

### Comparing `xlandsat-0.4.0/xlandsat/_io.py` & `xlandsat-0.5.0/xlandsat/_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,37 +18,56 @@
     2: "blue",
     3: "green",
     4: "red",
     5: "nir",
     6: "swir1",
     7: "swir2",
     8: "pan",
+    9: "cirrus",
     10: "thermal",
+    11: "thermal2",
 }
 BAND_TITLES = {
     1: "coastal aerosol",
     2: "blue",
     3: "green",
     4: "red",
     5: "near-infrared",
     6: "short-wave infrared 1",
     7: "short-wave infrared 2",
     8: "panchromatic",
+    9: "cirrus",
     10: "thermal",
+    11: "thermal 2",
 }
-BAND_UNITS = {
+BAND_UNITS_L2 = {
     1: "reflectance",
     2: "reflectance",
     3: "reflectance",
     4: "reflectance",
     5: "reflectance",
     6: "reflectance",
     7: "reflectance",
     8: "reflectance",
+    9: "reflectance",
     10: "Kelvin",
+    11: "Kelvin",
+}
+BAND_UNITS_L1 = {
+    1: "reflectance",
+    2: "reflectance",
+    3: "reflectance",
+    4: "reflectance",
+    5: "reflectance",
+    6: "reflectance",
+    7: "reflectance",
+    8: "reflectance",
+    9: "reflectance",
+    10: "radiance",
+    11: "radiance",
 }
 
 
 def load_scene(path, bands=None, region=None, dtype="float16"):
     """
     Load a Landsat scene downloaded from USGS EarthExplorer.
 
@@ -255,43 +274,52 @@
     }
     band_data = raw_data[row_min:row_max, col_min:col_max].astype(dtype)
     del raw_data
     band_data[band_data == 0] = np.nan
     mult, add = scaling_parameters(metadata, number)
     band_data *= mult
     band_data += add
+    if metadata["processing_level"] == "L1TP":
+        units = BAND_UNITS_L1[number]
+    else:
+        units = BAND_UNITS_L2[number]
     band = xr.DataArray(
         data=band_data,
         dims=("northing", "easting"),
         name=BAND_NAMES[number],
         coords=coords,
         attrs={
             "long_name": BAND_TITLES[number],
-            "units": BAND_UNITS[number],
+            "units": units,
             "number": number,
             "filename": pathlib.Path(fname).name,
             "scaling_mult": mult,
             "scaling_add": add,
         },
     )
     return band
 
 
 def scaling_parameters(metadata, number):
     """
     Get the scaling parameters for the band of the given number.
     """
     mult, add = None, None
-    mult_entries = [f"mult_band_{number}", f"mult_band_st_b{number}"]
-    add_entries = [f"add_band_{number}", f"add_band_st_b{number}"]
-    for key in metadata:
-        if any(key.endswith(entry) for entry in mult_entries):
-            mult = metadata[key]
-        if any(key.endswith(entry) for entry in add_entries):
-            add = metadata[key]
+    if number in set(range(1, 10)):
+        mult_entry = f"reflectance_mult_band_{number}"
+        add_entry = f"reflectance_add_band_{number}"
+    else:
+        if metadata["processing_level"] == "L1TP":
+            mult_entry = f"radiance_mult_band_{number}"
+            add_entry = f"radiance_add_band_{number}"
+        else:
+            mult_entry = f"temperature_mult_band_st_b{number}"
+            add_entry = f"temperature_add_band_st_b{number}"
+    mult = metadata[mult_entry]
+    add = metadata[add_entry]
     return mult, add
 
 
 def coordinates_from_metadata(metadata, band_type):
     """
     Generate the UTM pixel coordinate arrays from the metadata.
     """
@@ -391,14 +419,16 @@
         "ROLL_ANGLE",
         "SUN_AZIMUTH",
         "SUN_ELEVATION",
         "EARTH_SUN_DISTANCE",
         "CORNER_",
         "REFLECTANCE_MULT_BAND_",
         "REFLECTANCE_ADD_BAND_",
+        "RADIANCE_MULT_BAND_",
+        "RADIANCE_ADD_BAND_",
         "TEMPERATURE_MULT_BAND_",
         "TEMPERATURE_ADD_BAND_",
     ]
     for item in metadata_raw:
         for field in text_data:
             if item.startswith(field) and field.lower() not in metadata:
                 metadata[field.lower()] = item.split(" = ")[-1].replace('"', "")
```

### Comparing `xlandsat-0.4.0/xlandsat/_pansharpen.py` & `xlandsat-0.5.0/xlandsat/_pansharpen.py`

 * *Files identical despite different names*

### Comparing `xlandsat-0.4.0/xlandsat/datasets.py` & `xlandsat-0.5.0/xlandsat/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,18 @@
         "LC08_L2SP_218074_20190130_20200829_02_T1-cropped.tar.gz": "md5:4ae61a2d7a8b853c727c0c433680cece",
         # Brumadinho - before
         "LC08_L2SP_218074_20190114_20200829_02_T1-cropped.tar.gz": "md5:d2a503c944bb7ef3b41294d44b77e98c",
         # Liverpool
         "LC08_L2SP_204023_20200927_20201006_02_T1-cropped.tar.gz": "md5:3c07e343ccf959be4e5dd5c9aca4e0a4",
         # Liverpool - Panchromatic
         "LC08_L1TP_204023_20200927_20201006_02_T1-cropped.tar.gz": "md5:7d43f8580b8e583d137a93f9ae51a73d",
-        # Momotombo
+        # Momotombo L2
         "LC08_L2SP_017051_20151205_20200908_02_T1-cropped.tar.gz": "md5:8cc2e4c15e65940a7152fc1c8b412aa9",
+        # Momotombo L1
+        "LC08_L1TP_017051_20151205_20200908_02_T1-cropped.tar.gz": "md5:112d42e7adf709ac3a1179bbeedded6d",
         # Roraima
         "LC08_L2SP_232056_20151004_20200908_02_T1-cropped.tar.gz": "md5:f236a8b024aa4a4c62bee294d3bd737f",
         # Manaus
         "LC09_L2SP_231062_20230723_20230802_02_T1-cropped.tar.gz": "md5:ffe2003e665dc7a1a3155011f700a61d",
     },
 )
 
@@ -183,15 +185,15 @@
     """
     return _fetch(
         "LC08_L1TP_204023_20200927_20201006_02_T1-cropped.tar.gz",
         untar,
     )
 
 
-def fetch_momotombo(untar=False):
+def fetch_momotombo(untar=False, level=2):
     """
     Download a sample scene from the December 2015 Momotombo volcano eruption
 
     This is a cropped version of a Landsat 8 scene from 2015/12/05. It was
     taken during the December 2015 eruption of `Momotombo volcano
     <https://en.wikipedia.org/wiki/Momotombo>`__, Nicaragua.
 
@@ -205,24 +207,37 @@
     (`CC0 <https://creativecommons.org/publicdomain/zero/1.0/>`__)
 
     Parameters
     ----------
     untar : bool
         If True, unpack the tar archive after downloading and return a path to
         the folder containing the unpacked files instead. Default is False.
+    level : int
+        Which level of data to load. Default is to load Level 2 surface
+        reflectance data. Can also be Level 1 top-of-the-atmosphere
+        reflectance.
 
     Returns
     -------
     path : str
         The path to the downloaded `.tar` file that contains the scene.
     """
-    return _fetch(
-        "LC08_L2SP_017051_20151205_20200908_02_T1-cropped.tar.gz",
-        untar,
-    )
+    if level not in {1, 2}:
+        raise ValueError(f"Invalid data level '{level}'. Must be 1 or 2.")
+    if level == 2:
+        data = _fetch(
+            "LC08_L2SP_017051_20151205_20200908_02_T1-cropped.tar.gz",
+            untar,
+        )
+    else:
+        data = _fetch(
+            "LC08_L1TP_017051_20151205_20200908_02_T1-cropped.tar.gz",
+            untar,
+        )
+    return data
 
 
 def fetch_roraima(untar=False):
     """
     Download a sample scene from Mount Roraima surrounded by clouds
 
     Roraima is a *tepui* located in the junction of Brazil, Guyana, and
```

### Comparing `xlandsat-0.4.0/xlandsat/tests/test_io.py` & `xlandsat-0.5.0/xlandsat/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xlandsat-0.4.0/xlandsat.egg-info/PKG-INFO` & `xlandsat-0.5.0/xlandsat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: xlandsat
-Version: 0.4.0
-Summary: Load Landsat remote sensing images into xarray
-Home-page: https://github.com/compgeolab/xlandsat
-Author: Leonardo Uieda
-Author-email: leouieda@gmail.com
+Version: 0.5.0
+Summary: Analyze Landsat remote sensing images using xarray
+Author-email: Leonardo Uieda <leo@uieda.com>
 License: MIT License
 Project-URL: Documentation, https://www.compgeolab.org/xlandsat
-Project-URL: Release Notes, https://github.com/compgeolab/xlandsat/releases
+Project-URL: Changelog, https://www.compgeolab.org/xlandsat/latest/changes.html
 Project-URL: Bug Tracker, https://github.com/compgeolab/xlandsat/issues
 Project-URL: Source Code, https://github.com/compgeolab/xlandsat
-Keywords: xarray,remote-sensing,landsat
-Platform: any
-Classifier: Development Status :: 3 - Alpha
+Keywords: xarray,remote sensing,satellite,landsat
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+License-File: AUTHORS.md
 Requires-Dist: numpy>=1.19
 Requires-Dist: scipy>=1.5
 Requires-Dist: xarray>=0.16
 Requires-Dist: scikit-image>=0.18
 Requires-Dist: pooch>=1.3.0
 
 <img src="https://github.com/compgeolab/xlandsat/raw/main/doc/_static/banner.jpg" alt="xlandsat">
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: xlandsat Version: 0.4.0 Summary: Load Landsat
-remote sensing images into xarray Home-page: https://github.com/compgeolab/
-xlandsat Author: Leonardo Uieda Author-email: leouieda@gmail.com License: MIT
-License Project-URL: Documentation, https://www.compgeolab.org/xlandsat
-Project-URL: Release Notes, https://github.com/compgeolab/xlandsat/releases
-Project-URL: Bug Tracker, https://github.com/compgeolab/xlandsat/issues
-Project-URL: Source Code, https://github.com/compgeolab/xlandsat Keywords:
-xarray,remote-sensing,landsat Platform: any Classifier: Development Status :: 3
-- Alpha Classifier: Intended Audience :: Science/Research Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Natural Language :: English Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Software
-Development :: Libraries Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.txt Requires-Dist: numpy>=1.19 Requires-
-Dist: scipy>=1.5 Requires-Dist: xarray>=0.16 Requires-Dist: scikit-image>=0.18
-Requires-Dist: pooch>=1.3.0[xlandsat]
+Metadata-Version: 2.1 Name: xlandsat Version: 0.5.0 Summary: Analyze Landsat
+remote sensing images using xarray Author-email: Leonardo Uieda
+uieda.com> License: MIT License Project-URL: Documentation, https://
+www.compgeolab.org/xlandsat Project-URL: Changelog, https://www.compgeolab.org/
+xlandsat/latest/changes.html Project-URL: Bug Tracker, https://github.com/
+compgeolab/xlandsat/issues Project-URL: Source Code, https://github.com/
+compgeolab/xlandsat Keywords: xarray,remote sensing,satellite,landsat
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Developers Classifier: Intended Audience :: Education Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE.txt License-File: AUTHORS.md Requires-Dist: numpy>=1.19
+Requires-Dist: scipy>=1.5 Requires-Dist: xarray>=0.16 Requires-Dist: scikit-
+image>=0.18 Requires-Dist: pooch>=1.3.0[xlandsat]
               AAnnaallyyzzee LLaannddssaatt rreemmoottee sseennssiinngg iimmaaggeess uussiinngg xxaarrrraayy
    _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_l_a_t_e_s_t_) â¢ _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg_ _(_h_o_w_ _y_o_u_ _c_a_n_ _h_e_l_p_) â¢ _CC_oo_mm_pp_GG_ee_oo_LL_aa_bb
  _[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _P_y_P_I_]_[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _c_o_n_d_a_-_f_o_r_g_e_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _s_t_a_t_u_s_]
              _[_C_o_m_p_a_t_i_b_l_e_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_._]_[_D_O_I_ _u_s_e_d_ _f_o_r_ _c_i_t_a_t_i_o_n_s_]
 ## About **xlandsat** is Python library for loading and analyzing Landsat
 scenes downloaded from [USGS EarthExplorer](https://earthexplorer.usgs.gov)
 with the power of [xarray](https://xarray.dev/). We take care of reading the
```

### Comparing `xlandsat-0.4.0/xlandsat.egg-info/SOURCES.txt` & `xlandsat-0.5.0/xlandsat.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 AUTHORS.md
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 xlandsat/__init__.py
 xlandsat/_composite.py
 xlandsat/_enhancement.py
 xlandsat/_interpolation.py
 xlandsat/_io.py
 xlandsat/_pansharpen.py
 xlandsat/_version.py
 xlandsat/_version_generated.py
 xlandsat/datasets.py
 xlandsat.egg-info/PKG-INFO
 xlandsat.egg-info/SOURCES.txt
 xlandsat.egg-info/dependency_links.txt
 xlandsat.egg-info/requires.txt
 xlandsat.egg-info/top_level.txt
-xlandsat.egg-info/zip-safe
 xlandsat/tests/__init__.py
 xlandsat/tests/test_datasets.py
 xlandsat/tests/test_io.py
```

