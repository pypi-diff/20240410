# Comparing `tmp/perun.proxygui-3.5.1.tar.gz` & `tmp/perun.proxygui-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxygui-3.5.1.tar", last modified: Mon Mar 18 23:20:41 2024, max compression
+gzip compressed data, was "perun.proxygui-4.0.0.tar", last modified: Wed Apr 10 13:33:08 2024, max compression
```

## Comparing `perun.proxygui-3.5.1.tar` & `perun.proxygui-4.0.0.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.610792 perun.proxygui-3.5.1/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/LICENSE
--rw-rw-rw-   0     1001 root         (0)       46 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/MANIFEST.in
--rw-r--r--   0     1001 root         (0)     9393 2024-03-18 23:20:41.610792 perun.proxygui-3.5.1/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)     8072 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.546793 perun.proxygui-3.5.1/perun/proxygui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.546793 perun.proxygui-3.5.1/perun/proxygui/api/
--rw-rw-rw-   0     1001 root         (0)        0 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/api/__init__.py
--rw-rw-rw-   0     1001 root         (0)     2389 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/api/backchannel_logout_api.py
--rw-rw-rw-   0     1001 root         (0)     4476 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/api/ban_api.py
--rw-rw-rw-   0     1001 root         (0)     4825 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/api/consent_api.py
--rw-rw-rw-   0     1001 root         (0)    10175 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/api/heuristic_api.py
--rw-rw-rw-   0     1001 root         (0)     3037 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/api/kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)     6008 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/app.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.546793 perun.proxygui-3.5.1/perun/proxygui/gui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/__init__.py
--rw-rw-rw-   0     1001 root         (0)    19806 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/gui.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.546793 perun.proxygui-3.5.1/perun/proxygui/gui/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.538793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.538793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.550793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.550793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
--rw-rw-rw-   0     1001 root         (0)   141520 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)       99 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
--rw-rw-rw-   0     1001 root         (0)      612 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
--rw-rw-rw-   0     1001 root         (0)       67 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.550793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
--rw-rw-rw-   0     1001 root         (0)      688 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
--rw-rw-rw-   0     1001 root         (0)       19 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)      949 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
--rw-rw-rw-   0     1001 root         (0)     1663 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.550793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
--rw-rw-rw-   0     1001 root         (0)      477 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.538793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.550793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
--rw-rw-rw-   0     1001 root         (0)      631 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
--rw-rw-rw-   0     1001 root         (0)     1451 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)     3089 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
--rw-rw-rw-   0     1001 root         (0)     1617 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
--rw-rw-rw-   0     1001 root         (0)     1776 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
--rw-rw-rw-   0     1001 root         (0)      437 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
--rw-rw-rw-   0     1001 root         (0)      387 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
--rw-rw-rw-   0     1001 root         (0)     2945 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
--rw-rw-rw-   0     1001 root         (0)     2624 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
--rw-rw-rw-   0     1001 root         (0)      713 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
--rw-rw-rw-   0     1001 root         (0)     1899 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.554793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
--rw-rw-rw-   0     1001 root         (0)      815 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
--rw-rw-rw-   0     1001 root         (0)      571 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.554793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
--rw-rw-rw-   0     1001 root         (0)      421 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
--rw-rw-rw-   0     1001 root         (0)      403 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
--rw-rw-rw-   0     1001 root         (0)     2758 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.554793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
--rw-rw-rw-   0     1001 root         (0)      198 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
--rw-rw-rw-   0     1001 root         (0)      684 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
--rw-rw-rw-   0     1001 root         (0)    29997 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
--rw-rw-rw-   0     1001 root         (0)      244 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.538793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.558793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
--rw-rw-rw-   0     1001 root         (0)    22637 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
--rw-rw-rw-   0     1001 root         (0)    21057 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
--rw-rw-rw-   0     1001 root         (0)    22481 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
--rw-rw-rw-   0     1001 root         (0)    35533 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
--rw-rw-rw-   0     1001 root         (0)    34805 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
--rw-rw-rw-   0     1001 root         (0)    28733 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
--rw-rw-rw-   0     1001 root         (0)    20267 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28025 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
--rw-rw-rw-   0     1001 root         (0)    25884 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
--rw-rw-rw-   0     1001 root         (0)   363233 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
--rw-rw-rw-   0     1001 root         (0)    27013 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
--rw-rw-rw-   0     1001 root         (0)    33321 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
--rw-rw-rw-   0     1001 root         (0)    31511 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
--rw-rw-rw-   0     1001 root         (0)    34010 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28152 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
--rw-rw-rw-   0     1001 root         (0)    36726 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
--rw-rw-rw-   0     1001 root         (0)    28663 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
--rw-rw-rw-   0     1001 root         (0)    22030 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.562793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.578793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/
--rw-rw-rw-   0     1001 root         (0)   125046 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
--rw-rw-rw-   0     1001 root         (0)   252563 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
--rw-rw-rw-   0     1001 root         (0)  1052500 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
--rw-rw-rw-   0     1001 root         (0)  1125125 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
--rw-rw-rw-   0     1001 root         (0)  1125144 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
--rw-rw-rw-   0     1001 root         (0)  1125123 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
--rw-rw-rw-   0     1001 root         (0)  1125119 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
--rw-rw-rw-   0     1001 root         (0)  1125120 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
--rw-rw-rw-   0     1001 root         (0)  1125147 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
--rw-rw-rw-   0     1001 root         (0)  1125545 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
--rw-rw-rw-   0     1001 root         (0)  1126098 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)   139176 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
--rw-rw-rw-   0     1001 root         (0)     2596 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css
--rw-rw-rw-   0     1001 root         (0)    48080 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/print.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.582793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/
--rw-rw-rw-   0     1001 root         (0)     2596 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
--rw-rw-rw-   0     1001 root         (0)    46987 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
--rw-rw-rw-   0     1001 root         (0)   303728 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   332353 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   332557 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
--rw-rw-rw-   0     1001 root         (0)     5778 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
--rw-rw-rw-   0     1001 root         (0)   312236 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   341456 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   341664 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style.css
--rw-rw-rw-   0     1001 root         (0)     5772 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.586793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/
--rw-rw-rw-   0     1001 root         (0)    87048 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    74284 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)   208892 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
--rw-rw-rw-   0     1001 root         (0)   159376 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
--rw-rw-rw-   0     1001 root         (0)     1632 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
--rw-rw-rw-   0     1001 root         (0)     1837 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
--rw-rw-rw-   0     1001 root         (0)     1484 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
--rw-rw-rw-   0     1001 root         (0)      988 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
--rw-rw-rw-   0     1001 root         (0)    12252 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
--rw-rw-rw-   0     1001 root         (0)     9596 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.586793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.590793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/
--rw-rw-rw-   0     1001 root         (0)    70841 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
--rw-rw-rw-   0     1001 root         (0)     4348 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
--rw-rw-rw-   0     1001 root         (0)      151 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
--rw-rw-rw-   0     1001 root         (0)      281 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
--rw-rw-rw-   0     1001 root         (0)      149 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
--rw-rw-rw-   0     1001 root         (0)      304 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
--rw-rw-rw-   0     1001 root         (0)     7406 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
--rw-rw-rw-   0     1001 root         (0)     4426 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
--rw-rw-rw-   0     1001 root         (0)      443 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/logo.svg
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.590793 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/
--rw-rw-rw-   0     1001 root         (0)   218591 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/app.js
--rw-rw-rw-   0     1001 root         (0)   659454 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map
--rw-rw-rw-   0     1001 root         (0)   337945 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/d3.js
--rw-rw-rw-   0     1001 root         (0)     2707 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js
--rw-rw-rw-   0     1001 root         (0)     8806 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js
--rw-rw-rw-   0     1001 root         (0)    26171 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
--rw-rw-rw-   0     1001 root         (0)     4075 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
--rw-rw-rw-   0     1001 root         (0)   284394 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js
--rw-rw-rw-   0     1001 root         (0)   610160 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.594793 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/css/
--rw-rw-rw-   0     1001 root         (0)   155845 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0     1001 root         (0)   431289 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.594793 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/js/
--rw-rw-rw-   0     1001 root         (0)    78743 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0     1001 root         (0)   325834 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0     1001 root         (0)       78 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/campus-idp-muni.js
--rw-rw-rw-   0     1001 root         (0)     7336 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/campus-idp.css
--rw-rw-rw-   0     1001 root         (0)     4859 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/campus-idp.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.594793 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/css/
--rw-rw-rw-   0     1001 root         (0)    73577 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/css/all.css
--rw-rw-rw-   0     1001 root         (0)    59305 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/css/all.min.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.598793 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/
--rw-rw-rw-   0     1001 root         (0)   134294 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0     1001 root         (0)   747927 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0     1001 root         (0)   133988 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0     1001 root         (0)    89988 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    76736 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)    34034 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0     1001 root         (0)   144714 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0     1001 root         (0)    33736 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0     1001 root         (0)    16276 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0     1001 root         (0)    13224 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0     1001 root         (0)   203030 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0     1001 root         (0)   918991 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0     1001 root         (0)   202744 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0     1001 root         (0)   101648 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0     1001 root         (0)    78268 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.602793 perun.proxygui-3.5.1/perun/proxygui/gui/static/images/
--rw-rw-rw-   0     1001 root         (0)      490 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/images/check.svg
--rw-rw-rw-   0     1001 root         (0)      536 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/images/circle-check-regular.svg
--rw-rw-rw-   0     1001 root         (0)      483 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
--rw-rw-rw-   0     1001 root         (0)      730 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/images/questionmark.svg
--rw-rw-rw-   0     1001 root         (0)      625 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/images/spinner.svg
--rw-rw-rw-   0     1001 root         (0)    89501 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/jquery-3.6.0.min.js
--rw-rw-rw-   0     1001 root         (0)      627 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/proxygui.css
--rw-rw-rw-   0     1001 root         (0)     1427 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/proxygui.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.602793 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/
--rw-rw-rw-   0     1001 root         (0)    15836 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
--rw-rw-rw-   0     1001 root         (0)     8266 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
--rw-rw-rw-   0     1001 root         (0)     8862 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
--rw-rw-rw-   0     1001 root         (0)     8873 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
--rw-rw-rw-   0     1001 root         (0)     7692 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.css
--rw-rw-rw-   0     1001 root         (0)     8344 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.default.css
--rw-rw-rw-   0     1001 root         (0)    11438 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/js/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.602793 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/js/standalone/
--rw-rw-rw-   0     1001 root         (0)    64906 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.606793 perun.proxygui-3.5.1/perun/proxygui/gui/templates/
--rw-rw-rw-   0     1001 root         (0)    15205 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/ConsentRegistration.html
--rw-rw-rw-   0     1001 root         (0)     9047 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/HeuristicData.html
--rw-rw-rw-   0     1001 root         (0)      747 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/IsTestingSP.html
--rw-rw-rw-   0     1001 root         (0)     3091 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/Logout.html
--rw-rw-rw-   0     1001 root         (0)     1131 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResetEmailSent.html
--rw-rw-rw-   0     1001 root         (0)     1942 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResetInitiated.html
--rw-rw-rw-   0     1001 root         (0)     1133 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
--rw-rw-rw-   0     1001 root         (0)     1021 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResult.html
--rw-rw-rw-   0     1001 root         (0)      795 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/MissingAuth.html
--rw-rw-rw-   0     1001 root         (0)     1019 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/OidcError.html
--rw-rw-rw-   0     1001 root         (0)     1223 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/Post-logout.html
--rw-rw-rw-   0     1001 root         (0)      907 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/SPAuthorization.html
--rw-rw-rw-   0     1001 root         (0)     2490 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/_footer.html
--rw-rw-rw-   0     1001 root         (0)     8103 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/_header.html
--rw-rw-rw-   0     1001 root         (0)     1175 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/authorization.html
--rw-rw-rw-   0     1001 root         (0)     3477 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/base.html
--rw-rw-rw-   0     1001 root         (0)      561 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/logout-iframe.html
--rw-rw-rw-   0     1001 root         (0)     3769 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/templates/logout-state.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/proxygui/gui/translations/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun/proxygui/gui/translations/cs/
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.606793 perun.proxygui-3.5.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/
--rw-rw-rw-   0     1001 root         (0)     2973 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-rw-   0     1001 root         (0)     8108 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
--rw-rw-rw-   0     1001 root         (0)     5372 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/jwt.py
--rw-rw-rw-   0     1001 root         (0)    19923 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/logout_manager.py
--rw-rw-rw-   0     1001 root         (0)     2480 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/oauth.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.606793 perun.proxygui-3.5.1/perun/proxygui/openapi/
--rw-rw-rw-   0     1001 root         (0)     6107 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/openapi/openapi.py
--rw-rw-rw-   0     1001 root         (0)    12933 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/openapi/openapi_data.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.606793 perun.proxygui-3.5.1/perun/proxygui/openapi/schemas/
--rw-rw-rw-   0     1001 root         (0)      997 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/openapi/schemas/arguments_schemas.py
--rw-rw-rw-   0     1001 root         (0)     1446 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/openapi/schemas/response_schemas.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.606793 perun.proxygui-3.5.1/perun/proxygui/tests/
--rw-rw-rw-   0     1001 root         (0)        0 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1816 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/shared_test_data.py
--rw-rw-rw-   0     1001 root         (0)     6908 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/test_ban_api.py
--rw-rw-rw-   0     1001 root         (0)     6635 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/test_consent_api.py
--rw-rw-rw-   0     1001 root         (0)     4713 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/test_consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2160 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/test_consent_request_db.py
--rw-rw-rw-   0     1001 root         (0)     6788 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/test_gui.py
--rw-rw-rw-   0     1001 root         (0)     1111 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/tests/test_kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)    20143 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/proxygui/user_manager.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.610792 perun.proxygui-3.5.1/perun/utils/
--rw-rw-rw-   0     1001 root         (0)     2496 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/ConfigStore.py
--rw-rw-rw-   0     1001 root         (0)       43 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/CustomExceptions.py
--rw-rw-rw-   0     1001 root         (0)     2555 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/CustomRPHandler.py
--rw-rw-rw-   0     1001 root         (0)      489 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/DatabaseService.py
--rw-rw-rw-   0     1001 root         (0)     4414 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/EmailService.py
--rw-rw-rw-   0     1001 root         (0)       96 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/Notification.py
--rw-rw-rw-   0     1001 root         (0)      816 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/Utils.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.610792 perun.proxygui-3.5.1/perun/utils/consent_framework/
--rw-rw-rw-   0     1001 root         (0)     1241 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/consent_framework/consent.py
--rw-rw-rw-   0     1001 root         (0)     2226 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/consent_framework/consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2274 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/consent_framework/consent_manager.py
--rw-rw-rw-   0     1001 root         (0)      730 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/consent_framework/consent_request.py
--rw-rw-rw-   0     1001 root         (0)     1371 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/consent_framework/consent_request_db.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.610792 perun.proxygui-3.5.1/perun/utils/logout_requests/
--rw-rw-rw-   0     1001 root         (0)     2001 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/logout_requests/BackchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)      832 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     3841 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/logout_requests/GraphLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     1361 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/logout_requests/LogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     2229 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/perun/utils/logout_requests/SamlLogoutRequest.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-03-18 23:20:41.542793 perun.proxygui-3.5.1/perun.proxygui.egg-info/
--rw-r--r--   0     1001 root         (0)     9393 2024-03-18 23:20:41.000000 perun.proxygui-3.5.1/perun.proxygui.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)    12784 2024-03-18 23:20:41.000000 perun.proxygui-3.5.1/perun.proxygui.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-03-18 23:20:41.000000 perun.proxygui-3.5.1/perun.proxygui.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      584 2024-03-18 23:20:41.000000 perun.proxygui-3.5.1/perun.proxygui.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)        6 2024-03-18 23:20:41.000000 perun.proxygui-3.5.1/perun.proxygui.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-03-18 23:20:41.610792 perun.proxygui-3.5.1/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1523 2024-03-18 23:20:08.000000 perun.proxygui-3.5.1/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.011754 perun.proxygui-4.0.0/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       46 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)     9393 2024-04-10 13:33:08.011754 perun.proxygui-4.0.0/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)     8072 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/proxygui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.935755 perun.proxygui-4.0.0/perun/proxygui/api/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/api/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     2389 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/api/backchannel_logout_api.py
+-rw-rw-rw-   0     1001 root         (0)     4476 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/api/ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     4825 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/api/consent_api.py
+-rw-rw-rw-   0     1001 root         (0)    10175 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/api/heuristic_api.py
+-rw-rw-rw-   0     1001 root         (0)     3037 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/api/kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)     6008 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/app.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.935755 perun.proxygui-4.0.0/perun/proxygui/gui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    19806 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/gui.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.935755 perun.proxygui-4.0.0/perun/proxygui/gui/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.927755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.927755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.935755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.935755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   141520 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)       99 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
+-rw-rw-rw-   0     1001 root         (0)      612 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
+-rw-rw-rw-   0     1001 root         (0)       67 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.939755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
+-rw-rw-rw-   0     1001 root         (0)      688 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
+-rw-rw-rw-   0     1001 root         (0)       19 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)      949 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
+-rw-rw-rw-   0     1001 root         (0)     1663 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.939755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
+-rw-rw-rw-   0     1001 root         (0)      477 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.927755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.939755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
+-rw-rw-rw-   0     1001 root         (0)      631 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
+-rw-rw-rw-   0     1001 root         (0)     1451 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
+-rw-rw-rw-   0     1001 root         (0)     1617 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
+-rw-rw-rw-   0     1001 root         (0)     1776 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
+-rw-rw-rw-   0     1001 root         (0)      437 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
+-rw-rw-rw-   0     1001 root         (0)      387 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
+-rw-rw-rw-   0     1001 root         (0)     2945 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
+-rw-rw-rw-   0     1001 root         (0)     2624 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
+-rw-rw-rw-   0     1001 root         (0)      713 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
+-rw-rw-rw-   0     1001 root         (0)     1899 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.939755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
+-rw-rw-rw-   0     1001 root         (0)      815 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
+-rw-rw-rw-   0     1001 root         (0)      571 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.939755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
+-rw-rw-rw-   0     1001 root         (0)      421 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
+-rw-rw-rw-   0     1001 root         (0)      403 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
+-rw-rw-rw-   0     1001 root         (0)     2758 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.939755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
+-rw-rw-rw-   0     1001 root         (0)      198 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
+-rw-rw-rw-   0     1001 root         (0)      684 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
+-rw-rw-rw-   0     1001 root         (0)    29997 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
+-rw-rw-rw-   0     1001 root         (0)      244 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.927755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.943755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
+-rw-rw-rw-   0     1001 root         (0)    22637 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    21057 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    22481 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
+-rw-rw-rw-   0     1001 root         (0)    35533 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    34805 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    28733 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    20267 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28025 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    25884 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
+-rw-rw-rw-   0     1001 root         (0)   363233 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
+-rw-rw-rw-   0     1001 root         (0)    27013 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    33321 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    31511 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    34010 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28152 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    36726 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
+-rw-rw-rw-   0     1001 root         (0)    28663 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
+-rw-rw-rw-   0     1001 root         (0)    22030 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.951755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.971755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   125046 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
+-rw-rw-rw-   0     1001 root         (0)   252563 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
+-rw-rw-rw-   0     1001 root         (0)  1052500 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125125 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125144 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125123 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125119 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125120 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125147 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125545 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
+-rw-rw-rw-   0     1001 root         (0)  1126098 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)   139176 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    48080 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.979755 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    46987 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
+-rw-rw-rw-   0     1001 root         (0)   303728 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   332353 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   332557 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
+-rw-rw-rw-   0     1001 root         (0)     5778 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
+-rw-rw-rw-   0     1001 root         (0)   312236 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   341456 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   341664 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css
+-rw-rw-rw-   0     1001 root         (0)     5772 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.983754 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/
+-rw-rw-rw-   0     1001 root         (0)    87048 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    74284 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   208892 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
+-rw-rw-rw-   0     1001 root         (0)   159376 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
+-rw-rw-rw-   0     1001 root         (0)     1632 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
+-rw-rw-rw-   0     1001 root         (0)     1837 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
+-rw-rw-rw-   0     1001 root         (0)     1484 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
+-rw-rw-rw-   0     1001 root         (0)      988 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
+-rw-rw-rw-   0     1001 root         (0)    12252 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
+-rw-rw-rw-   0     1001 root         (0)     9596 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.983754 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.987754 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/
+-rw-rw-rw-   0     1001 root         (0)    70841 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
+-rw-rw-rw-   0     1001 root         (0)     4348 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
+-rw-rw-rw-   0     1001 root         (0)      151 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
+-rw-rw-rw-   0     1001 root         (0)      281 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
+-rw-rw-rw-   0     1001 root         (0)      149 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
+-rw-rw-rw-   0     1001 root         (0)      304 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
+-rw-rw-rw-   0     1001 root         (0)     7406 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
+-rw-rw-rw-   0     1001 root         (0)     4426 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
+-rw-rw-rw-   0     1001 root         (0)      443 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/logo.svg
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.991754 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/
+-rw-rw-rw-   0     1001 root         (0)   218591 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js
+-rw-rw-rw-   0     1001 root         (0)   659454 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map
+-rw-rw-rw-   0     1001 root         (0)   337945 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js
+-rw-rw-rw-   0     1001 root         (0)     2707 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js
+-rw-rw-rw-   0     1001 root         (0)     8806 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js
+-rw-rw-rw-   0     1001 root         (0)    26171 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
+-rw-rw-rw-   0     1001 root         (0)     4075 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
+-rw-rw-rw-   0     1001 root         (0)   284394 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js
+-rw-rw-rw-   0     1001 root         (0)   610160 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.927755 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.991754 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/css/
+-rw-rw-rw-   0     1001 root         (0)   155845 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0     1001 root         (0)   431289 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.991754 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/js/
+-rw-rw-rw-   0     1001 root         (0)    78743 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0     1001 root         (0)   325834 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0     1001 root         (0)       78 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/campus-idp-muni.js
+-rw-rw-rw-   0     1001 root         (0)     7336 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/campus-idp.css
+-rw-rw-rw-   0     1001 root         (0)     4859 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/campus-idp.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.991754 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/css/
+-rw-rw-rw-   0     1001 root         (0)    73577 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/css/all.css
+-rw-rw-rw-   0     1001 root         (0)    59305 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.999755 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/
+-rw-rw-rw-   0     1001 root         (0)   134294 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0     1001 root         (0)   747927 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0     1001 root         (0)   133988 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    89988 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    76736 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)    34034 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0     1001 root         (0)   144714 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0     1001 root         (0)    33736 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    16276 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0     1001 root         (0)    13224 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   203030 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0     1001 root         (0)   918991 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0     1001 root         (0)   202744 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0     1001 root         (0)   101648 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0     1001 root         (0)    78268 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.999755 perun.proxygui-4.0.0/perun/proxygui/gui/static/images/
+-rw-rw-rw-   0     1001 root         (0)      490 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/images/check.svg
+-rw-rw-rw-   0     1001 root         (0)      536 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg
+-rw-rw-rw-   0     1001 root         (0)      483 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
+-rw-rw-rw-   0     1001 root         (0)      730 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/images/questionmark.svg
+-rw-rw-rw-   0     1001 root         (0)      625 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/images/spinner.svg
+-rw-rw-rw-   0     1001 root         (0)    89501 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js
+-rw-rw-rw-   0     1001 root         (0)      627 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/proxygui.css
+-rw-rw-rw-   0     1001 root         (0)     1427 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/proxygui.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.003754 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/
+-rw-rw-rw-   0     1001 root         (0)    15836 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
+-rw-rw-rw-   0     1001 root         (0)     8266 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
+-rw-rw-rw-   0     1001 root         (0)     8862 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
+-rw-rw-rw-   0     1001 root         (0)     8873 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
+-rw-rw-rw-   0     1001 root         (0)     7692 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.css
+-rw-rw-rw-   0     1001 root         (0)     8344 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css
+-rw-rw-rw-   0     1001 root         (0)    11438 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/js/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.003754 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/js/standalone/
+-rw-rw-rw-   0     1001 root         (0)    64906 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.003754 perun.proxygui-4.0.0/perun/proxygui/gui/templates/
+-rw-rw-rw-   0     1001 root         (0)    15205 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/ConsentRegistration.html
+-rw-rw-rw-   0     1001 root         (0)     9047 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/HeuristicData.html
+-rw-rw-rw-   0     1001 root         (0)      747 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/IsTestingSP.html
+-rw-rw-rw-   0     1001 root         (0)     3091 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/Logout.html
+-rw-rw-rw-   0     1001 root         (0)     1131 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html
+-rw-rw-rw-   0     1001 root         (0)     1942 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html
+-rw-rw-rw-   0     1001 root         (0)     1133 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
+-rw-rw-rw-   0     1001 root         (0)     1021 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResult.html
+-rw-rw-rw-   0     1001 root         (0)      795 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/MissingAuth.html
+-rw-rw-rw-   0     1001 root         (0)     1019 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/OidcError.html
+-rw-rw-rw-   0     1001 root         (0)     1223 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/Post-logout.html
+-rw-rw-rw-   0     1001 root         (0)      907 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/SPAuthorization.html
+-rw-rw-rw-   0     1001 root         (0)     2490 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/_footer.html
+-rw-rw-rw-   0     1001 root         (0)     8103 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/_header.html
+-rw-rw-rw-   0     1001 root         (0)     1175 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/authorization.html
+-rw-rw-rw-   0     1001 root         (0)     3477 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)      561 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/logout-iframe.html
+-rw-rw-rw-   0     1001 root         (0)     3769 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/templates/logout-state.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/proxygui/gui/translations/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun/proxygui/gui/translations/cs/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.003754 perun.proxygui-4.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/
+-rw-rw-rw-   0     1001 root         (0)     2973 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0     1001 root         (0)     8108 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
+-rw-rw-rw-   0     1001 root         (0)     5372 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/jwt.py
+-rw-rw-rw-   0     1001 root         (0)    20220 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/logout_manager.py
+-rw-rw-rw-   0     1001 root         (0)     2480 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/oauth.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.003754 perun.proxygui-4.0.0/perun/proxygui/openapi/
+-rw-rw-rw-   0     1001 root         (0)     6107 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/openapi/openapi.py
+-rw-rw-rw-   0     1001 root         (0)    12933 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/openapi/openapi_data.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.007754 perun.proxygui-4.0.0/perun/proxygui/openapi/schemas/
+-rw-rw-rw-   0     1001 root         (0)      997 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py
+-rw-rw-rw-   0     1001 root         (0)     1446 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/openapi/schemas/response_schemas.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.007754 perun.proxygui-4.0.0/perun/proxygui/tests/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1816 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/shared_test_data.py
+-rw-rw-rw-   0     1001 root         (0)     6409 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/test_ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     6635 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/test_consent_api.py
+-rw-rw-rw-   0     1001 root         (0)     4713 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/test_consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2160 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/test_consent_request_db.py
+-rw-rw-rw-   0     1001 root         (0)     6826 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/test_gui.py
+-rw-rw-rw-   0     1001 root         (0)     1111 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/tests/test_kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)    21910 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/proxygui/user_manager.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.007754 perun.proxygui-4.0.0/perun/utils/
+-rw-rw-rw-   0     1001 root         (0)     2496 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/ConfigStore.py
+-rw-rw-rw-   0     1001 root         (0)       43 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/CustomExceptions.py
+-rw-rw-rw-   0     1001 root         (0)     2555 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/CustomRPHandler.py
+-rw-rw-rw-   0     1001 root         (0)     1354 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/DatabaseService.py
+-rw-rw-rw-   0     1001 root         (0)     4414 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/EmailService.py
+-rw-rw-rw-   0     1001 root         (0)       96 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/Notification.py
+-rw-rw-rw-   0     1001 root         (0)      816 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/Utils.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.007754 perun.proxygui-4.0.0/perun/utils/consent_framework/
+-rw-rw-rw-   0     1001 root         (0)     1241 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/consent_framework/consent.py
+-rw-rw-rw-   0     1001 root         (0)     2226 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/consent_framework/consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2274 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/consent_framework/consent_manager.py
+-rw-rw-rw-   0     1001 root         (0)      730 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/consent_framework/consent_request.py
+-rw-rw-rw-   0     1001 root         (0)     1371 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/consent_framework/consent_request_db.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:08.007754 perun.proxygui-4.0.0/perun/utils/logout_requests/
+-rw-rw-rw-   0     1001 root         (0)     2001 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)      832 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     3841 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/logout_requests/GraphLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     1361 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/logout_requests/LogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     2229 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/perun/utils/logout_requests/SamlLogoutRequest.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-10 13:33:07.931755 perun.proxygui-4.0.0/perun.proxygui.egg-info/
+-rw-r--r--   0     1001 root         (0)     9393 2024-04-10 13:33:07.000000 perun.proxygui-4.0.0/perun.proxygui.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)    12784 2024-04-10 13:33:07.000000 perun.proxygui-4.0.0/perun.proxygui.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-04-10 13:33:07.000000 perun.proxygui-4.0.0/perun.proxygui.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      584 2024-04-10 13:33:07.000000 perun.proxygui-4.0.0/perun.proxygui.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)        6 2024-04-10 13:33:07.000000 perun.proxygui-4.0.0/perun.proxygui.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-04-10 13:33:08.011754 perun.proxygui-4.0.0/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1523 2024-04-10 13:32:36.000000 perun.proxygui-4.0.0/setup.py
```

### Comparing `perun.proxygui-3.5.1/LICENSE` & `perun.proxygui-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/PKG-INFO` & `perun.proxygui-4.0.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 3.5.1
+Version: 4.0.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
```

### Comparing `perun.proxygui-3.5.1/README.md` & `perun.proxygui-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/api/backchannel_logout_api.py` & `perun.proxygui-4.0.0/perun/proxygui/api/backchannel_logout_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/api/ban_api.py` & `perun.proxygui-4.0.0/perun/proxygui/api/ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/api/consent_api.py` & `perun.proxygui-4.0.0/perun/proxygui/api/consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/api/heuristic_api.py` & `perun.proxygui-4.0.0/perun/proxygui/api/heuristic_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/api/kerberos_auth_api.py` & `perun.proxygui-4.0.0/perun/proxygui/api/kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/app.py` & `perun.proxygui-4.0.0/perun/proxygui/app.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/gui.py` & `perun.proxygui-4.0.0/perun/proxygui/gui/gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/print.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/style.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/app.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/d3.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/campus-idp.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/campus-idp.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/campus-idp.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/campus-idp.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/css/all.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/css/all.min.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/images/circle-check-regular.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/images/questionmark.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/images/questionmark.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/images/spinner.svg` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/images/spinner.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/jquery-3.6.0.min.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/proxygui.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/proxygui.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/proxygui.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/proxygui.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.default.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js` & `perun.proxygui-4.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/ConsentRegistration.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/ConsentRegistration.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/HeuristicData.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/HeuristicData.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/IsTestingSP.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/IsTestingSP.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/Logout.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/Logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResetEmailSent.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResetInitiated.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/MfaResult.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/MfaResult.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/MissingAuth.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/MissingAuth.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/OidcError.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/OidcError.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/Post-logout.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/Post-logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/SPAuthorization.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/SPAuthorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/_footer.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/_header.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/_header.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/authorization.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/authorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/base.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/logout-iframe.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/logout-iframe.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/templates/logout-state.html` & `perun.proxygui-4.0.0/perun/proxygui/gui/templates/logout-state.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo` & `perun.proxygui-4.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po` & `perun.proxygui-4.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/jwt.py` & `perun.proxygui-4.0.0/perun/proxygui/jwt.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/logout_manager.py` & `perun.proxygui-4.0.0/perun/proxygui/logout_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import copy
+import json
 from datetime import datetime
+from typing import Union
 
 import requests
 from perun.connector import Logger
 from saml2 import samlp
 from saml2.mdstore import MetadataStore
 from saml2.s_utils import UnsupportedBinding
 from saml2.server import Server
+from sqlalchemy import select
 
 from perun.proxygui import jwt
 from perun.proxygui.jwt import JWTServiceProvider
 from perun.proxygui.user_manager import UserManager
 from perun.utils import Utils
 from perun.utils.CustomExceptions import InvalidJWTError
+from perun.utils.DatabaseService import DatabaseService
 from perun.utils.logout_requests.BackchannelLogoutRequest import (
     BackchannelLogoutRequest,
 )
 from perun.utils.logout_requests.FrontchannelLogoutRequest import (
     FrontchannelLogoutRequest,
 )
 from perun.utils.logout_requests.GraphLogoutRequest import GraphLogoutRequest
@@ -25,31 +29,19 @@
 
 SAML_REDIRECT_BINDING = "urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect"
 
 
 class LogoutManager:
     def __init__(self, cfg):
         self.user_manager = UserManager(cfg)
+        self.db_service = DatabaseService(cfg)
         self.logger = Logger.get_logger(__name__)
         self._cfg = cfg
         self.services_configuration = self.fetch_services_configuration()
 
-    def session_exists(self, ss_sid, is_ss_session):
-        ssp_sessions_collection = Utils.get_mongo_db_collection(
-            "ssp_database", self._cfg
-        )
-        if is_ss_session:
-            entries = ssp_sessions_collection.count_documents(
-                {"type": "session", "key": ss_sid}
-            )
-        else:
-            entries = 0
-
-        return entries > 0
-
     def validate_request_and_extract_params(self, ssp_key, request):
         logout_methods = [
             self._resolve_rp_initiated_logout_request,
             self._resolve_saml_initiated_logout_request,
             self._resolve_rp_initiated_alternative_logout_request,
         ]
 
@@ -193,41 +185,49 @@
 
         entry = satosa_sessions_collection.find_one(
             {"client_id": client_id, "claims.ssp_session_id": ssp_sid},
             {"sid_encrypted": 1},
         )
         return entry.get("sid_encrypted") if entry else None
 
-    def _get_rp_sid_from_sspid_ssp(self, client_id, ssp_sid):
-        ssp_sessions_collection = Utils.get_mongo_db_collection(
-            "ssp_database", self._cfg
+    def _get_rp_sid_from_sspid_ssp(self, client_id, ssp_sid) -> Union[str, None]:
+        ssp_engine = self.db_service.get_postgres_engine("ssp_database")
+        sessions_table_name = self._cfg["ssp_database"]["sessions_table_name"]
+        ssp_sessions_table = self.db_service.get_postgres_table(
+            ssp_engine, sessions_table_name
         )
+
         current_datetime = datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
-        entries = ssp_sessions_collection.find(
-            {
-                "$or": [
-                    {
-                        "$and": [
-                            {"type": "session"},
-                            {"key": ssp_sid},
-                            {"expire": {"$gt": current_datetime}},
-                        ]
-                    },
-                    {"$and": [{"type": "session"}, {"key": ssp_sid}, {"expire": None}]},
-                ]
-            },
-            {"session_indexes_detail": 1, "_id": 0},
-        )
-
-        for entry in entries:
-            session_details = entry.get("session_indexes_detail", {})
-            for issuer, data in session_details.items():
-                for sp, sid in data.items():
-                    if sp == client_id:
-                        return sid
+        with ssp_engine.begin() as conn:
+            query = select(ssp_sessions_table.c.session_indexes_detail).where(
+                (
+                    (
+                        (ssp_sessions_table.c._type == "session")
+                        & (ssp_sessions_table.c._key == ssp_sid)
+                        & (
+                            (ssp_sessions_table.c._expire > current_datetime)
+                            | (ssp_sessions_table.c._expire is None)
+                        )
+                    )
+                    | (
+                        (ssp_sessions_table.c._type == "session")
+                        & (ssp_sessions_table.c._key == ssp_sid)
+                        & (ssp_sessions_table.c._expire is None)
+                    )
+                )
+            )
+
+            result = conn.execute(query)
+            entries = result.fetchall()
+            for entry in entries:
+                session_details = json.loads(entry[0])
+                for issuer, data in session_details.items():
+                    for sp, sid in data.items():
+                        if sp == client_id:
+                            return sid
         return None
 
     def _is_redirect_uri_registered(self, client_id, post_logout_redirect_uri):
         client_config = self.services_configuration.get("RPS").get(client_id)
         if client_config:
             allowed_redirect_uris = client_config.get("POST_LOGOUT_REDIRECT_URIS", [])
             return post_logout_redirect_uri in allowed_redirect_uris
```

### Comparing `perun.proxygui-3.5.1/perun/proxygui/oauth.py` & `perun.proxygui-4.0.0/perun/proxygui/oauth.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/openapi/openapi.py` & `perun.proxygui-4.0.0/perun/proxygui/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/openapi/openapi_data.py` & `perun.proxygui-4.0.0/perun/proxygui/openapi/openapi_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/openapi/schemas/arguments_schemas.py` & `perun.proxygui-4.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/openapi/schemas/response_schemas.py` & `perun.proxygui-4.0.0/perun/proxygui/openapi/schemas/response_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/shared_test_data.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/shared_test_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/test_ban_api.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/test_ban_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import copy
 import gzip
 import io
 import json
+import mongomock
 import tarfile
 from http import HTTPStatus
-from unittest.mock import patch
-
-import mongomock
-
 from perun.proxygui.tests.shared_test_data import SHARED_TESTING_CONFIG, client
-
+from unittest.mock import patch
 
 # prevent client from being "unused" during static code analysis, it is injected to
 # the tests upon launch
 _ = client
 
 BAN_IN_DB_1 = {
     "description": None,
@@ -53,21 +50,14 @@
 BANS_NOT_IN_DB = [BAN_NOT_IN_DB_1, BAN_NOT_IN_DB_2]
 
 for ban in BANS_IN_DB:
     BAN_COLLECTION.insert_one(copy.deepcopy(ban))
 
 BANNED_SUBJECT = "banned_subject"
 ALLOWED_SUBJECT = "allowed_subject"
-SSP_SESSIONS_COLLECTION = MOCK_CLIENT["ssp_database"]["ssp_collection"]
-SSP_SESSIONS = [
-    {"user": BANNED_SUBJECT, "session_data": "1"},
-    {"user": BANNED_SUBJECT, "session_data": "2"},
-    {"user": ALLOWED_SUBJECT, "session_data": "1"},
-    {"user": ALLOWED_SUBJECT, "session_data": "2"},
-]
 
 SATOSA_SESSIONS_COLLECTION = MOCK_CLIENT["satosa_database"]["ssp_collection"]
 SATOSA_SESSIONS = [
     {"sub": BANNED_SUBJECT, "session_data": "1"},
     {"sub": BANNED_SUBJECT, "session_data": "2"},
     {"sub": ALLOWED_SUBJECT, "session_data": "1"},
     {"sub": ALLOWED_SUBJECT, "session_data": "2"},
@@ -117,29 +107,28 @@
 
     assert BAN_COLLECTION.count_documents({}) == number_of_bans_in_db
 
 
 @patch("perun.proxygui.user_manager.UserManager._delete_mitre_tokens")
 @patch("perun.proxygui.api.ban_api.get_ban_collection")
 @patch("perun.proxygui.user_manager.UserManager._get_satosa_sessions_collection")
-@patch("perun.proxygui.user_manager.UserManager._get_ssp_sessions_collection")
+@patch("perun.proxygui.user_manager.UserManager.logout")
 @patch("perun.connector.AdaptersManager.get_user_attributes")
 def test_ban_user_add_new_bans(
     mock_get_user_attributes,
-    mock_get_ssp_collection,
+    mock_logout,
     mock_get_satosa_collection,
     mock_get_ban_collection,
     mock_delete_mitre_tokens,
     client,
 ):
     mock_delete_mitre_tokens.return_value = 0
     mock_get_user_attributes.return_value = {
         SHARED_TESTING_CONFIG["perun_person_principal_names_attribute"]: BANNED_SUBJECT
     }
-    mock_get_ssp_collection.return_value = SSP_SESSIONS_COLLECTION
     mock_get_satosa_collection.return_value = SATOSA_SESSIONS_COLLECTION
     mock_get_ban_collection.return_value = BAN_COLLECTION
 
     all_user_bans = {ban["userId"]: ban for ban in BANS_IN_DB + BANS_NOT_IN_DB}
     number_of_bans_in_db = len(BANS_IN_DB)
     number_of_bans_not_in_db = len(BANS_NOT_IN_DB)
 
@@ -150,18 +139,16 @@
     assert (
         BAN_COLLECTION.count_documents({})
         == number_of_bans_in_db + number_of_bans_not_in_db
     )
     for ban in BANS_IN_DB + BANS_NOT_IN_DB:
         assert BAN_COLLECTION.find_one({"id": ban["id"]}) is not None
 
-    assert SSP_SESSIONS_COLLECTION.count_documents(
-        {}
-    ) == SSP_SESSIONS_COLLECTION.count_documents({"user": ALLOWED_SUBJECT})
-    assert SSP_SESSIONS_COLLECTION.find_one({"user": BANNED_SUBJECT}) is None
+    for ban in BANS_NOT_IN_DB:
+        mock_logout.assert_any_call(user_id=ban["userId"], include_refresh_tokens=True)
 
     assert SATOSA_SESSIONS_COLLECTION.count_documents(
         {}
     ) == SATOSA_SESSIONS_COLLECTION.count_documents({"sub": ALLOWED_SUBJECT})
     assert SATOSA_SESSIONS_COLLECTION.find_one({"sub": BANNED_SUBJECT}) is None
```

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/test_consent_api.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/test_consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/test_consent_db.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/test_consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/test_consent_request_db.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/test_consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/test_gui.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/test_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+import pytest
 import re
 import tempfile
-from unittest.mock import patch
-
-import pytest
 from flask_session import Session
-
 from perun.proxygui.app import get_flask_app
 from perun.proxygui.tests.shared_test_data import (
     SHARED_TESTING_CONFIG,
     OIDCAuthenticationMock,
 )
 from perun.utils.ConfigStore import ConfigStore
+from unittest.mock import patch
 
 MOCK_SESSIONS = [
     ("client_1", "session_id_1", "issuer_1"),
     ("client_2", "session_id_2", "issuer_2"),
 ]
 MOCK_SERVICE_NAMES = {"client_1": {"en": "Client 1"}, "client_2": {"en": "Client 2"}}
 MOCK_SERVICES_CONFIG = {
@@ -113,15 +111,15 @@
     cookies_missing = "cookies are missing"
     assert cookies_missing in result
 
 
 def test_logout_overview(client):
     with patch(
         "perun.proxygui.user_manager.UserManager._get_ssp_session_by_key",
-        return_value={"user": 123},
+        return_value={"eduperson_principal_name": 123},
     ), patch(
         "perun.proxygui.user_manager.UserManager.get_active_client_ids_for_user",
         return_value=MOCK_SESSIONS,
     ), patch(
         "perun.proxygui.user_manager.UserManager.get_active_client_ids_for_session",
         return_value=[MOCK_SESSIONS[0]],
     ), patch(
@@ -144,15 +142,15 @@
     redirected_url = response.headers["Location"]
     assert redirected_url.endswith("/logout")
 
 
 def test_logout_state_iframe(client):
     with patch(
         "perun.proxygui.user_manager.UserManager._get_ssp_session_by_key",
-        return_value={"user": 123},
+        return_value={"eduperson_principal_name": 123},
     ), patch(
         "perun.proxygui.user_manager.UserManager.get_active_client_ids_for_user",
         return_value=MOCK_SESSIONS,
     ), patch(
         "perun.proxygui.user_manager.UserManager.get_active_client_ids_for_session",
         return_value=[MOCK_SESSIONS[0]],
     ), patch(
```

### Comparing `perun.proxygui-3.5.1/perun/proxygui/tests/test_kerberos_auth_api.py` & `perun.proxygui-4.0.0/perun/proxygui/tests/test_kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/proxygui/user_manager.py` & `perun.proxygui-4.0.0/perun/proxygui/user_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import copy
 import json
 from datetime import datetime
-from typing import Any
+from typing import Any, Dict, List, Tuple, Union
 from typing import Optional
 
-import sqlalchemy
 from perun.connector import AdaptersManager
 from perun.connector import Logger
 from pymongo.collection import Collection
-from sqlalchemy import MetaData
-from sqlalchemy import delete, select
+from sqlalchemy import MetaData, delete, select, update
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm.session import Session
 
 from perun.proxygui import jwt
 from perun.proxygui.jwt import SingletonJWTServiceProvider
 from perun.utils.ConfigStore import ConfigStore
 from perun.utils.DatabaseService import DatabaseService
@@ -46,33 +44,51 @@
         attr_value_candidates = user_attrs.get(attr_name, [])
         attr_value = attr_value_candidates[0] if attr_value_candidates else None
 
         return attr_value
 
     def _revoke_ssp_sessions(
         self,
-        ssp_sessions_collection: Collection,
         subject: str = None,
         session_id: str = None,
     ) -> int:
-        if session_id:
-            result = ssp_sessions_collection.delete_many(
-                {"type": "session", "key": session_id}
-            )
-        elif subject:
-            result = ssp_sessions_collection.delete_many({"user": subject})
-        else:
-            return 0
+        ssp_engine = self.database_service.get_postgres_engine("ssp_database")
+        sessions_table_name = self._cfg["ssp_database"]["sessions_table_name"]
+        ssp_sessions_table = self.database_service.get_postgres_table(
+            ssp_engine, sessions_table_name
+        )
 
-        return result.deleted_count
+        with ssp_engine.begin() as conn:
+            if session_id:
+                delete_query = ssp_sessions_table.delete().where(
+                    (ssp_sessions_table.c._type == "session")
+                    & (ssp_sessions_table.c._key == session_id)
+                )
+            elif subject:
+                delete_query = ssp_sessions_table.delete().where(
+                    ssp_sessions_table.c.eduperson_principal_name == subject
+                )
+            else:
+                self.logger.error(
+                    "Unknown subject and session_id, cannot remove SSP session"
+                )
+                return 0
+            result = conn.execute(delete_query)
+            deleted_count = result.rowcount
+        return deleted_count
 
-    def _remove_ssp_session_index(self, ssp_session_id: str, client_id: str):
+    def _remove_ssp_session_index(self, ssp_session_id: str, client_id: str) -> None:
         """Removes single RP session index from SimpleSAMLSession"""
 
         entry = self._get_ssp_session_by_key(ssp_session_id)
+        if not entry:
+            self.logger.debug(
+                "No session found for %s, cannot remove index.", ssp_session_id
+            )
+            return
         session_details = entry.get("session_indexes_detail", {})
         session_indexes = entry.get("session_indexes", [])
         original_count = len(session_indexes)
         for issuer, data in session_details.items():
             for sp, sid in data.items():
                 if sp == client_id:
                     del data[sp]
@@ -80,15 +96,15 @@
                     break
         if session_indexes and len(session_indexes) != original_count:
             self.logger.info(
                 f"Removed single session index for client_id {client_id} in session "
                 f"{ssp_session_id}"
             )
             self._update_ssp_session_indexes(
-                ssp_session_id, entry.get("expire"), session_indexes, session_details
+                ssp_session_id, entry.get("_expire"), session_indexes, session_details
             )
 
     def _revoke_satosa_grants(
         self,
         satosa_sessions_collection: Collection,
         subject: str = None,
         session_id: str = None,
@@ -101,20 +117,14 @@
             query["client_id"] = client_id
         if session_id is not None:
             query["claims.ssp_session_id"] = session_id
         result = satosa_sessions_collection.delete_many(query)
 
         return result.deleted_count
 
-    def _get_postgres_engine(self) -> Engine:
-        connection_string = self._cfg["mitre_database"]["connection_string"]
-        engine = sqlalchemy.create_engine(connection_string)
-
-        return engine
-
     def _get_mitre_delete_statements(
         self,
         engine: Engine,
         user_id: str = None,
         session_id: str = None,
         include_refresh_tokens=False,
     ) -> list[Any]:
@@ -178,32 +188,29 @@
         self,
         user_id: str = None,
         session_id: str = None,
         include_refresh_tokens: bool = False,
     ) -> int:
         deleted_mitre_tokens_count = 0
 
-        engine = self._get_postgres_engine()
+        engine = self.database_service.get_postgres_engine("mitre_database")
         statements = self._get_mitre_delete_statements(
             engine, user_id, session_id, include_refresh_tokens
         )
         with engine.connect() as cnxn:
             for stmt in statements:
                 with cnxn.begin():
                     result = cnxn.execute(stmt)
                     deleted_mitre_tokens_count += result.rowcount
 
         return deleted_mitre_tokens_count
 
     def _get_satosa_sessions_collection(self) -> Collection:
         return self.database_service.get_mongo_db_collection("satosa_database")
 
-    def _get_ssp_sessions_collection(self) -> Collection:
-        return self.database_service.get_mongo_db_collection("ssp_database")
-
     def sub_to_user_id(self, sub: str, issuer: str) -> Optional[str]:
         """
         Get Perun user ID using user's 'sub' attribute
         :param sub: Perun user's subject attribute
         :return: Perun user ID
         """
         if sub and issuer:
@@ -245,26 +252,23 @@
             satosa_sessions_collection, subject, session_id
         )
 
         deleted_tokens_count = self._delete_mitre_tokens(
             user_id=user_id, include_refresh_tokens=include_refresh_tokens
         )
 
-        ssp_sessions_collection = self._get_ssp_sessions_collection()
-        revoked_sessions_count = self._revoke_ssp_sessions(
-            ssp_sessions_collection, subject, session_id
-        )
+        revoked_sessions_count = self._revoke_ssp_sessions(subject, session_id)
 
         self.logger.info(
             f"Logged out user {subject} from {revoked_sessions_count} SSP "
             f"sessions, deleted {revoked_grants_count} SATOSA sessions and "
             f"deleted {deleted_tokens_count} mitre tokens."
         )
 
-    def logout_from_service_op(self, subject, ssp_session_id, client_id):
+    def logout_from_service_op(self, subject, ssp_session_id, client_id) -> None:
         satosa_sessions_collection = self._get_satosa_sessions_collection()
         self._revoke_satosa_grants(
             satosa_sessions_collection, subject, ssp_session_id, client_id
         )
         self._remove_ssp_session_index(ssp_session_id, client_id)
         # todo - keep skipping mitre?
 
@@ -288,15 +292,15 @@
         satosa_clients = self._get_satosa_client_ids_by_session(session_id)
         # SKIP - mitre
 
         return ssp_clients + satosa_clients
 
     def _get_mitre_client_ids_by_user(self, user_id: str) -> list[str]:
         # todo - remove ? probably won't be used
-        engine = self._get_postgres_engine()
+        engine = self.database_service.get_postgres_engine("mitre_database")
         meta_data = MetaData()
         meta_data.reflect(engine)
         session = Session(bind=engine)
 
         AUTH_HOLDER_TBL = meta_data.tables["authentication_holder"]
         SAVED_USER_AUTH_TBL = meta_data.tables["saved_user_auth"]
         ACCESS_TOKEN_TBL = meta_data.tables["access_token"]
@@ -318,108 +322,131 @@
                             )
                         )
                     )
                 )
                 result = cnxn.execute(stmt)
         return [r[0] for r in result]
 
-    def get_user_id_by_ssp_session_id(self, ssp_session_id: str):
+    def get_user_id_by_ssp_session_id(self, ssp_session_id: str) -> Union[str, None]:
         if ssp_session_id is None:
             return None
         entry = self._get_ssp_session_by_key(ssp_session_id)
-        return entry.get("user") if entry is not None else None
+        return entry.get("eduperson_principal_name") if entry is not None else None
 
-    def _get_ssp_session_by_key(self, ssp_session_id):
+    def _get_ssp_session_by_key(self, ssp_session_id) -> Union[Dict[str, Any], None]:
         """
         Returns SSP session by its key (SimpleSAMLSessionID passed in cookies).
         Uses existing db indexes.
         :param ssp_session_id: SimpleSAMLSessionID
-        :return: session as stored in db
+        :return: session as stored in db or None if not found
         """
         current_datetime = datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
-        ssp_sessions_collection = self._get_ssp_sessions_collection()
-
-        return ssp_sessions_collection.find_one(
-            {
-                "$or": [
-                    {
-                        "$and": [
-                            {"type": "session"},
-                            {"key": ssp_session_id},
-                            {"expire": {"$gt": current_datetime}},
-                        ]
-                    },
-                    {
-                        "$and": [
-                            {"type": "session"},
-                            {"key": ssp_session_id},
-                            {"expire": None},
-                        ]
-                    },
-                ]
-            }
+        ssp_engine = self.database_service.get_postgres_engine("ssp_database")
+        sessions_table_name = self._cfg["ssp_database"]["sessions_table_name"]
+        ssp_sessions_table = self.database_service.get_postgres_table(
+            ssp_engine, sessions_table_name
         )
 
+        with ssp_engine.begin() as conn:
+            query = select(ssp_sessions_table).where(
+                (
+                    (ssp_sessions_table.c._type == "session")
+                    & (ssp_sessions_table.c._key == ssp_session_id)
+                    & (
+                        (ssp_sessions_table.c._expire > current_datetime)
+                        | (ssp_sessions_table.c._expire is None)
+                    )
+                )
+            )
+
+            result = conn.execute(query)
+            row = result.first()
+            if row:
+                row_dict = {
+                    column_name: value for column_name, value in zip(result.keys(), row)
+                }
+                row_dict["session_indexes_detail"] = (
+                    json.loads(row_dict["session_indexes_detail"])
+                    if row_dict.get("session_indexes_detail")
+                    else {}
+                )
+                return row_dict
+            else:
+                return None
+
     def _update_ssp_session_indexes(
         self, session_id, expiration, session_indexes, session_details
-    ):
+    ) -> None:
         """
         Updates SimpleSAMLSession's RP sessions
         :param session_id: the original session key
         :param expiration: the original expiration (so we could use index)
         :param session_indexes: new session indexes
         :param session_details: new session details
         """
-        ssp_sessions_collection = self._get_ssp_sessions_collection()
-        return ssp_sessions_collection.update_one(
-            {
-                "$or": [
-                    {
-                        "$and": [
-                            {"type": "session"},
-                            {"key": session_id},
-                            {"expire": expiration},
-                        ]
-                    },
-                    {
-                        "$and": [
-                            {"type": "session"},
-                            {"key": session_id},
-                            {"expire": None},
-                        ]
-                    },
-                ]
-            },
-            {
-                "$set": {
-                    "session_indexes_detail": session_details,
-                    "session_indexes": session_indexes,
-                }
-            },
+        ssp_engine = self.database_service.get_postgres_engine("ssp_database")
+        sessions_table_name = self._cfg["ssp_database"]["sessions_table_name"]
+        ssp_sessions_table = self.database_service.get_postgres_table(
+            ssp_engine, sessions_table_name
         )
 
-    def _get_ssp_entity_ids_by_user(self, sub: str):
-        ssp_sessions_collection = self._get_ssp_sessions_collection()
-        entries = ssp_sessions_collection.find(
-            {"user": sub}, {"session_indexes_detail": 1, "_id": 0}
+        with ssp_engine.begin() as conn:
+            update_query = (
+                update(ssp_sessions_table)
+                .where(
+                    (
+                        (ssp_sessions_table.c._type == "session")
+                        & (ssp_sessions_table.c._key == session_id)
+                        & (
+                            (ssp_sessions_table.c._expire == expiration)
+                            | (ssp_sessions_table.c._expire is None)
+                        )
+                    )
+                )
+                .values(
+                    session_indexes_detail=json.dumps(session_details),
+                    session_indexes=session_indexes,
+                )
+            )
+
+            conn.execute(update_query)
+
+    def _get_ssp_entity_ids_by_user(self, sub: str) -> List[Tuple[str, str, str]]:
+        ssp_engine = self.database_service.get_postgres_engine("ssp_database")
+        sessions_table_name = self._cfg["ssp_database"]["sessions_table_name"]
+        ssp_sessions_table = self.database_service.get_postgres_table(
+            ssp_engine, sessions_table_name
         )
 
-        result = []
-        for entry in entries:
-            session_details = entry.get("session_indexes_detail", {})
-            for issuer, data in session_details.items():
-                for sp, sid in data.items():
-                    result.append((sp, sid, issuer))
+        with ssp_engine.begin() as conn:
+            sql_query = select(ssp_sessions_table.c.session_indexes_detail).where(
+                ssp_sessions_table.c.eduperson_principal_name == sub
+            )
+
+            result = conn.execute(sql_query)
+
+            entries = result.fetchall()
+            result = []
+            for entry in entries:
+                session_details = json.loads(entry[0])
+                for issuer, data in session_details.items():
+                    for sp, sid in data.items():
+                        result.append((sp, sid, issuer))
+
         return result
 
-    def _get_ssp_entity_ids_by_session(self, session_id: str):
+    def _get_ssp_entity_ids_by_session(
+        self, session_id: str
+    ) -> List[Tuple[str, str, str]]:
         entry = self._get_ssp_session_by_key(session_id)
 
         result = []
-        session_details = entry.get("session_indexes_detail", {})
+        session_details = (
+            entry.get("session_indexes_detail", {}) if entry is not None else {}
+        )
         for issuer, data in session_details.items():
             for sp, sid in data.items():
                 result.append((sp, sid, issuer))
         return result
 
     def _get_satosa_client_ids_by_user(self, sub: str):
         search_argument = {"sub": sub}
```

### Comparing `perun.proxygui-3.5.1/perun/utils/ConfigStore.py` & `perun.proxygui-4.0.0/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/CustomRPHandler.py` & `perun.proxygui-4.0.0/perun/utils/CustomRPHandler.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/EmailService.py` & `perun.proxygui-4.0.0/perun/utils/EmailService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/Utils.py` & `perun.proxygui-4.0.0/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/consent_framework/consent.py` & `perun.proxygui-4.0.0/perun/utils/consent_framework/consent.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/consent_framework/consent_db.py` & `perun.proxygui-4.0.0/perun/utils/consent_framework/consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/consent_framework/consent_manager.py` & `perun.proxygui-4.0.0/perun/utils/consent_framework/consent_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/consent_framework/consent_request.py` & `perun.proxygui-4.0.0/perun/utils/consent_framework/consent_request.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/consent_framework/consent_request_db.py` & `perun.proxygui-4.0.0/perun/utils/consent_framework/consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/logout_requests/BackchannelLogoutRequest.py` & `perun.proxygui-4.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py` & `perun.proxygui-4.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/logout_requests/GraphLogoutRequest.py` & `perun.proxygui-4.0.0/perun/utils/logout_requests/GraphLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/logout_requests/LogoutRequest.py` & `perun.proxygui-4.0.0/perun/utils/logout_requests/LogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun/utils/logout_requests/SamlLogoutRequest.py` & `perun.proxygui-4.0.0/perun/utils/logout_requests/SamlLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun.proxygui.egg-info/PKG-INFO` & `perun.proxygui-4.0.0/perun.proxygui.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 3.5.1
+Version: 4.0.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
```

### Comparing `perun.proxygui-3.5.1/perun.proxygui.egg-info/SOURCES.txt` & `perun.proxygui-4.0.0/perun.proxygui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/perun.proxygui.egg-info/requires.txt` & `perun.proxygui-4.0.0/perun.proxygui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-3.5.1/setup.py` & `perun.proxygui-4.0.0/setup.py`

 * *Files identical despite different names*

