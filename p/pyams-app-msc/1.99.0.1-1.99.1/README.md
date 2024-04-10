# Comparing `tmp/pyams_app_msc-1.99.0.1.tar.gz` & `tmp/pyams_app_msc-1.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_app_msc-1.99.0.1.tar", last modified: Wed Feb 28 22:00:08 2024, max compression
+gzip compressed data, was "dist/pyams_app_msc-1.99.1.tar", last modified: Wed Apr 10 07:49:17 2024, max compression
```

## Comparing `pyams_app_msc-1.99.0.1.tar` & `pyams_app_msc-1.99.1.tar`

### file list

```diff
@@ -1,371 +1,373 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1666 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)      108 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/docs/booking.puml
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/docs/classes.puml
--rw-rw-rw-   0 root         (0) root         (0)    16507 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/docs/es-mapping.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/assets/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/clock.png
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/email.png
--rw-rw-rw-   0 root         (0) root         (0)   207972 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   117372 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    68004 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    25452 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   419720 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   156496 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    10832 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-v4compatibility.ttf
--rw-rw-rw-   0 root         (0) root         (0)     4792 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/fa-v4compatibility.woff2
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/form.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/phone.png
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/select2-spinner.gif
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/select2.png
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/select2x2.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/assets/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/css/dev/
--rw-rw-rw-   0 root         (0) root         (0)   263831 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/dev/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/css/dist/
--rw-rw-rw-   0 root         (0) root         (0)   337917 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/dist/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/css/img/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/clock.png
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/download.svg
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/email.png
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/form.png
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/link.svg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/phone.png
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/print.svg
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/search.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/css/img/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/
--rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/mscapp.js.map
--rw-rw-rw-   0 root         (0) root         (0)     4652 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    10624 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)     6409 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    19333 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
--rw-rw-rw-   0 root         (0) root         (0)    29675 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   209738 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
--rw-rw-rw-   0 root         (0) root         (0)   236865 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   182041 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
--rw-rw-rw-   0 root         (0) root         (0)   230602 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
--rw-rw-rw-   0 root         (0) root         (0)   181575 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
--rw-rw-rw-   0 root         (0) root         (0)   230045 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
--rw-rw-rw-   0 root         (0) root         (0)   174144 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
--rw-rw-rw-   0 root         (0) root         (0)   220941 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
--rw-rw-rw-   0 root         (0) root         (0)    21983 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)    18395 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18911 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
--rw-rw-rw-   0 root         (0) root         (0)    20127 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   450498 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
--rw-rw-rw-   0 root         (0) root         (0)   569896 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    46418 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
--rw-rw-rw-   0 root         (0) root         (0)    53162 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)   153997 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
--rw-rw-rw-   0 root         (0) root         (0)   189149 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   114212 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
--rw-rw-rw-   0 root         (0) root         (0)   139871 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/116.js
--rw-rw-rw-   0 root         (0) root         (0)     8340 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/137.js
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/178.js
--rw-rw-rw-   0 root         (0) root         (0)    67548 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/23.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/23.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/243.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/243.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16009 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/274.js
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/284.js
--rw-rw-rw-   0 root         (0) root         (0)    69465 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/458.js
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/47.js
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/481.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/481.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/528.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/528.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70026 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/612.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/612.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16008 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/623.js
--rw-rw-rw-   0 root         (0) root         (0)    61493 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/624.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/624.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   105878 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/660.js
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/660.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/671.js
--rw-rw-rw-   0 root         (0) root         (0)    69464 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/686.js
--rw-rw-rw-   0 root         (0) root         (0)    61491 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/698.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/698.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/814.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/814.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/830.js
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/854.js
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/860.js
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/882.js
--rw-rw-rw-   0 root         (0) root         (0)   937336 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/pkg/js/dist/mscapp.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3864 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/
--rw-rw-rw-   0 root         (0) root         (0)     1188 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/
--rw-rw-rw-   0 root         (0) root         (0)    12351 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/container.py
--rw-rw-rw-   0 root         (0) root         (0)     9596 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4366 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/reminder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6130 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    34192 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15231 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/home.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/reminder.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3080 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
--rw-rw-rw-   0 root         (0) root         (0)    37871 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/oauth/
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/oauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/oauth/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3332 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/oauth/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/
--rw-rw-rw-   0 root         (0) root         (0)     3511 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    12615 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8006 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15941 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/
--rw-rw-rw-   0 root         (0) root         (0)     3428 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4090 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2433 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7142 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/password.py
--rw-rw-rw-   0 root         (0) root         (0)    11384 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11447 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/
--rw-rw-rw-   0 root         (0) root         (0)    20552 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   167336 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)   167000 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
--rw-rw-rw-   0 root         (0) root         (0)   168644 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/
--rw-rw-rw-   0 root         (0) root         (0)    17175 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/api/
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4590 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/generations/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/include.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    61323 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
--rw-rw-rw-   0 root         (0) root         (0)   105450 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
--rw-rw-rw-   0 root         (0) root         (0)    74850 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/pyams_app_msc.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1750 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/
--rw-rw-rw-   0 root         (0) root         (0)     4447 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/api/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4485 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3476 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2050 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3704 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6790 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8068 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3360 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/
--rw-rw-rw-   0 root         (0) root         (0)     8288 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/audience.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    12263 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/audience.py
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/price.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/room.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/page.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/price.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/room.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/session.py
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11906 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9666 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/audience.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/planning.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/presentation.py
--rw-rw-rw-   0 root         (0) root         (0)     9318 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/price.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/room.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/session.py
--rw-rw-rw-   0 root         (0) root         (0)     2205 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/form.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     5255 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/
--rw-rw-rw-   0 root         (0) root         (0)    11860 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_form.js
--rw-rw-rw-   0 root         (0) root         (0)     5731 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_gis.js
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_i18n.js
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_search.js
--rw-rw-rw-   0 root         (0) root         (0)     9714 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4237 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/mscapp.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_content.scss
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_list.scss
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_search.scss
--rw-rw-rw-   0 root         (0) root         (0)     4329 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/msc.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/templates/select-admin-theater.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:08.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    20672 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/resources/js/msc.js
--rw-rw-rw-   0 root         (0) root         (0)     8006 2024-02-28 21:59:42.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/resources/js/msc.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1666 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12787 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      670 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-28 22:00:07.000000 pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/booking.puml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/classes.puml
+-rw-rw-rw-   0 root         (0) root         (0)    16507 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/es-mapping.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/email.png
+-rw-rw-rw-   0 root         (0) root         (0)   207972 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   117372 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    68004 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    25452 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   419720 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   156496 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    10832 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/form.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/layers-2x.png
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/layers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/marker-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/select2-spinner.gif
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/select2.png
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/select2x2.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/dev/
+-rw-rw-rw-   0 root         (0) root         (0)   263831 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/dev/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   337917 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/dist/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/download.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/email.png
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/form.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/print.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/js/dev/
+-rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    10624 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    19333 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    29675 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   209738 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   236865 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   182041 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
+-rw-rw-rw-   0 root         (0) root         (0)   230602 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   181575 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
+-rw-rw-rw-   0 root         (0) root         (0)   230045 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   174144 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
+-rw-rw-rw-   0 root         (0) root         (0)   220941 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    21983 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    18395 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   450498 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   569896 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    46418 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    53162 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   153997 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   189149 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   114212 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   139871 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/js/dist/
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/116.js
+-rw-rw-rw-   0 root         (0) root         (0)     8340 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/137.js
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/178.js
+-rw-rw-rw-   0 root         (0) root         (0)    67548 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/23.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/23.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/243.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/243.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16009 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/274.js
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/284.js
+-rw-rw-rw-   0 root         (0) root         (0)    69465 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/458.js
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/47.js
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/481.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/481.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/528.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/528.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70026 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/612.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/612.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/623.js
+-rw-rw-rw-   0 root         (0) root         (0)    61493 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/624.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/624.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   105878 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/660.js
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/660.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/671.js
+-rw-rw-rw-   0 root         (0) root         (0)    69464 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/686.js
+-rw-rw-rw-   0 root         (0) root         (0)    61491 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/698.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/698.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/814.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/814.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/830.js
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/854.js
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/860.js
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/882.js
+-rw-rw-rw-   0 root         (0) root         (0)   937336 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3871 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/
+-rw-rw-rw-   0 root         (0) root         (0)    12350 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     9596 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/reminder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    34191 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15231 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/home.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3080 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
+-rw-rw-rw-   0 root         (0) root         (0)    38087 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    12615 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8006 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15941 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4090 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/password.py
+-rw-rw-rw-   0 root         (0) root         (0)    11384 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    11638 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/
+-rw-rw-rw-   0 root         (0) root         (0)    20552 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   167336 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   167000 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   168644 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/
+-rw-rw-rw-   0 root         (0) root         (0)    17171 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8628 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    61512 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
+-rw-rw-rw-   0 root         (0) root         (0)   105688 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
+-rw-rw-rw-   0 root         (0) root         (0)    74943 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/pyams_app_msc.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/
+-rw-rw-rw-   0 root         (0) root         (0)     4447 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3360 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/
+-rw-rw-rw-   0 root         (0) root         (0)     8288 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4330 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/audience.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    12262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/room.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12429 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9666 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/planning.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/presentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9318 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5255 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_form.js
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_gis.js
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_i18n.js
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_search.js
+-rw-rw-rw-   0 root         (0) root         (0)     9714 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/mscapp.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_content.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_list.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_search.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/msc.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/templates/select-admin-theater.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    20672 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.js
+-rw-rw-rw-   0 root         (0) root         (0)     8006 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:49:12.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/top_level.txt
```

### Comparing `pyams_app_msc-1.99.0.1/LICENSE` & `pyams_app_msc-1.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/PKG-INFO` & `pyams_app_msc-1.99.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyams_app_msc
-Version: 1.99.0.1
+Version: 1.99.1
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
@@ -38,23 +37,30 @@
 is available on `Gitlab <https://gitlab.com/pyams>`_ and pushed to `Github
 <https://github.com/py-ams>`_. Doctests are available in the *doctests* source folder.
 
 
 What is PyAMS MSC application?
 ==============================
 
-PyAMS MSC application is a french web application ("Ma Sortie Cinéma") which is used to manage sessions
+PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - added edit forms content getters
+ - added custom catalog entry roles adapters
+ - removed roles restrictions menu entries from theater navigation menu
+ - removed source folder from movie theater activity types properties (issue #6)
+ - changed reminder delay unit from hours to days (issue #4]
+ - updated theater settings edit form (issue #4)
+
 1.99.0.1
 --------
  - fixed packaging issue
 
 1.99.0
 ------
  - first preliminary release
-
-
```

### Comparing `pyams_app_msc-1.99.0.1/docs/README.rst` & `pyams_app_msc-1.99.1/docs/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 is available on `Gitlab <https://gitlab.com/pyams>`_ and pushed to `Github
 <https://github.com/py-ams>`_. Doctests are available in the *doctests* source folder.
 
 
 What is PyAMS MSC application?
 ==============================
 
-PyAMS MSC application is a french web application ("Ma Sortie Cinéma") which is used to manage sessions
+PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
```

### Comparing `pyams_app_msc-1.99.0.1/docs/classes.puml` & `pyams_app_msc-1.99.1/docs/classes.puml`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/docs/es-mapping.json` & `pyams_app_msc-1.99.1/docs/es-mapping.json`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/clock.png` & `pyams_app_msc-1.99.1/pkg/assets/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/email.png` & `pyams_app_msc-1.99.1/pkg/assets/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-brands-400.ttf` & `pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-brands-400.woff2` & `pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-regular-400.ttf` & `pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-regular-400.woff2` & `pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-solid-900.ttf` & `pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-solid-900.woff2` & `pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-v4compatibility.ttf` & `pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/fa-v4compatibility.woff2` & `pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/form.png` & `pyams_app_msc-1.99.1/pkg/assets/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/layers-2x.png` & `pyams_app_msc-1.99.1/pkg/assets/layers-2x.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/layers.png` & `pyams_app_msc-1.99.1/pkg/assets/layers.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/list-item.png` & `pyams_app_msc-1.99.1/pkg/assets/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/map.png` & `pyams_app_msc-1.99.1/pkg/assets/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/marker-icon.png` & `pyams_app_msc-1.99.1/pkg/assets/marker-icon.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/mobile-menu.png` & `pyams_app_msc-1.99.1/pkg/assets/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/phone.png` & `pyams_app_msc-1.99.1/pkg/assets/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/select2-spinner.gif` & `pyams_app_msc-1.99.1/pkg/assets/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/select2.png` & `pyams_app_msc-1.99.1/pkg/assets/select2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/select2x2.png` & `pyams_app_msc-1.99.1/pkg/assets/select2x2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/assets/social-icons.png` & `pyams_app_msc-1.99.1/pkg/assets/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/dev/msc.css` & `pyams_app_msc-1.99.1/pkg/css/dev/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/dist/msc.css` & `pyams_app_msc-1.99.1/pkg/css/dist/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/clock.png` & `pyams_app_msc-1.99.1/pkg/css/img/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/download.svg` & `pyams_app_msc-1.99.1/pkg/css/img/download.svg`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/email.png` & `pyams_app_msc-1.99.1/pkg/css/img/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/form.png` & `pyams_app_msc-1.99.1/pkg/css/img/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/list-item.png` & `pyams_app_msc-1.99.1/pkg/css/img/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/map.png` & `pyams_app_msc-1.99.1/pkg/css/img/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/mobile-menu.png` & `pyams_app_msc-1.99.1/pkg/css/img/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/phone.png` & `pyams_app_msc-1.99.1/pkg/css/img/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/search.png` & `pyams_app_msc-1.99.1/pkg/css/img/search.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/css/img/social-icons.png` & `pyams_app_msc-1.99.1/pkg/css/img/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/mscapp.js` & `pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/mscapp.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map` & `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/116.js` & `pyams_app_msc-1.99.1/pkg/js/dist/116.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/137.js` & `pyams_app_msc-1.99.1/pkg/js/dist/137.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/23.js` & `pyams_app_msc-1.99.1/pkg/js/dist/23.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/23.js.LICENSE.txt` & `pyams_app_msc-1.99.1/pkg/js/dist/23.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/243.js` & `pyams_app_msc-1.99.1/pkg/js/dist/243.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/274.js` & `pyams_app_msc-1.99.1/pkg/js/dist/274.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/284.js` & `pyams_app_msc-1.99.1/pkg/js/dist/284.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/458.js` & `pyams_app_msc-1.99.1/pkg/js/dist/458.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/47.js` & `pyams_app_msc-1.99.1/pkg/js/dist/47.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/481.js` & `pyams_app_msc-1.99.1/pkg/js/dist/481.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/528.js` & `pyams_app_msc-1.99.1/pkg/js/dist/528.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/528.js.LICENSE.txt` & `pyams_app_msc-1.99.1/pkg/js/dist/528.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/612.js` & `pyams_app_msc-1.99.1/pkg/js/dist/612.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/612.js.LICENSE.txt` & `pyams_app_msc-1.99.1/pkg/js/dist/612.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/623.js` & `pyams_app_msc-1.99.1/pkg/js/dist/623.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/624.js` & `pyams_app_msc-1.99.1/pkg/js/dist/624.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/660.js` & `pyams_app_msc-1.99.1/pkg/js/dist/660.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/686.js` & `pyams_app_msc-1.99.1/pkg/js/dist/686.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/698.js` & `pyams_app_msc-1.99.1/pkg/js/dist/698.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/814.js` & `pyams_app_msc-1.99.1/pkg/js/dist/814.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/814.js.LICENSE.txt` & `pyams_app_msc-1.99.1/pkg/js/dist/814.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/830.js` & `pyams_app_msc-1.99.1/pkg/js/dist/830.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/854.js` & `pyams_app_msc-1.99.1/pkg/js/dist/854.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/860.js` & `pyams_app_msc-1.99.1/pkg/js/dist/860.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/882.js` & `pyams_app_msc-1.99.1/pkg/js/dist/882.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/mscapp.js` & `pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/pkg/js/dist/mscapp.js.LICENSE.txt` & `pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/setup.py` & `pyams_app_msc-1.99.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.0.1'
+version = '1.99.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 data_dir = 'pkg'
 data_files = [(d, [os.path.join(d, f) for f in files])
               for d, folders, files in os.walk(data_dir)]
 
 tests_require = [
@@ -80,15 +80,15 @@
           'persistent',
           'pillow',
           'pyams_catalog',
           'pyams_content',
           'pyams_content_api',
           'pyams_content_es',
           'pyams_file',
-          'pyams_form',
+          'pyams_form >= 2.1.0',
           'pyams_i18n',
           'pyams_layer',
           'pyams_mail',
           'pyams_pagelet',
           'pyams_portal',
           'pyams_scheduler',
           'pyams_security >= 2.2.1',
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/address/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/admininfo/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/banking/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/contact/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/schema.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/component/duration/zmi/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     theater = IMovieTheater(booking)
     task_id = f'reminder::{ICacheKeyValue(booking)}'
     if task_id in scheduler:
         del scheduler[task_id]
     settings = IMovieTheaterSettings(theater)
     if not settings.reminder_delay:
         return
-    reminder_date = booking.session.start_date - timedelta(hours=settings.reminder_delay)
+    reminder_date = booking.session.start_date - timedelta(days=settings.reminder_delay)
     if reminder_date < tztime(datetime.utcnow()):
         return
     if booking.send_reminder and not booking.reminder_date:
         task = BookingReminderTask(booking)
         task.name = f'Booking {task_id}'
         task.schedule_mode = SCHEDULER_TASK_DATE_MODE
         scheduler_info = IDateTaskScheduling(task)
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/container.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/reminder.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/task.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,15 +757,15 @@
         if context.status != BOOKING_STATUS.ACCEPTED.value:
             return None
         theater = IMovieTheater(context)
         settings = IMovieTheaterSettings(theater)
         if not settings.reminder_delay:
             return None
         reminder_date = (context.session.start_date -
-                         datetime.timedelta(hours=settings.reminder_delay))
+                         datetime.timedelta(days=settings.reminder_delay))
         if reminder_date < tztime(datetime.datetime.utcnow()):
             return None
         return FormGroupChecker.__new__(cls)
 
     legend = _("Booking reminder")
     fields = Fields(IBookingInfo).select('send_reminder', 'reminder_subject',
                                          'reminder_message')
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/dashboard.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/home.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/home.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/reminder.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/search.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/task.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/booking/zmi/workflow.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from pyams_content.feature.history.interfaces import IHistoryContainer
 from pyams_content.feature.history.zmi.viewlet import HistoryCommentsContentProvider
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
 from pyams_form.group import Group
 from pyams_form.interfaces import DISPLAY_MODE
-from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IGroup
+from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IFormContent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_mail.interfaces import IPrincipalMailInfo
 from pyams_mail.message import HTMLMessage
 from pyams_security.interfaces import ISecurityManager
 from pyams_skin.interfaces.viewlet import IFormHeaderViewletManager, IHelpViewletManager
 from pyams_skin.schema.button import ActionButton, CloseButton, SubmitButton
 from pyams_skin.viewlet.help import AlertMessage
@@ -465,21 +465,25 @@
 
     _mode = DISPLAY_MODE
 
     legend = _("Session properties")
     fields = Fields(ISession).select('capacity') + Fields(IBookingContainer).select('free_seats')
     weight = 1
 
-    def get_content(self):
-        return ISession(self.context)
-
     def update_widgets(self, prefix=None, use_form_mode=True):
         super().update_widgets(prefix, use_form_mode=False)
 
 
+@adapter_config(required=(IBookingInfo, IAdminLayer, SessionInfoDisplayForm),
+                provides=IFormContent)
+def booking_info_display_form_content(context, request, group):
+    """Booking info display form group content getter"""
+    return ISession(context)
+
+
 @adapter_config(name='booking.group',
                 required=(IBookingInfo, IAdminLayer, BaseBookingAdminForm),
                 provides=IGroup)
 class BookingWorkflowInfoGroup(Group):
     """Booking info group"""
 
     legend = _("Booking properties")
@@ -855,15 +859,15 @@
     """Booking accept workflow reminder group"""
 
     def __new__(cls, context, request, view):
         theater = IMovieTheater(context)
         settings = IMovieTheaterSettings(theater)
         if not settings.reminder_delay:
             return None
-        reminder_date = context.session.start_date - timedelta(hours=settings.reminder_delay)
+        reminder_date = context.session.start_date - timedelta(days=settings.reminder_delay)
         if reminder_date < tztime(datetime.utcnow()):
             return None
         return FormGroupChecker.__new__(cls)
 
     fields = Fields(IBookingInfo).select('send_reminder', 'reminder_subject',
                                          'reminder_message')
     weight = 20
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/messaging/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/zmi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_*** module
 
 """
 
-__docformat__ = 'restructuredtext'
-
 from pyams_app_msc.feature.messaging import IMessagingSettings
 from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
+from pyams_form.interfaces.form import IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_site.interfaces import ISiteRoot
+from pyams_utils.adapter import adapter_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
+__docformat__ = 'restructuredtext'
+
 from pyams_app_msc import _
 
 
 @viewlet_config(name='messaging-settings.menu',
                 context=ISiteRoot, layer=IAdminLayer,
                 manager=IPropertiesMenu, weight=700,
                 permission=MANAGE_SITE_ROOT_PERMISSION)
@@ -49,9 +51,13 @@
     """Messaging settings edit form"""
 
     title = _("Messaging service settings")
     legend = _("Messaging properties")
 
     fields = Fields(IMessagingSettings)
 
-    def get_content(self):
-        return IMessagingSettings(self.context)
+
+@adapter_config(required=(ISiteRoot, IPyAMSLayer, MessagingSettingsEditForm),
+                provides=IFormContent)
+def site_root_messaging_edit_form_content(context, request, form):
+    """Site root messaging edit form content getter"""
+    return IMessagingSettings(context)
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/oauth/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/oauth/skin/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/session.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/session.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from zope.interface import Interface
 
 from pyams_app_msc.feature.profile import IUserProfile
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.form import EditForm
-from pyams_form.interfaces.form import IAJAXFormRenderer
+from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.skin.page import PortalContextIndexPage
 from pyams_security.interfaces import LOGIN_REFERER_KEY
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 
 __docformat__ = 'restructuredtext'
 
@@ -37,31 +37,35 @@
     """User profile edit form"""
 
     title = _("My user profile")
     legend = _("Account settings")
 
     fields = Fields(IUserProfile).omit('active')
 
-    def get_content(self):
-        return IUserProfile(self.request)
-
     def update_actions(self):
         super().update_actions()
         action = self.actions.get('apply')
         if action is not None:
             action.add_class('btn-primary')
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         email = self.widgets.get('email')
         if email is not None:
             email.readonly = 'readonly'
 
 
 @adapter_config(required=(Interface, IPyAMSLayer, UserProfileEditForm),
+                provides=IFormContent)
+def user_profile_edit_form_content(context, request, form):
+    """User profile edit form content getter"""
+    return IUserProfile(request)
+
+
+@adapter_config(required=(Interface, IPyAMSLayer, UserProfileEditForm),
                 provides=IAJAXFormRenderer)
 class UserProfileEditFormRenderer(ContextRequestViewAdapter):
     """User profile edit form renderer"""
 
     def render(self, changes):
         result = {
             'status': 'redirect'
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/password.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/password.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/register.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/register.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/task.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,9 +281,13 @@
 class OperatorProfileGroup(Group):
     """Operator profile group"""
 
     legend = _("Operator profile")
 
     fields = Fields(IOperatorProfile)
 
-    def get_content(self):
-        return IOperatorProfile(self.request.principal)
+
+@adapter_config(required=(Interface, IAdminLayer, OperatorProfileGroup),
+                provides=IFormContent)
+def operator_profile_group_content(context, request, group):
+    """Operator profile edit group content getter"""
+    return IOperatorProfile(request.principal)
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/profile/zmi/widget.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     posters_size = FieldProperty(ITMDBConfiguration['posters_size'])
     download_videos = FieldProperty(ITMDBConfiguration['download_videos'])
     restrict_videos_language = FieldProperty(ITMDBConfiguration['restrict_videos_language'])
 
     def get_proxy_info(self, request=None, protocol=None):
         """Proxy information getter"""
         info = self.proxy_info
-        if info is None:
+        if not info:
             return {}
         if request is None:
             request = check_request()
         url = info.get_proxy_url(request)
         if not url:
             return {}
         if protocol is None:
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/api/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/api/schema.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from zope.interface import Interface
 
 from pyams_app_msc.feature.tmdb import ITMDBConfiguration
 from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IGroup
+from pyams_form.interfaces.form import IFormContent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_site.interfaces import ISiteRoot
 from pyams_utils.adapter import adapter_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm, FormGroupChecker
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu
@@ -61,16 +61,20 @@
     """TMDB configuration edit form"""
 
     title = _("TMDB service configuration")
     legend = _("TMDB service properties")
 
     fields = Fields(Interface)
 
-    def get_content(self):
-        return ITMDBConfiguration(self.context)
+
+@adapter_config(required=(ISiteRoot, IPyAMSLayer, TMDBConfigurationEditForm),
+                provides=IFormContent)
+def site_root_tmdb_configuration_edit_form_content(context, request, form):
+    """Site root TMDB configuration edit form content getter"""
+    return ITMDBConfiguration(context)
 
 
 @adapter_config(name='tmdb-configuration',
                 required=(ISiteRoot, IAdminLayer, TMDBConfigurationEditForm),
                 provides=IGroup)
 class TMDBConfigurationGroup(FormGroupChecker):
     """TMDB configuration group"""
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/feature/tmdb/zmi/lookup.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/lookup.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/generations/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/include.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/include.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 
 def include_package(config):
     """Pyramid package include"""
 
     # add translations
     config.add_translation_dirs('pyams_app_msc:locales')
 
+    # override PyAMS_content packages
+    config.include('pyams_content_es')
+    config.include('pyams_content_themes')
+    config.include('pyams_content_api')
+
     # register permissions
     config.register_permission({
         'id': MANAGE_THEATER_PERMISSION,
         'title': _("Manage movie theater properties")
     })
     config.register_permission({
         'id': VIEW_THEATER_PERMISSION,
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo` & `pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -37,25 +37,25 @@
 msgid "(unknown)"
 msgstr "(inconnue)"
 
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
 " &ast; **ATTENTION** &ast;<br />Le nombre de places encore disponibles sur "
-"cette séance n'est pas suffisant pour accueillir cette réservation !"
+"cet événement n'est pas suffisant pour accueillir cette réservation !"
 
 msgid "1 group"
 msgstr "1 groupe"
 
 msgid ""
 "A booking is archived automatically after session end and can't be modified "
 "anymore"
 msgstr ""
-"Une réservation est archivée automatiquement après la fin de la séance "
-"correspondante et ne peut plus être modifiée"
+"Une réservation est archivée automatiquement après la fin de l'événement "
+"correspondant et ne peut plus être modifiée"
 
 msgid "A movie theater is already registered with this name!"
 msgstr "Un autre cinéma est déjà inscrit avec ce nom !"
 
 msgid "A movie theater operator will process your request as soon as possible."
 msgstr ""
 "Un opérateur du cinéma va traiter votre demande dans les meilleurs délais, "
@@ -299,15 +299,18 @@
 msgid "Booking request confirmed!"
 msgstr "Demande de réservation confirmée !"
 
 msgid "Booking retention duration"
 msgstr "Durée de rétention des réservations"
 
 msgid "Booking session"
-msgstr "Nouvelle séance"
+msgstr "Nouvel événement"
+
+msgid "Booking settings"
+msgstr "Gestion des réservations"
 
 msgid "Booking temporarily accepted"
 msgstr "Acceptée (sous réserve)"
 
 msgid "Booking update"
 msgstr "Réservation modifiée"
 
@@ -326,16 +329,16 @@
 msgid "Calendar slot duration"
 msgstr "Durée des créneaux horaires"
 
 msgid "Calendar time slots frequency in week or day views"
 msgstr ""
 "Indiquée en minutes, cette valeur indique la durée des créneaux horaires "
 "affichés dans les vues par semaine ou par jour de l'agenda ; vous pouvez "
-"toujours ajuster la durée des séances plus finement, si besoin, dans le "
-"formulaire de mise à jour des propriétés d'une séance"
+"toujours ajuster la durée des événements plus finement, si besoin, dans le "
+"formulaire de mise à jour des propriétés d'un événement"
 
 msgid "Can't activate account with provided arguments!"
 msgstr ""
 "Impossible d'activer ce compte avec les paramètres de connexion indiqués !"
 
 msgid "Can't change password with provided arguments!"
 msgstr ""
@@ -353,19 +356,19 @@
 
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 "Le délai maximum après la réservation doit être indiqué pour utiliser ce "
 "mode d'annulation !"
 
 msgid "Cancel notice period"
-msgstr "Préavis minimum avant la séance"
+msgstr "Préavis minimum avant l'événement"
 
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
-"Le préavis minimum avant la séance doit être indiqué pour utiliser ce mode "
+"Le préavis minimum avant l'événement doit être indiqué pour utiliser ce mode "
 "d'annulation !"
 
 msgid "Cancelled"
 msgstr "Annulée"
 
 msgid "Cancelled booking"
 msgstr "Réservation annulée"
@@ -388,21 +391,21 @@
 msgid "Catalog presentation"
 msgstr "Entrées du catalogue"
 
 msgid "Catalog template configuration"
 msgstr "Modèle de présentation des entrées du catalogue"
 
 msgid "Change booking session"
-msgstr "Changement de séance"
+msgstr "Changement d'événement"
 
 msgid "Change password"
 msgstr "Changer de mot de passe"
 
 msgid "Change session"
-msgstr "Changer la séance"
+msgstr "Changer d'événement"
 
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 "Sélectionnez cette option lorsque le paiement est fait via un Pass Culture"
 
 msgid "Cinema audience"
 msgstr "Public"
@@ -458,15 +461,15 @@
 msgid "Click icon to switch price activity"
 msgstr "Cliquer cette icône pour activer ou désactiver ce tarif"
 
 msgid "Click icon to switch room activity"
 msgstr "Cliquer cette icône pour activer ou désactiver cette salle"
 
 msgid "Clone event..."
-msgstr "Dupliquer la séance"
+msgstr "Dupliquer l'événement"
 
 msgid "Closing time"
 msgstr "Heure de fermeture"
 
 msgid "Comments"
 msgstr "Commentaire"
 
@@ -530,15 +533,15 @@
 msgid "Cultural pass"
 msgstr "Pass Culture"
 
 msgid "Currency"
 msgstr "Devise"
 
 msgid "Current session bookings"
-msgstr "Réservations sur la séance"
+msgstr "Réservations sur l'événement"
 
 msgid "Custom properties"
 msgstr "Propriétés spécifiques"
 
 msgid "Dashboard"
 msgstr "Tableau de bord"
 
@@ -556,15 +559,15 @@
 msgid "Date:"
 msgstr "Date :"
 
 msgid "Day"
 msgstr "Jour"
 
 msgid "Default session duration"
-msgstr "Durée de base des séances"
+msgstr "Durée de base des événements"
 
 msgid "Default subject used for accepted booking notification"
 msgstr ""
 "Sujet par défaut d'un message d'acceptation d'une demande de réservation"
 
 msgid "Default subject used for cancelled booking notification"
 msgstr "Sujet par défaut d'un message d'annulation d'une réservation"
@@ -581,15 +584,15 @@
 "réservation en attente de validation"
 
 msgid "Default subject used for updated booking notification"
 msgstr ""
 "Sujet par défaut d'un message de modification d'une demande de réservation"
 
 msgid "Delete"
-msgstr "Supprimer la séance"
+msgstr "Supprimer l'événement"
 
 msgid "Designers"
 msgstr "Designers"
 
 msgid "Designers are users which are allowed to manage presentation templates"
 msgstr "Les designers peuvent gérer les modèles de présentation"
 
@@ -703,15 +706,15 @@
 msgid "Establishment of affiliation"
 msgstr "Établissement ou structure"
 
 msgid "First name"
 msgstr "Prénom"
 
 msgid "First time available for sessions planning"
-msgstr "Heure à partir de laquelle des séances peuvent être programmées"
+msgstr "Heure à partir de laquelle des événements peuvent être programmés"
 
 msgid "Floor, corridor..."
 msgstr "Niveau, couloir..."
 
 msgid "Forbidden cancellation"
 msgstr "Annulation impossible"
 
@@ -805,27 +808,27 @@
 
 msgid ""
 "If 'yes', a reminder message will be sent to the recipient a few days before "
 "the session take place; delay before session is defined into theater settings"
 msgstr ""
 "Si cette option est activée, un message de rappel sera envoyé au "
 "bénéficiaire de la réservations quelques heures ou jours avant le début de "
-"la séance ; ce délai est spécifié dans les paramètres du cinéma"
+"l'événement ; ce délai est spécifié dans les paramètres du cinéma"
 
 msgid ""
 "If 'yes', only videos tagged for selected language will be selected; "
 "otherwise, other videos tagged for any language may also be selected"
 msgstr ""
 "Si 'oui', seules les vidéos taggées pour la langue sélectionnée seront "
 "sélectionnées ; dans le cas contraire, d'autres vidéos taggés pour toutes "
 "les langues pourront également être sélectionnées"
 
 msgid "If 'yes', this session is 'temporary' and not confirmed yet!"
 msgstr ""
-"Si 'oui', cette séance est encore temporaire, en attente de confirmation..."
+"Si 'oui', cet événement est encore temporaire, en attente de confirmation..."
 
 msgid "If no label is set, activity label will be used"
 msgstr ""
 "Ce libellé sera affiché en lieu et place du titre de l'activité, s'il y en a "
 "une"
 
 msgid "Images URL"
@@ -859,15 +862,15 @@
 msgid "Language"
 msgstr "Langue"
 
 msgid "Last name"
 msgstr "Nom"
 
 msgid "Last time available for sessions planning"
-msgstr "Heure jusqu'à laquelle des séances peuvent être programmées"
+msgstr "Heure jusqu'à laquelle des événements peuvent être programmés"
 
 msgid "Last update"
 msgstr "Dernière modification"
 
 msgid "List"
 msgstr "Liste"
 
@@ -1134,27 +1137,27 @@
 msgid "New cinema room"
 msgstr "Nouvelle salle"
 
 msgid "New cinema room properties"
 msgstr "Propriétés de la nouvelle salle"
 
 msgid "New session"
-msgstr "Nouvelle séance"
+msgstr "Nouvel événement"
 
 msgid "New session properties"
-msgstr "Propriétés de la séance"
+msgstr "Propriétés de l'événement"
 
 msgid "New theater properties"
 msgstr "Propriétés du nouveau cinéma"
 
 msgid "Next page"
 msgstr "Page suivante"
 
 msgid "No session selected, booking was not changed."
-msgstr "Aucune séance sélectionnée, la réservation n'a pas été modifiée."
+msgstr "Aucun événement sélectionné, la réservation n'a pas été modifiée."
 
 msgid "Not displayed"
 msgstr "Non affichées"
 
 msgid "Notepad"
 msgstr "Bloc-notes"
 
@@ -1172,30 +1175,30 @@
 msgid "Notify recipient?"
 msgstr "Notifier le bénéficiaire"
 
 msgid "Number and street"
 msgstr "Numéro et rue"
 
 msgid "Number of accompanists seats reserved for this session"
-msgstr "Nombre de places réservées pour les accompagnants à cette séance"
+msgstr "Nombre de places réservées pour les accompagnants à cet événement"
 
 msgid "Number of actors "
 msgstr "Nombre maximal d'acteurs récupérés via l'API"
 
 msgid "Number of free seats for this session"
 msgstr ""
-"Nombre de places encore disponibles pour cette séance ; seules les "
+"Nombre de places encore disponibles pour cet événement ; seules les "
 "réservations validées sont prises en compte, y compris cette réservation le "
 "cas échéant"
 
 msgid "Number of groups or classrooms attending this session"
-msgstr "Nombre de groupes ou de classes participant à cette séance"
+msgstr "Nombre de groupes ou de classes participant à cet événement"
 
 msgid "Number of participants seats reserved for this session"
-msgstr "Nombre de places réservées pour les participants à cette séance"
+msgstr "Nombre de places réservées pour les participants à cet événement"
 
 msgid "Number of places available for this session"
 msgstr "Nombre maximal de places ouvertes à la réservation pour cette séance"
 
 msgid "Number of weeks to display sessions"
 msgstr "Nombre de semaines dont on souhaite afficher les séances"
 
@@ -1206,20 +1209,20 @@
 msgstr "VOST"
 
 msgid "Object:"
 msgstr "Objet :"
 
 msgid "Only external bookable sessions are visible to public for booking"
 msgstr ""
-"Seules les séances ouvertes aux réservations externes peuvent faire l'objet "
+"Seuls les événements ouverts aux réservations externes peuvent faire l'objet "
 "de demandes de réservations par les clients du site"
 
 msgid "Only internal bookable sessions are visible to operators for booking"
 msgstr ""
-"Seules les séances ouvertes aux réservations internes peuvent être réservées "
+"Seuls les événements ouverts aux réservations internes peuvent être réservés "
 "par les opérateurs du cinéma"
 
 msgid "Open for external booking"
 msgstr "Ouverte aux réservations externes"
 
 msgid "Open for internal booking"
 msgstr "Ouverte aux réservations internes"
@@ -1460,22 +1463,22 @@
 msgstr "Contenu du message"
 
 msgid ""
 "Reminder message will be sent to booking recipient {} hours before session "
 "begin date..."
 msgstr ""
 "Le message de rappel sera envoyé au bénéficiaire {} heures avant le début de "
-"la séance."
+"l'événement."
 
 msgid ""
 "Reminder message will be sent to the recipient a few days before the session "
 "take place; delay before session is defined into theater settings"
 msgstr ""
 "Le message de rappel est envoyé au bénéficiaire quelques heures ou jours "
-"avant le début de la séance, en fonction du paramétrage appliqué au niveau "
+"avant le début de l'événement, en fonction du paramétrage appliqué au niveau "
 "du cinéma"
 
 msgid "Reminder subject"
 msgstr "Sujet des messages"
 
 msgid "Request password reset"
 msgstr "Demander la réinitialisation du mot de passe"
@@ -1504,15 +1507,15 @@
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
 msgid "Seats"
 msgstr "Places"
 
 msgid "Select the session for which this booking is applied"
-msgstr "Nouvelle séance à laquelle doit s'appliquer la réservation"
+msgstr "Nouvel événement auquel doit s'appliquer la réservation"
 
 msgid "Selected audiences"
 msgstr "Publics concernés"
 
 msgid "Selected mailer"
 msgstr "Service de messagerie"
 
@@ -1528,65 +1531,65 @@
 msgid "Service URL"
 msgstr "URL du service"
 
 msgid "Session"
 msgstr "Séance"
 
 msgid "Session ID"
-msgstr "ID de la séance"
+msgstr "ID de l'événement"
 
 msgid "Session bookings"
 msgstr "Gestion des réservations"
 
 msgid "Session capacity"
 msgstr "Jauge"
 
 msgid "Session capacity has been reduced due to lower room capacity!"
 msgstr ""
-"La jauge de la séance a été réduite du fait de la capacité insuffisante de "
+"La jauge de l'événement a été réduite du fait de la capacité insuffisante de "
 "cette salle !"
 
 msgid "Session date"
-msgstr "Date de la séance"
+msgstr "Date de l'événement"
 
 msgid "Session date: ${date}."
 msgstr "Date de la séance : ${date}"
 
 msgid "Session duration delta"
-msgstr "Temps minimum entre les séances"
+msgstr "Temps minimum entre les événements"
 
 msgid "Session duration, given as time delta object"
 msgstr "Durée de la séance exprimée sous la forme d'un object \"timedelta\""
 
 msgid "Session end date"
 msgstr "Fin de la séance"
 
 msgid "Session planning"
-msgstr "Programmation d'une séance"
+msgstr "Programmation d'un événement"
 
 msgid "Session properties"
-msgstr "Propriétés de la séance"
+msgstr "Propriétés de l'événement"
 
 msgid "Session room"
 msgstr "Salle"
 
 msgid "Session seats display mode"
-msgstr "Affichage des places en séances"
+msgstr "Affichage des places dans l'agenda"
 
 msgid "Session start date"
 msgstr "Début de la séance"
 
 msgid "Session updated"
 msgstr "Séance modifiée"
 
 msgid "Sessions planned for today"
 msgstr "Séances programmées aujourd'hui"
 
 msgid "Sessions planning"
-msgstr "Agenda des séances programmées"
+msgstr "Agenda des événements programmés"
 
 msgid "Sessions weeks"
 msgstr "Nombre de semaines"
 
 msgid "Settings"
 msgstr "Paramètres"
 
@@ -1651,28 +1654,28 @@
 msgid "TV"
 msgstr "VF"
 
 msgid ""
 "Target room doesn't have enough capacity for confirmed seats of this session!"
 msgstr ""
 "La salle sélectionnée ne dispose pas d'une capacité suffisante pour "
-"accueillir les réservations confirmées à cette séance !"
+"accueillir les réservations confirmées à cet événement !"
 
 msgid "Temporary session"
 msgstr "En attente de confirmation"
 
 msgid "The number of validated seats is already higher than this gauge!"
 msgstr ""
 "Vous ne pouvez pas abaisser la jauge à un nombre de places inférieur au "
 "nombre de places déjà validées !"
 
 msgid "The reminder delay is set to {} hours before session start."
 msgstr ""
 "Le message de rappel sera envoyé au bénéficiaire {} heures avant le début de "
-"la séance."
+"l'événement."
 
 msgid ""
 "The site's description is 'hidden' into HTML's page headers; but it can be "
 "seen, for example, in some search engines results as content's description; "
 "if description is empty, content's header will be used."
 msgstr ""
 "Cette description est intégrée dans les en-têtes des pages HTML ; mais elle "
@@ -1690,48 +1693,48 @@
 msgstr "Salle dans laquelle la séance est planifiée"
 
 msgid "Theater week"
 msgstr "Sem. ciné."
 
 msgid "There are only {} free seats left in this session!"
 msgstr ""
-"<strong>ATTENTION :</strong> il ne reste que {} places libres sur cette "
-"séance !"
+"<strong>ATTENTION :</strong> il ne reste que {} places libres sur cet "
+"événement !"
 
 msgid "There is no confirmed booking for this session."
-msgstr "Aucune réservation validée pour cette séance."
+msgstr "Aucune réservation validée pour cet événement."
 
 msgid "There is no session planned for today."
-msgstr "Aucune séance n'est programmée aujourd'hui."
+msgstr "Aucun événement n'est programmé aujourd'hui."
 
 msgid "These comments are for internal use only"
 msgstr "Ce commentaire est à usage interne uniquement"
 
 msgid "These comments where added by booking recipient"
 msgstr "Ce commentaire précise la demande du bénéficiaire"
 
 msgid "These comments will be displayed to the users on booking form"
 msgstr ""
-"Ce commentaire sera visible sur le formulaire de réservation associé à cette "
-"séance"
+"Ce commentaire sera visible sur le formulaire de réservation associé à cet "
+"événement"
 
 msgid ""
 "These principals are allowed to create and manage sites and movie theaters"
 msgstr ""
 "Ces mandataires peuvent procéder à la création d'un nouveau cinéma et nommer "
 "ses gestionnaires"
 
 msgid "This audience is active"
 msgstr "Ce public est activé"
 
 msgid "This audience is not active"
 msgstr "Ce public n'est pas actif actuellement"
 
 msgid "This booking is already registered for this session..."
-msgstr "Cette séance est déjà celle concernée par cette réservation."
+msgstr "Cet événement est déjà celle concerné par cette réservation."
 
 msgid "This booking is archived and can't be modified anymore!"
 msgstr "Cette réservation est archivée et ne peut plus être modifiée !"
 
 msgid ""
 "This color will be used as base color for graphic elements displayed in "
 "quotations"
@@ -1776,36 +1779,36 @@
 "Cette image pourra être utilisée dans les documents et dans les messages "
 "produits par l'application"
 
 msgid ""
 "This is a default duration, in minutes, of sessions for which activity has "
 "no duration"
 msgstr ""
-"Cette durée, exprimée en minutes, est appliquée par défaut aux séances dont "
-"l'activité n'a pas de durée indiquée"
+"Cette durée, exprimée en minutes, est appliquée par défaut aux événements "
+"dont l'activité n'a pas de durée indiquée"
 
 msgid ""
-"This is a delay, given in hours before a session beginning, at which a "
+"This is a delay, given in days before a session beginning, at which a "
 "reminder message can be sent to booking recipients; leave value empty or set "
 "it to 0 to disable reminders messages"
 msgstr ""
-"Ce délai, exprimé en heures, indique combien de temps avant le début d'une "
-"séance est attendu avant l'envoi d'un message de rappel aux bénéficiaires "
+"Ce délai, exprimé en jours, indique combien de temps avant le début d'une "
+"activité est attendu avant l'envoi d'un message de rappel aux bénéficiaires "
 "d'une réservation ; vous pouvez laisser cette valeur vide ou indiquer la "
 "valeur 0 si vous ne souhaitez pas envoyer de messages de rappel. ATTENTION : "
 "les réservations confirmées au-delà de ce délai ne feront pas l'objet de "
 "messages de rappel !"
 
 msgid ""
 "This is a number of minutes which will be added automatically to activities "
 "duration when adding new sessions"
 msgstr ""
 "Cette durée, exprimée en minutes, indique la durée qui sera ajoutée "
-"automatiquement à la durée des films pour définir la durée des séances "
-"proposées aux gestionnaires"
+"automatiquement à la durée des activités pour définir la durée des séances "
+"proposée aux gestionnaires"
 
 msgid "This is the VAT rate which will be used in quotations"
 msgstr "Ceci est le taux de TVA appliqué lors de l'édition' des devis"
 
 msgid "This is the currency used for all transactions"
 msgstr "Ceci est la devise utilisée pour toutes les informations monétaires"
 
@@ -1824,23 +1827,23 @@
 msgstr "Ceci est l'âge minimum du public"
 
 msgid ""
 "This is the minimum amount of time before session, given in hours, during "
 "which a principal can cancel a booking by it's own way"
 msgstr ""
 "Ce préavis, indiqué en heures, correspond à la durée minimale avant le début "
-"de la séance jusqu'à laquelle un bénéficiaire peut encore annuler cette "
+"de l'événement jusqu'à laquelle un bénéficiaire peut encore annuler cette "
 "demande par lui-même, sans contacter le cinéma"
 
 msgid ""
 "This is the minimum amount of time, given in hours, during which a a booking "
 "is kept 'active' before being archived"
 msgstr ""
 "Ceci est la durée minimale, indiquée en heures, avant qu'une réservation "
-"associée à une séance terminée soit archivée automatiquement"
+"associée à un événement terminé ne soit archivée automatiquement"
 
 msgid "This is the price which is applied to each accompanying person"
 msgstr "Ceci est le tarif qui est appliqué à chaque accompagnateur"
 
 msgid "This is the price which is applied to each participant"
 msgstr "Ceci est le tarif qui est appliqué à chaque participant"
 
@@ -1915,16 +1918,16 @@
 msgstr "Cette salle n'est pas disponible actuellement"
 
 msgid ""
 "This template is used for reminder messages which are sent to sessions "
 "recipients a few days before they take place"
 msgstr ""
 "Ce modèle est utilisé pour les messages de rappel qui peuvent être envoyés "
-"quelques jours avant les séances aux bénéficiaires dont les réservations ont "
-"été acceptées"
+"quelques jours avant les événements aux bénéficiaires dont les réservations "
+"ont été acceptées"
 
 msgid "This template is used when a session booking is accepted"
 msgstr ""
 "Ce modèle est utilisé en cas d'acceptation d'une demande de réservation"
 
 msgid "This template is used when a session booking is cancelled"
 msgstr "Ce modèle est utilisé en cas d'annulation d'une demande de réservation"
@@ -2075,15 +2078,15 @@
 "demande. Pour toute question préalable, feuillez utiliser le formulaire de "
 "contact..."
 
 msgid ""
 "You can choose how session seats are displayed in movie theater planning view"
 msgstr ""
 "Vous pouvez choisir la façon dont les places sont affichées dans le planning "
-"des séances"
+"des activités"
 
 msgid ""
 "You can log in using your new account and get access to all site features."
 msgstr ""
 "Vous pouvez retourner à l'écran de connexion et utiliser vos nouveaux "
 "identifiants pour profiter de toutes les fonctionnalités du site."
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po` & `pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,84 +3,84 @@
 # PyAMS application for cinema reservation management
 #
 # This file is distributed under the same license as the PACKAGE package.
 # Thierry Florac <tflorac@ulthar.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS MSC application 1.0.0\n"
-"POT-Creation-Date: 2024-02-26 22:18+0100\n"
+"POT-Creation-Date: 2024-03-24 03:43+0100\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
 
-#: src/pyams_app_msc/include.py:48
+#: src/pyams_app_msc/include.py:53
 msgid "Manage movie theater properties"
 msgstr "Gérer les propriétés d'un cinéma"
 
-#: src/pyams_app_msc/include.py:52
+#: src/pyams_app_msc/include.py:57
 msgid "View movie theater properties"
 msgstr "Voir les propriétés d'un cinéma"
 
-#: src/pyams_app_msc/include.py:56
+#: src/pyams_app_msc/include.py:61
 msgid "Manage movie theater activities catalog"
 msgstr "Gérer le catalogue des activités d'un cinéma"
 
-#: src/pyams_app_msc/include.py:60
+#: src/pyams_app_msc/include.py:65
 msgid "Read movie theater activities catalog"
 msgstr "Voir le catalogue des activités d'un cinéma"
 
-#: src/pyams_app_msc/include.py:64
+#: src/pyams_app_msc/include.py:69
 msgid "Create booking request for movie theater activity"
 msgstr "Créer des demandes de réservations pour les séances d'un cinéma"
 
-#: src/pyams_app_msc/include.py:68
+#: src/pyams_app_msc/include.py:73
 msgid "View sessions planning on movie theater activities"
 msgstr "Voir le planning des séances d'un cinéma"
 
-#: src/pyams_app_msc/include.py:72
+#: src/pyams_app_msc/include.py:77
 msgid "Manage sessions planning on movie theater activities"
 msgstr "Gérer le planning des séances d'un cinéma"
 
-#: src/pyams_app_msc/include.py:76
+#: src/pyams_app_msc/include.py:81
 msgid "View booking information for movie theater activity"
 msgstr "Voir les réservations pour les séances d'un cinéma"
 
-#: src/pyams_app_msc/include.py:80
+#: src/pyams_app_msc/include.py:85
 msgid "Manage bookings for movie theater activity"
 msgstr "Gérer les réservations pour les séances d'un cinéma"
 
-#: src/pyams_app_msc/include.py:103
+#: src/pyams_app_msc/include.py:108
 msgid "MSC: Sites manager"
 msgstr "MSC : Administrateur délégué"
 
-#: src/pyams_app_msc/include.py:115
+#: src/pyams_app_msc/include.py:120
 msgid "MSC: Theater manager"
 msgstr "MSC : Administrateur d'un cinéma"
 
-#: src/pyams_app_msc/include.py:134
+#: src/pyams_app_msc/include.py:139
 msgid "MSC: Theater operator"
 msgstr "MSC : Opérateur d'un cinéma"
 
-#: src/pyams_app_msc/include.py:152
+#: src/pyams_app_msc/include.py:157
 msgid "MSC: Contributor"
 msgstr "MSC : Contributeur d'un cinéma"
 
-#: src/pyams_app_msc/include.py:169
+#: src/pyams_app_msc/include.py:174
 msgid "MSC: Theater consultant"
 msgstr "MSC : Invité d'un cinéma"
 
-#: src/pyams_app_msc/include.py:184
+#: src/pyams_app_msc/include.py:189
 msgid "MSC: Theater client"
 msgstr "MSC : Client d'un cinéma"
 
-#: src/pyams_app_msc/include.py:196
+#: src/pyams_app_msc/include.py:201
 msgid "MSC: Reservation owner"
 msgstr "MSC : Propriétaire d'une réservation"
 
 #: src/pyams_app_msc/feature/tmdb/interfaces.py:41
 msgid "Enable TMDB configuration"
 msgstr "Activer le service TMDB"
 
@@ -355,22 +355,22 @@
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:82
 msgid "Display confirmed/capacity seats"
 msgstr "Afficher les places acceptées / en jauge"
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:98
 msgid "Session seats display mode"
-msgstr "Affichage des places en séances"
+msgstr "Affichage des places dans l'agenda"
 
 #: src/pyams_app_msc/feature/profile/interfaces.py:99
 msgid ""
 "You can choose how session seats are displayed in movie theater planning view"
 msgstr ""
 "Vous pouvez choisir la façon dont les places sont affichées dans le planning "
-"des séances"
+"des activités"
 
 #: src/pyams_app_msc/feature/profile/task.py:56
 msgid "User profile cleaner"
 msgstr "Suppression de profil utilisateur"
 
 #: src/pyams_app_msc/feature/profile/zmi/__init__.py:62
 msgid "User add form"
@@ -647,23 +647,23 @@
 msgid ""
 "This prefix, if any, will be used as subject prefix to all sent email "
 "messages"
 msgstr ""
 "Ce préfixe, s'il est indiqué, sera positionné automatiquement au début du "
 "sujet de tous les mails envoyés"
 
-#: src/pyams_app_msc/feature/messaging/zmi/__init__.py:41
+#: src/pyams_app_msc/feature/messaging/zmi/__init__.py:43
 msgid "Messaging settings"
 msgstr "Paramétrage de la messagerie"
 
-#: src/pyams_app_msc/feature/messaging/zmi/__init__.py:51
+#: src/pyams_app_msc/feature/messaging/zmi/__init__.py:53
 msgid "Messaging service settings"
 msgstr "Paramètres de la messagerie"
 
-#: src/pyams_app_msc/feature/messaging/zmi/__init__.py:52
+#: src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr "Propriétés de la messagerie"
 
 #: src/pyams_app_msc/feature/planning/session.py:156
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
 msgid "{room} - {date} from {start_time} to {end_time}"
@@ -776,45 +776,45 @@
 #: src/pyams_app_msc/feature/planning/interfaces.py:113
 msgid "Temporary session"
 msgstr "En attente de confirmation"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:114
 msgid "If 'yes', this session is 'temporary' and not confirmed yet!"
 msgstr ""
-"Si 'oui', cette séance est encore temporaire, en attente de confirmation..."
+"Si 'oui', cet événement est encore temporaire, en attente de confirmation..."
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:118
 msgid "Open for internal booking"
 msgstr "Ouverte aux réservations internes"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:119
 msgid "Only internal bookable sessions are visible to operators for booking"
 msgstr ""
-"Seules les séances ouvertes aux réservations internes peuvent être réservées "
+"Seuls les événements ouverts aux réservations internes peuvent être réservés "
 "par les opérateurs du cinéma"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:123
 msgid "Open for external booking"
 msgstr "Ouverte aux réservations externes"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:124
 msgid "Only external bookable sessions are visible to public for booking"
 msgstr ""
-"Seules les séances ouvertes aux réservations externes peuvent faire l'objet "
+"Seuls les événements ouverts aux réservations externes peuvent faire l'objet "
 "de demandes de réservations par les clients du site"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:128
 msgid "Movie theater comments"
 msgstr "Commentaires du cinéma"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:129
 msgid "These comments will be displayed to the users on booking form"
 msgstr ""
-"Ce commentaire sera visible sur le formulaire de réservation associé à cette "
-"séance"
+"Ce commentaire sera visible sur le formulaire de réservation associé à cet "
+"événement"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:132
 #: src/pyams_app_msc/feature/booking/interfaces.py:165
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:59
 #: src/pyams_app_msc/shared/theater/interfaces/audience.py:58
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:103
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:62
@@ -838,37 +838,37 @@
 msgstr ""
 "Vous pouvez sélectionner une activité présente au sein de votre catalogue, "
 "ou ne rien sélectionner si vous voulez simplement indiquer qu'une période "
 "n'est pas disponible pour d'autres activités"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:61
 msgid "New session"
-msgstr "Nouvelle séance"
+msgstr "Nouvel événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:62
 msgid "New session properties"
-msgstr "Propriétés de la séance"
+msgstr "Propriétés de l'événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:169
 msgid "Bookings"
 msgstr "Réservations"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:172
 msgid "Delete"
-msgstr "Supprimer la séance"
+msgstr "Supprimer l'événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:182
 msgid "Session planning"
-msgstr "Programmation d'une séance"
+msgstr "Programmation d'un événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:183
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:468
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:665
 msgid "Session properties"
-msgstr "Propriétés de la séance"
+msgstr "Propriétés de l'événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:230
 msgid "Out of catalog activity"
 msgstr "(activité hors-catalogue)"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:252
 msgid "You can't define a session gauge higher than the room's capacity!"
@@ -886,37 +886,37 @@
 msgstr "La salle indiquée est inconnue !"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:351
 msgid ""
 "Target room doesn't have enough capacity for confirmed seats of this session!"
 msgstr ""
 "La salle sélectionnée ne dispose pas d'une capacité suffisante pour "
-"accueillir les réservations confirmées à cette séance !"
+"accueillir les réservations confirmées à cet événement !"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:379
 msgid "Bad parameters"
 msgstr "Paramètres incorrects."
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:390
 msgid "Session updated"
 msgstr "Séance modifiée"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:391
 msgid "Session capacity has been reduced due to lower room capacity!"
 msgstr ""
-"La jauge de la séance a été réduite du fait de la capacité insuffisante de "
+"La jauge de l'événement a été réduite du fait de la capacité insuffisante de "
 "cette salle !"
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:64
 msgid "Planning"
 msgstr "Agenda"
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:76
 msgid "Sessions planning"
-msgstr "Agenda des séances programmées"
+msgstr "Agenda des événements programmés"
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:131
 msgid "Theater week"
 msgstr "Sem. ciné."
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:145
 msgid "Today"
@@ -957,15 +957,15 @@
 
 #: src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:42
 msgid "Manage event booking..."
 msgstr "Gérer les réservations"
 
 #: src/pyams_app_msc/feature/planning/zmi/templates/planning.pt:50
 msgid "Clone event..."
-msgstr "Dupliquer la séance"
+msgstr "Dupliquer l'événement"
 
 #: src/pyams_app_msc/feature/quotation/__init__.py:166
 msgid "QUOTATION"
 msgstr "DEVIS"
 
 #: src/pyams_app_msc/feature/quotation/__init__.py:194
 msgid "#Quotation:"
@@ -1137,31 +1137,31 @@
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
 msgstr "Participants"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:126
 msgid "Number of participants seats reserved for this session"
-msgstr "Nombre de places réservées pour les participants à cette séance"
+msgstr "Nombre de places réservées pour les participants à cet événement"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:130
 msgid "Accompanists"
 msgstr "Accompagnateurs"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:131
 msgid "Number of accompanists seats reserved for this session"
-msgstr "Nombre de places réservées pour les accompagnants à cette séance"
+msgstr "Nombre de places réservées pour les accompagnants à cet événement"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:135
 msgid "Groups count"
 msgstr "Nombre de groupes"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:136
 msgid "Number of groups or classrooms attending this session"
-msgstr "Nombre de groupes ou de classes participant à cette séance"
+msgstr "Nombre de groupes ou de classes participant à cet événement"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:141
 msgid "Price"
 msgstr "Tarif"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:142
 msgid "Price applied to this booking"
@@ -1211,27 +1211,27 @@
 msgstr "Archivée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:170
 msgid ""
 "A booking is archived automatically after session end and can't be modified "
 "anymore"
 msgstr ""
-"Une réservation est archivée automatiquement après la fin de la séance "
-"correspondante et ne peut plus être modifiée"
+"Une réservation est archivée automatiquement après la fin de l'événement "
+"correspondant et ne peut plus être modifiée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:187
 msgid "Quotation number"
 msgstr "Numéro de devis"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:188
 msgid "This is the reference number of the quotation"
 msgstr "Ceci est la référence du devis"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:191
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:744
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:748
 msgid "Quotation message"
 msgstr "Message associé au devis"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:192
 msgid "This message is added to quotation as an information message"
 msgstr "Ce message d'information est associé au devis envoyé au client"
 
@@ -1283,15 +1283,15 @@
 #: src/pyams_app_msc/feature/booking/interfaces.py:214
 msgid ""
 "If 'yes', a reminder message will be sent to the recipient a few days before "
 "the session take place; delay before session is defined into theater settings"
 msgstr ""
 "Si cette option est activée, un message de rappel sera envoyé au "
 "bénéficiaire de la réservations quelques heures ou jours avant le début de "
-"la séance ; ce délai est spécifié dans les paramètres du cinéma"
+"l'événement ; ce délai est spécifié dans les paramètres du cinéma"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:220
 #: src/pyams_app_msc/shared/theater/interfaces/mail.py:81
 msgid "Reminder subject"
 msgstr "Sujet des messages"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:221
@@ -1304,15 +1304,15 @@
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:225
 msgid ""
 "Reminder message will be sent to the recipient a few days before the session "
 "take place; delay before session is defined into theater settings"
 msgstr ""
 "Le message de rappel est envoyé au bénéficiaire quelques heures ou jours "
-"avant le début de la séance, en fonction du paramétrage appliqué au niveau "
+"avant le début de l'événement, en fonction du paramétrage appliqué au niveau "
 "du cinéma"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:230
 msgid "Reminder date"
 msgstr "Date du rappel"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:231
@@ -1324,15 +1324,15 @@
 #: src/pyams_app_msc/feature/booking/interfaces.py:263
 msgid "Free seats"
 msgstr "Places disponibles"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:264
 msgid "Number of free seats for this session"
 msgstr ""
-"Nombre de places encore disponibles pour cette séance ; seules les "
+"Nombre de places encore disponibles pour cet événement ; seules les "
 "réservations validées sont prises en compte, y compris cette réservation le "
 "cas échéant"
 
 #: src/pyams_app_msc/feature/booking/task.py:51
 msgid "Bookings archiver task"
 msgstr "Archivage des réservations"
 
@@ -1385,23 +1385,23 @@
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:167
 msgid "change-booking-session-menu"
 msgstr "Changer de séance"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:207
 msgid "Booking session"
-msgstr "Nouvelle séance"
+msgstr "Nouvel événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:208
 msgid "Select the session for which this booking is applied"
-msgstr "Nouvelle séance à laquelle doit s'appliquer la réservation"
+msgstr "Nouvel événement auquel doit s'appliquer la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:217
 msgid "Change session"
-msgstr "Changer la séance"
+msgstr "Changer d'événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:221
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:460
 msgid "Cancel"
 msgstr "Annuler"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:234
@@ -1409,124 +1409,124 @@
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:473
 #, python-format
 msgid "Booking: {}"
 msgstr "Réservation : {}"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:237
 msgid "Change booking session"
-msgstr "Changement de séance"
+msgstr "Changement d'événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:241
 msgid "No session selected, booking was not changed."
-msgstr "Aucune séance sélectionnée, la réservation n'a pas été modifiée."
+msgstr "Aucun événement sélectionné, la réservation n'a pas été modifiée."
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:296
 msgid "This booking is already registered for this session..."
-msgstr "Cette séance est déjà celle concernée par cette réservation."
+msgstr "Cet événement est déjà celle concerné par cette réservation."
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:303
 #, python-format
 msgid "There are only {} free seats left in this session!"
 msgstr ""
-"<strong>ATTENTION :</strong> il ne reste que {} places libres sur cette "
-"séance !"
+"<strong>ATTENTION :</strong> il ne reste que {} places libres sur cet "
+"événement !"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:370
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:485
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:489
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:477
 msgid "Booking properties"
 msgstr "Propriétés de la réservation"
 
 #. Default: Cancel booking
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:618
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:622
 msgid "cancel-booking-menu"
 msgstr "Annuler"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:628
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:632
 msgid "Cancel booking"
 msgstr "Annuler la réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:629
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:633
 msgid "Booking cancelled"
 msgstr "Réservation annulée"
 
 #. Default: Refuse booking
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:654
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:658
 msgid "refuse-booking-menu"
 msgstr "Refuser"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:664
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:668
 msgid "Refuse booking"
 msgstr "Refuser la réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:665
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:669
 msgid "Booking refused"
 msgstr "Réservation refusée"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:678
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:682
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:447
 msgid "Quotation preview"
 msgstr "Prévisualiser le devis"
 
 #. Default: Optional booking
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:697
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:701
 msgid "option-booking-menu"
 msgstr "Accepter (sous réserve)"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:707
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:711
 msgid "Optional booking"
 msgstr "Accepter la réservation (sous réserve de confirmation)"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:708
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:712
 msgid "Booking temporarily accepted"
 msgstr "Acceptée (sous réserve)"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:739
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:743
 msgid "Include quotation"
 msgstr "Inclure le devis"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:740
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:744
 msgid "Include quotation document into notification message"
 msgstr "Inclure le devis au format PDF dans le message de notification"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:745
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:749
 msgid "This message will be added to quotation"
 msgstr "Ce commentaire sera ajouté dans les éléments du devis"
 
 #. Default: Accept booking
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:765
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:769
 msgid "accept-booking-menu"
 msgstr "Accepter"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:775
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:779
 msgid "Accept booking"
 msgstr "Accepter la réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:776
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:780
 msgid "Booking accepted"
 msgstr "Réservation acceptée"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:822
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:826
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:653
 msgid "You must set a price to accept a booking!"
 msgstr "Vous devez spécifier un tarif pour pouvoir accepter une réservation !"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:904
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:908
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
 " &ast; **ATTENTION** &ast;<br />Le nombre de places encore disponibles sur "
-"cette séance n'est pas suffisant pour accueillir cette réservation !"
+"cet événement n'est pas suffisant pour accueillir cette réservation !"
 
-#: src/pyams_app_msc/feature/booking/zmi/workflow.py:923
+#: src/pyams_app_msc/feature/booking/zmi/workflow.py:927
 #, python-format
 msgid "The reminder delay is set to {} hours before session start."
 msgstr ""
 "Le message de rappel sera envoyé au bénéficiaire {} heures avant le début de "
-"la séance."
+"l'événement."
 
 #: src/pyams_app_msc/feature/booking/zmi/task.py:41
 msgid "Add booking archiver task..."
 msgstr "Archivage des réservations"
 
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:70
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:77
@@ -1592,15 +1592,15 @@
 #: src/pyams_app_msc/feature/booking/zmi/search.py:64
 #: src/pyams_app_msc/feature/booking/zmi/search.py:115
 msgid "Advanced search"
 msgstr "Recherche avancée"
 
 #: src/pyams_app_msc/feature/booking/zmi/search.py:78
 msgid "Session date"
-msgstr "Date de la séance"
+msgstr "Date de l'événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/search.py:84
 msgid "Modification date"
 msgstr "Date de modification"
 
 #: src/pyams_app_msc/feature/booking/zmi/search.py:87
 msgid "Include archives"
@@ -1629,15 +1629,15 @@
 
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:240
 msgid "Archived booking"
 msgstr "Réservation archivée"
 
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:276
 msgid "Current session bookings"
-msgstr "Réservations sur la séance"
+msgstr "Réservations sur l'événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:288
 msgid "Session bookings"
 msgstr "Gestion des réservations"
 
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:302
 #, python-format
@@ -1687,36 +1687,36 @@
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:807
 #, python-format
 msgid ""
 "Reminder message will be sent to booking recipient {} hours before session "
 "begin date..."
 msgstr ""
 "Le message de rappel sera envoyé au bénéficiaire {} heures avant le début de "
-"la séance."
+"l'événement."
 
 #: src/pyams_app_msc/feature/booking/zmi/__init__.py:822
 msgid "Quotation has been reset!"
 msgstr "Le devis a été re-généré !"
 
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:52
 msgid "${groups}: ${participants} participants, ${accompanists} accompanists"
 msgstr ""
 "${groups} : ${participants} participants, ${accompanists} accompagnateurs"
 
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:65
 msgid "There is no confirmed booking for this session."
-msgstr "Aucune réservation validée pour cette séance."
+msgstr "Aucune réservation validée pour cet événement."
 
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:73
 msgid "There is no session planned for today."
-msgstr "Aucune séance n'est programmée aujourd'hui."
+msgstr "Aucun événement n'est programmé aujourd'hui."
 
 #: src/pyams_app_msc/feature/booking/skin/__init__.py:50
 msgid "Session ID"
-msgstr "ID de la séance"
+msgstr "ID de l'événement"
 
 #: src/pyams_app_msc/feature/booking/skin/__init__.py:54
 msgid "You can add optional comments to your booking request"
 msgstr ""
 "Vous pouvez ajouter un commentaire afin de faciliter le traitement de votre "
 "demande. Pour toute question préalable, feuillez utiliser le formulaire de "
 "contact..."
@@ -1996,27 +1996,27 @@
 msgid "Catalog template configuration"
 msgstr "Modèle de présentation des entrées du catalogue"
 
 #: src/pyams_app_msc/shared/theater/zmi/presentation.py:67
 msgid "Catalog layout"
 msgstr "Mise en page"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:39
+#: src/pyams_app_msc/shared/theater/zmi/types.py:43
 msgid "Activity types"
 msgstr "Types d'activités"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:49
+#: src/pyams_app_msc/shared/theater/zmi/types.py:53
 msgid "Add activity type"
 msgstr "Ajouter un type d'activité"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:58
+#: src/pyams_app_msc/shared/theater/zmi/types.py:73
 msgid "Activities types"
 msgstr "Types d'activités"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:59
+#: src/pyams_app_msc/shared/theater/zmi/types.py:74
 msgid "Movie theater activities types list"
 msgstr "Liste des types d'activités"
 
 #: src/pyams_app_msc/shared/theater/zmi/viewlet.py:39
 msgid "My theaters"
 msgstr "Mes cinémas"
 
@@ -2123,31 +2123,35 @@
 msgid "Movie theater settings"
 msgstr "Paramètres du cinéma"
 
 #: src/pyams_app_msc/shared/theater/zmi/__init__.py:242
 msgid "Main theater settings"
 msgstr "Paramètres principaux"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:258
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:262
+msgid "Booking settings"
+msgstr "Gestion des réservations"
+
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:275
 msgid "Booking cancel mode"
 msgstr "Gestion des annulations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:274
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:289
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 "Le délai maximum après la réservation doit être indiqué pour utiliser ce "
 "mode d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:277
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:292
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
-"Le préavis minimum avant la séance doit être indiqué pour utiliser ce mode "
+"Le préavis minimum avant l'événement doit être indiqué pour utiliser ce mode "
 "d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:286
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:301
 msgid "Quotations settings"
 msgstr "Gestion des devis"
 
 #: src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr "Gestion des tarifs"
@@ -2285,16 +2289,16 @@
 
 #: src/pyams_app_msc/shared/theater/interfaces/mail.py:86
 msgid ""
 "This template is used for reminder messages which are sent to sessions "
 "recipients a few days before they take place"
 msgstr ""
 "Ce modèle est utilisé pour les messages de rappel qui peuvent être envoyés "
-"quelques jours avant les séances aux bénéficiaires dont les réservations ont "
-"été acceptées"
+"quelques jours avant les événements aux bénéficiaires dont les réservations "
+"ont été acceptées"
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:35
 msgid "Active room?"
 msgstr "Salle active ?"
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:36
 msgid "An inactive room can't be selected to assign new activities"
@@ -2320,23 +2324,23 @@
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:49
 msgid "Opening time"
 msgstr "Heure d'ouverture"
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:50
 msgid "First time available for sessions planning"
-msgstr "Heure à partir de laquelle des séances peuvent être programmées"
+msgstr "Heure à partir de laquelle des événements peuvent être programmés"
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:54
 msgid "Closing time"
 msgstr "Heure de fermeture"
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:55
 msgid "Last time available for sessions planning"
-msgstr "Heure jusqu'à laquelle des séances peuvent être programmées"
+msgstr "Heure jusqu'à laquelle des événements peuvent être programmés"
 
 #: src/pyams_app_msc/shared/theater/interfaces/room.py:60
 #: src/pyams_app_msc/shared/theater/interfaces/audience.py:59
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:63
 msgid "This comment is for internal use only"
 msgstr "Ce commentaire est à usage interne uniquement"
 
@@ -2518,54 +2522,54 @@
 msgstr "Durée des créneaux horaires"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:171
 msgid "Calendar time slots frequency in week or day views"
 msgstr ""
 "Indiquée en minutes, cette valeur indique la durée des créneaux horaires "
 "affichés dans les vues par semaine ou par jour de l'agenda ; vous pouvez "
-"toujours ajuster la durée des séances plus finement, si besoin, dans le "
-"formulaire de mise à jour des propriétés d'une séance"
+"toujours ajuster la durée des événements plus finement, si besoin, dans le "
+"formulaire de mise à jour des propriétés d'un événement"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:177
 msgid "Default session duration"
-msgstr "Durée de base des séances"
+msgstr "Durée de base des événements"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:178
 msgid ""
 "This is a default duration, in minutes, of sessions for which activity has "
 "no duration"
 msgstr ""
-"Cette durée, exprimée en minutes, est appliquée par défaut aux séances dont "
-"l'activité n'a pas de durée indiquée"
+"Cette durée, exprimée en minutes, est appliquée par défaut aux événements "
+"dont l'activité n'a pas de durée indiquée"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:183
 msgid "Session duration delta"
-msgstr "Temps minimum entre les séances"
+msgstr "Temps minimum entre les événements"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:184
 msgid ""
 "This is a number of minutes which will be added automatically to activities "
 "duration when adding new sessions"
 msgstr ""
 "Cette durée, exprimée en minutes, indique la durée qui sera ajoutée "
-"automatiquement à la durée des films pour définir la durée des séances "
-"proposées aux gestionnaires"
+"automatiquement à la durée des activités pour définir la durée des séances "
+"proposée aux gestionnaires"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:189
 msgid "Reminder delay"
 msgstr "Délai de rappel"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:190
 msgid ""
-"This is a delay, given in hours before a session beginning, at which a "
+"This is a delay, given in days before a session beginning, at which a "
 "reminder message can be sent to booking recipients; leave value empty or set "
 "it to 0 to disable reminders messages"
 msgstr ""
-"Ce délai, exprimé en heures, indique combien de temps avant le début d'une "
-"séance est attendu avant l'envoi d'un message de rappel aux bénéficiaires "
+"Ce délai, exprimé en jours, indique combien de temps avant le début d'une "
+"activité est attendu avant l'envoi d'un message de rappel aux bénéficiaires "
 "d'une réservation ; vous pouvez laisser cette valeur vide ou indiquer la "
 "valeur 0 si vous ne souhaitez pas envoyer de messages de rappel. ATTENTION : "
 "les réservations confirmées au-delà de ce délai ne feront pas l'objet de "
 "messages de rappel !"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:195
 msgid "User booking cancel mode"
@@ -2590,36 +2594,36 @@
 msgstr ""
 "Ce délai maximum, indiqué en heures, correspond à la durée pendant laquelle, "
 "après avoir déposé sa demande de réservation, un bénéficiaire peut encore "
 "annuler cette demande par lui-même, sans contacter le cinéma"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:209
 msgid "Cancel notice period"
-msgstr "Préavis minimum avant la séance"
+msgstr "Préavis minimum avant l'événement"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:210
 msgid ""
 "This is the minimum amount of time before session, given in hours, during "
 "which a principal can cancel a booking by it's own way"
 msgstr ""
 "Ce préavis, indiqué en heures, correspond à la durée minimale avant le début "
-"de la séance jusqu'à laquelle un bénéficiaire peut encore annuler cette "
+"de l'événement jusqu'à laquelle un bénéficiaire peut encore annuler cette "
 "demande par lui-même, sans contacter le cinéma"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:216
 msgid "Booking retention duration"
 msgstr "Durée de rétention des réservations"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:217
 msgid ""
 "This is the minimum amount of time, given in hours, during which a a booking "
 "is kept 'active' before being archived"
 msgstr ""
 "Ceci est la durée minimale, indiquée en heures, avant qu'une réservation "
-"associée à une séance terminée soit archivée automatiquement"
+"associée à un événement terminé ne soit archivée automatiquement"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:223
 msgid "Quotation number format"
 msgstr "Format des numéros de devis"
 
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:224
 #, python-format
@@ -2848,15 +2852,15 @@
 msgid "Display free seats"
 msgstr "Afficher les places libres"
 
 #: src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py:40
 msgid "If 'no', number of free seats is not displayed"
 msgstr "Si 'non', le nombre de places libres ne sera pas affiché"
 
-#: src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py:64
+#: src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py:65
 msgid "Catalog entries with next planned sessions"
 msgstr "Entrées du catalogue avec les prochaines séances"
 
 #: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:62
 msgid "${seats} seats"
 msgstr "${seats} places"
 
@@ -2953,15 +2957,14 @@
 #: src/pyams_app_msc/root/interfaces.py:32
 msgid ""
 "These principals are allowed to create and manage sites and movie theaters"
 msgstr ""
 "Ces mandataires peuvent procéder à la création d'un nouveau cinéma et nommer "
 "ses gestionnaires"
 
-#, fuzzy
 #~ msgid "Display all booked seats"
 #~ msgstr "Afficher les places libres"
 
 #~ msgid "Preferred audiences"
 #~ msgstr "Publics privilégiés"
 
 #~ msgid "Movie theater comment"
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/locales/pyams_app_msc.pot` & `pyams_app_msc-1.99.1/src/pyams_app_msc/locales/pyams_app_msc.pot`

 * *Files 0% similar despite different names*

```diff
@@ -2,85 +2,85 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-02-26 22:18+0100\n"
+"POT-Creation-Date: 2024-03-24 03:43+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
-#: ./src/pyams_app_msc/include.py:48
+#: ./src/pyams_app_msc/include.py:53
 msgid "Manage movie theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:52
+#: ./src/pyams_app_msc/include.py:57
 msgid "View movie theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:56
+#: ./src/pyams_app_msc/include.py:61
 msgid "Manage movie theater activities catalog"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:60
+#: ./src/pyams_app_msc/include.py:65
 msgid "Read movie theater activities catalog"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:64
+#: ./src/pyams_app_msc/include.py:69
 msgid "Create booking request for movie theater activity"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:68
+#: ./src/pyams_app_msc/include.py:73
 msgid "View sessions planning on movie theater activities"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:72
+#: ./src/pyams_app_msc/include.py:77
 msgid "Manage sessions planning on movie theater activities"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:76
+#: ./src/pyams_app_msc/include.py:81
 msgid "View booking information for movie theater activity"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:80
+#: ./src/pyams_app_msc/include.py:85
 msgid "Manage bookings for movie theater activity"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:103
+#: ./src/pyams_app_msc/include.py:108
 msgid "MSC: Sites manager"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:115
+#: ./src/pyams_app_msc/include.py:120
 msgid "MSC: Theater manager"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:134
+#: ./src/pyams_app_msc/include.py:139
 msgid "MSC: Theater operator"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:152
+#: ./src/pyams_app_msc/include.py:157
 msgid "MSC: Contributor"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:169
+#: ./src/pyams_app_msc/include.py:174
 msgid "MSC: Theater consultant"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:184
+#: ./src/pyams_app_msc/include.py:189
 msgid "MSC: Theater client"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:196
+#: ./src/pyams_app_msc/include.py:201
 msgid "MSC: Reservation owner"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/tmdb/interfaces.py:41
 msgid "Enable TMDB configuration"
 msgstr ""
 
@@ -584,23 +584,23 @@
 
 #: ./src/pyams_app_msc/feature/messaging/interfaces.py:50
 msgid ""
 "This prefix, if any, will be used as subject prefix to all sent email "
 "messages"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:41
+#: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:43
 msgid "Messaging settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:51
+#: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:53
 msgid "Messaging service settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:52
+#: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/session.py:156
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
 msgid "{room} - {date} from {start_time} to {end_time}"
@@ -1135,15 +1135,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:188
 msgid "This is the reference number of the quotation"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:191
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:744
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:748
 msgid "Quotation message"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:192
 msgid "This message is added to quotation as an information message"
 msgstr ""
 
@@ -1317,99 +1317,99 @@
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:303
 #, python-format
 msgid "There are only {} free seats left in this session!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:370
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:485
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:489
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:477
 msgid "Booking properties"
 msgstr ""
 
 #. Default: Cancel booking
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:618
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:622
 msgid "cancel-booking-menu"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:628
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:632
 msgid "Cancel booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:629
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:633
 msgid "Booking cancelled"
 msgstr ""
 
 #. Default: Refuse booking
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:654
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:658
 msgid "refuse-booking-menu"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:664
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:668
 msgid "Refuse booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:665
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:669
 msgid "Booking refused"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:678
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:682
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:447
 msgid "Quotation preview"
 msgstr ""
 
 #. Default: Optional booking
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:697
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:701
 msgid "option-booking-menu"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:707
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:711
 msgid "Optional booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:708
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:712
 msgid "Booking temporarily accepted"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:739
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:743
 msgid "Include quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:740
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:744
 msgid "Include quotation document into notification message"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:745
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:749
 msgid "This message will be added to quotation"
 msgstr ""
 
 #. Default: Accept booking
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:765
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:769
 msgid "accept-booking-menu"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:775
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:779
 msgid "Accept booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:776
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:780
 msgid "Booking accepted"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:822
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:826
 #: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:653
 msgid "You must set a price to accept a booking!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:904
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:908
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:923
+#: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:927
 #, python-format
 msgid "The reminder delay is set to {} hours before session start."
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/task.py:41
 msgid "Add booking archiver task..."
 msgstr ""
@@ -1852,27 +1852,27 @@
 msgid "Catalog template configuration"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/presentation.py:67
 msgid "Catalog layout"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:39
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:43
 msgid "Activity types"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:49
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:53
 msgid "Add activity type"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:58
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:73
 msgid "Activities types"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:59
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:74
 msgid "Movie theater activities types list"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/viewlet.py:39
 msgid "My theaters"
 msgstr ""
 
@@ -1979,27 +1979,31 @@
 msgid "Movie theater settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:242
 msgid "Main theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:258
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:262
+msgid "Booking settings"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:275
 msgid "Booking cancel mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:274
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:289
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:277
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:292
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:286
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:301
 msgid "Quotations settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr ""
@@ -2363,15 +2367,15 @@
 
 #: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:189
 msgid "Reminder delay"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:190
 msgid ""
-"This is a delay, given in hours before a session beginning, at which a "
+"This is a delay, given in days before a session beginning, at which a "
 "reminder message can be sent to booking recipients; leave value empty or set "
 "it to 0 to disable reminders messages"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:195
 msgid "User booking cancel mode"
 msgstr ""
@@ -2621,15 +2625,15 @@
 msgid "Display free seats"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py:40
 msgid "If 'no', number of free seats is not displayed"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py:64
+#: ./src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py:65
 msgid "Catalog entries with next planned sessions"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:62
 msgid "${seats} seats"
 msgstr ""
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/reference/zmi/viewlet.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/root/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/api/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/index.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/index.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/manager.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/page.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/search.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/skin/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from pyams_app_msc.shared.theater import IMovieTheater
 from pyams_content.shared.common.zmi import SharedContentAddAction, SharedContentAddForm
 from pyams_content.shared.common.zmi.types.content import TypedSharedContentCustomInfoEditForm, \
     TypedSharedContentPropertiesEditForm
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.browser.select import SelectWidget
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IAJAXFormRenderer
+from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent
 from pyams_form.widget import FieldWidget
 from pyams_i18n.interfaces import INegotiator
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces import IViewContextPermissionChecker
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_skin.interfaces.widget import IDynamicSelectWidget
 from pyams_utils.adapter import NullAdapter, adapter_config
@@ -187,24 +187,27 @@
     def fields(self):
         """Form fields getter"""
         datatype = self.datatype
         if datatype is None:
             return Fields(Interface)
         return Fields(ICatalogEntryInfo).select(*datatype.field_names)
 
-    def get_content(self):
-        """Form content getter"""
-        return ICatalogEntryInfo(self.context)
-
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         synopsis = self.widgets.get('synopsis')
         if synopsis is not None:
             synopsis.add_class('h-200px')
 
 
+@adapter_config(required=(IWfCatalogEntry, IPyAMSLayer, CatalogEntryInformationEditForm),
+                provides=IFormContent)
+def catalog_entry_info_edit_form_content(context, request, form):
+    """Catalog entry information edit form content getter"""
+    return ICatalogEntryInfo(context)
+
+
 @adapter_config(required=(ICatalogEntryInfo, IAdminLayer, CatalogEntryInformationEditForm),
                 provides=IViewContextPermissionChecker)
 def catalog_entry_info_permission_checker(context, request, view):
     """Catalog entry activity info permission checker"""
     catalog_entry = get_parent(context, IWfCatalogEntry)
     return IViewContextPermissionChecker(catalog_entry)
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/dashboard.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/catalog/zmi/workflow.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/common/zmi/viewlet.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/site/zmi/viewlet.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/price.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/api/schema.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/audience.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     session_duration_delta = Int(title=_("Session duration delta"),
                                  description=_("This is a number of minutes which will be added automatically "
                                                "to activities duration when adding new sessions"),
                                  required=False,
                                  default=0)
 
     reminder_delay = Int(title=_("Reminder delay"),
-                         description=_("This is a delay, given in hours before a session beginning, at which "
+                         description=_("This is a delay, given in days before a session beginning, at which "
                                        "a reminder message can be sent to booking recipients; leave value "
                                        "empty or set it to 0 to disable reminders messages"),
                          required=False)
 
     booking_cancel_mode = Choice(title=_("User booking cancel mode"),
                                  description=_("This mode determines how and when a principal can cancel "
                                                "a booking by it's own way"),
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/audience.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/mail.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/price.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/interfaces/room.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/mail.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/page.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/price.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/room.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/session.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/settings.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pyams_app_msc.shared.theater.interfaces import BOOKING_CANCEL_MODE
 from pyams_content.interfaces import IBaseContent, MANAGE_SITE_TREE_PERMISSION
 from pyams_content.root.zmi.sites import SiteRootSitesTable
 from pyams_content.zmi.properties import PropertiesEditForm
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.group import Group
-from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IGroup
+from pyams_form.interfaces.form import IAJAXFormRenderer, IDataExtractedEvent, IFormContent, IGroup
 from pyams_i18n.interfaces import II18n, INegotiator
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_site.interfaces import ISiteRoot
 from pyams_skin.interfaces.viewlet import IBreadcrumbItem
 from pyams_skin.viewlet.breadcrumb import BreadcrumbItem
 from pyams_skin.viewlet.menu import MenuDivider, MenuItem
@@ -241,32 +241,47 @@
     title = _("Movie theater settings")
     legend = _("Main theater settings")
 
     fields = Fields(IMovieTheaterSettings).select('calendar_slot_duration',
                                                   'default_session_duration',
                                                   'session_duration_delta')
 
-    def get_content(self):
-        return IMovieTheaterSettings(self.context)
+
+@adapter_config(required=(IMovieTheater, IPyAMSLayer, MovieTheaterSettingsEditForm),
+                provides=IFormContent)
+def movie_theater_settings_edit_form_content(context, request, form):
+    """Movie theater settings edit form content getter"""
+    return IMovieTheaterSettings(context)
+
+
+@adapter_config(name='',
+                required=(IMovieTheater, IAdminLayer, MovieTheaterSettingsEditForm),
+                provides=IGroup)
+class MovieTheaterSettingsBookingGroup(Group):
+    """Movie theater settings booking group"""
+
+    legend = _("Booking settings")
+
+    fields = Fields(IMovieTheaterSettings).select('reminder_delay',
+                                                  'booking_retention_duration')
+    weight = 10
 
 
 @adapter_config(name='booking-cancel-mode.group',
                 required=(IMovieTheater, IAdminLayer, MovieTheaterSettingsEditForm),
                 provides=IGroup)
 class MovieTheaterSettingsBookingCancelModeGroup(Group):
     """Movie theater settings booking cancel mode"""
 
     legend = _("Booking cancel mode")
 
-    fields = Fields(IMovieTheaterSettings).select('reminder_delay',
-                                                  'booking_cancel_mode',
+    fields = Fields(IMovieTheaterSettings).select('booking_cancel_mode',
                                                   'booking_cancel_max_delay',
-                                                  'booking_cancel_notice_period',
-                                                  'booking_retention_duration')
-    weight = 10
+                                                  'booking_cancel_notice_period')
+    weight = 20
 
 
 @subscriber(IDataExtractedEvent, form_selector=MovieTheaterSettingsBookingCancelModeGroup)
 def handle_booking_cancel_mode(event):
     """Handle booking cancel mode"""
     data = event.data
     if (data.get('booking_cancel_mode') == BOOKING_CANCEL_MODE.MAX_DELAY.value) and \
@@ -283,15 +298,15 @@
 class MovieTheaterSettingsQuotationsGroup(Group):
     """Movie theater quotations settings group"""
 
     legend = _("Quotations settings")
 
     fields = Fields(IMovieTheaterSettings).select('quotation_number_format', 'quotation_logo',
                                                   'quotation_color', 'currency', 'vat_rate')
-    weight = 20
+    weight = 30
 
 
 @adapter_config(required=(IMovieTheater, IAdminLayer, MovieTheaterSettingsQuotationsGroup),
                 provides=IAJAXFormRenderer)
 class MovieTheaterSettingsQuotationsGroupRenderer(AJAXFormRenderer):
     """Movie theater quotations settings group renderer"""
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/audience.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/interfaces.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/mail.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/planning.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/planning.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/presentation.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/presentation.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/price.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/room.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/search.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/session.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/shared/theater/zmi/viewlet.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/form.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/form.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/layer.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/login.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/login.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_form.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_form.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_gis.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_gis.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_search.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_search.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/_utils.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_utils.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/js/app.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/app.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_content.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_content.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_footer.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_footer.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_forms.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_forms.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_layout.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_misc.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_misc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/_variables.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/resources/src/sass/msc.scss` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/msc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/skin/templates/select-admin-theater.pt` & `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/templates/select-admin-theater.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/test_utilsdocs.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/tests/test_utilsdocstrings.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/__init__.py` & `pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/resources/js/msc.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc/zmi/resources/js/msc.min.js` & `pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.min.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/PKG-INFO` & `pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyams-app-msc
-Version: 1.99.0.1
+Version: 1.99.1
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
@@ -38,23 +37,30 @@
 is available on `Gitlab <https://gitlab.com/pyams>`_ and pushed to `Github
 <https://github.com/py-ams>`_. Doctests are available in the *doctests* source folder.
 
 
 What is PyAMS MSC application?
 ==============================
 
-PyAMS MSC application is a french web application ("Ma Sortie Cinéma") which is used to manage sessions
+PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - added edit forms content getters
+ - added custom catalog entry roles adapters
+ - removed roles restrictions menu entries from theater navigation menu
+ - removed source folder from movie theater activity types properties (issue #6)
+ - changed reminder delay unit from hours to days (issue #4]
+ - updated theater settings edit form (issue #4)
+
 1.99.0.1
 --------
  - fixed packaging issue
 
 1.99.0
 ------
  - first preliminary release
-
-
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/SOURCES.txt` & `pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
 src/pyams_app_msc/shared/__init__.py
 src/pyams_app_msc/shared/catalog/__init__.py
 src/pyams_app_msc/shared/catalog/index.py
 src/pyams_app_msc/shared/catalog/interfaces.py
 src/pyams_app_msc/shared/catalog/manager.py
 src/pyams_app_msc/shared/catalog/page.py
 src/pyams_app_msc/shared/catalog/search.py
+src/pyams_app_msc/shared/catalog/security.py
 src/pyams_app_msc/shared/catalog/api/__init__.py
 src/pyams_app_msc/shared/catalog/portlet/__init__.py
 src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
 src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
 src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
 src/pyams_app_msc/shared/catalog/skin/__init__.py
 src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
@@ -242,14 +243,15 @@
 src/pyams_app_msc/shared/theater/zmi/__init__.py
 src/pyams_app_msc/shared/theater/zmi/audience.py
 src/pyams_app_msc/shared/theater/zmi/interfaces.py
 src/pyams_app_msc/shared/theater/zmi/mail.py
 src/pyams_app_msc/shared/theater/zmi/planning.py
 src/pyams_app_msc/shared/theater/zmi/presentation.py
 src/pyams_app_msc/shared/theater/zmi/price.py
+src/pyams_app_msc/shared/theater/zmi/restrictions.py
 src/pyams_app_msc/shared/theater/zmi/room.py
 src/pyams_app_msc/shared/theater/zmi/search.py
 src/pyams_app_msc/shared/theater/zmi/session.py
 src/pyams_app_msc/shared/theater/zmi/types.py
 src/pyams_app_msc/shared/theater/zmi/viewlet.py
 src/pyams_app_msc/skin/__init__.py
 src/pyams_app_msc/skin/form.py
```

### Comparing `pyams_app_msc-1.99.0.1/src/pyams_app_msc.egg-info/requires.txt` & `pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 persistent
 pillow
 pyams_catalog
 pyams_content
 pyams_content_api
 pyams_content_es
 pyams_file
-pyams_form
+pyams_form>=2.1.0
 pyams_i18n
 pyams_layer
 pyams_mail
 pyams_pagelet
 pyams_portal
 pyams_scheduler
 pyams_security>=2.2.1
```

