# Comparing `tmp/solie-8.5.1.tar.gz` & `tmp/solie-8.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solie-8.5.1.tar", max compression
+gzip compressed data, was "solie-8.6.0.tar", max compression
```

## Comparing `solie-8.5.1.tar` & `solie-8.6.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      787 2024-04-06 14:04:14.127818 solie-8.5.1/pyproject.toml
--rw-r--r--   0        0        0     2478 2024-03-09 13:27:55.333963 solie-8.5.1/README.md
--rw-r--r--   0        0        0       65 2024-04-04 12:33:45.799336 solie-8.5.1/solie/__init__.py
--rw-r--r--   0        0        0       85 2024-04-04 12:41:05.189192 solie-8.5.1/solie/__main__.py
--rw-r--r--   0        0        0      363 2024-04-05 00:02:40.054806 solie-8.5.1/solie/common/__init__.py
--rw-r--r--   0        0        0      293 2024-04-04 11:56:27.778407 solie-8.5.1/solie/common/connect_event.py
--rw-r--r--   0        0        0      280 2024-04-05 00:02:06.898492 solie-8.5.1/solie/common/info.py
--rw-r--r--   0        0        0     1259 2024-04-04 12:51:28.608601 solie-8.5.1/solie/common/parallel.py
--rw-r--r--   0        0        0       65 2024-04-04 11:36:05.301867 solie-8.5.1/solie/entry/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-05 11:40:24.240903 solie-8.5.1/solie/entry/lifetime.py
--rw-r--r--   0        0        0      202 2024-04-05 11:30:17.371547 solie-8.5.1/solie/entry/start.py
--rw-r--r--   0        0        0      668 2024-04-03 16:31:10.028573 solie-8.5.1/solie/overlay/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-04 13:05:54.660856 solie-8.5.1/solie/overlay/coin_selection.py
--rw-r--r--   0        0        0     4493 2024-04-04 11:57:06.554716 solie-8.5.1/solie/overlay/datapath_input.py
--rw-r--r--   0        0        0     2203 2024-04-03 16:31:10.033574 solie-8.5.1/solie/overlay/donation_guide.py
--rw-r--r--   0        0        0     2716 2024-04-04 11:58:19.815741 solie-8.5.1/solie/overlay/download_fill_option.py
--rw-r--r--   0        0        0      646 2024-04-03 16:31:10.037100 solie-8.5.1/solie/overlay/long_text_view.py
--rw-r--r--   0        0        0     8055 2024-04-04 11:58:27.486831 solie-8.5.1/solie/overlay/strategy_basic_input.py
--rw-r--r--   0        0        0     6210 2024-04-05 11:56:28.614118 solie-8.5.1/solie/overlay/strategy_develop_input.py
--rw-r--r--   0        0        0     2441 2024-04-03 16:31:10.041098 solie-8.5.1/solie/overlay/strategy_info_view.py
--rw-r--r--   0        0        0     7816 2024-04-04 13:09:54.727633 solie-8.5.1/solie/overlay/token_selection.py
--rw-r--r--   0        0        0    10899 2024-03-09 13:27:55.378483 solie-8.5.1/solie/static/icon/blank_coin.png
--rw-r--r--   0        0        0    11242 2024-03-09 13:27:55.379480 solie-8.5.1/solie/static/icon/traffic_light_green.png
--rw-r--r--   0        0        0    11165 2024-03-09 13:27:55.379480 solie-8.5.1/solie/static/icon/traffic_light_red.png
--rw-r--r--   0        0        0    10810 2024-03-09 13:27:55.380992 solie-8.5.1/solie/static/icon/traffic_light_yellow.png
--rw-r--r--   0        0        0    78060 2024-03-09 13:27:55.382001 solie-8.5.1/solie/static/lexend_bold.ttf
--rw-r--r--   0        0        0   556216 2024-03-09 13:27:55.388006 solie-8.5.1/solie/static/notosans_regular.ttf
--rw-r--r--   0        0        0   228761 2024-03-09 13:27:55.391007 solie-8.5.1/solie/static/product_icon.ico
--rw-r--r--   0        0        0   165542 2024-03-09 13:27:55.393001 solie-8.5.1/solie/static/product_icon.png
--rw-r--r--   0        0        0     1678 2024-03-29 12:50:13.329402 solie-8.5.1/solie/static/sample_decision_script.txt
--rw-r--r--   0        0        0     1015 2024-03-29 12:49:25.127196 solie-8.5.1/solie/static/sample_indicators_script.txt
--rw-r--r--   0        0        0   120456 2024-03-09 13:27:55.396002 solie-8.5.1/solie/static/source_code_pro.ttf
--rw-r--r--   0        0        0     3064 2024-04-06 11:43:43.146126 solie-8.5.1/solie/utility/__init__.py
--rw-r--r--   0        0        0    30449 2024-04-04 11:33:50.635949 solie-8.5.1/solie/utility/analyze_market.py
--rw-r--r--   0        0        0     3599 2024-04-03 16:31:10.045095 solie-8.5.1/solie/utility/api_requester.py
--rw-r--r--   0        0        0     2261 2024-04-04 14:21:39.539090 solie-8.5.1/solie/utility/api_streamer.py
--rw-r--r--   0        0        0     3762 2024-04-03 16:31:10.047095 solie-8.5.1/solie/utility/backward_compatibility.py
--rw-r--r--   0        0        0      379 2024-04-01 16:30:30.467934 solie-8.5.1/solie/utility/ball.py
--rw-r--r--   0        0        0     2238 2024-04-04 12:25:21.345905 solie-8.5.1/solie/utility/check_internet.py
--rw-r--r--   0        0        0      475 2024-04-01 16:30:30.473475 solie-8.5.1/solie/utility/compare_versions.py
--rw-r--r--   0        0        0      624 2024-03-30 00:54:45.144782 solie-8.5.1/solie/utility/convert.py
--rw-r--r--   0        0        0     7329 2024-04-06 10:20:38.815616 solie-8.5.1/solie/utility/download_from_binance.py
--rw-r--r--   0        0        0     2368 2024-04-04 14:26:08.098735 solie-8.5.1/solie/utility/log_handler.py
--rw-r--r--   0        0        0      294 2024-04-03 16:31:10.051094 solie-8.5.1/solie/utility/pandas_related.py
--rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.052097 solie-8.5.1/solie/utility/percent_axis_item.py
--rw-r--r--   0        0        0     8065 2024-04-03 23:15:40.155486 solie-8.5.1/solie/utility/rw_lock.py
--rw-r--r--   0        0        0      251 2024-04-03 16:31:10.055105 solie-8.5.1/solie/utility/simply_format.py
--rw-r--r--   0        0        0      229 2024-04-01 16:30:30.488484 solie-8.5.1/solie/utility/sort_pandas.py
--rw-r--r--   0        0        0     1647 2024-04-03 16:31:10.057101 solie-8.5.1/solie/utility/standardize.py
--rw-r--r--   0        0        0      484 2024-04-03 16:31:10.058095 solie-8.5.1/solie/utility/stop_flag.py
--rw-r--r--   0        0        0     1107 2024-04-03 16:31:10.059097 solie-8.5.1/solie/utility/structs.py
--rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.060102 solie-8.5.1/solie/utility/syntax_highlighter.py
--rw-r--r--   0        0        0     4848 2024-04-04 12:09:23.272841 solie-8.5.1/solie/utility/time_axis_item.py
--rw-r--r--   0        0        0      926 2024-04-06 11:42:39.262331 solie-8.5.1/solie/utility/timing.py
--rw-r--r--   0        0        0     1624 2024-04-03 16:31:10.062097 solie-8.5.1/solie/utility/user_settings.py
--rw-r--r--   0        0        0      813 2024-04-03 17:07:30.543145 solie-8.5.1/solie/widget/__init__.py
--rw-r--r--   0        0        0     5292 2024-04-04 11:59:09.143773 solie-8.5.1/solie/widget/ask_popup.py
--rw-r--r--   0        0        0      312 2024-04-01 14:45:12.996498 solie-8.5.1/solie/widget/brand_label.py
--rw-r--r--   0        0        0      836 2024-04-01 14:45:14.358385 solie-8.5.1/solie/widget/gauge.py
--rw-r--r--   0        0        0      236 2024-04-01 14:45:14.989682 solie-8.5.1/solie/widget/horizontal_divider.py
--rw-r--r--   0        0        0     1922 2024-04-04 11:59:20.593678 solie-8.5.1/solie/widget/log_list.py
--rw-r--r--   0        0        0     4184 2024-04-04 23:30:33.899456 solie-8.5.1/solie/widget/overlay_popup.py
--rw-r--r--   0        0        0       83 2024-04-01 14:45:50.650424 solie-8.5.1/solie/widget/popup_box.py
--rw-r--r--   0        0        0     3202 2024-04-03 16:31:10.068616 solie-8.5.1/solie/widget/script_editor.py
--rw-r--r--   0        0        0     2576 2024-04-03 16:31:10.069616 solie-8.5.1/solie/widget/splash_screen.py
--rw-r--r--   0        0        0       84 2024-04-01 14:04:49.291376 solie-8.5.1/solie/widget/symbol_box.py
--rw-r--r--   0        0        0       98 2024-04-01 14:04:49.292379 solie-8.5.1/solie/widget/transparent_scroll_area.py
--rw-r--r--   0        0        0      233 2024-04-01 14:04:49.293376 solie-8.5.1/solie/widget/vertical_divider.py
--rw-r--r--   0        0        0       50 2024-04-03 16:31:10.070617 solie-8.5.1/solie/window/__init__.py
--rw-r--r--   0        0        0    61287 2024-04-06 01:35:32.018253 solie-8.5.1/solie/window/compiled.py
--rw-r--r--   0        0        0    35529 2024-04-04 14:37:31.636472 solie-8.5.1/solie/window/main.py
--rw-r--r--   0        0        0      319 2024-04-04 11:50:37.144088 solie-8.5.1/solie/worker/__init__.py
--rw-r--r--   0        0        0    32281 2024-04-06 12:49:54.725669 solie-8.5.1/solie/worker/collector.py
--rw-r--r--   0        0        0    12495 2024-04-06 10:12:12.050859 solie-8.5.1/solie/worker/manager.py
--rw-r--r--   0        0        0    59289 2024-04-06 11:46:25.564267 solie-8.5.1/solie/worker/simulator.py
--rw-r--r--   0        0        0    10598 2024-04-04 12:31:28.938266 solie-8.5.1/solie/worker/strategist.py
--rw-r--r--   0        0        0    93922 2024-04-06 14:03:38.138786 solie-8.5.1/solie/worker/transactor.py
--rw-r--r--   0        0        0      695 2024-04-04 11:45:07.528915 solie-8.5.1/solie/worker/united.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 solie-8.5.1/PKG-INFO
+-rw-r--r--   0        0        0      838 2024-04-10 12:20:47.926581 solie-8.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2478 2024-03-09 13:27:55.333963 solie-8.6.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-04 12:33:45.799336 solie-8.6.0/solie/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-04 12:41:05.189192 solie-8.6.0/solie/__main__.py
+-rw-r--r--   0        0        0      363 2024-04-07 13:02:32.985238 solie-8.6.0/solie/common/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-04 11:56:27.778407 solie-8.6.0/solie/common/connect_event.py
+-rw-r--r--   0        0        0      280 2024-04-05 00:02:06.898492 solie-8.6.0/solie/common/info.py
+-rw-r--r--   0        0        0     1259 2024-04-04 12:51:28.608601 solie-8.6.0/solie/common/parallel.py
+-rw-r--r--   0        0        0       65 2024-04-04 11:36:05.301867 solie-8.6.0/solie/entry/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-07 13:02:32.987490 solie-8.6.0/solie/entry/lifetime.py
+-rw-r--r--   0        0        0      202 2024-04-05 11:30:17.371547 solie-8.6.0/solie/entry/start.py
+-rw-r--r--   0        0        0      668 2024-04-03 16:31:10.028573 solie-8.6.0/solie/overlay/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-07 12:14:28.067731 solie-8.6.0/solie/overlay/coin_selection.py
+-rw-r--r--   0        0        0     4493 2024-04-04 11:57:06.554716 solie-8.6.0/solie/overlay/datapath_input.py
+-rw-r--r--   0        0        0     2203 2024-04-03 16:31:10.033574 solie-8.6.0/solie/overlay/donation_guide.py
+-rw-r--r--   0        0        0     2716 2024-04-04 11:58:19.815741 solie-8.6.0/solie/overlay/download_fill_option.py
+-rw-r--r--   0        0        0      646 2024-04-03 16:31:10.037100 solie-8.6.0/solie/overlay/long_text_view.py
+-rw-r--r--   0        0        0     8055 2024-04-06 14:22:24.005864 solie-8.6.0/solie/overlay/strategy_basic_input.py
+-rw-r--r--   0        0        0     6210 2024-04-05 11:56:28.614118 solie-8.6.0/solie/overlay/strategy_develop_input.py
+-rw-r--r--   0        0        0     2441 2024-04-03 16:31:10.041098 solie-8.6.0/solie/overlay/strategy_info_view.py
+-rw-r--r--   0        0        0     7816 2024-04-04 13:09:54.727633 solie-8.6.0/solie/overlay/token_selection.py
+-rw-r--r--   0        0        0    10899 2024-03-09 13:27:55.378483 solie-8.6.0/solie/static/icon/blank_coin.png
+-rw-r--r--   0        0        0    11242 2024-03-09 13:27:55.379480 solie-8.6.0/solie/static/icon/traffic_light_green.png
+-rw-r--r--   0        0        0    11165 2024-03-09 13:27:55.379480 solie-8.6.0/solie/static/icon/traffic_light_red.png
+-rw-r--r--   0        0        0    10810 2024-03-09 13:27:55.380992 solie-8.6.0/solie/static/icon/traffic_light_yellow.png
+-rw-r--r--   0        0        0    78060 2024-03-09 13:27:55.382001 solie-8.6.0/solie/static/lexend_bold.ttf
+-rw-r--r--   0        0        0   556216 2024-03-09 13:27:55.388006 solie-8.6.0/solie/static/notosans_regular.ttf
+-rw-r--r--   0        0        0   228761 2024-03-09 13:27:55.391007 solie-8.6.0/solie/static/product_icon.ico
+-rw-r--r--   0        0        0   165542 2024-03-09 13:27:55.393001 solie-8.6.0/solie/static/product_icon.png
+-rw-r--r--   0        0        0     1678 2024-03-29 12:50:13.329402 solie-8.6.0/solie/static/sample_decision_script.txt
+-rw-r--r--   0        0        0     1015 2024-03-29 12:49:25.127196 solie-8.6.0/solie/static/sample_indicators_script.txt
+-rw-r--r--   0        0        0   120456 2024-03-09 13:27:55.396002 solie-8.6.0/solie/static/source_code_pro.ttf
+-rw-r--r--   0        0        0     3107 2024-04-10 03:50:26.530248 solie-8.6.0/solie/utility/__init__.py
+-rw-r--r--   0        0        0    30449 2024-04-04 11:33:50.635949 solie-8.6.0/solie/utility/analyze_market.py
+-rw-r--r--   0        0        0     3407 2024-04-09 14:53:35.865623 solie-8.6.0/solie/utility/api_requester.py
+-rw-r--r--   0        0        0     2152 2024-04-10 07:29:50.626617 solie-8.6.0/solie/utility/api_streamer.py
+-rw-r--r--   0        0        0     3790 2024-04-08 23:11:18.549232 solie-8.6.0/solie/utility/backward_compatibility.py
+-rw-r--r--   0        0        0      379 2024-04-01 16:30:30.467934 solie-8.6.0/solie/utility/ball.py
+-rw-r--r--   0        0        0     2078 2024-04-10 01:20:20.749960 solie-8.6.0/solie/utility/check_internet.py
+-rw-r--r--   0        0        0      475 2024-04-01 16:30:30.473475 solie-8.6.0/solie/utility/compare_versions.py
+-rw-r--r--   0        0        0      349 2024-04-08 23:14:43.019109 solie-8.6.0/solie/utility/convert.py
+-rw-r--r--   0        0        0     7427 2024-04-10 03:50:13.645081 solie-8.6.0/solie/utility/download_from_binance.py
+-rw-r--r--   0        0        0     2368 2024-04-04 14:26:08.098735 solie-8.6.0/solie/utility/log_handler.py
+-rw-r--r--   0        0        0      294 2024-04-03 16:31:10.051094 solie-8.6.0/solie/utility/pandas_related.py
+-rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.052097 solie-8.6.0/solie/utility/percent_axis_item.py
+-rw-r--r--   0        0        0     8045 2024-04-10 03:01:58.766568 solie-8.6.0/solie/utility/rw_lock.py
+-rw-r--r--   0        0        0      251 2024-04-03 16:31:10.055105 solie-8.6.0/solie/utility/simply_format.py
+-rw-r--r--   0        0        0      229 2024-04-01 16:30:30.488484 solie-8.6.0/solie/utility/sort_pandas.py
+-rw-r--r--   0        0        0     1657 2024-04-10 01:53:24.993795 solie-8.6.0/solie/utility/standardize.py
+-rw-r--r--   0        0        0      484 2024-04-03 16:31:10.058095 solie-8.6.0/solie/utility/stop_flag.py
+-rw-r--r--   0        0        0     1345 2024-04-08 23:20:15.075900 solie-8.6.0/solie/utility/structs.py
+-rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.060102 solie-8.6.0/solie/utility/syntax_highlighter.py
+-rw-r--r--   0        0        0     4848 2024-04-04 12:09:23.272841 solie-8.6.0/solie/utility/time_axis_item.py
+-rw-r--r--   0        0        0      974 2024-04-10 03:50:13.774340 solie-8.6.0/solie/utility/timing.py
+-rw-r--r--   0        0        0     1624 2024-04-03 16:31:10.062097 solie-8.6.0/solie/utility/user_settings.py
+-rw-r--r--   0        0        0      813 2024-04-03 17:07:30.543145 solie-8.6.0/solie/widget/__init__.py
+-rw-r--r--   0        0        0     5292 2024-04-04 11:59:09.143773 solie-8.6.0/solie/widget/ask_popup.py
+-rw-r--r--   0        0        0      312 2024-04-01 14:45:12.996498 solie-8.6.0/solie/widget/brand_label.py
+-rw-r--r--   0        0        0      836 2024-04-01 14:45:14.358385 solie-8.6.0/solie/widget/gauge.py
+-rw-r--r--   0        0        0      236 2024-04-01 14:45:14.989682 solie-8.6.0/solie/widget/horizontal_divider.py
+-rw-r--r--   0        0        0     1922 2024-04-04 11:59:20.593678 solie-8.6.0/solie/widget/log_list.py
+-rw-r--r--   0        0        0     4184 2024-04-04 23:30:33.899456 solie-8.6.0/solie/widget/overlay_popup.py
+-rw-r--r--   0        0        0       83 2024-04-01 14:45:50.650424 solie-8.6.0/solie/widget/popup_box.py
+-rw-r--r--   0        0        0     3202 2024-04-03 16:31:10.068616 solie-8.6.0/solie/widget/script_editor.py
+-rw-r--r--   0        0        0     2576 2024-04-03 16:31:10.069616 solie-8.6.0/solie/widget/splash_screen.py
+-rw-r--r--   0        0        0       84 2024-04-01 14:04:49.291376 solie-8.6.0/solie/widget/symbol_box.py
+-rw-r--r--   0        0        0       98 2024-04-01 14:04:49.292379 solie-8.6.0/solie/widget/transparent_scroll_area.py
+-rw-r--r--   0        0        0      233 2024-04-01 14:04:49.293376 solie-8.6.0/solie/widget/vertical_divider.py
+-rw-r--r--   0        0        0       50 2024-04-03 16:31:10.070617 solie-8.6.0/solie/window/__init__.py
+-rw-r--r--   0        0        0    61287 2024-04-06 01:35:32.018253 solie-8.6.0/solie/window/compiled.py
+-rw-r--r--   0        0        0    35530 2024-04-08 14:41:54.108003 solie-8.6.0/solie/window/main.py
+-rw-r--r--   0        0        0      319 2024-04-04 11:50:37.144088 solie-8.6.0/solie/worker/__init__.py
+-rw-r--r--   0        0        0    32182 2024-04-10 03:50:26.556809 solie-8.6.0/solie/worker/collector.py
+-rw-r--r--   0        0        0    12383 2024-04-08 23:21:25.803158 solie-8.6.0/solie/worker/manager.py
+-rw-r--r--   0        0        0    59263 2024-04-10 03:50:26.558796 solie-8.6.0/solie/worker/simulator.py
+-rw-r--r--   0        0        0    10563 2024-04-08 13:51:16.610473 solie-8.6.0/solie/worker/strategist.py
+-rw-r--r--   0        0        0    95247 2024-04-10 12:02:53.933835 solie-8.6.0/solie/worker/transactor.py
+-rw-r--r--   0        0        0      695 2024-04-04 11:45:07.528915 solie-8.6.0/solie/worker/united.py
+-rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 solie-8.6.0/PKG-INFO
```

### Comparing `solie-8.5.1/pyproject.toml` & `solie-8.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "solie"
-version = "8.5.1"
+version = "8.6.0"
 description = "GUI trading bot designed for targeting the futures markets of Binance"
 authors = ["Cunarist"]
 readme = "README.md"
 repository = "https://github.com/cunarist/solie"
+documentation = "https://solie-docs.cunarist.com"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 numpy = "^1.26.2"
 pandas = "^1.5.3"
 scipy = "^1.11.3"
-pyside6 = "^6.6.0"
+pyside6 = "^6.7.0"
 pyqtgraph = "^0.13.4"
-aiohttp = "^3.8.6"
+aiohttp = "^3.9.3"
 faust-cchardet = "^2.1.19"
 aiodns = "^3.1.1"
 aiofiles = "^23.2.1"
 apscheduler = "^3.10.4"
 pygments = "^2.17.1"
 yapf = "^0.32.0"
 getmac = "^0.8.3"
```

### Comparing `solie-8.5.1/README.md` & `solie-8.6.0/README.md`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/common/parallel.py` & `solie-8.6.0/solie/common/parallel.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/entry/lifetime.py` & `solie-8.6.0/solie/entry/lifetime.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/__init__.py` & `solie-8.6.0/solie/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/coin_selection.py` & `solie-8.6.0/solie/overlay/coin_selection.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/datapath_input.py` & `solie-8.6.0/solie/overlay/datapath_input.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/donation_guide.py` & `solie-8.6.0/solie/overlay/donation_guide.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/download_fill_option.py` & `solie-8.6.0/solie/overlay/download_fill_option.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/long_text_view.py` & `solie-8.6.0/solie/overlay/long_text_view.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/strategy_basic_input.py` & `solie-8.6.0/solie/overlay/strategy_basic_input.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/strategy_develop_input.py` & `solie-8.6.0/solie/overlay/strategy_develop_input.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/strategy_info_view.py` & `solie-8.6.0/solie/overlay/strategy_info_view.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/overlay/token_selection.py` & `solie-8.6.0/solie/overlay/token_selection.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/icon/blank_coin.png` & `solie-8.6.0/solie/static/icon/blank_coin.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/icon/traffic_light_green.png` & `solie-8.6.0/solie/static/icon/traffic_light_green.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/icon/traffic_light_red.png` & `solie-8.6.0/solie/static/icon/traffic_light_red.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/icon/traffic_light_yellow.png` & `solie-8.6.0/solie/static/icon/traffic_light_yellow.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/lexend_bold.ttf` & `solie-8.6.0/solie/static/lexend_bold.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/notosans_regular.ttf` & `solie-8.6.0/solie/static/notosans_regular.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/product_icon.ico` & `solie-8.6.0/solie/static/product_icon.ico`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/product_icon.png` & `solie-8.6.0/solie/static/product_icon.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/sample_decision_script.txt` & `solie-8.6.0/solie/static/sample_decision_script.txt`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/sample_indicators_script.txt` & `solie-8.6.0/solie/static/sample_indicators_script.txt`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/static/source_code_pro.ttf` & `solie-8.6.0/solie/static/source_code_pro.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/utility/__init__.py` & `solie-8.6.0/solie/utility/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     simulate_chunk,
 )
 from .api_requester import ApiRequester, ApiRequestError
 from .api_streamer import ApiStreamer
 from .backward_compatibility import examine_data_files
 from .ball import ball_ceil, ball_floor
 from .check_internet import (
-    add_connected_functions,
-    add_disconnected_functions,
     internet_connected,
     is_internet_checked,
     monitor_internet,
+    when_internet_connected,
+    when_internet_disconnected,
 )
 from .compare_versions import is_left_version_higher
-from .convert import list_to_dict, value_to_indexes
+from .convert import list_to_dict
 from .download_from_binance import (
     DownloadPreset,
     download_aggtrade_data,
     fill_holes_with_aggtrades,
 )
 from .log_handler import LogHandler
 from .pandas_related import combine_candle_data
@@ -35,45 +35,46 @@
     standardize_account_state,
     standardize_asset_record,
     standardize_candle_data,
     standardize_unrealized_changes,
 )
 from .stop_flag import find_stop_flag, make_stop_flag
 from .structs import (
+    BOARD_LOCK_OPTIONS,
+    ManagementSettings,
     SimulationSettings,
     SimulationSummary,
     Strategies,
     Strategy,
     TransactionSettings,
 )
 from .syntax_highlighter import SyntaxHighlighter
 from .time_axis_item import TimeAxisItem
-from .timing import add_task_duration, get_current_moment, get_task_duration
+from .timing import add_task_duration, get_task_duration, to_moment
 from .user_settings import (
     DataSettings,
     read_data_settings,
     read_datapath,
     save_data_settings,
     save_datapath,
 )
 
 __all__ = [
     "ApiRequester",
     "ApiRequestError",
     "ApiStreamer",
     "ball_ceil",
     "ball_floor",
-    "add_connected_functions",
-    "add_disconnected_functions",
+    "when_internet_connected",
+    "when_internet_disconnected",
     "internet_connected",
     "monitor_internet",
     "combine_candle_data",
     "is_left_version_higher",
     "list_to_dict",
-    "value_to_indexes",
     "decide",
     "download_aggtrade_data",
     "examine_data_files",
     "fill_holes_with_aggtrades",
     "LogHandler",
     "make_indicators",
     "PercentAxisItem",
@@ -105,9 +106,11 @@
     "DownloadPreset",
     "CalculationInput",
     "CalculationOutput",
     "simulate_chunk",
     "SimulationError",
     "is_internet_checked",
     "monitor_internet",
-    "get_current_moment",
+    "to_moment",
+    "ManagementSettings",
+    "BOARD_LOCK_OPTIONS",
 ]
```

### Comparing `solie-8.5.1/solie/utility/analyze_market.py` & `solie-8.6.0/solie/utility/analyze_market.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/utility/api_streamer.py` & `solie-8.6.0/solie/utility/api_streamer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import json
 import logging
 from typing import Callable, Coroutine
 
-import aiohttp
+from aiohttp import ClientError, ClientSession, WSMsgType
 
 logger = logging.getLogger(__name__)
 
 
 class ApiStreamError(Exception):
     def __init__(self, received: dict | list):
         formatted = json.dumps(received, indent=2)
@@ -18,46 +18,48 @@
     def __init__(
         self,
         url: str,
         handler: Callable[[dict], Coroutine] | Callable[[list], Coroutine],
     ):
         self._url = url
         self._handler = handler
-        self.session = aiohttp.ClientSession()
+        self._session = ClientSession()
+        self._is_open = True
 
-        if url != "":
-            asyncio.create_task(self._run_websocket())
+        asyncio.create_task(self._keep_connecting())
 
-    def __del__(self):
-        asyncio.create_task(self._close_self())
+    @property
+    def url(self) -> str:
+        return self._url
 
-    async def _run_websocket(self):
-        while True:
+    async def _keep_connecting(self):
+        while self._is_open:
             try:
-                async with self.session.ws_connect(self._url) as websocket:
-                    logger.info(f"Websocket connected: {self._url}")
-                    async for received_raw in websocket:
-                        if received_raw.type in (
-                            aiohttp.WSMsgType.CLOSED,
-                            aiohttp.WSMsgType.ERROR,
-                        ):
-                            logger.info(f"Websocket closed: {self._url}")
-                            break
-                        else:
-                            received = received_raw.json()
-
-                            def done_callback(task: asyncio.Task, received=received):
-                                error = task.exception()
-                                if error:
-                                    raise ApiStreamError(received) from error
-
-                            task = asyncio.create_task(self._handler(received))
-                            task.add_done_callback(done_callback)
-                    logger.info(f"Websocket stopped: {self._url}")
-            except Exception as error:
-                # Handle errors that might occur due to network issues
-                logger.exception(f"Websocket error: {error}")
-                # Wait for a few seconds before attempting to reconnect
-                await asyncio.sleep(5)
-
-    async def _close_self(self):
-        await self.session.close()
+                await self._keep_listening()
+            except ClientError:
+                # This happens when internet is disconnected, etc...
+                pass
+            await asyncio.sleep(5.0)
+
+    async def _keep_listening(self):
+        async with self._session.ws_connect(self._url, heartbeat=5.0) as websocket:
+            logger.info(f"Websocket connected\n{self._url}")
+            async for message in websocket:
+                if message.type == WSMsgType.ERROR:
+                    url = self._url
+                    parsed = json.dumps(message.json(), indent=2)
+                    logger.warning(f"Websocket got an error message\n{url}\n{parsed}")
+                else:
+                    content = message.json()
+
+                    def done_callback(task: asyncio.Task, content=content):
+                        error = task.exception()
+                        if error:
+                            raise ApiStreamError(content) from error
+
+                    task = asyncio.create_task(self._handler(content))
+                    task.add_done_callback(done_callback)
+            logger.info(f"Websocket disconnected\n{self._url}")
+
+    async def close(self):
+        self._is_open = False
+        await self._session.close()
```

### Comparing `solie-8.5.1/solie/utility/backward_compatibility.py` & `solie-8.6.0/solie/utility/backward_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             automation_settings["strategy_index"] = 0
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
             content = json.dumps(automation_settings, indent=2)
             await file.write(content)
     except Exception:
         pass
 
-    # 6.3: Auto_trade and manual_trade
+    # 6.3: Possible causes are now `auto_trade` and `manual_trade`
     try:
         filepath = datapath / "transactor" / "asset_record.pickle"
         asset_record: pd.DataFrame = await go(pd.read_pickle, filepath)
         asset_record["Cause"] = asset_record["Cause"].replace("trade", "auto_trade")
         await go(asset_record.to_pickle, filepath)
     except Exception:
         pass
```

### Comparing `solie-8.5.1/solie/utility/check_internet.py` & `solie-8.6.0/solie/utility/check_internet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 import asyncio
 import logging
 from typing import Callable, Coroutine
 
-import aiohttp
+from aiohttp import ClientSession
 
 logger = logging.getLogger(__name__)
 
+
+ATTEMPT_IP = [
+    "1.0.0.1",  # Cloudflare
+    "1.1.1.1",  # Cloudflare
+    "208.67.222.222",  # OpenDNS
+    "208.67.220.220",  # OpenDNS
+]
+
+is_connected = False
 is_internet_checked = asyncio.Event()
-was_connected = False
+
 connected_functions: list[Callable[[], Coroutine]] = []
 disconnected_functions: list[Callable[[], Coroutine]] = []
 
 
 def internet_connected():
     if is_internet_checked.is_set():
-        return was_connected
+        return is_connected
     else:
         raise RuntimeError("Internet connection is not being monitored")
 
 
 async def monitor_internet():
-    global was_connected
+    global is_connected
     while True:
-        # try to connect to DNS servers
-        attempt_ips = [
-            "1.0.0.1",  # Cloudflare
-            "1.1.1.1",  # Cloudflare
-            "8.8.4.4",  # Google
-            "8.8.8.8",  # Google
-            "9.9.9.9",  # Quad9
-            "149.112.112.112",  # Quad9
-            "208.67.222.222",  # OpenDNS
-            "208.67.220.220",  # OpenDNS
-        ]
-        is_connected = False
-        async with aiohttp.ClientSession() as session:
-            for attempt_ip in attempt_ips:
+        # Try to connect to DNS servers and analyze internet connection
+        was_connected = is_connected
+        analyzed = False
+        async with ClientSession() as session:
+            for attempt_ip in ATTEMPT_IP:
                 try:
                     async with session.get(f"http://{attempt_ip}") as response:
                         if response.status == 200:
-                            is_connected = True
+                            analyzed = True
                             break
                 except Exception:
                     pass
+        is_connected = analyzed
+        is_internet_checked.set()
 
-        # detect changes
+        # Detect changes
         if was_connected and not is_connected:
             for job in disconnected_functions:
                 asyncio.create_task(job())
             logger.warning("Internet disconnected")
         elif not was_connected and is_connected:
             for job in connected_functions:
                 asyncio.create_task(job())
             logger.info("Internet connected")
 
-        # remember connection state
-        was_connected = is_connected
-        is_internet_checked.set()
-
-        # wait for a while
+        # Wait for a while
         await asyncio.sleep(1)
 
 
-def add_connected_functions(job: Callable[[], Coroutine]):
+def when_internet_connected(job: Callable[[], Coroutine]):
     global connected_functions
     connected_functions.append(job)
 
 
-def add_disconnected_functions(job: Callable[[], Coroutine]):
+def when_internet_disconnected(job: Callable[[], Coroutine]):
     global disconnected_functions
     disconnected_functions.append(job)
```

### Comparing `solie-8.5.1/solie/utility/download_from_binance.py` & `solie-8.6.0/solie/utility/download_from_binance.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from urllib.request import urlopen
 
 import numpy as np
 import pandas as pd
 
+from .timing import to_moment
+
 
 @dataclass
 class DownloadPreset:
     symbol: str
     unit_size: str  # "daily" or "monthly"
     year: int
     month: int
@@ -141,24 +143,25 @@
     recent_candle_data: pd.DataFrame,
     aggtrades: pd.DataFrame,
     moment_to_fill_from: datetime,
     last_fetched_time: datetime,
 ) -> pd.DataFrame:
     fill_moment = moment_to_fill_from
 
-    while fill_moment < last_fetched_time - timedelta(seconds=10):
+    last_fetched_moment = to_moment(last_fetched_time)
+    while fill_moment < last_fetched_moment:
         block_start = fill_moment
         block_end = fill_moment + timedelta(seconds=10)
 
-        aggtrade_prices = []
-        aggtrade_volumes = []
+        aggtrade_prices: list[float] = []
+        aggtrade_volumes: list[float] = []
         for _, aggtrade in sorted(aggtrades.items()):
             # sorted by time
             aggtrade_time = datetime.fromtimestamp(
-                aggtrade["T"] / 1000, tz=timezone.utc
+                int(aggtrade["T"]) / 1000, tz=timezone.utc
             )
             if block_start <= aggtrade_time < block_end:
                 aggtrade_prices.append(float(aggtrade["p"]))
                 aggtrade_volumes.append(float(aggtrade["q"]))
 
         can_write = True
```

### Comparing `solie-8.5.1/solie/utility/log_handler.py` & `solie-8.6.0/solie/utility/log_handler.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/utility/percent_axis_item.py` & `solie-8.6.0/solie/utility/percent_axis_item.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/utility/rw_lock.py` & `solie-8.6.0/solie/utility/rw_lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from asyncio import AbstractEventLoop, Future, Task
 from collections import deque
-from typing import Any, Generic, TypeVar
+from typing import Generic, TypeVar
 
 
 # The internal lock object managing the RWLock state.
 class _RWLockCore:
     _RL = 1
     _WL = 2
 
@@ -13,15 +13,15 @@
         self._do_yield = not fast
         self._loop = loop
         self._read_waiters: deque[Future[None]] = deque()
         self._write_waiters: deque[Future[None]] = deque()
         self._r_state: int = 0
         self._w_state: int = 0
         # tasks will be few, so a list is not inefficient
-        self._owning: list[tuple[Task[Any], int]] = []
+        self._owning: list[tuple[Task, int]] = []
 
     @property
     def r_state(self) -> int:
         return self._r_state
 
     @property
     def w_state(self) -> int:
@@ -154,26 +154,26 @@
                     self._r_state += 1
 
 
 class _ContextManagerMixin:
     def __enter__(self):
         raise RuntimeError('"await" should be used as context manager expression')
 
-    def __exit__(self, *args: Any):
+    def __exit__(self, *args):
         # This must exist because __enter__ exists, even though that
         # always raises; that's how the with-statement works.
         pass  # pragma: no cover
 
     async def __aenter__(self):
         await self.acquire()
         # We have no use for the "as ..."  clause in the with
         # statement for locks.
         return None
 
-    async def __aexit__(self, *args: list[Any]):
+    async def __aexit__(self, *args: list):
         self.release()
 
     async def acquire(self):
         raise NotImplementedError  # pragma: no cover
 
     def release(self):
         raise NotImplementedError  # pragma: no cover
```

### Comparing `solie-8.5.1/solie/utility/standardize.py` & `solie-8.6.0/solie/utility/standardize.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,22 @@
         dtype=np.float32,
         index=pd.DatetimeIndex([], tz="UTC"),
     )
 
 
 def standardize_account_state(target_symbols: list[str]):
     return {
-        "observed_until": datetime.fromtimestamp(0, tz=timezone.utc),
-        "wallet_balance": 1,
+        "observed_until": datetime.fromtimestamp(0.0, tz=timezone.utc),
+        "wallet_balance": 1.0,
         "positions": {
             symbol: {
-                "margin": 0,
+                "margin": 0.0,
                 "direction": "none",
-                "entry_price": 0,
-                "update_time": datetime.fromtimestamp(0, tz=timezone.utc),
+                "entry_price": 0.0,
+                "update_time": datetime.fromtimestamp(0.0, tz=timezone.utc),
             }
             for symbol in target_symbols
         },
         "open_orders": {symbol: {} for symbol in target_symbols},
     }
```

### Comparing `solie-8.5.1/solie/utility/structs.py` & `solie-8.6.0/solie/utility/structs.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,7 +40,21 @@
 
 
 @dataclass
 class SimulationSummary:
     year: int
     strategy_code_name: str
     strategy_version: str
+
+
+BOARD_LOCK_OPTIONS = (
+    "NEVER",
+    "10_SECOND",
+    "1_MINUTE",
+    "10_MINUTE",
+    "1_HOUR",
+)
+
+
+@dataclass
+class ManagementSettings(DataClassJsonMixin):
+    lock_board: str = "NEVER"  # One of `BOARD_LOCK_OPTIONS`
```

### Comparing `solie-8.5.1/solie/utility/syntax_highlighter.py` & `solie-8.6.0/solie/utility/syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/utility/time_axis_item.py` & `solie-8.6.0/solie/utility/time_axis_item.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/utility/timing.py` & `solie-8.6.0/solie/utility/timing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from collections import deque
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 
 task_durations: dict[str, deque[float]] = {
     "add_candle_data": deque(maxlen=360),
     "add_book_tickers": deque(maxlen=1280),
     "add_mark_price": deque(maxlen=10),
     "add_aggregate_trades": deque(maxlen=1280),
     "collector_organize_data": deque(maxlen=60),
     "perform_transaction": deque(maxlen=360),
-    "display_light_transaction_lines": deque(maxlen=60),
     "display_transaction_lines": deque(maxlen=20),
 }
 
 
 def add_task_duration(task_name, duration):
     task_durations[task_name].append(duration)
 
 
 def get_task_duration() -> dict[str, deque[float]]:
     return task_durations
 
 
-def get_current_moment() -> datetime:
-    current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-    current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
-    return current_moment
+def to_moment(exact_time: datetime) -> datetime:
+    """
+    In Solie's terminlogy, moment refers to a time on a 10-second unit.
+    This is because one candlestick holds 10 seconds of information.
+    """
+    moment = exact_time.replace(microsecond=0)
+    moment = moment - timedelta(seconds=moment.second % 10)
+    return moment
```

### Comparing `solie-8.5.1/solie/utility/user_settings.py` & `solie-8.6.0/solie/utility/user_settings.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/__init__.py` & `solie-8.6.0/solie/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/ask_popup.py` & `solie-8.6.0/solie/widget/ask_popup.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/gauge.py` & `solie-8.6.0/solie/widget/gauge.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/log_list.py` & `solie-8.6.0/solie/widget/log_list.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/overlay_popup.py` & `solie-8.6.0/solie/widget/overlay_popup.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/script_editor.py` & `solie-8.6.0/solie/widget/script_editor.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/widget/splash_screen.py` & `solie-8.6.0/solie/widget/splash_screen.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/window/compiled.py` & `solie-8.6.0/solie/window/compiled.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/solie/window/main.py` & `solie-8.6.0/solie/window/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
         asyncio.create_task(monitor_internet())
         await is_internet_checked.wait()
         while not internet_connected():
             await ask(
                 "No internet connection",
                 "Internet connection is necessary for Solie to start up.",
-                ["Okay"],
+                ["Retry"],
             )
             await asyncio.sleep(1)
 
         # ■■■■■ Get datapath ■■■■■
 
         datapath = await read_datapath()
```

### Comparing `solie-8.5.1/solie/worker/collector.py` & `solie-8.6.0/solie/worker/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 from solie.common import go, outsource
 from solie.overlay import DonationGuide, DownloadFillOption
 from solie.utility import (
     ApiRequester,
     ApiStreamer,
     DownloadPreset,
     RWLock,
-    add_disconnected_functions,
     add_task_duration,
     combine_candle_data,
     download_aggtrade_data,
     fill_holes_with_aggtrades,
     find_stop_flag,
     format_numeric,
-    get_current_moment,
     internet_connected,
     make_stop_flag,
     sort_data_frame,
     standardize_candle_data,
+    to_moment,
+    when_internet_disconnected,
 )
 from solie.widget import overlay
 from solie.window import Window
 
 from .united import team
 
 logger = logging.getLogger(__name__)
@@ -48,15 +48,15 @@
         self.window = window
         self.scheduler = scheduler
         self.workerpath = window.datapath / "collector"
 
         # ■■■■■ internal memory ■■■■■
 
         self.price_precisions: dict[str, int] = {}  # Symbol and decimal places
-        self.markets_gone: list[str] = []  # Symbols
+        self.markets_gone: set[str] = set()  # Symbols
 
         # ■■■■■ remember and display ■■■■■
 
         self.api_requester = ApiRequester()
 
         self.aggtrade_candle_sizes = {}
         for symbol in window.data_settings.target_symbols:
@@ -122,35 +122,37 @@
             self.save_candle_data,
             trigger="cron",
             hour="*",
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
-        self.api_streamers = {
-            "MARK_PRICE": ApiStreamer(
-                "wss://fstream.binance.com/ws/!markPrice@arr@1s",
-                self.add_mark_price,
-            ),
-        }
-        for symbol in self.window.data_settings.target_symbols:
-            api_streamer = ApiStreamer(
-                f"wss://fstream.binance.com/ws/{symbol.lower()}@bookTicker",
+        self.mark_price_streamer = ApiStreamer(
+            "wss://fstream.binance.com/ws/!markPrice@arr@1s",
+            self.add_mark_price,
+        )
+
+        self.book_ticker_streamers = [
+            ApiStreamer(
+                f"wss://fstream.binance.com/ws/{s.lower()}@bookTicker",
                 self.add_book_tickers,
             )
-            self.api_streamers[f"BOOK_TICKER_{symbol}"] = api_streamer
-            api_streamer = ApiStreamer(
-                f"wss://fstream.binance.com/ws/{symbol.lower()}@aggTrade",
+            for s in self.window.data_settings.target_symbols
+        ]
+        self.aggtrade_streamers = [
+            ApiStreamer(
+                f"wss://fstream.binance.com/ws/{s.lower()}@aggTrade",
                 self.add_aggregate_trades,
             )
-            self.api_streamers[f"AGG_TRADE_{symbol}"] = api_streamer
+            for s in self.window.data_settings.target_symbols
+        ]
 
         # ■■■■■ invoked by the internet connection status change ■■■■■
 
-        add_disconnected_functions(self.clear_aggregate_trades)
+        when_internet_disconnected(self.clear_aggregate_trades)
 
         # ■■■■■ connect UI events ■■■■■
 
         job = self.guide_donation
         outsource(window.pushButton_9.clicked, job)
         job = self.download_fill_candle_data
         outsource(window.pushButton_2.clicked, job)
@@ -262,30 +264,30 @@
         # ■■■■■ check internet connection ■■■■■
 
         if not internet_connected():
             return
 
         # ■■■■■ moments ■■■■■
 
-        current_moment = get_current_moment()
+        current_moment = to_moment(datetime.now(timezone.utc))
         split_moment = current_moment - timedelta(days=2)
 
         # ■■■■■ fill holes ■■■■■
 
-        markets_gone = []
-        full_symbols = []
+        full_symbols: set[str] = set()
         request_count = 0
 
         # only the recent part
         async with self.candle_data.read_lock as cell:
             recent_candle_data = cell.data[cell.data.index >= split_moment].copy()
 
         did_fill = False
 
         target_symbols = self.window.data_settings.target_symbols
+        needed_moments = int((86400 - 60) / 10) + 1
         while len(full_symbols) < len(target_symbols) and request_count < 10:
             for symbol in target_symbols:
                 if symbol in full_symbols:
                     continue
 
                 from_moment = current_moment - timedelta(hours=24)
                 until_moment = current_moment - timedelta(minutes=1)
@@ -293,17 +295,17 @@
                 inspect_df: pd.DataFrame = recent_candle_data[symbol][
                     from_moment:until_moment
                 ]  # type:ignore
                 base_index = inspect_df.dropna().index
                 temp_sr = pd.Series(0, index=base_index)
                 written_moments = len(temp_sr)
 
-                if written_moments == (86400 - 60) / 10 + 1:
+                if written_moments == needed_moments:
                     # case when there are no holes
-                    full_symbols.append(symbol)
+                    full_symbols.add(symbol)
                     continue
 
                 if from_moment not in temp_sr.index:
                     temp_sr[from_moment] = np.nan
                 if until_moment not in temp_sr.index:
                     temp_sr[until_moment] = np.nan
                 temp_sr = await go(temp_sr.asfreq, "10S")
@@ -324,19 +326,18 @@
                     response = await self.api_requester.binance(
                         http_method="GET",
                         path="/fapi/v1/aggTrades",
                         payload=payload,
                     )
                     request_count += 1
                     if len(response) == 0:
-                        if symbol not in markets_gone:
-                            markets_gone.append(symbol)
+                        self.markets_gone.add(symbol)
                         break
                     for aggtrade in response:
-                        aggtrade_id = aggtrade["a"]
+                        aggtrade_id = int(aggtrade["a"])
                         aggtrades[aggtrade_id] = aggtrade
                     last_fetched_id = max(aggtrades.keys())
                     last_fetched_time = datetime.fromtimestamp(
                         aggtrades[last_fetched_id]["T"] / 1000, tz=timezone.utc
                     )
 
                 recent_candle_data = await go(
@@ -345,16 +346,14 @@
                     recent_candle_data,
                     aggtrades,
                     moment_to_fill_from,
                     last_fetched_time,
                 )
                 did_fill = True
 
-        self.markets_gone = markets_gone
-
         if not did_fill:
             return
 
         # combine
         async with self.candle_data.write_lock as cell:
             original_candle_data = cell.data[cell.data.index < split_moment]
             # in case the other data is added during the task
@@ -425,34 +424,36 @@
 
             text = ""
             text += f"24h candle data accumulation rate {cumulation_rate * 100:.2f}%"
             text += "  ⦁  "
             text += f"Realtime data length {written_length_text}"
         else:
             markets_gone = self.markets_gone
-            if len(markets_gone) == 1:
-                text = (
-                    f"It seems that {markets_gone[0]} market is removed by Binance."
-                    + " You should make a new data folder."
-                )
-            else:
-                text = (
-                    f"It seems that {', '.join(markets_gone)} markets are removed by Binance."
-                    + " You should make a new data folder."
-                )
+            text = (
+                f"It seems that {', '.join(markets_gone)} markets are removed by Binance."
+                + " You should make a new data folder."
+            )
 
         self.window.label_6.setText(text)
 
     async def check_candle_data_cumulation_rate(self) -> float:
-        current_moment = get_current_moment()
-        count_start_moment = current_moment - timedelta(hours=24)
+        # End slicing at previous moment
+        # because current moment might still be filling.
+        current_moment = to_moment(datetime.now(timezone.utc))
+        count_end_moment = current_moment - timedelta(seconds=10)
+        count_start_moment = count_end_moment - timedelta(hours=24)
+
+        # Pandas dataframe slicing uses inclusive end.
+        count_end_moment -= timedelta(seconds=1)
+
         async with self.candle_data.read_lock as cell:
-            cumulated_moments = len(cell.data[count_start_moment:].dropna())
-        needed_moments = 24 * 60 * 60 / 10
-        cumulation_rate = min(1.0, (cumulated_moments + 2) / needed_moments)
+            cumulated = len(cell.data[count_start_moment:count_end_moment].dropna())
+        needed_moments = 6 * 60 * 24
+        cumulation_rate = cumulated / needed_moments
+
         return cumulation_rate
 
     async def open_binance_data_page(self):
         await go(webbrowser.open, "https://www.binance.com/en/landing/data")
 
     async def download_fill_candle_data(self):
         # ■■■■■ ask filling type ■■■■■
@@ -689,15 +690,15 @@
         add_task_duration("add_aggregate_trades", duration)
 
     async def clear_aggregate_trades(self):
         async with self.aggregate_trades.write_lock as cell:
             cell.data = cell.data[0:0].copy()
 
     async def add_candle_data(self):
-        current_moment = get_current_moment()
+        current_moment = to_moment(datetime.now(timezone.utc))
         before_moment = current_moment - timedelta(seconds=10)
 
         async with self.aggregate_trades.read_lock as cell:
             data_length = len(cell.data)
         if data_length == 0:
             return
```

### Comparing `solie-8.5.1/solie/worker/manager.py` & `solie-8.6.0/solie/worker/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 import asyncio
-import json
 import logging
 import os
 import statistics
 import webbrowser
 from collections import deque
 from datetime import datetime, timedelta, timezone
 
 import aiofiles
 import aiofiles.os
 import time_machine
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from solie.common import PROCESS_COUNT, go, outsource
 from solie.utility import (
+    BOARD_LOCK_OPTIONS,
     ApiRequester,
+    ManagementSettings,
     get_task_duration,
     internet_connected,
     save_datapath,
-    value_to_indexes,
 )
 from solie.widget import ask
 from solie.window import Window
 
 from .united import team
 
-WINDOW_LOCK_OPTIONS = (
-    "NEVER",
-    "10_SECOND",
-    "1_MINUTE",
-    "10_MINUTE",
-    "1_HOUR",
-)
-
 logger = logging.getLogger(__name__)
 
 
 class Manager:
     def __init__(self, window: Window, scheduler: AsyncIOScheduler):
         # ■■■■■ for data management ■■■■■
 
@@ -52,17 +44,15 @@
 
         self.online_status = {
             "ping": 0,
             "server_time_differences": deque(maxlen=60),
         }
         self.binance_limits = {}
 
-        self.settings = {
-            "lock_board": "NEVER",
-        }
+        self.management_settings = ManagementSettings()
 
         time_traveller = time_machine.travel(datetime.now(timezone.utc))
         time_traveller.start()
         self.time_traveller = time_traveller
 
         # ■■■■■ repetitive schedules ■■■■■
 
@@ -90,16 +80,14 @@
             self.check_binance_limits,
             trigger="cron",
             hour="*",
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
-        self.api_streamers = {}
-
         # ■■■■■ invoked by the internet connection status change ■■■■■
 
         # ■■■■■ connect UI events ■■■■■
 
         job = self.run_script
         outsource(window.pushButton.clicked, job)
         job = self.open_datapath
@@ -113,40 +101,39 @@
         job = self.change_settings
         outsource(window.comboBox_3.currentIndexChanged, job)
 
     async def load(self):
         await aiofiles.os.makedirs(self.workerpath, exist_ok=True)
 
         # settings
-        filepath = self.workerpath / "settings.json"
+        filepath = self.workerpath / "management_settings.json"
         if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
                 content = await file.read()
-                self.settings = json.loads(content)
+                self.management_settings = ManagementSettings.from_json(content)
         self.window.comboBox_3.setCurrentIndex(
-            value_to_indexes(WINDOW_LOCK_OPTIONS, self.settings["lock_board"])[0]
+            BOARD_LOCK_OPTIONS.index(self.management_settings.lock_board)
         )
 
         # python script
         filepath = self.workerpath / "python_script.txt"
         if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
                 script = await file.read()
         else:
             script = "from solie.worker import team\n\nlogger.info(team)"
         self.window.plainTextEdit.setPlainText(script)
 
     async def change_settings(self):
         current_index = self.window.comboBox_3.currentIndex()
-        self.settings["lock_board"] = WINDOW_LOCK_OPTIONS[current_index]
+        self.management_settings.lock_board = BOARD_LOCK_OPTIONS[current_index]
 
-        filepath = self.workerpath / "settings.json"
+        filepath = self.workerpath / "management_settings.json"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(self.settings, indent=2)
-            await file.write(content)
+            await file.write(self.management_settings.to_json(indent=2))
 
     async def open_datapath(self):
         await go(os.startfile, self.window.datapath)
 
     async def deselect_log_output(self):
         self.window.listWidget.clearSelection()
 
@@ -317,25 +304,25 @@
         self.window.should_confirm_closing = False
         self.window.close()
 
     async def open_documentation(self):
         await go(webbrowser.open, "https://solie-docs.cunarist.com")
 
     async def lock_board(self):
-        lock_window_setting = self.settings["lock_board"]
+        lock_board = self.management_settings.lock_board
 
-        if lock_window_setting == "NEVER":
+        if lock_board == BOARD_LOCK_OPTIONS[0]:
             return
-        elif lock_window_setting == "10_SECOND":
+        elif lock_board == BOARD_LOCK_OPTIONS[1]:
             wait_time = timedelta(seconds=10)
-        elif lock_window_setting == "1_MINUTE":
+        elif lock_board == BOARD_LOCK_OPTIONS[2]:
             wait_time = timedelta(minutes=1)
-        elif lock_window_setting == "10_MINUTE":
+        elif lock_board == BOARD_LOCK_OPTIONS[3]:
             wait_time = timedelta(minutes=10)
-        elif lock_window_setting == "1_HOUR":
+        elif lock_board == BOARD_LOCK_OPTIONS[4]:
             wait_time = timedelta(hours=1)
         else:
             raise ValueError("Invalid duration value for locking the window")
 
         last_interaction_time = self.window.last_interaction
         if datetime.now(timezone.utc) < last_interaction_time + wait_time:
             return
```

### Comparing `solie-8.5.1/solie/worker/simulator.py` & `solie-8.6.0/solie/worker/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from solie.common import go, outsource, sync_manager
 from solie.utility import (
     CalculationInput,
     RWLock,
     SimulationSettings,
     SimulationSummary,
     find_stop_flag,
-    get_current_moment,
     make_indicators,
     make_stop_flag,
     simulate_chunk,
     sort_data_frame,
     sort_series,
     standardize_account_state,
     standardize_asset_record,
     standardize_unrealized_changes,
+    to_moment,
 )
 from solie.widget import ask
 from solie.window import Window
 
 from .united import team
 
 
@@ -81,16 +81,14 @@
             trigger="cron",
             hour="*",
             kwargs={"periodic": True},
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
-        self.api_streamers = {}
-
         # ■■■■■ invoked by the internet connection status change ■■■■■
 
         # ■■■■■ connect UI events ■■■■■
 
         job = self.display_range_information
         outsource(window.plot_widget_2.sigRangeChanged, job)
         job = self.set_minimum_view_range
@@ -195,15 +193,15 @@
 
         async with team.collector.candle_data.read_lock as cell:
             if len(cell.data) == 0:
                 return
 
         # ■■■■■ wait for the latest data to be added ■■■■■
 
-        current_moment = get_current_moment()
+        current_moment = to_moment(datetime.now(timezone.utc))
         before_moment = current_moment - timedelta(seconds=10)
 
         if periodic:
             for _ in range(50):
                 if find_stop_flag(task_name, task_id):
                     return
                 async with team.collector.candle_data.read_lock as cell:
@@ -988,15 +986,15 @@
         progress_list = sync_manager.list([0])
 
         if should_calculate:
             decision_script = strategy.decision_script
             indicators_script = strategy.indicators_script
 
             # a little more data for generation
-            provide_from = calculate_from - timedelta(days=7)
+            provide_from = calculate_from - timedelta(days=28)
             year_indicators = await go(
                 make_indicators,
                 target_symbols=target_symbols,
                 candle_data=year_candle_data[provide_from:calculate_until],
                 indicators_script=indicators_script,
             )
```

### Comparing `solie-8.5.1/solie/worker/strategist.py` & `solie-8.6.0/solie/worker/strategist.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,14 @@
         self.green_pixmap = QtGui.QPixmap()
         self.green_pixmap.load(str(iconpath / "traffic_light_green.png"))
 
         # ■■■■■ repetitive schedules ■■■■■
 
         # ■■■■■ websocket streamings ■■■■■
 
-        self.api_streamers = {}
-
         # ■■■■■ invoked by the internet connection status change ■■■■■
 
         # ■■■■■ connect UI events ■■■■■
 
         job = self.add_blank_strategy
         outsource(window.pushButton_5.clicked, job)
```

### Comparing `solie-8.5.1/solie/worker/transactor.py` & `solie-8.6.0/solie/worker/transactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,30 @@
 from solie.overlay import LongTextView
 from solie.utility import (
     ApiRequester,
     ApiRequestError,
     ApiStreamer,
     RWLock,
     TransactionSettings,
-    add_connected_functions,
     add_task_duration,
     ball_ceil,
     decide,
     find_stop_flag,
-    get_current_moment,
     internet_connected,
     list_to_dict,
     make_indicators,
     make_stop_flag,
     sort_data_frame,
     sort_series,
     standardize_account_state,
     standardize_asset_record,
     standardize_unrealized_changes,
+    to_moment,
+    when_internet_connected,
+    when_internet_disconnected,
 )
 from solie.widget import ask, overlay
 from solie.window import Window
 
 from .united import team
 
 logger = logging.getLogger(__name__)
@@ -138,27 +139,29 @@
             minute="*",
         )
         self.scheduler.add_job(
             self.save_large_data,
             trigger="cron",
             hour="*",
         )
+        self.scheduler.add_job(
+            self.update_user_data_stream,
+            trigger="cron",
+            hour="*",
+        )
 
         # ■■■■■ websocket streamings ■■■■■
 
-        self.api_streamers = {
-            "ACCOUNT": ApiStreamer(
-                "",
-                self.listen_to_account,
-            )
-        }
+        self.user_data_streamer: ApiStreamer | None = None
 
         # ■■■■■ invoked by the internet connection status change ■■■■■
 
-        add_connected_functions(self.watch_binance)
+        when_internet_connected(self.watch_binance)
+        when_internet_connected(self.update_user_data_stream)
+        when_internet_disconnected(self.update_user_data_stream)
 
         # ■■■■■ connect UI events ■■■■■
 
         # Special widgets
         job = self.display_range_information
         outsource(window.plot_widget.sigRangeChanged, job)
         job = self.set_minimum_view_range
@@ -237,25 +240,28 @@
             self.api_requester.update_keys(
                 read_data.binance_api_key, read_data.binance_api_secret
             )
 
         # unrealized changes
         filepath = self.workerpath / "unrealized_changes.pickle"
         if await aiofiles.os.path.isfile(filepath):
-            self.unrealized_changes = RWLock(await go(pd.read_pickle, filepath))
+            sr: pd.Series = await go(pd.read_pickle, filepath)
+            self.unrealized_changes = RWLock(sr)
 
         # asset record
         filepath = self.workerpath / "asset_record.pickle"
         if await aiofiles.os.path.isfile(filepath):
-            self.asset_record = RWLock(await go(pd.read_pickle, filepath))
+            df: pd.DataFrame = await go(pd.read_pickle, filepath)
+            self.asset_record = RWLock(df)
 
         # auto order record
         filepath = self.workerpath / "auto_order_record.pickle"
         if await aiofiles.os.path.isfile(filepath):
-            self.auto_order_record = RWLock(await go(pd.read_pickle, filepath))
+            df: pd.DataFrame = await go(pd.read_pickle, filepath)
+            self.auto_order_record = RWLock(df)
 
     async def organize_data(self):
         async with self.unrealized_changes.write_lock as cell:
             if not cell.data.index.is_unique:
                 unique_index = cell.data.index.drop_duplicates()
                 cell.data = cell.data.reindex(unique_index)
             if not cell.data.index.is_monotonic_increasing:
@@ -303,115 +309,140 @@
     async def save_scribbles(self):
         filepath = self.workerpath / "scribbles.pickle"
         async with aiofiles.open(filepath, "wb") as file:
             content = pickle.dumps(self.scribbles)
             await file.write(content)
 
     async def update_user_data_stream(self):
+        """
+        Prepares the WebSocket user data stream from Binance,
+        providing updates on account changes and market order results.
+
+        Although rare, the listen key may change over time.
+        Additionally, the Binance API documentation recommends
+        extending the user data stream every hour.
+        Thus, this function should be called periodically to maintain the stream.
+
+        - https://binance-docs.github.io/apidocs/futures/en/#start-user-data-stream-user_stream
+        """
+
+        async def close_stream():
+            if self.user_data_streamer:
+                await self.user_data_streamer.close()
+                self.user_data_streamer = None
+
         if not internet_connected():
+            await close_stream()
             return
 
         try:
-            payload = {}
             response = await self.api_requester.binance(
                 http_method="POST",
                 path="/fapi/v1/listenKey",
-                payload=payload,
             )
         except ApiRequestError:
+            await close_stream()
             return
 
         listen_key = response["listenKey"]
+        new_url = f"wss://fstream.binance.com/ws/{listen_key}"
+
+        if self.user_data_streamer:
+            if new_url == self.user_data_streamer.url:
+                # If the listen key hasn't changed, do nothing.
+                return
+            else:
+                # If the listen key has changed, close the previous session.
+                await self.user_data_streamer.close()
 
-        self.api_streamers["ACCOUNT"] = ApiStreamer(
-            "wss://fstream.binance.com/ws/" + listen_key,
+        self.user_data_streamer = ApiStreamer(
+            new_url,
             self.listen_to_account,
         )
 
     async def listen_to_account(self, received: dict):
         # ■■■■■ default values ■■■■■
 
-        event_type = received["e"]
-        event_timestamp = received["E"] / 1000
+        event_type = str(received["e"])
+        event_timestamp = int(received["E"]) / 1000
         event_time = datetime.fromtimestamp(event_timestamp, tz=timezone.utc)
 
         self.account_state["observed_until"] = event_time
 
         # ■■■■■ do the task according to event type ■■■■■
 
         if event_type == "listenKeyExpired":
-            text = "Binance user data stream listen key got expired"
+            text = "Binance user data stream listen key has expired"
             logger.warning(text)
             await self.update_user_data_stream()
 
-        if event_type == "ACCOUNT_UPDATE":
+        elif event_type == "ACCOUNT_UPDATE":
             about_update = received["a"]
             about_assets = about_update["B"]
             about_positions = about_update["P"]
 
             asset_token = self.window.data_settings.asset_token
 
             about_assets_keyed = list_to_dict(about_assets, "a")
-            if asset_token in about_assets_keyed:
-                about_asset = about_assets_keyed[asset_token]
-                wallet_balance = float(about_asset["wb"])
-                self.wallet_balance_state = wallet_balance
+            about_asset = about_assets_keyed[asset_token]
+            wallet_balance = float(about_asset["wb"])
+            self.account_state["wallet_balance"] = wallet_balance
 
             about_positions_keyed = list_to_dict(about_positions, "ps")
             if "BOTH" in about_positions_keyed:
                 about_position = about_positions_keyed["BOTH"]
 
                 target_symbols = self.window.data_settings.target_symbols
                 if about_position["s"] not in target_symbols:
                     return
 
-                symbol = about_position["s"]
+                symbol = str(about_position["s"])
                 amount = float(about_position["pa"])
                 entry_price = float(about_position["ep"])
 
                 leverage = self.leverages[symbol]
                 margin = abs(amount) * entry_price / leverage
-                if amount < 0:
+                if amount < 0.0:
                     direction = "short"
-                elif amount > 0:
+                elif amount > 0.0:
                     direction = "long"
                 else:
                     direction = "none"
 
                 self.account_state["positions"][symbol]["margin"] = margin
                 self.account_state["positions"][symbol]["direction"] = direction
                 self.account_state["positions"][symbol]["entry_price"] = entry_price
                 self.account_state["positions"][symbol]["update_time"] = event_time
 
-        if event_type == "ORDER_TRADE_UPDATE":
+        elif event_type == "ORDER_TRADE_UPDATE":
             about_update = received["o"]
 
             target_symbols = self.window.data_settings.target_symbols
             if about_update["s"] not in target_symbols:
                 return
 
             # from received
-            symbol = about_update.get("s")
-            order_id = about_update.get("i")
-            order_type = about_update.get("o")
-            order_status = about_update.get("X")
-            execution_type = about_update.get("x")
-
-            side = about_update.get("S")
-            close_position = about_update.get("cp")
-            is_maker = about_update.get("m")
-
-            origianal_quantity = float(about_update.get("q", 0))
-            executed_quantity = float(about_update.get("z", 0))
-            last_filled_quantity = float(about_update.get("l", 0))
-            last_filled_price = float(about_update.get("L", 0))
-            price = float(about_update.get("p", 0))
-            stop_price = float(about_update.get("sp", 0))
-            commission = float(about_update.get("n", 0))
-            realized_profit = float(about_update.get("rp", 0))
+            symbol = str(about_update["s"])
+            order_id = int(about_update["i"])
+            order_type = str(about_update["o"])
+            order_status = str(about_update["X"])
+            execution_type = str(about_update["x"])
+
+            side = str(about_update["S"])
+            close_position = bool(about_update["cp"])
+            is_maker = bool(about_update["m"])
+
+            origianal_quantity = float(about_update["q"])
+            executed_quantity = float(about_update["z"])
+            last_filled_quantity = float(about_update["l"])
+            last_filled_price = float(about_update["L"])
+            price = float(about_update["p"])
+            stop_price = float(about_update["sp"])
+            commission = float(about_update["n"])
+            realized_profit = float(about_update["rp"])
 
             # from remembered
             leverage = self.leverages[symbol]
             wallet_balance = self.account_state["wallet_balance"]
 
             # when the order is removed
             if order_status not in ("NEW", "PARTIALLY_FILLED"):
@@ -499,29 +530,27 @@
                 added_notional = last_filled_price * last_filled_quantity
                 added_margin = added_notional / leverage
                 added_margin_ratio = added_margin / wallet_balance
 
                 async with self.auto_order_record.read_lock as cell:
                     symbol_df = cell.data[cell.data["Symbol"] == symbol]
                     unique_order_ids = symbol_df["Order ID"].unique()
-                    if order_id in unique_order_ids:
-                        mask_sr = symbol_df["Order ID"] == order_id
 
                 async with self.asset_record.write_lock as cell:
                     symbol_df = cell.data[cell.data["Symbol"] == symbol]
                     recorded_id_list = symbol_df["Order ID"].tolist()
                     does_record_exist = order_id in recorded_id_list
                     last_index = cell.data.index[-1]
                     if does_record_exist:
                         mask_sr = symbol_df["Order ID"] == order_id
-                        recorded_time = symbol_df.index[mask_sr][0]
-                        recorded_value = symbol_df.loc[recorded_time, "Margin Ratio"]
-                        new_value = recorded_value + added_margin_ratio
-                        cell.data.loc[recorded_time, "Margin Ratio"] = new_value
-                        last_asset: float = cell.data.loc[last_index, "Result Asset"]  # type:ignore
+                        rec_time = symbol_df.index[mask_sr][0]
+                        rec_value = float(symbol_df.loc[rec_time, "Margin Ratio"])  # type:ignore
+                        new_value = rec_value + added_margin_ratio
+                        cell.data.loc[rec_time, "Margin Ratio"] = new_value
+                        last_asset = float(cell.data.loc[last_index, "Result Asset"])  # type:ignore
                         new_value = last_asset + added_revenue
                         cell.data.loc[last_index, "Result Asset"] = new_value
                     else:
                         record_time = event_time
                         while record_time in cell.data.index:
                             record_time += timedelta(milliseconds=1)
                         new_value = symbol
@@ -532,15 +561,15 @@
                         cell.data.loc[record_time, "Fill Price"] = new_value
                         new_value = "maker" if is_maker else "taker"
                         cell.data.loc[record_time, "Role"] = new_value
                         new_value = added_margin_ratio
                         cell.data.loc[record_time, "Margin Ratio"] = new_value
                         new_value = order_id
                         cell.data.loc[record_time, "Order ID"] = new_value
-                        last_asset: float = cell.data.loc[last_index, "Result Asset"]  # type:ignore
+                        last_asset = float(cell.data.loc[last_index, "Result Asset"])  # type:ignore
                         new_value = last_asset + added_revenue
                         cell.data.loc[record_time, "Result Asset"] = new_value
                         if order_id in unique_order_ids:
                             cell.data.loc[record_time, "Cause"] = "auto_trade"
                         else:
                             cell.data.loc[record_time, "Cause"] = "manual_trade"
                     if not cell.data.index.is_monotonic_increasing:
@@ -734,15 +763,15 @@
 
         async with team.collector.candle_data.read_lock as cell:
             if len(cell.data) == 0:
                 return
 
         # ■■■■■ wait for the latest data to be added ■■■■■
 
-        current_moment = get_current_moment()
+        current_moment = to_moment(datetime.now(timezone.utc))
         before_moment = current_moment - timedelta(seconds=10)
 
         if periodic:
             for _ in range(50):
                 if find_stop_flag(task_name, task_id):
                     return
                 async with team.collector.candle_data.read_lock as cell:
@@ -1309,15 +1338,15 @@
 
         cumulation_rate = await team.collector.check_candle_data_cumulation_rate()
         if cumulation_rate < 1:
             return
 
         # ■■■■■ Moment ■■■■■
 
-        current_moment = get_current_moment()
+        current_moment = to_moment(datetime.now(timezone.utc))
         before_moment = current_moment - timedelta(seconds=10)
 
         # ■■■■■ Play the progress bar ■■■■■
 
         is_cycle_done = False
 
         async def play_progress_bar():
@@ -1467,15 +1496,15 @@
         # ■■■■■ Check internet connection ■■■■■
 
         if not internet_connected():
             return
 
         # ■■■■■ Moment ■■■■■
 
-        current_moment = get_current_moment()
+        current_moment = to_moment(datetime.now(timezone.utc))
         before_moment = current_moment - timedelta(seconds=10)
 
         # ■■■■■ Request exchange information ■■■■■
 
         payload = {}
         response = await self.api_requester.binance(
             http_method="GET",
@@ -1962,15 +1991,16 @@
                         "side": order_side,
                         "quantity": quantity,
                         "reduceOnly": True,
                         "newOrderRespType": "RESULT",
                     }
                     now_orders.append(new_order)
                 else:
-                    logger.warn("Cannot close position when there isn't any")
+                    text = "Cannot close position when there isn't any"
+                    logger.warning(text)
 
             if "now_buy" in decision[symbol]:
                 command = decision[symbol]["now_buy"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 quantity = min(maximum_quantity, notional / current_price)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
@@ -2097,15 +2127,16 @@
                         "type": order_type,
                         "side": order_side,
                         "stopPrice": round(float(command["boundary"]), price_precision),
                         "closePosition": True,
                     }
                     later_orders.append(new_order)
                 else:
-                    logger.warn("Cannot place `later_up_close` with no open position")
+                    text = "Cannot place `later_up_close` with no open position"
+                    logger.warning(text)
 
             if "later_down_close" in decision[symbol]:
                 command = decision[symbol]["later_down_close"]
                 if current_direction in ("long", "short"):
                     if current_direction == "long":
                         order_side = "SELL"
                         order_type = "STOP_MARKET"
@@ -2118,15 +2149,16 @@
                         "type": order_type,
                         "side": order_side,
                         "stopPrice": round(float(command["boundary"]), price_precision),
                         "closePosition": True,
                     }
                     later_orders.append(new_order)
                 else:
-                    logger.warn("Cannot place `later_down_close` with no open position")
+                    text = "Cannot place `later_down_close` with no open position"
+                    logger.warning(text)
 
             if "later_up_buy" in decision[symbol]:
                 command = decision[symbol]["later_up_buy"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
```

### Comparing `solie-8.5.1/solie/worker/united.py` & `solie-8.6.0/solie/worker/united.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.1/PKG-INFO` & `solie-8.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: solie
-Version: 8.5.1
+Version: 8.6.0
 Summary: GUI trading bot designed for targeting the futures markets of Binance
 Home-page: https://github.com/cunarist/solie
 Author: Cunarist
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiodns (>=3.1.1,<4.0.0)
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
-Requires-Dist: aiohttp (>=3.8.6,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: faust-cchardet (>=2.1.19,<3.0.0)
 Requires-Dist: getmac (>=0.8.3,<0.9.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: pygments (>=2.17.1,<3.0.0)
 Requires-Dist: pyqtgraph (>=0.13.4,<0.14.0)
-Requires-Dist: pyside6 (>=6.6.0,<7.0.0)
+Requires-Dist: pyside6 (>=6.7.0,<7.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: time-machine (>=2.13.0,<3.0.0)
 Requires-Dist: xdialog (>=1.1.1,<2.0.0)
 Requires-Dist: yapf (>=0.32.0,<0.33.0)
+Project-URL: Documentation, https://solie-docs.cunarist.com
 Project-URL: Repository, https://github.com/cunarist/solie
 Description-Content-Type: text/markdown
 
 # Solie
 
 [![PyPI - Python Version](https://img.shields.io/pypi/v/solie)](https://pypi.org/project/solie/)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
```

