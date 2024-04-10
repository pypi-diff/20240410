# Comparing `tmp/unicms_template_unical-1.6.8.tar.gz` & `tmp/unicms_template_unical-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicms_template_unical-1.6.8.tar", last modified: Mon Jan 22 13:24:42 2024, max compression
+gzip compressed data, was "unicms_template_unical-1.6.9.tar", last modified: Tue Jan 23 08:54:48 2024, max compression
```

## Comparing `unicms_template_unical-1.6.8.tar` & `unicms_template_unical-1.6.9.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.594330 unicms_template_unical-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-22 13:24:42.594330 unicms_template_unical-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 13:24:42.594330 unicms_template_unical-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.546331 unicms_template_unical-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.550330 unicms_template_unical-1.6.8/src/unicms_template_unical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.546331 unicms_template_unical-1.6.8/src/unicms_template_unical/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.546331 unicms_template_unical-1.6.8/src/unicms_template_unical/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.550330 unicms_template_unical-1.6.8/src/unicms_template_unical/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    24837 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.546331 unicms_template_unical-1.6.8/src/unicms_template_unical/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.550330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.550330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/colors/
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/colors/unicms_unical.css
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/unicms_exbriner.css
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/unicms_unical.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.550330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    43664 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.558330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/addressbook.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/agenda.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/alert-red.svg
--rw-r--r--   0 runner    (1001) docker     (127)   130694 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/banner_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/chi.png
--rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/en.png
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/esp.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.558330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/favicon/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/favicon/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.562330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/ar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/en.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/es.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/eu.svg
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/fr.svg
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/it.svg
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/pt.svg
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/ru.svg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/zh.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/ita.png
--rw-r--r--   0 runner    (1001) docker     (127)   312996 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/library1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    27664 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_back.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32050 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_presta.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42300 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_unical_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_white.png
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_white_svg.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.570330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (127)  2979589 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/8ayw.png
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/HRS4R.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24514 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/ctc.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25799 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/demacs.svg
--rw-r--r--   0 runner    (1001) docker     (127)    27889 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/desf.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28678 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dfssn.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23742 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/diam.svg
--rw-r--r--   0 runner    (1001) docker     (127)    27886 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dibest.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dices.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28422 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dimeg.svg
--rw-r--r--   0 runner    (1001) docker     (127)    31883 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dinci.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/discag.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25944 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dispes.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/disu.svg
--rw-r--r--   0 runner    (1001) docker     (127)   106385 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/eu_funded.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23410 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/exbriner.png
--rw-r--r--   0 runner    (1001) docker     (127)    20713 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/fis.svg
--rw-r--r--   0 runner    (1001) docker     (127)   473786 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/master_ges.png
--rw-r--r--   0 runner    (1001) docker     (127)   853824 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/sssap.svg
--rw-r--r--   0 runner    (1001) docker     (127)   356948 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/news1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   441153 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/news2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   422058 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/news3.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   126770 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    40246 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical-live.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   508364 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical_banner.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.570330 unicms_template_unical-1.6.8/src/unicms_template_unical/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/js/external_link_new_tab.js
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/static/js/unicms_api_utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.574330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.574330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/base_v_original.html
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/error-page.html
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/unical_api_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    32706 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/unicms_unical.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.586330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_contact.html
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_arrow_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_main.html
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_side.html
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_links.html
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_live.html
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.546331 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.586330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_1/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.586330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_2/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.586330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_3/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.586330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/inits/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/inits/brython-init.html
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/loading-jumbo.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.594330 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/8ayw.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/corsi.html
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department.html
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_ctc.html
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_demacs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_desf.html
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dfssn.html
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_diam.html
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dibest.html
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dices.html
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dimeg.html
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dimes.html
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dinci.html
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_discag.html
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dispes.html
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_disu.html
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_fis.html
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/master_ges.html
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/multi_language.html
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/opendata.html
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/portale_home_v_original.html
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/project_exbriner.html
--rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/publication_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    12207 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/publication_view.html
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/sssap.html
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/unical.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/unical_right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.594330 unicms_template_unical-1.6.8/src/unicms_template_unical/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-01-22 13:24:35.000000 unicms_template_unical-1.6.8/src/unicms_template_unical/templatetags/unicms_template_unical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:24:42.594330 unicms_template_unical-1.6.8/unicms_template_unical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-22 13:24:42.000000 unicms_template_unical-1.6.8/unicms_template_unical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-01-22 13:24:42.000000 unicms_template_unical-1.6.8/unicms_template_unical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 13:24:42.000000 unicms_template_unical-1.6.8/unicms_template_unical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-22 13:24:42.000000 unicms_template_unical-1.6.8/unicms_template_unical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-22 13:24:42.000000 unicms_template_unical-1.6.8/unicms_template_unical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.232833 unicms_template_unical-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-23 08:54:48.232833 unicms_template_unical-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 08:54:48.232833 unicms_template_unical-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.180833 unicms_template_unical-1.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.184833 unicms_template_unical-1.6.9/src/unicms_template_unical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.180833 unicms_template_unical-1.6.9/src/unicms_template_unical/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.180833 unicms_template_unical-1.6.9/src/unicms_template_unical/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.188833 unicms_template_unical-1.6.9/src/unicms_template_unical/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    24837 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.184833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.188833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.188833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/colors/unicms_unical.css
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13343 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/unicms_unical.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.188833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    43664 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.196833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/addressbook.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/agenda.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/alert-red.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   130694 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/banner_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/chi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/en.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/esp.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.196833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/favicon/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/favicon/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.200833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/ar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/en.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/es.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/eu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/it.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/pt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/ru.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/zh.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/ita.png
+-rw-r--r--   0 runner    (1001) docker     (127)   312996 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/library1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    27664 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32050 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_presta.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42300 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_unical_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_white_svg.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.208833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)  2979589 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/8ayw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/HRS4R.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24514 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/ctc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25799 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/demacs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    27889 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/desf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28678 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dfssn.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23742 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/diam.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    27886 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dibest.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dices.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28422 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dimeg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    31883 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dinci.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/discag.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25944 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dispes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/disu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   106385 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/eu_funded.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23410 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/exbriner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20713 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/fis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   473786 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/master_ges.png
+-rw-r--r--   0 runner    (1001) docker     (127)   853824 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/sssap.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   356948 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/news1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   441153 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/news2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   422058 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/news3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   126770 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    40246 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical-live.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   508364 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical_banner.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.208833 unicms_template_unical-1.6.9/src/unicms_template_unical/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/js/external_link_new_tab.js
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/static/js/unicms_api_utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.208833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.212833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/base_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/error-page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/unical_api_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32706 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/unicms_unical.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.224833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_arrow_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_main.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_side.html
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_live.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.184833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.224833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.224833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.224833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_3/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.224833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/inits/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/inits/brython-init.html
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/loading-jumbo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.232833 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/8ayw.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/corsi.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_ctc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_demacs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_desf.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dfssn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_diam.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dibest.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dimeg.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dinci.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_discag.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dispes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_disu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_fis.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/master_ges.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/multi_language.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/opendata.html
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/portale_home_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/project_exbriner.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/publication_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12207 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/publication_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/sssap.html
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/unical.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/unical_right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.232833 unicms_template_unical-1.6.9/src/unicms_template_unical/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-01-23 08:54:41.000000 unicms_template_unical-1.6.9/src/unicms_template_unical/templatetags/unicms_template_unical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:54:48.232833 unicms_template_unical-1.6.9/unicms_template_unical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-23 08:54:48.000000 unicms_template_unical-1.6.9/unicms_template_unical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-01-23 08:54:48.000000 unicms_template_unical-1.6.9/unicms_template_unical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 08:54:48.000000 unicms_template_unical-1.6.9/unicms_template_unical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-23 08:54:48.000000 unicms_template_unical-1.6.9/unicms_template_unical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-23 08:54:48.000000 unicms_template_unical-1.6.9/unicms_template_unical.egg-info/top_level.txt
```

### Comparing `unicms_template_unical-1.6.8/LICENSE` & `unicms_template_unical-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/PKG-INFO` & `unicms_template_unical-1.6.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms_template_unical
-Version: 1.6.8
+Version: 1.6.9
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_unical-1.6.8/setup.py` & `unicms_template_unical-1.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  twine upload dist/*
 
 SRC_FOLDER = 'src'
 PKG_NAME = 'unicms_template_unical'
 
 setup(
     name=PKG_NAME,
-    version='1.6.8',
+    version='1.6.9',
 
     packages=[PKG_NAME],
     package_dir={PKG_NAME: f"{SRC_FOLDER}/{PKG_NAME}"},
 
     package_data={PKG_NAME: [i.replace(f'{SRC_FOLDER}/{PKG_NAME}/', '')
                                    for i in glob(f'{SRC_FOLDER}/{PKG_NAME}/**',
                                                  recursive=True)]
```

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo` & `unicms_template_unical-1.6.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po` & `unicms_template_unical-1.6.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/colors/unicms_exbriner.css` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/colors/unicms_exbriner.css`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/colors/unicms_unical.css` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/colors/unicms_unical.css`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/css/unicms_unical.css` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/css/unicms_unical.css`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 .form-check [type=checkbox]+label, .form-check [type=radio]+label {
   font-size: 1rem;
 }
 
 /** * Header Center Wrapper */
 @media (min-width: 992px) {
   .it-header-center-wrapper {
-    height: 130px;
+    min-height: 130px;
+    height: auto;
   }
 }
 /** * Logo */
 .it-header-center-wrapper .it-header-center-content-wrapper .it-brand-wrapper a .img {
   width: 100%;
 }
 /** * Header Navbar Wrapper */
```

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/addressbook.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/addressbook.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/agenda.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/agenda.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/alert-red.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/alert-red.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/banner_1.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/banner_1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/chi.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/chi.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/dimes.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/en.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/en.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/esp.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/esp.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/ar.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/ar.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/en.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/en.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/es.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/es.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/eu.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/eu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/flags/zh.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/flags/zh.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/ita.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/ita.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/library1.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/library1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo1.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo1.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_back.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_back.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_presta.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_presta.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_unical_white.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_unical_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_white.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_white.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logo_white_svg.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logo_white_svg.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/8ayw.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/8ayw.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/HRS4R.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/HRS4R.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/ctc.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/ctc.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/demacs.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/demacs.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/desf.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/desf.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dfssn.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dfssn.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/diam.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/diam.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dibest.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dibest.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dices.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dices.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dimeg.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dimeg.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dimes.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dinci.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dinci.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/discag.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/discag.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/dispes.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/dispes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/disu.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/disu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/eu_funded.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/eu_funded.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/eu_funded_white.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/eu_funded_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/exbriner.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/exbriner.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/fis.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/fis.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/master_ges.png` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/master_ges.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/logos/sssap.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/logos/sssap.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/news1.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/news1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/news2.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/news2.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/news3.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/news3.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/ponte-bucci-1.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/ponte-bucci-1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical-live.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical-live.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical_banner.jpg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical_banner.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical_logo.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical_logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg` & `unicms_template_unical-1.6.9/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/404.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/404.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/base_v_original.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/base_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/error-page.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/error-page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/unical_api_list.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/unical_api_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/bases/unicms_unical.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/bases/unicms_unical.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_contact.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_contact.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_contact_v2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_contact_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_arrow_icon.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_arrow_icon.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_main.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_main.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_side.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_side.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_alert.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_alert.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_live.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_live.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_card.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_card.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/loading-jumbo.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/loading-jumbo.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/8ayw.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/8ayw.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/corsi.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/corsi.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_ctc.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_ctc.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_demacs.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_demacs.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_desf.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_desf.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dfssn.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dfssn.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_diam.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_diam.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dibest.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dibest.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dices.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dices.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dimeg.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dimeg.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dimes.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dinci.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dinci.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_discag.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_discag.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_dispes.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_dispes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_disu.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_disu.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/department_fis.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/department_fis.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/master_ges.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/master_ges.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/multi_language.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/multi_language.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/opendata.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/opendata.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/portale_home_v_original.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/portale_home_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/project_exbriner.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/project_exbriner.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/publication_list.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/publication_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/publication_view.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/publication_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/publication_view_hero_original.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/publication_view_hero_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templates/pages/sssap.html` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templates/pages/sssap.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/src/unicms_template_unical/templatetags/unicms_template_unical.py` & `unicms_template_unical-1.6.9/src/unicms_template_unical/templatetags/unicms_template_unical.py`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.6.8/unicms_template_unical.egg-info/PKG-INFO` & `unicms_template_unical-1.6.9/unicms_template_unical.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms_template_unical
-Version: 1.6.8
+Version: 1.6.9
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_unical-1.6.8/unicms_template_unical.egg-info/SOURCES.txt` & `unicms_template_unical-1.6.9/unicms_template_unical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

