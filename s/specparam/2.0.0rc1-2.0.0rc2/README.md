# Comparing `tmp/specparam-2.0.0rc1.tar.gz` & `tmp/specparam-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tom/Code/ModCode/fooof/dist/.tmp-wqs63sl1/specparam-2.0.0rc1.tar", last modified: Wed Mar 27 01:02:13 2024, max compression
+gzip compressed data, was "/Users/tom/Code/ModCode/fooof/dist/.tmp-wle1biv1/specparam-2.0.0rc2.tar", last modified: Wed Apr 10 15:20:27 2024, max compression
```

## Comparing `specparam-2.0.0rc1.tar` & `specparam-2.0.0rc2.tar`

### file list

```diff
@@ -1,141 +1,149 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.752031 specparam-2.0.0rc1/
--rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 specparam-2.0.0rc1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       33 2023-07-22 19:10:52.000000 specparam-2.0.0rc1/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)    13943 2024-03-27 01:02:13.751584 specparam-2.0.0rc1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    12080 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/README.rst
--rw-r--r--   0 tom        (501) staff       (20)       17 2020-05-18 17:32:04.000000 specparam-2.0.0rc1/requirements.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2024-03-27 01:02:13.752102 specparam-2.0.0rc1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2476 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/setup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.690405 specparam-2.0.0rc1/specparam/
--rw-r--r--   0 tom        (501) staff       (20)      226 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.693732 specparam-2.0.0rc1/specparam/analysis/
--rw-r--r--   0 tom        (501) staff       (20)      221 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3938 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/analysis/error.py
--rw-r--r--   0 tom        (501) staff       (20)    10688 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/analysis/periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.695172 specparam-2.0.0rc1/specparam/bands/
--rw-r--r--   0 tom        (501) staff       (20)       50 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4091 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/bands/bands.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.702402 specparam-2.0.0rc1/specparam/core/
--rw-r--r--   0 tom        (501) staff       (20)       37 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      621 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/core/errors.py
--rw-r--r--   0 tom        (501) staff       (20)     5108 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/core/funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     3994 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/core/info.py
--rw-r--r--   0 tom        (501) staff       (20)    10551 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/core/io.py
--rw-r--r--   0 tom        (501) staff       (20)      423 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/core/items.py
--rw-r--r--   0 tom        (501) staff       (20)     2396 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/core/jacobians.py
--rw-r--r--   0 tom        (501) staff       (20)    10401 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/core/modutils.py
--rw-r--r--   0 tom        (501) staff       (20)     7868 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/core/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    21544 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/core/strings.py
--rw-r--r--   0 tom        (501) staff       (20)     7643 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/core/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.704631 specparam-2.0.0rc1/specparam/data/
--rw-r--r--   0 tom        (501) staff       (20)      112 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6149 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/data/conversions.py
--rw-r--r--   0 tom        (501) staff       (20)     4269 2023-09-23 03:08:20.000000 specparam-2.0.0rc1/specparam/data/data.py
--rw-r--r--   0 tom        (501) staff       (20)     7045 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/data/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.708795 specparam-2.0.0rc1/specparam/objs/
--rw-r--r--   0 tom        (501) staff       (20)      372 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    21807 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/objs/event.py
--rw-r--r--   0 tom        (501) staff       (20)    60017 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/objs/fit.py
--rw-r--r--   0 tom        (501) staff       (20)    22206 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/objs/group.py
--rw-r--r--   0 tom        (501) staff       (20)    12996 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/objs/time.py
--rw-r--r--   0 tom        (501) staff       (20)     9621 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/objs/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.718112 specparam-2.0.0rc1/specparam/plts/
--rw-r--r--   0 tom        (501) staff       (20)       77 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10427 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/plts/annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     5632 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)     1972 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/plts/error.py
--rw-r--r--   0 tom        (501) staff       (20)     3843 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/event.py
--rw-r--r--   0 tom        (501) staff       (20)     4212 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/group.py
--rw-r--r--   0 tom        (501) staff       (20)    12122 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/plts/model.py
--rw-r--r--   0 tom        (501) staff       (20)     5986 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     2913 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/settings.py
--rw-r--r--   0 tom        (501) staff       (20)     9093 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/spectra.py
--rw-r--r--   0 tom        (501) staff       (20)    10616 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/plts/style.py
--rw-r--r--   0 tom        (501) staff       (20)    11359 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/templates.py
--rw-r--r--   0 tom        (501) staff       (20)     3470 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/plts/time.py
--rw-r--r--   0 tom        (501) staff       (20)     6698 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/plts/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.721236 specparam-2.0.0rc1/specparam/sim/
--rw-r--r--   0 tom        (501) staff       (20)      247 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     7052 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/sim/gen.py
--rw-r--r--   0 tom        (501) staff       (20)     9899 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/sim/params.py
--rw-r--r--   0 tom        (501) staff       (20)    12293 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/sim/sim.py
--rw-r--r--   0 tom        (501) staff       (20)     9006 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/sim/transform.py
--rw-r--r--   0 tom        (501) staff       (20)      525 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/sim/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.723256 specparam-2.0.0rc1/specparam/tests/
--rw-r--r--   0 tom        (501) staff       (20)       54 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.724674 specparam-2.0.0rc1/specparam/tests/analysis/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1081 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/analysis/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)     2979 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/analysis/test_periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.725339 specparam-2.0.0rc1/specparam/tests/bands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1184 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/bands/test_bands.py
--rw-r--r--   0 tom        (501) staff       (20)     2044 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/conftest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.729957 specparam-2.0.0rc1/specparam/tests/core/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2972 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/tests/core/test_funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     1491 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/core/test_info.py
--rw-r--r--   0 tom        (501) staff       (20)     7838 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/core/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)      938 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/core/test_jacobians.py
--rw-r--r--   0 tom        (501) staff       (20)     3880 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/core/test_modutils.py
--rw-r--r--   0 tom        (501) staff       (20)     1199 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/core/test_reports.py
--rw-r--r--   0 tom        (501) staff       (20)     1530 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/core/test_strings.py
--rw-r--r--   0 tom        (501) staff       (20)     4434 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/core/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.732365 specparam-2.0.0rc1/specparam/tests/data/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3191 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/data/test_conversions.py
--rw-r--r--   0 tom        (501) staff       (20)     1490 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/data/test_data.py
--rw-r--r--   0 tom        (501) staff       (20)     5061 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/data/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.734550 specparam-2.0.0rc1/specparam/tests/objs/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5987 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/objs/test_event.py
--rw-r--r--   0 tom        (501) staff       (20)    14740 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/objs/test_fit.py
--rw-r--r--   0 tom        (501) staff       (20)    11369 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/objs/test_group.py
--rw-r--r--   0 tom        (501) staff       (20)     3559 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/objs/test_time.py
--rw-r--r--   0 tom        (501) staff       (20)     4671 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/tests/objs/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.741108 specparam-2.0.0rc1/specparam/tests/plts/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      881 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/tests/plts/test_annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     1447 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/plts/test_aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)      638 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/plts/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)      769 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/plts/test_event.py
--rw-r--r--   0 tom        (501) staff       (20)     1386 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/plts/test_group.py
--rw-r--r--   0 tom        (501) staff       (20)     1543 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/plts/test_model.py
--rw-r--r--   0 tom        (501) staff       (20)     1090 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/plts/test_periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     4069 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/plts/test_spectra.py
--rw-r--r--   0 tom        (501) staff       (20)     2701 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/plts/test_styles.py
--rw-r--r--   0 tom        (501) staff       (20)     1979 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/plts/test_templates.py
--rw-r--r--   0 tom        (501) staff       (20)      754 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/plts/test_time.py
--rw-r--r--   0 tom        (501) staff       (20)     3351 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/plts/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)      564 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/settings.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.743667 specparam-2.0.0rc1/specparam/tests/sim/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2169 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/tests/sim/test_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4062 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/sim/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)     2646 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/sim/test_sim.py
--rw-r--r--   0 tom        (501) staff       (20)     2515 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/sim/test_transform.py
--rw-r--r--   0 tom        (501) staff       (20)      336 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/sim/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     3647 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/tutils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.747105 specparam-2.0.0rc1/specparam/tests/utils/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5827 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/utils/test_data.py
--rw-r--r--   0 tom        (501) staff       (20)      323 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/utils/test_debug.py
--rw-r--r--   0 tom        (501) staff       (20)     1289 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/utils/test_download.py
--rw-r--r--   0 tom        (501) staff       (20)     2367 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/tests/utils/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)      582 2024-02-15 19:14:27.000000 specparam-2.0.0rc1/specparam/tests/utils/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)      581 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/tests/utils/test_reports.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.749743 specparam-2.0.0rc1/specparam/utils/
--rw-r--r--   0 tom        (501) staff       (20)      123 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    12430 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/utils/data.py
--rw-r--r--   0 tom        (501) staff       (20)      924 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/utils/debug.py
--rw-r--r--   0 tom        (501) staff       (20)     2538 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/utils/download.py
--rw-r--r--   0 tom        (501) staff       (20)     3408 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/utils/io.py
--rw-r--r--   0 tom        (501) staff       (20)     3022 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/utils/params.py
--rw-r--r--   0 tom        (501) staff       (20)     1715 2023-09-23 03:08:21.000000 specparam-2.0.0rc1/specparam/utils/reports.py
--rw-r--r--   0 tom        (501) staff       (20)       24 2024-03-27 00:59:59.000000 specparam-2.0.0rc1/specparam/version.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-27 01:02:13.750408 specparam-2.0.0rc1/specparam.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    13943 2024-03-27 01:02:13.000000 specparam-2.0.0rc1/specparam.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3498 2024-03-27 01:02:13.000000 specparam-2.0.0rc1/specparam.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2024-03-27 01:02:13.000000 specparam-2.0.0rc1/specparam.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      105 2024-03-27 01:02:13.000000 specparam-2.0.0rc1/specparam.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2024-03-27 01:02:13.000000 specparam-2.0.0rc1/specparam.egg-info/top_level.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.714868 specparam-2.0.0rc2/
+-rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 specparam-2.0.0rc2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       33 2023-07-22 19:10:52.000000 specparam-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    16668 2024-04-10 15:20:27.714103 specparam-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    14805 2024-04-09 19:38:42.000000 specparam-2.0.0rc2/README.rst
+-rw-r--r--   0 tom        (501) staff       (20)       17 2020-05-18 17:32:04.000000 specparam-2.0.0rc2/requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2024-04-10 15:20:27.715016 specparam-2.0.0rc2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2476 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.655825 specparam-2.0.0rc2/specparam/
+-rw-r--r--   0 tom        (501) staff       (20)      226 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.658619 specparam-2.0.0rc2/specparam/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)      221 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3938 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/analysis/error.py
+-rw-r--r--   0 tom        (501) staff       (20)    10688 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/analysis/periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.659360 specparam-2.0.0rc2/specparam/bands/
+-rw-r--r--   0 tom        (501) staff       (20)       50 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4091 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/bands/bands.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.663580 specparam-2.0.0rc2/specparam/core/
+-rw-r--r--   0 tom        (501) staff       (20)       37 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      621 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/core/errors.py
+-rw-r--r--   0 tom        (501) staff       (20)     5108 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/core/funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     3994 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/core/info.py
+-rw-r--r--   0 tom        (501) staff       (20)    13796 2024-04-10 13:48:24.000000 specparam-2.0.0rc2/specparam/core/io.py
+-rw-r--r--   0 tom        (501) staff       (20)      423 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/core/items.py
+-rw-r--r--   0 tom        (501) staff       (20)     2396 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/core/jacobians.py
+-rw-r--r--   0 tom        (501) staff       (20)    10401 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/core/modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)     7868 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/core/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    21544 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/core/strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     7643 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/core/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.665536 specparam-2.0.0rc2/specparam/data/
+-rw-r--r--   0 tom        (501) staff       (20)      112 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6149 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/data/conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     4269 2023-09-23 03:08:20.000000 specparam-2.0.0rc2/specparam/data/data.py
+-rw-r--r--   0 tom        (501) staff       (20)     7047 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/data/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.670504 specparam-2.0.0rc2/specparam/objs/
+-rw-r--r--   0 tom        (501) staff       (20)      374 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    26617 2024-04-10 14:06:50.000000 specparam-2.0.0rc2/specparam/objs/algorithm.py
+-rw-r--r--   0 tom        (501) staff       (20)    16984 2024-04-10 14:15:41.000000 specparam-2.0.0rc2/specparam/objs/base.py
+-rw-r--r--   0 tom        (501) staff       (20)    16790 2024-04-10 13:58:17.000000 specparam-2.0.0rc2/specparam/objs/data.py
+-rw-r--r--   0 tom        (501) staff       (20)     8861 2024-04-10 14:16:22.000000 specparam-2.0.0rc2/specparam/objs/event.py
+-rw-r--r--   0 tom        (501) staff       (20)     7282 2024-04-10 04:58:45.000000 specparam-2.0.0rc2/specparam/objs/group.py
+-rw-r--r--   0 tom        (501) staff       (20)    10781 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/objs/model.py
+-rw-r--r--   0 tom        (501) staff       (20)    38223 2024-04-10 14:14:23.000000 specparam-2.0.0rc2/specparam/objs/results.py
+-rw-r--r--   0 tom        (501) staff       (20)     6817 2024-04-10 04:58:45.000000 specparam-2.0.0rc2/specparam/objs/time.py
+-rw-r--r--   0 tom        (501) staff       (20)     9719 2024-04-06 20:15:56.000000 specparam-2.0.0rc2/specparam/objs/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.677204 specparam-2.0.0rc2/specparam/plts/
+-rw-r--r--   0 tom        (501) staff       (20)       77 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    10427 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/plts/annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     5632 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     1972 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/plts/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     3843 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/event.py
+-rw-r--r--   0 tom        (501) staff       (20)     4212 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/group.py
+-rw-r--r--   0 tom        (501) staff       (20)    12122 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/plts/model.py
+-rw-r--r--   0 tom        (501) staff       (20)     5986 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     2913 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)     9093 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)    10616 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/plts/style.py
+-rw-r--r--   0 tom        (501) staff       (20)    11359 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     3470 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/plts/time.py
+-rw-r--r--   0 tom        (501) staff       (20)     6698 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/plts/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.679653 specparam-2.0.0rc2/specparam/sim/
+-rw-r--r--   0 tom        (501) staff       (20)      247 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     7052 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/sim/gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     9899 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/sim/params.py
+-rw-r--r--   0 tom        (501) staff       (20)    12293 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/sim/sim.py
+-rw-r--r--   0 tom        (501) staff       (20)     9006 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/sim/transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      525 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/sim/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.681284 specparam-2.0.0rc2/specparam/tests/
+-rw-r--r--   0 tom        (501) staff       (20)       54 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.682487 specparam-2.0.0rc2/specparam/tests/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1081 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/analysis/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     2979 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/analysis/test_periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.683133 specparam-2.0.0rc2/specparam/tests/bands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1184 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/bands/test_bands.py
+-rw-r--r--   0 tom        (501) staff       (20)     2210 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/conftest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.686905 specparam-2.0.0rc2/specparam/tests/core/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2972 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/tests/core/test_funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     1491 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/core/test_info.py
+-rw-r--r--   0 tom        (501) staff       (20)     8291 2024-04-10 13:48:20.000000 specparam-2.0.0rc2/specparam/tests/core/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)      938 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/core/test_jacobians.py
+-rw-r--r--   0 tom        (501) staff       (20)     3880 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/core/test_modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)     1199 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/core/test_reports.py
+-rw-r--r--   0 tom        (501) staff       (20)     1530 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/core/test_strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     4434 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/tests/core/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.688795 specparam-2.0.0rc2/specparam/tests/data/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3191 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/data/test_conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1490 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/data/test_data.py
+-rw-r--r--   0 tom        (501) staff       (20)     5061 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/data/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.695282 specparam-2.0.0rc2/specparam/tests/objs/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      833 2024-04-06 20:15:56.000000 specparam-2.0.0rc2/specparam/tests/objs/test_algorithm.py
+-rw-r--r--   0 tom        (501) staff       (20)     1886 2024-04-10 04:58:45.000000 specparam-2.0.0rc2/specparam/tests/objs/test_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3048 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/objs/test_data.py
+-rw-r--r--   0 tom        (501) staff       (20)     5987 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/objs/test_event.py
+-rw-r--r--   0 tom        (501) staff       (20)    11369 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/tests/objs/test_group.py
+-rw-r--r--   0 tom        (501) staff       (20)    12986 2024-04-10 13:46:21.000000 specparam-2.0.0rc2/specparam/tests/objs/test_model.py
+-rw-r--r--   0 tom        (501) staff       (20)     3408 2024-04-10 04:58:45.000000 specparam-2.0.0rc2/specparam/tests/objs/test_results.py
+-rw-r--r--   0 tom        (501) staff       (20)     3559 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/objs/test_time.py
+-rw-r--r--   0 tom        (501) staff       (20)     4671 2024-04-10 04:58:53.000000 specparam-2.0.0rc2/specparam/tests/objs/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.701995 specparam-2.0.0rc2/specparam/tests/plts/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      861 2024-04-06 20:15:56.000000 specparam-2.0.0rc2/specparam/tests/plts/test_annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     1447 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/plts/test_aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)      638 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/plts/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)      769 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/plts/test_event.py
+-rw-r--r--   0 tom        (501) staff       (20)     1386 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/plts/test_group.py
+-rw-r--r--   0 tom        (501) staff       (20)     1543 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/plts/test_model.py
+-rw-r--r--   0 tom        (501) staff       (20)     1090 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/plts/test_periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     4069 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/plts/test_spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     2701 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/plts/test_styles.py
+-rw-r--r--   0 tom        (501) staff       (20)     1979 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/plts/test_templates.py
+-rw-r--r--   0 tom        (501) staff       (20)      754 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/plts/test_time.py
+-rw-r--r--   0 tom        (501) staff       (20)     3351 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/plts/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      564 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/settings.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.704619 specparam-2.0.0rc2/specparam/tests/sim/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2139 2024-04-06 20:15:56.000000 specparam-2.0.0rc2/specparam/tests/sim/test_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4062 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/sim/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)     2646 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/sim/test_sim.py
+-rw-r--r--   0 tom        (501) staff       (20)     2515 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/sim/test_transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      336 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/sim/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4027 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/tutils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.707961 specparam-2.0.0rc2/specparam/tests/utils/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5827 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/utils/test_data.py
+-rw-r--r--   0 tom        (501) staff       (20)      323 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/utils/test_debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     1289 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/tests/utils/test_download.py
+-rw-r--r--   0 tom        (501) staff       (20)     2373 2024-04-10 13:48:10.000000 specparam-2.0.0rc2/specparam/tests/utils/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)      562 2024-04-06 20:15:56.000000 specparam-2.0.0rc2/specparam/tests/utils/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)      581 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/tests/utils/test_reports.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.711292 specparam-2.0.0rc2/specparam/utils/
+-rw-r--r--   0 tom        (501) staff       (20)      123 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    12400 2024-04-10 14:11:16.000000 specparam-2.0.0rc2/specparam/utils/data.py
+-rw-r--r--   0 tom        (501) staff       (20)      924 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/utils/debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     2538 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/utils/download.py
+-rw-r--r--   0 tom        (501) staff       (20)     3408 2024-04-09 19:38:43.000000 specparam-2.0.0rc2/specparam/utils/io.py
+-rw-r--r--   0 tom        (501) staff       (20)     3022 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/utils/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     1715 2023-09-23 03:08:21.000000 specparam-2.0.0rc2/specparam/utils/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)       24 2024-04-10 14:20:39.000000 specparam-2.0.0rc2/specparam/version.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-10 15:20:27.711930 specparam-2.0.0rc2/specparam.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    16668 2024-04-10 15:20:27.000000 specparam-2.0.0rc2/specparam.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3746 2024-04-10 15:20:27.000000 specparam-2.0.0rc2/specparam.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2024-04-10 15:20:27.000000 specparam-2.0.0rc2/specparam.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      105 2024-04-10 15:20:27.000000 specparam-2.0.0rc2/specparam.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2024-04-10 15:20:27.000000 specparam-2.0.0rc2/specparam.egg-info/top_level.txt
```

### Comparing `specparam-2.0.0rc1/LICENSE` & `specparam-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/PKG-INFO` & `specparam-2.0.0rc2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specparam
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Spectral parameterization.
 Home-page: https://github.com/fooof-tools/fooof
 Download-URL: https://github.com/fooof-tools/fooof/releases
 Author: The Voytek Lab
 Author-email: voyteklab@gmail.com
 Maintainer: Thomas Donoghue
 Maintainer-email: tdonoghue.research@gmail.com
@@ -72,15 +72,15 @@
 
 .. |Paper| image:: https://img.shields.io/badge/paper-nn10.1038-informational.svg
 .. _Paper: https://doi.org/10.1038/s41593-020-00744-x
 
 
 Spectral parameterization (`specparam`, formerly `fooof`) is a fast, efficient, and physiologically-informed tool to parameterize neural power spectra.
 
-WARNING: this Github repository has been updated to a major update / breaking change from the current release of the `fooof` module, and is no longer consistent with the `fooof` version of the code.
+WARNING: this Github repository has been updated to a major update / breaking change from previous releases, which were under the `fooof` name, and now contains major breaking update for the new `specparam` version of the code. The new version is not fully released, though a test version is available (see installation instructions below).
 
 Overview
 --------
 
 The power spectrum model conceives of a model of the power spectrum as a combination of two distinct functional processes:
 
 - An aperiodic component, reflecting 1/f like characteristics, with
@@ -91,19 +91,47 @@
 
 The benefit of fitting a model in order to measure putative oscillations, is that peaks in the power spectrum are
 characterized in terms of their specific center frequency, power and bandwidth without requiring predefining
 specific bands of interest and controlling for the aperiodic component.
 The model also returns a measure of this aperiodic components of the signal, allowing for measuring and
 comparison of 1/f-like components of the signal within and between subjects.
 
+specparam (upcoming version)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+We are currently in the process of a major update to this tool, that includes a name changes (fooof -> specparam), and full rewrite of the code. This means that the new version will be incompatible with prior versions (in terms of the code having different names, and previous code no longer running as written), though note that the exact same procedures will be available (spectra can be fit in a way expected to give the same results), as well many new features.
+
+The new version is called `specparam` (spectral parameterization). There is a release candidate available for testing (see installation instructions).
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
+The fooof naming scheme, with most recent stable version 1.1 is the current main release, and is fully functional and stable, including everything that was introduced under the fooof name.
+
+Which version should I use?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The previous release version, fooof, is fully functional, and projects that are already using it might as well stick with that, unless any of the new functionality in specparam is particularly important. For projects that are just starting, the new specparam version may be of interest if some of the new features are of interest (e.g. time-resolved estimations), though note that as release candidates, the release are not guaranteed to be stable (future updates may make breaking changes). Note that for the same model and settings, fooof and specparam should be exactly equivalent, so in terms of outputs there should be no difference in choosing one or the other.
+
 Documentation
 -------------
 
+The `specparam` package includes a full set of code documentation.
+
+specparam (upcoming version)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To see the documentation for the candidate 2.0 release, see
+`here <https://specparam-tools.github.io/>`_.
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
 Documentation is available on the
-`documentation site <https://fooof-tools.github.io/fooof/index.html>`_.
+`documentation site <https://fooof-tools.github.io/>`_.
 
 This documentation includes:
 
 - `Motivations <https://fooof-tools.github.io/fooof/auto_motivations/index.html>`_:
   with motivating examples of why we recommend parameterizing neural power spectra
 - `Tutorials <https://fooof-tools.github.io/fooof/auto_tutorials/index.html>`_:
   with a step-by-step guide through the model and how to apply it
@@ -117,15 +145,15 @@
   which defines all the key terms used in the module
 - `Reference <https://fooof-tools.github.io/fooof/reference.html>`_:
   with information for how to reference and report on using the module
 
 Dependencies
 ------------
 
-SpecParam is written in Python, and requires Python >= 3.7 to run.
+`specparam` is written in Python, and requires Python >= 3.7 to run.
 
 It has the following required dependencies:
 
 - `numpy <https://github.com/numpy/numpy>`_
 - `scipy <https://github.com/scipy/scipy>`_ >= 0.19
 
 There are also optional dependencies, which are not required for model fitting itself, but offer extra functionality:
@@ -136,14 +164,34 @@
 - `pytest <https://github.com/pytest-dev/pytest>`_ is needed to run the test suite locally
 
 We recommend using the `Anaconda <https://www.anaconda.com/distribution/>`_ distribution to manage these requirements.
 
 Installation
 ------------
 
+specparam / fooof can be installed using pip.
+
+specparam (test version)
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+To install the current release candidate version for the new 2.0 version, you can do:
+
+.. code-block:: shell
+
+    $ pip install specparam
+
+The above will install the most recent release candidate.
+
+NOTE: specparam is currently available as a 'release candidate', meaning it is not finalized and fully released yet.
+This means it may not yet have all features that the ultimate 2.0 version will include, and things are not strictly
+guaranteed to stay the same (there may be further breaking changes in the ultimate 2.0 release).
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
 The current major release is the 1.X.X series, which is a breaking change from the prior 0.X.X series.
 
 Check the `changelog <https://fooof-tools.github.io/fooof/changelog.html>`_ for notes on updating to the new version.
 
 **Stable Version**
 
 To install the latest stable release, use pip:
@@ -186,15 +234,15 @@
 The original implementation of `specparam`, available in this repository, is implemented in Python.
 
 If you wish to run specparam from another language, there are a couple potential options:
 
 - a `wrapper`, which allows for running the Python code from another language
 - a `reimplementation`, which reflects a new implementation of the specparam algorithm in another language
 
-Below are listed some examples of wrappers and/or reimplementations in other languages (non-exhaustive).
+Below are listed some examples of wrappers and/or re-implementations in other languages (non-exhaustive).
 
 Matlab
 ~~~~~~
 
 In Matlab, there is a reimplementation available in common toolboxes:
 - The `Brainstorm <https://neuroimage.usc.edu/brainstorm/Introduction>`_ toolbox has a reimplementation of specparam (see the `Brainstorm fooof tutorial <https://neuroimage.usc.edu/brainstorm/Tutorials/Fooof>`_)
 - The `Fieldtrip <https://www.fieldtriptoolbox.org/>`_ toolbox also uses the same reimplementation (see the `Fieldtrip fooof tutorial <https://www.fieldtriptoolbox.org/example/fooof/>`_)
```

### Comparing `specparam-2.0.0rc1/README.rst` & `specparam-2.0.0rc2/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 .. |Paper| image:: https://img.shields.io/badge/paper-nn10.1038-informational.svg
 .. _Paper: https://doi.org/10.1038/s41593-020-00744-x
 
 
 Spectral parameterization (`specparam`, formerly `fooof`) is a fast, efficient, and physiologically-informed tool to parameterize neural power spectra.
 
-WARNING: this Github repository has been updated to a major update / breaking change from the current release of the `fooof` module, and is no longer consistent with the `fooof` version of the code.
+WARNING: this Github repository has been updated to a major update / breaking change from previous releases, which were under the `fooof` name, and now contains major breaking update for the new `specparam` version of the code. The new version is not fully released, though a test version is available (see installation instructions below).
 
 Overview
 --------
 
 The power spectrum model conceives of a model of the power spectrum as a combination of two distinct functional processes:
 
 - An aperiodic component, reflecting 1/f like characteristics, with
@@ -43,19 +43,47 @@
 
 The benefit of fitting a model in order to measure putative oscillations, is that peaks in the power spectrum are
 characterized in terms of their specific center frequency, power and bandwidth without requiring predefining
 specific bands of interest and controlling for the aperiodic component.
 The model also returns a measure of this aperiodic components of the signal, allowing for measuring and
 comparison of 1/f-like components of the signal within and between subjects.
 
+specparam (upcoming version)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+We are currently in the process of a major update to this tool, that includes a name changes (fooof -> specparam), and full rewrite of the code. This means that the new version will be incompatible with prior versions (in terms of the code having different names, and previous code no longer running as written), though note that the exact same procedures will be available (spectra can be fit in a way expected to give the same results), as well many new features.
+
+The new version is called `specparam` (spectral parameterization). There is a release candidate available for testing (see installation instructions).
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
+The fooof naming scheme, with most recent stable version 1.1 is the current main release, and is fully functional and stable, including everything that was introduced under the fooof name.
+
+Which version should I use?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The previous release version, fooof, is fully functional, and projects that are already using it might as well stick with that, unless any of the new functionality in specparam is particularly important. For projects that are just starting, the new specparam version may be of interest if some of the new features are of interest (e.g. time-resolved estimations), though note that as release candidates, the release are not guaranteed to be stable (future updates may make breaking changes). Note that for the same model and settings, fooof and specparam should be exactly equivalent, so in terms of outputs there should be no difference in choosing one or the other.
+
 Documentation
 -------------
 
+The `specparam` package includes a full set of code documentation.
+
+specparam (upcoming version)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To see the documentation for the candidate 2.0 release, see
+`here <https://specparam-tools.github.io/>`_.
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
 Documentation is available on the
-`documentation site <https://fooof-tools.github.io/fooof/index.html>`_.
+`documentation site <https://fooof-tools.github.io/>`_.
 
 This documentation includes:
 
 - `Motivations <https://fooof-tools.github.io/fooof/auto_motivations/index.html>`_:
   with motivating examples of why we recommend parameterizing neural power spectra
 - `Tutorials <https://fooof-tools.github.io/fooof/auto_tutorials/index.html>`_:
   with a step-by-step guide through the model and how to apply it
@@ -69,15 +97,15 @@
   which defines all the key terms used in the module
 - `Reference <https://fooof-tools.github.io/fooof/reference.html>`_:
   with information for how to reference and report on using the module
 
 Dependencies
 ------------
 
-SpecParam is written in Python, and requires Python >= 3.7 to run.
+`specparam` is written in Python, and requires Python >= 3.7 to run.
 
 It has the following required dependencies:
 
 - `numpy <https://github.com/numpy/numpy>`_
 - `scipy <https://github.com/scipy/scipy>`_ >= 0.19
 
 There are also optional dependencies, which are not required for model fitting itself, but offer extra functionality:
@@ -88,14 +116,34 @@
 - `pytest <https://github.com/pytest-dev/pytest>`_ is needed to run the test suite locally
 
 We recommend using the `Anaconda <https://www.anaconda.com/distribution/>`_ distribution to manage these requirements.
 
 Installation
 ------------
 
+specparam / fooof can be installed using pip.
+
+specparam (test version)
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+To install the current release candidate version for the new 2.0 version, you can do:
+
+.. code-block:: shell
+
+    $ pip install specparam
+
+The above will install the most recent release candidate.
+
+NOTE: specparam is currently available as a 'release candidate', meaning it is not finalized and fully released yet.
+This means it may not yet have all features that the ultimate 2.0 version will include, and things are not strictly
+guaranteed to stay the same (there may be further breaking changes in the ultimate 2.0 release).
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
 The current major release is the 1.X.X series, which is a breaking change from the prior 0.X.X series.
 
 Check the `changelog <https://fooof-tools.github.io/fooof/changelog.html>`_ for notes on updating to the new version.
 
 **Stable Version**
 
 To install the latest stable release, use pip:
@@ -138,15 +186,15 @@
 The original implementation of `specparam`, available in this repository, is implemented in Python.
 
 If you wish to run specparam from another language, there are a couple potential options:
 
 - a `wrapper`, which allows for running the Python code from another language
 - a `reimplementation`, which reflects a new implementation of the specparam algorithm in another language
 
-Below are listed some examples of wrappers and/or reimplementations in other languages (non-exhaustive).
+Below are listed some examples of wrappers and/or re-implementations in other languages (non-exhaustive).
 
 Matlab
 ~~~~~~
 
 In Matlab, there is a reimplementation available in common toolboxes:
 - The `Brainstorm <https://neuroimage.usc.edu/brainstorm/Introduction>`_ toolbox has a reimplementation of specparam (see the `Brainstorm fooof tutorial <https://neuroimage.usc.edu/brainstorm/Tutorials/Fooof>`_)
 - The `Fieldtrip <https://www.fieldtriptoolbox.org/>`_ toolbox also uses the same reimplementation (see the `Fieldtrip fooof tutorial <https://www.fieldtriptoolbox.org/example/fooof/>`_)
```

### Comparing `specparam-2.0.0rc1/setup.py` & `specparam-2.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/analysis/error.py` & `specparam-2.0.0rc2/specparam/analysis/error.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/analysis/periodic.py` & `specparam-2.0.0rc2/specparam/analysis/periodic.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/bands/bands.py` & `specparam-2.0.0rc2/specparam/bands/bands.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/errors.py` & `specparam-2.0.0rc2/specparam/core/errors.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/funcs.py` & `specparam-2.0.0rc2/specparam/core/funcs.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/info.py` & `specparam-2.0.0rc2/specparam/core/info.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/io.py` & `specparam-2.0.0rc2/specparam/core/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -232,14 +232,133 @@
             if save_data:
                 fg.power_spectra = event.spectrograms[ind, :, :].T
             fg.save(file_name + '_{:0{ndigits}d}'.format(ind, ndigits=ndigits),
                     file_path=file_path, append=append, save_results=save_results,
                     save_settings=save_settings, save_data=save_data)
 
 
+def load_model(file_name, file_path=None, regenerate=True, model=None):
+    """Load a SpectralModel object.
+
+    Parameters
+    ----------
+    Parameters
+    ----------
+    file_name : str
+        File(s) to load data from.
+    file_path : str, optional
+        Path to directory to load from. If None, loads from current directory.
+    regenerate : bool, optional, default: True
+        Whether to regenerate the model fit from the loaded data, if data is available.
+    model : SpectralModel
+        xx
+
+    Returns
+    -------
+    model : SpectralModel
+        Loaded model object with data from file.
+    """
+
+    # Check for model object, import (avoid circular) and initialize if not
+    if not model:
+        from specparam.objs import SpectralModel
+        model = SpectralModel()
+
+    model.load(file_name, file_path, regenerate)
+
+    return model
+
+
+def load_group(file_name, file_path=None, group=None):
+    """Load a SpectralGroupModel object.
+
+    Parameters
+    ----------
+    file_name : str
+        File(s) to load data from.
+    file_path : str, optional
+        Path to directory to load from. If None, loads from current directory.
+    group : SpectralGroupModel
+        xx
+
+    Returns
+    -------
+    group : SpectralGroupModel
+        Loaded model object with data from file.
+    """
+
+    # Check for model object, import (avoid circular) and initialize if not
+    if not group:
+        from specparam.objs import SpectralGroupModel
+        group = SpectralGroupModel()
+
+    group.load(file_name, file_path)
+
+    return group
+
+
+def load_time(file_name, file_path=None, peak_org=None, time=None):
+    """Load a SpectralTimeModel object.
+
+    Parameters
+    ----------
+    file_name : str
+        File(s) to load data from.
+    file_path : str, optional
+        Path to directory to load from. If None, loads from current directory.
+    peak_org : int or Bands, optional
+        How to organize peaks.
+        If int, extracts the first n peaks.
+        If Bands, extracts peaks based on band definitions.
+
+    Returns
+    -------
+    time : SpectralTimeModel
+        Loaded model object with data from file.
+    """
+
+    # Check for model object, import (avoid circular) and initialize if not
+    if not time:
+        from specparam.objs import SpectralTimeModel
+        time = SpectralTimeModel()
+
+    time.load(file_name, file_path, peak_org)
+
+    return time
+
+def load_event(file_name, file_path=None, peak_org=None, event=None):
+    """Load a SpectralTimeEventModel object.
+
+    Parameters
+    ----------
+    file_name : str
+        File(s) to load data from.
+    file_path : str, optional
+        Path to directory to load from. If None, loads from current directory.
+    peak_org : int or Bands, optional
+        How to organize peaks.
+        If int, extracts the first n peaks.
+        If Bands, extracts peaks based on band definitions.
+
+    Returns
+    -------
+    event : SpectralTimeEventModel
+        Loaded model object with data from file.
+    """
+
+    # Check for model object, import (avoid circular) and initialize if not
+    if not event:
+        from specparam.objs import SpectralTimeEventModel
+        event = SpectralTimeEventModel()
+
+    event.load(file_name, file_path, peak_org)
+
+    return event
+
+
 def load_json(file_name, file_path):
     """Load json file.
 
     Parameters
     ----------
     file_name : str or FileObject
         File to load data from.
```

### Comparing `specparam-2.0.0rc1/specparam/core/jacobians.py` & `specparam-2.0.0rc2/specparam/core/jacobians.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/modutils.py` & `specparam-2.0.0rc2/specparam/core/modutils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/reports.py` & `specparam-2.0.0rc2/specparam/core/reports.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/strings.py` & `specparam-2.0.0rc2/specparam/core/strings.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/core/utils.py` & `specparam-2.0.0rc2/specparam/core/utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/data/conversions.py` & `specparam-2.0.0rc2/specparam/data/conversions.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/data/data.py` & `specparam-2.0.0rc2/specparam/data/data.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/data/utils.py` & `specparam-2.0.0rc2/specparam/data/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     if isinstance(col, str):
         col = get_indices(infer_ap_func(fit_results.aperiodic_params))[col]
 
     # Allow for shortcut alias, without adding `_params`
     if name in ['aperiodic', 'peak', 'gaussian']:
         name = name + '_params'
 
-    # Extract the request data field from object
+    # Extract the requested data field from object
     out = getattr(fit_results, name)
 
     # Periodic values can be empty arrays and if so, replace with NaN array
     if isinstance(out, np.ndarray) and out.size == 0:
         out = np.array([np.nan, np.nan, np.nan])
 
     # Select out a specific column, if requested
```

### Comparing `specparam-2.0.0rc1/specparam/objs/time.py` & `specparam-2.0.0rc2/specparam/plts/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,366 +1,311 @@
-"""Time model object and associated code for fitting the model to spectrograms."""
+"""Plots for the model object.
 
-from functools import wraps
+Notes
+-----
+This file contains plotting functions that take as input a model object.
+"""
 
 import numpy as np
 
-from specparam.objs import SpectralModel, SpectralGroupModel
-from specparam.plts.time import plot_time_model
-from specparam.data.conversions import group_to_dict, group_to_dataframe, dict_to_df
-from specparam.data.utils import get_results_by_ind
-from specparam.core.utils import check_inds
-from specparam.core.reports import save_time_report
-from specparam.core.modutils import (copy_doc_func_to_method, docs_get_section,
-                                     replace_docstring_sections)
-from specparam.core.strings import gen_time_results_str
+from specparam.core.utils import nearest_ind
+from specparam.core.modutils import safe_import, check_dependency
+from specparam.sim.gen import gen_periodic
+from specparam.utils.data import trim_spectrum
+from specparam.utils.params import compute_fwhm
+from specparam.plts.spectra import plot_spectra
+from specparam.plts.settings import PLT_FIGSIZES, PLT_COLORS
+from specparam.plts.utils import check_ax, check_plot_kwargs, savefig
+from specparam.plts.style import style_spectrum_plot, style_plot
+
+plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
-def transpose_arg1(func):
-    """Decorator function to transpose the 1th argument input to a function."""
-
-    @wraps(func)
-    def decorated(*args, **kwargs):
-
-        if len(args) >= 2:
-            args = list(args)
-            args[2] = args[2].T if isinstance(args[2], np.ndarray) else args[2]
-        if 'spectrogram' in kwargs:
-            kwargs['spectrogram'] = kwargs['spectrogram'].T
-
-        return func(*args, **kwargs)
-
-    return decorated
-
-
-@replace_docstring_sections([docs_get_section(SpectralModel.__doc__, 'Parameters'),
-                             docs_get_section(SpectralModel.__doc__, 'Notes')])
-class SpectralTimeModel(SpectralGroupModel):
-    """Model a spectrogram as a combination of aperiodic and periodic components.
-
-    WARNING: frequency and power values inputs must be in linear space.
-
-    Passing in logged frequencies and/or power spectra is not detected,
-    and will silently produce incorrect results.
+@savefig
+@style_plot
+@check_dependency(plt, 'matplotlib')
+def plot_model(model, plot_peaks=None, plot_aperiodic=True, freqs=None, power_spectrum=None,
+               freq_range=None, plt_log=False, add_legend=True, ax=None, data_kwargs=None,
+               model_kwargs=None, aperiodic_kwargs=None, peak_kwargs=None, **plot_kwargs):
+    """Plot the power spectrum and model fit results from a model object.
 
     Parameters
     ----------
-    %copied in from SpectralModel object
-
-    Attributes
-    ----------
-    freqs : 1d array
-        Frequency values for the spectrogram.
-    spectrogram : 2d array
-        Power values for the spectrogram, as [n_freqs, n_time_windows].
-        Power values are stored internally in log10 scale.
-    freq_range : list of [float, float]
-        Frequency range of the spectrogram, as [lowest_freq, highest_freq].
-    freq_res : float
-        Frequency resolution of the spectrogram.
-    time_results : dict
-        Results of the model fit across each time window.
+    model : SpectralModel
+        Object containing a power spectrum and (optionally) results from fitting.
+    plot_peaks : None or {'shade', 'dot', 'outline', 'line'}, optional
+        What kind of approach to take to plot peaks. If None, peaks are not specifically plotted.
+        Can also be a combination of approaches, separated by '-', for example: 'shade-line'.
+    plot_aperiodic : boolean, optional, default: True
+        Whether to plot the aperiodic component of the model fit.
+    freqs : 1d array, optional
+        Frequency values of the power spectrum to plot, in linear space.
+        If provided, this overrides the values in the model object.
+    power_spectrum : 1d array, optional
+        Power values to plot, in linear space.
+        If provided, this overrides the values in the model object.
+    freq_range : list of [float, float], optional
+        Frequency range to plot, defined in linear space.
+    plt_log : boolean, optional, default: False
+        Whether to plot the frequency values in log10 spacing.
+    add_legend : boolean, optional, default: False
+        Whether to add a legend describing the plot components.
+    ax : matplotlib.Axes, optional
+        Figure axes upon which to plot.
+    data_kwargs, model_kwargs, aperiodic_kwargs, peak_kwargs : None or dict, optional
+        Keyword arguments to pass into the plot call for each plot element.
+    **plot_kwargs
+        Additional plot related keyword arguments, with styling options managed by ``style_plot``.
 
     Notes
     -----
-    %copied in from SpectralModel object
-    - The time object inherits from the group model, which in turn inherits from the
-      model object. As such it also has data attributes defined on the model object,
-      as well as additional attributes that are added to the group object (see notes
-      and attribute list in SpectralGroupModel).
-    - Notably, while this object organizes the results into the `time_results`
-      attribute, which may include sub-selecting peaks per band (depending on settings)
-      the `group_results` attribute is also available, which maintains the full
-      model results.
+    The y-axis (power) is plotted in log spacing by default.
     """
 
-    def __init__(self, *args, **kwargs):
-        """Initialize object with desired settings."""
-
-        SpectralGroupModel.__init__(self, *args, **kwargs)
-
-        self._reset_time_results()
-
-
-    def __getitem__(self, ind):
-        """Allow for indexing into the object to select fit results for a specific time window."""
-
-        return get_results_by_ind(self.time_results, ind)
-
-
-    @property
-    def n_peaks_(self):
-        """How many peaks were fit for each model."""
-
-        return [res.peak_params.shape[0] for res in self.group_results] \
-            if self.has_model else None
-
-
-    @property
-    def n_time_windows(self):
-        """How many time windows are included in the model object."""
-
-        return self.spectrogram.shape[1] if self.has_data else 0
-
-
-    def _reset_time_results(self):
-        """Set, or reset, time results to be empty."""
-
-        self.time_results = {}
-
-
-    @property
-    def spectrogram(self):
-        """Data attribute view on the power spectra, transposed to spectrogram orientation."""
-
-        return self.power_spectra.T
+    ax = check_ax(ax, plot_kwargs.pop('figsize', PLT_FIGSIZES['spectral']))
 
+    # Check inputs for what to plot
+    custom_spectrum = (np.any(freqs) and np.any(power_spectrum))
 
-    @transpose_arg1
-    def add_data(self, freqs, spectrogram, freq_range=None):
-        """Add data (frequencies and spectrogram values) to the current object.
+    # Log settings - note that power values in model objects are already logged
+    log_freqs = plt_log
+    log_powers = False
+
+    # Plot the data, if available
+    if model.has_data or custom_spectrum:
+        data_defaults = {'color' : PLT_COLORS['data'], 'linewidth' : 2.0,
+                         'label' : 'Original Spectrum' if add_legend else None}
+        data_kwargs = check_plot_kwargs(data_kwargs, data_defaults)
+        plot_spectra(freqs if custom_spectrum else model.freqs,
+                     power_spectrum if custom_spectrum else model.power_spectrum,
+                     log_freqs, log_powers if not custom_spectrum else True,
+                     freq_range, ax=ax, **data_kwargs)
+
+    # Add the full model fit, and components (if requested)
+    if model.has_model:
+        model_defaults = {'color' : PLT_COLORS['model'], 'linewidth' : 3.0, 'alpha' : 0.5,
+                          'label' : 'Full Model Fit' if add_legend else None}
+        model_kwargs = check_plot_kwargs(model_kwargs, model_defaults)
+        plot_spectra(model.freqs, model.modeled_spectrum_,
+                     log_freqs, log_powers, ax=ax, **model_kwargs)
+
+        # Plot the aperiodic component of the model fit
+        if plot_aperiodic:
+            aperiodic_defaults = {'color' : PLT_COLORS['aperiodic'], 'linewidth' : 3.0,
+                                  'alpha' : 0.5, 'linestyle' : 'dashed',
+                                  'label' : 'Aperiodic Fit' if add_legend else None}
+            aperiodic_kwargs = check_plot_kwargs(aperiodic_kwargs, aperiodic_defaults)
+            plot_spectra(model.freqs, model._ap_fit,
+                         log_freqs, log_powers, ax=ax, **aperiodic_kwargs)
+
+        # Plot the periodic components of the model fit
+        if plot_peaks:
+            _add_peaks(model, plot_peaks, plt_log, ax, peak_kwargs)
 
-        Parameters
-        ----------
-        freqs : 1d array
-            Frequency values for the spectrogram, in linear space.
-        spectrogram : 2d array, shape=[n_freqs, n_time_windows]
-            Matrix of power values, in linear space.
-        freq_range : list of [float, float], optional
-            Frequency range to restrict spectrogram to. If not provided, keeps the entire range.
+    # Apply default style to plot
+    style_spectrum_plot(ax, log_freqs, True)
 
-        Notes
-        -----
-        If called on an object with existing data and/or results
-        these will be cleared by this method call.
-        """
 
-        if np.any(self.freqs):
-            self._reset_time_results()
-        super().add_data(freqs, spectrogram, freq_range)
-
-
-    def report(self, freqs=None, spectrogram=None, freq_range=None,
-               peak_org=None, report_type='time', n_jobs=1, progress=None):
-        """Fit a spectrogram and display a report, with a plot and printed results.
-
-        Parameters
-        ----------
-        freqs : 1d array, optional
-            Frequency values for the spectrogram, in linear space.
-        spectrogram : 2d array, shape: [n_freqs, n_time_windows], optional
-            Spectrogram of power spectrum values, in linear space.
-        freq_range : list of [float, float], optional
-            Frequency range to fit the model to. If not provided, fits the entire given range.
-        peak_org : int or Bands
-            How to organize peaks.
-            If int, extracts the first n peaks.
-            If Bands, extracts peaks based on band definitions.
-        n_jobs : int, optional, default: 1
-            Number of jobs to run in parallel.
-            1 is no parallelization. -1 uses all available cores.
-        progress : {None, 'tqdm', 'tqdm.notebook'}, optional
-            Which kind of progress bar to use. If None, no progress bar is used.
-
-        Notes
-        -----
-        Data is optional, if data has already been added to the object.
-        """
-
-        self.fit(freqs, spectrogram, freq_range, peak_org, n_jobs=n_jobs, progress=progress)
-        self.plot(report_type)
-        self.print_results(report_type)
+def _add_peaks(model, approach, plt_log, ax, peak_kwargs):
+    """Add peaks to a model plot.
 
+    Parameters
+    ----------
+    model : SpectralModel
+        Model object containing results from fitting.
+    approach : {'shade', 'dot', 'outline', 'outline', 'line'}
+        What kind of approach to take to plot peaks.
+        Can also be a combination of approaches, separated by '-' (for example 'shade-line').
+    plt_log : boolean, optional, default: False
+        Whether to plot the frequency values in log10 spacing.
+    ax : matplotlib.Axes
+        Figure axes upon which to plot.
+    peak_kwargs : None or dict
+        Keyword arguments to pass into the plot call.
+        This can be a flat dictionary, with plot keyword arguments,
+        or a dictionary of dictionaries, with keys as labels indicating an `approach`,
+        and values which contain a dictionary of plot keywords for that approach.
 
-    def fit(self, freqs=None, spectrogram=None, freq_range=None, peak_org=None,
-            n_jobs=1, progress=None):
-        """Fit a spectrogram.
+    Notes
+    -----
+    This is a pass through function, that takes a specification of one
+    or multiple add peak approaches to use, and calls the relevant function(s).
+    """
 
-        Parameters
-        ----------
-        freqs : 1d array, optional
-            Frequency values for the spectrogram, in linear space.
-        spectrogram : 2d array, shape: [n_freqs, n_time_windows], optional
-            Spectrogram of power spectrum values, in linear space.
-        freq_range : list of [float, float], optional
-            Frequency range to fit the model to. If not provided, fits the entire given range.
-        peak_org : int or Bands
-            How to organize peaks.
-            If int, extracts the first n peaks.
-            If Bands, extracts peaks based on band definitions.
-        n_jobs : int, optional, default: 1
-            Number of jobs to run in parallel.
-            1 is no parallelization. -1 uses all available cores.
-        progress : {None, 'tqdm', 'tqdm.notebook'}, optional
-            Which kind of progress bar to use. If None, no progress bar is used.
+    # Input for kwargs could be None, so check if dict and typecast if not
+    peak_kwargs = peak_kwargs if isinstance(peak_kwargs, dict) else {}
 
-        Notes
-        -----
-        Data is optional, if data has already been added to the object.
-        """
+    # Split up approaches, in case multiple are specified, and apply each
+    for cur_approach in approach.split('-'):
 
-        super().fit(freqs, spectrogram, freq_range, n_jobs, progress)
-        if peak_org is not False:
-            self.convert_results(peak_org)
+        try:
 
+            # This unpacks kwargs, if it's embedded dictionaries for each approach
+            plot_kwargs = peak_kwargs.get(cur_approach, peak_kwargs)
 
-    def drop(self, inds):
-        """Drop one or more model fit results from the object.
+            # Pass through to the peak plotting function
+            ADD_PEAK_FUNCS[cur_approach](model, plt_log, ax, **plot_kwargs)
 
-        Parameters
-        ----------
-        inds : int or array_like of int or array_like of bool
-            Indices to drop model fit results for.
+        except KeyError:
+            raise ValueError("Plot peak type not understood.")
 
-        Notes
-        -----
-        This method sets the model fits as null, and preserves the shape of the model fits.
-        """
 
-        super().drop(inds)
-        for key in self.time_results.keys():
-            self.time_results[key][inds] = np.nan
+def _add_peaks_shade(model, plt_log, ax, **plot_kwargs):
+    """Add a shading in of all peaks.
 
+    Parameters
+    ----------
+    model : SpectralModel
+        Model object containing results from fitting.
+    plt_log : boolean
+        Whether to plot the frequency values in log10 spacing.
+    ax : matplotlib.Axes
+        Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into ``fill_between``.
+    """
 
-    def get_results(self):
-        """Return the results run across a spectrogram."""
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.25}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-        return self.time_results
+    for peak in model.gaussian_params_:
 
+        peak_freqs = np.log10(model.freqs) if plt_log else model.freqs
+        peak_line = model._ap_fit + gen_periodic(model.freqs, peak)
 
-    def get_group(self, inds, output_type='time'):
-        """Get a new model object with the specified sub-selection of model fits.
+        ax.fill_between(peak_freqs, peak_line, model._ap_fit, **plot_kwargs)
 
-        Parameters
-        ----------
-        inds : array_like of int or array_like of bool
-            Indices to extract from the object.
-        output_type : {'time', 'group'}, optional
-            Type of model object to extract:
-                'time' : SpectralTimeObject
-                'group' : SpectralGroupObject
 
-        Returns
-        -------
-        output : SpectralTimeModel or SpectralGroupModel
-            The requested selection of results data loaded into a new model object.
-        """
+def _add_peaks_dot(model, plt_log, ax, **plot_kwargs):
+    """Add a short line, from aperiodic to peak, with a dot at the top.
 
-        if output_type == 'time':
+    Parameters
+    ----------
+    model : SpectralModel
+        Model object containing results from fitting.
+    plt_log : boolean
+        Whether to plot the frequency values in log10 spacing.
+    ax : matplotlib.Axes
+        Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the plot call.
+    """
 
-            # Initialize a new model object, with same settings as current object
-            output = SpectralTimeModel(*self.get_settings(), verbose=self.verbose)
-            output.add_meta_data(self.get_meta_data())
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.6, 'lw' : 2.5, 'ms' : 6}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-            if inds is not None:
+    for peak in model.peak_params_:
 
-                # Check and convert indices encoding to list of int
-                inds = check_inds(inds)
+        ap_point = np.interp(peak[0], model.freqs, model._ap_fit)
+        freq_point = np.log10(peak[0]) if plt_log else peak[0]
 
-                # Add data for specified power spectra, if available
-                if self.has_data:
-                    output.power_spectra = self.power_spectra[inds, :]
+        # Add the line from the aperiodic fit up the tip of the peak
+        ax.plot([freq_point, freq_point], [ap_point, ap_point + peak[1]], **plot_kwargs)
 
-                # Add results for specified power spectra
-                output.group_results = [self.group_results[ind] for ind in inds]
-                output.time_results = get_results_by_ind(self.time_results, inds)
+        # Add an extra dot at the tip of the peak
+        ax.plot(freq_point, ap_point + peak[1], marker='o', **plot_kwargs)
 
-        if output_type == 'group':
-            output = super().get_group(inds)
 
-        return output
+def _add_peaks_outline(model, plt_log, ax, **plot_kwargs):
+    """Add an outline of each peak.
 
+    Parameters
+    ----------
+    model : SpectralModel
+        Model object containing results from fitting.
+    plt_log : boolean
+        Whether to plot the frequency values in log10 spacing.
+    ax : matplotlib.Axes
+        Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the plot call.
+    """
 
-    def print_results(self, print_type='time', concise=False):
-        """Print out SpectralTimeModel results.
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.7, 'lw' : 1.5}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-        Parameters
-        ----------
-        print_type : {'time', 'group'}
-            Which format to print results out in.
-        concise : bool, optional, default: False
-            Whether to print the report in a concise mode, or not.
-        """
+    for peak in model.gaussian_params_:
 
-        if print_type == 'time':
-            print(gen_time_results_str(self, concise))
-        if print_type == 'group':
-            super().print_results(concise)
+        # Define the frequency range around each peak to plot - peak bandwidth +/- 3
+        peak_range = [peak[0] - peak[2]*3, peak[0] + peak[2]*3]
 
+        # Generate a peak reconstruction for each peak, and trim to desired range
+        peak_line = model._ap_fit + gen_periodic(model.freqs, peak)
+        peak_freqs, peak_line = trim_spectrum(model.freqs, peak_line, peak_range)
 
-    @copy_doc_func_to_method(plot_time_model)
-    def plot(self, plot_type='time', save_fig=False, file_name=None, file_path=None, **plot_kwargs):
+        # Plot the peak outline
+        peak_freqs = np.log10(peak_freqs) if plt_log else peak_freqs
+        ax.plot(peak_freqs, peak_line, **plot_kwargs)
 
-        if plot_type == 'time':
-            plot_time_model(self, save_fig=save_fig, file_name=file_name,
-                            file_path=file_path, **plot_kwargs)
-        if plot_type == 'group':
-            super().plot(save_fig=save_fig, file_name=file_name, file_path=file_path, **plot_kwargs)
 
+def _add_peaks_line(model, plt_log, ax, **plot_kwargs):
+    """Add a long line, from the top of the plot, down through the peak, with an arrow at the top.
 
-    @copy_doc_func_to_method(save_time_report)
-    def save_report(self, file_name, file_path=None, add_settings=True):
+    Parameters
+    ----------
+    model : SpectralModel
+        Model object containing results from fitting.
+    plt_log : boolean
+        Whether to plot the frequency values in log10 spacing.
+    ax : matplotlib.Axes
+        Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the plot call.
+    """
 
-        save_time_report(self, file_name, file_path, add_settings)
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.7, 'lw' : 1.4, 'ms' : 10}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
+    ylims = ax.get_ylim()
 
-    def load(self, file_name, file_path=None, peak_org=None):
-        """Load time data from file.
+    for peak in model.peak_params_:
 
-        Parameters
-        ----------
-        file_name : str
-            File to load data from.
-        file_path : str, optional
-            Path to directory to load from. If None, loads from current directory.
-        peak_org : int or Bands
-            How to organize peaks.
-            If int, extracts the first n peaks.
-            If Bands, extracts peaks based on band definitions.
-        """
+        freq_point = np.log10(peak[0]) if plt_log else peak[0]
+        ax.plot([freq_point, freq_point], ylims, '-', **plot_kwargs)
+        ax.plot(freq_point, ylims[1], 'v', **plot_kwargs)
 
-        # Clear results so as not to have possible prior results interfere
-        self._reset_time_results()
-        super().load(file_name, file_path=file_path)
-        if peak_org is not False and self.group_results:
-            self.convert_results(peak_org)
 
+def _add_peaks_width(model, plt_log, ax, **plot_kwargs):
+    """Add a line across the width of peaks.
 
-    def to_df(self, peak_org=None):
-        """Convert and extract the model results as a pandas object.
+    Parameters
+    ----------
+    model : SpectralModel
+        Model object containing results from fitting.
+    plt_log : boolean
+        Whether to plot the frequency values in log10 spacing.
+    ax : matplotlib.Axes
+        Figure axes upon which to plot.
+    **plot_kwargs
+        Keyword arguments to pass into the plot call.
 
-        Parameters
-        ----------
-        peak_org : int or Bands, optional
-            How to organize peaks.
-            If int, extracts the first n peaks.
-            If Bands, extracts peaks based on band definitions.
-            If provided, re-extracts peak features; if not provided, converts from `time_results`.
+    Notes
+    -----
+    This line represents the bandwidth (width or gaussian standard deviation) of
+    the peak, though what is literally plotted is the full-width half-max.
+    """
 
-        Returns
-        -------
-        pd.DataFrame
-            Model results organized into a pandas object.
-        """
+    defaults = {'color' : PLT_COLORS['periodic'], 'alpha' : 0.6, 'lw' : 2.5, 'ms' : 6}
+    plot_kwargs = check_plot_kwargs(plot_kwargs, defaults)
 
-        if peak_org is not None:
-            df = group_to_dataframe(self.group_results, peak_org)
-        else:
-            df = dict_to_df(self.get_results())
+    for peak in model.gaussian_params_:
 
-        return df
+        peak_top = model.power_spectrum[nearest_ind(model.freqs, peak[0])]
+        bw_freqs = [peak[0] - 0.5 * compute_fwhm(peak[2]),
+                    peak[0] + 0.5 * compute_fwhm(peak[2])]
 
+        if plt_log:
+            bw_freqs = np.log10(bw_freqs)
 
-    def convert_results(self, peak_org):
-        """Convert the model results to be organized across time windows.
+        ax.plot(bw_freqs, [peak_top-(0.5*peak[1]), peak_top-(0.5*peak[1])], **plot_kwargs)
 
-        Parameters
-        ----------
-        peak_org : int or Bands
-            How to organize peaks.
-            If int, extracts the first n peaks.
-            If Bands, extracts peaks based on band definitions.
-        """
 
-        self.time_results = group_to_dict(self.group_results, peak_org)
+# Collect all the possible `add_peak_*` functions together
+ADD_PEAK_FUNCS = {
+    'shade' : _add_peaks_shade,
+    'dot' : _add_peaks_dot,
+    'outline' : _add_peaks_outline,
+    'line' : _add_peaks_line,
+    'width' : _add_peaks_width
+}
```

### Comparing `specparam-2.0.0rc1/specparam/objs/utils.py` & `specparam-2.0.0rc2/specparam/objs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,17 @@
                 temp_power_spectra = np.vstack([temp_power_spectra, m_obj.power_spectrum])
 
     # If the number of collected power spectra is consistent, then add them to object
     if len(group) == temp_power_spectra.shape[0]:
         group.power_spectra = temp_power_spectra
 
     # Set the check data mode, as True if any of the inputs have it on, False otherwise
-    group.set_check_data_mode(any(getattr(m_obj, '_check_data') for m_obj in model_objs))
+    group.set_check_modes(\
+        check_freqs=any(getattr(m_obj, '_check_freqs') for m_obj in model_objs),
+        check_data=any(getattr(m_obj, '_check_data') for m_obj in model_objs))
 
     # Add data information information
     group.add_meta_data(model_objs[0].get_meta_data())
 
     return group
```

### Comparing `specparam-2.0.0rc1/specparam/plts/annotate.py` & `specparam-2.0.0rc2/specparam/plts/annotate.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/aperiodic.py` & `specparam-2.0.0rc2/specparam/plts/aperiodic.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/error.py` & `specparam-2.0.0rc2/specparam/plts/error.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/event.py` & `specparam-2.0.0rc2/specparam/plts/event.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/group.py` & `specparam-2.0.0rc2/specparam/plts/group.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/periodic.py` & `specparam-2.0.0rc2/specparam/plts/periodic.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/settings.py` & `specparam-2.0.0rc2/specparam/plts/settings.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/spectra.py` & `specparam-2.0.0rc2/specparam/plts/spectra.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/style.py` & `specparam-2.0.0rc2/specparam/plts/style.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/templates.py` & `specparam-2.0.0rc2/specparam/plts/templates.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/time.py` & `specparam-2.0.0rc2/specparam/plts/time.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/plts/utils.py` & `specparam-2.0.0rc2/specparam/plts/utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/sim/gen.py` & `specparam-2.0.0rc2/specparam/sim/gen.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/sim/params.py` & `specparam-2.0.0rc2/specparam/sim/params.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/sim/sim.py` & `specparam-2.0.0rc2/specparam/sim/sim.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/sim/transform.py` & `specparam-2.0.0rc2/specparam/sim/transform.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/sim/utils.py` & `specparam-2.0.0rc2/specparam/sim/utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/analysis/test_error.py` & `specparam-2.0.0rc2/specparam/tests/analysis/test_error.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/analysis/test_periodic.py` & `specparam-2.0.0rc2/specparam/tests/analysis/test_periodic.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/bands/test_bands.py` & `specparam-2.0.0rc2/specparam/tests/bands/test_bands.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/conftest.py` & `specparam-2.0.0rc2/specparam/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 import shutil
 import pytest
 
 import numpy as np
 
 from specparam.core.modutils import safe_import
-from specparam.tests.tutils import (get_tfm, get_tfg, get_tft, get_tfe, get_tbands,
-                                    get_tresults, get_tdocstring)
+from specparam.tests.tutils import (get_tdata, get_tdata2d, get_tfm, get_tfg, get_tft, get_tfe,
+                                    get_tbands, get_tresults, get_tdocstring)
 from specparam.tests.settings import (BASE_TEST_FILE_PATH, TEST_DATA_PATH,
                                       TEST_REPORTS_PATH, TEST_PLOTS_PATH)
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
@@ -33,14 +33,22 @@
     # Remake (empty) directories
     os.mkdir(BASE_TEST_FILE_PATH)
     os.mkdir(TEST_DATA_PATH)
     os.mkdir(TEST_REPORTS_PATH)
     os.mkdir(TEST_PLOTS_PATH)
 
 @pytest.fixture(scope='session')
+def tdata():
+    yield get_tdata()
+
+@pytest.fixture(scope='session')
+def tdata2d():
+    yield get_tdata2d()
+
+@pytest.fixture(scope='session')
 def tfm():
     yield get_tfm()
 
 @pytest.fixture(scope='session')
 def tfg():
     yield get_tfg()
```

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_funcs.py` & `specparam-2.0.0rc2/specparam/tests/core/test_funcs.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_info.py` & `specparam-2.0.0rc2/specparam/tests/core/test_info.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_io.py` & `specparam-2.0.0rc2/specparam/tests/core/test_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,45 +37,45 @@
     out2 = get_files('.', 'search')
     assert isinstance(out2, list)
 
 def test_save_model_str(tfm):
     """Check saving model object data, with file specifiers as strings."""
 
     # Test saving out each set of save elements
-    file_name_res = 'test_res'
-    file_name_set = 'test_set'
-    file_name_dat = 'test_dat'
+    file_name_res = 'test_model_res'
+    file_name_set = 'test_model_set'
+    file_name_dat = 'test_model_dat'
 
     save_model(tfm, file_name_res, TEST_DATA_PATH, False, True, False, False)
     save_model(tfm, file_name_set, TEST_DATA_PATH, False, False, True, False)
     save_model(tfm, file_name_dat, TEST_DATA_PATH, False, False, False, True)
 
     assert os.path.exists(TEST_DATA_PATH / (file_name_res + '.json'))
     assert os.path.exists(TEST_DATA_PATH / (file_name_set + '.json'))
     assert os.path.exists(TEST_DATA_PATH / (file_name_dat + '.json'))
 
     # Test saving out all save elements
-    file_name_all = 'test_all'
+    file_name_all = 'test_model_all'
     save_model(tfm, file_name_all, TEST_DATA_PATH, False, True, True, True)
     assert os.path.exists(TEST_DATA_PATH / (file_name_all + '.json'))
 
 def test_save_model_append(tfm):
     """Check saving fm data, appending to a file."""
 
-    file_name = 'test_append'
+    file_name = 'test_model_append'
 
     save_model(tfm, file_name, TEST_DATA_PATH, True, True, True, True)
     save_model(tfm, file_name, TEST_DATA_PATH, True, True, True, True)
 
     assert os.path.exists(TEST_DATA_PATH / (file_name + '.json'))
 
 def test_save_model_fobj(tfm):
     """Check saving fm data, with file object file specifier."""
 
-    file_name = 'test_fileobj'
+    file_name = 'test_model_fileobj'
 
     # Save, using file-object: three successive lines with three possible save settings
     with open(TEST_DATA_PATH / (file_name + '.json'), 'w') as f_obj:
         save_model(tfm, f_obj, TEST_DATA_PATH, False, True, False, False)
         save_model(tfm, f_obj, TEST_DATA_PATH, False, False, True, False)
         save_model(tfm, f_obj, TEST_DATA_PATH, False, False, False, True)
 
@@ -159,31 +159,51 @@
 
     # Test saving out all save elements
     file_name_all = 'test_event_all'
     save_event(tfe, file_name_all, TEST_DATA_PATH, False, True, True, True)
     for ind in range(len(tfe)):
         assert os.path.exists(TEST_DATA_PATH / (file_name_all + '_' + str(ind) + '.json'))
 
+def test_load_model():
+
+    tmodel = load_model('test_model_all', TEST_DATA_PATH)
+    assert tmodel
+
+def test_load_group():
+
+    tgroup = load_group('test_group_all', TEST_DATA_PATH)
+    assert tgroup
+
+def test_load_time():
+
+    ttime = load_time('test_time_all', TEST_DATA_PATH)
+    assert ttime
+
+def test_load_event():
+
+    tevent = load_event('test_event_all', TEST_DATA_PATH)
+    assert tevent
+
 def test_load_json_str():
     """Test loading JSON file, with str file specifier.
     Loads files from test_save_model_str.
     """
 
-    file_name = 'test_all'
+    file_name = 'test_model_all'
 
     data = load_json(file_name, TEST_DATA_PATH)
 
     assert data
 
 def test_load_json_fobj():
     """Test loading JSON file, with file object file specifier.
     Loads files from test_save_model_str.
     """
 
-    file_name = 'test_all'
+    file_name = 'test_model_all'
 
     with open(TEST_DATA_PATH / (file_name + '.json'), 'r') as f_obj:
         data = load_json(f_obj, '')
 
     assert data
 
 def test_load_jsonlines():
@@ -197,15 +217,15 @@
         assert data
 
 def test_load_file_contents():
     """Check that loaded files contain the contents they should.
     Note that is this test fails, it likely stems from an issue from saving.
     """
 
-    file_name = 'test_all'
+    file_name = 'test_model_all'
     loaded_data = load_json(file_name, TEST_DATA_PATH)
 
     # Check settings
     for setting in OBJ_DESC['settings']:
         assert setting in loaded_data.keys()
 
     # Check results
```

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_jacobians.py` & `specparam-2.0.0rc2/specparam/tests/core/test_jacobians.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_modutils.py` & `specparam-2.0.0rc2/specparam/tests/core/test_modutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,42 +106,42 @@
     assert 'new note' in new_docstring
 
 def test_copy_doc_func_to_method(tdocstring):
 
     def tfunc(): pass
     tfunc.__doc__ = tdocstring
 
-    class tObj():
+    class tobj():
 
         @copy_doc_func_to_method(tfunc)
         def tmethod():
             pass
 
-    assert tObj.tmethod.__doc__
-    assert 'first' not in tObj.tmethod.__doc__
-    assert 'second' in tObj.tmethod.__doc__
+    assert tobj.tmethod.__doc__
+    assert 'first' not in tobj.tmethod.__doc__
+    assert 'second' in tobj.tmethod.__doc__
 
 
 def test_copy_doc_class(tdocstring):
 
-    class tObj1():
+    class tobj1():
         pass
-    tObj1.__doc__ = tdocstring
+    tobj1.__doc__ = tdocstring
 
     new_section = \
     """
     third : stuff
         Words, words, words.
     """
-    @copy_doc_class(tObj1, 'Parameters', new_section)
-    class tObj2():
+    @copy_doc_class(tobj1, 'Parameters', new_section)
+    class tobj2():
         pass
 
-    assert 'third' in tObj2.__doc__
-    assert 'third' not in tObj1.__doc__
+    assert 'third' in tobj2.__doc__
+    assert 'third' not in tobj1.__doc__
 
 def test_replace_docstring_sections(tdocstring):
 
     # Extract just the parameters section from general test docstring
     new_parameters = '\n'.join(tdocstring.split('\n')[2:8])
 
     @replace_docstring_sections(new_parameters)
```

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_reports.py` & `specparam-2.0.0rc2/specparam/tests/core/test_reports.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_strings.py` & `specparam-2.0.0rc2/specparam/tests/core/test_strings.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/core/test_utils.py` & `specparam-2.0.0rc2/specparam/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/data/test_conversions.py` & `specparam-2.0.0rc2/specparam/tests/data/test_conversions.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/data/test_data.py` & `specparam-2.0.0rc2/specparam/tests/data/test_data.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/data/test_utils.py` & `specparam-2.0.0rc2/specparam/tests/data/test_utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/objs/test_event.py` & `specparam-2.0.0rc2/specparam/tests/objs/test_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 def test_event_model():
     """Check event object initializes properly."""
 
     # Note: doesn't assert the object itself, which returns false empty
     fe = SpectralTimeEventModel(verbose=False)
     assert isinstance(fe, SpectralTimeEventModel)
 
-def test_event_getitem(tft):
+def test_event_getitem(tfe):
 
-    assert tft[0]
+    assert tfe[0]
 
 def test_event_iter(tfe):
 
     for out in tfe:
         assert out
 
 def test_event_n_peaks(tfe):
```

### Comparing `specparam-2.0.0rc1/specparam/tests/objs/test_fit.py` & `specparam-2.0.0rc2/specparam/tests/objs/test_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Tests for specparam.objs.fit, including the model object and it's methods.
+"""Tests for specparam.objs.model, including the model object and it's methods.
 
 NOTES
 -----
 The tests here are not strong tests for accuracy.
 They serve rather as 'smoke tests', for if anything fails completely.
 """
 
 import numpy as np
 from pytest import raises
 
 from specparam.core.items import OBJ_DESC
 from specparam.core.errors import FitError
 from specparam.core.utils import group_three
 from specparam.sim import gen_freqs, sim_power_spectrum
-from specparam.data import ModelSettings, SpectrumMetaData, FitResults
+from specparam.data import FitResults
 from specparam.core.modutils import safe_import
 from specparam.core.errors import DataError, NoDataError, InconsistentDataError
 
 pd = safe_import('pandas')
 
 from specparam.tests.settings import TEST_DATA_PATH
-from specparam.tests.tutils import get_tfm, plot_test
+from specparam.tests.tutils import default_spectrum_params, get_tfm, plot_test
 
-from specparam.objs.fit import *
+from specparam.objs.model import *
 
 ###################################################################################################
 ###################################################################################################
 
 def test_model_object():
     """Check model object initializes properly."""
 
@@ -71,19 +71,16 @@
     # Check model results - gaussian parameters
     for ii, gauss in enumerate(group_three(gauss_params)):
         assert np.allclose(gauss, tfm.gaussian_params_[ii], [2.0, 0.5, 1.0])
 
 def test_fit_nk_noise():
     """Test fit on noisy data, to make sure nothing breaks."""
 
-    ap_params = [50, 2]
-    gauss_params = [10, 0.5, 2, 20, 0.3, 4]
     nlv = 1.0
-
-    xs, ys = sim_power_spectrum([3, 50], ap_params, gauss_params, nlv)
+    xs, ys = sim_power_spectrum(*default_spectrum_params(), nlv=nlv)
 
     tfm = SpectralModel(max_n_peaks=8, verbose=False)
     tfm.fit(xs, ys)
 
     # No accuracy checking here - just checking that it ran
     assert tfm.has_model
 
@@ -130,16 +127,15 @@
         tfm._calc_error(metric='BAD')
 
 def test_checks():
     """Test various checks, errors and edge cases for model fitting.
     This tests all the input checking done in `_prepare_data`.
     """
 
-    xs, ys = sim_power_spectrum([3, 50], [50, 2], [10, 0.5, 2])
-
+    xs, ys = sim_power_spectrum(*default_spectrum_params())
     tfm = SpectralModel(verbose=False)
 
     ## Check checks & errors done in `_prepare_data`
 
     # Check wrong data type error
     with raises(DataError):
         tfm.fit(list(xs), list(ys))
@@ -156,15 +152,15 @@
     with raises(DataError):
         tfm.fit(xs, ys.astype('complex'))
 
     # Check trim_spectrum range
     tfm.fit(xs, ys, [3, 40])
 
     # Check freq of 0 issue
-    xs, ys = sim_power_spectrum([3, 50], [50, 2], [10, 0.5, 2])
+    xs, ys = sim_power_spectrum(*default_spectrum_params())
     tfm.fit(xs, ys)
     assert tfm.freqs[0] != 0
 
     # Check error for `check_freqs` - for if there is non-even frequency values
     with raises(DataError):
         tfm.fit(np.array([1, 2, 4]), np.array([1, 2, 3]))
 
@@ -182,51 +178,51 @@
         tfm.fit()
 
 def test_load():
     """Test loading data into model object. Note: loads files from test_core_io."""
 
     # Test loading just results
     tfm = SpectralModel(verbose=False)
-    file_name_res = 'test_res'
+    file_name_res = 'test_model_res'
     tfm.load(file_name_res, TEST_DATA_PATH)
     # Check that result attributes get filled
     for result in OBJ_DESC['results']:
         assert not np.all(np.isnan(getattr(tfm, result)))
     # Test that settings and data are None
     #   Except for aperiodic mode, which can be inferred from the data
     for setting in OBJ_DESC['settings']:
         if setting != 'aperiodic_mode':
             assert getattr(tfm, setting) is None
     assert getattr(tfm, 'power_spectrum') is None
 
     # Test loading just settings
     tfm = SpectralModel(verbose=False)
-    file_name_set = 'test_set'
+    file_name_set = 'test_model_set'
     tfm.load(file_name_set, TEST_DATA_PATH)
     for setting in OBJ_DESC['settings']:
         assert getattr(tfm, setting) is not None
     # Test that results and data are None
     for result in OBJ_DESC['results']:
         assert np.all(np.isnan(getattr(tfm, result)))
     assert tfm.power_spectrum is None
 
     # Test loading just data
     tfm = SpectralModel(verbose=False)
-    file_name_dat = 'test_dat'
+    file_name_dat = 'test_model_dat'
     tfm.load(file_name_dat, TEST_DATA_PATH)
     assert tfm.power_spectrum is not None
     # Test that settings and results are None
     for setting in OBJ_DESC['settings']:
         assert getattr(tfm, setting) is None
     for result in OBJ_DESC['results']:
         assert np.all(np.isnan(getattr(tfm, result)))
 
     # Test loading all elements
     tfm = SpectralModel(verbose=False)
-    file_name_all = 'test_all'
+    file_name_all = 'test_model_all'
     tfm.load(file_name_all, TEST_DATA_PATH)
     for result in OBJ_DESC['results']:
         assert not np.all(np.isnan(getattr(tfm, result)))
     for setting in OBJ_DESC['settings']:
         assert getattr(tfm, setting) is not None
     for data in OBJ_DESC['data']:
         assert getattr(tfm, data) is not None
@@ -257,88 +253,40 @@
 
     # Test that prior data does get cleared, when requesting not to clear
     tfm._reset_data_results(True, True, True)
     tfm.add_data(freqs, pows, clear_results=True)
     assert tfm.has_data
     assert not tfm.has_model
 
-def test_add_settings():
-    """Tests method to add settings to model object."""
-
-    # This test uses it's own model object, to not add stuff to the global one
-    tfm = get_tfm()
-
-    # Test adding settings
-    settings = ModelSettings([1, 4], 6, 0, 2, 'fixed')
-    tfm.add_settings(settings)
-    for setting in OBJ_DESC['settings']:
-        assert getattr(tfm, setting) == getattr(settings, setting)
-
-def test_add_meta_data():
-    """Tests method to add meta data to model object."""
-
-    # This test uses it's own model object, to not add stuff to the global one
-    tfm = get_tfm()
-
-    # Test adding meta data
-    meta_data = SpectrumMetaData([3, 40], 0.5)
-    tfm.add_meta_data(meta_data)
-    for meta_dat in OBJ_DESC['meta_data']:
-        assert getattr(tfm, meta_dat) == getattr(meta_data, meta_dat)
-
-def test_add_results():
-    """Tests method to add results to model object."""
-
-    # This test uses it's own model object, to not add stuff to the global one
-    tfm = get_tfm()
-
-    # Test adding results
-    results = FitResults([1, 1], [10, 0.5, 0.5], 0.95, 0.02, [10, 0.5, 0.25])
-    tfm.add_results(results)
-    assert tfm.has_model
-    for setting in OBJ_DESC['results']:
-        assert getattr(tfm, setting) == getattr(results, setting.strip('_'))
-
-def test_obj_gets(tfm):
-    """Tests methods that return data objects.
-
-    Checks: get_settings, get_meta_data, get_results
-    """
+def test_get_params(tfm):
+    """Test the get_params method."""
 
-    settings = tfm.get_settings()
-    assert isinstance(settings, ModelSettings)
-    meta_data = tfm.get_meta_data()
-    assert isinstance(meta_data, SpectrumMetaData)
-    results = tfm.get_results()
-    assert isinstance(results, FitResults)
+    for dname in ['aperiodic_params', 'aperiodic', 'peak_params', 'peak',
+                  'error', 'r_squared', 'gaussian_params', 'gaussian']:
+        assert np.any(tfm.get_params(dname))
 
-def test_get_components(tfm):
+        if dname == 'aperiodic_params' or dname == 'aperiodic':
+            for dtype in ['offset', 'exponent']:
+                assert np.any(tfm.get_params(dname, dtype))
+
+        if dname == 'peak_params' or dname == 'peak':
+            for dtype in ['CF', 'PW', 'BW']:
+                assert np.any(tfm.get_params(dname, dtype))
 
-    # Make sure test object has been fit
-    tfm.fit()
+def test_get_data(tfm):
 
-    # Test get data & model components
     for comp in ['full', 'aperiodic', 'peak']:
         for space in ['log', 'linear']:
             assert isinstance(tfm.get_data(comp, space), np.ndarray)
-            assert isinstance(tfm.get_model(comp, space), np.ndarray)
-
-def test_get_params(tfm):
-    """Test the get_params method."""
-
-    for dname in ['aperiodic', 'peak', 'error', 'r_squared']:
-        assert np.any(tfm.get_params(dname))
-
-def test_copy():
-    """Test copy model object method."""
 
-    tfm = SpectralModel(verbose=False)
-    ntfm = tfm.copy()
+def test_get_model(tfm):
 
-    assert tfm != ntfm
+    for comp in ['full', 'aperiodic', 'peak']:
+        for space in ['log', 'linear']:
+            assert isinstance(tfm.get_model(comp, space), np.ndarray)
 
 def test_prints(tfm):
     """Test methods that print (alias and pass through methods).
 
     Checks: print_settings, print_results, print_report_issue.
     """
 
@@ -368,67 +316,63 @@
         assert np.all(np.isnan(getattr(tfm, field)))
     assert tfm.freqs is None and tfm.modeled_spectrum_ is None
 
 def test_report(skip_if_no_mpl):
     """Check that running the top level model method runs."""
 
     tfm = SpectralModel(verbose=False)
-
-    tfm.report(*sim_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
+    tfm.report(*sim_power_spectrum(*default_spectrum_params()))
 
     assert tfm
 
 def test_fit_failure():
     """Test model fit failures."""
 
     ## Induce a runtime error, and check it runs through
     tfm = SpectralModel(verbose=False)
-    tfm._maxfev = 2
+    tfm._maxfev = 5
 
-    tfm.fit(*sim_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
+    tfm.fit(*sim_power_spectrum(*default_spectrum_params()))
 
     # Check after failing out of fit, all results are reset
     for result in OBJ_DESC['results']:
         assert np.all(np.isnan(getattr(tfm, result)))
 
     ## Monkey patch to check errors in general
     #  This mimics the main fit-failure, without requiring bad data / waiting for it to fail.
     tfm = SpectralModel(verbose=False)
     def raise_runtime_error(*args, **kwargs):
         raise FitError('Test-MonkeyPatch')
     tfm._fit_peaks = raise_runtime_error
 
     # Run a model fit - this should raise an error, but continue in try/except
-    tfm.fit(*sim_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
+    tfm.fit(*sim_power_spectrum(*default_spectrum_params()))
 
     # Check after failing out of fit, all results are reset
     for result in OBJ_DESC['results']:
         assert np.all(np.isnan(getattr(tfm, result)))
 
 def test_debug():
     """Test model object in debug mode, including with fit failures."""
 
     tfm = SpectralModel(verbose=False)
-    tfm._maxfev = 2
+    tfm._maxfev = 5
 
     tfm.set_debug_mode(True)
     assert tfm._debug is True
 
     with raises(FitError):
-        tfm.fit(*sim_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
+        tfm.fit(*sim_power_spectrum(*default_spectrum_params()))
 
-def test_set_check_modes(tfm):
+def test_set_check_modes():
     """Test changing check_modes using set_check_modes, and that checks get turned off.
     Note that testing for checks raising errors happens in test_checks.`"""
 
     tfm = SpectralModel(verbose=False)
-
     tfm.set_check_modes(False, False)
-    assert tfm._check_freqs is False
-    assert tfm._check_data is False
 
     # Add bad frequency data, with check freqs turned off
     freqs = np.array([1, 2, 4])
     powers = np.array([1, 2, 3])
     tfm.add_data(freqs, powers)
     assert tfm.has_data
 
@@ -443,20 +387,13 @@
     assert not tfm.has_model
 
     # Reset check modes to true
     tfm.set_check_modes(True, True)
     assert tfm._check_freqs is True
     assert tfm._check_data is True
 
-def test_set_run_modes():
-
-    tfm = SpectralModel(verbose=False)
-    tfm.set_run_modes(False, False, False)
-    for field in OBJ_DESC['run_modes']:
-        assert getattr(tfm, field) is False
-
 def test_to_df(tfm, tbands, skip_if_no_pandas):
 
     df1 = tfm.to_df(2)
     assert isinstance(df1, pd.Series)
     df2 = tfm.to_df(tbands)
     assert isinstance(df2, pd.Series)
```

### Comparing `specparam-2.0.0rc1/specparam/tests/objs/test_group.py` & `specparam-2.0.0rc2/specparam/tests/objs/test_group.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/objs/test_time.py` & `specparam-2.0.0rc2/specparam/tests/objs/test_time.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/objs/test_utils.py` & `specparam-2.0.0rc2/specparam/tests/objs/test_utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_annotate.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_annotate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Tests for specparam.plts.annotate."""
 
-import numpy as np
-
 from specparam.tests.tutils import plot_test
 from specparam.tests.settings import TEST_PLOTS_PATH
 
 from specparam.plts.annotate import *
 
 ###################################################################################################
 ###################################################################################################
```

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_aperiodic.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_aperiodic.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_error.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_error.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_event.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_event.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_group.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_group.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_model.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_model.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_periodic.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_periodic.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_spectra.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_spectra.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_styles.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_styles.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_templates.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_templates.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_time.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_time.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/plts/test_utils.py` & `specparam-2.0.0rc2/specparam/tests/plts/test_utils.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/settings.py` & `specparam-2.0.0rc2/specparam/tests/settings.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/sim/test_gen.py` & `specparam-2.0.0rc2/specparam/tests/sim/test_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Test functions for specparam.sim.gen"""
 
 import numpy as np
-from numpy import array_equal
 
 from specparam.sim.gen import *
 
 ###################################################################################################
 ###################################################################################################
 
 def test_gen_freqs():
```

### Comparing `specparam-2.0.0rc1/specparam/tests/sim/test_params.py` & `specparam-2.0.0rc2/specparam/tests/sim/test_params.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/sim/test_sim.py` & `specparam-2.0.0rc2/specparam/tests/sim/test_sim.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/sim/test_transform.py` & `specparam-2.0.0rc2/specparam/tests/sim/test_transform.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/tutils.py` & `specparam-2.0.0rc2/specparam/tests/tutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,45 +4,53 @@
 
 import numpy as np
 
 from specparam.bands import Bands
 from specparam.data import FitResults
 from specparam.objs import (SpectralModel, SpectralGroupModel,
                             SpectralTimeModel, SpectralTimeEventModel)
+from specparam.objs.data import BaseData, BaseData2D
 from specparam.core.modutils import safe_import
 from specparam.sim.params import param_sampler
 from specparam.sim.sim import sim_power_spectrum, sim_group_power_spectra, sim_spectrogram
 
 plt = safe_import('.pyplot', 'matplotlib')
 
 ###################################################################################################
 ###################################################################################################
 
-def get_tfm():
-    """Get a model object, with a fit power spectrum, for testing."""
+def get_tdata():
 
-    freq_range = [3, 50]
-    ap_params = [50, 2]
-    gaussian_params = [10, 0.5, 2, 20, 0.3, 4]
+    tdata = BaseData()
+    tdata.add_data(*sim_power_spectrum(*default_spectrum_params()))
+
+    return tdata
 
-    xs, ys = sim_power_spectrum(freq_range, ap_params, gaussian_params)
+def get_tdata2d():
+
+    n_spectra = 3
+    tdata2d = BaseData2D()
+    tdata2d.add_data(*sim_group_power_spectra(n_spectra, *default_group_params()))
+
+    return tdata2d
+
+def get_tfm():
+    """Get a model object, with a fit power spectrum, for testing."""
 
     tfm = SpectralModel(verbose=False)
-    tfm.fit(xs, ys)
+    tfm.fit(*sim_power_spectrum(*default_spectrum_params()))
 
     return tfm
 
 def get_tfg():
     """Get a group object, with some fit power spectra, for testing."""
 
     n_spectra = 3
-    xs, ys = sim_group_power_spectra(n_spectra, *default_group_params())
-
     tfg = SpectralGroupModel(verbose=False)
-    tfg.fit(xs, ys)
+    tfg.fit(*sim_group_power_spectra(n_spectra, *default_group_params()))
 
     return tfg
 
 def get_tft():
     """Get a time object, with some fit power spectra, for testing."""
 
     n_spectra = 3
@@ -97,14 +105,22 @@
     -------
     out : yay
         Words, words, words.
     """
 
     return docstring
 
+def default_spectrum_params():
+
+    freq_range = [3, 50]
+    ap_params = [1, 1]
+    gaussian_params = [10, 0.5, 2, 20, 0.3, 4]
+
+    return freq_range, ap_params, gaussian_params
+
 def default_group_params():
     """Create default parameters for simulating a test group of power spectra."""
 
     freq_range = [3, 50]
     ap_opts = param_sampler([[20, 2], [50, 2.5], [35, 1.5]])
     gauss_opts = param_sampler([[10, 0.5, 2], [10, 0.5, 2, 20, 0.3, 4]])
```

### Comparing `specparam-2.0.0rc1/specparam/tests/utils/test_data.py` & `specparam-2.0.0rc2/specparam/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/utils/test_download.py` & `specparam-2.0.0rc2/specparam/tests/utils/test_download.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/tests/utils/test_io.py` & `specparam-2.0.0rc2/specparam/tests/utils/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from specparam.utils.io import *
 
 ###################################################################################################
 ###################################################################################################
 
 def test_load_model():
 
-    file_name = 'test_all'
+    file_name = 'test_model_all'
 
     tfm = load_model(file_name, TEST_DATA_PATH)
 
     assert isinstance(tfm, SpectralModel)
 
     # Check that all elements get loaded
     for result in OBJ_DESC['results']:
```

### Comparing `specparam-2.0.0rc1/specparam/tests/utils/test_params.py` & `specparam-2.0.0rc2/specparam/tests/utils/test_params.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Test functions for specparam.utils.params."""
 
-import numpy as np
-
 from specparam.utils.params import *
 
 ###################################################################################################
 ###################################################################################################
 
 def test_compute_knee_frequency():
```

### Comparing `specparam-2.0.0rc1/specparam/tests/utils/test_reports.py` & `specparam-2.0.0rc2/specparam/tests/utils/test_reports.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/utils/data.py` & `specparam-2.0.0rc2/specparam/utils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     """Compute data presence (as number of non-NaN values) from an array of data.
 
     Parameters
     ----------
     data : 1d or 2d array
         Data array to check presence of.
     average : bool, optional, default: False
-        Whether to average across . Only used for 2d array inputs.
-        If False, for 2d array, the output is an array matching the length of the 0th dimension of the input.
-        If True, for 2d arrays, the output is a single value averaged across the whole array.
+        Whether to average across. Only used for 2d array inputs.
+        If False, the output is an array matching the length of the 0th dimension of the input.
+        If True, the output is a single value averaged across the whole array.
     output : {'ratio', 'percent'}
         Representation for the output:
             'ratio' - ratio value, between 0.0, 1.0.
             'percent' - percent value, betweeon 0-100%.
 
     Returns
     -------
```

### Comparing `specparam-2.0.0rc1/specparam/utils/debug.py` & `specparam-2.0.0rc2/specparam/utils/debug.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/utils/download.py` & `specparam-2.0.0rc2/specparam/utils/download.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/utils/io.py` & `specparam-2.0.0rc2/specparam/utils/io.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/utils/params.py` & `specparam-2.0.0rc2/specparam/utils/params.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam/utils/reports.py` & `specparam-2.0.0rc2/specparam/utils/reports.py`

 * *Files identical despite different names*

### Comparing `specparam-2.0.0rc1/specparam.egg-info/PKG-INFO` & `specparam-2.0.0rc2/specparam.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specparam
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Spectral parameterization.
 Home-page: https://github.com/fooof-tools/fooof
 Download-URL: https://github.com/fooof-tools/fooof/releases
 Author: The Voytek Lab
 Author-email: voyteklab@gmail.com
 Maintainer: Thomas Donoghue
 Maintainer-email: tdonoghue.research@gmail.com
@@ -72,15 +72,15 @@
 
 .. |Paper| image:: https://img.shields.io/badge/paper-nn10.1038-informational.svg
 .. _Paper: https://doi.org/10.1038/s41593-020-00744-x
 
 
 Spectral parameterization (`specparam`, formerly `fooof`) is a fast, efficient, and physiologically-informed tool to parameterize neural power spectra.
 
-WARNING: this Github repository has been updated to a major update / breaking change from the current release of the `fooof` module, and is no longer consistent with the `fooof` version of the code.
+WARNING: this Github repository has been updated to a major update / breaking change from previous releases, which were under the `fooof` name, and now contains major breaking update for the new `specparam` version of the code. The new version is not fully released, though a test version is available (see installation instructions below).
 
 Overview
 --------
 
 The power spectrum model conceives of a model of the power spectrum as a combination of two distinct functional processes:
 
 - An aperiodic component, reflecting 1/f like characteristics, with
@@ -91,19 +91,47 @@
 
 The benefit of fitting a model in order to measure putative oscillations, is that peaks in the power spectrum are
 characterized in terms of their specific center frequency, power and bandwidth without requiring predefining
 specific bands of interest and controlling for the aperiodic component.
 The model also returns a measure of this aperiodic components of the signal, allowing for measuring and
 comparison of 1/f-like components of the signal within and between subjects.
 
+specparam (upcoming version)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+We are currently in the process of a major update to this tool, that includes a name changes (fooof -> specparam), and full rewrite of the code. This means that the new version will be incompatible with prior versions (in terms of the code having different names, and previous code no longer running as written), though note that the exact same procedures will be available (spectra can be fit in a way expected to give the same results), as well many new features.
+
+The new version is called `specparam` (spectral parameterization). There is a release candidate available for testing (see installation instructions).
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
+The fooof naming scheme, with most recent stable version 1.1 is the current main release, and is fully functional and stable, including everything that was introduced under the fooof name.
+
+Which version should I use?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The previous release version, fooof, is fully functional, and projects that are already using it might as well stick with that, unless any of the new functionality in specparam is particularly important. For projects that are just starting, the new specparam version may be of interest if some of the new features are of interest (e.g. time-resolved estimations), though note that as release candidates, the release are not guaranteed to be stable (future updates may make breaking changes). Note that for the same model and settings, fooof and specparam should be exactly equivalent, so in terms of outputs there should be no difference in choosing one or the other.
+
 Documentation
 -------------
 
+The `specparam` package includes a full set of code documentation.
+
+specparam (upcoming version)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To see the documentation for the candidate 2.0 release, see
+`here <https://specparam-tools.github.io/>`_.
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
 Documentation is available on the
-`documentation site <https://fooof-tools.github.io/fooof/index.html>`_.
+`documentation site <https://fooof-tools.github.io/>`_.
 
 This documentation includes:
 
 - `Motivations <https://fooof-tools.github.io/fooof/auto_motivations/index.html>`_:
   with motivating examples of why we recommend parameterizing neural power spectra
 - `Tutorials <https://fooof-tools.github.io/fooof/auto_tutorials/index.html>`_:
   with a step-by-step guide through the model and how to apply it
@@ -117,15 +145,15 @@
   which defines all the key terms used in the module
 - `Reference <https://fooof-tools.github.io/fooof/reference.html>`_:
   with information for how to reference and report on using the module
 
 Dependencies
 ------------
 
-SpecParam is written in Python, and requires Python >= 3.7 to run.
+`specparam` is written in Python, and requires Python >= 3.7 to run.
 
 It has the following required dependencies:
 
 - `numpy <https://github.com/numpy/numpy>`_
 - `scipy <https://github.com/scipy/scipy>`_ >= 0.19
 
 There are also optional dependencies, which are not required for model fitting itself, but offer extra functionality:
@@ -136,14 +164,34 @@
 - `pytest <https://github.com/pytest-dev/pytest>`_ is needed to run the test suite locally
 
 We recommend using the `Anaconda <https://www.anaconda.com/distribution/>`_ distribution to manage these requirements.
 
 Installation
 ------------
 
+specparam / fooof can be installed using pip.
+
+specparam (test version)
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+To install the current release candidate version for the new 2.0 version, you can do:
+
+.. code-block:: shell
+
+    $ pip install specparam
+
+The above will install the most recent release candidate.
+
+NOTE: specparam is currently available as a 'release candidate', meaning it is not finalized and fully released yet.
+This means it may not yet have all features that the ultimate 2.0 version will include, and things are not strictly
+guaranteed to stay the same (there may be further breaking changes in the ultimate 2.0 release).
+
+fooof (stable version)
+~~~~~~~~~~~~~~~~~~~~~~
+
 The current major release is the 1.X.X series, which is a breaking change from the prior 0.X.X series.
 
 Check the `changelog <https://fooof-tools.github.io/fooof/changelog.html>`_ for notes on updating to the new version.
 
 **Stable Version**
 
 To install the latest stable release, use pip:
@@ -186,15 +234,15 @@
 The original implementation of `specparam`, available in this repository, is implemented in Python.
 
 If you wish to run specparam from another language, there are a couple potential options:
 
 - a `wrapper`, which allows for running the Python code from another language
 - a `reimplementation`, which reflects a new implementation of the specparam algorithm in another language
 
-Below are listed some examples of wrappers and/or reimplementations in other languages (non-exhaustive).
+Below are listed some examples of wrappers and/or re-implementations in other languages (non-exhaustive).
 
 Matlab
 ~~~~~~
 
 In Matlab, there is a reimplementation available in common toolboxes:
 - The `Brainstorm <https://neuroimage.usc.edu/brainstorm/Introduction>`_ toolbox has a reimplementation of specparam (see the `Brainstorm fooof tutorial <https://neuroimage.usc.edu/brainstorm/Tutorials/Fooof>`_)
 - The `Fieldtrip <https://www.fieldtriptoolbox.org/>`_ toolbox also uses the same reimplementation (see the `Fieldtrip fooof tutorial <https://www.fieldtriptoolbox.org/example/fooof/>`_)
```

### Comparing `specparam-2.0.0rc1/specparam.egg-info/SOURCES.txt` & `specparam-2.0.0rc2/specparam.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,21 @@
 specparam/core/strings.py
 specparam/core/utils.py
 specparam/data/__init__.py
 specparam/data/conversions.py
 specparam/data/data.py
 specparam/data/utils.py
 specparam/objs/__init__.py
+specparam/objs/algorithm.py
+specparam/objs/base.py
+specparam/objs/data.py
 specparam/objs/event.py
-specparam/objs/fit.py
 specparam/objs/group.py
+specparam/objs/model.py
+specparam/objs/results.py
 specparam/objs/time.py
 specparam/objs/utils.py
 specparam/plts/__init__.py
 specparam/plts/annotate.py
 specparam/plts/aperiodic.py
 specparam/plts/error.py
 specparam/plts/event.py
@@ -75,17 +79,21 @@
 specparam/tests/core/test_strings.py
 specparam/tests/core/test_utils.py
 specparam/tests/data/__init__.py
 specparam/tests/data/test_conversions.py
 specparam/tests/data/test_data.py
 specparam/tests/data/test_utils.py
 specparam/tests/objs/__init__.py
+specparam/tests/objs/test_algorithm.py
+specparam/tests/objs/test_base.py
+specparam/tests/objs/test_data.py
 specparam/tests/objs/test_event.py
-specparam/tests/objs/test_fit.py
 specparam/tests/objs/test_group.py
+specparam/tests/objs/test_model.py
+specparam/tests/objs/test_results.py
 specparam/tests/objs/test_time.py
 specparam/tests/objs/test_utils.py
 specparam/tests/plts/__init__.py
 specparam/tests/plts/test_annotate.py
 specparam/tests/plts/test_aperiodic.py
 specparam/tests/plts/test_error.py
 specparam/tests/plts/test_event.py
```

