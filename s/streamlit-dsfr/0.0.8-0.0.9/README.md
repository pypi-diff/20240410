# Comparing `tmp/streamlit-dsfr-0.0.8.tar.gz` & `tmp/streamlit-dsfr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-dsfr-0.0.8.tar", last modified: Fri Jan 26 11:01:04 2024, max compression
+gzip compressed data, was "streamlit-dsfr-0.0.9.tar", last modified: Fri Feb  2 09:50:32 2024, max compression
```

## Comparing `streamlit-dsfr-0.0.8.tar` & `streamlit-dsfr-0.0.9.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/
--rw-r--r--   0 root         (0) root         (0)       44 2024-01-26 11:00:08.000000 streamlit-dsfr-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1207 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2024-01-26 11:00:08.000000 streamlit-dsfr-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-26 11:00:08.000000 streamlit-dsfr-0.0.8/VERSION
--rw-r--r--   0 root         (0) root         (0)      855 2024-01-26 11:00:08.000000 streamlit-dsfr-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/
--rw-r--r--   0 root         (0) root         (0)    29608 2024-01-26 11:00:14.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.322528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_alert/
--rw-r--r--   0 root         (0) root         (0)     4448 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_alert/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_badge/
--rw-r--r--   0 root         (0) root         (0)     4448 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_badge/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_breadcrumb/
--rw-r--r--   0 root         (0) root         (0)     4458 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_breadcrumb/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_button/
--rw-r--r--   0 root         (0) root         (0)     4449 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_button/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_checkbox/
--rw-r--r--   0 root         (0) root         (0)     4551 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_checkbox/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.326527 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.334528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/
--rw-r--r--   0 root         (0) root         (0)      914 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrAlert.tFZy4mCO.js
--rw-r--r--   0 root         (0) root         (0)      914 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBadge.gLg-CXXd.js
--rw-r--r--   0 root         (0) root         (0)      929 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBreadcrumb.79FUC984.js
--rw-r--r--   0 root         (0) root         (0)     1630 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButton.5AkE1u2l.js
--rw-r--r--   0 root         (0) root         (0)     1735 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrCheckbox.TNj2wexB.js
--rw-r--r--   0 root         (0) root         (0)     1405 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFileUpload.IdR5fkhs.js
--rw-r--r--   0 root         (0) root         (0)     2136 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFooter.so92d35v.js
--rw-r--r--   0 root         (0) root         (0)     1794 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrInput.PfsGa47n.js
--rw-r--r--   0 root         (0) root         (0)     1001 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrPicture.BG7gzqcn.js
--rw-r--r--   0 root         (0) root         (0)     1545 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRadioButtonSet.j3YqEKSL.js
--rw-r--r--   0 root         (0) root         (0)     1797 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRange.WiM63mXm.js
--rw-r--r--   0 root         (0) root         (0)    52216 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.Lusn3uPo.woff
--rw-r--r--   0 root         (0) root         (0)    42092 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.mI04Wx9M.woff2
--rw-r--r--   0 root         (0) root         (0)    56436 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.VpzzqYz6.woff
--rw-r--r--   0 root         (0) root         (0)    45300 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.alvVdTYc.woff2
--rw-r--r--   0 root         (0) root         (0)    50440 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.6lmsSnc8.woff
--rw-r--r--   0 root         (0) root         (0)    41368 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.7GX88oPX.woff2
--rw-r--r--   0 root         (0) root         (0)    43916 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.GJ3thv45.woff2
--rw-r--r--   0 root         (0) root         (0)    54492 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.STgl0sbt.woff
--rw-r--r--   0 root         (0) root         (0)    41940 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.A6bVQEda.woff2
--rw-r--r--   0 root         (0) root         (0)    51292 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.prCK3SSS.woff
--rw-r--r--   0 root         (0) root         (0)    44572 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.FqmRU-8D.woff2
--rw-r--r--   0 root         (0) root         (0)    54680 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.T_DBs5K5.woff
--rw-r--r--   0 root         (0) root         (0)    51140 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.8SHksZge.woff
--rw-r--r--   0 root         (0) root         (0)    41328 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.mgqq5yTO.woff2
--rw-r--r--   0 root         (0) root         (0)    44284 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.3R_BbTaN.woff2
--rw-r--r--   0 root         (0) root         (0)    54328 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.UCbE0jax.woff
--rw-r--r--   0 root         (0) root         (0)   114508 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.FN9ubN3N.woff
--rw-r--r--   0 root         (0) root         (0)    80368 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.gs3wZvgE.woff2
--rw-r--r--   0 root         (0) root         (0)   114016 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.9CKHJdJx.woff
--rw-r--r--   0 root         (0) root         (0)    79472 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.D5gUInLE.woff2
--rw-r--r--   0 root         (0) root         (0)   235463 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/StreamlitVue.ZFQEvSxb.js
--rw-r--r--   0 root         (0) root         (0)      779 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/client.t80Hv_Jg.js
--rw-r--r--   0 root         (0) root         (0)   810231 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/index.O_j7wwKi.css
--rw-r--r--   0 root         (0) root         (0)    70486 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/runtime-dom.esm-bundler.xzzcc6UT.js
--rw-r--r--   0 root         (0) root         (0)      137 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_alert.x0NNfw9T.css
--rw-r--r--   0 root         (0) root         (0)       98 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_checkbox._xlQgrDX.css
--rw-r--r--   0 root         (0) root         (0)      117 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_input.S6zC6ajS.css
--rw-r--r--   0 root         (0) root         (0)       76 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_picture.wTCAjD5j.css
--rw-r--r--   0 root         (0) root         (0)      203 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_radio.owPTSQFN.css
--rw-r--r--   0 root         (0) root         (0)      208 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_range.OgT-Uti3.css
--rw-r--r--   0 root         (0) root         (0)      330 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.334528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_file_upload/
--rw-r--r--   0 root         (0) root         (0)     4458 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_file_upload/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_footer/
--rw-r--r--   0 root         (0) root         (0)     4450 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_footer/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_input/
--rw-r--r--   0 root         (0) root         (0)     4564 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_input/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_picture/
--rw-r--r--   0 root         (0) root         (0)     4527 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_picture/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_radio/
--rw-r--r--   0 root         (0) root         (0)     4667 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_radio/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_range/
--rw-r--r--   0 root         (0) root         (0)     4655 2024-01-26 11:00:57.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_range/index.html
--rw-r--r--   0 root         (0) root         (0)     3443 2024-01-26 11:00:08.000000 streamlit-dsfr-0.0.8/streamlit_dsfr/override_font_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 11:01:04.338528 streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1207 2024-01-26 11:01:04.000000 streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4034 2024-01-26 11:01:04.000000 streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 11:01:04.000000 streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      140 2024-01-26 11:01:04.000000 streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-01-26 11:01:04.000000 streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-02-02 09:49:33.000000 streamlit-dsfr-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2024-02-02 09:49:33.000000 streamlit-dsfr-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2024-02-02 09:49:33.000000 streamlit-dsfr-0.0.9/VERSION
+-rw-r--r--   0 root         (0) root         (0)      855 2024-02-02 09:49:33.000000 streamlit-dsfr-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/
+-rw-r--r--   0 root         (0) root         (0)    33557 2024-02-02 09:49:40.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.438500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_alert/
+-rw-r--r--   0 root         (0) root         (0)     4448 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_alert/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_badge/
+-rw-r--r--   0 root         (0) root         (0)     4448 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_badge/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_breadcrumb/
+-rw-r--r--   0 root         (0) root         (0)     4458 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_breadcrumb/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_button/
+-rw-r--r--   0 root         (0) root         (0)     4449 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_button/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_buttons_group/
+-rw-r--r--   0 root         (0) root         (0)     4460 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_buttons_group/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_checkbox/
+-rw-r--r--   0 root         (0) root         (0)     4551 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_checkbox/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.442499 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/
+-rw-r--r--   0 root         (0) root         (0)      914 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrAlert.qHAssOJm.js
+-rw-r--r--   0 root         (0) root         (0)      914 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBadge.U7kOfHPN.js
+-rw-r--r--   0 root         (0) root         (0)      929 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBreadcrumb.24AdnYLs.js
+-rw-r--r--   0 root         (0) root         (0)     1488 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButton.F0Lzs9zA.js
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButtonGroup.MtpDLhtp.js
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrCheckbox.HBUYPhr5.js
+-rw-r--r--   0 root         (0) root         (0)     1405 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFileUpload.Qd737a0v.js
+-rw-r--r--   0 root         (0) root         (0)     2136 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFooter.vqQJXfur.js
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrInput.DWr3u8eg.js
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrPicture.vdniiHOI.js
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRadioButtonSet.I8DloxHK.js
+-rw-r--r--   0 root         (0) root         (0)     1797 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRange.uSCKVJAW.js
+-rw-r--r--   0 root         (0) root         (0)    52216 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.Lusn3uPo.woff
+-rw-r--r--   0 root         (0) root         (0)    42092 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.mI04Wx9M.woff2
+-rw-r--r--   0 root         (0) root         (0)    56436 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.VpzzqYz6.woff
+-rw-r--r--   0 root         (0) root         (0)    45300 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.alvVdTYc.woff2
+-rw-r--r--   0 root         (0) root         (0)    50440 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.6lmsSnc8.woff
+-rw-r--r--   0 root         (0) root         (0)    41368 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.7GX88oPX.woff2
+-rw-r--r--   0 root         (0) root         (0)    43916 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.GJ3thv45.woff2
+-rw-r--r--   0 root         (0) root         (0)    54492 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.STgl0sbt.woff
+-rw-r--r--   0 root         (0) root         (0)    41940 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.A6bVQEda.woff2
+-rw-r--r--   0 root         (0) root         (0)    51292 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.prCK3SSS.woff
+-rw-r--r--   0 root         (0) root         (0)    44572 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.FqmRU-8D.woff2
+-rw-r--r--   0 root         (0) root         (0)    54680 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.T_DBs5K5.woff
+-rw-r--r--   0 root         (0) root         (0)    51140 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.8SHksZge.woff
+-rw-r--r--   0 root         (0) root         (0)    41328 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.mgqq5yTO.woff2
+-rw-r--r--   0 root         (0) root         (0)    44284 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.3R_BbTaN.woff2
+-rw-r--r--   0 root         (0) root         (0)    54328 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.UCbE0jax.woff
+-rw-r--r--   0 root         (0) root         (0)   114508 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.FN9ubN3N.woff
+-rw-r--r--   0 root         (0) root         (0)    80368 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.gs3wZvgE.woff2
+-rw-r--r--   0 root         (0) root         (0)   114016 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.9CKHJdJx.woff
+-rw-r--r--   0 root         (0) root         (0)    79472 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.D5gUInLE.woff2
+-rw-r--r--   0 root         (0) root         (0)   237284 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/StreamlitVue.CglRiHNi.js
+-rw-r--r--   0 root         (0) root         (0)      779 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/client.forxb5ot.js
+-rw-r--r--   0 root         (0) root         (0)   810231 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/index.O_j7wwKi.css
+-rw-r--r--   0 root         (0) root         (0)    70486 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/runtime-dom.esm-bundler.CLhb1nSG.js
+-rw-r--r--   0 root         (0) root         (0)      137 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_alert.x0NNfw9T.css
+-rw-r--r--   0 root         (0) root         (0)       98 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_checkbox._xlQgrDX.css
+-rw-r--r--   0 root         (0) root         (0)      134 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_input.sx26c0dS.css
+-rw-r--r--   0 root         (0) root         (0)       76 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_picture.wTCAjD5j.css
+-rw-r--r--   0 root         (0) root         (0)      203 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_radio.owPTSQFN.css
+-rw-r--r--   0 root         (0) root         (0)      208 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_range.OgT-Uti3.css
+-rw-r--r--   0 root         (0) root         (0)      330 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_file_upload/
+-rw-r--r--   0 root         (0) root         (0)     4458 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_file_upload/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_footer/
+-rw-r--r--   0 root         (0) root         (0)     4450 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_footer/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_input/
+-rw-r--r--   0 root         (0) root         (0)     4581 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_input/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_picture/
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_picture/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_radio/
+-rw-r--r--   0 root         (0) root         (0)     4667 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_radio/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_range/
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-02-02 09:50:25.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_range/index.html
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-02-02 09:49:33.000000 streamlit-dsfr-0.0.9/streamlit_dsfr/override_font_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:50:32.458500 streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-02-02 09:50:32.000000 streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4166 2024-02-02 09:50:32.000000 streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 09:50:32.000000 streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2024-02-02 09:50:32.000000 streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-02-02 09:50:32.000000 streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/top_level.txt
```

### Comparing `streamlit-dsfr-0.0.8/PKG-INFO` & `streamlit-dsfr-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-dsfr
-Version: 0.0.8
+Version: 0.0.9
 Summary: VueDsfr components for Streamlit
 Author-email: Matiboux <matiboux@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
```

### Comparing `streamlit-dsfr-0.0.8/README.md` & `streamlit-dsfr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/pyproject.toml` & `streamlit-dsfr-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/__init__.py` & `streamlit-dsfr-0.0.9/streamlit_dsfr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 supported_components = {
     'dsfr_default': 'st_dsfr_default',
     'dsfr_alert': 'st_dsfr_alert',
     'dsfr_badge': 'st_dsfr_badge',
     'dsfr_breadcrumb': 'st_dsfr_breadcrumb',
     'dsfr_button': 'st_dsfr_button',
+    'dsfr_buttons_group': 'st_dsfr_buttons_group',
 	'dsfr_checkbox': 'st_dsfr_checkbox',
 	'dsfr_file_upload': 'st_dsfr_file_upload',
     'dsfr_input': 'st_dsfr_input',
 	'dsfr_picture': 'st_dsfr_picture',
     'dsfr_radio': 'st_dsfr_radio',
 	'dsfr_range': 'st_dsfr_range',
 }
@@ -174,15 +175,15 @@
 	if disabled is not None:
 		kwargs['disabled'] = disabled
 
 	if type is not None:
 		if type == 'secondary':
 			kwargs['secondary'] = True
 		elif type == 'tertiary':
-			kwargs['secondary'] = True
+			kwargs['tertiary'] = True
 	else:
 		if secondary is not None:
 			kwargs['secondary'] = secondary
 		if tertiary is not None:
 			kwargs['tertiary'] = tertiary
 
 	if icon is not None:
@@ -247,14 +248,157 @@
 		disabled = disabled,
 		use_container_width = use_container_width,
 		copy = content,
 	)
 
 dsfr_copy_button = copy_button
 
+def buttons_group(
+	labels: Iterable[str],
+	key: Optional[Union[str, int]] = None,
+	inline: Optional[bool] = None,
+	size: Optional[str] = None,
+	*,
+	disabled: Union[Optional[bool], list[Optional[bool]]] = None,
+	# Buttons
+	type: Union[Optional[str], list[Optional[str]]] = None,
+	secondary: Union[Optional[bool], list[Optional[bool]]] = None,
+	tertiary: Union[Optional[bool], list[Optional[bool]]] = None,
+	icon: Union[Optional[str], list[Optional[str]]] = None,
+	iconOnly: Union[Optional[bool], list[Optional[bool]]] = None,
+	noOutline: Union[Optional[bool], list[Optional[bool]]] = None,
+	link: Union[Optional[str], list[Optional[str]]] = None,
+	copy: Union[Optional[str], list[Optional[str]]] = None,
+	# Group
+	align: Optional[str] = None,
+	reverse: Optional[bool] = None,
+	iconRight: Optional[bool] = None,
+	equisized: Optional[bool] = None,
+	**kwargs,
+):
+	"""
+	Streamlit DSFR Button component
+
+	Streamlit standard component equivalent:
+	https://docs.streamlit.io/library/api-reference/widgets/st.button
+	"""
+
+	buttons = []
+
+	if isinstance(labels, str):
+		labels = [labels]
+	for label in labels:
+		buttons.append({
+			'label': label,
+		})
+
+	if type is not None:
+		if isinstance(type, list):
+			for i, each in enumerate(type):
+				if each == 'secondary':
+					kwargs['secondary'] = True
+				elif each == 'tertiary':
+					kwargs['tertiary'] = True
+		else:
+			for button in buttons:
+				if type == 'secondary':
+					kwargs['secondary'] = True
+				elif type == 'tertiary':
+					kwargs['tertiary'] = True
+	else:
+		if secondary is not None:
+			if isinstance(secondary, list):
+				for i, each in enumerate(secondary):
+					if each is not None:
+						buttons[i]['secondary'] = each
+			else:
+				for button in buttons:
+					button['secondary'] = secondary
+		if tertiary is not None:
+			if isinstance(tertiary, list):
+				for i, each in enumerate(tertiary):
+					if each is not None:
+						buttons[i]['tertiary'] = each
+			else:
+				for button in buttons:
+					button['tertiary'] = tertiary
+
+	if disabled is not None:
+		if isinstance(disabled, list):
+			for i, each in enumerate(disabled):
+				if each is not None:
+					buttons[i]['disabled'] = each
+		else:
+			for button in buttons:
+				button['disabled'] = disabled
+
+	if icon is not None:
+		if isinstance(icon, list):
+			for i, each in enumerate(icon):
+				if each is not None:
+					buttons[i]['icon'] = each
+		else:
+			for button in buttons:
+				button['icon'] = icon
+
+	if iconOnly is not None:
+		if isinstance(iconOnly, list):
+			for i, each in enumerate(iconOnly):
+				if each is not None:
+					buttons[i]['iconOnly'] = each
+		else:
+			for button in buttons:
+				button['iconOnly'] = iconOnly
+
+	if noOutline is not None:
+		if isinstance(noOutline, list):
+			for i, each in enumerate(noOutline):
+				if each is not None:
+					buttons[i]['noOutline'] = each
+		else:
+			for button in buttons:
+				button['noOutline'] = noOutline
+
+	if link is not None:
+		if isinstance(link, list):
+			for i, each in enumerate(link):
+				if each is not None:
+					buttons[i]['link'] = each
+		else:
+			for button in buttons:
+				button['link'] = link
+
+	if copy is not None:
+		if isinstance(copy, list):
+			for i, each in enumerate(copy):
+				if each is not None:
+					buttons[i]['copy'] = each
+		else:
+			for button in buttons:
+				button['copy'] = copy
+
+	kwargs['buttons'] = buttons
+
+	if align is not None:
+		kwargs['align'] = align
+	if inline is not None:
+		kwargs['inlineLayoutWhen'] = 'always' if inline else 'never'
+	if reverse is not None:
+		kwargs['reverse'] = reverse
+	if iconRight is not None:
+		kwargs['iconRight'] = iconRight
+	if size is not None:
+		kwargs['size'] = size
+	if equisized is not None:
+		kwargs['equisized'] = equisized
+
+	return _dsfr_buttons_group_func(**kwargs, key = key, default = [False for _ in buttons])
+
+dsfr_buttons_group = buttons_group
+
 def checkbox(
 	label: str, # Standard
 	value: Optional[bool] = None, # Standard
 	key: Optional[Union[str, int]] = None, # Standard
 	help: Optional[str] = None, # Standard
 	small: Optional[bool] = None,
 	required: Optional[bool] = None,
@@ -415,14 +559,15 @@
 	isInvalid: Optional[bool] = None,
 	isValid: Optional[bool] = None,
 	isTextarea: Optional[bool] = None,
 	isWithWarning: Optional[bool] = None,
 	labelClass: Optional[str] = None,
 	wrapperClass: Optional[str] = None,
 	requiredTip: Optional[str] = None,
+	height: Optional[int] = None,
 	**kwargs,
 ):
 	"""
 	Streamlit DSFR Input component
 	"""
 	kwargs['label'] = label
 
@@ -466,14 +611,16 @@
 		kwargs['isWithWarning'] = isWithWarning
 	if labelClass is not None:
 		kwargs['labelClass'] = labelClass
 	if wrapperClass is not None:
 		kwargs['wrapperClass'] = wrapperClass
 	if requiredTip is not None:
 		kwargs['requiredTip'] = requiredTip
+	if height is not None:
+		kwargs['height'] = height
 
 	return _dsfr_input_func(**kwargs, key = key, default = kwargs['modelValue'])
 
 dsfr_input = input
 
 def text_input(
 	label: str, # Standard
@@ -607,15 +754,15 @@
 	)
 
 dsfr_number_input = number_input
 
 def text_area(
 	label: str, # Standard
 	value: Optional[str] = None, # Standard
-	# height: Optional[int] = None, # Standard
+	height: Optional[int] = None, # Standard
 	# max_chars: Optional[int] = None, # Standard
 	key: Optional[Union[str, int]] = None, # Standard
 	help: Optional[str] = None, # Standard
 	# on_change: Optional[Callable] = None, # Standard
 	# args: Optional[tuple] = None, # Standard
 	# kwargs: Optional[dict] = None, # Standard
 	*,
@@ -642,14 +789,15 @@
 	"""
 	if value is None:
 		value = ''
 
 	return dsfr_input(
 		label = label,
 		value = value,
+		height = height,
 		key = key,
 		help = help,
 		placeholder = placeholder,
 		disabled = disabled,
 		hint = hint,
 		labelVisible = labelVisible,
 		id = id,
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_alert/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_buttons_group/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1pKcPR" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrAlert.tFZy4mCO.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrAlert&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z2lW4xP" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrButtonGroup.MtpDLhtp.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrButtonGroup&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_badge/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_badge/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1eUvIB" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrBadge.gLg-CXXd.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrBadge&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1eUvIB" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrBadge.U7kOfHPN.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrBadge&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_breadcrumb/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_breadcrumb/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1NTbsh" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrBreadcrumb.79FUC984.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrBreadcrumb&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1NTbsh" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrBreadcrumb.24AdnYLs.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrBreadcrumb&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_button/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_input/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,3 +1,4 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="ZI3AMx" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrButton.5AkE1u2l.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrButton&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+.component[data-v-dc4eef68]{margin:4px}.component[data-v-dc4eef68] textarea.fr-input{min-height:var(--dsfr-input-height);resize:none}
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Zeq8RV" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrInput.DWr3u8eg.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrInput&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_checkbox/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_checkbox/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,4 +1,4 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
 .component[data-v-107dca5f] .fr-fieldset__element{margin-bottom:0;padding-left:0;padding-right:0}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="1uszWX" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrCheckbox.TNj2wexB.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrCheckbox&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="1uszWX" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrCheckbox.HBUYPhr5.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrCheckbox&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrAlert.tFZy4mCO.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrAlert.qHAssOJm.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     _ as n,
     u as _,
     f as l,
     S as i
-} from "./StreamlitVue.ZFQEvSxb.js";
+} from "./StreamlitVue.CglRiHNi.js";
 import {
     d as s,
     o as a,
     c as m,
     a as f,
     n as u,
     g as d,
     b as S
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const b = s({
         __name: "DsfrAlert",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBadge.gLg-CXXd.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBadge.U7kOfHPN.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     _ as n,
     u as _,
     h as d,
     S as i
-} from "./StreamlitVue.ZFQEvSxb.js";
+} from "./StreamlitVue.CglRiHNi.js";
 import {
     d as s,
     o as a,
     c as m,
     a as l,
     n as u,
     g as f,
     b as g
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const B = s({
         __name: "DsfrBadge",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBreadcrumb.79FUC984.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBreadcrumb.24AdnYLs.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     _ as n,
     u as _,
     k as m,
     S as u
-} from "./StreamlitVue.ZFQEvSxb.js";
+} from "./StreamlitVue.CglRiHNi.js";
 import {
     d as s,
     o as a,
     c as d,
     a as i,
     n as l,
     g as f,
     b
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const B = s({
         __name: "DsfrBreadcrumb",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButton.5AkE1u2l.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButtonGroup.MtpDLhtp.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,116 +1,103 @@
 import {
-    _ as u,
+    _ as m,
     u as _,
-    a as t,
-    A as f,
-    S as m
-} from "./StreamlitVue.ZFQEvSxb.js";
+    H as b,
+    a as p,
+    S as g
+} from "./StreamlitVue.CglRiHNi.js";
 import {
-    d as p,
-    r as i,
-    e as v,
-    f as b,
+    d as f,
+    r as y,
     o as d,
-    c as B,
-    a as E,
-    m as g,
-    h as k,
-    b as C
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
-const S = p({
-    __name: "DsfrButton",
+    c as k,
+    a as v,
+    m as C,
+    e as B,
+    b as S
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
+const h = f({
+    __name: "DsfrButtonGroup",
     props: {
         args: {},
         width: {},
         disabled: {
             type: Boolean
         },
         theme: {}
     },
     setup(r, {
-        expose: s
+        expose: a
     }) {
-        s(), _();
-        const o = r,
-            e = i(!1),
-            n = i(!1),
-            a = c => {
-                !n.value && e.value && (e.value = !1, t.setComponentValue(e.value))
-            };
-        v(() => {
-            t.events.addEventListener(t.RENDER_EVENT, a)
-        }), b(() => {
-            t.events.removeEventListener(t.RENDER_EVENT, a)
-        });
+        a(), _();
+        const t = r,
+            e = y(Array(t.args.buttons?.length ?? 0).fill(!1));
+        async function i(u) {
+            let o = u.target;
+            for (; o && !o.classList.contains("fr-btn");) o = o.parentElement;
+            if (!o) {
+                console.error("Button not found for click event:", u);
+                return
+            }
+            const c = Array.from(o.parentElement?.parentElement?.children ?? []).indexOf(o.parentElement),
+                s = t.args.buttons?.[c];
+            s && (s.link ? window.open(s.link, "_blank")?.focus() : s.copy && navigator.clipboard.writeText(s.copy).catch(n => {
+                console.error("Failed to copy:", n)
+            })), e.value.some(n => n) && (e.value = Array(t.args.buttons?.length ?? 0).fill(!1), p.setComponentValue([...e.value]), await new Promise(n => setTimeout(n, 50))), e.value[c] = !0, p.setComponentValue([...e.value]), await new Promise(n => setTimeout(n, 50)), e.value[c] = !1, p.setComponentValue([...e.value])
+        }
         const l = {
-            props: o,
+            props: t,
             clicked: e,
-            isFocused: n,
-            onRenderEvent: a,
-            onClick: () => {
-                o.args.link ? window.open(o.args.link, "_blank")?.focus() : o.args.copy && navigator.clipboard.writeText(o.args.copy).catch(c => {
-                    console.error("Failed to copy:", c)
-                }), e.value || (e.value = !0, t.setComponentValue(e.value))
-            },
-            onFocus: () => {
-                n.value = !0
-            },
-            onBlur: () => {
-                n.value = !1
-            },
-            get DsfrButton() {
-                return f
+            onClick: i,
+            get DsfrButtonGroup() {
+                return b
             }
         };
         return Object.defineProperty(l, "__isScriptSetup", {
             enumerable: !1,
             value: !0
         }), l
     }
 });
 
-function y(r, s, o, e, n, a) {
-    return d(), B("div", {
+function w(r, a, t, e, i, l) {
+    return d(), k("div", {
         class: "component",
-        style: k(r.style)
-    }, [E(e.DsfrButton, g(e.props.args, {
-        label: e.props.args.label || "Button",
+        style: B(r.style)
+    }, [v(e.DsfrButtonGroup, C(e.props.args, {
         disabled: e.props.disabled || e.props.args.disabled,
-        onClick: e.onClick,
-        onFocus: e.onFocus,
-        onBlur: e.onBlur
-    }), null, 16, ["label", "disabled"])], 4)
+        onClick: e.onClick
+    }), null, 16, ["disabled"])], 4)
 }
-const D = u(S, [
-        ["render", y]
+const x = m(h, [
+        ["render", w]
     ]),
-    h = p({
-        __name: "DsfrButton",
+    D = f({
+        __name: "DsfrButtonGroup",
         setup(r, {
-            expose: s
+            expose: a
         }) {
-            s();
-            const o = {
-                StreamlitComponent: m,
-                Component: D
+            a();
+            const t = {
+                StreamlitComponent: g,
+                Component: x
             };
-            return Object.defineProperty(o, "__isScriptSetup", {
+            return Object.defineProperty(t, "__isScriptSetup", {
                 enumerable: !1,
                 value: !0
-            }), o
+            }), t
         }
     });
 
-function x(r, s, o, e, n, a) {
-    return d(), C(e.StreamlitComponent, {
+function E(r, a, t, e, i, l) {
+    return d(), S(e.StreamlitComponent, {
         component: e.Component,
         "client:load": ""
     })
 }
-const T = u(h, [
-    ["render", x]
+const V = m(D, [
+    ["render", E]
 ]);
 export {
-    T as
+    V as
     default
 };
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrCheckbox.TNj2wexB.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrCheckbox.HBUYPhr5.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,29 @@
 import {
     _ as p,
     u as i,
     b as m,
     a as _,
     S as u
-} from "./StreamlitVue.ZFQEvSxb.js"; /* empty css                                  */
+} from "./StreamlitVue.CglRiHNi.js"; /* empty css                                  */
 import {
     d,
     r as f,
-    i as b,
+    f as b,
     o as l,
     c as h,
     a as k,
-    j as C,
+    h as C,
     w as x,
     m as g,
-    h as y,
-    k as S,
+    e as y,
+    i as S,
     t as v,
     b as D
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const V = d({
     __name: "DsfrCheckbox",
     props: {
         args: {},
         width: {},
         disabled: {
             type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFileUpload.IdR5fkhs.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFileUpload.Qd737a0v.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     _ as c,
     u as f,
     z as b,
     a as g,
     S as C
-} from "./StreamlitVue.ZFQEvSxb.js";
+} from "./StreamlitVue.CglRiHNi.js";
 import {
     d as i,
     o as _,
     c as h,
     a as v,
     m as S,
     b as U
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const x = i({
         __name: "DsfrFileUpload",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFooter.so92d35v.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFooter.vqQJXfur.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 import {
     _ as n,
     u as i,
     c as l,
     S as m
-} from "./StreamlitVue.ZFQEvSxb.js";
+} from "./StreamlitVue.CglRiHNi.js";
 import {
     d as s,
     o as t,
     c as g,
     a as k,
     b as _
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const L = s({
         __name: "DsfrFooter",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrPicture.BG7gzqcn.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrPicture.vdniiHOI.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     _ as n,
     u as _,
     e as i,
     S as u
-} from "./StreamlitVue.ZFQEvSxb.js"; /* empty css                                 */
+} from "./StreamlitVue.CglRiHNi.js"; /* empty css                                 */
 import {
     d as s,
     o as a,
     c as m,
     a as d,
     n as l,
     g as f,
     b as P
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const S = s({
         __name: "DsfrPicture",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRadioButtonSet.j3YqEKSL.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRadioButtonSet.I8DloxHK.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 import {
     _ as d,
     u as c,
     w as _,
     a as m,
     S as f
-} from "./StreamlitVue.ZFQEvSxb.js"; /* empty css                               */
+} from "./StreamlitVue.CglRiHNi.js"; /* empty css                               */
 import {
     d as l,
     r as S,
     o as u,
     c as g,
     a as b,
-    j as v,
+    h as v,
     w as B,
     m as V,
-    k as x,
+    i as x,
     t as C,
     b as D
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
-const k = l({
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
+const h = l({
         __name: "DsfrRadioButtonSet",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
             },
@@ -70,19 +70,19 @@
         _: 2
     }, [e.props.args.requiredTip ? {
         name: "required-tip",
         fn: B(() => [x(C(e.props.args.requiredTip), 1)]),
         key: "0"
     } : void 0]), 1040, ["options", "modelValue"])])
 }
-const R = d(k, [
+const R = d(h, [
         ["render", y],
         ["__scopeId", "data-v-61d47d67"]
     ]),
-    h = l({
+    k = l({
         __name: "DsfrRadioButtonSet",
         setup(o, {
             expose: r
         }) {
             r();
             const t = {
                 StreamlitComponent: f,
@@ -97,14 +97,14 @@
 
 function O(o, r, t, e, n, s) {
     return u(), D(e.StreamlitComponent, {
         component: e.Component,
         "client:load": ""
     })
 }
-const U = d(h, [
+const j = d(k, [
     ["render", O]
 ]);
 export {
-    U as
+    j as
     default
 };
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRange.WiM63mXm.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRange.uSCKVJAW.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 import {
     _ as c,
     u as v,
     E as b,
     a as S,
     S as V
-} from "./StreamlitVue.ZFQEvSxb.js"; /* empty css                               */
+} from "./StreamlitVue.CglRiHNi.js"; /* empty css                               */
 import {
     d as u,
     r as m,
     o as _,
-    c as x,
-    a as C,
-    j as h,
+    c as h,
+    a as x,
+    h as C,
     w as l,
-    m as k,
-    k as p,
+    m as y,
+    i as p,
     t as i,
-    b as y
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js"; /* empty css                               */
+    b as k
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js"; /* empty css                               */
 const D = u({
         __name: "DsfrRange",
         props: {
             args: {},
             width: {},
             disabled: {
                 type: Boolean
@@ -67,19 +67,19 @@
         }
     }),
     U = {
         class: "component"
     };
 
 function R(s, o, a, e, r, t) {
-    return _(), x("div", U, [C(e.DsfrRange, k(e.props.args, {
+    return _(), h("div", U, [x(e.DsfrRange, y(e.props.args, {
         disabled: e.props.disabled || e.props.args.disabled,
         modelValue: e.value,
         "onUpdate:modelValue": [o[0] || (o[0] = n => e.value = n), e.onUpdateModelValue]
-    }), h({
+    }), C({
         _: 2
     }, [e.props.args.label ? {
         name: "label",
         fn: l(() => [p(i(e.props.args.label), 1)]),
         key: "0"
     } : void 0, e.props.args.hint ? {
         name: "hint",
@@ -91,15 +91,15 @@
         key: "2"
     } : void 0]), 1040, ["disabled", "modelValue"])])
 }
 const B = c(D, [
         ["render", R],
         ["__scopeId", "data-v-81302ce6"]
     ]),
-    j = u({
+    w = u({
         __name: "DsfrRange",
         setup(s, {
             expose: o
         }) {
             o();
             const a = {
                 StreamlitComponent: V,
@@ -108,20 +108,20 @@
             return Object.defineProperty(a, "__isScriptSetup", {
                 enumerable: !1,
                 value: !0
             }), a
         }
     });
 
-function w(s, o, a, e, r, t) {
-    return _(), y(e.StreamlitComponent, {
+function E(s, o, a, e, r, t) {
+    return _(), k(e.StreamlitComponent, {
         component: e.Component,
         "client:load": ""
     })
 }
-const N = c(j, [
-    ["render", w]
+const N = c(w, [
+    ["render", E]
 ]);
 export {
     N as
     default
 };
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.Lusn3uPo.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.Lusn3uPo.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.mI04Wx9M.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.mI04Wx9M.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.VpzzqYz6.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.VpzzqYz6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.alvVdTYc.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.alvVdTYc.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.6lmsSnc8.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.6lmsSnc8.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.7GX88oPX.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.7GX88oPX.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.GJ3thv45.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.GJ3thv45.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.STgl0sbt.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.STgl0sbt.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.A6bVQEda.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.A6bVQEda.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.prCK3SSS.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium.prCK3SSS.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.FqmRU-8D.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.FqmRU-8D.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.T_DBs5K5.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Medium_Italic.T_DBs5K5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.8SHksZge.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.8SHksZge.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.mgqq5yTO.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.mgqq5yTO.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.3R_BbTaN.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.3R_BbTaN.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.UCbE0jax.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.UCbE0jax.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.FN9ubN3N.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.FN9ubN3N.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.gs3wZvgE.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.gs3wZvgE.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.9CKHJdJx.woff` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.9CKHJdJx.woff`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.D5gUInLE.woff2` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.D5gUInLE.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/StreamlitVue.ZFQEvSxb.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/StreamlitVue.CglRiHNi.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,205 +1,205 @@
 /* empty css                               */
 import {
     d as ht,
-    r as It,
-    e as Pn,
-    l as Er,
-    f as io,
+    r as pt,
+    j as wn,
+    k as kr,
+    l as ro,
     p as gl,
     o as m,
-    c as b,
+    c as v,
     q as g,
     t as C,
     s as dt,
     u as k,
     v as _l,
     x as wl,
-    b as Mt,
-    w as Se,
-    y as cn,
-    h as xn,
-    i as Is,
-    z as L,
+    b as xt,
+    w as Fe,
+    y as dn,
+    e as hn,
+    f as Os,
+    z as w,
     A as Sl,
-    B as or,
-    C as Rr,
+    B as lr,
+    C as Ur,
     D as Il,
     E as Bl,
-    F as rt,
-    k as vt,
+    F as st,
+    i as bt,
     T as Ol,
     G as Fl,
     H as Al,
-    I as un,
-    J as Ln,
-    K as ei,
-    m as pe,
-    n as ro,
+    I as He,
+    J as fn,
+    K as ii,
+    m as re,
+    a as br,
+    n as so,
     L as Dl,
     M as Tl,
-    a as Bs,
     N as Nl
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js";
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js";
 
-function Ml(n) {
+function xl(n) {
     return n && n.__esModule && Object.prototype.hasOwnProperty.call(n, "default") ? n.default : n
 }
-var so = {
+var oo = {
         exports: {}
     },
-    W = {};
+    G = {};
 /** @license React v16.13.1
  * react-is.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
 var ft = typeof Symbol == "function" && Symbol.for,
-    Cr = ft ? Symbol.for("react.element") : 60103,
-    kr = ft ? Symbol.for("react.portal") : 60106,
-    zi = ft ? Symbol.for("react.fragment") : 60107,
-    Wi = ft ? Symbol.for("react.strict_mode") : 60108,
-    Yi = ft ? Symbol.for("react.profiler") : 60114,
-    Gi = ft ? Symbol.for("react.provider") : 60109,
-    Hi = ft ? Symbol.for("react.context") : 60110,
-    Ur = ft ? Symbol.for("react.async_mode") : 60111,
-    qi = ft ? Symbol.for("react.concurrent_mode") : 60111,
-    Ji = ft ? Symbol.for("react.forward_ref") : 60112,
-    Ki = ft ? Symbol.for("react.suspense") : 60113,
-    xl = ft ? Symbol.for("react.suspense_list") : 60120,
-    Zi = ft ? Symbol.for("react.memo") : 60115,
-    Xi = ft ? Symbol.for("react.lazy") : 60116,
+    $r = ft ? Symbol.for("react.element") : 60103,
+    Vr = ft ? Symbol.for("react.portal") : 60106,
+    Yi = ft ? Symbol.for("react.fragment") : 60107,
+    Gi = ft ? Symbol.for("react.strict_mode") : 60108,
+    Hi = ft ? Symbol.for("react.profiler") : 60114,
+    qi = ft ? Symbol.for("react.provider") : 60109,
+    Ji = ft ? Symbol.for("react.context") : 60110,
+    Pr = ft ? Symbol.for("react.async_mode") : 60111,
+    Ki = ft ? Symbol.for("react.concurrent_mode") : 60111,
+    Zi = ft ? Symbol.for("react.forward_ref") : 60112,
+    Xi = ft ? Symbol.for("react.suspense") : 60113,
+    Ml = ft ? Symbol.for("react.suspense_list") : 60120,
+    Qi = ft ? Symbol.for("react.memo") : 60115,
+    tr = ft ? Symbol.for("react.lazy") : 60116,
     Ll = ft ? Symbol.for("react.block") : 60121,
     El = ft ? Symbol.for("react.fundamental") : 60117,
     Rl = ft ? Symbol.for("react.responder") : 60118,
     Cl = ft ? Symbol.for("react.scope") : 60119;
 
 function Et(n) {
     if (typeof n == "object" && n !== null) {
         var t = n.$$typeof;
         switch (t) {
-            case Cr:
+            case $r:
                 switch (n = n.type, n) {
-                    case Ur:
-                    case qi:
-                    case zi:
-                    case Yi:
-                    case Wi:
+                    case Pr:
                     case Ki:
+                    case Yi:
+                    case Hi:
+                    case Gi:
+                    case Xi:
                         return n;
                     default:
                         switch (n = n && n.$$typeof, n) {
-                            case Hi:
                             case Ji:
-                            case Xi:
                             case Zi:
-                            case Gi:
+                            case tr:
+                            case Qi:
+                            case qi:
                                 return n;
                             default:
                                 return t
                         }
                 }
-            case kr:
+            case Vr:
                 return t
         }
     }
 }
 
-function oo(n) {
-    return Et(n) === qi
+function ao(n) {
+    return Et(n) === Ki
 }
-W.AsyncMode = Ur;
-W.ConcurrentMode = qi;
-W.ContextConsumer = Hi;
-W.ContextProvider = Gi;
-W.Element = Cr;
-W.ForwardRef = Ji;
-W.Fragment = zi;
-W.Lazy = Xi;
-W.Memo = Zi;
-W.Portal = kr;
-W.Profiler = Yi;
-W.StrictMode = Wi;
-W.Suspense = Ki;
-W.isAsyncMode = function(n) {
-    return oo(n) || Et(n) === Ur
+G.AsyncMode = Pr;
+G.ConcurrentMode = Ki;
+G.ContextConsumer = Ji;
+G.ContextProvider = qi;
+G.Element = $r;
+G.ForwardRef = Zi;
+G.Fragment = Yi;
+G.Lazy = tr;
+G.Memo = Qi;
+G.Portal = Vr;
+G.Profiler = Hi;
+G.StrictMode = Gi;
+G.Suspense = Xi;
+G.isAsyncMode = function(n) {
+    return ao(n) || Et(n) === Pr
 };
-W.isConcurrentMode = oo;
-W.isContextConsumer = function(n) {
-    return Et(n) === Hi
+G.isConcurrentMode = ao;
+G.isContextConsumer = function(n) {
+    return Et(n) === Ji
 };
-W.isContextProvider = function(n) {
-    return Et(n) === Gi
+G.isContextProvider = function(n) {
+    return Et(n) === qi
 };
-W.isElement = function(n) {
-    return typeof n == "object" && n !== null && n.$$typeof === Cr
+G.isElement = function(n) {
+    return typeof n == "object" && n !== null && n.$$typeof === $r
 };
-W.isForwardRef = function(n) {
-    return Et(n) === Ji
+G.isForwardRef = function(n) {
+    return Et(n) === Zi
 };
-W.isFragment = function(n) {
-    return Et(n) === zi
+G.isFragment = function(n) {
+    return Et(n) === Yi
 };
-W.isLazy = function(n) {
-    return Et(n) === Xi
+G.isLazy = function(n) {
+    return Et(n) === tr
 };
-W.isMemo = function(n) {
-    return Et(n) === Zi
+G.isMemo = function(n) {
+    return Et(n) === Qi
 };
-W.isPortal = function(n) {
-    return Et(n) === kr
+G.isPortal = function(n) {
+    return Et(n) === Vr
 };
-W.isProfiler = function(n) {
-    return Et(n) === Yi
+G.isProfiler = function(n) {
+    return Et(n) === Hi
 };
-W.isStrictMode = function(n) {
-    return Et(n) === Wi
+G.isStrictMode = function(n) {
+    return Et(n) === Gi
 };
-W.isSuspense = function(n) {
-    return Et(n) === Ki
+G.isSuspense = function(n) {
+    return Et(n) === Xi
 };
-W.isValidElementType = function(n) {
-    return typeof n == "string" || typeof n == "function" || n === zi || n === qi || n === Yi || n === Wi || n === Ki || n === xl || typeof n == "object" && n !== null && (n.$$typeof === Xi || n.$$typeof === Zi || n.$$typeof === Gi || n.$$typeof === Hi || n.$$typeof === Ji || n.$$typeof === El || n.$$typeof === Rl || n.$$typeof === Cl || n.$$typeof === Ll)
+G.isValidElementType = function(n) {
+    return typeof n == "string" || typeof n == "function" || n === Yi || n === Ki || n === Hi || n === Gi || n === Xi || n === Ml || typeof n == "object" && n !== null && (n.$$typeof === tr || n.$$typeof === Qi || n.$$typeof === qi || n.$$typeof === Ji || n.$$typeof === Zi || n.$$typeof === El || n.$$typeof === Rl || n.$$typeof === Cl || n.$$typeof === Ll)
 };
-W.typeOf = Et;
-so.exports = W;
-var kl = so.exports,
-    ao = kl,
+G.typeOf = Et;
+oo.exports = G;
+var kl = oo.exports,
+    lo = kl,
     Ul = {
         $$typeof: !0,
         render: !0,
         defaultProps: !0,
         displayName: !0,
         propTypes: !0
     },
-    Vl = {
+    $l = {
         $$typeof: !0,
         compare: !0,
         defaultProps: !0,
         displayName: !0,
         propTypes: !0,
         type: !0
     },
-    lo = {};
-lo[ao.ForwardRef] = Ul;
-lo[ao.Memo] = Vl;
-var co = {
+    co = {};
+co[lo.ForwardRef] = Ul;
+co[lo.Memo] = $l;
+var uo = {
         exports: {}
     },
-    Y = {};
+    H = {};
 /*
 object-assign
 (c) Sindre Sorhus
 @license MIT
 */
-var Os = Object.getOwnPropertySymbols,
-    $l = Object.prototype.hasOwnProperty,
+var Fs = Object.getOwnPropertySymbols,
+    Vl = Object.prototype.hasOwnProperty,
     Pl = Object.prototype.propertyIsEnumerable;
 
 function jl(n) {
     if (n == null) throw new TypeError("Object.assign cannot be called with null or undefined");
     return Object(n)
 }
 
@@ -220,162 +220,162 @@
     } catch {
         return !1
     }
 }
 var Wl = zl() ? Object.assign : function(n, t) {
     for (var e, i = jl(n), r, s = 1; s < arguments.length; s++) {
         e = Object(arguments[s]);
-        for (var o in e) $l.call(e, o) && (i[o] = e[o]);
-        if (Os) {
-            r = Os(e);
+        for (var o in e) Vl.call(e, o) && (i[o] = e[o]);
+        if (Fs) {
+            r = Fs(e);
             for (var a = 0; a < r.length; a++) Pl.call(e, r[a]) && (i[r[a]] = e[r[a]])
         }
     }
     return i
 };
 /** @license React v16.14.0
  * react.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
-var Vr = Wl,
-    jt = typeof Symbol == "function" && Symbol.for,
-    jn = jt ? Symbol.for("react.element") : 60103,
-    Yl = jt ? Symbol.for("react.portal") : 60106,
-    Gl = jt ? Symbol.for("react.fragment") : 60107,
-    Hl = jt ? Symbol.for("react.strict_mode") : 60108,
-    ql = jt ? Symbol.for("react.profiler") : 60114,
-    Jl = jt ? Symbol.for("react.provider") : 60109,
-    Kl = jt ? Symbol.for("react.context") : 60110,
-    Zl = jt ? Symbol.for("react.forward_ref") : 60112,
-    Xl = jt ? Symbol.for("react.suspense") : 60113,
-    Ql = jt ? Symbol.for("react.memo") : 60115,
-    tc = jt ? Symbol.for("react.lazy") : 60116,
-    Fs = typeof Symbol == "function" && Symbol.iterator;
+var jr = Wl,
+    zt = typeof Symbol == "function" && Symbol.for,
+    jn = zt ? Symbol.for("react.element") : 60103,
+    Yl = zt ? Symbol.for("react.portal") : 60106,
+    Gl = zt ? Symbol.for("react.fragment") : 60107,
+    Hl = zt ? Symbol.for("react.strict_mode") : 60108,
+    ql = zt ? Symbol.for("react.profiler") : 60114,
+    Jl = zt ? Symbol.for("react.provider") : 60109,
+    Kl = zt ? Symbol.for("react.context") : 60110,
+    Zl = zt ? Symbol.for("react.forward_ref") : 60112,
+    Xl = zt ? Symbol.for("react.suspense") : 60113,
+    Ql = zt ? Symbol.for("react.memo") : 60115,
+    tc = zt ? Symbol.for("react.lazy") : 60116,
+    As = typeof Symbol == "function" && Symbol.iterator;
 
 function zn(n) {
     for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + n, e = 1; e < arguments.length; e++) t += "&args[]=" + encodeURIComponent(arguments[e]);
     return "Minified React error #" + n + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
 }
-var uo = {
+var ho = {
         isMounted: function() {
             return !1
         },
         enqueueForceUpdate: function() {},
         enqueueReplaceState: function() {},
         enqueueSetState: function() {}
     },
-    ho = {};
+    fo = {};
 
-function bn(n, t, e) {
-    this.props = n, this.context = t, this.refs = ho, this.updater = e || uo
+function Sn(n, t, e) {
+    this.props = n, this.context = t, this.refs = fo, this.updater = e || ho
 }
-bn.prototype.isReactComponent = {};
-bn.prototype.setState = function(n, t) {
+Sn.prototype.isReactComponent = {};
+Sn.prototype.setState = function(n, t) {
     if (typeof n != "object" && typeof n != "function" && n != null) throw Error(zn(85));
     this.updater.enqueueSetState(this, n, t, "setState")
 };
-bn.prototype.forceUpdate = function(n) {
+Sn.prototype.forceUpdate = function(n) {
     this.updater.enqueueForceUpdate(this, n, "forceUpdate")
 };
 
-function fo() {}
-fo.prototype = bn.prototype;
+function po() {}
+po.prototype = Sn.prototype;
 
-function $r(n, t, e) {
-    this.props = n, this.context = t, this.refs = ho, this.updater = e || uo
+function zr(n, t, e) {
+    this.props = n, this.context = t, this.refs = fo, this.updater = e || ho
 }
-var Pr = $r.prototype = new fo;
-Pr.constructor = $r;
-Vr(Pr, bn.prototype);
-Pr.isPureReactComponent = !0;
-var jr = {
+var Wr = zr.prototype = new po;
+Wr.constructor = zr;
+jr(Wr, Sn.prototype);
+Wr.isPureReactComponent = !0;
+var Yr = {
         current: null
     },
-    po = Object.prototype.hasOwnProperty,
-    yo = {
+    yo = Object.prototype.hasOwnProperty,
+    mo = {
         key: !0,
         ref: !0,
         __self: !0,
         __source: !0
     };
 
-function mo(n, t, e) {
+function vo(n, t, e) {
     var i, r = {},
         s = null,
         o = null;
     if (t != null)
-        for (i in t.ref !== void 0 && (o = t.ref), t.key !== void 0 && (s = "" + t.key), t) po.call(t, i) && !yo.hasOwnProperty(i) && (r[i] = t[i]);
+        for (i in t.ref !== void 0 && (o = t.ref), t.key !== void 0 && (s = "" + t.key), t) yo.call(t, i) && !mo.hasOwnProperty(i) && (r[i] = t[i]);
     var a = arguments.length - 2;
     if (a === 1) r.children = e;
     else if (1 < a) {
         for (var l = Array(a), c = 0; c < a; c++) l[c] = arguments[c + 2];
         r.children = l
     }
     if (n && n.defaultProps)
         for (i in a = n.defaultProps, a) r[i] === void 0 && (r[i] = a[i]);
     return {
         $$typeof: jn,
         type: n,
         key: s,
         ref: o,
         props: r,
-        _owner: jr.current
+        _owner: Yr.current
     }
 }
 
 function ec(n, t) {
     return {
         $$typeof: jn,
         type: n.type,
         key: t,
         ref: n.ref,
         props: n.props,
         _owner: n._owner
     }
 }
 
-function zr(n) {
+function Gr(n) {
     return typeof n == "object" && n !== null && n.$$typeof === jn
 }
 
 function nc(n) {
     var t = {
         "=": "=0",
         ":": "=2"
     };
     return "$" + ("" + n).replace(/[=:]/g, function(e) {
         return t[e]
     })
 }
-var vo = /\/+/g,
-    ci = [];
+var bo = /\/+/g,
+    di = [];
 
-function bo(n, t, e, i) {
-    if (ci.length) {
-        var r = ci.pop();
+function go(n, t, e, i) {
+    if (di.length) {
+        var r = di.pop();
         return r.result = n, r.keyPrefix = t, r.func = e, r.context = i, r.count = 0, r
     }
     return {
         result: n,
         keyPrefix: t,
         func: e,
         context: i,
         count: 0
     }
 }
 
-function go(n) {
-    n.result = null, n.keyPrefix = null, n.func = null, n.context = null, n.count = 0, 10 > ci.length && ci.push(n)
+function _o(n) {
+    n.result = null, n.keyPrefix = null, n.func = null, n.context = null, n.count = 0, 10 > di.length && di.push(n)
 }
 
-function mr(n, t, e, i) {
+function gr(n, t, e, i) {
     var r = typeof n;
     (r === "undefined" || r === "boolean") && (n = null);
     var s = !1;
     if (n === null) s = !0;
     else switch (r) {
         case "string":
         case "number":
@@ -384,112 +384,112 @@
         case "object":
             switch (n.$$typeof) {
                 case jn:
                 case Yl:
                     s = !0
             }
     }
-    if (s) return e(i, n, t === "" ? "." + ar(n, 0) : t), 1;
+    if (s) return e(i, n, t === "" ? "." + cr(n, 0) : t), 1;
     if (s = 0, t = t === "" ? "." : t + ":", Array.isArray(n))
         for (var o = 0; o < n.length; o++) {
             r = n[o];
-            var a = t + ar(r, o);
-            s += mr(r, a, e, i)
-        } else if (n === null || typeof n != "object" ? a = null : (a = Fs && n[Fs] || n["@@iterator"], a = typeof a == "function" ? a : null), typeof a == "function")
-            for (n = a.call(n), o = 0; !(r = n.next()).done;) r = r.value, a = t + ar(r, o++), s += mr(r, a, e, i);
+            var a = t + cr(r, o);
+            s += gr(r, a, e, i)
+        } else if (n === null || typeof n != "object" ? a = null : (a = As && n[As] || n["@@iterator"], a = typeof a == "function" ? a : null), typeof a == "function")
+            for (n = a.call(n), o = 0; !(r = n.next()).done;) r = r.value, a = t + cr(r, o++), s += gr(r, a, e, i);
         else if (r === "object") throw e = "" + n, Error(zn(31, e === "[object Object]" ? "object with keys {" + Object.keys(n).join(", ") + "}" : e, ""));
     return s
 }
 
-function vr(n, t, e) {
-    return n == null ? 0 : mr(n, "", t, e)
+function _r(n, t, e) {
+    return n == null ? 0 : gr(n, "", t, e)
 }
 
-function ar(n, t) {
+function cr(n, t) {
     return typeof n == "object" && n !== null && n.key != null ? nc(n.key) : t.toString(36)
 }
 
 function ic(n, t) {
     n.func.call(n.context, t, n.count++)
 }
 
 function rc(n, t, e) {
     var i = n.result,
         r = n.keyPrefix;
-    n = n.func.call(n.context, t, n.count++), Array.isArray(n) ? br(n, i, e, function(s) {
+    n = n.func.call(n.context, t, n.count++), Array.isArray(n) ? wr(n, i, e, function(s) {
         return s
-    }) : n != null && (zr(n) && (n = ec(n, r + (!n.key || t && t.key === n.key ? "" : ("" + n.key).replace(vo, "$&/") + "/") + e)), i.push(n))
+    }) : n != null && (Gr(n) && (n = ec(n, r + (!n.key || t && t.key === n.key ? "" : ("" + n.key).replace(bo, "$&/") + "/") + e)), i.push(n))
 }
 
-function br(n, t, e, i, r) {
+function wr(n, t, e, i, r) {
     var s = "";
-    e != null && (s = ("" + e).replace(vo, "$&/") + "/"), t = bo(t, s, i, r), vr(n, rc, t), go(t)
+    e != null && (s = ("" + e).replace(bo, "$&/") + "/"), t = go(t, s, i, r), _r(n, rc, t), _o(t)
 }
-var _o = {
+var wo = {
     current: null
 };
 
-function me() {
-    var n = _o.current;
+function ge() {
+    var n = wo.current;
     if (n === null) throw Error(zn(321));
     return n
 }
 var sc = {
-    ReactCurrentDispatcher: _o,
+    ReactCurrentDispatcher: wo,
     ReactCurrentBatchConfig: {
         suspense: null
     },
-    ReactCurrentOwner: jr,
+    ReactCurrentOwner: Yr,
     IsSomeRendererActing: {
         current: !1
     },
-    assign: Vr
+    assign: jr
 };
-Y.Children = {
+H.Children = {
     map: function(n, t, e) {
         if (n == null) return n;
         var i = [];
-        return br(n, i, null, t, e), i
+        return wr(n, i, null, t, e), i
     },
     forEach: function(n, t, e) {
         if (n == null) return n;
-        t = bo(null, null, t, e), vr(n, ic, t), go(t)
+        t = go(null, null, t, e), _r(n, ic, t), _o(t)
     },
     count: function(n) {
-        return vr(n, function() {
+        return _r(n, function() {
             return null
         }, null)
     },
     toArray: function(n) {
         var t = [];
-        return br(n, t, null, function(e) {
+        return wr(n, t, null, function(e) {
             return e
         }), t
     },
     only: function(n) {
-        if (!zr(n)) throw Error(zn(143));
+        if (!Gr(n)) throw Error(zn(143));
         return n
     }
 };
-Y.Component = bn;
-Y.Fragment = Gl;
-Y.Profiler = ql;
-Y.PureComponent = $r;
-Y.StrictMode = Hl;
-Y.Suspense = Xl;
-Y.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = sc;
-Y.cloneElement = function(n, t, e) {
+H.Component = Sn;
+H.Fragment = Gl;
+H.Profiler = ql;
+H.PureComponent = zr;
+H.StrictMode = Hl;
+H.Suspense = Xl;
+H.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = sc;
+H.cloneElement = function(n, t, e) {
     if (n == null) throw Error(zn(267, n));
-    var i = Vr({}, n.props),
+    var i = jr({}, n.props),
         r = n.key,
         s = n.ref,
         o = n._owner;
     if (t != null) {
-        if (t.ref !== void 0 && (s = t.ref, o = jr.current), t.key !== void 0 && (r = "" + t.key), n.type && n.type.defaultProps) var a = n.type.defaultProps;
-        for (l in t) po.call(t, l) && !yo.hasOwnProperty(l) && (i[l] = t[l] === void 0 && a !== void 0 ? a[l] : t[l])
+        if (t.ref !== void 0 && (s = t.ref, o = Yr.current), t.key !== void 0 && (r = "" + t.key), n.type && n.type.defaultProps) var a = n.type.defaultProps;
+        for (l in t) yo.call(t, l) && !mo.hasOwnProperty(l) && (i[l] = t[l] === void 0 && a !== void 0 ? a[l] : t[l])
     }
     var l = arguments.length - 2;
     if (l === 1) i.children = e;
     else if (1 < l) {
         a = Array(l);
         for (var c = 0; c < l; c++) a[c] = arguments[c + 2];
         i.children = a
@@ -499,94 +499,94 @@
         type: n.type,
         key: r,
         ref: s,
         props: i,
         _owner: o
     }
 };
-Y.createContext = function(n, t) {
+H.createContext = function(n, t) {
     return t === void 0 && (t = null), n = {
         $$typeof: Kl,
         _calculateChangedBits: t,
         _currentValue: n,
         _currentValue2: n,
         _threadCount: 0,
         Provider: null,
         Consumer: null
     }, n.Provider = {
         $$typeof: Jl,
         _context: n
     }, n.Consumer = n
 };
-Y.createElement = mo;
-Y.createFactory = function(n) {
-    var t = mo.bind(null, n);
+H.createElement = vo;
+H.createFactory = function(n) {
+    var t = vo.bind(null, n);
     return t.type = n, t
 };
-Y.createRef = function() {
+H.createRef = function() {
     return {
         current: null
     }
 };
-Y.forwardRef = function(n) {
+H.forwardRef = function(n) {
     return {
         $$typeof: Zl,
         render: n
     }
 };
-Y.isValidElement = zr;
-Y.lazy = function(n) {
+H.isValidElement = Gr;
+H.lazy = function(n) {
     return {
         $$typeof: tc,
         _ctor: n,
         _status: -1,
         _result: null
     }
 };
-Y.memo = function(n, t) {
+H.memo = function(n, t) {
     return {
         $$typeof: Ql,
         type: n,
         compare: t === void 0 ? null : t
     }
 };
-Y.useCallback = function(n, t) {
-    return me().useCallback(n, t)
+H.useCallback = function(n, t) {
+    return ge().useCallback(n, t)
 };
-Y.useContext = function(n, t) {
-    return me().useContext(n, t)
+H.useContext = function(n, t) {
+    return ge().useContext(n, t)
 };
-Y.useDebugValue = function() {};
-Y.useEffect = function(n, t) {
-    return me().useEffect(n, t)
+H.useDebugValue = function() {};
+H.useEffect = function(n, t) {
+    return ge().useEffect(n, t)
 };
-Y.useImperativeHandle = function(n, t, e) {
-    return me().useImperativeHandle(n, t, e)
+H.useImperativeHandle = function(n, t, e) {
+    return ge().useImperativeHandle(n, t, e)
 };
-Y.useLayoutEffect = function(n, t) {
-    return me().useLayoutEffect(n, t)
+H.useLayoutEffect = function(n, t) {
+    return ge().useLayoutEffect(n, t)
 };
-Y.useMemo = function(n, t) {
-    return me().useMemo(n, t)
+H.useMemo = function(n, t) {
+    return ge().useMemo(n, t)
 };
-Y.useReducer = function(n, t, e) {
-    return me().useReducer(n, t, e)
+H.useReducer = function(n, t, e) {
+    return ge().useReducer(n, t, e)
 };
-Y.useRef = function(n) {
-    return me().useRef(n)
+H.useRef = function(n) {
+    return ge().useRef(n)
 };
-Y.useState = function(n) {
-    return me().useState(n)
+H.useState = function(n) {
+    return ge().useState(n)
 };
-Y.version = "16.14.0";
-co.exports = Y;
-var oc = co.exports;
-const ac = Ml(oc);
+H.version = "16.14.0";
+uo.exports = H;
+var oc = uo.exports;
+const ac = xl(oc);
 
-function w(n, t, e, i) {
+function S(n, t, e, i) {
     function r(s) {
         return s instanceof e ? s : new e(function(o) {
             o(s)
         })
     }
     return new(e || (e = Promise))(function(s, o) {
         function a(d) {
@@ -608,15 +608,15 @@
         function c(d) {
             d.done ? s(d.value) : r(d.value).then(a, l)
         }
         c((i = i.apply(n, t || [])).next())
     })
 }
 
-function As(n) {
+function Ds(n) {
     var t = typeof Symbol == "function" && Symbol.iterator,
         e = t && n[t],
         i = 0;
     if (e) return e.call(n);
     if (n && typeof n.length == "number") return {
         next: function() {
             return n && i >= n.length && (n = void 0), {
@@ -628,35 +628,35 @@
     throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
 }
 
 function M(n) {
     return this instanceof M ? (this.v = n, this) : new M(n)
 }
 
-function te(n, t, e) {
+function ne(n, t, e) {
     if (!Symbol.asyncIterator) throw new TypeError("Symbol.asyncIterator is not defined.");
     var i = e.apply(n, t || []),
         r, s = [];
     return r = {}, o("next"), o("throw"), o("return"), r[Symbol.asyncIterator] = function() {
         return this
     }, r;
 
     function o(y) {
         i[y] && (r[y] = function(_) {
-            return new Promise(function(G, et) {
-                s.push([y, _, G, et]) > 1 || a(y, _)
+            return new Promise(function(V, P) {
+                s.push([y, _, V, P]) > 1 || a(y, _)
             })
         })
     }
 
     function a(y, _) {
         try {
             l(i[y](_))
-        } catch (G) {
-            h(s[0][3], G)
+        } catch (V) {
+            h(s[0][3], V)
         }
     }
 
     function l(y) {
         y.value instanceof M ? Promise.resolve(y.value.v).then(c, d) : h(s[0][2], y)
     }
 
@@ -669,15 +669,15 @@
     }
 
     function h(y, _) {
         y(_), s.shift(), s.length && a(s[0][0], s[0][1])
     }
 }
 
-function ni(n) {
+function ri(n) {
     var t, e;
     return t = {}, i("next"), i("throw", function(r) {
         throw r
     }), i("return"), t[Symbol.iterator] = function() {
         return this
     }, t;
 
@@ -687,19 +687,19 @@
                 value: M(n[r](o)),
                 done: !1
             } : s ? s(o) : o
         } : s
     }
 }
 
-function je(n) {
+function Ye(n) {
     if (!Symbol.asyncIterator) throw new TypeError("Symbol.asyncIterator is not defined.");
     var t = n[Symbol.asyncIterator],
         e;
-    return t ? t.call(n) : (n = typeof As == "function" ? As(n) : n[Symbol.iterator](), e = {}, i("next"), i("throw"), i("return"), e[Symbol.asyncIterator] = function() {
+    return t ? t.call(n) : (n = typeof Ds == "function" ? Ds(n) : n[Symbol.iterator](), e = {}, i("next"), i("throw"), i("return"), e[Symbol.asyncIterator] = function() {
         return this
     }, e);
 
     function i(s) {
         e[s] = n[s] && function(o) {
             return new Promise(function(a, l) {
                 o = n[s](o), r(a, l, o.done, o.value)
@@ -713,32 +713,32 @@
                 value: c,
                 done: a
             })
         }, o)
     }
 }
 const lc = new TextDecoder("utf-8"),
-    gr = n => lc.decode(n),
+    Sr = n => lc.decode(n),
     cc = new TextEncoder,
-    Wr = n => cc.encode(n),
-    [vp, uc] = (() => {
+    Hr = n => cc.encode(n),
+    [bp, uc] = (() => {
         const n = () => {
             throw new Error("BigInt is not available in this environment")
         };
 
         function t() {
             throw n()
         }
         return t.asIntN = () => {
             throw n()
         }, t.asUintN = () => {
             throw n()
         }, typeof BigInt < "u" ? [BigInt, !0] : [t, !1]
     })(),
-    [Wn, bp] = (() => {
+    [Wn, gp] = (() => {
         const n = () => {
             throw new Error("BigInt64Array is not available in this environment")
         };
         class t {
             static get BYTES_PER_ELEMENT() {
                 return 8
             }
@@ -750,15 +750,15 @@
             }
             constructor() {
                 throw n()
             }
         }
         return typeof BigInt64Array < "u" ? [BigInt64Array, !0] : [t, !1]
     })(),
-    [Yn, gp] = (() => {
+    [Yn, _p] = (() => {
         const n = () => {
             throw new Error("BigUint64Array is not available in this environment")
         };
         class t {
             static get BYTES_PER_ELEMENT() {
                 return 8
             }
@@ -771,31 +771,31 @@
             constructor() {
                 throw n()
             }
         }
         return typeof BigUint64Array < "u" ? [BigUint64Array, !0] : [t, !1]
     })(),
     dc = n => typeof n == "number",
-    wo = n => typeof n == "boolean",
+    So = n => typeof n == "boolean",
     ct = n => typeof n == "function",
     Ot = n => n != null && Object(n) === n,
-    Ie = n => Ot(n) && ct(n.then),
+    Ae = n => Ot(n) && ct(n.then),
     Gn = n => Ot(n) && ct(n[Symbol.iterator]),
-    gn = n => Ot(n) && ct(n[Symbol.asyncIterator]),
-    _r = n => Ot(n) && Ot(n.schema),
-    So = n => Ot(n) && "done" in n && "value" in n,
-    Io = n => Ot(n) && ct(n.stat) && dc(n.fd),
-    Bo = n => Ot(n) && Yr(n.body),
-    Qi = n => "_getDOMStream" in n && "_getNodeStream" in n,
-    hc = n => Ot(n) && ct(n.abort) && ct(n.getWriter) && !Qi(n),
-    Yr = n => Ot(n) && ct(n.cancel) && ct(n.getReader) && !Qi(n),
-    fc = n => Ot(n) && ct(n.end) && ct(n.write) && wo(n.writable) && !Qi(n),
-    Oo = n => Ot(n) && ct(n.read) && ct(n.pipe) && wo(n.readable) && !Qi(n),
+    In = n => Ot(n) && ct(n[Symbol.asyncIterator]),
+    Ir = n => Ot(n) && Ot(n.schema),
+    Io = n => Ot(n) && "done" in n && "value" in n,
+    Bo = n => Ot(n) && ct(n.stat) && dc(n.fd),
+    Oo = n => Ot(n) && qr(n.body),
+    er = n => "_getDOMStream" in n && "_getNodeStream" in n,
+    hc = n => Ot(n) && ct(n.abort) && ct(n.getWriter) && !er(n),
+    qr = n => Ot(n) && ct(n.cancel) && ct(n.getReader) && !er(n),
+    fc = n => Ot(n) && ct(n.end) && ct(n.write) && So(n.writable) && !er(n),
+    Fo = n => Ot(n) && ct(n.read) && ct(n.pipe) && So(n.readable) && !er(n),
     pc = n => Ot(n) && ct(n.clear) && ct(n.bytes) && ct(n.position) && ct(n.setPosition) && ct(n.capacity) && ct(n.getBufferIdentifier) && ct(n.createLong),
-    Gr = typeof SharedArrayBuffer < "u" ? SharedArrayBuffer : ArrayBuffer;
+    Jr = typeof SharedArrayBuffer < "u" ? SharedArrayBuffer : ArrayBuffer;
 
 function yc(n) {
     const t = n[0] ? [n[0]] : [];
     let e, i, r, s;
     for (let o, a, l = 0, c = 0, d = n.length; ++l < d;) {
         if (o = t[c], a = n[l], !o || !a || o.buffer !== a.buffer || a.byteOffset < o.byteOffset) {
             a && (t[++c] = a);
@@ -812,85 +812,85 @@
             continue
         }
         t[c] = new Uint8Array(o.buffer, e, i - e + s)
     }
     return t
 }
 
-function Ds(n, t, e = 0, i = t.byteLength) {
+function Ts(n, t, e = 0, i = t.byteLength) {
     const r = n.byteLength,
         s = new Uint8Array(n.buffer, n.byteOffset, r),
         o = new Uint8Array(t.buffer, t.byteOffset, Math.min(i, r));
     return s.set(o, e), n
 }
 
-function ne(n, t) {
+function se(n, t) {
     const e = yc(n),
         i = e.reduce((d, h) => d + h.byteLength, 0);
     let r, s, o, a = 0,
         l = -1;
     const c = Math.min(t || Number.POSITIVE_INFINITY, i);
     for (const d = e.length; ++l < d;) {
         if (r = e[l], s = r.subarray(0, Math.min(r.length, c - a)), c <= a + s.length) {
-            s.length < r.length ? e[l] = r.subarray(s.length) : s.length === r.length && l++, o ? Ds(o, s, a) : o = s;
+            s.length < r.length ? e[l] = r.subarray(s.length) : s.length === r.length && l++, o ? Ts(o, s, a) : o = s;
             break
         }
-        Ds(o || (o = new Uint8Array(c)), s, a), a += s.length
+        Ts(o || (o = new Uint8Array(c)), s, a), a += s.length
     }
     return [o || new Uint8Array(0), e.slice(l), i - (o ? o.byteLength : 0)]
 }
 
-function q(n, t) {
-    let e = So(t) ? t.value : t;
-    return e instanceof n ? n === Uint8Array ? new n(e.buffer, e.byteOffset, e.byteLength) : e : e ? (typeof e == "string" && (e = Wr(e)), e instanceof ArrayBuffer ? new n(e) : e instanceof Gr ? new n(e) : pc(e) ? q(n, e.bytes()) : ArrayBuffer.isView(e) ? e.byteLength <= 0 ? new n(0) : new n(e.buffer, e.byteOffset, e.byteLength / n.BYTES_PER_ELEMENT) : n.from(e)) : new n(0)
-}
-const Bn = n => q(Int32Array, n),
-    U = n => q(Uint8Array, n),
-    wr = n => (n.next(), n);
+function K(n, t) {
+    let e = Io(t) ? t.value : t;
+    return e instanceof n ? n === Uint8Array ? new n(e.buffer, e.byteOffset, e.byteLength) : e : e ? (typeof e == "string" && (e = Hr(e)), e instanceof ArrayBuffer ? new n(e) : e instanceof Jr ? new n(e) : pc(e) ? K(n, e.bytes()) : ArrayBuffer.isView(e) ? e.byteLength <= 0 ? new n(0) : new n(e.buffer, e.byteOffset, e.byteLength / n.BYTES_PER_ELEMENT) : n.from(e)) : new n(0)
+}
+const An = n => K(Int32Array, n),
+    U = n => K(Uint8Array, n),
+    Br = n => (n.next(), n);
 
 function* mc(n, t) {
     const e = function*(r) {
             yield r
         },
-        i = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof Gr ? e(t) : Gn(t) ? t : e(t);
-    return yield* wr(function*(r) {
+        i = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof Jr ? e(t) : Gn(t) ? t : e(t);
+    return yield* Br(function*(r) {
         let s = null;
-        do s = r.next(yield q(n, s)); while (!s.done)
+        do s = r.next(yield K(n, s)); while (!s.done)
     }(i[Symbol.iterator]())), new n
 }
 const vc = n => mc(Uint8Array, n);
 
-function Fo(n, t) {
-    return te(this, arguments, function*() {
-        if (Ie(t)) return yield M(yield M(yield* ni(je(Fo(n, yield M(t))))));
+function Ao(n, t) {
+    return ne(this, arguments, function*() {
+        if (Ae(t)) return yield M(yield M(yield* ri(Ye(Ao(n, yield M(t))))));
         const i = function(o) {
-                return te(this, arguments, function*() {
+                return ne(this, arguments, function*() {
                     yield yield M(yield M(o))
                 })
             },
             r = function(o) {
-                return te(this, arguments, function*() {
-                    yield M(yield* ni(je(wr(function*(a) {
+                return ne(this, arguments, function*() {
+                    yield M(yield* ri(Ye(Br(function*(a) {
                         let l = null;
                         do l = a.next(yield l?.value); while (!l.done)
                     }(o[Symbol.iterator]())))))
                 })
             },
-            s = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof Gr ? i(t) : Gn(t) ? r(t) : gn(t) ? t : i(t);
-        return yield M(yield* ni(je(wr(function(o) {
-            return te(this, arguments, function*() {
+            s = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof Jr ? i(t) : Gn(t) ? r(t) : In(t) ? t : i(t);
+        return yield M(yield* ri(Ye(Br(function(o) {
+            return ne(this, arguments, function*() {
                 let a = null;
-                do a = yield M(o.next(yield yield M(q(n, a)))); while (!a.done)
+                do a = yield M(o.next(yield yield M(K(n, a)))); while (!a.done)
             })
         }(s[Symbol.asyncIterator]()))))), yield M(new n)
     })
 }
-const bc = n => Fo(Uint8Array, n);
+const bc = n => Ao(Uint8Array, n);
 
-function Hr(n, t, e) {
+function Kr(n, t, e) {
     if (n !== 0) {
         e = e.slice(0, t + 1);
         for (let i = -1; ++i <= t;) e[i] += n
     }
     return e
 }
 
@@ -899,43 +899,43 @@
     const i = n.length;
     if (i !== t.length) return !1;
     if (i > 0)
         do
             if (n[e] !== t[e]) return !1; while (++e < i);
     return !0
 }
-const Ct = {
+const kt = {
         fromIterable(n) {
-            return Zn(_c(n))
+            return Qn(_c(n))
         },
         fromAsyncIterable(n) {
-            return Zn(wc(n))
+            return Qn(wc(n))
         },
         fromDOMStream(n) {
-            return Zn(Sc(n))
+            return Qn(Sc(n))
         },
         fromNodeStream(n) {
-            return Zn(Bc(n))
+            return Qn(Bc(n))
         },
         toDOMStream(n, t) {
             throw new Error('"toDOMStream" not available in this environment')
         },
         toNodeStream(n, t) {
             throw new Error('"toNodeStream" not available in this environment')
         }
     },
-    Zn = n => (n.next(), n);
+    Qn = n => (n.next(), n);
 
 function* _c(n) {
     let t, e = !1,
         i = [],
         r, s, o, a = 0;
 
     function l() {
-        return s === "peek" ? ne(i, o)[0] : ([r, i, a] = ne(i, o), r)
+        return s === "peek" ? se(i, o)[0] : ([r, i, a] = se(i, o), r)
     }({
         cmd: s,
         size: o
     } = yield null);
     const c = vc(n)[Symbol.iterator]();
     try {
         do
@@ -952,21 +952,21 @@
     } finally {
         e === !1 && typeof c.return == "function" && c.return(null)
     }
     return null
 }
 
 function wc(n) {
-    return te(this, arguments, function*() {
+    return ne(this, arguments, function*() {
         let e, i = !1,
             r = [],
             s, o, a, l = 0;
 
         function c() {
-            return o === "peek" ? ne(r, a)[0] : ([s, r, l] = ne(r, a), s)
+            return o === "peek" ? se(r, a)[0] : ([s, r, l] = se(r, a), s)
         }({
             cmd: o,
             size: a
         } = yield yield M(null));
         const d = bc(n)[Symbol.asyncIterator]();
         try {
             do
@@ -984,22 +984,22 @@
             i === !1 && typeof d.return == "function" && (yield M(d.return(new Uint8Array(0))))
         }
         return yield M(null)
     })
 }
 
 function Sc(n) {
-    return te(this, arguments, function*() {
+    return ne(this, arguments, function*() {
         let e = !1,
             i = !1,
             r = [],
             s, o, a, l = 0;
 
         function c() {
-            return o === "peek" ? ne(r, a)[0] : ([s, r, l] = ne(r, a), s)
+            return o === "peek" ? se(r, a)[0] : ([s, r, l] = se(r, a), s)
         }({
             cmd: o,
             size: a
         } = yield yield M(null));
         const d = new Ic(n);
         try {
             do
@@ -1026,198 +1026,198 @@
     get closed() {
         return this.reader ? this.reader.closed.catch(() => {}) : Promise.resolve()
     }
     releaseLock() {
         this.reader && this.reader.releaseLock(), this.reader = null
     }
     cancel(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const {
                 reader: e,
                 source: i
             } = this;
             e && (yield e.cancel(t).catch(() => {})), i && i.locked && this.releaseLock()
         })
     }
     read(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             if (t === 0) return {
                 done: this.reader == null,
                 value: new Uint8Array(0)
             };
             const e = yield this.reader.read();
             return !e.done && (e.value = U(e)), e
         })
     }
 }
-const lr = (n, t) => {
+const ur = (n, t) => {
     const e = r => i([t, r]);
     let i;
     return [t, e, new Promise(r => (i = r) && n.once(t, e))]
 };
 
 function Bc(n) {
-    return te(this, arguments, function*() {
+    return ne(this, arguments, function*() {
         const e = [];
         let i = "error",
             r = !1,
             s = null,
             o, a, l = 0,
             c = [],
             d;
 
         function h() {
-            return o === "peek" ? ne(c, a)[0] : ([d, c, l] = ne(c, a), d)
+            return o === "peek" ? se(c, a)[0] : ([d, c, l] = se(c, a), d)
         }
         if ({
                 cmd: o,
                 size: a
             } = yield yield M(null), n.isTTY) return yield yield M(new Uint8Array(0)), yield M(null);
         try {
-            e[0] = lr(n, "end"), e[1] = lr(n, "error");
+            e[0] = ur(n, "end"), e[1] = ur(n, "error");
             do {
-                if (e[2] = lr(n, "readable"), [i, s] = yield M(Promise.race(e.map(_ => _[2]))), i === "error") break;
+                if (e[2] = ur(n, "readable"), [i, s] = yield M(Promise.race(e.map(_ => _[2]))), i === "error") break;
                 if ((r = i === "end") || (Number.isFinite(a - l) ? (d = U(n.read(a - l)), d.byteLength < a - l && (d = U(n.read()))) : d = U(n.read()), d.byteLength > 0 && (c.push(d), l += d.byteLength)), r || a <= l)
                     do({
                         cmd: o,
                         size: a
                     } = yield yield M(h())); while (a < l)
             } while (!r)
         } finally {
             yield M(y(e, i === "error" ? s : null))
         }
         return yield M(null);
 
-        function y(_, G) {
-            return d = c = null, new Promise((et, ot) => {
-                for (const [nt, He] of _) n.off(nt, He);
+        function y(_, V) {
+            return d = c = null, new Promise((P, et) => {
+                for (const [q, Rt] of _) n.off(q, Rt);
                 try {
-                    const nt = n.destroy;
-                    nt && nt.call(n, G), G = void 0
-                } catch (nt) {
-                    G = nt || G
+                    const q = n.destroy;
+                    q && q.call(n, V), V = void 0
+                } catch (q) {
+                    V = q || V
                 } finally {
-                    G != null ? ot(G) : et()
+                    V != null ? et(V) : P()
                 }
             })
         }
     })
 }
 var Nt;
 (function(n) {
     n[n.V1 = 0] = "V1", n[n.V2 = 1] = "V2", n[n.V3 = 2] = "V3", n[n.V4 = 3] = "V4", n[n.V5 = 4] = "V5"
 })(Nt || (Nt = {}));
-var xt;
+var Mt;
 (function(n) {
     n[n.Sparse = 0] = "Sparse", n[n.Dense = 1] = "Dense"
-})(xt || (xt = {}));
+})(Mt || (Mt = {}));
 var Bt;
 (function(n) {
     n[n.HALF = 0] = "HALF", n[n.SINGLE = 1] = "SINGLE", n[n.DOUBLE = 2] = "DOUBLE"
 })(Bt || (Bt = {}));
-var ye;
+var be;
 (function(n) {
     n[n.DAY = 0] = "DAY", n[n.MILLISECOND = 1] = "MILLISECOND"
-})(ye || (ye = {}));
-var V;
+})(be || (be = {}));
+var $;
 (function(n) {
     n[n.SECOND = 0] = "SECOND", n[n.MILLISECOND = 1] = "MILLISECOND", n[n.MICROSECOND = 2] = "MICROSECOND", n[n.NANOSECOND = 3] = "NANOSECOND"
-})(V || (V = {}));
-var Be;
+})($ || ($ = {}));
+var De;
 (function(n) {
     n[n.YEAR_MONTH = 0] = "YEAR_MONTH", n[n.DAY_TIME = 1] = "DAY_TIME", n[n.MONTH_DAY_NANO = 2] = "MONTH_DAY_NANO"
-})(Be || (Be = {}));
-var $;
+})(De || (De = {}));
+var j;
 (function(n) {
     n[n.NONE = 0] = "NONE", n[n.Schema = 1] = "Schema", n[n.DictionaryBatch = 2] = "DictionaryBatch", n[n.RecordBatch = 3] = "RecordBatch", n[n.Tensor = 4] = "Tensor", n[n.SparseTensor = 5] = "SparseTensor"
-})($ || ($ = {}));
+})(j || (j = {}));
 var u;
 (function(n) {
     n[n.NONE = 0] = "NONE", n[n.Null = 1] = "Null", n[n.Int = 2] = "Int", n[n.Float = 3] = "Float", n[n.Binary = 4] = "Binary", n[n.Utf8 = 5] = "Utf8", n[n.Bool = 6] = "Bool", n[n.Decimal = 7] = "Decimal", n[n.Date = 8] = "Date", n[n.Time = 9] = "Time", n[n.Timestamp = 10] = "Timestamp", n[n.Interval = 11] = "Interval", n[n.List = 12] = "List", n[n.Struct = 13] = "Struct", n[n.Union = 14] = "Union", n[n.FixedSizeBinary = 15] = "FixedSizeBinary", n[n.FixedSizeList = 16] = "FixedSizeList", n[n.Map = 17] = "Map", n[n.Dictionary = -1] = "Dictionary", n[n.Int8 = -2] = "Int8", n[n.Int16 = -3] = "Int16", n[n.Int32 = -4] = "Int32", n[n.Int64 = -5] = "Int64", n[n.Uint8 = -6] = "Uint8", n[n.Uint16 = -7] = "Uint16", n[n.Uint32 = -8] = "Uint32", n[n.Uint64 = -9] = "Uint64", n[n.Float16 = -10] = "Float16", n[n.Float32 = -11] = "Float32", n[n.Float64 = -12] = "Float64", n[n.DateDay = -13] = "DateDay", n[n.DateMillisecond = -14] = "DateMillisecond", n[n.TimestampSecond = -15] = "TimestampSecond", n[n.TimestampMillisecond = -16] = "TimestampMillisecond", n[n.TimestampMicrosecond = -17] = "TimestampMicrosecond", n[n.TimestampNanosecond = -18] = "TimestampNanosecond", n[n.TimeSecond = -19] = "TimeSecond", n[n.TimeMillisecond = -20] = "TimeMillisecond", n[n.TimeMicrosecond = -21] = "TimeMicrosecond", n[n.TimeNanosecond = -22] = "TimeNanosecond", n[n.DenseUnion = -23] = "DenseUnion", n[n.SparseUnion = -24] = "SparseUnion", n[n.IntervalDayTime = -25] = "IntervalDayTime", n[n.IntervalYearMonth = -26] = "IntervalYearMonth"
 })(u || (u = {}));
-var ae;
+var de;
 (function(n) {
     n[n.OFFSET = 0] = "OFFSET", n[n.DATA = 1] = "DATA", n[n.VALIDITY = 2] = "VALIDITY", n[n.TYPE = 3] = "TYPE"
-})(ae || (ae = {}));
+})(de || (de = {}));
 const Oc = void 0;
 
-function En(n) {
+function Rn(n) {
     if (n === null) return "null";
     if (n === Oc) return "undefined";
     switch (typeof n) {
         case "number":
             return `${n}`;
         case "bigint":
             return `${n}`;
         case "string":
             return `"${n}"`
     }
-    return typeof n[Symbol.toPrimitive] == "function" ? n[Symbol.toPrimitive]("string") : ArrayBuffer.isView(n) ? n instanceof Wn || n instanceof Yn ? `[${[...n].map(t=>En(t))}]` : `[${n}]` : ArrayBuffer.isView(n) ? `[${n}]` : JSON.stringify(n, (t, e) => typeof e == "bigint" ? `${e}` : e)
+    return typeof n[Symbol.toPrimitive] == "function" ? n[Symbol.toPrimitive]("string") : ArrayBuffer.isView(n) ? n instanceof Wn || n instanceof Yn ? `[${[...n].map(t=>Rn(t))}]` : `[${n}]` : ArrayBuffer.isView(n) ? `[${n}]` : JSON.stringify(n, (t, e) => typeof e == "bigint" ? `${e}` : e)
 }
 const Fc = Symbol.for("isArrowBigNum");
 
-function zt(n, ...t) {
-    return t.length === 0 ? Object.setPrototypeOf(q(this.TypedArray, n), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(n, ...t), this.constructor.prototype)
+function Wt(n, ...t) {
+    return t.length === 0 ? Object.setPrototypeOf(K(this.TypedArray, n), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(n, ...t), this.constructor.prototype)
 }
-zt.prototype[Fc] = !0;
-zt.prototype.toJSON = function() {
-    return `"${ze(this)}"`
+Wt.prototype[Fc] = !0;
+Wt.prototype.toJSON = function() {
+    return `"${Ge(this)}"`
 };
-zt.prototype.valueOf = function() {
-    return Ao(this)
+Wt.prototype.valueOf = function() {
+    return Do(this)
 };
-zt.prototype.toString = function() {
-    return ze(this)
+Wt.prototype.toString = function() {
+    return Ge(this)
 };
-zt.prototype[Symbol.toPrimitive] = function(n = "default") {
+Wt.prototype[Symbol.toPrimitive] = function(n = "default") {
     switch (n) {
         case "number":
-            return Ao(this);
+            return Do(this);
         case "string":
-            return ze(this);
+            return Ge(this);
         case "default":
-            return Sr(this)
+            return Or(this)
     }
-    return ze(this)
+    return Ge(this)
 };
 
-function rn(...n) {
-    return zt.apply(this, n)
+function on(...n) {
+    return Wt.apply(this, n)
 }
 
-function sn(...n) {
-    return zt.apply(this, n)
+function an(...n) {
+    return Wt.apply(this, n)
 }
 
-function Rn(...n) {
-    return zt.apply(this, n)
+function Cn(...n) {
+    return Wt.apply(this, n)
 }
-Object.setPrototypeOf(rn.prototype, Object.create(Int32Array.prototype));
-Object.setPrototypeOf(sn.prototype, Object.create(Uint32Array.prototype));
-Object.setPrototypeOf(Rn.prototype, Object.create(Uint32Array.prototype));
-Object.assign(rn.prototype, zt.prototype, {
-    constructor: rn,
+Object.setPrototypeOf(on.prototype, Object.create(Int32Array.prototype));
+Object.setPrototypeOf(an.prototype, Object.create(Uint32Array.prototype));
+Object.setPrototypeOf(Cn.prototype, Object.create(Uint32Array.prototype));
+Object.assign(on.prototype, Wt.prototype, {
+    constructor: on,
     signed: !0,
     TypedArray: Int32Array,
     BigIntArray: Wn
 });
-Object.assign(sn.prototype, zt.prototype, {
-    constructor: sn,
+Object.assign(an.prototype, Wt.prototype, {
+    constructor: an,
     signed: !1,
     TypedArray: Uint32Array,
     BigIntArray: Yn
 });
-Object.assign(Rn.prototype, zt.prototype, {
-    constructor: Rn,
+Object.assign(Cn.prototype, Wt.prototype, {
+    constructor: Cn,
     signed: !0,
     TypedArray: Uint32Array,
     BigIntArray: Yn
 });
 
-function Ao(n) {
+function Do(n) {
     const {
         buffer: t,
         byteOffset: e,
         length: i,
         signed: r
     } = n, s = new Yn(t, e, i), o = r && s[s.length - 1] & BigInt(1) << BigInt(63);
     let a = BigInt(o ? 1 : 0),
@@ -1225,62 +1225,62 @@
     if (o) {
         for (const c of s) a += ~c * (BigInt(1) << BigInt(32) * l++);
         a *= BigInt(-1)
     } else
         for (const c of s) a += c * (BigInt(1) << BigInt(32) * l++);
     return a
 }
-let ze, Sr;
-uc ? (Sr = n => n.byteLength === 8 ? new n.BigIntArray(n.buffer, n.byteOffset, 1)[0] : cr(n), ze = n => n.byteLength === 8 ? `${new n.BigIntArray(n.buffer,n.byteOffset,1)[0]}` : cr(n)) : (ze = cr, Sr = ze);
+let Ge, Or;
+uc ? (Or = n => n.byteLength === 8 ? new n.BigIntArray(n.buffer, n.byteOffset, 1)[0] : dr(n), Ge = n => n.byteLength === 8 ? `${new n.BigIntArray(n.buffer,n.byteOffset,1)[0]}` : dr(n)) : (Ge = dr, Or = Ge);
 
-function cr(n) {
+function dr(n) {
     let t = "";
     const e = new Uint32Array(2);
     let i = new Uint16Array(n.buffer, n.byteOffset, n.byteLength / 2);
     const r = new Uint32Array((i = new Uint16Array(i).reverse()).buffer);
     let s = -1;
     const o = i.length - 1;
     do {
         for (e[0] = i[s = 0]; s < o;) i[s++] = e[1] = e[0] / 10, e[0] = (e[0] - e[1] * 10 << 16) + i[s];
         i[s] = e[1] = e[0] / 10, e[0] = e[0] - e[1] * 10, t = `${e[0]}${t}`
     } while (r[0] || r[1] || r[2] || r[3]);
     return t ?? "0"
 }
-class qr {
+class Zr {
     static new(t, e) {
         switch (e) {
             case !0:
-                return new rn(t);
+                return new on(t);
             case !1:
-                return new sn(t)
+                return new an(t)
         }
         switch (t.constructor) {
             case Int8Array:
             case Int16Array:
             case Int32Array:
             case Wn:
-                return new rn(t)
+                return new on(t)
         }
-        return t.byteLength === 16 ? new Rn(t) : new sn(t)
+        return t.byteLength === 16 ? new Cn(t) : new an(t)
     }
     static signed(t) {
-        return new rn(t)
+        return new on(t)
     }
     static unsigned(t) {
-        return new sn(t)
+        return new an(t)
     }
     static decimal(t) {
-        return new Rn(t)
+        return new Cn(t)
     }
     constructor(t, e) {
-        return qr.new(t, e)
+        return Zr.new(t, e)
     }
 }
-var Do, To, No, Mo, xo, Lo, Eo, Ro, Co, ko, Uo, Vo, $o, Po, jo, zo, Wo, Yo, Go;
-class S {
+var To, No, xo, Mo, Lo, Eo, Ro, Co, ko, Uo, $o, Vo, Po, jo, zo, Wo, Yo, Go, Ho;
+class I {
     static isNull(t) {
         return t?.typeId === u.Null
     }
     static isInt(t) {
         return t?.typeId === u.Int
     }
     static isFloat(t) {
@@ -1328,36 +1328,36 @@
     static isMap(t) {
         return t?.typeId === u.Map
     }
     static isDictionary(t) {
         return t?.typeId === u.Dictionary
     }
     static isDenseUnion(t) {
-        return S.isUnion(t) && t.mode === xt.Dense
+        return I.isUnion(t) && t.mode === Mt.Dense
     }
     static isSparseUnion(t) {
-        return S.isUnion(t) && t.mode === xt.Sparse
+        return I.isUnion(t) && t.mode === Mt.Sparse
     }
     get typeId() {
         return u.NONE
     }
 }
-Do = Symbol.toStringTag;
-S[Do] = (n => (n.children = null, n.ArrayType = Array, n[Symbol.toStringTag] = "DataType"))(S.prototype);
-let Oe = class extends S {
+To = Symbol.toStringTag;
+I[To] = (n => (n.children = null, n.ArrayType = Array, n[Symbol.toStringTag] = "DataType"))(I.prototype);
+let Te = class extends I {
     toString() {
         return "Null"
     }
     get typeId() {
         return u.Null
     }
 };
-To = Symbol.toStringTag;
-Oe[To] = (n => n[Symbol.toStringTag] = "Null")(Oe.prototype);
-class Fe extends S {
+No = Symbol.toStringTag;
+Te[No] = (n => n[Symbol.toStringTag] = "Null")(Te.prototype);
+class Ne extends I {
     constructor(t, e) {
         super(), this.isSigned = t, this.bitWidth = e
     }
     get typeId() {
         return u.Int
     }
     get ArrayType() {
@@ -1373,28 +1373,28 @@
         }
         throw new Error(`Unrecognized ${this[Symbol.toStringTag]} type`)
     }
     toString() {
         return `${this.isSigned?"I":"Ui"}nt${this.bitWidth}`
     }
 }
-No = Symbol.toStringTag;
-Fe[No] = (n => (n.isSigned = null, n.bitWidth = null, n[Symbol.toStringTag] = "Int"))(Fe.prototype);
-class Cn extends Fe {
+xo = Symbol.toStringTag;
+Ne[xo] = (n => (n.isSigned = null, n.bitWidth = null, n[Symbol.toStringTag] = "Int"))(Ne.prototype);
+class kn extends Ne {
     constructor() {
         super(!0, 32)
     }
     get ArrayType() {
         return Int32Array
     }
 }
-Object.defineProperty(Cn.prototype, "ArrayType", {
+Object.defineProperty(kn.prototype, "ArrayType", {
     value: Int32Array
 });
-class kn extends S {
+class Un extends I {
     constructor(t) {
         super(), this.precision = t
     }
     get typeId() {
         return u.Float
     }
     get ArrayType() {
@@ -1409,129 +1409,129 @@
         throw new Error(`Unrecognized ${this[Symbol.toStringTag]} type`)
     }
     toString() {
         return `Float${this.precision<<5||16}`
     }
 }
 Mo = Symbol.toStringTag;
-kn[Mo] = (n => (n.precision = null, n[Symbol.toStringTag] = "Float"))(kn.prototype);
-let ui = class extends S {
+Un[Mo] = (n => (n.precision = null, n[Symbol.toStringTag] = "Float"))(Un.prototype);
+let hi = class extends I {
     constructor() {
         super()
     }
     get typeId() {
         return u.Binary
     }
     toString() {
         return "Binary"
     }
 };
-xo = Symbol.toStringTag;
-ui[xo] = (n => (n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "Binary"))(ui.prototype);
-let di = class extends S {
+Lo = Symbol.toStringTag;
+hi[Lo] = (n => (n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "Binary"))(hi.prototype);
+let fi = class extends I {
     constructor() {
         super()
     }
     get typeId() {
         return u.Utf8
     }
     toString() {
         return "Utf8"
     }
 };
-Lo = Symbol.toStringTag;
-di[Lo] = (n => (n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "Utf8"))(di.prototype);
-let hi = class extends S {
+Eo = Symbol.toStringTag;
+fi[Eo] = (n => (n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "Utf8"))(fi.prototype);
+let pi = class extends I {
     constructor() {
         super()
     }
     get typeId() {
         return u.Bool
     }
     toString() {
         return "Bool"
     }
 };
-Eo = Symbol.toStringTag;
-hi[Eo] = (n => (n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "Bool"))(hi.prototype);
-let fi = class extends S {
+Ro = Symbol.toStringTag;
+pi[Ro] = (n => (n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "Bool"))(pi.prototype);
+let yi = class extends I {
     constructor(t, e, i = 128) {
         super(), this.scale = t, this.precision = e, this.bitWidth = i
     }
     get typeId() {
         return u.Decimal
     }
     toString() {
         return `Decimal[${this.precision}e${this.scale>0?"+":""}${this.scale}]`
     }
 };
-Ro = Symbol.toStringTag;
-fi[Ro] = (n => (n.scale = null, n.precision = null, n.ArrayType = Uint32Array, n[Symbol.toStringTag] = "Decimal"))(fi.prototype);
-class pi extends S {
+Co = Symbol.toStringTag;
+yi[Co] = (n => (n.scale = null, n.precision = null, n.ArrayType = Uint32Array, n[Symbol.toStringTag] = "Decimal"))(yi.prototype);
+class mi extends I {
     constructor(t) {
         super(), this.unit = t
     }
     get typeId() {
         return u.Date
     }
     toString() {
-        return `Date${(this.unit+1)*32}<${ye[this.unit]}>`
+        return `Date${(this.unit+1)*32}<${be[this.unit]}>`
     }
 }
-Co = Symbol.toStringTag;
-pi[Co] = (n => (n.unit = null, n.ArrayType = Int32Array, n[Symbol.toStringTag] = "Date"))(pi.prototype);
-class Un extends S {
+ko = Symbol.toStringTag;
+mi[ko] = (n => (n.unit = null, n.ArrayType = Int32Array, n[Symbol.toStringTag] = "Date"))(mi.prototype);
+class $n extends I {
     constructor(t, e) {
         super(), this.unit = t, this.bitWidth = e
     }
     get typeId() {
         return u.Time
     }
     toString() {
-        return `Time${this.bitWidth}<${V[this.unit]}>`
+        return `Time${this.bitWidth}<${$[this.unit]}>`
     }
     get ArrayType() {
         switch (this.bitWidth) {
             case 32:
                 return Int32Array;
             case 64:
                 return Wn
         }
         throw new Error(`Unrecognized ${this[Symbol.toStringTag]} type`)
     }
 }
-ko = Symbol.toStringTag;
-Un[ko] = (n => (n.unit = null, n.bitWidth = null, n[Symbol.toStringTag] = "Time"))(Un.prototype);
-class yi extends S {
+Uo = Symbol.toStringTag;
+$n[Uo] = (n => (n.unit = null, n.bitWidth = null, n[Symbol.toStringTag] = "Time"))($n.prototype);
+class vi extends I {
     constructor(t, e) {
         super(), this.unit = t, this.timezone = e
     }
     get typeId() {
         return u.Timestamp
     }
     toString() {
-        return `Timestamp<${V[this.unit]}${this.timezone?`, ${this.timezone}`:""}>`
+        return `Timestamp<${$[this.unit]}${this.timezone?`, ${this.timezone}`:""}>`
     }
 }
-Uo = Symbol.toStringTag;
-yi[Uo] = (n => (n.unit = null, n.timezone = null, n.ArrayType = Int32Array, n[Symbol.toStringTag] = "Timestamp"))(yi.prototype);
-class mi extends S {
+$o = Symbol.toStringTag;
+vi[$o] = (n => (n.unit = null, n.timezone = null, n.ArrayType = Int32Array, n[Symbol.toStringTag] = "Timestamp"))(vi.prototype);
+class bi extends I {
     constructor(t) {
         super(), this.unit = t
     }
     get typeId() {
         return u.Interval
     }
     toString() {
-        return `Interval<${Be[this.unit]}>`
+        return `Interval<${De[this.unit]}>`
     }
 }
 Vo = Symbol.toStringTag;
-mi[Vo] = (n => (n.unit = null, n.ArrayType = Int32Array, n[Symbol.toStringTag] = "Interval"))(mi.prototype);
-let vi = class extends S {
+bi[Vo] = (n => (n.unit = null, n.ArrayType = Int32Array, n[Symbol.toStringTag] = "Interval"))(bi.prototype);
+let gi = class extends I {
     constructor(t) {
         super(), this.children = [t]
     }
     get typeId() {
         return u.List
     }
     toString() {
@@ -1543,56 +1543,56 @@
     get valueField() {
         return this.children[0]
     }
     get ArrayType() {
         return this.valueType.ArrayType
     }
 };
-$o = Symbol.toStringTag;
-vi[$o] = (n => (n.children = null, n[Symbol.toStringTag] = "List"))(vi.prototype);
-class yt extends S {
+Po = Symbol.toStringTag;
+gi[Po] = (n => (n.children = null, n[Symbol.toStringTag] = "List"))(gi.prototype);
+class mt extends I {
     constructor(t) {
         super(), this.children = t
     }
     get typeId() {
         return u.Struct
     }
     toString() {
         return `Struct<{${this.children.map(t=>`${t.name}:${t.type}`).join(", ")}}>`
     }
 }
-Po = Symbol.toStringTag;
-yt[Po] = (n => (n.children = null, n[Symbol.toStringTag] = "Struct"))(yt.prototype);
-class bi extends S {
+jo = Symbol.toStringTag;
+mt[jo] = (n => (n.children = null, n[Symbol.toStringTag] = "Struct"))(mt.prototype);
+class _i extends I {
     constructor(t, e, i) {
         super(), this.mode = t, this.children = i, this.typeIds = e = Int32Array.from(e), this.typeIdToChildIndex = e.reduce((r, s, o) => (r[s] = o) && r || r, Object.create(null))
     }
     get typeId() {
         return u.Union
     }
     toString() {
         return `${this[Symbol.toStringTag]}<${this.children.map(t=>`${t.type}`).join(" | ")}>`
     }
 }
-jo = Symbol.toStringTag;
-bi[jo] = (n => (n.mode = null, n.typeIds = null, n.children = null, n.typeIdToChildIndex = null, n.ArrayType = Int8Array, n[Symbol.toStringTag] = "Union"))(bi.prototype);
-let gi = class extends S {
+zo = Symbol.toStringTag;
+_i[zo] = (n => (n.mode = null, n.typeIds = null, n.children = null, n.typeIdToChildIndex = null, n.ArrayType = Int8Array, n[Symbol.toStringTag] = "Union"))(_i.prototype);
+let wi = class extends I {
     constructor(t) {
         super(), this.byteWidth = t
     }
     get typeId() {
         return u.FixedSizeBinary
     }
     toString() {
         return `FixedSizeBinary[${this.byteWidth}]`
     }
 };
-zo = Symbol.toStringTag;
-gi[zo] = (n => (n.byteWidth = null, n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "FixedSizeBinary"))(gi.prototype);
-let _i = class extends S {
+Wo = Symbol.toStringTag;
+wi[Wo] = (n => (n.byteWidth = null, n.ArrayType = Uint8Array, n[Symbol.toStringTag] = "FixedSizeBinary"))(wi.prototype);
+let Si = class extends I {
     constructor(t, e) {
         super(), this.listSize = t, this.children = [e]
     }
     get typeId() {
         return u.FixedSizeList
     }
     get valueType() {
@@ -1604,17 +1604,17 @@
     get ArrayType() {
         return this.valueType.ArrayType
     }
     toString() {
         return `FixedSizeList[${this.listSize}]<${this.valueType}>`
     }
 };
-Wo = Symbol.toStringTag;
-_i[Wo] = (n => (n.children = null, n.listSize = null, n[Symbol.toStringTag] = "FixedSizeList"))(_i.prototype);
-class wi extends S {
+Yo = Symbol.toStringTag;
+Si[Yo] = (n => (n.children = null, n.listSize = null, n[Symbol.toStringTag] = "FixedSizeList"))(Si.prototype);
+class Ii extends I {
     constructor(t, e = !1) {
         super(), this.children = [t], this.keysSorted = e
     }
     get typeId() {
         return u.Map
     }
     get keyType() {
@@ -1626,18 +1626,18 @@
     get childType() {
         return this.children[0].type
     }
     toString() {
         return `Map<{${this.children[0].type.children.map(t=>`${t.name}:${t.type}`).join(", ")}}>`
     }
 }
-Yo = Symbol.toStringTag;
-wi[Yo] = (n => (n.children = null, n.keysSorted = null, n[Symbol.toStringTag] = "Map_"))(wi.prototype);
+Go = Symbol.toStringTag;
+Ii[Go] = (n => (n.children = null, n.keysSorted = null, n[Symbol.toStringTag] = "Map_"))(Ii.prototype);
 const Ac = (n => () => ++n)(-1);
-class dn extends S {
+class pn extends I {
     constructor(t, e, i, r) {
         super(), this.indices = e, this.dictionary = t, this.isOrdered = r || !1, this.id = i == null ? Ac() : typeof i == "number" ? i : i.low
     }
     get typeId() {
         return u.Dictionary
     }
     get children() {
@@ -1649,18 +1649,18 @@
     get ArrayType() {
         return this.dictionary.ArrayType
     }
     toString() {
         return `Dictionary<${this.indices}, ${this.dictionary}>`
     }
 }
-Go = Symbol.toStringTag;
-dn[Go] = (n => (n.id = null, n.indices = null, n.isOrdered = null, n.dictionary = null, n[Symbol.toStringTag] = "Dictionary"))(dn.prototype);
+Ho = Symbol.toStringTag;
+pn[Ho] = (n => (n.id = null, n.indices = null, n.isOrdered = null, n.dictionary = null, n[Symbol.toStringTag] = "Dictionary"))(pn.prototype);
 
-function le(n) {
+function he(n) {
     const t = n;
     switch (n.typeId) {
         case u.Decimal:
             return n.bitWidth / 32;
         case u.Timestamp:
             return 2;
         case u.Date:
@@ -1682,15 +1682,15 @@
     visit(...t) {
         return this.getVisitFn(t[0], !1).apply(this, t)
     }
     getVisitFn(t, e = !0) {
         return Dc(this, t, e)
     }
     getVisitFnByTypeId(t, e = !0) {
-        return Xe(this, t, e)
+        return tn(this, t, e)
     }
     visitNull(t, ...e) {
         return null
     }
     visitBool(t, ...e) {
         return null
     }
@@ -1741,18 +1741,18 @@
     }
     visitMap(t, ...e) {
         return null
     }
 }
 
 function Dc(n, t, e = !0) {
-    return typeof t == "number" ? Xe(n, t, e) : typeof t == "string" && t in u ? Xe(n, u[t], e) : t && t instanceof S ? Xe(n, Ts(t), e) : t?.type && t.type instanceof S ? Xe(n, Ts(t.type), e) : Xe(n, u.NONE, e)
+    return typeof t == "number" ? tn(n, t, e) : typeof t == "string" && t in u ? tn(n, u[t], e) : t && t instanceof I ? tn(n, Ns(t), e) : t?.type && t.type instanceof I ? tn(n, Ns(t.type), e) : tn(n, u.NONE, e)
 }
 
-function Xe(n, t, e = !0) {
+function tn(n, t, e = !0) {
     let i = null;
     switch (t) {
         case u.Null:
             i = n.visitNull;
             break;
         case u.Bool:
             i = n.visitBool;
@@ -1882,15 +1882,15 @@
             break
     }
     if (typeof i == "function") return i;
     if (!e) return () => null;
     throw new Error(`Unrecognized type '${u[t]}'`)
 }
 
-function Ts(n) {
+function Ns(n) {
     switch (n.typeId) {
         case u.Null:
             return u.Null;
         case u.Int: {
             const {
                 bitWidth: t,
                 isSigned: e
@@ -1923,63 +1923,63 @@
             return u.Utf8;
         case u.Bool:
             return u.Bool;
         case u.Decimal:
             return u.Decimal;
         case u.Time:
             switch (n.unit) {
-                case V.SECOND:
+                case $.SECOND:
                     return u.TimeSecond;
-                case V.MILLISECOND:
+                case $.MILLISECOND:
                     return u.TimeMillisecond;
-                case V.MICROSECOND:
+                case $.MICROSECOND:
                     return u.TimeMicrosecond;
-                case V.NANOSECOND:
+                case $.NANOSECOND:
                     return u.TimeNanosecond
             }
             return u.Time;
         case u.Timestamp:
             switch (n.unit) {
-                case V.SECOND:
+                case $.SECOND:
                     return u.TimestampSecond;
-                case V.MILLISECOND:
+                case $.MILLISECOND:
                     return u.TimestampMillisecond;
-                case V.MICROSECOND:
+                case $.MICROSECOND:
                     return u.TimestampMicrosecond;
-                case V.NANOSECOND:
+                case $.NANOSECOND:
                     return u.TimestampNanosecond
             }
             return u.Timestamp;
         case u.Date:
             switch (n.unit) {
-                case ye.DAY:
+                case be.DAY:
                     return u.DateDay;
-                case ye.MILLISECOND:
+                case be.MILLISECOND:
                     return u.DateMillisecond
             }
             return u.Date;
         case u.Interval:
             switch (n.unit) {
-                case Be.DAY_TIME:
+                case De.DAY_TIME:
                     return u.IntervalDayTime;
-                case Be.YEAR_MONTH:
+                case De.YEAR_MONTH:
                     return u.IntervalYearMonth
             }
             return u.Interval;
         case u.Map:
             return u.Map;
         case u.List:
             return u.List;
         case u.Struct:
             return u.Struct;
         case u.Union:
             switch (n.mode) {
-                case xt.Dense:
+                case Mt.Dense:
                     return u.DenseUnion;
-                case xt.Sparse:
+                case Mt.Sparse:
                     return u.SparseUnion
             }
             return u.Union;
         case u.FixedSizeBinary:
             return u.FixedSizeBinary;
         case u.FixedSizeList:
             return u.FixedSizeList;
@@ -2009,179 +2009,179 @@
 R.prototype.visitTimeMillisecond = null;
 R.prototype.visitTimeMicrosecond = null;
 R.prototype.visitTimeNanosecond = null;
 R.prototype.visitDenseUnion = null;
 R.prototype.visitSparseUnion = null;
 R.prototype.visitIntervalDayTime = null;
 R.prototype.visitIntervalYearMonth = null;
-const Ho = new Float64Array(1),
-    Ke = new Uint32Array(Ho.buffer);
+const qo = new Float64Array(1),
+    Xe = new Uint32Array(qo.buffer);
 
-function qo(n) {
+function Jo(n) {
     const t = (n & 31744) >> 10,
         e = (n & 1023) / 1024,
         i = Math.pow(-1, (n & 32768) >> 15);
     switch (t) {
         case 31:
             return i * (e ? Number.NaN : 1 / 0);
         case 0:
             return i * (e ? 6103515625e-14 * e : 0)
     }
     return i * Math.pow(2, t - 15) * (1 + e)
 }
 
 function Tc(n) {
     if (n !== n) return 32256;
-    Ho[0] = n;
-    const t = (Ke[1] & 2147483648) >> 16 & 65535;
-    let e = Ke[1] & 2146435072,
+    qo[0] = n;
+    const t = (Xe[1] & 2147483648) >> 16 & 65535;
+    let e = Xe[1] & 2146435072,
         i = 0;
-    return e >= 1089470464 ? Ke[0] > 0 ? e = 31744 : (e = (e & 2080374784) >> 16, i = (Ke[1] & 1048575) >> 10) : e <= 1056964608 ? (i = 1048576 + (Ke[1] & 1048575), i = 1048576 + (i << (e >> 20) - 998) >> 21, e = 0) : (e = e - 1056964608 >> 10, i = (Ke[1] & 1048575) + 512 >> 10), t | e | i & 65535
+    return e >= 1089470464 ? Xe[0] > 0 ? e = 31744 : (e = (e & 2080374784) >> 16, i = (Xe[1] & 1048575) >> 10) : e <= 1056964608 ? (i = 1048576 + (Xe[1] & 1048575), i = 1048576 + (i << (e >> 20) - 998) >> 21, e = 0) : (e = e - 1056964608 >> 10, i = (Xe[1] & 1048575) + 512 >> 10), t | e | i & 65535
 }
-class A extends R {}
+class D extends R {}
 
-function N(n) {
+function x(n) {
     return (t, e, i) => {
         if (t.setValid(e, i != null)) return n(t, e, i)
     }
 }
 const Nc = (n, t, e) => {
         n[t] = Math.trunc(e / 864e5)
     },
-    Jr = (n, t, e) => {
+    Xr = (n, t, e) => {
         n[t] = Math.trunc(e % 4294967296), n[t + 1] = Math.trunc(e / 4294967296)
     },
-    Mc = (n, t, e) => {
+    xc = (n, t, e) => {
         n[t] = Math.trunc(e * 1e3 % 4294967296), n[t + 1] = Math.trunc(e * 1e3 / 4294967296)
     },
-    xc = (n, t, e) => {
+    Mc = (n, t, e) => {
         n[t] = Math.trunc(e * 1e6 % 4294967296), n[t + 1] = Math.trunc(e * 1e6 / 4294967296)
     },
-    Jo = (n, t, e, i) => {
+    Ko = (n, t, e, i) => {
         if (e + 1 < t.length) {
             const {
                 [e]: r, [e + 1]: s
             } = t;
             n.set(i.subarray(0, s - r), r)
         }
     },
     Lc = ({
         offset: n,
         values: t
     }, e, i) => {
         const r = n + e;
         i ? t[r >> 3] |= 1 << r % 8 : t[r >> 3] &= ~(1 << r % 8)
     },
-    ve = ({
+    _e = ({
         values: n
     }, t, e) => {
         n[t] = e
     },
-    Kr = ({
+    Qr = ({
         values: n
     }, t, e) => {
         n[t] = e
     },
-    Ko = ({
+    Zo = ({
         values: n
     }, t, e) => {
         n[t] = Tc(e)
     },
     Ec = (n, t, e) => {
         switch (n.type.precision) {
             case Bt.HALF:
-                return Ko(n, t, e);
+                return Zo(n, t, e);
             case Bt.SINGLE:
             case Bt.DOUBLE:
-                return Kr(n, t, e)
+                return Qr(n, t, e)
         }
     },
-    Zo = ({
+    Xo = ({
         values: n
     }, t, e) => {
         Nc(n, t, e.valueOf())
     },
-    Xo = ({
+    Qo = ({
         values: n
     }, t, e) => {
-        Jr(n, t * 2, e.valueOf())
+        Xr(n, t * 2, e.valueOf())
     },
     Rc = ({
         stride: n,
         values: t
     }, e, i) => {
         t.set(i.subarray(0, n), n * e)
     },
     Cc = ({
         values: n,
         valueOffsets: t
-    }, e, i) => Jo(n, t, e, i),
+    }, e, i) => Ko(n, t, e, i),
     kc = ({
         values: n,
         valueOffsets: t
     }, e, i) => {
-        Jo(n, t, e, Wr(i))
+        Ko(n, t, e, Hr(i))
     },
     Uc = (n, t, e) => {
-        n.type.unit === ye.DAY ? Zo(n, t, e) : Xo(n, t, e)
+        n.type.unit === be.DAY ? Xo(n, t, e) : Qo(n, t, e)
     },
-    Qo = ({
-        values: n
-    }, t, e) => Jr(n, t * 2, e / 1e3),
     ta = ({
         values: n
-    }, t, e) => Jr(n, t * 2, e),
+    }, t, e) => Xr(n, t * 2, e / 1e3),
     ea = ({
         values: n
-    }, t, e) => Mc(n, t * 2, e),
+    }, t, e) => Xr(n, t * 2, e),
     na = ({
         values: n
     }, t, e) => xc(n, t * 2, e),
-    Vc = (n, t, e) => {
+    ia = ({
+        values: n
+    }, t, e) => Mc(n, t * 2, e),
+    $c = (n, t, e) => {
         switch (n.type.unit) {
-            case V.SECOND:
-                return Qo(n, t, e);
-            case V.MILLISECOND:
+            case $.SECOND:
                 return ta(n, t, e);
-            case V.MICROSECOND:
+            case $.MILLISECOND:
                 return ea(n, t, e);
-            case V.NANOSECOND:
-                return na(n, t, e)
+            case $.MICROSECOND:
+                return na(n, t, e);
+            case $.NANOSECOND:
+                return ia(n, t, e)
         }
     },
-    ia = ({
+    ra = ({
         values: n
     }, t, e) => {
         n[t] = e
     },
-    ra = ({
+    sa = ({
         values: n
     }, t, e) => {
         n[t] = e
     },
-    sa = ({
+    oa = ({
         values: n
     }, t, e) => {
         n[t] = e
     },
-    oa = ({
+    aa = ({
         values: n
     }, t, e) => {
         n[t] = e
     },
-    $c = (n, t, e) => {
+    Vc = (n, t, e) => {
         switch (n.type.unit) {
-            case V.SECOND:
-                return ia(n, t, e);
-            case V.MILLISECOND:
+            case $.SECOND:
                 return ra(n, t, e);
-            case V.MICROSECOND:
+            case $.MILLISECOND:
                 return sa(n, t, e);
-            case V.NANOSECOND:
-                return oa(n, t, e)
+            case $.MICROSECOND:
+                return oa(n, t, e);
+            case $.NANOSECOND:
+                return aa(n, t, e)
         }
     },
     Pc = ({
         values: n,
         stride: t
     }, e, i) => {
         n.set(i.subarray(0, t), t * e)
@@ -2210,122 +2210,122 @@
     },
     Wc = (n, t) => (e, i, r, s) => i && e(i, n, t[s]),
     Yc = (n, t) => (e, i, r, s) => i && e(i, n, t.get(s)),
     Gc = (n, t) => (e, i, r, s) => i && e(i, n, t.get(r.name)),
     Hc = (n, t) => (e, i, r, s) => i && e(i, n, t[r.name]),
     qc = (n, t, e) => {
         const i = n.type.children.map(s => Vt.getVisitFn(s.type)),
-            r = e instanceof Map ? Gc(t, e) : e instanceof P ? Yc(t, e) : Array.isArray(e) ? Wc(t, e) : Hc(t, e);
+            r = e instanceof Map ? Gc(t, e) : e instanceof z ? Yc(t, e) : Array.isArray(e) ? Wc(t, e) : Hc(t, e);
         n.type.children.forEach((s, o) => r(i[o], n.children[o], s, o))
     },
     Jc = (n, t, e) => {
-        n.type.mode === xt.Dense ? aa(n, t, e) : la(n, t, e)
+        n.type.mode === Mt.Dense ? la(n, t, e) : ca(n, t, e)
     },
-    aa = (n, t, e) => {
+    la = (n, t, e) => {
         const i = n.type.typeIdToChildIndex[n.typeIds[t]],
             r = n.children[i];
         Vt.visit(r, n.valueOffsets[t], e)
     },
-    la = (n, t, e) => {
+    ca = (n, t, e) => {
         const i = n.type.typeIdToChildIndex[n.typeIds[t]],
             r = n.children[i];
         Vt.visit(r, t, e)
     },
     Kc = (n, t, e) => {
         var i;
         (i = n.dictionary) === null || i === void 0 || i.set(n.values[t], e)
     },
     Zc = (n, t, e) => {
-        n.type.unit === Be.DAY_TIME ? ca(n, t, e) : ua(n, t, e)
+        n.type.unit === De.DAY_TIME ? ua(n, t, e) : da(n, t, e)
     },
-    ca = ({
+    ua = ({
         values: n
     }, t, e) => {
         n.set(e.subarray(0, 2), 2 * t)
     },
-    ua = ({
+    da = ({
         values: n
     }, t, e) => {
         n[t] = e[0] * 12 + e[1] % 12
     },
     Xc = (n, t, e) => {
         const {
             stride: i
         } = n, r = n.children[0], s = Vt.getVisitFn(r);
         if (Array.isArray(e))
             for (let o = -1, a = t * i; ++o < i;) s(r, a + o, e[o]);
         else
             for (let o = -1, a = t * i; ++o < i;) s(r, a + o, e.get(o))
     };
-A.prototype.visitBool = N(Lc);
-A.prototype.visitInt = N(ve);
-A.prototype.visitInt8 = N(ve);
-A.prototype.visitInt16 = N(ve);
-A.prototype.visitInt32 = N(ve);
-A.prototype.visitInt64 = N(ve);
-A.prototype.visitUint8 = N(ve);
-A.prototype.visitUint16 = N(ve);
-A.prototype.visitUint32 = N(ve);
-A.prototype.visitUint64 = N(ve);
-A.prototype.visitFloat = N(Ec);
-A.prototype.visitFloat16 = N(Ko);
-A.prototype.visitFloat32 = N(Kr);
-A.prototype.visitFloat64 = N(Kr);
-A.prototype.visitUtf8 = N(kc);
-A.prototype.visitBinary = N(Cc);
-A.prototype.visitFixedSizeBinary = N(Rc);
-A.prototype.visitDate = N(Uc);
-A.prototype.visitDateDay = N(Zo);
-A.prototype.visitDateMillisecond = N(Xo);
-A.prototype.visitTimestamp = N(Vc);
-A.prototype.visitTimestampSecond = N(Qo);
-A.prototype.visitTimestampMillisecond = N(ta);
-A.prototype.visitTimestampMicrosecond = N(ea);
-A.prototype.visitTimestampNanosecond = N(na);
-A.prototype.visitTime = N($c);
-A.prototype.visitTimeSecond = N(ia);
-A.prototype.visitTimeMillisecond = N(ra);
-A.prototype.visitTimeMicrosecond = N(sa);
-A.prototype.visitTimeNanosecond = N(oa);
-A.prototype.visitDecimal = N(Pc);
-A.prototype.visitList = N(jc);
-A.prototype.visitStruct = N(qc);
-A.prototype.visitUnion = N(Jc);
-A.prototype.visitDenseUnion = N(aa);
-A.prototype.visitSparseUnion = N(la);
-A.prototype.visitDictionary = N(Kc);
-A.prototype.visitInterval = N(Zc);
-A.prototype.visitIntervalDayTime = N(ca);
-A.prototype.visitIntervalYearMonth = N(ua);
-A.prototype.visitFixedSizeList = N(Xc);
-A.prototype.visitMap = N(zc);
-const Vt = new A,
-    $t = Symbol.for("parent"),
-    on = Symbol.for("rowIndex");
-class Zr {
+D.prototype.visitBool = x(Lc);
+D.prototype.visitInt = x(_e);
+D.prototype.visitInt8 = x(_e);
+D.prototype.visitInt16 = x(_e);
+D.prototype.visitInt32 = x(_e);
+D.prototype.visitInt64 = x(_e);
+D.prototype.visitUint8 = x(_e);
+D.prototype.visitUint16 = x(_e);
+D.prototype.visitUint32 = x(_e);
+D.prototype.visitUint64 = x(_e);
+D.prototype.visitFloat = x(Ec);
+D.prototype.visitFloat16 = x(Zo);
+D.prototype.visitFloat32 = x(Qr);
+D.prototype.visitFloat64 = x(Qr);
+D.prototype.visitUtf8 = x(kc);
+D.prototype.visitBinary = x(Cc);
+D.prototype.visitFixedSizeBinary = x(Rc);
+D.prototype.visitDate = x(Uc);
+D.prototype.visitDateDay = x(Xo);
+D.prototype.visitDateMillisecond = x(Qo);
+D.prototype.visitTimestamp = x($c);
+D.prototype.visitTimestampSecond = x(ta);
+D.prototype.visitTimestampMillisecond = x(ea);
+D.prototype.visitTimestampMicrosecond = x(na);
+D.prototype.visitTimestampNanosecond = x(ia);
+D.prototype.visitTime = x(Vc);
+D.prototype.visitTimeSecond = x(ra);
+D.prototype.visitTimeMillisecond = x(sa);
+D.prototype.visitTimeMicrosecond = x(oa);
+D.prototype.visitTimeNanosecond = x(aa);
+D.prototype.visitDecimal = x(Pc);
+D.prototype.visitList = x(jc);
+D.prototype.visitStruct = x(qc);
+D.prototype.visitUnion = x(Jc);
+D.prototype.visitDenseUnion = x(la);
+D.prototype.visitSparseUnion = x(ca);
+D.prototype.visitDictionary = x(Kc);
+D.prototype.visitInterval = x(Zc);
+D.prototype.visitIntervalDayTime = x(ua);
+D.prototype.visitIntervalYearMonth = x(da);
+D.prototype.visitFixedSizeList = x(Xc);
+D.prototype.visitMap = x(zc);
+const Vt = new D,
+    Pt = Symbol.for("parent"),
+    ln = Symbol.for("rowIndex");
+class ts {
     constructor(t, e) {
-        return this[$t] = t, this[on] = e, new Proxy(this, new tu)
+        return this[Pt] = t, this[ln] = e, new Proxy(this, new tu)
     }
     toArray() {
         return Object.values(this.toJSON())
     }
     toJSON() {
-        const t = this[on],
-            e = this[$t],
+        const t = this[ln],
+            e = this[Pt],
             i = e.type.children,
             r = {};
         for (let s = -1, o = i.length; ++s < o;) r[i[s].name] = Ft.visit(e.children[s], t);
         return r
     }
     toString() {
-        return `{${[...this].map(([t,e])=>`${En(t)}: ${En(e)}`).join(", ")}}`
+        return `{${[...this].map(([t,e])=>`${Rn(t)}: ${Rn(e)}`).join(", ")}}`
     } [Symbol.for("nodejs.util.inspect.custom")]() {
         return this.toString()
     } [Symbol.iterator]() {
-        return new Qc(this[$t], this[on])
+        return new Qc(this[Pt], this[ln])
     }
 }
 class Qc {
     constructor(t, e) {
         this.childIndex = 0, this.children = t.children, this.rowIndex = e, this.childFields = t.type.children, this.numChildren = this.childFields.length
     } [Symbol.iterator]() {
         return this
@@ -2337,27 +2337,27 @@
             value: [this.childFields[t].name, Ft.visit(this.children[t], this.rowIndex)]
         }) : {
             done: !0,
             value: null
         }
     }
 }
-Object.defineProperties(Zr.prototype, {
+Object.defineProperties(ts.prototype, {
     [Symbol.toStringTag]: {
         enumerable: !1,
         configurable: !1,
         value: "Row"
     },
-    [$t]: {
+    [Pt]: {
         writable: !0,
         enumerable: !1,
         configurable: !1,
         value: null
     },
-    [on]: {
+    [ln]: {
         writable: !0,
         enumerable: !1,
         configurable: !1,
         value: -1
     }
 });
 class tu {
@@ -2367,279 +2367,279 @@
     deleteProperty() {
         return !1
     }
     preventExtensions() {
         return !0
     }
     ownKeys(t) {
-        return t[$t].type.children.map(e => e.name)
+        return t[Pt].type.children.map(e => e.name)
     }
     has(t, e) {
-        return t[$t].type.children.findIndex(i => i.name === e) !== -1
+        return t[Pt].type.children.findIndex(i => i.name === e) !== -1
     }
     getOwnPropertyDescriptor(t, e) {
-        if (t[$t].type.children.findIndex(i => i.name === e) !== -1) return {
+        if (t[Pt].type.children.findIndex(i => i.name === e) !== -1) return {
             writable: !0,
             enumerable: !0,
             configurable: !0
         }
     }
     get(t, e) {
         if (Reflect.has(t, e)) return t[e];
-        const i = t[$t].type.children.findIndex(r => r.name === e);
+        const i = t[Pt].type.children.findIndex(r => r.name === e);
         if (i !== -1) {
-            const r = Ft.visit(t[$t].children[i], t[on]);
+            const r = Ft.visit(t[Pt].children[i], t[ln]);
             return Reflect.set(t, e, r), r
         }
     }
     set(t, e, i) {
-        const r = t[$t].type.children.findIndex(s => s.name === e);
-        return r !== -1 ? (Vt.visit(t[$t].children[r], t[on], i), Reflect.set(t, e, i)) : Reflect.has(t, e) || typeof e == "symbol" ? Reflect.set(t, e, i) : !1
+        const r = t[Pt].type.children.findIndex(s => s.name === e);
+        return r !== -1 ? (Vt.visit(t[Pt].children[r], t[ln], i), Reflect.set(t, e, i)) : Reflect.has(t, e) || typeof e == "symbol" ? Reflect.set(t, e, i) : !1
     }
 }
-class I extends R {}
+class B extends R {}
 
-function D(n) {
+function T(n) {
     return (t, e) => t.getValid(e) ? n(t, e) : null
 }
 const eu = (n, t) => 864e5 * n[t],
-    Xr = (n, t) => 4294967296 * n[t + 1] + (n[t] >>> 0),
+    es = (n, t) => 4294967296 * n[t + 1] + (n[t] >>> 0),
     nu = (n, t) => 4294967296 * (n[t + 1] / 1e3) + (n[t] >>> 0) / 1e3,
     iu = (n, t) => 4294967296 * (n[t + 1] / 1e6) + (n[t] >>> 0) / 1e6,
-    da = n => new Date(n),
-    ru = (n, t) => da(eu(n, t)),
-    su = (n, t) => da(Xr(n, t)),
+    ha = n => new Date(n),
+    ru = (n, t) => ha(eu(n, t)),
+    su = (n, t) => ha(es(n, t)),
     ou = (n, t) => null,
-    ha = (n, t, e) => {
+    fa = (n, t, e) => {
         if (e + 1 >= t.length) return null;
         const i = t[e],
             r = t[e + 1];
         return n.subarray(i, r)
     },
     au = ({
         offset: n,
         values: t
     }, e) => {
         const i = n + e;
         return (t[i >> 3] & 1 << i % 8) !== 0
     },
-    fa = ({
+    pa = ({
         values: n
     }, t) => ru(n, t),
-    pa = ({
+    ya = ({
         values: n
     }, t) => su(n, t * 2),
-    Te = ({
+    Le = ({
         stride: n,
         values: t
     }, e) => t[n * e],
     lu = ({
         stride: n,
         values: t
-    }, e) => qo(t[n * e]),
-    ya = ({
+    }, e) => Jo(t[n * e]),
+    ma = ({
         values: n
     }, t) => n[t],
     cu = ({
         stride: n,
         values: t
     }, e) => t.subarray(n * e, n * (e + 1)),
     uu = ({
         values: n,
         valueOffsets: t
-    }, e) => ha(n, t, e),
+    }, e) => fa(n, t, e),
     du = ({
         values: n,
         valueOffsets: t
     }, e) => {
-        const i = ha(n, t, e);
-        return i !== null ? gr(i) : null
+        const i = fa(n, t, e);
+        return i !== null ? Sr(i) : null
     },
     hu = ({
         values: n
     }, t) => n[t],
     fu = ({
         type: n,
         values: t
-    }, e) => n.precision !== Bt.HALF ? t[e] : qo(t[e]),
-    pu = (n, t) => n.type.unit === ye.DAY ? fa(n, t) : pa(n, t),
-    ma = ({
-        values: n
-    }, t) => 1e3 * Xr(n, t * 2),
+    }, e) => n.precision !== Bt.HALF ? t[e] : Jo(t[e]),
+    pu = (n, t) => n.type.unit === be.DAY ? pa(n, t) : ya(n, t),
     va = ({
         values: n
-    }, t) => Xr(n, t * 2),
+    }, t) => 1e3 * es(n, t * 2),
     ba = ({
         values: n
-    }, t) => nu(n, t * 2),
+    }, t) => es(n, t * 2),
     ga = ({
         values: n
+    }, t) => nu(n, t * 2),
+    _a = ({
+        values: n
     }, t) => iu(n, t * 2),
     yu = (n, t) => {
         switch (n.type.unit) {
-            case V.SECOND:
-                return ma(n, t);
-            case V.MILLISECOND:
+            case $.SECOND:
                 return va(n, t);
-            case V.MICROSECOND:
+            case $.MILLISECOND:
                 return ba(n, t);
-            case V.NANOSECOND:
-                return ga(n, t)
+            case $.MICROSECOND:
+                return ga(n, t);
+            case $.NANOSECOND:
+                return _a(n, t)
         }
     },
-    _a = ({
-        values: n
-    }, t) => n[t],
     wa = ({
         values: n
     }, t) => n[t],
     Sa = ({
         values: n
     }, t) => n[t],
     Ia = ({
         values: n
     }, t) => n[t],
+    Ba = ({
+        values: n
+    }, t) => n[t],
     mu = (n, t) => {
         switch (n.type.unit) {
-            case V.SECOND:
-                return _a(n, t);
-            case V.MILLISECOND:
+            case $.SECOND:
                 return wa(n, t);
-            case V.MICROSECOND:
+            case $.MILLISECOND:
                 return Sa(n, t);
-            case V.NANOSECOND:
-                return Ia(n, t)
+            case $.MICROSECOND:
+                return Ia(n, t);
+            case $.NANOSECOND:
+                return Ba(n, t)
         }
     },
     vu = ({
         values: n,
         stride: t
-    }, e) => qr.decimal(n.subarray(t * e, t * (e + 1))),
+    }, e) => Zr.decimal(n.subarray(t * e, t * (e + 1))),
     bu = (n, t) => {
         const {
             valueOffsets: e,
             stride: i,
             children: r
         } = n, {
             [t * i]: s,
             [t * i + 1]: o
         } = e, l = r[0].slice(s, o - s);
-        return new P([l])
+        return new z([l])
     },
     gu = (n, t) => {
         const {
             valueOffsets: e,
             children: i
         } = n, {
             [t]: r,
             [t + 1]: s
         } = e, o = i[0];
-        return new Qr(o.slice(r, s - r))
+        return new ns(o.slice(r, s - r))
     },
-    _u = (n, t) => new Zr(n, t),
-    wu = (n, t) => n.type.mode === xt.Dense ? Ba(n, t) : Oa(n, t),
-    Ba = (n, t) => {
+    _u = (n, t) => new ts(n, t),
+    wu = (n, t) => n.type.mode === Mt.Dense ? Oa(n, t) : Fa(n, t),
+    Oa = (n, t) => {
         const e = n.type.typeIdToChildIndex[n.typeIds[t]],
             i = n.children[e];
         return Ft.visit(i, n.valueOffsets[t])
     },
-    Oa = (n, t) => {
+    Fa = (n, t) => {
         const e = n.type.typeIdToChildIndex[n.typeIds[t]],
             i = n.children[e];
         return Ft.visit(i, t)
     },
     Su = (n, t) => {
         var e;
         return (e = n.dictionary) === null || e === void 0 ? void 0 : e.get(n.values[t])
     },
-    Iu = (n, t) => n.type.unit === Be.DAY_TIME ? Fa(n, t) : Aa(n, t),
-    Fa = ({
+    Iu = (n, t) => n.type.unit === De.DAY_TIME ? Aa(n, t) : Da(n, t),
+    Aa = ({
         values: n
     }, t) => n.subarray(2 * t, 2 * (t + 1)),
-    Aa = ({
+    Da = ({
         values: n
     }, t) => {
         const e = n[t],
             i = new Int32Array(2);
         return i[0] = Math.trunc(e / 12), i[1] = Math.trunc(e % 12), i
     },
     Bu = (n, t) => {
         const {
             stride: e,
             children: i
         } = n, s = i[0].slice(t * e, e);
-        return new P([s])
+        return new z([s])
     };
-I.prototype.visitNull = D(ou);
-I.prototype.visitBool = D(au);
-I.prototype.visitInt = D(hu);
-I.prototype.visitInt8 = D(Te);
-I.prototype.visitInt16 = D(Te);
-I.prototype.visitInt32 = D(Te);
-I.prototype.visitInt64 = D(ya);
-I.prototype.visitUint8 = D(Te);
-I.prototype.visitUint16 = D(Te);
-I.prototype.visitUint32 = D(Te);
-I.prototype.visitUint64 = D(ya);
-I.prototype.visitFloat = D(fu);
-I.prototype.visitFloat16 = D(lu);
-I.prototype.visitFloat32 = D(Te);
-I.prototype.visitFloat64 = D(Te);
-I.prototype.visitUtf8 = D(du);
-I.prototype.visitBinary = D(uu);
-I.prototype.visitFixedSizeBinary = D(cu);
-I.prototype.visitDate = D(pu);
-I.prototype.visitDateDay = D(fa);
-I.prototype.visitDateMillisecond = D(pa);
-I.prototype.visitTimestamp = D(yu);
-I.prototype.visitTimestampSecond = D(ma);
-I.prototype.visitTimestampMillisecond = D(va);
-I.prototype.visitTimestampMicrosecond = D(ba);
-I.prototype.visitTimestampNanosecond = D(ga);
-I.prototype.visitTime = D(mu);
-I.prototype.visitTimeSecond = D(_a);
-I.prototype.visitTimeMillisecond = D(wa);
-I.prototype.visitTimeMicrosecond = D(Sa);
-I.prototype.visitTimeNanosecond = D(Ia);
-I.prototype.visitDecimal = D(vu);
-I.prototype.visitList = D(bu);
-I.prototype.visitStruct = D(_u);
-I.prototype.visitUnion = D(wu);
-I.prototype.visitDenseUnion = D(Ba);
-I.prototype.visitSparseUnion = D(Oa);
-I.prototype.visitDictionary = D(Su);
-I.prototype.visitInterval = D(Iu);
-I.prototype.visitIntervalDayTime = D(Fa);
-I.prototype.visitIntervalYearMonth = D(Aa);
-I.prototype.visitFixedSizeList = D(Bu);
-I.prototype.visitMap = D(gu);
-const Ft = new I,
-    qt = Symbol.for("keys"),
-    an = Symbol.for("vals");
-class Qr {
+B.prototype.visitNull = T(ou);
+B.prototype.visitBool = T(au);
+B.prototype.visitInt = T(hu);
+B.prototype.visitInt8 = T(Le);
+B.prototype.visitInt16 = T(Le);
+B.prototype.visitInt32 = T(Le);
+B.prototype.visitInt64 = T(ma);
+B.prototype.visitUint8 = T(Le);
+B.prototype.visitUint16 = T(Le);
+B.prototype.visitUint32 = T(Le);
+B.prototype.visitUint64 = T(ma);
+B.prototype.visitFloat = T(fu);
+B.prototype.visitFloat16 = T(lu);
+B.prototype.visitFloat32 = T(Le);
+B.prototype.visitFloat64 = T(Le);
+B.prototype.visitUtf8 = T(du);
+B.prototype.visitBinary = T(uu);
+B.prototype.visitFixedSizeBinary = T(cu);
+B.prototype.visitDate = T(pu);
+B.prototype.visitDateDay = T(pa);
+B.prototype.visitDateMillisecond = T(ya);
+B.prototype.visitTimestamp = T(yu);
+B.prototype.visitTimestampSecond = T(va);
+B.prototype.visitTimestampMillisecond = T(ba);
+B.prototype.visitTimestampMicrosecond = T(ga);
+B.prototype.visitTimestampNanosecond = T(_a);
+B.prototype.visitTime = T(mu);
+B.prototype.visitTimeSecond = T(wa);
+B.prototype.visitTimeMillisecond = T(Sa);
+B.prototype.visitTimeMicrosecond = T(Ia);
+B.prototype.visitTimeNanosecond = T(Ba);
+B.prototype.visitDecimal = T(vu);
+B.prototype.visitList = T(bu);
+B.prototype.visitStruct = T(_u);
+B.prototype.visitUnion = T(wu);
+B.prototype.visitDenseUnion = T(Oa);
+B.prototype.visitSparseUnion = T(Fa);
+B.prototype.visitDictionary = T(Su);
+B.prototype.visitInterval = T(Iu);
+B.prototype.visitIntervalDayTime = T(Aa);
+B.prototype.visitIntervalYearMonth = T(Da);
+B.prototype.visitFixedSizeList = T(Bu);
+B.prototype.visitMap = T(gu);
+const Ft = new B,
+    Kt = Symbol.for("keys"),
+    cn = Symbol.for("vals");
+class ns {
     constructor(t) {
-        return this[qt] = new P([t.children[0]]).memoize(), this[an] = t.children[1], new Proxy(this, new Fu)
+        return this[Kt] = new z([t.children[0]]).memoize(), this[cn] = t.children[1], new Proxy(this, new Fu)
     } [Symbol.iterator]() {
-        return new Ou(this[qt], this[an])
+        return new Ou(this[Kt], this[cn])
     }
     get size() {
-        return this[qt].length
+        return this[Kt].length
     }
     toArray() {
         return Object.values(this.toJSON())
     }
     toJSON() {
-        const t = this[qt],
-            e = this[an],
+        const t = this[Kt],
+            e = this[cn],
             i = {};
         for (let r = -1, s = t.length; ++r < s;) i[t.get(r)] = Ft.visit(e, r);
         return i
     }
     toString() {
-        return `{${[...this].map(([t,e])=>`${En(t)}: ${En(e)}`).join(", ")}}`
+        return `{${[...this].map(([t,e])=>`${Rn(t)}: ${Rn(e)}`).join(", ")}}`
     } [Symbol.for("nodejs.util.inspect.custom")]() {
         return this.toString()
     }
 }
 class Ou {
     constructor(t, e) {
         this.keys = t, this.vals = e, this.keyIndex = 0, this.numKeys = t.length
@@ -2664,181 +2664,181 @@
     deleteProperty() {
         return !1
     }
     preventExtensions() {
         return !0
     }
     ownKeys(t) {
-        return t[qt].toArray().map(String)
+        return t[Kt].toArray().map(String)
     }
     has(t, e) {
-        return t[qt].includes(e)
+        return t[Kt].includes(e)
     }
     getOwnPropertyDescriptor(t, e) {
-        if (t[qt].indexOf(e) !== -1) return {
+        if (t[Kt].indexOf(e) !== -1) return {
             writable: !0,
             enumerable: !0,
             configurable: !0
         }
     }
     get(t, e) {
         if (Reflect.has(t, e)) return t[e];
-        const i = t[qt].indexOf(e);
+        const i = t[Kt].indexOf(e);
         if (i !== -1) {
-            const r = Ft.visit(Reflect.get(t, an), i);
+            const r = Ft.visit(Reflect.get(t, cn), i);
             return Reflect.set(t, e, r), r
         }
     }
     set(t, e, i) {
-        const r = t[qt].indexOf(e);
-        return r !== -1 ? (Vt.visit(Reflect.get(t, an), r, i), Reflect.set(t, e, i)) : Reflect.has(t, e) ? Reflect.set(t, e, i) : !1
+        const r = t[Kt].indexOf(e);
+        return r !== -1 ? (Vt.visit(Reflect.get(t, cn), r, i), Reflect.set(t, e, i)) : Reflect.has(t, e) ? Reflect.set(t, e, i) : !1
     }
 }
-Object.defineProperties(Qr.prototype, {
+Object.defineProperties(ns.prototype, {
     [Symbol.toStringTag]: {
         enumerable: !1,
         configurable: !1,
         value: "Row"
     },
-    [qt]: {
+    [Kt]: {
         writable: !0,
         enumerable: !1,
         configurable: !1,
         value: null
     },
-    [an]: {
+    [cn]: {
         writable: !0,
         enumerable: !1,
         configurable: !1,
         value: null
     }
 });
-let Ns;
+let xs;
 
-function Da(n, t, e, i) {
+function Ta(n, t, e, i) {
     const {
         length: r = 0
     } = n;
     let s = typeof t != "number" ? 0 : t,
         o = typeof e != "number" ? r : e;
-    return s < 0 && (s = (s % r + r) % r), o < 0 && (o = (o % r + r) % r), o < s && (Ns = s, s = o, o = Ns), o > r && (o = r), i ? i(n, s, o) : [s, o]
+    return s < 0 && (s = (s % r + r) % r), o < 0 && (o = (o % r + r) % r), o < s && (xs = s, s = o, o = xs), o > r && (o = r), i ? i(n, s, o) : [s, o]
 }
 const Ms = n => n !== n;
 
-function _n(n) {
+function Bn(n) {
     if (typeof n !== "object" || n === null) return Ms(n) ? Ms : e => e === n;
     if (n instanceof Date) {
         const e = n.valueOf();
         return i => i instanceof Date ? i.valueOf() === e : !1
     }
-    return ArrayBuffer.isView(n) ? e => e ? gc(n, e) : !1 : n instanceof Map ? Du(n) : Array.isArray(n) ? Au(n) : n instanceof P ? Tu(n) : Nu(n, !0)
+    return ArrayBuffer.isView(n) ? e => e ? gc(n, e) : !1 : n instanceof Map ? Du(n) : Array.isArray(n) ? Au(n) : n instanceof z ? Tu(n) : Nu(n, !0)
 }
 
 function Au(n) {
     const t = [];
-    for (let e = -1, i = n.length; ++e < i;) t[e] = _n(n[e]);
-    return tr(t)
+    for (let e = -1, i = n.length; ++e < i;) t[e] = Bn(n[e]);
+    return nr(t)
 }
 
 function Du(n) {
     let t = -1;
     const e = [];
-    for (const i of n.values()) e[++t] = _n(i);
-    return tr(e)
+    for (const i of n.values()) e[++t] = Bn(i);
+    return nr(e)
 }
 
 function Tu(n) {
     const t = [];
-    for (let e = -1, i = n.length; ++e < i;) t[e] = _n(n.get(e));
-    return tr(t)
+    for (let e = -1, i = n.length; ++e < i;) t[e] = Bn(n.get(e));
+    return nr(t)
 }
 
 function Nu(n, t = !1) {
     const e = Object.keys(n);
     if (!t && e.length === 0) return () => !1;
     const i = [];
-    for (let r = -1, s = e.length; ++r < s;) i[r] = _n(n[e[r]]);
-    return tr(i, e)
+    for (let r = -1, s = e.length; ++r < s;) i[r] = Bn(n[e[r]]);
+    return nr(i, e)
 }
 
-function tr(n, t) {
+function nr(n, t) {
     return e => {
         if (!e || typeof e != "object") return !1;
         switch (e.constructor) {
             case Array:
-                return Mu(n, e);
+                return xu(n, e);
             case Map:
-                return xs(n, e, e.keys());
-            case Qr:
-            case Zr:
+                return Ls(n, e, e.keys());
+            case ns:
+            case ts:
             case Object:
             case void 0:
-                return xs(n, e, t || Object.keys(e))
+                return Ls(n, e, t || Object.keys(e))
         }
-        return e instanceof P ? xu(n, e) : !1
+        return e instanceof z ? Mu(n, e) : !1
     }
 }
 
-function Mu(n, t) {
+function xu(n, t) {
     const e = n.length;
     if (t.length !== e) return !1;
     for (let i = -1; ++i < e;)
         if (!n[i](t[i])) return !1;
     return !0
 }
 
-function xu(n, t) {
+function Mu(n, t) {
     const e = n.length;
     if (t.length !== e) return !1;
     for (let i = -1; ++i < e;)
         if (!n[i](t.get(i))) return !1;
     return !0
 }
 
-function xs(n, t, e) {
+function Ls(n, t, e) {
     const i = e[Symbol.iterator](),
         r = t instanceof Map ? t.keys() : Object.keys(t)[Symbol.iterator](),
         s = t instanceof Map ? t.values() : Object.values(t)[Symbol.iterator]();
     let o = 0;
     const a = n.length;
     let l = s.next(),
         c = i.next(),
         d = r.next();
     for (; o < a && !c.done && !d.done && !l.done && !(c.value !== d.value || !n[o](l.value)); ++o, c = i.next(), d = r.next(), l = s.next());
     return o === a && c.done && d.done && l.done ? !0 : (i.return && i.return(), r.return && r.return(), s.return && s.return(), !1)
 }
 
-function Ta(n, t, e, i) {
+function Na(n, t, e, i) {
     return (e & 1 << i) !== 0
 }
 
 function Lu(n, t, e, i) {
     return (e & 1 << i) >> i
 }
 
-function ts(n, t, e) {
+function is(n, t, e) {
     const i = e.byteLength + 7 & -8;
     if (n > 0 || e.byteLength < i) {
         const r = new Uint8Array(i);
-        return r.set(n % 8 === 0 ? e.subarray(n >> 3) : Si(new es(e, n, t, null, Ta)).subarray(0, i)), r
+        return r.set(n % 8 === 0 ? e.subarray(n >> 3) : Bi(new rs(e, n, t, null, Na)).subarray(0, i)), r
     }
     return e
 }
 
-function Si(n) {
+function Bi(n) {
     const t = [];
     let e = 0,
         i = 0,
         r = 0;
     for (const o of n) o && (r |= 1 << i), ++i === 8 && (t[e++] = r, r = i = 0);
     (e === 0 || i > 0) && (t[e++] = r);
     const s = new Uint8Array(t.length + 7 & -8);
     return s.set(t), s
 }
-class es {
+class rs {
     constructor(t, e, i, r, s) {
         this.bytes = t, this.length = i, this.context = r, this.get = s, this.bit = e % 8, this.byteIndex = e >> 3, this.byte = t[this.byteIndex++], this.index = 0
     }
     next() {
         return this.index < this.length ? (this.bit === 8 && (this.bit = 0, this.byte = this.bytes[this.byteIndex++]), {
             value: this.get(this.context, this.index++, this.byte, this.bit++)
         }) : {
@@ -2846,47 +2846,47 @@
             value: null
         }
     } [Symbol.iterator]() {
         return this
     }
 }
 
-function Ir(n, t, e) {
+function Fr(n, t, e) {
     if (e - t <= 0) return 0;
     if (e - t < 8) {
         let s = 0;
-        for (const o of new es(n, t, e - t, n, Lu)) s += o;
+        for (const o of new rs(n, t, e - t, n, Lu)) s += o;
         return s
     }
     const i = e >> 3 << 3,
         r = t + (t % 8 === 0 ? 0 : 8 - t % 8);
-    return Ir(n, t, r) + Ir(n, i, e) + Eu(n, r >> 3, i - r >> 3)
+    return Fr(n, t, r) + Fr(n, i, e) + Eu(n, r >> 3, i - r >> 3)
 }
 
 function Eu(n, t, e) {
     let i = 0,
         r = Math.trunc(t);
     const s = new DataView(n.buffer, n.byteOffset, n.byteLength),
         o = e === void 0 ? n.byteLength : r + e;
-    for (; o - r >= 4;) i += ur(s.getUint32(r)), r += 4;
-    for (; o - r >= 2;) i += ur(s.getUint16(r)), r += 2;
-    for (; o - r >= 1;) i += ur(s.getUint8(r)), r += 1;
+    for (; o - r >= 4;) i += hr(s.getUint32(r)), r += 4;
+    for (; o - r >= 2;) i += hr(s.getUint16(r)), r += 2;
+    for (; o - r >= 1;) i += hr(s.getUint8(r)), r += 1;
     return i
 }
 
-function ur(n) {
+function hr(n) {
     let t = Math.trunc(n);
     return t = t - (t >>> 1 & 1431655765), t = (t & 858993459) + (t >>> 2 & 858993459), (t + (t >>> 4) & 252645135) * 16843009 >>> 24
 }
 const Ru = -1;
-class K {
+class X {
     constructor(t, e, i, r, s, o = [], a) {
         this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(i || 0, 0)), this._nullCount = Math.floor(Math.max(r || 0, -1));
         let l;
-        s instanceof K ? (this.stride = s.stride, this.values = s.values, this.typeIds = s.typeIds, this.nullBitmap = s.nullBitmap, this.valueOffsets = s.valueOffsets) : (this.stride = le(t), s && ((l = s[0]) && (this.valueOffsets = l), (l = s[1]) && (this.values = l), (l = s[2]) && (this.nullBitmap = l), (l = s[3]) && (this.typeIds = l))), this.nullable = this._nullCount !== 0 && this.nullBitmap && this.nullBitmap.byteLength > 0
+        s instanceof X ? (this.stride = s.stride, this.values = s.values, this.typeIds = s.typeIds, this.nullBitmap = s.nullBitmap, this.valueOffsets = s.valueOffsets) : (this.stride = he(t), s && ((l = s[0]) && (this.valueOffsets = l), (l = s[1]) && (this.values = l), (l = s[2]) && (this.nullBitmap = l), (l = s[3]) && (this.typeIds = l))), this.nullable = this._nullCount !== 0 && this.nullBitmap && this.nullBitmap.byteLength > 0
     }
     get typeId() {
         return this.type.typeId
     }
     get ArrayType() {
         return this.type.ArrayType
     }
@@ -2902,15 +2902,15 @@
             typeIds: s
         } = this;
         return e && (t += e.byteLength), i && (t += i.byteLength), r && (t += r.byteLength), s && (t += s.byteLength), this.children.reduce((o, a) => o + a.byteLength, t)
     }
     get nullCount() {
         let t = this._nullCount,
             e;
-        return t <= Ru && (e = this.nullBitmap) && (this._nullCount = t = this.length - Ir(e, this.offset, this.offset + this.length)), t
+        return t <= Ru && (e = this.nullBitmap) && (this._nullCount = t = this.length - Fr(e, this.offset, this.offset + this.length)), t
     }
     getValid(t) {
         if (this.nullable && this.nullCount > 0) {
             const e = this.offset + t;
             return (this.nullBitmap[e >> 3] & 1 << e % 8) !== 0
         }
         return !0
@@ -2929,15 +2929,15 @@
         const {
             nullBitmap: i,
             offset: r
         } = this, s = r + t >> 3, o = (r + t) % 8, a = i[s] >> o & 1;
         return e ? a === 0 && (i[s] |= 1 << o, this._nullCount = this.nullCount + 1) : a === 1 && (i[s] &= ~(1 << o), this._nullCount = this.nullCount - 1), e
     }
     clone(t = this.type, e = this.offset, i = this.length, r = this._nullCount, s = this, o = this.children) {
-        return new K(t, e, i, r, s, o, this.dictionary)
+        return new X(t, e, i, r, s, o, this.dictionary)
     }
     slice(t, e) {
         const {
             stride: i,
             typeId: r,
             children: s
         } = this, o = +(this._nullCount === 0) - 1, a = r === 16 ? i : 1, l = this._sliceBuffers(t, e, i, r);
@@ -2945,211 +2945,211 @@
     }
     _changeLengthAndBackfillNullBitmap(t) {
         if (this.typeId === u.Null) return this.clone(this.type, 0, t, 0);
         const {
             length: e,
             nullCount: i
         } = this, r = new Uint8Array((t + 63 & -64) >> 3).fill(255, 0, e >> 3);
-        r[e >> 3] = (1 << e - (e & -8)) - 1, i > 0 && r.set(ts(this.offset, e, this.nullBitmap), 0);
+        r[e >> 3] = (1 << e - (e & -8)) - 1, i > 0 && r.set(is(this.offset, e, this.nullBitmap), 0);
         const s = this.buffers;
-        return s[ae.VALIDITY] = r, this.clone(this.type, 0, t, i + (t - e), s)
+        return s[de.VALIDITY] = r, this.clone(this.type, 0, t, i + (t - e), s)
     }
     _sliceBuffers(t, e, i, r) {
         let s;
         const {
             buffers: o
         } = this;
-        return (s = o[ae.TYPE]) && (o[ae.TYPE] = s.subarray(t, t + e)), (s = o[ae.OFFSET]) && (o[ae.OFFSET] = s.subarray(t, t + e + 1)) || (s = o[ae.DATA]) && (o[ae.DATA] = r === 6 ? s : s.subarray(i * t, i * (t + e))), o
+        return (s = o[de.TYPE]) && (o[de.TYPE] = s.subarray(t, t + e)), (s = o[de.OFFSET]) && (o[de.OFFSET] = s.subarray(t, t + e + 1)) || (s = o[de.DATA]) && (o[de.DATA] = r === 6 ? s : s.subarray(i * t, i * (t + e))), o
     }
     _sliceChildren(t, e, i) {
         return t.map(r => r.slice(e, i))
     }
 }
-K.prototype.children = Object.freeze([]);
-class Dn extends R {
+X.prototype.children = Object.freeze([]);
+class xn extends R {
     visit(t) {
         return this.getVisitFn(t.type).call(this, t)
     }
     visitNull(t) {
         const {
             ["type"]: e, ["offset"]: i = 0, ["length"]: r = 0
         } = t;
-        return new K(e, i, r, 0)
+        return new X(e, i, r, 0)
     }
     visitBool(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
             ["length"]: o = s.length >> 3,
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitInt(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
             ["length"]: o = s.length,
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitFloat(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
             ["length"]: o = s.length,
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitUtf8(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.data), s = U(t.nullBitmap), o = Bn(t.valueOffsets), {
+        } = t, r = U(t.data), s = U(t.nullBitmap), o = An(t.valueOffsets), {
             ["length"]: a = o.length - 1,
             ["nullCount"]: l = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, a, l, [o, r, s])
+        return new X(e, i, a, l, [o, r, s])
     }
     visitBinary(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.data), s = U(t.nullBitmap), o = Bn(t.valueOffsets), {
+        } = t, r = U(t.data), s = U(t.nullBitmap), o = An(t.valueOffsets), {
             ["length"]: a = o.length - 1,
             ["nullCount"]: l = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, a, l, [o, r, s])
+        return new X(e, i, a, l, [o, r, s])
     }
     visitFixedSizeBinary(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
-            ["length"]: o = s.length / le(e),
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
+            ["length"]: o = s.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitDate(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
-            ["length"]: o = s.length / le(e),
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
+            ["length"]: o = s.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitTimestamp(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
-            ["length"]: o = s.length / le(e),
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
+            ["length"]: o = s.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitTime(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
-            ["length"]: o = s.length / le(e),
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
+            ["length"]: o = s.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitDecimal(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
-            ["length"]: o = s.length / le(e),
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
+            ["length"]: o = s.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitList(t) {
         const {
             ["type"]: e, ["offset"]: i = 0, ["child"]: r
-        } = t, s = U(t.nullBitmap), o = Bn(t.valueOffsets), {
+        } = t, s = U(t.nullBitmap), o = An(t.valueOffsets), {
             ["length"]: a = o.length - 1,
             ["nullCount"]: l = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, a, l, [o, void 0, s], [r])
+        return new X(e, i, a, l, [o, void 0, s], [r])
     }
     visitStruct(t) {
         const {
             ["type"]: e, ["offset"]: i = 0, ["children"]: r = []
         } = t, s = U(t.nullBitmap), {
             length: o = r.reduce((l, {
                 length: c
             }) => Math.max(l, c), 0),
             nullCount: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, void 0, s], r)
+        return new X(e, i, o, a, [void 0, void 0, s], r)
     }
     visitUnion(t) {
         const {
             ["type"]: e, ["offset"]: i = 0, ["children"]: r = []
-        } = t, s = U(t.nullBitmap), o = q(e.ArrayType, t.typeIds), {
+        } = t, s = U(t.nullBitmap), o = K(e.ArrayType, t.typeIds), {
             ["length"]: a = o.length,
             ["nullCount"]: l = t.nullBitmap ? -1 : 0
         } = t;
-        if (S.isSparseUnion(e)) return new K(e, i, a, l, [void 0, void 0, s, o], r);
-        const c = Bn(t.valueOffsets);
-        return new K(e, i, a, l, [c, void 0, s, o], r)
+        if (I.isSparseUnion(e)) return new X(e, i, a, l, [void 0, void 0, s, o], r);
+        const c = An(t.valueOffsets);
+        return new X(e, i, a, l, [c, void 0, s, o], r)
     }
     visitDictionary(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.indices.ArrayType, t.data), {
-            ["dictionary"]: o = new P([new Dn().visit({
+        } = t, r = U(t.nullBitmap), s = K(e.indices.ArrayType, t.data), {
+            ["dictionary"]: o = new z([new xn().visit({
                 type: e.dictionary
             })])
         } = t, {
             ["length"]: a = s.length,
             ["nullCount"]: l = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, a, l, [void 0, s, r], [], o)
+        return new X(e, i, a, l, [void 0, s, r], [], o)
     }
     visitInterval(t) {
         const {
             ["type"]: e, ["offset"]: i = 0
-        } = t, r = U(t.nullBitmap), s = q(e.ArrayType, t.data), {
-            ["length"]: o = s.length / le(e),
+        } = t, r = U(t.nullBitmap), s = K(e.ArrayType, t.data), {
+            ["length"]: o = s.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, s, r])
+        return new X(e, i, o, a, [void 0, s, r])
     }
     visitFixedSizeList(t) {
         const {
-            ["type"]: e, ["offset"]: i = 0, ["child"]: r = new Dn().visit({
+            ["type"]: e, ["offset"]: i = 0, ["child"]: r = new xn().visit({
                 type: e.valueType
             })
         } = t, s = U(t.nullBitmap), {
-            ["length"]: o = r.length / le(e),
+            ["length"]: o = r.length / he(e),
             ["nullCount"]: a = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, o, a, [void 0, void 0, s], [r])
+        return new X(e, i, o, a, [void 0, void 0, s], [r])
     }
     visitMap(t) {
         const {
-            ["type"]: e, ["offset"]: i = 0, ["child"]: r = new Dn().visit({
+            ["type"]: e, ["offset"]: i = 0, ["child"]: r = new xn().visit({
                 type: e.childType
             })
-        } = t, s = U(t.nullBitmap), o = Bn(t.valueOffsets), {
+        } = t, s = U(t.nullBitmap), o = An(t.valueOffsets), {
             ["length"]: a = o.length - 1,
             ["nullCount"]: l = t.nullBitmap ? -1 : 0
         } = t;
-        return new K(e, i, a, l, [o, void 0, s], [r])
+        return new X(e, i, a, l, [o, void 0, s], [r])
     }
 }
 
 function E(n) {
-    return new Dn().visit(n)
+    return new xn().visit(n)
 }
-class Ls {
+class Es {
     constructor(t = 0, e) {
         this.numChunks = t, this.getChunkIterator = e, this.chunkIndex = 0, this.chunkIterator = this.getChunkIterator(0)
     }
     next() {
         for (; this.chunkIndex < this.numChunks;) {
             const t = this.chunkIterator.next();
             if (!t.done) return t;
@@ -3160,23 +3160,23 @@
             value: null
         }
     } [Symbol.iterator]() {
         return this
     }
 }
 
-function Na(n) {
+function xa(n) {
     return n.reduce((t, e) => t + e.nullCount, 0)
 }
 
 function Ma(n) {
     return n.reduce((t, e, i) => (t[i + 1] = t[i] + e.length, t), new Uint32Array(n.length + 1))
 }
 
-function xa(n, t, e, i) {
+function La(n, t, e, i) {
     const r = [];
     for (let s = -1, o = n.length; ++s < o;) {
         const a = n[s],
             l = t[s],
             {
                 length: c
             } = a;
@@ -3189,53 +3189,53 @@
         const d = Math.max(0, e - l),
             h = Math.min(i - l, c);
         r.push(a.slice(d, h - d))
     }
     return r.length === 0 && r.push(n[0].slice(0, 0)), r
 }
 
-function ns(n, t, e, i) {
+function ss(n, t, e, i) {
     let r = 0,
         s = 0,
         o = t.length - 1;
     do {
         if (r >= o - 1) return e < t[o] ? i(n, r, e - t[r]) : null;
         s = r + Math.trunc((o - r) * .5), e < t[s] ? o = s : r = s
     } while (r < o)
 }
 
-function is(n, t) {
+function os(n, t) {
     return n.getValid(t)
 }
 
-function ln(n) {
+function un(n) {
     function t(e, i, r) {
         return n(e[i], r)
     }
     return function(e) {
         const i = this.data;
-        return ns(i, this._offsets, e, t)
+        return ss(i, this._offsets, e, t)
     }
 }
 
-function La(n) {
+function Ea(n) {
     let t;
 
     function e(i, r, s) {
         return n(i[r], s, t)
     }
     return function(i, r) {
         const s = this.data;
         t = r;
-        const o = ns(s, this._offsets, i, e);
+        const o = ss(s, this._offsets, i, e);
         return t = void 0, o
     }
 }
 
-function Ea(n) {
+function Ra(n) {
     let t;
 
     function e(i, r, s) {
         let o = s,
             a = 0,
             l = 0;
         for (let c = r - 1, d = i.length; ++c < d;) {
@@ -3244,110 +3244,110 @@
             o = 0, l += h.length
         }
         return -1
     }
     return function(i, r) {
         t = i;
         const s = this.data,
-            o = typeof r != "number" ? e(s, 0, 0) : ns(s, this._offsets, r, e);
+            o = typeof r != "number" ? e(s, 0, 0) : ss(s, this._offsets, r, e);
         return t = void 0, o
     }
 }
-class B extends R {}
+class O extends R {}
 
 function Cu(n, t) {
     return t === null && n.length > 0 ? 0 : -1
 }
 
 function ku(n, t) {
     const {
         nullBitmap: e
     } = n;
     if (!e || n.nullCount <= 0) return -1;
     let i = 0;
-    for (const r of new es(e, n.offset + (t || 0), n.length, e, Ta)) {
+    for (const r of new rs(e, n.offset + (t || 0), n.length, e, Na)) {
         if (!r) return i;
         ++i
     }
     return -1
 }
 
-function x(n, t, e) {
+function L(n, t, e) {
     if (t === void 0) return -1;
     if (t === null) return ku(n, e);
     const i = Ft.getVisitFn(n),
-        r = _n(t);
+        r = Bn(t);
     for (let s = (e || 0) - 1, o = n.length; ++s < o;)
         if (r(i(n, s))) return s;
     return -1
 }
 
-function Ra(n, t, e) {
+function Ca(n, t, e) {
     const i = Ft.getVisitFn(n),
-        r = _n(t);
+        r = Bn(t);
     for (let s = (e || 0) - 1, o = n.length; ++s < o;)
         if (r(i(n, s))) return s;
     return -1
 }
-B.prototype.visitNull = Cu;
-B.prototype.visitBool = x;
-B.prototype.visitInt = x;
-B.prototype.visitInt8 = x;
-B.prototype.visitInt16 = x;
-B.prototype.visitInt32 = x;
-B.prototype.visitInt64 = x;
-B.prototype.visitUint8 = x;
-B.prototype.visitUint16 = x;
-B.prototype.visitUint32 = x;
-B.prototype.visitUint64 = x;
-B.prototype.visitFloat = x;
-B.prototype.visitFloat16 = x;
-B.prototype.visitFloat32 = x;
-B.prototype.visitFloat64 = x;
-B.prototype.visitUtf8 = x;
-B.prototype.visitBinary = x;
-B.prototype.visitFixedSizeBinary = x;
-B.prototype.visitDate = x;
-B.prototype.visitDateDay = x;
-B.prototype.visitDateMillisecond = x;
-B.prototype.visitTimestamp = x;
-B.prototype.visitTimestampSecond = x;
-B.prototype.visitTimestampMillisecond = x;
-B.prototype.visitTimestampMicrosecond = x;
-B.prototype.visitTimestampNanosecond = x;
-B.prototype.visitTime = x;
-B.prototype.visitTimeSecond = x;
-B.prototype.visitTimeMillisecond = x;
-B.prototype.visitTimeMicrosecond = x;
-B.prototype.visitTimeNanosecond = x;
-B.prototype.visitDecimal = x;
-B.prototype.visitList = x;
-B.prototype.visitStruct = x;
-B.prototype.visitUnion = x;
-B.prototype.visitDenseUnion = Ra;
-B.prototype.visitSparseUnion = Ra;
-B.prototype.visitDictionary = x;
-B.prototype.visitInterval = x;
-B.prototype.visitIntervalDayTime = x;
-B.prototype.visitIntervalYearMonth = x;
-B.prototype.visitFixedSizeList = x;
-B.prototype.visitMap = x;
-const Ii = new B;
-class O extends R {}
+O.prototype.visitNull = Cu;
+O.prototype.visitBool = L;
+O.prototype.visitInt = L;
+O.prototype.visitInt8 = L;
+O.prototype.visitInt16 = L;
+O.prototype.visitInt32 = L;
+O.prototype.visitInt64 = L;
+O.prototype.visitUint8 = L;
+O.prototype.visitUint16 = L;
+O.prototype.visitUint32 = L;
+O.prototype.visitUint64 = L;
+O.prototype.visitFloat = L;
+O.prototype.visitFloat16 = L;
+O.prototype.visitFloat32 = L;
+O.prototype.visitFloat64 = L;
+O.prototype.visitUtf8 = L;
+O.prototype.visitBinary = L;
+O.prototype.visitFixedSizeBinary = L;
+O.prototype.visitDate = L;
+O.prototype.visitDateDay = L;
+O.prototype.visitDateMillisecond = L;
+O.prototype.visitTimestamp = L;
+O.prototype.visitTimestampSecond = L;
+O.prototype.visitTimestampMillisecond = L;
+O.prototype.visitTimestampMicrosecond = L;
+O.prototype.visitTimestampNanosecond = L;
+O.prototype.visitTime = L;
+O.prototype.visitTimeSecond = L;
+O.prototype.visitTimeMillisecond = L;
+O.prototype.visitTimeMicrosecond = L;
+O.prototype.visitTimeNanosecond = L;
+O.prototype.visitDecimal = L;
+O.prototype.visitList = L;
+O.prototype.visitStruct = L;
+O.prototype.visitUnion = L;
+O.prototype.visitDenseUnion = Ca;
+O.prototype.visitSparseUnion = Ca;
+O.prototype.visitDictionary = L;
+O.prototype.visitInterval = L;
+O.prototype.visitIntervalDayTime = L;
+O.prototype.visitIntervalYearMonth = L;
+O.prototype.visitFixedSizeList = L;
+O.prototype.visitMap = L;
+const Oi = new O;
+class F extends R {}
 
-function T(n) {
+function N(n) {
     const {
         type: t
     } = n;
-    if (n.nullCount === 0 && n.stride === 1 && (t.typeId === u.Timestamp || t instanceof Fe && t.bitWidth !== 64 || t instanceof Un && t.bitWidth !== 64 || t instanceof kn && t.precision !== Bt.HALF)) return new Ls(n.data.length, i => {
+    if (n.nullCount === 0 && n.stride === 1 && (t.typeId === u.Timestamp || t instanceof Ne && t.bitWidth !== 64 || t instanceof $n && t.bitWidth !== 64 || t instanceof Un && t.precision !== Bt.HALF)) return new Es(n.data.length, i => {
         const r = n.data[i];
         return r.values.subarray(0, r.length)[Symbol.iterator]()
     });
     let e = 0;
-    return new Ls(n.data.length, i => {
+    return new Es(n.data.length, i => {
         const s = n.data[i].length,
             o = n.slice(e, e + s);
         return e += s, new Uu(o)
     })
 }
 class Uu {
     constructor(t) {
@@ -3360,60 +3360,60 @@
             done: !0,
             value: null
         }
     } [Symbol.iterator]() {
         return this
     }
 }
-O.prototype.visitNull = T;
-O.prototype.visitBool = T;
-O.prototype.visitInt = T;
-O.prototype.visitInt8 = T;
-O.prototype.visitInt16 = T;
-O.prototype.visitInt32 = T;
-O.prototype.visitInt64 = T;
-O.prototype.visitUint8 = T;
-O.prototype.visitUint16 = T;
-O.prototype.visitUint32 = T;
-O.prototype.visitUint64 = T;
-O.prototype.visitFloat = T;
-O.prototype.visitFloat16 = T;
-O.prototype.visitFloat32 = T;
-O.prototype.visitFloat64 = T;
-O.prototype.visitUtf8 = T;
-O.prototype.visitBinary = T;
-O.prototype.visitFixedSizeBinary = T;
-O.prototype.visitDate = T;
-O.prototype.visitDateDay = T;
-O.prototype.visitDateMillisecond = T;
-O.prototype.visitTimestamp = T;
-O.prototype.visitTimestampSecond = T;
-O.prototype.visitTimestampMillisecond = T;
-O.prototype.visitTimestampMicrosecond = T;
-O.prototype.visitTimestampNanosecond = T;
-O.prototype.visitTime = T;
-O.prototype.visitTimeSecond = T;
-O.prototype.visitTimeMillisecond = T;
-O.prototype.visitTimeMicrosecond = T;
-O.prototype.visitTimeNanosecond = T;
-O.prototype.visitDecimal = T;
-O.prototype.visitList = T;
-O.prototype.visitStruct = T;
-O.prototype.visitUnion = T;
-O.prototype.visitDenseUnion = T;
-O.prototype.visitSparseUnion = T;
-O.prototype.visitDictionary = T;
-O.prototype.visitInterval = T;
-O.prototype.visitIntervalDayTime = T;
-O.prototype.visitIntervalYearMonth = T;
-O.prototype.visitFixedSizeList = T;
-O.prototype.visitMap = T;
-const rs = new O,
-    Vu = (n, t) => n + t;
-class Ne extends R {
+F.prototype.visitNull = N;
+F.prototype.visitBool = N;
+F.prototype.visitInt = N;
+F.prototype.visitInt8 = N;
+F.prototype.visitInt16 = N;
+F.prototype.visitInt32 = N;
+F.prototype.visitInt64 = N;
+F.prototype.visitUint8 = N;
+F.prototype.visitUint16 = N;
+F.prototype.visitUint32 = N;
+F.prototype.visitUint64 = N;
+F.prototype.visitFloat = N;
+F.prototype.visitFloat16 = N;
+F.prototype.visitFloat32 = N;
+F.prototype.visitFloat64 = N;
+F.prototype.visitUtf8 = N;
+F.prototype.visitBinary = N;
+F.prototype.visitFixedSizeBinary = N;
+F.prototype.visitDate = N;
+F.prototype.visitDateDay = N;
+F.prototype.visitDateMillisecond = N;
+F.prototype.visitTimestamp = N;
+F.prototype.visitTimestampSecond = N;
+F.prototype.visitTimestampMillisecond = N;
+F.prototype.visitTimestampMicrosecond = N;
+F.prototype.visitTimestampNanosecond = N;
+F.prototype.visitTime = N;
+F.prototype.visitTimeSecond = N;
+F.prototype.visitTimeMillisecond = N;
+F.prototype.visitTimeMicrosecond = N;
+F.prototype.visitTimeNanosecond = N;
+F.prototype.visitDecimal = N;
+F.prototype.visitList = N;
+F.prototype.visitStruct = N;
+F.prototype.visitUnion = N;
+F.prototype.visitDenseUnion = N;
+F.prototype.visitSparseUnion = N;
+F.prototype.visitDictionary = N;
+F.prototype.visitInterval = N;
+F.prototype.visitIntervalDayTime = N;
+F.prototype.visitIntervalYearMonth = N;
+F.prototype.visitFixedSizeList = N;
+F.prototype.visitMap = N;
+const as = new F,
+    $u = (n, t) => n + t;
+class Ee extends R {
     visitNull(t, e) {
         return 0
     }
     visitInt(t, e) {
         return t.type.bitWidth / 8
     }
     visitFloat(t, e) {
@@ -3428,34 +3428,34 @@
     visitDate(t, e) {
         return (t.type.unit + 1) * 4
     }
     visitTime(t, e) {
         return t.type.bitWidth / 8
     }
     visitTimestamp(t, e) {
-        return t.type.unit === V.SECOND ? 4 : 8
+        return t.type.unit === $.SECOND ? 4 : 8
     }
     visitInterval(t, e) {
         return (t.type.unit + 1) * 4
     }
     visitStruct(t, e) {
-        return t.children.reduce((i, r) => i + ie.visit(r, e), 0)
+        return t.children.reduce((i, r) => i + oe.visit(r, e), 0)
     }
     visitFixedSizeBinary(t, e) {
         return t.type.byteWidth
     }
     visitMap(t, e) {
-        return 8 + t.children.reduce((i, r) => i + ie.visit(r, e), 0)
+        return 8 + t.children.reduce((i, r) => i + oe.visit(r, e), 0)
     }
     visitDictionary(t, e) {
         var i;
         return t.type.indices.bitWidth / 8 + (((i = t.dictionary) === null || i === void 0 ? void 0 : i.getByteLength(t.values[e])) || 0)
     }
 }
-const $u = ({
+const Vu = ({
         valueOffsets: n
     }, t) => 8 + (n[t + 1] - n[t]),
     Pu = ({
         valueOffsets: n
     }, t) => 8 + (n[t + 1] - n[t]),
     ju = ({
         valueOffsets: n,
@@ -3465,86 +3465,86 @@
         const r = e[0],
             {
                 [i * t]: s
             } = n,
             {
                 [i * t + 1]: o
             } = n,
-            a = ie.getVisitFn(r.type),
+            a = oe.getVisitFn(r.type),
             l = r.slice(s, o - s);
         let c = 8;
         for (let d = -1, h = o - s; ++d < h;) c += a(l, d);
         return c
     },
     zu = ({
         stride: n,
         children: t
     }, e) => {
         const i = t[0],
             r = i.slice(e * n, n),
-            s = ie.getVisitFn(i.type);
+            s = oe.getVisitFn(i.type);
         let o = 0;
         for (let a = -1, l = r.length; ++a < l;) o += s(r, a);
         return o
     },
-    Wu = (n, t) => n.type.mode === xt.Dense ? Ca(n, t) : ka(n, t),
-    Ca = ({
+    Wu = (n, t) => n.type.mode === Mt.Dense ? ka(n, t) : Ua(n, t),
+    ka = ({
         type: n,
         children: t,
         typeIds: e,
         valueOffsets: i
     }, r) => {
         const s = n.typeIdToChildIndex[e[r]];
-        return 8 + ie.visit(t[s], i[r])
+        return 8 + oe.visit(t[s], i[r])
     },
-    ka = ({
+    Ua = ({
         children: n
-    }, t) => 4 + ie.visitMany(n, n.map(() => t)).reduce(Vu, 0);
-Ne.prototype.visitUtf8 = $u;
-Ne.prototype.visitBinary = Pu;
-Ne.prototype.visitList = ju;
-Ne.prototype.visitFixedSizeList = zu;
-Ne.prototype.visitUnion = Wu;
-Ne.prototype.visitDenseUnion = Ca;
-Ne.prototype.visitSparseUnion = ka;
-const ie = new Ne;
-var Ua;
+    }, t) => 4 + oe.visitMany(n, n.map(() => t)).reduce($u, 0);
+Ee.prototype.visitUtf8 = Vu;
+Ee.prototype.visitBinary = Pu;
+Ee.prototype.visitList = ju;
+Ee.prototype.visitFixedSizeList = zu;
+Ee.prototype.visitUnion = Wu;
+Ee.prototype.visitDenseUnion = ka;
+Ee.prototype.visitSparseUnion = Ua;
+const oe = new Ee;
+var $a;
 const Va = {},
-    $a = {};
-class P {
+    Pa = {};
+class z {
     constructor(t) {
         var e, i, r;
-        const s = t[0] instanceof P ? t.flatMap(a => a.data) : t;
-        if (s.length === 0 || s.some(a => !(a instanceof K))) throw new TypeError("Vector constructor expects an Array of Data instances.");
+        const s = t[0] instanceof z ? t.flatMap(a => a.data) : t;
+        if (s.length === 0 || s.some(a => !(a instanceof X))) throw new TypeError("Vector constructor expects an Array of Data instances.");
         const o = (e = s[0]) === null || e === void 0 ? void 0 : e.type;
         switch (s.length) {
             case 0:
                 this._offsets = [0];
                 break;
             case 1: {
                 const {
                     get: a,
                     set: l,
                     indexOf: c,
                     byteLength: d
                 } = Va[o.typeId], h = s[0];
-                this.isValid = y => is(h, y), this.get = y => a(h, y), this.set = (y, _) => l(h, y, _), this.indexOf = y => c(h, y), this.getByteLength = y => d(h, y), this._offsets = [0, h.length];
+                this.isValid = y => os(h, y), this.get = y => a(h, y), this.set = (y, _) => l(h, y, _), this.indexOf = y => c(h, y), this.getByteLength = y => d(h, y), this._offsets = [0, h.length];
                 break
             }
             default:
-                Object.setPrototypeOf(this, $a[o.typeId]), this._offsets = Ma(s);
+                Object.setPrototypeOf(this, Pa[o.typeId]), this._offsets = Ma(s);
                 break
         }
-        this.data = s, this.type = o, this.stride = le(o), this.numChildren = (r = (i = o.children) === null || i === void 0 ? void 0 : i.length) !== null && r !== void 0 ? r : 0, this.length = this._offsets[this._offsets.length - 1]
+        this.data = s, this.type = o, this.stride = he(o), this.numChildren = (r = (i = o.children) === null || i === void 0 ? void 0 : i.length) !== null && r !== void 0 ? r : 0, this.length = this._offsets[this._offsets.length - 1]
     }
     get byteLength() {
         return this._byteLength === -1 && (this._byteLength = this.data.reduce((t, e) => t + e.byteLength, 0)), this._byteLength
     }
     get nullCount() {
-        return this._nullCount === -1 && (this._nullCount = Na(this.data)), this._nullCount
+        return this._nullCount === -1 && (this._nullCount = xa(this.data)), this._nullCount
     }
     get ArrayType() {
         return this.type.ArrayType
     }
     get[Symbol.toStringTag]() {
         return `${this.VectorName}<${this.type[Symbol.toStringTag]}>`
     }
@@ -3563,24 +3563,24 @@
     }
     includes(t, e) {
         return this.indexOf(t, e) > 0
     }
     getByteLength(t) {
         return 0
     } [Symbol.iterator]() {
-        return rs.visit(this)
+        return as.visit(this)
     }
     concat(...t) {
-        return new P(this.data.concat(t.flatMap(e => e.data).flat(Number.POSITIVE_INFINITY)))
+        return new z(this.data.concat(t.flatMap(e => e.data).flat(Number.POSITIVE_INFINITY)))
     }
     slice(t, e) {
-        return new P(Da(this, t, e, ({
+        return new z(Ta(this, t, e, ({
             data: i,
             _offsets: r
-        }, s, o) => xa(i, r, s, o)))
+        }, s, o) => La(i, r, s, o)))
     }
     toJSON() {
         return [...this]
     }
     toArray() {
         const {
             type: t,
@@ -3616,79 +3616,79 @@
         return `[${[...this].join(",")}]`
     }
     getChild(t) {
         var e;
         return this.getChildAt((e = this.type.children) === null || e === void 0 ? void 0 : e.findIndex(i => i.name === t))
     }
     getChildAt(t) {
-        return t > -1 && t < this.numChildren ? new P(this.data.map(({
+        return t > -1 && t < this.numChildren ? new z(this.data.map(({
             children: e
         }) => e[t])) : null
     }
     get isMemoized() {
-        return S.isDictionary(this.type) ? this.data[0].dictionary.isMemoized : !1
+        return I.isDictionary(this.type) ? this.data[0].dictionary.isMemoized : !1
     }
     memoize() {
-        if (S.isDictionary(this.type)) {
-            const t = new Bi(this.data[0].dictionary),
+        if (I.isDictionary(this.type)) {
+            const t = new Fi(this.data[0].dictionary),
                 e = this.data.map(i => {
                     const r = i.clone();
                     return r.dictionary = t, r
                 });
-            return new P(e)
+            return new z(e)
         }
-        return new Bi(this)
+        return new Fi(this)
     }
     unmemoize() {
-        if (S.isDictionary(this.type) && this.isMemoized) {
+        if (I.isDictionary(this.type) && this.isMemoized) {
             const t = this.data[0].dictionary.unmemoize(),
                 e = this.data.map(i => {
                     const r = i.clone();
                     return r.dictionary = t, r
                 });
-            return new P(e)
+            return new z(e)
         }
         return this
     }
 }
-Ua = Symbol.toStringTag;
-P[Ua] = (n => {
-    n.type = S.prototype, n.data = [], n.length = 0, n.stride = 1, n.numChildren = 0, n._nullCount = -1, n._byteLength = -1, n._offsets = new Uint32Array([0]), n[Symbol.isConcatSpreadable] = !0;
+$a = Symbol.toStringTag;
+z[$a] = (n => {
+    n.type = I.prototype, n.data = [], n.length = 0, n.stride = 1, n.numChildren = 0, n._nullCount = -1, n._byteLength = -1, n._offsets = new Uint32Array([0]), n[Symbol.isConcatSpreadable] = !0;
     const t = Object.keys(u).map(e => u[e]).filter(e => typeof e == "number" && e !== u.NONE);
     for (const e of t) {
         const i = Ft.getVisitFnByTypeId(e),
             r = Vt.getVisitFnByTypeId(e),
-            s = Ii.getVisitFnByTypeId(e),
-            o = ie.getVisitFnByTypeId(e);
+            s = Oi.getVisitFnByTypeId(e),
+            o = oe.getVisitFnByTypeId(e);
         Va[e] = {
             get: i,
             set: r,
             indexOf: s,
             byteLength: o
-        }, $a[e] = Object.create(n, {
+        }, Pa[e] = Object.create(n, {
             isValid: {
-                value: ln(is)
+                value: un(os)
             },
             get: {
-                value: ln(Ft.getVisitFnByTypeId(e))
+                value: un(Ft.getVisitFnByTypeId(e))
             },
             set: {
-                value: La(Vt.getVisitFnByTypeId(e))
+                value: Ea(Vt.getVisitFnByTypeId(e))
             },
             indexOf: {
-                value: Ea(Ii.getVisitFnByTypeId(e))
+                value: Ra(Oi.getVisitFnByTypeId(e))
             },
             getByteLength: {
-                value: ln(ie.getVisitFnByTypeId(e))
+                value: un(oe.getVisitFnByTypeId(e))
             }
         })
     }
     return "Vector"
-})(P.prototype);
-class Bi extends P {
+})(z.prototype);
+class Fi extends z {
     constructor(t) {
         super(t.data);
         const e = this.get,
             i = this.set,
             r = this.slice,
             s = new Array(this.length);
         Object.defineProperty(this, "get", {
@@ -3699,25 +3699,25 @@
                 return s[o] = l, l
             }
         }), Object.defineProperty(this, "set", {
             value(o, a) {
                 i.call(this, o, a), s[o] = a
             }
         }), Object.defineProperty(this, "slice", {
-            value: (o, a) => new Bi(r.call(this, o, a))
+            value: (o, a) => new Fi(r.call(this, o, a))
         }), Object.defineProperty(this, "isMemoized", {
             value: !0
         }), Object.defineProperty(this, "unmemoize", {
-            value: () => new P(this.data)
+            value: () => new z(this.data)
         }), Object.defineProperty(this, "memoize", {
             value: () => this
         })
     }
 }
-class Br {
+class Ar {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     offset() {
@@ -3732,47 +3732,47 @@
     static sizeOf() {
         return 24
     }
     static createBlock(t, e, i, r) {
         return t.prep(8, 24), t.writeInt64(r), t.pad(4), t.writeInt32(i), t.writeInt64(e), t.offset()
     }
 }
-const dr = 2,
-    Jt = 4,
-    ue = 4,
-    J = 4,
-    _e = new Int32Array(2),
-    Es = new Float32Array(_e.buffer),
-    Rs = new Float64Array(_e.buffer),
-    Xn = new Uint16Array(new Uint8Array([1, 0]).buffer)[0] === 1;
-let he = class Or {
+const fr = 2,
+    Zt = 4,
+    pe = 4,
+    Z = 4,
+    Be = new Int32Array(2),
+    Rs = new Float32Array(Be.buffer),
+    Cs = new Float64Array(Be.buffer),
+    ti = new Uint16Array(new Uint8Array([1, 0]).buffer)[0] === 1;
+let me = class Dr {
     constructor(t, e) {
         this.low = t | 0, this.high = e | 0
     }
     static create(t, e) {
-        return t == 0 && e == 0 ? Or.ZERO : new Or(t, e)
+        return t == 0 && e == 0 ? Dr.ZERO : new Dr(t, e)
     }
     toFloat64() {
         return (this.low >>> 0) + this.high * 4294967296
     }
     equals(t) {
         return this.low == t.low && this.high == t.high
     }
 };
-he.ZERO = new he(0, 0);
-var Fr;
+me.ZERO = new me(0, 0);
+var Tr;
 (function(n) {
     n[n.UTF8_BYTES = 1] = "UTF8_BYTES", n[n.UTF16_STRING = 2] = "UTF16_STRING"
-})(Fr || (Fr = {}));
-let hn = class Pa {
+})(Tr || (Tr = {}));
+let yn = class ja {
         constructor(t) {
             this.bytes_ = t, this.position_ = 0
         }
         static allocate(t) {
-            return new Pa(new Uint8Array(t))
+            return new ja(new Uint8Array(t))
         }
         clear() {
             this.position_ = 0
         }
         bytes() {
             return this.bytes_
         }
@@ -3800,24 +3800,24 @@
         readInt32(t) {
             return this.bytes_[t] | this.bytes_[t + 1] << 8 | this.bytes_[t + 2] << 16 | this.bytes_[t + 3] << 24
         }
         readUint32(t) {
             return this.readInt32(t) >>> 0
         }
         readInt64(t) {
-            return new he(this.readInt32(t), this.readInt32(t + 4))
+            return new me(this.readInt32(t), this.readInt32(t + 4))
         }
         readUint64(t) {
-            return new he(this.readUint32(t), this.readUint32(t + 4))
+            return new me(this.readUint32(t), this.readUint32(t + 4))
         }
         readFloat32(t) {
-            return _e[0] = this.readInt32(t), Es[0]
+            return Be[0] = this.readInt32(t), Rs[0]
         }
         readFloat64(t) {
-            return _e[Xn ? 0 : 1] = this.readInt32(t), _e[Xn ? 1 : 0] = this.readInt32(t + 4), Rs[0]
+            return Be[ti ? 0 : 1] = this.readInt32(t), Be[ti ? 1 : 0] = this.readInt32(t + 4), Cs[0]
         }
         writeInt8(t, e) {
             this.bytes_[t] = e
         }
         writeUint8(t, e) {
             this.bytes_[t] = e
         }
@@ -3836,38 +3836,38 @@
         writeInt64(t, e) {
             this.writeInt32(t, e.low), this.writeInt32(t + 4, e.high)
         }
         writeUint64(t, e) {
             this.writeUint32(t, e.low), this.writeUint32(t + 4, e.high)
         }
         writeFloat32(t, e) {
-            Es[0] = e, this.writeInt32(t, _e[0])
+            Rs[0] = e, this.writeInt32(t, Be[0])
         }
         writeFloat64(t, e) {
-            Rs[0] = e, this.writeInt32(t, _e[Xn ? 0 : 1]), this.writeInt32(t + 4, _e[Xn ? 1 : 0])
+            Cs[0] = e, this.writeInt32(t, Be[ti ? 0 : 1]), this.writeInt32(t + 4, Be[ti ? 1 : 0])
         }
         getBufferIdentifier() {
-            if (this.bytes_.length < this.position_ + Jt + ue) throw new Error("FlatBuffers: ByteBuffer is too short to contain an identifier.");
+            if (this.bytes_.length < this.position_ + Zt + pe) throw new Error("FlatBuffers: ByteBuffer is too short to contain an identifier.");
             let t = "";
-            for (let e = 0; e < ue; e++) t += String.fromCharCode(this.readInt8(this.position_ + Jt + e));
+            for (let e = 0; e < pe; e++) t += String.fromCharCode(this.readInt8(this.position_ + Zt + e));
             return t
         }
         __offset(t, e) {
             const i = t - this.readInt32(t);
             return e < this.readInt16(i) ? this.readInt16(i + e) : 0
         }
         __union(t, e) {
             return t.bb_pos = e + this.readInt32(e), t.bb = this, t
         }
         __string(t, e) {
             t += this.readInt32(t);
             const i = this.readInt32(t);
             let r = "",
                 s = 0;
-            if (t += Jt, e === Fr.UTF8_BYTES) return this.bytes_.subarray(t, t + i);
+            if (t += Zt, e === Tr.UTF8_BYTES) return this.bytes_.subarray(t, t + i);
             for (; s < i;) {
                 let o;
                 const a = this.readUint8(t + s++);
                 if (a < 192) o = a;
                 else {
                     const l = this.readUint8(t + s++);
                     if (a < 224) o = (a & 31) << 6 | l & 63;
@@ -3887,27 +3887,27 @@
         __union_with_string(t, e) {
             return typeof t == "string" ? this.__string(e) : this.__union(t, e)
         }
         __indirect(t) {
             return t + this.readInt32(t)
         }
         __vector(t) {
-            return t + this.readInt32(t) + Jt
+            return t + this.readInt32(t) + Zt
         }
         __vector_len(t) {
             return this.readInt32(t + this.readInt32(t))
         }
         __has_identifier(t) {
-            if (t.length != ue) throw new Error("FlatBuffers: file identifier must be length " + ue);
-            for (let e = 0; e < ue; e++)
-                if (t.charCodeAt(e) != this.readInt8(this.position() + Jt + e)) return !1;
+            if (t.length != pe) throw new Error("FlatBuffers: file identifier must be length " + pe);
+            for (let e = 0; e < pe; e++)
+                if (t.charCodeAt(e) != this.readInt8(this.position() + Zt + e)) return !1;
             return !0
         }
         createLong(t, e) {
-            return he.create(t, e)
+            return me.create(t, e)
         }
         createScalarList(t, e) {
             const i = [];
             for (let r = 0; r < e; ++r) t(r) !== null && i.push(t(r));
             return i
         }
         createObjList(t, e) {
@@ -3915,19 +3915,19 @@
             for (let r = 0; r < e; ++r) {
                 const s = t(r);
                 s !== null && i.push(s.unpack())
             }
             return i
         }
     },
-    ja = class za {
+    za = class Wa {
         constructor(t) {
             this.minalign = 1, this.vtable = null, this.vtable_in_use = 0, this.isNested = !1, this.object_start = 0, this.vtables = [], this.vector_num_elems = 0, this.force_defaults = !1, this.string_maps = null;
             let e;
-            t ? e = t : e = 1024, this.bb = hn.allocate(e), this.space = e
+            t ? e = t : e = 1024, this.bb = yn.allocate(e), this.space = e
         }
         clear() {
             this.bb.clear(), this.space = this.bb.capacity(), this.minalign = 1, this.vtable = null, this.vtable_in_use = 0, this.isNested = !1, this.object_start = 0, this.vtables = [], this.vector_num_elems = 0, this.force_defaults = !1, this.string_maps = null
         }
         forceDefaults(t) {
             this.force_defaults = t
         }
@@ -3938,15 +3938,15 @@
             return this.bb.bytes().subarray(this.bb.position(), this.bb.position() + this.offset())
         }
         prep(t, e) {
             t > this.minalign && (this.minalign = t);
             const i = ~(this.bb.capacity() - this.space + e) + 1 & t - 1;
             for (; this.space < i + t + e;) {
                 const r = this.bb.capacity();
-                this.bb = za.growByteBuffer(this.bb), this.space += this.bb.capacity() - r
+                this.bb = Wa.growByteBuffer(this.bb), this.space += this.bb.capacity() - r
             }
             this.pad(i)
         }
         pad(t) {
             for (let e = 0; e < t; e++) this.bb.writeInt8(--this.space, 0)
         }
         writeInt8(t) {
@@ -4021,19 +4021,19 @@
         offset() {
             return this.bb.capacity() - this.space
         }
         static growByteBuffer(t) {
             const e = t.capacity();
             if (e & 3221225472) throw new Error("FlatBuffers: cannot grow buffer beyond 2 gigabytes.");
             const i = e << 1,
-                r = hn.allocate(i);
+                r = yn.allocate(i);
             return r.setPosition(i - e), r.bytes().set(t.bytes(), i - e), r
         }
         addOffset(t) {
-            this.prep(Jt, 0), this.writeInt32(this.offset() - t + Jt)
+            this.prep(Zt, 0), this.writeInt32(this.offset() - t + Zt)
         }
         startObject(t) {
             this.notNested(), this.vtable == null && (this.vtable = []), this.vtable_in_use = t;
             for (let e = 0; e < t; e++) this.vtable[e] = 0;
             this.isNested = !0, this.object_start = this.offset()
         }
         endObject() {
@@ -4042,48 +4042,48 @@
             const t = this.offset();
             let e = this.vtable_in_use - 1;
             for (; e >= 0 && this.vtable[e] == 0; e--);
             const i = e + 1;
             for (; e >= 0; e--) this.addInt16(this.vtable[e] != 0 ? t - this.vtable[e] : 0);
             const r = 2;
             this.addInt16(t - this.object_start);
-            const s = (i + r) * dr;
+            const s = (i + r) * fr;
             this.addInt16(s);
             let o = 0;
             const a = this.space;
             t: for (e = 0; e < this.vtables.length; e++) {
                 const l = this.bb.capacity() - this.vtables[e];
                 if (s == this.bb.readInt16(l)) {
-                    for (let c = dr; c < s; c += dr)
+                    for (let c = fr; c < s; c += fr)
                         if (this.bb.readInt16(a + c) != this.bb.readInt16(l + c)) continue t;
                     o = this.vtables[e];
                     break
                 }
             }
             return o ? (this.space = this.bb.capacity() - t, this.bb.writeInt32(this.space, o - t)) : (this.vtables.push(this.offset()), this.bb.writeInt32(this.bb.capacity() - t, this.offset() - t)), this.isNested = !1, t
         }
         finish(t, e, i) {
-            const r = i ? J : 0;
+            const r = i ? Z : 0;
             if (e) {
                 const s = e;
-                if (this.prep(this.minalign, Jt + ue + r), s.length != ue) throw new Error("FlatBuffers: file identifier must be length " + ue);
-                for (let o = ue - 1; o >= 0; o--) this.writeInt8(s.charCodeAt(o))
+                if (this.prep(this.minalign, Zt + pe + r), s.length != pe) throw new Error("FlatBuffers: file identifier must be length " + pe);
+                for (let o = pe - 1; o >= 0; o--) this.writeInt8(s.charCodeAt(o))
             }
-            this.prep(this.minalign, Jt + r), this.addOffset(t), r && this.addInt32(this.bb.capacity() - this.space), this.bb.setPosition(this.space)
+            this.prep(this.minalign, Zt + r), this.addOffset(t), r && this.addInt32(this.bb.capacity() - this.space), this.bb.setPosition(this.space)
         }
         finishSizePrefixed(t, e) {
             this.finish(t, e, !0)
         }
         requiredField(t, e) {
             const i = this.bb.capacity() - t,
                 r = i - this.bb.readInt32(i);
             if (!(this.bb.readInt16(r + e) != 0)) throw new Error("FlatBuffers: field " + e + " must be set")
         }
         startVector(t, e, i) {
-            this.notNested(), this.vector_num_elems = e, this.prep(Jt, t * e), this.prep(i, t * e)
+            this.notNested(), this.vector_num_elems = e, this.prep(Zt, t * e), this.prep(i, t * e)
         }
         endVector() {
             return this.writeInt32(this.vector_num_elems), this.offset()
         }
         createSharedString(t) {
             if (!t) return 0;
             if (this.string_maps || (this.string_maps = new Map), this.string_maps.has(t)) return this.string_maps.get(t);
@@ -4109,15 +4109,15 @@
                 }
             }
             this.addInt8(0), this.startVector(1, e.length, 1), this.bb.setPosition(this.space -= e.length);
             for (let i = 0, r = this.space, s = this.bb.bytes(); i < e.length; i++) s[r++] = e[i];
             return this.endVector()
         }
         createLong(t, e) {
-            return he.create(t, e)
+            return me.create(t, e)
         }
         createObjectOffset(t) {
             return t === null ? 0 : typeof t == "string" ? this.createString(t) : t.pack(this)
         }
         createObjectOffsetList(t) {
             const e = [];
             for (let i = 0; i < t.length; ++i) {
@@ -4138,15 +4138,15 @@
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsKeyValue(t, e) {
         return (e || new ut).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsKeyValue(t, e) {
-        return t.setPosition(t.position() + J), (e || new ut).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new ut).__init(t.readInt32(t.position()) + t.position(), t)
     }
     key(t) {
         const e = this.bb.__offset(this.bb_pos, 4);
         return e ? this.bb.__string(this.bb_pos + e, t) : null
     }
     value(t) {
         const e = this.bb.__offset(this.bb_pos, 6);
@@ -4164,38 +4164,38 @@
     static endKeyValue(t) {
         return t.endObject()
     }
     static createKeyValue(t, e, i) {
         return ut.startKeyValue(t), ut.addKey(t, e), ut.addValue(t, i), ut.endKeyValue(t)
     }
 }
-var fn;
+var mn;
 (function(n) {
     n[n.V1 = 0] = "V1", n[n.V2 = 1] = "V2", n[n.V3 = 2] = "V3", n[n.V4 = 3] = "V4", n[n.V5 = 4] = "V5"
-})(fn || (fn = {}));
-var pn;
+})(mn || (mn = {}));
+var vn;
 (function(n) {
     n[n.Little = 0] = "Little", n[n.Big = 1] = "Big"
-})(pn || (pn = {}));
-var Oi;
+})(vn || (vn = {}));
+var Ai;
 (function(n) {
     n[n.DenseArray = 0] = "DenseArray"
-})(Oi || (Oi = {}));
+})(Ai || (Ai = {}));
 class Tt {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsInt(t, e) {
         return (e || new Tt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsInt(t, e) {
-        return t.setPosition(t.position() + J), (e || new Tt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Tt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     bitWidth() {
         const t = this.bb.__offset(this.bb_pos, 4);
         return t ? this.bb.readInt32(this.bb_pos + t) : 0
     }
     isSigned() {
         const t = this.bb.__offset(this.bb_pos, 6);
@@ -4213,26 +4213,26 @@
     static endInt(t) {
         return t.endObject()
     }
     static createInt(t, e, i) {
         return Tt.startInt(t), Tt.addBitWidth(t, e), Tt.addIsSigned(t, i), Tt.endInt(t)
     }
 }
-class de {
+class ye {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsDictionaryEncoding(t, e) {
-        return (e || new de).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new ye).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsDictionaryEncoding(t, e) {
-        return t.setPosition(t.position() + J), (e || new de).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new ye).__init(t.readInt32(t.position()) + t.position(), t)
     }
     id() {
         const t = this.bb.__offset(this.bb_pos, 4);
         return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
     }
     indexType(t) {
         const e = this.bb.__offset(this.bb_pos, 6);
@@ -4240,127 +4240,127 @@
     }
     isOrdered() {
         const t = this.bb.__offset(this.bb_pos, 8);
         return t ? !!this.bb.readInt8(this.bb_pos + t) : !1
     }
     dictionaryKind() {
         const t = this.bb.__offset(this.bb_pos, 10);
-        return t ? this.bb.readInt16(this.bb_pos + t) : Oi.DenseArray
+        return t ? this.bb.readInt16(this.bb_pos + t) : Ai.DenseArray
     }
     static startDictionaryEncoding(t) {
         t.startObject(4)
     }
     static addId(t, e) {
         t.addFieldInt64(0, e, t.createLong(0, 0))
     }
     static addIndexType(t, e) {
         t.addFieldOffset(1, e, 0)
     }
     static addIsOrdered(t, e) {
         t.addFieldInt8(2, +e, 0)
     }
     static addDictionaryKind(t, e) {
-        t.addFieldInt16(3, e, Oi.DenseArray)
+        t.addFieldInt16(3, e, Ai.DenseArray)
     }
     static endDictionaryEncoding(t) {
         return t.endObject()
     }
 }
-class Ce {
+class $e {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsBinary(t, e) {
-        return (e || new Ce).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new $e).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsBinary(t, e) {
-        return t.setPosition(t.position() + J), (e || new Ce).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new $e).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static startBinary(t) {
         t.startObject(0)
     }
     static endBinary(t) {
         return t.endObject()
     }
     static createBinary(t) {
-        return Ce.startBinary(t), Ce.endBinary(t)
+        return $e.startBinary(t), $e.endBinary(t)
     }
 }
-class ke {
+class Ve {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsBool(t, e) {
-        return (e || new ke).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Ve).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsBool(t, e) {
-        return t.setPosition(t.position() + J), (e || new ke).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Ve).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static startBool(t) {
         t.startObject(0)
     }
     static endBool(t) {
         return t.endObject()
     }
     static createBool(t) {
-        return ke.startBool(t), ke.endBool(t)
+        return Ve.startBool(t), Ve.endBool(t)
     }
 }
-var Fi;
+var Di;
 (function(n) {
     n[n.DAY = 0] = "DAY", n[n.MILLISECOND = 1] = "MILLISECOND"
-})(Fi || (Fi = {}));
-let ii = class Qe {
+})(Di || (Di = {}));
+let si = class en {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsDate(t, e) {
-        return (e || new Qe).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new en).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsDate(t, e) {
-        return t.setPosition(t.position() + J), (e || new Qe).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new en).__init(t.readInt32(t.position()) + t.position(), t)
     }
     unit() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : Fi.MILLISECOND
+        return t ? this.bb.readInt16(this.bb_pos + t) : Di.MILLISECOND
     }
     static startDate(t) {
         t.startObject(1)
     }
     static addUnit(t, e) {
-        t.addFieldInt16(0, e, Fi.MILLISECOND)
+        t.addFieldInt16(0, e, Di.MILLISECOND)
     }
     static endDate(t) {
         return t.endObject()
     }
     static createDate(t, e) {
-        return Qe.startDate(t), Qe.addUnit(t, e), Qe.endDate(t)
+        return en.startDate(t), en.addUnit(t, e), en.endDate(t)
     }
 };
-class _t {
+class wt {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsDecimal(t, e) {
-        return (e || new _t).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new wt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsDecimal(t, e) {
-        return t.setPosition(t.position() + J), (e || new _t).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new wt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     precision() {
         const t = this.bb.__offset(this.bb_pos, 4);
         return t ? this.bb.readInt32(this.bb_pos + t) : 0
     }
     scale() {
         const t = this.bb.__offset(this.bb_pos, 6);
@@ -4382,33 +4382,33 @@
     static addBitWidth(t, e) {
         t.addFieldInt32(2, e, 128)
     }
     static endDecimal(t) {
         return t.endObject()
     }
     static createDecimal(t, e, i, r) {
-        return _t.startDecimal(t), _t.addPrecision(t, e), _t.addScale(t, i), _t.addBitWidth(t, r), _t.endDecimal(t)
+        return wt.startDecimal(t), wt.addPrecision(t, e), wt.addScale(t, i), wt.addBitWidth(t, r), wt.endDecimal(t)
     }
 }
-var yn;
+var bn;
 (function(n) {
     n[n.SECOND = 0] = "SECOND", n[n.MILLISECOND = 1] = "MILLISECOND", n[n.MICROSECOND = 2] = "MICROSECOND", n[n.NANOSECOND = 3] = "NANOSECOND"
-})(yn || (yn = {}));
-class Kt {
+})(bn || (bn = {}));
+class Xt {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsFixedSizeBinary(t, e) {
-        return (e || new Kt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Xt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsFixedSizeBinary(t, e) {
-        return t.setPosition(t.position() + J), (e || new Kt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Xt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     byteWidth() {
         const t = this.bb.__offset(this.bb_pos, 4);
         return t ? this.bb.readInt32(this.bb_pos + t) : 0
     }
     static startFixedSizeBinary(t) {
         t.startObject(1)
@@ -4416,29 +4416,29 @@
     static addByteWidth(t, e) {
         t.addFieldInt32(0, e, 0)
     }
     static endFixedSizeBinary(t) {
         return t.endObject()
     }
     static createFixedSizeBinary(t, e) {
-        return Kt.startFixedSizeBinary(t), Kt.addByteWidth(t, e), Kt.endFixedSizeBinary(t)
+        return Xt.startFixedSizeBinary(t), Xt.addByteWidth(t, e), Xt.endFixedSizeBinary(t)
     }
 }
-class Zt {
+class Qt {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsFixedSizeList(t, e) {
-        return (e || new Zt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Qt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsFixedSizeList(t, e) {
-        return t.setPosition(t.position() + J), (e || new Zt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Qt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     listSize() {
         const t = this.bb.__offset(this.bb_pos, 4);
         return t ? this.bb.readInt32(this.bb_pos + t) : 0
     }
     static startFixedSizeList(t) {
         t.startObject(1)
@@ -4446,120 +4446,120 @@
     static addListSize(t, e) {
         t.addFieldInt32(0, e, 0)
     }
     static endFixedSizeList(t) {
         return t.endObject()
     }
     static createFixedSizeList(t, e) {
-        return Zt.startFixedSizeList(t), Zt.addListSize(t, e), Zt.endFixedSizeList(t)
+        return Qt.startFixedSizeList(t), Qt.addListSize(t, e), Qt.endFixedSizeList(t)
     }
 }
-var Ai;
+var Ti;
 (function(n) {
     n[n.HALF = 0] = "HALF", n[n.SINGLE = 1] = "SINGLE", n[n.DOUBLE = 2] = "DOUBLE"
-})(Ai || (Ai = {}));
-class Xt {
+})(Ti || (Ti = {}));
+class te {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsFloatingPoint(t, e) {
-        return (e || new Xt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new te).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsFloatingPoint(t, e) {
-        return t.setPosition(t.position() + J), (e || new Xt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new te).__init(t.readInt32(t.position()) + t.position(), t)
     }
     precision() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : Ai.HALF
+        return t ? this.bb.readInt16(this.bb_pos + t) : Ti.HALF
     }
     static startFloatingPoint(t) {
         t.startObject(1)
     }
     static addPrecision(t, e) {
-        t.addFieldInt16(0, e, Ai.HALF)
+        t.addFieldInt16(0, e, Ti.HALF)
     }
     static endFloatingPoint(t) {
         return t.endObject()
     }
     static createFloatingPoint(t, e) {
-        return Xt.startFloatingPoint(t), Xt.addPrecision(t, e), Xt.endFloatingPoint(t)
+        return te.startFloatingPoint(t), te.addPrecision(t, e), te.endFloatingPoint(t)
     }
 }
-var Di;
+var Ni;
 (function(n) {
     n[n.YEAR_MONTH = 0] = "YEAR_MONTH", n[n.DAY_TIME = 1] = "DAY_TIME", n[n.MONTH_DAY_NANO = 2] = "MONTH_DAY_NANO"
-})(Di || (Di = {}));
-class Qt {
+})(Ni || (Ni = {}));
+class ee {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsInterval(t, e) {
-        return (e || new Qt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new ee).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsInterval(t, e) {
-        return t.setPosition(t.position() + J), (e || new Qt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new ee).__init(t.readInt32(t.position()) + t.position(), t)
     }
     unit() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : Di.YEAR_MONTH
+        return t ? this.bb.readInt16(this.bb_pos + t) : Ni.YEAR_MONTH
     }
     static startInterval(t) {
         t.startObject(1)
     }
     static addUnit(t, e) {
-        t.addFieldInt16(0, e, Di.YEAR_MONTH)
+        t.addFieldInt16(0, e, Ni.YEAR_MONTH)
     }
     static endInterval(t) {
         return t.endObject()
     }
     static createInterval(t, e) {
-        return Qt.startInterval(t), Qt.addUnit(t, e), Qt.endInterval(t)
+        return ee.startInterval(t), ee.addUnit(t, e), ee.endInterval(t)
     }
 }
-class Ue {
+class Pe {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsList(t, e) {
-        return (e || new Ue).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Pe).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsList(t, e) {
-        return t.setPosition(t.position() + J), (e || new Ue).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Pe).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static startList(t) {
         t.startObject(0)
     }
     static endList(t) {
         return t.endObject()
     }
     static createList(t) {
-        return Ue.startList(t), Ue.endList(t)
+        return Pe.startList(t), Pe.endList(t)
     }
 }
-let ri = class tn {
+let oi = class nn {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsMap(t, e) {
-        return (e || new tn).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new nn).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsMap(t, e) {
-        return t.setPosition(t.position() + J), (e || new tn).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new nn).__init(t.readInt32(t.position()) + t.position(), t)
     }
     keysSorted() {
         const t = this.bb.__offset(this.bb_pos, 4);
         return t ? !!this.bb.readInt8(this.bb_pos + t) : !1
     }
     static startMap(t) {
         t.startObject(1)
@@ -4567,157 +4567,157 @@
     static addKeysSorted(t, e) {
         t.addFieldInt8(0, +e, 0)
     }
     static endMap(t) {
         return t.endObject()
     }
     static createMap(t, e) {
-        return tn.startMap(t), tn.addKeysSorted(t, e), tn.endMap(t)
+        return nn.startMap(t), nn.addKeysSorted(t, e), nn.endMap(t)
     }
 };
-class Ve {
+class je {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsNull(t, e) {
-        return (e || new Ve).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new je).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsNull(t, e) {
-        return t.setPosition(t.position() + J), (e || new Ve).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new je).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static startNull(t) {
         t.startObject(0)
     }
     static endNull(t) {
         return t.endObject()
     }
     static createNull(t) {
-        return Ve.startNull(t), Ve.endNull(t)
+        return je.startNull(t), je.endNull(t)
     }
 }
-class $e {
+class ze {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsStruct_(t, e) {
-        return (e || new $e).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new ze).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsStruct_(t, e) {
-        return t.setPosition(t.position() + J), (e || new $e).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new ze).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static startStruct_(t) {
         t.startObject(0)
     }
     static endStruct_(t) {
         return t.endObject()
     }
     static createStruct_(t) {
-        return $e.startStruct_(t), $e.endStruct_(t)
+        return ze.startStruct_(t), ze.endStruct_(t)
     }
 }
-class kt {
+class Ut {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsTime(t, e) {
-        return (e || new kt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Ut).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsTime(t, e) {
-        return t.setPosition(t.position() + J), (e || new kt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Ut).__init(t.readInt32(t.position()) + t.position(), t)
     }
     unit() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : yn.MILLISECOND
+        return t ? this.bb.readInt16(this.bb_pos + t) : bn.MILLISECOND
     }
     bitWidth() {
         const t = this.bb.__offset(this.bb_pos, 6);
         return t ? this.bb.readInt32(this.bb_pos + t) : 32
     }
     static startTime(t) {
         t.startObject(2)
     }
     static addUnit(t, e) {
-        t.addFieldInt16(0, e, yn.MILLISECOND)
+        t.addFieldInt16(0, e, bn.MILLISECOND)
     }
     static addBitWidth(t, e) {
         t.addFieldInt32(1, e, 32)
     }
     static endTime(t) {
         return t.endObject()
     }
     static createTime(t, e, i) {
-        return kt.startTime(t), kt.addUnit(t, e), kt.addBitWidth(t, i), kt.endTime(t)
+        return Ut.startTime(t), Ut.addUnit(t, e), Ut.addBitWidth(t, i), Ut.endTime(t)
     }
 }
-class Ut {
+class $t {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsTimestamp(t, e) {
-        return (e || new Ut).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new $t).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsTimestamp(t, e) {
-        return t.setPosition(t.position() + J), (e || new Ut).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new $t).__init(t.readInt32(t.position()) + t.position(), t)
     }
     unit() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : yn.SECOND
+        return t ? this.bb.readInt16(this.bb_pos + t) : bn.SECOND
     }
     timezone(t) {
         const e = this.bb.__offset(this.bb_pos, 6);
         return e ? this.bb.__string(this.bb_pos + e, t) : null
     }
     static startTimestamp(t) {
         t.startObject(2)
     }
     static addUnit(t, e) {
-        t.addFieldInt16(0, e, yn.SECOND)
+        t.addFieldInt16(0, e, bn.SECOND)
     }
     static addTimezone(t, e) {
         t.addFieldOffset(1, e, 0)
     }
     static endTimestamp(t) {
         return t.endObject()
     }
     static createTimestamp(t, e, i) {
-        return Ut.startTimestamp(t), Ut.addUnit(t, e), Ut.addTimezone(t, i), Ut.endTimestamp(t)
+        return $t.startTimestamp(t), $t.addUnit(t, e), $t.addTimezone(t, i), $t.endTimestamp(t)
     }
 }
-var Ti;
+var xi;
 (function(n) {
     n[n.Sparse = 0] = "Sparse", n[n.Dense = 1] = "Dense"
-})(Ti || (Ti = {}));
-class wt {
+})(xi || (xi = {}));
+class St {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsUnion(t, e) {
-        return (e || new wt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new St).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsUnion(t, e) {
-        return t.setPosition(t.position() + J), (e || new wt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new St).__init(t.readInt32(t.position()) + t.position(), t)
     }
     mode() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : Ti.Sparse
+        return t ? this.bb.readInt16(this.bb_pos + t) : xi.Sparse
     }
     typeIds(t) {
         const e = this.bb.__offset(this.bb_pos, 6);
         return e ? this.bb.readInt32(this.bb.__vector(this.bb_pos + e) + t * 4) : 0
     }
     typeIdsLength() {
         const t = this.bb.__offset(this.bb_pos, 6);
@@ -4727,15 +4727,15 @@
         const t = this.bb.__offset(this.bb_pos, 6);
         return t ? new Int32Array(this.bb.bytes().buffer, this.bb.bytes().byteOffset + this.bb.__vector(this.bb_pos + t), this.bb.__vector_len(this.bb_pos + t)) : null
     }
     static startUnion(t) {
         t.startObject(2)
     }
     static addMode(t, e) {
-        t.addFieldInt16(0, e, Ti.Sparse)
+        t.addFieldInt16(0, e, xi.Sparse)
     }
     static addTypeIds(t, e) {
         t.addFieldOffset(1, e, 0)
     }
     static createTypeIdsVector(t, e) {
         t.startVector(4, e.length, 4);
         for (let i = e.length - 1; i >= 0; i--) t.addInt32(e[i]);
@@ -4744,80 +4744,80 @@
     static startTypeIdsVector(t, e) {
         t.startVector(4, e, 4)
     }
     static endUnion(t) {
         return t.endObject()
     }
     static createUnion(t, e, i) {
-        return wt.startUnion(t), wt.addMode(t, e), wt.addTypeIds(t, i), wt.endUnion(t)
+        return St.startUnion(t), St.addMode(t, e), St.addTypeIds(t, i), St.endUnion(t)
     }
 }
-class Pe {
+class We {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsUtf8(t, e) {
-        return (e || new Pe).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new We).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsUtf8(t, e) {
-        return t.setPosition(t.position() + J), (e || new Pe).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new We).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static startUtf8(t) {
         t.startObject(0)
     }
     static endUtf8(t) {
         return t.endObject()
     }
     static createUtf8(t) {
-        return Pe.startUtf8(t), Pe.endUtf8(t)
+        return We.startUtf8(t), We.endUtf8(t)
     }
 }
-var Q;
+var nt;
 (function(n) {
     n[n.NONE = 0] = "NONE", n[n.Null = 1] = "Null", n[n.Int = 2] = "Int", n[n.FloatingPoint = 3] = "FloatingPoint", n[n.Binary = 4] = "Binary", n[n.Utf8 = 5] = "Utf8", n[n.Bool = 6] = "Bool", n[n.Decimal = 7] = "Decimal", n[n.Date = 8] = "Date", n[n.Time = 9] = "Time", n[n.Timestamp = 10] = "Timestamp", n[n.Interval = 11] = "Interval", n[n.List = 12] = "List", n[n.Struct_ = 13] = "Struct_", n[n.Union = 14] = "Union", n[n.FixedSizeBinary = 15] = "FixedSizeBinary", n[n.FixedSizeList = 16] = "FixedSizeList", n[n.Map = 17] = "Map", n[n.Duration = 18] = "Duration", n[n.LargeBinary = 19] = "LargeBinary", n[n.LargeUtf8 = 20] = "LargeUtf8", n[n.LargeList = 21] = "LargeList"
-})(Q || (Q = {}));
-let Rt = class si {
+})(nt || (nt = {}));
+let Ct = class ai {
         constructor() {
             this.bb = null, this.bb_pos = 0
         }
         __init(t, e) {
             return this.bb_pos = t, this.bb = e, this
         }
         static getRootAsField(t, e) {
-            return (e || new si).__init(t.readInt32(t.position()) + t.position(), t)
+            return (e || new ai).__init(t.readInt32(t.position()) + t.position(), t)
         }
         static getSizePrefixedRootAsField(t, e) {
-            return t.setPosition(t.position() + J), (e || new si).__init(t.readInt32(t.position()) + t.position(), t)
+            return t.setPosition(t.position() + Z), (e || new ai).__init(t.readInt32(t.position()) + t.position(), t)
         }
         name(t) {
             const e = this.bb.__offset(this.bb_pos, 4);
             return e ? this.bb.__string(this.bb_pos + e, t) : null
         }
         nullable() {
             const t = this.bb.__offset(this.bb_pos, 6);
             return t ? !!this.bb.readInt8(this.bb_pos + t) : !1
         }
         typeType() {
             const t = this.bb.__offset(this.bb_pos, 8);
-            return t ? this.bb.readUint8(this.bb_pos + t) : Q.NONE
+            return t ? this.bb.readUint8(this.bb_pos + t) : nt.NONE
         }
         type(t) {
             const e = this.bb.__offset(this.bb_pos, 10);
             return e ? this.bb.__union(t, this.bb_pos + e) : null
         }
         dictionary(t) {
             const e = this.bb.__offset(this.bb_pos, 12);
-            return e ? (t || new de).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+            return e ? (t || new ye).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
         }
         children(t, e) {
             const i = this.bb.__offset(this.bb_pos, 14);
-            return i ? (e || new si).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + i) + t * 4), this.bb) : null
+            return i ? (e || new ai).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + i) + t * 4), this.bb) : null
         }
         childrenLength() {
             const t = this.bb.__offset(this.bb_pos, 14);
             return t ? this.bb.__vector_len(this.bb_pos + t) : 0
         }
         customMetadata(t, e) {
             const i = this.bb.__offset(this.bb_pos, 16);
@@ -4833,15 +4833,15 @@
         static addName(t, e) {
             t.addFieldOffset(0, e, 0)
         }
         static addNullable(t, e) {
             t.addFieldInt8(1, +e, 0)
         }
         static addTypeType(t, e) {
-            t.addFieldInt8(2, e, Q.NONE)
+            t.addFieldInt8(2, e, nt.NONE)
         }
         static addType(t, e) {
             t.addFieldOffset(3, e, 0)
         }
         static addDictionary(t, e) {
             t.addFieldOffset(4, e, 0)
         }
@@ -4867,34 +4867,34 @@
         static startCustomMetadataVector(t, e) {
             t.startVector(4, e, 4)
         }
         static endField(t) {
             return t.endObject()
         }
     },
-    Yt = class oe {
+    Ht = class ue {
         constructor() {
             this.bb = null, this.bb_pos = 0
         }
         __init(t, e) {
             return this.bb_pos = t, this.bb = e, this
         }
         static getRootAsSchema(t, e) {
-            return (e || new oe).__init(t.readInt32(t.position()) + t.position(), t)
+            return (e || new ue).__init(t.readInt32(t.position()) + t.position(), t)
         }
         static getSizePrefixedRootAsSchema(t, e) {
-            return t.setPosition(t.position() + J), (e || new oe).__init(t.readInt32(t.position()) + t.position(), t)
+            return t.setPosition(t.position() + Z), (e || new ue).__init(t.readInt32(t.position()) + t.position(), t)
         }
         endianness() {
             const t = this.bb.__offset(this.bb_pos, 4);
-            return t ? this.bb.readInt16(this.bb_pos + t) : pn.Little
+            return t ? this.bb.readInt16(this.bb_pos + t) : vn.Little
         }
         fields(t, e) {
             const i = this.bb.__offset(this.bb_pos, 6);
-            return i ? (e || new Rt).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + i) + t * 4), this.bb) : null
+            return i ? (e || new Ct).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + i) + t * 4), this.bb) : null
         }
         fieldsLength() {
             const t = this.bb.__offset(this.bb_pos, 6);
             return t ? this.bb.__vector_len(this.bb_pos + t) : 0
         }
         customMetadata(t, e) {
             const i = this.bb.__offset(this.bb_pos, 8);
@@ -4912,15 +4912,15 @@
             const t = this.bb.__offset(this.bb_pos, 10);
             return t ? this.bb.__vector_len(this.bb_pos + t) : 0
         }
         static startSchema(t) {
             t.startObject(4)
         }
         static addEndianness(t, e) {
-            t.addFieldInt16(0, e, pn.Little)
+            t.addFieldInt16(0, e, vn.Little)
         }
         static addFields(t, e) {
             t.addFieldOffset(1, e, 0)
         }
         static createFieldsVector(t, e) {
             t.startVector(4, e.length, 4);
             for (let i = e.length - 1; i >= 0; i--) t.addOffset(e[i]);
@@ -4957,49 +4957,49 @@
         static finishSchemaBuffer(t, e) {
             t.finish(e)
         }
         static finishSizePrefixedSchemaBuffer(t, e) {
             t.finish(e, void 0, !0)
         }
         static createSchema(t, e, i, r, s) {
-            return oe.startSchema(t), oe.addEndianness(t, e), oe.addFields(t, i), oe.addCustomMetadata(t, r), oe.addFeatures(t, s), oe.endSchema(t)
+            return ue.startSchema(t), ue.addEndianness(t, e), ue.addFields(t, i), ue.addCustomMetadata(t, r), ue.addFeatures(t, s), ue.endSchema(t)
         }
     };
 class Dt {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsFooter(t, e) {
         return (e || new Dt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsFooter(t, e) {
-        return t.setPosition(t.position() + J), (e || new Dt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Dt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     version() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : fn.V1
+        return t ? this.bb.readInt16(this.bb_pos + t) : mn.V1
     }
     schema(t) {
         const e = this.bb.__offset(this.bb_pos, 6);
-        return e ? (t || new Yt).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+        return e ? (t || new Ht).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
     }
     dictionaries(t, e) {
         const i = this.bb.__offset(this.bb_pos, 8);
-        return i ? (e || new Br).__init(this.bb.__vector(this.bb_pos + i) + t * 24, this.bb) : null
+        return i ? (e || new Ar).__init(this.bb.__vector(this.bb_pos + i) + t * 24, this.bb) : null
     }
     dictionariesLength() {
         const t = this.bb.__offset(this.bb_pos, 8);
         return t ? this.bb.__vector_len(this.bb_pos + t) : 0
     }
     recordBatches(t, e) {
         const i = this.bb.__offset(this.bb_pos, 10);
-        return i ? (e || new Br).__init(this.bb.__vector(this.bb_pos + i) + t * 24, this.bb) : null
+        return i ? (e || new Ar).__init(this.bb.__vector(this.bb_pos + i) + t * 24, this.bb) : null
     }
     recordBatchesLength() {
         const t = this.bb.__offset(this.bb_pos, 10);
         return t ? this.bb.__vector_len(this.bb_pos + t) : 0
     }
     customMetadata(t, e) {
         const i = this.bb.__offset(this.bb_pos, 12);
@@ -5009,15 +5009,15 @@
         const t = this.bb.__offset(this.bb_pos, 12);
         return t ? this.bb.__vector_len(this.bb_pos + t) : 0
     }
     static startFooter(t) {
         t.startObject(5)
     }
     static addVersion(t, e) {
-        t.addFieldInt16(0, e, fn.V1)
+        t.addFieldInt16(0, e, mn.V1)
     }
     static addSchema(t, e) {
         t.addFieldOffset(1, e, 0)
     }
     static addDictionaries(t, e) {
         t.addFieldOffset(2, e, 0)
     }
@@ -5047,62 +5047,62 @@
     static finishFooterBuffer(t, e) {
         t.finish(e)
     }
     static finishSizePrefixedFooterBuffer(t, e) {
         t.finish(e, void 0, !0)
     }
 }
-class j {
+class W {
     constructor(t = [], e, i) {
-        this.fields = t || [], this.metadata = e || new Map, i || (i = Ar(t)), this.dictionaries = i
+        this.fields = t || [], this.metadata = e || new Map, i || (i = Nr(t)), this.dictionaries = i
     }
     get[Symbol.toStringTag]() {
         return "Schema"
     }
     get names() {
         return this.fields.map(t => t.name)
     }
     toString() {
         return `Schema<{ ${this.fields.map((t,e)=>`${e}: ${t}`).join(", ")} }>`
     }
     select(t) {
         const e = new Set(t),
             i = this.fields.filter(r => e.has(r.name));
-        return new j(i, this.metadata)
+        return new W(i, this.metadata)
     }
     selectAt(t) {
         const e = t.map(i => this.fields[i]).filter(Boolean);
-        return new j(e, this.metadata)
+        return new W(e, this.metadata)
     }
     assign(...t) {
-        const e = t[0] instanceof j ? t[0] : Array.isArray(t[0]) ? new j(t[0]) : new j(t),
+        const e = t[0] instanceof W ? t[0] : Array.isArray(t[0]) ? new W(t[0]) : new W(t),
             i = [...this.fields],
-            r = Qn(Qn(new Map, this.metadata), e.metadata),
+            r = ei(ei(new Map, this.metadata), e.metadata),
             s = e.fields.filter(a => {
                 const l = i.findIndex(c => c.name === a.name);
                 return ~l ? (i[l] = a.clone({
-                    metadata: Qn(Qn(new Map, i[l].metadata), a.metadata)
+                    metadata: ei(ei(new Map, i[l].metadata), a.metadata)
                 })) && !1 : !0
             }),
-            o = Ar(s, new Map);
-        return new j([...i, ...s], r, new Map([...this.dictionaries, ...o]))
+            o = Nr(s, new Map);
+        return new W([...i, ...s], r, new Map([...this.dictionaries, ...o]))
     }
 }
-j.prototype.fields = null;
-j.prototype.metadata = null;
-j.prototype.dictionaries = null;
-class X {
+W.prototype.fields = null;
+W.prototype.metadata = null;
+W.prototype.dictionaries = null;
+class tt {
     constructor(t, e, i = !1, r) {
         this.name = t, this.type = e, this.nullable = i, this.metadata = r || new Map
     }
     static new(...t) {
         let [e, i, r, s] = t;
         return t[0] && typeof t[0] == "object" && ({
             name: e
-        } = t[0], i === void 0 && (i = t[0].type), r === void 0 && (r = t[0].nullable), s === void 0 && (s = t[0].metadata)), new X(`${e}`, i, r, s)
+        } = t[0], i === void 0 && (i = t[0].type), r === void 0 && (r = t[0].nullable), s === void 0 && (s = t[0].metadata)), new tt(`${e}`, i, r, s)
     }
     get typeId() {
         return this.type.typeId
     }
     get[Symbol.toStringTag]() {
         return "Field"
     }
@@ -5112,58 +5112,58 @@
     clone(...t) {
         let [e, i, r, s] = t;
         return !t[0] || typeof t[0] != "object" ? [e = this.name, i = this.type, r = this.nullable, s = this.metadata] = t : {
             name: e = this.name,
             type: i = this.type,
             nullable: r = this.nullable,
             metadata: s = this.metadata
-        } = t[0], X.new(e, i, r, s)
+        } = t[0], tt.new(e, i, r, s)
     }
 }
-X.prototype.type = null;
-X.prototype.name = null;
-X.prototype.nullable = null;
-X.prototype.metadata = null;
+tt.prototype.type = null;
+tt.prototype.name = null;
+tt.prototype.nullable = null;
+tt.prototype.metadata = null;
 
-function Qn(n, t) {
+function ei(n, t) {
     return new Map([...n || new Map, ...t || new Map])
 }
 
-function Ar(n, t = new Map) {
+function Nr(n, t = new Map) {
     for (let e = -1, i = n.length; ++e < i;) {
         const s = n[e].type;
-        if (S.isDictionary(s)) {
+        if (I.isDictionary(s)) {
             if (!t.has(s.id)) t.set(s.id, s.dictionary);
             else if (t.get(s.id) !== s.dictionary) throw new Error("Cannot create Schema containing two different dictionaries with the same Id")
         }
-        s.children && s.children.length > 0 && Ar(s.children, t)
+        s.children && s.children.length > 0 && Nr(s.children, t)
     }
     return t
 }
-var Cs = he,
-    Yu = ja,
-    Gu = hn;
+var ks = me,
+    Yu = za,
+    Gu = yn;
 class Vn {
     constructor(t, e = Nt.V4, i, r) {
         this.schema = t, this.version = e, i && (this._recordBatches = i), r && (this._dictionaryBatches = r)
     }
     static decode(t) {
         t = new Gu(U(t));
         const e = Dt.getRootAsFooter(t),
-            i = j.decode(e.schema());
+            i = W.decode(e.schema());
         return new Hu(i, e)
     }
     static encode(t) {
         const e = new Yu,
-            i = j.encode(e, t.schema);
+            i = W.encode(e, t.schema);
         Dt.startRecordBatchesVector(e, t.numRecordBatches);
-        for (const o of [...t.recordBatches()].slice().reverse()) Ae.encode(e, o);
+        for (const o of [...t.recordBatches()].slice().reverse()) xe.encode(e, o);
         const r = e.endVector();
         Dt.startDictionariesVector(e, t.numDictionaries);
-        for (const o of [...t.dictionaryBatches()].slice().reverse()) Ae.encode(e, o);
+        for (const o of [...t.dictionaryBatches()].slice().reverse()) xe.encode(e, o);
         const s = e.endVector();
         return Dt.startFooter(e), Dt.addSchema(e, i), Dt.addVersion(e, Nt.V4), Dt.addRecordBatches(e, r), Dt.addDictionaries(e, s), Dt.finishFooterBuffer(e, Dt.endFooter(e)), e.asUint8Array()
     }
     get numRecordBatches() {
         return this._recordBatches.length
     }
     get numDictionaries() {
@@ -5189,59 +5189,59 @@
     }
     get numDictionaries() {
         return this._footer.dictionariesLength()
     }
     getRecordBatch(t) {
         if (t >= 0 && t < this.numRecordBatches) {
             const e = this._footer.recordBatches(t);
-            if (e) return Ae.decode(e)
+            if (e) return xe.decode(e)
         }
         return null
     }
     getDictionaryBatch(t) {
         if (t >= 0 && t < this.numDictionaries) {
             const e = this._footer.dictionaries(t);
-            if (e) return Ae.decode(e)
+            if (e) return xe.decode(e)
         }
         return null
     }
 }
-class Ae {
+class xe {
     constructor(t, e, i) {
         this.metaDataLength = t, this.offset = typeof i == "number" ? i : i.low, this.bodyLength = typeof e == "number" ? e : e.low
     }
     static decode(t) {
-        return new Ae(t.metaDataLength(), t.bodyLength(), t.offset())
+        return new xe(t.metaDataLength(), t.bodyLength(), t.offset())
     }
     static encode(t, e) {
         const {
             metaDataLength: i
-        } = e, r = new Cs(e.offset, 0), s = new Cs(e.bodyLength, 0);
-        return Br.createBlock(t, r, i, s)
+        } = e, r = new ks(e.offset, 0), s = new ks(e.bodyLength, 0);
+        return Ar.createBlock(t, r, i, s)
     }
 }
-const tt = Object.freeze({
+const it = Object.freeze({
     done: !0,
     value: void 0
 });
-class ks {
+class Us {
     constructor(t) {
         this._json = t
     }
     get schema() {
         return this._json.schema
     }
     get batches() {
         return this._json.batches || []
     }
     get dictionaries() {
         return this._json.dictionaries || []
     }
 }
-class ss {
+class ls {
     tee() {
         return this._getDOMStream().tee()
     }
     pipe(t, e) {
         return this._getNodeStream().pipe(t, e)
     }
     pipeTo(t, e) {
@@ -5253,23 +5253,23 @@
     _getDOMStream() {
         return this._DOMStream || (this._DOMStream = this.toDOMStream())
     }
     _getNodeStream() {
         return this._nodeStream || (this._nodeStream = this.toNodeStream())
     }
 }
-class qu extends ss {
+class qu extends ls {
     constructor() {
         super(), this._values = [], this.resolvers = [], this._closedPromise = new Promise(t => this._closedPromiseResolve = t)
     }
     get closed() {
         return this._closedPromise
     }
     cancel(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             yield this.return(t)
         })
     }
     write(t) {
         this._ensureOpen() && (this.resolvers.length <= 0 ? this._values.push(t) : this.resolvers.shift().resolve({
             done: !1,
             value: t
@@ -5284,43 +5284,43 @@
         }))
     }
     close() {
         if (this._closedPromiseResolve) {
             const {
                 resolvers: t
             } = this;
-            for (; t.length > 0;) t.shift().resolve(tt);
+            for (; t.length > 0;) t.shift().resolve(it);
             this._closedPromiseResolve(), this._closedPromiseResolve = void 0
         }
     } [Symbol.asyncIterator]() {
         return this
     }
     toDOMStream(t) {
-        return Ct.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
+        return kt.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
     }
     toNodeStream(t) {
-        return Ct.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
+        return kt.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
     }
     throw (t) {
-        return w(this, void 0, void 0, function*() {
-            return yield this.abort(t), tt
+        return S(this, void 0, void 0, function*() {
+            return yield this.abort(t), it
         })
     }
     return (t) {
-        return w(this, void 0, void 0, function*() {
-            return yield this.close(), tt
+        return S(this, void 0, void 0, function*() {
+            return yield this.close(), it
         })
     }
     read(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return (yield this.next(t, "read")).value
         })
     }
     peek(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return (yield this.next(t, "peek")).value
         })
     }
     next(...t) {
         return this._values.length > 0 ? Promise.resolve({
             done: !1,
             value: this._values.shift()
@@ -5328,56 +5328,56 @@
             done: !0,
             value: this._error.error
         }) : this._closedPromiseResolve ? new Promise((e, i) => {
             this.resolvers.push({
                 resolve: e,
                 reject: i
             })
-        }) : Promise.resolve(tt)
+        }) : Promise.resolve(it)
     }
     _ensureOpen() {
         if (this._closedPromiseResolve) return !0;
         throw new Error("AsyncQueue is closed")
     }
 }
-class oi extends qu {
+class li extends qu {
     write(t) {
         if ((t = U(t)).byteLength > 0) return super.write(t)
     }
     toString(t = !1) {
-        return t ? gr(this.toUint8Array(!0)) : this.toUint8Array(!1).then(gr)
+        return t ? Sr(this.toUint8Array(!0)) : this.toUint8Array(!1).then(Sr)
     }
     toUint8Array(t = !1) {
-        return t ? ne(this._values)[0] : w(this, void 0, void 0, function*() {
+        return t ? se(this._values)[0] : S(this, void 0, void 0, function*() {
             var e, i;
             const r = [];
             let s = 0;
             try {
-                for (var o = je(this), a; a = yield o.next(), !a.done;) {
+                for (var o = Ye(this), a; a = yield o.next(), !a.done;) {
                     const l = a.value;
                     r.push(l), s += l.byteLength
                 }
             } catch (l) {
                 e = {
                     error: l
                 }
             } finally {
                 try {
                     a && !a.done && (i = o.return) && (yield i.call(o))
                 } finally {
                     if (e) throw e.error
                 }
             }
-            return ne(r, s)[0]
+            return se(r, s)[0]
         })
     }
 }
-class Ni {
+class Mi {
     constructor(t) {
-        t && (this.source = new Ju(Ct.fromIterable(t)))
+        t && (this.source = new Ju(kt.fromIterable(t)))
     } [Symbol.iterator]() {
         return this
     }
     next(t) {
         return this.source.next(t)
     }
     throw (t) {
@@ -5389,17 +5389,17 @@
     peek(t) {
         return this.source.peek(t)
     }
     read(t) {
         return this.source.read(t)
     }
 }
-class mn {
+class gn {
     constructor(t) {
-        t instanceof mn ? this.source = t.source : t instanceof oi ? this.source = new Ee(Ct.fromAsyncIterable(t)) : Oo(t) ? this.source = new Ee(Ct.fromNodeStream(t)) : Yr(t) ? this.source = new Ee(Ct.fromDOMStream(t)) : Bo(t) ? this.source = new Ee(Ct.fromDOMStream(t.body)) : Gn(t) ? this.source = new Ee(Ct.fromIterable(t)) : Ie(t) ? this.source = new Ee(Ct.fromAsyncIterable(t)) : gn(t) && (this.source = new Ee(Ct.fromAsyncIterable(t)))
+        t instanceof gn ? this.source = t.source : t instanceof li ? this.source = new ke(kt.fromAsyncIterable(t)) : Fo(t) ? this.source = new ke(kt.fromNodeStream(t)) : qr(t) ? this.source = new ke(kt.fromDOMStream(t)) : Oo(t) ? this.source = new ke(kt.fromDOMStream(t.body)) : Gn(t) ? this.source = new ke(kt.fromIterable(t)) : Ae(t) ? this.source = new ke(kt.fromAsyncIterable(t)) : In(t) && (this.source = new ke(kt.fromAsyncIterable(t)))
     } [Symbol.asyncIterator]() {
         return this
     }
     next(t) {
         return this.source.next(t)
     }
     throw (t) {
@@ -5437,64 +5437,64 @@
     next(t, e = "read") {
         return this.source.next({
             cmd: e,
             size: t
         })
     }
     throw (t) {
-        return Object.create(this.source.throw && this.source.throw(t) || tt)
+        return Object.create(this.source.throw && this.source.throw(t) || it)
     }
     return (t) {
-        return Object.create(this.source.return && this.source.return(t) || tt)
+        return Object.create(this.source.return && this.source.return(t) || it)
     }
 }
-class Ee {
+class ke {
     constructor(t) {
         this.source = t, this._closedPromise = new Promise(e => this._closedPromiseResolve = e)
     }
     cancel(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             yield this.return(t)
         })
     }
     get closed() {
         return this._closedPromise
     }
     read(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return (yield this.next(t, "read")).value
         })
     }
     peek(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return (yield this.next(t, "peek")).value
         })
     }
     next(t, e = "read") {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return yield this.source.next({
                 cmd: e,
                 size: t
             })
         })
     }
     throw (t) {
-        return w(this, void 0, void 0, function*() {
-            const e = this.source.throw && (yield this.source.throw(t)) || tt;
+        return S(this, void 0, void 0, function*() {
+            const e = this.source.throw && (yield this.source.throw(t)) || it;
             return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(e)
         })
     }
     return (t) {
-        return w(this, void 0, void 0, function*() {
-            const e = this.source.return && (yield this.source.return(t)) || tt;
+        return S(this, void 0, void 0, function*() {
+            const e = this.source.return && (yield this.source.return(t)) || it;
             return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(e)
         })
     }
 }
-class Us extends Ni {
+class $s extends Mi {
     constructor(t, e) {
         super(), this.position = 0, this.buffer = U(t), this.size = typeof e > "u" ? this.buffer.byteLength : e
     }
     readInt32(t) {
         const {
             buffer: e,
             byteOffset: i
@@ -5529,36 +5529,36 @@
     return (t) {
         return this.close(), {
             done: !0,
             value: t
         }
     }
 }
-class Mi extends mn {
+class Li extends gn {
     constructor(t, e) {
-        super(), this.position = 0, this._handle = t, typeof e == "number" ? this.size = e : this._pending = w(this, void 0, void 0, function*() {
+        super(), this.position = 0, this._handle = t, typeof e == "number" ? this.size = e : this._pending = S(this, void 0, void 0, function*() {
             this.size = (yield t.stat()).size, delete this._pending
         })
     }
     readInt32(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const {
                 buffer: e,
                 byteOffset: i
             } = yield this.readAt(t, 4);
             return new DataView(e, i).getInt32(0, !0)
         })
     }
     seek(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return this._pending && (yield this._pending), this.position = Math.min(t, this.size), t < this.size
         })
     }
     read(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             this._pending && (yield this._pending);
             const {
                 _handle: e,
                 size: i,
                 position: r
             } = this;
             if (e && r < i) {
@@ -5574,59 +5574,59 @@
                 } = yield e.read(c, o, c.byteLength - o, s));
                 return c
             }
             return null
         })
     }
     readAt(t, e) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             this._pending && (yield this._pending);
             const {
                 _handle: i,
                 size: r
             } = this;
             if (i && t + e < r) {
                 const s = Math.min(r, t + e),
                     o = new Uint8Array(s - t);
                 return (yield i.read(o, 0, e, t)).buffer
             }
             return new Uint8Array(e)
         })
     }
     close() {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const t = this._handle;
             this._handle = null, t && (yield t.close())
         })
     }
     throw (t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return yield this.close(), {
                 done: !0,
                 value: t
             }
         })
     }
     return (t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return yield this.close(), {
                 done: !0,
                 value: t
             }
         })
     }
 }
 const Ku = 65536;
 
-function nn(n) {
+function sn(n) {
     return n < 0 && (n = 4294967295 + n + 1), `0x${n.toString(16)}`
 }
-const vn = 8,
-    os = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8];
-class Wa {
+const _n = 8,
+    cs = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8];
+class Ya {
     constructor(t) {
         this.buffer = t
     }
     high() {
         return this.buffer[1]
     }
     low() {
@@ -5650,54 +5650,54 @@
     equals(t) {
         return this.buffer[1] === t.buffer[1] && this.buffer[0] == t.buffer[0]
     }
     greaterThan(t) {
         return t.lessThan(this)
     }
     hex() {
-        return `${nn(this.buffer[1])} ${nn(this.buffer[0])}`
+        return `${sn(this.buffer[1])} ${sn(this.buffer[0])}`
     }
 }
-class z extends Wa {
+class Y extends Ya {
     times(t) {
         return this._times(t), this
     }
     plus(t) {
         return this._plus(t), this
     }
     static from(t, e = new Uint32Array(2)) {
-        return z.fromString(typeof t == "string" ? t : t.toString(), e)
+        return Y.fromString(typeof t == "string" ? t : t.toString(), e)
     }
     static fromNumber(t, e = new Uint32Array(2)) {
-        return z.fromString(t.toString(), e)
+        return Y.fromString(t.toString(), e)
     }
     static fromString(t, e = new Uint32Array(2)) {
         const i = t.length,
-            r = new z(e);
+            r = new Y(e);
         for (let s = 0; s < i;) {
-            const o = vn < i - s ? vn : i - s,
-                a = new z(new Uint32Array([Number.parseInt(t.slice(s, s + o), 10), 0])),
-                l = new z(new Uint32Array([os[o], 0]));
+            const o = _n < i - s ? _n : i - s,
+                a = new Y(new Uint32Array([Number.parseInt(t.slice(s, s + o), 10), 0])),
+                l = new Y(new Uint32Array([cs[o], 0]));
             r.times(l), r.plus(a), s += o
         }
         return r
     }
     static convertArray(t) {
         const e = new Uint32Array(t.length * 2);
-        for (let i = -1, r = t.length; ++i < r;) z.from(t[i], new Uint32Array(e.buffer, e.byteOffset + 2 * i * 4, 2));
+        for (let i = -1, r = t.length; ++i < r;) Y.from(t[i], new Uint32Array(e.buffer, e.byteOffset + 2 * i * 4, 2));
         return e
     }
     static multiply(t, e) {
-        return new z(new Uint32Array(t.buffer)).times(e)
+        return new Y(new Uint32Array(t.buffer)).times(e)
     }
     static add(t, e) {
-        return new z(new Uint32Array(t.buffer)).plus(e)
+        return new Y(new Uint32Array(t.buffer)).plus(e)
     }
 }
-class gt extends Wa {
+class _t extends Ya {
     negate() {
         return this.buffer[0] = ~this.buffer[0] + 1, this.buffer[1] = ~this.buffer[1], this.buffer[0] == 0 && ++this.buffer[1], this
     }
     times(t) {
         return this._times(t), this
     }
     plus(t) {
@@ -5705,113 +5705,113 @@
     }
     lessThan(t) {
         const e = this.buffer[1] << 0,
             i = t.buffer[1] << 0;
         return e < i || e === i && this.buffer[0] < t.buffer[0]
     }
     static from(t, e = new Uint32Array(2)) {
-        return gt.fromString(typeof t == "string" ? t : t.toString(), e)
+        return _t.fromString(typeof t == "string" ? t : t.toString(), e)
     }
     static fromNumber(t, e = new Uint32Array(2)) {
-        return gt.fromString(t.toString(), e)
+        return _t.fromString(t.toString(), e)
     }
     static fromString(t, e = new Uint32Array(2)) {
         const i = t.startsWith("-"),
             r = t.length,
-            s = new gt(e);
+            s = new _t(e);
         for (let o = i ? 1 : 0; o < r;) {
-            const a = vn < r - o ? vn : r - o,
-                l = new gt(new Uint32Array([Number.parseInt(t.slice(o, o + a), 10), 0])),
-                c = new gt(new Uint32Array([os[a], 0]));
+            const a = _n < r - o ? _n : r - o,
+                l = new _t(new Uint32Array([Number.parseInt(t.slice(o, o + a), 10), 0])),
+                c = new _t(new Uint32Array([cs[a], 0]));
             s.times(c), s.plus(l), o += a
         }
         return i ? s.negate() : s
     }
     static convertArray(t) {
         const e = new Uint32Array(t.length * 2);
-        for (let i = -1, r = t.length; ++i < r;) gt.from(t[i], new Uint32Array(e.buffer, e.byteOffset + 2 * i * 4, 2));
+        for (let i = -1, r = t.length; ++i < r;) _t.from(t[i], new Uint32Array(e.buffer, e.byteOffset + 2 * i * 4, 2));
         return e
     }
     static multiply(t, e) {
-        return new gt(new Uint32Array(t.buffer)).times(e)
+        return new _t(new Uint32Array(t.buffer)).times(e)
     }
     static add(t, e) {
-        return new gt(new Uint32Array(t.buffer)).plus(e)
+        return new _t(new Uint32Array(t.buffer)).plus(e)
     }
 }
-class Gt {
+class qt {
     constructor(t) {
         this.buffer = t
     }
     high() {
-        return new gt(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
+        return new _t(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
     }
     low() {
-        return new gt(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset, 2))
+        return new _t(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset, 2))
     }
     negate() {
         return this.buffer[0] = ~this.buffer[0] + 1, this.buffer[1] = ~this.buffer[1], this.buffer[2] = ~this.buffer[2], this.buffer[3] = ~this.buffer[3], this.buffer[0] == 0 && ++this.buffer[1], this.buffer[1] == 0 && ++this.buffer[2], this.buffer[2] == 0 && ++this.buffer[3], this
     }
     times(t) {
-        const e = new z(new Uint32Array([this.buffer[3], 0])),
-            i = new z(new Uint32Array([this.buffer[2], 0])),
-            r = new z(new Uint32Array([this.buffer[1], 0])),
-            s = new z(new Uint32Array([this.buffer[0], 0])),
-            o = new z(new Uint32Array([t.buffer[3], 0])),
-            a = new z(new Uint32Array([t.buffer[2], 0])),
-            l = new z(new Uint32Array([t.buffer[1], 0])),
-            c = new z(new Uint32Array([t.buffer[0], 0]));
-        let d = z.multiply(s, c);
+        const e = new Y(new Uint32Array([this.buffer[3], 0])),
+            i = new Y(new Uint32Array([this.buffer[2], 0])),
+            r = new Y(new Uint32Array([this.buffer[1], 0])),
+            s = new Y(new Uint32Array([this.buffer[0], 0])),
+            o = new Y(new Uint32Array([t.buffer[3], 0])),
+            a = new Y(new Uint32Array([t.buffer[2], 0])),
+            l = new Y(new Uint32Array([t.buffer[1], 0])),
+            c = new Y(new Uint32Array([t.buffer[0], 0]));
+        let d = Y.multiply(s, c);
         this.buffer[0] = d.low();
-        const h = new z(new Uint32Array([d.high(), 0]));
-        return d = z.multiply(r, c), h.plus(d), d = z.multiply(s, l), h.plus(d), this.buffer[1] = h.low(), this.buffer[3] = h.lessThan(d) ? 1 : 0, this.buffer[2] = h.high(), new z(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(z.multiply(i, c)).plus(z.multiply(r, l)).plus(z.multiply(s, a)), this.buffer[3] += z.multiply(e, c).plus(z.multiply(i, l)).plus(z.multiply(r, a)).plus(z.multiply(s, o)).low(), this
+        const h = new Y(new Uint32Array([d.high(), 0]));
+        return d = Y.multiply(r, c), h.plus(d), d = Y.multiply(s, l), h.plus(d), this.buffer[1] = h.low(), this.buffer[3] = h.lessThan(d) ? 1 : 0, this.buffer[2] = h.high(), new Y(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(Y.multiply(i, c)).plus(Y.multiply(r, l)).plus(Y.multiply(s, a)), this.buffer[3] += Y.multiply(e, c).plus(Y.multiply(i, l)).plus(Y.multiply(r, a)).plus(Y.multiply(s, o)).low(), this
     }
     plus(t) {
         const e = new Uint32Array(4);
         return e[3] = this.buffer[3] + t.buffer[3] >>> 0, e[2] = this.buffer[2] + t.buffer[2] >>> 0, e[1] = this.buffer[1] + t.buffer[1] >>> 0, e[0] = this.buffer[0] + t.buffer[0] >>> 0, e[0] < this.buffer[0] >>> 0 && ++e[1], e[1] < this.buffer[1] >>> 0 && ++e[2], e[2] < this.buffer[2] >>> 0 && ++e[3], this.buffer[3] = e[3], this.buffer[2] = e[2], this.buffer[1] = e[1], this.buffer[0] = e[0], this
     }
     hex() {
-        return `${nn(this.buffer[3])} ${nn(this.buffer[2])} ${nn(this.buffer[1])} ${nn(this.buffer[0])}`
+        return `${sn(this.buffer[3])} ${sn(this.buffer[2])} ${sn(this.buffer[1])} ${sn(this.buffer[0])}`
     }
     static multiply(t, e) {
-        return new Gt(new Uint32Array(t.buffer)).times(e)
+        return new qt(new Uint32Array(t.buffer)).times(e)
     }
     static add(t, e) {
-        return new Gt(new Uint32Array(t.buffer)).plus(e)
+        return new qt(new Uint32Array(t.buffer)).plus(e)
     }
     static from(t, e = new Uint32Array(4)) {
-        return Gt.fromString(typeof t == "string" ? t : t.toString(), e)
+        return qt.fromString(typeof t == "string" ? t : t.toString(), e)
     }
     static fromNumber(t, e = new Uint32Array(4)) {
-        return Gt.fromString(t.toString(), e)
+        return qt.fromString(t.toString(), e)
     }
     static fromString(t, e = new Uint32Array(4)) {
         const i = t.startsWith("-"),
             r = t.length,
-            s = new Gt(e);
+            s = new qt(e);
         for (let o = i ? 1 : 0; o < r;) {
-            const a = vn < r - o ? vn : r - o,
-                l = new Gt(new Uint32Array([Number.parseInt(t.slice(o, o + a), 10), 0, 0, 0])),
-                c = new Gt(new Uint32Array([os[a], 0, 0, 0]));
+            const a = _n < r - o ? _n : r - o,
+                l = new qt(new Uint32Array([Number.parseInt(t.slice(o, o + a), 10), 0, 0, 0])),
+                c = new qt(new Uint32Array([cs[a], 0, 0, 0]));
             s.times(c), s.plus(l), o += a
         }
         return i ? s.negate() : s
     }
     static convertArray(t) {
         const e = new Uint32Array(t.length * 4);
-        for (let i = -1, r = t.length; ++i < r;) Gt.from(t[i], new Uint32Array(e.buffer, e.byteOffset + 4 * 4 * i, 4));
+        for (let i = -1, r = t.length; ++i < r;) qt.from(t[i], new Uint32Array(e.buffer, e.byteOffset + 4 * 4 * i, 4));
         return e
     }
 }
-class Ya extends R {
+class Ga extends R {
     constructor(t, e, i, r) {
         super(), this.nodesIndex = -1, this.buffersIndex = -1, this.bytes = t, this.nodes = e, this.buffers = i, this.dictionaries = r
     }
     visit(t) {
-        return super.visit(t instanceof X ? t.type : t)
+        return super.visit(t instanceof tt ? t.type : t)
     }
     visitNull(t, {
         length: e
     } = this.nextFieldNode()) {
         return E({
             type: t,
             length: e
@@ -5961,15 +5961,15 @@
             length: e,
             nullCount: i,
             nullBitmap: this.readNullBitmap(t, i),
             children: this.visitMany(t.children)
         })
     }
     visitUnion(t) {
-        return t.mode === xt.Sparse ? this.visitSparseUnion(t) : this.visitDenseUnion(t)
+        return t.mode === Mt.Sparse ? this.visitSparseUnion(t) : this.visitDenseUnion(t)
     }
     visitDenseUnion(t, {
         length: e,
         nullCount: i
     } = this.nextFieldNode()) {
         return E({
             type: t,
@@ -6065,50 +6065,50 @@
     } = this.nextBufferRange()) {
         return this.bytes.subarray(i, i + e)
     }
     readDictionary(t) {
         return this.dictionaries.get(t.id)
     }
 }
-class Zu extends Ya {
+class Zu extends Ga {
     constructor(t, e, i, r) {
         super(new Uint8Array(0), e, i, r), this.sources = t
     }
     readNullBitmap(t, e, {
         offset: i
     } = this.nextBufferRange()) {
-        return e <= 0 ? new Uint8Array(0) : Si(this.sources[i])
+        return e <= 0 ? new Uint8Array(0) : Bi(this.sources[i])
     }
     readOffsets(t, {
         offset: e
     } = this.nextBufferRange()) {
-        return q(Uint8Array, q(Int32Array, this.sources[e]))
+        return K(Uint8Array, K(Int32Array, this.sources[e]))
     }
     readTypeIds(t, {
         offset: e
     } = this.nextBufferRange()) {
-        return q(Uint8Array, q(t.ArrayType, this.sources[e]))
+        return K(Uint8Array, K(t.ArrayType, this.sources[e]))
     }
     readData(t, {
         offset: e
     } = this.nextBufferRange()) {
         const {
             sources: i
         } = this;
-        return S.isTimestamp(t) || (S.isInt(t) || S.isTime(t)) && t.bitWidth === 64 || S.isDate(t) && t.unit === ye.MILLISECOND ? q(Uint8Array, gt.convertArray(i[e])) : S.isDecimal(t) ? q(Uint8Array, Gt.convertArray(i[e])) : S.isBinary(t) || S.isFixedSizeBinary(t) ? Xu(i[e]) : S.isBool(t) ? Si(i[e]) : S.isUtf8(t) ? Wr(i[e].join("")) : q(Uint8Array, q(t.ArrayType, i[e].map(r => +r)))
+        return I.isTimestamp(t) || (I.isInt(t) || I.isTime(t)) && t.bitWidth === 64 || I.isDate(t) && t.unit === be.MILLISECOND ? K(Uint8Array, _t.convertArray(i[e])) : I.isDecimal(t) ? K(Uint8Array, qt.convertArray(i[e])) : I.isBinary(t) || I.isFixedSizeBinary(t) ? Xu(i[e]) : I.isBool(t) ? Bi(i[e]) : I.isUtf8(t) ? Hr(i[e].join("")) : K(Uint8Array, K(t.ArrayType, i[e].map(r => +r)))
     }
 }
 
 function Xu(n) {
     const t = n.join(""),
         e = new Uint8Array(t.length / 2);
     for (let i = 0; i < t.length; i += 2) e[i >> 1] = Number.parseInt(t.slice(i, i + 2), 16);
     return e
 }
-class F extends R {
+class A extends R {
     compareSchemas(t, e) {
         return t === e || e instanceof t.constructor && this.compareManyFields(t.fields, e.fields)
     }
     compareManyFields(t, e) {
         return t === e || Array.isArray(t) && Array.isArray(e) && t.length === e.length && t.every((i, r) => this.compareFields(i, e[r]))
     }
     compareFields(t, e) {
@@ -6120,115 +6120,115 @@
     return t instanceof n.constructor
 }
 
 function Hn(n, t) {
     return n === t || At(n, t)
 }
 
-function be(n, t) {
+function we(n, t) {
     return n === t || At(n, t) && n.bitWidth === t.bitWidth && n.isSigned === t.isSigned
 }
 
-function er(n, t) {
+function ir(n, t) {
     return n === t || At(n, t) && n.precision === t.precision
 }
 
 function Qu(n, t) {
     return n === t || At(n, t) && n.byteWidth === t.byteWidth
 }
 
-function as(n, t) {
+function us(n, t) {
     return n === t || At(n, t) && n.unit === t.unit
 }
 
 function qn(n, t) {
     return n === t || At(n, t) && n.unit === t.unit && n.timezone === t.timezone
 }
 
 function Jn(n, t) {
     return n === t || At(n, t) && n.unit === t.unit && n.bitWidth === t.bitWidth
 }
 
 function td(n, t) {
-    return n === t || At(n, t) && n.children.length === t.children.length && De.compareManyFields(n.children, t.children)
+    return n === t || At(n, t) && n.children.length === t.children.length && Me.compareManyFields(n.children, t.children)
 }
 
 function ed(n, t) {
-    return n === t || At(n, t) && n.children.length === t.children.length && De.compareManyFields(n.children, t.children)
+    return n === t || At(n, t) && n.children.length === t.children.length && Me.compareManyFields(n.children, t.children)
 }
 
-function ls(n, t) {
-    return n === t || At(n, t) && n.mode === t.mode && n.typeIds.every((e, i) => e === t.typeIds[i]) && De.compareManyFields(n.children, t.children)
+function ds(n, t) {
+    return n === t || At(n, t) && n.mode === t.mode && n.typeIds.every((e, i) => e === t.typeIds[i]) && Me.compareManyFields(n.children, t.children)
 }
 
 function nd(n, t) {
-    return n === t || At(n, t) && n.id === t.id && n.isOrdered === t.isOrdered && De.visit(n.indices, t.indices) && De.visit(n.dictionary, t.dictionary)
+    return n === t || At(n, t) && n.id === t.id && n.isOrdered === t.isOrdered && Me.visit(n.indices, t.indices) && Me.visit(n.dictionary, t.dictionary)
 }
 
-function cs(n, t) {
+function hs(n, t) {
     return n === t || At(n, t) && n.unit === t.unit
 }
 
 function id(n, t) {
-    return n === t || At(n, t) && n.listSize === t.listSize && n.children.length === t.children.length && De.compareManyFields(n.children, t.children)
+    return n === t || At(n, t) && n.listSize === t.listSize && n.children.length === t.children.length && Me.compareManyFields(n.children, t.children)
 }
 
 function rd(n, t) {
-    return n === t || At(n, t) && n.keysSorted === t.keysSorted && n.children.length === t.children.length && De.compareManyFields(n.children, t.children)
+    return n === t || At(n, t) && n.keysSorted === t.keysSorted && n.children.length === t.children.length && Me.compareManyFields(n.children, t.children)
 }
-F.prototype.visitNull = Hn;
-F.prototype.visitBool = Hn;
-F.prototype.visitInt = be;
-F.prototype.visitInt8 = be;
-F.prototype.visitInt16 = be;
-F.prototype.visitInt32 = be;
-F.prototype.visitInt64 = be;
-F.prototype.visitUint8 = be;
-F.prototype.visitUint16 = be;
-F.prototype.visitUint32 = be;
-F.prototype.visitUint64 = be;
-F.prototype.visitFloat = er;
-F.prototype.visitFloat16 = er;
-F.prototype.visitFloat32 = er;
-F.prototype.visitFloat64 = er;
-F.prototype.visitUtf8 = Hn;
-F.prototype.visitBinary = Hn;
-F.prototype.visitFixedSizeBinary = Qu;
-F.prototype.visitDate = as;
-F.prototype.visitDateDay = as;
-F.prototype.visitDateMillisecond = as;
-F.prototype.visitTimestamp = qn;
-F.prototype.visitTimestampSecond = qn;
-F.prototype.visitTimestampMillisecond = qn;
-F.prototype.visitTimestampMicrosecond = qn;
-F.prototype.visitTimestampNanosecond = qn;
-F.prototype.visitTime = Jn;
-F.prototype.visitTimeSecond = Jn;
-F.prototype.visitTimeMillisecond = Jn;
-F.prototype.visitTimeMicrosecond = Jn;
-F.prototype.visitTimeNanosecond = Jn;
-F.prototype.visitDecimal = Hn;
-F.prototype.visitList = td;
-F.prototype.visitStruct = ed;
-F.prototype.visitUnion = ls;
-F.prototype.visitDenseUnion = ls;
-F.prototype.visitSparseUnion = ls;
-F.prototype.visitDictionary = nd;
-F.prototype.visitInterval = cs;
-F.prototype.visitIntervalDayTime = cs;
-F.prototype.visitIntervalYearMonth = cs;
-F.prototype.visitFixedSizeList = id;
-F.prototype.visitMap = rd;
-const De = new F;
+A.prototype.visitNull = Hn;
+A.prototype.visitBool = Hn;
+A.prototype.visitInt = we;
+A.prototype.visitInt8 = we;
+A.prototype.visitInt16 = we;
+A.prototype.visitInt32 = we;
+A.prototype.visitInt64 = we;
+A.prototype.visitUint8 = we;
+A.prototype.visitUint16 = we;
+A.prototype.visitUint32 = we;
+A.prototype.visitUint64 = we;
+A.prototype.visitFloat = ir;
+A.prototype.visitFloat16 = ir;
+A.prototype.visitFloat32 = ir;
+A.prototype.visitFloat64 = ir;
+A.prototype.visitUtf8 = Hn;
+A.prototype.visitBinary = Hn;
+A.prototype.visitFixedSizeBinary = Qu;
+A.prototype.visitDate = us;
+A.prototype.visitDateDay = us;
+A.prototype.visitDateMillisecond = us;
+A.prototype.visitTimestamp = qn;
+A.prototype.visitTimestampSecond = qn;
+A.prototype.visitTimestampMillisecond = qn;
+A.prototype.visitTimestampMicrosecond = qn;
+A.prototype.visitTimestampNanosecond = qn;
+A.prototype.visitTime = Jn;
+A.prototype.visitTimeSecond = Jn;
+A.prototype.visitTimeMillisecond = Jn;
+A.prototype.visitTimeMicrosecond = Jn;
+A.prototype.visitTimeNanosecond = Jn;
+A.prototype.visitDecimal = Hn;
+A.prototype.visitList = td;
+A.prototype.visitStruct = ed;
+A.prototype.visitUnion = ds;
+A.prototype.visitDenseUnion = ds;
+A.prototype.visitSparseUnion = ds;
+A.prototype.visitDictionary = nd;
+A.prototype.visitInterval = hs;
+A.prototype.visitIntervalDayTime = hs;
+A.prototype.visitIntervalYearMonth = hs;
+A.prototype.visitFixedSizeList = id;
+A.prototype.visitMap = rd;
+const Me = new A;
 
-function Dr(n, t) {
-    return De.compareSchemas(n, t)
+function xr(n, t) {
+    return Me.compareSchemas(n, t)
 }
 
-function hr(n, t) {
+function pr(n, t) {
     return sd(n, t.map(e => e.data.concat()))
 }
 
 function sd(n, t) {
     const e = [...n.fields],
         i = [],
         r = {
@@ -6238,21 +6238,21 @@
         o = 0,
         a = -1;
     const l = t.length;
     let c, d = [];
     for (; r.numBatches-- > 0;) {
         for (o = Number.POSITIVE_INFINITY, a = -1; ++a < l;) d[a] = c = t[a].shift(), o = Math.min(o, c ? c.length : o);
         Number.isFinite(o) && (d = od(e, o, d, t, r), o > 0 && (i[s++] = E({
-            type: new yt(e),
+            type: new mt(e),
             length: o,
             nullCount: 0,
             children: d.slice()
         })))
     }
-    return [n = n.assign(e), i.map(h => new St(n, h))]
+    return [n = n.assign(e), i.map(h => new It(n, h))]
 }
 
 function od(n, t, e, i, r) {
     var s;
     const o = (t + 63 & -64) >> 3;
     for (let a = -1, l = i.length; ++a < l;) {
         const c = e[a],
@@ -6268,46 +6268,46 @@
                 nullCount: t,
                 nullBitmap: new Uint8Array(o)
             })
         }
     }
     return e
 }
-var Ga;
-class pt {
+var Ha;
+class yt {
     constructor(...t) {
         var e, i;
-        if (t.length === 0) return this.batches = [], this.schema = new j([]), this._offsets = [0], this;
+        if (t.length === 0) return this.batches = [], this.schema = new W([]), this._offsets = [0], this;
         let r, s;
-        t[0] instanceof j && (r = t.shift()), t[t.length - 1] instanceof Uint32Array && (s = t.pop());
+        t[0] instanceof W && (r = t.shift()), t[t.length - 1] instanceof Uint32Array && (s = t.pop());
         const o = l => {
                 if (l) {
-                    if (l instanceof St) return [l];
-                    if (l instanceof pt) return l.batches;
-                    if (l instanceof K) {
-                        if (l.type instanceof yt) return [new St(new j(l.type.children), l)]
+                    if (l instanceof It) return [l];
+                    if (l instanceof yt) return l.batches;
+                    if (l instanceof X) {
+                        if (l.type instanceof mt) return [new It(new W(l.type.children), l)]
                     } else {
                         if (Array.isArray(l)) return l.flatMap(c => o(c));
                         if (typeof l[Symbol.iterator] == "function") return [...l].flatMap(c => o(c));
                         if (typeof l == "object") {
                             const c = Object.keys(l),
-                                d = c.map(_ => new P([l[_]])),
-                                h = new j(c.map((_, G) => new X(String(_), d[G].type))),
-                                [, y] = hr(h, d);
-                            return y.length === 0 ? [new St(l)] : y
+                                d = c.map(_ => new z([l[_]])),
+                                h = new W(c.map((_, V) => new tt(String(_), d[V].type))),
+                                [, y] = pr(h, d);
+                            return y.length === 0 ? [new It(l)] : y
                         }
                     }
                 }
                 return []
             },
             a = t.flatMap(l => o(l));
-        if (r = (i = r ?? ((e = a[0]) === null || e === void 0 ? void 0 : e.schema)) !== null && i !== void 0 ? i : new j([]), !(r instanceof j)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
+        if (r = (i = r ?? ((e = a[0]) === null || e === void 0 ? void 0 : e.schema)) !== null && i !== void 0 ? i : new W([]), !(r instanceof W)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
         for (const l of a) {
-            if (!(l instanceof St)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
-            if (!Dr(r, l.schema)) throw new TypeError("Table and inner RecordBatch schemas must be equivalent.")
+            if (!(l instanceof It)) throw new TypeError("Table constructor expects a [Schema, RecordBatch[]] pair.");
+            if (!xr(r, l.schema)) throw new TypeError("Table and inner RecordBatch schemas must be equivalent.")
         }
         this.schema = r, this.batches = a, this._offsets = s ?? Ma(this.data)
     }
     get data() {
         return this.batches.map(({
             data: t
         }) => t)
@@ -6315,30 +6315,30 @@
     get numCols() {
         return this.schema.fields.length
     }
     get numRows() {
         return this.data.reduce((t, e) => t + e.length, 0)
     }
     get nullCount() {
-        return this._nullCount === -1 && (this._nullCount = Na(this.data)), this._nullCount
+        return this._nullCount === -1 && (this._nullCount = xa(this.data)), this._nullCount
     }
     isValid(t) {
         return !1
     }
     get(t) {
         return null
     }
     set(t, e) {}
     indexOf(t, e) {
         return -1
     }
     getByteLength(t) {
         return 0
     } [Symbol.iterator]() {
-        return this.batches.length > 0 ? rs.visit(new P(this.data)) : new Array(0)[Symbol.iterator]()
+        return this.batches.length > 0 ? as.visit(new z(this.data)) : new Array(0)[Symbol.iterator]()
     }
     toArray() {
         return [...this]
     }
     toString() {
         return `[
   ${this.toArray().join(`,
@@ -6346,23 +6346,23 @@
 ]`
     }
     concat(...t) {
         const e = this.schema,
             i = this.data.concat(t.flatMap(({
                 data: r
             }) => r));
-        return new pt(e, i.map(r => new St(e, r)))
+        return new yt(e, i.map(r => new It(e, r)))
     }
     slice(t, e) {
         const i = this.schema;
-        [t, e] = Da({
+        [t, e] = Ta({
             length: this.numRows
         }, t, e);
-        const r = xa(this.data, this._offsets, t, e);
-        return new pt(i, r.map(s => new St(i, s)))
+        const r = La(this.data, this._offsets, t, e);
+        return new yt(i, r.map(s => new It(i, s)))
     }
     getChild(t) {
         return this.getChildAt(this.schema.fields.findIndex(e => e.name === t))
     }
     getChildAt(t) {
         if (t > -1 && t < this.schema.fields.length) {
             const e = this.data.map(i => i.children[t]);
@@ -6372,109 +6372,109 @@
                 } = this.schema.fields[t], r = E({
                     type: i,
                     length: 0,
                     nullCount: 0
                 });
                 e.push(r._changeLengthAndBackfillNullBitmap(this.numRows))
             }
-            return new P(e)
+            return new z(e)
         }
         return null
     }
     setChild(t, e) {
         var i;
         return this.setChildAt((i = this.schema.fields) === null || i === void 0 ? void 0 : i.findIndex(r => r.name === t), e)
     }
     setChildAt(t, e) {
         let i = this.schema,
             r = [...this.batches];
         if (t > -1 && t < this.numCols) {
-            e || (e = new P([E({
-                type: new Oe,
+            e || (e = new z([E({
+                type: new Te,
                 length: this.numRows
             })]));
             const s = i.fields.slice(),
                 o = s[t].clone({
                     type: e.type
                 }),
                 a = this.schema.fields.map((l, c) => this.getChildAt(c));
-            [s[t], a[t]] = [o, e], [i, r] = hr(i, a)
+            [s[t], a[t]] = [o, e], [i, r] = pr(i, a)
         }
-        return new pt(i, r)
+        return new yt(i, r)
     }
     select(t) {
         const e = this.schema.fields.reduce((i, r, s) => i.set(r.name, s), new Map);
         return this.selectAt(t.map(i => e.get(i)).filter(i => i > -1))
     }
     selectAt(t) {
         const e = this.schema.selectAt(t),
             i = this.batches.map(r => r.selectAt(t));
-        return new pt(e, i)
+        return new yt(e, i)
     }
     assign(t) {
         const e = this.schema.fields,
             [i, r] = t.schema.fields.reduce((a, l, c) => {
                 const [d, h] = a, y = e.findIndex(_ => _.name === l.name);
                 return ~y ? h[y] = c : d.push(c), a
             }, [
                 [],
                 []
             ]),
             s = this.schema.assign(t.schema),
             o = [...e.map((a, l) => [l, r[l]]).map(([a, l]) => l === void 0 ? this.getChildAt(a) : t.getChildAt(l)), ...i.map(a => t.getChildAt(a))].filter(Boolean);
-        return new pt(...hr(s, o))
+        return new yt(...pr(s, o))
     }
 }
-Ga = Symbol.toStringTag;
-pt[Ga] = (n => (n.schema = null, n.batches = [], n._offsets = new Uint32Array([0]), n._nullCount = -1, n[Symbol.isConcatSpreadable] = !0, n.isValid = ln(is), n.get = ln(Ft.getVisitFn(u.Struct)), n.set = La(Vt.getVisitFn(u.Struct)), n.indexOf = Ea(Ii.getVisitFn(u.Struct)), n.getByteLength = ln(ie.getVisitFn(u.Struct)), "Table"))(pt.prototype);
-var Ha;
-let St = class Fn {
+Ha = Symbol.toStringTag;
+yt[Ha] = (n => (n.schema = null, n.batches = [], n._offsets = new Uint32Array([0]), n._nullCount = -1, n[Symbol.isConcatSpreadable] = !0, n.isValid = un(os), n.get = un(Ft.getVisitFn(u.Struct)), n.set = Ea(Vt.getVisitFn(u.Struct)), n.indexOf = Ra(Oi.getVisitFn(u.Struct)), n.getByteLength = un(oe.getVisitFn(u.Struct)), "Table"))(yt.prototype);
+var qa;
+let It = class Tn {
     constructor(...t) {
         switch (t.length) {
             case 2: {
-                if ([this.schema] = t, !(this.schema instanceof j)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
+                if ([this.schema] = t, !(this.schema instanceof W)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
                 if ([, this.data = E({
                         nullCount: 0,
-                        type: new yt(this.schema.fields),
+                        type: new mt(this.schema.fields),
                         children: this.schema.fields.map(e => E({
                             type: e.type,
                             nullCount: 0
                         }))
-                    })] = t, !(this.data instanceof K)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
+                    })] = t, !(this.data instanceof X)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
                 [this.schema, this.data] = Vs(this.schema, this.data.children);
                 break
             }
             case 1: {
                 const [e] = t, {
                     fields: i,
                     children: r,
                     length: s
-                } = Object.keys(e).reduce((l, c, d) => (l.children[d] = e[c], l.length = Math.max(l.length, e[c].length), l.fields[d] = X.new({
+                } = Object.keys(e).reduce((l, c, d) => (l.children[d] = e[c], l.length = Math.max(l.length, e[c].length), l.fields[d] = tt.new({
                     name: c,
                     type: e[c].type,
                     nullable: !0
                 }), l), {
                     length: 0,
                     fields: new Array,
                     children: new Array
-                }), o = new j(i), a = E({
-                    type: new yt(i),
+                }), o = new W(i), a = E({
+                    type: new mt(i),
                     length: s,
                     children: r,
                     nullCount: 0
                 });
                 [this.schema, this.data] = Vs(o, a.children, s);
                 break
             }
             default:
                 throw new TypeError("RecordBatch constructor expects an Object mapping names to child Data, or a [Schema, Data] pair.")
         }
     }
     get dictionaries() {
-        return this._dictionaries || (this._dictionaries = qa(this.schema.fields, this.data.children))
+        return this._dictionaries || (this._dictionaries = Ja(this.schema.fields, this.data.children))
     }
     get numCols() {
         return this.schema.fields.length
     }
     get numRows() {
         return this.data.length
     }
@@ -6487,89 +6487,89 @@
     get(t) {
         return Ft.visit(this.data, t)
     }
     set(t, e) {
         return Vt.visit(this.data, t, e)
     }
     indexOf(t, e) {
-        return Ii.visit(this.data, t, e)
+        return Oi.visit(this.data, t, e)
     }
     getByteLength(t) {
-        return ie.visit(this.data, t)
+        return oe.visit(this.data, t)
     } [Symbol.iterator]() {
-        return rs.visit(new P([this.data]))
+        return as.visit(new z([this.data]))
     }
     toArray() {
         return [...this]
     }
     concat(...t) {
-        return new pt(this.schema, [this, ...t])
+        return new yt(this.schema, [this, ...t])
     }
     slice(t, e) {
-        const [i] = new P([this.data]).slice(t, e).data;
-        return new Fn(this.schema, i)
+        const [i] = new z([this.data]).slice(t, e).data;
+        return new Tn(this.schema, i)
     }
     getChild(t) {
         var e;
         return this.getChildAt((e = this.schema.fields) === null || e === void 0 ? void 0 : e.findIndex(i => i.name === t))
     }
     getChildAt(t) {
-        return t > -1 && t < this.schema.fields.length ? new P([this.data.children[t]]) : null
+        return t > -1 && t < this.schema.fields.length ? new z([this.data.children[t]]) : null
     }
     setChild(t, e) {
         var i;
         return this.setChildAt((i = this.schema.fields) === null || i === void 0 ? void 0 : i.findIndex(r => r.name === t), e)
     }
     setChildAt(t, e) {
         let i = this.schema,
             r = this.data;
         if (t > -1 && t < this.numCols) {
-            e || (e = new P([E({
-                type: new Oe,
+            e || (e = new z([E({
+                type: new Te,
                 length: this.numRows
             })]));
             const s = i.fields.slice(),
                 o = r.children.slice(),
                 a = s[t].clone({
                     type: e.type
                 });
-            [s[t], o[t]] = [a, e.data[0]], i = new j(s, new Map(this.schema.metadata)), r = E({
-                type: new yt(s),
+            [s[t], o[t]] = [a, e.data[0]], i = new W(s, new Map(this.schema.metadata)), r = E({
+                type: new mt(s),
                 children: o
             })
         }
-        return new Fn(i, r)
+        return new Tn(i, r)
     }
     select(t) {
         const e = this.schema.select(t),
-            i = new yt(e.fields),
+            i = new mt(e.fields),
             r = [];
         for (const s of t) {
             const o = this.schema.fields.findIndex(a => a.name === s);
             ~o && (r[o] = this.data.children[o])
         }
-        return new Fn(e, E({
+        return new Tn(e, E({
             type: i,
             length: this.numRows,
             children: r
         }))
     }
     selectAt(t) {
         const e = this.schema.selectAt(t),
             i = t.map(s => this.data.children[s]).filter(Boolean),
             r = E({
-                type: new yt(e.fields),
+                type: new mt(e.fields),
                 length: this.numRows,
                 children: i
             });
-        return new Fn(e, r)
+        return new Tn(e, r)
     }
 };
-Ha = Symbol.toStringTag;
-St[Ha] = (n => (n._nullCount = -1, n[Symbol.isConcatSpreadable] = !0, "RecordBatch"))(St.prototype);
+qa = Symbol.toStringTag;
+It[qa] = (n => (n._nullCount = -1, n[Symbol.isConcatSpreadable] = !0, "RecordBatch"))(It.prototype);
 
 function Vs(n, t, e = t.reduce((i, r) => Math.max(i, r.length), 0)) {
     var i;
     const r = [...n.fields],
         s = [...t],
         o = (e + 63 & -64) >> 3;
     for (const [a, l] of n.fields.entries()) {
@@ -6580,91 +6580,91 @@
             type: l.type,
             length: e,
             nullCount: e,
             nullBitmap: new Uint8Array(o)
         }))
     }
     return [n.assign(r), E({
-        type: new yt(r),
+        type: new mt(r),
         length: e,
         children: s
     })]
 }
 
-function qa(n, t, e = new Map) {
+function Ja(n, t, e = new Map) {
     for (let i = -1, r = n.length; ++i < r;) {
         const o = n[i].type,
             a = t[i];
-        if (S.isDictionary(o)) {
+        if (I.isDictionary(o)) {
             if (!e.has(o.id)) a.dictionary && e.set(o.id, a.dictionary);
             else if (e.get(o.id) !== a.dictionary) throw new Error("Cannot create Schema containing two different dictionaries with the same Id")
         }
-        o.children && o.children.length > 0 && qa(o.children, a.children, e)
+        o.children && o.children.length > 0 && Ja(o.children, a.children, e)
     }
     return e
 }
-class us extends St {
+class fs extends It {
     constructor(t) {
         const e = t.fields.map(r => E({
                 type: r.type
             })),
             i = E({
-                type: new yt(t.fields),
+                type: new mt(t.fields),
                 nullCount: 0,
                 children: e
             });
         super(t, i)
     }
 }
-var xi;
+var Ei;
 (function(n) {
     n[n.BUFFER = 0] = "BUFFER"
-})(xi || (xi = {}));
-var Li;
+})(Ei || (Ei = {}));
+var Ri;
 (function(n) {
     n[n.LZ4_FRAME = 0] = "LZ4_FRAME", n[n.ZSTD = 1] = "ZSTD"
-})(Li || (Li = {}));
-class we {
+})(Ri || (Ri = {}));
+class Oe {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsBodyCompression(t, e) {
-        return (e || new we).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Oe).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsBodyCompression(t, e) {
-        return t.setPosition(t.position() + J), (e || new we).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Oe).__init(t.readInt32(t.position()) + t.position(), t)
     }
     codec() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt8(this.bb_pos + t) : Li.LZ4_FRAME
+        return t ? this.bb.readInt8(this.bb_pos + t) : Ri.LZ4_FRAME
     }
     method() {
         const t = this.bb.__offset(this.bb_pos, 6);
-        return t ? this.bb.readInt8(this.bb_pos + t) : xi.BUFFER
+        return t ? this.bb.readInt8(this.bb_pos + t) : Ei.BUFFER
     }
     static startBodyCompression(t) {
         t.startObject(2)
     }
     static addCodec(t, e) {
-        t.addFieldInt8(0, e, Li.LZ4_FRAME)
+        t.addFieldInt8(0, e, Ri.LZ4_FRAME)
     }
     static addMethod(t, e) {
-        t.addFieldInt8(1, e, xi.BUFFER)
+        t.addFieldInt8(1, e, Ei.BUFFER)
     }
     static endBodyCompression(t) {
         return t.endObject()
     }
     static createBodyCompression(t, e, i) {
-        return we.startBodyCompression(t), we.addCodec(t, e), we.addMethod(t, i), we.endBodyCompression(t)
+        return Oe.startBodyCompression(t), Oe.addCodec(t, e), Oe.addMethod(t, i), Oe.endBodyCompression(t)
     }
 }
-class Ja {
+class Ka {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     offset() {
@@ -6676,15 +6676,15 @@
     static sizeOf() {
         return 16
     }
     static createBuffer(t, e, i) {
         return t.prep(8, 16), t.writeInt64(i), t.writeInt64(e), t.offset()
     }
 }
-let Ka = class {
+let Za = class {
         constructor() {
             this.bb = null, this.bb_pos = 0
         }
         __init(t, e) {
             return this.bb_pos = t, this.bb = e, this
         }
         length() {
@@ -6696,50 +6696,50 @@
         static sizeOf() {
             return 16
         }
         static createFieldNode(t, e, i) {
             return t.prep(8, 16), t.writeInt64(i), t.writeInt64(e), t.offset()
         }
     },
-    ce = class Tr {
+    fe = class Mr {
         constructor() {
             this.bb = null, this.bb_pos = 0
         }
         __init(t, e) {
             return this.bb_pos = t, this.bb = e, this
         }
         static getRootAsRecordBatch(t, e) {
-            return (e || new Tr).__init(t.readInt32(t.position()) + t.position(), t)
+            return (e || new Mr).__init(t.readInt32(t.position()) + t.position(), t)
         }
         static getSizePrefixedRootAsRecordBatch(t, e) {
-            return t.setPosition(t.position() + J), (e || new Tr).__init(t.readInt32(t.position()) + t.position(), t)
+            return t.setPosition(t.position() + Z), (e || new Mr).__init(t.readInt32(t.position()) + t.position(), t)
         }
         length() {
             const t = this.bb.__offset(this.bb_pos, 4);
             return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
         }
         nodes(t, e) {
             const i = this.bb.__offset(this.bb_pos, 6);
-            return i ? (e || new Ka).__init(this.bb.__vector(this.bb_pos + i) + t * 16, this.bb) : null
+            return i ? (e || new Za).__init(this.bb.__vector(this.bb_pos + i) + t * 16, this.bb) : null
         }
         nodesLength() {
             const t = this.bb.__offset(this.bb_pos, 6);
             return t ? this.bb.__vector_len(this.bb_pos + t) : 0
         }
         buffers(t, e) {
             const i = this.bb.__offset(this.bb_pos, 8);
-            return i ? (e || new Ja).__init(this.bb.__vector(this.bb_pos + i) + t * 16, this.bb) : null
+            return i ? (e || new Ka).__init(this.bb.__vector(this.bb_pos + i) + t * 16, this.bb) : null
         }
         buffersLength() {
             const t = this.bb.__offset(this.bb_pos, 8);
             return t ? this.bb.__vector_len(this.bb_pos + t) : 0
         }
         compression(t) {
             const e = this.bb.__offset(this.bb_pos, 10);
-            return e ? (t || new we).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+            return e ? (t || new Oe).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
         }
         static startRecordBatch(t) {
             t.startObject(4)
         }
         static addLength(t, e) {
             t.addFieldInt64(0, e, t.createLong(0, 0))
         }
@@ -6758,34 +6758,34 @@
         static addCompression(t, e) {
             t.addFieldOffset(3, e, 0)
         }
         static endRecordBatch(t) {
             return t.endObject()
         }
     },
-    en = class Nr {
+    rn = class Lr {
         constructor() {
             this.bb = null, this.bb_pos = 0
         }
         __init(t, e) {
             return this.bb_pos = t, this.bb = e, this
         }
         static getRootAsDictionaryBatch(t, e) {
-            return (e || new Nr).__init(t.readInt32(t.position()) + t.position(), t)
+            return (e || new Lr).__init(t.readInt32(t.position()) + t.position(), t)
         }
         static getSizePrefixedRootAsDictionaryBatch(t, e) {
-            return t.setPosition(t.position() + J), (e || new Nr).__init(t.readInt32(t.position()) + t.position(), t)
+            return t.setPosition(t.position() + Z), (e || new Lr).__init(t.readInt32(t.position()) + t.position(), t)
         }
         id() {
             const t = this.bb.__offset(this.bb_pos, 4);
             return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
         }
         data(t) {
             const e = this.bb.__offset(this.bb_pos, 6);
-            return e ? (t || new ce).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+            return e ? (t || new fe).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
         }
         isDelta() {
             const t = this.bb.__offset(this.bb_pos, 8);
             return t ? !!this.bb.readInt8(this.bb_pos + t) : !1
         }
         static startDictionaryBatch(t) {
             t.startObject(3)
@@ -6799,38 +6799,38 @@
         static addIsDelta(t, e) {
             t.addFieldInt8(2, +e, 0)
         }
         static endDictionaryBatch(t) {
             return t.endObject()
         }
     };
-var Ei;
+var Ci;
 (function(n) {
     n[n.NONE = 0] = "NONE", n[n.Schema = 1] = "Schema", n[n.DictionaryBatch = 2] = "DictionaryBatch", n[n.RecordBatch = 3] = "RecordBatch", n[n.Tensor = 4] = "Tensor", n[n.SparseTensor = 5] = "SparseTensor"
-})(Ei || (Ei = {}));
-let ge = class Wt {
+})(Ci || (Ci = {}));
+let Ie = class Gt {
     constructor() {
         this.bb = null, this.bb_pos = 0
     }
     __init(t, e) {
         return this.bb_pos = t, this.bb = e, this
     }
     static getRootAsMessage(t, e) {
-        return (e || new Wt).__init(t.readInt32(t.position()) + t.position(), t)
+        return (e || new Gt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     static getSizePrefixedRootAsMessage(t, e) {
-        return t.setPosition(t.position() + J), (e || new Wt).__init(t.readInt32(t.position()) + t.position(), t)
+        return t.setPosition(t.position() + Z), (e || new Gt).__init(t.readInt32(t.position()) + t.position(), t)
     }
     version() {
         const t = this.bb.__offset(this.bb_pos, 4);
-        return t ? this.bb.readInt16(this.bb_pos + t) : fn.V1
+        return t ? this.bb.readInt16(this.bb_pos + t) : mn.V1
     }
     headerType() {
         const t = this.bb.__offset(this.bb_pos, 6);
-        return t ? this.bb.readUint8(this.bb_pos + t) : Ei.NONE
+        return t ? this.bb.readUint8(this.bb_pos + t) : Ci.NONE
     }
     header(t) {
         const e = this.bb.__offset(this.bb_pos, 8);
         return e ? this.bb.__union(t, this.bb_pos + e) : null
     }
     bodyLength() {
         const t = this.bb.__offset(this.bb_pos, 10);
@@ -6844,18 +6844,18 @@
         const t = this.bb.__offset(this.bb_pos, 12);
         return t ? this.bb.__vector_len(this.bb_pos + t) : 0
     }
     static startMessage(t) {
         t.startObject(5)
     }
     static addVersion(t, e) {
-        t.addFieldInt16(0, e, fn.V1)
+        t.addFieldInt16(0, e, mn.V1)
     }
     static addHeaderType(t, e) {
-        t.addFieldInt8(1, e, Ei.NONE)
+        t.addFieldInt8(1, e, Ci.NONE)
     }
     static addHeader(t, e) {
         t.addFieldOffset(2, e, 0)
     }
     static addBodyLength(t, e) {
         t.addFieldInt64(3, e, t.createLong(0, 0))
     }
@@ -6876,229 +6876,229 @@
     static finishMessageBuffer(t, e) {
         t.finish(e)
     }
     static finishSizePrefixedMessageBuffer(t, e) {
         t.finish(e, void 0, !0)
     }
     static createMessage(t, e, i, r, s, o) {
-        return Wt.startMessage(t), Wt.addVersion(t, e), Wt.addHeaderType(t, i), Wt.addHeader(t, r), Wt.addBodyLength(t, s), Wt.addCustomMetadata(t, o), Wt.endMessage(t)
+        return Gt.startMessage(t), Gt.addVersion(t, e), Gt.addHeaderType(t, i), Gt.addHeader(t, r), Gt.addBodyLength(t, s), Gt.addCustomMetadata(t, o), Gt.endMessage(t)
     }
 };
-var ad = he;
+var ad = me;
 class ld extends R {
     visit(t, e) {
         return t == null || e == null ? void 0 : super.visit(t, e)
     }
     visitNull(t, e) {
-        return Ve.startNull(e), Ve.endNull(e)
+        return je.startNull(e), je.endNull(e)
     }
     visitInt(t, e) {
         return Tt.startInt(e), Tt.addBitWidth(e, t.bitWidth), Tt.addIsSigned(e, t.isSigned), Tt.endInt(e)
     }
     visitFloat(t, e) {
-        return Xt.startFloatingPoint(e), Xt.addPrecision(e, t.precision), Xt.endFloatingPoint(e)
+        return te.startFloatingPoint(e), te.addPrecision(e, t.precision), te.endFloatingPoint(e)
     }
     visitBinary(t, e) {
-        return Ce.startBinary(e), Ce.endBinary(e)
+        return $e.startBinary(e), $e.endBinary(e)
     }
     visitBool(t, e) {
-        return ke.startBool(e), ke.endBool(e)
+        return Ve.startBool(e), Ve.endBool(e)
     }
     visitUtf8(t, e) {
-        return Pe.startUtf8(e), Pe.endUtf8(e)
+        return We.startUtf8(e), We.endUtf8(e)
     }
     visitDecimal(t, e) {
-        return _t.startDecimal(e), _t.addScale(e, t.scale), _t.addPrecision(e, t.precision), _t.addBitWidth(e, t.bitWidth), _t.endDecimal(e)
+        return wt.startDecimal(e), wt.addScale(e, t.scale), wt.addPrecision(e, t.precision), wt.addBitWidth(e, t.bitWidth), wt.endDecimal(e)
     }
     visitDate(t, e) {
-        return ii.startDate(e), ii.addUnit(e, t.unit), ii.endDate(e)
+        return si.startDate(e), si.addUnit(e, t.unit), si.endDate(e)
     }
     visitTime(t, e) {
-        return kt.startTime(e), kt.addUnit(e, t.unit), kt.addBitWidth(e, t.bitWidth), kt.endTime(e)
+        return Ut.startTime(e), Ut.addUnit(e, t.unit), Ut.addBitWidth(e, t.bitWidth), Ut.endTime(e)
     }
     visitTimestamp(t, e) {
         const i = t.timezone && e.createString(t.timezone) || void 0;
-        return Ut.startTimestamp(e), Ut.addUnit(e, t.unit), i !== void 0 && Ut.addTimezone(e, i), Ut.endTimestamp(e)
+        return $t.startTimestamp(e), $t.addUnit(e, t.unit), i !== void 0 && $t.addTimezone(e, i), $t.endTimestamp(e)
     }
     visitInterval(t, e) {
-        return Qt.startInterval(e), Qt.addUnit(e, t.unit), Qt.endInterval(e)
+        return ee.startInterval(e), ee.addUnit(e, t.unit), ee.endInterval(e)
     }
     visitList(t, e) {
-        return Ue.startList(e), Ue.endList(e)
+        return Pe.startList(e), Pe.endList(e)
     }
     visitStruct(t, e) {
-        return $e.startStruct_(e), $e.endStruct_(e)
+        return ze.startStruct_(e), ze.endStruct_(e)
     }
     visitUnion(t, e) {
-        wt.startTypeIdsVector(e, t.typeIds.length);
-        const i = wt.createTypeIdsVector(e, t.typeIds);
-        return wt.startUnion(e), wt.addMode(e, t.mode), wt.addTypeIds(e, i), wt.endUnion(e)
+        St.startTypeIdsVector(e, t.typeIds.length);
+        const i = St.createTypeIdsVector(e, t.typeIds);
+        return St.startUnion(e), St.addMode(e, t.mode), St.addTypeIds(e, i), St.endUnion(e)
     }
     visitDictionary(t, e) {
         const i = this.visit(t.indices, e);
-        return de.startDictionaryEncoding(e), de.addId(e, new ad(t.id, 0)), de.addIsOrdered(e, t.isOrdered), i !== void 0 && de.addIndexType(e, i), de.endDictionaryEncoding(e)
+        return ye.startDictionaryEncoding(e), ye.addId(e, new ad(t.id, 0)), ye.addIsOrdered(e, t.isOrdered), i !== void 0 && ye.addIndexType(e, i), ye.endDictionaryEncoding(e)
     }
     visitFixedSizeBinary(t, e) {
-        return Kt.startFixedSizeBinary(e), Kt.addByteWidth(e, t.byteWidth), Kt.endFixedSizeBinary(e)
+        return Xt.startFixedSizeBinary(e), Xt.addByteWidth(e, t.byteWidth), Xt.endFixedSizeBinary(e)
     }
     visitFixedSizeList(t, e) {
-        return Zt.startFixedSizeList(e), Zt.addListSize(e, t.listSize), Zt.endFixedSizeList(e)
+        return Qt.startFixedSizeList(e), Qt.addListSize(e, t.listSize), Qt.endFixedSizeList(e)
     }
     visitMap(t, e) {
-        return ri.startMap(e), ri.addKeysSorted(e, t.keysSorted), ri.endMap(e)
+        return oi.startMap(e), oi.addKeysSorted(e, t.keysSorted), oi.endMap(e)
     }
 }
-const fr = new ld;
+const yr = new ld;
 
 function cd(n, t = new Map) {
-    return new j(dd(n, t), ai(n.customMetadata), t)
+    return new W(dd(n, t), ci(n.customMetadata), t)
 }
 
-function Za(n) {
-    return new Lt(n.count, Xa(n.columns), Qa(n.columns))
+function Xa(n) {
+    return new Lt(n.count, Qa(n.columns), tl(n.columns))
 }
 
 function ud(n) {
-    return new re(Za(n.data), n.id, n.isDelta)
+    return new ae(Xa(n.data), n.id, n.isDelta)
 }
 
 function dd(n, t) {
-    return (n.fields || []).filter(Boolean).map(e => X.fromJSON(e, t))
+    return (n.fields || []).filter(Boolean).map(e => tt.fromJSON(e, t))
 }
 
-function $s(n, t) {
-    return (n.children || []).filter(Boolean).map(e => X.fromJSON(e, t))
+function Ps(n, t) {
+    return (n.children || []).filter(Boolean).map(e => tt.fromJSON(e, t))
 }
 
-function Xa(n) {
-    return (n || []).reduce((t, e) => [...t, new Ge(e.count, hd(e.VALIDITY)), ...Xa(e.children)], [])
+function Qa(n) {
+    return (n || []).reduce((t, e) => [...t, new Ke(e.count, hd(e.VALIDITY)), ...Qa(e.children)], [])
 }
 
-function Qa(n, t = []) {
+function tl(n, t = []) {
     for (let e = -1, i = (n || []).length; ++e < i;) {
         const r = n[e];
-        r.VALIDITY && t.push(new ee(t.length, r.VALIDITY.length)), r.TYPE && t.push(new ee(t.length, r.TYPE.length)), r.OFFSET && t.push(new ee(t.length, r.OFFSET.length)), r.DATA && t.push(new ee(t.length, r.DATA.length)), t = Qa(r.children, t)
+        r.VALIDITY && t.push(new ie(t.length, r.VALIDITY.length)), r.TYPE && t.push(new ie(t.length, r.TYPE.length)), r.OFFSET && t.push(new ie(t.length, r.OFFSET.length)), r.DATA && t.push(new ie(t.length, r.DATA.length)), t = tl(r.children, t)
     }
     return t
 }
 
 function hd(n) {
     return (n || []).reduce((t, e) => t + +(e === 0), 0)
 }
 
 function fd(n, t) {
     let e, i, r, s, o, a;
-    return !t || !(s = n.dictionary) ? (o = js(n, $s(n, t)), r = new X(n.name, o, n.nullable, ai(n.customMetadata))) : t.has(e = s.id) ? (i = (i = s.indexType) ? Ps(i) : new Cn, a = new dn(t.get(e), i, e, s.isOrdered), r = new X(n.name, a, n.nullable, ai(n.customMetadata))) : (i = (i = s.indexType) ? Ps(i) : new Cn, t.set(e, o = js(n, $s(n, t))), a = new dn(o, i, e, s.isOrdered), r = new X(n.name, a, n.nullable, ai(n.customMetadata))), r || null
+    return !t || !(s = n.dictionary) ? (o = zs(n, Ps(n, t)), r = new tt(n.name, o, n.nullable, ci(n.customMetadata))) : t.has(e = s.id) ? (i = (i = s.indexType) ? js(i) : new kn, a = new pn(t.get(e), i, e, s.isOrdered), r = new tt(n.name, a, n.nullable, ci(n.customMetadata))) : (i = (i = s.indexType) ? js(i) : new kn, t.set(e, o = zs(n, Ps(n, t))), a = new pn(o, i, e, s.isOrdered), r = new tt(n.name, a, n.nullable, ci(n.customMetadata))), r || null
 }
 
-function ai(n) {
+function ci(n) {
     return new Map(Object.entries(n || {}))
 }
 
-function Ps(n) {
-    return new Fe(n.isSigned, n.bitWidth)
+function js(n) {
+    return new Ne(n.isSigned, n.bitWidth)
 }
 
-function js(n, t) {
+function zs(n, t) {
     const e = n.type.name;
     switch (e) {
         case "NONE":
-            return new Oe;
+            return new Te;
         case "null":
-            return new Oe;
+            return new Te;
         case "binary":
-            return new ui;
+            return new hi;
         case "utf8":
-            return new di;
+            return new fi;
         case "bool":
-            return new hi;
+            return new pi;
         case "list":
-            return new vi((t || [])[0]);
+            return new gi((t || [])[0]);
         case "struct":
-            return new yt(t || []);
+            return new mt(t || []);
         case "struct_":
-            return new yt(t || [])
+            return new mt(t || [])
     }
     switch (e) {
         case "int": {
             const i = n.type;
-            return new Fe(i.isSigned, i.bitWidth)
+            return new Ne(i.isSigned, i.bitWidth)
         }
         case "floatingpoint": {
             const i = n.type;
-            return new kn(Bt[i.precision])
+            return new Un(Bt[i.precision])
         }
         case "decimal": {
             const i = n.type;
-            return new fi(i.scale, i.precision, i.bitWidth)
+            return new yi(i.scale, i.precision, i.bitWidth)
         }
         case "date": {
             const i = n.type;
-            return new pi(ye[i.unit])
+            return new mi(be[i.unit])
         }
         case "time": {
             const i = n.type;
-            return new Un(V[i.unit], i.bitWidth)
+            return new $n($[i.unit], i.bitWidth)
         }
         case "timestamp": {
             const i = n.type;
-            return new yi(V[i.unit], i.timezone)
+            return new vi($[i.unit], i.timezone)
         }
         case "interval": {
             const i = n.type;
-            return new mi(Be[i.unit])
+            return new bi(De[i.unit])
         }
         case "union": {
             const i = n.type;
-            return new bi(xt[i.mode], i.typeIds || [], t || [])
+            return new _i(Mt[i.mode], i.typeIds || [], t || [])
         }
         case "fixedsizebinary": {
             const i = n.type;
-            return new gi(i.byteWidth)
+            return new wi(i.byteWidth)
         }
         case "fixedsizelist": {
             const i = n.type;
-            return new _i(i.listSize, (t || [])[0])
+            return new Si(i.listSize, (t || [])[0])
         }
         case "map": {
             const i = n.type;
-            return new wi((t || [])[0], i.keysSorted)
+            return new Ii((t || [])[0], i.keysSorted)
         }
     }
     throw new Error(`Unrecognized type: "${e}"`)
 }
-var We = he,
-    pd = ja,
-    yd = hn;
-class mt {
+var qe = me,
+    pd = za,
+    yd = yn;
+class vt {
     constructor(t, e, i, r) {
         this._version = e, this._headerType = i, this.body = new Uint8Array(0), r && (this._createHeader = () => r), this._bodyLength = typeof t == "number" ? t : t.low
     }
     static fromJSON(t, e) {
-        const i = new mt(0, Nt.V4, e);
+        const i = new vt(0, Nt.V4, e);
         return i._createHeader = md(t, e), i
     }
     static decode(t) {
         t = new yd(U(t));
-        const e = ge.getRootAsMessage(t),
+        const e = Ie.getRootAsMessage(t),
             i = e.bodyLength(),
             r = e.version(),
             s = e.headerType(),
-            o = new mt(i, r, s);
+            o = new vt(i, r, s);
         return o._createHeader = vd(e, s), o
     }
     static encode(t) {
         const e = new pd;
         let i = -1;
-        return t.isSchema() ? i = j.encode(e, t.header()) : t.isRecordBatch() ? i = Lt.encode(e, t.header()) : t.isDictionaryBatch() && (i = re.encode(e, t.header())), ge.startMessage(e), ge.addVersion(e, Nt.V4), ge.addHeader(e, i), ge.addHeaderType(e, t.headerType), ge.addBodyLength(e, new We(t.bodyLength, 0)), ge.finishMessageBuffer(e, ge.endMessage(e)), e.asUint8Array()
+        return t.isSchema() ? i = W.encode(e, t.header()) : t.isRecordBatch() ? i = Lt.encode(e, t.header()) : t.isDictionaryBatch() && (i = ae.encode(e, t.header())), Ie.startMessage(e), Ie.addVersion(e, Nt.V4), Ie.addHeader(e, i), Ie.addHeaderType(e, t.headerType), Ie.addBodyLength(e, new qe(t.bodyLength, 0)), Ie.finishMessageBuffer(e, Ie.endMessage(e)), e.asUint8Array()
     }
     static from(t, e = 0) {
-        if (t instanceof j) return new mt(0, Nt.V4, $.Schema, t);
-        if (t instanceof Lt) return new mt(e, Nt.V4, $.RecordBatch, t);
-        if (t instanceof re) return new mt(e, Nt.V4, $.DictionaryBatch, t);
+        if (t instanceof W) return new vt(0, Nt.V4, j.Schema, t);
+        if (t instanceof Lt) return new vt(e, Nt.V4, j.RecordBatch, t);
+        if (t instanceof ae) return new vt(e, Nt.V4, j.DictionaryBatch, t);
         throw new Error(`Unrecognized Message header: ${t}`)
     }
     get type() {
         return this.headerType
     }
     get version() {
         return this._version
@@ -7109,21 +7109,21 @@
     get bodyLength() {
         return this._bodyLength
     }
     header() {
         return this._createHeader()
     }
     isSchema() {
-        return this.headerType === $.Schema
+        return this.headerType === j.Schema
     }
     isRecordBatch() {
-        return this.headerType === $.RecordBatch
+        return this.headerType === j.RecordBatch
     }
     isDictionaryBatch() {
-        return this.headerType === $.DictionaryBatch
+        return this.headerType === j.DictionaryBatch
     }
 }
 class Lt {
     constructor(t, e, i) {
         this._nodes = e, this._buffers = i, this._length = typeof t == "number" ? t : t.low
     }
     get nodes() {
@@ -7132,15 +7132,15 @@
     get length() {
         return this._length
     }
     get buffers() {
         return this._buffers
     }
 }
-class re {
+class ae {
     constructor(t, e, i = !1) {
         this._data = t, this._isDelta = i, this._id = typeof e == "number" ? e : e.low
     }
     get id() {
         return this._id
     }
     get data() {
@@ -7155,443 +7155,443 @@
     get nodes() {
         return this.data.nodes
     }
     get buffers() {
         return this.data.buffers
     }
 }
-class ee {
+class ie {
     constructor(t, e) {
         this.offset = typeof t == "number" ? t : t.low, this.length = typeof e == "number" ? e : e.low
     }
 }
-class Ge {
+class Ke {
     constructor(t, e) {
         this.length = typeof t == "number" ? t : t.low, this.nullCount = typeof e == "number" ? e : e.low
     }
 }
 
 function md(n, t) {
     return () => {
         switch (t) {
-            case $.Schema:
-                return j.fromJSON(n);
-            case $.RecordBatch:
+            case j.Schema:
+                return W.fromJSON(n);
+            case j.RecordBatch:
                 return Lt.fromJSON(n);
-            case $.DictionaryBatch:
-                return re.fromJSON(n)
+            case j.DictionaryBatch:
+                return ae.fromJSON(n)
         }
-        throw new Error(`Unrecognized Message type: { name: ${$[t]}, type: ${t} }`)
+        throw new Error(`Unrecognized Message type: { name: ${j[t]}, type: ${t} }`)
     }
 }
 
 function vd(n, t) {
     return () => {
         switch (t) {
-            case $.Schema:
-                return j.decode(n.header(new Yt));
-            case $.RecordBatch:
-                return Lt.decode(n.header(new ce), n.version());
-            case $.DictionaryBatch:
-                return re.decode(n.header(new en), n.version())
-        }
-        throw new Error(`Unrecognized Message type: { name: ${$[t]}, type: ${t} }`)
-    }
-}
-X.encode = Dd;
-X.decode = Fd;
-X.fromJSON = fd;
-j.encode = Ad;
-j.decode = bd;
-j.fromJSON = cd;
+            case j.Schema:
+                return W.decode(n.header(new Ht));
+            case j.RecordBatch:
+                return Lt.decode(n.header(new fe), n.version());
+            case j.DictionaryBatch:
+                return ae.decode(n.header(new rn), n.version())
+        }
+        throw new Error(`Unrecognized Message type: { name: ${j[t]}, type: ${t} }`)
+    }
+}
+tt.encode = Dd;
+tt.decode = Fd;
+tt.fromJSON = fd;
+W.encode = Ad;
+W.decode = bd;
+W.fromJSON = cd;
 Lt.encode = Td;
 Lt.decode = gd;
-Lt.fromJSON = Za;
-re.encode = Nd;
-re.decode = _d;
-re.fromJSON = ud;
-Ge.encode = Md;
-Ge.decode = Sd;
-ee.encode = xd;
-ee.decode = wd;
+Lt.fromJSON = Xa;
+ae.encode = Nd;
+ae.decode = _d;
+ae.fromJSON = ud;
+Ke.encode = xd;
+Ke.decode = Sd;
+ie.encode = Md;
+ie.decode = wd;
 
 function bd(n, t = new Map) {
     const e = Od(n, t);
-    return new j(e, li(n), t)
+    return new W(e, ui(n), t)
 }
 
 function gd(n, t = Nt.V4) {
     if (n.compression() !== null) throw new Error("Record batch compression not implemented");
     return new Lt(n.length(), Id(n), Bd(n, t))
 }
 
 function _d(n, t = Nt.V4) {
-    return new re(Lt.decode(n.data(), t), n.id(), n.isDelta())
+    return new ae(Lt.decode(n.data(), t), n.id(), n.isDelta())
 }
 
 function wd(n) {
-    return new ee(n.offset(), n.length())
+    return new ie(n.offset(), n.length())
 }
 
 function Sd(n) {
-    return new Ge(n.length(), n.nullCount())
+    return new Ke(n.length(), n.nullCount())
 }
 
 function Id(n) {
     const t = [];
-    for (let e, i = -1, r = -1, s = n.nodesLength(); ++i < s;)(e = n.nodes(i)) && (t[++r] = Ge.decode(e));
+    for (let e, i = -1, r = -1, s = n.nodesLength(); ++i < s;)(e = n.nodes(i)) && (t[++r] = Ke.decode(e));
     return t
 }
 
 function Bd(n, t) {
     const e = [];
-    for (let i, r = -1, s = -1, o = n.buffersLength(); ++r < o;)(i = n.buffers(r)) && (t < Nt.V4 && (i.bb_pos += 8 * (r + 1)), e[++s] = ee.decode(i));
+    for (let i, r = -1, s = -1, o = n.buffersLength(); ++r < o;)(i = n.buffers(r)) && (t < Nt.V4 && (i.bb_pos += 8 * (r + 1)), e[++s] = ie.decode(i));
     return e
 }
 
 function Od(n, t) {
     const e = [];
-    for (let i, r = -1, s = -1, o = n.fieldsLength(); ++r < o;)(i = n.fields(r)) && (e[++s] = X.decode(i, t));
+    for (let i, r = -1, s = -1, o = n.fieldsLength(); ++r < o;)(i = n.fields(r)) && (e[++s] = tt.decode(i, t));
     return e
 }
 
-function zs(n, t) {
+function Ws(n, t) {
     const e = [];
-    for (let i, r = -1, s = -1, o = n.childrenLength(); ++r < o;)(i = n.children(r)) && (e[++s] = X.decode(i, t));
+    for (let i, r = -1, s = -1, o = n.childrenLength(); ++r < o;)(i = n.children(r)) && (e[++s] = tt.decode(i, t));
     return e
 }
 
 function Fd(n, t) {
     let e, i, r, s, o, a;
-    return !t || !(a = n.dictionary()) ? (r = Ys(n, zs(n, t)), i = new X(n.name(), r, n.nullable(), li(n))) : t.has(e = a.id().low) ? (s = (s = a.indexType()) ? Ws(s) : new Cn, o = new dn(t.get(e), s, e, a.isOrdered()), i = new X(n.name(), o, n.nullable(), li(n))) : (s = (s = a.indexType()) ? Ws(s) : new Cn, t.set(e, r = Ys(n, zs(n, t))), o = new dn(r, s, e, a.isOrdered()), i = new X(n.name(), o, n.nullable(), li(n))), i || null
+    return !t || !(a = n.dictionary()) ? (r = Gs(n, Ws(n, t)), i = new tt(n.name(), r, n.nullable(), ui(n))) : t.has(e = a.id().low) ? (s = (s = a.indexType()) ? Ys(s) : new kn, o = new pn(t.get(e), s, e, a.isOrdered()), i = new tt(n.name(), o, n.nullable(), ui(n))) : (s = (s = a.indexType()) ? Ys(s) : new kn, t.set(e, r = Gs(n, Ws(n, t))), o = new pn(r, s, e, a.isOrdered()), i = new tt(n.name(), o, n.nullable(), ui(n))), i || null
 }
 
-function li(n) {
+function ui(n) {
     const t = new Map;
     if (n)
         for (let e, i, r = -1, s = Math.trunc(n.customMetadataLength()); ++r < s;)(e = n.customMetadata(r)) && (i = e.key()) != null && t.set(i, e.value());
     return t
 }
 
-function Ws(n) {
-    return new Fe(n.isSigned(), n.bitWidth())
+function Ys(n) {
+    return new Ne(n.isSigned(), n.bitWidth())
 }
 
-function Ys(n, t) {
+function Gs(n, t) {
     const e = n.typeType();
     switch (e) {
-        case Q.NONE:
-            return new Oe;
-        case Q.Null:
-            return new Oe;
-        case Q.Binary:
-            return new ui;
-        case Q.Utf8:
-            return new di;
-        case Q.Bool:
+        case nt.NONE:
+            return new Te;
+        case nt.Null:
+            return new Te;
+        case nt.Binary:
             return new hi;
-        case Q.List:
-            return new vi((t || [])[0]);
-        case Q.Struct_:
-            return new yt(t || [])
+        case nt.Utf8:
+            return new fi;
+        case nt.Bool:
+            return new pi;
+        case nt.List:
+            return new gi((t || [])[0]);
+        case nt.Struct_:
+            return new mt(t || [])
     }
     switch (e) {
-        case Q.Int: {
+        case nt.Int: {
             const i = n.type(new Tt);
-            return new Fe(i.isSigned(), i.bitWidth())
-        }
-        case Q.FloatingPoint: {
-            const i = n.type(new Xt);
-            return new kn(i.precision())
+            return new Ne(i.isSigned(), i.bitWidth())
         }
-        case Q.Decimal: {
-            const i = n.type(new _t);
-            return new fi(i.scale(), i.precision(), i.bitWidth())
+        case nt.FloatingPoint: {
+            const i = n.type(new te);
+            return new Un(i.precision())
         }
-        case Q.Date: {
-            const i = n.type(new ii);
-            return new pi(i.unit())
+        case nt.Decimal: {
+            const i = n.type(new wt);
+            return new yi(i.scale(), i.precision(), i.bitWidth())
         }
-        case Q.Time: {
-            const i = n.type(new kt);
-            return new Un(i.unit(), i.bitWidth())
+        case nt.Date: {
+            const i = n.type(new si);
+            return new mi(i.unit())
         }
-        case Q.Timestamp: {
+        case nt.Time: {
             const i = n.type(new Ut);
-            return new yi(i.unit(), i.timezone())
+            return new $n(i.unit(), i.bitWidth())
         }
-        case Q.Interval: {
-            const i = n.type(new Qt);
-            return new mi(i.unit())
+        case nt.Timestamp: {
+            const i = n.type(new $t);
+            return new vi(i.unit(), i.timezone())
         }
-        case Q.Union: {
-            const i = n.type(new wt);
-            return new bi(i.mode(), i.typeIdsArray() || [], t || [])
+        case nt.Interval: {
+            const i = n.type(new ee);
+            return new bi(i.unit())
         }
-        case Q.FixedSizeBinary: {
-            const i = n.type(new Kt);
-            return new gi(i.byteWidth())
+        case nt.Union: {
+            const i = n.type(new St);
+            return new _i(i.mode(), i.typeIdsArray() || [], t || [])
         }
-        case Q.FixedSizeList: {
-            const i = n.type(new Zt);
-            return new _i(i.listSize(), (t || [])[0])
+        case nt.FixedSizeBinary: {
+            const i = n.type(new Xt);
+            return new wi(i.byteWidth())
         }
-        case Q.Map: {
-            const i = n.type(new ri);
-            return new wi((t || [])[0], i.keysSorted())
+        case nt.FixedSizeList: {
+            const i = n.type(new Qt);
+            return new Si(i.listSize(), (t || [])[0])
+        }
+        case nt.Map: {
+            const i = n.type(new oi);
+            return new Ii((t || [])[0], i.keysSorted())
         }
     }
-    throw new Error(`Unrecognized type: "${Q[e]}" (${e})`)
+    throw new Error(`Unrecognized type: "${nt[e]}" (${e})`)
 }
 
 function Ad(n, t) {
-    const e = t.fields.map(s => X.encode(n, s));
-    Yt.startFieldsVector(n, e.length);
-    const i = Yt.createFieldsVector(n, e),
-        r = t.metadata && t.metadata.size > 0 ? Yt.createCustomMetadataVector(n, [...t.metadata].map(([s, o]) => {
+    const e = t.fields.map(s => tt.encode(n, s));
+    Ht.startFieldsVector(n, e.length);
+    const i = Ht.createFieldsVector(n, e),
+        r = t.metadata && t.metadata.size > 0 ? Ht.createCustomMetadataVector(n, [...t.metadata].map(([s, o]) => {
             const a = n.createString(`${s}`),
                 l = n.createString(`${o}`);
             return ut.startKeyValue(n), ut.addKey(n, a), ut.addValue(n, l), ut.endKeyValue(n)
         })) : -1;
-    return Yt.startSchema(n), Yt.addFields(n, i), Yt.addEndianness(n, Ld ? pn.Little : pn.Big), r !== -1 && Yt.addCustomMetadata(n, r), Yt.endSchema(n)
+    return Ht.startSchema(n), Ht.addFields(n, i), Ht.addEndianness(n, Ld ? vn.Little : vn.Big), r !== -1 && Ht.addCustomMetadata(n, r), Ht.endSchema(n)
 }
 
 function Dd(n, t) {
     let e = -1,
         i = -1,
         r = -1;
     const s = t.type;
     let o = t.typeId;
-    S.isDictionary(s) ? (o = s.dictionary.typeId, r = fr.visit(s, n), i = fr.visit(s.dictionary, n)) : i = fr.visit(s, n);
-    const a = (s.children || []).map(d => X.encode(n, d)),
-        l = Rt.createChildrenVector(n, a),
-        c = t.metadata && t.metadata.size > 0 ? Rt.createCustomMetadataVector(n, [...t.metadata].map(([d, h]) => {
+    I.isDictionary(s) ? (o = s.dictionary.typeId, r = yr.visit(s, n), i = yr.visit(s.dictionary, n)) : i = yr.visit(s, n);
+    const a = (s.children || []).map(d => tt.encode(n, d)),
+        l = Ct.createChildrenVector(n, a),
+        c = t.metadata && t.metadata.size > 0 ? Ct.createCustomMetadataVector(n, [...t.metadata].map(([d, h]) => {
             const y = n.createString(`${d}`),
                 _ = n.createString(`${h}`);
             return ut.startKeyValue(n), ut.addKey(n, y), ut.addValue(n, _), ut.endKeyValue(n)
         })) : -1;
-    return t.name && (e = n.createString(t.name)), Rt.startField(n), Rt.addType(n, i), Rt.addTypeType(n, o), Rt.addChildren(n, l), Rt.addNullable(n, !!t.nullable), e !== -1 && Rt.addName(n, e), r !== -1 && Rt.addDictionary(n, r), c !== -1 && Rt.addCustomMetadata(n, c), Rt.endField(n)
+    return t.name && (e = n.createString(t.name)), Ct.startField(n), Ct.addType(n, i), Ct.addTypeType(n, o), Ct.addChildren(n, l), Ct.addNullable(n, !!t.nullable), e !== -1 && Ct.addName(n, e), r !== -1 && Ct.addDictionary(n, r), c !== -1 && Ct.addCustomMetadata(n, c), Ct.endField(n)
 }
 
 function Td(n, t) {
     const e = t.nodes || [],
         i = t.buffers || [];
-    ce.startNodesVector(n, e.length);
-    for (const o of e.slice().reverse()) Ge.encode(n, o);
+    fe.startNodesVector(n, e.length);
+    for (const o of e.slice().reverse()) Ke.encode(n, o);
     const r = n.endVector();
-    ce.startBuffersVector(n, i.length);
-    for (const o of i.slice().reverse()) ee.encode(n, o);
+    fe.startBuffersVector(n, i.length);
+    for (const o of i.slice().reverse()) ie.encode(n, o);
     const s = n.endVector();
-    return ce.startRecordBatch(n), ce.addLength(n, new We(t.length, 0)), ce.addNodes(n, r), ce.addBuffers(n, s), ce.endRecordBatch(n)
+    return fe.startRecordBatch(n), fe.addLength(n, new qe(t.length, 0)), fe.addNodes(n, r), fe.addBuffers(n, s), fe.endRecordBatch(n)
 }
 
 function Nd(n, t) {
     const e = Lt.encode(n, t.data);
-    return en.startDictionaryBatch(n), en.addId(n, new We(t.id, 0)), en.addIsDelta(n, t.isDelta), en.addData(n, e), en.endDictionaryBatch(n)
+    return rn.startDictionaryBatch(n), rn.addId(n, new qe(t.id, 0)), rn.addIsDelta(n, t.isDelta), rn.addData(n, e), rn.endDictionaryBatch(n)
 }
 
-function Md(n, t) {
-    return Ka.createFieldNode(n, new We(t.length, 0), new We(t.nullCount, 0))
+function xd(n, t) {
+    return Za.createFieldNode(n, new qe(t.length, 0), new qe(t.nullCount, 0))
 }
 
-function xd(n, t) {
-    return Ja.createBuffer(n, new We(t.offset, 0), new We(t.length, 0))
+function Md(n, t) {
+    return Ka.createBuffer(n, new qe(t.offset, 0), new qe(t.length, 0))
 }
 const Ld = (() => {
         const n = new ArrayBuffer(2);
         return new DataView(n).setInt16(0, 256, !0), new Int16Array(n)[0] === 256
     })(),
-    ds = n => `Expected ${$[n]} Message in stream, but was null or length 0.`,
-    hs = n => `Header pointer of flatbuffer-encoded ${$[n]} Message is null or length 0.`,
-    tl = (n, t) => `Expected to read ${n} metadata bytes, but only read ${t}.`,
-    el = (n, t) => `Expected to read ${n} bytes for message body, but only read ${t}.`;
-class nl {
+    ps = n => `Expected ${j[n]} Message in stream, but was null or length 0.`,
+    ys = n => `Header pointer of flatbuffer-encoded ${j[n]} Message is null or length 0.`,
+    el = (n, t) => `Expected to read ${n} metadata bytes, but only read ${t}.`,
+    nl = (n, t) => `Expected to read ${n} bytes for message body, but only read ${t}.`;
+class il {
     constructor(t) {
-        this.source = t instanceof Ni ? t : new Ni(t)
+        this.source = t instanceof Mi ? t : new Mi(t)
     } [Symbol.iterator]() {
         return this
     }
     next() {
         let t;
-        return (t = this.readMetadataLength()).done || t.value === -1 && (t = this.readMetadataLength()).done || (t = this.readMetadata(t.value)).done ? tt : t
+        return (t = this.readMetadataLength()).done || t.value === -1 && (t = this.readMetadataLength()).done || (t = this.readMetadata(t.value)).done ? it : t
     }
     throw (t) {
         return this.source.throw(t)
     }
     return (t) {
         return this.source.return(t)
     }
     readMessage(t) {
         let e;
         if ((e = this.next()).done) return null;
-        if (t != null && e.value.headerType !== t) throw new Error(ds(t));
+        if (t != null && e.value.headerType !== t) throw new Error(ps(t));
         return e.value
     }
     readMessageBody(t) {
         if (t <= 0) return new Uint8Array(0);
         const e = U(this.source.read(t));
-        if (e.byteLength < t) throw new Error(el(t, e.byteLength));
+        if (e.byteLength < t) throw new Error(nl(t, e.byteLength));
         return e.byteOffset % 8 === 0 && e.byteOffset + e.byteLength <= e.buffer.byteLength ? e : e.slice()
     }
     readSchema(t = !1) {
-        const e = $.Schema,
+        const e = j.Schema,
             i = this.readMessage(e),
             r = i?.header();
-        if (t && !r) throw new Error(hs(e));
+        if (t && !r) throw new Error(ys(e));
         return r
     }
     readMetadataLength() {
-        const t = this.source.read(nr),
-            e = t && new hn(t),
+        const t = this.source.read(rr),
+            e = t && new yn(t),
             i = e?.readInt32(0) || 0;
         return {
             done: i === 0,
             value: i
         }
     }
     readMetadata(t) {
         const e = this.source.read(t);
-        if (!e) return tt;
-        if (e.byteLength < t) throw new Error(tl(t, e.byteLength));
+        if (!e) return it;
+        if (e.byteLength < t) throw new Error(el(t, e.byteLength));
         return {
             done: !1,
-            value: mt.decode(e)
+            value: vt.decode(e)
         }
     }
 }
 class Ed {
     constructor(t, e) {
-        this.source = t instanceof mn ? t : Io(t) ? new Mi(t, e) : new mn(t)
+        this.source = t instanceof gn ? t : Bo(t) ? new Li(t, e) : new gn(t)
     } [Symbol.asyncIterator]() {
         return this
     }
     next() {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             let t;
-            return (t = yield this.readMetadataLength()).done || t.value === -1 && (t = yield this.readMetadataLength()).done || (t = yield this.readMetadata(t.value)).done ? tt : t
+            return (t = yield this.readMetadataLength()).done || t.value === -1 && (t = yield this.readMetadataLength()).done || (t = yield this.readMetadata(t.value)).done ? it : t
         })
     }
     throw (t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return yield this.source.throw(t)
         })
     }
     return (t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return yield this.source.return(t)
         })
     }
     readMessage(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             let e;
             if ((e = yield this.next()).done) return null;
-            if (t != null && e.value.headerType !== t) throw new Error(ds(t));
+            if (t != null && e.value.headerType !== t) throw new Error(ps(t));
             return e.value
         })
     }
     readMessageBody(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             if (t <= 0) return new Uint8Array(0);
             const e = U(yield this.source.read(t));
-            if (e.byteLength < t) throw new Error(el(t, e.byteLength));
+            if (e.byteLength < t) throw new Error(nl(t, e.byteLength));
             return e.byteOffset % 8 === 0 && e.byteOffset + e.byteLength <= e.buffer.byteLength ? e : e.slice()
         })
     }
     readSchema(t = !1) {
-        return w(this, void 0, void 0, function*() {
-            const e = $.Schema,
+        return S(this, void 0, void 0, function*() {
+            const e = j.Schema,
                 i = yield this.readMessage(e), r = i?.header();
-            if (t && !r) throw new Error(hs(e));
+            if (t && !r) throw new Error(ys(e));
             return r
         })
     }
     readMetadataLength() {
-        return w(this, void 0, void 0, function*() {
-            const t = yield this.source.read(nr), e = t && new hn(t), i = e?.readInt32(0) || 0;
+        return S(this, void 0, void 0, function*() {
+            const t = yield this.source.read(rr), e = t && new yn(t), i = e?.readInt32(0) || 0;
             return {
                 done: i === 0,
                 value: i
             }
         })
     }
     readMetadata(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const e = yield this.source.read(t);
-            if (!e) return tt;
-            if (e.byteLength < t) throw new Error(tl(t, e.byteLength));
+            if (!e) return it;
+            if (e.byteLength < t) throw new Error(el(t, e.byteLength));
             return {
                 done: !1,
-                value: mt.decode(e)
+                value: vt.decode(e)
             }
         })
     }
 }
-class Rd extends nl {
+class Rd extends il {
     constructor(t) {
-        super(new Uint8Array(0)), this._schema = !1, this._body = [], this._batchIndex = 0, this._dictionaryIndex = 0, this._json = t instanceof ks ? t : new ks(t)
+        super(new Uint8Array(0)), this._schema = !1, this._body = [], this._batchIndex = 0, this._dictionaryIndex = 0, this._json = t instanceof Us ? t : new Us(t)
     }
     next() {
         const {
             _json: t
         } = this;
         if (!this._schema) return this._schema = !0, {
             done: !1,
-            value: mt.fromJSON(t.schema, $.Schema)
+            value: vt.fromJSON(t.schema, j.Schema)
         };
         if (this._dictionaryIndex < t.dictionaries.length) {
             const e = t.dictionaries[this._dictionaryIndex++];
             return this._body = e.data.columns, {
                 done: !1,
-                value: mt.fromJSON(e, $.DictionaryBatch)
+                value: vt.fromJSON(e, j.DictionaryBatch)
             }
         }
         if (this._batchIndex < t.batches.length) {
             const e = t.batches[this._batchIndex++];
             return this._body = e.columns, {
                 done: !1,
-                value: mt.fromJSON(e, $.RecordBatch)
+                value: vt.fromJSON(e, j.RecordBatch)
             }
         }
-        return this._body = [], tt
+        return this._body = [], it
     }
     readMessageBody(t) {
         return e(this._body);
 
         function e(i) {
             return (i || []).reduce((r, s) => [...r, ...s.VALIDITY && [s.VALIDITY] || [], ...s.TYPE && [s.TYPE] || [], ...s.OFFSET && [s.OFFSET] || [], ...s.DATA && [s.DATA] || [], ...e(s.children)], [])
         }
     }
     readMessage(t) {
         let e;
         if ((e = this.next()).done) return null;
-        if (t != null && e.value.headerType !== t) throw new Error(ds(t));
+        if (t != null && e.value.headerType !== t) throw new Error(ps(t));
         return e.value
     }
     readSchema() {
-        const t = $.Schema,
+        const t = j.Schema,
             e = this.readMessage(t),
             i = e?.header();
-        if (!e || !i) throw new Error(hs(t));
+        if (!e || !i) throw new Error(ys(t));
         return i
     }
 }
-const nr = 4,
-    Mr = "ARROW1",
-    $n = new Uint8Array(Mr.length);
-for (let n = 0; n < Mr.length; n += 1) $n[n] = Mr.codePointAt(n);
-
-function fs(n, t = 0) {
-    for (let e = -1, i = $n.length; ++e < i;)
-        if ($n[e] !== n[t + e]) return !1;
+const rr = 4,
+    Er = "ARROW1",
+    Pn = new Uint8Array(Er.length);
+for (let n = 0; n < Er.length; n += 1) Pn[n] = Er.codePointAt(n);
+
+function ms(n, t = 0) {
+    for (let e = -1, i = Pn.length; ++e < i;)
+        if (Pn[e] !== n[t + e]) return !1;
     return !0
 }
-const Kn = $n.length,
-    il = Kn + nr,
-    Cd = Kn * 2 + nr;
-class fe extends ss {
+const Kn = Pn.length,
+    rl = Kn + rr,
+    Cd = Kn * 2 + rr;
+class ve extends ls {
     constructor(t) {
         super(), this._impl = t
     }
     get closed() {
         return this._impl.closed
     }
     get schema() {
@@ -7637,78 +7637,78 @@
         return this._impl.cancel()
     }
     reset(t) {
         return this._impl.reset(t), this._DOMStream = void 0, this._nodeStream = void 0, this
     }
     open(t) {
         const e = this._impl.open(t);
-        return Ie(e) ? e.then(() => this) : this
+        return Ae(e) ? e.then(() => this) : this
     }
     readRecordBatch(t) {
         return this._impl.isFile() ? this._impl.readRecordBatch(t) : null
     } [Symbol.iterator]() {
         return this._impl[Symbol.iterator]()
     } [Symbol.asyncIterator]() {
         return this._impl[Symbol.asyncIterator]()
     }
     toDOMStream() {
-        return Ct.toDOMStream(this.isSync() ? {
+        return kt.toDOMStream(this.isSync() ? {
             [Symbol.iterator]: () => this
         } : {
             [Symbol.asyncIterator]: () => this
         })
     }
     toNodeStream() {
-        return Ct.toNodeStream(this.isSync() ? {
+        return kt.toNodeStream(this.isSync() ? {
             [Symbol.iterator]: () => this
         } : {
             [Symbol.asyncIterator]: () => this
         }, {
             objectMode: !0
         })
     }
     static throughNode(t) {
         throw new Error('"throughNode" not available in this environment')
     }
     static throughDOM(t, e) {
         throw new Error('"throughDOM" not available in this environment')
     }
     static from(t) {
-        return t instanceof fe ? t : _r(t) ? $d(t) : Io(t) ? zd(t) : Ie(t) ? w(this, void 0, void 0, function*() {
-            return yield fe.from(yield t)
-        }) : Bo(t) || Yr(t) || Oo(t) || gn(t) ? jd(new mn(t)) : Pd(new Ni(t))
+        return t instanceof ve ? t : Ir(t) ? Vd(t) : Bo(t) ? zd(t) : Ae(t) ? S(this, void 0, void 0, function*() {
+            return yield ve.from(yield t)
+        }) : Oo(t) || qr(t) || Fo(t) || In(t) ? jd(new gn(t)) : Pd(new Mi(t))
     }
     static readAll(t) {
-        return t instanceof fe ? t.isSync() ? Gs(t) : Hs(t) : _r(t) || ArrayBuffer.isView(t) || Gn(t) || So(t) ? Gs(t) : Hs(t)
+        return t instanceof ve ? t.isSync() ? Hs(t) : qs(t) : Ir(t) || ArrayBuffer.isView(t) || Gn(t) || Io(t) ? Hs(t) : qs(t)
     }
 }
-class Ri extends fe {
+class ki extends ve {
     constructor(t) {
         super(t), this._impl = t
     }
     readAll() {
         return [...this]
     } [Symbol.iterator]() {
         return this._impl[Symbol.iterator]()
     } [Symbol.asyncIterator]() {
-        return te(this, arguments, function*() {
-            yield M(yield* ni(je(this[Symbol.iterator]())))
+        return ne(this, arguments, function*() {
+            yield M(yield* ri(Ye(this[Symbol.iterator]())))
         })
     }
 }
-class Ci extends fe {
+class Ui extends ve {
     constructor(t) {
         super(t), this._impl = t
     }
     readAll() {
         var t, e;
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const i = new Array;
             try {
-                for (var r = je(this), s; s = yield r.next(), !s.done;) {
+                for (var r = Ye(this), s; s = yield r.next(), !s.done;) {
                     const o = s.value;
                     i.push(o)
                 }
             } catch (o) {
                 t = {
                     error: o
                 }
@@ -7723,25 +7723,25 @@
         })
     } [Symbol.iterator]() {
         throw new Error("AsyncRecordBatchStreamReader is not Iterable")
     } [Symbol.asyncIterator]() {
         return this._impl[Symbol.asyncIterator]()
     }
 }
-class rl extends Ri {
+class sl extends ki {
     constructor(t) {
         super(t), this._impl = t
     }
 }
-class kd extends Ci {
+class kd extends Ui {
     constructor(t) {
         super(t), this._impl = t
     }
 }
-class sl {
+class ol {
     constructor(t = new Map) {
         this.closed = !1, this.autoDestroy = !0, this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.dictionaries = t
     }
     get numDictionaries() {
         return this._dictionaryIndex
     }
     get numRecordBatches() {
@@ -7761,65 +7761,65 @@
     }
     reset(t) {
         return this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.schema = t, this.dictionaries = new Map, this
     }
     _loadRecordBatch(t, e) {
         const i = this._loadVectors(t, e, this.schema.fields),
             r = E({
-                type: new yt(this.schema.fields),
+                type: new mt(this.schema.fields),
                 length: t.length,
                 children: i
             });
-        return new St(this.schema, r)
+        return new It(this.schema, r)
     }
     _loadDictionaryBatch(t, e) {
         const {
             id: i,
             isDelta: r
         } = t, {
             dictionaries: s,
             schema: o
         } = this, a = s.get(i);
         if (r || !a) {
             const l = o.dictionaries.get(i),
                 c = this._loadVectors(t.data, e, [l]);
-            return (a && r ? a.concat(new P(c)) : new P(c)).memoize()
+            return (a && r ? a.concat(new z(c)) : new z(c)).memoize()
         }
         return a.memoize()
     }
     _loadVectors(t, e, i) {
-        return new Ya(e, t.nodes, t.buffers, this.dictionaries).visitMany(i)
+        return new Ga(e, t.nodes, t.buffers, this.dictionaries).visitMany(i)
     }
 }
-class ki extends sl {
+class $i extends ol {
     constructor(t, e) {
-        super(e), this._reader = _r(t) ? new Rd(this._handle = t) : new nl(this._handle = t)
+        super(e), this._reader = Ir(t) ? new Rd(this._handle = t) : new il(this._handle = t)
     }
     isSync() {
         return !0
     }
     isStream() {
         return !0
     } [Symbol.iterator]() {
         return this
     }
     cancel() {
         !this.closed && (this.closed = !0) && (this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
     }
     open(t) {
-        return this.closed || (this.autoDestroy = al(this, t), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
+        return this.closed || (this.autoDestroy = ll(this, t), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
     }
     throw (t) {
-        return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.throw(t) : tt
+        return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.throw(t) : it
     }
     return (t) {
-        return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.return(t) : tt
+        return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.return(t) : it
     }
     next() {
-        if (this.closed) return tt;
+        if (this.closed) return it;
         let t;
         const {
             _reader: e
         } = this;
         for (; t = this._readNextMessageAndValidate();)
             if (t.isSchema()) this.reset(t.header());
             else if (t.isRecordBatch()) {
@@ -7835,56 +7835,56 @@
             const i = t.header(),
                 r = e.readMessageBody(t.bodyLength),
                 s = this._loadDictionaryBatch(i, r);
             this.dictionaries.set(i.id, s)
         }
         return this.schema && this._recordBatchIndex === 0 ? (this._recordBatchIndex++, {
             done: !1,
-            value: new us(this.schema)
+            value: new fs(this.schema)
         }) : this.return()
     }
     _readNextMessageAndValidate(t) {
         return this._reader.readMessage(t)
     }
 }
-class Ui extends sl {
+class Vi extends ol {
     constructor(t, e) {
         super(e), this._reader = new Ed(this._handle = t)
     }
     isAsync() {
         return !0
     }
     isStream() {
         return !0
     } [Symbol.asyncIterator]() {
         return this
     }
     cancel() {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             !this.closed && (this.closed = !0) && (yield this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
         })
     }
     open(t) {
-        return w(this, void 0, void 0, function*() {
-            return this.closed || (this.autoDestroy = al(this, t), this.schema || (this.schema = yield this._reader.readSchema()) || (yield this.cancel())), this
+        return S(this, void 0, void 0, function*() {
+            return this.closed || (this.autoDestroy = ll(this, t), this.schema || (this.schema = yield this._reader.readSchema()) || (yield this.cancel())), this
         })
     }
     throw (t) {
-        return w(this, void 0, void 0, function*() {
-            return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.throw(t): tt
+        return S(this, void 0, void 0, function*() {
+            return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.throw(t): it
         })
     }
     return (t) {
-        return w(this, void 0, void 0, function*() {
-            return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.return(t): tt
+        return S(this, void 0, void 0, function*() {
+            return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.return(t): it
         })
     }
     next() {
-        return w(this, void 0, void 0, function*() {
-            if (this.closed) return tt;
+        return S(this, void 0, void 0, function*() {
+            if (this.closed) return it;
             let t;
             const {
                 _reader: e
             } = this;
             for (; t = yield this._readNextMessageAndValidate();)
                 if (t.isSchema()) yield this.reset(t.header());
                 else if (t.isRecordBatch()) {
@@ -7899,27 +7899,27 @@
                 this._dictionaryIndex++;
                 const i = t.header(),
                     r = yield e.readMessageBody(t.bodyLength), s = this._loadDictionaryBatch(i, r);
                 this.dictionaries.set(i.id, s)
             }
             return this.schema && this._recordBatchIndex === 0 ? (this._recordBatchIndex++, {
                 done: !1,
-                value: new us(this.schema)
+                value: new fs(this.schema)
             }) : yield this.return()
         })
     }
     _readNextMessageAndValidate(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             return yield this._reader.readMessage(t)
         })
     }
 }
-class ol extends ki {
+class al extends $i {
     constructor(t, e) {
-        super(t instanceof Us ? t : new Us(t), e)
+        super(t instanceof $s ? t : new $s(t), e)
     }
     get footer() {
         return this._footer
     }
     get numDictionaries() {
         return this._footer ? this._footer.numDictionaries : 0
     }
@@ -7941,56 +7941,56 @@
     }
     readRecordBatch(t) {
         var e;
         if (this.closed) return null;
         this._footer || this.open();
         const i = (e = this._footer) === null || e === void 0 ? void 0 : e.getRecordBatch(t);
         if (i && this._handle.seek(i.offset)) {
-            const r = this._reader.readMessage($.RecordBatch);
+            const r = this._reader.readMessage(j.RecordBatch);
             if (r?.isRecordBatch()) {
                 const s = r.header(),
                     o = this._reader.readMessageBody(r.bodyLength);
                 return this._loadRecordBatch(s, o)
             }
         }
         return null
     }
     _readDictionaryBatch(t) {
         var e;
         const i = (e = this._footer) === null || e === void 0 ? void 0 : e.getDictionaryBatch(t);
         if (i && this._handle.seek(i.offset)) {
-            const r = this._reader.readMessage($.DictionaryBatch);
+            const r = this._reader.readMessage(j.DictionaryBatch);
             if (r?.isDictionaryBatch()) {
                 const s = r.header(),
                     o = this._reader.readMessageBody(r.bodyLength),
                     a = this._loadDictionaryBatch(s, o);
                 this.dictionaries.set(s.id, a)
             }
         }
     }
     _readFooter() {
         const {
             _handle: t
-        } = this, e = t.size - il, i = t.readInt32(e), r = t.readAt(e - i, i);
+        } = this, e = t.size - rl, i = t.readInt32(e), r = t.readAt(e - i, i);
         return Vn.decode(r)
     }
     _readNextMessageAndValidate(t) {
         var e;
         if (this._footer || this.open(), this._footer && this._recordBatchIndex < this.numRecordBatches) {
             const i = (e = this._footer) === null || e === void 0 ? void 0 : e.getRecordBatch(this._recordBatchIndex);
             if (i && this._handle.seek(i.offset)) return this._reader.readMessage(t)
         }
         return null
     }
 }
-class Ud extends Ui {
+class Ud extends Vi {
     constructor(t, ...e) {
         const i = typeof e[0] != "number" ? e.shift() : void 0,
             r = e[0] instanceof Map ? e.shift() : void 0;
-        super(t instanceof Mi ? t : new Mi(t, i), r)
+        super(t instanceof Li ? t : new Li(t, i), r)
     }
     get footer() {
         return this._footer
     }
     get numDictionaries() {
         return this._footer ? this._footer.numDictionaries : 0
     }
@@ -8005,160 +8005,160 @@
     }
     open(t) {
         const e = Object.create(null, {
             open: {
                 get: () => super.open
             }
         });
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             if (!this.closed && !this._footer) {
                 this.schema = (this._footer = yield this._readFooter()).schema;
                 for (const i of this._footer.dictionaryBatches()) i && (yield this._readDictionaryBatch(this._dictionaryIndex++))
             }
             return yield e.open.call(this, t)
         })
     }
     readRecordBatch(t) {
         var e;
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             if (this.closed) return null;
             this._footer || (yield this.open());
             const i = (e = this._footer) === null || e === void 0 ? void 0 : e.getRecordBatch(t);
             if (i && (yield this._handle.seek(i.offset))) {
-                const r = yield this._reader.readMessage($.RecordBatch);
+                const r = yield this._reader.readMessage(j.RecordBatch);
                 if (r?.isRecordBatch()) {
                     const s = r.header(),
                         o = yield this._reader.readMessageBody(r.bodyLength);
                     return this._loadRecordBatch(s, o)
                 }
             }
             return null
         })
     }
     _readDictionaryBatch(t) {
         var e;
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const i = (e = this._footer) === null || e === void 0 ? void 0 : e.getDictionaryBatch(t);
             if (i && (yield this._handle.seek(i.offset))) {
-                const r = yield this._reader.readMessage($.DictionaryBatch);
+                const r = yield this._reader.readMessage(j.DictionaryBatch);
                 if (r?.isDictionaryBatch()) {
                     const s = r.header(),
                         o = yield this._reader.readMessageBody(r.bodyLength), a = this._loadDictionaryBatch(s, o);
                     this.dictionaries.set(s.id, a)
                 }
             }
         })
     }
     _readFooter() {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             const {
                 _handle: t
             } = this;
             t._pending && (yield t._pending);
-            const e = t.size - il,
+            const e = t.size - rl,
                 i = yield t.readInt32(e), r = yield t.readAt(e - i, i);
             return Vn.decode(r)
         })
     }
     _readNextMessageAndValidate(t) {
-        return w(this, void 0, void 0, function*() {
+        return S(this, void 0, void 0, function*() {
             if (this._footer || (yield this.open()), this._footer && this._recordBatchIndex < this.numRecordBatches) {
                 const e = this._footer.getRecordBatch(this._recordBatchIndex);
                 if (e && (yield this._handle.seek(e.offset))) return yield this._reader.readMessage(t)
             }
             return null
         })
     }
 }
-class Vd extends ki {
+class $d extends $i {
     constructor(t, e) {
         super(t, e)
     }
     _loadVectors(t, e, i) {
         return new Zu(e, t.nodes, t.buffers, this.dictionaries).visitMany(i)
     }
 }
 
-function al(n, t) {
+function ll(n, t) {
     return t && typeof t.autoDestroy == "boolean" ? t.autoDestroy : n.autoDestroy
 }
 
-function* Gs(n) {
-    const t = fe.from(n);
+function* Hs(n) {
+    const t = ve.from(n);
     try {
         if (!t.open({
                 autoDestroy: !1
             }).closed)
             do yield t; while (!t.reset().open().closed)
     } finally {
         t.cancel()
     }
 }
 
-function Hs(n) {
-    return te(this, arguments, function*() {
-        const e = yield M(fe.from(n));
+function qs(n) {
+    return ne(this, arguments, function*() {
+        const e = yield M(ve.from(n));
         try {
             if (!(yield M(e.open({
                     autoDestroy: !1
                 }))).closed)
                 do yield yield M(e); while (!(yield M(e.reset().open())).closed)
         } finally {
             yield M(e.cancel())
         }
     })
 }
 
-function $d(n) {
-    return new Ri(new Vd(n))
+function Vd(n) {
+    return new ki(new $d(n))
 }
 
 function Pd(n) {
     const t = n.peek(Kn + 7 & -8);
-    return t && t.byteLength >= 4 ? fs(t) ? new rl(new ol(n.read())) : new Ri(new ki(n)) : new Ri(new ki(function*() {}()))
+    return t && t.byteLength >= 4 ? ms(t) ? new sl(new al(n.read())) : new ki(new $i(n)) : new ki(new $i(function*() {}()))
 }
 
 function jd(n) {
-    return w(this, void 0, void 0, function*() {
+    return S(this, void 0, void 0, function*() {
         const t = yield n.peek(Kn + 7 & -8);
-        return t && t.byteLength >= 4 ? fs(t) ? new rl(new ol(yield n.read())) : new Ci(new Ui(n)) : new Ci(new Ui(function() {
-            return te(this, arguments, function*() {})
+        return t && t.byteLength >= 4 ? ms(t) ? new sl(new al(yield n.read())) : new Ui(new Vi(n)) : new Ui(new Vi(function() {
+            return ne(this, arguments, function*() {})
         }()))
     })
 }
 
 function zd(n) {
-    return w(this, void 0, void 0, function*() {
+    return S(this, void 0, void 0, function*() {
         const {
             size: t
-        } = yield n.stat(), e = new Mi(n, t);
-        return t >= Cd && fs(yield e.readAt(0, Kn + 7 & -8)) ? new kd(new Ud(e)) : new Ci(new Ui(e))
+        } = yield n.stat(), e = new Li(n, t);
+        return t >= Cd && ms(yield e.readAt(0, Kn + 7 & -8)) ? new kd(new Ud(e)) : new Ui(new Vi(e))
     })
 }
-class st extends R {
+class ot extends R {
     constructor() {
         super(), this._byteLength = 0, this._nodes = [], this._buffers = [], this._bufferRegions = []
     }
     static assemble(...t) {
-        const e = r => r.flatMap(s => Array.isArray(s) ? e(s) : s instanceof St ? s.data.children : s.data),
-            i = new st;
+        const e = r => r.flatMap(s => Array.isArray(s) ? e(s) : s instanceof It ? s.data.children : s.data),
+            i = new ot;
         return i.visitMany(e(t)), i
     }
     visit(t) {
-        if (t instanceof P) return this.visitMany(t.data), this;
+        if (t instanceof z) return this.visitMany(t.data), this;
         const {
             type: e
         } = t;
-        if (!S.isDictionary(e)) {
+        if (!I.isDictionary(e)) {
             const {
                 length: i,
                 nullCount: r
             } = t;
             if (i > 2147483647) throw new RangeError("Cannot write arrays larger than 2^31 - 1 in length");
-            S.isNull(e) || Pt.call(this, r <= 0 ? new Uint8Array(0) : ts(t.offset, i, t.nullBitmap)), this.nodes.push(new Ge(i, r))
+            I.isNull(e) || jt.call(this, r <= 0 ? new Uint8Array(0) : is(t.offset, i, t.nullBitmap)), this.nodes.push(new Ke(i, r))
         }
         return super.visit(t)
     }
     visitNull(t) {
         return this
     }
     visitDictionary(t) {
@@ -8174,96 +8174,96 @@
         return this._byteLength
     }
     get bufferRegions() {
         return this._bufferRegions
     }
 }
 
-function Pt(n) {
+function jt(n) {
     const t = n.byteLength + 7 & -8;
-    return this.buffers.push(n), this.bufferRegions.push(new ee(this._byteLength, t)), this._byteLength += t, this
+    return this.buffers.push(n), this.bufferRegions.push(new ie(this._byteLength, t)), this._byteLength += t, this
 }
 
 function Wd(n) {
     const {
         type: t,
         length: e,
         typeIds: i,
         valueOffsets: r
     } = n;
-    if (Pt.call(this, i), t.mode === xt.Sparse) return xr.call(this, n);
-    if (t.mode === xt.Dense) {
-        if (n.offset <= 0) return Pt.call(this, r), xr.call(this, n);
+    if (jt.call(this, i), t.mode === Mt.Sparse) return Rr.call(this, n);
+    if (t.mode === Mt.Dense) {
+        if (n.offset <= 0) return jt.call(this, r), Rr.call(this, n);
         {
             const s = i.reduce((d, h) => Math.max(d, h), i[0]),
                 o = new Int32Array(s + 1),
                 a = new Int32Array(s + 1).fill(-1),
                 l = new Int32Array(e),
-                c = Hr(-r[0], e, r);
+                c = Kr(-r[0], e, r);
             for (let d, h, y = -1; ++y < e;)(h = a[d = i[y]]) === -1 && (h = a[d] = c[d]), l[y] = c[y] - h, ++o[d];
-            Pt.call(this, l);
+            jt.call(this, l);
             for (let d, h = -1, y = t.children.length; ++h < y;)
                 if (d = n.children[h]) {
                     const _ = t.typeIds[h],
-                        G = Math.min(e, o[_]);
-                    this.visit(d.slice(a[_], G))
+                        V = Math.min(e, o[_]);
+                    this.visit(d.slice(a[_], V))
                 }
         }
     }
     return this
 }
 
 function Yd(n) {
     let t;
-    return n.nullCount >= n.length ? Pt.call(this, new Uint8Array(0)) : (t = n.values) instanceof Uint8Array ? Pt.call(this, ts(n.offset, n.length, t)) : Pt.call(this, Si(n.values))
+    return n.nullCount >= n.length ? jt.call(this, new Uint8Array(0)) : (t = n.values) instanceof Uint8Array ? jt.call(this, is(n.offset, n.length, t)) : jt.call(this, Bi(n.values))
 }
 
-function Me(n) {
-    return Pt.call(this, n.values.subarray(0, n.length * n.stride))
+function Re(n) {
+    return jt.call(this, n.values.subarray(0, n.length * n.stride))
 }
 
-function ll(n) {
+function cl(n) {
     const {
         length: t,
         values: e,
         valueOffsets: i
     } = n, r = i[0], s = i[t], o = Math.min(s - r, e.byteLength - r);
-    return Pt.call(this, Hr(-i[0], t, i)), Pt.call(this, e.subarray(r, r + o)), this
+    return jt.call(this, Kr(-i[0], t, i)), jt.call(this, e.subarray(r, r + o)), this
 }
 
-function ps(n) {
+function vs(n) {
     const {
         length: t,
         valueOffsets: e
     } = n;
-    return e && Pt.call(this, Hr(e[0], t, e)), this.visit(n.children[0])
+    return e && jt.call(this, Kr(e[0], t, e)), this.visit(n.children[0])
 }
 
-function xr(n) {
+function Rr(n) {
     return this.visitMany(n.type.children.map((t, e) => n.children[e]).filter(Boolean))[0]
 }
-st.prototype.visitBool = Yd;
-st.prototype.visitInt = Me;
-st.prototype.visitFloat = Me;
-st.prototype.visitUtf8 = ll;
-st.prototype.visitBinary = ll;
-st.prototype.visitFixedSizeBinary = Me;
-st.prototype.visitDate = Me;
-st.prototype.visitTimestamp = Me;
-st.prototype.visitTime = Me;
-st.prototype.visitDecimal = Me;
-st.prototype.visitList = ps;
-st.prototype.visitStruct = xr;
-st.prototype.visitUnion = Wd;
-st.prototype.visitInterval = Me;
-st.prototype.visitFixedSizeList = ps;
-st.prototype.visitMap = ps;
-class cl extends ss {
+ot.prototype.visitBool = Yd;
+ot.prototype.visitInt = Re;
+ot.prototype.visitFloat = Re;
+ot.prototype.visitUtf8 = cl;
+ot.prototype.visitBinary = cl;
+ot.prototype.visitFixedSizeBinary = Re;
+ot.prototype.visitDate = Re;
+ot.prototype.visitTimestamp = Re;
+ot.prototype.visitTime = Re;
+ot.prototype.visitDecimal = Re;
+ot.prototype.visitList = vs;
+ot.prototype.visitStruct = Rr;
+ot.prototype.visitUnion = Wd;
+ot.prototype.visitInterval = Re;
+ot.prototype.visitFixedSizeList = vs;
+ot.prototype.visitMap = vs;
+class ul extends ls {
     constructor(t) {
-        super(), this._position = 0, this._started = !1, this._sink = new oi, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, Ot(t) || (t = {
+        super(), this._position = 0, this._started = !1, this._sink = new li, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, Ot(t) || (t = {
             autoDestroy: !0,
             writeLegacyIpcFormat: !1
         }), this._autoDestroy = typeof t.autoDestroy == "boolean" ? t.autoDestroy : !0, this._writeLegacyIpcFormat = typeof t.writeLegacyIpcFormat == "boolean" ? t.writeLegacyIpcFormat : !1
     }
     static throughNode(t) {
         throw new Error('"throughNode" not available in this environment')
     }
@@ -8273,15 +8273,15 @@
     toString(t = !1) {
         return this._sink.toString(t)
     }
     toUint8Array(t = !1) {
         return this._sink.toUint8Array(t)
     }
     writeAll(t) {
-        return Ie(t) ? t.then(e => this.writeAll(e)) : gn(t) ? bs(this, t) : vs(this, t)
+        return Ae(t) ? t.then(e => this.writeAll(e)) : In(t) ? ws(this, t) : _s(this, t)
     }
     get closed() {
         return this._sink.closed
     } [Symbol.asyncIterator]() {
         return this._sink[Symbol.asyncIterator]()
     }
     toDOMStream(t) {
@@ -8296,78 +8296,78 @@
     abort(t) {
         return this.reset()._sink.abort(t)
     }
     finish() {
         return this._autoDestroy ? this.close() : this.reset(this._sink, this._schema), this
     }
     reset(t = this._sink, e = null) {
-        return t === this._sink || t instanceof oi ? this._sink = t : (this._sink = new oi, t && hc(t) ? this.toDOMStream({
+        return t === this._sink || t instanceof li ? this._sink = t : (this._sink = new li, t && hc(t) ? this.toDOMStream({
             type: "bytes"
         }).pipeTo(t) : t && fc(t) && this.toNodeStream({
             objectMode: !1
-        }).pipe(t)), this._started && this._schema && this._writeFooter(this._schema), this._started = !1, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, (!e || !Dr(e, this._schema)) && (e == null ? (this._position = 0, this._schema = null) : (this._started = !0, this._schema = e, this._writeSchema(e))), this
+        }).pipe(t)), this._started && this._schema && this._writeFooter(this._schema), this._started = !1, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, (!e || !xr(e, this._schema)) && (e == null ? (this._position = 0, this._schema = null) : (this._started = !0, this._schema = e, this._writeSchema(e))), this
     }
     write(t) {
         let e = null;
         if (this._sink) {
             if (t == null) return this.finish() && void 0;
-            if (t instanceof pt && !(e = t.schema)) return this.finish() && void 0;
-            if (t instanceof St && !(e = t.schema)) return this.finish() && void 0
+            if (t instanceof yt && !(e = t.schema)) return this.finish() && void 0;
+            if (t instanceof It && !(e = t.schema)) return this.finish() && void 0
         } else throw new Error("RecordBatchWriter is closed");
-        if (e && !Dr(e, this._schema)) {
+        if (e && !xr(e, this._schema)) {
             if (this._started && this._autoDestroy) return this.close();
             this.reset(this._sink, e)
         }
-        t instanceof St ? t instanceof us || this._writeRecordBatch(t) : t instanceof pt ? this.writeAll(t.batches) : Gn(t) && this.writeAll(t)
+        t instanceof It ? t instanceof fs || this._writeRecordBatch(t) : t instanceof yt ? this.writeAll(t.batches) : Gn(t) && this.writeAll(t)
     }
     _writeMessage(t, e = 8) {
         const i = e - 1,
-            r = mt.encode(t),
+            r = vt.encode(t),
             s = r.byteLength,
             o = this._writeLegacyIpcFormat ? 4 : 8,
             a = s + o + i & ~i,
             l = a - s - o;
-        return t.headerType === $.RecordBatch ? this._recordBatchBlocks.push(new Ae(a, t.bodyLength, this._position)) : t.headerType === $.DictionaryBatch && this._dictionaryBlocks.push(new Ae(a, t.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(a - o)), s > 0 && this._write(r), this._writePadding(l)
+        return t.headerType === j.RecordBatch ? this._recordBatchBlocks.push(new xe(a, t.bodyLength, this._position)) : t.headerType === j.DictionaryBatch && this._dictionaryBlocks.push(new xe(a, t.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(a - o)), s > 0 && this._write(r), this._writePadding(l)
     }
     _write(t) {
         if (this._started) {
             const e = U(t);
             e && e.byteLength > 0 && (this._sink.write(e), this._position += e.byteLength)
         }
         return this
     }
     _writeSchema(t) {
-        return this._writeMessage(mt.from(t))
+        return this._writeMessage(vt.from(t))
     }
     _writeFooter(t) {
         return this._writeLegacyIpcFormat ? this._write(Int32Array.of(0)) : this._write(Int32Array.of(-1, 0))
     }
     _writeMagic() {
-        return this._write($n)
+        return this._write(Pn)
     }
     _writePadding(t) {
         return t > 0 ? this._write(new Uint8Array(t)) : this
     }
     _writeRecordBatch(t) {
         const {
             byteLength: e,
             nodes: i,
             bufferRegions: r,
             buffers: s
-        } = st.assemble(t), o = new Lt(t.numRows, i, r), a = mt.from(o, e);
+        } = ot.assemble(t), o = new Lt(t.numRows, i, r), a = vt.from(o, e);
         return this._writeDictionaries(t)._writeMessage(a)._writeBodyBuffers(s)
     }
     _writeDictionaryBatch(t, e, i = !1) {
         this._dictionaryDeltaOffsets.set(e, t.length + (this._dictionaryDeltaOffsets.get(e) || 0));
         const {
             byteLength: r,
             nodes: s,
             bufferRegions: o,
             buffers: a
-        } = st.assemble(new P([t])), l = new Lt(t.length, s, o), c = new re(l, e, i), d = mt.from(c, r);
+        } = ot.assemble(new z([t])), l = new Lt(t.length, s, o), c = new ae(l, e, i), d = vt.from(c, r);
         return this._writeMessage(d)._writeBodyBuffers(a)
     }
     _writeBodyBuffers(t) {
         let e, i, r;
         for (let s = -1, o = t.length; ++s < o;)(e = t[s]) && (i = e.byteLength) > 0 && (this._write(e), (r = (i + 7 & -8) - i) > 0 && this._writePadding(r));
         return this
     }
@@ -8376,49 +8376,49 @@
             let r = this._dictionaryDeltaOffsets.get(e) || 0;
             if (r === 0 || (i = i?.slice(r)).length > 0)
                 for (const s of i.data) this._writeDictionaryBatch(s, e, r > 0), r += s.length
         }
         return this
     }
 }
-class ys extends cl {
+class bs extends ul {
     static writeAll(t, e) {
-        const i = new ys(e);
-        return Ie(t) ? t.then(r => i.writeAll(r)) : gn(t) ? bs(i, t) : vs(i, t)
+        const i = new bs(e);
+        return Ae(t) ? t.then(r => i.writeAll(r)) : In(t) ? ws(i, t) : _s(i, t)
     }
 }
-class ms extends cl {
+class gs extends ul {
     static writeAll(t) {
-        const e = new ms;
-        return Ie(t) ? t.then(i => e.writeAll(i)) : gn(t) ? bs(e, t) : vs(e, t)
+        const e = new gs;
+        return Ae(t) ? t.then(i => e.writeAll(i)) : In(t) ? ws(e, t) : _s(e, t)
     }
     constructor() {
         super(), this._autoDestroy = !0
     }
     _writeSchema(t) {
         return this._writeMagic()._writePadding(2)
     }
     _writeFooter(t) {
         const e = Vn.encode(new Vn(t, Nt.V4, this._recordBatchBlocks, this._dictionaryBlocks));
         return super._writeFooter(t)._write(e)._write(Int32Array.of(e.byteLength))._writeMagic()
     }
 }
 
-function vs(n, t) {
+function _s(n, t) {
     let e = t;
-    t instanceof pt && (e = t.batches, n.reset(void 0, t.schema));
+    t instanceof yt && (e = t.batches, n.reset(void 0, t.schema));
     for (const i of e) n.write(i);
     return n.finish()
 }
 
-function bs(n, t) {
+function ws(n, t) {
     var e, i, r, s;
-    return w(this, void 0, void 0, function*() {
+    return S(this, void 0, void 0, function*() {
         try {
-            for (e = je(t); i = yield e.next(), !i.done;) {
+            for (e = Ye(t); i = yield e.next(), !i.done;) {
                 const o = i.value;
                 n.write(o)
             }
         } catch (o) {
             r = {
                 error: o
             }
@@ -8429,23 +8429,23 @@
                 if (r) throw r.error
             }
         }
         return n.finish()
     })
 }
 
-function An(n) {
-    const t = fe.from(n);
-    return Ie(t) ? t.then(e => An(e)) : t.isAsync() ? t.readAll().then(e => new pt(e)) : new pt(t.readAll())
+function Nn(n) {
+    const t = ve.from(n);
+    return Ae(t) ? t.then(e => Nn(e)) : t.isAsync() ? t.readAll().then(e => new yt(e)) : new yt(t.readAll())
 }
 
-function pr(n, t = "stream") {
-    return (t === "stream" ? ys : ms).writeAll(n).toUint8Array(!0)
+function mr(n, t = "stream") {
+    return (t === "stream" ? bs : gs).writeAll(n).toUint8Array(!0)
 }
-var qs = function() {
+var Js = function() {
         function n(t, e, i, r) {
             var s = this;
             this.getCell = function(o, a) {
                 var l = o < s.headerRows && a < s.headerColumns,
                     c = o >= s.headerRows && a < s.headerColumns,
                     d = o < s.headerRows && a >= s.headerColumns;
                 if (l) {
@@ -8472,35 +8472,35 @@
                         classNames: h.join(" "),
                         content: s.getContent(s.indexTable, _, a)
                     }
                 } else {
                     var _ = o - s.headerRows,
                         y = a - s.headerColumns,
                         h = ["data", "row" + _, "col" + y],
-                        G = s.styler ? s.getContent(s.styler.displayValuesTable, _, y) : s.getContent(s.dataTable, _, y);
+                        V = s.styler ? s.getContent(s.styler.displayValuesTable, _, y) : s.getContent(s.dataTable, _, y);
                     return {
                         type: "data",
                         id: "T_".concat(s.uuid, "row").concat(_, "_col").concat(y),
                         classNames: h.join(" "),
-                        content: G
+                        content: V
                     }
                 }
             }, this.getContent = function(o, a, l) {
                 var c = o.getChildAt(l);
                 if (c === null) return "";
                 var d = s.getColumnTypeId(o, l);
                 switch (d) {
                     case u.Timestamp:
                         return s.nanosToDate(c.get(a));
                     default:
                         return c.get(a)
                 }
-            }, this.dataTable = An(t), this.indexTable = An(e), this.columnsTable = An(i), this.styler = r ? {
+            }, this.dataTable = Nn(t), this.indexTable = Nn(e), this.columnsTable = Nn(i), this.styler = r ? {
                 caption: r.caption,
-                displayValuesTable: An(r.displayValues),
+                displayValuesTable: Nn(r.displayValues),
                 styles: r.styles,
                 uuid: r.uuid
             } : void 0
         }
         return Object.defineProperty(n.prototype, "rows", {
             get: function() {
                 return this.indexTable.numRows + this.columnsTable.numCols
@@ -8571,65 +8571,65 @@
             get: function() {
                 return this.columnsTable
             },
             enumerable: !1,
             configurable: !0
         }), n.prototype.serialize = function() {
             return {
-                data: pr(this.dataTable),
-                index: pr(this.indexTable),
-                columns: pr(this.columnsTable)
+                data: mr(this.dataTable),
+                index: mr(this.indexTable),
+                columns: mr(this.columnsTable)
             }
         }, n.prototype.getColumnTypeId = function(t, e) {
             return t.schema.fields[e].type.typeId
         }, n.prototype.nanosToDate = function(t) {
             return new Date(t / 1e6)
         }, n
     }(),
-    Tn = function() {
-        return Tn = Object.assign || function(n) {
+    Mn = function() {
+        return Mn = Object.assign || function(n) {
             for (var t, e = 1, i = arguments.length; e < i; e++) {
                 t = arguments[e];
                 for (var r in t) Object.prototype.hasOwnProperty.call(t, r) && (n[r] = t[r])
             }
             return n
-        }, Tn.apply(this, arguments)
+        }, Mn.apply(this, arguments)
     },
-    Nn;
+    Ln;
 (function(n) {
     n.COMPONENT_READY = "streamlit:componentReady", n.SET_COMPONENT_VALUE = "streamlit:setComponentValue", n.SET_FRAME_HEIGHT = "streamlit:setFrameHeight"
-})(Nn || (Nn = {}));
-var Ht = function() {
+})(Ln || (Ln = {}));
+var Jt = function() {
         function n() {}
         return n.API_VERSION = 1, n.RENDER_EVENT = "streamlit:render", n.events = new EventTarget, n.registeredMessageListener = !1, n.setComponentReady = function() {
-            n.registeredMessageListener || (window.addEventListener("message", n.onMessageEvent), n.registeredMessageListener = !0), n.sendBackMsg(Nn.COMPONENT_READY, {
+            n.registeredMessageListener || (window.addEventListener("message", n.onMessageEvent), n.registeredMessageListener = !0), n.sendBackMsg(Ln.COMPONENT_READY, {
                 apiVersion: n.API_VERSION
             })
         }, n.setFrameHeight = function(t) {
-            t === void 0 && (t = document.body.scrollHeight), t !== n.lastFrameHeight && (n.lastFrameHeight = t, n.sendBackMsg(Nn.SET_FRAME_HEIGHT, {
+            t === void 0 && (t = document.body.scrollHeight), t !== n.lastFrameHeight && (n.lastFrameHeight = t, n.sendBackMsg(Ln.SET_FRAME_HEIGHT, {
                 height: t
             }))
         }, n.setComponentValue = function(t) {
             var e;
-            t instanceof qs ? (e = "dataframe", t = t.serialize()) : Hd(t) ? (e = "bytes", t = new Uint8Array(t.buffer)) : t instanceof ArrayBuffer ? (e = "bytes", t = new Uint8Array(t)) : e = "json", n.sendBackMsg(Nn.SET_COMPONENT_VALUE, {
+            t instanceof Js ? (e = "dataframe", t = t.serialize()) : Hd(t) ? (e = "bytes", t = new Uint8Array(t.buffer)) : t instanceof ArrayBuffer ? (e = "bytes", t = new Uint8Array(t)) : e = "json", n.sendBackMsg(Ln.SET_COMPONENT_VALUE, {
                 value: t,
                 dataType: e
             })
         }, n.onMessageEvent = function(t) {
             var e = t.data.type;
             switch (e) {
                 case n.RENDER_EVENT:
                     n.onRenderMessage(t.data);
                     break
             }
         }, n.onRenderMessage = function(t) {
             var e = t.args;
             e == null && (console.error("Got null args in onRenderMessage. This should never happen"), e = {});
             var i = t.dfs && t.dfs.length > 0 ? n.argsDataframeToObject(t.dfs) : {};
-            e = Tn(Tn({}, e), i);
+            e = Mn(Mn({}, e), i);
             var r = !!t.disabled,
                 s = t.theme;
             s && Gd(s);
             var o = {
                     disabled: r,
                     args: e,
                     theme: s
@@ -8646,17 +8646,17 @@
             });
             return Object.fromEntries(e)
         }, n.toArrowTable = function(t) {
             var e, i = (e = t.data, e.data),
                 r = e.index,
                 s = e.columns,
                 o = e.styler;
-            return new qs(i, r, s, o)
+            return new Js(i, r, s, o)
         }, n.sendBackMsg = function(t, e) {
-            window.parent.postMessage(Tn({
+            window.parent.postMessage(Mn({
                 isStreamlitMessage: !0,
                 type: t
             }, e), "*")
         }, n
     }(),
     Gd = function(n) {
         var t = document.createElement("style");
@@ -8707,43 +8707,43 @@
 (function(n) {
     qd(t, n);
 
     function t() {
         return n !== null && n.apply(this, arguments) || this
     }
     return t.prototype.componentDidMount = function() {
-        Ht.setFrameHeight()
+        Jt.setFrameHeight()
     }, t.prototype.componentDidUpdate = function() {
-        Ht.setFrameHeight()
+        Jt.setFrameHeight()
     }, t
 })(ac.PureComponent);
-const ul = (n, t) => {
+const dl = (n, t) => {
         const e = n.__vccOpts || n;
         for (const [i, r] of t) e[i] = r;
         return e
     },
     Jd = ht({
         __name: "WithStreamlitConnection",
         setup(n, {
             expose: t
         }) {
             t();
-            const e = It(void 0),
-                i = It(void 0),
-                r = It(NaN),
+            const e = pt(void 0),
+                i = pt(void 0),
+                r = pt(NaN),
                 s = a => {
                     const l = a;
                     e.value = l.detail, i.value = void 0, r.value = window.innerWidth
                 };
-            Pn(() => {
-                Ht.events.addEventListener(Ht.RENDER_EVENT, s), Ht.setComponentReady()
-            }), Er(() => {
-                i.value !== void 0 && Ht.setFrameHeight()
-            }), io(() => {
-                Ht.events.removeEventListener(Ht.RENDER_EVENT, s)
+            wn(() => {
+                Jt.events.addEventListener(Jt.RENDER_EVENT, s), Jt.setComponentReady()
+            }), kr(() => {
+                i.value !== void 0 && Jt.setFrameHeight()
+            }), ro(() => {
+                Jt.events.removeEventListener(Jt.RENDER_EVENT, s)
             }), gl(a => {
                 i.value = String(a)
             });
             const o = {
                 renderData: e,
                 componentError: i,
                 innerWidth: r,
@@ -8763,23 +8763,23 @@
         class: "err__title"
     }, "Component Error", -1)),
     Qd = {
         class: "err__msg"
     };
 
 function th(n, t, e, i, r, s) {
-    return m(), b("div", null, [i.componentError !== void 0 ? (m(), b("div", Zd, [Xd, g("div", Qd, "Message: " + C(i.componentError), 1)])) : i.renderData !== void 0 ? dt(n.$slots, "default", {
+    return m(), v("div", null, [i.componentError !== void 0 ? (m(), v("div", Zd, [Xd, g("div", Qd, "Message: " + C(i.componentError), 1)])) : i.renderData !== void 0 ? dt(n.$slots, "default", {
         key: 1,
         width: i.innerWidth,
         args: i.renderData.args,
         disabled: i.renderData.disabled,
         theme: i.renderData.theme
     }, void 0, !0) : k("", !0)])
 }
-const eh = ul(Jd, [
+const eh = dl(Jd, [
         ["render", th],
         ["__scopeId", "data-v-ad0b980e"]
     ]),
     nh = ht({
         __name: "StreamlitComponent",
         props: {
             component: {}
@@ -8809,53 +8809,53 @@
                 enumerable: !1,
                 value: !0
             }), r
         }
     });
 
 function ih(n, t, e, i, r, s) {
-    return m(), Mt(i.WithStreamlitConnection, null, {
-        default: Se(({
+    return m(), xt(i.WithStreamlitConnection, null, {
+        default: Fe(({
             width: o,
             args: a,
             disabled: l,
             theme: c
         }) => [g("div", {
             class: "component-wrapper",
-            style: xn(i.streamlitStyle(c))
-        }, [(m(), Mt(cn(i.props.component), {
+            style: hn(i.streamlitStyle(c))
+        }, [(m(), xt(dn(i.props.component), {
             width: o,
             args: a,
             disabled: l,
             theme: c
         }, null, 8, ["width", "args", "disabled", "theme"]))], 4)]),
         _: 1
     })
 }
-const Tp = ul(nh, [
+const Np = dl(nh, [
         ["render", ih],
         ["__scopeId", "data-v-ba378196"]
     ]),
     rh = {
         "<": "&lt;",
         ">": "&gt;",
         '"': "&quot;",
         "'": "&#039;",
         "&": "&amp;"
     };
 let sh = 0;
 var oh = n => n.replace(/[<>"&]/g, t => rh[t] || t),
     ah = n => n + sh++;
-const Js = {},
+const Ks = {},
     lh = ht({
         name: "OhVueIcon",
         props: {
             name: {
                 type: String,
-                validator: n => !n || n in Js || (console.warn(`Invalid prop: prop "name" is referring to an unregistered icon "${n}".
+                validator: n => !n || n in Ks || (console.warn(`Invalid prop: prop "name" is referring to an unregistered icon "${n}".
 Please make sure you have imported this icon before using it.`), !1)
             },
             title: String,
             fill: String,
             scale: {
                 type: [Number, String],
                 default: 1
@@ -8870,29 +8870,29 @@
             speed: {
                 validator: n => n === "fast" || n === "slow"
             },
             label: String,
             inverse: Boolean
         },
         setup(n) {
-            const t = It([]),
-                e = Is({
+            const t = pt([]),
+                e = Os({
                     outerScale: 1.2,
                     x: null,
                     y: null
                 }),
-                i = Is({
+                i = Os({
                     width: 0,
                     height: 0
                 }),
-                r = L(() => {
-                    const et = Number(n.scale);
-                    return isNaN(et) || et <= 0 ? (console.warn('Invalid prop: prop "scale" should be a number over 0.'), e.outerScale) : et * e.outerScale
+                r = w(() => {
+                    const P = Number(n.scale);
+                    return isNaN(P) || P <= 0 ? (console.warn('Invalid prop: prop "scale" should be a number over 0.'), e.outerScale) : P * e.outerScale
                 }),
-                s = L(() => ({
+                s = w(() => ({
                     "ov-icon": !0,
                     "ov-inverse": n.inverse,
                     "ov-flip-horizontal": n.flip === "horizontal",
                     "ov-flip-vertical": n.flip === "vertical",
                     "ov-flip-both": n.flip === "both",
                     "ov-spin": n.animation === "spin",
                     "ov-spin-pulse": n.animation === "spin-pulse",
@@ -8901,57 +8901,57 @@
                     "ov-pulse": n.animation === "pulse",
                     "ov-flash": n.animation === "flash",
                     "ov-float": n.animation === "float",
                     "ov-hover": n.hover,
                     "ov-fast": n.speed === "fast",
                     "ov-slow": n.speed === "slow"
                 })),
-                o = L(() => n.name ? Js[n.name] : null),
-                a = L(() => o.value ? `${o.value.minX} ${o.value.minY} ${o.value.width} ${o.value.height}` : `0 0 ${c.value} ${d.value}`),
-                l = L(() => {
+                o = w(() => n.name ? Ks[n.name] : null),
+                a = w(() => o.value ? `${o.value.minX} ${o.value.minY} ${o.value.width} ${o.value.height}` : `0 0 ${c.value} ${d.value}`),
+                l = w(() => {
                     if (!o.value) return 1;
                     const {
-                        width: et,
-                        height: ot
+                        width: P,
+                        height: et
                     } = o.value;
-                    return Math.max(et, ot) / 16
+                    return Math.max(P, et) / 16
                 }),
-                c = L(() => i.width || o.value && o.value.width / l.value * r.value || 0),
-                d = L(() => i.height || o.value && o.value.height / l.value * r.value || 0),
-                h = L(() => r.value !== 1 && {
+                c = w(() => i.width || o.value && o.value.width / l.value * r.value || 0),
+                d = w(() => i.height || o.value && o.value.height / l.value * r.value || 0),
+                h = w(() => r.value !== 1 && {
                     fontSize: r.value + "em"
                 }),
-                y = L(() => {
+                y = w(() => {
                     if (!o.value || !o.value.raw) return null;
-                    const et = {};
-                    let ot = o.value.raw;
-                    return ot = ot.replace(/\s(?:xml:)?id=(["']?)([^"')\s]+)\1/g, (nt, He, wn) => {
-                        const Le = ah("vat-");
-                        return et[wn] = Le, ` id="${Le}"`
-                    }), ot = ot.replace(/#(?:([^'")\s]+)|xpointer\(id\((['"]?)([^')]+)\2\)\))/g, (nt, He, wn, Le) => {
-                        const qe = He || Le;
-                        return qe && et[qe] ? `#${et[qe]}` : nt
-                    }), ot
+                    const P = {};
+                    let et = o.value.raw;
+                    return et = et.replace(/\s(?:xml:)?id=(["']?)([^"')\s]+)\1/g, (q, Rt, le) => {
+                        const Yt = ah("vat-");
+                        return P[le] = Yt, ` id="${Yt}"`
+                    }), et = et.replace(/#(?:([^'")\s]+)|xpointer\(id\((['"]?)([^')]+)\2\)\))/g, (q, Rt, le, Yt) => {
+                        const Se = Rt || Yt;
+                        return Se && P[Se] ? `#${P[Se]}` : q
+                    }), et
                 }),
-                _ = L(() => o.value && o.value.attr ? o.value.attr : {}),
-                G = () => {
+                _ = w(() => o.value && o.value.attr ? o.value.attr : {}),
+                V = () => {
                     if (!n.name && n.name !== null && t.value.length === 0) return void console.warn('Invalid prop: prop "name" is required.');
                     if (o.value) return;
-                    let et = 0,
-                        ot = 0;
-                    t.value.forEach(nt => {
-                        nt.outerScale = r.value, et = Math.max(et, nt.width), ot = Math.max(ot, nt.height)
-                    }), i.width = et, i.height = ot, t.value.forEach(nt => {
-                        nt.x = (et - nt.width) / 2, nt.y = (ot - nt.height) / 2
+                    let P = 0,
+                        et = 0;
+                    t.value.forEach(q => {
+                        q.outerScale = r.value, P = Math.max(P, q.width), et = Math.max(et, q.height)
+                    }), i.width = P, i.height = et, t.value.forEach(q => {
+                        q.x = (P - q.width) / 2, q.y = (et - q.height) / 2
                     })
                 };
-            return Pn(() => {
-                G()
-            }), Er(() => {
-                G()
+            return wn(() => {
+                V()
+            }), kr(() => {
+                V()
             }), {
                 ...Sl(e),
                 children: t,
                 icon: o,
                 klass: s,
                 style: h,
                 width: c,
@@ -8979,39 +8979,39 @@
                 class: this.klass,
                 style: this.style
             };
             if (t = Object.assign(t, n), this.raw) {
                 const r = this.title ? `<title>${oh(this.title)}</title>${this.raw}` : this.raw;
                 t.innerHTML = r
             }
-            const e = this.title ? [or("title", this.title)] : [],
-                i = (r, s, o) => or(r, {
+            const e = this.title ? [lr("title", this.title)] : [],
+                i = (r, s, o) => lr(r, {
                     ...s,
                     key: `${r}-${o}`
                 });
-            return or("svg", t, this.raw ? void 0 : e.concat([this.$slots.default ? this.$slots.default() : this.icon ? [...this.icon.paths.map((r, s) => i("path", r, s)), ...this.icon.polygons.map((r, s) => i("polygon", r, s))] : []]))
+            return lr("svg", t, this.raw ? void 0 : e.concat([this.$slots.default ? this.$slots.default() : this.icon ? [...this.icon.paths.map((r, s) => i("path", r, s)), ...this.icon.polygons.map((r, s) => i("polygon", r, s))] : []]))
         }
     });
 
-function gs(n, t) {
+function Ss(n, t) {
     t === void 0 && (t = {});
     var e = t.insertAt;
     if (n && typeof document < "u") {
         var i = document.head || document.getElementsByTagName("head")[0],
             r = document.createElement("style");
         r.type = "text/css", e === "top" && i.firstChild ? i.insertBefore(r, i.firstChild) : i.appendChild(r), r.styleSheet ? r.styleSheet.cssText = n : r.appendChild(document.createTextNode(n))
     }
 }
-gs(`.ov-icon {
+Ss(`.ov-icon {
   display: inline-block;
   overflow: visible;
   vertical-align: -0.2em;
 }
 `);
-gs(`/* ---------------- spin ---------------- */
+Ss(`/* ---------------- spin ---------------- */
 .ov-spin:not(.ov-hover),
 .ov-spin.ov-hover:hover,
 .ov-parent.ov-hover:hover > .ov-spin {
   animation: ov-spin 1s linear infinite;
 }
 
 .ov-spin:not(.ov-hover).ov-fast,
@@ -9246,15 +9246,15 @@
     transform: translateY(-3px);
   }
   50% {
     transform: translateY(3px);
   }
 }
 `);
-gs(`.ov-flip-horizontal {
+Ss(`.ov-flip-horizontal {
   transform: scale(-1, 1);
 }
 
 .ov-flip-vertical {
   transform: scale(1, -1);
 }
 
@@ -9263,27 +9263,27 @@
 }
 
 .ov-inverse {
   color: #fff;
 }
 `);
 const ch = "abcdefghijklmnopqrstuvwyz0123456789",
-    Ks = ch.repeat(10),
+    Zs = ch.repeat(10),
     uh = () => {
-        const n = Math.floor(Math.random() * Ks.length);
-        return Ks[n]
+        const n = Math.floor(Math.random() * Zs.length);
+        return Zs[n]
     },
-    xe = (n = "", t = "") => (n ? n + "-" : "") + dh(5) + (t ? "-" + t : ""),
+    Ce = (n = "", t = "") => (n ? n + "-" : "") + dh(5) + (t ? "-" + t : ""),
     dh = n => Array.from({
         length: n
     }).map(uh).join(""),
     hh = () => {
-        const n = It(),
-            t = It(!1),
-            e = It(!1),
+        const n = pt(),
+            t = pt(!1),
+            e = pt(!1),
             i = () => {
                 if (!n.value) return;
                 n.value.style.setProperty("--collapser", "none");
                 const r = n.value.offsetHeight;
                 n.value.style.setProperty("--collapse", -r + "px"), n.value.style.setProperty("--collapser", "")
             };
         return {
@@ -9306,25 +9306,25 @@
     fh = ["id"],
     ph = {
         class: "alert-content"
     },
     yh = {
         class: "fr-alert__description"
     },
-    Np = ht({
+    xp = ht({
         __name: "DsfrAlert",
         props: {
             closed: {
                 type: Boolean
             },
             closeable: {
                 type: Boolean
             },
             id: {
-                default: () => xe("basic", "alert")
+                default: () => Ce("basic", "alert")
             },
             title: {
                 default: ""
             },
             description: {},
             small: {
                 type: Boolean
@@ -9339,31 +9339,31 @@
         emits: ["close"],
         setup(n, {
             emit: t
         }) {
             const e = n,
                 i = t,
                 r = () => i("close"),
-                s = L(() => [`fr-alert--${e.type}`, {
+                s = w(() => [`fr-alert--${e.type}`, {
                     "fr-alert--sm": e.small
                 }]);
-            return (o, a) => (m(), Mt(Ol, {
+            return (o, a) => (m(), xt(Ol, {
                 name: "slide-fade"
             }, {
-                default: Se(() => [o.closed ? k("", !0) : (m(), b("div", {
+                default: Fe(() => [o.closed ? k("", !0) : (m(), v("div", {
                     key: 0,
                     id: o.id,
-                    class: rt(["fr-alert", s.value])
-                }, [g("div", ph, [o.small ? k("", !0) : (m(), Mt(cn(o.titleTag), {
+                    class: st(["fr-alert", s.value])
+                }, [g("div", ph, [o.small ? k("", !0) : (m(), xt(dn(o.titleTag), {
                     key: 0,
                     class: "fr-alert__title"
                 }, {
-                    default: Se(() => [vt(C(o.title), 1)]),
+                    default: Fe(() => [bt(C(o.title), 1)]),
                     _: 1
-                })), g("p", yh, [dt(o.$slots, "default", {}, () => [vt(C(o.description), 1)])])]), o.closeable ? (m(), b("button", {
+                })), g("p", yh, [dt(o.$slots, "default", {}, () => [bt(C(o.description), 1)])])]), o.closeable ? (m(), v("button", {
                     key: 0,
                     class: "fr-btn fr-btn--close",
                     title: "Fermer",
                     "aria-label": "Fermer",
                     onClick: r
                 })) : k("", !0)], 10, fh))]),
                 _: 3
@@ -9385,88 +9385,88 @@
                 type: Boolean
             },
             ellipsis: {
                 type: Boolean
             }
         },
         setup(n) {
-            return (t, e) => (m(), b("p", {
-                class: rt(["fr-badge", {
+            return (t, e) => (m(), v("p", {
+                class: st(["fr-badge", {
                     [`fr-badge--${t.type}`]: t.type,
                     "fr-badge--no-icon": t.noIcon,
                     "fr-badge--sm": t.small
                 }]),
                 title: t.ellipsis ? t.label : void 0
             }, [g("span", {
-                class: rt(t.ellipsis ? "fr-ellipsis" : "")
+                class: st(t.ellipsis ? "fr-ellipsis" : "")
             }, C(t.label), 3)], 10, mh))
         }
     }),
     vh = {
         role: "navigation",
         class: "fr-breadcrumb",
         "aria-label": "vous êtes ici :"
     },
     bh = ["aria-expanded", "aria-controls"],
     gh = ["id"],
     _h = {
         class: "fr-breadcrumb__list"
     },
     wh = ["aria-current"],
-    xp = ht({
+    Lp = ht({
         __name: "DsfrBreadcrumb",
         props: {
             breadcrumbId: {
-                default: () => xe("breadcrumb")
+                default: () => Ce("breadcrumb")
             },
             links: {
                 default: () => [{
                     text: ""
                 }]
             }
         },
         setup(n) {
             const {
                 collapse: t,
                 collapsing: e,
                 cssExpanded: i,
                 doExpand: r,
                 onTransitionEnd: s
-            } = hh(), o = It(!1);
-            return Rr(o, (a, l) => {
+            } = hh(), o = pt(!1);
+            return Ur(o, (a, l) => {
                 a !== l && r(a)
-            }), (a, l) => (m(), b("nav", vh, [Fl(g("button", {
+            }), (a, l) => (m(), v("nav", vh, [Fl(g("button", {
                 class: "fr-breadcrumb__button",
                 "aria-expanded": o.value,
                 "aria-controls": a.breadcrumbId,
                 onClick: l[0] || (l[0] = c => o.value = !o.value)
             }, " Voir le fil d’Ariane ", 8, bh), [
                 [Al, !o.value]
             ]), g("div", {
                 id: a.breadcrumbId,
                 ref_key: "collapse",
                 ref: t,
-                class: rt(["fr-collapse", {
-                    "fr-collapse--expanded": ei(i),
-                    "fr-collapsing": ei(e)
+                class: st(["fr-collapse", {
+                    "fr-collapse--expanded": ii(i),
+                    "fr-collapsing": ii(e)
                 }]),
-                onTransitionend: l[1] || (l[1] = c => ei(s)(o.value))
-            }, [g("ol", _h, [(m(!0), b(un, null, Ln(a.links, (c, d) => (m(), b("li", {
+                onTransitionend: l[1] || (l[1] = c => ii(s)(o.value))
+            }, [g("ol", _h, [(m(!0), v(He, null, fn(a.links, (c, d) => (m(), v("li", {
                 key: d,
                 class: "fr-breadcrumb__item",
                 "data-testid": "lis"
-            }, [c.to ? (m(), Mt(cn("RouterLink"), {
+            }, [c.to ? (m(), xt(dn("RouterLink"), {
                 key: 0,
                 class: "fr-breadcrumb__link",
                 to: c.to,
                 "aria-current": d === a.links.length - 1 ? "page" : void 0
             }, {
-                default: Se(() => [vt(C(c.text), 1)]),
+                default: Fe(() => [bt(C(c.text), 1)]),
                 _: 2
-            }, 1032, ["to", "aria-current"])) : k("", !0), c.to ? k("", !0) : (m(), b("a", {
+            }, 1032, ["to", "aria-current"])) : k("", !0), c.to ? k("", !0) : (m(), v("a", {
                 key: 1,
                 class: "fr-breadcrumb__link",
                 "aria-current": d === a.links.length - 1 ? "page" : void 0
             }, C(c.text), 9, wh))]))), 128))])], 42, gh)]))
         }
     }),
     Sh = ["title", "disabled", "aria-disabled"],
@@ -9508,37 +9508,37 @@
                 default: () => {}
             }
         },
         setup(n, {
             expose: t
         }) {
             const e = n,
-                i = L(() => ["sm", "small"].includes(e.size)),
-                r = L(() => ["md", "medium"].includes(e.size)),
-                s = L(() => ["lg", "large"].includes(e.size)),
-                o = It(null);
+                i = w(() => ["sm", "small"].includes(e.size)),
+                r = w(() => ["md", "medium"].includes(e.size)),
+                s = w(() => ["lg", "large"].includes(e.size)),
+                o = pt(null);
             t({
                 focus: () => {
                     var d;
                     (d = o.value) == null || d.focus()
                 }
             });
-            const a = L(() => typeof e.icon == "string" && e.icon.startsWith("fr-icon-")),
-                l = L(() => e.iconOnly ? 1.25 : .8325),
-                c = L(() => typeof e.icon == "string" ? {
+            const a = w(() => typeof e.icon == "string" && e.icon.startsWith("fr-icon-")),
+                l = w(() => e.iconOnly ? 1.25 : .8325),
+                c = w(() => typeof e.icon == "string" ? {
                     scale: l.value,
                     name: e.icon
                 } : {
                     scale: l.value,
                     ...e.icon
                 });
-            return (d, h) => (m(), b("button", {
+            return (d, h) => (m(), v("button", {
                 ref_key: "btn",
                 ref: o,
-                class: rt({
+                class: st({
                     "fr-btn": !0,
                     "fr-btn--secondary": d.secondary && !d.tertiary,
                     "fr-btn--tertiary": d.tertiary && !d.secondary && !d.noOutline,
                     "fr-btn--tertiary-no-outline": d.tertiary && !d.secondary && d.noOutline,
                     "fr-btn--sm": i.value,
                     "fr-btn--md": r.value,
                     "fr-btn--lg": s.value,
@@ -9548,51 +9548,135 @@
                     reverse: d.iconRight && !a.value,
                     "justify-center": !a.value && d.iconOnly,
                     [d.icon]: a.value
                 }),
                 title: d.iconOnly ? d.label : void 0,
                 disabled: d.disabled,
                 "aria-disabled": d.disabled,
-                style: xn(!a.value && d.iconOnly ? {
+                style: hn(!a.value && d.iconOnly ? {
                     "padding-inline": "0.5rem"
                 } : {}),
                 onClick: h[0] || (h[0] = y => d.onClick ? d.onClick(y) : () => {})
-            }, [d.icon && !a.value ? (m(), Mt(ei(lh), ro(pe({
+            }, [d.icon && !a.value ? (m(), xt(ii(lh), so(re({
                 key: 0
-            }, c.value)), null, 16)) : k("", !0), d.iconOnly ? k("", !0) : (m(), b("span", Ih, [vt(C(d.label) + " ", 1), dt(d.$slots, "default", {}, void 0, !0)]))], 14, Sh))
+            }, c.value)), null, 16)) : k("", !0), d.iconOnly ? k("", !0) : (m(), v("span", Ih, [bt(C(d.label) + " ", 1), dt(d.$slots, "default", {}, void 0, !0)]))], 14, Sh))
         }
     }),
-    _s = (n, t) => {
+    Is = (n, t) => {
         const e = n.__vccOpts || n;
         for (const [i, r] of t) e[i] = r;
         return e
     },
-    Lp = _s(Bh, [
+    Oh = Is(Bh, [
         ["__scopeId", "data-v-7fc52401"]
     ]),
-    Oh = ["id", "name", "checked", "data-testid", "data-test"],
-    Fh = ["for"],
-    Ah = {
+    Ep = ht({
+        __name: "DsfrButtonGroup",
+        props: {
+            buttons: {
+                default: () => []
+            },
+            reverse: {
+                type: Boolean
+            },
+            equisized: {
+                type: Boolean
+            },
+            iconRight: {
+                type: Boolean
+            },
+            align: {
+                default: void 0
+            },
+            inlineLayoutWhen: {
+                type: [String, Boolean],
+                default: "never"
+            },
+            size: {
+                default: "md"
+            }
+        },
+        setup(n) {
+            const t = n,
+                e = pt(null),
+                i = w(() => ["sm", "small"].includes(t.size)),
+                r = w(() => ["md", "medium"].includes(t.size)),
+                s = w(() => ["lg", "large"].includes(t.size)),
+                o = w(() => ["always", "", !0].includes(t.inlineLayoutWhen)),
+                a = w(() => ["sm", "small"].includes(t.inlineLayoutWhen)),
+                l = w(() => ["md", "medium"].includes(t.inlineLayoutWhen)),
+                c = w(() => ["lg", "large"].includes(t.inlineLayoutWhen)),
+                d = w(() => t.align === "center"),
+                h = w(() => t.align === "right"),
+                y = pt("auto"),
+                _ = w(() => `--equisized-width: ${y.value};`),
+                V = async () => {
+                    var P;
+                    let et = 0;
+                    await new Promise(q => setTimeout(q, 100)), (P = e.value) == null || P.querySelectorAll(".fr-btn").forEach(q => {
+                        const Rt = q,
+                            le = Rt.offsetWidth,
+                            Yt = window.getComputedStyle(Rt),
+                            Se = +Yt.marginLeft.replace("px", ""),
+                            Zn = +Yt.marginRight.replace("px", "");
+                        Rt.style.width = "var(--equisized-width)";
+                        const Xn = le + Se + Zn;
+                        Xn > et && (et = Xn)
+                    }), y.value = et + "px"
+                };
+            return wn(async () => {
+                !e.value || !t.equisized || await V()
+            }), (P, et) => (m(), v("ul", {
+                ref_key: "buttonsEl",
+                ref: e,
+                style: hn(_.value),
+                class: st(["fr-btns-group", {
+                    "fr-btns-group--equisized": P.equisized,
+                    "fr-btns-group--sm": i.value,
+                    "fr-btns-group--md": r.value,
+                    "fr-btns-group--lg": s.value,
+                    "fr-btns-group--inline-sm": o.value || a.value,
+                    "fr-btns-group--inline-md": o.value || l.value,
+                    "fr-btns-group--inline-lg": o.value || c.value,
+                    "fr-btns-group--center": d.value,
+                    "fr-btns-group--right": h.value,
+                    "fr-btns-group--icon-right": P.iconRight,
+                    "fr-btns-group--inline-reverse": P.reverse
+                }]),
+                "data-testid": "fr-btns"
+            }, [(m(!0), v(He, null, fn(P.buttons, ({
+                onClick: q,
+                ...Rt
+            }, le) => (m(), v("li", {
+                key: le
+            }, [br(Oh, re(Rt, {
+                onClick: q
+            }), null, 16, ["onClick"])]))), 128)), dt(P.$slots, "default")], 6))
+        }
+    }),
+    Fh = ["id", "name", "checked", "data-testid", "data-test"],
+    Ah = ["for"],
+    Dh = {
         key: 0,
         class: "required"
     },
-    Dh = {
+    Th = {
         key: 0,
         class: "fr-hint-text"
     },
-    Th = {
+    Nh = {
         key: 0,
         class: "fr-messages-group",
         "aria-live": "assertive"
     },
-    Ep = ht({
+    Rp = ht({
         __name: "DsfrCheckbox",
         props: {
             id: {
-                default: () => xe("basic", "checkbox")
+                default: () => Ce("basic", "checkbox")
             },
             name: {},
             required: {
                 type: Boolean
             },
             modelValue: {
                 type: Boolean
@@ -9618,62 +9702,62 @@
         },
         emits: ["update:modelValue"],
         setup(n, {
             emit: t
         }) {
             const e = n,
                 i = t,
-                r = L(() => e.errorMessage || e.validMessage),
-                s = L(() => e.errorMessage ? "fr-error-text" : "fr-valid-text"),
+                r = w(() => e.errorMessage || e.validMessage),
+                s = w(() => e.errorMessage ? "fr-error-text" : "fr-valid-text"),
                 o = a => {
                     i("update:modelValue", a.target.checked)
                 };
-            return (a, l) => (m(), b("div", {
-                class: rt(["fr-fieldset__element", {
+            return (a, l) => (m(), v("div", {
+                class: st(["fr-fieldset__element", {
                     "fr-fieldset__element--inline": a.inline
                 }])
             }, [g("div", {
-                class: rt(["fr-checkbox-group", {
+                class: st(["fr-checkbox-group", {
                     "fr-checkbox-group--error": a.errorMessage,
                     "fr-checkbox-group--valid": a.validMessage,
                     "fr-checkbox-group--sm": a.small
                 }])
-            }, [g("input", pe({
+            }, [g("input", re({
                 id: a.id,
                 name: a.name,
                 type: "checkbox",
                 checked: a.modelValue
             }, a.$attrs, {
                 "data-testid": `input-checkbox-${a.id}`,
                 "data-test": `input-checkbox-${a.id}`,
                 onChange: l[0] || (l[0] = c => o(c))
-            }), null, 16, Oh), g("label", {
+            }), null, 16, Fh), g("label", {
                 for: a.id,
                 class: "fr-label"
-            }, [dt(a.$slots, "label", {}, () => [vt(C(a.label) + " ", 1), dt(a.$slots, "required-tip", {}, () => [a.required ? (m(), b("span", Ah, " *")) : k("", !0)])]), a.hint ? (m(), b("span", Dh, C(a.hint), 1)) : k("", !0)], 8, Fh), r.value ? (m(), b("div", Th, [g("p", {
-                class: rt(["fr-message--info flex items-center", s.value])
+            }, [dt(a.$slots, "label", {}, () => [bt(C(a.label) + " ", 1), dt(a.$slots, "required-tip", {}, () => [a.required ? (m(), v("span", Dh, " *")) : k("", !0)])]), a.hint ? (m(), v("span", Th, C(a.hint), 1)) : k("", !0)], 8, Ah), r.value ? (m(), v("div", Nh, [g("p", {
+                class: st(["fr-message--info flex items-center", s.value])
             }, C(r.value), 3)])) : k("", !0)], 2)], 2))
         }
     }),
-    Nh = ["for"],
+    xh = ["for"],
     Mh = {
         key: 0,
         class: "fr-hint-text"
     },
-    xh = ["id", "aria-describedby", "value", "disabled", "accept"],
-    Lh = {
+    Lh = ["id", "aria-describedby", "value", "disabled", "accept"],
+    Eh = {
         key: 0,
         class: "fr-messages-group"
     },
-    Eh = ["id"],
-    Rp = ht({
+    Rh = ["id"],
+    Cp = ht({
         __name: "DsfrFileUpload",
         props: {
             id: {
-                default: () => xe("file-upload")
+                default: () => Ce("file-upload")
             },
             label: {
                 default: "Ajouter un fichier"
             },
             accept: {
                 default: () => []
             },
@@ -9698,171 +9782,171 @@
             emit: t
         }) {
             const e = t,
                 i = r => {
                     var s, o;
                     e("update:modelValue", (s = r.target) == null ? void 0 : s.value), e("change", (o = r.target) == null ? void 0 : o.files)
                 };
-            return (r, s) => (m(), b("div", {
-                class: rt(["fr-upload-group", {
+            return (r, s) => (m(), v("div", {
+                class: st(["fr-upload-group", {
                     "fr-upload-group--error": r.error,
                     "fr-upload-group--valid": r.validMessage,
                     "fr-upload-group--disabled": r.disabled
                 }])
             }, [g("label", {
                 class: "fr-label",
                 for: r.id
-            }, [vt(C(r.label) + " ", 1), r.hint ? (m(), b("span", Mh, C(r.hint), 1)) : k("", !0)], 8, Nh), g("input", pe({
+            }, [bt(C(r.label) + " ", 1), r.hint ? (m(), v("span", Mh, C(r.hint), 1)) : k("", !0)], 8, xh), g("input", re({
                 id: r.id,
                 class: "fr-upload",
                 type: "file",
                 "aria-describedby": r.error || r.validMessage ? `${r.id}-desc` : void 0
             }, r.$attrs, {
                 value: r.modelValue,
                 disabled: r.disabled,
                 accept: r.accept.join(","),
                 onChange: s[0] || (s[0] = o => i(o))
-            }), null, 16, xh), r.error || r.validMessage ? (m(), b("div", Lh, [r.error ? (m(), b("p", {
+            }), null, 16, Lh), r.error || r.validMessage ? (m(), v("div", Eh, [r.error ? (m(), v("p", {
                 key: 0,
                 id: `${r.id}-desc`,
                 class: "fr-error-text fr-mt-3v"
-            }, C(r.error ?? r.validMessage), 9, Eh)) : k("", !0)])) : k("", !0)], 2))
+            }, C(r.error ?? r.validMessage), 9, Rh)) : k("", !0)])) : k("", !0)], 2))
         }
     }),
-    Rh = ["innerHTML"],
-    Ch = ht({
+    Ch = ["innerHTML"],
+    kh = ht({
         __name: "DsfrLogo",
         props: {
             small: {
                 type: Boolean
             },
             large: {
                 type: Boolean
             },
             logoText: {
                 default: () => "Gouvernement"
             }
         },
         setup(n) {
             const t = n,
-                e = L(() => t.logoText instanceof Array ? t.logoText.join("<br>") : t.logoText);
-            return (i, r) => (m(), b("p", {
-                class: rt(["fr-logo", {
+                e = w(() => t.logoText instanceof Array ? t.logoText.join("<br>") : t.logoText);
+            return (i, r) => (m(), v("p", {
+                class: st(["fr-logo", {
                     "fr-logo--sm": i.small && !i.large,
                     "fr-logo--lg": i.large && !i.small
                 }]),
                 innerHTML: e.value
-            }, null, 10, Rh))
+            }, null, 10, Ch))
         }
     }),
-    kh = {
+    Uh = {
         class: "fr-footer__partners"
     },
-    Uh = {
+    $h = {
         key: 0,
         class: "fr-footer__partners-title"
     },
     Vh = {
         class: "fr-footer__partners-logos"
     },
-    $h = {
+    Ph = {
         key: 0,
         class: "fr-footer__partners-main"
     },
-    Ph = ["href"],
-    jh = ["src", "alt"],
-    zh = {
+    jh = ["href"],
+    zh = ["src", "alt"],
+    Wh = {
         class: "fr-footer__partners-sub"
     },
-    Wh = ["href"],
-    Yh = ["src", "alt"],
-    Gh = ht({
+    Yh = ["href"],
+    Gh = ["src", "alt"],
+    Hh = ht({
         __name: "DsfrFooterPartners",
         props: {
             mainPartner: {
                 default: void 0
             },
             subPartners: {
                 default: () => []
             },
             title: {
                 default: ""
             }
         },
         setup(n) {
-            return (t, e) => (m(), b("div", kh, [t.title ? (m(), b("h4", Uh, C(t.title), 1)) : k("", !0), g("div", Vh, [t.mainPartner ? (m(), b("div", $h, [g("a", {
+            return (t, e) => (m(), v("div", Uh, [t.title ? (m(), v("h4", $h, C(t.title), 1)) : k("", !0), g("div", Vh, [t.mainPartner ? (m(), v("div", Ph, [g("a", {
                 class: "fr-footer__partners-link",
                 href: t.mainPartner.href,
                 target: "_blank",
                 rel: "noopener noreferrer"
             }, [g("img", {
                 class: "fr-footer__logo",
                 src: t.mainPartner.logo,
                 alt: t.mainPartner.name
-            }, null, 8, jh)], 8, Ph)])) : k("", !0), g("div", zh, [g("ul", null, [(m(!0), b(un, null, Ln(t.subPartners, (i, r) => (m(), b("li", {
+            }, null, 8, zh)], 8, jh)])) : k("", !0), g("div", Wh, [g("ul", null, [(m(!0), v(He, null, fn(t.subPartners, (i, r) => (m(), v("li", {
                 key: r
             }, [g("a", {
                 class: "fr-footer__partners-link",
                 href: i.href,
                 target: "_blank",
                 rel: "noopener noreferrer"
             }, [g("img", {
                 class: "fr-footer__logo",
                 src: i.logo,
                 alt: i.name
-            }, null, 8, Yh)], 8, Wh)]))), 128))])])])]))
+            }, null, 8, Gh)], 8, Yh)]))), 128))])])])]))
         }
     }),
-    Hh = {
+    qh = {
         id: "footer",
         class: "fr-footer",
         role: "contentinfo"
     },
-    qh = {
+    Jh = {
         key: 0,
         class: "fr-footer__top"
     },
-    Jh = {
+    Kh = {
         class: "fr-container"
     },
-    Kh = {
+    Zh = {
         class: "fr-grid-row fr-grid-row--start fr-grid-row--gutters"
     },
-    Zh = {
+    Xh = {
         class: "fr-container"
     },
-    Xh = {
+    Qh = {
         class: "fr-footer__body"
     },
-    Qh = {
+    tf = {
         class: "fr-footer__brand fr-enlarge-link"
     },
-    tf = ["src", "alt"],
-    ef = {
+    ef = ["src", "alt"],
+    nf = {
         class: "fr-footer__content"
     },
-    nf = {
+    rf = {
         class: "fr-footer__content-desc"
     },
-    rf = {
+    sf = {
         class: "fr-footer__content-list"
     },
-    sf = ["href"],
-    of = {
+    of = ["href"],
+    af = {
         class: "fr-footer__bottom"
     },
-    af = {
+    lf = {
         class: "fr-footer__bottom-list"
     },
-    lf = ["href", "data-testid"],
-    cf = {
+    cf = ["href", "data-testid"],
+    uf = {
         key: 0,
         class: "fr-footer__bottom-copy"
     },
-    uf = ht({
+    df = ht({
         __name: "DsfrFooter",
         props: {
             a11yCompliance: {
                 default: "non conforme"
             },
             a11yComplianceLink: {
                 default: "/a11y"
@@ -9950,111 +10034,111 @@
             },
             licenceName: {
                 default: "licence etalab-2.0"
             }
         },
         setup(n) {
             const t = n,
-                e = L(() => [...t.beforeMandatoryLinks, ...t.mandatoryLinks, ...t.afterMandatoryLinks]),
+                e = w(() => [...t.beforeMandatoryLinks, ...t.mandatoryLinks, ...t.afterMandatoryLinks]),
                 i = Dl(),
-                r = L(() => {
+                r = w(() => {
                     var l;
                     return (l = i["footer-link-lists"]) == null ? void 0 : l.call(i).length
                 }),
-                s = L(() => {
+                s = w(() => {
                     const l = t.licenceTo || t.licenceLinkProps.to;
                     return l && typeof l == "string" && l.startsWith("http")
                 }),
-                o = L(() => s.value ? "" : t.licenceTo),
-                a = L(() => s.value ? t.licenceTo : "");
+                o = w(() => s.value ? "" : t.licenceTo),
+                a = w(() => s.value ? t.licenceTo : "");
             return (l, c) => {
                 const d = Tl("RouterLink");
-                return m(), b("footer", Hh, [r.value ? (m(), b("div", qh, [g("div", Jh, [g("div", Kh, [dt(l.$slots, "footer-link-lists", {}, void 0, !0)])])])) : k("", !0), g("div", Zh, [g("div", Xh, [g("div", Qh, [Bs(d, {
+                return m(), v("footer", qh, [r.value ? (m(), v("div", Jh, [g("div", Kh, [g("div", Zh, [dt(l.$slots, "footer-link-lists", {}, void 0, !0)])])])) : k("", !0), g("div", Xh, [g("div", Qh, [g("div", tf, [br(d, {
                     to: l.homeLink,
                     title: "Retour à l’accueil"
                 }, {
-                    default: Se(() => [Bs(Ch, {
+                    default: Fe(() => [br(kh, {
                         "logo-text": l.logoText
                     }, null, 8, ["logo-text"])]),
                     _: 1
-                }, 8, ["to"]), l.operatorImgSrc ? (m(), Mt(d, {
+                }, 8, ["to"]), l.operatorImgSrc ? (m(), xt(d, {
                     key: 0,
                     class: "fr-footer__brand-link",
                     to: l.operatorTo,
                     title: l.operatorLinkText
                 }, {
-                    default: Se(() => [g("img", {
+                    default: Fe(() => [g("img", {
                         class: "fr-footer__logo fr-responsive-img",
-                        style: xn([typeof l.operatorImgStyle == "string" ? l.operatorImgStyle : "", {
+                        style: hn([typeof l.operatorImgStyle == "string" ? l.operatorImgStyle : "", {
                             "margin-left": "0.5px",
                             padding: "1rem",
                             ...typeof l.operatorImgStyle == "object" ? l.operatorImgStyle : {},
                             "max-width": "12.5rem"
                         }]),
                         src: l.operatorImgSrc,
                         alt: l.operatorImgAlt
-                    }, null, 12, tf)]),
+                    }, null, 12, ef)]),
                     _: 1
-                }, 8, ["to", "title"])) : k("", !0)]), g("div", ef, [g("p", nf, [dt(l.$slots, "description", {}, () => [vt(C(l.descText), 1)], !0)]), g("ul", rf, [(m(!0), b(un, null, Ln(l.ecosystemLinks, (h, y) => (m(), b("li", {
+                }, 8, ["to", "title"])) : k("", !0)]), g("div", nf, [g("p", rf, [dt(l.$slots, "description", {}, () => [bt(C(l.descText), 1)], !0)]), g("ul", sf, [(m(!0), v(He, null, fn(l.ecosystemLinks, (h, y) => (m(), v("li", {
                     key: y,
                     class: "fr-footer__content-item"
                 }, [g("a", {
                     class: "fr-footer__content-link",
                     href: h.href,
                     target: "_blank",
                     rel: "noopener noreferrer"
-                }, C(h.label), 9, sf)]))), 128))])])]), l.partners ? (m(), Mt(Gh, ro(pe({
+                }, C(h.label), 9, of)]))), 128))])])]), l.partners ? (m(), xt(Hh, so(re({
                     key: 0
-                }, l.partners)), null, 16)) : k("", !0), g("div", of, [g("ul", af, [(m(!0), b(un, null, Ln(e.value, (h, y) => (m(), b("li", {
+                }, l.partners)), null, 16)) : k("", !0), g("div", af, [g("ul", lf, [(m(!0), v(He, null, fn(e.value, (h, y) => (m(), v("li", {
                     key: y,
                     class: "fr-footer__bottom-item"
-                }, [typeof h.to == "string" && h.to.startsWith("http") ? (m(), b("a", {
+                }, [typeof h.to == "string" && h.to.startsWith("http") ? (m(), v("a", {
                     key: 0,
                     class: "fr-footer__bottom-link",
                     href: h.to,
                     "data-testid": h.to
-                }, C(h.label), 9, lf)) : (m(), Mt(d, {
+                }, C(h.label), 9, cf)) : (m(), xt(d, {
                     key: 1,
                     class: "fr-footer__bottom-link",
                     to: h.to ?? "#",
                     "data-testid": h.to
                 }, {
-                    default: Se(() => [vt(C(h.label), 1)]),
+                    default: Fe(() => [bt(C(h.label), 1)]),
                     _: 2
-                }, 1032, ["to", "data-testid"]))]))), 128))]), l.licenceText ? (m(), b("div", cf, [g("p", null, [vt(C(l.licenceText) + " ", 1), (m(), Mt(cn(s.value ? "a" : "RouterLink"), pe({
+                }, 1032, ["to", "data-testid"]))]))), 128))]), l.licenceText ? (m(), v("div", uf, [g("p", null, [bt(C(l.licenceText) + " ", 1), (m(), xt(dn(s.value ? "a" : "RouterLink"), re({
                     class: "fr-link-licence no-content-after",
                     to: s.value ? null : o.value,
                     href: a.value,
                     target: s.value ? "_blank" : void 0,
                     rel: "noopener noreferrer"
                 }, l.licenceLinkProps), {
-                    default: Se(() => [vt(C(l.licenceName), 1)]),
+                    default: Fe(() => [bt(C(l.licenceName), 1)]),
                     _: 1
                 }, 16, ["to", "href", "target"]))])])) : k("", !0)])])])
             }
         }
     }),
-    Cp = _s(uf, [
+    kp = Is(df, [
         ["__scopeId", "data-v-078e0714"]
     ]),
-    df = ["for"],
-    hf = {
+    hf = ["for"],
+    ff = {
         key: 0,
         class: "required"
     },
-    ff = {
+    pf = {
         key: 0,
         class: "fr-hint-text"
     },
-    pf = ht({
+    yf = ht({
         inheritAttrs: !1,
         __name: "DsfrInput",
         props: {
             id: {
-                default: () => xe("basic", "input")
+                default: () => Ce("basic", "input")
             },
             descriptionId: {
                 default: void 0
             },
             hint: {
                 default: ""
             },
@@ -10087,47 +10171,47 @@
             }
         },
         setup(n, {
             expose: t
         }) {
             const e = n,
                 i = Nl(),
-                r = It(null),
+                r = pt(null),
                 s = () => {
                     var c;
                     return (c = r.value) == null ? void 0 : c.focus()
                 },
-                o = L(() => e.isTextarea ? "textarea" : "input"),
-                a = L(() => e.isWithWrapper || i.type === "date" || !!e.wrapperClass),
-                l = L(() => ["fr-label", {
+                o = w(() => e.isTextarea ? "textarea" : "input"),
+                a = w(() => e.isWithWrapper || i.type === "date" || !!e.wrapperClass),
+                l = w(() => ["fr-label", {
                     invisible: !e.labelVisible
                 }, e.labelClass]);
             return t({
                 focus: s
-            }), (c, d) => (m(), b(un, null, [g("label", {
-                class: rt(l.value),
+            }), (c, d) => (m(), v(He, null, [g("label", {
+                class: st(l.value),
                 for: c.id
-            }, [dt(c.$slots, "label", {}, () => [vt(C(c.label) + " ", 1), dt(c.$slots, "required-tip", {}, () => [c.$attrs.required ? (m(), b("span", hf, " *")) : k("", !0)], !0)], !0), c.hint ? (m(), b("span", ff, C(c.hint), 1)) : k("", !0)], 10, df), a.value ? (m(), b("div", {
+            }, [dt(c.$slots, "label", {}, () => [bt(C(c.label) + " ", 1), dt(c.$slots, "required-tip", {}, () => [c.$attrs.required ? (m(), v("span", ff, " *")) : k("", !0)], !0)], !0), c.hint ? (m(), v("span", pf, C(c.hint), 1)) : k("", !0)], 10, hf), a.value ? (m(), v("div", {
                 key: 1,
-                class: rt([{
+                class: st([{
                     "fr-input-wrap": c.isWithWrapper || c.$attrs.type === "date"
                 }, c.wrapperClass])
-            }, [(m(), Mt(cn(o.value), pe({
+            }, [(m(), xt(dn(o.value), re({
                 id: c.id
             }, c.$attrs, {
                 ref_key: "__input",
                 ref: r,
                 class: ["fr-input", {
                     "fr-input--error": c.isInvalid,
                     "fr-input--valid": c.isValid
                 }],
                 value: c.modelValue,
                 "aria-describedby": c.descriptionId || void 0,
                 onInput: d[1] || (d[1] = h => c.$emit("update:modelValue", h.target.value))
-            }), null, 16, ["id", "class", "value", "aria-describedby"]))], 2)) : (m(), Mt(cn(o.value), pe({
+            }), null, 16, ["id", "class", "value", "aria-describedby"]))], 2)) : (m(), xt(dn(o.value), re({
                 key: 0,
                 id: c.id
             }, c.$attrs, {
                 ref_key: "__input",
                 ref: r,
                 class: ["fr-input", {
                     "fr-input--error": c.isInvalid,
@@ -10135,586 +10219,586 @@
                 }],
                 value: c.modelValue,
                 "aria-describedby": c.descriptionId || void 0,
                 onInput: d[0] || (d[0] = h => c.$emit("update:modelValue", h.target.value))
             }), null, 16, ["id", "class", "value", "aria-describedby"]))], 64))
         }
     }),
-    kp = _s(pf, [
+    Up = Is(yf, [
         ["__scopeId", "data-v-74e3acc7"]
     ]);
 /*!
  * tabbable 6.2.0
  * @license MIT, https://github.com/focus-trap/tabbable/blob/master/LICENSE
  */
-var dl = ["input:not([inert])", "select:not([inert])", "textarea:not([inert])", "a[href]:not([inert])", "button:not([inert])", "[tabindex]:not(slot):not([inert])", "audio[controls]:not([inert])", "video[controls]:not([inert])", '[contenteditable]:not([contenteditable="false"]):not([inert])', "details>summary:first-of-type:not([inert])", "details:not([inert])"],
-    Vi = dl.join(","),
-    hl = typeof Element > "u",
-    Ye = hl ? function() {} : Element.prototype.matches || Element.prototype.msMatchesSelector || Element.prototype.webkitMatchesSelector,
-    $i = !hl && Element.prototype.getRootNode ? function(n) {
+var hl = ["input:not([inert])", "select:not([inert])", "textarea:not([inert])", "a[href]:not([inert])", "button:not([inert])", "[tabindex]:not(slot):not([inert])", "audio[controls]:not([inert])", "video[controls]:not([inert])", '[contenteditable]:not([contenteditable="false"]):not([inert])', "details>summary:first-of-type:not([inert])", "details:not([inert])"],
+    Pi = hl.join(","),
+    fl = typeof Element > "u",
+    Je = fl ? function() {} : Element.prototype.matches || Element.prototype.msMatchesSelector || Element.prototype.webkitMatchesSelector,
+    ji = !fl && Element.prototype.getRootNode ? function(n) {
         var t;
         return n == null || (t = n.getRootNode) === null || t === void 0 ? void 0 : t.call(n)
     } : function(n) {
         return n?.ownerDocument
     },
-    Pi = function n(t, e) {
+    zi = function n(t, e) {
         var i;
         e === void 0 && (e = !0);
         var r = t == null || (i = t.getAttribute) === null || i === void 0 ? void 0 : i.call(t, "inert"),
             s = r === "" || r === "true",
             o = s || e && t && n(t.parentNode);
         return o
     },
-    yf = function(n) {
+    mf = function(n) {
         var t, e = n == null || (t = n.getAttribute) === null || t === void 0 ? void 0 : t.call(n, "contenteditable");
         return e === "" || e === "true"
     },
-    fl = function(n, t, e) {
-        if (Pi(n)) return [];
-        var i = Array.prototype.slice.apply(n.querySelectorAll(Vi));
-        return t && Ye.call(n, Vi) && i.unshift(n), i = i.filter(e), i
+    pl = function(n, t, e) {
+        if (zi(n)) return [];
+        var i = Array.prototype.slice.apply(n.querySelectorAll(Pi));
+        return t && Je.call(n, Pi) && i.unshift(n), i = i.filter(e), i
     },
-    pl = function n(t, e, i) {
+    yl = function n(t, e, i) {
         for (var r = [], s = Array.from(t); s.length;) {
             var o = s.shift();
-            if (!Pi(o, !1))
+            if (!zi(o, !1))
                 if (o.tagName === "SLOT") {
                     var a = o.assignedElements(),
                         l = a.length ? a : o.children,
                         c = n(l, !0, i);
                     i.flatten ? r.push.apply(r, c) : r.push({
                         scopeParent: o,
                         candidates: c
                     })
                 } else {
-                    var d = Ye.call(o, Vi);
+                    var d = Je.call(o, Pi);
                     d && i.filter(o) && (e || !t.includes(o)) && r.push(o);
                     var h = o.shadowRoot || typeof i.getShadowRoot == "function" && i.getShadowRoot(o),
-                        y = !Pi(h, !1) && (!i.shadowRootFilter || i.shadowRootFilter(o));
+                        y = !zi(h, !1) && (!i.shadowRootFilter || i.shadowRootFilter(o));
                     if (h && y) {
                         var _ = n(h === !0 ? o.children : h.children, !0, i);
                         i.flatten ? r.push.apply(r, _) : r.push({
                             scopeParent: o,
                             candidates: _
                         })
                     } else s.unshift.apply(s, o.children)
                 }
         }
         return r
     },
-    yl = function(n) {
+    ml = function(n) {
         return !isNaN(parseInt(n.getAttribute("tabindex"), 10))
     },
-    Re = function(n) {
+    Ue = function(n) {
         if (!n) throw new Error("No node provided");
-        return n.tabIndex < 0 && (/^(AUDIO|VIDEO|DETAILS)$/.test(n.tagName) || yf(n)) && !yl(n) ? 0 : n.tabIndex
-    },
-    mf = function(n, t) {
-        var e = Re(n);
-        return e < 0 && t && !yl(n) ? 0 : e
+        return n.tabIndex < 0 && (/^(AUDIO|VIDEO|DETAILS)$/.test(n.tagName) || mf(n)) && !ml(n) ? 0 : n.tabIndex
     },
     vf = function(n, t) {
+        var e = Ue(n);
+        return e < 0 && t && !ml(n) ? 0 : e
+    },
+    bf = function(n, t) {
         return n.tabIndex === t.tabIndex ? n.documentOrder - t.documentOrder : n.tabIndex - t.tabIndex
     },
-    ml = function(n) {
+    vl = function(n) {
         return n.tagName === "INPUT"
     },
-    bf = function(n) {
-        return ml(n) && n.type === "hidden"
-    },
     gf = function(n) {
+        return vl(n) && n.type === "hidden"
+    },
+    _f = function(n) {
         var t = n.tagName === "DETAILS" && Array.prototype.slice.apply(n.children).some(function(e) {
             return e.tagName === "SUMMARY"
         });
         return t
     },
-    _f = function(n, t) {
+    wf = function(n, t) {
         for (var e = 0; e < n.length; e++)
             if (n[e].checked && n[e].form === t) return n[e]
     },
-    wf = function(n) {
+    Sf = function(n) {
         if (!n.name) return !0;
-        var t = n.form || $i(n),
+        var t = n.form || ji(n),
             e = function(s) {
                 return t.querySelectorAll('input[type="radio"][name="' + s + '"]')
             },
             i;
         if (typeof window < "u" && typeof window.CSS < "u" && typeof window.CSS.escape == "function") i = e(window.CSS.escape(n.name));
         else try {
             i = e(n.name)
         } catch (s) {
             return console.error("Looks like you have a radio button with a name attribute containing invalid CSS selector characters and need the CSS.escape polyfill: %s", s.message), !1
         }
-        var r = _f(i, n.form);
+        var r = wf(i, n.form);
         return !r || r === n
     },
-    Sf = function(n) {
-        return ml(n) && n.type === "radio"
-    },
     If = function(n) {
-        return Sf(n) && !wf(n)
+        return vl(n) && n.type === "radio"
     },
     Bf = function(n) {
-        var t, e = n && $i(n),
+        return If(n) && !Sf(n)
+    },
+    Of = function(n) {
+        var t, e = n && ji(n),
             i = (t = e) === null || t === void 0 ? void 0 : t.host,
             r = !1;
         if (e && e !== n) {
             var s, o, a;
             for (r = !!((s = i) !== null && s !== void 0 && (o = s.ownerDocument) !== null && o !== void 0 && o.contains(i) || n != null && (a = n.ownerDocument) !== null && a !== void 0 && a.contains(n)); !r && i;) {
                 var l, c, d;
-                e = $i(i), i = (l = e) === null || l === void 0 ? void 0 : l.host, r = !!((c = i) !== null && c !== void 0 && (d = c.ownerDocument) !== null && d !== void 0 && d.contains(i))
+                e = ji(i), i = (l = e) === null || l === void 0 ? void 0 : l.host, r = !!((c = i) !== null && c !== void 0 && (d = c.ownerDocument) !== null && d !== void 0 && d.contains(i))
             }
         }
         return r
     },
-    Zs = function(n) {
+    Xs = function(n) {
         var t = n.getBoundingClientRect(),
             e = t.width,
             i = t.height;
         return e === 0 && i === 0
     },
-    Of = function(n, t) {
+    Ff = function(n, t) {
         var e = t.displayCheck,
             i = t.getShadowRoot;
         if (getComputedStyle(n).visibility === "hidden") return !0;
-        var r = Ye.call(n, "details>summary:first-of-type"),
+        var r = Je.call(n, "details>summary:first-of-type"),
             s = r ? n.parentElement : n;
-        if (Ye.call(s, "details:not([open]) *")) return !0;
+        if (Je.call(s, "details:not([open]) *")) return !0;
         if (!e || e === "full" || e === "legacy-full") {
             if (typeof i == "function") {
                 for (var o = n; n;) {
                     var a = n.parentElement,
-                        l = $i(n);
-                    if (a && !a.shadowRoot && i(a) === !0) return Zs(n);
+                        l = ji(n);
+                    if (a && !a.shadowRoot && i(a) === !0) return Xs(n);
                     n.assignedSlot ? n = n.assignedSlot : !a && l !== n.ownerDocument ? n = l.host : n = a
                 }
                 n = o
             }
-            if (Bf(n)) return !n.getClientRects().length;
+            if (Of(n)) return !n.getClientRects().length;
             if (e !== "legacy-full") return !0
-        } else if (e === "non-zero-area") return Zs(n);
+        } else if (e === "non-zero-area") return Xs(n);
         return !1
     },
-    Ff = function(n) {
+    Af = function(n) {
         if (/^(INPUT|BUTTON|SELECT|TEXTAREA)$/.test(n.tagName))
             for (var t = n.parentElement; t;) {
                 if (t.tagName === "FIELDSET" && t.disabled) {
                     for (var e = 0; e < t.children.length; e++) {
                         var i = t.children.item(e);
-                        if (i.tagName === "LEGEND") return Ye.call(t, "fieldset[disabled] *") ? !0 : !i.contains(n)
+                        if (i.tagName === "LEGEND") return Je.call(t, "fieldset[disabled] *") ? !0 : !i.contains(n)
                     }
                     return !0
                 }
                 t = t.parentElement
             }
         return !1
     },
-    ji = function(n, t) {
-        return !(t.disabled || Pi(t) || bf(t) || Of(t, n) || gf(t) || Ff(t))
+    Wi = function(n, t) {
+        return !(t.disabled || zi(t) || gf(t) || Ff(t, n) || _f(t) || Af(t))
     },
-    Lr = function(n, t) {
-        return !(If(t) || Re(t) < 0 || !ji(n, t))
+    Cr = function(n, t) {
+        return !(Bf(t) || Ue(t) < 0 || !Wi(n, t))
     },
-    Af = function(n) {
+    Df = function(n) {
         var t = parseInt(n.getAttribute("tabindex"), 10);
         return !!(isNaN(t) || t >= 0)
     },
-    Df = function n(t) {
+    Tf = function n(t) {
         var e = [],
             i = [];
         return t.forEach(function(r, s) {
             var o = !!r.scopeParent,
                 a = o ? r.scopeParent : r,
-                l = mf(a, o),
+                l = vf(a, o),
                 c = o ? n(r.candidates) : a;
             l === 0 ? o ? e.push.apply(e, c) : e.push(a) : i.push({
                 documentOrder: s,
                 tabIndex: l,
                 item: r,
                 isScope: o,
                 content: c
             })
-        }), i.sort(vf).reduce(function(r, s) {
+        }), i.sort(bf).reduce(function(r, s) {
             return s.isScope ? r.push.apply(r, s.content) : r.push(s.content), r
         }, []).concat(e)
     },
-    Tf = function(n, t) {
+    Nf = function(n, t) {
         t = t || {};
         var e;
-        return t.getShadowRoot ? e = pl([n], t.includeContainer, {
-            filter: Lr.bind(null, t),
+        return t.getShadowRoot ? e = yl([n], t.includeContainer, {
+            filter: Cr.bind(null, t),
             flatten: !1,
             getShadowRoot: t.getShadowRoot,
-            shadowRootFilter: Af
-        }) : e = fl(n, t.includeContainer, Lr.bind(null, t)), Df(e)
+            shadowRootFilter: Df
+        }) : e = pl(n, t.includeContainer, Cr.bind(null, t)), Tf(e)
     },
-    Nf = function(n, t) {
+    xf = function(n, t) {
         t = t || {};
         var e;
-        return t.getShadowRoot ? e = pl([n], t.includeContainer, {
-            filter: ji.bind(null, t),
+        return t.getShadowRoot ? e = yl([n], t.includeContainer, {
+            filter: Wi.bind(null, t),
             flatten: !0,
             getShadowRoot: t.getShadowRoot
-        }) : e = fl(n, t.includeContainer, ji.bind(null, t)), e
+        }) : e = pl(n, t.includeContainer, Wi.bind(null, t)), e
     },
-    Ze = function(n, t) {
+    Qe = function(n, t) {
         if (t = t || {}, !n) throw new Error("No node provided");
-        return Ye.call(n, Vi) === !1 ? !1 : Lr(t, n)
+        return Je.call(n, Pi) === !1 ? !1 : Cr(t, n)
     },
-    Mf = dl.concat("iframe").join(","),
-    yr = function(n, t) {
+    Mf = hl.concat("iframe").join(","),
+    vr = function(n, t) {
         if (t = t || {}, !n) throw new Error("No node provided");
-        return Ye.call(n, Mf) === !1 ? !1 : ji(t, n)
+        return Je.call(n, Mf) === !1 ? !1 : Wi(t, n)
     };
 /*!
  * focus-trap 7.5.4
  * @license MIT, https://github.com/focus-trap/focus-trap/blob/master/LICENSE
  */
-function Xs(n, t) {
+function Qs(n, t) {
     var e = Object.keys(n);
     if (Object.getOwnPropertySymbols) {
         var i = Object.getOwnPropertySymbols(n);
         t && (i = i.filter(function(r) {
             return Object.getOwnPropertyDescriptor(n, r).enumerable
         })), e.push.apply(e, i)
     }
     return e
 }
 
-function Qs(n) {
+function to(n) {
     for (var t = 1; t < arguments.length; t++) {
         var e = arguments[t] != null ? arguments[t] : {};
-        t % 2 ? Xs(Object(e), !0).forEach(function(i) {
-            xf(n, i, e[i])
-        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(n, Object.getOwnPropertyDescriptors(e)) : Xs(Object(e)).forEach(function(i) {
+        t % 2 ? Qs(Object(e), !0).forEach(function(i) {
+            Lf(n, i, e[i])
+        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(n, Object.getOwnPropertyDescriptors(e)) : Qs(Object(e)).forEach(function(i) {
             Object.defineProperty(n, i, Object.getOwnPropertyDescriptor(e, i))
         })
     }
     return n
 }
 
-function xf(n, t, e) {
-    return t = Ef(t), t in n ? Object.defineProperty(n, t, {
+function Lf(n, t, e) {
+    return t = Rf(t), t in n ? Object.defineProperty(n, t, {
         value: e,
         enumerable: !0,
         configurable: !0,
         writable: !0
     }) : n[t] = e, n
 }
 
-function Lf(n, t) {
+function Ef(n, t) {
     if (typeof n != "object" || n === null) return n;
     var e = n[Symbol.toPrimitive];
     if (e !== void 0) {
         var i = e.call(n, t || "default");
         if (typeof i != "object") return i;
         throw new TypeError("@@toPrimitive must return a primitive value.")
     }
     return (t === "string" ? String : Number)(n)
 }
 
-function Ef(n) {
-    var t = Lf(n, "string");
+function Rf(n) {
+    var t = Ef(n, "string");
     return typeof t == "symbol" ? t : String(t)
 }
-var to = {
+var eo = {
         activateTrap: function(n, t) {
             if (n.length > 0) {
                 var e = n[n.length - 1];
                 e !== t && e.pause()
             }
             var i = n.indexOf(t);
             i === -1 || n.splice(i, 1), n.push(t)
         },
         deactivateTrap: function(n, t) {
             var e = n.indexOf(t);
             e !== -1 && n.splice(e, 1), n.length > 0 && n[n.length - 1].unpause()
         }
     },
-    Rf = function(n) {
+    Cf = function(n) {
         return n.tagName && n.tagName.toLowerCase() === "input" && typeof n.select == "function"
     },
-    Cf = function(n) {
+    kf = function(n) {
         return n?.key === "Escape" || n?.key === "Esc" || n?.keyCode === 27
     },
-    Mn = function(n) {
+    En = function(n) {
         return n?.key === "Tab" || n?.keyCode === 9
     },
-    kf = function(n) {
-        return Mn(n) && !n.shiftKey
-    },
     Uf = function(n) {
-        return Mn(n) && n.shiftKey
+        return En(n) && !n.shiftKey
     },
-    eo = function(n) {
+    $f = function(n) {
+        return En(n) && n.shiftKey
+    },
+    no = function(n) {
         return setTimeout(n, 0)
     },
-    no = function(n, t) {
+    io = function(n, t) {
         var e = -1;
         return n.every(function(i, r) {
             return t(i) ? (e = r, !1) : !0
         }), e
     },
-    On = function(n) {
+    Dn = function(n) {
         for (var t = arguments.length, e = new Array(t > 1 ? t - 1 : 0), i = 1; i < t; i++) e[i - 1] = arguments[i];
         return typeof n == "function" ? n.apply(void 0, e) : n
     },
-    ti = function(n) {
+    ni = function(n) {
         return n.target.shadowRoot && typeof n.composedPath == "function" ? n.composedPath()[0] : n.target
     },
     Vf = [],
-    $f = function(n, t) {
+    Pf = function(n, t) {
         var e = t?.document || document,
             i = t?.trapStack || Vf,
-            r = Qs({
+            r = to({
                 returnFocusOnDeactivate: !0,
                 escapeDeactivates: !0,
                 delayInitialFocus: !0,
-                isKeyForward: kf,
-                isKeyBackward: Uf
+                isKeyForward: Uf,
+                isKeyBackward: $f
             }, t),
             s = {
                 containers: [],
                 containerGroups: [],
                 tabbableGroups: [],
                 nodeFocusedBeforeActivation: null,
                 mostRecentlyFocusedNode: null,
                 active: !1,
                 paused: !1,
                 delayInitialFocusTimer: void 0,
                 recentNavEvent: void 0
             },
-            o, a = function(p, f, v) {
-                return p && p[f] !== void 0 ? p[f] : r[v || f]
+            o, a = function(p, f, b) {
+                return p && p[f] !== void 0 ? p[f] : r[b || f]
             },
             l = function(p, f) {
-                var v = typeof f?.composedPath == "function" ? f.composedPath() : void 0;
-                return s.containerGroups.findIndex(function(Z) {
-                    var H = Z.container,
-                        it = Z.tabbableNodes;
-                    return H.contains(p) || v?.includes(H) || it.find(function(at) {
+                var b = typeof f?.composedPath == "function" ? f.composedPath() : void 0;
+                return s.containerGroups.findIndex(function(Q) {
+                    var J = Q.container,
+                        rt = Q.tabbableNodes;
+                    return J.contains(p) || b?.includes(J) || rt.find(function(at) {
                         return at === p
                     })
                 })
             },
             c = function(p) {
                 var f = r[p];
                 if (typeof f == "function") {
-                    for (var v = arguments.length, Z = new Array(v > 1 ? v - 1 : 0), H = 1; H < v; H++) Z[H - 1] = arguments[H];
-                    f = f.apply(void 0, Z)
+                    for (var b = arguments.length, Q = new Array(b > 1 ? b - 1 : 0), J = 1; J < b; J++) Q[J - 1] = arguments[J];
+                    f = f.apply(void 0, Q)
                 }
                 if (f === !0 && (f = void 0), !f) {
                     if (f === void 0 || f === !1) return f;
                     throw new Error("`".concat(p, "` was specified but was not a node, or did not return a node"))
                 }
-                var it = f;
-                if (typeof f == "string" && (it = e.querySelector(f), !it)) throw new Error("`".concat(p, "` as selector refers to no known node"));
-                return it
+                var rt = f;
+                if (typeof f == "string" && (rt = e.querySelector(f), !rt)) throw new Error("`".concat(p, "` as selector refers to no known node"));
+                return rt
             },
             d = function() {
                 var p = c("initialFocus");
                 if (p === !1) return !1;
-                if (p === void 0 || !yr(p, r.tabbableOptions))
+                if (p === void 0 || !vr(p, r.tabbableOptions))
                     if (l(e.activeElement) >= 0) p = e.activeElement;
                     else {
                         var f = s.tabbableGroups[0],
-                            v = f && f.firstTabbableNode;
-                        p = v || c("fallbackFocus")
+                            b = f && f.firstTabbableNode;
+                        p = b || c("fallbackFocus")
                     } if (!p) throw new Error("Your focus-trap needs to have at least one focusable element");
                 return p
             },
             h = function() {
                 if (s.containerGroups = s.containers.map(function(p) {
-                        var f = Tf(p, r.tabbableOptions),
-                            v = Nf(p, r.tabbableOptions),
-                            Z = f.length > 0 ? f[0] : void 0,
-                            H = f.length > 0 ? f[f.length - 1] : void 0,
-                            it = v.find(function(lt) {
-                                return Ze(lt)
+                        var f = Nf(p, r.tabbableOptions),
+                            b = xf(p, r.tabbableOptions),
+                            Q = f.length > 0 ? f[0] : void 0,
+                            J = f.length > 0 ? f[f.length - 1] : void 0,
+                            rt = b.find(function(lt) {
+                                return Qe(lt)
                             }),
-                            at = v.slice().reverse().find(function(lt) {
-                                return Ze(lt)
+                            at = b.slice().reverse().find(function(lt) {
+                                return Qe(lt)
                             }),
-                            bt = !!f.find(function(lt) {
-                                return Re(lt) > 0
+                            gt = !!f.find(function(lt) {
+                                return Ue(lt) > 0
                             });
                         return {
                             container: p,
                             tabbableNodes: f,
-                            focusableNodes: v,
-                            posTabIndexesFound: bt,
-                            firstTabbableNode: Z,
-                            lastTabbableNode: H,
-                            firstDomTabbableNode: it,
+                            focusableNodes: b,
+                            posTabIndexesFound: gt,
+                            firstTabbableNode: Q,
+                            lastTabbableNode: J,
+                            firstDomTabbableNode: rt,
                             lastDomTabbableNode: at,
                             nextTabbableNode: function(lt) {
-                                var Je = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0,
-                                    In = f.indexOf(lt);
-                                return In < 0 ? Je ? v.slice(v.indexOf(lt) + 1).find(function(se) {
-                                    return Ze(se)
-                                }) : v.slice(0, v.indexOf(lt)).reverse().find(function(se) {
-                                    return Ze(se)
-                                }) : f[In + (Je ? 1 : -1)]
+                                var Ze = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0,
+                                    Fn = f.indexOf(lt);
+                                return Fn < 0 ? Ze ? b.slice(b.indexOf(lt) + 1).find(function(ce) {
+                                    return Qe(ce)
+                                }) : b.slice(0, b.indexOf(lt)).reverse().find(function(ce) {
+                                    return Qe(ce)
+                                }) : f[Fn + (Ze ? 1 : -1)]
                             }
                         }
                     }), s.tabbableGroups = s.containerGroups.filter(function(p) {
                         return p.tabbableNodes.length > 0
                     }), s.tabbableGroups.length <= 0 && !c("fallbackFocus")) throw new Error("Your focus-trap must have at least one container with at least one tabbable node in it at all times");
                 if (s.containerGroups.find(function(p) {
                         return p.posTabIndexesFound
                     }) && s.containerGroups.length > 1) throw new Error("At least one node with a positive tabindex was found in one of your focus-trap's multiple containers. Positive tabindexes are only supported in single-container focus-traps.")
             },
             y = function p(f) {
-                var v = f.activeElement;
-                if (v) return v.shadowRoot && v.shadowRoot.activeElement !== null ? p(v.shadowRoot) : v
+                var b = f.activeElement;
+                if (b) return b.shadowRoot && b.shadowRoot.activeElement !== null ? p(b.shadowRoot) : b
             },
             _ = function p(f) {
                 if (f !== !1 && f !== y(document)) {
                     if (!f || !f.focus) {
                         p(d());
                         return
                     }
                     f.focus({
                         preventScroll: !!r.preventScroll
-                    }), s.mostRecentlyFocusedNode = f, Rf(f) && f.select()
+                    }), s.mostRecentlyFocusedNode = f, Cf(f) && f.select()
                 }
             },
-            G = function(p) {
+            V = function(p) {
                 var f = c("setReturnFocus", p);
                 return f || (f === !1 ? !1 : p)
             },
-            et = function(p) {
+            P = function(p) {
                 var f = p.target,
-                    v = p.event,
-                    Z = p.isBackward,
-                    H = Z === void 0 ? !1 : Z;
-                f = f || ti(v), h();
-                var it = null;
+                    b = p.event,
+                    Q = p.isBackward,
+                    J = Q === void 0 ? !1 : Q;
+                f = f || ni(b), h();
+                var rt = null;
                 if (s.tabbableGroups.length > 0) {
-                    var at = l(f, v),
-                        bt = at >= 0 ? s.containerGroups[at] : void 0;
-                    if (at < 0) H ? it = s.tabbableGroups[s.tabbableGroups.length - 1].lastTabbableNode : it = s.tabbableGroups[0].firstTabbableNode;
-                    else if (H) {
-                        var lt = no(s.tabbableGroups, function(rr) {
-                            var sr = rr.firstTabbableNode;
-                            return f === sr
+                    var at = l(f, b),
+                        gt = at >= 0 ? s.containerGroups[at] : void 0;
+                    if (at < 0) J ? rt = s.tabbableGroups[s.tabbableGroups.length - 1].lastTabbableNode : rt = s.tabbableGroups[0].firstTabbableNode;
+                    else if (J) {
+                        var lt = io(s.tabbableGroups, function(or) {
+                            var ar = or.firstTabbableNode;
+                            return f === ar
                         });
-                        if (lt < 0 && (bt.container === f || yr(f, r.tabbableOptions) && !Ze(f, r.tabbableOptions) && !bt.nextTabbableNode(f, !1)) && (lt = at), lt >= 0) {
-                            var Je = lt === 0 ? s.tabbableGroups.length - 1 : lt - 1,
-                                In = s.tabbableGroups[Je];
-                            it = Re(f) >= 0 ? In.lastTabbableNode : In.lastDomTabbableNode
-                        } else Mn(v) || (it = bt.nextTabbableNode(f, !1))
+                        if (lt < 0 && (gt.container === f || vr(f, r.tabbableOptions) && !Qe(f, r.tabbableOptions) && !gt.nextTabbableNode(f, !1)) && (lt = at), lt >= 0) {
+                            var Ze = lt === 0 ? s.tabbableGroups.length - 1 : lt - 1,
+                                Fn = s.tabbableGroups[Ze];
+                            rt = Ue(f) >= 0 ? Fn.lastTabbableNode : Fn.lastDomTabbableNode
+                        } else En(b) || (rt = gt.nextTabbableNode(f, !1))
                     } else {
-                        var se = no(s.tabbableGroups, function(rr) {
-                            var sr = rr.lastTabbableNode;
-                            return f === sr
+                        var ce = io(s.tabbableGroups, function(or) {
+                            var ar = or.lastTabbableNode;
+                            return f === ar
                         });
-                        if (se < 0 && (bt.container === f || yr(f, r.tabbableOptions) && !Ze(f, r.tabbableOptions) && !bt.nextTabbableNode(f)) && (se = at), se >= 0) {
-                            var bl = se === s.tabbableGroups.length - 1 ? 0 : se + 1,
-                                Ss = s.tabbableGroups[bl];
-                            it = Re(f) >= 0 ? Ss.firstTabbableNode : Ss.firstDomTabbableNode
-                        } else Mn(v) || (it = bt.nextTabbableNode(f))
+                        if (ce < 0 && (gt.container === f || vr(f, r.tabbableOptions) && !Qe(f, r.tabbableOptions) && !gt.nextTabbableNode(f)) && (ce = at), ce >= 0) {
+                            var bl = ce === s.tabbableGroups.length - 1 ? 0 : ce + 1,
+                                Bs = s.tabbableGroups[bl];
+                            rt = Ue(f) >= 0 ? Bs.firstTabbableNode : Bs.firstDomTabbableNode
+                        } else En(b) || (rt = gt.nextTabbableNode(f))
                     }
-                } else it = c("fallbackFocus");
-                return it
+                } else rt = c("fallbackFocus");
+                return rt
             },
-            ot = function(p) {
-                var f = ti(p);
+            et = function(p) {
+                var f = ni(p);
                 if (!(l(f, p) >= 0)) {
-                    if (On(r.clickOutsideDeactivates, p)) {
+                    if (Dn(r.clickOutsideDeactivates, p)) {
                         o.deactivate({
                             returnFocus: r.returnFocusOnDeactivate
                         });
                         return
                     }
-                    On(r.allowOutsideClick, p) || p.preventDefault()
+                    Dn(r.allowOutsideClick, p) || p.preventDefault()
                 }
             },
-            nt = function(p) {
-                var f = ti(p),
-                    v = l(f, p) >= 0;
-                if (v || f instanceof Document) v && (s.mostRecentlyFocusedNode = f);
+            q = function(p) {
+                var f = ni(p),
+                    b = l(f, p) >= 0;
+                if (b || f instanceof Document) b && (s.mostRecentlyFocusedNode = f);
                 else {
                     p.stopImmediatePropagation();
-                    var Z, H = !0;
+                    var Q, J = !0;
                     if (s.mostRecentlyFocusedNode)
-                        if (Re(s.mostRecentlyFocusedNode) > 0) {
-                            var it = l(s.mostRecentlyFocusedNode),
-                                at = s.containerGroups[it].tabbableNodes;
+                        if (Ue(s.mostRecentlyFocusedNode) > 0) {
+                            var rt = l(s.mostRecentlyFocusedNode),
+                                at = s.containerGroups[rt].tabbableNodes;
                             if (at.length > 0) {
-                                var bt = at.findIndex(function(lt) {
+                                var gt = at.findIndex(function(lt) {
                                     return lt === s.mostRecentlyFocusedNode
                                 });
-                                bt >= 0 && (r.isKeyForward(s.recentNavEvent) ? bt + 1 < at.length && (Z = at[bt + 1], H = !1) : bt - 1 >= 0 && (Z = at[bt - 1], H = !1))
+                                gt >= 0 && (r.isKeyForward(s.recentNavEvent) ? gt + 1 < at.length && (Q = at[gt + 1], J = !1) : gt - 1 >= 0 && (Q = at[gt - 1], J = !1))
                             }
                         } else s.containerGroups.some(function(lt) {
-                            return lt.tabbableNodes.some(function(Je) {
-                                return Re(Je) > 0
+                            return lt.tabbableNodes.some(function(Ze) {
+                                return Ue(Ze) > 0
                             })
-                        }) || (H = !1);
-                    else H = !1;
-                    H && (Z = et({
+                        }) || (J = !1);
+                    else J = !1;
+                    J && (Q = P({
                         target: s.mostRecentlyFocusedNode,
                         isBackward: r.isKeyBackward(s.recentNavEvent)
-                    })), _(Z || s.mostRecentlyFocusedNode || d())
+                    })), _(Q || s.mostRecentlyFocusedNode || d())
                 }
                 s.recentNavEvent = void 0
             },
-            He = function(p) {
+            Rt = function(p) {
                 var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
                 s.recentNavEvent = p;
-                var v = et({
+                var b = P({
                     event: p,
                     isBackward: f
                 });
-                v && (Mn(p) && p.preventDefault(), _(v))
+                b && (En(p) && p.preventDefault(), _(b))
             },
-            wn = function(p) {
-                if (Cf(p) && On(r.escapeDeactivates, p) !== !1) {
+            le = function(p) {
+                if (kf(p) && Dn(r.escapeDeactivates, p) !== !1) {
                     p.preventDefault(), o.deactivate();
                     return
-                }(r.isKeyForward(p) || r.isKeyBackward(p)) && He(p, r.isKeyBackward(p))
+                }(r.isKeyForward(p) || r.isKeyBackward(p)) && Rt(p, r.isKeyBackward(p))
             },
-            Le = function(p) {
-                var f = ti(p);
-                l(f, p) >= 0 || On(r.clickOutsideDeactivates, p) || On(r.allowOutsideClick, p) || (p.preventDefault(), p.stopImmediatePropagation())
+            Yt = function(p) {
+                var f = ni(p);
+                l(f, p) >= 0 || Dn(r.clickOutsideDeactivates, p) || Dn(r.allowOutsideClick, p) || (p.preventDefault(), p.stopImmediatePropagation())
             },
-            qe = function() {
-                if (s.active) return to.activateTrap(i, o), s.delayInitialFocusTimer = r.delayInitialFocus ? eo(function() {
+            Se = function() {
+                if (s.active) return eo.activateTrap(i, o), s.delayInitialFocusTimer = r.delayInitialFocus ? no(function() {
                     _(d())
-                }) : _(d()), e.addEventListener("focusin", nt, !0), e.addEventListener("mousedown", ot, {
+                }) : _(d()), e.addEventListener("focusin", q, !0), e.addEventListener("mousedown", et, {
                     capture: !0,
                     passive: !1
-                }), e.addEventListener("touchstart", ot, {
+                }), e.addEventListener("touchstart", et, {
                     capture: !0,
                     passive: !1
-                }), e.addEventListener("click", Le, {
+                }), e.addEventListener("click", Yt, {
                     capture: !0,
                     passive: !1
-                }), e.addEventListener("keydown", wn, {
+                }), e.addEventListener("keydown", le, {
                     capture: !0,
                     passive: !1
                 }), o
             },
-            ws = function() {
-                if (s.active) return e.removeEventListener("focusin", nt, !0), e.removeEventListener("mousedown", ot, !0), e.removeEventListener("touchstart", ot, !0), e.removeEventListener("click", Le, !0), e.removeEventListener("keydown", wn, !0), o
+            Zn = function() {
+                if (s.active) return e.removeEventListener("focusin", q, !0), e.removeEventListener("mousedown", et, !0), e.removeEventListener("touchstart", et, !0), e.removeEventListener("click", Yt, !0), e.removeEventListener("keydown", le, !0), o
             },
-            vl = function(p) {
-                var f = p.some(function(v) {
-                    var Z = Array.from(v.removedNodes);
-                    return Z.some(function(H) {
-                        return H === s.mostRecentlyFocusedNode
+            Xn = function(p) {
+                var f = p.some(function(b) {
+                    var Q = Array.from(b.removedNodes);
+                    return Q.some(function(J) {
+                        return J === s.mostRecentlyFocusedNode
                     })
                 });
                 f && _(d())
             },
-            ir = typeof window < "u" && "MutationObserver" in window ? new MutationObserver(vl) : void 0,
-            Sn = function() {
-                ir && (ir.disconnect(), s.active && !s.paused && s.containers.map(function(p) {
-                    ir.observe(p, {
+            sr = typeof window < "u" && "MutationObserver" in window ? new MutationObserver(Xn) : void 0,
+            On = function() {
+                sr && (sr.disconnect(), s.active && !s.paused && s.containers.map(function(p) {
+                    sr.observe(p, {
                         subtree: !0,
                         childList: !0
                     })
                 }))
             };
         return o = {
             get active() {
@@ -10722,68 +10806,68 @@
             },
             get paused() {
                 return s.paused
             },
             activate: function(p) {
                 if (s.active) return this;
                 var f = a(p, "onActivate"),
-                    v = a(p, "onPostActivate"),
-                    Z = a(p, "checkCanFocusTrap");
-                Z || h(), s.active = !0, s.paused = !1, s.nodeFocusedBeforeActivation = e.activeElement, f?.();
-                var H = function() {
-                    Z && h(), qe(), Sn(), v?.()
+                    b = a(p, "onPostActivate"),
+                    Q = a(p, "checkCanFocusTrap");
+                Q || h(), s.active = !0, s.paused = !1, s.nodeFocusedBeforeActivation = e.activeElement, f?.();
+                var J = function() {
+                    Q && h(), Se(), On(), b?.()
                 };
-                return Z ? (Z(s.containers.concat()).then(H, H), this) : (H(), this)
+                return Q ? (Q(s.containers.concat()).then(J, J), this) : (J(), this)
             },
             deactivate: function(p) {
                 if (!s.active) return this;
-                var f = Qs({
+                var f = to({
                     onDeactivate: r.onDeactivate,
                     onPostDeactivate: r.onPostDeactivate,
                     checkCanReturnFocus: r.checkCanReturnFocus
                 }, p);
-                clearTimeout(s.delayInitialFocusTimer), s.delayInitialFocusTimer = void 0, ws(), s.active = !1, s.paused = !1, Sn(), to.deactivateTrap(i, o);
-                var v = a(f, "onDeactivate"),
-                    Z = a(f, "onPostDeactivate"),
-                    H = a(f, "checkCanReturnFocus"),
-                    it = a(f, "returnFocus", "returnFocusOnDeactivate");
-                v?.();
+                clearTimeout(s.delayInitialFocusTimer), s.delayInitialFocusTimer = void 0, Zn(), s.active = !1, s.paused = !1, On(), eo.deactivateTrap(i, o);
+                var b = a(f, "onDeactivate"),
+                    Q = a(f, "onPostDeactivate"),
+                    J = a(f, "checkCanReturnFocus"),
+                    rt = a(f, "returnFocus", "returnFocusOnDeactivate");
+                b?.();
                 var at = function() {
-                    eo(function() {
-                        it && _(G(s.nodeFocusedBeforeActivation)), Z?.()
+                    no(function() {
+                        rt && _(V(s.nodeFocusedBeforeActivation)), Q?.()
                     })
                 };
-                return it && H ? (H(G(s.nodeFocusedBeforeActivation)).then(at, at), this) : (at(), this)
+                return rt && J ? (J(V(s.nodeFocusedBeforeActivation)).then(at, at), this) : (at(), this)
             },
             pause: function(p) {
                 if (s.paused || !s.active) return this;
                 var f = a(p, "onPause"),
-                    v = a(p, "onPostPause");
-                return s.paused = !0, f?.(), ws(), Sn(), v?.(), this
+                    b = a(p, "onPostPause");
+                return s.paused = !0, f?.(), Zn(), On(), b?.(), this
             },
             unpause: function(p) {
                 if (!s.paused || !s.active) return this;
                 var f = a(p, "onUnpause"),
-                    v = a(p, "onPostUnpause");
-                return s.paused = !1, f?.(), h(), qe(), Sn(), v?.(), this
+                    b = a(p, "onPostUnpause");
+                return s.paused = !1, f?.(), h(), Se(), On(), b?.(), this
             },
             updateContainerElements: function(p) {
                 var f = [].concat(p).filter(Boolean);
-                return s.containers = f.map(function(v) {
-                    return typeof v == "string" ? e.querySelector(v) : v
-                }), s.active && h(), Sn(), this
+                return s.containers = f.map(function(b) {
+                    return typeof b == "string" ? e.querySelector(b) : b
+                }), s.active && h(), On(), this
             }
         }, o.updateContainerElements(n), o
     };
 /*!
  * focus-trap-vue v4.0.2
  * (c) 2023 Eduardo San Martin Morote
  * @license MIT
  */
-const Pf = {
+const jf = {
     escapeDeactivates: {
         type: Boolean,
         default: !0
     },
     returnFocusOnDeactivate: {
         type: Boolean,
         default: !0
@@ -10808,32 +10892,32 @@
 };
 ht({
     props: Object.assign({
         active: {
             type: Boolean,
             default: !0
         }
-    }, Pf),
+    }, jf),
     emits: ["update:active", "activate", "postActivate", "deactivate", "postDeactivate"],
     render() {
         return this.renderImpl()
     },
     setup(n, {
         slots: t,
         emit: e
     }) {
         let i;
-        const r = It(null),
-            s = L(() => {
+        const r = pt(null),
+            s = w(() => {
                 const a = r.value;
                 return a && (a instanceof HTMLElement ? a : a.$el)
             });
 
         function o() {
-            return i || (i = $f(s.value, {
+            return i || (i = Pf(s.value, {
                 escapeDeactivates: n.escapeDeactivates,
                 allowOutsideClick: n.allowOutsideClick,
                 returnFocusOnDeactivate: n.returnFocusOnDeactivate,
                 clickOutsideDeactivates: n.clickOutsideDeactivates,
                 onActivate: () => {
                     e("update:active", !0), e("activate")
                 },
@@ -10845,22 +10929,22 @@
                 initialFocus: n.initialFocus,
                 fallbackFocus: n.fallbackFocus,
                 tabbableOptions: n.tabbableOptions,
                 delayInitialFocus: n.delayInitialFocus,
                 preventScroll: n.preventScroll
             }))
         }
-        return Pn(() => {
-            Rr(() => n.active, a => {
+        return wn(() => {
+            Ur(() => n.active, a => {
                 a && s.value ? o().activate() : i && (i.deactivate(), (!s.value || s.value.nodeType === Node.COMMENT_NODE) && (i = null))
             }, {
                 immediate: !0,
                 flush: "post"
             })
-        }), io(() => {
+        }), ro(() => {
             i && i.deactivate(), i = null
         }), {
             activate() {
                 o().activate()
             },
             deactivate() {
                 i && i.deactivate()
@@ -10871,23 +10955,23 @@
                 return !a || !a.length || a.length > 1 ? (console.error("[focus-trap-vue]: FocusTrap requires exactly one child."), a) : Bl(a[0], {
                     ref: r
                 })
             }
         }
     }
 });
-const jf = ["aria-label"],
-    zf = {
+const zf = ["aria-label"],
+    Wf = {
         class: "fr-content-media__img"
     },
-    Wf = ["src", "alt", "title", "ratio"],
-    Yf = {
+    Yf = ["src", "alt", "title", "ratio"],
+    Gf = {
         class: "fr-content-media__caption"
     },
-    Up = ht({
+    $p = ht({
         __name: "DsfrPicture",
         props: {
             alt: {
                 default: ""
             },
             legend: {
                 default: ""
@@ -10900,51 +10984,51 @@
                 default: ""
             },
             ratio: {
                 default: "16x9"
             }
         },
         setup(n) {
-            return (t, e) => (m(), b("figure", {
-                class: rt(["fr-content-media", {
+            return (t, e) => (m(), v("figure", {
+                class: st(["fr-content-media", {
                     "fr-content-media--sm": t.size == "small",
                     "fr-content-media--lg": t.size == "large"
                 }]),
                 role: "group",
                 "aria-label": t.legend
-            }, [g("div", zf, [dt(t.$slots, "default", {}, () => [t.src ? (m(), b("img", {
+            }, [g("div", Wf, [dt(t.$slots, "default", {}, () => [t.src ? (m(), v("img", {
                 key: 0,
                 src: t.src,
-                class: rt(["fr-responsive-img", `fr-ratio-${t.ratio}`]),
+                class: st(["fr-responsive-img", `fr-ratio-${t.ratio}`]),
                 alt: t.alt,
                 title: t.title,
                 ratio: t.ratio
-            }, null, 10, Wf)) : k("", !0)])]), g("figcaption", Yf, C(t.legend), 1)], 10, jf))
+            }, null, 10, Yf)) : k("", !0)])]), g("figcaption", Gf, C(t.legend), 1)], 10, zf))
         }
     }),
-    Gf = ["id", "name", "value", "checked"],
-    Hf = ["for"],
-    qf = {
+    Hf = ["id", "name", "value", "checked"],
+    qf = ["for"],
+    Jf = {
         key: 0,
         class: "required"
     },
-    Jf = {
+    Kf = {
         key: 0,
         class: "fr-hint-text"
     },
-    Kf = {
+    Zf = {
         key: 0,
         class: "fr-radio-rich__pictogram"
     },
-    Zf = ["src"],
-    Xf = ht({
+    Xf = ["src"],
+    Qf = ht({
         __name: "DsfrRadioButton",
         props: {
             id: {
-                default: () => xe("basic", "checkbox")
+                default: () => Ce("basic", "checkbox")
             },
             name: {},
             modelValue: {
                 default: ""
             },
             small: {
                 type: Boolean
@@ -10962,59 +11046,59 @@
             img: {
                 default: ""
             }
         },
         emits: ["update:modelValue"],
         setup(n) {
             const t = n,
-                e = L(() => !!t.img);
-            return (i, r) => (m(), b("div", {
-                class: rt(["fr-fieldset__element", {
+                e = w(() => !!t.img);
+            return (i, r) => (m(), v("div", {
+                class: st(["fr-fieldset__element", {
                     "fr-fieldset__element--inline": i.inline
                 }])
             }, [g("div", {
-                class: rt(["fr-radio-group", {
+                class: st(["fr-radio-group", {
                     "fr-radio-rich": e.value,
                     "fr-radio-group--sm": i.small
                 }])
-            }, [g("input", pe({
+            }, [g("input", re({
                 id: i.id,
                 type: "radio",
                 name: i.name,
                 value: i.value,
                 checked: i.modelValue === i.value
             }, i.$attrs, {
                 onClick: r[0] || (r[0] = s => i.$emit("update:modelValue", i.value))
-            }), null, 16, Gf), g("label", {
+            }), null, 16, Hf), g("label", {
                 for: i.id,
                 class: "fr-label"
-            }, [dt(i.$slots, "label", {}, () => [vt(C(i.label) + " ", 1), dt(i.$slots, "required-tip", {}, () => [i.$attrs.required ? (m(), b("span", qf, " *")) : k("", !0)])]), i.hint ? (m(), b("span", Jf, C(i.hint), 1)) : k("", !0)], 8, Hf), i.img ? (m(), b("div", Kf, [g("img", {
+            }, [dt(i.$slots, "label", {}, () => [bt(C(i.label) + " ", 1), dt(i.$slots, "required-tip", {}, () => [i.$attrs.required ? (m(), v("span", Jf, " *")) : k("", !0)])]), i.hint ? (m(), v("span", Kf, C(i.hint), 1)) : k("", !0)], 8, qf), i.img ? (m(), v("div", Zf, [g("img", {
                 src: i.img,
                 alt: ""
-            }, null, 8, Zf)])) : k("", !0)], 2)], 2))
+            }, null, 8, Xf)])) : k("", !0)], 2)], 2))
         }
     }),
-    Qf = {
+    tp = {
         class: "fr-form-group"
     },
-    tp = ["disabled", "aria-labelledby", "role"],
-    ep = ["id"],
-    np = {
+    ep = ["disabled", "aria-labelledby", "role"],
+    np = ["id"],
+    ip = {
         key: 0,
         class: "required"
     },
-    ip = ["id"],
-    rp = {
+    rp = ["id"],
+    sp = {
         class: "line-1"
     },
     Vp = ht({
         __name: "DsfrRadioButtonSet",
         props: {
             titleId: {
-                default: () => xe("radio-button", "group")
+                default: () => Ce("radio-button", "group")
             },
             disabled: {
                 type: Boolean
             },
             required: {
                 type: Boolean
             },
@@ -11043,76 +11127,76 @@
         },
         emits: ["update:modelValue"],
         setup(n, {
             emit: t
         }) {
             const e = n,
                 i = t,
-                r = L(() => e.errorMessage || e.validMessage),
-                s = L(() => e.errorMessage ? "fr-error-text" : "fr-valid-text"),
+                r = w(() => e.errorMessage || e.validMessage),
+                s = w(() => e.errorMessage ? "fr-error-text" : "fr-valid-text"),
                 o = a => {
                     a !== e.modelValue && i("update:modelValue", a)
                 };
-            return (a, l) => (m(), b("div", Qf, [g("fieldset", {
-                class: rt(["fr-fieldset", {
+            return (a, l) => (m(), v("div", tp, [g("fieldset", {
+                class: st(["fr-fieldset", {
                     "fr-fieldset--error": a.errorMessage,
                     "fr-fieldset--valid": a.validMessage
                 }]),
                 disabled: a.disabled,
                 "aria-labelledby": `${a.titleId} messages-${a.titleId}`,
                 role: a.errorMessage || a.validMessage ? "group" : void 0
-            }, [a.legend ? (m(), b("legend", {
+            }, [a.legend ? (m(), v("legend", {
                 key: 0,
                 id: a.titleId,
                 class: "fr-fieldset__legend fr-fieldset__legend--regular"
-            }, [dt(a.$slots, "legend", {}, () => [vt(C(a.legend) + " ", 1), dt(a.$slots, "required-tip", {}, () => [a.required ? (m(), b("span", np, " *")) : k("", !0)])])], 8, ep)) : k("", !0), dt(a.$slots, "default", {}, () => [(m(!0), b(un, null, Ln(a.options, (c, d) => (m(), Mt(Xf, pe({
+            }, [dt(a.$slots, "legend", {}, () => [bt(C(a.legend) + " ", 1), dt(a.$slots, "required-tip", {}, () => [a.required ? (m(), v("span", ip, " *")) : k("", !0)])])], 8, np)) : k("", !0), dt(a.$slots, "default", {}, () => [(m(!0), v(He, null, fn(a.options, (c, d) => (m(), xt(Qf, re({
                 key: c.value || d,
                 name: a.name
             }, c, {
                 small: a.small,
                 inline: a.inline,
                 "model-value": a.modelValue,
                 "onUpdate:modelValue": l[0] || (l[0] = h => o(h))
-            }), null, 16, ["name", "small", "inline", "model-value"]))), 128))]), r.value ? (m(), b("div", {
+            }), null, 16, ["name", "small", "inline", "model-value"]))), 128))]), r.value ? (m(), v("div", {
                 key: 1,
                 id: `messages-${a.titleId}`,
                 class: "fr-messages-group",
                 "aria-live": "assertive"
             }, [g("p", {
-                class: rt(["fr-message--info flex items-center", s.value])
-            }, [g("span", rp, C(r.value), 1)], 2)], 8, ip)) : k("", !0)], 10, tp)]))
+                class: st(["fr-message--info flex items-center", s.value])
+            }, [g("span", sp, C(r.value), 1)], 2)], 8, rp)) : k("", !0)], 10, ep)]))
         }
     }),
-    sp = ["id"],
     op = ["id"],
-    ap = {
+    ap = ["id"],
+    lp = {
         class: "fr-hint-text"
     },
-    lp = ["data-fr-prefix", "data-fr-suffix"],
-    cp = ["id", "min", "max", "step", "value", "disabled", "aria-labelledby", "aria-describedby"],
+    cp = ["data-fr-prefix", "data-fr-suffix"],
     up = ["id", "min", "max", "step", "value", "disabled", "aria-labelledby", "aria-describedby"],
-    dp = {
+    dp = ["id", "min", "max", "step", "value", "disabled", "aria-labelledby", "aria-describedby"],
+    hp = {
         key: 1,
         class: "fr-range__min",
         "aria-hidden": "true",
         "data-fr-js-range-limit": "true"
     },
-    hp = {
+    fp = {
         key: 2,
         class: "fr-range__max",
         "aria-hidden": "true",
         "data-fr-js-range-limit": "true"
     },
-    fp = ["id"],
     pp = ["id"],
-    $p = ht({
+    yp = ["id"],
+    Pp = ht({
         __name: "DsfrRange",
         props: {
             id: {
-                default: () => xe("range")
+                default: () => Ce("range")
             },
             min: {
                 default: 0
             },
             max: {
                 default: 100
             },
@@ -11150,106 +11234,106 @@
         },
         emits: ["update:modelValue", "update:lowerValue"],
         setup(n, {
             emit: t
         }) {
             const e = n,
                 i = t,
-                r = It(),
-                s = It(),
-                o = It(),
-                a = L(() => e.lowerValue !== void 0),
-                l = L(() => e.lowerValue === void 0 ? `transform: translateX(${(e.modelValue-e.min)/(e.max-e.min)*o.value}px) translateX(-${e.modelValue}%);` : `transform: translateX(${(e.modelValue+e.lowerValue-e.min)/2/(e.max-e.min)*o.value}px) translateX(-${e.lowerValue+(e.modelValue-e.lowerValue)/2}%);`),
-                c = L(() => {
+                r = pt(),
+                s = pt(),
+                o = pt(),
+                a = w(() => e.lowerValue !== void 0),
+                l = w(() => e.lowerValue === void 0 ? `transform: translateX(${(e.modelValue-e.min)/(e.max-e.min)*o.value}px) translateX(-${e.modelValue}%);` : `transform: translateX(${(e.modelValue+e.lowerValue-e.min)/2/(e.max-e.min)*o.value}px) translateX(-${e.lowerValue+(e.modelValue-e.lowerValue)/2}%);`),
+                c = w(() => {
                     const h = (e.modelValue - e.min) / (e.max - e.min) * o.value - (a.value ? 12 : 0),
                         y = ((e.lowerValue ?? 0) - e.min) / (e.max - e.min) * o.value;
                     return {
                         "--progress-right": h + 24 + "px",
                         ...a.value ? {
                             "--progress-left": y + 12 + "px"
                         } : {}
                     }
                 });
-            Rr([() => e.modelValue, () => e.lowerValue], ([h, y]) => {
+            Ur([() => e.modelValue, () => e.lowerValue], ([h, y]) => {
                 y !== void 0 && (a.value && h < y && i("update:lowerValue", h), a.value && y > h && i("update:modelValue", y))
             });
-            const d = L(() => (e.prefix ?? "").concat(a.value ? `${e.lowerValue} - ` : "").concat("" + e.modelValue).concat(e.suffix ?? ""));
-            return Pn(() => {
+            const d = w(() => (e.prefix ?? "").concat(a.value ? `${e.lowerValue} - ` : "").concat("" + e.modelValue).concat(e.suffix ?? ""));
+            return wn(() => {
                 var h;
                 o.value = (h = r.value) == null ? void 0 : h.offsetWidth
-            }), (h, y) => (m(), b("div", {
+            }), (h, y) => (m(), v("div", {
                 id: `${h.id}-group`,
-                class: rt(["fr-range-group", {
+                class: st(["fr-range-group", {
                     "fr-range-group--error": h.message
                 }])
             }, [g("label", {
                 id: `${h.id}-label`,
                 class: "fr-label"
-            }, [dt(h.$slots, "label", {}, () => [vt(C(h.label), 1)]), g("span", ap, [dt(h.$slots, "hint", {}, () => [vt(C(h.hint), 1)])])], 8, op), g("div", {
-                class: rt(["fr-range", {
+            }, [dt(h.$slots, "label", {}, () => [bt(C(h.label), 1)]), g("span", lp, [dt(h.$slots, "hint", {}, () => [bt(C(h.hint), 1)])])], 8, ap), g("div", {
+                class: st(["fr-range", {
                     "fr-range--sm": h.small,
                     "fr-range--double": a.value,
                     "fr-range-group--disabled": h.disabled
                 }]),
                 "data-fr-js-range": "true",
                 "data-fr-prefix": h.prefix ?? void 0,
                 "data-fr-suffix": h.suffix ?? void 0,
-                style: xn(c.value)
+                style: hn(c.value)
             }, [g("span", {
                 ref_key: "output",
                 ref: s,
                 class: "fr-range__output",
                 "data-fr-js-range-output": "true",
-                style: xn(l.value)
-            }, C(d.value), 5), a.value ? (m(), b("input", {
+                style: hn(l.value)
+            }, C(d.value), 5), a.value ? (m(), v("input", {
                 key: 0,
                 id: `${h.id}-2`,
                 type: "range",
                 min: h.min,
                 max: h.max,
                 step: h.step,
                 value: h.lowerValue,
                 disabled: h.disabled,
                 "aria-labelledby": `${h.id}-label`,
                 "aria-describedby": `${h.id}-messages`,
                 onInput: y[0] || (y[0] = _ => {
-                    var G;
-                    return i("update:lowerValue", +((G = _.target) == null ? void 0 : G.value))
+                    var V;
+                    return i("update:lowerValue", +((V = _.target) == null ? void 0 : V.value))
                 })
-            }, null, 40, cp)) : k("", !0), g("input", {
+            }, null, 40, up)) : k("", !0), g("input", {
                 id: h.id,
                 ref_key: "input",
                 ref: r,
                 type: "range",
                 min: h.min,
                 max: h.max,
                 step: h.step,
                 value: h.modelValue,
                 disabled: h.disabled,
                 "aria-labelledby": `${h.id}-label`,
                 "aria-describedby": `${h.id}-messages`,
                 onInput: y[1] || (y[1] = _ => {
-                    var G;
-                    return i("update:modelValue", +((G = _.target) == null ? void 0 : G.value))
+                    var V;
+                    return i("update:modelValue", +((V = _.target) == null ? void 0 : V.value))
                 })
-            }, null, 40, up), h.hideIndicators ? k("", !0) : (m(), b("span", dp, C(h.min), 1)), h.hideIndicators ? k("", !0) : (m(), b("span", hp, C(h.max), 1))], 14, lp), g("div", {
+            }, null, 40, dp), h.hideIndicators ? k("", !0) : (m(), v("span", hp, C(h.min), 1)), h.hideIndicators ? k("", !0) : (m(), v("span", fp, C(h.max), 1))], 14, cp), g("div", {
                 id: `${h.id}-messages`,
                 class: "fr-messages-group",
                 "aria-live": "polite"
-            }, [dt(h.$slots, "messages", {}, () => [h.message ? (m(), b("p", {
+            }, [dt(h.$slots, "messages", {}, () => [h.message ? (m(), v("p", {
                 key: 0,
                 id: `${h.id}-message-error`,
                 class: "fr-message fr-message--error"
-            }, C(h.message), 9, pp)) : k("", !0)])], 8, fp)], 10, sp))
+            }, C(h.message), 9, yp)) : k("", !0)])], 8, pp)], 10, op))
         }
     });
 
-function Pp() {
-    Pn(() => {
-        Ht.setFrameHeight()
-    }), Er(() => {
-        Ht.setFrameHeight()
+function jp() {
+    wn(() => {
+        Jt.setFrameHeight()
+    }), kr(() => {
+        Jt.setFrameHeight()
     })
 }
 export {
-    Lp as A, $p as E, kp as G, Tp as S, ul as _, Ht as a, Ep as b, Cp as c, Up as e, Np as f, Mp as h, xp as k, Pp as u, Vp as w, Rp as z
+    Oh as A, Pp as E, Up as G, Ep as H, Np as S, dl as _, Jt as a, Rp as b, kp as c, $p as e, xp as f, Mp as h, Lp as k, jp as u, Vp as w, Cp as z
 };
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/client.t80Hv_Jg.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/client.forxb5ot.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     d,
     B as s,
     O as f,
     P as m,
     S as y
-} from "./runtime-dom.esm-bundler.xzzcc6UT.js";
+} from "./runtime-dom.esm-bundler.CLhb1nSG.js";
 const S = () => {},
     A = d({
         props: {
             value: String,
             name: String,
             hydrate: {
                 type: Boolean,
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/index.O_j7wwKi.css` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/index.O_j7wwKi.css`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_default/_astro/runtime-dom.esm-bundler.xzzcc6UT.js` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_default/_astro/runtime-dom.esm-bundler.CLhb1nSG.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3988,9 +3988,9 @@
     if (typeof MathMLElement == "function" && e instanceof MathMLElement) return "mathml"
 }
 
 function yi(e) {
     return re(e) ? document.querySelector(e) : e
 }
 export {
-    tf as A, To as B, wn as C, de as D, Ge as E, cn as F, ff as G, _f as H, ge as I, uf as J, ll as K, hf as L, rf as M, pf as N, bf as O, yf as P, of as S, pi as T, ce as a, li as b, gf as c, cf as d, Vr as e, kr as f, ho as g, fn as h, ns as i, af as j, ci as k, jl as l, po as m, zo as n, ds as o, Kl as p, fi as q, ef as r, df as s, Qo as t, mf as u, nf as v, ml as w, sf as x, lf as y, Eo as z
+    tf as A, To as B, wn as C, de as D, Ge as E, cn as F, ff as G, _f as H, ge as I, uf as J, ll as K, hf as L, rf as M, pf as N, bf as O, yf as P, of as S, pi as T, ce as a, li as b, gf as c, cf as d, fn as e, ns as f, ho as g, af as h, ci as i, Vr as j, jl as k, kr as l, po as m, zo as n, ds as o, Kl as p, fi as q, ef as r, df as s, Qo as t, mf as u, nf as v, ml as w, sf as x, lf as y, Eo as z
 };
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_file_upload/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_file_upload/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z23fFeF" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrFileUpload.IdR5fkhs.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrFileUpload&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z23fFeF" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrFileUpload.Qd737a0v.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrFileUpload&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_footer/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_alert/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1cGN6D" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrFooter.so92d35v.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrFooter&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1pKcPR" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrAlert.qHAssOJm.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrAlert&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_input/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_picture/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,4 +1,4 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-.component[data-v-17d449db]{margin:4px}.component[data-v-17d449db] textarea.fr-input{min-height:5.75rem;resize:none}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Zeq8RV" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrInput.PfsGa47n.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrInput&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+.component[data-v-dcb3aa53] .fr-content-media{margin-top:0;margin-bottom:0}
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="1b8oUq" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrPicture.vdniiHOI.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrPicture&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_picture/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_footer/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,4 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-.component[data-v-dcb3aa53] .fr-content-media{margin-top:0;margin-bottom:0}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="1b8oUq" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrPicture.BG7gzqcn.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrPicture&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Z1cGN6D" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrFooter.vqQJXfur.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrFooter&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_radio/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_radio/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,4 +1,4 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
 .component[data-v-61d47d67] .fr-fieldset{margin-bottom:-.5rem}.component[data-v-61d47d67] .fr-fieldset__legend{padding-bottom:.5rem}.component[data-v-61d47d67] .fr-fieldset__element{margin-bottom:.5rem}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="8Sdnq" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrRadioButtonSet.j3YqEKSL.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrRadioButtonSet&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="8Sdnq" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrRadioButtonSet.I8DloxHK.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrRadioButtonSet&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/frontend/st_dsfr_range/index.html` & `streamlit-dsfr-0.0.9/streamlit_dsfr/frontend/st_dsfr_button/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,4 +1,3 @@
 <!DOCTYPE html><html data-astro-cid-5hce7sga> <head><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="/component/streamlit_dsfr.dsfr_default/_astro/index.O_j7wwKi.css" />
 <style>.err__title[data-v-ad0b980e],.err__msg[data-v-ad0b980e]{margin:0}.component-wrapper[data-v-ba378196]{display:flex;flex-direction:column}
-.component[data-v-81302ce6] .fr-range[data-fr-js-range]:after{clip-path:polygon(var(--progress-left) 0,calc(var(--progress-right) - 24px) 0,calc(var(--progress-right) - 24px) 100%,var(--progress-left) 100%)}
-</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="Zv6ztk" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrRange.WiM63mXm.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.t80Hv_Jg.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrRange&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
+</style></head> <body data-astro-cid-5hce7sga>   <style>astro-island,astro-slot,astro-static-slot{display:contents}</style><script>(()=>{var e=async t=>{await(await t())()};(self.Astro||(self.Astro={})).load=e;window.dispatchEvent(new Event("astro:load"));})();;(()=>{var b=Object.defineProperty;var f=(c,o,i)=>o in c?b(c,o,{enumerable:!0,configurable:!0,writable:!0,value:i}):c[o]=i;var l=(c,o,i)=>(f(c,typeof o!="symbol"?o+"":o,i),i);var p;{let c={0:t=>m(t),1:t=>i(t),2:t=>new RegExp(t),3:t=>new Date(t),4:t=>new Map(i(t)),5:t=>new Set(i(t)),6:t=>BigInt(t),7:t=>new URL(t),8:t=>new Uint8Array(t),9:t=>new Uint16Array(t),10:t=>new Uint32Array(t)},o=t=>{let[e,r]=t;return e in c?c[e](r):void 0},i=t=>t.map(o),m=t=>typeof t!="object"||t===null?t:Object.fromEntries(Object.entries(t).map(([e,r])=>[e,o(r)]));customElements.get("astro-island")||customElements.define("astro-island",(p=class extends HTMLElement{constructor(){super(...arguments);l(this,"Component");l(this,"hydrator");l(this,"hydrate",async()=>{var d;if(!this.hydrator||!this.isConnected)return;let e=(d=this.parentElement)==null?void 0:d.closest("astro-island[ssr]");if(e){e.addEventListener("astro:hydrate",this.hydrate,{once:!0});return}let r=this.querySelectorAll("astro-slot"),a={},h=this.querySelectorAll("template[data-astro-template]");for(let n of h){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("data-astro-template")||"default"]=n.innerHTML,n.remove())}for(let n of r){let s=n.closest(this.tagName);s!=null&&s.isSameNode(this)&&(a[n.getAttribute("name")||"default"]=n.innerHTML)}let u;try{u=this.hasAttribute("props")?m(JSON.parse(this.getAttribute("props"))):{}}catch(n){let s=this.getAttribute("component-url")||"<unknown>",y=this.getAttribute("component-export");throw y&&(s+=` (export ${y})`),console.error(`[hydrate] Error parsing props for component ${s}`,this.getAttribute("props"),n),n}await this.hydrator(this)(this.Component,u,a,{client:this.getAttribute("client")}),this.removeAttribute("ssr"),this.dispatchEvent(new CustomEvent("astro:hydrate"))});l(this,"unmount",()=>{this.isConnected||this.dispatchEvent(new CustomEvent("astro:unmount"))})}disconnectedCallback(){document.removeEventListener("astro:after-swap",this.unmount),document.addEventListener("astro:after-swap",this.unmount,{once:!0})}connectedCallback(){if(!this.hasAttribute("await-children")||document.readyState==="interactive"||document.readyState==="complete")this.childrenConnectedCallback();else{let e=()=>{document.removeEventListener("DOMContentLoaded",e),r.disconnect(),this.childrenConnectedCallback()},r=new MutationObserver(()=>{var a;((a=this.lastChild)==null?void 0:a.nodeType)===Node.COMMENT_NODE&&this.lastChild.nodeValue==="astro:end"&&(this.lastChild.remove(),e())});r.observe(this,{childList:!0}),document.addEventListener("DOMContentLoaded",e)}}async childrenConnectedCallback(){let e=this.getAttribute("before-hydration-url");e&&await import(e),this.start()}start(){let e=JSON.parse(this.getAttribute("opts")),r=this.getAttribute("client");if(Astro[r]===void 0){window.addEventListener(`astro:${r}`,()=>this.start(),{once:!0});return}Astro[r](async()=>{let a=this.getAttribute("renderer-url"),[h,{default:u}]=await Promise.all([import(this.getAttribute("component-url")),a?import(a):()=>()=>{}]),d=this.getAttribute("component-export")||"default";if(!d.includes("."))this.Component=h[d];else{this.Component=h;for(let n of d.split("."))this.Component=this.Component[n]}return this.hydrator=u,this.hydrate},e,this)}attributeChangedCallback(){this.hydrate()}},l(p,"observedAttributes",["props"]),p))}})();</script><astro-island uid="ZI3AMx" component-url="/component/streamlit_dsfr.dsfr_default/_astro/DsfrButton.F0Lzs9zA.js" component-export="default" renderer-url="/component/streamlit_dsfr.dsfr_default/_astro/client.forxb5ot.js" props="{}" ssr="" client="load" opts="{&quot;name&quot;:&quot;DsfrButton&quot;,&quot;value&quot;:true}" await-children=""><div client:load data-v-ba378196 data-v-ad0b980e><!----></div><!--astro:end--></astro-island>   </body></html>
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr/override_font_family.py` & `streamlit-dsfr-0.0.9/streamlit_dsfr/override_font_family.py`

 * *Files identical despite different names*

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/PKG-INFO` & `streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-dsfr
-Version: 0.0.8
+Version: 0.0.9
 Summary: VueDsfr components for Streamlit
 Author-email: Matiboux <matiboux@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
```

### Comparing `streamlit-dsfr-0.0.8/streamlit_dsfr.egg-info/SOURCES.txt` & `streamlit-dsfr-0.0.9/streamlit_dsfr.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 streamlit_dsfr.egg-info/dependency_links.txt
 streamlit_dsfr.egg-info/requires.txt
 streamlit_dsfr.egg-info/top_level.txt
 streamlit_dsfr/frontend/st_dsfr_alert/index.html
 streamlit_dsfr/frontend/st_dsfr_badge/index.html
 streamlit_dsfr/frontend/st_dsfr_breadcrumb/index.html
 streamlit_dsfr/frontend/st_dsfr_button/index.html
+streamlit_dsfr/frontend/st_dsfr_buttons_group/index.html
 streamlit_dsfr/frontend/st_dsfr_checkbox/index.html
 streamlit_dsfr/frontend/st_dsfr_default/index.html
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrAlert.tFZy4mCO.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBadge.gLg-CXXd.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBreadcrumb.79FUC984.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButton.5AkE1u2l.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrCheckbox.TNj2wexB.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFileUpload.IdR5fkhs.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFooter.so92d35v.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrInput.PfsGa47n.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrPicture.BG7gzqcn.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRadioButtonSet.j3YqEKSL.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRange.WiM63mXm.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrAlert.qHAssOJm.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBadge.U7kOfHPN.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrBreadcrumb.24AdnYLs.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButton.F0Lzs9zA.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrButtonGroup.MtpDLhtp.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrCheckbox.HBUYPhr5.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFileUpload.Qd737a0v.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrFooter.vqQJXfur.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrInput.DWr3u8eg.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrPicture.vdniiHOI.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRadioButtonSet.I8DloxHK.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/DsfrRange.uSCKVJAW.js
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.Lusn3uPo.woff
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold.mI04Wx9M.woff2
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.VpzzqYz6.woff
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Bold_Italic.alvVdTYc.woff2
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.6lmsSnc8.woff
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light.7GX88oPX.woff2
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Light_Italic.GJ3thv45.woff2
@@ -42,21 +44,21 @@
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular.mgqq5yTO.woff2
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.3R_BbTaN.woff2
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Marianne-Regular_Italic.UCbE0jax.woff
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.FN9ubN3N.woff
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-ExtraBold.gs3wZvgE.woff2
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.9CKHJdJx.woff
 streamlit_dsfr/frontend/st_dsfr_default/_astro/Spectral-Regular.D5gUInLE.woff2
-streamlit_dsfr/frontend/st_dsfr_default/_astro/StreamlitVue.ZFQEvSxb.js
-streamlit_dsfr/frontend/st_dsfr_default/_astro/client.t80Hv_Jg.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/StreamlitVue.CglRiHNi.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/client.forxb5ot.js
 streamlit_dsfr/frontend/st_dsfr_default/_astro/index.O_j7wwKi.css
-streamlit_dsfr/frontend/st_dsfr_default/_astro/runtime-dom.esm-bundler.xzzcc6UT.js
+streamlit_dsfr/frontend/st_dsfr_default/_astro/runtime-dom.esm-bundler.CLhb1nSG.js
 streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_alert.x0NNfw9T.css
 streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_checkbox._xlQgrDX.css
-streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_input.S6zC6ajS.css
+streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_input.sx26c0dS.css
 streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_picture.wTCAjD5j.css
 streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_radio.owPTSQFN.css
 streamlit_dsfr/frontend/st_dsfr_default/_astro/st_dsfr_range.OgT-Uti3.css
 streamlit_dsfr/frontend/st_dsfr_file_upload/index.html
 streamlit_dsfr/frontend/st_dsfr_footer/index.html
 streamlit_dsfr/frontend/st_dsfr_input/index.html
 streamlit_dsfr/frontend/st_dsfr_picture/index.html
```

