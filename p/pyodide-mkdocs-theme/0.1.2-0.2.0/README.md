# Comparing `tmp/pyodide_mkdocs_theme-0.1.2.tar.gz` & `tmp/pyodide_mkdocs_theme-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.1.2.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.2.0.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.1.2.tar` & `pyodide_mkdocs_theme-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.1.2/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-07 16:13:56.353971 pyodide_mkdocs_theme-0.1.2/README.md
--rw-r--r--   0        0        0     1347 2024-04-08 19:00:54.546808 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     6071 2024-04-07 19:41:30.518314 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-08 19:00:54.578809 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4832 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4935 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21947 2024-04-08 18:55:57.181446 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4062 2024-04-06 19:50:40.682880 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11234 2024-04-07 10:49:12.948368 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0     6948 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4013 2024-04-08 18:53:29.656488 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0     7303 2024-04-08 14:28:15.731641 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11890 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    12230 2024-04-08 14:28:15.731641 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     2899 2024-04-04 17:32:31.188228 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     8427 2024-04-04 20:46:58.718283 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2653 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-08 19:00:54.502807 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6553 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     7206 2024-04-07 06:55:38.270867 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9589 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3530 2024-04-06 11:30:24.316895 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6051 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16436 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      137 2024-03-05 13:24:26.138158 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/README.md
--rw-r--r--   0        0        0     3986 2024-04-07 12:16:07.564974 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js
--rw-r--r--   0        0        0     7119 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-07 10:49:36.669062 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js
--rw-r--r--   0        0        0     4297 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js
--rw-r--r--   0        0        0     3626 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css
--rw-r--r--   0        0        0     1490 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3582 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css
--rw-r--r--   0        0        0    31978 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css
--rw-r--r--   0        0        0     1527 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4233 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-07 09:15:49.456003 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css
--rw-r--r--   0        0        0    12598 2024-04-07 10:53:56.264647 pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1689 2024-04-08 19:00:50.978699 pyodide_mkdocs_theme-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.0/README.md
+-rw-r--r--   0        0        0     1347 2024-04-09 19:35:24.738160 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     6071 2024-04-08 19:01:06.315166 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-09 19:35:24.766160 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4832 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4969 2024-04-09 18:36:57.659855 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    22072 2024-04-09 18:36:08.002399 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4062 2024-04-06 19:50:40.682880 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11234 2024-04-07 10:49:12.948368 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0     6948 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4013 2024-04-08 19:01:06.315166 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0     8457 2024-04-09 18:42:09.792988 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11890 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    12321 2024-04-09 18:44:53.161770 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     2899 2024-04-04 17:32:31.188228 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     8427 2024-04-04 20:46:58.718283 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2653 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-09 19:35:24.690158 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6553 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     3986 2024-04-07 12:16:07.564974 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7119 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-07 10:49:36.669062 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4297 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3626 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-extrahead.css
+-rw-r--r--   0        0        0     7138 2024-04-09 19:08:03.522506 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9689 2024-04-09 19:25:01.928095 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3530 2024-04-06 11:30:24.316895 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6051 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16604 2024-04-09 18:52:21.314960 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3582 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css
+-rw-r--r--   0        0        0    31978 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css
+-rw-r--r--   0        0        0     1527 2024-04-04 09:56:58.202965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4233 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-07 09:15:49.456003 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css
+-rw-r--r--   0        0        0    12598 2024-04-07 10:53:56.264647 pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1689 2024-04-09 19:35:22.082082 pyodide_mkdocs_theme-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.0/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.1.2/LICENSE` & `pyodide_mkdocs_theme-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/README.md` & `pyodide_mkdocs_theme-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 def _IDE_maker(env:MaestroIDE, mode:str):
     """
     @script_name: Partial path from the directory holding the sujet.md file, to the one holding
                   all the other required files, ending with the common prefix for the exercice.
                   Ex:   "exo" to extract:   "exo.py", "exo_corr.py", "exo_test.py", ...
                       "sub_exA/exo" for:  "sub_exA/exo.py", "sub_exA/exo_corr.py", ...
-    @MAX:         Number of tries before the solution becomes visible (default=5).
+    @MAX:         Number of tries before the solution becomes visible (default: validations config)
     @SANS:        String of spaces or coma separated python functions or modules/packages the
                   user cannot use. By default, nothing is forbidden.
                       - Every string section that matches a builtin callable forbid that function
                         by replacing it with another function which will raise an error if called
                       - Every string section prefixed with a fot forbids a method call. Here a
                         simple string containment check is done opn the user's code, to check it
                         does not contain the desired method name with the dot before it.
@@ -52,24 +52,24 @@
                         import (in any way/syntax) involving that name will raise an error.
     @SIZE:        Max number of lines of the IDE (default=30).
     @ID:          Optional. To use to differentiate two IDEs using the same python root file.
     @WHITE:       String of spaces or coma separated python modules/packages that have to be
                   preloaded before the code restrictions (@SANS) are applied.
     @LOGS:        If True, failing assertions without feedback during the private tests will
                   be augmented automatically with the code of the assertion itself. If None,
-                  use the global `show_code_on_failed_assertions` plugin value, defined in
+                  use the global `show_assertion_code_on_failed_test` plugin value, defined in
                   `mkdocs.yml`, to determine what to do (default=None).
     @REC_LIMIT:   Setup a specific recursion limit value for the runtime (-1 if not used)
     @TERM_H:      Number of lines to use for the terminal size (ignored for vertical terminals)
     """
 
     @wraps(_IDE_maker)
     def wrapped(
         script_name: str = "",
-        MAX: Union[int, Literal["+"]] = 5,
+        MAX: Optional[Union[int, Literal["+"]]] = None,
         SANS: str = "",
         SIZE: int = 30,
         ID: int = None,
         WHITE: str = "",
         LOGS: Optional[bool] = None,
         REC_LIMIT: int = -1,
         TERM_H: int = 10,
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
-"""
-Macros to insert IDE (aka. editor + terminal + buttons)
-"""
 # pylint: disable=unused-argument
 
 
 import re
 import hashlib
 from typing import Any, ClassVar, Dict, List, Literal, Optional, Tuple, Union
 from dataclasses import dataclass
@@ -71,16 +68,18 @@
     """
 
     mode: Union[Literal[""],Literal["_v"]]
     """ The terminal will be below (mode="") or on the right (mode="_v") of the editor.
         (what an awful interface, yeah... x) )
     """
 
-    max_attempts: Union[int, Literal["+"]]
-    """ Maximum number of attempts before the solution admonition will become available """
+    max_attempts: Optional[Union[int, Literal["+"]]]
+    """ Maximum number of attempts before the solution admonition will become available.
+        If None, use the global default value.
+    """
 
     excluded: str
     """ String of spaces or coma separated python functions or modules/packages that are forbidden
         at runtime. By default, nothing is forbidden.
             - Every string section that matches a builtin callable forbid that function by
               replacing it with another function which will raise an error if called.
             - Every string section prefixed with a fot forbids a method call. Here a simple
@@ -107,15 +106,15 @@
     """ Used to disambiguate the ids of two IDEs, if the same file is used several times
         in the document.
     """
 
     auto_log_assert: Optional[bool]
     """ If True, failing assertions without feedback during the private tests will be
         augmented automatically with the code of the assertion itself. If None, use
-        the global `show_code_on_failed_assertions` plugin value and defined in
+        the global `show_assertion_code_on_failed_test` plugin value and defined in
         `CONFIG.showFailedAssertionsOnValidation` in the JS runtime.
     """
 
     rec_limit: int
     """ If used, the recursion limit of the pyodide runtime will be updated before the user's
         code or the tests are run.
         Note that this also forbids the use of the `sys.setrecurionlimit` at runtime.
@@ -174,14 +173,17 @@
     )
 
 
 
 
     def __post_init__(self):
 
+        if self.max_attempts is None:
+            self.max_attempts = self.my_env.max_attempts_before_corr_available
+
         self.files_data = IdeFilesExtractor(self.my_env, self.script_name, self.id)
 
         if 0 <= self.rec_limit < self.my_env.MIN_RECURSION_LIMIT:
             with_id = f' (ID={ self.id })' if self.id is not None else ''
             raise BuildError(
                 f"The recursion limit for {self.my_env.page.file.src_uri}:{self.script_name}"
                 f"{with_id} is set too low and may causes runtime troubles. Please set it to "
@@ -451,15 +453,15 @@
         if self.has_corr:
             # first indentation must be removed, EXCEPT one level, because handled lower
             # for the whole block
             one_level = '    '
             fence = build_code_fence(
                 corr_content,
                 one_level + self.indentation,
-                title="Proposition de correction"
+                title="🐍 Proposition de correction"
             )
             md_div.append(  one_level+fence.strip())
 
         if self.has_corr and self.has_rem:
             md_div.append( f'    <span class="{ HtmlClass.rem_fake_h3 }">Remarques :</span>')
 
         if self.has_rem:
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 EXTRAS_MACROS_PROPS = (
     "" if not _NEW_MACROS_PLUGIN_PROPS else "\nNew config in MacrosPlugin:" + ''.join(
         f'\n\t{name}' for name in _NEW_MACROS_PLUGIN_PROPS
     )
 )
 
 
-J2_STRING                   = _SRC_MACROS_CONF['include_dir'].default
-DEFAULT_MODULE_NAME         = _SRC_MACROS_CONF['module_name'].default
-DEFAULT_UNDEFINED_BEHAVIOR  = _SRC_MACROS_CONF['on_undefined'].default
+J2_STRING                  = _SRC_MACROS_CONF['include_dir'].default
+DEFAULT_MODULE_NAME        = _SRC_MACROS_CONF['module_name'].default
+DEFAULT_UNDEFINED_BEHAVIOR = _SRC_MACROS_CONF['on_undefined'].default
 
 
 
 
 
 
 
@@ -79,33 +79,60 @@
 
     scripts_url = typ_deprecated_with_custom_msg('scripts_url', str)
     site_root   = typ_deprecated_with_custom_msg('site_root', str)
 
 
 
 
+class ValidationConfig(Config):
+    """ All options related to validation tests (IDEs) """
+
+    show_assertion_code_on_failed_test = C.Type(bool, default=True)
+    """
+    When an assertion fails in the secret tests and that assertion doesn't have any assertion
+    message, the code of the assertion itself will be displayed in the terminal if this option
+    is set to True (default).
+    This behavior is global, but can be overridden on a "per IDE" base, using the `auto_log_assert`
+    optional argument.
+    """
+
+    max_attempts_before_corr_available = C.Type(int, default=5)
+    """
+    Global setting for all IDE in the documentation: max number of tries a user can do before
+    correction and remarks become available (reminder: they are in a retracted details/admonition,
+    so the user still has to click to so the content. This way, they can still try to get the code
+    right before actually giving up).
+    """
+
+    decrease_attempts_on_user_code_failure = C.Type(bool, default=True)
+    """ If true, any failure when running the user code will decrease the number of attempts left.
+        Note this means even syntax errors will decrease the count, when the validation button is
+        used.
+        When this option is set to True, the user will have to comment out the public tests to get
+        the number of attempts changing, which is not obvious for new users).
+    """
+
+
+
+
 # Only defines the values exposed to the user in mkdocs.yml.
 # When a property is declared here, don't forgot to add the related extractor on the
 # BaseMaestro class.
 class PyodideMacrosConfig(Config):
     """
     Configuration for the main pyodide-mkdocs-theme plugin.
     """
 
-    others = C.SubConfig(OtherConfig)
+    _others = C.SubConfig(OtherConfig)
+    """ Old configuration options (unmaintained, so far) """
 
 
-    show_code_on_failed_assertions = C.Type(bool, default=True)
-    """
-    When an assertion fails in the secret tests and that assertion doesn't have any assertion
-    message, the code of the assertion itself will be displayed in the terminal if this option
-    is set to True (default).
-    This behavior is global, but can be overridden on a "per IDE" base, using the `auto_log_assert`
-    optional argument.
-    """
+    validations = C.SubConfig(ValidationConfig)
+    """ Configuration related to the validation tests in IDEs """
+
 
     skip_py_md_paths_names_validation = C.Type(bool, default=False)
     """
     By default, the path names of all the `.py` and `.md` files present in the docs_dir are checked
     so that they do not contain any character other than letters, digits, dot or dash. This
     ensure the IDE related macros will properly work.
     If unwanted characters are found, a BuildError is raised. Setting this flag to True will bypass
@@ -136,23 +163,14 @@
     """
     Encoding to use when loading yaml data from the original MacrosPlugin.
     (The original method doesn't use any encoding argument, which can lead to different behaviors
     between Windows and Linux (typically: during a pipeline!).
     """
 
 
-    encrypt_corrections_and_rems = C.Type(bool, default=True)
-    """
-    Define if the html tags containing the correction and remarks have to be encrypted or not when
-    building the website. Passing this to False can be useful during development, but value should
-    _ALWAYS_ be set to true on the deployed website: keep in mind the search engine can otherwise
-    dig out content of those while the user is searching for something else.
-    """
-
-
     macros_with_indents = C.Type(str, default='')
     """
     Allow to register external macros that will use the `PyodideMacrosPlugin.get_indent` logistic
     to insert indented multiline contents in the page.
     `macro_with_indents` is a space separated string of all the names of the macros to register.
     """
 
@@ -169,14 +187,23 @@
     """
     If True, no error will be raised when checking the configuration of the macros plugin against
     the one of pyodide-macros. Note that if this error is raised, the build probably won't succeed
     or the output will probably be buggy.
     """
 
 
+    encrypt_corrections_and_rems = C.Type(bool, default=True)
+    """
+    Define if the html tags containing the correction and remarks have to be encrypted or not when
+    building the website. Passing this to False can be useful during development, but value should
+    _ALWAYS_ be set to true on the deployed website: keep in mind the search engine can otherwise
+    dig out content of those while the user is searching for something else.
+    """
+
+
     _dev_mode = C.Type(bool, default=False)
     """ Run the plugin in development mode (don't use that...) """
 
 
     # ---------------------------------------------------------------------------------------
     # Replication of MacrosPlugin options (merging the config_scheme properties programmatically
     # is not enough, unfortunately...)
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,164 @@
 
 
 
 
 
 
 
+
+class BaseMaestro( BasePlugin[PyodideMacrosConfig] ):
+    """
+    Main class, regrouping the basic configurations, properties, getters and/or constants
+    for the different children classes: each of them will inherit from MaestroConfig.
+    It is also used as "sink" for the super calls of other classes that are not implemented
+    on the MacrosPlugin class.
+
+    Note that, for the ConfigExtractor for to properly work, the class hierarchy has to
+    extend MacrosPlugin at some point.
+    """
+
+    load_yaml_encoding: str = ConfigExtractor()
+    macros_with_indents: str = ConfigExtractor()
+    ignore_macros_plugin_diffs: bool = ConfigExtractor()
+
+    skip_py_md_paths_names_validation: bool = ConfigExtractor()
+    check_python_files: bool   = ConfigExtractor()
+    soft_check: bool = ConfigExtractor()
+
+    encrypt_corrections_and_rems: bool = ConfigExtractor()
+    bypass_indent_errors: bool = ConfigExtractor()
+    _dev_mode: bool = ConfigExtractor()
+
+    show_assertion_code_on_failed_test: bool = ConfigExtractor("validations")
+    max_attempts_before_corr_available: bool = ConfigExtractor("validations")
+    decrease_attempts_on_user_code_failure: bool = ConfigExtractor("validations")
+
+    scripts_url: str = ConfigExtractor("_others")
+    site_root: str = ConfigExtractor("_others")
+
+    page: Page  # just as a reminder: defined by MacrosPlugin
+
+    # global mkdocs config data:
+    site_url: str = ConfigExtractor(root='_conf')
+    docs_dir: str = ConfigExtractor(root='_conf')
+    repo_url: str = ConfigExtractor(root='_conf')
+
+    #----------------------------------------------------------------------------
+    # WARNING: the following properties are assigned from the PyodideMacrosPlugin
+
+    docs_dir_path: Path
+    """ Current docs_dir of the project as a Path object (ABSOLUTE path) """
+
+    docs_dir_cwd_rel: Path
+    """ docs_dir Path object, but relative to the CWD, at runtime """
+
+    _macro_with_indent_pattern:re.Pattern = None
+    """
+    Pattern to re.match macro calls that will need to handle indentation levels.
+    Built at runtime (depends on `macro_with_indents`)
+    """
+
+    #----------------------------------------------------------------------------
+
+    version:str = __version__
+
+    pmt_url:str = 'https://gitlab.com/frederic-zinelli/pyodide-mkdocs-theme'
+
+
+    _pages_indents: 'PageIndents'
+    """
+    Cache storing the indentations for each jinja/macro template in a Page.
+    A page is entirely studied the first time it's seen and the result of the indentation levels
+    are stored.
+    The data stays correct throughout the md->html conversion because the indentation levels
+    "horizontal") are not affected by the content growing ("vertical").
+    """
+
+    _running_macro: Optional[str] = None
+    """
+    Name of the macro currently running (or the last one called. None if no macro called yet).
+    """
+
+
+
+    def on_config(self, config:MkDocsConfig):
+        # pylint: disable=unused-argument, no-member, missing-function-docstring
+        self._pages_indents = PageIndents()
+
+        super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
+
+
+    #----------------------------------------------------------------------------
+
+
+    def get_indent_in_current_page(self, macro_predicate:re.Pattern):
+        """
+        Extract the indentation needed for the given macro template call.
+        @throws:    BuildError if the same macro call is found several times in the page.
+        """
+        return self._pages_indents.get_indent(self, macro_predicate)
+
+
+    def is_macro_with_indent(self, macro_call:str) -> bool:
+        """
+        Return True if the given macro call requires to register indentation data.
+        This is using a white list, so that user defined macro cannot cause troubles.
+        """
+        return bool(self._macro_with_indent_pattern.match(macro_call))
+
+
+    def level_up_from_current_page(self, url:str=None) -> str:
+        """
+        Return the appropriate number of ".." steps needed to build a relative url to go from the
+        current page url back to the root directory.
+
+        Note there are no trailing backslash.
+
+        @url: relative to the docs_dir (ex: "exercices/ ..."). If None, use self.page.url instead.
+        """
+        url = self.page.url if url is None else url
+        page_loc:Path = self.docs_dir_path / url
+        segments = page_loc.relative_to(self.docs_dir_path).parts
+        out = len(segments) * ['..']
+        return '/'.join(out) or '.'
+
+
+    #----------------------------------------------------------------------------
+
+
+    def _omg_they_killed_keanu(self,page_name:str, page_on_context:Page=None):
+        """ Debugging purpose only. Use as breakpoint utility.
+            @page_on_context argument used when called "outside" of the macro logic (fro example,
+            in external hooks)
+        """
+        page = page_on_context or self.page
+        if page_name == page.url:
+            logger.error("Breakpoint! (the CALL to this method should be removed)")
+
+
+    def warn_unmaintained(self, that:str):
+        """
+        Generic warning message for people trying to used untested/unmaintained macros.
+        """
+        logger.warning(
+            f"{ that.capitalize() } has not been maintained since the original pyodide-mkdocs "
+            "project and may not currently work.\n"
+            "Please open an issue on the pyodide-mkdocs-theme repository, providing a concrete "
+            "use case so that it can be updated.\n\n"
+            f"\t{ self.pmt_url }"
+        )
+
+
+
+
+
+
+
+
 class PageIndents( Dict[PageUrl, Dict[str,str]] ):
     """ Cache storing the indentations for each jinja/macro template in all Pages.
         a page is entirely studied the first time it's seen and the result of the indentation
         levels are stored.
         The data stays correct throughout the md->html conversion because the indentation
         levels "horizontal") are not affected by the content growing ("vertical").
     """
@@ -172,153 +322,7 @@
                     "page!\nIf this is coming from one of your own macro, you will need to add "
                     "the related logic and argument in your code."
                 )
             raise BuildError( err_msg + epilogue )
 
 
 
-
-
-
-
-
-MACROS_PLUGIN_VARS_ROOT = 'variables'
-PMT_MACROS_ROOT = "config"
-
-
-class BaseMaestro( BasePlugin[PyodideMacrosConfig] ):
-    """
-    Main class, regrouping the basic configurations, properties, getters and/or constants
-    for the different children classes: each of them will inherit from MaestroConfig.
-    It is also used as "sink" for the super calls of other classes that are not implemented
-    on the MacrosPlugin class.
-
-    Note that, for the ConfigExtractor for to properly work, the class hierarchy has to
-    extend MacrosPlugin at some point.
-    """
-
-
-    show_code_on_failed_assertions: bool = ConfigExtractor()
-    skip_py_md_paths_names_validation: bool = ConfigExtractor()
-    check_python_files: bool  = ConfigExtractor()
-    soft_check: bool          = ConfigExtractor()
-    load_yaml_encoding: str   = ConfigExtractor()
-    _dev_mode: bool           = ConfigExtractor()
-    encrypt_corrections_and_rems: bool = ConfigExtractor()
-    macros_with_indents: str  = ConfigExtractor()
-    bypass_indent_errors: bool = ConfigExtractor()
-    ignore_macros_plugin_diffs: bool = ConfigExtractor()
-
-    scripts_url: str    = ConfigExtractor("others")
-    site_root: str      = ConfigExtractor("others")
-
-    page: Page  # just as a reminder: defined by MacrosPlugin
-
-    # global mkdocs config data:
-    site_url: str = ConfigExtractor(root='_conf')
-    docs_dir: str = ConfigExtractor(root='_conf')
-    repo_url: str = ConfigExtractor(root='_conf')
-
-    #----------------------------------------------------------------------------
-    # WARNING: the following properties are assigned from the PyodideMacrosPlugin
-
-    docs_dir_path: Path
-    """ Current docs_dir of the project as a Path object (ABSOLUTE path) """
-
-    docs_dir_cwd_rel: Path
-    """ docs_dir Path object, but relative to the CWD, at runtime """
-
-    _macro_with_indent_pattern:re.Pattern = None
-    """
-    Pattern to re.match macro calls that will need to handle indentation levels.
-    Built at runtime (depends on `macro_with_indents`)
-    """
-
-    #----------------------------------------------------------------------------
-
-    version:str = __version__
-
-    pmt_url:str = 'https://gitlab.com/frederic-zinelli/pyodide-mkdocs-theme'
-
-
-    _pages_indents: PageIndents
-    """
-    Cache storing the indentations for each jinja/macro template in a Page.
-    A page is entirely studied the first time it's seen and the result of the indentation levels
-    are stored.
-    The data stays correct throughout the md->html conversion because the indentation levels
-    "horizontal") are not affected by the content growing ("vertical").
-    """
-
-    _running_macro: Optional[str] = None
-    """
-    Name of the macro currently running (or the last one called. None if no macro called yet).
-    """
-
-
-
-    def on_config(self, config:MkDocsConfig):
-        # pylint: disable=unused-argument, no-member, missing-function-docstring
-        self._pages_indents = PageIndents()
-
-        super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
-
-
-    #----------------------------------------------------------------------------
-
-
-    def get_indent_in_current_page(self, macro_predicate:re.Pattern):
-        """
-        Extract the indentation needed for the given macro template call.
-        @throws:    BuildError if the same macro call is found several times in the page.
-        """
-        return self._pages_indents.get_indent(self, macro_predicate)
-
-
-    def is_macro_with_indent(self, macro_call:str) -> bool:
-        """
-        Return True if the given macro call requires to register indentation data.
-        This is using a white list, so that user defined macro cannot cause troubles.
-        """
-        return bool(self._macro_with_indent_pattern.match(macro_call))
-
-
-    def level_up_from_current_page(self, url:str=None) -> str:
-        """
-        Return the appropriate number of ".." steps needed to build a relative url to go from the
-        current page url back to the root directory.
-
-        Note there are no trailing backslash.
-
-        @url: relative to the docs_dir (ex: "exercices/ ..."). If None, use self.page.url instead.
-        """
-        url = self.page.url if url is None else url
-        page_loc:Path = self.docs_dir_path / url
-        segments = page_loc.relative_to(self.docs_dir_path).parts
-        out = len(segments) * ['..']
-        return '/'.join(out) or '.'
-
-
-    #----------------------------------------------------------------------------
-
-
-    def _omg_they_killed_keanu(self,page_name:str, page_on_context:Page=None):
-        """ Debugging purpose only. Use as breakpoint utility.
-            @page_on_context argument used when called "outside" of the macro logic (fro example,
-            in external hooks)
-        """
-        page = page_on_context or self.page
-        if page_name == page.url:
-            logger.error("Breakpoint! (the CALL to this method should be removed)")
-
-
-    def warn_unmaintained(self, that:str):
-        """
-        Generic warning message for people trying to used untested/unmaintained macros.
-        """
-        logger.warning(
-            f"{ that.capitalize() } has not been maintained since the original pyodide-mkdocs "
-            "project and may not currently work.\n"
-            "Please open an issue on the pyodide-mkdocs-theme repository, providing a concrete "
-            "use case so that it can be updated.\n\n"
-            f"\t{ self.pmt_url }"
-        )
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/main.html`

 * *Files 10% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 <script src="https://cdn.jsdelivr.net/npm/lodash@4.17.20/lodash.min.js" type="text/javascript"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ace.min.js" charset="utf-8" type="text/javascript" integrity="sha512-GQpIYSKNIPIC763JKTNALj+t18/nfLdzw5gITgFGa31aK/4NmjyPKsfqrjh7CuzpJaG3nqEleeVcWUhHad9Axg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ext-language_tools.min.js" charset="utf-8" type="text/javascript" integrity="sha512-iK7yTkCkv7MbFwTqRgHTbmIqoiiLq6BsyNjymnFyB5a7pEQwYThj9QIgqBy9+XPPwj7+hAEHyR2npOHL1bz4Qg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdn.jsdelivr.net/pyodide/v0.25.0/full/pyodide.js"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery.terminal@2.34.0/js/jquery.terminal.min.js"></script>
 <!-- PYODIDE - insertion token -->
-<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js"></script>
-<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js"></script>
-<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js"></script>
-<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/mathjax-libs.js"></script>
-<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js"></script>
-<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js"></script>
+<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/0_config-libs.js"></script>
+<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/functools-libs.js"></script>
+<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/jsLogger-libs.js"></script>
+<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/mathjax-libs.js"></script>
+<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/securedPagesData-libs.js"></script>
+<script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_globalGuiButtons-libs.js"></script>
 <!-- PYODIDE - insertion token -->
 <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js" type="text/javascript" charset="utf-8"></script>
 <script type="application/javascript">
   CONFIG.CURRENT_REVISION = "pyodide-mkdocs-theme v{{ config.plugins.pyodide_macros.version }}"
-  CONFIG.showFailedAssertionsOnValidation = {{ config.plugins.pyodide_macros.show_code_on_failed_assertions | tojson }}
+  CONFIG.showFailedAssertionsOnValidation = {{ config.plugins.pyodide_macros.show_assertion_code_on_failed_test | tojson }}
+  CONFIG.decreaseAttemptsUnUserCodeFailure = {{ config.plugins.pyodide_macros.decrease_attempts_on_user_code_failure | tojson }}
   CONFIG.encryptCorrectionsAndRems = {{ config.plugins.pyodide_macros.encrypt_corrections_and_rems | tojson }}
   CONFIG.buttonIconsDirectory = "{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/images/"
 </script>
 {% endblock %}
 
 
 {% block extrahead %}
@@ -70,15 +71,15 @@
 {% endif %}
 <!-- PYODIDE - insertion token -->
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/pyoditeur-extrahead.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/qcm/qcm-extrahead.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/terminal-extrahead.css">
-<link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css">
+<link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_header-btns-extrahead.css">
 <!-- PYODIDE - insertion token -->
 {% endblock %}
 
 
 {% block scripts %}
 {{ super() }}
 <!-- PYODIDE - insertion token -->
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -53,19 +53,21 @@
 
     await waitForPyodideReady();
     jsLogger("[Validate]")
 
     let [code, terminal, options] = await setupRuntimeAndTerminal(editorName);
     let finalMsg = "",
         stdErr = ""
+    let decrease_count = false
 
     try {
         // Define the user's code in the environment and run the public tests (if any)
         stdErr = await runPythonCodeWithOptions(code, terminal, options)
 
+        decrease_count = CONFIG.decreaseAttemptsUnUserCodeFailure && stdErr
 
         // Run the validation tests only if the user's code succeeded at the previous step
         if (!stdErr) {
 
             // If still running, run the original public tests and the secret ones...
             const publicTests = securedExtraction(editorName, CONFIG.ideProp.publicTests)
             const secretTests = securedExtraction(editorName, CONFIG.ideProp.secretTests)
@@ -75,27 +77,27 @@
             if (!secretTests) return
 
             const autoLogAssert = securedExtraction(editorName, CONFIG.ideProp.autoLogAssert)
             options.autoLogAssert = autoLogAssert !== null ? autoLogAssert : CONFIG.showFailedAssertionsOnValidation
             options.withStdOut = false
 
             const fullTests = `${ publicTests }\n\n${ secretTests }`
-            stdErr = await runPythonCodeWithOptions(fullTests, terminal, options)
+            decrease_count = stdErr = await runPythonCodeWithOptions(fullTests, terminal, options)
+        }
+
+        // On error, manage the counter of tries and the revelation of the solution, otherwise
+        // reveal the solutions + setup success message (displayed in teardown step):
+        if (!stdErr) {
+            unhideSolutionAndRem(editorName)
+            finalMsg = buildSuccessMessage(editorName)
 
-            // On error, manage the counter of tries and the revelation of the solution, otherwise
-            // reveal the solutions + setup success message (displayed in teardown step):
-            if (stdErr) {
-                const nAttemptsLeft = updateIdeCounter(editorName)
-                if (unhideSolutionAndRem(editorName, nAttemptsLeft, false)) {
-                    finalMsg = enhanceFailureMsg(editorName, stdErr)
-                }
-
-            } else {
-                unhideSolutionAndRem(editorName)
-                finalMsg = buildSuccessMessage(editorName)
+        } else if (decrease_count) {
+            const nAttemptsLeft = updateIdeCounter(editorName)
+            if (unhideSolutionAndRem(editorName, nAttemptsLeft, false)) {
+                finalMsg = enhanceFailureMsg(editorName, stdErr)
             }
         }
 
     } finally {
         tearDownRuntimeAndTerminal(terminal, stdErr, finalMsg)
     }
     $.terminal.active().focus()
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -118,15 +118,15 @@
             const plural = nope.length > 1 ? "s" : ""
             const nopes = nope.map(s => s.slice(1)).join(', ')
             const msg = `${ CONFIG.MSG.exclusionMarker } method${plural}: ${ nopes }`
             throw new PythonError(msg)
         }
 
         // Detect possible user imports and install the packages to allow their imports:
-        await installAndImportMissingModules(code, options)
+        await installAndImportMissingModules(code, options, terminal)
 
     } catch (err) {
         const strErr = generateErrorLog(err, code)
         terminal.echo(strErr);
         return strErr
     }
 
@@ -196,15 +196,15 @@
 /**Explore the user's code to find missing modules to install. If some are found, load micropip
  * (if not done yet), then install all the missing modules.
  * Also import all the packages present in options.whiteList.
  *
  * @code : the user's code
  * @options :Same as `runPythonCodeWithOptions`
  * */
-const installAndImportMissingModules = async function(code, options) {
+const installAndImportMissingModules = async function(code, options, terminal) {
 
     const pkgReplacements = options.packagesAliases
     const whiteList = options.whiteList
 
     // Things to import whatever happens:
     const preImport = whiteList.map(name => 'import ' + name)
 
@@ -214,22 +214,24 @@
         name => !installedModules.includes(name) && !options.excluded.includes(name)
     )
 
     if (missing.length) {
         await pyodide.loadPackage("micropip");
         let micropip = pyodide.pyimport("micropip");
 
+        terminal.echo(`Installation de certains packages. Ceci peut prendre un certain temps...`)
         for (let name of missing) {
             if (name in pkgReplacements) {
                 preImport.push(`import ${ pkgReplacements[name] } as ${ name }`)
                 name = pkgReplacements[name]
             }
             jsLogger("[Micropip] - Install", name)
             await micropip.install(name);
         }
+        terminal.echo(`Installations terminées!`)
     }
 
     // Import everything that is needed (either because module aliasing or because the code
     // restrictions would forbid it later):
     pyodide.runPython(preImport.join('\n'))
 }
 
@@ -329,15 +331,15 @@
  *
  * ## SOLUTION FOR BUILTINS FUNCTIONS:
  *
  * - Redeclare forbidden things in the global scope, through `globals()`, using an object that will
  *   systematically throw an ExclusionError when it's called.
  * - Since those are in the global scope, they are visible through `dir()`, so add some make up on
  *   those, using a class that redefines its __qualname__ and __repr__, so that it's less obvious
- *   they are the anticheats (it will still remain obvious for those who know enough, but if they
+ *   they are the anti-cheats (it will still remain obvious for those who know enough, but if they
  *   can find about that, they probably could solve the problem the right way anyway).
  * - The (hidden) function `move_forward('builtin_name')` can be used in the tests to get back the
  *   original builtin. If used, it must be done inside a closure, so that the original builtin
  *   doesn't override the "Raiser" in the global scope (see below).
  * - Pyodide runtime won't see those globals, so it is not affected in any way. Only the user's or
  *   tester's codes are.
  * - Since the hacked version are available to the user in the global runtime, they could just
@@ -349,29 +351,29 @@
  * ## SOLUTION FOR IMPORTS
  *
  * The main problem about `import` is that it actually go directly through `__builtins__`, using
  * `__import__`. So in that case, there is no other choice than hacking directly the __builtins__,
  * and then put it back in place when not useful anymore.
  *
  *
- * ## RECUSION LIMIT
+ * ## RECURSION LIMIT
  *
  * The sys module function is directly hacked, then put back in place: meaning, the function
- * setrecursionlimit is replaced at user's rutnime with a Raiser object. 
+ * setrecursionlimit is replaced at user's runtime with a Raiser object.
  *
  * */
 const setupExclusions = (excluded, recLimit) => {
-    // Store None in the __builtins___ dict for things that aren't builtin functions, aka, names 
+    // Store None in the __builtins___ dict for things that aren't builtin functions, aka, names
     // of forbidden module.
 
     /** WARNING!
-     *  Keep in mind that the code of the Raiser instances will run "in context". 
+     *  Keep in mind that the code of the Raiser instances will run "in context".
      *  This means it will be subject to existing exclusions, so it must never use a function that
      *  could be forbidden. Possibly...
-     *  Force this reason, copies of all the butilins used in the Raiser code are stored locally,
+     *  Force this reason, copies of all the builtins used in the Raiser code are stored locally,
      *  to be sure the Raiser won't use Raiser instances... XD
      * */
     const code = `
     def _hack():
 
         class Raiser:
             __name__ = __qualname__ = 'function'
```

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/0_config-libs.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/functools-libs.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/globalsAndTools/z_header-btns-extrahead.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/qcm/qcm-extrahead.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.2.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.1.2/pyproject.toml` & `pyodide_mkdocs_theme-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.1.2"
+version = "0.2.0"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.1.2/PKG-INFO` & `pyodide_mkdocs_theme-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.1.2
+Version: 0.2.0
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

