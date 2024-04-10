# Comparing `tmp/python_cmethods-2.1.0-py3-none-any.whl.zip` & `tmp/python_cmethods-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 39870 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1034 b- defN 24-Mar-10 06:28 cmethods/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Mar-10 06:28 cmethods/_version.py
--rw-r--r--  2.0 unx     6672 b- defN 24-Mar-10 06:28 cmethods/core.py
--rw-r--r--  2.0 unx     9297 b- defN 24-Mar-10 06:28 cmethods/distribution.py
--rw-r--r--  2.0 unx     4700 b- defN 24-Mar-10 06:28 cmethods/scaling.py
--rw-r--r--  2.0 unx      882 b- defN 24-Mar-10 06:28 cmethods/static.py
--rw-r--r--  2.0 unx      499 b- defN 24-Mar-10 06:28 cmethods/types.py
--rw-r--r--  2.0 unx     7369 b- defN 24-Mar-10 06:28 cmethods/utils.py
--rw-r--r--  2.0 unx    32891 b- defN 24-Mar-10 06:28 python_cmethods-2.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    51733 b- defN 24-Mar-10 06:28 python_cmethods-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-10 06:28 python_cmethods-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-10 06:28 python_cmethods-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1031 b- defN 24-Mar-10 06:28 python_cmethods-2.1.0.dist-info/RECORD
-13 files, 116620 bytes uncompressed, 38160 bytes compressed:  67.3%
+Zip file size: 42351 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     4962 b- defN 24-Apr-09 17:35 cmethods/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-09 17:35 cmethods/_version.py
+-rw-r--r--  2.0 unx     6664 b- defN 24-Apr-09 17:35 cmethods/core.py
+-rw-r--r--  2.0 unx     9285 b- defN 24-Apr-09 17:35 cmethods/distribution.py
+-rw-r--r--  2.0 unx     4688 b- defN 24-Apr-09 17:35 cmethods/scaling.py
+-rw-r--r--  2.0 unx      882 b- defN 24-Apr-09 17:35 cmethods/static.py
+-rw-r--r--  2.0 unx      499 b- defN 24-Apr-09 17:35 cmethods/types.py
+-rw-r--r--  2.0 unx     7369 b- defN 24-Apr-09 17:35 cmethods/utils.py
+-rw-r--r--  2.0 unx    32891 b- defN 24-Apr-09 17:35 python_cmethods-2.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    54973 b- defN 24-Apr-09 17:35 python_cmethods-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 17:35 python_cmethods-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 24-Apr-09 17:35 python_cmethods-2.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-09 17:35 python_cmethods-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1134 b- defN 24-Apr-09 17:35 python_cmethods-2.2.0.dist-info/RECORD
+14 files, 123901 bytes uncompressed, 40469 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -18,23 +18,26 @@
 
 Filename: cmethods/types.py
 Comment: 
 
 Filename: cmethods/utils.py
 Comment: 
 
-Filename: python_cmethods-2.1.0.dist-info/LICENSE
+Filename: python_cmethods-2.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: python_cmethods-2.1.0.dist-info/METADATA
+Filename: python_cmethods-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: python_cmethods-2.1.0.dist-info/WHEEL
+Filename: python_cmethods-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: python_cmethods-2.1.0.dist-info/top_level.txt
+Filename: python_cmethods-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: python_cmethods-2.1.0.dist-info/RECORD
+Filename: python_cmethods-2.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: python_cmethods-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmethods/__init__.py

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
+# pylint: disable=consider-using-f-string,logging-not-lazy
 
 r"""
     Module providing the a method named "adjust" to apply different bias
     correction techniques to time-series climate data.
 
     Some variables used in this package:
 
@@ -20,16 +21,174 @@
     F = Cumulative Distribution Function
     \mu = mean
     \sigma = standard deviation
     i = index
     _{m} = long-term monthly interval
 """
 
-from cmethods.core import adjust
+from __future__ import annotations
+
+import logging
+import sys
 
-__author__ = "Benjamin Thomas Schwertfeger"
-__copyright__ = __author__
-__email__ = "contact@b-schwertfeger.de"
-__link__ = "https://github.com/btschwertfeger"
-__github__ = "https://github.com/btschwertfeger/python-cmethods"
+import cloup
+import xarray as xr
+from cloup import (
+    HelpFormatter,
+    HelpTheme,
+    Path,
+    Style,
+    command,
+    option,
+    option_group,
+    version_option,
+)
+from cloup.constraints import Equal, If, require_all
+
+from cmethods.core import adjust
 
 __all__ = ["adjust"]
+
+
+@command(
+    context_settings={
+        "auto_envvar_prefix": "CMETHODS",
+        "help_option_names": ["-h", "--help"],
+    },
+    formatter_settings=HelpFormatter.settings(
+        theme=HelpTheme(
+            invoked_command=Style(fg="bright_yellow"),
+            heading=Style(fg="bright_white", bold=True),
+            constraint=Style(fg="magenta"),
+            col1=Style(fg="bright_yellow"),
+        ),
+    ),
+)
+@version_option(message="%version%")
+@option(
+    "--obs",
+    "--observations",
+    required=True,
+    type=Path(exists=True),
+    help="Reference data set (control period)",
+)
+@option(
+    "--simh",
+    "--simulated-historical",
+    required=True,
+    type=Path(exists=True),
+    help="Modeled data set (control period)",
+)
+@option(
+    "--simp",
+    "--simulated-scenario",
+    required=True,
+    type=Path(exists=True),
+    help="Modeled data set (scenario period)",
+)
+@option(
+    "--method",
+    required=True,
+    type=cloup.Choice(
+        [
+            "linear_scaling",
+            "variance_scaling",
+            "delta_method",
+            "quantile_mapping",
+            "quantile_delta_mapping",
+        ],
+        case_sensitive=False,
+    ),
+    help="Bias adjustment method to apply",
+)
+@option(
+    "--kind",
+    required=True,
+    type=cloup.Choice(["+", "add", "*", "mult"]),
+    help="Kind of adjustment",
+)
+@option(
+    "--variable",
+    required=True,
+    type=str,
+    help="Variable of interest",
+)
+@option(
+    "-o",
+    "--output",
+    required=True,
+    type=str,
+    callback=lambda _, __, value: (value if value.endswith(".nc") else f"{value}.nc"),
+    help="Output file name",
+)
+@option_group(
+    "Scaling-Based Adjustment Options",
+    option(
+        "--group",
+        type=str,
+        help="Temporal grouping",
+    ),
+    constraint=If(
+        Equal("method", "linear_scaling")
+        & Equal("method", "variance_scaling")
+        & Equal("method", "delta_method"),
+        then=require_all,
+    ),
+)
+@option_group(
+    "Distribution-Based Adjustment Options",
+    option(
+        "--quantiles",
+        type=int,
+        help="Quantiles to respect",
+    ),
+    constraint=If(
+        Equal("method", "quantile_mapping") & Equal("method", "quantile_delta_mapping"),
+        then=require_all,
+    ),
+)
+def cli(**kwargs) -> None:
+    """
+    Command-line tool to apply bias correction procedures to climate data.
+
+    Copyright (C) 2023 Benjamin Thomas Schwertfeger\n
+    GitHub: https://github.com/btschwertfeger/python-cmethods
+    """
+
+    logging.basicConfig(
+        format="%(asctime)s %(levelname)8s | %(message)s",
+        datefmt="%Y/%m/%d %H:%M:%S",
+        level=logging.INFO,
+    )
+
+    logging.info("Loading data sets ...")
+    try:
+        for key, message in zip(
+            ("obs", "simh", "simp"),
+            (
+                "observation data set",
+                "modeled data set of the control period",
+                "modeled data set of the scenario period",
+            ),
+        ):
+            kwargs[key] = xr.open_dataset(kwargs[key])
+            if not isinstance(kwargs[key], xr.Dataset):
+                raise TypeError("The data sets must be type xarray.Dataset")
+
+            if kwargs["variable"] not in kwargs[key]:
+                raise KeyError(
+                    f"Variable '{kwargs['variable']}' is missing in the {message}",
+                )
+            kwargs[key] = kwargs[key][kwargs["variable"]]
+    except (TypeError, KeyError) as exc:
+        logging.error(exc)
+        sys.exit(1)
+
+    logging.info("Data sets loaded ...")
+    kwargs["n_quantiles"] = kwargs["quantiles"]
+    del kwargs["quantiles"]
+
+    logging.info("Applying %s ..." % kwargs["method"])
+    result = adjust(**kwargs)
+
+    logging.info("Saving result to %s ..." % kwargs["output"])
+    result.to_netcdf(kwargs["output"])
```

## cmethods/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '2.1.0'
-__version_tuple__ = version_tuple = (2, 1, 0)
+__version__ = version = '2.2.0'
+__version_tuple__ = version_tuple = (2, 2, 0)
```

## cmethods/core.py

```diff
@@ -103,22 +103,22 @@
     **kwargs,
 ) -> XRData:
     """
     Function to apply a bias correction technique on single and multidimensional
     data sets. For more information please refer to the method specific
     requirements and execution examples.
 
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html
 
 
     The time dimension of ``obs``, ``simh`` and ``simp`` must be named ``time``.
 
     If the sizes of time dimensions of the input data sets differ, you have to
     pass the hidden ``input_core_dims`` parameter, see
-    https://python-cmethods.readthedocs.io/en/latest/src/getting_started.html#advanced-usage
+    https://python-cmethods.readthedocs.io/en/latest/getting_started.html#advanced-usage
     for more information.
 
     :param method: Technique to apply
     :type method: str
     :param obs: The reference/observational data set
     :type obs: XRData
     :param simh: The modeled data of the control period
```

## cmethods/distribution.py

```diff
@@ -34,15 +34,15 @@
     simp: NPData,
     n_quantiles: int,
     kind: str = "+",
     **kwargs: Any,
 ) -> np.ndarray:
     r"""
     **Do not call this function directly, please use :func:`cmethods.adjust`**
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html#quantile-mapping
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html#quantile-mapping
     """
     check_adjust_called(
         function_name="quantile_mapping",
         adjust_called=kwargs.get("adjust_called", None),
     )
     check_np_types(obs=obs, simh=simh, simp=simp)
 
@@ -95,15 +95,15 @@
     simh: xr.core.dataarray.DataArray,
     simp: xr.core.dataarray.DataArray,
     n_quantiles: int,
     kind: str = "+",
     **kwargs: Any,
 ) -> NPData:
     r"""
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html#detrended_quantile_mapping
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html#detrended_quantile_mapping
 
     This function can only be applied to 1-dimensional data.
     """
 
     # TODO: this function should also benefit from ufunc -- but how? # pylint: disable=fixme
 
     if kind not in MULTIPLICATIVE and kind not in ADDITIVE:
@@ -213,15 +213,15 @@
     n_quantiles: int,
     kind: str = "+",
     **kwargs: Any,
 ) -> NPData:
     r"""
     **Do not call this function directly, please use :func:`cmethods.adjust`**
 
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html#quantile-delta-mapping
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html#quantile-delta-mapping
     """
     check_adjust_called(
         function_name="quantile_delta_mapping",
         adjust_called=kwargs.get("adjust_called", None),
     )
     check_np_types(obs=obs, simh=simh, simp=simp)
```

## cmethods/scaling.py

```diff
@@ -35,15 +35,15 @@
     simp: NPData,
     kind: str = "+",
     **kwargs: Any,
 ) -> NPData:
     r"""
     **Do not call this function directly, please use :func:`cmethods.adjust`**
 
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html#linear-scaling
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html#linear-scaling
     """
     check_adjust_called(
         function_name="linear_scaling",
         adjust_called=kwargs.get("adjust_called", None),
     )
     check_np_types(obs=obs, simh=simh, simp=simp)
 
@@ -77,15 +77,15 @@
     simp: NPData,
     kind: str = "+",
     **kwargs: Any,
 ) -> NPData:
     r"""
     **Do not call this function directly, please use :func:`cmethods.CMethods.adjust`**
 
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html#variance-scaling
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html#variance-scaling
     """
     check_adjust_called(
         function_name="variance_scaling",
         adjust_called=kwargs.get("adjust_called", None),
     )
     check_np_types(obs=obs, simh=simp, simp=simp)
 
@@ -122,15 +122,15 @@
     simh: NPData,
     simp: NPData,
     kind: str = "+",
     **kwargs: Any,
 ) -> NPData:
     r"""
     **Do not call this function directly, please use :func:`cmethods.adjust`**
-    See https://python-cmethods.readthedocs.io/en/latest/src/methods.html#delta-method
+    See https://python-cmethods.readthedocs.io/en/latest/methods.html#delta-method
     """
     check_adjust_called(
         function_name="delta_method",
         adjust_called=kwargs.get("adjust_called", None),
     )
     check_np_types(obs=obs, simh=simh, simp=simp)
```

## Comparing `python_cmethods-2.1.0.dist-info/LICENSE` & `python_cmethods-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_cmethods-2.1.0.dist-info/METADATA` & `python_cmethods-2.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.1.0
+Version: 2.2.0
 Summary: Collection of bias correction procedures for single and multidimensional climate data
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -656,111 +656,129 @@
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray >=2022.11.0
 Requires-Dist: netCDF4 >=1.6.1
 Requires-Dist: numpy
+Requires-Dist: cloup
 Provides-Extra: dev
-Requires-Dist: pytest ; extra == 'dev'
-Requires-Dist: pytest-cov ; extra == 'dev'
-Requires-Dist: zarr ; extra == 'dev'
-Requires-Dist: dask[distributed] ; extra == 'dev'
-Requires-Dist: scikit-learn ; extra == 'dev'
-Requires-Dist: scipy ; extra == 'dev'
 Requires-Dist: setuptools-scm ; extra == 'dev'
 Requires-Dist: sphinx ; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
-Requires-Dist: ruff ==0.1.13 ; extra == 'dev'
+Requires-Dist: ruff ==0.3.5 ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Provides-Extra: examples
 Requires-Dist: click ; extra == 'examples'
 Requires-Dist: matplotlib ; extra == 'examples'
 Provides-Extra: jupyter
 Requires-Dist: venv-kernel ; extra == 'jupyter'
+Provides-Extra: test
+Requires-Dist: pytest ; extra == 'test'
+Requires-Dist: pytest-cov ; extra == 'test'
+Requires-Dist: zarr ; extra == 'test'
+Requires-Dist: dask[distributed] ; extra == 'test'
+Requires-Dist: scikit-learn ; extra == 'test'
+Requires-Dist: scipy ; extra == 'test'
 
 # python-cmethods
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-cmethods)
 [![Generic badge](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11|_3.12-blue.svg)](https://shields.io/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
 
 [![CI/CD](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/github/btschwertfeger/python-cmethods/branch/master/graph/badge.svg?token=OSO4PAABPD)](https://codecov.io/github/btschwertfeger/python-cmethods)
 
+[![OpenSSF ScoreCard](https://img.shields.io/ossf-scorecard/github.com/btschwertfeger/python-cmethods?label=openssf%20scorecard&style=flat)](https://securityscorecards.dev/viewer/?uri=github.com/btschwertfeger/python-cmethods)
+[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8666/badge)](https://www.bestpractices.dev/projects/8666)
+
 ![release](https://shields.io/github/release-date/btschwertfeger/python-cmethods)
 ![release](https://shields.io/github/v/release/btschwertfeger/python-cmethods?display_name=tag)
 [![DOI](https://zenodo.org/badge/496160109.svg)](https://zenodo.org/badge/latestdoi/496160109)
 [![Documentation Status](https://readthedocs.org/projects/python-cmethods/badge/?version=stable)](https://python-cmethods.readthedocs.io/en/latest/?badge=stable)
 
 </div>
 
-This Python module serves as a collection of different scale- and
-distribution-based bias correction techniques for climate sciences.
-
-The documentation is available at: [https://python-cmethods.readthedocs.io/en/stable/](https://python-cmethods.readthedocs.io/en/stable/)
+Welcome to python-cmethods, a powerful Python package designed for bias
+correction and adjustment of climate data. Built with a focus on ease of use and
+efficiency, python-cmethods offers a comprehensive suite of functions tailored
+for applying bias correction methods to climate model simulations and
+observational datasets via command-line interface and API.
 
 Please cite this project as described in
 https://zenodo.org/doi/10.5281/zenodo.7652755.
 
-> ⚠️ For the application of bias corrections on _large data sets_ it is
-> recommended to also try the command-line tool
-> [BiasAdjustCXX](https://github.com/btschwertfeger/BiasAdjustCXX).
-
----
-
 ## Table of Contents
 
 1. [ About ](#about)
 2. [ Available Methods ](#methods)
 3. [ Installation ](#installation)
 4. [ Usage and Examples ](#examples)
 5. [ Notes ](#notes)
 6. [ Contribution ](#contribution)
 7. [ References ](#references)
 
----
-
 <a name="about"></a>
 
 ## 1. About
 
-These programs and data structures are developed with the aim of reducing
-discrepancies between modeled and observed climate data. Historical data is
-utilized to calibrate variables from current and future time series to achieve
-distributional properties that closely resemble the possible actual values.
+Bias correction in climate research involves the adjustment of systematic errors
+or biases present in climate model simulations or observational datasets to
+improve their accuracy and reliability, ensuring that the data better represents
+actual climate conditions. This process typically involves statistical methods
+or empirical relationships to correct for biases caused by factors such as
+instrument calibration, spatial resolution, or model deficiencies.
 
 <figure>
   <img
   src="doc/_static/images/biasCdiagram.png?raw=true"
   alt="Schematic representation of a bias adjustment procedure"
   style="background-color: white; border-radius: 7px">
   <figcaption>Figure 1: Schematic representation of a bias adjustment procedure</figcaption>
 </figure>
 
-For instance, modeled data typically indicate values that are colder than the
-actual values. To address this issue, an adjustment procedure is employed. The
-figure below illustrates the observed, modeled, and adjusted values, revealing
-that the delta adjusted time series ($T^{*DM}_{sim,p}$) are significantly more
-similar to the observed data ($T{obs,p}$) than the raw modeled data
-($T_{sim,p}$).
+python-cmethods empowers scientists to effectively address those biases in
+climate data, ensuring greater accuracy and reliability in research and
+decision-making processes. By leveraging cutting-edge techniques and seamless
+integration with popular libraries like [xarray](https://xarray.dev/) and
+[Dask](https://docs.dask.org/en/stable/), this package simplifies the process
+of bias adjustment, even when dealing with large-scale climate simulations and
+extensive spatial domains.
+
+In this way, for example, modeled data, which on average represent values that
+are too cold, can be easily bias-corrected by applying any adjustment procedure
+included in this package.
+
+For instance, modeled data can report values that are way colder than the those
+data reported by reanalysis time-series. To address this issue, an adjustment
+procedure can be employed. The figure below illustrates the observed, modeled,
+and adjusted values, revealing that the delta-adjusted time series
+($T^{*DM}_{sim,p}$) is significantly more similar to the observational data
+($T{obs,p}$) than the raw model output ($T_{sim,p}$).
 
 <figure>
   <img
   src="doc/_static/images/dm-doy-plot.png?raw=true"
   alt="Temperature per day of year in modeled, observed and bias-adjusted climate data"
   style="background-color: white; border-radius: 7px">
   <figcaption>Figure 2: Temperature per day of year in observed, modeled, and bias-adjusted climate data</figcaption>
 </figure>
 
+The mathematical foundations supporting each bias correction technique
+implemented in python-cmethods are integral to the package, ensuring
+transparency and reproducibility in the correction process. Each method is
+accompanied by references to trusted publications, reinforcing the reliability
+and rigor of the corrections applied.
+
 <a name="methods"></a>
 
 ## 2. Available Methods
 
 python-cmethods provides the following bias correction techniques:
 
 - Linear Scaling
@@ -774,47 +792,103 @@
 methods as well as sample scripts:
 https://python-cmethods.readthedocs.io/en/stable/
 
 - Except for the variance scaling, all methods can be applied on stochastic and
   non-stochastic climate variables. Variance scaling can only be applied on
   non-stochastic climate variables.
 
-  - Non-stochastic climate variables are those that can be predicted with relative
-    certainty based on factors such as location, elevation, and season. Examples
-    of non-stochastic climate variables include air temperature, air pressure, and
-    solar radiation.
-
-  - Stochastic climate variables, on the other hand, are those that exhibit a high
-    degree of variability and unpredictability, making them difficult to forecast
-    accurately. Precipitation is an example of a stochastic climate variable
-    because it can vary greatly in timing, intensity, and location due to complex
-    atmospheric and meteorological processes.
+  - Non-stochastic climate variables are those that can be predicted with
+    relative certainty based on factors such as location, elevation, and season.
+    Examples of non-stochastic climate variables include air temperature, air
+    pressure, and solar radiation.
+
+  - Stochastic climate variables, on the other hand, are those that exhibit a
+    high degree of variability and unpredictability, making them difficult to
+    forecast accurately. Precipitation is an example of a stochastic climate
+    variable because it can vary greatly in timing, intensity, and location due
+    to complex atmospheric and meteorological processes.
 
 - Except for the detrended quantile mapping (DQM) technique, all methods can be
   applied to 1- and 3-dimensional data sets. The implementation of DQM to
   3-dimensional data is still in progress.
 
 - Except for DQM, all methods can be applied using `cmethods.adjust`. Chunked
   data for computing e.g. in a dask cluster is possible as well.
 
-- For any questions -- please open an issue at https://github.com/btschwertfeger/python-cmethods/issues
+- For any questions -- please open an issue at
+  https://github.com/btschwertfeger/python-cmethods/issues
 
 <a name="installation"></a>
 
 ## 3. Installation
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
----
-
 <a name="examples"></a>
 
-## 4. Usage and Examples
+## 4. CLI Usage
+
+The python-cmethods package provides a command-line interface for applying
+various bias correction methods out of the box.
+
+Keep in mind that due to the various kinds of data and possibilities to
+pre-process those, the CLI only provides a basic application of the implemented
+techniques. For special parameters, adjustments, and data preparation, please
+use programming interface.
+
+Listing the parameters and their requirements is available by passing the
+`--help` option:
+
+```bash
+cmethods --help
+```
+
+Applying the cmethods tool on the provided example data using the linear scaling
+approach is shown below:
+
+```bash
+cmethods \
+  --obs examples/input_data/observations.nc \
+  --simh examples/input_data/control.nc \
+  --simp examples/input_data/scenario.nc \
+  --method linear_scaling \
+  --kind add \
+  --variable tas \
+  --group time.month \
+  --output linear_scaling.nc
+
+2024/04/08 18:11:12     INFO | Loading data sets ...
+2024/04/08 18:11:12     INFO | Data sets loaded ...
+2024/04/08 18:11:12     INFO | Applying linear_scaling ...
+2024/04/08 18:11:15     INFO | Saving result to linear_scaling.nc ...
+```
+
+For applying a distribution-based bias correction technique, the following
+example may help:
+
+```bash
+cmethods \
+  --obs examples/input_data/observations.nc \
+  --simh examples/input_data/control.nc \
+  --simp examples/input_data/scenario.nc \
+  --method quantile_delta_mapping \
+  --kind add \
+  --variable tas \
+  --quantiles 1000 \
+  --output quantile_delta_mapping.nc
+
+2024/04/08 18:16:34     INFO | Loading data sets ...
+2024/04/08 18:16:35     INFO | Data sets loaded ...
+2024/04/08 18:16:35     INFO | Applying quantile_delta_mapping ...
+2024/04/08 18:16:35     INFO | Saving result to quantile_delta_mapping.nc ...
+```
+
+## 5. Programming Interface Usage and Examples
 
 ```python
 import xarray as xr
 from cmethods import adjust
 
 obsh = xr.open_dataset("input_data/observations.nc")
 simh = xr.open_dataset("input_data/control.nc")
@@ -856,16 +930,17 @@
   applied to single and multdimensional data sets by executing the
   `cmethods.adjust` function.
 
 ## Examples (see repository on [GitHub](https://github.com/btschwertfeger/python-cmethods))
 
 Notebook with different methods and plots: `/examples/examples.ipynb`
 
-There is also an example script (`/examples/biasadjust.py`) that can be used to apply the available bias correction methods
-on 1- and 3-dimensional data sets (see `/examples/input_data/*.nc`).
+There is also an example script (`/examples/biasadjust.py`) that can be used to
+apply the available bias correction methods on 1- and 3-dimensional data sets
+(see `/examples/input_data/*.nc`).
 
 Help:
 
 ```bash
 ╰─ python3 biasadjust.py --help
 ```
 
@@ -897,16 +972,14 @@
 
 Notes:
 
 - Data sets must have the same spatial resolutions.
 - This script is far away from perfect - so please see it, as a starting point.
   (:
 
----
-
 <a name="notes"></a>
 
 ## 5. Notes
 
 - Computation in Python takes some time, so this is only for demonstration. When
   adjusting large datasets, you should either use chunked data using for example
   a dask cluster or to apply the command-line tool
@@ -924,16 +997,14 @@
   long-term mean values, but using a 31-day interval, which takes the 31
   surrounding values over all years as the basis for calculating the mean
   values. This is not yet implemented, because even the computation for this
   takes so much time, that it is not worth implementing it in python - but this
   is available in
   [BiasAdjustCXX](https://github.com/btschwertfeger/BiasAdjustCXX).
 
----
-
 <a name="contribution"></a>
 
 ## 6. 🆕 Contributions
 
 … are welcome but:
 
 - First check if there is an existing issue or PR that addresses your
@@ -955,9 +1026,7 @@
 - Quantile and Detrended Quantile Mapping based on: Alex J. Cannon and Stephen R. Sobie and Trevor Q. Murdock _"Bias Correction of GCM Precipitation by Quantile Mapping: How Well Do Methods Preserve Changes in Quantiles and Extremes?"_ (https://doi.org/10.1175/JCLI-D-14-00754.1)
 - Quantile Delta Mapping based on: Tong, Y., Gao, X., Han, Z. et al. _"Bias correction of temperature and precipitation over China for RCM simulations using the QM and QDM methods"_. Clim Dyn 57, 1425–1443 (2021). (https://doi.org/10.1007/s00382-020-05447-4)
 - I'd like to express my gratitude to @riley-brady for initiating and
   contributing to the discussion on
   https://github.com/btschwertfeger/python-cmethods/issues/47. I appreciate all
   the valuable suggestions provided throughout the implementation of the
   subsequent changes.
-
----
```

## Comparing `python_cmethods-2.1.0.dist-info/RECORD` & `python_cmethods-2.2.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-cmethods/__init__.py,sha256=jHnrhGHjbAlUKWhA5v7eQ0rDAVpCFUSbFYtCMtqVsmY,1034
-cmethods/_version.py,sha256=N_eoCB5RSZeFANRJsHZ9FylE5ILLKrp6YmjX8ezqFpA,411
-cmethods/core.py,sha256=tnuaymtGxV9-XNPqu8l6_Qf03WQ9T0vSOZyAbMyrtL4,6672
-cmethods/distribution.py,sha256=nIQNagcibvXw8sI_im08-EmbwOqoa0fStrzhCf5CEh8,9297
-cmethods/scaling.py,sha256=wHzJIZRtmF5xTZ3nULi6fPE8tdnleiDq6KDcUCP9AWk,4700
+cmethods/__init__.py,sha256=mx9-N_JxSHWC4NVCk9ZN6etVMSevaY9v60l3-TnvNxQ,4962
+cmethods/_version.py,sha256=pbL_Q6fDSZl5UbKP04ZFdzrJpd1PO1gH7IwJCwLV7mk,411
+cmethods/core.py,sha256=rjDQouH6-oLYh-DeYrHWByUC7ippkFg03ttq-1VU9Is,6664
+cmethods/distribution.py,sha256=0tQQzP8XIgcNpG2IuH8Wl2j-drYFoGg3B6tmsl4wldY,9285
+cmethods/scaling.py,sha256=jowXipBg4re11w9oaKq4si2wfecwb_Y_XfH_jkR3FEo,4688
 cmethods/static.py,sha256=CyNV8KpwCEH57nzKDb5cJORLAWVL42bb5V6bAK4xRdo,882
 cmethods/types.py,sha256=w-PlDd1fnO6ZCtKrYSE1ekSt5apRAPdli0u3mvMRcOg,499
 cmethods/utils.py,sha256=nEAwe58CfttflZBiX4I1U0k8yRPfykB-dX_EECVBu-0,7369
-python_cmethods-2.1.0.dist-info/LICENSE,sha256=aWDDKEmW35SXvOYO6cDj59glcnidaHqMHQkmKuqo-is,32891
-python_cmethods-2.1.0.dist-info/METADATA,sha256=Kuv7HGB9KOs_LUGuabsq5bxlq3vnkdrqDpq-Jnb9zaI,51733
-python_cmethods-2.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-python_cmethods-2.1.0.dist-info/top_level.txt,sha256=UHtEc5x8YAveY0Wq0ZJdipip7Fh-oZ8M9tnaxxCoaG4,9
-python_cmethods-2.1.0.dist-info/RECORD,,
+python_cmethods-2.2.0.dist-info/LICENSE,sha256=aWDDKEmW35SXvOYO6cDj59glcnidaHqMHQkmKuqo-is,32891
+python_cmethods-2.2.0.dist-info/METADATA,sha256=x6F-InI7iNdf446re6RUHPj918R-jg2NBsETzQnhcUE,54973
+python_cmethods-2.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+python_cmethods-2.2.0.dist-info/entry_points.txt,sha256=jx7BJ_oeDAJptOH725RsfI1qAh4y5sYogHotOXEL9dE,42
+python_cmethods-2.2.0.dist-info/top_level.txt,sha256=UHtEc5x8YAveY0Wq0ZJdipip7Fh-oZ8M9tnaxxCoaG4,9
+python_cmethods-2.2.0.dist-info/RECORD,,
```

