# Comparing `tmp/ms2rescore-3.1.0.dev1.tar.gz` & `tmp/ms2rescore-3.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-3.1.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ms2rescore-3.1.0.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-3.1.0.dev1.tar` & `ms2rescore-3.1.0.dev2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-04-09 13:22:55.220965 ms2rescore-3.1.0.dev1/LICENSE
--rw-r--r--   0        0        0     6477 2024-04-09 13:22:55.220965 ms2rescore-3.1.0.dev1/README.md
--rw-r--r--   0        0        0      458 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/__init__.py
--rw-r--r--   0        0        0     5876 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/__main__.py
--rw-r--r--   0        0        0     5957 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/config_parser.py
--rw-r--r--   0        0        0     9176 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/core.py
--rw-r--r--   0        0        0      633 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/exceptions.py
--rw-r--r--   0        0        0      803 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/__init__.py
--rw-r--r--   0        0        0      522 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/base.py
--rw-r--r--   0        0        0     3436 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/basic.py
--rw-r--r--   0        0        0    10496 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/deeplc.py
--rw-r--r--   0        0        0     6261 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/im2deep.py
--rw-r--r--   0        0        0    10740 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ionmob.py
--rw-r--r--   0        0        0     7069 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/maxquant.py
--rw-r--r--   0        0        0    17272 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ms2pip.py
--rw-r--r--   0        0        0        0 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/__init__.py
--rw-r--r--   0        0        0      419 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/__main__.py
--rw-r--r--   0        0        0    25980 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/app.py
--rw-r--r--   0        0        0    11797 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/function2ctk.py
--rw-r--r--   0        0        0    14890 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/widgets.py
--rw-r--r--   0        0        0        0 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default.json
--rw-r--r--   0        0        0      601 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default_tims.json
--rw-r--r--   0        0        0    12404 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_schema.json
--rw-r--r--   0        0        0        0 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0        0        0 44669194 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0        0        0     4837 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark-white.png
--rw-r--r--   0        0        0     5557 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark.png
--rw-r--r--   0        0        0    52066 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/ms2rescore_logo.png
--rw-r--r--   0        0        0    43034 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0        0        0     5068 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/ms2rescore-gui-theme.json
--rw-r--r--   0        0        0     7974 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/parse_psms.py
--rw-r--r--   0        0        0     1935 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/parse_spectra.py
--rw-r--r--   0        0        0      138 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/__init__.py
--rw-r--r--   0        0        0      614 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/__main__.py
--rw-r--r--   0        0        0    18659 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/charts.py
--rw-r--r--   0        0        0    14785 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/generate.py
--rw-r--r--   0        0        0        0 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/__init__.py
--rw-r--r--   0        0        0     1677 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/about.html
--rw-r--r--   0        0        0     3182 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/base.html
--rw-r--r--   0        0        0      107 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/config.html
--rw-r--r--   0        0        0      138 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/features.html
--rw-r--r--   0        0        0       22 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/log.html
--rw-r--r--   0        0        0      559 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/metadata.html
--rw-r--r--   0        0        0      341 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/overview.html
--rw-r--r--   0        0        0      831 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/stats-card.html
--rw-r--r--   0        0        0     1904 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/style.html
--rw-r--r--   0        0        0      138 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/target-decoy.html
--rw-r--r--   0        0        0     5189 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/texts.toml
--rw-r--r--   0        0        0     2804 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/utils.py
--rw-r--r--   0        0        0      302 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/__init__.py
--rw-r--r--   0        0        0     8749 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/mokapot.py
--rw-r--r--   0        0        0     7869 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/percolator.py
--rw-r--r--   0        0        0     3717 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/utils.py
--rw-r--r--   0        0        0     2680 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 13:42:16.821182 ms2rescore-3.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0     6477 2024-04-10 13:42:16.821182 ms2rescore-3.1.0.dev2/README.md
+-rw-r--r--   0        0        0      458 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     5876 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     5957 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0     9229 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/core.py
+-rw-r--r--   0        0        0      633 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      803 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/base.py
+-rw-r--r--   0        0        0     3436 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/basic.py
+-rw-r--r--   0        0        0    10496 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0     6261 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/im2deep.py
+-rw-r--r--   0        0        0    10740 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ionmob.py
+-rw-r--r--   0        0        0     7069 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    17272 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ms2pip.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/__main__.py
+-rw-r--r--   0        0        0    25980 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/app.py
+-rw-r--r--   0        0        0    11797 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/function2ctk.py
+-rw-r--r--   0        0        0    14890 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/gui/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0      601 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default_tims.json
+-rw-r--r--   0        0        0    12404 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:16.873182 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2024-04-10 13:42:17.029183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     5068 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/package_data/ms2rescore-gui-theme.json
+-rw-r--r--   0        0        0     7974 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/parse_psms.py
+-rw-r--r--   0        0        0     1935 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/parse_spectra.py
+-rw-r--r--   0        0        0      138 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/__main__.py
+-rw-r--r--   0        0        0    18673 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/charts.py
+-rw-r--r--   0        0        0    14787 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/generate.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/__init__.py
+-rw-r--r--   0        0        0     1677 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/about.html
+-rw-r--r--   0        0        0     3182 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/base.html
+-rw-r--r--   0        0        0      107 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/config.html
+-rw-r--r--   0        0        0      138 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/features.html
+-rw-r--r--   0        0        0       22 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/log.html
+-rw-r--r--   0        0        0      559 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/metadata.html
+-rw-r--r--   0        0        0      341 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/overview.html
+-rw-r--r--   0        0        0      831 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/stats-card.html
+-rw-r--r--   0        0        0     1904 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/style.html
+-rw-r--r--   0        0        0      138 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/target-decoy.html
+-rw-r--r--   0        0        0     5189 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/templates/texts.toml
+-rw-r--r--   0        0        0     2804 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/report/utils.py
+-rw-r--r--   0        0        0      302 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     8809 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/mokapot.py
+-rw-r--r--   0        0        0     8207 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     3717 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2680 2024-04-10 13:42:17.033183 ms2rescore-3.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev2/PKG-INFO
```

### Comparing `ms2rescore-3.1.0.dev1/LICENSE` & `ms2rescore-3.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/README.md` & `ms2rescore-3.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/__main__.py` & `ms2rescore-3.1.0.dev2/ms2rescore/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/config_parser.py` & `ms2rescore-3.1.0.dev2/ms2rescore/config_parser.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/core.py` & `ms2rescore-3.1.0.dev2/ms2rescore/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,16 +171,16 @@
 
     # Add missing values
     if rt_required or im_required:
         logger.info("Parsing missing retention time and/or ion mobility values from spectra...")
         get_missing_values(psm_list, config, rt_required=rt_required, im_required=im_required)
 
     # Check if values are now present
-    for value_name in ["retention_time", "ion_mobility"]:
-        if (
+    for value_name, required in [("retention_time", rt_required), ("ion_mobility", im_required)]:
+        if required and (
             0.0 in psm_list[value_name]
             or None in psm_list[value_name]
             or np.isnan(psm_list[value_name]).any()
         ):
             if all(v is None or v == 0.0 or np.isnan(v) for v in psm_list[value_name]):
                 raise exceptions.MissingValuesError(
                     f"Could not find any '{value_name}' values in PSM or spectrum files. Disable "
```

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/exceptions.py` & `ms2rescore-3.1.0.dev2/ms2rescore/exceptions.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/__init__.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/base.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/base.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/basic.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/basic.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/deeplc.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/deeplc.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/im2deep.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/im2deep.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ionmob.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ionmob.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/maxquant.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/maxquant.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ms2pip.py` & `ms2rescore-3.1.0.dev2/ms2rescore/feature_generators/ms2pip.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/gui/app.py` & `ms2rescore-3.1.0.dev2/ms2rescore/gui/app.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/gui/function2ctk.py` & `ms2rescore-3.1.0.dev2/ms2rescore/gui/function2ctk.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/gui/widgets.py` & `ms2rescore-3.1.0.dev2/ms2rescore/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default.json` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default_tims.json` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_default_tims.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/config_schema.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark-white.png` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark.png` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/github-mark.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/ms2rescore_logo.png` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/ms2rescore_logo.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/package_data/ms2rescore-gui-theme.json` & `ms2rescore-3.1.0.dev2/ms2rescore/package_data/ms2rescore-gui-theme.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/parse_psms.py` & `ms2rescore-3.1.0.dev2/ms2rescore/parse_psms.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/parse_spectra.py` & `ms2rescore-3.1.0.dev2/ms2rescore/parse_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/__main__.py` & `ms2rescore-3.1.0.dev2/ms2rescore/report/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/charts.py` & `ms2rescore-3.1.0.dev2/ms2rescore/report/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,28 +369,28 @@
         figure.add_annotation(
             text="No data available for comparison.",
             showarrow=False,
         )
         return figure
 
     levels = before.levels  # ["psms", "peptides", "proteins"] if all available
-    indexers = ["index", "index", "mokapot protein group"]
+    indexers = ["index", "peptide", "mokapot protein group"]
 
     overlap_data = defaultdict(dict)
     for level, indexer in zip(levels, indexers):
         df_before = before.confidence_estimates[level]
         df_after = after.confidence_estimates[level]
         if df_before is None and df_after is None:
             continue
 
         set_before = set(df_before[df_before["mokapot q-value"] <= 0.01][indexer])
         set_after = set(df_after[df_after["mokapot q-value"] <= 0.01][indexer])
 
         overlap_data["removed"][level] = -len(set_before - set_after)
-        overlap_data["retained"][level] = len(set_before | set_after)
+        overlap_data["retained"][level] = len(set_after.intersection(set_before))
         overlap_data["gained"][level] = len(set_after - set_before)
 
     colors = ["#953331", "#316395", "#319545"]
     fig = plotly.subplots.make_subplots(rows=3, cols=1)
 
     for i, level in enumerate(levels):
         for (item, data), color in zip(overlap_data.items(), colors):
```

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/generate.py` & `ms2rescore-3.1.0.dev2/ms2rescore/report/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             continue
         increase = (after - before) / before * 100
         stats.append(
             {
                 "item": level_name,
                 "card_color": card_color,
                 "number": after,
-                "diff": f"{after - before:+}",
+                "diff": f"({after - before:+})",
                 "percentage": f"{increase:.1f}%",
                 "is_increase": increase > 0,
                 "bar_percentage": before / after * 100 if increase > 0 else after / before * 100,
                 "bar_color": "#24a143" if increase > 0 else "#a12424",
             }
         )
     return stats
```

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/about.html` & `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/about.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/base.html` & `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/base.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/metadata.html` & `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/stats-card.html` & `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/stats-card.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/style.html` & `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/style.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/texts.toml` & `ms2rescore-3.1.0.dev2/ms2rescore/report/templates/texts.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/report/utils.py` & `ms2rescore-3.1.0.dev2/ms2rescore/report/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/mokapot.py` & `ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/mokapot.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import pandas as pd
 import psm_utils
 from mokapot.brew import brew
 from mokapot.dataset import LinearPsmDataset
 from pyteomics.mass import nist_mass
 
 logger = logging.getLogger(__name__)
+logging.getLogger("numba").setLevel(logging.WARNING)
 
 
 def rescore(
     psm_list: psm_utils.PSMList,
     output_file_root: str = "ms2rescore",
     fasta_file: Optional[str] = None,
     write_weights: bool = False,
@@ -85,15 +86,15 @@
     # Add proteins
     if fasta_file:
         logger.debug(f"Adding protein info from {fasta_file} with options: `{protein_kwargs}`")
         lin_psm_data.add_proteins(fasta_file, **protein_kwargs)
 
     # Rescore
     logger.debug(f"Mokapot brew options: `{kwargs}`")
-    confidence_results, models = brew(lin_psm_data, **kwargs)
+    confidence_results, models = brew(lin_psm_data, rng=8, **kwargs)
 
     # Reshape confidence estimates to match PSMList
     mokapot_values_targets = (
         confidence_results.confidence_estimates["psms"]
         .set_index("index")
         .sort_index()[["mokapot score", "mokapot q-value", "mokapot PEP"]]
     )
```

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/percolator.py` & `ms2rescore-3.1.0.dev2/ms2rescore/rescoring_engines/percolator.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     `doi:10.1007/s13361-016-1460-7 <https://doi.org/10.1007/s13361-016-1460-7>`_
 
 """
 
 import logging
 import subprocess
 from typing import Any, Dict, Optional
+from copy import deepcopy
 
-import numpy as np
 import psm_utils
 
 from ms2rescore.exceptions import MS2RescoreError
 
 logger = logging.getLogger(__name__)
 
 
@@ -99,16 +99,23 @@
 
     pin_filepath = f"{output_file_root}.pin"
     percolator_cmd = _construct_percolator_command(percolator_kwargs, pin_filepath)
 
     # Need to be able to link back to original PSMs, so reindex spectrum IDs, but copy PSM list
     # to avoid modifying original...
     # TODO: Better approach for this?
-    psm_list_reindexed = psm_list.copy()
-    psm_list_reindexed["spectrum_id"] = np.arange(len(psm_list_reindexed))
+
+    psm_list_reindexed = deepcopy(psm_list)
+    psm_list_reindexed.set_ranks()
+    psm_list_reindexed["spectrum_id"] = [
+        f"{psm.get_usi(as_url=False)}_{psm.rank}" for psm in psm_list_reindexed
+    ]
+    spectrum_id_index = {
+        spectrum_id: index for index, spectrum_id in enumerate(psm_list_reindexed["spectrum_id"])
+    }
 
     _write_pin_file(psm_list_reindexed, pin_filepath)
 
     logger.debug(f"Running percolator command {' '.join(percolator_cmd)}")
     try:
         output = subprocess.run(percolator_cmd, capture_output=True)
     except FileNotFoundError as e:
@@ -130,31 +137,36 @@
         "Percolator output: \n" + _decode_string(output.stderr), extra={"highlighter": None}
     )
 
     _update_psm_scores(
         psm_list,
         percolator_kwargs["results-psms"],
         percolator_kwargs["decoy-results-psms"],
+        spectrum_id_index,
     )
 
 
-def _update_psm_scores(psm_list: psm_utils.PSMList, target_pout: str, decoy_pout: str):
+def _update_psm_scores(
+    psm_list: psm_utils.PSMList, target_pout: str, decoy_pout: str, spectrum_id_index: list
+):
     """
     Update PSM scores with Percolator results.
 
     PSMs from the target and decoy pout files are mapped back by their collection, run,
     spectrum_id, and peptidoform.
 
     """
     target_psms = psm_utils.io.read_file(target_pout, filetype="percolator")
     decoy_psms = psm_utils.io.read_file(decoy_pout, filetype="percolator")
     psm_list_percolator = psm_utils.PSMList(psm_list=target_psms.psm_list + decoy_psms.psm_list)
 
     # Sort by reindexed spectrum_id so order matches original PSM list
-    psm_list_percolator[np.argsort(psm_list_percolator["spectrum_id"])]
+    psm_list_percolator = sorted(
+        psm_list_percolator, key=lambda psm: spectrum_id_index[psm["spectrum_id"]]
+    )
 
     if not len(psm_list) == len(psm_list_percolator):
         raise MS2RescoreError(
             f"Number of PSMs in original list ({len(psm_list)}) does not match number of PSMs in "
             f"Percolator output ({len(psm_list_percolator)})"
         )
```

### Comparing `ms2rescore-3.1.0.dev1/ms2rescore/utils.py` & `ms2rescore-3.1.0.dev2/ms2rescore/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/pyproject.toml` & `ms2rescore-3.1.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.1.0.dev1/PKG-INFO` & `ms2rescore-3.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 3.1.0.dev1
+Version: 3.1.0.dev2
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
 Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
 Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
```

