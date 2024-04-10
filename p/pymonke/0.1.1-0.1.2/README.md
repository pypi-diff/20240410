# Comparing `tmp/pymonke-0.1.1.tar.gz` & `tmp/pymonke-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonke-0.1.1.tar", last modified: Mon Apr  8 16:38:28 2024, max compression
+gzip compressed data, was "pymonke-0.1.2.tar", last modified: Wed Apr 10 16:17:01 2024, max compression
```

## Comparing `pymonke-0.1.1.tar` & `pymonke-0.1.2.tar`

### file list

```diff
@@ -1,74 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.227686 pymonke-0.1.1/
--rw-rw-rw-   0        0        0     1095 2024-01-31 16:24:15.000000 pymonke-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      695 2024-04-08 16:38:28.227185 pymonke-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5033 2024-03-03 13:48:10.000000 pymonke-0.1.1/README.md
--rw-rw-rw-   0        0        0      160 2024-03-03 13:48:10.000000 pymonke-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      920 2024-04-08 16:38:28.228685 pymonke-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.172651 pymonke-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.183165 pymonke-0.1.1/src/pymonke/
--rw-rw-rw-   0        0        0      371 2024-04-08 16:27:10.000000 pymonke-0.1.1/src/pymonke/__init__.py
--rw-rw-rw-   0        0        0      269 2024-03-15 15:51:29.000000 pymonke-0.1.1/src/pymonke/__main__.py
--rw-rw-rw-   0        0        0     1548 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.191167 pymonke-0.1.1/src/pymonke/fit/
--rw-rw-rw-   0        0        0      133 2024-03-29 19:58:06.000000 pymonke-0.1.1/src/pymonke/fit/__init__.py
--rw-rw-rw-   0        0        0     1106 2024-03-29 19:57:55.000000 pymonke-0.1.1/src/pymonke/fit/__misc.py
--rw-rw-rw-   0        0        0    10791 2024-04-08 08:02:31.000000 pymonke-0.1.1/src/pymonke/fit/fit.py
--rw-rw-rw-   0        0        0     3684 2024-04-08 07:55:52.000000 pymonke-0.1.1/src/pymonke/fit/fit_result.py
--rw-rw-rw-   0        0        0     6855 2024-04-08 08:00:58.000000 pymonke-0.1.1/src/pymonke/fit/parse.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.200167 pymonke-0.1.1/src/pymonke/gui/
--rw-rw-rw-   0        0        0      289 2024-03-22 17:45:13.000000 pymonke-0.1.1/src/pymonke/gui/__init__.py
--rw-rw-rw-   0        0        0     3880 2024-04-08 16:31:06.000000 pymonke-0.1.1/src/pymonke/gui/app.py
--rw-rw-rw-   0        0        0     1185 2024-03-23 22:03:51.000000 pymonke-0.1.1/src/pymonke/gui/browse_frame.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.203671 pymonke-0.1.1/src/pymonke/gui/data_init/
--rw-rw-rw-   0        0        0        0 2024-03-17 12:55:10.000000 pymonke-0.1.1/src/pymonke/gui/data_init/__init__.py
--rw-rw-rw-   0        0        0      751 2024-03-23 20:42:12.000000 pymonke-0.1.1/src/pymonke/gui/data_init/browse_save_frame.py
--rw-rw-rw-   0        0        0     5217 2024-03-24 15:12:49.000000 pymonke-0.1.1/src/pymonke/gui/data_init/data_init_frame.py
--rw-rw-rw-   0        0        0     1398 2024-03-24 08:58:03.000000 pymonke-0.1.1/src/pymonke/gui/data_init/status_frame.py
--rw-rw-rw-   0        0        0     5729 2024-03-25 15:55:43.000000 pymonke-0.1.1/src/pymonke/gui/dict_frame.py
--rw-rw-rw-   0        0        0     1123 2024-03-23 22:07:47.000000 pymonke-0.1.1/src/pymonke/gui/entry_label_frame.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.206173 pymonke-0.1.1/src/pymonke/gui/fitting/
--rw-rw-rw-   0        0        0     3505 2024-03-25 22:43:11.000000 pymonke-0.1.1/src/pymonke/gui/fitting/add_args_frame.py
--rw-rw-rw-   0        0        0    10162 2024-04-08 16:09:40.000000 pymonke-0.1.1/src/pymonke/gui/fitting/fit_frame.py
--rw-rw-rw-   0        0        0     2462 2024-03-24 15:12:59.000000 pymonke-0.1.1/src/pymonke/gui/fitting/fit_option_menu.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.208672 pymonke-0.1.1/src/pymonke/gui/formula/
--rw-rw-rw-   0        0        0     2889 2024-03-23 21:13:25.000000 pymonke-0.1.1/src/pymonke/gui/formula/formula_frame.py
--rw-rw-rw-   0        0        0     1424 2024-03-23 21:18:19.000000 pymonke-0.1.1/src/pymonke/gui/formula/parameter_frame.py
--rw-rw-rw-   0        0        0     2421 2024-04-08 16:10:31.000000 pymonke-0.1.1/src/pymonke/gui/formula/parameters_scrollable_frame.py
--rw-rw-rw-   0        0        0      388 2024-03-23 21:44:32.000000 pymonke-0.1.1/src/pymonke/gui/info_label.py
--rw-rw-rw-   0        0        0      561 2024-03-25 22:19:40.000000 pymonke-0.1.1/src/pymonke/gui/labeled_entry.py
--rw-rw-rw-   0        0        0     2628 2024-03-25 15:19:40.000000 pymonke-0.1.1/src/pymonke/gui/list_frame.py
--rw-rw-rw-   0        0        0      225 2024-04-08 16:32:10.000000 pymonke-0.1.1/src/pymonke/gui/main.py
--rw-rw-rw-   0        0        0     3038 2024-03-23 22:27:18.000000 pymonke-0.1.1/src/pymonke/gui/misc.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.212174 pymonke-0.1.1/src/pymonke/gui/plot/
--rw-rw-rw-   0        0        0     3560 2024-03-25 13:24:18.000000 pymonke-0.1.1/src/pymonke/gui/plot/limits_frame.py
--rw-rw-rw-   0        0        0     5207 2024-04-08 16:19:07.000000 pymonke-0.1.1/src/pymonke/gui/plot/misc_data_frame.py
--rw-rw-rw-   0        0        0     2148 2024-04-08 16:31:36.000000 pymonke-0.1.1/src/pymonke/gui/plot/plot_canvas.py
--rw-rw-rw-   0        0        0     4544 2024-04-02 20:38:13.000000 pymonke-0.1.1/src/pymonke/gui/plot/plot_frame.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.215674 pymonke-0.1.1/src/pymonke/latex/
--rw-rw-rw-   0        0        0      175 2024-04-02 12:24:16.000000 pymonke-0.1.1/src/pymonke/latex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.217175 pymonke-0.1.1/src/pymonke/latex/tests/
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/latex/tests/__init__.py
--rw-rw-rw-   0        0        0     1225 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/latex/tests/table_test.py
--rw-rw-rw-   0        0        0     3096 2024-04-02 08:30:50.000000 pymonke-0.1.1/src/pymonke/latex/tex_table.py
--rw-rw-rw-   0        0        0     4420 2024-04-02 11:45:56.000000 pymonke-0.1.1/src/pymonke/latex/utils.py
--rw-rw-rw-   0        0        0     1549 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/latex/utils.pyi
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.222184 pymonke-0.1.1/src/pymonke/misc/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:06:30.000000 pymonke-0.1.1/src/pymonke/misc/__init__.py
--rw-rw-rw-   0        0        0     1853 2024-04-02 12:26:57.000000 pymonke-0.1.1/src/pymonke/misc/benchmark.py
--rw-rw-rw-   0        0        0     3198 2024-04-02 14:02:30.000000 pymonke-0.1.1/src/pymonke/misc/dataframe.py
--rw-rw-rw-   0        0        0     1010 2024-04-02 12:27:25.000000 pymonke-0.1.1/src/pymonke/misc/file_management.py
--rw-rw-rw-   0        0        0      757 2024-04-02 20:39:13.000000 pymonke-0.1.1/src/pymonke/misc/pymonke_json_decoder.py
--rw-rw-rw-   0        0        0      297 2024-04-02 14:33:51.000000 pymonke-0.1.1/src/pymonke/misc/pymonke_json_encoder.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.224685 pymonke-0.1.1/src/pymonke/mmath/
--rw-rw-rw-   0        0        0       65 2024-04-02 12:36:10.000000 pymonke-0.1.1/src/pymonke/mmath/__init__.py
--rw-rw-rw-   0        0        0      759 2024-04-02 12:35:53.000000 pymonke-0.1.1/src/pymonke/mmath/rounding.py
--rw-rw-rw-   0        0        0      890 2024-03-14 10:22:20.000000 pymonke-0.1.1/src/pymonke/mmath/statistics.py
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.1/src/pymonke/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.226686 pymonke-0.1.1/src/pymonke.egg-info/
--rw-rw-rw-   0        0        0      695 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 16:38:28.000000 pymonke-0.1.1/src/pymonke.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 16:38:28.225685 pymonke-0.1.1/tests/
--rw-rw-rw-   0        0        0     2028 2024-04-08 16:33:36.000000 pymonke-0.1.1/tests/test.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.169873 pymonke-0.1.2/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1075 2024-02-20 17:30:31.000000 pymonke-0.1.2/LICENSE
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      673 2024-04-10 16:17:01.169873 pymonke-0.1.2/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2675 2024-04-10 16:09:02.000000 pymonke-0.1.2/README.md
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      151 2024-03-02 14:13:07.000000 pymonke-0.1.2/pyproject.toml
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      879 2024-04-10 16:17:01.169873 pymonke-0.1.2/setup.cfg
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.162873 pymonke-0.1.2/src/
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.164873 pymonke-0.1.2/src/pymonke/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      376 2024-04-10 16:14:32.000000 pymonke-0.1.2/src/pymonke/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      253 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/__main__.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.165873 pymonke-0.1.2/src/pymonke/fit/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      878 2024-04-10 07:52:58.000000 pymonke-0.1.2/src/pymonke/fit/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1093 2024-04-10 07:41:56.000000 pymonke-0.1.2/src/pymonke/fit/__misc.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)    11971 2024-04-10 15:13:30.000000 pymonke-0.1.2/src/pymonke/fit/fit.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     5275 2024-04-10 15:13:30.000000 pymonke-0.1.2/src/pymonke/fit/fit_result.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     7249 2024-04-10 15:14:19.000000 pymonke-0.1.2/src/pymonke/fit/parse.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.166873 pymonke-0.1.2/src/pymonke/gui/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      597 2024-04-10 16:10:52.000000 pymonke-0.1.2/src/pymonke/gui/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     3791 2024-04-10 08:02:30.000000 pymonke-0.1.2/src/pymonke/gui/app.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1171 2024-04-10 08:03:04.000000 pymonke-0.1.2/src/pymonke/gui/browse_frame.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.166873 pymonke-0.1.2/src/pymonke/gui/data_init/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       14 2024-04-10 08:05:14.000000 pymonke-0.1.2/src/pymonke/gui/data_init/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      728 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/data_init/browse_save_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     5092 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/data_init/data_init_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1360 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/data_init/status_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     5583 2024-04-10 08:03:16.000000 pymonke-0.1.2/src/pymonke/gui/dict_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1109 2024-04-10 08:03:23.000000 pymonke-0.1.2/src/pymonke/gui/entry_label_frame.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.166873 pymonke-0.1.2/src/pymonke/gui/fitting/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       15 2024-04-10 08:06:26.000000 pymonke-0.1.2/src/pymonke/gui/fitting/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     3418 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/fitting/add_args_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     9932 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/fitting/fit_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2397 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/fitting/fit_option_menu.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.167873 pymonke-0.1.2/src/pymonke/gui/formula/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       15 2024-04-10 08:06:22.000000 pymonke-0.1.2/src/pymonke/gui/formula/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2811 2024-04-10 14:50:36.000000 pymonke-0.1.2/src/pymonke/gui/formula/formula_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1379 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/formula/parameter_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2358 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/formula/parameters_scrollable_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      390 2024-04-10 08:03:32.000000 pymonke-0.1.2/src/pymonke/gui/info_label.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      559 2024-04-10 08:03:42.000000 pymonke-0.1.2/src/pymonke/gui/labeled_entry.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2569 2024-04-10 08:03:51.000000 pymonke-0.1.2/src/pymonke/gui/list_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      361 2024-04-10 14:49:53.000000 pymonke-0.1.2/src/pymonke/gui/main.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2949 2024-04-10 08:04:07.000000 pymonke-0.1.2/src/pymonke/gui/misc.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.167873 pymonke-0.1.2/src/pymonke/gui/plot/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       15 2024-04-10 08:06:27.000000 pymonke-0.1.2/src/pymonke/gui/plot/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     3455 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/plot/limits_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     5066 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/plot/misc_data_frame.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2088 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/gui/plot/plot_canvas.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     4557 2024-04-10 06:55:32.000000 pymonke-0.1.2/src/pymonke/gui/plot/plot_frame.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.168873 pymonke-0.1.2/src/pymonke/latex/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      169 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/latex/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2976 2024-04-10 15:18:44.000000 pymonke-0.1.2/src/pymonke/latex/tex_table.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     4341 2024-04-10 15:24:34.000000 pymonke-0.1.2/src/pymonke/latex/utils.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1338 2024-04-10 15:23:42.000000 pymonke-0.1.2/src/pymonke/latex/utils.pyi
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.168873 pymonke-0.1.2/src/pymonke/misc/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/misc/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1851 2024-04-10 15:26:03.000000 pymonke-0.1.2/src/pymonke/misc/benchmark.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     3533 2024-04-10 15:29:13.000000 pymonke-0.1.2/src/pymonke/misc/dataframe.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      980 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/misc/file_management.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      732 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/misc/pymonke_json_decoder.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      289 2024-04-09 15:28:22.000000 pymonke-0.1.2/src/pymonke/misc/pymonke_json_encoder.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.169873 pymonke-0.1.2/src/pymonke/mmath/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       74 2024-04-10 07:34:41.000000 pymonke-0.1.2/src/pymonke/mmath/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      614 2024-04-10 08:02:08.000000 pymonke-0.1.2/src/pymonke/mmath/rounding.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1123 2024-04-10 07:40:56.000000 pymonke-0.1.2/src/pymonke/mmath/statistics.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        0 2024-03-02 09:10:47.000000 pymonke-0.1.2/src/pymonke/py.typed
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-10 16:17:01.169873 pymonke-0.1.2/src/pymonke.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      673 2024-04-10 16:17:01.000000 pymonke-0.1.2/src/pymonke.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1809 2024-04-10 16:17:01.000000 pymonke-0.1.2/src/pymonke.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2024-04-10 16:17:01.000000 pymonke-0.1.2/src/pymonke.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      139 2024-04-10 16:17:01.000000 pymonke-0.1.2/src/pymonke.egg-info/requires.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        8 2024-04-10 16:17:01.000000 pymonke-0.1.2/src/pymonke.egg-info/top_level.txt
```

### Comparing `pymonke-0.1.1/LICENSE` & `pymonke-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Gabriel Remiszewski
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Gabriel Remiszewski
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pymonke-0.1.1/src/pymonke/fit/__misc.py` & `pymonke-0.1.2/src/pymonke/fit/__misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from typing import Any
-
-
-def generate_meta_dict() -> dict[str, Any]:
-    """Generates a dictionary with all possible keys accepted by the Fit class as meta data and sets the values
-    to none."""
-    return {
-        "plotting_style": None,
-        "file": None,
-        "x": None,
-        "y": None,
-        "fits": {
-            "generic fit name": {
-                "plotting_style": None,
-                "fit_type": "odr",
-                "function": "m * x + b",
-                "x_min_limit": None,
-                "x_max_limit": None,
-                "plot_x_min_limit": None,
-                "plot_x_max_limit": None,
-                "start_parameters": None,
-                "fit_points": None,
-                "absolute_sigma": None,
-                "check_finite": None,
-                "label": None
-            }
-        },
-        "x_min_limit": None,
-        "x_max_limit": None,
-        "y_min_limit": None,
-        "y_max_limit": None,
-        "figure_style": None,
-        "figure_dpi": None,
-        "figure_size": None,
-        "label": None
-    }
+from typing import Any
+
+
+def generate_meta_dict() -> dict[str, Any]:
+    """Generates a dictionary with all possible keys accepted by the Fit class as meta data and sets the values
+    to none."""
+    return {
+        "plotting_style": None,
+        "file": None,
+        "x": None,
+        "y": None,
+        "latex": None,
+        "fits": {
+            "generic fit name": {
+                "plotting_style": None,
+                "fit_type": "odr",
+                "function": "m * x + b",
+                "x_min_limit": None,
+                "x_max_limit": None,
+                "plot_x_min_limit": None,
+                "plot_x_max_limit": None,
+                "start_parameters": None,
+                "fit_points": None,
+                "absolute_sigma": None,
+                "check_finite": None,
+                "label": None
+            }
+        },
+        "x_min_limit": None,
+        "x_max_limit": None,
+        "y_min_limit": None,
+        "y_max_limit": None,
+        "figure_style": None,
+        "figure_dpi": None,
+        "figure_size": None,
+        "label": None
+    }
```

### Comparing `pymonke-0.1.1/src/pymonke/fit/fit.py` & `pymonke-0.1.2/src/pymonke/fit/fit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,274 +1,300 @@
-from typing import List, Dict, Tuple, Callable, TypeAlias, Optional, Any
-import warnings
-
-import matplotlib.pyplot as plt
-from matplotlib.figure import Figure, SubFigure
-from matplotlib.axes import Axes
-from mypy_extensions import VarArg
-import numpy as np
-from pandas import DataFrame, Series
-from scipy import odr
-from scipy.optimize import curve_fit
-
-from .fit_result import FitResult, result
-from .parse import parse_function, replace_funcs, numerical, scalar, array, parse_variable_str
-from ..misc.dataframe import get_error_column_name, has_uncertainty
-from ..misc.file_management import read_data_into_dataframe
-
-func_type: TypeAlias = Callable[[numerical, VarArg(scalar)], numerical]
-
-
-class Fit:
-    def __init__(self, meta: dict, data: DataFrame | None = None):
-        self.meta = meta
-        if data is None:
-            self.file: str = meta["file"]
-            if (args := meta.get("read_data_args")) is not None:
-                self.data: DataFrame = read_data_into_dataframe(self.file, **args)
-            else:
-                self.data = read_data_into_dataframe(self.file)
-        else:
-            self.data = data
-
-        self.result: Optional[dict[str, FitResult]] = None
-
-        self.column_names = self.__get_column_names(meta.get("error_marker"))
-
-    def __get_column_names(self, error_marker: List[str] | None = None) -> Dict[str, str]:
-        if error_marker is None:
-            error_marker = ["err", "error", "fehler", "Err", "Error", "Fehler"]
-        names: Dict[str, str] = dict()
-        names["x"] = self.meta["x"]
-        names["y"] = self.meta["y"]
-        x_error = get_error_column_name(self.data, names["x"], error_marker)
-        y_error = get_error_column_name(self.data, names["y"], error_marker)
-
-        names["y error"] = y_error
-        names["x error"] = x_error
-
-        return names
-
-    # ------------------------------------------------------------------------------------
-    # -------------------------------Plot with Matplotlib---------------------------------
-    # ------------------------------------------------------------------------------------
-    def plot(self, figure_id: Optional[int | str | Figure | SubFigure] = None, ax: Optional[Axes] = None):
-        if (style := self.meta.get("figure_style")) is None:
-            style = "science"
-        try:
-            plt.style.use(style)
-        except Exception as e:
-            message = f"figure style {style} not found. Using default instead.\n{e}"
-            warnings.warn(message, RuntimeWarning)
-            plt.style.use("default")
-
-        if ax is None:
-            if (size := self.meta.get("figure_size")) is None:
-                size = (6, 4.7)
-            if (dpi := self.meta.get("figure_dpi")) is None:
-                dpi = 120
-            plt.figure(num=figure_id, figsize=size, dpi=dpi)
-
-        data = self.__get_data()
-        x, y, sx, sy = data["x"], data["y"], data["sx"], data["sy"]
-
-        plotting_style = {
-            "linestyle": "",
-            "ms": 4,
-            "marker": "o",
-            "capsize": 3.5,
-            "zorder": 2
-        }
-
-        if (more_style := self.meta.get("plotting_style")) is not None:
-            plotting_style.update(more_style)
-
-        if ax is None:
-            plt.errorbar(x, y, yerr=sy, xerr=sx, **plotting_style,
-                         label=self.meta.get("label") or "Data Points")
-            plt.xlim(self.__get_xlim(self.meta))
-            plt.ylim(self.__get_ylim(self.meta, plt.ylim()))
-            plt.rc('axes', axisbelow=True)
-        else:
-            ax.errorbar(x, y, yerr=sy, xerr=sx, **plotting_style,
-                        label=self.meta.get("label") or "Data Points")
-            ax.set_xlim(self.__get_xlim(self.meta))
-            ax.set_ylim(self.__get_ylim(self.meta, ax.get_ylim()))
-            ax.set_axisbelow(True)
-
-        if self.result is not None:
-            for fit_name in self.result.keys():
-                self.__plot_fit(fit_name, self.result[fit_name], ax)
-
-        if ax is None:
-            plt.legend()
-        else:
-            ax.legend()
-
-    def __plot_fit(self, name: str, fit_res: FitResult, ax: Optional[Axes] = None) -> None:
-        meta: dict = self.meta["fits"][name]
-        if (points := meta.get("fit_points")) is None:
-            points = 150
-
-        plotting_style = {
-            "linestyle": "--",
-            "zorder": 1,
-            "linewidth": 1.6,
-        }
-
-        if (more_style := meta.get("plotting_style")) is not None:
-            plotting_style.update(more_style)
-
-        limits: List[float] = list(self.__get_xlim(meta))
-        if (val := meta.get("plot_x_min_limit")) is not None:
-            limits[0] = val
-        if (val := meta.get("plot_x_max_limit")) is not None:
-            limits[1] = val
-        x = np.linspace(*limits, points)
-        label = parse_variable_str(meta.get("label") or "$\\chi^2 = #chi $", fit_res, self.meta.get("latex") or False)
-        if ax is None:
-            plt.plot(x, fit_res.eval(x), **plotting_style, label=label)
-        else:
-            ax.plot(x, fit_res.eval(x), **plotting_style, label=label)
-
-    # ----------------------------------------------------------------------------------------
-
-    def get_results_as_dict(self) -> Dict[str, Any]:
-        result = dict()
-        for key, value in self.result.items():
-            result[key] = value.as_dict(True)
-
-        return result
-
-    def __get_xlim(self, meta: dict) -> Tuple[float, float]:
-        x = self.column_names["x"]
-        if (x_min := meta.get("x_min_limit")) is None:
-            x_min = self.data[x].min()
-        if (x_max := meta.get("x_max_limit")) is None:
-            x_max = self.data[x].max()
-
-        return x_min, x_max
-
-    def __get_ylim(self, meta: dict, ylim: Tuple[float, float]) -> Tuple[float, float]:
-        ylim = list(ylim)
-        if (y_min := meta.get("y_min_limit")) is not None:
-            ylim[0] = y_min
-        if (y_max := meta.get("y_max_limit")) is not None:
-            ylim[1] = y_max
-
-        return tuple(ylim)
-
-    def run(self) -> dict[str, FitResult]:
-        if (val := self.meta.get("fits")) is None:
-            return dict()
-        fits_meta: dict[str, dict] = val
-        result: dict[str, FitResult] = dict()
-        for fit_name in fits_meta.keys():
-            result[fit_name] = self.__do_fit(fits_meta[fit_name])
-
-        self.result = result
-
-        return result
-
-    def __do_fit(self, meta: dict) -> FitResult:
-        if meta["fit_type"] == "optimize.curve_fit":
-            return self.__do_optimize_curve_fit(meta)
-        elif meta["fit_type"] == "odr":
-            return self.__do_odr_fit(meta)
-        else:
-            raise ValueError(f"unknown fit type: {meta['fit_type']}")
-
-    def __do_optimize_curve_fit(self, meta: dict) -> FitResult:
-        function, params, p0, lim, arrays = self.__get_fitting_data(meta)
-        x, y, y_error = arrays["x"], arrays["y"], arrays["sy"]
-        assert isinstance(x, Series) and isinstance(y, Series) and isinstance(y_error, Series)
-
-        if (b := meta.get("absolute_sigma")) is None:
-            b = False
-        if (check_finite := meta.get("check_finite")) is None:
-            check_finite = False
-        out: tuple = curve_fit(function, xdata=x, ydata=y, sigma=y_error, absolute_sigma=b,
-                               check_finite=check_finite, p0=p0)
-        popt, pcov = out
-        # fit_res = FitResult(function, params, popt, np.sqrt(pcov.diagonal()))
-        # fit_res.set_reduced_chi_squared(x, y, y_error)
-        fit_res = result(function, x, y, y_error, param_names=params, params=popt,
-                         params_std_dev=np.sqrt(pcov.diagonal()))
-        return fit_res
-
-    def __do_odr_fit(self, meta: dict) -> FitResult:
-        function, params, p0, lim, arrays = self.__get_fitting_data(meta)
-        x, y, sy = arrays["x"], arrays["y"], arrays["sy"]
-        sx = arrays.get("sx")
-        assert isinstance(x, Series) and isinstance(y, Series) and isinstance(sy, Series)
-        if (b := meta.get("absolute_sigma")) is None:
-            b = False
-
-        if b:
-            odr_data = odr.RealData(x=x, y=y, sy=sy, sx=sx)
-        else:
-            wd = None
-            if sx is not None:
-                wd = 1 / sx ** 2
-            odr_data = odr.Data(x=x, y=y, we=1 / sy ** 2, wd=wd)
-
-        def odr_func(_b: list, _x: float | int) -> numerical:
-            return function(_x, *_b)
-
-        odr_model = odr.Model(odr_func)
-        odr_odr = odr.ODR(odr_data, odr_model, p0)
-        odr_out: odr.Output = odr_odr.run()
-        # fit_res = FitResult(function, params, odr_out.beta, odr_out.sd_beta)
-        # fit_res.set_reduced_chi_squared(x, y, sy)
-        fit_res = result(function, x, y, sy, param_names=params, params=odr_out.beta, params_std_dev=odr_out.sd_beta,
-                         sx=sx)
-        return fit_res
-
-    def __get_fitting_data(self, meta: dict) -> Any:
-
-        p0: List[float | int] = meta["start_parameters"]
-        x_min, x_max = self.__get_xlim(meta)
-
-        query = f"{self.column_names['x']} >= {x_min} and {self.column_names['x']} <= {x_max}"
-        # data = self.data.query(query)
-
-        fitting_data = self.__get_data(query)
-
-        function, params = parse_function(replace_funcs(meta["function"]))
-
-        lim: Tuple[float, float] = (x_min, x_max)
-
-        return function, params, p0, lim, fitting_data
-
-    def __get_data(self, query: str = None) -> dict[str, Any]:
-        if query is None:
-            data = self.data
-        else:
-            data = self.data.query(query)
-
-        x: Series
-        sx: Optional[Series] = None
-        y: Series
-        sy: Series
-
-        if has_uncertainty(data[self.column_names["x"]]):
-            x = data[self.column_names["x"]].apply(lambda x: x.nominal_value)
-            sx = data[self.column_names["x"]].apply(lambda x: x.std_dev)
-        else:
-            x = data[self.column_names["x"]]
-            if (name := self.column_names.get("x error")) is not None:
-                sx = data[name]
-        if has_uncertainty(data[self.column_names["y"]]):
-            y = data[self.column_names["y"]].apply(lambda x: x.nominal_value)
-            sy = data[self.column_names["y"]].apply(lambda x: x.std_dev)
-        else:
-            y = data[self.column_names["y"]]
-            sy = data[self.column_names["y error"]]
-
-        fitting_data: Dict[str, array | Optional[array]] = {
-            "x": x,
-            "y": y,
-            "sy": sy,
-            "sx": sx,
-        }
-
-        return fitting_data
+from typing import List, Dict, Tuple, Callable, TypeAlias, Optional, Any
+import warnings
+
+import matplotlib.pyplot as plt
+from matplotlib.figure import Figure, SubFigure
+from matplotlib.axes import Axes
+from mypy_extensions import VarArg
+import numpy as np
+from pandas import DataFrame, Series
+from scipy import odr
+from scipy.optimize import curve_fit
+
+from .fit_result import FitResult, result
+from .parse import parse_function, replace_funcs, _numerical, _scalar, _array, _parse_variable_str
+from ..misc.dataframe import get_error_column_name, has_uncertainty
+from ..misc.file_management import read_data_into_dataframe
+
+_func_type: TypeAlias = Callable[[_numerical, VarArg(_scalar)], _numerical]
+
+
+class Fit:
+    """Class for data fitting"""
+    def __init__(self, meta: dict, data: DataFrame | None = None):
+        """
+        :param meta: Dictionary containing all the data needed to fit a model to the data.
+        :param data: DataFrame containing the data used to fit one or multiple models. If this is None,
+        the data will be read from the file specified in the meta dict.
+        :raises keyError: If meta does not specify a file with the data.
+        """
+        self.meta = meta
+        """Dictionary containing all the data needed to fit a model to the data."""
+
+        if data is None:
+            self.__file: str = meta["file"]
+            if (args := meta.get("read_data_args")) is not None:
+                self.data: DataFrame = read_data_into_dataframe(self.__file, **args)
+            else:
+                self.data = read_data_into_dataframe(self.__file)
+        else:
+            self.data = data
+
+        self.result: Optional[dict[str, FitResult]] = None
+        """The Results of the fits. Because one can do multiple fits with the same data, the 
+        results will be stored in a dictionary with FitResult objects as values."""
+
+        self.__column_names = self.__get_column_names(meta.get("error_marker"))
+
+    def __get_column_names(self, error_marker: List[str] | None = None) -> Dict[str, str | None]:
+        if error_marker is None:
+            error_marker = ["err", "error", "fehler", "Err", "Error", "Fehler"]
+        names: Dict[str, str | None] = dict()
+        names["x"] = self.meta["x"]
+        names["y"] = self.meta["y"]
+        assert names["x"] is not None and names["y"] is not None
+        x_error = get_error_column_name(self.data, names["x"], error_marker)
+        y_error = get_error_column_name(self.data, names["y"], error_marker)
+
+        names["y error"] = y_error
+        names["x error"] = x_error
+
+        return names
+
+    # ------------------------------------------------------------------------------------
+    # -------------------------------Plot with Matplotlib---------------------------------
+    # ------------------------------------------------------------------------------------
+    def plot(self, figure_id: Optional[int | str | Figure | SubFigure] = None, ax: Optional[Axes] = None):
+        """Plot the fitted data with matplotlib.
+
+        :param figure_id: If given, plot the data in the figure with this ID.
+        :param ax: If given, plot the data in the given Axes"""
+        if (style := self.meta.get("figure_style")) is None:
+            style = "default"
+        try:
+            plt.style.use(style)
+        except Exception as e:
+            message = f"figure style {style} not found. Using default instead.\n{e}"
+            warnings.warn(message, RuntimeWarning)
+            plt.style.use("default")
+
+        if ax is None:
+            if (size := self.meta.get("figure_size")) is None:
+                size = (6, 4.7)
+            if (dpi := self.meta.get("figure_dpi")) is None:
+                dpi = 120
+            plt.figure(num=figure_id, figsize=size, dpi=dpi)
+
+        data = self.__get_data()
+        x, y, sx, sy = data["x"], data["y"], data["sx"], data["sy"]
+
+        plotting_style = {
+            "linestyle": "",
+            "ms": 4,
+            "marker": "o",
+            "capsize": 3.5,
+            "zorder": 2
+        }
+
+        if (more_style := self.meta.get("plotting_style")) is not None:
+            plotting_style.update(more_style)
+
+        if ax is None:
+            plt.errorbar(x, y, yerr=sy, xerr=sx, **plotting_style,  # type: ignore
+                         label=self.meta.get("label") or "Data Points")
+            plt.xlim(self.__get_xlim(self.meta))
+            plt.ylim(self.__get_ylim(self.meta, plt.ylim()))
+            plt.rc('axes', axisbelow=True)
+        else:
+            ax.errorbar(x, y, yerr=sy, xerr=sx, **plotting_style,  # type: ignore
+                        label=self.meta.get("label") or "Data Points")
+            ax.set_xlim(self.__get_xlim(self.meta))
+            ax.set_ylim(self.__get_ylim(self.meta, ax.get_ylim()))
+            ax.set_axisbelow(True)
+
+        if self.result is not None:
+            for fit_name in self.result.keys():
+                self.__plot_fit(fit_name, self.result[fit_name], ax)
+
+        if ax is None:
+            plt.legend()
+        else:
+            ax.legend()
+
+    def __plot_fit(self, name: str, fit_res: FitResult, ax: Optional[Axes] = None) -> None:
+        meta: dict = self.meta["fits"][name]
+        if (points := meta.get("fit_points")) is None:
+            points = 150
+
+        plotting_style = {
+            "linestyle": "--",
+            "zorder": 1,
+            "linewidth": 1.6,
+        }
+
+        if (more_style := meta.get("plotting_style")) is not None:
+            plotting_style.update(more_style)
+
+        limits: List[float] = list(self.__get_xlim(meta))
+        if (val := meta.get("plot_x_min_limit")) is not None:
+            limits[0] = val
+        if (val := meta.get("plot_x_max_limit")) is not None:
+            limits[1] = val
+        x = np.linspace(*limits, points)  # type: ignore
+        label = _parse_variable_str(meta.get("label") or "$\\chi^2 = #chi $", fit_res, self.meta.get("latex") or False)
+        if ax is None:
+            plt.plot(x, fit_res.eval(x), **plotting_style, label=label)  # type: ignore
+        else:
+            ax.plot(x, fit_res.eval(x), **plotting_style, label=label)  # type: ignore
+
+    # ----------------------------------------------------------------------------------------
+
+    def get_results_as_dict(self) -> Dict[str, Any]:
+        """
+
+        :return: Dictionary, but turns fit FitResult object into a dictionary
+        """
+        if self.result is None:
+            raise Exception("No Result available. Try to run the fits first.")
+        result = dict()
+        for key, value in self.result.items():
+            result[key] = value.as_dict(True)
+
+        return result
+
+    def __get_xlim(self, meta: dict) -> Tuple[float, float]:
+        x = self.__column_names["x"]
+        if (x_min := meta.get("x_min_limit")) is None:
+            x_min = self.data[x].min()
+        if (x_max := meta.get("x_max_limit")) is None:
+            x_max = self.data[x].max()
+
+        return x_min, x_max
+
+    def __get_ylim(self, meta: dict, ylim: Tuple[float, float]) -> Tuple[float, float]:
+        ylim_: list = list(ylim)
+        if (y_min := meta.get("y_min_limit")) is not None:
+            ylim_[0] = y_min
+        if (y_max := meta.get("y_max_limit")) is not None:
+            ylim_[1] = y_max
+
+        return ylim_[0], ylim_[1]
+
+    def run(self) -> dict[str, FitResult]:
+        """Do the fits with the specified fitting methods
+
+        :return: A dictionary containing FitResult objects as values with the fit names as keys
+        """
+        if (val := self.meta.get("fits")) is None:
+            return dict()
+        fits_meta: dict[str, dict] = val
+        result: dict[str, FitResult] = dict()
+        for fit_name in fits_meta.keys():
+            result[fit_name] = self.__do_fit(fits_meta[fit_name])
+
+        self.result = result
+
+        return result
+
+    def __do_fit(self, meta: dict) -> FitResult:
+        if meta["fit_type"] == "optimize.curve_fit":
+            return self.__do_optimize_curve_fit(meta)
+        elif meta["fit_type"] == "odr":
+            return self.__do_odr_fit(meta)
+        else:
+            raise ValueError(f"unknown fit type: {meta['fit_type']}")
+
+    def __do_optimize_curve_fit(self, meta: dict) -> FitResult:
+        function, params, p0, lim, arrays = self.__get_fitting_data(meta)
+        x, y, y_error = arrays["x"], arrays["y"], arrays["sy"]
+        assert isinstance(x, Series) and isinstance(y, Series) and isinstance(y_error, Series)
+
+        if (b := meta.get("absolute_sigma")) is None:
+            b = False
+        if (check_finite := meta.get("check_finite")) is None:
+            check_finite = False
+        out: tuple = curve_fit(function, xdata=x, ydata=y, sigma=y_error, absolute_sigma=b,
+                               check_finite=check_finite, p0=p0)
+        popt, pcov = out
+        # fit_res = FitResult(function, params, popt, np.sqrt(pcov.diagonal()))
+        # fit_res.set_reduced_chi_squared(x, y, y_error)
+        fit_res = result(function, x, y, y_error, param_names=params, params=popt,
+                         params_std_dev=np.sqrt(pcov.diagonal()))
+        return fit_res
+
+    def __do_odr_fit(self, meta: dict) -> FitResult:
+        function, params, p0, lim, arrays = self.__get_fitting_data(meta)
+        x, y, sy = arrays["x"], arrays["y"], arrays["sy"]
+        sx = arrays.get("sx")
+        assert isinstance(x, Series) and isinstance(y, Series) and isinstance(sy, Series)
+        if (b := meta.get("absolute_sigma")) is None:
+            b = False
+
+        if b:
+            odr_data = odr.RealData(x=x, y=y, sy=sy, sx=sx)
+        else:
+            wd = None
+            if sx is not None:
+                wd = 1 / sx ** 2
+            odr_data = odr.Data(x=x, y=y, we=1 / sy ** 2, wd=wd)
+
+        def odr_func(_b: list, _x: float | int) -> _numerical:
+            return function(_x, *_b)
+
+        odr_model = odr.Model(odr_func)
+        odr_odr = odr.ODR(odr_data, odr_model, p0)
+        odr_out: odr.Output = odr_odr.run()
+        # fit_res = FitResult(function, params, odr_out.beta, odr_out.sd_beta)
+        # fit_res.set_reduced_chi_squared(x, y, sy)
+        fit_res = result(function, x, y, sy, param_names=params, params=odr_out.beta, params_std_dev=odr_out.sd_beta,
+                         sx=sx)
+        return fit_res
+
+    def __get_fitting_data(self, meta: dict) -> Any:
+
+        p0: List[float | int] = meta["start_parameters"]
+        x_min, x_max = self.__get_xlim(meta)
+
+        query = f"{self.__column_names['x']} >= {x_min} and {self.__column_names['x']} <= {x_max}"
+        # data = self.data.query(query)
+
+        fitting_data = self.__get_data(query)
+
+        function, params = parse_function(replace_funcs(meta["function"]))
+
+        lim: Tuple[float, float] = (x_min, x_max)
+
+        return function, params, p0, lim, fitting_data
+
+    def __get_data(self, query: str = None) -> dict[str, Any]:
+        if query is None:
+            data = self.data
+        else:
+            data = self.data.query(query)
+
+        x: Series
+        sx: Optional[Series] = None
+        y: Series
+        sy: Series
+
+        if has_uncertainty(data[self.__column_names["x"]]):
+            x = data[self.__column_names["x"]].apply(lambda x: x.nominal_value)
+            sx = data[self.__column_names["x"]].apply(lambda x: x.std_dev)
+        else:
+            x = data[self.__column_names["x"]]
+            if (name := self.__column_names.get("x error")) is not None:
+                sx = data[name]
+        if has_uncertainty(data[self.__column_names["y"]]):
+            y = data[self.__column_names["y"]].apply(lambda x: x.nominal_value)
+            sy = data[self.__column_names["y"]].apply(lambda x: x.std_dev)
+        else:
+            y = data[self.__column_names["y"]]
+            sy = data[self.__column_names["y error"]]
+
+        fitting_data: Dict[str, _array | Optional[_array]] = {
+            "x": x,
+            "y": y,
+            "sy": sy,
+            "sx": sx,
+        }
+
+        return fitting_data
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/app.py` & `pymonke-0.1.2/src/pymonke/gui/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,107 @@
-from typing import Optional, Any
-
-import customtkinter as ctk
-from pandas import DataFrame, Series
-
-from .data_init.data_init_frame import DataInitFrame
-from .dict_frame import DictFrame
-from .fitting.fit_frame import FitFrame
-from .misc import Root
-from .plot.plot_frame import PlotFrame
-from ..fit.fit import Fit
-from ..fit.fit_result import FitResult
-from ..misc.dataframe import get_error_column_name
-
-
-class App(Root, ctk.CTk):
-    def __init__(self, rel_height: float = 0.6, rel_width: float = 0.8):
-        ctk.CTk.__init__(self)
-
-        self.geometry(self.__get_geometry(rel_height, rel_width))
-        self.title("PyMonke data fitting")
-        self.grid_columnconfigure((0, 1), weight=5)
-        self.grid_columnconfigure(2, weight=8)
-        self.fit: Optional[Fit] = None
-
-        # DATA
-        self.meta: dict[str, Any] = dict()
-        self.data: Optional[DataFrame] = None
-        self.fit_result: Optional[dict[str, FitResult]] = None
-
-        self.plot_frame = PlotFrame(master=self)
-        self.plot_frame.grid(row=0, column=1)
-
-        self.data_init = DataInitFrame(master=self)
-        self.data_init.load_meta_frame.button.configure(command=self.load_meta)
-        self.data_init.browse_data_frame.button.configure(command=self.load_data)
-        self.data_init.grid(row=0, column=0)
-
-        self.fit_frame = FitFrame(master=self)
-        self.fit_frame.grid(row=0, column=2, sticky="nsew", padx=50, rowspan=2)
-
-    def __get_geometry(self, rel_height: float, rel_width: float) -> str:
-        screen_width = self.winfo_screenwidth() * rel_width
-        screen_height = self.winfo_screenheight() * rel_height
-        result = f"{int(screen_width)}x{int(screen_height)}"
-        return result
-
-    def get_fit_frame(self) -> FitFrame:
-        return self.fit_frame
-
-    def get_fit_meta(self) -> Optional[dict[str, Any]]:
-        fit = self.get_fit_frame().get_fit_name()
-        if fit is None:
-            return None
-        ret = self.meta["fits"][fit]
-        assert isinstance(ret, dict)
-        return ret
-
-    def load_meta(self) -> None:
-        if (val := self.data_init.load_meta()) is not None:
-            while self.meta != dict():
-                self.meta.popitem()
-            self.meta.update(val)
-        self.load_from_meta()
-
-    def load_data(self) -> None:
-        self.data = self.data_init.load_data()
-
-    def load_from_meta(self) -> None:
-        # self.read_data_arguments_frame.load_parameters(self.meta)
-        self.fit_frame.delete_all_fits()
-        self.data_init.load_from_meta()
-        self.plot_frame.load_from_meta()
-        self.fit_frame.load_from_meta()
-        # self.load_plotting_style_arguments_from_fit_meta()
-
-    def get_plot_frame(self) -> Any:
-        return self.plot_frame
-
-    def get_x(self) -> "Optional[Series[float]]":
-        if (x := self.meta.get("x")) is not None and self.data is not None:
-            assert isinstance(self.data, dict)
-            return self.data[x]
-        return None
-
-    def do_fit(self) -> Fit:
-        fit: Fit = Fit(meta=self.meta, data=self.data)
-        self.fit_result = fit.run()
-        return fit
-
-    def get_y(self) -> "Optional[Series[float]]":
-        if (y := self.meta.get("y")) is not None and self.data is not None:
-            assert isinstance(self.data, dict)
-            return self.data[y]
-        return None
-
-    def get_sy(self) -> "Optional[Series[float]]":
-        if (y := self.meta.get("y")) is not None and self.data is not None:
-            return self.data[get_error_column_name(self.data, y)]
-        return None
-
-    def get_sx(self) -> "Optional[Series[float]]":
-        if (x := self.meta.get("x")) is not None and self.data is not None:
-            return self.data.get(get_error_column_name(self.data, x))
-        return None
+"""@private"""
+
+from typing import Optional, Any
+
+import customtkinter as ctk
+from pandas import DataFrame, Series
+
+from .data_init.data_init_frame import DataInitFrame
+from .dict_frame import DictFrame
+from .fitting.fit_frame import FitFrame
+from .misc import Root
+from .plot.plot_frame import PlotFrame
+from ..fit.fit import Fit
+from ..fit.fit_result import FitResult
+from ..misc.dataframe import get_error_column_name
+
+
+class App(Root, ctk.CTk):
+    def __init__(self, rel_height: float = 0.6, rel_width: float = 0.8):
+        ctk.CTk.__init__(self)
+
+        self.geometry(self.__get_geometry(rel_height, rel_width))
+        self.title("PyMonke data fitting")
+        self.grid_columnconfigure((0, 1), weight=5)
+        self.grid_columnconfigure(2, weight=8)
+        self.fit: Optional[Fit] = None
+
+        # DATA
+        self.meta: dict[str, Any] = dict()
+        self.data: Optional[DataFrame] = None
+        self.fit_result: Optional[dict[str, FitResult]] = None
+
+        self.plot_frame = PlotFrame(master=self)
+        self.plot_frame.grid(row=0, column=1)
+
+        self.data_init = DataInitFrame(master=self)
+        self.data_init.load_meta_frame.button.configure(command=self.load_meta)
+        self.data_init.browse_data_frame.button.configure(command=self.load_data)
+        self.data_init.grid(row=0, column=0)
+
+        self.fit_frame = FitFrame(master=self)
+        self.fit_frame.grid(row=0, column=2, sticky="nsew", padx=50, rowspan=2)
+
+    def __get_geometry(self, rel_height: float, rel_width: float) -> str:
+        screen_width = self.winfo_screenwidth() * rel_width
+        screen_height = self.winfo_screenheight() * rel_height
+        result = f"{int(screen_width)}x{int(screen_height)}"
+        return result
+
+    def get_fit_frame(self) -> FitFrame:
+        return self.fit_frame
+
+    def get_fit_meta(self) -> Optional[dict[str, Any]]:
+        fit = self.get_fit_frame().get_fit_name()
+        if fit is None:
+            return None
+        ret = self.meta["fits"][fit]
+        assert isinstance(ret, dict)
+        return ret
+
+    def load_meta(self) -> None:
+        if (val := self.data_init.load_meta()) is not None:
+            while self.meta != dict():
+                self.meta.popitem()
+            self.meta.update(val)
+        self.load_from_meta()
+
+    def load_data(self) -> None:
+        self.data = self.data_init.load_data()
+
+    def load_from_meta(self) -> None:
+        # self.read_data_arguments_frame.load_parameters(self.meta)
+        self.fit_frame.delete_all_fits()
+        self.data_init.load_from_meta()
+        self.plot_frame.load_from_meta()
+        self.fit_frame.load_from_meta()
+        # self.load_plotting_style_arguments_from_fit_meta()
+
+    def get_plot_frame(self) -> Any:
+        return self.plot_frame
+
+    def get_x(self) -> "Optional[Series[float]]":
+        if (x := self.meta.get("x")) is not None and self.data is not None:
+            assert isinstance(self.data, dict)
+            return self.data[x]
+        return None
+
+    def do_fit(self) -> Fit:
+        fit: Fit = Fit(meta=self.meta, data=self.data)
+        self.fit_result = fit.run()
+        return fit
+
+    def get_y(self) -> "Optional[Series[float]]":
+        if (y := self.meta.get("y")) is not None and self.data is not None:
+            assert isinstance(self.data, dict)
+            return self.data[y]
+        return None
+
+    def get_sy(self) -> "Optional[Series[float]]":
+        if (y := self.meta.get("y")) is not None and self.data is not None:
+            return self.data[get_error_column_name(self.data, y)]
+        return None
+
+    def get_sx(self) -> "Optional[Series[float]]":
+        if (x := self.meta.get("x")) is not None and self.data is not None:
+            return self.data.get(get_error_column_name(self.data, x))
+        return None
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/browse_frame.py` & `pymonke-0.1.2/src/pymonke/gui/browse_frame.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from customtkinter import CTkFrame, CTkEntry, StringVar, CTkButton
-
-from typing import Any
-
-from .misc import browse_files
-
-
-class BrowseFrame(CTkFrame):
-    def __init__(self, file_type: str, placeholder: str = "Enter the file path", browse_text: str = "browse",
-                 **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-
-        self.type = file_type
-        self.file_path = StringVar(master=self, value=None)
-        self.entry = CTkEntry(master=self, placeholder_text=placeholder, width=200)
-        self.entry.bind("<Leave>", self.__check_text_if_empty)
-        self.entry.grid(row=0, column=0, sticky="w")
-
-        self.button = CTkButton(master=self, text=browse_text, command=self.browse, width=40)
-        self.button.grid(row=0, column=1)
-
-    def browse(self) -> Any:
-        self.entry.configure(textvariable=self.file_path)
-        self.file_path.set(browse_files("select Data file", self.type))
-
-    def __check_text_if_empty(self, _: Any = None) -> Any:
-        if self.file_path.get() == "":
-            self.entry.configure(textvariable=None)
-        else:
-            self.entry.configure(textvariable=self.file_path)
+"""@private"""
+
+from customtkinter import CTkFrame, CTkEntry, StringVar, CTkButton
+
+from typing import Any
+
+from .misc import browse_files
+
+
+class BrowseFrame(CTkFrame):
+    def __init__(self, file_type: str, placeholder: str = "Enter the file path", browse_text: str = "browse",
+                 **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+
+        self.type = file_type
+        self.file_path = StringVar(master=self, value=None)
+        self.entry = CTkEntry(master=self, placeholder_text=placeholder, width=200)
+        self.entry.bind("<Leave>", self.__check_text_if_empty)
+        self.entry.grid(row=0, column=0, sticky="w")
+
+        self.button = CTkButton(master=self, text=browse_text, command=self.browse, width=40)
+        self.button.grid(row=0, column=1)
+
+    def browse(self) -> Any:
+        self.entry.configure(textvariable=self.file_path)
+        self.file_path.set(browse_files("select Data file", self.type))
+
+    def __check_text_if_empty(self, _: Any = None) -> Any:
+        if self.file_path.get() == "":
+            self.entry.configure(textvariable=None)
+        else:
+            self.entry.configure(textvariable=self.file_path)
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/data_init/browse_save_frame.py` & `pymonke-0.1.2/src/pymonke/gui/data_init/browse_save_frame.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from customtkinter import CTkFrame, CTkButton
-
-import json
-from typing import Any
-
-from ..browse_frame import BrowseFrame
-from ..misc import get_meta
-
-
-class BrowseSaveFrame(CTkFrame):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-        self.save_button = CTkButton(master=self, text="Save", width=30, command=self.save)
-        self.save_button.grid(row=0, column=0)
-
-        self.browse_frame = BrowseFrame(master=self, file_type=".*")
-        self.browse_frame.grid(row=0, column=1)
-
-    def save(self) -> None:
-        file = self.browse_frame.file_path.get()
-        with open(file, "w") as f:
-            _input: str = json.dumps(get_meta(self), indent=4)
-            f.write(_input)
+from customtkinter import CTkFrame, CTkButton
+
+import json
+from typing import Any
+
+from ..browse_frame import BrowseFrame
+from ..misc import get_meta
+
+
+class BrowseSaveFrame(CTkFrame):
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+        self.save_button = CTkButton(master=self, text="Save", width=30, command=self.save)
+        self.save_button.grid(row=0, column=0)
+
+        self.browse_frame = BrowseFrame(master=self, file_type=".*")
+        self.browse_frame.grid(row=0, column=1)
+
+    def save(self) -> None:
+        file = self.browse_frame.file_path.get()
+        with open(file, "w") as f:
+            _input: str = json.dumps(get_meta(self), indent=4)
+            f.write(_input)
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/data_init/data_init_frame.py` & `pymonke-0.1.2/src/pymonke/gui/data_init/data_init_frame.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-from customtkinter import CTkFrame
-import pandas as pd
-
-import json
-from typing import Any, Optional
-
-from .browse_save_frame import BrowseSaveFrame
-from ..browse_frame import BrowseFrame
-from ..entry_label_frame import EntryLabelFrame
-from ..fitting.fit_frame import FitFrame
-from ..misc import get_root
-from ..misc import get_data, get_meta, get_root
-from .status_frame import StatusFrame
-
-from pymonke.misc.file_management import read_data_into_dataframe
-from pymonke.misc.dataframe import get_error_column_name
-
-
-class DataInitFrame(CTkFrame):
-    def __init__(self, **kwargs: Any) -> None:
-        CTkFrame.__init__(self, **kwargs)
-
-        self.browse_data_frame = BrowseFrame(file_type="*.csv; *.txt", master=self, placeholder="Enter the data file")
-        self.browse_data_frame.grid(row=0, column=0, columnspan=2)
-
-        self.load_meta_frame = BrowseFrame(file_type=".json", master=self, browse_text="load",
-                                           placeholder="Enter the meta data for plotting")
-        self.load_meta_frame.grid(row=1, column=0, columnspan=2)
-
-        self.x_data_frame = EntryLabelFrame(master=self, label="X")
-        self.x_data_frame.entry.bind("<Return>", self.save_x_name)
-        self.x_data_frame.grid(row=2, column=0)
-        self.y_data_frame = EntryLabelFrame(master=self, label="Y")
-        self.y_data_frame.entry.bind("<Return>", self.save_y_name)
-        self.y_data_frame.grid(row=2, column=1)
-
-        self.status = StatusFrame(master=self, height=400)
-        self.status.grid(row=4, column=0, columnspan=2, sticky="ns")
-
-        self.save_meta_frame = BrowseSaveFrame(master=self)
-        self.save_meta_frame.save_button.configure(command=self.save_meta_to_file)
-        self.save_meta_frame.grid(row=3, column=0, columnspan=2)
-
-    def load_data(self, browse: bool = True) -> Optional[pd.DataFrame]:
-        try:
-            if browse:
-                self.browse_data_frame.browse()
-            file_path = self.browse_data_frame.file_path.get()
-            if (kwargs := get_meta(self).get("read_data_args")) is None:
-                kwargs = dict()
-            data = read_data_into_dataframe(file_path, **kwargs)
-            get_meta(self)["file"] = file_path
-            self.status.add_info(text="data loaded successfully")
-            return data
-        except Exception as e:
-            self.status.add_error(str(e))
-            return None
-
-    def load_meta(self) -> Optional[dict[str, Any]]:
-        try:
-            fit_frame: FitFrame = get_root(self).get_fit_frame()
-            fit_frame.delete_all_fits()
-            self.load_meta_frame.browse()
-            file_path = self.load_meta_frame.file_path.get()
-            data: dict[str, Any] = json.loads(open(file_path).read())
-            self.status.add_info("Meta Data loaded successfully")
-            return data
-        except Exception as e:
-            self.status.add_error(str(e))
-            return None
-
-    def check_xy_input(self, xy: str) -> None:
-        if "x" in xy:
-            if (text := self.x_data_frame.text.get()) is not None and self.entry_in_dataframe(text):
-                self.status.add_info("X column found")
-            else:
-                self.status.add_error("X column not found")
-        if "y" in xy:
-            if (text := self.y_data_frame.text.get()) is not None and self.entry_in_dataframe(text):
-                self.status.add_info("Y column found")
-                data = get_data(self)
-                assert isinstance(data, pd.DataFrame)
-                if get_error_column_name(data, text) is None:
-                    self.status.add_error("Y Error not found")
-
-            else:
-                self.status.add_error("Y column not found")
-
-    def entry_in_dataframe(self, name: str) -> bool:
-        if (data := get_data(self)) is not None:
-            return name in data
-        else:
-            return False
-
-    def save_x_name(self, _: Any = None) -> None:
-        x_name = self.x_data_frame.text.get()
-        get_meta(self)["x"] = x_name
-        self.check_xy_input("x")
-        get_root(self).get_plot_frame().plot_data()
-
-    def save_y_name(self, _: Any = None) -> None:
-        y_name = self.y_data_frame.text.get()
-        get_meta(self)["y"] = y_name
-        self.check_xy_input("y")
-        get_root(self).get_plot_frame().plot_data()
-
-    def load_from_meta(self) -> None:
-        """Function that initializes values in this frame if metadata is loaded."""
-        meta = get_meta(self)
-        if (file := meta.get("file")) is not None:
-            self.browse_data_frame.file_path.set(file)
-            get_root(self).data = self.load_data(False)
-
-        if (x := meta.get("x")) is not None:
-            self.x_data_frame.text.set(x)
-        if (y := meta.get("y")) is not None:
-            self.y_data_frame.text.set(y)
-        self.check_xy_input("xy")
-
-    def save_meta_to_file(self) -> None:
-        try:
-            self.save_meta_frame.save()
-            self.status.add_info("Meta data saved to file successfully")
-        except Exception as e:
-            self.status.add_error(str(e))
+from customtkinter import CTkFrame
+import pandas as pd
+
+import json
+from typing import Any, Optional
+
+from .browse_save_frame import BrowseSaveFrame
+from ..browse_frame import BrowseFrame
+from ..entry_label_frame import EntryLabelFrame
+from ..fitting.fit_frame import FitFrame
+from ..misc import get_root
+from ..misc import get_data, get_meta, get_root
+from .status_frame import StatusFrame
+
+from pymonke.misc.file_management import read_data_into_dataframe
+from pymonke.misc.dataframe import get_error_column_name
+
+
+class DataInitFrame(CTkFrame):
+    def __init__(self, **kwargs: Any) -> None:
+        CTkFrame.__init__(self, **kwargs)
+
+        self.browse_data_frame = BrowseFrame(file_type="*.csv; *.txt", master=self, placeholder="Enter the data file")
+        self.browse_data_frame.grid(row=0, column=0, columnspan=2)
+
+        self.load_meta_frame = BrowseFrame(file_type=".json", master=self, browse_text="load",
+                                           placeholder="Enter the meta data for plotting")
+        self.load_meta_frame.grid(row=1, column=0, columnspan=2)
+
+        self.x_data_frame = EntryLabelFrame(master=self, label="X")
+        self.x_data_frame.entry.bind("<Return>", self.save_x_name)
+        self.x_data_frame.grid(row=2, column=0)
+        self.y_data_frame = EntryLabelFrame(master=self, label="Y")
+        self.y_data_frame.entry.bind("<Return>", self.save_y_name)
+        self.y_data_frame.grid(row=2, column=1)
+
+        self.status = StatusFrame(master=self, height=400)
+        self.status.grid(row=4, column=0, columnspan=2, sticky="ns")
+
+        self.save_meta_frame = BrowseSaveFrame(master=self)
+        self.save_meta_frame.save_button.configure(command=self.save_meta_to_file)
+        self.save_meta_frame.grid(row=3, column=0, columnspan=2)
+
+    def load_data(self, browse: bool = True) -> Optional[pd.DataFrame]:
+        try:
+            if browse:
+                self.browse_data_frame.browse()
+            file_path = self.browse_data_frame.file_path.get()
+            if (kwargs := get_meta(self).get("read_data_args")) is None:
+                kwargs = dict()
+            data = read_data_into_dataframe(file_path, **kwargs)
+            get_meta(self)["file"] = file_path
+            self.status.add_info(text="data loaded successfully")
+            return data
+        except Exception as e:
+            self.status.add_error(str(e))
+            return None
+
+    def load_meta(self) -> Optional[dict[str, Any]]:
+        try:
+            fit_frame: FitFrame = get_root(self).get_fit_frame()
+            fit_frame.delete_all_fits()
+            self.load_meta_frame.browse()
+            file_path = self.load_meta_frame.file_path.get()
+            data: dict[str, Any] = json.loads(open(file_path).read())
+            self.status.add_info("Meta Data loaded successfully")
+            return data
+        except Exception as e:
+            self.status.add_error(str(e))
+            return None
+
+    def check_xy_input(self, xy: str) -> None:
+        if "x" in xy:
+            if (text := self.x_data_frame.text.get()) is not None and self.entry_in_dataframe(text):
+                self.status.add_info("X column found")
+            else:
+                self.status.add_error("X column not found")
+        if "y" in xy:
+            if (text := self.y_data_frame.text.get()) is not None and self.entry_in_dataframe(text):
+                self.status.add_info("Y column found")
+                data = get_data(self)
+                assert isinstance(data, pd.DataFrame)
+                if get_error_column_name(data, text) is None:
+                    self.status.add_error("Y Error not found")
+
+            else:
+                self.status.add_error("Y column not found")
+
+    def entry_in_dataframe(self, name: str) -> bool:
+        if (data := get_data(self)) is not None:
+            return name in data
+        else:
+            return False
+
+    def save_x_name(self, _: Any = None) -> None:
+        x_name = self.x_data_frame.text.get()
+        get_meta(self)["x"] = x_name
+        self.check_xy_input("x")
+        get_root(self).get_plot_frame().plot_data()
+
+    def save_y_name(self, _: Any = None) -> None:
+        y_name = self.y_data_frame.text.get()
+        get_meta(self)["y"] = y_name
+        self.check_xy_input("y")
+        get_root(self).get_plot_frame().plot_data()
+
+    def load_from_meta(self) -> None:
+        """Function that initializes values in this frame if metadata is loaded."""
+        meta = get_meta(self)
+        if (file := meta.get("file")) is not None:
+            self.browse_data_frame.file_path.set(file)
+            get_root(self).data = self.load_data(False)
+
+        if (x := meta.get("x")) is not None:
+            self.x_data_frame.text.set(x)
+        if (y := meta.get("y")) is not None:
+            self.y_data_frame.text.set(y)
+        self.check_xy_input("xy")
+
+    def save_meta_to_file(self) -> None:
+        try:
+            self.save_meta_frame.save()
+            self.status.add_info("Meta data saved to file successfully")
+        except Exception as e:
+            self.status.add_error(str(e))
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/data_init/status_frame.py` & `pymonke-0.1.2/src/pymonke/gui/data_init/status_frame.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from customtkinter import CTkFrame, CTkButton, CTkLabel
-from collections import deque
-
-from typing import Any
-
-
-class StatusFrame(CTkFrame):
-    def __init__(self, max_length: int = 10, **kwargs: Any) -> None:
-        CTkFrame.__init__(self, **kwargs)
-        self.max_length = max_length
-        self.labels: deque[CTkLabel] = deque()
-        self.button = CTkButton(self, text="Clear", command=self.clear)
-        self.grid_rowconfigure(tuple(range(max_length + 1)), minsize=25)
-        self.button.grid(row=max_length, column=0)
-
-    def add_info(self, text: str) -> None:
-        self.add_text(text, "green")
-
-    def add_error(self, text: str) -> None:
-        self.add_text(text, "red")
-
-    def add_text(self, text: str, color: str) -> None:
-        if len(self.labels) == self.max_length:
-            self.delete_first()
-        label = CTkLabel(master=self, text=text, text_color=color, height=25)
-        label.grid(row=len(self.labels), column=0, sticky="ew")
-        self.labels.append(label)
-        self.button.grid(row=self.max_length, column=0)
-
-    def delete_first(self) -> None:
-        self.labels[0].destroy()
-        self.labels.popleft()
-        for i, label in enumerate(self.labels):
-            label.grid(row=i, column=0, sticky="ew")
-
-    def clear(self) -> None:
-        while len(self.labels) > 0:
-            self.delete_first()
+from customtkinter import CTkFrame, CTkButton, CTkLabel
+from collections import deque
+
+from typing import Any
+
+
+class StatusFrame(CTkFrame):
+    def __init__(self, max_length: int = 10, **kwargs: Any) -> None:
+        CTkFrame.__init__(self, **kwargs)
+        self.max_length = max_length
+        self.labels: deque[CTkLabel] = deque()
+        self.button = CTkButton(self, text="Clear", command=self.clear)
+        self.grid_rowconfigure(tuple(range(max_length + 1)), minsize=25)
+        self.button.grid(row=max_length, column=0)
+
+    def add_info(self, text: str) -> None:
+        self.add_text(text, "green")
+
+    def add_error(self, text: str) -> None:
+        self.add_text(text, "red")
+
+    def add_text(self, text: str, color: str) -> None:
+        if len(self.labels) == self.max_length:
+            self.delete_first()
+        label = CTkLabel(master=self, text=text, text_color=color, height=25)
+        label.grid(row=len(self.labels), column=0, sticky="ew")
+        self.labels.append(label)
+        self.button.grid(row=self.max_length, column=0)
+
+    def delete_first(self) -> None:
+        self.labels[0].destroy()
+        self.labels.popleft()
+        for i, label in enumerate(self.labels):
+            label.grid(row=i, column=0, sticky="ew")
+
+    def clear(self) -> None:
+        while len(self.labels) > 0:
+            self.delete_first()
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/fitting/add_args_frame.py` & `pymonke-0.1.2/src/pymonke/gui/fitting/add_args_frame.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from customtkinter import CTkFrame, CTkCheckBox
-
-from typing import Any, Optional
-
-from ..labeled_entry import LabeledEntry
-
-
-class AddArgsFrame(CTkFrame):
-    def __init__(self, meta: Optional[dict[str, Any]] = None, **kwargs: Any) -> None:
-        CTkFrame.__init__(self, **kwargs)
-        self.grid_columnconfigure(0, weight=1)
-        self.fitting_points_entry = LabeledEntry(master=self, label="Fitting Points")
-        self.fitting_points_entry.entry.bind("<Return>", self.fitting_points_entry_callback)
-        self.fitting_points_entry.grid(row=0, column=0, pady=10, sticky="we")
-
-        self.absolute_sigma_checkbox = CTkCheckBox(master=self, text="Absolute Sigma", command=self.update_values)
-        self.absolute_sigma_checkbox.grid(row=1, column=0, sticky="w")
-
-        self.check_finite_checkbox = CTkCheckBox(master=self, text="Check Finite", command=self.update_values)
-        self.check_finite_checkbox.grid(row=2, column=0, sticky="w")
-
-        self.label_entry = LabeledEntry(master=self, label="Label")
-        self.label_entry.entry.grid_configure(sticky="we")
-        self.label_entry.entry.bind("<Return>", self.update_values)
-        self.label_entry.grid(row=3, column=0, sticky="we")
-
-        self.meta: Optional[dict[str, Any]] = meta
-
-    def get_values(self) -> dict[str, Any]:
-        res = {
-            "fit_points": self.get_fitting_points_entry(),
-            "absolute_sigma": bool(self.absolute_sigma_checkbox.get()),
-            "check_finite": bool(self.check_finite_checkbox.get()),
-            "label": self.label_entry.text_var.get()
-        }
-
-        return res
-
-    def update_values(self, _event: Any = None) -> None:
-        res = self.get_values()
-        if self.meta is not None:
-            self.meta.update(res)
-
-    def load_from_meta(self) -> None:
-        if self.meta is not None:
-            self.load(self.meta)
-
-    def load(self, data: dict[str, Any]) -> None:
-        self.set_fitting_points_entry(data.get("fit_points", None))
-        self.update_fitting_points_entry()
-        if data.get("absolute_sigma") or False:
-            self.absolute_sigma_checkbox.select()
-        else:
-            self.absolute_sigma_checkbox.deselect()
-        if data.get("check_finite") or False:
-            self.check_finite_checkbox.select()
-        else:
-            self.check_finite_checkbox.deselect()
-        self.label_entry.text_var.set(data.get("label") or "")
-
-    def fitting_points_entry_callback(self, _: Any = None) -> None:
-        self.update_fitting_points_entry()
-        self.update_values()
-
-    def get_fitting_points_entry(self) -> Optional[int]:
-        text = self.fitting_points_entry.text_var.get()
-        if text == "":
-            return None
-        else:
-            return int(text)
-
-    def set_fitting_points_entry(self, value: Optional[int]) -> None:
-        if value is None:
-            self.fitting_points_entry.text_var.set("")
-        else:
-            self.fitting_points_entry.text_var.set(str(value))
-        self.update_fitting_points_entry()
-
-    def update_fitting_points_entry(self) -> None:
-        text = self.fitting_points_entry.text_var.get()
-        if text == "":
-            self.fitting_points_entry.text = ""
-        try:
-            _ = int(text)
-            self.fitting_points_entry.text = text
-        except ValueError as _:
-            self.fitting_points_entry.text_var.set(self.fitting_points_entry.text)
+from customtkinter import CTkFrame, CTkCheckBox
+
+from typing import Any, Optional
+
+from ..labeled_entry import LabeledEntry
+
+
+class AddArgsFrame(CTkFrame):
+    def __init__(self, meta: Optional[dict[str, Any]] = None, **kwargs: Any) -> None:
+        CTkFrame.__init__(self, **kwargs)
+        self.grid_columnconfigure(0, weight=1)
+        self.fitting_points_entry = LabeledEntry(master=self, label="Fitting Points")
+        self.fitting_points_entry.entry.bind("<Return>", self.fitting_points_entry_callback)
+        self.fitting_points_entry.grid(row=0, column=0, pady=10, sticky="we")
+
+        self.absolute_sigma_checkbox = CTkCheckBox(master=self, text="Absolute Sigma", command=self.update_values)
+        self.absolute_sigma_checkbox.grid(row=1, column=0, sticky="w")
+
+        self.check_finite_checkbox = CTkCheckBox(master=self, text="Check Finite", command=self.update_values)
+        self.check_finite_checkbox.grid(row=2, column=0, sticky="w")
+
+        self.label_entry = LabeledEntry(master=self, label="Label")
+        self.label_entry.entry.grid_configure(sticky="we")
+        self.label_entry.entry.bind("<Return>", self.update_values)
+        self.label_entry.grid(row=3, column=0, sticky="we")
+
+        self.meta: Optional[dict[str, Any]] = meta
+
+    def get_values(self) -> dict[str, Any]:
+        res = {
+            "fit_points": self.get_fitting_points_entry(),
+            "absolute_sigma": bool(self.absolute_sigma_checkbox.get()),
+            "check_finite": bool(self.check_finite_checkbox.get()),
+            "label": self.label_entry.text_var.get()
+        }
+
+        return res
+
+    def update_values(self, _event: Any = None) -> None:
+        res = self.get_values()
+        if self.meta is not None:
+            self.meta.update(res)
+
+    def load_from_meta(self) -> None:
+        if self.meta is not None:
+            self.load(self.meta)
+
+    def load(self, data: dict[str, Any]) -> None:
+        self.set_fitting_points_entry(data.get("fit_points", None))
+        self.update_fitting_points_entry()
+        if data.get("absolute_sigma") or False:
+            self.absolute_sigma_checkbox.select()
+        else:
+            self.absolute_sigma_checkbox.deselect()
+        if data.get("check_finite") or False:
+            self.check_finite_checkbox.select()
+        else:
+            self.check_finite_checkbox.deselect()
+        self.label_entry.text_var.set(data.get("label") or "")
+
+    def fitting_points_entry_callback(self, _: Any = None) -> None:
+        self.update_fitting_points_entry()
+        self.update_values()
+
+    def get_fitting_points_entry(self) -> Optional[int]:
+        text = self.fitting_points_entry.text_var.get()
+        if text == "":
+            return None
+        else:
+            return int(text)
+
+    def set_fitting_points_entry(self, value: Optional[int]) -> None:
+        if value is None:
+            self.fitting_points_entry.text_var.set("")
+        else:
+            self.fitting_points_entry.text_var.set(str(value))
+        self.update_fitting_points_entry()
+
+    def update_fitting_points_entry(self) -> None:
+        text = self.fitting_points_entry.text_var.get()
+        if text == "":
+            self.fitting_points_entry.text = ""
+        try:
+            _ = int(text)
+            self.fitting_points_entry.text = text
+        except ValueError as _:
+            self.fitting_points_entry.text_var.set(self.fitting_points_entry.text)
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/fitting/fit_frame.py` & `pymonke-0.1.2/src/pymonke/gui/fitting/fit_frame.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-from customtkinter import CTkFrame, CTkOptionMenu
-
-from typing import Any, Optional
-
-from .add_args_frame import AddArgsFrame
-from ..formula.formula_frame import FormulaFrame
-from .fit_option_menu import FitComboBox
-from ..list_frame import ListFrame
-from ..misc import get_meta, get_root
-from ..plot.limits_frame import LimitsFrame
-from ..dict_frame import DictFrame
-
-
-class FitFrame(CTkFrame):
-    def __init__(self, **kwargs: Any) -> None:
-        CTkFrame.__init__(self, **kwargs)
-        self.formula_frame = FormulaFrame(master=self, width=6000)
-        self.formula_frame.grid(row=0, column=0, sticky="nsew", columnspan=2)
-        self.formula_frame.entry_bindings = [self.update_to_meta,
-                                             self.update_start_parameter_entries_from_formula_frame]
-        self.grid_columnconfigure(0, weight=3)
-        self.grid_rowconfigure(0, weight=5)
-        self.grid_rowconfigure((1, 2, 3, 4), weight=1)
-        self.grid_columnconfigure(1, weight=2)
-
-        self.fit_meta: Optional[dict[str, Any]] = None
-
-        self.fit_combo_box = FitComboBox(master=self)
-        self.fit_combo_box.selection_bindings = [self.set_fit_meta, self.load_from_fit_meta,
-                                                 self.update_start_parameter_entries_from_formula_frame]
-        self.fit_combo_box.return_bindings = [self.set_fit_meta, self.load_from_fit_meta,
-                                              self.update_start_parameter_entries_from_formula_frame]
-        self.fit_combo_box.grid(row=1, column=0, sticky="w")
-
-        self.fit_type_option = CTkOptionMenu(master=self, values=["OLS", "ODR"], command=self.update_to_meta)
-        self.fit_type_option.set("OLS")
-        self.fit_type_option.grid(row=1, column=1, sticky="e")
-
-        self.start_parameter_frame = ListFrame(text="Start Parameters", has_add_button=False, master=self)
-        self.start_parameter_frame.entry_bindings = [self.update_start_parameters]
-        self.start_parameter_frame.grid(row=2, column=0, columnspan=1, pady=0)
-
-        self.limits_frame = LimitsFrame(master=self, label="Fitting Limits")
-        self.limits_frame.entry_bindings = [self.update_to_meta]
-        self.limits_frame.grid(row=3, column=0, columnspan=1)
-
-        self.plot_limits_frame = LimitsFrame(master=self, label="Plotting Limits")
-        self.plot_limits_frame.entry_bindings = [self.update_to_meta]
-        self.plot_limits_frame.grid(row=4, column=0, columnspan=1)
-
-        self.plotting_style_arguments = DictFrame(master=self, text="Plotting Style Arguments")
-        self.plotting_style_arguments.grid(row=5, column=0, pady=20, columnspan=1)
-
-        self.add_args_frame = AddArgsFrame(master=self, width=200)
-        self.add_args_frame.grid(row=2, column=1, sticky="nsew", padx=5, rowspan=3, pady=20)
-
-    def update_start_parameter_entries_from_formula_frame(self) -> None:
-        params: list[str] = self.formula_frame.params
-
-        # search for already set parameters in meta
-        if (fit_meta := self.get_fit_meta()) is not None:
-            if (start_parameters := fit_meta.get("start_parameters")) is not None:
-                if len(start_parameters) == len(params):
-                    self.start_parameter_frame.set_parameters(start_parameters)
-                    return
-        self.start_parameter_frame.set_parameters([0] * len(params))
-
-    def set_param_values(self, values: dict[str, Any]) -> None:
-        self.formula_frame.parameters.set_param_values(values)
-
-    def set_params_values_from_results(self) -> None:
-        fit_name = self.get_fit_name()
-        if fit_name is not None:
-            fit_result = get_root(self).fit_result
-            if fit_result is not None:
-                result = fit_result.get(fit_name)
-                if result is not None:
-                    get_root(self).get_fit_frame().set_param_values(result.as_dict(False))
-
-    def get_fit_type(self) -> str:
-        if self.fit_type_option.get() == "OLS":
-            return "optimize.curve_fit"
-        elif self.fit_type_option.get() == "ODR":
-            return "odr"
-        else:
-            raise Exception("unknown fitting type")
-
-    def set_fit_type(self, _type: str) -> None:
-        if _type == "optimize.curve_fit":
-            self.fit_type_option.set("OLS")
-        elif _type == "odr":
-            self.fit_type_option.set("ODR")
-
-    def delete_all_fits(self) -> None:
-        for opt in self.fit_combo_box.cget("values"):
-            if opt != "Add Fit":
-                self.fit_combo_box.delete_option(opt)
-
-    def update_to_meta(self, _: Any = None) -> None:
-        """update meta from all child objects"""
-        if self.fit_meta is None:
-            return
-        update = {
-            "fit_type": self.get_fit_type(),
-            "function": self.formula_frame.text,
-            "x_min_limit": self.limits_frame.min,
-            "x_max_limit": self.limits_frame.max,
-            "plot_x_min_limit": self.plot_limits_frame.min,
-            "plot_x_max_limit": self.plot_limits_frame.max,
-            "start_parameters": self.get_start_parameters()
-        }
-
-        self.fit_meta.update(update)
-
-    # -----------------------------------------------------------------------------
-    # -------------------------Fit Combo Box---------------------------------------
-    # -----------------------------------------------------------------------------
-
-    def get_fit_name(self) -> Optional[str]:
-        if (val := self.fit_combo_box.selected) == "Add Fit":
-            return None
-        else:
-            return val
-
-    def get_fit_meta(self) -> Optional[dict[str, Any]]:
-        if (val := self.fit_combo_box.selected) == "Add Fit":
-            return None
-        else:
-            ret = get_meta(self)["fits"][val]
-            assert isinstance(ret, dict)
-            return ret
-
-    def set_fit_meta(self) -> None:
-        """Set self.fit_meta to the meta dictionary that corresponds to the fit set in the combo box."""
-        self.fit_meta = self.get_fit_meta()
-        if self.fit_meta is None:
-            self.plotting_style_arguments.meta = None
-            self.add_args_frame.meta = None
-            return
-        if (meta := self.fit_meta.get("plotting_style")) is None:
-            self.fit_meta["plotting_style"] = dict()
-            meta = self.fit_meta["plotting_style"]
-        self.plotting_style_arguments.meta = meta
-        self.add_args_frame.meta = self.fit_meta
-
-    def get_start_parameters(self) -> list[float]:
-        p0: list[float] = []
-        for param in self.start_parameter_frame.get_list():
-            if param == "":
-                p0.append(0)
-            else:
-                p0.append(float(param))
-
-        return p0
-
-    def update_start_parameters(self, _: Any = None) -> None:
-        p0 = self.get_start_parameters()
-
-        if self.fit_meta is not None:
-            self.fit_meta.update({"start_parameters": p0})
-
-    # -----PLOTTING-STYLE-----------------------------------------------------------
-    def get_plotting_style_arguments(self) -> dict[str, float | str]:
-        return self.plotting_style_arguments.get_args()
-
-    def load_plotting_style_arguments_from_fit_meta(self) -> None:
-        if (fit_name := self.get_fit_name()) is None:
-            return
-        fit_meta = get_meta(self)["fits"][fit_name]
-        if (plotting_style := fit_meta.get("plotting_style")) is not None:
-            self.plotting_style_arguments.load_parameters(plotting_style)
-
-    def update_plotting_style(self) -> None:
-        if (val := self.get_fit_name()) is None:
-            return
-        args = self.get_plotting_style_arguments()
-        if get_meta(self)["fits"][val].get("plotting_style") is None:
-            get_meta(self)["fits"][val]["plotting_style"] = args
-        else:
-            get_meta(self)["fits"][val]["plotting_style"].update(args)
-
-    def load_limits_from_fit_meta(self) -> None:
-        if (val := self.get_fit_name()) is None:
-            return
-        d = get_meta(self)["fits"][val]
-        self.limits_frame.min = d.get("x_min_limit")
-        self.limits_frame.max = d.get("x_max_limit")
-        self.plot_limits_frame.min = d.get("plot_x_min_limit")
-        self.plot_limits_frame.max = d.get("plot_x_max_limit")
-        self.set_params_values_from_results()
-
-    def load_from_fit_meta(self, _: Any = None) -> None:
-        """if Values exist in meta[fit_name]. load them in."""
-        if (fit := self.get_fit_meta()) is None:
-            self.formula_frame.text = ""
-            self.plotting_style_arguments.load_parameters({})
-            self.limits_frame.set_limits(None, None)
-            self.plot_limits_frame.set_limits(None, None)
-            self.add_args_frame.load({
-                "fit_points": None,
-                "absolute_sigma": False,
-                "check_finite": False,
-            })
-            self.fit_type_option.set("OLS")
-            return
-        if (func := fit.get("function")) is None:
-            func = ""
-        self.formula_frame.text = func
-        if (fit_type := fit.get("fit_type")) is not None:
-            self.set_fit_type(fit_type)
-        else:
-            self.set_fit_type("OLS")
-        self.load_limits_from_fit_meta()
-        self.load_plotting_style_arguments_from_fit_meta()
-        self.update_start_parameter_entries_from_formula_frame()
-        self.add_args_frame.load_from_meta()
-
-    def update_from_to_meta(self, _: Any = None) -> None:
-        self.load_from_fit_meta()
-        self.update_to_meta()
-
-    def load_from_meta(self, _: Any = None) -> None:
-        meta = get_meta(self)
-        if (fits := meta.get("fits")) is not None:
-            if len(fits) >= 1:
-                self.fit_combo_box.configure(values=[*(keys := list(fits.keys())), "Add Fit"])
-                self.fit_combo_box.set(keys[0])
-                self.fit_combo_box.selected = keys[0]
-                self.set_fit_meta()
-                self.load_from_fit_meta()
+from customtkinter import CTkFrame, CTkOptionMenu
+
+from typing import Any, Optional
+
+from .add_args_frame import AddArgsFrame
+from ..formula.formula_frame import FormulaFrame
+from .fit_option_menu import FitComboBox
+from ..list_frame import ListFrame
+from ..misc import get_meta, get_root
+from ..plot.limits_frame import LimitsFrame
+from ..dict_frame import DictFrame
+
+
+class FitFrame(CTkFrame):
+    def __init__(self, **kwargs: Any) -> None:
+        CTkFrame.__init__(self, **kwargs)
+        self.formula_frame = FormulaFrame(master=self, width=6000)
+        self.formula_frame.grid(row=0, column=0, sticky="nsew", columnspan=2)
+        self.formula_frame.entry_bindings = [self.update_to_meta,
+                                             self.update_start_parameter_entries_from_formula_frame]
+        self.grid_columnconfigure(0, weight=3)
+        self.grid_rowconfigure(0, weight=5)
+        self.grid_rowconfigure((1, 2, 3, 4), weight=1)
+        self.grid_columnconfigure(1, weight=2)
+
+        self.fit_meta: Optional[dict[str, Any]] = None
+
+        self.fit_combo_box = FitComboBox(master=self)
+        self.fit_combo_box.selection_bindings = [self.set_fit_meta, self.load_from_fit_meta,
+                                                 self.update_start_parameter_entries_from_formula_frame]
+        self.fit_combo_box.return_bindings = [self.set_fit_meta, self.load_from_fit_meta,
+                                              self.update_start_parameter_entries_from_formula_frame]
+        self.fit_combo_box.grid(row=1, column=0, sticky="w")
+
+        self.fit_type_option = CTkOptionMenu(master=self, values=["OLS", "ODR"], command=self.update_to_meta)
+        self.fit_type_option.set("OLS")
+        self.fit_type_option.grid(row=1, column=1, sticky="e")
+
+        self.start_parameter_frame = ListFrame(text="Start Parameters", has_add_button=False, master=self)
+        self.start_parameter_frame.entry_bindings = [self.update_start_parameters]
+        self.start_parameter_frame.grid(row=2, column=0, columnspan=1, pady=0)
+
+        self.limits_frame = LimitsFrame(master=self, label="Fitting Limits")
+        self.limits_frame.entry_bindings = [self.update_to_meta]
+        self.limits_frame.grid(row=3, column=0, columnspan=1)
+
+        self.plot_limits_frame = LimitsFrame(master=self, label="Plotting Limits")
+        self.plot_limits_frame.entry_bindings = [self.update_to_meta]
+        self.plot_limits_frame.grid(row=4, column=0, columnspan=1)
+
+        self.plotting_style_arguments = DictFrame(master=self, text="Plotting Style Arguments")
+        self.plotting_style_arguments.grid(row=5, column=0, pady=20, columnspan=1)
+
+        self.add_args_frame = AddArgsFrame(master=self, width=200)
+        self.add_args_frame.grid(row=2, column=1, sticky="nsew", padx=5, rowspan=3, pady=20)
+
+    def update_start_parameter_entries_from_formula_frame(self) -> None:
+        params: list[str] = self.formula_frame.params
+
+        # search for already set parameters in meta
+        if (fit_meta := self.get_fit_meta()) is not None:
+            if (start_parameters := fit_meta.get("start_parameters")) is not None:
+                if len(start_parameters) == len(params):
+                    self.start_parameter_frame.set_parameters(start_parameters)
+                    return
+        self.start_parameter_frame.set_parameters([0] * len(params))
+
+    def set_param_values(self, values: dict[str, Any]) -> None:
+        self.formula_frame.parameters.set_param_values(values)
+
+    def set_params_values_from_results(self) -> None:
+        fit_name = self.get_fit_name()
+        if fit_name is not None:
+            fit_result = get_root(self).fit_result
+            if fit_result is not None:
+                result = fit_result.get(fit_name)
+                if result is not None:
+                    get_root(self).get_fit_frame().set_param_values(result.as_dict(False))
+
+    def get_fit_type(self) -> str:
+        if self.fit_type_option.get() == "OLS":
+            return "optimize.curve_fit"
+        elif self.fit_type_option.get() == "ODR":
+            return "odr"
+        else:
+            raise Exception("unknown fitting type")
+
+    def set_fit_type(self, _type: str) -> None:
+        if _type == "optimize.curve_fit":
+            self.fit_type_option.set("OLS")
+        elif _type == "odr":
+            self.fit_type_option.set("ODR")
+
+    def delete_all_fits(self) -> None:
+        for opt in self.fit_combo_box.cget("values"):
+            if opt != "Add Fit":
+                self.fit_combo_box.delete_option(opt)
+
+    def update_to_meta(self, _: Any = None) -> None:
+        """update meta from all child objects"""
+        if self.fit_meta is None:
+            return
+        update = {
+            "fit_type": self.get_fit_type(),
+            "function": self.formula_frame.text,
+            "x_min_limit": self.limits_frame.min,
+            "x_max_limit": self.limits_frame.max,
+            "plot_x_min_limit": self.plot_limits_frame.min,
+            "plot_x_max_limit": self.plot_limits_frame.max,
+            "start_parameters": self.get_start_parameters()
+        }
+
+        self.fit_meta.update(update)
+
+    # -----------------------------------------------------------------------------
+    # -------------------------Fit Combo Box---------------------------------------
+    # -----------------------------------------------------------------------------
+
+    def get_fit_name(self) -> Optional[str]:
+        if (val := self.fit_combo_box.selected) == "Add Fit":
+            return None
+        else:
+            return val
+
+    def get_fit_meta(self) -> Optional[dict[str, Any]]:
+        if (val := self.fit_combo_box.selected) == "Add Fit":
+            return None
+        else:
+            ret = get_meta(self)["fits"][val]
+            assert isinstance(ret, dict)
+            return ret
+
+    def set_fit_meta(self) -> None:
+        """Set self.fit_meta to the meta dictionary that corresponds to the fit set in the combo box."""
+        self.fit_meta = self.get_fit_meta()
+        if self.fit_meta is None:
+            self.plotting_style_arguments.meta = None
+            self.add_args_frame.meta = None
+            return
+        if (meta := self.fit_meta.get("plotting_style")) is None:
+            self.fit_meta["plotting_style"] = dict()
+            meta = self.fit_meta["plotting_style"]
+        self.plotting_style_arguments.meta = meta
+        self.add_args_frame.meta = self.fit_meta
+
+    def get_start_parameters(self) -> list[float]:
+        p0: list[float] = []
+        for param in self.start_parameter_frame.get_list():
+            if param == "":
+                p0.append(0)
+            else:
+                p0.append(float(param))
+
+        return p0
+
+    def update_start_parameters(self, _: Any = None) -> None:
+        p0 = self.get_start_parameters()
+
+        if self.fit_meta is not None:
+            self.fit_meta.update({"start_parameters": p0})
+
+    # -----PLOTTING-STYLE-----------------------------------------------------------
+    def get_plotting_style_arguments(self) -> dict[str, float | str]:
+        return self.plotting_style_arguments.get_args()
+
+    def load_plotting_style_arguments_from_fit_meta(self) -> None:
+        if (fit_name := self.get_fit_name()) is None:
+            return
+        fit_meta = get_meta(self)["fits"][fit_name]
+        if (plotting_style := fit_meta.get("plotting_style")) is not None:
+            self.plotting_style_arguments.load_parameters(plotting_style)
+
+    def update_plotting_style(self) -> None:
+        if (val := self.get_fit_name()) is None:
+            return
+        args = self.get_plotting_style_arguments()
+        if get_meta(self)["fits"][val].get("plotting_style") is None:
+            get_meta(self)["fits"][val]["plotting_style"] = args
+        else:
+            get_meta(self)["fits"][val]["plotting_style"].update(args)
+
+    def load_limits_from_fit_meta(self) -> None:
+        if (val := self.get_fit_name()) is None:
+            return
+        d = get_meta(self)["fits"][val]
+        self.limits_frame.min = d.get("x_min_limit")
+        self.limits_frame.max = d.get("x_max_limit")
+        self.plot_limits_frame.min = d.get("plot_x_min_limit")
+        self.plot_limits_frame.max = d.get("plot_x_max_limit")
+        self.set_params_values_from_results()
+
+    def load_from_fit_meta(self, _: Any = None) -> None:
+        """if Values exist in meta[fit_name]. load them in."""
+        if (fit := self.get_fit_meta()) is None:
+            self.formula_frame.text = ""
+            self.plotting_style_arguments.load_parameters({})
+            self.limits_frame.set_limits(None, None)
+            self.plot_limits_frame.set_limits(None, None)
+            self.add_args_frame.load({
+                "fit_points": None,
+                "absolute_sigma": False,
+                "check_finite": False,
+            })
+            self.fit_type_option.set("OLS")
+            return
+        if (func := fit.get("function")) is None:
+            func = ""
+        self.formula_frame.text = func
+        if (fit_type := fit.get("fit_type")) is not None:
+            self.set_fit_type(fit_type)
+        else:
+            self.set_fit_type("OLS")
+        self.load_limits_from_fit_meta()
+        self.load_plotting_style_arguments_from_fit_meta()
+        self.update_start_parameter_entries_from_formula_frame()
+        self.add_args_frame.load_from_meta()
+
+    def update_from_to_meta(self, _: Any = None) -> None:
+        self.load_from_fit_meta()
+        self.update_to_meta()
+
+    def load_from_meta(self, _: Any = None) -> None:
+        meta = get_meta(self)
+        if (fits := meta.get("fits")) is not None:
+            if len(fits) >= 1:
+                self.fit_combo_box.configure(values=[*(keys := list(fits.keys())), "Add Fit"])
+                self.fit_combo_box.set(keys[0])
+                self.fit_combo_box.selected = keys[0]
+                self.set_fit_meta()
+                self.load_from_fit_meta()
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/fitting/fit_option_menu.py` & `pymonke-0.1.2/src/pymonke/gui/fitting/fit_option_menu.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from customtkinter import CTkComboBox
-
-from typing import Callable, Any
-
-from ..misc import get_root, get_meta
-
-
-class FitComboBox(CTkComboBox):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, values=["Add Fit"], command=self.on_selection)
-        self.bind("<Return>", self.add_or_rename)
-
-        self.selection_bindings: list[Callable[[], None]] = []
-        self.return_bindings: list[Callable[[], None]] = []
-        self.delete_bindings: list[Callable[[], None]] = []
-
-        self.selected: str = "Add Fit"
-
-    def add_or_rename(self, _: Any = None) -> None:
-        if (fits := get_meta(self).get("fits")) is None:
-            get_meta(self)["fits"] = fits = dict()
-
-        fit_name: str = self.get()
-        old: list[str] = self.cget("values")
-        if fit_name in old:
-            return
-        if self.selected == "Add Fit":  # Add
-            if fit_name == "Add Fit":
-                return
-            old.insert(-2, fit_name)
-            self.configure(values=old)
-            self.set(fit_name)
-            fits[fit_name] = dict()
-            self.selected = fit_name
-        else:  # Rename or delete
-            if fit_name == "":
-                self.delete_option(self.selected)
-            else:
-                for i, name in enumerate(old):
-                    if name == self.selected:
-                        old[i] = fit_name
-                fits[fit_name] = fits.pop(self.selected)
-                self.selected = fit_name
-                self.configure(values=old)
-        # self.change_meta_of_plotting_arguments()
-        for binding in self.return_bindings:
-            binding()
-
-    def delete_option(self, option_to_delete: str) -> None:
-        options: list[str] = self.cget("values")
-        if option_to_delete not in options:
-            raise ValueError(f"Invalid option: {option_to_delete}. Cannot delete option because it does not exist.")
-        get_root(self).meta["fits"].pop(option_to_delete)
-        options.remove(option_to_delete)
-        self.set("Add Fit")
-        self.selected = "Add Fit"
-        self.configure(values=options)
-        for binding in self.delete_bindings:
-            binding()
-
-    def on_selection(self, _: Any = None) -> None:
-        self.selected = self.get()
-        for binding in self.selection_bindings:
-            binding()
-        # self.change_meta_of_plotting_arguments()
+from customtkinter import CTkComboBox
+
+from typing import Callable, Any
+
+from ..misc import get_root, get_meta
+
+
+class FitComboBox(CTkComboBox):
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__(**kwargs, values=["Add Fit"], command=self.on_selection)
+        self.bind("<Return>", self.add_or_rename)
+
+        self.selection_bindings: list[Callable[[], None]] = []
+        self.return_bindings: list[Callable[[], None]] = []
+        self.delete_bindings: list[Callable[[], None]] = []
+
+        self.selected: str = "Add Fit"
+
+    def add_or_rename(self, _: Any = None) -> None:
+        if (fits := get_meta(self).get("fits")) is None:
+            get_meta(self)["fits"] = fits = dict()
+
+        fit_name: str = self.get()
+        old: list[str] = self.cget("values")
+        if fit_name in old:
+            return
+        if self.selected == "Add Fit":  # Add
+            if fit_name == "Add Fit":
+                return
+            old.insert(-2, fit_name)
+            self.configure(values=old)
+            self.set(fit_name)
+            fits[fit_name] = dict()
+            self.selected = fit_name
+        else:  # Rename or delete
+            if fit_name == "":
+                self.delete_option(self.selected)
+            else:
+                for i, name in enumerate(old):
+                    if name == self.selected:
+                        old[i] = fit_name
+                fits[fit_name] = fits.pop(self.selected)
+                self.selected = fit_name
+                self.configure(values=old)
+        # self.change_meta_of_plotting_arguments()
+        for binding in self.return_bindings:
+            binding()
+
+    def delete_option(self, option_to_delete: str) -> None:
+        options: list[str] = self.cget("values")
+        if option_to_delete not in options:
+            raise ValueError(f"Invalid option: {option_to_delete}. Cannot delete option because it does not exist.")
+        get_root(self).meta["fits"].pop(option_to_delete)
+        options.remove(option_to_delete)
+        self.set("Add Fit")
+        self.selected = "Add Fit"
+        self.configure(values=options)
+        for binding in self.delete_bindings:
+            binding()
+
+    def on_selection(self, _: Any = None) -> None:
+        self.selected = self.get()
+        for binding in self.selection_bindings:
+            binding()
+        # self.change_meta_of_plotting_arguments()
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/formula/parameter_frame.py` & `pymonke-0.1.2/src/pymonke/gui/formula/parameter_frame.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from customtkinter import CTkFrame, CTkEntry, StringVar, CTkLabel
-
-from typing import Any, Callable
-
-
-class ParameterFrame(CTkFrame):
-    def __init__(self, name: str, **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-
-        self.name = name
-        self.value = CTkLabel(master=self, text="", width=120)
-        self.name_var = StringVar(master=self, value=name)
-        self.name_entry = CTkEntry(master=self, textvariable=self.name_var, width=50)
-        self.name_entry.grid(row=0, column=0, padx=10)
-        self.name_entry.bind("<Return>", command=self.rename)
-        self.value.grid(row=0, column=1, sticky="w")
-
-    def get_name(self) -> str:
-        return self.name
-
-    def set_name(self, name: str) -> None:
-        self.name = name
-        self.name_var.set(name)
-
-    def get_entry(self) -> str:
-        ret = self.name_entry.get()
-        assert isinstance(ret, str)
-        return ret
-
-    def reset_entry(self) -> None:
-        """Resets the entry to the name."""
-        self.set_name(self.name)
-
-    def set_value(self, value: Any) -> None:
-        self.value.configure(text=str(value))
-
-    def rename(self, _: Any) -> None:
-        temp = self.master
-        while True:
-            if hasattr(temp, "rename"):
-                if callable(temp.rename):
-                    temp.rename()
-                    return
-            temp = temp.master
-
+from customtkinter import CTkFrame, CTkEntry, StringVar, CTkLabel
+
+from typing import Any, Callable
+
+
+class ParameterFrame(CTkFrame):
+    def __init__(self, name: str, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+
+        self.name = name
+        self.value = CTkLabel(master=self, text="", width=120)
+        self.name_var = StringVar(master=self, value=name)
+        self.name_entry = CTkEntry(master=self, textvariable=self.name_var, width=50)
+        self.name_entry.grid(row=0, column=0, padx=10)
+        self.name_entry.bind("<Return>", command=self.rename)
+        self.value.grid(row=0, column=1, sticky="w")
+
+    def get_name(self) -> str:
+        return self.name
+
+    def set_name(self, name: str) -> None:
+        self.name = name
+        self.name_var.set(name)
+
+    def get_entry(self) -> str:
+        ret = self.name_entry.get()
+        assert isinstance(ret, str)
+        return ret
+
+    def reset_entry(self) -> None:
+        """Resets the entry to the name."""
+        self.set_name(self.name)
+
+    def set_value(self, value: Any) -> None:
+        self.value.configure(text=str(value))
+
+    def rename(self, _: Any) -> None:
+        temp = self.master
+        while True:
+            if hasattr(temp, "rename"):
+                if callable(temp.rename):
+                    temp.rename()
+                    return
+            temp = temp.master
+
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/formula/parameters_scrollable_frame.py` & `pymonke-0.1.2/src/pymonke/gui/formula/parameters_scrollable_frame.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from customtkinter import CTkScrollableFrame
-
-from typing import Optional, Any
-
-from pymonke.fit.parse import rename_parameters, RepetitionError
-from .parameter_frame import ParameterFrame
-from ..misc import EntryError
-
-
-class ParametersScrollableFrame(CTkScrollableFrame):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-
-        self.param_frames: dict[str, ParameterFrame] = dict()
-
-    def generate_parameter_frames(self, params: list[str]) -> None:
-        self.delete_parameter_frames()
-
-        for index, param in enumerate(params):
-            self.param_frames[param] = ParameterFrame(master=self, name=param)
-            self.param_frames[param].grid(row=index, column=0, sticky="ew")
-
-    def get_params(self) -> Optional[list[str]]:
-        if (val := self.param_frames) is None:
-            return None
-        return list(val.keys())
-
-    def set_param_values(self, values: dict[str, Any]) -> None:
-        keys = self.param_frames.keys()
-        if keys != values.keys():
-            raise EntryError("Parameter names do not match.")
-        for key in keys:
-            self.param_frames[key].set_value(values[key])
-
-    def delete_parameter_frames(self) -> None:
-        if self.param_frames is not None:
-            for frame in self.param_frames.values():
-                frame.destroy()
-        self.param_frames = dict()
-
-    def rename_entries(self, formula: str) -> str:
-        """Renames the entries if this is possible and outputs the new formula."""
-        param_rename = dict()
-        for old, frame in zip(self.param_frames.keys(), self.param_frames.values()):
-            if old != (new := frame.get_entry()):
-                param_rename[old] = new
-        try:
-            formula = rename_parameters(formula, param_rename)  # could fail
-        except (RepetitionError, ValueError) as e:
-            for frame in self.param_frames.values():
-                frame.reset_entry()
-            raise EntryError(e.__repr__())
-
-        for old in param_rename.keys():
-            new = param_rename[old]
-            frame = self.param_frames[old]
-            frame.set_name(new)
-            self.param_frames[new] = self.param_frames.pop(old)
-        return formula
-
-    def reset_parameter_entries(self) -> None:
-        for frame in self.param_frames.values():
-            frame.reset_entry()
+from customtkinter import CTkScrollableFrame
+
+from typing import Optional, Any
+
+from pymonke.fit.parse import rename_parameters, RepetitionError
+from .parameter_frame import ParameterFrame
+from ..misc import EntryError
+
+
+class ParametersScrollableFrame(CTkScrollableFrame):
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+
+        self.param_frames: dict[str, ParameterFrame] = dict()
+
+    def generate_parameter_frames(self, params: list[str]) -> None:
+        self.delete_parameter_frames()
+
+        for index, param in enumerate(params):
+            self.param_frames[param] = ParameterFrame(master=self, name=param)
+            self.param_frames[param].grid(row=index, column=0, sticky="ew")
+
+    def get_params(self) -> Optional[list[str]]:
+        if (val := self.param_frames) is None:
+            return None
+        return list(val.keys())
+
+    def set_param_values(self, values: dict[str, Any]) -> None:
+        keys = self.param_frames.keys()
+        if keys != values.keys():
+            raise EntryError("Parameter names do not match.")
+        for key in keys:
+            self.param_frames[key].set_value(values[key])
+
+    def delete_parameter_frames(self) -> None:
+        if self.param_frames is not None:
+            for frame in self.param_frames.values():
+                frame.destroy()
+        self.param_frames = dict()
+
+    def rename_entries(self, formula: str) -> str:
+        """Renames the entries if this is possible and outputs the new formula."""
+        param_rename = dict()
+        for old, frame in zip(self.param_frames.keys(), self.param_frames.values()):
+            if old != (new := frame.get_entry()):
+                param_rename[old] = new
+        try:
+            formula = rename_parameters(formula, param_rename)  # could fail
+        except (RepetitionError, ValueError) as e:
+            for frame in self.param_frames.values():
+                frame.reset_entry()
+            raise EntryError(e.__repr__())
+
+        for old in param_rename.keys():
+            new = param_rename[old]
+            frame = self.param_frames[old]
+            frame.set_name(new)
+            self.param_frames[new] = self.param_frames.pop(old)
+        return formula
+
+    def reset_parameter_entries(self) -> None:
+        for frame in self.param_frames.values():
+            frame.reset_entry()
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/misc.py` & `pymonke-0.1.2/src/pymonke/gui/misc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,107 @@
-from customtkinter import CTkBaseClass
-import pandas as pd
-
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
-import os
-from tkinter import filedialog
-from typing import Any, Optional
-
-
-class EntryError(Exception):
-    """Error that occurs when trying to enter a text into an entry that is not supposed to be entered
-    by the user."""
-
-    def __init__(self, text: str = "Invalid Entry"):
-        Exception.__init__(self, text)
-
-
-def browse_files(text: str, file_type: str) -> str:
-    """Search for a file in the file explorer."""
-    filename = filedialog.askopenfilename(initialdir=os.getcwd(), title="Select a File",
-                                          filetypes=((text, file_type), ("all files", "*.*")))
-
-    return filename
-
-
-@dataclass
-class Root:
-    meta: dict[str, Any] = field(default_factory=dict)
-    data: Optional[pd.DataFrame] = None
-    fit_result: Optional[dict[str, Any]] = None
-
-    @abstractmethod
-    def load_from_meta(self) -> None:
-        """Update everything based on the meta dictionary."""
-        pass
-
-    @abstractmethod
-    def get_x(self) -> "Optional[pd.Series[float]]": pass
-
-    @abstractmethod
-    def get_y(self) -> "Optional[pd.Series[float]]": pass
-
-    @abstractmethod
-    def get_sx(self) -> "Optional[pd.Series[float]]": pass
-
-    @abstractmethod
-    def get_sy(self) -> "Optional[pd.Series[float]]": pass
-
-    @abstractmethod
-    def get_plot_frame(self) -> Any: pass
-
-    @abstractmethod
-    def do_fit(self) -> Any: pass
-
-    @abstractmethod
-    def get_fit_frame(self) -> Any: pass
-
-    @abstractmethod
-    def get_fit_meta(self) -> Optional[dict[str, Any]]: pass
-
-    @abstractmethod
-    def get_additional_arguments(self) -> dict[str, Any]: pass
-
-    @abstractmethod
-    def get_plotting_style_arguments(self) -> dict[str, Any]: pass
-
-    def __lt__(self, other: Any) -> bool:
-        assert isinstance(self.data, pd.DataFrame)
-        return len(self.data) < len(other.data)
-
-    def __hash__(self) -> int:
-        return hash(1)
-
-
-def get_meta(obj: CTkBaseClass) -> dict[str, Any]:
-    """Get the metadata for data fitting by looking for a master object that has the meta attribute
-    and is a subclass of Root."""
-    master = obj.master
-    while not isinstance(master, Root):
-        master = master.master
-
-    assert isinstance(master, Root)
-    return master.meta
-
-
-def get_data(obj: CTkBaseClass) -> Optional[pd.DataFrame]:
-    """Get the metadata for data fitting by looking for a master object that has the meta attribute
-    and is a subclass of Root."""
-    master = obj.master
-    while not isinstance(master, Root):
-        master = master.master
-
-    assert isinstance(master, Root)
-    return master.data
-
-
-def get_root(obj: CTkBaseClass) -> Root:
-    """Get the Root object."""
-    master = obj.master
-    while not isinstance(master, Root):
-        master = master.master
-
-    assert isinstance(master, Root)
-    return master
+"""@private"""
+
+from customtkinter import CTkBaseClass
+import pandas as pd
+
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+import os
+from tkinter import filedialog
+from typing import Any, Optional
+
+
+class EntryError(Exception):
+    """Error that occurs when trying to enter a text into an entry that is not supposed to be entered
+    by the user."""
+
+    def __init__(self, text: str = "Invalid Entry"):
+        Exception.__init__(self, text)
+
+
+def browse_files(text: str, file_type: str) -> str:
+    """Search for a file in the file explorer."""
+    filename = filedialog.askopenfilename(initialdir=os.getcwd(), title="Select a File",
+                                          filetypes=((text, file_type), ("all files", "*.*")))
+
+    return filename
+
+
+@dataclass
+class Root:
+    meta: dict[str, Any] = field(default_factory=dict)
+    data: Optional[pd.DataFrame] = None
+    fit_result: Optional[dict[str, Any]] = None
+
+    @abstractmethod
+    def load_from_meta(self) -> None:
+        """Update everything based on the meta dictionary."""
+        pass
+
+    @abstractmethod
+    def get_x(self) -> "Optional[pd.Series[float]]": pass
+
+    @abstractmethod
+    def get_y(self) -> "Optional[pd.Series[float]]": pass
+
+    @abstractmethod
+    def get_sx(self) -> "Optional[pd.Series[float]]": pass
+
+    @abstractmethod
+    def get_sy(self) -> "Optional[pd.Series[float]]": pass
+
+    @abstractmethod
+    def get_plot_frame(self) -> Any: pass
+
+    @abstractmethod
+    def do_fit(self) -> Any: pass
+
+    @abstractmethod
+    def get_fit_frame(self) -> Any: pass
+
+    @abstractmethod
+    def get_fit_meta(self) -> Optional[dict[str, Any]]: pass
+
+    @abstractmethod
+    def get_additional_arguments(self) -> dict[str, Any]: pass
+
+    @abstractmethod
+    def get_plotting_style_arguments(self) -> dict[str, Any]: pass
+
+    def __lt__(self, other: Any) -> bool:
+        assert isinstance(self.data, pd.DataFrame)
+        return len(self.data) < len(other.data)
+
+    def __hash__(self) -> int:
+        return hash(1)
+
+
+def get_meta(obj: CTkBaseClass) -> dict[str, Any]:
+    """Get the metadata for data fitting by looking for a master object that has the meta attribute
+    and is a subclass of Root."""
+    master = obj.master
+    while not isinstance(master, Root):
+        master = master.master
+
+    assert isinstance(master, Root)
+    return master.meta
+
+
+def get_data(obj: CTkBaseClass) -> Optional[pd.DataFrame]:
+    """Get the metadata for data fitting by looking for a master object that has the meta attribute
+    and is a subclass of Root."""
+    master = obj.master
+    while not isinstance(master, Root):
+        master = master.master
+
+    assert isinstance(master, Root)
+    return master.data
+
+
+def get_root(obj: CTkBaseClass) -> Root:
+    """Get the Root object."""
+    master = obj.master
+    while not isinstance(master, Root):
+        master = master.master
+
+    assert isinstance(master, Root)
+    return master
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/plot/misc_data_frame.py` & `pymonke-0.1.2/src/pymonke/gui/plot/misc_data_frame.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-from customtkinter import CTkFrame, CTkCheckBox
-
-import json
-from typing import Any, Optional, AnyStr
-
-from ..labeled_entry import LabeledEntry
-from ..misc import get_meta
-
-
-def dumps(obj: Any) -> str:
-    obj = json.dumps(obj)
-    ret = obj.replace("[", "").replace("]", "").replace(" ", "").replace("'", "").replace('"', "")
-    assert isinstance(ret, str)
-    return ret
-
-
-class MiscDataFrame(CTkFrame):
-    def __init__(self, meta: Optional[dict[str, Any]] = None, **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-        self.figure_style_entry = LabeledEntry(master=self, label="Figure style")
-        self.figure_style_entry.entry.bind("<Return>", self.callback)
-        self.figure_style_entry.grid(row=0, column=0, pady=5)
-
-        self.figure_size_entry = LabeledEntry(master=self, label="Figure size")
-        self.figure_size_entry.entry.bind("<Return>", self.callback)
-        self.figure_size_entry.grid(row=1, column=0, pady=5)
-
-        self.dpi_entry = LabeledEntry(master=self, label="DPI")
-        self.dpi_entry.entry.bind("<Return>", self.callback)
-        self.dpi_entry.grid(row=0, column=1, pady=5)
-
-        self.label_entry = LabeledEntry(master=self, label="Label")
-        self.label_entry.entry.bind("<Return>", self.callback)
-        self.label_entry.grid(row=1, column=1, pady=5)
-
-        self.latex_check_box = CTkCheckBox(master=self, text="Latex", command=self.callback)
-        self.latex_check_box.grid(row=2, column=0, pady=5)
-
-        self.meta = meta
-
-    def callback(self, _: Any = None) -> None:
-        # self.update_figure_style(self.figure_style_entry.text_var.get())
-        figure_style: Optional[list[str]] = self.set_figure_style(self.figure_style_entry.text_var.get())
-        figure_size: Optional[tuple[float, float]] = self.set_figure_size(self.figure_size_entry.text_var.get())
-        dpi: Optional[float] = self.set_dpi(self.dpi_entry.text_var.get())
-        label: str = self.get_label()
-        latex: bool = bool(self.latex_check_box.get())
-        data = {
-            "figure_style": figure_style,
-            "figure_size": figure_size,
-            "figure_dpi": dpi,
-            "label": label,
-            "latex": latex,
-        }
-
-        if self.meta is not None:
-            self.meta.update(data)
-
-    def load_from_meta(self) -> None:
-        if self.meta is None:
-            return
-        self.set_figure_style((self.meta.get("figure_style") or ""))
-        self.set_figure_size(self.meta.get("figure_size") or "")
-        self.set_dpi(self.meta.get("figure_dpi") or "")
-        self.set_label(self.meta.get("label") or "")
-        if self.meta.get("latex") or False:
-            self.latex_check_box.select()
-        else:
-            self.latex_check_box.deselect()
-
-    def get_figure_style(self) -> list[str]:
-        text = self.figure_style_entry.text
-        ret = text.split(",")
-        assert isinstance(ret, list)
-        return ret
-
-    def set_figure_style(self, text: str | Any) -> Optional[list[str]]:
-        if text is None:
-            return None
-        if not isinstance(text, str):
-            text = dumps(text)
-        if text == "":
-            self.figure_style_entry.text = ""
-            self.figure_style_entry.text_var.set("")
-            return None
-        self.figure_style_entry.text = text
-        self.figure_style_entry.text_var.set(text)
-        ret = text.split(",")
-        assert isinstance(ret, list)
-        return ret
-
-    def get_figure_size(self) -> Optional[tuple[float, float]]:
-        return self.set_figure_size(self.figure_size_entry.text)
-
-    def set_figure_size(self, text: str) -> Optional[tuple[float, float]]:
-        if text is None:
-            return None
-        if not isinstance(text, str):
-            text = dumps(text)
-        entry = self.figure_size_entry
-        if text == "":
-            entry.text = ""
-            entry.text_var.set("")
-            return None
-        try:
-            ret = text.split(",")
-            assert len(ret) == 2 and isinstance(ret, list)
-            res = float(ret[0]), float(ret[1])
-            entry.text_var.set(text)
-            entry.text = text
-            return res[0], res[1]
-        except (AssertionError, ValueError):
-            entry.text_var.set(entry.text)
-            return self.get_figure_size()
-
-    def get_dpi(self) -> Optional[float]:
-        return self.set_dpi(self.dpi_entry.text)
-
-    def set_dpi(self, text: str) -> Optional[float]:
-        entry = self.dpi_entry
-        if text == "":
-            entry.text = ""
-            entry.text_var.set("")
-            return None
-        try:
-            val = float(text)
-            entry.text = text
-            entry.text_var.set(text)
-            return val
-        except ValueError:
-            entry.text_var.set(entry.text)
-            return self.get_dpi()
-
-    def set_label(self, text: str) -> str:
-        self.label_entry.text = text
-        self.label_entry.text_var.set(text)
-        return text
-
-    def get_label(self) -> str:
-        return self.set_label(self.label_entry.text_var.get())
-
+from customtkinter import CTkFrame, CTkCheckBox
+
+import json
+from typing import Any, Optional, AnyStr
+
+from ..labeled_entry import LabeledEntry
+from ..misc import get_meta
+
+
+def dumps(obj: Any) -> str:
+    obj = json.dumps(obj)
+    ret = obj.replace("[", "").replace("]", "").replace(" ", "").replace("'", "").replace('"', "")
+    assert isinstance(ret, str)
+    return ret
+
+
+class MiscDataFrame(CTkFrame):
+    def __init__(self, meta: Optional[dict[str, Any]] = None, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+        self.figure_style_entry = LabeledEntry(master=self, label="Figure style")
+        self.figure_style_entry.entry.bind("<Return>", self.callback)
+        self.figure_style_entry.grid(row=0, column=0, pady=5)
+
+        self.figure_size_entry = LabeledEntry(master=self, label="Figure size")
+        self.figure_size_entry.entry.bind("<Return>", self.callback)
+        self.figure_size_entry.grid(row=1, column=0, pady=5)
+
+        self.dpi_entry = LabeledEntry(master=self, label="DPI")
+        self.dpi_entry.entry.bind("<Return>", self.callback)
+        self.dpi_entry.grid(row=0, column=1, pady=5)
+
+        self.label_entry = LabeledEntry(master=self, label="Label")
+        self.label_entry.entry.bind("<Return>", self.callback)
+        self.label_entry.grid(row=1, column=1, pady=5)
+
+        self.latex_check_box = CTkCheckBox(master=self, text="Latex", command=self.callback)
+        self.latex_check_box.grid(row=2, column=0, pady=5)
+
+        self.meta = meta
+
+    def callback(self, _: Any = None) -> None:
+        # self.update_figure_style(self.figure_style_entry.text_var.get())
+        figure_style: Optional[list[str]] = self.set_figure_style(self.figure_style_entry.text_var.get())
+        figure_size: Optional[tuple[float, float]] = self.set_figure_size(self.figure_size_entry.text_var.get())
+        dpi: Optional[float] = self.set_dpi(self.dpi_entry.text_var.get())
+        label: str = self.get_label()
+        latex: bool = bool(self.latex_check_box.get())
+        data = {
+            "figure_style": figure_style,
+            "figure_size": figure_size,
+            "figure_dpi": dpi,
+            "label": label,
+            "latex": latex,
+        }
+
+        if self.meta is not None:
+            self.meta.update(data)
+
+    def load_from_meta(self) -> None:
+        if self.meta is None:
+            return
+        self.set_figure_style((self.meta.get("figure_style") or ""))
+        self.set_figure_size(self.meta.get("figure_size") or "")
+        self.set_dpi(self.meta.get("figure_dpi") or "")
+        self.set_label(self.meta.get("label") or "")
+        if self.meta.get("latex") or False:
+            self.latex_check_box.select()
+        else:
+            self.latex_check_box.deselect()
+
+    def get_figure_style(self) -> list[str]:
+        text = self.figure_style_entry.text
+        ret = text.split(",")
+        assert isinstance(ret, list)
+        return ret
+
+    def set_figure_style(self, text: str | Any) -> Optional[list[str]]:
+        if text is None:
+            return None
+        if not isinstance(text, str):
+            text = dumps(text)
+        if text == "":
+            self.figure_style_entry.text = ""
+            self.figure_style_entry.text_var.set("")
+            return None
+        self.figure_style_entry.text = text
+        self.figure_style_entry.text_var.set(text)
+        ret = text.split(",")
+        assert isinstance(ret, list)
+        return ret
+
+    def get_figure_size(self) -> Optional[tuple[float, float]]:
+        return self.set_figure_size(self.figure_size_entry.text)
+
+    def set_figure_size(self, text: str) -> Optional[tuple[float, float]]:
+        if text is None:
+            return None
+        if not isinstance(text, str):
+            text = dumps(text)
+        entry = self.figure_size_entry
+        if text == "":
+            entry.text = ""
+            entry.text_var.set("")
+            return None
+        try:
+            ret = text.split(",")
+            assert len(ret) == 2 and isinstance(ret, list)
+            res = float(ret[0]), float(ret[1])
+            entry.text_var.set(text)
+            entry.text = text
+            return res[0], res[1]
+        except (AssertionError, ValueError):
+            entry.text_var.set(entry.text)
+            return self.get_figure_size()
+
+    def get_dpi(self) -> Optional[float]:
+        return self.set_dpi(self.dpi_entry.text)
+
+    def set_dpi(self, text: str) -> Optional[float]:
+        entry = self.dpi_entry
+        if text == "":
+            entry.text = ""
+            entry.text_var.set("")
+            return None
+        try:
+            val = float(text)
+            entry.text = text
+            entry.text_var.set(text)
+            return val
+        except ValueError:
+            entry.text_var.set(entry.text)
+            return self.get_dpi()
+
+    def set_label(self, text: str) -> str:
+        self.label_entry.text = text
+        self.label_entry.text_var.set(text)
+        return text
+
+    def get_label(self) -> str:
+        return self.set_label(self.label_entry.text_var.get())
+
```

### Comparing `pymonke-0.1.1/src/pymonke/gui/plot/plot_frame.py` & `pymonke-0.1.2/src/pymonke/gui/plot/plot_frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,108 @@
-from customtkinter import CTkFrame, CTkButton
-
-import json
-from typing import Any
-
-from pymonke.misc.pymonke_json_encoder import PyMonkeJSONEncoder
-from ..data_init.browse_save_frame import BrowseSaveFrame
-from ..dict_frame import DictFrame
-from ..fitting.fit_frame import FitFrame
-from ..info_label import InfoLabel
-from .limits_frame import LimitsFrame
-from ..misc import get_meta, get_root
-from .misc_data_frame import MiscDataFrame
-from .plot_canvas import PlotCanvas
-
-
-class PlotFrame(CTkFrame):
-    def __init__(self, **kwargs: Any) -> None:
-        CTkFrame.__init__(self, **kwargs)
-        self.canvas = PlotCanvas(master=self)
-        self.canvas.grid(row=0, column=0, columnspan=3)
-
-        self.x_limits_frame = LimitsFrame(master=self, label="X Limits", meta=get_meta(self),
-                                          max_lim_key="x_max_limit", min_lim_key="x_min_limit")
-        self.x_limits_frame.entry_bindings = [self.canvas.set_limits_from_meta]
-        self.x_limits_frame.grid(row=1, column=0, columnspan=2)
-
-        self.y_limits_frame = LimitsFrame(master=self, label="Y Limits", meta=get_meta(self),
-                                          max_lim_key="y_max_limit", min_lim_key="y_min_limit")
-        self.y_limits_frame.entry_bindings = [self.canvas.set_limits_from_meta]
-        self.y_limits_frame.grid(row=2, column=0, columnspan=2)
-
-        self.button = CTkButton(self, text="Fit Data", command=self.plot_data)
-        self.button.grid(row=3, column=0, columnspan=2)
-
-        self.info_label = InfoLabel(master=self, text="")
-        self.info_label.grid(row=4, column=0, columnspan=3, pady=5)
-
-        if get_meta(self).get("plotting_style") is None:
-            get_meta(self)["plotting_style"] = dict()
-        self.plotting_arguments = DictFrame(master=self, text="Plotting arguments",
-                                            meta=get_meta(self)["plotting_style"])
-        self.plotting_arguments.grid(row=5, column=0, columnspan=2, pady=5, padx=10)
-
-        self.misc_data_frame = MiscDataFrame(master=self)
-        self.misc_data_frame.meta = get_meta(self)
-        self.misc_data_frame.grid(row=1, column=2, rowspan=2)
-
-        self.save_results_frame = BrowseSaveFrame(master=self)
-        self.save_results_frame.save_button.configure(command=self.save_results)
-        self.save_results_frame.grid(row=5, column=2, padx=10)
-
-    def plot_data(self) -> None:
-        try:
-            self.canvas.plot_data()
-            _min, _max = self.canvas.ax.get_xlim()
-            self.x_limits_frame.set_limits(_min, _max)
-            self.info_label.show_info("Plotting the data and/or fitting successful.")
-        except Exception as e:
-            self.info_label.show_error(e.__repr__())
-
-        # show parameter values after the fit
-        fit_frame: FitFrame = get_root(self).get_fit_frame()
-        fit_frame.set_params_values_from_results()
-
-    def load_from_meta(self) -> None:
-        self.plot_data()
-        meta = get_meta(self)
-        _min, _max = meta.get("x_min_limit"), meta.get("x_max_limit")
-        if _min is not None:
-            self.x_limits_frame.set_min(_min)
-        if _max is not None:
-            self.x_limits_frame.set_max(_max)
-        self.canvas.set_x_limits(_min, _max)
-
-        if get_meta(self).get("plotting_style") is None:
-            get_meta(self)["plotting_style"] = dict()
-        self.plotting_arguments.meta = get_meta(self)["plotting_style"]
-        self.plotting_arguments.load_from_meta()
-        self.misc_data_frame.load_from_meta()
-
-    def load_limits_to_meta(self, _: Any = None) -> None:
-        _min = float(self.x_limits_frame.min_var.get())
-        _max = float(self.x_limits_frame.max_var.get())
-        get_meta(self)["x_min_limit"] = _min
-        get_meta(self)["x_max_limit"] = _max
-
-    def save_results(self) -> None:
-        try:
-            results = get_root(self).fit_result
-            ret = dict()
-            if results is None:
-                return
-            for key in results.keys():
-                ret[key] = results[key].as_dict(True)  # type: ignore
-
-            text = json.dumps(ret, indent=2, cls=PyMonkeJSONEncoder)
-            file = self.save_results_frame.browse_frame.file_path.get()
-            with open(file, "w") as f:
-                f.write(text)
-            self.info_label.show_info("Results saved successfully.")
-        except Exception as e:
-            self.info_label.show_error(e.__repr__())
-
-
+from customtkinter import CTkFrame, CTkButton
+
+import json
+from typing import Any
+import warnings
+
+from pymonke.misc.pymonke_json_encoder import PyMonkeJSONEncoder
+from ..data_init.browse_save_frame import BrowseSaveFrame
+from ..dict_frame import DictFrame
+from ..fitting.fit_frame import FitFrame
+from ..info_label import InfoLabel
+from .limits_frame import LimitsFrame
+from ..misc import get_meta, get_root
+from .misc_data_frame import MiscDataFrame
+from .plot_canvas import PlotCanvas
+
+
+class PlotFrame(CTkFrame):
+    def __init__(self, **kwargs: Any) -> None:
+        CTkFrame.__init__(self, **kwargs)
+        self.canvas = PlotCanvas(master=self)
+        self.canvas.grid(row=0, column=0, columnspan=3)
+
+        self.x_limits_frame = LimitsFrame(master=self, label="X Limits", meta=get_meta(self),
+                                          max_lim_key="x_max_limit", min_lim_key="x_min_limit")
+        self.x_limits_frame.entry_bindings = [self.canvas.set_limits_from_meta]
+        self.x_limits_frame.grid(row=1, column=0, columnspan=2)
+
+        self.y_limits_frame = LimitsFrame(master=self, label="Y Limits", meta=get_meta(self),
+                                          max_lim_key="y_max_limit", min_lim_key="y_min_limit")
+        self.y_limits_frame.entry_bindings = [self.canvas.set_limits_from_meta]
+        self.y_limits_frame.grid(row=2, column=0, columnspan=2)
+
+        self.button = CTkButton(self, text="Fit Data", command=self.plot_data)
+        self.button.grid(row=3, column=0, columnspan=2)
+
+        self.info_label = InfoLabel(master=self, text="")
+        self.info_label.grid(row=4, column=0, columnspan=3, pady=5)
+
+        if get_meta(self).get("plotting_style") is None:
+            get_meta(self)["plotting_style"] = dict()
+        self.plotting_arguments = DictFrame(master=self, text="Plotting arguments",
+                                            meta=get_meta(self)["plotting_style"])
+        self.plotting_arguments.grid(row=5, column=0, columnspan=2, pady=5, padx=10)
+
+        self.misc_data_frame = MiscDataFrame(master=self)
+        self.misc_data_frame.meta = get_meta(self)
+        self.misc_data_frame.grid(row=1, column=2, rowspan=2)
+
+        self.save_results_frame = BrowseSaveFrame(master=self)
+        self.save_results_frame.save_button.configure(command=self.save_results)
+        self.save_results_frame.grid(row=5, column=2, padx=10)
+
+    def plot_data(self) -> None:
+        warnings.filterwarnings("error")
+        try:
+            self.canvas.plot_data()
+            _min, _max = self.canvas.ax.get_xlim()
+            self.x_limits_frame.set_limits(_min, _max)
+            self.info_label.show_info("Plotting the data and/or fitting successful.")
+        except (Exception, RuntimeWarning) as e:
+            self.info_label.show_error(e.__repr__())
+
+        # show parameter values after the fit
+        fit_frame: FitFrame = get_root(self).get_fit_frame()
+        fit_frame.set_params_values_from_results()
+        warnings.filterwarnings("default")
+
+    def load_from_meta(self) -> None:
+        self.plot_data()
+        meta = get_meta(self)
+        _min, _max = meta.get("x_min_limit"), meta.get("x_max_limit")
+        if _min is not None:
+            self.x_limits_frame.set_min(_min)
+        if _max is not None:
+            self.x_limits_frame.set_max(_max)
+        self.canvas.set_x_limits(_min, _max)
+
+        if get_meta(self).get("plotting_style") is None:
+            get_meta(self)["plotting_style"] = dict()
+        self.plotting_arguments.meta = get_meta(self)["plotting_style"]
+        self.plotting_arguments.load_from_meta()
+        self.misc_data_frame.load_from_meta()
+
+    def load_limits_to_meta(self, _: Any = None) -> None:
+        _min = float(self.x_limits_frame.min_var.get())
+        _max = float(self.x_limits_frame.max_var.get())
+        get_meta(self)["x_min_limit"] = _min
+        get_meta(self)["x_max_limit"] = _max
+
+    def save_results(self) -> None:
+        try:
+            results = get_root(self).fit_result
+            ret = dict()
+            if results is None:
+                return
+            for key in results.keys():
+                ret[key] = results[key].as_dict(True)  # type: ignore
+
+            text = json.dumps(ret, indent=2, cls=PyMonkeJSONEncoder)
+            file = self.save_results_frame.browse_frame.file_path.get()
+            with open(file, "w") as f:
+                f.write(text)
+            self.info_label.show_info("Results saved successfully.")
+        except Exception as e:
+            self.info_label.show_error(e.__repr__())
+
+
```

### Comparing `pymonke-0.1.1/src/pymonke/latex/utils.py` & `pymonke-0.1.2/src/pymonke/latex/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import pandas as pd
-
-from uncertainties import ufloat
-from typing import Any
-
-from ..misc.dataframe import get_error_column_name
-
-
-def transform_dataframe_to_latex_ready(data: pd.DataFrame, **kwargs: Any) -> pd.DataFrame:
-    # initialize all keyword arguments
-    if kwargs.get("error_marker") is None:
-        kwargs["error_marker"] = ["err", "error", "fehler", "Err", "Error", "Fehler"]
-    else:
-        list(kwargs["error_marker"])
-    if kwargs.get("columns") is None:
-        kwargs["columns"] = {}
-    else:
-        dict(kwargs["columns"])
-    if kwargs.get("ignore_rest") is None:
-        kwargs["ignore_rest"] = False
-    if not isinstance(kwargs["ignore_rest"], bool):
-        raise TypeError("ignore_rest must be boolean")
-    if kwargs.get("is_table_num") is None:
-        kwargs["is_table_num"] = True
-    if not isinstance(kwargs["is_table_num"], bool):
-        raise TypeError("is_table must be a boolean")
-    if kwargs.get("siunitx_column_option") is None:
-        kwargs["siunitx_column_option"] = {}
-    else:
-        dict(kwargs["siunitx_column_option"])
-
-    new_dataframe = data.copy()  # new dataframe for end result
-    new_dataframe = new_dataframe.apply(lambda x: replace_ufloat_with_latex_macro(x, **kwargs), axis=0)
-
-    # look for columns with errors
-    for column in data.columns:
-        error = get_error_column_name(data, column, kwargs["error_marker"])
-        if error is None:
-            continue
-        num_data = data[column]
-        error_data = data[error]
-        new_data = []
-        option: str | None = kwargs["siunitx_column_option"].get(column)
-        for x, err in zip(num_data, error_data):
-            num = "{:S}".format(ufloat(x, err))
-            # if kwargs["is_table_num"]:
-            #     new_data.append(NumWithError(x, err).display_table_separate(option))
-            # else:
-            #     new_data.append(NumWithError(x, err).display_separate(option))
-            new_data.append(num_in_siunitx(num, kwargs["is_table_num"], option))
-        new_dataframe[column] = new_data
-        new_dataframe.drop(error, axis=1, inplace=True)
-
-
-    if kwargs["ignore_rest"]:
-        columns = list(new_dataframe.columns)
-        columns_to_ignore = [c for c in columns if c not in kwargs["columns"]]
-        new_dataframe.drop(columns=columns_to_ignore, inplace=True)
-
-    for col in list(new_dataframe.columns):
-        option = kwargs["siunitx_column_option"].get(col)
-        is_table_num: bool = kwargs["is_table_num"]
-        new_dataframe[col] = [__display_num_value(i, option, is_table_num) if isinstance(i, (int, float)) else i
-                              for i in new_dataframe[col]]
-
-    new_dataframe.rename(columns=kwargs["columns"], inplace=True)
-
-    return new_dataframe
-
-
-def num_in_siunitx(num: str, is_table_num: bool = False, option: str | None = None) -> str:
-    """Wraps number string insided \num or \tablenum macro depending on is_table_num boolean.
-    option is another string put in []  as a macro option. """
-    if is_table_num:
-        text = "tablenum"
-    else:
-        text = "num"
-    if option is None:
-        option = ""
-    else:
-        option = f"[{option}]"
-
-    return f"\\{text}{option}{{{num}}}"
-
-
-def replace_ufloat_with_latex_macro(x: pd.Series, **kwargs: Any) -> pd.Series:
-    def func(i: Any) -> Any:
-        try:
-            val = "{:S}".format(i)
-            return num_in_siunitx(val, kwargs.get("is_table_num") or False,
-                                  kwargs["siunitx_column_option"].get(x.name))
-        except:
-            return i
-
-    return x.apply(func)
-
-
-def __display_num_value(x: int | float, option: str | None = None, is_table_num: bool = True) -> str | None:
-    """takes a number and formats it to use with the siunitx package. Returns None if the value is not a number
-    Example
-    -------
-    __display_num_value(2.3, sinuitx_option="round-mode=figures") -> \tablenum[round-mode=figures]{2.3}"""
-    if str(x) == "nan":
-        return None
-    if option != "" and option is not None:
-        option = f"[{option}]"
-    else:
-        option = ""
-
-    macro = "tablenum"
-    if not is_table_num:
-        macro = "num"
-    return f"\\{macro}{option}{{{x}}}"
-
-
-if __name__ == "__main__":
-    print(__display_num_value(2.23, option="round-mode=figures", is_table_num=False))
+import pandas as pd
+
+from uncertainties import ufloat  # type: ignore
+from typing import Any
+
+from ..misc.dataframe import get_error_column_name
+
+
+def transform_dataframe_to_latex_ready(data: pd.DataFrame, **kwargs: Any) -> pd.DataFrame:
+    # initialize all keyword arguments
+    if kwargs.get("error_marker") is None:
+        kwargs["error_marker"] = ["err", "error", "fehler", "Err", "Error", "Fehler"]
+    else:
+        list(kwargs["error_marker"])
+    if kwargs.get("columns") is None:
+        kwargs["columns"] = {}
+    else:
+        dict(kwargs["columns"])
+    if kwargs.get("ignore_rest") is None:
+        kwargs["ignore_rest"] = False
+    if not isinstance(kwargs["ignore_rest"], bool):
+        raise TypeError("ignore_rest must be boolean")
+    if kwargs.get("is_table_num") is None:
+        kwargs["is_table_num"] = True
+    if not isinstance(kwargs["is_table_num"], bool):
+        raise TypeError("is_table must be a boolean")
+    if kwargs.get("siunitx_column_option") is None:
+        kwargs["siunitx_column_option"] = {}
+    else:
+        dict(kwargs["siunitx_column_option"])
+
+    new_dataframe = data.copy()  # new dataframe for end result
+    new_dataframe = new_dataframe.apply(lambda x: _replace_ufloat_with_latex_macro(x, **kwargs), axis=0)
+
+    # look for columns with errors
+    for column in data.columns:
+        error = get_error_column_name(data, column, kwargs["error_marker"])
+        if error is None:
+            continue
+        num_data = data[column]
+        error_data = data[error]
+        new_data = []
+        option: str | None = kwargs["siunitx_column_option"].get(column)
+        for x, err in zip(num_data, error_data):
+            num = "{:S}".format(ufloat(x, err))
+            # if kwargs["is_table_num"]:
+            #     new_data.append(NumWithError(x, err).display_table_separate(option))
+            # else:
+            #     new_data.append(NumWithError(x, err).display_separate(option))
+            new_data.append(_num_in_siunitx(num, kwargs["is_table_num"], option))
+        new_dataframe[column] = new_data
+        new_dataframe.drop(error, axis=1, inplace=True)
+
+
+    if kwargs["ignore_rest"]:
+        columns = list(new_dataframe.columns)
+        columns_to_ignore = [c for c in columns if c not in kwargs["columns"]]
+        new_dataframe.drop(columns=columns_to_ignore, inplace=True)
+
+    for col in list(new_dataframe.columns):
+        option = kwargs["siunitx_column_option"].get(col)
+        is_table_num: bool = kwargs["is_table_num"]
+        new_dataframe[col] = [__display_num_value(i, option, is_table_num) if isinstance(i, (int, float)) else i
+                              for i in new_dataframe[col]]
+
+    new_dataframe.rename(columns=kwargs["columns"], inplace=True)
+
+    return new_dataframe
+
+
+def _num_in_siunitx(num: str, is_table_num: bool = False, option: str | None = None) -> str:
+    """Wraps number string insided \num or \tablenum macro depending on is_table_num boolean.
+    option is another string put in []  as a macro option. """
+    if is_table_num:
+        text = "tablenum"
+    else:
+        text = "num"
+    if option is None:
+        option = ""
+    else:
+        option = f"[{option}]"
+
+    return f"\\{text}{option}{{{num}}}"
+
+
+def _replace_ufloat_with_latex_macro(x: pd.Series, **kwargs: Any) -> pd.Series:
+    def func(i: Any) -> Any:
+        try:
+            val = "{:S}".format(i)  # type: ignore
+            return _num_in_siunitx(val, kwargs.get("is_table_num") or False,
+                                   kwargs["siunitx_column_option"].get(x.name))
+        except:
+            return i
+
+    return x.apply(func)
+
+
+def __display_num_value(x: int | float, option: str | None = None, is_table_num: bool = True) -> str | None:
+    """takes a number and formats it to use with the siunitx package. Returns None if the value is not a number
+    Example
+    -------
+    __display_num_value(2.3, sinuitx_option="round-mode=figures") -> \tablenum[round-mode=figures]{2.3}"""
+    if str(x) == "nan":
+        return None
+    if option != "" and option is not None:
+        option = f"[{option}]"
+    else:
+        option = ""
+
+    macro = "tablenum"
+    if not is_table_num:
+        macro = "num"
+    return f"\\{macro}{option}{{{x}}}"
+
+
+if __name__ == "__main__":
+    print(__display_num_value(2.23, option="round-mode=figures", is_table_num=False))
```

### Comparing `pymonke-0.1.1/src/pymonke/misc/benchmark.py` & `pymonke-0.1.2/src/pymonke/misc/benchmark.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from colorama import Fore, Style
-import timeit
-from typing import Any, TypeAlias, Callable
-
-import numpy as np
-
-from ..mmath.rounding import roundup
-
-func: TypeAlias = Callable[[], Any]
-
-
-def green(text: str) -> str:
-    return f"{Fore.GREEN} {text} {Style.RESET_ALL}"
-
-
-def red(text: str) -> str:
-    return f"{Fore.RED}{text}{Style.RESET_ALL}"
-
-
-def bench_compare(func1: func, func2: func, name: str, number: int = 10_000, iters: int = 20) -> None:
-    x1: Any = []
-    x2: Any = []
-    for _ in range(iters):
-        x1.append(timeit.timeit(func1, globals=locals(), number=number) / number)
-        x2.append(timeit.timeit(func2, globals=locals(), number=number) / number)
-    x1, x2 = np.array(x1[1:]), np.array(x2[1:])
-    m1, m2 = x1.mean(), x2.mean()
-    std1, std2 = x1.std(), x2.std()
-    if m1 > m2:
-        x = round(m1 / m2 - 1, 2)
-        err = roundup(np.sqrt((std1 / m2)**2 + (m1*std2 / m2**2)**2), 2)
-        print(f"{name} benchmark: {x}x +- {err}x {green('faster')} {iters * number} iterations.")
-    else:
-        x = round(m2 / m1 - 1, 2)
-        err = roundup(np.sqrt((std2 / m1) ** 2 + (m2 * std1 / m1 ** 2) ** 2), 2)
-        print(f"{name} benchmark: {x}x +- {err}x {red('slower')} {iters * number} iterations.")
-
-
-def timing(number: int = 10_000, iters: int = 20) -> Callable:
-    def _timing(_func: Callable) -> Callable:
-        def inner():
-            runs = []
-            for _ in range(iters):
-                runs.append(timeit.timeit(_func, globals=locals(), number=number) / number)
-            mean, std = np.mean(runs[1:]), np.std(runs[1:])
-
-            x, err = "{:.2e}".format(mean), "{:.2e}".format(std)
-            print(f"Function '{_func.__name__}' benchmark: {x} +- {err} seconds with {iters * number} iterations.")
-
-        return inner
-
-    return _timing
+"""@private"""
+
+from colorama import Fore, Style  #  type: ignore
+import timeit
+from typing import Any, TypeAlias, Callable
+
+import numpy as np
+
+from ..mmath.rounding import roundup  #  type: ignore
+
+func: TypeAlias = Callable[[], Any]
+
+
+def green(text: str) -> str:
+    return f"{Fore.GREEN} {text} {Style.RESET_ALL}"
+
+
+def red(text: str) -> str:
+    return f"{Fore.RED}{text}{Style.RESET_ALL}"
+
+
+def bench_compare(func1: func, func2: func, name: str, number: int = 10_000, iters: int = 20) -> None:
+    x1: Any = []
+    x2: Any = []
+    for _ in range(iters):
+        x1.append(timeit.timeit(func1, globals=locals(), number=number) / number)
+        x2.append(timeit.timeit(func2, globals=locals(), number=number) / number)
+    x1, x2 = np.array(x1[1:]), np.array(x2[1:])
+    m1, m2 = x1.mean(), x2.mean()
+    std1, std2 = x1.std(), x2.std()
+    if m1 > m2:
+        x = round(m1 / m2 - 1, 2)
+        err = roundup(np.sqrt((std1 / m2)**2 + (m1*std2 / m2**2)**2), 2)
+        print(f"{name} benchmark: {x}x +- {err}x {green('faster')} {iters * number} iterations.")
+    else:
+        x = round(m2 / m1 - 1, 2)
+        err = roundup(np.sqrt((std2 / m1) ** 2 + (m2 * std1 / m1 ** 2) ** 2), 2)
+        print(f"{name} benchmark: {x}x +- {err}x {red('slower')} {iters * number} iterations.")
+
+
+def timing(number: int = 10_000, iters: int = 20) -> Callable:
+    def _timing(_func: Callable) -> Callable:
+        def inner():
+            runs = []
+            for _ in range(iters):
+                runs.append(timeit.timeit(_func, globals=locals(), number=number) / number)
+            mean, std = np.mean(runs[1:]), np.std(runs[1:])
+
+            x, err = "{:.2e}".format(mean), "{:.2e}".format(std)
+            print(f"Function '{_func.__name__}' benchmark: {x} +- {err} seconds with {iters * number} iterations.")
+
+        return inner
+
+    return _timing
```

### Comparing `pymonke-0.1.1/src/pymonke/misc/dataframe.py` & `pymonke-0.1.2/src/pymonke/misc/dataframe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,88 @@
-from pandas import DataFrame
-
-from typing import List, Sequence, Any, Iterable
-
-from uncertainties.core import Variable, AffineScalarFunc
-from uncertainties import ufloat
-
-
-def get_error_column_name(data: DataFrame, column: str, error_marker: List[str] | None = None) -> str | None:
-    """Get the columns name that is the uncertainty of the column argument. return None if not found.
-    parameters
-    ----------
-    data: DataFrame
-    The dataframe to analyze.
-    column: str
-    The name of the column which represents a series of values that have an uncertainty.
-    error_marker: List[str]
-    A list of words that indicate that a column represents a series of uncertainties.
-    """
-    columns = list(data.columns)
-    if column not in columns:
-        raise ValueError("column not in DataFrame")
-
-    if error_marker is None:
-        error_marker = ["error", "err", "fehler", "Error", "Err", "Fehler"]
-
-    error_separator = ["_", "-", " ", ""]
-    result: str | None = None
-    for marker in error_marker:
-        for separator in error_separator:
-            if f"{column}{separator}{marker}" in columns:
-                if result is None:
-                    result = f"{column}{separator}{marker}"
-                else:
-                    text = f"""Error in DataFrame for the column {column} could not be determined because 
-                    of ambivalence. Error marker are {error_marker}"""
-                    raise ValueError(text)
-    return result
-
-
-def has_uncertainty(data: Iterable) -> bool:
-    """checks if the data sequence has an uncertainty attached to it."""
-    for element in data:
-        if not isinstance(element, (Variable, AffineScalarFunc)):
-            return False
-    return True
-
-
-def separate_uncertainties(dataframe: DataFrame, inplace: bool = False, error_name: str = "error") -> DataFrame:
-    if inplace:
-        new_dataframe = dataframe
-    else:
-        new_dataframe = dataframe.copy()
-
-    for column in dataframe.columns:
-        if has_uncertainty(new_dataframe[column]):
-            data = new_dataframe[column]
-            new_dataframe[f"{column} {error_name}"] = [x.std_dev for x in data]
-            new_dataframe[column] = [x.nominal_value for x in data]
-
-    return new_dataframe
-
-
-def join_uncertainties(dataframe: DataFrame, inplace: bool = False,
-                       error_marker: List[str] | None = None) -> DataFrame:
-    """If a Series has uncertainties in another DataFrame, it finds them and  joins
-    into one Series with the Variable type of the uncertainties package."""
-    if inplace:
-        new_dataframe = dataframe
-    else:
-        new_dataframe = dataframe.copy()
-
-    error_columns: list[str] = []
-    for column in new_dataframe.columns:
-        if (error_name := get_error_column_name(new_dataframe, column, error_marker)) is not None:
-            error_columns.append(error_name)
-            new_dataframe[column] = [ufloat(x, err) for x, err in
-                                     zip(new_dataframe[column], new_dataframe[error_name])]
-
-    new_dataframe.drop(error_columns, axis=1, inplace=True)
-    return new_dataframe
+from pandas import DataFrame
+
+from typing import List, Sequence, Any, Iterable
+
+from uncertainties.core import Variable, AffineScalarFunc  # type: ignore
+from uncertainties import ufloat  #type: ignore
+
+
+def get_error_column_name(data: DataFrame, column: str, error_marker: List[str] | None = None) -> str | None:
+    """@private Get the columns name that is the uncertainty of the column argument. return None if not found.
+    parameters
+    ----------
+    data: DataFrame
+    The dataframe to analyze.
+    column: str
+    The name of the column which represents a series of values that have an uncertainty.
+    error_marker: List[str]
+    A list of words that indicate that a column represents a series of uncertainties.
+    """
+    columns = list(data.columns)
+    if column not in columns:
+        raise ValueError("column not in DataFrame")
+
+    if error_marker is None:
+        error_marker = ["error", "err", "fehler", "Error", "Err", "Fehler"]
+
+    error_separator = ["_", "-", " ", ""]
+    result: str | None = None
+    for marker in error_marker:
+        for separator in error_separator:
+            if f"{column}{separator}{marker}" in columns:
+                if result is None:
+                    result = f"{column}{separator}{marker}"
+                else:
+                    text = f"""Error in DataFrame for the column {column} could not be determined because 
+                    of ambivalence. Error marker are {error_marker}"""
+                    raise ValueError(text)
+    return result
+
+
+def has_uncertainty(data: Iterable) -> bool:
+    """@private checks if the data sequence has an uncertainty attached to it."""
+    for element in data:
+        if not isinstance(element, (Variable, AffineScalarFunc)):
+            return False
+    return True
+
+
+def separate_uncertainties(dataframe: DataFrame, inplace: bool = False, error_name: str = "error") -> DataFrame:
+    """If a column inside a DataFrame consists of Variable objects of the uncertainty package,
+    seperates the values and standard deviations into to separate column.
+
+    :param dataframe: Input DataFrame.
+    :param inplace: If True, do an inplace operation.
+    :param error_name: string that gets appended to the column name of the standard deviations.
+    """
+    if inplace:
+        new_dataframe = dataframe
+    else:
+        new_dataframe = dataframe.copy()
+
+    for column in dataframe.columns:
+        if has_uncertainty(new_dataframe[column]):
+            data = new_dataframe[column]
+            new_dataframe[f"{column} {error_name}"] = [x.std_dev for x in data]
+            new_dataframe[column] = [x.nominal_value for x in data]
+
+    return new_dataframe
+
+
+def join_uncertainties(dataframe: DataFrame, inplace: bool = False,
+                       error_marker: List[str] | None = None) -> DataFrame:
+    """If a Series has uncertainties in another DataFrame, it finds them and  joins
+    into one Series with the Variable type of the uncertainties package."""
+    if inplace:
+        new_dataframe = dataframe
+    else:
+        new_dataframe = dataframe.copy()
+
+    error_columns: list[str] = []
+    for column in new_dataframe.columns:
+        if (error_name := get_error_column_name(new_dataframe, column, error_marker)) is not None:
+            error_columns.append(error_name)
+            new_dataframe[column] = [ufloat(x, err) for x, err in
+                                     zip(new_dataframe[column], new_dataframe[error_name])]
+
+    new_dataframe.drop(error_columns, axis=1, inplace=True)
+    return new_dataframe
```

### Comparing `pymonke-0.1.1/src/pymonke/misc/file_management.py` & `pymonke-0.1.2/src/pymonke/misc/file_management.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import numpy as np
-import pandas as pd
-from pandas import DataFrame
-
-from typing import List, Any
-
-
-def get_file_type(filename: str) -> str:
-    return filename.split('.')[-1]
-
-
-def read_txt_into_dataframe(file: str, skiprows: int = 1, **args: Any) -> DataFrame:
-    columns: List[str]
-    with open(file, 'r') as f:
-        if (delim := args.get("delimiter")) is None:
-            delim = " "
-        columns = f.readline().replace(delim, " ").replace("\t", " ").replace("\n", "").split(" ")
-    data = np.loadtxt(file, skiprows=skiprows, **args)
-    return DataFrame(data=data, columns=columns)
-
-
-def read_data_into_dataframe(file: str, **args: Any) -> DataFrame:
-    """tries to Convert the file into a DataFrame"""
-    file_type = get_file_type(file)
-    if file_type == "csv":
-        return pd.read_csv(file, **args)
-    elif file_type == "txt":
-        return read_txt_into_dataframe(file, **args)
-    else:
-        raise ValueError(f"File type {file_type} not supported")
+import numpy as np
+import pandas as pd
+from pandas import DataFrame
+
+from typing import List, Any
+
+
+def get_file_type(filename: str) -> str:
+    return filename.split('.')[-1]
+
+
+def read_txt_into_dataframe(file: str, skiprows: int = 1, **args: Any) -> DataFrame:
+    columns: List[str]
+    with open(file, 'r') as f:
+        if (delim := args.get("delimiter")) is None:
+            delim = " "
+        columns = f.readline().replace(delim, " ").replace("\t", " ").replace("\n", "").split(" ")
+    data = np.loadtxt(file, skiprows=skiprows, **args)
+    return DataFrame(data=data, columns=columns)
+
+
+def read_data_into_dataframe(file: str, **args: Any) -> DataFrame:
+    """tries to Convert the file into a DataFrame"""
+    file_type = get_file_type(file)
+    if file_type == "csv":
+        return pd.read_csv(file, **args)
+    elif file_type == "txt":
+        return read_txt_into_dataframe(file, **args)
+    else:
+        raise ValueError(f"File type {file_type} not supported")
```

### Comparing `pymonke-0.1.1/src/pymonke/misc/pymonke_json_decoder.py` & `pymonke-0.1.2/src/pymonke/misc/pymonke_json_decoder.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from json.decoder import JSONDecoder
-from uncertainties import ufloat_fromstr
-
-from typing import Any
-
-
-class PyMonkeJSONDecoder(JSONDecoder):
-    def __init__(self) -> None:
-        super().__init__(object_hook=self.__object_hook)
-
-    @staticmethod
-    def __object_hook(obj: Any) -> Any:
-        for key, value in obj.items():
-            if isinstance(value, str):
-                obj[key] = PyMonkeJSONDecoder.try_to_ufloat(value)
-            elif isinstance(value, list):
-                obj[key] = [PyMonkeJSONDecoder.try_to_ufloat(x) for x in value]
-
-        return obj
-
-    @staticmethod
-    def try_to_ufloat(x: str) -> Any:
-        try:
-            return ufloat_fromstr(x)
-        except ValueError:
+from json.decoder import JSONDecoder
+from uncertainties import ufloat_fromstr
+
+from typing import Any
+
+
+class PyMonkeJSONDecoder(JSONDecoder):
+    def __init__(self) -> None:
+        super().__init__(object_hook=self.__object_hook)
+
+    @staticmethod
+    def __object_hook(obj: Any) -> Any:
+        for key, value in obj.items():
+            if isinstance(value, str):
+                obj[key] = PyMonkeJSONDecoder.try_to_ufloat(value)
+            elif isinstance(value, list):
+                obj[key] = [PyMonkeJSONDecoder.try_to_ufloat(x) for x in value]
+
+        return obj
+
+    @staticmethod
+    def try_to_ufloat(x: str) -> Any:
+        try:
+            return ufloat_fromstr(x)
+        except ValueError:
             return x
```

### Comparing `pymonke-0.1.1/src/pymonke.egg-info/SOURCES.txt` & `pymonke-0.1.2/src/pymonke.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/pymonke/__init__.py
 src/pymonke/__main__.py
-src/pymonke/constants.py
 src/pymonke/py.typed
 src/pymonke.egg-info/PKG-INFO
 src/pymonke.egg-info/SOURCES.txt
 src/pymonke.egg-info/dependency_links.txt
 src/pymonke.egg-info/requires.txt
 src/pymonke.egg-info/top_level.txt
 src/pymonke/fit/__init__.py
@@ -26,33 +25,33 @@
 src/pymonke/gui/list_frame.py
 src/pymonke/gui/main.py
 src/pymonke/gui/misc.py
 src/pymonke/gui/data_init/__init__.py
 src/pymonke/gui/data_init/browse_save_frame.py
 src/pymonke/gui/data_init/data_init_frame.py
 src/pymonke/gui/data_init/status_frame.py
+src/pymonke/gui/fitting/__init__.py
 src/pymonke/gui/fitting/add_args_frame.py
 src/pymonke/gui/fitting/fit_frame.py
 src/pymonke/gui/fitting/fit_option_menu.py
+src/pymonke/gui/formula/__init__.py
 src/pymonke/gui/formula/formula_frame.py
 src/pymonke/gui/formula/parameter_frame.py
 src/pymonke/gui/formula/parameters_scrollable_frame.py
+src/pymonke/gui/plot/__init__.py
 src/pymonke/gui/plot/limits_frame.py
 src/pymonke/gui/plot/misc_data_frame.py
 src/pymonke/gui/plot/plot_canvas.py
 src/pymonke/gui/plot/plot_frame.py
 src/pymonke/latex/__init__.py
 src/pymonke/latex/tex_table.py
 src/pymonke/latex/utils.py
 src/pymonke/latex/utils.pyi
-src/pymonke/latex/tests/__init__.py
-src/pymonke/latex/tests/table_test.py
 src/pymonke/misc/__init__.py
 src/pymonke/misc/benchmark.py
 src/pymonke/misc/dataframe.py
 src/pymonke/misc/file_management.py
 src/pymonke/misc/pymonke_json_decoder.py
 src/pymonke/misc/pymonke_json_encoder.py
 src/pymonke/mmath/__init__.py
 src/pymonke/mmath/rounding.py
-src/pymonke/mmath/statistics.py
-tests/test.py
+src/pymonke/mmath/statistics.py
```

