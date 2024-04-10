# Comparing `tmp/simim-0.3.4.tar.gz` & `tmp/simim-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simim-0.3.4.tar", last modified: Fri Mar 15 00:15:34 2024, max compression
+gzip compressed data, was "simim-0.3.5.tar", last modified: Wed Apr 10 04:53:18 2024, max compression
```

## Comparing `simim-0.3.4.tar` & `simim-0.3.5.tar`

### file list

```diff
@@ -1,71 +1,78 @@
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.935943 simim-0.3.4/
--rw-r--r--   0 keenan   (649963457) 1357073302     1067 2024-03-15 00:09:14.000000 simim-0.3.4/LICENSE
--rw-r--r--   0 keenan   (649963457) 1357073302     3255 2024-03-15 00:15:34.935697 simim-0.3.4/PKG-INFO
--rw-r--r--   0 keenan   (649963457) 1357073302     1184 2024-03-07 16:02:37.000000 simim-0.3.4/README.md
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.926253 simim-0.3.4/docs/
--rw-r--r--   0 keenan   (649963457) 1357073302     2467 2024-03-08 22:52:24.000000 simim-0.3.4/docs/conf.py
--rw-r--r--   0 keenan   (649963457) 1357073302     1149 2024-03-15 00:12:19.000000 simim-0.3.4/pyproject.toml
--rw-r--r--   0 keenan   (649963457) 1357073302       38 2024-03-15 00:15:34.935982 simim-0.3.4/setup.cfg
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.927055 simim-0.3.4/simim/
--rw-r--r--   0 keenan   (649963457) 1357073302      263 2024-03-07 15:56:24.000000 simim-0.3.4/simim/__init__.py
--rw-r--r--   0 keenan   (649963457) 1357073302    22753 2024-03-15 00:09:14.000000 simim-0.3.4/simim/_handlers.py
--rw-r--r--   0 keenan   (649963457) 1357073302     9781 2024-03-01 20:03:27.000000 simim-0.3.4/simim/_paths.py
--rw-r--r--   0 keenan   (649963457) 1357073302      651 2024-03-07 15:56:24.000000 simim-0.3.4/simim/_pltsetup.py
--rw-r--r--   0 keenan   (649963457) 1357073302     1720 2024-02-28 22:19:04.000000 simim-0.3.4/simim/constants.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.930042 simim-0.3.4/simim/galprops/
--rw-r--r--   0 keenan   (649963457) 1357073302       87 2024-02-28 23:24:15.000000 simim-0.3.4/simim/galprops/__init__.py
--rw-r--r--   0 keenan   (649963457) 1357073302    10173 2024-03-07 15:56:24.000000 simim-0.3.4/simim/galprops/galprops.py
--rw-r--r--   0 keenan   (649963457) 1357073302    31442 2024-03-15 00:09:14.000000 simim-0.3.4/simim/galprops/galprops_am.py
--rw-r--r--   0 keenan   (649963457) 1357073302     2581 2024-02-28 23:39:58.000000 simim-0.3.4/simim/galprops/galprops_builtin.py
--rw-r--r--   0 keenan   (649963457) 1357073302    10949 2024-02-28 22:12:47.000000 simim-0.3.4/simim/galprops/line_co.py
--rw-r--r--   0 keenan   (649963457) 1357073302     1252 2024-02-28 21:12:40.000000 simim-0.3.4/simim/galprops/line_co_dutycycle.py
--rw-r--r--   0 keenan   (649963457) 1357073302     2926 2024-02-28 21:39:26.000000 simim-0.3.4/simim/galprops/line_densegas.py
--rw-r--r--   0 keenan   (649963457) 1357073302    14272 2024-02-28 22:19:50.000000 simim-0.3.4/simim/galprops/line_fir.py
--rw-r--r--   0 keenan   (649963457) 1357073302    13740 2024-02-28 22:12:23.000000 simim-0.3.4/simim/galprops/line_fir_yang.py
--rw-r--r--   0 keenan   (649963457) 1357073302     1054 2024-02-28 21:43:51.000000 simim-0.3.4/simim/galprops/log10normal.py
--rw-r--r--   0 keenan   (649963457) 1357073302    10201 2024-03-01 20:03:27.000000 simim-0.3.4/simim/galprops/sfr_behroozi13.py
--rw-r--r--   0 keenan   (649963457) 1357073302    14797 2024-03-15 00:09:14.000000 simim-0.3.4/simim/galprops/sfr_bethermin17.py
--rw-r--r--   0 keenan   (649963457) 1357073302     7816 2024-03-15 00:09:14.000000 simim-0.3.4/simim/galprops/sfr_ir.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.930919 simim-0.3.4/simim/instrument/
--rw-r--r--   0 keenan   (649963457) 1357073302      140 2024-03-07 15:56:24.000000 simim-0.3.4/simim/instrument/__init__.py
--rw-r--r--   0 keenan   (649963457) 1357073302     4630 2024-03-07 15:56:24.000000 simim-0.3.4/simim/instrument/_helpers.py
--rw-r--r--   0 keenan   (649963457) 1357073302    54001 2024-03-07 15:56:24.000000 simim-0.3.4/simim/instrument/instrument.py
--rw-r--r--   0 keenan   (649963457) 1357073302     1765 2024-03-07 15:56:24.000000 simim-0.3.4/simim/instrument/noise_functions.py
--rw-r--r--   0 keenan   (649963457) 1357073302     2491 2024-03-07 15:56:24.000000 simim-0.3.4/simim/instrument/spatial_response.py
--rw-r--r--   0 keenan   (649963457) 1357073302      590 2024-03-07 15:56:24.000000 simim-0.3.4/simim/instrument/spectral_response.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.931317 simim-0.3.4/simim/lightcone/
--rw-r--r--   0 keenan   (649963457) 1357073302       80 2024-03-01 20:03:27.000000 simim-0.3.4/simim/lightcone/__init__.py
--rw-r--r--   0 keenan   (649963457) 1357073302    19182 2024-03-07 15:56:24.000000 simim-0.3.4/simim/lightcone/lchandler.py
--rw-r--r--   0 keenan   (649963457) 1357073302    35373 2024-03-07 15:56:24.000000 simim-0.3.4/simim/lightcone/lcmaker.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.931587 simim-0.3.4/simim/map/
--rw-r--r--   0 keenan   (649963457) 1357073302      259 2024-03-01 20:03:27.000000 simim-0.3.4/simim/map/__init__.py
--rw-r--r--   0 keenan   (649963457) 1357073302    93547 2024-03-07 15:56:24.000000 simim-0.3.4/simim/map/gridder.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.932301 simim-0.3.4/simim/resources/
--rw-r--r--   0 keenan   (649963457) 1357073302   645911 2013-04-08 17:19:38.000000 simim-0.3.4/simim/resources/behroozi13_release.dat
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.933623 simim-0.3.4/simim/siminterface/
--rw-r--r--   0 keenan   (649963457) 1357073302      161 2024-02-28 12:19:30.000000 simim-0.3.4/simim/siminterface/__init__.py
--rw-r--r--   0 keenan   (649963457) 1357073302     5393 2024-02-26 13:49:27.000000 simim-0.3.4/simim/siminterface/_illustris_datahandling.py
--rw-r--r--   0 keenan   (649963457) 1357073302    27068 2024-02-28 19:23:15.000000 simim-0.3.4/simim/siminterface/_rawsiminterface.py
--rw-r--r--   0 keenan   (649963457) 1357073302      910 2024-02-26 11:16:48.000000 simim-0.3.4/simim/siminterface/_sims.py
--rw-r--r--   0 keenan   (649963457) 1357073302    26044 2024-02-28 12:11:08.000000 simim-0.3.4/simim/siminterface/illustris.py
--rw-r--r--   0 keenan   (649963457) 1357073302    23886 2024-03-03 18:25:44.000000 simim-0.3.4/simim/siminterface/simhandler.py
--rw-r--r--   0 keenan   (649963457) 1357073302    17135 2024-02-28 12:11:10.000000 simim-0.3.4/simim/siminterface/universemachine.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.935447 simim-0.3.4/simim.egg-info/
--rw-r--r--   0 keenan   (649963457) 1357073302     3255 2024-03-15 00:15:34.000000 simim-0.3.4/simim.egg-info/PKG-INFO
--rw-r--r--   0 keenan   (649963457) 1357073302     1579 2024-03-15 00:15:34.000000 simim-0.3.4/simim.egg-info/SOURCES.txt
--rw-r--r--   0 keenan   (649963457) 1357073302        1 2024-03-15 00:15:34.000000 simim-0.3.4/simim.egg-info/dependency_links.txt
--rw-r--r--   0 keenan   (649963457) 1357073302       48 2024-03-15 00:15:34.000000 simim-0.3.4/simim.egg-info/entry_points.txt
--rw-r--r--   0 keenan   (649963457) 1357073302       65 2024-03-15 00:15:34.000000 simim-0.3.4/simim.egg-info/requires.txt
--rw-r--r--   0 keenan   (649963457) 1357073302       28 2024-03-15 00:15:34.000000 simim-0.3.4/simim.egg-info/top_level.txt
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.934626 simim-0.3.4/tests/
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.934765 simim-0.3.4/tests/by_eye_checks/
--rw-r--r--   0 keenan   (649963457) 1357073302     1550 2024-03-14 23:47:34.000000 simim-0.3.4/tests/by_eye_checks/e2e_sfr.py
-drwxr-xr-x   0 keenan   (649963457) 1357073302        0 2024-03-15 00:15:34.935226 simim-0.3.4/tests/old_test_code/
--rw-r--r--   0 keenan   (649963457) 1357073302    12155 2024-02-28 21:12:40.000000 simim-0.3.4/tests/old_test_code/lightcone.py
--rw-r--r--   0 keenan   (649963457) 1357073302     4493 2024-02-28 21:12:40.000000 simim-0.3.4/tests/old_test_code/properties.py
--rw-r--r--   0 keenan   (649963457) 1357073302     2456 2024-03-07 14:54:14.000000 simim-0.3.4/tests/old_test_code/siminterface.py
--rw-r--r--   0 keenan   (649963457) 1357073302     6207 2024-03-07 15:56:24.000000 simim-0.3.4/tests/test_gridder.py
--rw-r--r--   0 keenan   (649963457) 1357073302     1799 2024-03-07 15:56:24.000000 simim-0.3.4/tests/test_imports.py
--rw-r--r--   0 keenan   (649963457) 1357073302    24778 2024-03-07 15:56:24.000000 simim-0.3.4/tests/test_instrument.py
--rw-r--r--   0 keenan   (649963457) 1357073302     3187 2024-02-28 21:05:15.000000 simim-0.3.4/tests/test_rawsiminterface.py
--rw-r--r--   0 keenan   (649963457) 1357073302      431 2024-03-07 15:56:24.000000 simim-0.3.4/tests/test_siminterface.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.659098 simim-0.3.5/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1067 2024-03-15 00:09:14.000000 simim-0.3.5/LICENSE
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3411 2024-04-10 04:53:18.658861 simim-0.3.5/PKG-INFO
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1339 2024-04-10 04:52:29.000000 simim-0.3.5/README.md
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.637712 simim-0.3.5/docs/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2467 2024-03-08 22:52:24.000000 simim-0.3.5/docs/conf.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1149 2024-04-10 04:51:51.000000 simim-0.3.5/pyproject.toml
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       38 2024-04-10 04:53:18.659141 simim-0.3.5/setup.cfg
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.639182 simim-0.3.5/simim/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      263 2024-03-07 15:56:24.000000 simim-0.3.5/simim/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    24509 2024-03-15 23:47:46.000000 simim-0.3.5/simim/_handlers.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     9754 2024-03-15 23:47:34.000000 simim-0.3.5/simim/_paths.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      651 2024-03-07 15:56:24.000000 simim-0.3.5/simim/_pltsetup.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1767 2024-04-09 16:09:24.000000 simim-0.3.5/simim/constants.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.642485 simim-0.3.5/simim/galprops/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       87 2024-02-28 23:24:15.000000 simim-0.3.5/simim/galprops/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10173 2024-03-07 15:56:24.000000 simim-0.3.5/simim/galprops/galprops.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    31442 2024-03-15 00:09:14.000000 simim-0.3.5/simim/galprops/galprops_am.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2581 2024-02-28 23:39:58.000000 simim-0.3.5/simim/galprops/galprops_builtin.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10949 2024-02-28 22:12:47.000000 simim-0.3.5/simim/galprops/line_co.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1252 2024-02-28 21:12:40.000000 simim-0.3.5/simim/galprops/line_co_dutycycle.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2926 2024-02-28 21:39:26.000000 simim-0.3.5/simim/galprops/line_densegas.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    14272 2024-02-28 22:19:50.000000 simim-0.3.5/simim/galprops/line_fir.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    13740 2024-02-28 22:12:23.000000 simim-0.3.5/simim/galprops/line_fir_yang.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1054 2024-02-28 21:43:51.000000 simim-0.3.5/simim/galprops/log10normal.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10201 2024-03-01 20:03:27.000000 simim-0.3.5/simim/galprops/sfr_behroozi13.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    14797 2024-03-15 00:09:14.000000 simim-0.3.5/simim/galprops/sfr_bethermin17.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     7816 2024-03-15 00:09:14.000000 simim-0.3.5/simim/galprops/sfr_ir.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.647513 simim-0.3.5/simim/instrument/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      140 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     4630 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/_helpers.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    54001 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/instrument.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1765 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/noise_functions.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2491 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/spatial_response.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      590 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/spectral_response.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.648185 simim-0.3.5/simim/lightcone/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       80 2024-03-01 20:03:27.000000 simim-0.3.5/simim/lightcone/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    20117 2024-03-15 23:47:46.000000 simim-0.3.5/simim/lightcone/lchandler.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    35373 2024-03-07 15:56:24.000000 simim-0.3.5/simim/lightcone/lcmaker.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.650167 simim-0.3.5/simim/map/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      259 2024-03-01 20:03:27.000000 simim-0.3.5/simim/map/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)   108750 2024-03-20 23:56:41.000000 simim-0.3.5/simim/map/gridder.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.650543 simim-0.3.5/simim/resources/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)   645911 2013-04-08 17:19:38.000000 simim-0.3.5/simim/resources/behroozi13_release.dat
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.653856 simim-0.3.5/simim/siminterface/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      160 2024-03-21 15:01:42.000000 simim-0.3.5/simim/siminterface/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     5393 2024-02-26 13:49:27.000000 simim-0.3.5/simim/siminterface/_illustris_datahandling.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    27068 2024-02-28 19:23:15.000000 simim-0.3.5/simim/siminterface/_rawsiminterface.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      879 2024-03-21 14:33:27.000000 simim-0.3.5/simim/siminterface/_sims.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    26058 2024-03-21 14:32:20.000000 simim-0.3.5/simim/siminterface/illustris.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    26736 2024-03-15 23:47:46.000000 simim-0.3.5/simim/siminterface/simhandler.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    18073 2024-03-21 23:03:50.000000 simim-0.3.5/simim/siminterface/universemachine.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.658596 simim-0.3.5/simim.egg-info/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3411 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/PKG-INFO
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1741 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/SOURCES.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)        1 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/dependency_links.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       48 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/entry_points.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       65 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/requires.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       38 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/top_level.txt
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.655173 simim-0.3.5/simim_dev/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    12877 2024-03-15 00:09:14.000000 simim-0.3.5/simim_dev/dev_features.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     8200 2024-03-24 18:32:20.000000 simim-0.3.5/simim_dev/dev_lim_stats.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     4021 2024-03-24 14:06:11.000000 simim-0.3.5/simim_dev/dev_spectral_functions.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3270 2024-03-15 00:09:14.000000 simim-0.3.5/simim_dev/old_obs_noise.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    52131 2024-03-15 00:09:14.000000 simim-0.3.5/simim_dev/old_obs_radio.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.657660 simim-0.3.5/tests/
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.657975 simim-0.3.5/tests/by_eye_checks/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1550 2024-03-14 23:47:34.000000 simim-0.3.5/tests/by_eye_checks/e2e_sfr.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1848 2024-03-21 23:11:46.000000 simim-0.3.5/tests/make_testbox_resource.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.658217 simim-0.3.5/tests/old_test_code/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    12155 2024-02-28 21:12:40.000000 simim-0.3.5/tests/old_test_code/lightcone.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    11512 2024-03-20 23:23:48.000000 simim-0.3.5/tests/test_gridder.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1799 2024-03-07 15:56:24.000000 simim-0.3.5/tests/test_imports.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    24778 2024-03-07 15:56:24.000000 simim-0.3.5/tests/test_instrument.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3187 2024-02-28 21:05:15.000000 simim-0.3.5/tests/test_rawsiminterface.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3153 2024-03-21 23:16:14.000000 simim-0.3.5/tests/test_rawsiminterface2.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      431 2024-03-07 15:56:24.000000 simim-0.3.5/tests/test_siminterface.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    11485 2024-03-20 23:58:31.000000 simim-0.3.5/tests/test_spec_gridder.py
```

### Comparing `simim-0.3.4/LICENSE` & `simim-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/PKG-INFO` & `simim-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simim
-Version: 0.3.4
+Version: 0.3.5
 Summary: Code for simulating the radio, sub-mm and FIR sky
 Author: R P Keenan
 License: MIT License
         
         Copyright (c) 2024 R P Keenan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,7 +63,13 @@
 1. simim directory - source code for the SimIM package
 2. setupsimim.py - script for completing SimIM setup when building from GitHub source code
 3. docs directory - code for building documentation
 4. tests directory - unit tests; these cover more recent additions to the SimIM source code
 but are relatively sparse for the galprops, lightcone, and siminterface modules.
 5. pyproject.toml, .readthedocs.yaml, .gitignore - config files for pip,
    readthedocs, and git
+
+Change Log
+----------
+Version 0.3.5
+- Update ascii loader for UniverseMachine to use less memory and hopefully run faster
+- Minor bug fixes and some tests
```

### Comparing `simim-0.3.4/README.md` & `simim-0.3.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -19,7 +19,13 @@
 1. simim directory - source code for the SimIM package
 2. setupsimim.py - script for completing SimIM setup when building from GitHub source code
 3. docs directory - code for building documentation
 4. tests directory - unit tests; these cover more recent additions to the SimIM source code
 but are relatively sparse for the galprops, lightcone, and siminterface modules.
 5. pyproject.toml, .readthedocs.yaml, .gitignore - config files for pip,
    readthedocs, and git
+
+Change Log
+----------
+Version 0.3.5
+- Update ascii loader for UniverseMachine to use less memory and hopefully run faster
+- Minor bug fixes and some tests
```

### Comparing `simim-0.3.4/docs/conf.py` & `simim-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/pyproject.toml` & `simim-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "simim"
 authors = [{name = "R P Keenan"}]
 description = "Code for simulating the radio, sub-mm and FIR sky"
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.3.4"
+version = "0.3.5"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Astronomy"
 ]
 keywords = [
     "astronomy", "line intensity mapping", "LIM", "extragalactic",
```

### Comparing `simim-0.3.4/simim/_handlers.py` & `simim-0.3.5/simim/_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,29 @@
     """Generic class for handling SimIM formatted simulation data
     
     The simim.siminterface.SnapHandler and 
     simim.lightcone.LCHandler child classes build on this
     code.
     """
 
-    def __init__(self,path,objectname,groupname):
+    def __init__(self,path,objectname,groupname,in_h_units):
         """Initialize the Handler instance
 
         Parameters
         ----------
         path : string
             Path for the .hdf5 file containing the simulation
         objectname : string    
             A name for the type of object contained
         groupname : string
             A name for the specific object contained
+        in_h_units : bool
+            If True, values will be returned, plotted, etc. in units including little h.
+            If False, little h dependence will be removed. This can be overridden in 
+            most method calls.
         """
 
         self.path = path
 
         self.objectname = objectname
         self.groupname = groupname
 
@@ -51,14 +55,31 @@
         self.extra_props = {'h':self.h}
 
         # Initialize the indices of active properties
         self.inds_all = np.arange(self.nhalos_all).astype('int')
         self.inds_active = np.arange(self.nhalos_all).astype('int')
         self.nhalos_active = len(self.inds_active)
 
+        # Little h
+        self.set_in_h_units(in_h_units)
+
+    def set_in_h_units(self,in_h_units):
+        """Globally set whether units are interpreted to be in little h units
+
+        Changes the default way units are processed
+        
+        Parameters
+        ----------
+        in_h_units : bool
+            If True, values will, by default, be returned in units including little h.
+            If False, little h dependence will be removed.
+        """
+
+        self.default_in_h_units = in_h_units
+
     def extract_keys(self,set='any'):
         """Get the fields attached to a file
 
         Parameters
         ----------
         set : {'any','loaded','saved','generated'}
             What type of keys to return, default is all
@@ -159,35 +180,39 @@
 
         for property_name in property_names:
             if not property_name in self.properties_loaded.keys():
                 warnings.warn("Property {} is not loaded".format(property_name))
 
             self.properties_loaded.pop(property_name, None)
 
-    def return_property(self, property_name, use_all_inds=False, in_h_units=False):
+    def return_property(self, property_name, use_all_inds=False, in_h_units=None):
         """Load a property from lightcone file and return
 
         Parameters
         ----------
         property_name : str
             The name of the field to be loaded
         use_all_inds : bool
             If True values will be returned for all halos, otherwise only
             active halos will be returned. Default is False, but by default
             all halos are active
-        in_h_units : bool (default is False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be returned in units including little h.
-            If False, little h dependence will be removed.
+            If False, little h dependence will be removed. Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         property_values : array
             Values of the requested property
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         if use_all_inds:
             inds = self.inds_all
         else:
             inds = self.inds_active
 
         if not property_name in self.properties_all:
             raise ValueError("{} does not have this property".format(self.objectname))
@@ -368,15 +393,15 @@
                         if i != property_name:
                             properties_all_new.append(i)
                     self.properties_all = properties_all_new
 
                     self.properties_units.pop(property_name,None)
                     self.properties_h_dependence.pop(property_name,None)
 
-    def set_property_range(self,property_name=None,pmin=-np.inf,pmax=np.inf,reset=True, in_h_units=False):
+    def set_property_range(self,property_name=None,pmin=-np.inf,pmax=np.inf,reset=True, in_h_units=None):
         """Set a range in a given property to be the active indices. If no
         arguments are passed, this resets the active indices to all halos
 
         Parameters
         ----------
         property_name : str
             The name of the field to use
@@ -385,25 +410,29 @@
         pmax : float
             The maximum value of the property to bracket the selected range.
         reset : bool, optional
             If True, the active indices will be those selected between pmin and
             pmax. If False, the active indices will be that satisfy pmin<=p<=pmax
             and which were previously in the active indices (ie this allows
             selection over multiple properties.)
-        in_h_units : bool (default=False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, pmin and pmax will be taken to have units including little h,
             otherwise, they will be assumed to have units with no h dependence
             (and have the correct dependency applied before setting cuts for parameters
-            where the stored catalog values are in h units).
+            where the stored catalog values are in h units). Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         None
         """
-
+        
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+        
         if property_name is None:
             self.inds_active = np.copy(self.inds_all)
 
         else:
             vals = self.return_property(property_name,use_all_inds=True,in_h_units=in_h_units)
             inds = np.nonzero((vals>=pmin) & (vals<=pmax))[0]
 
@@ -412,15 +441,15 @@
             else:
                 self.inds_active = np.intersect1d(inds,self.inds_active)
         
         self.nhalos_active = len(self.inds_active)
 
     def eval_stat(self, stat_function, kwargs, kw_remap={}, other_kws={},
                   use_all_inds=False,
-                  give_args_in_h_units=False):
+                  give_args_in_h_units=None):
         """Evaluate stat_function over the objects in a Handler instance
         and return the result
 
         This can be used to evaluate any function of the the properties contained
         in the simulation, but is generally envisioned as a way to compute 
         ensemble statistics (means, luminosity functions, correlations, etc.)
 
@@ -437,32 +466,35 @@
             one would use kw_remap={'a':'mass'}
         other_kws : dict, optional
             A dictionary of additional keyword arguments passed directly to
             the stat_function call
         use_all_inds : bool, default=False
             If True function will be computed using all halos, otherwise only
             active halos will be evaluated.
-        give_args_in_h_units : bool, default=False
+        give_args_in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be fed to stat_function in units including little h.
-            If False, little h dependence will be removed.
+            If False, little h dependence will be removed first. Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         vals 
             The value(s) returned by stat_function
         
         Examples
         --------
         Compute the total halo mass in a simulation accesed via the variable
         ``handler``:
         
         >>> handler.eval_stat(np.sum, kwargs=['a'], kw_remap={'a':'mass'})
-
         """
 
+        if give_args_in_h_units is None:
+            give_args_in_h_units = self.default_in_h_units
+
         # Check that target has required fields (ie kwargs) - as written this is incompatible with remapping keywords
         # for kwarg in kwargs:
         #     if not self.has_property(kwarg) and not kwarg in self.extra_props.keys():
         #         raise ValueError("Property {} not found".format(kwarg))
 
         arguments = {}
         for kwarg in other_kws.keys():
@@ -485,15 +517,15 @@
         vals = stat_function(**arguments)
 
         return vals
 
     @pltdeco
     def plot(self, xname, *ynames,
              use_all_inds = False,
-             save=None, axkws={}, plotkws={},in_h_units=False):
+             save=None, axkws={}, plotkws={},in_h_units=None):
         """Make a scatter plot of two properties
 
         Parameters
         ----------
         xname : str
             The name of the field to use as the x-value
         *ynames : str
@@ -509,24 +541,29 @@
             If specified, the plot will be saved to the given location
         axkws : dict, optional
             A dictionary of keyword args and values that will be fed to ax.set()
             when creating the plot axes
         plotkws : dict, optional
             A dictionary of keyword args and values that will be fed to
             plt.plot() when creating the plot data
-        in_h_units : bool (default is False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be plotted in units including little h. If
-            False, little h dependence will be removed.
+            False, little h dependence will be removed. Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         None
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         fig,ax = plt.subplots()
+    
         fig.subplots_adjust(left=.15,right=.95,bottom=.15,top=.95)
         ax.set(**axkws)
         
         if 'ls' not in plotkws and 'linestyle' not in plotkws:
             plotkws['ls'] = ''
         if 'marker' not in plotkws:
             plotkws['marker'] = '.'
@@ -549,15 +586,15 @@
         if save != None:
             plt.savefig(save)
         plt.show()
 
     @pltdeco
     def hist(self, *property_names,
              use_all_inds = False,
-             logtransform=False, save=None, axkws={}, plotkws={},in_h_units=False):
+             logtransform=False, save=None, axkws={}, plotkws={},in_h_units=None):
         """Make a histogram of a property
 
         Parameters
         ----------
         *property_names : str
             The name(s) of the field(s) to use, multiple fields can be given and
             will be plotted on the same axes with the same settings
@@ -571,24 +608,27 @@
             If specified, the plot will be saved to the given location
         axkws : dict, optional
             A dictionary of keyword args and values that will be fed to ax.set()
             when creating the plot axes
         plotkws : dict, optional
             A dictionary of keyword args and values that will be fed to
             plt.hist() when creating the plot data
-        in_h_units : bool (default is False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be plotted in units including little h. If
-            False, little h dependence will be removed.
-
+            False, little h dependence will be removed. Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         None
         """
-
+        
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+        
         fig,ax = plt.subplots()
         ax.set(**axkws)
 
         for pn in property_names:
             x = self.return_property(pn,use_all_inds=use_all_inds,in_h_units=in_h_units)
             if logtransform:
                 x = np.log10(x)
```

### Comparing `simim-0.3.4/simim/_paths.py` & `simim-0.3.5/simim/_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,15 @@
             self.sims = _checkload_path_file(os.path.join(self.root,self.simpath_ext))
             self.props = _checkload_path_file(os.path.join(self.root,self.proppath_ext))
         
     def _setuppath(self,root='~',confirm_with_user=False):
         """Create a directory root/simim_resources/simulations"""
 
         # Get the right thing for the home directory
-        if root == '~':
-            root = os.path.expanduser("~")
+        root = os.path.expanduser(root)
 
         # Check if a root already exists and whehter it should be replaced
         if self.root is not None:
             if root != self.root:
                 print("A root has already been specified:")
                 print("   {}".format(self.root))
                 answer = input("Do you want to set a new root? y/n: ")
```

### Comparing `simim-0.3.4/simim/_pltsetup.py` & `simim-0.3.5/simim/_pltsetup.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/constants.py` & `simim-0.3.5/simim/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ### PHYSICAL CONSTANTS ###
 # All in SI units
 c = 2.99792458e8 # m s^-1; speed of light
 kB = 1.3806e-23 # m^2 kg s^-2 K^-1; boltzmann constant
+hP = 6.62607015e-34 # J Hz^-1; Planck constant
 
 ### UNIT CONVERSION ###
 Lsun_to_W = 3.828e26
 Mpc_to_m = 3.0857e22
 
 ### FREQUENCIES FOR VARIOUS SPECTRAL LINES ###
 # All values come from Splatalogue and are given in Hz.
```

### Comparing `simim-0.3.4/simim/galprops/galprops.py` & `simim-0.3.5/simim/galprops/galprops.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/galprops_am.py` & `simim-0.3.5/simim/galprops/galprops_am.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/galprops_builtin.py` & `simim-0.3.5/simim/galprops/galprops_builtin.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/line_co.py` & `simim-0.3.5/simim/galprops/line_co.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/line_co_dutycycle.py` & `simim-0.3.5/simim/galprops/line_co_dutycycle.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/line_densegas.py` & `simim-0.3.5/simim/galprops/line_densegas.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/line_fir.py` & `simim-0.3.5/simim/galprops/line_fir.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/line_fir_yang.py` & `simim-0.3.5/simim/galprops/line_fir_yang.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/log10normal.py` & `simim-0.3.5/simim/galprops/log10normal.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/sfr_behroozi13.py` & `simim-0.3.5/simim/galprops/sfr_behroozi13.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/sfr_bethermin17.py` & `simim-0.3.5/simim/galprops/sfr_bethermin17.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/galprops/sfr_ir.py` & `simim-0.3.5/simim/galprops/sfr_ir.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/instrument/_helpers.py` & `simim-0.3.5/simim/instrument/_helpers.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/instrument/instrument.py` & `simim-0.3.5/simim/instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/instrument/noise_functions.py` & `simim-0.3.5/simim/instrument/noise_functions.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/instrument/spatial_response.py` & `simim-0.3.5/simim/instrument/spatial_response.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/instrument/spectral_response.py` & `simim-0.3.5/simim/instrument/spectral_response.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/lightcone/lchandler.py` & `simim-0.3.5/simim/lightcone/lchandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     The general philosophy of Handlers is to not load actual properties of 
     a halo into memory until they are requested, and to remove them from 
     memory when they are no longer in use (or at least make it convenient
     to do so).
     """
 
-    def __init__(self,sim,name,number):
+    def __init__(self,sim,name,number,in_h_units=False):
         """Initialize Handler for a specified lightcone
 
         This class a generic interface for interacting with data in SimIM's
         standardize lightcone format. 
 
         Light cones must first be built using simim.lightcone.LCMaker.
         Lightcones are saved in sets in the SimIM data directory, each set of
@@ -41,15 +41,19 @@
         Parameters
         ----------
         sim : str
             The name of the simulation from which the lightcone was generated. 
         name : str
             The name of the lightcone set. 
         number : int
-            The numeric index of the lightcone within the set        
+            The numeric index of the lightcone within the set
+        in_h_units : bool
+            If True, values will be returned, plotted, etc. in units including little h.
+            If False, little h dependence will be removed. This can be overridden in 
+            most method calls.
         """
 
         # Handle file path stuff
         paths = _SimIMPaths()
         if not sim in paths.lcs:
             raise ValueError("Lightcones for simulation {} not found. Try generating them or updating the path".format(sim))
         path = paths.lcs[sim]
@@ -58,15 +62,15 @@
             raise ValueError("Lightcones named '{}' not found. Try generating them or updating the path".format(name))
         path = os.path.join(path, name)
 
         if not os.path.exists(os.path.join(path,'lc_{:04d}.hdf5'.format(number))):
             raise ValueError("Lightcone number '{}' not found.".format(number))
         path = os.path.join(path,'lc_{:04d}.hdf5'.format(number))
 
-        super().__init__(path=path,objectname='Lightcone',groupname='Lightcone Full')
+        super().__init__(path=path,objectname='Lightcone',groupname='Lightcone Full',in_h_units=in_h_units)
 
         # Get the metadata
         self.metadata = {}
         with h5py.File(self.path,'r') as file:
             for key in file.attrs.keys():
                 self.metadata[key] = file.attrs[key]
 
@@ -84,15 +88,15 @@
         self.extra_props['open_angle'] = self.open_angle
         self.extra_props['shape'] = self.shape
         self.extra_props['aspect_ratio'] = self.aspect_ratio
         self.extra_props['minimum redshift'] = self.minimum_redshift
         self.extra_props['maximum redshift'] = self.maximum_redshift
 
 
-    def volume(self,redshift_min=None,redshift_max=None,shape=None,open_angle=None,aspect_ratio=None,in_h_units=False):
+    def volume(self,redshift_min=None,redshift_max=None,shape=None,open_angle=None,aspect_ratio=None,in_h_units=None):
         """Compute the comoving volume of the light cone
 
         Parameters
         ----------
         redshift_min, redshift_max : float, optional
             The minimum/maximum redshift to consider - the minimum/maximum
             redshift of the lightcone by default
@@ -100,25 +104,28 @@
             The opening angle of the lightcone - by default matches the
             lightcone
         aspect_ratio : float, optional
             The aspect ratio of the box sides (for square lightcones) -
             by default matches the lightcone
         shape : 'box', 'circle', optional
             The shape of the box - by default matches the lightcone
-        in_h_units : bool (default is False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be returned in units including little h.
-            If False, little h dependence will be removed.
-
+            If False, little h dependence will be removed. Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         volume : float
             The volume of the lightcone in comoving Mpc^3
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         # Set defaults
         if redshift_min == None:
             redshift_min=self.metadata['minimum redshift']
         if redshift_max == None:
             redshift_max=self.metadata['maximum redshift']
         if shape == None:
             shape=self.metadata['shape']
@@ -158,19 +165,22 @@
         volume = (v2-v1) * area/(4*np.pi)
 
         if in_h_units:
             volume *= self.h**3
 
         return volume
 
-    def eval_stat_evo(self, redshift_bins, stat_function, kwargs, kw_remap={}, other_kws={}, zmin_kw=False, zmax_kw=False, volume_kw=False, give_args_in_h_units=False):
+    def eval_stat_evo(self, redshift_bins, stat_function, kwargs, kw_remap={}, other_kws={}, zmin_kw=False, zmax_kw=False, volume_kw=False, give_args_in_h_units=None):
         """Compute the evolution of a statistic over a specified set of
         redshift bins
         """
 
+        if give_args_in_h_units is None:
+            give_args_in_h_units = self.default_in_h_units
+
         redshift_bins = np.sort(redshift_bins)
         
         inds_active_save = np.copy(self.inds_active)
 
         vals = []
         for bin in range(len(redshift_bins)-1):
             self.set_property_range('redshift',
@@ -200,15 +210,15 @@
         # Reset active inds
         self.inds_active = np.copy(inds_active_save)
 
         return redshift_bins, vals
 
     def grid(self, *property_names, 
              restfreq=None,
-             in_h_units=False,use_all_inds=False,
+             in_h_units=None,use_all_inds=False,
              res=None,ralim=None,declim=None,zlim=None,
              norm=None):
         """Place selected properties into a 3d grid
         
         Uses the properties of the array to construct a position
         (ra,dec,redshift)-value (property_names) grid. Only required argument is
         a valid property name or names. Additional arguments can specify the
@@ -220,18 +230,18 @@
         ----------
         property_names : str
             The name or names of properties in the Handler instance
         restfreq : float
             A rest frequency to use for converting the third axis from redshift
             to frequency. The returned axis will be constructed as
             restfreq/(1+z)
-        in_h_units : bool, default=False
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, positions and property values fed to the gridder will be in
             units including little h. If False, little h dependence will be
-            removed.
+            removed. Defaults to whatever is set globally for the Handler instance.
         use_all_inds : bool, default=False
             If True function all halos will be gridded, otherwise only active
             halos will be included.
         res : float, optional
             The resolution for the grid in Mpc (if in_h_units==False) or Mpc/h
             (if in_h_units==True). If no value is specified, it will default to
             1/100th of the box edge length
@@ -246,14 +256,17 @@
 
         Returns
         -------
         grid : simim.map.grid instance
             The gridded properties
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+        
         x = self.return_property('ra',in_h_units=in_h_units,use_all_inds=use_all_inds)
         y = self.return_property('dec',in_h_units=in_h_units,use_all_inds=use_all_inds)
         z = self.return_property('redshift',in_h_units=in_h_units,use_all_inds=use_all_inds)
         if restfreq is not None:
             z = restfreq/(1+z)
         props = np.array([self.return_property(p,in_h_units=in_h_units,use_all_inds=use_all_inds) for p in property_names]).T
         
@@ -289,15 +302,15 @@
         grid.grid *= norm
 
         return grid
 
 
 
     @pltdeco
-    def animate(self, save=None, use_all_inds=False, colorpropname='mass',colorscale='log', sizepropname='mass',sizescale='log',in_h_units=False):
+    def animate(self, save=None, use_all_inds=False, colorpropname='mass',colorscale='log', sizepropname='mass',sizescale='log',in_h_units=None):
         """Make an animation of the light cone
 
         Parameters
         ----------
         use_all_inds : bool, optional
             If True values will be assigned for all halos, otherwise only
             active halos will be evaluated, and others will be assigned nan.
@@ -305,23 +318,27 @@
         save : str, optional
             If specified, the plot will be saved to the given location
         colorpropname : str
             Name of the property used to determine marker color for each
             galaxy, default is 'mass'
         colorpropscale : 'log' or 'linear'
             Determines how the colorbar will be applied. Default is 'log'
-        in_h_units : bool (default is False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be plotted in units including little h.
-            If False, little h dependence will be removed.
+            If False, little h dependence will be removed. Defaults to whatever
+            is set globally for the Handler instance.
 
         Returns
         -------
         None
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+            
         x = self.return_property('pos_x',use_all_inds=use_all_inds,in_h_units=in_h_units)
         y = self.return_property('pos_y',use_all_inds=use_all_inds,in_h_units=in_h_units)
         z = self.return_property('pos_z',use_all_inds=use_all_inds,in_h_units=in_h_units)
 
         ra = self.return_property('ra',use_all_inds=use_all_inds,in_h_units=in_h_units)
         dec = self.return_property('dec',use_all_inds=use_all_inds,in_h_units=in_h_units)
         redshift = self.return_property('redshift',use_all_inds=use_all_inds,in_h_units=in_h_units)
```

### Comparing `simim-0.3.4/simim/lightcone/lcmaker.py` & `simim-0.3.5/simim/lightcone/lcmaker.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/map/gridder.py` & `simim-0.3.5/simim/map/gridder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Callable
+from numpy.typing import ArrayLike
 import warnings
 import os
 
 import numpy as np
 from scipy.signal import fftconvolve
 
 from simim._pltsetup import *
@@ -546,15 +548,43 @@
                      }
         if self.grid_active:
             save_data['grid'] = self.grid
 
         savefunc(path,**save_data)
 
 
-    def add_from_cat(self,positions,values=None,new_props=False):
+    def add_new_prop(self,value=None):
+        """Add a new property to the grid"""
+
+        if self.grid_active:
+            if value is None:
+                value = np.zeros(np.concatenate((self.n_pixels,[1])))
+            elif value.ndim == self.grid.ndim:
+                if np.any(value.shape[:-1] != self.n_pixels):
+                    raise ValueError("Value array must match shape of grid")
+            elif value.ndim == self.n_dimensions:
+                if np.any(value.shape != self.n_pixels):
+                    raise ValueError("Value array must match shape of grid")
+                value = value[...,np.newaxis]
+            else:
+                raise ValueError("Value array must match shape of grid")
+
+            self.grid = np.concatenate((self.grid,value),axis=-1)
+            self.n_properties += value.shape[-1]
+
+        # Different behavior if grid isn't activated yet
+        if not self.grid_active:
+            if value is not None:
+                raise ValueError("data array for this Grid has not been initialized, cannot add new values in property array -- use add_new_prop(value=None) to add an empty new property without initializing grid")
+            else:
+                self.n_properties += 1
+
+
+
+    def add_from_cat(self,positions,values=None,new_props=False,properties=None):
         """Add values to the grid
 
         Parameters
         ----------
         positions : array
             The positions of each object should be an n_objects x n_dimensions
             array
@@ -563,72 +593,355 @@
             values is not specified and the Grid's n_properties attribute is 
             equal to 1, counts in cell for each postions value will be added 
             to the grid.
         new_props : bool (optional)
             If True, this method will create new entries along the poperty
             dimension for each set of values given rather than adding them
             on top of existing values. Default is False.
+        properties : int or list of ints (optional)
+            If specified, the values will only be added to the specified property
+            indices. If None, values will be added to all property indices.
+            Ignored if new_props = True
         """
         
         if not self.grid_active:
             raise ValueError("data array for this Grid has not been initialized")
         
         if np.any(self.fourier_space):
             raise ValueError("Some axes are in fourier space, cannot add new properties in map space.")
-
+        
         # If the positions array is empty don't need to do much
         if len(positions) == 0:
             if positions.ndim == 1:
                 positions = positions.reshape((positions.shape[0],1))
 
                 if new_props:
                     new_n_properties = values.shape[1]
                     new_grid = np.zeros(np.concatenate((self.n_pixels,[new_n_properties])))
-                    self.grid = np.concatenate((self.grid,new_grid),axis=-1)
-                    self.n_properties = self.n_properties + new_n_properties
+                    self.add_new_prop(new_grid)
 
         # Otherwise make sure the positions array is in the right shape and matches the shape of the grid
         else:
             positions = np.array(positions,ndmin=1,copy=True)
             if positions.shape[0] > 0:
                 if positions.shape[1] !=self.n_dimensions:
                     raise ValueError('positions (dim={}) does not have the right number of dimensions for the grid (dim={})'.format(positions.shape[1],self.n_dimensions))
 
             if values is None:
                 values = np.ones(len(positions))
             values = np.array(values,ndmin=1,copy=True)
             if values.ndim == 1:
                 values = values.reshape((values.shape[0],1))
 
-            if values.shape[1] != self.n_properties and not new_props:
-                raise ValueError("Values array does not contain the correct number of properties.")
             if values.shape[0] != positions.shape[0]:
-                raise ValueError("position and values array do not have equal lenght.")
+                raise ValueError("position and values array do not have equal length.")
 
             # Put data into coordinate units
             positions -= self.center_point.reshape(1,self.n_dimensions)
             positions += self.side_length.reshape(1,self.n_dimensions)/2
             positions /= self.pixel_size.reshape(1,self.n_dimensions)
             positions = np.floor(positions).astype('int')
 
             # Get rid of anything that doesn't fit
             values = values[(~np.any(positions<0,axis=1)) & (~np.any(positions>=self.n_pixels,axis=1))]
             positions = positions[(~np.any(positions<0,axis=1)) & (~np.any(positions>=self.n_pixels,axis=1))]
+            positions = tuple(positions.T[i] for i in range(positions.shape[1]))
 
-            if not new_props:
-                np.add.at(self.grid,tuple(np.split(positions,self.n_dimensions,axis=1)),np.expand_dims(values,1))
-            else:
+            if new_props:
                 new_n_properties = values.shape[1]
                 new_grid = np.zeros(np.concatenate((self.n_pixels,[new_n_properties])))
-                np.add.at(new_grid,tuple(np.split(positions,self.n_dimensions,axis=1)),np.expand_dims(values,1))
-                self.grid = np.concatenate((self.grid,new_grid),axis=-1)
-                self.n_properties = self.n_properties + new_n_properties
+                np.add.at(new_grid,positions,values)
+                self.add_new_prop(new_grid)
+
+            else:
+                properties = self._check_property_input(properties)
+                if values.shape[1] != len(properties) and values.shape[1] != 1:
+                    raise ValueError("Values array does not contain the correct number of properties.")
+
+                for ip in properties:
+                    if values.shape[1] == 1:
+                        v = values.flatten()
+                    else:
+                        v = values[:,ip]
+                    np.add.at(self.grid,positions+(ip,),v)
 
             # Count the number of objects
-            self.n_objects += positions.shape[0]
+            self.n_objects += len(values)
+
+
+    def add_from_pos_plus_array(self, positions: ArrayLike, values: ArrayLike, ax: int = -1, new_prop: bool = False, properties: int = None):
+        """Add values to a grid from a list of positions (dimension N-1), and
+        the values along the final dimension
+        
+        Takes an array of positions with 1 dimension less than the dimensionality 
+        of the grid plus an array that will be added at that position along the final 
+        dimension.
+
+        Parameters
+        ----------
+        positions : array
+            The positions of each object should be an n_objects x (n_dimensions-1)
+            array
+        values : array
+            Values to grid, should be an n_objects x grid_size_in_final_dimension array.
+        ax : int (optional)
+            The axis along which the values are to be added, by default the final position
+            axis is assumed
+        new_prop : bool (optional)
+            If True, this method will create a new entry along the poperty
+            dimension of the grid rather than adding values on top of any existing values
+            in the grid. Default is False.
+        properties : int or list of ints (optional)
+            If specified, the values will only be added to the specified property
+            indices. If None, values will be added to all property indices.
+            Ignored if new_props = True
+        """
+
+        if not self.grid_active:
+            raise ValueError("data array for this Grid has not been initialized")
+        
+        if np.any(self.fourier_space):
+            raise ValueError("Some axes are in fourier space, cannot add new properties in map space.")
+
+        # Check that the grid has the specified axis
+        if ax < 0: 
+            ax = self.n_dimensions+ax
+        if ax>=self.n_dimensions or ax<0:
+            raise ValueError('specified axes not valid')
+
+        # If the positions array is empty don't need to do much
+        if len(positions) == 0:
+            if positions.ndim == 1:
+                if new_prop:
+                    new_grid = np.zeros(np.concatenate((self.n_pixels,[1])))
+                    self.add_new_prop(new_grid)
+            
+            return
+
+        # Otherwise make sure the positions and values arrays are in the right shapes and match the shape of the grid
+        positions = np.array(positions,ndmin=2)
+        values = np.array(values,ndmin=2)
+
+        if positions.shape[0] > 0:
+            if positions.shape[1] != self.n_dimensions-1:
+                raise ValueError('positions (dim={}) should have one fewer dimensions than the grid (dim={})'.format(positions.shape[1],self.n_dimensions))
+
+        if values.shape[0] != positions.shape[0]:
+            raise ValueError("values (len={}) and positions (len={}) should have the same first dimension length".format(len(values), len(positions)))
+
+        if values.shape[1] != self.n_pixels[ax]:
+            raise ValueError("The second dimension size of values (d={}) should match the size of grid dimension {} (d={})".format(values.shape[0],ax,self.n_pixels[ax]))
+
+        # Put data into coordinate units
+        cp = np.delete(self.center_point,ax).reshape(1, self.n_dimensions-1)
+        sl = np.delete(self.side_length,ax).reshape(1, self.n_dimensions-1)
+        px = np.delete(self.pixel_size,ax).reshape(1, self.n_dimensions-1)
+        nx = np.delete(self.n_pixels,ax)
+
+        positions = (positions - cp + sl/2) / px
+        positions = np.floor(positions).astype('int')
+
+        # Get rid of anything that doesn't fit
+        values = values[(~np.any(positions<0,axis=1)) & (~np.any(positions>=nx,axis=1))]
+        positions = positions[(~np.any(positions<0,axis=1)) & (~np.any(positions>=nx,axis=1))]
+
+        # Convert postions into tuples of coordinate lists:
+        positions = tuple(positions.T[i] for i in range(positions.shape[1]))
+
+        # Move array-axis to predictable location (end of grid)
+        if not new_prop:
+            if properties is None:
+                self.grid = np.moveaxis(self.grid,ax,-2)
+                np.add.at(self.grid, positions, np.expand_dims(values,2))
+                self.grid = np.moveaxis(self.grid,-2,ax)
+            else:
+                properties = self._check_property_input(properties)
+                for ip in properties:
+                    self.grid = np.moveaxis(self.grid,ax,-2)
+                    np.add.at(self.grid, positions+(slice(None),ip,), values)
+                    self.grid = np.moveaxis(self.grid,-2,ax)
+
+
+        else:
+            new_grid = np.zeros(np.concatenate((self.n_pixels,[1])))
+            new_grid = np.moveaxis(new_grid,ax,-2)
+            np.add.at(new_grid,positions,np.expand_dims(values,2))
+            new_grid = np.moveaxis(new_grid,-2,ax)
+            
+            self.add_new_prop(new_grid)
+
+        # Count the number of objects
+        self.n_objects += len(values)
+
+
+    def add_from_spec_func(self, positions: ArrayLike, spec_function: Callable, spec_function_arguments: ArrayLike = None, spec_ax: int = -1,
+                           is_cumulative: bool = False, eval_as_loop=False, 
+                           careful_with_memory: bool = True,
+                           new_prop: bool = False, properties: int = None):
+        """Add spectra to a grid
+        
+        Takes an array of positions with 1 dimension less than the dimensionality 
+        of the grid plus a function that is evaluated over the final dimension of
+        the grid. The function is evaulated at axis value along the final axis.
+
+        spec_function should take as its first argument an array of frequencies 
+        (values of the Grid instances axis matching the spec_ax parameter), and as its
+        second argument an array of shape n_objects x n_parameters containing any 
+        additional function arguments for the spec_function. The parameters for each
+        object are then passed as spec_function_arguments. By default, it is assumed
+        that the function will be evaluated simultaneously for all objects, and
+        return an array of shape (n_objects x spec_ax_length).
+        
+        Example spec_function:
+        >>> # Gaussian spectral line w/ 100 km/s sigma, assumes axis is in GHz
+        >>> # and line rest frequency is 115 GHz
+        >>> def spec_func(axis, params):
+        >>> ... lum = params[:,0]
+        >>> ... redshift = params[:,1]
+        >>> ... nu0 = 115/(1+redshift) # Redshift line center
+        >>> ... nu_sig = 300 / 3e5 * nu0 # FWHM in GHz
+        >>> ... # Reshape arrays so everything broadcasts together into the right shape:
+        >>> ... lum = lum.reshape(-1,1)
+        >>> ... nu_sig = nu_sig.reshape(-1,1)
+        >>> ... nu0 = nu0.reshape(-1,1)
+        >>> ... ax = axis.reshape(1,-1)
+        >>> ... spec = lum / np.sqrt(2*np.pi*nu_sig**2) * np.exp(-0.5 * (ax-nu0)**2/nu_sig**2)
+        >>> ... return spec
+        The corresponding spec_function_arguments would be
+        >>> spec_function_arguments = np.array([[lum1, redshift1],...,[lumn,redshiftn]])
+        
+        The optimal way to characterize a spectrum for this type of gridding is
+        in terms of its cumulative value along spectral axis, which can then be
+        evaluated at each bin edge and differenced to return an integrated 
+        spectrum that will not depend on the steps along the grid or (for example)
+        lose flux from narrow peaks that aren't well sampled by the Grid axis.
+        If spec_function is written as a cumulative function, then set ``is_cumulative``
+        to True, and the spectrum will be constructed by evaluating spec_function
+        at the edges of the axis cells and then differencing. This is not the default
+        as it is not common to write analytic formulae for the integral of a spectrum.
+
+        Parameters
+        ----------
+        positions : array
+            The positions of each object should be an n_objects x (n_dimensions-1)
+            array
+        spec_function : Callable
+            Function that will be evaluated to compute the spectra of each object
+        spec_function_args : array
+            Array of shape n_objects x n_function_parameters that will be passed 
+            to spec_function when evaluating spectra of each object
+        spec_ax : int (optional)
+            The axis along which the values are to be added, by default the final position
+            axis is assumed
+        eval_as_loop : bool (default = False)
+            If True, the spec_function will be evaluated in a loop - one call per 
+            object in the positions and spec_function_args arrays.
+        is_cumulative : bool (default = False)
+            If True, the spec_function returns the integral of the spectrum from 0 to
+            a given point along the axis, and the final spectrum is calculated by 
+            differencing evaluated values at the edge of each bin in the Grid.
+        careful_with_memory : bool (default = True)
+            If True, the input arrays of positions and spec_function_args will be 
+            broken up into smaller chunks and added to the grid one chunk at a time.
+            This is helpful for preventing memory overflows when processing large
+            catalogs. The chunk size is determined so that the number of array 
+            elements used to hold spectra is never larger than the number of array
+            elements in the grid itself.
+        new_prop : bool (optional)
+            If True, this method will create a new entry along the poperty
+            dimension of the grid rather than adding values on top of any existing values
+            in the grid. Default is False.
+        properties : int or list of ints (optional)
+            If specified, the values will only be added to the specified property
+            indices. If None, values will be added to all property indices.
+            Ignored if new_props = True
+        """
+
+        if not hasattr(spec_function, '__call__'):
+            raise ValueError("spec_function must have a __call__ method")
+
+        if not self.grid_active:
+            raise ValueError("data array for this Grid has not been initialized")
+        
+        if np.any(self.fourier_space):
+            raise ValueError("Some axes are in fourier space, cannot add new properties in map space.")
+
+        # Check that the grid has the specified spec_axis
+        if spec_ax < 0: 
+            spec_ax = self.n_dimensions+spec_ax
+        if spec_ax>=self.n_dimensions or spec_ax<0:
+            raise ValueError('specified spec_ax not valid')
+
+        # If the positions array is empty don't need to do much
+        if len(positions) == 0:
+            if positions.ndim == 1:
+                if new_prop:
+                    new_grid = np.zeros(np.concatenate((self.n_pixels,[1])))
+                    self.new_prop(new_grid)
+            
+            return
+
+        # Otherwise make sure the positions and spec_function_arguments arrays are in the right shapes and match the shape of the grid
+        positions = np.array(positions,ndmin=2)
+        if positions.shape[0] > 0:
+            if positions.shape[1] != self.n_dimensions-1:
+                raise ValueError('positions (dim={}) should have one fewer dimensions than the grid (dim={})'.format(positions.shape[1],self.n_dimensions))
+
+        if spec_function_arguments is None:
+            spec_function_arguments = np.zeros((len(positions),0))
+        else:
+            spec_function_arguments = np.array(spec_function_arguments,ndmin=1)
+        
+        if spec_function_arguments.shape[0] != positions.shape[0]:
+            raise ValueError('spec_function_arguments must have the same length as positions')
+        if spec_function_arguments.ndim == 1:
+            spec_function_arguments = spec_function_arguments[...,np.newaxis]
+
+        # Determine if a loop is necessary
+        if careful_with_memory:
+            chunk_size = np.prod(np.delete(self.n_pixels,spec_ax)) # maximum number of spectral channels computed equals size of the grid
+        else:
+            chunk_size = len(positions)
+
+        # Pick axis to use
+        if is_cumulative:
+            spec_axis_eval = self.axes[spec_ax]
+        else:
+            spec_axis_eval = self.axes_centers[spec_ax]
+
+        # Loop is here to allow a version which minimizes memory usage.
+        # default parameters will cause the loop to only happen once and
+        # simultaneously evaluate all spectra
+        for i in range(np.ceil(len(positions)/chunk_size).astype(int)):
+            
+            pi = positions[i*chunk_size:(i+1)*chunk_size]
+            argi = spec_function_arguments[i*chunk_size:(i+1)*chunk_size]
+
+
+            if eval_as_loop:
+                values = []
+                for ig in range(len(pi)):
+                    values.append(spec_function(spec_axis_eval, argi[ig].reshape(1,-1)).flatten())
+            else:
+                values = spec_function(spec_axis_eval, argi)
+            
+            values = np.array(values,ndmin=2)
+
+            if is_cumulative:
+                values = np.diff(values, axis=1)
+
+            if values.shape[1] != self.n_pixels[spec_ax]:
+                raise ValueError("The length of the returned spectrum (l={}) should match the size of grid dimension {}".format(values.shape[1],spec_ax))
+            if values.shape[0] != len(pi):
+                raise ValueError("The number of returned spectra should match the number of positions")
+        
+            self.add_from_pos_plus_array(pi, values, new_prop=new_prop, properties=properties, ax=spec_ax)
+            if new_prop: # After first loop need to change behavior
+                new_prop = False
+                properties = self.n_properties - 1
 
 
     def sum_properties(self,properties=None,in_place=True):
         """Sum values of different properties
         
         Parameters
         ----------
@@ -656,16 +969,15 @@
         
         properties = np.array(properties,ndmin=1)
         if not np.all(np.isin(properties,np.arange(self.n_properties))):
             raise ValueError("Some property indices do not correspond to property indices of the grid")
         
         sum_grid = np.expand_dims(np.sum(self.grid[...,tuple(properties)],axis=-1),-1)
         if in_place:
-            self.grid = np.concatenate((self.grid,sum_grid),axis=-1)
-            self.n_properties += 1
+            self.add_new_prop(sum_grid)
 
             return self
             
         else:
             new_grid = self.copy_axes(n_properties=1)
             new_grid.init_grid()
             new_grid.grid = sum_grid
@@ -2098,7 +2410,8 @@
         """
         super().__init__(*axes,n_properties=n_properties,axunits=axunits,gridunits=gridunits)
         self.init_grid()
         shape = self.grid.shape
         self.grid = np.expand_dims(function(*self.axes_centers,**function_kwargs),axis=-1)
         if self.grid.shape != shape:
             raise ValueError("function does not produce a grid of the correct shape")
+
```

### Comparing `simim-0.3.4/simim/resources/behroozi13_release.dat` & `simim-0.3.5/simim/resources/behroozi13_release.dat`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/siminterface/_illustris_datahandling.py` & `simim-0.3.5/simim/siminterface/_illustris_datahandling.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/siminterface/_rawsiminterface.py` & `simim-0.3.5/simim/siminterface/_rawsiminterface.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/simim/siminterface/_sims.py` & `simim-0.3.5/simim/siminterface/_sims.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """List of accepted simulations and code to check if an input matches
 
 All simulations which are handled by the current version of SimIM are 
 listed here, this will have to be modified if adding support for 
 additional simulations"""
 
-_acceptedsims = ['Illustris-1','Illustris-2','Illustris-3',
-                 'Illustris-1-Dark','Illustris-2-Dark','Illustris-3-Dark',
-                 'TNG300-1','TNG300-2','TNG300-3',
-                 'TNG300-1-Dark','TNG300-2-Dark','TNG300-3-Dark',
-                 'TNG100-1','TNG100-2','TNG100-3',
-                 'TNG100-1-Dark','TNG100-2-Dark','TNG100-3-Dark',
-                 'UniverseMachine-BolshoiPlanck','UniverseMachine-SMDPL','UniverseMachine-MDPL2']
+_illsims = ['Illustris-1','Illustris-2','Illustris-3','Illustris-1-Dark','Illustris-2-Dark','Illustris-3-Dark']
+_tngsims = ['TNG300-1','TNG300-2','TNG300-3','TNG300-1-Dark','TNG300-2-Dark','TNG300-3-Dark','TNG100-1','TNG100-2','TNG100-3','TNG100-1-Dark','TNG100-2-Dark','TNG100-3-Dark']
+_umsims = ['UniverseMachine-BolshoiPlanck','UniverseMachine-SMDPL','UniverseMachine-MDPL2','_testbox']
+_acceptedsims = _illsims + _tngsims + _umsims
 
 def _checksim(sim):
     """Check if a specified simulation name is acceptable"""
 
     if not sim in _acceptedsims:
         raise NameError("Simulation '{}' not recognized/supported".format(sim))
```

### Comparing `simim-0.3.4/simim/siminterface/illustris.py` & `simim-0.3.5/simim/siminterface/illustris.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 import warnings
 
 import numpy as np
 
 from simim.siminterface import _illustris_datahandling as idh
 from simim.siminterface._rawsiminterface import SimCatalogs, Snapshot
-from simim.siminterface._sims import _checksim
+from simim.siminterface._sims import _checksim, _illsims, _tngsims
 
 class IllustrisCatalogs(SimCatalogs):
     """Class to download and format Illustris or TNG group catalogs"""
 
     def __init__(self,
                  sim, 
                  api_key,
@@ -42,22 +42,22 @@
             to 'all' which will use all known snapshots.
         updatepath : optional, bool
             Defaults to True. If True, the path parameter will be saved as the 
             default path to this simulation in future uses.
         """
         
         # Figure out the snapshots needed
-        if sim[:3] == 'Ill':
+        if sim in _illsims:
             self.allsnaps = np.arange(136)
 
             # For Illustris-1 some snapshots were lost
             if sim == 'Illustris-1':
                 self.allsnaps = np.setdiff1d(self.allsnaps,[53,55])
 
-        elif sim[:3] == 'TNG':
+        elif sim in _tngsims:
             self.allsnaps =  np.arange(100)
 
         # Initialize catalog
         SimCatalogs.__init__(self,sim, path, snaps, updatepath)
 
         self.api_key = api_key
 
@@ -80,15 +80,15 @@
                         # Peculiar velocity of the group, computed as the sum
                         # of the mass weighted velocities of all
                         # particles/cells in this group, of all types. No unit
                         # conversion is needed.
                         'SubhaloVel':[('v_x','f','km/s',0),('v_y','f','km/s',0),('v_z','f','km/s',0)]
                         }
 
-        if self.sim[:3] == 'TNG' and self.sim[-4:] != 'Dark':
+        if self.sim in _tngsims and self.sim[-4:] != 'Dark':
             self.basic_fields['SubhaloFlag'] = [('flag','int','none',0)]
             # Flag field indicating suitability of this subhalo for
             # certain types of analysis. If zero, this subhalo should
             # generally be excluded, and is not thought to be of
             # cosmological origin. That is, it may have formed within
             # an existing halo, or is possibly a baryonic fragment of
             # a disk or other galactic structure identified by Subfind.
@@ -211,15 +211,15 @@
                             # snapshot table for stars.
                             'SubhaloStellarPhotometrics':
                                 [('phot_U','f','mag',0),('phot_B','f','mag',0),('phot_V','f','mag',0),
                                 ('phot_K','f','mag',0),('phot_g','f','mag',0),('phot_r','f','mag',0),
                                 ('phot_i','f','mag',0),('phot_z','f','mag',0)]
                             }
 
-        if self.sim[:3] == 'TNG' and self.sim[-4:] != 'Dark':
+        if self.sim in _tngsims and self.sim[-4:] != 'Dark':
             tng_matter_fields ={# Individual abundances: H, He, C, N, O, Ne, Mg, Si,
                          # Fe, total (in this order). Each is the dimensionless
                          # ratio of the total mass in that species divided by
                          # the total gas mass, both restricted to gas cells
                          # within twice the stellar half mass radius. The tenth
                          # entry contains the 'total' of all other (i.e.
                          # untracked) metals.
@@ -296,17 +296,17 @@
             file_path = os.path.join(self.path,'raw','groups_{:03d}'.format(i))
             if not os.path.exists(file_path):
                 not_downloaded.append(i)
         if len(not_downloaded) > 0:
             warnings.warn("No data exists for snapshots {} - run .download".format(not_downloaded))
 
         # File naming conventions for the raw simulation downloads:
-        if self.sim[:3] == 'Ill':
+        if self.sim in _illsims:
             self.raw_fname = 'groups_'
-        if self.sim[:3] == 'TNG':
+        if self.sim == _tngsims:
             self.raw_fname = 'fof_subhalo_tab_'
 
     # Function to load the data in a format we want:
     def _loader(self, path, snapshot, fields):
         """Loader to get a field from a snapshot halo catalog
 
         This is promarily meant for internal use by the .format method
```

### Comparing `simim-0.3.4/simim/siminterface/simhandler.py` & `simim-0.3.5/simim/siminterface/simhandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,62 +18,87 @@
     
     The simplest way to initialize a SnapHandler instance is probably via a
     SimHandler instance for the simulation containing the snapshot in question.
     Then the method SimHandler.get_snap will return a Handler instance for the
     snapshot with only the snapshot index-number specified.
     """
 
-    def __init__(self,path,snap,redshift,cosmo,box_edge):
+    def __init__(self,path,snap,redshift,cosmo,box_edge,in_h_units=False):
         """Initialize Handler for a simulation snapshot
         
         Parameters
         ----------
         path : string
             Path to SimIM formatted file containing the snapshot (most likely
             [path to SimIM data directory]/[Simulation Name]/data.hdf5)
         snap : int
             Index-number of the snapshot within the whole simulation
         redshift : float
             Redshift at which the snapshot was taken
         cosmo : dict
             Dictionary containing the cosmological parameters for the simulation
         box_edge : float
-            The edge length of the simulation box, should be in units of Mpc/h.
+            The edge length of the simulation box, should ALWAYS be in units of Mpc/h.
+        in_h_units : bool
+            If True, values will be returned, plotted, etc. in units including little h.
+            If False, little h dependence will be removed. This can be overridden in 
+            most method calls.
         """
 
-        super().__init__(path,objectname='Snapshot',groupname='Snapshot {}'.format(snap))
+        self.h = cosmo.h
+        self.box_edge_h = box_edge
+        self.box_edge_no_h = box_edge / self.h
+        super().__init__(path,objectname='Snapshot',groupname='Snapshot {}'.format(snap),in_h_units=in_h_units)
 
         self.redshift = redshift
         self.cosmo = cosmo
-        self.box_edge = box_edge
-        self.box_edge_no_h = box_edge / self.h
-
+        
         self.extra_props['cosmo'] = self.cosmo
         self.extra_props['redshift'] = self.redshift
+        self.extra_props['box_edge_h'] = self.box_edge_h
+        self.extra_props['box_edge_no_h'] = self.box_edge_h / self.h
+
+    def set_in_h_units(self,in_h_units):
+        """Globally set whether units are interpreted to be in little h units
+
+        Changes the default way units are processed
+        
+        Parameters
+        ----------
+        in_h_units : bool
+            If True, values will, by default, be returned in units including little h.
+            If False, little h dependence will be removed.
+        """
+
+        self.default_in_h_units = in_h_units
+        if in_h_units:
+            self.box_edge = self.box_edge_h 
+        else:
+            self.box_edge = self.box_edge_no_h
         self.extra_props['box_edge'] = self.box_edge
-        self.extra_props['box_edge_no_h'] = self.box_edge / self.h
+
 
     def grid(self,*property_names,
-             in_h_units=False,use_all_inds=False,
+             in_h_units=None,use_all_inds=False,
              res=None,xlim=None,ylim=None,zlim=None,
              norm=None):
         """Place selected properties into a 3d grid
         
         Uses the properties of the array to construct a position (pos_x,pos_y,pos_z)-
         value (property_names) grid. Only required argument is a valid property name
         or names. Additional arguments can specify the limits and resolution of the grid
 
         Parameters
         ----------
         property_names : str
             The name or names of properties in the Handler instance
-        in_h_units : bool, default=False
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, positions and property values fed to the gridder will be
             in units including little h. If False, little h dependence will be 
-            removed.
+            removed. Defaults to whatever is set globally for the Handler instance.
         use_all_inds : bool, default=False
             If True function all halos will be gridded, otherwise only
             active halos will be included.
         res : float, optional
             The resolution for the grid in Mpc (if in_h_units==False) or Mpc/h
             (if in_h_units==True). If no value is specified, it will default to
             1/100th of the box edge length
@@ -89,21 +114,24 @@
 
         Returns
         -------
         grid : simim.map.grid instance
             The gridded properties
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         x = self.return_property('pos_x',in_h_units=in_h_units,use_all_inds=use_all_inds)
         y = self.return_property('pos_y',in_h_units=in_h_units,use_all_inds=use_all_inds)
         z = self.return_property('pos_z',in_h_units=in_h_units,use_all_inds=use_all_inds)
         props = np.array([self.return_property(p,in_h_units=in_h_units,use_all_inds=use_all_inds) for p in property_names]).T
         
         if in_h_units:
-            side = self.box_edge
+            side = self.box_edge_h
         else:
             side = self.box_edge_no_h
 
         c = []
         l = []
 
         for lim in [xlim,ylim,zlim]:
@@ -144,15 +172,15 @@
     of a given simulation.
 
     The general philosophy of Handlers is to not load actual properties of a
     halo into memory until they are requested, and to remove them from memory
     when they are no longer in use (or at least make it convenient to do so).
     """
 
-    def __init__(self,sim,init_snaps=False):
+    def __init__(self,sim,init_snaps=False,in_h_units=False):
         """Initialize Handler for a specified simulation
 
         Provides a generic interface for interacting with data from
         any simulation that has been converted to SimIM format and is
         accessible to memory. Note that simulations must be downloaded
         and formatted (see e.g. simim.siminterface.illustris or 
         simim.siminterface.universemachine for code to accomplish this)
@@ -163,14 +191,18 @@
             Name of the simulation to load.
         init_snaps : bool, default=False
             Setting this as True will create persistent Handler instances 
             for every snapshot, rather than doing so when data from a given 
             handler is called for. This is generally not necessary, but is
             used when creating properties for all snapshots but NOT writing
             them to disk.
+        in_h_units : bool
+            If True, values will be returned, plotted, etc. in units including little h.
+            If False, little h dependence will be removed. This can be overridden in 
+            most method calls.
         """
 
         # Check that we can handle the specified sim
         _checksim(sim)
 
         # Set up a place to keep the data
         paths = _SimIMPaths()
@@ -190,22 +222,30 @@
 
         # Sort out redshift matching to stuff
         snaps_sorted = np.sort(np.copy(self.snap_meta),order='redshift')
         self.z_bins = [snap['redshift_min'] for snap in snaps_sorted]
         self.z_bins.append(snaps_sorted[-1]['redshift_max'])
         self.z_bin_snaps = [snap['index'] for snap in snaps_sorted]
 
+        # How to deal with h
+        self.default_in_h_units = in_h_units
+
         # Make the cosmology
         self.cosmo = FlatLambdaCDM(H0=100*self.metadata['cosmo_h']*u.km/u.s/u.Mpc,
                                    Om0=self.metadata['cosmo_omega_matter'],
                                    Ob0=self.metadata['cosmo_omega_baryon'],
                                    Tcmb0=2.7255*u.K)
-        self.box_edge = self.metadata['box_edge']
-        self.box_edge_no_h = self.box_edge / self.h
+        self.box_edge_h = self.metadata['box_edge']
+        self.box_edge_no_h = self.box_edge_h / self.h
 
+        if self.default_in_h_units:
+            self.box_edge = self.box_edge_h
+        else:
+            self.box_edge = self.box_edge_no_h
+        
         # Get keys and units
         with h5py.File(os.path.join(self.path,'data.hdf5'),'r') as file:
             snaps = [i for i in file.keys()]
             keys = [i for i in file[snaps[0]].keys() if i != 'mass_cuts']
 
             key_units = {key:file[snaps[0]][key].attrs['units'] for key in keys}
             key_h_dependence = {key:file[snaps[0]][key].attrs['h dependence'] for key in keys}
@@ -235,32 +275,58 @@
         self.snap_handlers = {}
         # Set up snapshot handlers
         for i in range(len(self.snap_meta)):
 
             snap = self.snap_meta['index'][i]
             redshift = self.snap_meta['redshift'][i]
 
-            self.snap_handlers[str(snap)] = SnapHandler(self.path+'/data.hdf5',snap,redshift,self.cosmo,self.box_edge)
+            self.snap_handlers[str(snap)] = SnapHandler(self.path+'/data.hdf5',snap,redshift,self.cosmo,self.box_edge_h,in_h_units=self.default_in_h_units)
         print("Snapshots initialized.")
         self.init_snaps = True
 
-    def number_volumes(self,volume,in_h_units=False):
+    def set_in_h_units(self,in_h_units):
+        """Globally set whether units are interpreted to be in little h units
+
+        Changes the default way units are processed
+        
+        Parameters
+        ----------
+        in_h_units : bool
+            If True, values will, by default, be returned in units including little h.
+            If False, little h dependence will be removed.
+        """
+
+        self.default_in_h_units = in_h_units
+        if in_h_units:
+            self.box_edge = self.box_edge_h 
+        else:
+            self.box_edge = self.box_edge_no_h
+        
+        if self.init_snaps:
+            for snap in self.snap_handlers.values():
+                snap.set_in_h_units(in_h_units)
+
+
+    def number_volumes(self,volume,in_h_units=None):
         """Compute the number of times a specified volume can fit in the simulation box
         
         Parameters
         ----------
         volume : float
             The volume to check in units of Mpc^3
-        in_h_units : bool, default = False
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True the value of volume will be assumed to have units of
             (Mpc/h)^3
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         if in_h_units:
-            return volume / self.box_edge**3
+            return volume / self.box_edge_h**3
         else:
             return volume / self.box_edge_no_h**3
 
     def extract_snap_meta(self,snap):
         """Get the meta-data for a snapshot
 
         Parameters
@@ -312,33 +378,36 @@
         -------
         keys
             The fields of each snapshot
         """
 
         return self.keys
 
-    def get_mass_index(self,mass,snap,in_h_units=False):
+    def get_mass_index(self,mass,snap,in_h_units=None):
         """Find the indices above a specified mass
 
         Parameters
         ----------
         mass : float
             Minimum mass to access in Msun units
         snap : int
             Number of snapshot to be extracted
-        in_h_units : bool (default=False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, mass will be taken to have units including little h,
             otherwise, it will be assumed to have units with no h dependence.
 
         Returns
         -------
         index : int
             The index
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         if not snap in self.snap_meta['index']:
             raise ValueError("Snapshot not found")
 
         with h5py.File(os.path.join(self.path,'data.hdf5'),'r') as file:
             mass_cuts = file["Snapshot {}".format(snap)]['mass_cuts']
 
             if in_h_units:
@@ -373,15 +442,15 @@
         snap_meta = self.extract_snap_meta(snap)
 
         if self.init_snaps:
             return self.snap_handlers[str(snap_meta['index'])]
         else:
             snap = snap_meta['index']
             redshift = snap_meta['redshift']
-            return SnapHandler(self.path+'/data.hdf5',snap,redshift,self.cosmo,self.box_edge)
+            return SnapHandler(self.path+'/data.hdf5',snap,redshift,self.cosmo,self.box_edge_h)
 
     def get_snap_from_z(self,z):
         """Return a SnapHandler instance for the snapshot closest to a requested redshift
         
         Parameters
         ----------
         z : float
@@ -391,15 +460,15 @@
         -------
         SnapHandler
             A SnapHandler instance for the requested snapshot
         """
 
         return self.get_snap(self.z_to_snap(z))
 
-    def set_property_range(self,property_name=None,pmin=-np.inf,pmax=np.inf,reset=True, in_h_units=False):
+    def set_property_range(self,property_name=None,pmin=-np.inf,pmax=np.inf,reset=True, in_h_units=None):
         """Restrict property range for all snapshots
         
         This is a wraper around SnapHandler.set_property_range
         that iteratively applies it to all snapshots. Initializing
         handlers for each snapshot is necessary for this to work.
 
         Parameters
@@ -411,21 +480,24 @@
         pmax : float
             The maximum value of the property to bracket the selected range.
         reset : bool, optional
             If True, the active indices will be those selected between pmin and
             pmax. If False, the active indices will be that satisfy pmin<=p<=pmax
             and which were previously in the active indices (ie this allows
             selection over multiple properties.)
-        in_h_units : bool (default=False)
+        in_h_units : bool (default is determined by self.default_in_h_units)
             If True, pmin and pmax will be taken to have units including little h,
             otherwise, they will be assumed to have units with no h dependence
             (and have the correct dependency applied before setting cuts for parameters
             where the stored catalog values are in h units).
         """
 
+        if in_h_units is None:
+            in_h_units = self.default_in_h_units
+
         if not self.init_snaps:
             raise ValueError("This handler instance was not initialized with snapshots available")
         for i in range(len(self.snap_meta)):
             snap = self.snap_meta['index'][i]
             handler = self.get_snap(snap)
             handler.set_property_range(property_name=property_name,pmin=pmin,pmax=pmax,reset=reset,in_h_units=in_h_units)
 
@@ -538,15 +610,15 @@
                                 raise ValueError("Property {} is not userd-defined and cannot be deleted".format(name))
                             elif not file[handler.groupname][name].attrs['userdefined']:
                                 raise ValueError("Property {} is not userd-defined and cannot be deleted".format(name))
 
             handler.delete_property(*property_names)
 
     def snap_stat(self, stat_function, kwargs, kw_remap={}, other_kws={},
-                  give_args_in_h_units=False, use_all_inds=False, snaps=None):
+                  give_args_in_h_units=None, use_all_inds=False, snaps=None):
         """Evaluate stat_function over every snapshot and return results
 
         This is a wraper around SnapHandler.eval_stat that iteratively 
         applies it to all snapshots. 
         
         Parameters
         ----------
@@ -561,29 +633,32 @@
             one would use kw_remap={'a':'mass'}
         other_kws : dict, optional
             A dictionary of additional keyword arguments passed directly to
             the stat_function call
         use_all_inds : bool, default=False
             If True function will be computed using all halos, otherwise only
             active halos will be evaluated.
-        give_args_in_h_units : bool, default=False
+        give_args_in_h_units : bool (default is determined by self.default_in_h_units)
             If True, values will be fed to stat_function in units including little h.
             If False, little h dependence will be removed.
         snaps : list, optional
             A list of snapshots on which to evaluate the stat_function. If none is 
             specified all snapshots will be used.
             
         Returns
         -------
         vals : list
             List containing the value(s) returned by stat_function on each snapshot
         redshifts : list
             List containing the redshift of each snapshot        
         """
 
+        if give_args_in_h_units is None:
+            give_args_in_h_units = self.default_in_h_units
+
         vals = []
         redshifts = []
 
         if snaps is None:
             snaps = np.arange(len(self.snap_meta))
         for i in snaps:
             snap = self.snap_meta['index'][i]
```

### Comparing `simim-0.3.4/simim/siminterface/universemachine.py` & `simim-0.3.5/simim/siminterface/universemachine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import os
 import warnings
+import shutil
 from fnmatch import fnmatch
 
 from urllib.request import urlretrieve
 import requests
+try:
+    from importlib.resources import files
+except:
+    from importlib_resources import files
 
 import numpy as np
 
 from simim.siminterface._rawsiminterface import SimCatalogs, Snapshot
 from simim.siminterface._sims import _checksim
 
+_testsnaps = np.array(['sfr_catalog_0.055623.txt','sfr_catalog_0.506185.txt','sfr_catalog_0.994717.txt'])
+
 class UniversemachineCatalogs(SimCatalogs):
     def __init__(self,
                  sim, path='auto',
                  snaps='all',
                  updatepath=True,
                  ):
         """Initialize an interface with the UniverseMachine Bolshoi/MD catalogs
@@ -39,47 +46,55 @@
 
         if sim == 'UniverseMachine-BolshoiPlanck':
             self.allsnaps = np.arange(178)
         elif sim == 'UniverseMachine-SMDPL':
             self.allsnaps = np.arange(118)
         elif sim == 'UniverseMachine-MDPL2':
             self.allsnaps = np.arange(126)
+        elif sim == '_testbox':
+            self.allsnaps = np.arange(len(_testsnaps))
 
         super().__init__(sim, path, snaps, updatepath)
 
         self.web_path = os.path.join(self.path, 'web_paths.npy')
         if self.sim == 'UniverseMachine-BolshoiPlanck':
             self.webpage = 'https://halos.as.arizona.edu/UniverseMachine/DR1/SFR_ASCII/'
             self._loader = self._ascii_loader
         elif self.sim == 'UniverseMachine-SMDPL':
             self.webpage = 'https://halos.as.arizona.edu/UniverseMachine/DR1/SMDPL_SFR/'
             self._loader = self._bin_loader
         elif self.sim == 'UniverseMachine-MDPL2':
             self.webpage = 'https://halos.as.arizona.edu/UniverseMachine/DR1/MDPL2_SFR/'
             self._loader = self._bin_loader
+        elif self.sim == '_testbox':
+            simim_path = files('simim')
+            self.webpage = simim_path.joinpath('resources','_testbox')
+            self._loader = self._ascii_loader
 
-        if os.path.exists(self.web_path):
+        if self.sim == '_testbox':
+            self.web_files = _testsnaps
+        elif os.path.exists(self.web_path):
             self.web_files = np.load(self.web_path)
         else:
             # Get file names and scale factors from the interweb
             try:
                 html_text = requests.get(self.webpage).text
-                files = [t for t in html_text.split(' ') if fnmatch(t, "*sfr_catalog_*")]
-                files = [t.split('"')[1] for t in files]
-                self.web_files = np.array(files)
+                web_files = [t for t in html_text.split(' ') if fnmatch(t, "*sfr_catalog_*")]
+                web_files = [t.split('"')[1] for t in web_files]
+                self.web_files = np.array(web_files)
             except:
                 raise ValueError("Unable to access file names on {}".format(self.webpage))
             np.save(self.web_path,self.web_files)
 
         # Identify keys that will require unit conversions
         # For UM these are mostly empty because everythings in units
         # we like already.
         # Note that binary files have different units for halo masses
         # than the text files + different format for position/velocity data
-        if self.sim == 'UniverseMachine-BolshoiPlanck':
+        if self.sim == 'UniverseMachine-BolshoiPlanck' or self.sim == '_testbox':
             self.basic_fields = {
                 #X Y Z: halo position (comoving Mpc/h)
                 #VX VY VZ: halo velocity (physical peculiar km/s)
                 'x':[('pos_x','f','Mpc/h',-1)],
                 'y':[('pos_y','f','Mpc/h',-1)],
                 'z':[('pos_z','f','Mpc/h',-1)],
                 'vx':[('v_x','f','km/s',0)],
@@ -145,15 +160,15 @@
             'obs_sfr':[('sfr_obs','f','Msun/yr',0)],
 
             #Obs_UV: Observed UV Magnitude (M_1500 AB)
             'obs_uv':[('phot_uv_obs','f','mag',0)],
             }
         
         # Fields in ascii but not binary files: smhm, obs_sssfr
-        if self.sim == 'UniverseMachine-BolshoiPlanck':
+        if self.sim == 'UniverseMachine-BolshoiPlanck' or self.sim == '_testbox':
             #SSFR: observed SSFR
             self.matter_fields['obs_ssfr'] = [('ssfr_obs','f','?',0)]
             #SMHM: SM/HM ratio
             self.matter_fields['smhm'] = [('stellar_to_halo_mass_ratio','f','None',0)]
         
         # Fields in binary but not ascii files: lvmp, A_UV, empty
         else:
@@ -213,15 +228,15 @@
         """
 
         dtype_raw = np.dtype(dtype=[('id', 'i'), ('descid','i'),('upid','i'),('flags','i'),('uparent_dist','f'),
                                     ('x','f'),('y','f'),('z','f'),('vx','f'),('vy','f'),('vz','f'),
                                     ('m','f'),('v','f'),('mp','f'),('vmp','f'),('r','f'),
                                     ('rank1','f'),('rank2','f'),('ra','f'),('rarank','f'),
                                     ('sm','f'),('icl','f'),('sfr','f'),('obs_sm','f'),('obs_sfr','f'),('obs_ssfr','f'),('smhm','f'),('obs_uv','f')])
-        data_raw = np.genfromtxt(os.path.join(path,self.web_files[snapshot]), dtype=dtype_raw, comments='#')
+        data_raw = np.loadtxt(os.path.join(path,self.web_files[snapshot]), dtype=dtype_raw, comments='#')
         subhaols = {}
         for key in fields:
             subhaols[key] = data_raw[key]
         n_halos = len(data_raw)
 
         return subhaols, n_halos
 
@@ -290,33 +305,35 @@
             >>> x = UniversemachineCatalogs(...,snaps=[10,11,12])
             >>> x.download()
         """
         
         # Check that metadata doesn't already exist
         if not redownload:
             if os.path.exists(self.meta_path):
-                warnings.warn("Metadata appears to exist already")
+                warnings.warn("Metadata appears to exist already: {}".format(self.meta_path))
                 return
 
         self.metadata = {'name':self.sim,
                          'number_snaps':len(self.web_files)}
         # Assign the correct data for different simulation boxes
-        if self.sim in ['UniverseMachine-BolshoiPlanck','UniverseMachine-SMDPL','UniverseMachine-MDPL2']:
+        if self.sim in ['UniverseMachine-BolshoiPlanck','UniverseMachine-SMDPL','UniverseMachine-MDPL2','_testbox']:
             self.metadata['cosmo_name'] = 'Planck'
             self.metadata['cosmo_omega_matter'] = 0.307
             self.metadata['cosmo_omega_lambda'] = 0.693
             self.metadata['cosmo_omega_baryon'] = 0.048
             self.metadata['cosmo_h'] = 0.678
 
         if self.sim == 'UniverseMachine-BolshoiPlanck':
             self.metadata['box_edge'] = 250
         elif self.sim == 'UniverseMachine-SMDPL':
             self.metadata['box_edge'] = 400
         elif self.sim == 'UniverseMachine-MDPL2':
             self.metadata['box_edge'] = 1000
+        elif self.sim == '_testbox':
+            self.metadata['box_edge'] = 10
 
         self.box_edge = self.metadata['box_edge']
         self.h = self.metadata['cosmo_h']
 
         # Scale factors, redshifts, and sort files (read from file names)
         a = np.array([float(t.split('_')[-1][:-4]) for t in self.web_files])
         redshifts = 1/a-1
@@ -368,15 +385,16 @@
     def download(self, redownload=False):
         """Download UniverseMachine catalogs"""
 
         if not os.path.exists(os.path.join(self.path,'raw')):
             os.mkdir(os.path.join(self.path,'raw'))
 
         # Download metadata if not present
-        self.download_meta(redownload=False)
+        if not os.path.exists(self.meta_path):
+            self.download_meta()
 
         # Add a check for already downloaded files
         if redownload:
             self.download_snaps = np.copy(self.snaps)
         else:
             self.download_snaps = []
             for snap in self.snaps:
@@ -387,13 +405,16 @@
                     self.download_snaps.append(snap)
 
         # Download each snap
         for i in range(len(self.download_snaps)):
             snap = self.download_snaps[i]
             print("downloading item {} of {} ({})".format(i+1,len(self.download_snaps),self.web_files[snap]))
             file_path = os.path.join(self.path,'raw',self.web_files[snap])
-            urlretrieve(self.webpage+self.web_files[snap],file_path)
+            if self.sim == '_testbox':
+                shutil.copy(self.webpage.joinpath(self.web_files[snap]),file_path)
+            else:
+                urlretrieve(self.webpage+self.web_files[snap],file_path)
 
 # Wrapper for back compatibility
 def universemachine_catalogs(*args, **kwargs):
     warnings.warn("universemachine_catalogs is depricated, use UniversemachineCatalogs instead")
     return UniversemachineCatalogs(*args, **kwargs)
```

### Comparing `simim-0.3.4/simim.egg-info/PKG-INFO` & `simim-0.3.5/simim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simim
-Version: 0.3.4
+Version: 0.3.5
 Summary: Code for simulating the radio, sub-mm and FIR sky
 Author: R P Keenan
 License: MIT License
         
         Copyright (c) 2024 R P Keenan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,7 +63,13 @@
 1. simim directory - source code for the SimIM package
 2. setupsimim.py - script for completing SimIM setup when building from GitHub source code
 3. docs directory - code for building documentation
 4. tests directory - unit tests; these cover more recent additions to the SimIM source code
 but are relatively sparse for the galprops, lightcone, and siminterface modules.
 5. pyproject.toml, .readthedocs.yaml, .gitignore - config files for pip,
    readthedocs, and git
+
+Change Log
+----------
+Version 0.3.5
+- Update ascii loader for UniverseMachine to use less memory and hopefully run faster
+- Minor bug fixes and some tests
```

### Comparing `simim-0.3.4/simim.egg-info/SOURCES.txt` & `simim-0.3.5/simim.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -41,16 +41,22 @@
 simim/siminterface/__init__.py
 simim/siminterface/_illustris_datahandling.py
 simim/siminterface/_rawsiminterface.py
 simim/siminterface/_sims.py
 simim/siminterface/illustris.py
 simim/siminterface/simhandler.py
 simim/siminterface/universemachine.py
+simim_dev/dev_features.py
+simim_dev/dev_lim_stats.py
+simim_dev/dev_spectral_functions.py
+simim_dev/old_obs_noise.py
+simim_dev/old_obs_radio.py
+tests/make_testbox_resource.py
 tests/test_gridder.py
 tests/test_imports.py
 tests/test_instrument.py
 tests/test_rawsiminterface.py
+tests/test_rawsiminterface2.py
 tests/test_siminterface.py
+tests/test_spec_gridder.py
 tests/by_eye_checks/e2e_sfr.py
-tests/old_test_code/lightcone.py
-tests/old_test_code/properties.py
-tests/old_test_code/siminterface.py
+tests/old_test_code/lightcone.py
```

### Comparing `simim-0.3.4/tests/by_eye_checks/e2e_sfr.py` & `simim-0.3.5/tests/by_eye_checks/e2e_sfr.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/tests/old_test_code/lightcone.py` & `simim-0.3.5/tests/old_test_code/lightcone.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/tests/test_gridder.py` & `simim-0.3.5/tests/test_gridder.py`

 * *Files 27% similar despite different names*

```diff
@@ -66,14 +66,37 @@
 
     g3 = Grid(1, (5,5), 10, 1)
     g3.init_grid()
 
     assert np.all(g1.grid == g2.grid)
     assert np.all(g1.grid == g3.grid)
 
+def test_add_new_prop():
+    g = Grid(1, (5,5), (10,10), (1,1))
+
+    g.add_new_prop()
+    assert g.n_properties == 2
+
+    with pytest.raises(Exception):
+        g.add_new_prop(10)
+    with pytest.raises(Exception):
+        g.add_new_prop(np.zeros((10,10)))
+
+    g.init_grid()
+    assert g.n_properties == 2
+    assert g.grid.shape == (10,10,2)
+
+    g.add_new_prop(np.zeros((10,10)))
+    assert g.n_properties == 3
+    assert g.grid.shape == (10,10,3)
+
+    g.add_new_prop(np.zeros((10,10,2)))
+    assert g.n_properties == 5
+    assert g.grid.shape == (10,10,5)
+
 
 def test_crop():
     g = Grid(1, (5,5), (10,10), (1,1))
     g.init_grid()
 
     g.crop(0,1,9)
     assert g.grid.shape == (8,10,1)
@@ -171,14 +194,87 @@
     assert np.isclose(g.grid[0,1,0], 1.1)
     assert np.isclose(g.grid[1,9,0], 1.1)
     assert np.isclose(g.grid[6,8,0], 1.1)
     assert np.isclose(g.grid[0,1,1], .1)
     assert np.isclose(g.grid[1,9,1], .1)
     assert np.isclose(g.grid[6,8,1], .1)
 
+def test_add_from_cat_property_idx():
+    g = Grid(1, (5,5), (10,10), (1,1))
+    g.init_grid()
+    positions = np.array([[0.5,1.4],[1.2,9.9],[6.2,8.8]])
+    values = 0.1*np.ones(len(positions))
+    
+    # One property in grid:
+    g.add_from_cat(positions=positions, properties=0)
+    assert np.sum(g.grid) == 3
+    assert g.grid[0,1,0] == 1
+    assert g.grid[1,9,0] == 1
+    assert g.grid[6,8,0] == 1
+
+    # Add on top of existing
+    g.add_from_cat(positions=positions, values=values, properties=0)
+    assert np.isclose(np.sum(g.grid), 3.3)
+    assert np.isclose(g.grid[0,1,0], 1.1)
+    assert np.isclose(g.grid[1,9,0], 1.1)
+    assert np.isclose(g.grid[6,8,0], 1.1)
+
+    # Add into new property
+    g.add_from_cat(positions=positions, values=values, new_props=True)
+    assert np.isclose(np.sum(g.grid), 3.6)
+    assert np.isclose(g.grid[0,1,0], 1.1)
+    assert np.isclose(g.grid[1,9,0], 1.1)
+    assert np.isclose(g.grid[6,8,0], 1.1)
+    assert np.isclose(g.grid[0,1,1], .1)
+    assert np.isclose(g.grid[1,9,1], .1)
+    assert np.isclose(g.grid[6,8,1], .1)
+
+    # Add on top of original property
+    g.add_from_cat(positions=positions, values=values, properties=0)
+    assert np.isclose(np.sum(g.grid), 3.9)
+    assert np.isclose(g.grid[0,1,0], 1.2)
+    assert np.isclose(g.grid[1,9,0], 1.2)
+    assert np.isclose(g.grid[6,8,0], 1.2)
+    assert np.isclose(g.grid[0,1,1], .1)
+    assert np.isclose(g.grid[1,9,1], .1)
+    assert np.isclose(g.grid[6,8,1], .1)
+
+    # Add on top of new property
+    g.add_from_cat(positions=positions, values=values, properties=1)
+    assert np.isclose(np.sum(g.grid), 4.2)
+    assert np.isclose(g.grid[0,1,0], 1.2)
+    assert np.isclose(g.grid[1,9,0], 1.2)
+    assert np.isclose(g.grid[6,8,0], 1.2)
+    assert np.isclose(g.grid[0,1,1], .2)
+    assert np.isclose(g.grid[1,9,1], .2)
+    assert np.isclose(g.grid[6,8,1], .2)
+
+    # Add on top of both properties - values only has 1 property dim
+    g.add_from_cat(positions=positions, values=values, properties=None)
+    assert np.isclose(np.sum(g.grid), 4.8)
+    assert np.isclose(g.grid[0,1,0], 1.3)
+    assert np.isclose(g.grid[1,9,0], 1.3)
+    assert np.isclose(g.grid[6,8,0], 1.3)
+    assert np.isclose(g.grid[0,1,1], .3)
+    assert np.isclose(g.grid[1,9,1], .3)
+    assert np.isclose(g.grid[6,8,1], .3)
+
+    # Add on top of both properties - values only has 2 property dims
+    values_new = 0.2*np.ones(len(positions))
+    g.add_from_cat(positions=positions, values=np.array([values,values_new]).T, properties=None)
+    assert np.isclose(np.sum(g.grid), 5.7)
+    assert np.isclose(g.grid[0,1,0], 1.4)
+    assert np.isclose(g.grid[1,9,0], 1.4)
+    assert np.isclose(g.grid[6,8,0], 1.4)
+    assert np.isclose(g.grid[0,1,1], .5)
+    assert np.isclose(g.grid[1,9,1], .5)
+    assert np.isclose(g.grid[6,8,1], .5)
+
+
+
 def test_add_from_cat_edges():
     g = Grid(1, (5,5), (10,10), (1,1))
     g.init_grid()
     positions = np.array([[2,2],[8,8],[10,10],[0,0]],dtype=float)
     values = 0.1*np.ones(len(positions))
     
     g.add_from_cat(positions=positions,values=values)
@@ -207,8 +303,68 @@
 
     g.add_from_cat(positions=positions2,values=values2)
 
     s1 = g.sample(positions=positions1)
     s2 = g.sample(positions=positions2)
 
     assert np.all(np.isclose(s1, 0.1))
-    assert np.all(np.isclose(s2, 0.3))
+    assert np.all(np.isclose(s2, 0.3))
+
+
+
+def test_add_array():
+    g = Grid(1, (5,4), (10,8), (1,1))
+    g.init_grid()
+    positions0 = np.array([[0.5],[1.2]])
+    spec0 = np.ones((len(positions0),g.n_pixels[1]))
+    positions1 = np.array([[5]])
+    spec1 = np.ones((len(positions1),g.n_pixels[0]))
+
+    # Add some spectra:
+    g.add_from_pos_plus_array(positions=positions0,values=spec0)
+    assert np.sum(g.grid) == 16
+    assert np.all(g.grid[0] == 1)
+    assert np.all(g.grid[1] == 1)
+
+    # Other axis
+    g.add_from_pos_plus_array(positions=positions1,values=spec1,ax=0)
+    assert np.sum(g.grid) == 26
+    assert np.all(g.grid[2:,5] == 1)
+    assert np.all(g.grid[:2,5] == 2)
+
+    # New axis
+    g.add_from_pos_plus_array(positions=positions1,values=spec1,ax=0,new_prop=True)
+    assert np.sum(g.grid) == 36
+    assert np.all(g.grid[2:,5,0] == 1)
+    assert np.all(g.grid[:2,5,0] == 2)
+    assert np.all(g.grid[:,5,1] == 1)
+
+    # Add to multi-prop axis
+    g.add_from_pos_plus_array(positions=positions1,values=spec1,ax=0,properties=0)
+    assert np.sum(g.grid) == 46
+    assert np.all(g.grid[2:,5,0] == 2)
+    assert np.all(g.grid[:2,5,0] == 3)
+    assert np.all(g.grid[:,5,1] == 1)
+
+    # Add to multi-prop axis
+    g.add_from_pos_plus_array(positions=positions1,values=spec1,ax=0,properties=None)
+    assert np.sum(g.grid) == 66
+    assert np.all(g.grid[2:,5,0] == 3)
+    assert np.all(g.grid[:2,5,0] == 4)
+    assert np.all(g.grid[:,5,1] == 2)
+
+def test_add_array_3d():
+    g = Grid(1, (0,0,0), 5, 1)
+    g.init_grid()
+
+    position = np.array([[0,0]])
+    value = np.ones(5)
+    g.add_from_pos_plus_array(positions=position,values=np.array([value]),ax=0)
+    g.add_from_pos_plus_array(positions=position,values=np.array([value]),ax=1)
+    g.add_from_pos_plus_array(positions=position,values=np.array([value]),ax=2)
+
+    assert np.sum(g.grid) == 15
+    assert g.grid[2,2,2] == 3
+    assert g.grid[2,2,0] == 1
+    assert g.grid[2,0,2] == 1
+    assert g.grid[0,2,2] == 1
+
```

### Comparing `simim-0.3.4/tests/test_imports.py` & `simim-0.3.5/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/tests/test_instrument.py` & `simim-0.3.5/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.4/tests/test_rawsiminterface.py` & `simim-0.3.5/tests/test_rawsiminterface.py`

 * *Files identical despite different names*

