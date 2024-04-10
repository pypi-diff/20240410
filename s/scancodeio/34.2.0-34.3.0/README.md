# Comparing `tmp/scancodeio-34.2.0.tar.gz` & `tmp/scancodeio-34.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scancodeio-34.2.0.tar", last modified: Thu Mar 28 16:06:52 2024, max compression
+gzip compressed data, was "scancodeio-34.3.0.tar", last modified: Wed Apr 10 16:28:55 2024, max compression
```

## Comparing `scancodeio-34.2.0.tar` & `scancodeio-34.3.0.tar`

### file list

```diff
@@ -1,549 +1,552 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.452242 scancodeio-34.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.336243 scancodeio-34.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.344243 scancodeio-34.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.github/workflows/publish-docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-28 16:06:36.000000 scancodeio-34.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    54301 2024-03-28 16:06:36.000000 scancodeio-34.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-28 16:06:36.000000 scancodeio-34.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-28 16:06:36.000000 scancodeio-34.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 16:06:36.000000 scancodeio-34.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-28 16:06:36.000000 scancodeio-34.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-28 16:06:36.000000 scancodeio-34.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-03-28 16:06:52.452242 scancodeio-34.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-28 16:06:36.000000 scancodeio-34.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docker-compose-offline.yml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docker-compose.dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docker.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.352243 scancodeio-34.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/application-settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/automation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/built-in-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/command-line-interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/custom-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/data-models.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/distros-os-images.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.360243 scancodeio-34.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   347827 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/license-clarity-scan-summary.png
--rw-r--r--   0 runner    (1001) docker     (127)   113257 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/output-files-download-results.png
--rw-r--r--   0 runner    (1001) docker     (127)    49405 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/output-files-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    59030 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/output-files-xlsx-packages.png
--rw-r--r--   0 runner    (1001) docker     (127)    56604 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/output-files-xlsx-resources.png
--rw-r--r--   0 runner    (1001) docker     (127)   161773 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
--rw-r--r--   0 runner    (1001) docker     (127)    45598 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
--rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
--rw-r--r--   0 runner    (1001) docker     (127)    47458 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-license-policies-results.png
--rw-r--r--   0 runner    (1001) docker     (127)   148235 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-errors-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    71050 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-packages-charts.png
--rw-r--r--   0 runner    (1001) docker     (127)   115814 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-packages-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    86303 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-project-details.png
--rw-r--r--   0 runner    (1001) docker     (127)   152148 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-project-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-project-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    50351 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (127)   165263 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-resources-charts.png
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-resources-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   191624 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/tutorial-web-ui-run-log-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)    53788 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-archive-action.png
--rw-r--r--   0 runner    (1001) docker     (127)   127740 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-archive-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)   153488 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-create-project.png
--rw-r--r--   0 runner    (1001) docker     (127)    52651 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-delete-action.png
--rw-r--r--   0 runner    (1001) docker     (127)   108653 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-delete-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-project-details.png
--rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-project-list-empty.png
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-project-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    52920 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-reset-action.png
--rw-r--r--   0 runner    (1001) docker     (127)    93458 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/images/user-interface-reset-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16103 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/output-files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/project-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/rest-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/scanpipe-concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/scanpipe-pipes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_api_analyze_package_archive.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_cli_analyze_codebase.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_cli_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_license_policies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_vulnerablecode_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_web_ui_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/tutorial_web_ui_review_scan_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-03-28 16:06:36.000000 scancodeio-34.2.0/docs/user-interface.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.336243 scancodeio-34.2.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.336243 scancodeio-34.2.0/etc/nginx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.360243 scancodeio-34.2.0/etc/nginx/conf.d/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/nginx/conf.d/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.360243 scancodeio-34.2.0/etc/nginx/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/nginx/examples/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.368243 scancodeio-34.2.0/etc/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/isc.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-03-28 16:06:36.000000 scancodeio-34.2.0/etc/thirdparty/python.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)  5705128 2024-03-28 16:06:37.000000 scancodeio-34.2.0/etc/thirdparty/virtualenv.pyz
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-28 16:06:37.000000 scancodeio-34.2.0/etc/thirdparty/virtualenv.pyz.ABOUT
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-03-28 16:06:37.000000 scancodeio-34.2.0/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scan.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.368243 scancodeio-34.2.0/scancodeio/
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/scan.NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.376243 scancodeio-34.2.0/scancodeio/static/
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   422462 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/ace-1.20.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)   368864 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/ace-1.9.5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/add-inputs.js
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/billboard-3.0.1-datalab.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   465309 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   207302 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/bulma-0.9.4.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/bulma-toast-2.4.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/cc-by-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/highlight-10.6.0.css
--rw-r--r--   0 runner    (1001) docker     (127)   133121 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/highlight-10.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/highlight.js-10.6.0.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    15888 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/html5sortable-0.9.17.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    44717 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/htmx-1.9.5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/htmx-1.9.5.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/static/ofl-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scancodeio/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.452242 scancodeio-34.2.0/scancodeio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-03-28 16:06:52.000000 scancodeio-34.2.0/scancodeio.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.376243 scancodeio-34.2.0/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.376243 scancodeio-34.2.0/scanpipe/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    25421 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.336243 scancodeio-34.2.0/scanpipe/management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.380243 scancodeio-34.2.0/scanpipe/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/add-input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/add-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/archive-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/create-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/create-user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/delete-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/list-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/purldb-scan-queue-worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/reset-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/show-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/management/commands/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.388243 scancodeio-34.2.0/scanpipe/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0002_run_id_and_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0003_remove_run_run_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0004_run_pipeline_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0005_project_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0008_package_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0011_codebaseresource_is_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0012_run_scancodeio_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0013_project_is_archived.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0014_webhooksubscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0018_codebaseresource_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0019_auto_20220804_1836.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0021_codebaseresource_package_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0023_migrate_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0026_run_current_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0028_codebaserelation_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0033_project_notes_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0034_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0035_set_projects_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0036_alter_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0040_discovereddependency_affected_by_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0041_projectmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0043_delete_projecterror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0045_scan_codebase_packages_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0046_discoveredpackage_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0047_discoveredpackage_scanpipe_di_version_44de05_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0048_inputsource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0049_input_sources_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0050_remove_project_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0051_rename_pipelines_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0052_run_selected_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0053_restructure_pipelines_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0054_rename_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   120580 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.392243 scancodeio-34.2.0/scanpipe/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/collect_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/deploy_to_develop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/docker_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/find_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/inspect_elf_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/inspect_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/load_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/load_sbom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/match_to_matchcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/populate_purldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/resolve_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/root_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/scan_codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipelines/scan_single_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.396243 scancodeio-34.2.0/scanpipe/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (127)    60696 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/js.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/matchcode.py
--rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/pathmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/purldb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/scancode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.396243 scancodeio-34.2.0/scanpipe/pipes/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45964 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/vulnerablecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/pipes/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.340243 scancodeio-34.2.0/scanpipe/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.396243 scancodeio-34.2.0/scanpipe/templates/account/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/account/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.396243 scancodeio-34.2.0/scanpipe/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/registration/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.396243 scancodeio-34.2.0/scanpipe/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.400243 scancodeio-34.2.0/scanpipe/templates/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/app_monitoring.html
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/attribution.html
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dependency_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dependency_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.400243 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/dropdown_hoverable.html
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown_choices_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/help_dropdown_tooltip.html
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/project_download_dropdown.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.404243 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/file_filter.html
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/filter_sort.html
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/form_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/messages.html
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/navbar_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/pagination_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_clone_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_downloads.html
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_labels.html
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_list_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/search_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/license_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/license_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/message_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.408243 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/clone_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/run_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/run_modal_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/package_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/package_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.408243 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_codebase.html
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_inputs.html
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_outputs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_pipelines.html
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/project_charts.html
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/project_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/project_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/project_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/project_settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/relation_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/resource_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/resource_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.412243 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/field_default.html
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/field_raw.html
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_default.html
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_detections.html
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_purldb_loader.html
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tabset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.412243 scancodeio-34.2.0/scanpipe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.432242 scancodeio-34.2.0/scanpipe/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)   223597 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/archive.zip
--rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (127)    21668 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    88110 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (127)    53875 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
--rw-r--r--   0 runner    (1001) docker     (127)    90354 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
--rw-r--r--   0 runner    (1001) docker     (127)    92805 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
--rw-r--r--   0 runner    (1001) docker     (127)    91287 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/basic-rootfs.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
--rw-r--r--   0 runner    (1001) docker     (127)  1447917 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/centos.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)  5427973 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/centos_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.432242 scancodeio-34.2.0/scanpipe/tests/data/codebase/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/codebase/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/codebase/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/codebase/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.432242 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.436242 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   105830 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json
--rw-r--r--   0 runner    (1001) docker     (127)   138679 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json
--rw-r--r--   0 runner    (1001) docker     (127)   139669 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json
--rw-r--r--   0 runner    (1001) docker     (127)   124554 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/missing_bom_format.json
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/missing_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/not_valid.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.436242 scancodeio-34.2.0/scanpipe/tests/data/d2d/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.436242 scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/
--rw-r--r--   0 runner    (1001) docker     (127)    60018 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
--rw-r--r--   0 runner    (1001) docker     (127)    37100 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.440243 scancodeio-34.2.0/scanpipe/tests/data/d2d/find_java_packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.440243 scancodeio-34.2.0/scanpipe/tests/data/d2d/jars/
--rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
--rw-r--r--   0 runner    (1001) docker     (127)    37325 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.440243 scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/license_mit.md
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/project.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/project_notice.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/non_whitespace_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d/whitespace_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.340243 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.436242 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/from/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/from/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.436242 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/debian.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/debian_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)    57175 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-images.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    24550 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)   176998 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)   148656 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/flume-ng-node-d2d-input.json
--rw-r--r--   0 runner    (1001) docker     (127)   156717 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/flume-ng-node-d2d.json
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/foobar.qcow2.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    62008 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1674309 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.440243 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0.tgz
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/javascript_collect_symbols.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.440243 scancodeio-34.2.0/scanpipe/tests/data/jvm/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/jvm/common.java
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/jvm/no-package.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.444243 scancodeio-34.2.0/scanpipe/tests/data/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/package.expected.json
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/poor_values.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/toml.json
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/manifests/toml.spdx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.340243 scancodeio-34.2.0/scanpipe/tests/data/matchcode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.444243 scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    32504 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/notice.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.444243 scancodeio-34.2.0/scanpipe/tests/data/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/outputs/expected_attribution.html
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/outputs/render_me.html
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/policies.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.444243 scancodeio-34.2.0/scanpipe/tests/data/scancode/
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
--rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.444243 scancodeio-34.2.0/scanpipe/tests/data/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/settings/scancode-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.444243 scancodeio-34.2.0/scanpipe/tests/data/spdx/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/spdx/example-2.3.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/data/windows-container-rootfs.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.448243 scancodeio-34.2.0/scanpipe/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/profile_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/raise_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/register_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/steps_as_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipelines/with_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:52.452242 scancodeio-34.2.0/scanpipe/tests/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (127)    58850 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_js.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_matchcode.py
--rw-r--r--   0 runner    (1001) docker     (127)    28436 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_pathmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_purldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_rootfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_scancode.py
--rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/pipes/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/regen_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44714 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    36535 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)   109259 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    51320 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_scancodeio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    46619 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    72631 2024-03-28 16:06:37.000000 scancodeio-34.2.0/scanpipe/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-03-28 16:06:52.452242 scancodeio-34.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1297 2024-03-28 16:06:37.000000 scancodeio-34.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.889352 scancodeio-34.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.781350 scancodeio-34.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/publish-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    54610 2024-04-10 16:28:50.000000 scancodeio-34.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-10 16:28:50.000000 scancodeio-34.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-10 16:28:50.000000 scancodeio-34.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-10 16:28:50.000000 scancodeio-34.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-10 16:28:50.000000 scancodeio-34.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 16:28:50.000000 scancodeio-34.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-10 16:28:55.889352 scancodeio-34.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 16:28:50.000000 scancodeio-34.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker-compose-offline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker-compose.dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.785350 scancodeio-34.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/application-settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/automation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/built-in-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/command-line-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/custom-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/data-models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/distros-os-images.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.793350 scancodeio-34.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   347827 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/license-clarity-scan-summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   113257 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-download-results.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49405 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59030 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-xlsx-packages.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56604 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-xlsx-resources.png
+-rw-r--r--   0 runner    (1001) docker     (127)   161773 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45598 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47458 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-license-policies-results.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148235 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-errors-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71050 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-charts.png
+-rw-r--r--   0 runner    (1001) docker     (127)   115814 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86303 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (127)   152148 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-project-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50351 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165263 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-charts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   191624 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-run-log-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53788 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-archive-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127740 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-archive-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153488 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-create-project.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52651 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-delete-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108653 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-delete-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-project-list-empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52920 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-reset-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93458 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-reset-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16404 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/output-files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/project-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/rest-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/scanpipe-concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/scanpipe-pipes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_api_analyze_package_archive.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_cli_analyze_codebase.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_cli_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_license_policies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_vulnerablecode_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_web_ui_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_web_ui_review_scan_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/user-interface.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/etc/nginx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.793350 scancodeio-34.3.0/etc/nginx/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/nginx/conf.d/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.793350 scancodeio-34.3.0/etc/nginx/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/nginx/examples/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.801350 scancodeio-34.3.0/etc/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/isc.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/python.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)  5705128 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-10 16:28:50.000000 scancodeio-34.3.0/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scan.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.805350 scancodeio-34.3.0/scancodeio/
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/scan.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.809350 scancodeio-34.3.0/scancodeio/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   422462 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.20.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)   368864 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.9.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/add-inputs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/billboard-3.0.1-datalab.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   465309 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   207302 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/cc-by-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.css
+-rw-r--r--   0 runner    (1001) docker     (127)   133121 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/highlight.js-10.6.0.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    15888 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    44717 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/htmx-1.9.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/htmx-1.9.5.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ofl-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.885352 scancodeio-34.3.0/scancodeio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21925 2024-04-10 16:28:55.000000 scancodeio-34.3.0/scancodeio.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.809350 scancodeio-34.3.0/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.813351 scancodeio-34.3.0/scanpipe/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25421 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/scanpipe/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.813351 scancodeio-34.3.0/scanpipe/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/add-input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/add-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/archive-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/create-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/create-user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/delete-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/list-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/purldb-scan-queue-worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/reset-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/show-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.821351 scancodeio-34.3.0/scanpipe/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0002_run_id_and_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0003_remove_run_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0004_run_pipeline_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0005_project_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0008_package_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0011_codebaseresource_is_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0012_run_scancodeio_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0013_project_is_archived.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0014_webhooksubscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0018_codebaseresource_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0019_auto_20220804_1836.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0021_codebaseresource_package_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0023_migrate_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0026_run_current_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0028_codebaserelation_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0033_project_notes_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0034_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0035_set_projects_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0036_alter_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0040_discovereddependency_affected_by_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0041_projectmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0043_delete_projecterror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0045_scan_codebase_packages_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0046_discoveredpackage_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0047_discoveredpackage_scanpipe_di_version_44de05_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0048_inputsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0049_input_sources_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0050_remove_project_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0051_rename_pipelines_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0052_run_selected_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0053_restructure_pipelines_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0054_rename_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120580 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.825351 scancodeio-34.3.0/scanpipe/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/collect_source_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/collect_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/deploy_to_develop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/docker_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/find_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/inspect_elf_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/inspect_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/load_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/load_sbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/match_to_matchcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/populate_purldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/resolve_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/root_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/scan_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/scan_single_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60696 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/matchcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/purldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/scancode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/pipes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45964 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/source_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/vulnerablecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/scanpipe/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/account/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/registration/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.833351 scancodeio-34.3.0/scanpipe/templates/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/app_monitoring.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/attribution.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.837351 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/dropdown_hoverable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown_choices_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/help_dropdown_tooltip.html
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_download_dropdown.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.841351 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/file_filter.html
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/filter_sort.html
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/form_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/navbar_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_clone_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_downloads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_labels.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_list_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/search_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/license_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/license_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/message_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.841351 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/clone_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/package_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/package_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.845351 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_codebase.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_inputs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_outputs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_pipelines.html
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_charts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/relation_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.845351 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_raw.html
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_detections.html
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_purldb_loader.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tabset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.849351 scancodeio-34.3.0/scanpipe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.869351 scancodeio-34.3.0/scanpipe/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   223597 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/archive.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)    21668 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88110 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53875 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90354 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92805 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
+-rw-r--r--   0 runner    (1001) docker     (127)    91287 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1447917 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/centos.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  5427973 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/centos_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.869351 scancodeio-34.3.0/scanpipe/tests/data/codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/codebase/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/codebase/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/codebase/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.869351 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   105830 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   138679 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)   139669 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)   124554 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/missing_bom_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/missing_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/not_valid.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    60018 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    37100 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/
+-rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    37325 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/license_mit.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project_notice.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/non_whitespace_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/whitespace_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.777350 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/debian.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/debian_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)    57175 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    24550 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   176998 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)   148656 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d-input.json
+-rw-r--r--   0 runner    (1001) docker     (127)   156717 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/foobar.qcow2.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    62008 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1674309 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/javascript_collect_symbols.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/jvm/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/jvm/common.java
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/jvm/no-package.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/package.expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/poor_values.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.spdx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.777350 scancodeio-34.3.0/scanpipe/tests/data/matchcode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    32504 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/notice.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/outputs/expected_attribution.html
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/outputs/render_me.html
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/policies.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/scancode/
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/settings/scancode-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/spdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/spdx/example-2.3.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/windows-container-rootfs.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/profile_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/raise_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/register_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/steps_as_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/with_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.885352 scancodeio-34.3.0/scanpipe/tests/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58850 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_matchcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28436 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_purldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_scancode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_source_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/regen_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44714 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36535 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109259 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52454 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_scancodeio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46619 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72631 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-10 16:28:55.889352 scancodeio-34.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1297 2024-04-10 16:28:50.000000 scancodeio-34.3.0/setup.py
```

### Comparing `scancodeio-34.2.0/.github/workflows/ci.yml` & `scancodeio-34.3.0/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,17 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install universal ctags
         run: sudo apt-get install -y universal-ctags
+    
+      - name: Install xgettext
+        run: sudo apt-get install -y gettext
 
       - name: Install dependencies
         run: make dev envfile
 
       - name: Validate code format
         run: make check
```

### Comparing `scancodeio-34.2.0/.github/workflows/publish-docker.yml` & `scancodeio-34.3.0/.github/workflows/publish-docker.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/.github/workflows/pypi-release.yml` & `scancodeio-34.3.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/.gitignore` & `scancodeio-34.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/.readthedocs.yaml` & `scancodeio-34.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/CHANGELOG.rst` & `scancodeio-34.3.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+v34.3.0 (2024-04-10)
+--------------------
+
+- Associate resolved packages with their source codebase resource.
+  https://github.com/nexB/scancode.io/issues/1140
+
+- Add a new `CollectSourceStrings` pipeline (addon) for collecting source string using
+  xgettext.
+  https://github.com/nexB/scancode.io/pull/1160
+
 v34.2.0 (2024-03-28)
 --------------------
 
 - Add support for Python 3.12 and upgrade to Python 3.12 in the Dockerfile.
   https://github.com/nexB/scancode.io/pull/1138
 
 - Add support for CycloneDX XML inputs.
```

### Comparing `scancodeio-34.2.0/Dockerfile` & `scancodeio-34.3.0/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # Do not write Python .pyc files
 ENV PYTHONDONTWRITEBYTECODE 1
 # Add the app dir in the Python path for entry points availability
 ENV PYTHONPATH $PYTHONPATH:$APP_DIR
 
 # OS requirements as per
 # https://scancode-toolkit.readthedocs.io/en/latest/getting-started/install.html
-# Also install universal-ctags for symbol collection.
+# Also install universal-ctags and xgettext for symbol and string collection.
 RUN apt-get update \
  && apt-get install -y --no-install-recommends \
        bzip2 \
        xz-utils \
        zlib1g \
        libxml2-dev \
        libxslt1-dev \
@@ -56,14 +56,15 @@
        libgpgme11 \
        libdevmapper1.02.1 \
        libguestfs-tools \
        linux-image-amd64 \
        git \
        wait-for-it \
        universal-ctags \
+       gettext \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
 
 # Create the APP_USER group and user
 RUN addgroup --system $APP_USER \
  && adduser --system --group --home=$APP_DIR $APP_USER \
  && chown $APP_USER:$APP_USER $APP_DIR
```

### Comparing `scancodeio-34.2.0/LICENSE` & `scancodeio-34.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/Makefile` & `scancodeio-34.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/NOTICE` & `scancodeio-34.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/PKG-INFO` & `scancodeio-34.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scancodeio
-Version: 34.2.0
+Version: 34.3.0
 Summary: Automate software composition analysis pipelines
 Home-page: https://github.com/nexB/scancode.io
 Author: nexB Inc.
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,scan,license,package,dependency,copyright,filetype,author,extract,licensing,scancode,scanpipe,docker,rootfs,vm,virtual machine,pipeline,code analysis,container
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `scancodeio-34.2.0/README.rst` & `scancodeio-34.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docker-compose-offline.yml` & `scancodeio-34.3.0/docker-compose-offline.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docker-compose.yml` & `scancodeio-34.3.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/Makefile` & `scancodeio-34.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/application-settings.rst` & `scancodeio-34.3.0/docs/application-settings.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/automation.rst` & `scancodeio-34.3.0/docs/automation.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/built-in-pipelines.rst` & `scancodeio-34.3.0/docs/built-in-pipelines.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,22 @@
 
 Analyse Docker Windows Image
 ----------------------------
 .. autoclass:: scanpipe.pipelines.docker_windows.DockerWindows()
     :members:
     :member-order: bysource
 
+.. _pipeline_collect_source_strings:
+
+Collect Source Strings (addon)
+--------------------------------
+.. autoclass:: scanpipe.pipelines.collect_source_strings.CollectSourceStrings()
+    :members:
+    :member-order: bysource
+
 .. _pipeline_collect_symbols:
 
 Collect Codebase Symbols (addon)
 --------------------------------
 .. autoclass:: scanpipe.pipelines.collect_symbols.CollectSymbols()
     :members:
     :member-order: bysource
```

### Comparing `scancodeio-34.2.0/docs/command-line-interface.rst` & `scancodeio-34.3.0/docs/command-line-interface.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 .. _command_line_interface:
 
 Command Line Interface
 ======================
 
-A ``scanpipe`` command can be executed through the ``docker compose`` command line
-interface with::
+The ``scanpipe`` command can be executed using the Docker Compose command line interface.
+
+If the Docker Compose stack is already running, you can execute the command as follows:
+
+.. code-block:: shell
 
     docker compose exec -it web scanpipe COMMAND
 
-Alternatively, you can start a ``bash`` session in a new Docker container to execute
-multiple ``scanpipe`` commands::
+If the ScanCode.io services are not currently running, you can use the following command:
+
+.. code-block:: shell
+
+    docker compose run --rm web scanpipe COMMAND
+
+Additionally, you can start a new Docker container and execute multiple
+``scanpipe`` commands within a ``bash`` session:
+
+.. code-block:: shell
 
     docker compose run web bash
     scanpipe COMMAND
     scanpipe COMMAND
     ...
 
 .. warning::
@@ -240,14 +251,16 @@
 
 Optional arguments:
 
 - ``--print`` Print the output to stdout instead of creating a file. This is not
   compatible with the XLSX and CSV formats.
   It cannot be used when multiple formats are provided.
 
+Refer to :ref:`Mount projects workspace <mount_projects_workspace_volume>` to access
+your outputs on the host machine when running with Docker.
 
 `$ scanpipe archive-project --project PROJECT`
 ----------------------------------------------
 
 Archives a project and remove selected work directories.
 
 Optional arguments:
```

### Comparing `scancodeio-34.2.0/docs/conf.py` & `scancodeio-34.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/contributing.rst` & `scancodeio-34.3.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/custom-pipelines.rst` & `scancodeio-34.3.0/docs/custom-pipelines.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/data-models.rst` & `scancodeio-34.3.0/docs/data-models.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/distros-os-images.rst` & `scancodeio-34.3.0/docs/distros-os-images.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/faq.rst` & `scancodeio-34.3.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/license-clarity-scan-summary.png` & `scancodeio-34.3.0/docs/images/license-clarity-scan-summary.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/output-files-download-results.png` & `scancodeio-34.3.0/docs/images/output-files-download-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/output-files-projects-list.png` & `scancodeio-34.3.0/docs/images/output-files-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/output-files-xlsx-packages.png` & `scancodeio-34.3.0/docs/images/output-files-xlsx-packages.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/output-files-xlsx-resources.png` & `scancodeio-34.3.0/docs/images/output-files-xlsx-resources.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-find-vulnerabilities-extra-data.png` & `scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-extra-data.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-find-vulnerabilities-icon-link.png` & `scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-icon-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-find-vulnerabilities-packages-link.png` & `scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-packages-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-license-policies-results.png` & `scancodeio-34.3.0/docs/images/tutorial-license-policies-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-errors-list.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-errors-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-packages-charts.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-packages-list.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-project-details.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-project-form.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-project-form.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-project-list.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-projects-list.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-resources-charts.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-resources-filter.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-filter.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/tutorial-web-ui-run-log-modal.png` & `scancodeio-34.3.0/docs/images/tutorial-web-ui-run-log-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-archive-action.png` & `scancodeio-34.3.0/docs/images/user-interface-archive-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-archive-modal.png` & `scancodeio-34.3.0/docs/images/user-interface-archive-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-create-project.png` & `scancodeio-34.3.0/docs/images/user-interface-create-project.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-delete-action.png` & `scancodeio-34.3.0/docs/images/user-interface-delete-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-delete-modal.png` & `scancodeio-34.3.0/docs/images/user-interface-delete-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-project-details.png` & `scancodeio-34.3.0/docs/images/user-interface-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-project-list-empty.png` & `scancodeio-34.3.0/docs/images/user-interface-project-list-empty.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-project-list.png` & `scancodeio-34.3.0/docs/images/user-interface-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-reset-action.png` & `scancodeio-34.3.0/docs/images/user-interface-reset-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/images/user-interface-reset-modal.png` & `scancodeio-34.3.0/docs/images/user-interface-reset-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/index.rst` & `scancodeio-34.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/installation.rst` & `scancodeio-34.3.0/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -257,21 +257,32 @@
         bzip2 xz-utils zlib1g libxml2-dev libxslt1-dev libpopt0 \
         libgpgme11 libdevmapper1.02.1 libguestfs-tools
 
 See also `ScanCode-toolkit Prerequisites <https://scancode-toolkit.readthedocs.io/en/
 latest/getting-started/install.html#prerequisites>`_ for more details.
 
 For the :ref:`pipeline_collect_symbols` pipeline, `Universal Ctags <https://github.com/universal-ctags/ctags>`_ is needed.
-On **Linux** install it using::
 
-    sudo apt-get install universal-ctags
+    * On **Linux** install it using::
 
-On **MacOS** install Universal Ctags using Homebrew::
+        sudo apt-get install universal-ctags
 
-    brew install universal-ctags
+    * On **MacOS** install Universal Ctags using Homebrew::
+
+        brew install universal-ctags
+
+For the :ref:`pipeline_collect_source_strings` pipeline, `gettext <https://www.gnu.org/software/gettext/>`_ is needed.
+
+    * On **Linux** install it using::
+
+        sudo apt-get install gettext
+
+    * On **MacOS** install gettext using Homebrew::
+
+        brew install gettext
 
 Clone and Configure
 ^^^^^^^^^^^^^^^^^^^
 
  * Clone the `ScanCode.io GitHub repository <https://github.com/nexB/scancode.io>`_::
 
     git clone https://github.com/nexB/scancode.io.git && cd scancode.io
```

### Comparing `scancodeio-34.2.0/docs/introduction.rst` & `scancodeio-34.3.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/make.bat` & `scancodeio-34.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/output-files.rst` & `scancodeio-34.3.0/docs/output-files.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,36 @@
 
 .. note::
     The previous command will output the scan results in a file format
     – as specified – with the output files created in the
     ``PROJECT``'s :guilabel:`output/` directory. By default, JSON output
     files are created when no file format is given.
 
+.. _mount_projects_workspace_volume:
+
+.. warning::
+    When running with Docker, ensure that the output files workspace is assigned
+    to a volume to be accessible on the host machine.
+
+    To add local input files to a project using the :ref:`command_line_interface`,
+    additional arguments need to be passed to the ``docker compose`` command.
+
+    For example, using the following command will mount and make available the
+    projects workspace on the host at ``~/projects/``:
+
+    .. code-block:: bash
+
+        mkdir ~/projects/
+        docker compose run --volume ~/projects/:/var/scancodeio/workspace/projects/ \
+            web scanpipe output --project my_project --format json
+
+    Alternatively, you can also locate the Docker volumes directory on your host
+    machine. For instance, on Linux, it's typically found at:
+    ``/var/lib/docker/volumes/``.
+
 Web UI
 ^^^^^^
 When using the ScanCode.io web application, you can download the results of your
 project in your preferred output format within the project page.
 
 .. image:: images/output-files-download-results.png
```

### Comparing `scancodeio-34.2.0/docs/project-configuration.rst` & `scancodeio-34.3.0/docs/project-configuration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/rest-api.rst` & `scancodeio-34.3.0/docs/rest-api.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/scanpipe-concepts.rst` & `scancodeio-34.3.0/docs/scanpipe-concepts.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/scanpipe-pipes.rst` & `scancodeio-34.3.0/docs/scanpipe-pipes.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_api_analyze_package_archive.rst` & `scancodeio-34.3.0/docs/tutorial_api_analyze_package_archive.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_cli_analyze_codebase.rst` & `scancodeio-34.3.0/docs/tutorial_cli_analyze_codebase.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_cli_analyze_docker_image.rst` & `scancodeio-34.3.0/docs/tutorial_cli_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_license_policies.rst` & `scancodeio-34.3.0/docs/tutorial_license_policies.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_vulnerablecode_integration.rst` & `scancodeio-34.3.0/docs/tutorial_vulnerablecode_integration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_web_ui_analyze_docker_image.rst` & `scancodeio-34.3.0/docs/tutorial_web_ui_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/tutorial_web_ui_review_scan_results.rst` & `scancodeio-34.3.0/docs/tutorial_web_ui_review_scan_results.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/docs/user-interface.rst` & `scancodeio-34.3.0/docs/user-interface.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/nginx/examples/ssl.conf` & `scancodeio-34.3.0/etc/nginx/examples/ssl.conf`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/apache-2.0.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/bsd-new.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/bsd-simplified.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/isc.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/isc.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/lgpl-2.1-plus.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/lgpl-2.1-plus.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/mit.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/python.LICENSE` & `scancodeio-34.3.0/etc/thirdparty/python.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/virtualenv.pyz` & `scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/etc/thirdparty/virtualenv.pyz.ABOUT` & `scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/__init__.py` & `scancodeio-34.3.0/scancodeio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import sys
 import warnings
 from contextlib import suppress
 from pathlib import Path
 
 import git
 
-VERSION = "34.2.0"
+VERSION = "34.3.0"
 
 PROJECT_DIR = Path(__file__).resolve().parent
 ROOT_DIR = PROJECT_DIR.parent
 SCAN_NOTICE = PROJECT_DIR.joinpath("scan.NOTICE").read_text()
 GITHUB_URL = "https://github.com/nexB/scancode.io"
```

### Comparing `scancodeio-34.2.0/scancodeio/auth.py` & `scancodeio-34.3.0/scancodeio/auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/context_processors.py` & `scancodeio-34.3.0/scancodeio/context_processors.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/settings.py` & `scancodeio-34.3.0/scancodeio/settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js` & `scancodeio-34.3.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/ace-1.20.0.min.js` & `scancodeio-34.3.0/scancodeio/static/ace-1.20.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/ace-1.9.5.min.js` & `scancodeio-34.3.0/scancodeio/static/ace-1.9.5.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/add-inputs.js` & `scancodeio-34.3.0/scancodeio/static/add-inputs.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/billboard-3.0.1-datalab.min.css` & `scancodeio-34.3.0/scancodeio/static/billboard-3.0.1-datalab.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/billboard-3.0.1.pkgd.min.js` & `scancodeio-34.3.0/scancodeio/static/billboard-3.0.1.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/bsd-new.LICENSE` & `scancodeio-34.3.0/scancodeio/static/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/bsd-simplified.LICENSE` & `scancodeio-34.3.0/scancodeio/static/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/bulma-0.9.4.min.css` & `scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT` & `scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/bulma-toast-2.4.1.min.js` & `scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT` & `scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/cc-by-4.0.LICENSE` & `scancodeio-34.3.0/scancodeio/static/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/favicon.ico` & `scancodeio-34.3.0/scancodeio/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/highlight-10.6.0.css` & `scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.css`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/highlight-10.6.0.min.js` & `scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/html5sortable-0.9.17.min.js` & `scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT` & `scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/htmx-1.9.5.min.js` & `scancodeio-34.3.0/scancodeio/static/htmx-1.9.5.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/main.js` & `scancodeio-34.3.0/scancodeio/static/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/mit.LICENSE` & `scancodeio-34.3.0/scancodeio/static/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/static/ofl-1.1.LICENSE` & `scancodeio-34.3.0/scancodeio/static/ofl-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/urls.py` & `scancodeio-34.3.0/scancodeio/urls.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/worker.py` & `scancodeio-34.3.0/scancodeio/worker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio/wsgi.py` & `scancodeio-34.3.0/scancodeio/wsgi.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scancodeio.egg-info/SOURCES.txt` & `scancodeio-34.3.0/scancodeio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 scanpipe/migrations/0051_rename_pipelines_data.py
 scanpipe/migrations/0052_run_selected_groups.py
 scanpipe/migrations/0053_restructure_pipelines_data.py
 scanpipe/migrations/0054_rename_pipeline.py
 scanpipe/migrations/0055_discoveredpackage_datafile_paths.py
 scanpipe/migrations/__init__.py
 scanpipe/pipelines/__init__.py
+scanpipe/pipelines/collect_source_strings.py
 scanpipe/pipelines/collect_symbols.py
 scanpipe/pipelines/deploy_to_develop.py
 scanpipe/pipelines/docker.py
 scanpipe/pipelines/docker_windows.py
 scanpipe/pipelines/find_vulnerabilities.py
 scanpipe/pipelines/inspect_elf_binaries.py
 scanpipe/pipelines/inspect_packages.py
@@ -236,14 +237,15 @@
 scanpipe/pipes/matchcode.py
 scanpipe/pipes/output.py
 scanpipe/pipes/pathmap.py
 scanpipe/pipes/purldb.py
 scanpipe/pipes/resolve.py
 scanpipe/pipes/rootfs.py
 scanpipe/pipes/scancode.py
+scanpipe/pipes/source_strings.py
 scanpipe/pipes/spdx.py
 scanpipe/pipes/symbols.py
 scanpipe/pipes/vulnerablecode.py
 scanpipe/pipes/windows.py
 scanpipe/pipes/schemas/spdx-schema-2.3.json
 scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT
 scanpipe/templates/account/profile.html
@@ -483,10 +485,11 @@
 scanpipe/tests/pipes/test_output.py
 scanpipe/tests/pipes/test_pathmap.py
 scanpipe/tests/pipes/test_pipes.py
 scanpipe/tests/pipes/test_purldb.py
 scanpipe/tests/pipes/test_resolve.py
 scanpipe/tests/pipes/test_rootfs.py
 scanpipe/tests/pipes/test_scancode.py
+scanpipe/tests/pipes/test_source_strings.py
 scanpipe/tests/pipes/test_spdx.py
 scanpipe/tests/pipes/test_symbols.py
 scanpipe/tests/pipes/test_windows.py
```

### Comparing `scancodeio-34.2.0/scanpipe/__init__.py` & `scancodeio-34.3.0/scanpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/api/__init__.py` & `scancodeio-34.3.0/scanpipe/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/api/serializers.py` & `scancodeio-34.3.0/scanpipe/api/serializers.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/api/views.py` & `scancodeio-34.3.0/scanpipe/api/views.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/apps.py` & `scancodeio-34.3.0/scanpipe/apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/filters.py` & `scancodeio-34.3.0/scanpipe/filters.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/forms.py` & `scancodeio-34.3.0/scanpipe/forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/__init__.py` & `scancodeio-34.3.0/scanpipe/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/add-input.py` & `scancodeio-34.3.0/scanpipe/management/commands/add-input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/add-pipeline.py` & `scancodeio-34.3.0/scanpipe/management/commands/add-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/archive-project.py` & `scancodeio-34.3.0/scanpipe/management/commands/archive-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/create-project.py` & `scancodeio-34.3.0/scanpipe/management/commands/create-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/create-user.py` & `scancodeio-34.3.0/scanpipe/management/commands/create-user.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/delete-project.py` & `scancodeio-34.3.0/scanpipe/management/commands/delete-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/execute.py` & `scancodeio-34.3.0/scanpipe/management/commands/execute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/list-project.py` & `scancodeio-34.3.0/scanpipe/management/commands/list-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/output.py` & `scancodeio-34.3.0/scanpipe/management/commands/output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/purldb-scan-queue-worker.py` & `scancodeio-34.3.0/scanpipe/management/commands/purldb-scan-queue-worker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/reset-project.py` & `scancodeio-34.3.0/scanpipe/management/commands/reset-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/show-pipeline.py` & `scancodeio-34.3.0/scanpipe/management/commands/show-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/management/commands/status.py` & `scancodeio-34.3.0/scanpipe/management/commands/status.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0001_initial.py` & `scancodeio-34.3.0/scanpipe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0002_run_id_and_log.py` & `scancodeio-34.3.0/scanpipe/migrations/0002_run_id_and_log.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0004_run_pipeline_name.py` & `scancodeio-34.3.0/scanpipe/migrations/0004_run_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py` & `scancodeio-34.3.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py` & `scancodeio-34.3.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0008_package_extra_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0008_package_extra_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0013_project_is_archived.py` & `scancodeio-34.3.0/scanpipe/migrations/0013_project_is_archived.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0014_webhooksubscription.py` & `scancodeio-34.3.0/scanpipe/migrations/0014_webhooksubscription.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0019_auto_20220804_1836.py` & `scancodeio-34.3.0/scanpipe/migrations/0019_auto_20220804_1836.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0022_create_discovereddependencies_model.py` & `scancodeio-34.3.0/scanpipe/migrations/0022_create_discovereddependencies_model.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0023_migrate_dependencies.py` & `scancodeio-34.3.0/scanpipe/migrations/0023_migrate_dependencies.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0028_codebaserelation_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0028_codebaserelation_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py` & `scancodeio-34.3.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py` & `scancodeio-34.3.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py` & `scancodeio-34.3.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0033_project_notes_project_settings.py` & `scancodeio-34.3.0/scanpipe/migrations/0033_project_notes_project_settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0035_set_projects_slug.py` & `scancodeio-34.3.0/scanpipe/migrations/0035_set_projects_slug.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0038_migrate_vulnerability_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0038_migrate_vulnerability_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py` & `scancodeio-34.3.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0041_projectmessage.py` & `scancodeio-34.3.0/scanpipe/migrations/0041_projectmessage.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py` & `scancodeio-34.3.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0045_scan_codebase_packages_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0045_scan_codebase_packages_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0046_discoveredpackage_tag.py` & `scancodeio-34.3.0/scanpipe/migrations/0046_discoveredpackage_tag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0048_inputsource.py` & `scancodeio-34.3.0/scanpipe/migrations/0048_inputsource.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0049_input_sources_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0049_input_sources_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0051_rename_pipelines_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0051_rename_pipelines_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0052_run_selected_groups.py` & `scancodeio-34.3.0/scanpipe/migrations/0052_run_selected_groups.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0053_restructure_pipelines_data.py` & `scancodeio-34.3.0/scanpipe/migrations/0053_restructure_pipelines_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0054_rename_pipeline.py` & `scancodeio-34.3.0/scanpipe/migrations/0054_rename_pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py` & `scancodeio-34.3.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/models.py` & `scancodeio-34.3.0/scanpipe/models.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/__init__.py` & `scancodeio-34.3.0/scanpipe/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/collect_symbols.py` & `scancodeio-34.3.0/scanpipe/pipelines/collect_symbols.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/deploy_to_develop.py` & `scancodeio-34.3.0/scanpipe/pipelines/deploy_to_develop.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/docker.py` & `scancodeio-34.3.0/scanpipe/pipelines/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/docker_windows.py` & `scancodeio-34.3.0/scanpipe/pipelines/docker_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/find_vulnerabilities.py` & `scancodeio-34.3.0/scanpipe/pipelines/find_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/inspect_elf_binaries.py` & `scancodeio-34.3.0/scanpipe/pipelines/inspect_elf_binaries.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/inspect_packages.py` & `scancodeio-34.3.0/scanpipe/pipelines/inspect_packages.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/load_inventory.py` & `scancodeio-34.3.0/scanpipe/pipelines/load_inventory.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/load_sbom.py` & `scancodeio-34.3.0/scanpipe/pipelines/load_sbom.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/match_to_matchcode.py` & `scancodeio-34.3.0/scanpipe/pipelines/match_to_matchcode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/populate_purldb.py` & `scancodeio-34.3.0/scanpipe/pipelines/populate_purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/resolve_dependencies.py` & `scancodeio-34.3.0/scanpipe/pipelines/resolve_dependencies.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/root_filesystem.py` & `scancodeio-34.3.0/scanpipe/pipelines/root_filesystem.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/scan_codebase.py` & `scancodeio-34.3.0/scanpipe/pipelines/scan_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipelines/scan_single_package.py` & `scancodeio-34.3.0/scanpipe/pipelines/scan_single_package.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/__init__.py` & `scancodeio-34.3.0/scanpipe/pipes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     )
 
     if package:
         package.update_from_data(package_data)
     else:
         package = DiscoveredPackage.create_from_data(project, package_data)
 
-    if codebase_resources:
+    if package and codebase_resources:
         package.add_resources(codebase_resources)
 
     return package
 
 
 def create_local_files_package(project, defaults, codebase_resources=None):
     """Create a local-files package using provided ``defaults`` data."""
```

### Comparing `scancodeio-34.2.0/scanpipe/pipes/codebase.py` & `scancodeio-34.3.0/scanpipe/pipes/codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/compliance.py` & `scancodeio-34.3.0/scanpipe/pipes/compliance.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/cyclonedx.py` & `scancodeio-34.3.0/scanpipe/pipes/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/d2d.py` & `scancodeio-34.3.0/scanpipe/pipes/d2d.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/docker.py` & `scancodeio-34.3.0/scanpipe/pipes/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/elf.py` & `scancodeio-34.3.0/scanpipe/pipes/elf.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/fetch.py` & `scancodeio-34.3.0/scanpipe/pipes/fetch.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/flag.py` & `scancodeio-34.3.0/scanpipe/pipes/flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/input.py` & `scancodeio-34.3.0/scanpipe/pipes/input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/js.py` & `scancodeio-34.3.0/scanpipe/pipes/js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/jvm.py` & `scancodeio-34.3.0/scanpipe/pipes/jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/matchcode.py` & `scancodeio-34.3.0/scanpipe/pipes/matchcode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/output.py` & `scancodeio-34.3.0/scanpipe/pipes/output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/pathmap.py` & `scancodeio-34.3.0/scanpipe/pipes/pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/purldb.py` & `scancodeio-34.3.0/scanpipe/pipes/purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/resolve.py` & `scancodeio-34.3.0/scanpipe/pipes/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,20 @@
             description="No resources found with package data",
             model=model,
         )
         return
 
     for resource in manifest_resources:
         if packages := get_packages_from_manifest(resource.location, package_registry):
+            for package_data in packages:
+                package_data["codebase_resources"] = [resource]
             resolved_packages.extend(packages)
         else:
             project.add_error(
-                description="No packages could be resolved for",
+                description="No packages could be resolved",
                 model=model,
                 resource=resource,
             )
 
     return resolved_packages
 
 
@@ -76,15 +78,16 @@
 
     If resolved, create packages out of resolved dependencies,
     otherwise create dependencies.
     """
     for package_data in packages:
         package_data = set_license_expression(package_data)
         dependencies = package_data.pop("dependencies", [])
-        update_or_create_package(project, package_data)
+        codebase_resources = package_data.pop("codebase_resources", [])
+        update_or_create_package(project, package_data, codebase_resources)
 
         for dependency_data in dependencies:
             if resolved:
                 if resolved_package := dependency_data.get("resolved_package"):
                     resolved_package.pop("dependencies", [])
                     update_or_create_package(project, resolved_package)
             else:
```

### Comparing `scancodeio-34.2.0/scanpipe/pipes/rootfs.py` & `scancodeio-34.3.0/scanpipe/pipes/rootfs.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/scancode.py` & `scancodeio-34.3.0/scanpipe/pipes/scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/schemas/spdx-schema-2.3.json` & `scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT` & `scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/spdx.py` & `scancodeio-34.3.0/scanpipe/pipes/spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/symbols.py` & `scancodeio-34.3.0/scanpipe/pipes/symbols.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/vulnerablecode.py` & `scancodeio-34.3.0/scanpipe/pipes/vulnerablecode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/pipes/windows.py` & `scancodeio-34.3.0/scanpipe/pipes/windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tasks.py` & `scancodeio-34.3.0/scanpipe/tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/account/profile.html` & `scancodeio-34.3.0/scanpipe/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/registration/login.html` & `scancodeio-34.3.0/scanpipe/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/rest_framework/api.html` & `scancodeio-34.3.0/scanpipe/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/app_monitoring.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/app_monitoring.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/attribution.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/base.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/base.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/dependency_detail.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/dependency_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/dropdowns/project_download_dropdown.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_download_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/breadcrumb.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/file_filter.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/file_filter.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/list_view_thead.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/list_view_thead.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/navbar_header.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/navbar_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/pagination.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/pagination_header.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_clone_form.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_clone_form.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_downloads.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_downloads.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_list_table.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_list_table.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/project_summary_level.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_summary_level.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/resource_path_links.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_path_links.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/run_status_tag.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/run_status_tag.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/includes/search_field.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/search_field.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/license_detail.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/license_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/license_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/license_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/message_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/message_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/clone_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/clone_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/run_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/run_modal_content.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/package_detail.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/package_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/package_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/package_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_codebase.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_codebase.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_inputs.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_inputs.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_outputs.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_outputs.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/project_pipelines.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_pipelines.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/project_charts.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_charts.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/project_detail.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/project_form.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_form.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/project_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/project_settings.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_settings.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/relation_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/relation_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/resource_detail.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/resource_list.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_detections.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_detections.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_packages.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_packages.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_relations.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_relations.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_resources.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_resources.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/templates/scanpipe/tabset/tabset.html` & `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tabset.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/__init__.py` & `scancodeio-34.3.0/scanpipe/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/alpine_3_15_4.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/archive.zip` & `scancodeio-34.3.0/scanpipe/tests/data/archive.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_tree.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_tree.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json` & `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/basic-rootfs.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json` & `scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/centos.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/centos.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/centos_scan_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/centos_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/missing_schema.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/missing_schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/cyclonedx/nested.cdx.json` & `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/nested.cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/expected.json` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/license_mit.md` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/license_mit.md`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/project.LICENSE` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d/legal/project_notice.txt` & `scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project_notice.txt`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/from/main.js` & `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/from/unmain.js` & `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/unmain.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/main.js.map` & `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/main.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map` & `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map` & `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl` & `scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/debian.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/debian.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/debian_scan_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/debian_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html` & `scancodeio-34.3.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-images.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json` & `scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json` & `scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz` & `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json` & `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz` & `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json` & `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/flume-ng-node-d2d-input.json` & `scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d-input.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/flume-ng-node-d2d.json` & `scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/foobar.qcow2.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/foobar.qcow2.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar` & `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar` & `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json` & `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json` & `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json` & `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0.tgz` & `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0.tgz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json` & `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json` & `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/javascript_collect_symbols.json` & `scancodeio-34.3.0/scanpipe/tests/data/javascript_collect_symbols.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/jvm/common.java` & `scancodeio-34.3.0/scanpipe/tests/data/jvm/common.java`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/package.expected.json` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/package.expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/package.json` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/toml.json` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/manifests/toml.spdx.json` & `scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json` & `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json` & `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json` & `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz` & `scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json` & `scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json` & `scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/notice.NOTICE` & `scancodeio-34.3.0/scanpipe/tests/data/notice.NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx` & `scancodeio-34.3.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/outputs/expected_attribution.html` & `scancodeio-34.3.0/scanpipe/tests/data/outputs/expected_attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json` & `scancodeio-34.3.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/scancode/package_assembly_codebase.json` & `scancodeio-34.3.0/scanpipe/tests/data/scancode/package_assembly_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/spdx/example-2.3.1.json` & `scancodeio-34.3.0/scanpipe/tests/data/spdx/example-2.3.1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/data/windows-container-rootfs.tar` & `scancodeio-34.3.0/scanpipe/tests/data/windows-container-rootfs.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipelines/do_nothing.py` & `scancodeio-34.3.0/scanpipe/tests/pipelines/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipelines/profile_step.py` & `scancodeio-34.3.0/scanpipe/tests/pipelines/profile_step.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipelines/raise_exception.py` & `scancodeio-34.3.0/scanpipe/tests/pipelines/raise_exception.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipelines/register_from_file.py` & `scancodeio-34.3.0/scanpipe/tests/pipelines/register_from_file.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipelines/steps_as_attribute.py` & `scancodeio-34.3.0/scanpipe/tests/pipelines/steps_as_attribute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipelines/with_groups.py` & `scancodeio-34.3.0/scanpipe/tests/pipelines/with_groups.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_codebase.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_cyclonedx.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_d2d.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_d2d.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_docker.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_fetch.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_fetch.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_flag.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_input.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_js.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_jvm.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_matchcode.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_matchcode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_output.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_pathmap.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_pipes.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_pipes.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,17 @@
         # Make sure we can assign a package to multiple Resources calling
         # update_or_create_package() several times.
         resource2 = make_resource_file(project=p1, path="filename2.ext")
         package2 = pipes.update_or_create_package(p1, package_data2, [resource2])
         self.assertIn(package2, resource1.discovered_packages.all())
         self.assertIn(package2, resource2.discovered_packages.all())
 
+        # Make sure the following does not raise an exception
+        self.assertIsNone(pipes.update_or_create_package(p1, {}, [resource1]))
+
     def test_scanpipe_pipes_update_or_create_package_codebase_resources(self):
         p1 = Project.objects.create(name="Analysis")
         resource1 = make_resource_file(project=p1, path="filename.ext")
         resource2 = make_resource_file(project=p1, path="filename2.ext")
         resources = [resource1, resource2]
 
         # On creation
```

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_purldb.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_resolve.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,18 @@
 
         packages = resolve.get_packages(
             project1,
             resolve.sbom_registry,
             resources,
         )
         self.assertEqual(1, len(packages))
-        self.assertEqual("toml", packages[0]["name"])
+        package = packages[0]
+        self.assertEqual("toml", package["name"])
+        resource1 = project1.codebaseresources.get(name="toml.spdx.json")
+        self.assertEqual([resource1], package.get("codebase_resources"))
 
     def test_scanpipe_resolve_create_packages_and_dependencies(self):
         project1 = Project.objects.create(name="Analysis")
         input_location = self.data_location / "manifests" / "toml.spdx.json"
 
         project1.copy_input_from(input_location)
         copy_inputs(project1.inputs(), project1.codebase_path)
@@ -210,7 +213,11 @@
             project1,
             resolve.sbom_registry,
             resources,
         )
         resolve.create_packages_and_dependencies(project1, packages)
         self.assertEqual(1, project1.discoveredpackages.count())
         self.assertEqual(0, project1.discovereddependencies.count())
+
+        resource1 = project1.codebaseresources.get(name="toml.spdx.json")
+        package = project1.discoveredpackages.get()
+        self.assertEqual(resource1, package.codebase_resources.get())
```

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_rootfs.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_rootfs.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_scancode.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_spdx.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_symbols.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_symbols.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/pipes/test_windows.py` & `scancodeio-34.3.0/scanpipe/tests/pipes/test_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/regen_test_data.py` & `scancodeio-34.3.0/scanpipe/tests/regen_test_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_api.py` & `scancodeio-34.3.0/scanpipe/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_apps.py` & `scancodeio-34.3.0/scanpipe/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_auth.py` & `scancodeio-34.3.0/scanpipe/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_commands.py` & `scancodeio-34.3.0/scanpipe/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_filters.py` & `scancodeio-34.3.0/scanpipe/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_forms.py` & `scancodeio-34.3.0/scanpipe/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_models.py` & `scancodeio-34.3.0/scanpipe/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_pipelines.py` & `scancodeio-34.3.0/scanpipe/tests/test_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -911,15 +911,15 @@
         pipeline = run.make_pipeline_instance()
 
         project1.move_input_from(tempfile.mkstemp(suffix="requirements.txt")[1])
         pipeline.execute()
         self.assertEqual(1, project1.projectmessages.count())
         message = project1.projectmessages.get()
         self.assertEqual("get_packages_from_manifest", message.model)
-        expected = "No packages could be resolved for"
+        expected = "No packages could be resolved"
         self.assertIn(expected, message.description)
 
     def test_scanpipe_resolve_dependencies_pipeline_integration_misc(self):
         pipeline_name = "resolve_dependencies"
         project1 = Project.objects.create(name="Analysis")
 
         input_location = self.data_location / "manifests" / "requirements.txt"
@@ -1236,7 +1236,34 @@
         exitcode, out = pipeline.execute()
         self.assertEqual(0, exitcode, msg=out)
 
         main_file = project1.codebaseresources.files()[0]
         result_extra_data_symbols = main_file.extra_data.get("source_symbols")
         expected_extra_data_symbols = ["generatePassword", "passwordLength", "charSet"]
         self.assertCountEqual(expected_extra_data_symbols, result_extra_data_symbols)
+
+    @skipIf(sys.platform != "linux", "Only supported on Linux")
+    def test_scanpipe_collect_source_strings_pipeline_integration(self):
+        pipeline_name = "collect_source_strings"
+        project1 = Project.objects.create(name="Analysis")
+
+        dir = project1.codebase_path / "codefile"
+        dir.mkdir(parents=True)
+
+        file_location = self.data_location / "d2d-javascript" / "from" / "main.js"
+        copy_input(file_location, dir)
+
+        pipes.collect_and_create_codebase_resources(project1)
+
+        run = project1.add_pipeline(pipeline_name)
+        pipeline = run.make_pipeline_instance()
+
+        exitcode, out = pipeline.execute()
+        self.assertEqual(0, exitcode, msg=out)
+
+        main_file = project1.codebaseresources.files()[0]
+        result_extra_data_strings = main_file.extra_data.get("source_strings")
+        expected_extra_data_strings = [
+            "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890!@#$%^&*()_-+=",  # noqa
+            "Enter the desired length of your password:",
+        ]
+        self.assertCountEqual(expected_extra_data_strings, result_extra_data_strings)
```

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_scancodeio.py` & `scancodeio-34.3.0/scanpipe/tests/test_scancodeio.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_tasks.py` & `scancodeio-34.3.0/scanpipe/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/tests/test_views.py` & `scancodeio-34.3.0/scanpipe/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/urls.py` & `scancodeio-34.3.0/scanpipe/urls.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/scanpipe/views.py` & `scancodeio-34.3.0/scanpipe/views.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.2.0/setup.cfg` & `scancodeio-34.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scancodeio
-version = 34.2.0
+version = 34.3.0
 license = Apache-2.0
 description = Automate software composition analysis pipelines
 long_description = file:README.rst
 author = nexB Inc.
 author_email = info@aboutcode.org
 url = https://github.com/nexB/scancode.io
 classifiers = 
@@ -105,14 +105,15 @@
 [options.entry_points]
 console_scripts = 
 	scanpipe = scancodeio:command_line
 scancodeio_pipelines = 
 	analyze_docker_image = scanpipe.pipelines.docker:Docker
 	analyze_root_filesystem_or_vm_image = scanpipe.pipelines.root_filesystem:RootFS
 	analyze_windows_docker_image = scanpipe.pipelines.docker_windows:DockerWindows
+	collect_source_strings = scanpipe.pipelines.collect_source_strings:CollectSourceStrings
 	collect_symbols = scanpipe.pipelines.collect_symbols:CollectSymbols
 	find_vulnerabilities = scanpipe.pipelines.find_vulnerabilities:FindVulnerabilities
 	inspect_elf_binaries = scanpipe.pipelines.inspect_elf_binaries:InspectELFBinaries
 	inspect_packages = scanpipe.pipelines.inspect_packages:InspectPackages
 	load_inventory = scanpipe.pipelines.load_inventory:LoadInventory
 	load_sbom = scanpipe.pipelines.load_sbom:LoadSBOM
 	map_deploy_to_develop = scanpipe.pipelines.deploy_to_develop:DeployToDevelop
@@ -136,15 +137,15 @@
 ignore = E203,W503
 
 [pydocstyle]
 ignore = D1,D203,D205,D212,D400,D415
 
 [bumpver]
 version_pattern = "MAJOR.MINOR.PATCH"
-current_version = "34.2.0"
+current_version = "34.3.0"
 
 [bumpver:file_patterns]
 setup.cfg = 
 	version = {version}
 	current_version = "{version}"
 scancodeio/__init__.py = {version}
```

### Comparing `scancodeio-34.2.0/setup.py` & `scancodeio-34.3.0/setup.py`

 * *Files identical despite different names*

