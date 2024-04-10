# Comparing `tmp/exspy-0.1.tar.gz` & `tmp/exspy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exspy-0.1.tar", last modified: Sun Dec  3 10:27:57 2023, max compression
+gzip compressed data, was "exspy-0.2.tar", last modified: Wed Apr 10 11:41:31 2024, max compression
```

## Comparing `exspy-0.1.tar` & `exspy-0.2.tar`

### file list

```diff
@@ -1,189 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.990394 exspy-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.962394 exspy-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.962394 exspy-0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-03 10:27:39.000000 exspy-0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-03 10:27:39.000000 exspy-0.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-03 10:27:39.000000 exspy-0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-03 10:27:39.000000 exspy-0.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.962394 exspy-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-03 10:27:39.000000 exspy-0.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-03 10:27:39.000000 exspy-0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-03 10:27:39.000000 exspy-0.1/.github/workflows/package_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-03 10:27:39.000000 exspy-0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-12-03 10:27:39.000000 exspy-0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-03 10:27:39.000000 exspy-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-03 10:27:39.000000 exspy-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-03 10:27:39.000000 exspy-0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-03 10:27:39.000000 exspy-0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2023-12-03 10:27:39.000000 exspy-0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35155 2023-12-03 10:27:39.000000 exspy-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-03 10:27:39.000000 exspy-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44362 2023-12-03 10:27:57.990394 exspy-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-03 10:27:39.000000 exspy-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.966394 exspy-0.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-03 10:27:39.000000 exspy-0.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.966394 exspy-0.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2023-12-03 10:27:39.000000 exspy-0.1/doc/_static/hyperspy.ico
--rw-r--r--   0 runner    (1001) docker     (127)    18979 2023-12-03 10:27:39.000000 exspy-0.1/doc/_static/hyperspy_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-03 10:27:39.000000 exspy-0.1/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-03 10:27:39.000000 exspy-0.1/doc/citing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2023-12-03 10:27:39.000000 exspy-0.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-03 10:27:39.000000 exspy-0.1/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-03 10:27:39.000000 exspy-0.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-12-03 10:27:39.000000 exspy-0.1/doc/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-03 10:27:39.000000 exspy-0.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.966394 exspy-0.1/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-03 10:27:39.000000 exspy-0.1/doc/reference/components.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-03 10:27:39.000000 exspy-0.1/doc/reference/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-03 10:27:39.000000 exspy-0.1/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-03 10:27:39.000000 exspy-0.1/doc/reference/material.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-03 10:27:39.000000 exspy-0.1/doc/reference/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-03 10:27:39.000000 exspy-0.1/doc/reference/signals.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.966394 exspy-0.1/doc/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/dielectric_function.rst
--rw-r--r--   0 runner    (1001) docker     (127)    28277 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/eds.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22071 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/eels.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.970394 exspy-0.1/doc/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    13986 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_background_subtraction.png
--rw-r--r--   0 runner    (1001) docker     (127)    16601 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_energy_axis_gui.png
--rw-r--r--   0 runner    (1001) docker     (127)    48603 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_fitting.png
--rw-r--r--   0 runner    (1001) docker     (127)    71453 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_get_lines_intensity.png
--rw-r--r--   0 runner    (1001) docker     (127)    36511 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_get_lines_intensity_all.png
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_integration_windows.png
--rw-r--r--   0 runner    (1001) docker     (127)    12246 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_microscope_parameters_gui.png
--rw-r--r--   0 runner    (1001) docker     (127)    38376 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_plot_Xray_a.png
--rw-r--r--   0 runner    (1001) docker     (127)    41755 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_plot_Xray_default.png
--rw-r--r--   0 runner    (1001) docker     (127)    29985 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_plot_spectrum.png
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EDS_preferences_gui.png
--rw-r--r--   0 runner    (1001) docker     (127)    33852 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EELS_BN_B_zoomin.png
--rw-r--r--   0 runner    (1001) docker     (127)    50399 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EELS_BN_B_zoomin_with_gaussians.png
--rw-r--r--   0 runner    (1001) docker     (127)    76023 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/EELS_edges_at_energy.png
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/curve_fitting_BN.png
--rw-r--r--   0 runner    (1001) docker     (127)    38996 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/plot_images_eds.png
--rw-r--r--   0 runner    (1001) docker     (127)    99712 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/plot_images_eds_cmap_factors_side_by_side.png
--rw-r--r--   0 runner    (1001) docker     (127)    41975 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/images/plot_images_eds_cmap_list.png
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2023-12-03 10:27:39.000000 exspy-0.1/doc/user_guide/metadata_structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.970394 exspy-0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-03 10:27:39.000000 exspy-0.1/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.970394 exspy-0.1/examples/model_fitting/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-03 10:27:39.000000 exspy-0.1/examples/model_fitting/EELS_curve_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-03 10:27:39.000000 exspy-0.1/examples/model_fitting/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2023-12-03 10:27:39.000000 exspy-0.1/examples/model_fitting/coreloss_spectrum.msa
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2023-12-03 10:27:39.000000 exspy-0.1/examples/model_fitting/lowloss_spectrum.msa
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-03 10:27:39.000000 exspy-0.1/examples/model_fitting/plot_residual.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-03 10:27:39.000000 exspy-0.1/examples/model_fitting/simple_arctan_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.974394 exspy-0.1/exspy/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-12-03 10:27:39.000000 exspy-0.1/exspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2023-12-03 10:27:39.000000 exspy-0.1/exspy/_defaults_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.974394 exspy-0.1/exspy/components/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/eels_arctan.py
--rw-r--r--   0 runner    (1001) docker     (127)    21366 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/eels_cl_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/eels_double_power_law.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/eels_vignetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/pes_core_line_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/pes_see.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/pes_voigt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2023-12-03 10:27:39.000000 exspy-0.1/exspy/components/volume_plasmon_drude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-12-03 10:27:39.000000 exspy-0.1/exspy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.974394 exspy-0.1/exspy/data/
--rw-r--r--   0 runner    (1001) docker     (127)    31008 2023-12-03 10:27:39.000000 exspy-0.1/exspy/data/EDS_SEM_TM002.hspy
--rw-r--r--   0 runner    (1001) docker     (127)    28680 2023-12-03 10:27:39.000000 exspy-0.1/exspy/data/EDS_TEM_FePt_nanoparticles.hspy
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2023-12-03 10:27:39.000000 exspy-0.1/exspy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.974394 exspy-0.1/exspy/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-12-03 10:27:39.000000 exspy-0.1/exspy/docstrings/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-12-03 10:27:39.000000 exspy-0.1/exspy/hyperspy_extension.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.978394 exspy-0.1/exspy/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.978394 exspy-0.1/exspy/misc/eds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eds/eds.py
--rw-r--r--   0 runner    (1001) docker     (127)   764856 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eds/ffast_mac.py
--rw-r--r--   0 runner    (1001) docker     (127)    24412 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.978394 exspy-0.1/exspy/misc/eels/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/base_gos.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/eelsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/effective_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/electron_inelastic_mean_free_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/gosh_gos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/hartree_slater_gos.py
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/hydrogenic_gos.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/eels/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)   373325 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2023-12-03 10:27:39.000000 exspy-0.1/exspy/misc/material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.978394 exspy-0.1/exspy/models/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-03 10:27:39.000000 exspy-0.1/exspy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35925 2023-12-03 10:27:39.000000 exspy-0.1/exspy/models/edsmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-12-03 10:27:39.000000 exspy-0.1/exspy/models/edssemmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-12-03 10:27:39.000000 exspy-0.1/exspy/models/edstemmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    45809 2023-12-03 10:27:39.000000 exspy-0.1/exspy/models/eelsmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signal_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.982394 exspy-0.1/exspy/signals/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signals/dielectric_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    45833 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signals/eds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signals/eds_sem.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40523 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signals/eds_tem.py
--rw-r--r--   0 runner    (1001) docker     (127)    78489 2023-12-03 10:27:39.000000 exspy-0.1/exspy/signals/eels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.982394 exspy-0.1/exspy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.982394 exspy-0.1/exspy/tests/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_EELSarctan.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_ceels_cl_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_double_power_law.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_pes_core_line_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_pes_see.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_pes_voigt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/components/test_volume_plasmon_drude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.982394 exspy-0.1/exspy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/data/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/data/test_eelsdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.982394 exspy-0.1/exspy/tests/drawing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/drawing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.982394 exspy-0.1/exspy/tests/drawing/data/
--rw-r--r--   0 runner    (1001) docker     (127)    26920 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/drawing/data/Cr_L_cl.hspy
--rw-r--r--   0 runner    (1001) docker     (127)    27372 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/drawing/data/Cr_L_ll.hspy
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/drawing/test_plot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/drawing/test_plot_spectra_markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.986394 exspy-0.1/exspy/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/misc/test_eds.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/misc/test_eds_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/misc/test_eels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/misc/test_gos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/misc/test_material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.986394 exspy-0.1/exspy/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/models/test_edsmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    28856 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/models/test_eelsmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/models/test_linear_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.986394 exspy-0.1/exspy/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.986394 exspy-0.1/exspy/tests/signals/data/
--rw-r--r--   0 runner    (1001) docker     (127)   134536 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/data/EELS_LL_linescan_simulated_thickness_variation.hspy
--rw-r--r--   0 runner    (1001) docker     (127)    39332 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/data/EELS_ZLP_linescan_simulated_thickness_variation.hspy
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_assign_subclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (127)    14639 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_edges_range.py
--rw-r--r--   0 runner    (1001) docker     (127)    15199 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_eds_sem.py
--rw-r--r--   0 runner    (1001) docker     (127)    23982 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_eds_tem.py
--rw-r--r--   0 runner    (1001) docker     (127)    23226 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_eels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/signals/test_kramers_kronig_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-12-03 10:27:39.000000 exspy-0.1/exspy/tests/test_non-uniform_not-implemented.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 10:27:57.986394 exspy-0.1/exspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44362 2023-12-03 10:27:57.000000 exspy-0.1/exspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-12-03 10:27:57.000000 exspy-0.1/exspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 10:27:57.000000 exspy-0.1/exspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-03 10:27:57.000000 exspy-0.1/exspy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-12-03 10:27:57.000000 exspy-0.1/exspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-03 10:27:57.000000 exspy-0.1/exspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-03 10:27:39.000000 exspy-0.1/prepare_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2023-12-03 10:27:39.000000 exspy-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-03 10:27:39.000000 exspy-0.1/releasing_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-03 10:27:57.990394 exspy-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.089428 exspy-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.061428 exspy-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.061428 exspy-0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-10 11:41:20.000000 exspy-0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 11:41:20.000000 exspy-0.2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 11:41:20.000000 exspy-0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 11:41:20.000000 exspy-0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 11:41:20.000000 exspy-0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.061428 exspy-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-10 11:41:20.000000 exspy-0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 11:41:20.000000 exspy-0.2/.github/workflows/package_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-10 11:41:20.000000 exspy-0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 11:41:20.000000 exspy-0.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 11:41:20.000000 exspy-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 11:41:20.000000 exspy-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 11:41:20.000000 exspy-0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-10 11:41:20.000000 exspy-0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-10 11:41:20.000000 exspy-0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35155 2024-04-10 11:41:20.000000 exspy-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 11:41:20.000000 exspy-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45125 2024-04-10 11:41:31.089428 exspy-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-10 11:41:20.000000 exspy-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.061428 exspy-0.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 11:41:20.000000 exspy-0.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.061428 exspy-0.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    28401 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-banner-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-banner-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30181 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-banner-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-banner-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18129 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy-logo-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   320411 2024-04-10 11:41:20.000000 exspy-0.2/doc/_static/exspy.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 11:41:20.000000 exspy-0.2/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-10 11:41:20.000000 exspy-0.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 11:41:20.000000 exspy-0.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 11:41:20.000000 exspy-0.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-10 11:41:20.000000 exspy-0.2/doc/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-10 11:41:20.000000 exspy-0.2/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.065428 exspy-0.2/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 11:41:20.000000 exspy-0.2/doc/reference/components.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-10 11:41:20.000000 exspy-0.2/doc/reference/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 11:41:20.000000 exspy-0.2/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-10 11:41:20.000000 exspy-0.2/doc/reference/material.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-10 11:41:20.000000 exspy-0.2/doc/reference/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-10 11:41:20.000000 exspy-0.2/doc/reference/signals.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.065428 exspy-0.2/doc/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/dielectric_function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28277 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/eds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/eels.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.069428 exspy-0.2/doc/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_background_subtraction.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_energy_axis_gui.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48603 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_fitting.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71453 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_get_lines_intensity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36511 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_get_lines_intensity_all.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_integration_windows.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_microscope_parameters_gui.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38376 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_plot_Xray_a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41755 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_plot_Xray_default.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29985 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_plot_spectrum.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EDS_preferences_gui.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33852 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EELS_BN_B_zoomin.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50399 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EELS_BN_B_zoomin_with_gaussians.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76023 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/EELS_edges_at_energy.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/curve_fitting_BN.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38996 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/plot_images_eds.png
+-rw-r--r--   0 runner    (1001) docker     (127)    99712 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/plot_images_eds_cmap_factors_side_by_side.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41975 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/images/plot_images_eds_cmap_list.png
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-10 11:41:20.000000 exspy-0.2/doc/user_guide/metadata_structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.069428 exspy-0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 11:41:20.000000 exspy-0.2/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.069428 exspy-0.2/examples/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 11:41:20.000000 exspy-0.2/examples/model_fitting/EELS_curve_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 11:41:20.000000 exspy-0.2/examples/model_fitting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-04-10 11:41:20.000000 exspy-0.2/examples/model_fitting/coreloss_spectrum.msa
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-04-10 11:41:20.000000 exspy-0.2/examples/model_fitting/lowloss_spectrum.msa
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 11:41:20.000000 exspy-0.2/examples/model_fitting/plot_residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 11:41:20.000000 exspy-0.2/examples/model_fitting/simple_arctan_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.069428 exspy-0.2/exspy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-10 11:41:20.000000 exspy-0.2/exspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-10 11:41:20.000000 exspy-0.2/exspy/_defaults_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.073428 exspy-0.2/exspy/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/eels_arctan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21352 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/eels_cl_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/eels_double_power_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/eels_vignetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/pes_core_line_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/pes_see.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/pes_voigt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-10 11:41:20.000000 exspy-0.2/exspy/components/volume_plasmon_drude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-10 11:41:20.000000 exspy-0.2/exspy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.073428 exspy-0.2/exspy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    31008 2024-04-10 11:41:20.000000 exspy-0.2/exspy/data/EDS_SEM_TM002.hspy
+-rw-r--r--   0 runner    (1001) docker     (127)    28680 2024-04-10 11:41:20.000000 exspy-0.2/exspy/data/EDS_TEM_FePt_nanoparticles.hspy
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-10 11:41:20.000000 exspy-0.2/exspy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.073428 exspy-0.2/exspy/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-10 11:41:20.000000 exspy-0.2/exspy/docstrings/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-10 11:41:20.000000 exspy-0.2/exspy/hyperspy_extension.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.073428 exspy-0.2/exspy/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.077428 exspy-0.2/exspy/misc/eds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eds/eds.py
+-rw-r--r--   0 runner    (1001) docker     (127)   764868 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eds/ffast_mac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24470 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.077428 exspy-0.2/exspy/misc/eels/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/base_gos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12489 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/eelsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/effective_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/electron_inelastic_mean_free_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/gosh_gos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/hartree_slater_gos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/hydrogenic_gos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/eels/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201058 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-10 11:41:20.000000 exspy-0.2/exspy/misc/material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.077428 exspy-0.2/exspy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-10 11:41:20.000000 exspy-0.2/exspy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-04-10 11:41:20.000000 exspy-0.2/exspy/models/edsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-10 11:41:20.000000 exspy-0.2/exspy/models/edssemmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-10 11:41:20.000000 exspy-0.2/exspy/models/edstemmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45809 2024-04-10 11:41:20.000000 exspy-0.2/exspy/models/eelsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signal_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.077428 exspy-0.2/exspy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signals/dielectric_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45515 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signals/eds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signals/eds_sem.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40507 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signals/eds_tem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78337 2024-04-10 11:41:20.000000 exspy-0.2/exspy/signals/eels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.081428 exspy-0.2/exspy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.081428 exspy-0.2/exspy/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/coreloss_spectrum.msa
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/lowloss_spectrum.msa
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_EELSarctan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_double_power_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_eels_cl_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_pes_core_line_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_pes_see.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_pes_voigt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/components/test_volume_plasmon_drude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.081428 exspy-0.2/exspy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/data/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/data/test_eelsdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.081428 exspy-0.2/exspy/tests/drawing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/drawing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.081428 exspy-0.2/exspy/tests/drawing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    26920 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/drawing/data/Cr_L_cl.hspy
+-rw-r--r--   0 runner    (1001) docker     (127)    27372 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/drawing/data/Cr_L_ll.hspy
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/drawing/test_plot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/drawing/test_plot_spectra_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.081428 exspy-0.2/exspy/tests/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/misc/test_eds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/misc/test_eds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/misc/test_eels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/misc/test_gos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/misc/test_material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.085428 exspy-0.2/exspy/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/models/test_edsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28757 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/models/test_eelsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/models/test_linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.085428 exspy-0.2/exspy/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.085428 exspy-0.2/exspy/tests/signals/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   134536 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/data/EELS_LL_linescan_simulated_thickness_variation.hspy
+-rw-r--r--   0 runner    (1001) docker     (127)    39332 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/data/EELS_ZLP_linescan_simulated_thickness_variation.hspy
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_assign_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_edges_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_eds_sem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_eds_tem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23290 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_eels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/signals/test_kramers_kronig_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-10 11:41:20.000000 exspy-0.2/exspy/tests/test_non-uniform_not-implemented.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.085428 exspy-0.2/exspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45125 2024-04-10 11:41:31.000000 exspy-0.2/exspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-10 11:41:31.000000 exspy-0.2/exspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:41:31.000000 exspy-0.2/exspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 11:41:31.000000 exspy-0.2/exspy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 11:41:31.000000 exspy-0.2/exspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 11:41:31.000000 exspy-0.2/exspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-10 11:41:20.000000 exspy-0.2/prepare_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 11:41:20.000000 exspy-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-10 11:41:20.000000 exspy-0.2/releasing_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:41:31.089428 exspy-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:41:31.085428 exspy-0.2/upcoming_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-10 11:41:20.000000 exspy-0.2/upcoming_changes/README.rst
```

### Comparing `exspy-0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `exspy-0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 Minimum working example of code
 ```
 
 #### Expected behavior
 A clear and concise description of what you expected to happen.
 
 #### Python environement:
- - exSpy version: 0.x.x
+ - eXSpy version: 0.x.x
  - HyperSpy version: 1.x.x
  - Python version: 3.x
 
 #### Additional context
 Add any other context about the problem here. If necessary, add screenshots to help explain your problem.
```

### Comparing `exspy-0.1/.github/PULL_REQUEST_TEMPLATE.md` & `exspy-0.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `exspy-0.1/.github/workflows/docs.yml` & `exspy-0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `exspy-0.1/.github/workflows/release.yml` & `exspy-0.2/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     runs-on: ubuntu-latest
     name: Upload to pypi
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
     - name: Download dist
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
 
     - name: Display downloaded files
       run: |
         ls -shR
       working-directory: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
@@ -48,8 +48,8 @@
     name: Create GitHub Release
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
       - name: Create Release
         if: ${{ startsWith(github.ref, 'refs/tags/') && github.repository_owner == 'hyperspy' }}
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564
```

### Comparing `exspy-0.1/.github/workflows/tests.yml` & `exspy-0.2/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             PYTHON_VERSION: '3.8'
           - os: ubuntu
             PYTHON_VERSION: '3.10'
           - os: ubuntu
             PYTHON_VERSION: '3.12'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: get repository name
         shell: bash
         run: echo "REPOSITORY_NAME=${GITHUB_REPOSITORY#*/}" >> $GITHUB_ENV
 
@@ -36,15 +36,15 @@
         if: ${{ github.repository_owner != 'hyperspy' }}
         # Needs to fetch the tags from upstream to get the
         # correct version with setuptools_scm
         run: |
           git remote add upstream https://github.com/hyperspy/${{ env.REPOSITORY_NAME }}.git
           git fetch upstream --tags
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: ${{ matrix.PYTHON_VERSION }}
 
       - name: Display version
         run: |
           python --version
@@ -60,10 +60,10 @@
 
       - name: Run test suite
         run: |
           pytest --pyargs exspy -n 2 --cov=. --cov-report=xml
 
       - name: Upload coverage to Codecov
         if: ${{ always() }}
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `exspy-0.1/.readthedocs.yaml` & `exspy-0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `exspy-0.1/CHANGES.rst` & `exspy-0.2/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,37 @@
 https://exspy.readthedocs.io/en/latest/changes.html
 
 
 .. towncrier-draft-entries:: |release| [UNRELEASED]
 
 .. towncrier release notes start
 
+0.2 (2024-04-10)
+================
+
+Bug Fixes
+---------
+
+- Fix restoring Gosh and Hartree Slater GOS from stored models. (`#32 <https://github.com/hyperspy/exspy/issues/32>`_)
+
+
+Improved Documentation
+----------------------
+
+- Add eXSpy logo and adapt spelling to capital X (`#22 <https://github.com/hyperspy/exspy/issues/22>`_)
+- Fix DOI and add more badges to readme file. (`#36 <https://github.com/hyperspy/exspy/issues/36>`_, `#38 <https://github.com/hyperspy/exspy/issues/38>`_)
+
+
+Maintenance
+-----------
+
+- Use `ruff <https://docs.astral.sh/ruff>`_ for linting and formatting the code. Remove redundant GitHub workflow in favour of pre-commit. (`#27 <https://github.com/hyperspy/exspy/issues/27>`_)
+- Fix deprecation scipy and numpy warnings. (`#33 <https://github.com/hyperspy/exspy/issues/33>`_)
+
+
 0.1 (2023-12-03)
 ================
 
 New features
 ------------
 - Support for tabulated :ref:`Generalised Oscillator Strengths (GOS) <eels.GOS>` using the
   `GOSH <https://gitlab.com/gguzzina/gosh>`_ open file format. By default, a freely
@@ -35,12 +58,12 @@
 - Add package and test workflow (`#10 <https://github.com/hyperspy/exspy/pull/10>`_)
 - Add python 3.12 (`#10 <https://github.com/hyperspy/exspy/pull/10>`_)
 - Add release workflow (`#10 <https://github.com/hyperspy/exspy/pull/10>`_)
 
 Initiation (2023-10-28)
 =======================
 
-- exSpy was split out of the `HyperSpy repository
+- eXSpy was split out of the `HyperSpy repository
   <https://github.com/hyperspy/hyperspy>`_ on Oct. 28, 2023. The X-ray energy
   dispersive spectroscopy (EDS) and energy electron loss spectroscopy (EELS)
   functionalities so far developed in HyperSpy were moved to the
-  `exSpy repository <https://github.com/hyperspy/exspy>`_.
+  `eXSpy repository <https://github.com/hyperspy/exspy>`_.
```

### Comparing `exspy-0.1/CONTRIBUTING.rst` & `exspy-0.2/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _contributing_label:
 
 Contributing
 ************
 
-exSpy is meant to be a community maintained project. We welcome contributions
+eXSpy is meant to be a community maintained project. We welcome contributions
 in the form of bug reports, documentation, code, feature requests, and more.
 In the following we refer to some resources to help you make useful contributions.
 
 Issues
 ======
 
 The `issue tracker <https://github.com/hyperspy/exspy/issues>`_ can be used to
@@ -16,15 +16,15 @@
 
 - give a minimal example demonstrating the bug,
 - copy and paste the error traceback.
 
 Pull Requests
 =============
 
-If you want to contribute to the exSpy source code, you can send us a
+If you want to contribute to the eXSpy source code, you can send us a
 `pull request <https://github.com/hyperspy/exspy/pulls>`_. Small bug fixes or
 corrections to the user guide are typically a good starting point. But don't
 hesitate also for significant code contributions - if needed, we'll help you
 to get the code ready to common standards.
 
 Please refer to the
 `HyperSpy developer guide <http://hyperspy.org/hyperspy-doc/current/dev_guide/intro.html>`_
@@ -40,35 +40,35 @@
 As quality assurance, to improve the code, and to ensure a generalized
 functionality, pull requests need to be thoroughly reviewed by at least one
 other member of the development team before being merged.
 
 Documentation
 =============
 
-The exSpy documentation consists of three elements:
+The eXSpy documentation consists of three elements:
 
 - Docstrings following the `numpy standard
   <https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard>`_
   that document the functionality of individual methods on `GitHub
   <https://github.com/hyperspy/exspy>`_.
 - The `documentation <https://exspy.readthedocs.io>`_ written using `Sphinx
   <https://www.sphinx-doc.org>`_ and hosted on `Read the Docs
   <https://exspy.readthedocs.io>`_. The source is part of the `GitHub repository
   <https://github.com/hyperspy/exspy/tree/main/doc>`_.
-- Jupyter notebooks in the `exSpy demos repository
+- Jupyter notebooks in the `eXSpy demos repository
   <https://github.com/hyperspy/exspy-demos>`_ on GitHub that provide tutorials and example
   workflows.
 
 Improving documentation is always welcome and a good way of starting out to learn the GitHub
 functionality. You can contribute through pull requests to the respective repositories.
 
 Code style
 ==========
 
-exSpy follows `Style Guide for Python Code <https://www.python.org/dev/peps/pep-0008/>`_
+eXSpy follows `Style Guide for Python Code <https://www.python.org/dev/peps/pep-0008/>`_
 with `The Black Code style
 <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_.
 
 For `docstrings <https://www.python.org/dev/peps/pep-0257/>`_, we follow the `numpydoc
 <https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard>`_ standard.
 
 Package imports should be structured into three blocks with blank lines between
@@ -77,25 +77,25 @@
 - standard libraries (like ``os`` and ``typing``),
 - third party packages (like ``numpy`` and ``hyperspy``),
 - and finally ``exspy`` imports.
 
 Writing tests
 =============
 
-All functionality in exSpy is tested via the `pytest <https://docs.pytest.org>`_
+All functionality in eXSpy is tested via the `pytest <https://docs.pytest.org>`_
 framework. The tests reside in the ``test`` directory. Tests are short methods that call
-functions in exSpy and compare resulting output values with known answers.
+functions in eXSpy and compare resulting output values with known answers.
 Please refer to the `HyperSpy development guide
 <https://hyperspy.org/hyperspy-doc/current/dev_guide/testing.html>`_ for further
 information on tests.
 
 Releasing a new version
 =======================
 
-exSpy versioning follows `semantic versioning <https://semver.org/spec/v2.0.0.html>`_
+eXSpy versioning follows `semantic versioning <https://semver.org/spec/v2.0.0.html>`_
 and the version number is therefore a three-part number: MAJOR.MINOR.PATCH.
 Each number will change depending on the type of changes according to the following:
 
 - MAJOR increases when making incompatible API changes,
 - MINOR increases when adding functionality in a backwards compatible manner, and
 - PATCH increases when making backwards compatible bug fixes.
```

### Comparing `exspy-0.1/LICENSE` & `exspy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exspy-0.1/PKG-INFO` & `exspy-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exspy
-Version: 0.1
+Version: 0.2
 Summary: EELS and EDS analysis with the HyperSpy framework
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,31 +676,28 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <http://www.gnu.org/philosophy/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://hyperspy.org/exspy
 Project-URL: Bug Reports, https://github.com/hyperspy/exspy/issues
 Project-URL: Source, https://github.com/hyperspy/exspy
-Keywords: data analysis,microscopy,electron microscopy,electron energy loss spectroscopy,X-ray energy-dispersive spectroscopy
+Keywords: python,hyperspy,data analysis,microscopy,electron microscopy,electron energy loss spectroscopy,energy-dispersive X-ray spectroscopy,X-ray energy-dispersive spectroscopy,EELS,EDS,EDX,SEM,STEM,TEM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask[array]
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: matplotlib
 Requires-Dist: numexpr
@@ -737,22 +734,30 @@
 Requires-Dist: exspy[gui-jupyter]; extra == "all"
 Requires-Dist: exspy[gui-traitsui]; extra == "all"
 
 
 [![Tests](https://github.com/hyperspy/exspy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/exspy/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/exspy/badge/?version=latest)](https://exspy.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/hyperspy/exspy/graph/badge.svg?token=X7T3LE121Q)](https://codecov.io/gh/hyperspy/exspy)
+[![CodeQL](https://github.com/hyperspy/exspy/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/hyperspy/exspy/actions/workflows/github-code-scanning/codeql)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hyperspy/exspy/main.svg)](https://results.pre-commit.ci/latest/github/hyperspy/exspy/main)
+
+
+[![Python Version](https://img.shields.io/pypi/pyversions/exspy.svg?style=flat)](https://pypi.python.org/pypi/exspy)
+[![PyPi Version](http://img.shields.io/pypi/v/exspy.svg?style=flat)](https://pypi.python.org/pypi/exspy)
+[![Anaconda Version](https://anaconda.org/conda-forge/exspy/badges/version.svg)](https://anaconda.org/conda-forge/exspy)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.10252344.svg)](https://zenodo.org/doi/10.5281/zenodo.10252344)
 
-**exSpy** is a Python package extending the functionality for multi-dimensional
+**eXSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of X-rays Energy Dispersive Spectroscopy (EDS)
 and Electron Energy Loss Spectroscopy (EELS).
 
-Go to the documentation for instructions on how to install exSpy and start an
+Go to the documentation for instructions on how to install eXSpy and start an
 analysis: [Read the docs](https://exspy.readthedocs.io).
 
 Everyone is welcome to contribute. Please read our
 [contributing guidelines](https://github.com/hyperspy/exspy/blob/main/CONTRIBUTING.rst) and get started!
 
-Development of exSpy is documented in the
+Development of eXSpy is documented in the
 [changelog](https://github.com/hyperspy/exspy/blob/main/CHANGES.rst).
```

### Comparing `exspy-0.1/doc/Makefile` & `exspy-0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/conf.py` & `exspy-0.2/doc/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 import hyperspy.api as hs
-import logging
 import numpydoc
 from packaging.version import Version
 
 
 # Set logging level to `ERROR` to avoid exspy warning in documentation
 hs.set_log_level("ERROR")
 
 
 # -- Project information -----------------------------------------------------
 
-project = "exSpy"
-copyright = "2023, exSpy Developers"
-author = "exSpy Developers"
+project = "eXSpy"
+copyright = "2023, eSpy Developers"
+author = "eXSpy Developers"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -101,28 +100,26 @@
         {
             "name": "Gitter",
             "url": "https://gitter.im/hyperspy/hyperspy",
             "icon": "fab fa-gitter",
         },
     ],
     "logo": {
-        "text": "exSpy",
+        "alt_text": "eXSpy",
+        "image_light": "_static/exspy-banner-light.svg",
+        "image_dark": "_static/exspy-banner-dark.svg",
     },
     "header_links_before_dropdown": 6,
     "navigation_with_keys": False,
 }
 
-# The name of an image file (relative to this directory) to place at the top
-# of the sidebar.
-html_logo = "_static/hyperspy_logo.png"
-
 # -- Options for sphinx_favicon extension -----------------------------------
 
 favicons = [
-    "hyperspy.ico",
+    "exspy.ico",
 ]
 
 # Check links to API when building documentation
 nitpicky = False
 # Remove when fixed in hyperspy
 nitpick_ignore_regex = [(r"py:.*", r"hyperspy.api.*")]
```

### Comparing `exspy-0.1/doc/intro.rst` & `exspy-0.2/doc/intro.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Welcome to exSpy's documentation!
-***********************************
-**exSpy** is a Python package extending the functionality for multi-dimensional
+Welcome to the documentation of eXSpy!
+**************************************
+**eXSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the `HyperSpy <https://hyperspy.org/>`_ library. It is
 aimed at helping with the analysis of X-rays Energy Dispersive Spectroscopy (EDS)
 and Electron Energy Loss Spectroscopy (EELS).
 
 Check out the :ref:`installation <install-label>` section for further information,
 including how to start using this project.
 
@@ -23,99 +23,103 @@
   .. grid-item-card::
     :link: user_guide/install
     :link-type: doc
 
     :octicon:`rocket;2em;sd-text-info` Getting Started
     ^^^
 
-    New to HyperSpy or Python? The getting started guide provides an
-    introduction on basic usage of HyperSpy and how to install it.
+    New to eXSpy or the HyperSpy ecosystem? The getting started guide provides an
+    introduction on basic usage of eXSpy and how to install it.
 
   .. grid-item-card::
     :link: user_guide/index
     :link-type: doc
 
     :octicon:`book;2em;sd-text-info` User Guide
     ^^^
 
-    The user guide provides in-depth information on key concepts of HyperSpy
+    The user guide provides in-depth information on key concepts of eXSpy
     and how to use it along with background information and explanations.
 
   .. grid-item-card::
     :link: reference/index
     :link-type: doc
 
     :octicon:`code-square;2em;sd-text-info` Reference
     ^^^
 
     Documentation of the metadata specification and of the Application Progamming Interface (API),
-    which describe how HyperSpy functions work and which parameters can be used.
+    which describe how eXSpy functions work and which parameters can be used.
 
   .. grid-item-card::
     :link: auto_examples/index
     :link-type: doc
 
     :octicon:`zap;2em;sd-text-info` Example
     ^^^
 
-    Short examples illustrating simple tasks.
+    Gallery of short examples illustrating simple tasks that
+    can be performed with eXSpy and HyperSpy.
 
   .. grid-item-card::
     :link: https://github.com/hyperspy/exspy-demos
 
     :octicon:`workflow;2em;sd-text-info` Tutorials
     ^^^
 
-    Tutorials in form of Jupyter Notebooks to learn how to
-    process multi-dimensional data using HyperSpy.
+    Tutorials in form of Jupyter Notebooks to learn how to process
+    multi-dimensional electron/X-ray spectroscopy data using eXSpy.
 
   .. grid-item-card::
     :link: contributing
     :link-type: doc
 
     :octicon:`people;2em;sd-text-info` Contributing
     ^^^
 
-    HyperSpy is a community project maintained for and by its users.
-    There are many ways you can help!
+    eXSpy and the whole HyperSpy ecosystem are a community project
+    maintained for and by its users. There are many ways you can help!
 
-Citing exSpy
+Citing eXSpy
 ============
 
-If exSpy has been significant to a project that leads to an academic
+If eXSpy has been significant to a project that leads to an academic
 publication, please acknowledge that fact by citing it. The DOI in the
 badge below is the `Concept DOI <https://help.zenodo.org/faq/#versioning>`_ of
-HyperSpy. It can be used to cite the project without referring to a specific
-version. If you are citing exSpy because you have used it to process data,
+eXSpy. It can be used to cite the project without referring to a specific
+version. If you are citing eXSpy because you have used it to process data,
 please use the DOI of the specific version that you have employed. You can
 find it by clicking on the DOI badge below.
 
-.. image:: https://zenodo.org/badge/doi/10.5281/zenodo.592838.svg
-   :target: https://doi.org/10.5281/zenodo.592838
+.. image:: https://zenodo.org/badge/doi/10.5281/zenodo.10252344.svg
+   :class: sd-bg-transparent
+   :alt: doi: 10.5281/zenodo.10252344
+   :target: https://zenodo.org/doi/10.5281/zenodo.10252344
 
-HyperSpy's citation in the scientific literature
+Citation in the scientific literature
 ------------------------------------------------
 
-Given the increasing number of articles that cite HyperSpy we do not maintain a list of
-articles citing HyperSpy. For an up to date list search for
-HyperSpy in a scientific database e.g. `Google Scholar
+Given the increasing number of articles that cite HyperSpy and its extension
+packages, we do not maintain a list of
+articles citing eXSpy or HyperSpy. For an up to date list search for
+exspy/HyperSpy in a scientific database e.g. `Google Scholar
 <https://scholar.google.co.uk/scholar?q=hyperspy>`_.
 
 .. Warning::
     Articles published before 2012 may mention the HyperSpy project under
     its old name, `EELSLab`.
 
 
 License
 =======
 
-**exSpy** is free software: you can redistribute it and/or modify
+**eXSpy** is free software: you can redistribute it and/or modify
 it under the terms of the `GNU General Public License (GPL)
 <https://www.gnu.org/licenses/#GPL>`_ as published by
 the Free Software Foundation, either version 3 of the license, or
 (at your option) any later version.
 
-**exSpy** is distributed in the hope that it will be useful,
+**eXSpy** is distributed in the hope that it will be useful,
 but **without any warranty**; without even the implied warranty of
 **merchantability** or **fitness for a particular purpose**. See the
 `GNU General Public License <https://www.gnu.org/licenses/#GPL>`_
 for more details.
```

### Comparing `exspy-0.1/doc/make.bat` & `exspy-0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/bibliography.rst` & `exspy-0.2/doc/user_guide/bibliography.rst`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/dielectric_function.rst` & `exspy-0.2/doc/user_guide/dielectric_function.rst`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/eds.rst` & `exspy-0.2/doc/user_guide/eds.rst`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/eels.rst` & `exspy-0.2/doc/user_guide/eels.rst`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_background_subtraction.png` & `exspy-0.2/doc/user_guide/images/EDS_background_subtraction.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_energy_axis_gui.png` & `exspy-0.2/doc/user_guide/images/EDS_energy_axis_gui.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_fitting.png` & `exspy-0.2/doc/user_guide/images/EDS_fitting.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_get_lines_intensity.png` & `exspy-0.2/doc/user_guide/images/EDS_get_lines_intensity.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_get_lines_intensity_all.png` & `exspy-0.2/doc/user_guide/images/EDS_get_lines_intensity_all.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_integration_windows.png` & `exspy-0.2/doc/user_guide/images/EDS_integration_windows.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_microscope_parameters_gui.png` & `exspy-0.2/doc/user_guide/images/EDS_microscope_parameters_gui.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_plot_Xray_a.png` & `exspy-0.2/doc/user_guide/images/EDS_plot_Xray_a.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_plot_Xray_default.png` & `exspy-0.2/doc/user_guide/images/EDS_plot_Xray_default.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_plot_spectrum.png` & `exspy-0.2/doc/user_guide/images/EDS_plot_spectrum.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EDS_preferences_gui.png` & `exspy-0.2/doc/user_guide/images/EDS_preferences_gui.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EELS_BN_B_zoomin.png` & `exspy-0.2/doc/user_guide/images/EELS_BN_B_zoomin.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EELS_BN_B_zoomin_with_gaussians.png` & `exspy-0.2/doc/user_guide/images/EELS_BN_B_zoomin_with_gaussians.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/EELS_edges_at_energy.png` & `exspy-0.2/doc/user_guide/images/EELS_edges_at_energy.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/curve_fitting_BN.png` & `exspy-0.2/doc/user_guide/images/curve_fitting_BN.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/plot_images_eds.png` & `exspy-0.2/doc/user_guide/images/plot_images_eds.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/plot_images_eds_cmap_factors_side_by_side.png` & `exspy-0.2/doc/user_guide/images/plot_images_eds_cmap_factors_side_by_side.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/images/plot_images_eds_cmap_list.png` & `exspy-0.2/doc/user_guide/images/plot_images_eds_cmap_list.png`

 * *Files identical despite different names*

### Comparing `exspy-0.1/doc/user_guide/install.rst` & `exspy-0.2/doc/user_guide/install.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 
 .. _install-label:
 
 .. warning::
-    These installation instructions are pending the release of the first version of exSpy.
+    These installation instructions are pending the release of the first version of eXSpy.
     In the meantime, you will need to install the development version, see instructions
     below.
 
 Installation
 ************
 
-To install exSpy, you have the following options (independent of the operating system you use):
+To install eXSpy, you have the following options (independent of the operating system you use):
 
-1. exSpy is included in the `HyperSpy Bundle <https://hyperspy.org/hyperspy-bundle/>`_,
+1. eXSpy is included in the `HyperSpy Bundle <https://hyperspy.org/hyperspy-bundle/>`_,
    a standalone program that includes a python distribution and all relevant libraries
    (recommended if you do not use *python* for anything else).
 2. :ref:`conda` (recommended if you are also working with other *python* packages).
 3. :ref:`pip`.
 4. Installing the development version from `GitHub <https://github.com/hyperspy/exspy/>`_.
    Refer to the appropriate section in the :external+hyperspy:ref:`HyperSpy user guide
-   <install-dev>` (replacing ``hyperspy`` by ``exSpy``).
+   <install-dev>` (replacing ``hyperspy`` by ``exspy``).
 
 
 .. _conda:
 
 Installation using conda
 ========================
 
-Follow these 3 steps to install exSpy using **conda** and start using it.
+Follow these 3 steps to install eXSpy using **conda** and start using it.
 
 1. Creating a conda environment
 -------------------------------
 
-exSpy requires Python 3 and ``conda`` -- we suggest using the Python 3 version
+eXSpy requires Python 3 and ``conda`` -- we suggest using the Python 3 version
 of `Miniforge <https://conda-forge.org/miniforge/>`_.
 
-We recommend creating a new environment for the exSpy package (or installing
+We recommend creating a new environment for the eXSpy package (or installing
 it in the :external+hyperspy:ref:`HyperSpy <anaconda-install>`
 environment, if you have one already). To create a new environment:
 
 1. Load the miniforge prompt.
 2. Run the following command:
 
 .. code-block:: bash
 
     (base) conda create -n exspy -y
 
 
 2. Installing the package in the new environment
 ------------------------------------------------
 
-Now activate the exSpy environment and install the package from ``conda-forge``:
+Now activate the eXSpy environment and install the package from ``conda-forge``:
 
 .. code-block:: bash
 
     (base) conda activate exspy
     (exspy) conda install -c conda-forge exspy -y
 
 Required dependencies will be installed automatically.
@@ -65,32 +65,32 @@
    If you run into trouble, check the more detailed documentation in the
    :external+hyperspy:ref:`HyperSpy user guide <anaconda-install>`.
 
 
 3. Getting Started
 ------------------
 
-To get started using exSpy, especially if you are unfamiliar with Python, we
+To get started using eXSpy, especially if you are unfamiliar with Python, we
 recommend using `Jupyter notebooks <https://jupyter.org/>`_. Having installed
-exSpy as above, a Jupyter notebook can be installed and opened using the following commands
+eXSpy as above, a Jupyter notebook can be installed and opened using the following commands
 entered into an anaconda prompt (from scratch):
 
 .. code-block:: bash
 
     (base) conda activate exspy
     (exspy) conda install -c conda-forge jupyterlab -y
     (exspy) jupyter lab
 
 
 .. _pip:
 
 Installation using pip
 ======================
 
-Alternatively, you can also find exSpy in the `Python Package Index (PyPI) <https://pypi.org>`_
+Alternatively, you can also find eXSpy in the `Python Package Index (PyPI) <https://pypi.org>`_
 and install it using (requires ``pip``):
 
 .. code-block:: bash
 
     pip install exspy
 
 Required dependencies will be installed automatically.
@@ -109,9 +109,9 @@
 
 .. code-block:: bash
 
     pip install exspy --upgrade
 
 .. Note::
 
-    If you want to be notified about new releases, please *Watch (Releases only)* the `exSpy repository
+    If you want to be notified about new releases, please *Watch (Releases only)* the `eXSpy repository
     on GitHub <https://github.com/hyperspy/exspy/>`_ (requires a GitHub account).
```

### Comparing `exspy-0.1/doc/user_guide/metadata_structure.rst` & `exspy-0.2/doc/user_guide/metadata_structure.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _metadata_structure:
 
-exSpy Metadata Structure
+eXSpy Metadata Structure
 ************************
 
-**exSpy** extends the :external+hyperspy:ref:`HyperSpy metadata structure
+**eXSpy** extends the :external+hyperspy:ref:`HyperSpy metadata structure
 <metadata_structure>`
 with conventions for metadata specific to its signal types. Refer to the
 :external+hyperspy:ref:`HyperSpy metadata documentation <metadata_structure>`
 for general metadata fields.
 
 The metadata of any **signal objects** is stored in the ``metadata`` attribute,
 which has a tree structure. By convention, the node labels are capitalized and
@@ -121,15 +121,15 @@
 
 Signal
 ======
 
 signal_type
     type: string
 
-    String that describes the type of signal. Currently, the only exSpy
+    String that describes the type of signal. Currently, the only eXSpy
     specific signal class is ``EELS``, ``EDS``, ``EDS_SEM`` or ``EDS_TEM``.
 
 See also :external+hyperspy:ref:`HyperSpy-Metadata-Sample <signal-metadata>`.
 
 .. _source-metadata:
 
 Acquisition_instrument
```

### Comparing `exspy-0.1/examples/model_fitting/coreloss_spectrum.msa` & `exspy-0.2/examples/model_fitting/coreloss_spectrum.msa`

 * *Files identical despite different names*

### Comparing `exspy-0.1/examples/model_fitting/lowloss_spectrum.msa` & `exspy-0.2/examples/model_fitting/lowloss_spectrum.msa`

 * *Files identical despite different names*

### Comparing `exspy-0.1/examples/model_fitting/plot_residual.py` & `exspy-0.2/examples/model_fitting/plot_residual.py`

 * *Files identical despite different names*

### Comparing `exspy-0.1/examples/model_fitting/simple_arctan_fit.py` & `exspy-0.2/examples/model_fitting/simple_arctan_fit.py`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/__init__.py` & `exspy-0.2/exspy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from importlib.metadata import version
 from pathlib import Path
 
 from . import components
 from . import data
 from . import models
```

### Comparing `exspy-0.1/exspy/_defaults_parser.py` & `exspy-0.2/exspy/_defaults_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import configparser
 import logging
 import os
 from pathlib import Path
 
 import traits.api as t
```

### Comparing `exspy-0.1/exspy/components/__init__.py` & `exspy-0.2/exspy/components/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Components """
+"""Components"""
 
 from .eels_arctan import EELSArctan
 from .eels_cl_edge import EELSCLEdge
 from .eels_double_power_law import DoublePowerLaw
 from .eels_vignetting import Vignetting
 from .pes_core_line_shape import PESCoreLineShape
 from .pes_see import SEE
```

### Comparing `exspy-0.1/exspy/components/eels_arctan.py` & `exspy-0.2/exspy/components/eels_arctan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
-from hyperspy._components.expression import Expression
+import hyperspy.api as hs
 
 
-class EELSArctan(Expression):
+class EELSArctan(hs.model.components1D.Expression):
     r"""Arctan function component for EELS (with minimum at zero).
 
     .. math::
 
         f(x) = A \cdot \left( \frac{\pi}{2} +
                \arctan \left[ k \left( x-x_0 \right) \right] \right)
```

### Comparing `exspy-0.1/exspy/components/eels_cl_edge.py` & `exspy-0.2/exspy/components/eels_cl_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import functools
 import logging
 import math
 
 import numpy as np
@@ -74,19 +74,19 @@
     Several possibilities are available for tabulated GOS.
 
     The preferred option is to use a database of cross sections in GOSH
     format. One such database can be freely downloaded from Zenodo at:
     https://zenodo.org/record/6599071 while information on the GOSH format
     are available at: https://gitlab.com/gguzzina/gosh .
 
-    exSpy also supports Peter Rez's Hartree Slater cross sections
+    eXSpy also supports Peter Rez's Hartree Slater cross sections
     parametrised as distributed by Gatan in their Digital Micrograph (DM)
-    software. If Digital Micrograph is installed in the system exSpy in the
-    standard location exSpy should find the path to the HS GOS folder.
-    Otherwise, the location of the folder can be defined in exSpy
+    software. If Digital Micrograph is installed in the system eXSpy in the
+    standard location eXSpy should find the path to the HS GOS folder.
+    Otherwise, the location of the folder can be defined in eXSpy
     preferences, which can be done through ~:func:`~.api.preferences.gui` or
     the :attr:`~api.preferences.EELS.eels_gos_files_path` variable.
 
     Parameters
     ----------
     element_subshell : str or dict
         Usually a string, for example, ``'Ti_L3'`` for the GOS of the titanium L3
@@ -136,17 +136,15 @@
         The width of the energy region, from the ionization edge onset, where
         the model is a spline function and/or any component
         in ``fine_structure_components`` instead of the EELS ionization
         edges simulation.
     fine_structure_components : set, default ``set()``
         A set containing components to model the fine structure region
         of the EELS ionization edge.
-    """.format(
-        _GOSH_DOI
-    )
+    """.format(_GOSH_DOI)
 
     _fine_structure_smoothing = 0.3
     _fine_structure_coeff_free = True
     _fine_structure_spline_active = True
 
     def __init__(self, element_subshell, GOS="gosh", gos_file_path=None):
         # Declare the parameters
```

### Comparing `exspy-0.1/exspy/components/eels_double_power_law.py` & `exspy-0.2/exspy/components/eels_double_power_law.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import numpy as np
 
 from hyperspy.docstrings.parameters import FUNCTION_ND_DOCSTRING
-from hyperspy._components.expression import Expression
+import hyperspy.api as hs
 
 
-class DoublePowerLaw(Expression):
+class DoublePowerLaw(hs.model.components1D.Expression):
     r"""Double power law component for EELS spectra.
 
     .. math::
 
         f(x) = A \cdot [s_r \cdot (x - x_0 - x_s)^{-r} + (x - x_0)^{-r}]
 
     ============= =============
```

### Comparing `exspy-0.1/exspy/components/eels_vignetting.py` & `exspy-0.2/exspy/components/eels_vignetting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import numpy as np
 from hyperspy.component import Component
-from hyperspy._components.gaussian import Gaussian
+import hyperspy.api as hs
 
 
 class Vignetting(Component):
-
     """
     Model the vignetting of the lens with a cos^4 law multiplied by lines on
     the edges
     """
 
     def __init__(self):
         Component.__init__(
@@ -43,43 +42,45 @@
                 "sigma",
             ],
         )
         self.left.value = np.nan
         self.right.value = np.nan
         self.side_vignetting = False
         self.fix_side_vignetting()
-        self.gaussian = Gaussian()
+        self.gaussian = hs.model.components1D.Gaussian()
         self.gaussian.centre.free, self.gaussian.A.free = False, False
         self.sigma.value = 1.0
         self.gaussian.A.value = 1.0
         self.period.value = 1.0
         self.extension_nch = 100
         self._position = self.optical_center
 
     def function(self, x):
         sigma = self.sigma.value
         x0 = self.optical_center.value
         A = self.height.value
         period = self.period.value
         la = self.left_slope.value
         ra = self.right_slope.value
-        l = self.left.value
-        r = self.right.value
+        left = self.left.value
+        right = self.right.value
         ex = self.extension_nch
         if self.side_vignetting is True:
             x = x.tolist()
             x = (
                 list(range(-ex, 0))
                 + x
                 + list(range(int(x[-1]) + 1, int(x[-1]) + ex + 1))
             )
             x = np.array(x)
             v1 = A * np.cos((x - x0) / (2 * np.pi * period)) ** 4
             v2 = np.where(
-                x < l, 1.0 - (l - x) * la, np.where(x < r, 1.0, 1.0 - (x - r) * ra)
+                x < left,
+                1.0 - (left - x) * la,
+                np.where(x < right, 1.0, 1.0 - (x - right) * ra),
             )
             self.gaussian.sigma.value = sigma
             self.gaussian.origin.value = (x[-1] + x[0]) / 2
             result = np.convolve(self.gaussian.function(x), v1 * v2, "same")
             return result[ex:-ex]
         else:
             return A * np.cos((x - x0) / (2 * np.pi * period)) ** 4
```

### Comparing `exspy-0.1/exspy/components/pes_core_line_shape.py` & `exspy-0.2/exspy/components/pes_core_line_shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import math
 
 from hyperspy.component import Component
 from hyperspy.docstrings.parameters import FUNCTION_ND_DOCSTRING
 
@@ -28,15 +28,14 @@
 def _calculate_shirley_background(values):
     cf = np.cumsum(values, axis=-1)
     # necessary to work with `function_nd`
     return cf[..., -1][np.newaxis].T - cf
 
 
 class PESCoreLineShape(Component):
-
     """ """
 
     def __init__(self, A=1.0, FWHM=1.0, origin=0.0, ab=0.0, shirley=0.0):
         Component.__init__(self, ["A", "FWHM", "origin", "ab", "shirley"])
         self.ab.value = 0
         self.ab.free = False
         self.A.value = A
```

### Comparing `exspy-0.1/exspy/components/pes_see.py` & `exspy-0.2/exspy/components/pes_see.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import numpy as np
 import logging
 
-from hyperspy._components.expression import Expression
+import hyperspy.api as hs
+
 
 _logger = logging.getLogger(__name__)
 
 
-class SEE(Expression):
+class SEE(hs.model.components1D.Expression):
     r"""Secondary electron emission component for Photoemission Spectroscopy.
 
     .. math::
         :nowrap:
 
         \[
         f(x) =
```

### Comparing `exspy-0.1/exspy/components/pes_voigt.py` & `exspy-0.2/exspy/components/pes_voigt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import math
 
 from hyperspy.component import Component, _get_scaling_factor
 from hyperspy._components.gaussian import _estimate_gaussian_parameters
```

### Comparing `exspy-0.1/exspy/components/volume_plasmon_drude.py` & `exspy-0.2/exspy/components/volume_plasmon_drude.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 
 import hyperspy.api as hs
 
 
 class VolumePlasmonDrude(hs.model.components1D.Expression):
@@ -91,19 +91,15 @@
             2
             * x
             * fwhm
             * plasmon_energy
             * intensity
             * (
                 (x**4 + (x * fwhm) ** 2 - plasmon_energy**4)
-                / (
-                    x**4
-                    + x**2 * (fwhm**2 - 2 * plasmon_energy**2)
-                    + plasmon_energy**4
-                )
+                / (x**4 + x**2 * (fwhm**2 - 2 * plasmon_energy**2) + plasmon_energy**4)
                 ** 2
             ),
             0,
         )
 
     # Partial derivative with respect to the plasmon linewidth delta_E_p
     def grad_fwhm(self, x):
@@ -113,24 +109,16 @@
 
         return np.where(
             x > 0,
             x
             * plasmon_energy
             * intensity
             * (
-                (
-                    x**4
-                    - x**2 * (2 * plasmon_energy**2 + fwhm**2)
-                    + plasmon_energy**4
-                )
-                / (
-                    x**4
-                    + x**2 * (fwhm**2 - 2 * plasmon_energy**2)
-                    + plasmon_energy**4
-                )
+                (x**4 - x**2 * (2 * plasmon_energy**2 + fwhm**2) + plasmon_energy**4)
+                / (x**4 + x**2 * (fwhm**2 - 2 * plasmon_energy**2) + plasmon_energy**4)
                 ** 2
             ),
             0,
         )
 
     def grad_intensity(self, x):
         return self.function(x) / self.intensity.value
```

### Comparing `exspy-0.1/exspy/conftest.py` & `exspy-0.2/exspy/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+
+import importlib
 
 try:
     # Set traits toolkit to work in a headless system
     # Capture error when toolkit is already previously set which typically
     # occurs when building the doc locally
     from traits.etsconfig.api import ETSConfig
 
@@ -29,17 +31,19 @@
 
 # pytest-mpl 0.7 already import pyplot, so setting the matplotlib backend to
 # 'agg' as early as we can is useless for testing.
 import matplotlib.pyplot as plt
 
 import pytest
 import numpy as np
-import matplotlib
 import hyperspy.api as hs
 
+# Use matplotlib fixture to clean up figure, setup backend, etc.
+from matplotlib.testing.conftest import mpl_test_settings  # noqa: F401
+
 
 @pytest.fixture(autouse=True)
 def add_np(doctest_namespace):
     doctest_namespace["np"] = np
     doctest_namespace["plt"] = plt
     doctest_namespace["hs"] = hs
 
@@ -52,20 +56,18 @@
 def setup_module(mod, pdb_cmdopt):
     if pdb_cmdopt:
         import dask
 
         dask.set_options(get=dask.local.get_sync)
 
 
-from matplotlib.testing.conftest import mpl_test_settings
+pytest_mpl_spec = importlib.util.find_spec("pytest_mpl")
 
 
-try:
-    import pytest_mpl
-except ImportError:
+if pytest_mpl_spec is None:
     # Register dummy marker to allow running the test suite without pytest-mpl
     def pytest_configure(config):
         config.addinivalue_line(
             "markers",
             "mpl_image_compare: dummy marker registration to allow running "
             "without the pytest-mpl plugin.",
         )
```

### Comparing `exspy-0.1/exspy/data/EDS_SEM_TM002.hspy` & `exspy-0.2/exspy/data/EDS_SEM_TM002.hspy`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/data/EDS_TEM_FePt_nanoparticles.hspy` & `exspy-0.2/exspy/data/EDS_TEM_FePt_nanoparticles.hspy`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/data/__init__.py` & `exspy-0.2/exspy/data/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
-import functools
 from pathlib import Path
 import warnings
 
 import numpy as np
 from scipy import interpolate
 
 import hyperspy.api as hs
```

### Comparing `exspy-0.1/exspy/docstrings/model.py` & `exspy-0.2/exspy/docstrings/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
-"""Common docstring snippets for model.
+"""Common docstring snippets for model."""
 
-"""
 from exspy.misc.eels.gosh_gos import _GOSH_DOI
 
 GOS_PARAMETER = """GOS : 'hydrogenic', 'gosh', 'Hartree-Slater'.
             The GOS to use. Default is ``'gosh'``.
 
         gos_file_path : str, None
             Only with GOS='gosh'. Specify the file path of the gosh file
-            to use. If None, use the file from doi:{}""".format(
-    _GOSH_DOI
-)
+            to use. If None, use the file from doi:{}""".format(_GOSH_DOI)
 
 EELSMODEL_PARAMETERS = """ll : None or EELSSpectrum
             If an EELSSpectrum is provided, it will be assumed that it is
             a low-loss EELS spectrum, and it will be used to simulate the
             effect of multiple scattering by convolving it with the EELS
             spectrum.
         auto_background : bool
@@ -45,10 +42,8 @@
             add the ionization edges as defined in the
             :class:`~.api.signals.EELSSpectrum` instance. Adding a new element to
             the spectrum using the :meth:`~.api.signals.EELSSpectrum.add_elements`
             method automatically add the corresponding ionisation edges to the model.
         {}
         dictionary : None or dict
             A dictionary to be used to recreate a model. Usually generated using
-            :meth:`~.model.BaseModel.as_dictionary`""".format(
-    GOS_PARAMETER
-)
+            :meth:`~.model.BaseModel.as_dictionary`""".format(GOS_PARAMETER)
```

### Comparing `exspy-0.1/exspy/hyperspy_extension.yaml` & `exspy-0.2/exspy/hyperspy_extension.yaml`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/misc/eds/eds.py` & `exspy-0.2/exspy/misc/eds/eds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 from exspy.misc.eds.utils import (
     edx_cross_section_to_zeta,
     electron_range,
     get_xray_lines_near_energy,
     take_off_angle,
```

### Comparing `exspy-0.1/exspy/misc/eds/ffast_mac.py` & `exspy-0.2/exspy/misc/eds/ffast_mac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # Chantler, C.T., Olsen, K., Dragoset, R.A., Kishore, A.R., Kotochigova,
 # S.A., and Zucker, D.S. (2005), X-Ray Form Factor, Attenuation and
 # Scattering Tables (version 2.1).
 # units cm^2/g
 
 from hyperspy.misc import utils
 
+# fmt: off
+
 ffast_mac = {'Ru': {'mass_absorption_coefficient (cm2/g)': [199360.0, 198330.0, 196750.0, 194530.0, 191680.0, 188160.0, 184010.0, 179240.0, 173900.0, 168030.0, 161720.0, 155050.0, 148080.0, 140920.0, 133640.0, 126320.0, 119050.0, 111890.0, 104900.0, 97628.0, 88273.0, 83018.0, 81057.0, 80545.0, 137480.0, 136560.0, 130800.0, 109930.0, 90227.0, 75783.0, 64664.0, 55753.0, 48403.0, 42219.0, 37562.0, 36946.0, 36449.0, 36161.0, 36630.0, 35616.0, 33344.0, 29474.0, 26109.0, 23171.0, 20599.0, 18343.0, 16360.0, 14614.0, 13075.0, 11715.0, 10512.0, 9444.8, 8496.1, 7649.7, 6892.5, 6213.3, 5602.6, 5052.5, 4555.9, 4278.7, 4180.5, 4178.8, 4152.7, 7745.7, 7761.5, 7815.4, 7874.5, 10454.0, 10911.0, 12318.0, 15520.0, 18498.0, 20594.0, 21565.0, 21450.0, 20470.0, 20339.0, 20012.0, 19922.0, 22293.0, 21909.0, 21719.0, 21356.0, 21298.0, 21185.0, 22047.0, 21606.0, 20374.0, 18244.0, 16804.0, 16331.0, 16208.0, 16850.0, 16729.0, 16268.0, 14825.0, 12973.0, 11310.0, 9838.6, 8535.4, 7382.2, 6377.9, 5506.7, 4716.8, 4026.6, 3408.9, 2890.5, 2454.9, 2088.2, 1779.2, 1518.4, 1298.1, 1105.5, 938.86, 798.41, 679.61, 578.54, 493.06, 466.46, 449.9, 445.63, 1595.9, 1538.7, 1525.6, 1521.9, 1466.0, 1451.6, 1995.6, 1946.9, 1782.6, 1678.5, 1592.8, 1571.1, 1780.3, 1700.5, 1653.6, 1391.4, 1212.5, 1030.3, 866.03, 727.75, 611.86, 514.7, 433.08, 362.71, 303.45, 253.57, 212.08, 177.55, 148.78, 124.42, 103.21, 85.697, 71.222, 59.217, 49.218, 40.811, 33.786, 27.923, 23.098, 19.124, 15.848, 13.145, 10.912, 10.668, 10.227, 10.114, 67.868, 65.103, 61.789, 51.765, 43.567, 36.492, 30.434, 25.355, 21.127, 17.605, 14.672, 12.229, 10.18, 8.4239, 6.9713, 5.7697, 4.7756, 3.9528, 3.2718, 2.7068, 2.2387, 1.8492, 1.523, 1.2543, 1.0321, 0.84874, 0.69797, 0.57402, 0.4721, 0.38829, 0.31938, 0.2627, 0.2161, 0.17777, 0.14624, 0.12031, 0.098979, 0.081433, 0.067001, 0.055128, 0.04536, 0.037324, 0.030713, 0.025274, 0.020798, 0.017116, 0.014085, 0.0],
                     'energies (keV)': [0.01069, 0.01142761, 0.01221612, 0.01305903, 0.0139601, 0.01492335, 0.01595306, 0.01705382, 0.01823053, 0.01948844, 0.02083314, 0.02227063, 0.0238073, 0.02545001, 0.02720606, 0.02908327, 0.03109002, 0.03323523, 0.03552846, 0.03797993, 0.04060054, 0.042238, 0.0428845, 0.0430569, 0.0433155, 0.04340198, 0.043962, 0.04639671, 0.04959809, 0.05302035, 0.05667876, 0.06058959, 0.06477028, 0.06923942, 0.073402, 0.07401695, 0.0745255, 0.0748251, 0.0752745, 0.076398, 0.07912411, 0.08458368, 0.09041995, 0.09665893, 0.1033284, 0.1104581, 0.1180797, 0.1262272, 0.1349368, 0.1442475, 0.1542005, 0.1648404, 0.1762144, 0.1883732, 0.2013709, 0.2152655, 0.2301188, 0.245997, 0.2629708, 0.273812, 0.277928, 0.278003, 0.2791206, 0.280797, 0.2811158, 0.282182, 0.2833164, 0.285018, 0.289272, 0.3005128, 0.3212482, 0.3434143, 0.3671099, 0.3924405, 0.4195189, 0.4484657, 0.451388, 0.458297, 0.4601394, 0.462903, 0.469812, 0.473144, 0.4794098, 0.480386, 0.4823172, 0.485214, 0.492456, 0.5124891, 0.5478508, 0.5733, 0.582075, 0.584415, 0.5856525, 0.587925, 0.5967, 0.6260625, 0.6692609, 0.7154399, 0.7648052, 0.8175768, 0.8739896, 0.9342948, 0.9987612, 1.067676, 1.141345, 1.220098, 1.304285, 1.394281, 1.490486, 1.593329, 1.703269, 1.820795, 1.94643, 2.080733, 2.224304, 2.377781, 2.541848, 2.717235, 2.781142, 2.82371, 2.835062, 2.852089, 2.894658, 2.904724, 2.907562, 2.952066, 2.963933, 2.981735, 3.026238, 3.10515, 3.15952, 3.20788, 3.220776, 3.24012, 3.28848, 3.319406, 3.548445, 3.793288, 4.055024, 4.334821, 4.633924, 4.953664, 5.295467, 5.660855, 6.051453, 6.469004, 6.915365, 7.392525, 7.902609, 8.44789, 9.030794, 9.653919, 10.32004, 11.03212, 11.79334, 12.60708, 13.47697, 14.40688, 15.40095, 16.46362, 17.59961, 18.81398, 20.11215, 21.49988, 21.67486, 22.00661, 22.09508, 22.22779, 22.55954, 22.98338, 24.56923, 26.2645, 28.07676, 30.01405, 32.08502, 34.29889, 36.66551, 39.19543, 41.89992, 44.79101, 47.88159, 51.18542, 54.71721, 58.4927, 62.5287, 66.84318, 71.45536, 76.38578, 81.6564, 87.29069, 93.31374, 99.75239, 106.6353, 113.9931, 121.8587, 130.2669, 139.2553, 148.864, 159.1356, 170.1159, 181.8539, 194.4018, 207.8156, 222.1548, 237.4835, 253.8699, 271.3869, 290.1126, 310.1304, 331.5294, 354.4049, 378.8588, 405.0001, 432.9451, 0.0]},
              'Re': {'mass_absorption_coefficient (cm2/g)': [12574.0, 12380.0, 11100.0, 11011.0, 10992.0, 50183.0, 49391.0, 72464.0, 79935.0, 87210.0, 93764.0, 99067.0, 102640.0, 104140.0, 103380.0, 100380.0, 95333.0, 88613.0, 80669.0, 71997.0, 63066.0, 54267.0, 45970.0, 38422.0, 31754.0, 29930.0, 28604.0, 28261.0, 56187.0, 54035.0, 53089.0, 44443.0, 39056.0, 37365.0, 36924.0, 41471.0, 40847.0, 39026.0, 33631.0, 30574.0, 29084.0, 28704.0, 38917.0, 37638.0, 37387.0, 31553.0, 26528.0, 22170.0, 18547.0, 15680.0, 13540.0, 12064.0, 11178.0, 10981.0, 10896.0, 10878.0, 11042.0, 10999.0, 10996.0, 11076.0, 11536.0, 12319.0, 13355.0, 14586.0, 15934.0, 17315.0, 18651.0, 19871.0, 20906.0, 21641.0, 22028.0, 22071.0, 21799.0, 21253.0, 20484.0, 19981.0, 19742.0, 19677.0, 20266.0, 20174.0, 20020.0, 19840.0, 19575.0, 19504.0, 19900.0, 19629.0, 19500.0, 18216.0, 16910.0, 15622.0, 14377.0, 13192.0, 12079.0, 11487.0, 11254.0, 11193.0, 11860.0, 11797.0, 11633.0, 10808.0, 10223.0, 10156.0, 10089.0, 10022.0, 9955.6, 9889.6, 9824.0, 9773.6, 9758.7, 9894.0, 9850.8, 9786.3, 9722.1, 9658.3, 9594.8, 9531.7, 9469.0, 9406.6, 9344.5, 9282.8, 9221.4, 9160.4, 9099.7, 9039.4, 8979.3, 8919.6, 8860.3, 8801.2, 8742.5, 8684.1, 8626.1, 8568.3, 8510.8, 8453.7, 8396.9, 8340.3, 8284.1, 8228.2, 8172.5, 8117.2, 8062.2, 8007.4, 7952.9, 7898.8, 7844.9, 7791.3, 7738.0, 7715.0, 7877.4, 7874.9, 7824.1, 7771.0, 7718.2, 7665.6, 7613.4, 7561.4, 7509.7, 7458.2, 7407.0, 7356.0, 7305.4, 7254.9, 7204.8, 7154.9, 7105.3, 7055.9, 7006.8, 6958.0, 6909.4, 6861.1, 6813.0, 6765.2, 6717.6, 6670.2, 6623.1, 6576.3, 6529.7, 6483.3, 6437.2, 6391.3, 6345.7, 6300.3, 6255.1, 6210.2, 6165.5, 6121.1, 6076.7, 6032.4, 5988.3, 5941.6, 5891.2, 5841.1, 5791.4, 5742.0, 5692.9, 5644.1, 5595.7, 5547.7, 5499.9, 5452.5, 5405.5, 5358.7, 5312.3, 5266.3, 5220.5, 5175.1, 5130.1, 5085.3, 5040.9, 4996.8, 4953.1, 4909.7, 4866.6, 4823.8, 4781.3, 4739.2, 4697.4, 4655.8, 4614.5, 4573.6, 4532.9, 4492.6, 4452.6, 4412.9, 4373.5, 4334.4, 4295.7, 4257.2, 4219.0, 4181.2, 4143.6, 4106.4, 4069.5, 4032.8, 3996.5, 3960.4, 3924.7, 3889.3, 3854.1, 3819.2, 3784.7, 3750.4, 3716.4, 3682.6, 3644.1, 3606.0, 3568.3, 3531.0, 3494.1, 3457.7, 3421.7, 3386.0, 3348.4, 3311.3, 3274.6, 3238.2, 3202.3, 3166.9, 3131.8, 3097.3, 3063.1, 3029.3, 2994.7, 2960.4, 2926.5, 2893.0, 2860.0, 2827.3, 2795.1, 2763.3, 2731.9, 2700.9, 2670.2, 2640.0, 2610.1, 2580.6, 2551.5, 2522.8, 2494.4, 2466.3, 2438.6, 2411.3, 2384.3, 2357.6, 2331.3, 2305.2, 2279.5, 2254.2, 2229.1, 2204.3, 2179.9, 2155.7, 2131.9, 2108.3, 2085.1, 2062.1, 2039.4, 2017.0, 1994.8, 1972.9, 1951.3, 1929.9, 1908.9, 1888.0, 1867.4, 1847.1, 1827.0, 1807.2, 1787.5, 1768.2, 1749.0, 1730.1, 1711.4, 1693.0, 1674.8, 1656.7, 1638.9, 1621.3, 1604.0, 1586.8, 1569.8, 1553.0, 1536.5, 1520.1, 1503.9, 1487.9, 1472.1, 1456.5, 1441.1, 1425.9, 1410.8, 1395.9, 1381.2, 1366.6, 1352.2, 1338.0, 1324.0, 1310.1, 1296.4, 1282.8, 1269.4, 1256.2, 1243.1, 1230.1, 1217.3, 1204.7, 1192.2, 1179.8, 1167.6, 1155.5, 1143.6, 1131.8, 1120.2, 1108.6, 1097.2, 1086.0, 1074.8, 1063.8, 1052.9, 1042.0, 1031.1, 1020.4, 1009.7, 999.2, 988.8, 978.52, 968.36, 958.32, 948.39, 938.57, 930.67, 3066.5, 3062.7, 3026.1, 2989.9, 2954.1, 2918.8, 2884.0, 2849.5, 2826.2, 4180.9, 4172.8, 4122.3, 4072.5, 4023.3, 3974.7, 3926.7, 3879.3, 3832.5, 3786.2, 3740.6, 3695.4, 3650.9, 3606.9, 3563.3, 3520.2, 3477.7, 3435.7, 3394.3, 3353.3, 3312.8, 3272.9, 3233.4, 3194.4, 3155.9, 3117.9, 3080.3, 3043.2, 3006.6, 2970.4, 2934.6, 2899.3, 2864.4, 2829.9, 2795.9, 2762.3, 2729.1, 2696.3, 2663.9, 2631.9, 2614.2, 3051.7, 3050.0, 3012.4, 2975.4, 2938.8, 2902.7, 2867.0, 2831.8, 2796.6, 2761.5, 2726.9, 2693.6, 2661.3, 2629.6, 2598.3, 2567.1, 2536.3, 2505.8, 2475.8, 2446.2, 2417.1, 2388.3, 2359.9, 2331.8, 2304.2, 2276.9, 2263.7, 2405.5, 2405.0, 2376.3, 2347.6, 2319.2, 2291.2, 2263.5, 2236.2, 2209.2, 2182.6, 2156.2, 2130.9, 2106.3, 2082.1, 2058.3, 2034.8, 2011.6, 1988.8, 1966.2, 1961.1, 2030.6, 2029.9, 2007.8, 1985.2, 1962.9, 1940.8, 1917.9, 1894.9, 1872.2, 1849.8, 1827.6, 1805.6, 1783.8, 1762.2, 1740.9, 1719.9, 1699.1, 1678.5, 1658.2, 1638.2, 1618.4, 1598.8, 1579.5, 1560.3, 1541.5, 1522.8, 1504.4, 1486.1, 1468.1, 1450.3, 1432.8, 1415.4, 1398.2, 1381.3, 1364.5, 1348.0, 1331.6, 1315.4, 1299.5, 1283.7, 1268.1, 1252.7, 1237.4, 1222.4, 1207.6, 1192.9, 1178.5, 1164.2, 1150.1, 1136.1, 1122.4, 1108.7, 1094.8, 1081.1, 1067.6, 1054.3, 1041.1, 1028.1, 1015.2, 1002.3, 989.48, 976.89, 964.46, 952.2, 940.11, 928.18, 916.42, 904.82, 893.37, 882.08, 870.94, 859.95, 849.11, 838.42, 827.87, 817.46, 807.2, 797.07, 787.08, 777.22, 767.5, 757.91, 748.44, 739.1, 729.89, 720.8, 711.84, 702.99, 694.26, 685.65, 677.15, 668.76, 660.49, 652.33, 644.27, 636.33, 628.48, 620.69, 612.84, 605.1, 597.46, 589.92, 582.49, 575.15, 567.87, 560.68, 553.59, 546.59, 539.69, 532.88, 526.17, 519.54, 513.0, 506.55, 500.17, 493.86, 487.64, 481.5, 475.44, 469.47, 463.58, 457.76, 452.0, 446.24, 440.57, 434.97, 429.44, 423.99, 418.61, 413.31, 408.07, 402.91, 397.81, 392.78, 387.82, 382.93, 378.1, 373.34, 368.63, 364.0, 359.41, 354.86, 350.37, 345.95, 341.58, 337.27, 333.02, 328.83, 324.69, 320.6, 316.57, 312.59, 308.67, 304.79, 300.97, 297.2, 293.48, 289.8, 286.18, 282.6, 279.07, 275.59, 272.15, 268.76, 265.41, 262.11, 258.85, 255.63, 252.45, 249.32, 246.22, 243.17, 240.16, 237.18, 234.25, 231.35, 228.49, 225.67, 222.88, 220.14, 217.42, 214.74, 212.1, 209.49, 206.92, 204.37, 201.86, 199.39, 196.94, 194.53, 192.15, 189.8, 187.48, 185.18, 182.92, 180.69, 178.49, 176.31, 174.16, 172.04, 169.95, 167.88, 165.84, 163.83, 161.84, 159.88, 157.94, 155.99, 154.07, 152.18, 150.31, 148.46, 146.63, 144.82, 143.01, 141.23, 122.4, 102.1, 85.275, 85.171, 81.694, 80.801, 215.03, 206.47, 192.12, 162.68, 159.87, 155.98, 154.26, 211.96, 203.57, 200.05, 191.94, 189.86, 216.47, 215.7, 208.44, 181.84, 152.93, 128.55, 107.92, 90.543, 75.994, 63.816, 53.585, 44.958, 37.732, 31.639, 26.324, 21.86, 18.169, 15.114, 12.583, 10.484, 8.7415, 7.2943, 6.0809, 5.0699, 4.2218, 3.5035, 2.9089, 2.4151, 2.1041, 2.0173, 2.0065, 1.9949, 10.048, 9.6829, 8.6629, 7.2598, 6.089, 5.1151, 4.2756, 3.5744, 2.9885, 2.4991, 2.0901, 1.7482, 1.4597, 1.2173, 1.0153, 0.84684, 0.70641, 0.58933, 0.49169, 0.41027, 0.34236, 0.28571, 0.23846, 0.19903, 0.16744, 0.1409, 0.11858, 0.0998, 0.084002, 0.0],
                     'energies (keV)': [0.005235171, 0.005313308, 0.005941418, 0.006032358, 0.006056608, 0.006092984, 0.006183924, 0.01069, 0.01142761, 0.01221612, 0.01305903, 0.0139601, 0.01492335, 0.01595306, 0.01705382, 0.01823053, 0.01948844, 0.02083314, 0.02227063, 0.0238073, 0.02545001, 0.02720606, 0.02908327, 0.03109002, 0.03323523, 0.033908, 0.034427, 0.0345654, 0.034773, 0.035292, 0.03552846, 0.03797993, 0.039788, 0.040397, 0.0405594, 0.04060054, 0.040803, 0.041412, 0.04340198, 0.044688, 0.045372, 0.0455544, 0.045828, 0.04639671, 0.046512, 0.04959809, 0.05302035, 0.05667876, 0.06058959, 0.06477028, 0.06923942, 0.07401695, 0.07912411, 0.081144, 0.082386, 0.0827172, 0.083214, 0.084456, 0.08458368, 0.09041995, 0.09665893, 0.1033284, 0.1104581, 0.1180797, 0.1262272, 0.1349368, 0.1442475, 0.1542005, 0.1648404, 0.1762144, 0.1883732, 0.2013709, 0.2152655, 0.2301188, 0.245997, 0.254996, 0.258899, 0.2599398, 0.261501, 0.2629708, 0.265404, 0.268226, 0.2723315, 0.2734263, 0.2750685, 0.279174, 0.2811158, 0.3005128, 0.3212482, 0.3434143, 0.3671099, 0.3924405, 0.4195189, 0.435512, 0.442178, 0.4439556, 0.446622, 0.4484657, 0.453288, 0.4794098, 0.5, 0.5025, 0.5050125, 0.50753756, 0.51007525, 0.51262563, 0.51518875, 0.51717493, 0.5177647, 0.51862505, 0.52035352, 0.52295529, 0.52557007, 0.52819792, 0.53083891, 0.5334931, 0.53616057, 0.53884137, 0.54153558, 0.54424325, 0.54696447, 0.54969929, 0.55244779, 0.55521003, 0.55798608, 0.56077601, 0.56357989, 0.56639779, 0.56922978, 0.57207593, 0.5749363, 0.57781099, 0.58070004, 0.58360354, 0.58652156, 0.58945417, 0.59240144, 0.59536345, 0.59834026, 0.60133196, 0.60433862, 0.60736032, 0.61039712, 0.6134491, 0.61651635, 0.61959893, 0.62269693, 0.62404375, 0.62581041, 0.62595625, 0.62893946, 0.63208416, 0.63524458, 0.6384208, 0.64161291, 0.64482097, 0.64804508, 0.6512853, 0.65454173, 0.65781444, 0.66110351, 0.66440903, 0.66773107, 0.67106973, 0.67442508, 0.6777972, 0.68118619, 0.68459212, 0.68801508, 0.69145515, 0.69491243, 0.69838699, 0.70187893, 0.70538832, 0.70891526, 0.71245984, 0.71602214, 0.71960225, 0.72320026, 0.72681626, 0.73045034, 0.7341026, 0.73777311, 0.74146197, 0.74516928, 0.74889513, 0.75263961, 0.7564028, 0.76018482, 0.76398574, 0.76780567, 0.7716447, 0.77550292, 0.77938044, 0.78327734, 0.78719373, 0.79112969, 0.79508534, 0.79906077, 0.80305607, 0.80707135, 0.81110671, 0.81516224, 0.81923806, 0.82333425, 0.82745092, 0.83158817, 0.83574611, 0.83992484, 0.84412447, 0.84834509, 0.85258682, 0.85684975, 0.861134, 0.86543967, 0.86976687, 0.8741157, 0.87848628, 0.88287871, 0.8872931, 0.89172957, 0.89618822, 0.90066916, 0.9051725, 0.90969837, 0.91424686, 0.91881809, 0.92341218, 0.92802924, 0.93266939, 0.93733274, 0.9420194, 0.9467295, 0.95146315, 0.95622046, 0.96100156, 0.96580657, 0.9706356, 0.97548878, 0.98036623, 0.98526806, 0.9901944, 0.99514537, 1.0001211, 1.0051217, 1.0101473, 1.015198, 1.020274, 1.0253754, 1.0305023, 1.0356548, 1.0408331, 1.0460372, 1.0512674, 1.0565238, 1.0618064, 1.0671154, 1.072451, 1.0778132, 1.0832023, 1.0886183, 1.0940614, 1.0995317, 1.1050294, 1.1105545, 1.1161073, 1.1216878, 1.1272963, 1.1329328, 1.1385974, 1.1442904, 1.1500119, 1.1557619, 1.1615407, 1.1673484, 1.1731852, 1.1790511, 1.1849464, 1.1908711, 1.1968254, 1.2028096, 1.2088236, 1.2148677, 1.2209421, 1.2270468, 1.233182, 1.2393479, 1.2455447, 1.2517724, 1.2580312, 1.2643214, 1.270643, 1.2769962, 1.2833812, 1.2897981, 1.2962471, 1.3027283, 1.309242, 1.3157882, 1.3223671, 1.328979, 1.3356239, 1.342302, 1.3490135, 1.3557586, 1.3625374, 1.36935, 1.3761968, 1.3830778, 1.3899932, 1.3969431, 1.4039278, 1.4109475, 1.4180022, 1.4250922, 1.4322177, 1.4393788, 1.4465757, 1.4538086, 1.4610776, 1.468383, 1.4757249, 1.4831035, 1.490519, 1.4979716, 1.5054615, 1.5129888, 1.5205537, 1.5281565, 1.5357973, 1.5434763, 1.5511937, 1.5589496, 1.5667444, 1.5745781, 1.582451, 1.5903633, 1.5983151, 1.6063066, 1.6143382, 1.6224099, 1.6305219, 1.6386745, 1.6468679, 1.6551022, 1.6633777, 1.6716946, 1.6800531, 1.6884534, 1.6968956, 1.7053801, 1.713907, 1.7224766, 1.7310889, 1.7397444, 1.7484431, 1.7571853, 1.7659712, 1.7748011, 1.7836751, 1.7925935, 1.8015565, 1.8105642, 1.8196171, 1.8287151, 1.8378587, 1.847048, 1.8562833, 1.8655647, 1.8748925, 1.8825065, 1.8832935, 1.884267, 1.8936883, 1.9031567, 1.9126725, 1.9222359, 1.9318471, 1.9415063, 1.9481516, 1.9496484, 1.9512138, 1.9609699, 1.9707747, 1.9806286, 1.9905318, 2.0004844, 2.0104868, 2.0205393, 2.030642, 2.0407952, 2.0509992, 2.0612542, 2.0715604, 2.0819182, 2.0923278, 2.1027895, 2.1133034, 2.1238699, 2.1344893, 2.1451617, 2.1558875, 2.166667, 2.1775003, 2.1883878, 2.1993297, 2.2103264, 2.221378, 2.2324849, 2.2436473, 2.2548656, 2.2661399, 2.2774706, 2.2888579, 2.3003022, 2.3118037, 2.3233628, 2.3349796, 2.3466545, 2.3583878, 2.3649801, 2.36962, 2.3701797, 2.3820306, 2.3939407, 2.4059104, 2.41794, 2.4300297, 2.4421798, 2.4543907, 2.4666627, 2.478996, 2.491391, 2.5038479, 2.5163672, 2.528949, 2.5415938, 2.5543017, 2.5670732, 2.5799086, 2.5928082, 2.6057722, 2.6188011, 2.6318951, 2.6450545, 2.6582798, 2.6715712, 2.6780604, 2.6849291, 2.6851398, 2.6983537, 2.7118455, 2.7254047, 2.7390317, 2.7527269, 2.7664905, 2.780323, 2.7942246, 2.8081957, 2.8222367, 2.8363479, 2.8505296, 2.8647823, 2.8791062, 2.8935017, 2.9079692, 2.9225091, 2.9258366, 2.9371216, 2.9375634, 2.9518072, 2.9665662, 2.9813991, 2.9963061, 3.0112876, 3.026344, 3.0414758, 3.0566831, 3.0719666, 3.0873264, 3.102763, 3.1182768, 3.1338682, 3.1495376, 3.1652853, 3.1811117, 3.1970172, 3.2130023, 3.2290673, 3.2452127, 3.2614387, 3.2777459, 3.2941347, 3.3106053, 3.3271584, 3.3437941, 3.3605131, 3.3773157, 3.3942023, 3.4111733, 3.4282291, 3.4453703, 3.4625971, 3.4799101, 3.4973097, 3.5147962, 3.5323702, 3.5500321, 3.5677822, 3.5856211, 3.6035492, 3.621567, 3.6396748, 3.6578732, 3.6761626, 3.6945434, 3.7130161, 3.7315812, 3.7502391, 3.7689903, 3.7878352, 3.8067744, 3.8258083, 3.8449373, 3.864162, 3.8834828, 3.9029002, 3.9224147, 3.9420268, 3.9617369, 3.9815456, 4.0014533, 4.0214606, 4.0415679, 4.0617757, 4.0820846, 4.102495, 4.1230075, 4.1436226, 4.1643407, 4.1851624, 4.2060882, 4.2271186, 4.2482542, 4.2694955, 4.290843, 4.3122972, 4.3338587, 4.355528, 4.3773056, 4.3991921, 4.4211881, 4.443294, 4.4655105, 4.4878381, 4.5102772, 4.5328286, 4.5554928, 4.5782702, 4.6011616, 4.6241674, 4.6472882, 4.6705247, 4.6938773, 4.7173467, 4.7409334, 4.7646381, 4.7884613, 4.8124036, 4.8364656, 4.8606479, 4.8849512, 4.9093759, 4.9339228, 4.9585924, 4.9833854, 5.0083023, 5.0333438, 5.0585105, 5.0838031, 5.1092221, 5.1347682, 5.1604421, 5.1862443, 5.2121755, 5.2382364, 5.2644276, 5.2907497, 5.3172034, 5.3437895, 5.3705084, 5.3973609, 5.4243477, 5.4514695, 5.4787268, 5.5061205, 5.5336511, 5.5613193, 5.5891259, 5.6170716, 5.6451569, 5.6733827, 5.7017496, 5.7302584, 5.7589096, 5.7877042, 5.8166427, 5.8457259, 5.8749546, 5.9043293, 5.933851, 5.9635202, 5.9933378, 6.0233045, 6.053421, 6.0836882, 6.1141066, 6.1446771, 6.1754005, 6.2062775, 6.2373089, 6.2684954, 6.2998379, 6.3313371, 6.3629938, 6.3948088, 6.4267828, 6.4589167, 6.4912113, 6.5236674, 6.5562857, 6.5890671, 6.6220125, 6.6551225, 6.6883981, 6.7218401, 6.7554493, 6.7892266, 6.8231727, 6.8572886, 6.891575, 6.9260329, 6.9606631, 6.9954664, 7.0304437, 7.0655959, 7.1009239, 7.1364285, 7.1721107, 7.2079712, 7.2440111, 7.2802311, 7.3166323, 7.3532155, 7.3899815, 7.4269314, 7.4640661, 7.5013864, 7.5388934, 7.5765878, 7.6144708, 7.6525431, 7.6908058, 7.7292599, 7.7679062, 7.8067457, 7.8457794, 7.8850083, 7.9244334, 7.9640555, 8.0038758, 8.0438952, 8.0841147, 8.1245352, 8.1651579, 8.2059837, 8.2470136, 8.2882487, 8.3296899, 8.3713384, 8.4131951, 8.455261, 8.4975373, 8.540025, 9.030794, 9.653919, 10.32004, 10.32459, 10.48262, 10.52476, 10.58798, 10.74601, 11.03212, 11.71953, 11.79334, 11.89891, 11.94674, 12.01849, 12.19787, 12.27617, 12.46407, 12.51417, 12.58933, 12.60708, 12.77723, 13.47697, 14.40688, 15.40095, 16.46362, 17.59961, 18.81398, 20.11215, 21.49988, 22.98338, 24.56923, 26.2645, 28.07676, 30.01405, 32.08502, 34.29889, 36.66551, 39.19543, 41.89992, 44.79101, 47.88159, 51.18542, 54.71721, 58.4927, 62.5287, 66.84318, 70.24287, 71.31802, 71.45536, 71.60472, 72.03478, 73.10993, 76.38578, 81.6564, 87.29069, 93.31374, 99.75239, 106.6353, 113.9931, 121.8587, 130.2669, 139.2553, 148.864, 159.1356, 170.1159, 181.8539, 194.4018, 207.8156, 222.1548, 237.4835, 253.8699, 271.3869, 290.1126, 310.1304, 331.5294, 354.4049, 378.8588, 405.0001, 432.9451, 0.0]},
              'Ra': {'mass_absorption_coefficient (cm2/g)': [210240.0, 195520.0, 180640.0, 130300.0, 95222.0, 70955.0, 53769.0, 41353.0, 32220.0, 25389.0, 20197.0, 16194.0, 13066.0, 10593.0, 9108.4, 8693.0, 8619.8, 8586.7, 9572.7, 9110.2, 7857.9, 6328.5, 5137.7, 4197.5, 3447.3, 2844.8, 2713.9, 2600.2, 2571.1, 249970.0, 239310.0, 232330.0, 191230.0, 147860.0, 103470.0, 67758.0, 42713.0, 26528.0, 16540.0, 10506.0, 6873.6, 4665.9, 3299.3, 2767.2, 2586.1, 2541.2, 3858.8, 3801.6, 3659.9, 3033.4, 2487.5, 2101.6, 1916.8, 1857.8, 1842.9, 2526.4, 2525.4, 2430.9, 2144.1, 1856.7, 1643.4, 1607.4, 1568.9, 1559.1, 1682.6, 1648.0, 1618.5, 1490.9, 1425.9, 1403.9, 1398.3, 1571.9, 1598.6, 1822.9, 2616.4, 4076.0, 6070.3, 8227.2, 10108.0, 11399.0, 11852.0, 11887.0, 11919.0, 11947.0, 11971.0, 11991.0, 12008.0, 12022.0, 12032.0, 12038.0, 12041.0, 12041.0, 12038.0, 12032.0, 12022.0, 12009.0, 11994.0, 11975.0, 11954.0, 11930.0, 11904.0, 11875.0, 11843.0, 11809.0, 11773.0, 11734.0, 11693.0, 11650.0, 11605.0, 11558.0, 11510.0, 11459.0, 11406.0, 11352.0, 11297.0, 11239.0, 11181.0, 11120.0, 11100.0, 11945.0, 11920.0, 11860.0, 11799.0, 11736.0, 11672.0, 11608.0, 11542.0, 11475.0, 11408.0, 11340.0, 11271.0, 11265.0, 11737.0, 11691.0, 11623.0, 11554.0, 11485.0, 11415.0, 11344.0, 11273.0, 11202.0, 11130.0, 11058.0, 10986.0, 10913.0, 10840.0, 10767.0, 10693.0, 10619.0, 10545.0, 10471.0, 10397.0, 10322.0, 10248.0, 10173.0, 10098.0, 10024.0, 9948.9, 9874.1, 9799.4, 9724.6, 9649.9, 9575.3, 9500.7, 9426.3, 9352.0, 9277.9, 9204.0, 9130.2, 9056.7, 8983.5, 8910.4, 8837.7, 8765.2, 8693.1, 8621.2, 8549.7, 8478.5, 8407.6, 8337.1, 8267.0, 8197.3, 8127.9, 8059.0, 7990.4, 7922.3, 7854.6, 7787.3, 7720.4, 7654.0, 7588.1, 7522.6, 7457.5, 7393.0, 7328.9, 7265.2, 7202.1, 7144.4, 7139.4, 7567.2, 7526.2, 7462.3, 7398.6, 7335.3, 7272.5, 7210.2, 7148.4, 7087.1, 7026.3, 6965.9, 6906.0, 6846.6, 6787.7, 6729.3, 6671.4, 6613.9, 6557.0, 6500.5, 6444.5, 6389.0, 6334.0, 6279.5, 6225.4, 6171.8, 6118.6, 6065.9, 6010.7, 5955.9, 5901.5, 5846.8, 5791.3, 5736.2, 5681.5, 5627.4, 5573.6, 5520.3, 5469.3, 5467.5, 5522.3, 5492.9, 5440.5, 5388.5, 5336.2, 5283.9, 5231.9, 5180.5, 5129.5, 5078.9, 5028.9, 4979.5, 4930.5, 4882.0, 4834.0, 4786.4, 4739.3, 4692.7, 4646.4, 4600.7, 4555.4, 4510.5, 4466.0, 4422.0, 4378.5, 4334.1, 4285.4, 4251.9, 4323.1, 4315.2, 4275.1, 4227.6, 4180.8, 4134.5, 4088.8, 4043.7, 3999.1, 3955.1, 3911.4, 3868.0, 3825.3, 3783.1, 3741.4, 3700.2, 3659.5, 3619.4, 3579.7, 3540.6, 3501.9, 3463.7, 3426.0, 3388.7, 3351.9, 3315.6, 3279.7, 3244.2, 3209.0, 3174.2, 3139.9, 3106.0, 3072.5, 3039.4, 3006.7, 2974.4, 2942.5, 2911.0, 2879.9, 2849.1, 2818.7, 2788.6, 2759.0, 2729.4, 2700.1, 2671.2, 2642.6, 2614.3, 2586.4, 2558.8, 2531.6, 2504.6, 2478.0, 2451.7, 2425.6, 2399.8, 2374.3, 2349.1, 2324.3, 2299.7, 2275.3, 2251.3, 2227.5, 2204.1, 2180.9, 2157.9, 2135.3, 2112.8, 2090.7, 2068.8, 2047.2, 2025.8, 2004.6, 1983.7, 1963.1, 1942.6, 1922.4, 1902.5, 1882.7, 1863.2, 1844.0, 1824.9, 1806.1, 1787.4, 1769.0, 1750.8, 1732.8, 1715.0, 1697.4, 1680.1, 1662.9, 1645.9, 1629.1, 1612.4, 1596.0, 1579.8, 1563.7, 1547.9, 1532.2, 1516.6, 1501.3, 1486.1, 1471.1, 1456.3, 1441.7, 1427.2, 1412.8, 1398.6, 1384.6, 1370.8, 1357.1, 1343.5, 1330.1, 1316.9, 1303.7, 1290.7, 1277.8, 1265.0, 1252.4, 1239.9, 1227.6, 1215.4, 1203.3, 1191.4, 1179.6, 1167.9, 1156.3, 1144.9, 1133.6, 1122.5, 1111.4, 1100.5, 1089.7, 1079.0, 1068.5, 1058.0, 1047.7, 1037.4, 1027.3, 1017.3, 1007.1, 996.65, 986.36, 976.18, 966.11, 956.16, 946.32, 936.59, 926.97, 917.45, 908.05, 898.44, 888.88, 879.43, 870.09, 860.86, 851.73, 842.71, 833.79, 824.97, 816.25, 807.63, 799.11, 790.69, 782.36, 774.13, 765.99, 757.94, 749.98, 742.12, 734.34, 726.65, 719.05, 711.54, 704.11, 696.75, 689.46, 682.26, 675.14, 668.09, 661.13, 654.25, 647.44, 640.71, 632.95, 624.93, 617.01, 609.21, 601.51, 593.92, 586.43, 585.83, 1532.0, 1515.6, 1495.4, 1475.5, 1455.8, 1436.4, 1417.3, 1398.5, 1379.9, 1361.6, 1359.1, 1959.4, 1940.0, 1914.2, 1888.7, 1863.5, 1838.7, 1814.2, 1790.1, 1766.3, 1742.8, 1719.6, 1696.8, 1674.2, 1652.0, 1630.1, 1608.4, 1587.1, 1565.9, 1545.1, 1524.5, 1504.2, 1484.2, 1464.4, 1444.9, 1425.7, 1406.8, 1388.1, 1369.6, 1351.4, 1333.5, 1315.8, 1299.0, 1298.3, 1510.3, 1500.0, 1481.2, 1462.6, 1444.3, 1426.2, 1408.4, 1390.7, 1373.4, 1356.2, 1339.2, 1322.5, 1305.9, 1289.6, 1273.2, 1257.1, 1241.2, 1225.5, 1210.0, 1194.7, 1179.5, 1164.6, 1149.9, 1135.2, 1120.7, 1106.4, 1092.3, 1078.3, 1064.6, 1051.0, 1037.6, 1024.3, 1011.2, 998.34, 988.4, 985.61, 1044.7, 1036.5, 1023.6, 1010.9, 998.4, 986.01, 973.76, 961.67, 949.73, 937.95, 926.32, 914.85, 903.54, 892.36, 881.66, 881.33, 910.8, 908.9, 897.94, 887.11, 876.42, 865.84, 855.31, 844.92, 834.65, 824.52, 814.51, 804.6, 794.82, 785.17, 775.63, 766.21, 756.91, 747.72, 738.64, 729.67, 720.82, 712.07, 703.44, 694.91, 686.49, 678.17, 669.96, 661.85, 653.84, 645.94, 638.13, 630.41, 622.77, 615.23, 607.78, 600.43, 593.17, 586.0, 578.92, 571.91, 564.95, 558.07, 551.28, 544.58, 537.96, 531.42, 524.97, 518.6, 512.3, 506.09, 499.96, 493.9, 487.83, 481.82, 475.88, 470.01, 464.22, 458.5, 452.86, 447.29, 441.79, 436.31, 430.89, 425.54, 420.26, 415.05, 409.9, 404.83, 399.81, 394.86, 389.98, 385.16, 380.4, 375.7, 371.06, 366.49, 361.97, 357.51, 353.1, 348.76, 344.47, 340.23, 336.05, 331.93, 327.86, 323.84, 319.87, 315.95, 312.08, 308.27, 304.5, 300.78, 297.07, 293.4, 289.78, 286.21, 282.68, 279.2, 275.76, 272.37, 269.02, 265.72, 262.46, 259.24, 256.06, 252.92, 249.83, 246.77, 243.76, 240.78, 237.84, 234.94, 232.08, 229.25, 226.46, 223.71, 194.51, 162.71, 136.21, 114.22, 95.879, 80.554, 67.779, 56.935, 50.072, 48.141, 47.869, 47.644, 117.99, 113.5, 101.05, 84.282, 77.895, 74.726, 73.91, 102.87, 99.499, 98.973, 98.945, 95.101, 94.104, 107.2, 103.3, 97.085, 81.871, 68.987, 58.142, 49.014, 41.071, 34.373, 28.745, 24.032, 20.113, 16.798, 14.002, 11.68, 9.7504, 8.146, 6.8107, 5.6985, 4.7716, 3.9983, 3.3462, 2.8028, 2.3426, 1.942, 1.6096, 1.3351, 1.2598, 1.2075, 1.194, 5.3627, 5.1646, 5.0868, 4.2898, 3.6138, 3.0412, 2.5585, 2.1518, 1.8075, 1.5183, 1.2755, 1.0715, 0.9003, 0.7567, 0.63628, 0.53509, 0.45004, 0.37855, 0.31845, 0.26792, 0.22543, 0.1897, 0.15964, 0.13436, 0.0],
                     'energies (keV)': [0.018894, 0.019176, 0.01948844, 0.02083314, 0.02227063, 0.0238073, 0.02545001, 0.02720606, 0.02908327, 0.03109002, 0.03323523, 0.03552846, 0.03797993, 0.04060054, 0.04263, 0.0432825, 0.04340198, 0.0434565, 0.0437175, 0.04437, 0.04639671, 0.04959809, 0.05302035, 0.05667876, 0.06058959, 0.06477028, 0.065856, 0.066864, 0.0671328, 0.067536, 0.068544, 0.06923942, 0.07401695, 0.07912411, 0.08458368, 0.09041995, 0.09665893, 0.1033284, 0.1104581, 0.1180797, 0.1262272, 0.1349368, 0.1442475, 0.149744, 0.152036, 0.1526472, 0.153564, 0.1542005, 0.155856, 0.1648404, 0.1762144, 0.1883732, 0.196392, 0.199398, 0.2001996, 0.2013709, 0.201402, 0.204408, 0.2152655, 0.2301188, 0.245997, 0.249312, 0.253128, 0.2541456, 0.255672, 0.259488, 0.2629708, 0.2811158, 0.292922, 0.2974055, 0.2986011, 0.3005128, 0.304878, 0.3212482, 0.3434143, 0.3671099, 0.3924405, 0.4195189, 0.4484657, 0.4794098, 0.5, 0.5025, 0.5050125, 0.50753756, 0.51007525, 0.51262563, 0.51518875, 0.5177647, 0.52035352, 0.52295529, 0.52557007, 0.52819792, 0.53083891, 0.5334931, 0.53616057, 0.53884137, 0.54153558, 0.54424325, 0.54696447, 0.54969929, 0.55244779, 0.55521003, 0.55798608, 0.56077601, 0.56357989, 0.56639779, 0.56922978, 0.57207593, 0.5749363, 0.57781099, 0.58070004, 0.58360354, 0.58652156, 0.58945417, 0.59240144, 0.59536345, 0.59834026, 0.60133196, 0.60233476, 0.60306523, 0.60433862, 0.60736032, 0.61039712, 0.6134491, 0.61651635, 0.61959893, 0.62269693, 0.62581041, 0.62893946, 0.63208416, 0.63524458, 0.63551339, 0.63628665, 0.6384208, 0.64161291, 0.64482097, 0.64804508, 0.6512853, 0.65454173, 0.65781444, 0.66110351, 0.66440903, 0.66773107, 0.67106973, 0.67442508, 0.6777972, 0.68118619, 0.68459212, 0.68801508, 0.69145515, 0.69491243, 0.69838699, 0.70187893, 0.70538832, 0.70891526, 0.71245984, 0.71602214, 0.71960225, 0.72320026, 0.72681626, 0.73045034, 0.7341026, 0.73777311, 0.74146197, 0.74516928, 0.74889513, 0.75263961, 0.7564028, 0.76018482, 0.76398574, 0.76780567, 0.7716447, 0.77550292, 0.77938044, 0.78327734, 0.78719373, 0.79112969, 0.79508534, 0.79906077, 0.80305607, 0.80707135, 0.81110671, 0.81516224, 0.81923806, 0.82333425, 0.82745092, 0.83158817, 0.83574611, 0.83992484, 0.84412447, 0.84834509, 0.85258682, 0.85684975, 0.861134, 0.86543967, 0.86976687, 0.8741157, 0.87813301, 0.87848628, 0.88006703, 0.88287871, 0.8872931, 0.89172957, 0.89618822, 0.90066916, 0.9051725, 0.90969837, 0.91424686, 0.91881809, 0.92341218, 0.92802924, 0.93266939, 0.93733274, 0.9420194, 0.9467295, 0.95146315, 0.95622046, 0.96100156, 0.96580657, 0.9706356, 0.97548878, 0.98036623, 0.98526806, 0.9901944, 0.99514537, 1.0001211, 1.0051217, 1.0101473, 1.015198, 1.020274, 1.0253754, 1.0305023, 1.0356548, 1.0408331, 1.0460372, 1.0512674, 1.0563415, 1.0565238, 1.0588586, 1.0618064, 1.0671154, 1.072451, 1.0778132, 1.0832023, 1.0886183, 1.0940614, 1.0995317, 1.1050294, 1.1105545, 1.1161073, 1.1216878, 1.1272963, 1.1329328, 1.1385974, 1.1442904, 1.1500119, 1.1557619, 1.1615407, 1.1673484, 1.1731852, 1.1790511, 1.1849464, 1.1908711, 1.1968254, 1.2028096, 1.2069862, 1.2088236, 1.2098138, 1.2148677, 1.2209421, 1.2270468, 1.233182, 1.2393479, 1.2455447, 1.2517724, 1.2580312, 1.2643214, 1.270643, 1.2769962, 1.2833812, 1.2897981, 1.2962471, 1.3027283, 1.309242, 1.3157882, 1.3223671, 1.328979, 1.3356239, 1.342302, 1.3490135, 1.3557586, 1.3625374, 1.36935, 1.3761968, 1.3830778, 1.3899932, 1.3969431, 1.4039278, 1.4109475, 1.4180022, 1.4250922, 1.4322177, 1.4393788, 1.4465757, 1.4538086, 1.4610776, 1.468383, 1.4757249, 1.4831035, 1.490519, 1.4979716, 1.5054615, 1.5129888, 1.5205537, 1.5281565, 1.5357973, 1.5434763, 1.5511937, 1.5589496, 1.5667444, 1.5745781, 1.582451, 1.5903633, 1.5983151, 1.6063066, 1.6143382, 1.6224099, 1.6305219, 1.6386745, 1.6468679, 1.6551022, 1.6633777, 1.6716946, 1.6800531, 1.6884534, 1.6968956, 1.7053801, 1.713907, 1.7224766, 1.7310889, 1.7397444, 1.7484431, 1.7571853, 1.7659712, 1.7748011, 1.7836751, 1.7925935, 1.8015565, 1.8105642, 1.8196171, 1.8287151, 1.8378587, 1.847048, 1.8562833, 1.8655647, 1.8748925, 1.884267, 1.8936883, 1.9031567, 1.9126725, 1.9222359, 1.9318471, 1.9415063, 1.9512138, 1.9609699, 1.9707747, 1.9806286, 1.9905318, 2.0004844, 2.0104868, 2.0205393, 2.030642, 2.0407952, 2.0509992, 2.0612542, 2.0715604, 2.0819182, 2.0923278, 2.1027895, 2.1133034, 2.1238699, 2.1344893, 2.1451617, 2.1558875, 2.166667, 2.1775003, 2.1883878, 2.1993297, 2.2103264, 2.221378, 2.2324849, 2.2436473, 2.2548656, 2.2661399, 2.2774706, 2.2888579, 2.3003022, 2.3118037, 2.3233628, 2.3349796, 2.3466545, 2.3583878, 2.3701797, 2.3820306, 2.3939407, 2.4059104, 2.41794, 2.4300297, 2.4421798, 2.4543907, 2.4666627, 2.478996, 2.491391, 2.5038479, 2.5163672, 2.528949, 2.5415938, 2.5543017, 2.5670732, 2.5799086, 2.5928082, 2.6057722, 2.6188011, 2.6318951, 2.6450545, 2.6582798, 2.6715712, 2.6849291, 2.6983537, 2.7118455, 2.7254047, 2.7390317, 2.7527269, 2.7664905, 2.780323, 2.7942246, 2.8081957, 2.8222367, 2.8363479, 2.8505296, 2.8647823, 2.8791062, 2.8935017, 2.9079692, 2.9225091, 2.9371216, 2.9518072, 2.9665662, 2.9813991, 2.9963061, 3.0112876, 3.026344, 3.0414758, 3.0566831, 3.0719666, 3.0873264, 3.102763, 3.1040119, 3.1057879, 3.1182768, 3.1338682, 3.1495376, 3.1652853, 3.1811117, 3.1970172, 3.2130023, 3.2290673, 3.2452127, 3.2473832, 3.2494167, 3.2614387, 3.2777459, 3.2941347, 3.3106053, 3.3271584, 3.3437941, 3.3605131, 3.3773157, 3.3942023, 3.4111733, 3.4282291, 3.4453703, 3.4625971, 3.4799101, 3.4973097, 3.5147962, 3.5323702, 3.5500321, 3.5677822, 3.5856211, 3.6035492, 3.621567, 3.6396748, 3.6578732, 3.6761626, 3.6945434, 3.7130161, 3.7315812, 3.7502391, 3.7689903, 3.7870982, 3.7878352, 3.7965019, 3.8067744, 3.8258083, 3.8449373, 3.864162, 3.8834828, 3.9029002, 3.9224147, 3.9420268, 3.9617369, 3.9815456, 4.0014533, 4.0214606, 4.0415679, 4.0617757, 4.0820846, 4.102495, 4.1230075, 4.1436226, 4.1643407, 4.1851624, 4.2060882, 4.2271186, 4.2482542, 4.2694955, 4.290843, 4.3122972, 4.3338587, 4.355528, 4.3773056, 4.3991921, 4.4211881, 4.443294, 4.4655105, 4.4829005, 4.4878381, 4.4960996, 4.5102772, 4.5328286, 4.5554928, 4.5782702, 4.6011616, 4.6241674, 4.6472882, 4.6705247, 4.6938773, 4.7173467, 4.7409334, 4.7646381, 4.7884613, 4.8116809, 4.8124036, 4.8323191, 4.8364656, 4.8606479, 4.8849512, 4.9093759, 4.9339228, 4.9585924, 4.9833854, 5.0083023, 5.0333438, 5.0585105, 5.0838031, 5.1092221, 5.1347682, 5.1604421, 5.1862443, 5.2121755, 5.2382364, 5.2644276, 5.2907497, 5.3172034, 5.3437895, 5.3705084, 5.3973609, 5.4243477, 5.4514695, 5.4787268, 5.5061205, 5.5336511, 5.5613193, 5.5891259, 5.6170716, 5.6451569, 5.6733827, 5.7017496, 5.7302584, 5.7589096, 5.7877042, 5.8166427, 5.8457259, 5.8749546, 5.9043293, 5.933851, 5.9635202, 5.9933378, 6.0233045, 6.053421, 6.0836882, 6.1141066, 6.1446771, 6.1754005, 6.2062775, 6.2373089, 6.2684954, 6.2998379, 6.3313371, 6.3629938, 6.3948088, 6.4267828, 6.4589167, 6.4912113, 6.5236674, 6.5562857, 6.5890671, 6.6220125, 6.6551225, 6.6883981, 6.7218401, 6.7554493, 6.7892266, 6.8231727, 6.8572886, 6.891575, 6.9260329, 6.9606631, 6.9954664, 7.0304437, 7.0655959, 7.1009239, 7.1364285, 7.1721107, 7.2079712, 7.2440111, 7.2802311, 7.3166323, 7.3532155, 7.3899815, 7.4269314, 7.4640661, 7.5013864, 7.5388934, 7.5765878, 7.6144708, 7.6525431, 7.6908058, 7.7292599, 7.7679062, 7.8067457, 7.8457794, 7.8850083, 7.9244334, 7.9640555, 8.0038758, 8.0438952, 8.0841147, 8.1245352, 8.1651579, 8.2059837, 8.2470136, 8.2882487, 8.3296899, 8.3713384, 8.4131951, 8.455261, 8.4975373, 8.540025, 9.030794, 9.653919, 10.32004, 11.03212, 11.79334, 12.60708, 13.47697, 14.40688, 15.13551, 15.36718, 15.40095, 15.42896, 15.52162, 15.75329, 16.46362, 17.59961, 18.11461, 18.39188, 18.46582, 18.57672, 18.81398, 18.85197, 18.85399, 19.14052, 19.21746, 19.33288, 19.62143, 20.11215, 21.49988, 22.98338, 24.56923, 26.2645, 28.07676, 30.01405, 32.08502, 34.29889, 36.66551, 39.19543, 41.89992, 44.79101, 47.88159, 51.18542, 54.71721, 58.4927, 62.5287, 66.84318, 71.45536, 76.38578, 81.6564, 87.29069, 93.31374, 99.75239, 101.8435, 103.4023, 103.818, 104.4415, 106.0003, 106.6353, 113.9931, 121.8587, 130.2669, 139.2553, 148.864, 159.1356, 170.1159, 181.8539, 194.4018, 207.8156, 222.1548, 237.4835, 253.8699, 271.3869, 290.1126, 310.1304, 331.5294, 354.4049, 378.8588, 405.0001, 432.9451, 0.0]},
              'Rb': {'mass_absorption_coefficient (cm2/g)': [1155.1, 1197.9, 1241.7, 1293.7, 2177.5, 2206.8, 2533.4, 3616.9, 7005.6, 11952.0, 18002.0, 24420.0, 30356.0, 35096.0, 38217.0, 39620.0, 39459.0, 38040.0, 37567.0, 37062.0, 36922.0, 39341.0, 38941.0, 38820.0, 38408.0, 38383.0, 38230.0, 39094.0, 38523.0, 36832.0, 33878.0, 30792.0, 28524.0, 27833.0, 27726.0, 27651.0, 28648.0, 27968.0, 25985.0, 23154.0, 20536.0, 18144.0, 15977.0, 14023.0, 12269.0, 10705.0, 9318.2, 8093.3, 7015.6, 6070.6, 5244.5, 4524.3, 3897.8, 3354.1, 2883.2, 2425.2, 2042.0, 1721.9, 1453.7, 1227.6, 1038.1, 879.02, 745.38, 679.83, 655.01, 648.62, 3109.1, 3068.7, 3037.3, 2964.2, 2892.3, 2855.2, 3979.8, 3797.3, 3543.2, 3184.6, 3059.8, 3027.9, 3435.0, 3413.0, 3310.1, 2897.9, 2470.0, 2095.0, 1774.1, 1500.6, 1264.5, 1062.0, 892.76, 747.35, 623.99, 520.11, 433.24, 360.87, 300.85, 251.04, 209.67, 175.18, 146.5, 122.62, 102.67, 85.691, 71.32, 58.603, 48.201, 39.683, 32.703, 26.976, 22.274, 18.409, 16.742, 16.035, 15.853, 120.04, 117.14, 114.83, 96.694, 81.066, 68.293, 57.49, 48.106, 40.198, 33.564, 28.02, 23.316, 19.381, 16.029, 13.243, 10.942, 9.0405, 7.4694, 6.1706, 5.0953, 4.2076, 3.4749, 2.8699, 2.3704, 1.9558, 1.6074, 1.3212, 1.0848, 0.88866, 0.72801, 0.59643, 0.48865, 0.40036, 0.32804, 0.26879, 0.22026, 0.18049, 0.14791, 0.12121, 0.099338, 0.081414, 0.066726, 0.05469, 0.044826, 0.036743, 0.030118, 0.024688, 0.020238, 0.01659, 0.0136, 0.01115, 0.009141, 0.0074943, 0.0],
```

### Comparing `exspy-0.1/exspy/misc/eds/utils.py` & `exspy-0.2/exspy/misc/eds/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import numpy as np
 import math
 from scipy import constants
 from hyperspy.misc.utils import stack
 from exspy.misc.elements import elements as elements_db
@@ -461,16 +461,18 @@
 
     intens = intens.reshape(dim)
     if mask is not None:
         from hyperspy.signals import BaseSignal
 
         if isinstance(mask, BaseSignal):
             mask = mask.data
+        if mask.dtype != bool:
+            mask = mask.astype(bool)
         for i in range(dim[0]):
-            intens[i][(mask == True)] = 0
+            intens[i][mask] = 0
 
     return intens
 
 
 quantification_cliff_lorimer.__doc__ %= _ABSORPTION_CORRECTION_DOCSTRING
```

### Comparing `exspy-0.1/exspy/misc/eels/base_gos.py` & `exspy-0.2/exspy/misc/eels/base_gos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import math
 
 import numpy as np
 from scipy import constants, integrate, interpolate
 
@@ -140,13 +140,13 @@
             pp2 = p02 - E / R * (gamma - E / 1022120)
             qa0sqmax = qa0sqmin + 4 * np.sqrt(p02 * pp2) * (math.sin(angle / 2)) ** 2
             qmin = math.sqrt(qa0sqmin) / a0
             qmax = math.sqrt(qa0sqmax) / a0
             # Perform the integration in a log grid
             qaxis, gos = self.get_qaxis_and_gos(i, qmin, qmax)
             logsqa0qaxis = np.log((a0 * qaxis) ** 2)
-            qint[i] = integrate.simps(gos, logsqa0qaxis)
+            qint[i] = integrate.simpson(gos, x=logsqa0qaxis)
         E = self.energy_axis + energy_shift
         # Energy differential cross section in (barn/eV/atom)
         qint *= (4.0 * np.pi * a0**2.0 * R**2 / E / T * self.subshell_factor) * 1e28
         self.qint = qint
         return interpolate.make_interp_spline(E, qint, k=3)
```

### Comparing `exspy-0.1/exspy/misc/eels/eelsdb.py` & `exspy-0.2/exspy/misc/eels/eelsdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 """This module provides tools to interact with The EELS Database."""
+
 import requests
 import logging
 
 from hyperspy.defaults_parser import preferences
 from hyperspy.docstrings.signal import SHOW_PROGRESSBAR_ARG
 from hyperspy.external.progressbar import progressbar
 from hyperspy.io import dict2signal
@@ -251,15 +252,15 @@
         "https://api.eelsdb.eu/spectra", params=params, verify=verify_certificate
     )
     spectra = []
     jsons = request.json()
     if "message" in jsons:
         # Invalid query, EELSdb raises error.
         raise IOError(
-            "Please report the following error to the exSpy developers: "
+            "Please report the following error to the eXSpy developers: "
             f"{jsons['message']}."
         )
 
     for json_spectrum in progressbar(jsons, disable=not show_progressbar):
         download_link = json_spectrum["download_link"]
         if download_link.split(".")[-1].lower() != "msa":
             _logger.exception(
@@ -274,15 +275,15 @@
         try:
             s = dict2signal(parse_msa_string(msa_string)[0])
             emsa = s.original_metadata
             s._original_metadata = type(s.original_metadata)({"json": json_spectrum})
             s.original_metadata.emsa = emsa
             spectra.append(s)
 
-        except:
+        except Exception:
             # parse_msa_string or dict2signal may fail if the EMSA file is not
             # a valid one.
             _logger.exception(
                 "Failed to load the spectrum.\n"
                 "Title: %s id: %s.\n"
                 "Please report this error to https://eelsdb.eu/about \n"
                 % (json_spectrum["title"], json_spectrum["id"])
```

### Comparing `exspy-0.1/exspy/misc/eels/effective_angle.py` & `exspy-0.2/exspy/misc/eels/effective_angle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import math
 
 
 def effective_angle(E0, E, alpha, beta):
     """Calculates the effective collection angle
```

### Comparing `exspy-0.1/exspy/misc/eels/electron_inelastic_mean_free_path.py` & `exspy-0.2/exspy/misc/eels/electron_inelastic_mean_free_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import numpy as np
 import math
 
 
 def _F(electron_energy):
@@ -101,17 +101,15 @@
     E_p = 28.816 * math.sqrt(N_v * rho / M)
     gamma = 0.191 / math.sqrt(rho)
     U = (E_p / 28.816) ** 2
     C = 19.7 - 9.1 * U
     D = 534 - 208 * U
     beta = -1 + 9.44 / math.sqrt(E_p**2 + E_g**2) + 0.69 * rho**0.1
     iMFP = (
-        alpha
-        * E
-        / (E_p**2 * (beta * math.log(gamma * alpha * E) - C / E + D / E**2))
+        alpha * E / (E_p**2 * (beta * math.log(gamma * alpha * E) - C / E + D / E**2))
     )
     return iMFP
 
 
 def iMFP_angular_correction(density, beam_energy, alpha, beta):
     """Estimate the effect of limited collection angle on EELS mean free path
```

### Comparing `exspy-0.1/exspy/misc/eels/gosh_gos.py` & `exspy-0.2/exspy/misc/eels/gosh_gos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import logging
 
 import h5py
 import numpy as np
 import pooch
 from scipy import constants
@@ -72,14 +72,15 @@
     _name = "gosh"
     _whitelist = {
         "gos_array": None,
         "rel_energy_axis": None,
         "qaxis": None,
         "element": None,
         "subshell": None,
+        "subshell_factor": None,
     }
 
     def __init__(self, element_subshell, gos_file_path=None):
         """
         Parameters
         ----------
         element_subshell : str
```

### Comparing `exspy-0.1/exspy/misc/eels/hartree_slater_gos.py` & `exspy-0.2/exspy/misc/eels/hartree_slater_gos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import logging
 from pathlib import Path
 
 import numpy as np
 from scipy import constants
 
@@ -64,15 +64,14 @@
     "O4,5": {"table": "O5", "factor": 5 / 3},
     "O4": {"table": "O5", "factor": 2 / 3},
     "O5": {"table": "O5", "factor": 1},
 }
 
 
 class HartreeSlaterGOS(TabulatedGOS):
-
     """Read Hartree-Slater Generalized Oscillator Strength parametrized
     from files.
 
     Parameters
     ----------
     element_subshell : {str, dict}
         Usually a string, for example, 'Ti_L3' for the GOS of the titanium L3
@@ -104,14 +103,15 @@
     _name = "Hartree-Slater"
     _whitelist = {
         "gos_array": None,
         "rel_energy_axis": None,
         "qaxis": None,
         "element": None,
         "subshell": None,
+        "subshell_factor": None,
     }
 
     def read_elements(self):
         super().read_elements()
         self.subshell_factor = conventions[self.subshell]["factor"]
 
     def read_gos_data(self):  # pragma: no cover
```

### Comparing `exspy-0.1/exspy/misc/eels/hydrogenic_gos.py` & `exspy-0.2/exspy/misc/eels/hydrogenic_gos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import math
 import logging
 
 import numpy as np
 from scipy import integrate, interpolate, constants
 
@@ -60,15 +60,14 @@
 # IE1=[118,149,189,229,270,320,377,438,500,564,628,695,769,846,
 # 926,1008,1096,1194,1142,1248,1359,1476,1596,1727]
 
 R = constants.value("Rydberg constant times hc in eV")
 
 
 class HydrogenicGOS(BaseGOS):
-
     """Computes the K and L GOS using R. Egerton's  routines.
 
     Parameters
     ----------
     element_subshell : str
         For example, 'Ti_L3' for the GOS of the titanium L3 subshell
```

### Comparing `exspy-0.1/exspy/misc/eels/tools.py` & `exspy-0.2/exspy/misc/eels/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import math
 import numbers
 import logging
 
 import numpy as np
 import matplotlib.pyplot as plt
@@ -56,30 +56,28 @@
         variance_sorted = variance.squeeze()[sorting_index_array]
         variance2fit = variance_sorted[average_higher_than]
         average2fit = average_sorted[average_higher_than]
     else:
         variance2fit = variance
         average2fit = average
 
-    fit = np.polyfit(average2fit, variance2fit, pol_order)
+    fit = np.polynomial.Polynomial.fit(average2fit, variance2fit, pol_order)
     if weighted is True:
-        from hyperspy._signals.signal1D import Signal1D
-        from hyperspy.models.model1d import Model1D
-        from hyperspy.components1d import Line
+        import hyperspy.api as hs
 
-        s = Signal1D(variance2fit)
+        s = hs.signals.Signal1D(variance2fit)
         s.axes_manager.signal_axes[0].axis = average2fit
-        m = Model1D(s)
-        l = Line()
-        l.a.value = fit[1]
-        l.b.value = fit[0]
-        m.append(l)
+        m = s.create_model()
+        line = hs.model.components1D.Polynomial()
+        line.a.value = fit[1]
+        line.b.value = fit[0]
+        m.append(line)
         m.fit(weights=True)
-        fit[0] = l.b.value
-        fit[1] = l.a.value
+        fit[0] = line.b.value
+        fit[1] = line.a.value
 
     if plot_results is True:
         plt.figure()
         plt.scatter(average.squeeze(), variance.squeeze())
         plt.xlabel("Counts")
         plt.ylabel("Variance")
         plt.plot(average2fit, np.polyval(fit, average2fit), color="red")
@@ -105,37 +103,38 @@
     plot_results=True,
     weighted=False,
     store_results="ask",
 ):
     """Find the scale and offset of the Poissonian noise
 
     By comparing an SI with its denoised version (i.e. by PCA),
-    this plots an
-    estimation of the variance as a function of the number of counts
-    and fits a
-    polynomy to the result.
+    this plots an estimation of the variance as a function of the number of counts
+    and fits a polynomial to the result.
 
     Parameters
     ----------
-    noisy_SI, clean_SI : signal1D.Signal1D instances
-    mask : numpy bool array
+    noisy_SI, clean_SI : hyperspy.api.signals.Signal1D
+    mask : numpy.ndarray
         To define the channels that will be used in the calculation.
     pol_order : int
-        The order of the polynomy.
+        The order of the polynomial.
     higher_than: float
         To restrict the fit to counts over the given value.
-    return_results : Bool
-    plot_results : Bool
+    return_results : bool
+        Whether to return the results or not.
+    plot_results : bool
+        Whether to plot the results or not.
     store_results: {True, False, "ask"}, default "ask"
         If True, it stores the result in the signal metadata
 
     Returns
     -------
-    Dictionary with the result of a linear fit to estimate the offset
-    and scale factor
+    dict
+        Dictionary with the result of a linear fit to estimate the offset
+        and scale factor
 
     """
     with noisy_signal.unfolded(), clean_signal.unfolded():
         # The rest of the code assumes that the first data axis
         # is the navigation axis. We transpose the data if that is not the
         # case.
         ns = (
@@ -203,15 +202,15 @@
             )
             noisy_signal.metadata.set_item(
                 "Signal.Noise_properties.Variance_linear_model." "correlation_factor", c
             )
             noisy_signal.metadata.set_item(
                 "Signal.Noise_properties.Variance_linear_model."
                 + "parameters_estimation_method",
-                "exSpy",
+                "eXSpy",
             )
 
     if return_results is True:
         return results0
 
 
 def power_law_perc_area(E1, E2, r):
```

### Comparing `exspy-0.1/exspy/misc/material.py` & `exspy-0.2/exspy/misc/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from collections.abc import Iterable
 import numpy as np
 import numbers
 import copy
 
 from exspy.misc.elements import elements as elements_db
```

### Comparing `exspy-0.1/exspy/models/edsmodel.py` & `exspy-0.2/exspy/models/edsmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from __future__ import division
 
 import warnings
 import numpy as np
 import math
 import logging
@@ -93,15 +93,14 @@
 
 
 def _get_scale(E1, E_ref1, fact):
     return "{} + {} * (x - {})".format(E1, fact, E_ref1)
 
 
 class EDSModel(Model1D):
-
     """Build and fit a model of an EDS Signal1D.
 
     Parameters
     ----------
     spectrum : EDSSpectrum (or any EDSSpectrum subclass) instance.
 
     auto_add_lines : bool
```

### Comparing `exspy-0.1/exspy/models/edssemmodel.py` & `exspy-0.2/exspy/models/edssemmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from exspy.models.edsmodel import EDSModel
 
 
 class EDSSEMModel(EDSModel):
-
     """Build and fit a model to EDS data acquired in the SEM.
 
     Parameters
     ----------
     spectrum : EDSSEMSpectrum
 
     auto_add_lines : bool
```

### Comparing `exspy-0.1/exspy/models/edstemmodel.py` & `exspy-0.2/exspy/models/edstemmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from exspy.models.edsmodel import EDSModel
 
 
 class EDSTEMModel(EDSModel):
-
     """Build and fit a model to EDS data acquired in the TEM.
 
     Parameters
     ----------
     spectrum : EDSTEMSpectrum
 
     auto_add_lines : bool
```

### Comparing `exspy-0.1/exspy/models/eelsmodel.py` & `exspy-0.2/exspy/models/eelsmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import copy
 import logging
 import warnings
 
 import numpy as np
```

### Comparing `exspy-0.1/exspy/signal_tools.py` & `exspy-0.2/exspy/signal_tools.py`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/signals/__init__.py` & `exspy-0.2/exspy/signals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Modules containing the exSpy signals and their lazy counterparts.
+Modules containing the eXSpy signals and their lazy counterparts.
 
 EELSSpectrum
     For electron energy-loss data with ``signal_dimension`` equal one, i.e.
     spectral data of ``n`` dimensions. The signal is binned by default.
 EDSTEMSpectrum
     For electron energy-dispersive X-ray data acquired in a transmission
     electron microscopy with ``signal_dimension`` equal one, i.e.
@@ -12,14 +12,15 @@
     For electron energy-dispersive X-ray data acquired in a scanning
     electron microscope with ``signal_dimension`` equal one, i.e.
     spectral data of ``n`` dimensions. The signal is binned by default.
 DielectricFunction
     For dielectric function data with ``signal_dimension`` equal one. The signal
     is unbinned by default.
 """
+
 from .dielectric_function import DielectricFunction, LazyDielectricFunction
 from .eds import EDSSpectrum, LazyEDSSpectrum
 from .eds_sem import EDSSEMSpectrum, LazyEDSSEMSpectrum
 from .eds_tem import EDSTEMSpectrum, LazyEDSTEMSpectrum
 from .eels import EELSSpectrum, LazyEELSSpectrum
```

### Comparing `exspy-0.1/exspy/signals/dielectric_function.py` & `exspy-0.2/exspy/signals/dielectric_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 from scipy import constants
-from scipy.integrate import simps, cumtrapz
+from scipy.integrate import simpson, cumulative_trapezoid
 
 from hyperspy._signals.complex_signal1d import (
     ComplexSignal1D,
     LazyComplexSignal1D,
 )
 from hyperspy.docstrings.signal import LAZYSIGNAL_DOC
 from exspy.misc.eels.tools import eels_constant
 
 
 class DielectricFunction(ComplexSignal1D):
-
     """Signal class for dielectric functions."""
 
     _signal_type = "DielectricFunction"
     _alias_signal_types = ["dielectric function"]
 
     def get_number_of_effective_electrons(self, nat, cumulative=False):
         r"""
@@ -79,37 +78,37 @@
         m0 = constants.value("electron mass")
         epsilon0 = constants.epsilon_0  # Vacuum permittivity [F/m]
         hbar = constants.hbar  # Reduced Plank constant [J·s]
         k = 2 * epsilon0 * m0 / (np.pi * nat * hbar**2)
 
         axis = self.axes_manager.signal_axes[0]
         if cumulative is False:
-            dneff1 = k * simps(
+            dneff1 = k * simpson(
                 (-1.0 / self.data).imag * axis.axis,
                 x=axis.axis,
                 axis=axis.index_in_array,
             )
-            dneff2 = k * simps(
+            dneff2 = k * simpson(
                 self.data.imag * axis.axis, x=axis.axis, axis=axis.index_in_array
             )
             neff1 = self._get_navigation_signal(data=dneff1)
             neff2 = self._get_navigation_signal(data=dneff2)
         else:
             neff1 = self._deepcopy_with_new_data(
                 k
-                * cumtrapz(
+                * cumulative_trapezoid(
                     (-1.0 / self.data).imag * axis.axis,
                     x=axis.axis,
                     axis=axis.index_in_array,
                     initial=0,
                 )
             )
             neff2 = self._deepcopy_with_new_data(
                 k
-                * cumtrapz(
+                * cumulative_trapezoid(
                     self.data.imag * axis.axis,
                     x=axis.axis,
                     axis=axis.index_in_array,
                     initial=0,
                 )
             )
 
@@ -168,11 +167,10 @@
         s.data = s.data.real
         s.set_signal_type("EELS")
         s.metadata.General.title = "EELS calculated from " + self.metadata.General.title
         return s
 
 
 class LazyDielectricFunction(DielectricFunction, LazyComplexSignal1D):
-
     """Lazy signal class for dielectric functions."""
 
     __doc__ += LAZYSIGNAL_DOC.replace("__BASECLASS__", "DielectricFunction")
```

### Comparing `exspy-0.1/exspy/signals/eds.py` & `exspy-0.2/exspy/signals/eds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import itertools
 import logging
 
 import numpy as np
 import warnings
 from collections.abc import Iterable
 from matplotlib import pyplot as plt
 
+import hyperspy.api as hs
 from hyperspy import utils
 from hyperspy.signal import BaseSignal
 from hyperspy._signals.signal1d import Signal1D, LazySignal1D
 from exspy.misc.elements import elements as elements_db
 from exspy.misc.eds import utils as utils_eds
 from hyperspy.misc.utils import isiterable
-from hyperspy.utils.markers import Texts, VerticalLines, Lines
 from hyperspy.docstrings.plot import BASE_PLOT_DOCSTRING_PARAMETERS, PLOT1D_DOCSTRING
 from hyperspy.docstrings.signal import LAZYSIGNAL_DOC
 
+
 _logger = logging.getLogger(__name__)
 
 
 class EDSSpectrum(Signal1D):
     """General signal class for EDS spectra."""
 
     _signal_type = "EDS"
@@ -75,21 +76,17 @@
         is not None
         """
 
         units_name = self.axes_manager.signal_axes[0].units
 
         if FWHM_MnKa == "auto":
             if self.metadata.Signal.signal_type == "EDS_SEM":
-                FWHM_MnKa = (
-                    self.metadata.Acquisition_instrument.SEM.Detector.EDS.energy_resolution_MnKa
-                )
+                FWHM_MnKa = self.metadata.Acquisition_instrument.SEM.Detector.EDS.energy_resolution_MnKa
             elif self.metadata.Signal.signal_type == "EDS_TEM":
-                FWHM_MnKa = (
-                    self.metadata.Acquisition_instrument.TEM.Detector.EDS.energy_resolution_MnKa
-                )
+                FWHM_MnKa = self.metadata.Acquisition_instrument.TEM.Detector.EDS.energy_resolution_MnKa
             else:
                 raise NotImplementedError(
                     "This method only works for EDS_TEM or EDS_SEM signals. "
                     "You can use `set_signal_type('EDS_TEM')` or"
                     "`set_signal_type('EDS_SEM')` to convert to one of these"
                     "signal types."
                 )
@@ -1012,22 +1009,22 @@
 
         Parameters
         ----------
         position: 2D array of float
             The position on the signal axis. Each row corresponds to a
             group.
         kwargs
-            keywords argument for :py:class:`~.api.plot.markers.VerticalLine`
+            keywords argument for :class:`hyperspy.api.plot.markers.VerticalLine`
         """
         colors = itertools.cycle(
             np.sort(plt.rcParams["axes.prop_cycle"].by_key()["color"])
         )
 
         for x, color in zip(position, colors):
-            line = VerticalLines(offsets=x, color=color, **kwargs)
+            line = hs.plot.markers.VerticalLines(offsets=x, color=color, **kwargs)
             self.add_marker(line, render_figure=False)
         if render_figure:
             self._render_figure(plot=["signal_plot"])
 
     def add_xray_lines_markers(self, xray_lines, render_figure=True):
         """
         Add marker on a spec.plot() with the name of the selected X-ray
@@ -1036,39 +1033,34 @@
         Parameters
         ----------
         xray_lines: list of string
             A valid list of X-ray lines
         """
         if self._plot is None or not self._plot.is_active:
             raise RuntimeError("The signal needs to be plotted.")
-        norm = self._plot.signal_plot.ax_lines[0].norm
-        minimum_intensity = self.data[self.data > 0].min() if norm == "log" else 0
         line_names = []
         segments = np.empty((len(xray_lines), 2, 2))
         offsets = np.empty((len(xray_lines), 2))
         # might want to set the intensity based on the alpha line intensity
         for i, xray_line in enumerate(xray_lines):
             element, line = utils_eds._get_element_and_line(xray_line)
-            relative_factor = elements_db[element]["Atomic_properties"]["Xray_lines"][
-                line
-            ]["weight"]
             eng = self._get_line_energy(f"{element}_{line}")
             segments[i] = [[eng, 0], [eng, 1]]
             offsets[i] = [eng, 1]
             line_names.append(
                 r"$\mathrm{%s}_{\mathrm{%s}}$"
                 % utils_eds._get_element_and_line(xray_line)
             )
 
-        line_markers = Lines(
+        line_markers = hs.plot.markers.Lines(
             segments=segments,
             transform="relative",
             color="black",
         )
-        text_markers = Texts(
+        text_markers = hs.plot.markers.Texts(
             offsets=offsets,
             texts=line_names,
             offset_transform="relative",
             rotation=np.pi / 2,
             horizontalalignment="left",
             verticalalignment="bottom",
             facecolor="black",
@@ -1142,15 +1134,15 @@
                 y2 = self.isig[bw[2]].data
             else:
                 y2 = self.isig[bw[2] : bw[3]].mean(-1).data
             x1 = (bw[0] + bw[1]) / 2.0
             x2 = (bw[2] + bw[3]) / 2.0
             segments.append([[x1, y1[0]], [x2, y2[0]]])
         segments = np.array(segments)
-        lines = Lines(segments=segments, color="black")
+        lines = hs.plot.markers.Lines(segments=segments, color="black")
         self.add_marker(lines, render_figure=False)
         if render_figure:
             self._render_figure(plot=["signal_plot"])
 
 
 class LazyEDSSpectrum(EDSSpectrum, LazySignal1D):
     """Lazy general signal class for EDS spectra."""
```

### Comparing `exspy-0.1/exspy/signals/eds_sem.py` & `exspy-0.2/exspy/signals/eds_sem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import logging
 
 import traits.api as t
 
 from hyperspy.docstrings.signal import LAZYSIGNAL_DOC
 from hyperspy.signal import BaseSetMetadataItems
@@ -46,15 +46,14 @@
         "Acquisition_instrument.SEM.Detector.EDS.azimuth_angle": "azimuth_angle",
         "Acquisition_instrument.SEM.Detector.EDS.elevation_angle": "elevation_angle",
         "Acquisition_instrument.SEM.Detector.EDS.energy_resolution_MnKa": "energy_resolution_MnKa",
     }
 
 
 class EDSSEMSpectrum(EDSSpectrum):
-
     """Signal class for EDS spectra measured in an SEM."""
 
     _signal_type = "EDS_SEM"
 
     def __init__(self, *args, **kwards):
         super().__init__(*args, **kwards)
         # Attributes defaults
@@ -253,17 +252,15 @@
         >>> s.set_microscope_parameters(energy_resolution_MnKa=135.)
         >>> print('Now set to %s eV' %
         >>>       s.metadata.Acquisition_instrument.
         >>>       SEM.Detector.EDS.energy_resolution_MnKa)
         Default value 130.0 eV
         Now set to 135.0 eV
 
-        """.format(
-        DISPLAY_DT, TOOLKIT_DT
-    )
+        """.format(DISPLAY_DT, TOOLKIT_DT)
 
     def _are_microscope_parameters_missing(self):
         """Check if the EDS parameters necessary for quantification
         are defined in metadata. If not, in interactive mode
         raises an UI item to fill the values
 
         """
@@ -314,11 +311,10 @@
             *args,
             **kwargs,
         )
         return model
 
 
 class LazyEDSSEMSpectrum(EDSSEMSpectrum, LazyEDSSpectrum):
-
     """Lazy signal class for EDS spectra measured in an SEM."""
 
     __doc__ += LAZYSIGNAL_DOC.replace("__BASECLASS__", "EDSSEMSpectrum")
```

### Comparing `exspy-0.1/exspy/signals/eds_tem.py` & `exspy-0.2/exspy/signals/eds_tem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import warnings
 import logging
 
 import traits.api as t
 import numpy as np
@@ -65,15 +65,14 @@
         "Acquisition_instrument.TEM.beam_current": "beam_current",
         "Acquisition_instrument.TEM.probe_area": "probe_area",
         "Acquisition_instrument.TEM.Detector.EDS.real_time": "real_time",
     }
 
 
 class EDSTEMSpectrum(EDSSpectrum):
-
     """Signal class for EDS spectra measured in an TEM."""
 
     _signal_type = "EDS_TEM"
 
     def __init__(self, *args, **kwards):
         super().__init__(*args, **kwards)
         # Attributes defaults
@@ -208,17 +207,15 @@
         >>>       TEM.Detector.EDS.energy_resolution_MnKa)
         >>> s.set_microscope_parameters(energy_resolution_MnKa=135.)
         >>> print(s.metadata.Acquisition_instrument.
         >>>       TEM.Detector.EDS.energy_resolution_MnKa)
         133.312296
         135.0
 
-        """.format(
-        DISPLAY_DT, TOOLKIT_DT
-    )
+        """.format(DISPLAY_DT, TOOLKIT_DT)
 
     def _are_microscope_parameters_missing(self):
         """Check if the EDS parameters necessary for quantification are
         defined in metadata."""
         must_exist = (
             "Acquisition_instrument.TEM.beam_energy",
             "Acquisition_instrument.TEM.Detector.EDS.live_time",
@@ -982,11 +979,10 @@
             # convert density from g/cm3 to kg/m2: factor of 1E3
             elemental_mt = element_composition * thickness_map * density * 1e-8
             mass_thickness += elemental_mt
         return mass_thickness
 
 
 class LazyEDSTEMSpectrum(EDSTEMSpectrum, LazyEDSSpectrum):
-
     """Lazy signal class for EDS spectra measured in an TEM."""
 
     __doc__ += LAZYSIGNAL_DOC.replace("__BASECLASS__", "EDSTEMSpectrum")
```

### Comparing `exspy-0.1/exspy/signals/eels.py` & `exspy-0.2/exspy/signals/eels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numbers
 import logging
 
 import numpy as np
 import dask.array as da
 import traits.api as t
 from scipy import constants
 from prettytable import PrettyTable
-from matplotlib.collections import LineCollection
 
 import hyperspy.api as hs
 from hyperspy.signal import BaseSetMetadataItems, BaseSignal
 from hyperspy._signals.signal1d import Signal1D, LazySignal1D
-import hyperspy.axes
-from hyperspy.components1d import PowerLaw
 from hyperspy.misc.utils import display, isiterable, underline
 from hyperspy.misc.math_tools import optimal_fft_size
 
 from hyperspy.ui_registry import add_gui_method, DISPLAY_DT, TOOLKIT_DT
-from hyperspy.utils.markers import Texts, Lines
 from hyperspy.docstrings.signal1d import (
     CROP_PARAMETER_DOC,
     SPIKES_DIAGNOSIS_DOCSTRING,
     MASK_ZERO_LOSS_PEAK_WIDTH,
     SPIKES_REMOVAL_TOOL_DOCSTRING,
 )
 from hyperspy.docstrings.signal import (
@@ -72,15 +68,14 @@
         "Acquisition_instrument.TEM.convergence_angle": "convergence_angle",
         "Acquisition_instrument.TEM.beam_energy": "beam_energy",
         "Acquisition_instrument.TEM.Detector.EELS.collection_angle": "collection_angle",
     }
 
 
 class EELSSpectrum(Signal1D):
-
     """Signal class for EELS spectra."""
 
     _signal_type = "EELS"
     _alias_signal_types = ["TEM EELS"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -620,18 +615,18 @@
                     # example 1D signal and pretty much always binned. Should
                     # probably at some point be joint
                     ind = ax.value2index(threshold)
                     data = data[:ind]
                     if binned:
                         return data.sum()
                     else:
-                        from scipy.integrate import simps
+                        from scipy.integrate import simpson
 
                         axis = ax.axis[:ind]
-                        return simps(y=data, x=axis)
+                        return simpson(y=data, x=axis)
 
             I0 = self.map(
                 estimating_function,
                 threshold=threshold,
                 ragged=False,
                 show_progressbar=show_progressbar,
                 inplace=False,
@@ -1056,28 +1051,26 @@
         size = ll_size + cl_size - 1
         # Calculate the optimal FFT size
         size = optimal_fft_size(size)
 
         axis = ll.axes_manager.signal_axes[0]
         if fwhm is None:
             fwhm = float(
-                ll.get_current_signal().estimate_peak_width()._get_current_data()
+                ll.get_current_signal().estimate_peak_width()._get_current_data()[0]
             )
             _logger.info("FWHM = %1.2f" % fwhm)
 
         I0 = ll.estimate_elastic_scattering_intensity(threshold=threshold)
         I0 = I0.data
         if ll.axes_manager.navigation_size > 0:
             I0_shape = list(I0.shape)
             I0_shape.insert(axis.index_in_array, 1)
             I0 = I0.reshape(I0_shape)
 
-        from hyperspy.components1d import Gaussian
-
-        g = Gaussian()
+        g = hs.model.components1D.Gaussian()
         g.sigma.value = fwhm / 2.3548
         g.A.value = 1
         g.centre.value = 0
         zl = g.function(
             np.linspace(axis.offset, axis.offset + axis.scale * (size - 1), size)
         )
         z = np.fft.rfft(zl)
@@ -1230,17 +1223,15 @@
             The energy of the electron beam in keV.
         convergence_angle : float
             The microscope convergence semi-angle in mrad.
         collection_angle : float
             The collection semi-angle in mrad.
         {}
         {}
-        """.format(
-        TOOLKIT_DT, DISPLAY_DT
-    )
+        """.format(TOOLKIT_DT, DISPLAY_DT)
 
     def power_law_extrapolation(
         self, window_size=20, extrapolation_size=1024, add_noise=False, fix_neg_r=False
     ):
         """
         Extrapolate the spectrum to the right using a powerlaw.
 
@@ -1287,15 +1278,15 @@
             )
             s.data = da.concatenate([left_data, right_data], axis=axis.index_in_array)
         else:
             # just old code
             s.data = np.zeros(new_shape)
             s.data[..., : axis.size] = self.data
         s.get_dimensions_from_data()
-        pl = PowerLaw()
+        pl = hs.model.components1D.PowerLaw()
         pl._axes_manager = self.axes_manager
         A, r = pl.estimate_parameters(
             s,
             axis.index2value(axis.size - window_size),
             axis.index2value(axis.size - 1),
             out=True,
         )
@@ -1454,15 +1445,15 @@
         self._are_microscope_parameters_missing(ignore_parameters=["convergence_angle"])
         e0 = s.metadata.Acquisition_instrument.TEM.beam_energy
         beta = s.metadata.Acquisition_instrument.TEM.Detector.EELS.collection_angle
 
         axis = s.axes_manager.signal_axes[0]
         eaxis = axis.axis.copy()
 
-        if isinstance(zlp, hyperspy.signal.BaseSignal):
+        if isinstance(zlp, hs.signals.BaseSignal):
             if (
                 zlp.axes_manager.navigation_dimension
                 == self.axes_manager.navigation_dimension
             ):
                 if zlp.axes_manager.signal_dimension == 0:
                     i0 = zlp.data
                 else:
@@ -1480,15 +1471,15 @@
             i0 = zlp
         else:
             raise ValueError(
                 "The zero-loss peak input is not valid, it must be\
                              in the BaseSignal class or a Number."
             )
 
-        if isinstance(t, hyperspy.signal.BaseSignal):
+        if isinstance(t, hs.signals.BaseSignal):
             if (
                 t.axes_manager.navigation_dimension
                 == self.axes_manager.navigation_dimension
             ) and (t.axes_manager.signal_dimension == 0):
                 t = t.data
                 t = t.reshape(np.insert(t.shape, axis.index_in_array, 1))
             else:
@@ -1711,21 +1702,21 @@
         offsets = np.empty((len(index), 2))
         for i, ind in enumerate(index):
             segments[i] = [[ind, 1], [ind, 1.1]]
             offsets[i] = [ind, 1.1]
         return offsets, segments
 
     def _initialise_markers(self):
-        self._edge_markers["lines"] = Lines(
+        self._edge_markers["lines"] = hs.plot.markers.Lines(
             segments=np.empty((0, 2, 2)),
             transform="relative",
             color="black",
             shift=np.array([0.0, 0.19]),
         )
-        self._edge_markers["texts"] = Texts(
+        self._edge_markers["texts"] = hs.plot.markers.Texts(
             offsets=np.empty((0, 2)),
             texts=np.empty((0,)),
             offset_transform="relative",
             rotation=np.pi / 2,
             horizontalalignment="left",
             verticalalignment="bottom",
             facecolor="black",
@@ -1763,15 +1754,15 @@
                     "s.add_elements, or specify elements, edge "
                     "families or edges directly"
                 )
         else:
             extra_element_edge_family.extend(np.atleast_1d(plot_edges))
             try:
                 elements = self.metadata.Sample.elements
-            except:
+            except Exception:
                 elements = []
 
         element_edge_family = elements + extra_element_edge_family
         edges_dict = self._get_edges(element_edge_family, only_edges)
 
         return edges_dict
 
@@ -1975,15 +1966,15 @@
             )
         if out is None:
             return m
         else:
             out.events.data_changed.trigger(obj=out)
         return m
 
-    rebin.__doc__ = hyperspy.signal.BaseSignal.rebin.__doc__
+    rebin.__doc__ = hs.signals.BaseSignal.rebin.__doc__
 
     def vacuum_mask(
         self, threshold=10.0, start_energy=None, closing=True, opening=False
     ):
         """
         Generate mask of the vacuum region
 
@@ -2025,11 +2016,10 @@
         if opening:
             mask.data = binary_erosion(mask.data, border_value=1)
             mask.data = binary_dilation(mask.data, border_value=0)
         return mask
 
 
 class LazyEELSSpectrum(EELSSpectrum, LazySignal1D):
-
     """Lazy signal class for EELS spectra."""
 
     __doc__ += LAZYSIGNAL_DOC.replace("__BASECLASS__", "EELSSpectrum")
```

### Comparing `exspy-0.1/exspy/tests/components/test_EELSarctan.py` & `exspy-0.2/exspy/tests/components/test_EELSarctan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 
 from exspy.components import EELSArctan
 
 
 def test_function():
```

### Comparing `exspy-0.1/exspy/tests/components/test_ceels_cl_edge.py` & `exspy-0.2/exspy/tests/misc/test_eds_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
+import pytest
 
-def test_eels_cl_edge():
-    pass
+from exspy.misc.eds.utils import _get_element_and_line
+
+
+def test_get_element_and_line():
+    assert _get_element_and_line("Mn_Ka") == ("Mn", "Ka")
+
+    with pytest.raises(ValueError):
+        _get_element_and_line("MnKa") == -1
```

### Comparing `exspy-0.1/exspy/tests/components/test_double_power_law.py` & `exspy-0.2/exspy/tests/components/test_double_power_law.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import pytest
 
 import hyperspy.api as hs
 
 from exspy.components import DoublePowerLaw
@@ -46,16 +46,14 @@
 
 class TestDoublePowerLaw:
     def setup_method(self, method):
         s = hs.signals.Signal1D(np.zeros(1024))
         s.axes_manager[0].offset = 100
         s.axes_manager[0].scale = 0.1
         m = s.create_model()
-        exspy = pytest.importorskip("exspy")
-        from exspy.components import DoublePowerLaw
 
         m.append(DoublePowerLaw())
         m[0].A.value = 1000
         m[0].r.value = 4
         m[0].ratio.value = 200
         self.m = m
```

### Comparing `exspy-0.1/exspy/tests/components/test_pes_core_line_shape.py` & `exspy-0.2/exspy/tests/components/test_pes_core_line_shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import pytest
 
 import hyperspy.api as hs
 
 from exspy.components import PESCoreLineShape
```

### Comparing `exspy-0.1/exspy/tests/components/test_pes_see.py` & `exspy-0.2/exspy/tests/components/test_pes_see.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 
 import hyperspy.api as hs
 from hyperspy.misc.test_utils import ignore_warning
 
 from exspy.components import SEE
```

### Comparing `exspy-0.1/exspy/tests/components/test_pes_voigt.py` & `exspy-0.2/exspy/tests/components/test_pes_voigt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import itertools
 
 import numpy as np
 import pytest
 
-from hyperspy.exceptions import VisibleDeprecationWarning
 from hyperspy.signals import Signal1D
 
 from exspy.components import PESVoigt
 
 
 TRUE_FALSE_2_TUPLE = [p for p in itertools.product((True, False), repeat=2)]
 
@@ -57,16 +56,14 @@
 def test_function_spinorbit():
     g = PESVoigt()
     g.area.value = 5
     g.FWHM.value = 0.5
     g.gamma.value = 0.2
     g.centre.value = 1
     g.spin_orbit_splitting = True
-    spin_orbit_branching_ratio = 0.4
-    spin_orbit_splitting_energy = 0.72
     np.testing.assert_allclose(g.function(0), 1.553312)
     np.testing.assert_allclose(g.function(1), 5.612734)
     assert g._position is g.centre
 
 
 def test_function_shirleybackground():
     g = PESVoigt()
```

### Comparing `exspy-0.1/exspy/tests/components/test_volume_plasmon_drude.py` & `exspy-0.2/exspy/tests/components/test_volume_plasmon_drude.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 
 from exspy.components import VolumePlasmonDrude
 
 
 def test_function():
```

### Comparing `exspy-0.1/exspy/tests/data/test_data.py` & `exspy-0.2/exspy/tests/data/test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import pytest
 
 import exspy
 
 
 def test_eds_sem():
```

### Comparing `exspy-0.1/exspy/tests/data/test_eelsdb.py` & `exspy-0.2/exspy/tests/data/test_eelsdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import warnings
 
 import pytest
 import requests
 from requests.exceptions import SSLError
```

### Comparing `exspy-0.1/exspy/tests/drawing/data/Cr_L_cl.hspy` & `exspy-0.2/exspy/tests/drawing/data/Cr_L_cl.hspy`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/tests/drawing/data/Cr_L_ll.hspy` & `exspy-0.2/exspy/tests/drawing/data/Cr_L_ll.hspy`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/tests/drawing/test_plot_model.py` & `exspy-0.2/exspy/tests/drawing/test_plot_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The HyperSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of HyperSpy.
+# This file is part of eXSpy.
 #
-# HyperSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# HyperSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import pytest
 from pathlib import Path
 
 import hyperspy.api as hs
 from hyperspy.components1d import Gaussian
```

### Comparing `exspy-0.1/exspy/tests/drawing/test_plot_spectra_markers.py` & `exspy-0.2/exspy/tests/drawing/test_plot_spectra_markers.py`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/tests/misc/test_eds.py` & `exspy-0.2/exspy/tests/misc/test_eds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 
 from exspy.misc.eds.utils import get_xray_lines_near_energy, take_off_angle
 
 
 def test_xray_lines_near_energy():
```

### Comparing `exspy-0.1/exspy/tests/misc/test_eels.py` & `exspy-0.2/exspy/tests/misc/test_eels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import pytest
 
 from exspy.misc.eels.tools import get_edges_near_energy, get_info_from_edges
 
 
 def test_single_edge():
```

### Comparing `exspy-0.1/exspy/tests/misc/test_gos.py` & `exspy-0.2/exspy/tests/misc/test_gos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from pathlib import Path
 
 import h5py
 import pooch
 import pytest
```

### Comparing `exspy-0.1/exspy/tests/misc/test_material.py` & `exspy-0.2/exspy/tests/misc/test_material.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import pytest
 
 import exspy as ex
 from exspy.misc.elements import elements_db
 import hyperspy.api as hs
```

### Comparing `exspy-0.1/exspy/tests/models/test_edsmodel.py` & `exspy-0.2/exspy/tests/models/test_edsmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import pytest
 
 from hyperspy.decorators import lazifyTestClass
 from hyperspy.misc import utils
```

### Comparing `exspy-0.1/exspy/tests/models/test_eelsmodel.py` & `exspy-0.2/exspy/tests/models/test_eelsmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import contextlib
 import io
 from unittest import mock
 
 import numpy as np
 import pooch
@@ -94,20 +94,20 @@
         assert True in is_pl_instance
 
     def test_auto_add_edges_false(self):
         m = self.s.create_model(auto_background=False)
         from hyperspy.components1d import PowerLaw
 
         is_pl_instance = [isinstance(c, PowerLaw) for c in m]
-        assert not True in is_pl_instance
+        assert True not in is_pl_instance
 
     def test_auto_add_edges_false_names(self):
         m = self.s.create_model(auto_add_edges=False)
         cnames = [component.name for component in m]
-        assert not "B_K" in cnames or "C_K" in cnames
+        assert "B_K" not in cnames or "C_K" in cnames
 
     def test_convolved_ll_not_set(self):
         m = self.s.create_model(auto_add_edges=False)
         with pytest.raises(RuntimeError, match="not set"):
             m.convolved = True
 
     def test_low_loss(self):
@@ -254,15 +254,15 @@
         self.m.signal = s_new
         assert self.m.signal == s_new
 
     def test_signal1d_property_wrong_value_setter(self):
         m = self.m
         s = hs.signals.Signal1D(np.ones(200))
         with pytest.raises(ValueError):
-            self.m.signal = s
+            m.signal = s
 
     def test_remove(self):
         m = self.m
         c_k = m.components.C_K
         assert c_k in m
         m.remove(c_k)
         assert c_k not in m
@@ -582,20 +582,18 @@
         Fe.fine_structure_coeff.free = False
         Fe.fine_structure_spline_active = False
         assert not Fe.fine_structure_coeff.free
         Fe.fine_structure_spline_active = True
         assert not Fe.fine_structure_coeff.free
 
     def test_fine_structure_spline(self):
-        v2i = self.m.signal.axes_manager[0].value2index
         Fe = self.m.components.Fe_L3
         Fe.fine_structure_active = True
         Fe.fine_structure_spline_active = True
         Fe.fine_structure_width = 30
-        onset = Fe.onset_energy.value
         axis1 = np.linspace(
             Fe.onset_energy.value,
             Fe.onset_energy.value + Fe.fine_structure_width,
             endpoint=False,
         )
         assert np.all(Fe.function(axis1) == 0)
         Fe.fine_structure_coeff.value = (
```

### Comparing `exspy-0.1/exspy/tests/models/test_linear_model.py` & `exspy-0.2/exspy/tests/models/test_linear_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import numpy as np
 import pytest
 from hyperspy.decorators import lazifyTestClass
-from hyperspy._components.gaussian import Gaussian
-from hyperspy._components.lorentzian import Lorentzian
 import hyperspy.api as hs
 
 import exspy
 from exspy.signals import EELSSpectrum
 
 
 @lazifyTestClass
@@ -96,16 +94,16 @@
 
 
 class TestWarningSlowMultifit:
     def setup_method(self, method):
         s = hs.data.two_gaussians().inav[0]
         s.set_signal_type("EELS")
         m = s.create_model(auto_background=False, auto_add_edges=False)
-        g1 = Gaussian(centre=40)
-        g2 = Gaussian(centre=55)
+        g1 = hs.model.components1D.Gaussian(centre=40)
+        g2 = hs.model.components1D.Gaussian(centre=55)
         m.extend([g1, g2])
 
         # make dummy twinning
         g2.centre.twin = g1.centre
         g2.centre.twin_function_expr = "15 + x"
         g2.A.twin = g1.A
         g2.centre.twin_function_expr = "2 * x"
@@ -130,60 +128,60 @@
 
     # Create signal to convolve
     to_convolve_component = hs.model.components1D.Gaussian(A=100, sigma=5, centre=10)
     to_convolve = EELSSpectrum(to_convolve_component.function(np.arange(100)))
     to_convolve.axes_manager[-1].offset = -to_convolve_component.centre.value
 
     # Create reference signal from model with convolution
-    l_ref = Lorentzian(A=100, centre=20, gamma=4)
+    l_ref = hs.model.components1D.Lorentzian(A=100, centre=20, gamma=4)
     m_ref = s_ref.create_model(auto_add_edges=False, auto_background=False)
     m_ref.append(l_ref)
     m_ref.low_loss = to_convolve
     s = m_ref.as_signal()
 
     if nav_dim >= 1:
         s = hs.stack([s] * 2)
         to_convolve = hs.stack([to_convolve] * 2)
     if nav_dim == 2:
         s = hs.stack([s] * 3)
         to_convolve = hs.stack([to_convolve] * 3)
 
     m = s.create_model(auto_add_edges=False, auto_background=False)
-    l = Lorentzian(centre=20, gamma=4)
-    m.append(l)
+    lor = hs.model.components1D.Lorentzian(centre=20, gamma=4)
+    m.append(lor)
     assert not m.convolved
     m.low_loss = to_convolve
     assert m.convolved
     m.set_parameters_not_free(only_nonlinear=True)
     with pytest.warns(UserWarning):
         m.multifit(optimizer="lstsq")
 
-    np.testing.assert_allclose(l_ref.A.value, l.A.value)
-    np.testing.assert_allclose(l_ref.centre.value, l.centre.value)
-    np.testing.assert_allclose(l_ref.gamma.value, l.gamma.value)
+    np.testing.assert_allclose(l_ref.A.value, lor.A.value)
+    np.testing.assert_allclose(l_ref.centre.value, lor.centre.value)
+    np.testing.assert_allclose(l_ref.gamma.value, lor.gamma.value)
     np.testing.assert_allclose(m.as_signal().data, s.data)
     if nav_dim in (1, 2):
-        np.testing.assert_allclose(l.A.map["values"].mean(), l_ref.A.value)
-        np.testing.assert_allclose(l.centre.map["values"].mean(), l_ref.centre.value)
-        np.testing.assert_allclose(l.gamma.map["values"].mean(), l_ref.gamma.value)
+        np.testing.assert_allclose(lor.A.map["values"].mean(), l_ref.A.value)
+        np.testing.assert_allclose(lor.centre.map["values"].mean(), l_ref.centre.value)
+        np.testing.assert_allclose(lor.gamma.map["values"].mean(), l_ref.gamma.value)
 
 
 @pytest.mark.parametrize("nav_dim", (0, 1, 2))
 @pytest.mark.parametrize("convolve", (True, False))
 def test_expression_multiple_linear_parameter(nav_dim, convolve):
     """
     This test checks that linear fitting works with convolution with
      - single and multidimensional fit (warning raise)
      - multiple free parameters for the same component (different code path)
     """
     s_ref = EELSSpectrum(np.ones(20))
     p_ref = hs.model.components1D.Polynomial(order=2, a0=25, a1=-50, a2=2.5)
 
     # Create signal to convolve
-    to_convolve_component = Gaussian(A=100, sigma=5, centre=10)
+    to_convolve_component = hs.model.components1D.Gaussian(A=100, sigma=5, centre=10)
     to_convolve = hs.signals.Signal1D(to_convolve_component.function(np.arange(1000)))
     to_convolve.axes_manager[-1].offset = -to_convolve_component.centre.value
 
     m_ref = s_ref.create_model(auto_add_edges=False, auto_background=False)
     m_ref.extend([p_ref])
     if convolve:
         m_ref.low_loss = to_convolve
@@ -220,36 +218,36 @@
 
 
 @pytest.mark.parametrize("nav_dim", (0, 1, 2))
 def test_multiple_linear_parameters_convolution(nav_dim):
     s_ref = EELSSpectrum(np.ones(1000))
 
     # Create signal to convolve
-    to_convolve_component = Gaussian(A=1000, sigma=50, centre=100)
+    to_convolve_component = hs.model.components1D.Gaussian(A=1000, sigma=50, centre=100)
     to_convolve = EELSSpectrum(to_convolve_component.function(np.arange(1000)))
     to_convolve.axes_manager[-1].offset = -to_convolve_component.centre.value
 
-    l_ref1 = Lorentzian(A=100, centre=200, gamma=10)
-    l_ref2 = Lorentzian(A=100, centre=600, gamma=20)
+    l_ref1 = hs.model.components1D.Lorentzian(A=100, centre=200, gamma=10)
+    l_ref2 = hs.model.components1D.Lorentzian(A=100, centre=600, gamma=20)
 
     m_ref = s_ref.create_model(auto_add_edges=False, auto_background=False)
     m_ref.extend([l_ref1, l_ref2])
     m_ref.low_loss = to_convolve
     s = m_ref.as_signal()
 
     if nav_dim >= 1:
         s = hs.stack([s] * 2)
         to_convolve = hs.stack([to_convolve] * 2)
     if nav_dim == 2:
         s = hs.stack([s] * 3)
         to_convolve = hs.stack([to_convolve] * 3)
 
     m = s.create_model(auto_add_edges=False, auto_background=False)
-    l1 = Lorentzian(centre=200, gamma=10)
-    l2 = Lorentzian(centre=600, gamma=20)
+    l1 = hs.model.components1D.Lorentzian(centre=200, gamma=10)
+    l2 = hs.model.components1D.Lorentzian(centre=600, gamma=20)
     m.extend([l1, l2])
     assert not m.convolved
     m.low_loss = to_convolve
     assert m.convolved
     m.set_parameters_not_free(only_nonlinear=True)
     with pytest.warns(UserWarning):
         m.multifit(optimizer="lstsq")
```

### Comparing `exspy-0.1/exspy/tests/signals/data/EELS_LL_linescan_simulated_thickness_variation.hspy` & `exspy-0.2/exspy/tests/signals/data/EELS_LL_linescan_simulated_thickness_variation.hspy`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/tests/signals/data/EELS_ZLP_linescan_simulated_thickness_variation.hspy` & `exspy-0.2/exspy/tests/signals/data/EELS_ZLP_linescan_simulated_thickness_variation.hspy`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/tests/signals/test_assign_subclass.py` & `exspy-0.2/exspy/tests/signals/test_assign_subclass.py`

 * *Files identical despite different names*

### Comparing `exspy-0.1/exspy/tests/signals/test_binned.py` & `exspy-0.2/exspy/tests/signals/test_binned.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
-import numpy as np
 import hyperspy.api as hs
 
 import exspy
 
 
 def test_dielectric_function_binned_default():
     s = exspy.signals.DielectricFunction([0])
```

### Comparing `exspy-0.1/exspy/tests/signals/test_edges_range.py` & `exspy-0.2/exspy/tests/signals/test_edges_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 from copy import deepcopy
 
 import numpy as np
 
 import exspy
 from exspy.signal_tools import EdgesRange
```

### Comparing `exspy-0.1/exspy/tests/signals/test_eds_sem.py` & `exspy-0.2/exspy/tests/signals/test_eds_sem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import pytest
 
 import numpy as np
 
 from hyperspy import utils
 from hyperspy.components1d import Gaussian
```

### Comparing `exspy-0.1/exspy/tests/signals/test_eds_tem.py` & `exspy-0.2/exspy/tests/signals/test_eds_tem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import warnings
 
 import numpy as np
 import pytest
 
 from hyperspy.components1d import Gaussian
```

### Comparing `exspy-0.1/exspy/tests/signals/test_eels.py` & `exspy-0.2/exspy/tests/signals/test_eels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
+import importlib
 
 import numpy as np
 import pytest
 from pathlib import Path
 
 import hyperspy.api as hs
 from hyperspy.decorators import lazifyTestClass
@@ -279,21 +280,19 @@
     with pytest.warns():
         s._spikes_diagnosis(use_gui=False)
 
     hs.preferences.GUIs.enable_traitsui_gui = False
     with pytest.warns():
         s._spikes_diagnosis(use_gui=True)
 
-    hs.preferences.GUIs.enable_traitsui_gui = True
-    try:
-        import hyperspy_gui_traitsui
+    hyperspy_gui_traitsui_spec = importlib.util.find_spec("hyperspy_gui_traitsui")
 
+    if hyperspy_gui_traitsui_spec is None:
+        hs.preferences.GUIs.enable_traitsui_gui = True
         s._spikes_diagnosis(use_gui=True)
-    except ImportError:
-        pass
 
 
 @lazifyTestClass
 class TestPowerLawExtrapolation:
     def setup_method(self, method):
         s = exspy.signals.EELSSpectrum(0.1 * np.arange(50, 250, 0.5) ** -3.0)
         s.axes_manager[-1].is_binned = False
```

### Comparing `exspy-0.1/exspy/tests/signals/test_kramers_kronig_transform.py` & `exspy-0.2/exspy/tests/signals/test_kramers_kronig_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
 import numpy as np
 import pytest
 
 import hyperspy.api as hs
 from hyperspy.components1d import Lorentzian
```

### Comparing `exspy-0.1/exspy/tests/test_non-uniform_not-implemented.py` & `exspy-0.2/exspy/tests/test_non-uniform_not-implemented.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2007-2023 The exSpy developers
+# Copyright 2007-2024 The eXSpy developers
 #
-# This file is part of exSpy.
+# This file is part of eXSpy.
 #
-# exSpy is free software: you can redistribute it and/or modify
+# eXSpy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# exSpy is distributed in the hope that it will be useful,
+# eXSpy is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with exSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
+# along with eXSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import pytest
 
 import exspy
 
 
 def test_eels():
```

### Comparing `exspy-0.1/exspy.egg-info/PKG-INFO` & `exspy-0.2/exspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exspy
-Version: 0.1
+Version: 0.2
 Summary: EELS and EDS analysis with the HyperSpy framework
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,31 +676,28 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <http://www.gnu.org/philosophy/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://hyperspy.org/exspy
 Project-URL: Bug Reports, https://github.com/hyperspy/exspy/issues
 Project-URL: Source, https://github.com/hyperspy/exspy
-Keywords: data analysis,microscopy,electron microscopy,electron energy loss spectroscopy,X-ray energy-dispersive spectroscopy
+Keywords: python,hyperspy,data analysis,microscopy,electron microscopy,electron energy loss spectroscopy,energy-dispersive X-ray spectroscopy,X-ray energy-dispersive spectroscopy,EELS,EDS,EDX,SEM,STEM,TEM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask[array]
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: matplotlib
 Requires-Dist: numexpr
@@ -737,22 +734,30 @@
 Requires-Dist: exspy[gui-jupyter]; extra == "all"
 Requires-Dist: exspy[gui-traitsui]; extra == "all"
 
 
 [![Tests](https://github.com/hyperspy/exspy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/exspy/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/exspy/badge/?version=latest)](https://exspy.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/hyperspy/exspy/graph/badge.svg?token=X7T3LE121Q)](https://codecov.io/gh/hyperspy/exspy)
+[![CodeQL](https://github.com/hyperspy/exspy/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/hyperspy/exspy/actions/workflows/github-code-scanning/codeql)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hyperspy/exspy/main.svg)](https://results.pre-commit.ci/latest/github/hyperspy/exspy/main)
+
+
+[![Python Version](https://img.shields.io/pypi/pyversions/exspy.svg?style=flat)](https://pypi.python.org/pypi/exspy)
+[![PyPi Version](http://img.shields.io/pypi/v/exspy.svg?style=flat)](https://pypi.python.org/pypi/exspy)
+[![Anaconda Version](https://anaconda.org/conda-forge/exspy/badges/version.svg)](https://anaconda.org/conda-forge/exspy)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.10252344.svg)](https://zenodo.org/doi/10.5281/zenodo.10252344)
 
-**exSpy** is a Python package extending the functionality for multi-dimensional
+**eXSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of X-rays Energy Dispersive Spectroscopy (EDS)
 and Electron Energy Loss Spectroscopy (EELS).
 
-Go to the documentation for instructions on how to install exSpy and start an
+Go to the documentation for instructions on how to install eXSpy and start an
 analysis: [Read the docs](https://exspy.readthedocs.io).
 
 Everyone is welcome to contribute. Please read our
 [contributing guidelines](https://github.com/hyperspy/exspy/blob/main/CONTRIBUTING.rst) and get started!
 
-Development of exSpy is documented in the
+Development of eXSpy is documented in the
 [changelog](https://github.com/hyperspy/exspy/blob/main/CHANGES.rst).
```

### Comparing `exspy-0.1/exspy.egg-info/SOURCES.txt` & `exspy-0.2/exspy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,32 +6,38 @@
 LICENSE
 MANIFEST.in
 README.md
 prepare_release.py
 pyproject.toml
 releasing_guide.md
 .github/PULL_REQUEST_TEMPLATE.md
+.github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/custom.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/black.yml
 .github/workflows/docs.yml
 .github/workflows/package_and_test.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 doc/Makefile
 doc/changes.rst
-doc/citing.rst
 doc/conf.py
 doc/contributing.rst
 doc/index.rst
 doc/intro.rst
 doc/make.bat
-doc/_static/hyperspy.ico
-doc/_static/hyperspy_logo.png
+doc/_static/exspy-banner-dark.png
+doc/_static/exspy-banner-dark.svg
+doc/_static/exspy-banner-light.png
+doc/_static/exspy-banner-light.svg
+doc/_static/exspy-logo-dark.png
+doc/_static/exspy-logo-dark.svg
+doc/_static/exspy-logo-light.png
+doc/_static/exspy-logo-light.svg
+doc/_static/exspy.ico
 doc/reference/components.rst
 doc/reference/data.rst
 doc/reference/index.rst
 doc/reference/material.rst
 doc/reference/models.rst
 doc/reference/signals.rst
 doc/user_guide/bibliography.rst
@@ -117,17 +123,19 @@
 exspy/signals/eds.py
 exspy/signals/eds_sem.py
 exspy/signals/eds_tem.py
 exspy/signals/eels.py
 exspy/tests/__init__.py
 exspy/tests/test_non-uniform_not-implemented.py
 exspy/tests/components/__init__.py
+exspy/tests/components/coreloss_spectrum.msa
+exspy/tests/components/lowloss_spectrum.msa
 exspy/tests/components/test_EELSarctan.py
-exspy/tests/components/test_ceels_cl_edge.py
 exspy/tests/components/test_double_power_law.py
+exspy/tests/components/test_eels_cl_edge.py
 exspy/tests/components/test_pes_core_line_shape.py
 exspy/tests/components/test_pes_see.py
 exspy/tests/components/test_pes_voigt.py
 exspy/tests/components/test_volume_plasmon_drude.py
 exspy/tests/data/test_data.py
 exspy/tests/data/test_eelsdb.py
 exspy/tests/drawing/__init__.py
@@ -150,8 +158,9 @@
 exspy/tests/signals/test_binned.py
 exspy/tests/signals/test_edges_range.py
 exspy/tests/signals/test_eds_sem.py
 exspy/tests/signals/test_eds_tem.py
 exspy/tests/signals/test_eels.py
 exspy/tests/signals/test_kramers_kronig_transform.py
 exspy/tests/signals/data/EELS_LL_linescan_simulated_thickness_variation.hspy
-exspy/tests/signals/data/EELS_ZLP_linescan_simulated_thickness_variation.hspy
+exspy/tests/signals/data/EELS_ZLP_linescan_simulated_thickness_variation.hspy
+upcoming_changes/README.rst
```

### Comparing `exspy-0.1/prepare_release.py` & `exspy-0.2/prepare_release.py`

 * *Files identical despite different names*

### Comparing `exspy-0.1/pyproject.toml` & `exspy-0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,43 @@
 
 [project]
 name = "exspy"
 description = "EELS and EDS analysis with the HyperSpy framework"
 requires-python = ">=3.8"
 readme = "README.md"
 keywords=[
+    "python",
+    "hyperspy",
     "data analysis",
     "microscopy",
     "electron microscopy",
     "electron energy loss spectroscopy",
-    "X-ray energy-dispersive spectroscopy"
+    "energy-dispersive X-ray spectroscopy",
+    "X-ray energy-dispersive spectroscopy",
+    "EELS",
+    "EDS",
+    "EDX",
+    "SEM",
+    "STEM",
+    "TEM",
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Topic :: Software Development :: Libraries",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Physics",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
-  "Operating System :: Microsoft :: Windows",
-  "Operating System :: POSIX",
-  "Operating System :: Unix",
-  "Operating System :: MacOS",
 ]
 dependencies = [
   "dask[array]",
   "hyperspy>=2.0rc0",
   "matplotlib",
   "numexpr",
   "numpy",
@@ -110,57 +116,31 @@
 include = ["exspy*"]
 # Excluding rsciio.tests.data folder is done in MANIFEST.in
 # because setuptools doesn't support it in pyproject.toml
 
 [tool.setuptools.package-data]
 "*" = [
   "*hspy",
-  "*.yaml"
+  "*.yaml",
+  "*.msa",
   ]
 
 [tool.setuptools_scm]
 # Presence enables setuptools_scm, the version will be determine at build time from git
 # The version will be updated by the `prepare_release.py` script
-fallback_version = "0.2.dev0"
-
+fallback_version = "0.3.dev0"
 
 [tool.towncrier]
-package_dir = "exspy"
-filename = "CHANGES.rst"
 directory = "upcoming_changes/"
-title_format = "{version} ({project_date})"
+filename = "CHANGES.rst"
 issue_format = "`#{issue} <https://github.com/hyperspy/exspy/issues/{issue}>`_"
-
-  [[tool.towncrier.type]]
-  directory = "new"
-  name = "New features"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "bugfix"
-  name = "Bug Fixes"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "doc"
-  name = "Improved Documentation"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "deprecation"
-  name = "Deprecations"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "enhancements"
-  name = "Enhancements"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "api"
-  name = "API changes"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "maintenance"
-  name = "Maintenance"
-  showcontent = true
+title_format = "{version} ({project_date})"
+package_dir = "exspy"
+type = [
+    { directory = "new", name = "New features", showcontent = true },
+    { directory = "enhancements", name = "Enhancements", showcontent = true },
+    { directory = "bugfix", name = "Bug Fixes", showcontent = true },
+    { directory = "api", name = "API changes", showcontent = true },
+    { directory = "deprecation", name = "Deprecations", showcontent = true },
+    { directory = "doc", name = "Improved Documentation", showcontent = true },
+    { directory = "maintenance", name = "Maintenance", showcontent = true },
+]
```

### Comparing `exspy-0.1/releasing_guide.md` & `exspy-0.2/releasing_guide.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-# Releasing a new exSpy version
+# Releasing a new eXSpy version
 
-To publish a new exSpy release do the following steps:
+To publish a new eXSpy release do the following steps:
 
 ## Preparation
 
 - In a pull request, prepare the release by running the `prepare_release.py` python script (e.g. `python prepare_release.py 0.2`) , which will do the following:
   - update the release notes in `CHANGES.rst` by running `towncrier`,
   - update the `setuptools_scm` fallback version in `pyproject.toml` (for a patch release, this will stay the same).
 - Check release notes
 - Let that PR collect comments for a day to ensure that other maintainers are comfortable
   with releasing
 - Set correct date and version number in `CHANGES.rst`
 
 ## Tag and Release
 
-- Create a tag e.g. `git tag -a v0.1.1 -m "exSpy version 0.1.1"`
+- Create a tag e.g. `git tag -a v0.1.1 -m "eXSpy version 0.1.1"`
 - Push tag to user fork for a test run `git push origin v0.1.1`. Will run the release
   workflow without uploading to PyPi
-- Push tag to exSpy repository to trigger release `git push upstream v0.1.1`
+- Push tag to eXSpy repository to trigger release `git push upstream v0.1.1`
   (this triggers the GitHub action to create the sdist and wheel and upload to
   PyPi automatically). :warning: this is a point of no return :warning:
 
 ## Post-release action
 
-- Update version in other branches if necessary
-- Prepare `CHANGES.rst` for development by adding `UNRELEASED` headline
 - Merge the PR
 
 ## Follow-up
 
 - Tidy up and close corresponding milestone or project
 - A PR to the conda-forge feedstock will be created by the conda-forge bot
```

