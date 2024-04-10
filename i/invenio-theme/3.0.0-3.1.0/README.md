# Comparing `tmp/invenio-theme-3.0.0.tar.gz` & `tmp/invenio-theme-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-theme-3.0.0.tar", last modified: Wed Mar 20 15:10:38 2024, max compression
+gzip compressed data, was "dist/invenio-theme-3.1.0.tar", last modified: Wed Apr 10 12:40:00 2024, max compression
```

## Comparing `invenio-theme-3.0.0.tar` & `invenio-theme-3.1.0.tar`

### file list

```diff
@@ -1,479 +1,479 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)    39567 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/static/base.png
--rw-r--r--   0 runner    (1001) docker     (127)    27194 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/static/cover.png
--rw-r--r--   0 runner    (1001) docker     (127)    45698 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/static/error.png
--rw-r--r--   0 runner    (1001) docker     (127)    48992 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/static/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/js/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/js/invenio_theme/base.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/header.scss
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/type.scss
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/base.js
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   256056 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   266158 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot
--rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   268604 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot
--rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77192 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    49064 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   253461 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.variables
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.variables
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.variables
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.variables
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.variables
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.variables
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.variables
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.variables
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.variables
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.variables
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.variables
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.variables
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.variables
--rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.variables
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.variables
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.variables
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.variables
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.variables
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.variables
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.variables
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.variables
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.variables
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.variables
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.variables
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.variables
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.variables
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.variables
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.variables
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.variables
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.variables
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.variables
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.variables
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.variables
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.variables
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.variables
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/header.scss
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/type.scss
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15178 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-120.png
--rw-r--r--   0 runner    (1001) docker     (127)    20939 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-152.png
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-167.png
--rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-180.png
--rw-r--r--   0 runner    (1001) docker     (127)    93062 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/images/invenio-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/static/images/square-placeholder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/401.html
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/403.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/429.html
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/500.html
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/admin_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/admin_layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/body.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/header_frontpage.html
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/header_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/javascript.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/macros/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/macros/messages.html
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/macros/truncate.html
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_admin.html
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_cover.html
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_settings.html
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/401.html
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/403.html
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/429.html
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/500.html
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/body.html
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/javascript.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/invenio_theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20511 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-20 15:10:37.000000 invenio-theme-3.0.0/invenio_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:10:38.000000 invenio-theme-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/tests/test_invenio_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-20 15:10:32.000000 invenio-theme-3.0.0/tests/test_invenio_theme_error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    39567 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/static/base.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27194 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/static/cover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45698 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/static/error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48992 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/static/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/js/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/js/invenio_theme/base.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   256056 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   266158 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   268604 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77192 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    49064 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   253461 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.variables
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.variables
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15178 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-120.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20939 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-152.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-167.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-180.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93062 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/images/invenio-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/static/images/square-placeholder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/401.html
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/429.html
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/admin_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/admin_layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/body.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/header_frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/javascript.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/macros/messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/macros/truncate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_cover.html
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/401.html
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/429.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/body.html
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/javascript.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/invenio_theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20511 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/invenio_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:40:00.000000 invenio-theme-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/tests/test_invenio_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-10 12:39:53.000000 invenio-theme-3.1.0/tests/test_invenio_theme_error_handler.py
```

### Comparing `invenio-theme-3.0.0/.editorconfig` & `invenio-theme-3.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/.github/workflows/pypi-publish.yml` & `invenio-theme-3.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/.github/workflows/tests.yml` & `invenio-theme-3.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/.tx/config` & `invenio-theme-3.1.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/AUTHORS.rst` & `invenio-theme-3.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/CHANGES.rst` & `invenio-theme-3.1.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,443 +9,450 @@
 00000080: 642f 6f72 206d 6f64 6966 7920 6974 0a20  d/or modify it. 
 00000090: 2020 2075 6e64 6572 2074 6865 2074 6572     under the ter
 000000a0: 6d73 206f 6620 7468 6520 4d49 5420 4c69  ms of the MIT Li
 000000b0: 6365 6e73 653b 2073 6565 204c 4943 454e  cense; see LICEN
 000000c0: 5345 2066 696c 6520 666f 7220 6d6f 7265  SE file for more
 000000d0: 2064 6574 6169 6c73 2e0a 0a43 6861 6e67   details...Chang
 000000e0: 6573 0a3d 3d3d 3d3d 3d3d 0a0a 5665 7273  es.=======..Vers
-000000f0: 696f 6e20 332e 302e 3020 2872 656c 6561  ion 3.0.0 (relea
-00000100: 7365 6420 3230 3234 2d30 332d 3139 290a  sed 2024-03-19).
-00000110: 0a2d 2067 6c6f 6261 6c3a 2072 656d 6f76  .- global: remov
-00000120: 6520 6272 6561 6463 7275 6d62 2073 7570  e breadcrumb sup
-00000130: 706f 7274 0a2d 2067 6c6f 6261 6c3a 2069  port.- global: i
-00000140: 6e74 726f 6475 6365 2073 6861 7265 6420  ntroduce shared 
-00000150: 6d65 6e75 0a2d 2067 6c6f 6261 6c3a 2070  menu.- global: p
-00000160: 7265 7061 7261 7469 6f6e 2066 6f72 2063  reparation for c
-00000170: 6f6d 7061 7469 6269 6c69 7479 2077 6974  ompatibility wit
-00000180: 6820 466c 6173 6b20 7632 2e33 2e78 2064  h Flask v2.3.x d
-00000190: 6570 7265 6361 7469 6f6e 730a 2d20 7265  eprecations.- re
-000001a0: 6661 6374 6f72 3a20 6375 7272 656e 745f  factor: current_
-000001b0: 7468 656d 655f 6963 6f6e 7320 7769 7468  theme_icons with
-000001c0: 6f75 7420 6170 706c 6963 6174 696f 6e20  out application 
-000001d0: 636f 6e74 6578 740a 0a56 6572 7369 6f6e  context..Version
-000001e0: 2032 2e35 2e31 3020 2872 656c 6561 7365   2.5.10 (release
-000001f0: 6420 3230 3234 2d30 312d 3238 290a 0a2d  d 2024-01-28)..-
-00000200: 2069 6e73 7461 6c6c 6174 696f 6e3a 2066   installation: f
-00000210: 6978 2073 7068 696e 7820 6465 7065 6e64  ix sphinx depend
-00000220: 656e 6379 0a0a 5665 7273 696f 6e20 322e  ency..Version 2.
-00000230: 352e 3920 2872 656c 6561 7365 6420 3230  5.9 (released 20
-00000240: 3234 2d30 312d 3238 290a 0a2d 2067 6c6f  24-01-28)..- glo
-00000250: 6261 6c3a 2063 6861 6e67 6520 6d61 7468  bal: change math
-00000260: 206f 7065 7261 7469 6f6e 2074 6f20 6265   operation to be
-00000270: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-00000280: 2073 6173 7332 2e30 0a0a 5665 7273 696f   sass2.0..Versio
-00000290: 6e20 322e 352e 3820 2872 656c 6561 7365  n 2.5.8 (release
-000002a0: 6420 3230 3233 2d31 322d 3132 290a 0a2d  d 2023-12-12)..-
-000002b0: 2072 6570 6c61 6365 2063 6b65 6469 746f   replace ckedito
-000002c0: 7220 7769 7468 2074 696e 796d 6365 2064  r with tinymce d
-000002d0: 7565 2074 6f20 6c69 6365 6e73 6520 6973  ue to license is
-000002e0: 7375 650a 0a56 6572 7369 6f6e 2032 2e35  sue..Version 2.5
-000002f0: 2e37 2028 7265 6c65 6173 6564 2032 3032  .7 (released 202
-00000300: 332d 3130 2d32 3629 0a0a 2d20 636f 6d6d  3-10-26)..- comm
-00000310: 756e 6974 7920 6c6f 676f 3a20 6669 7820  unity logo: fix 
-00000320: 7265 6e64 6572 696e 6720 6120 706c 6163  rendering a plac
-00000330: 6568 6f6c 6465 720a 0a56 6572 7369 6f6e  eholder..Version
-00000340: 2032 2e35 2e36 2028 7265 6c65 6173 6564   2.5.6 (released
-00000350: 2032 3032 332d 3130 2d32 3029 0a0a 2d20   2023-10-20)..- 
-00000360: 646f 6e27 7420 6f76 6572 7269 6465 206c  don't override l
-00000370: 696e 6b73 2073 7479 6c65 2069 6e20 666c  inks style in fl
-00000380: 6173 6865 6420 6d65 7373 6167 6573 0a0a  ashed messages..
-00000390: 5665 7273 696f 6e20 322e 352e 3520 2872  Version 2.5.5 (r
-000003a0: 656c 6561 7365 6420 3230 3233 2d30 392d  eleased 2023-09-
-000003b0: 3139 290a 0a2d 2073 7479 6c69 6e67 3a20  19)..- styling: 
-000003c0: 6164 6420 3320 636f 6c75 6d6e 2074 656d  add 3 column tem
-000003d0: 706c 6174 6520 636c 6173 730a 0a56 6572  plate class..Ver
-000003e0: 7369 6f6e 2032 2e35 2e34 2028 7265 6c65  sion 2.5.4 (rele
-000003f0: 6173 6564 2032 3032 332d 3039 2d31 3129  ased 2023-09-11)
-00000400: 0a0a 2d20 7363 7373 3a20 6669 7820 636f  ..- scss: fix co
-00000410: 6d70 6174 6962 696c 6974 7920 7769 7468  mpatibility with
-00000420: 206c 6174 6573 7420 6c65 7373 2076 6572   latest less ver
-00000430: 7369 6f6e 0a0a 5665 7273 696f 6e20 322e  sion..Version 2.
-00000440: 352e 3320 2872 656c 6561 7365 6420 3230  5.3 (released 20
-00000450: 3233 2d30 382d 3038 290a 0a2d 2073 7479  23-08-08)..- sty
-00000460: 6c65 7368 6565 7473 3a20 6164 6420 7072  lesheets: add pr
-00000470: 6566 6f72 6d61 7474 6564 2074 6167 2073  eformatted tag s
-00000480: 7479 6c69 6e67 2066 6f6e 740a 0a56 6572  tyling font..Ver
-00000490: 7369 6f6e 2032 2e35 2e32 2028 7265 6c65  sion 2.5.2 (rele
-000004a0: 6173 6564 2032 3032 332d 3038 2d31 3429  ased 2023-08-14)
-000004b0: 0a0a 2d20 696e 7374 616c 6c61 7469 6f6e  ..- installation
-000004c0: 3a20 7069 6e20 466c 6173 6b2d 4d65 6e75  : pin Flask-Menu
-000004d0: 2074 6f20 6060 3c76 312e 302e 3060 602e   to ``<v1.0.0``.
-000004e0: 0a0a 5665 7273 696f 6e20 322e 352e 3120  ..Version 2.5.1 
-000004f0: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
-00000500: 382d 3134 290a 0a2d 2074 6865 6d65 3a20  8-14)..- theme: 
-00000510: 6275 6766 6978 2074 6f20 6465 6372 6561  bugfix to decrea
-00000520: 7365 207a 2d69 6e64 6578 2076 616c 7565  se z-index value
-00000530: 0a0a 5665 7273 696f 6e20 322e 352e 3020  ..Version 2.5.0 
-00000540: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
-00000550: 382d 3039 290a 0a2d 2074 6865 6d65 3a20  8-09)..- theme: 
-00000560: 6164 6420 7574 696c 6974 7920 636c 6173  add utility clas
-00000570: 7365 730a 0a56 6572 7369 6f6e 2032 2e34  ses..Version 2.4
-00000580: 2e30 2028 7265 6c65 6173 6564 2032 3032  .0 (released 202
-00000590: 332d 3038 2d30 3229 0a0a 2d20 7468 656d  3-08-02)..- them
-000005a0: 653a 2061 6464 2073 6f6d 6520 6765 6e65  e: add some gene
-000005b0: 7261 6c20 636c 6173 7365 7320 616e 6420  ral classes and 
-000005c0: 6669 7865 7320 616c 6967 6e6d 656e 7420  fixes alignment 
-000005d0: 666f 7220 6c61 6265 6c65 6420 666c 7569  for labeled flui
-000005e0: 6420 6275 7474 6f6e 730a 0a56 6572 7369  d buttons..Versi
-000005f0: 6f6e 2032 2e33 2e30 2028 7265 6c65 6173  on 2.3.0 (releas
-00000600: 6564 2032 3032 332d 3037 2d33 3129 0a0a  ed 2023-07-31)..
-00000610: 2d20 7365 7474 696e 6773 2070 6167 653a  - settings page:
-00000620: 2049 6d70 726f 7665 2074 656d 706c 6174   Improve templat
-00000630: 6520 666f 7220 6131 3179 0a0a 5665 7273  e for a11y..Vers
-00000640: 696f 6e20 322e 322e 3020 2872 656c 6561  ion 2.2.0 (relea
-00000650: 7365 6420 3230 3233 2d30 372d 3236 290a  sed 2023-07-26).
-00000660: 0a2d 2074 6865 6d65 3a20 6164 6420 6765  .- theme: add ge
-00000670: 6e65 7261 6c20 7374 796c 6520 696d 7072  neral style impr
-00000680: 6f76 656d 656e 7473 0a0a 5665 7273 696f  ovements..Versio
-00000690: 6e20 322e 312e 3320 2872 656c 6561 7365  n 2.1.3 (release
-000006a0: 6420 3230 3233 2d30 372d 3234 290a 0a2d  d 2023-07-24)..-
-000006b0: 206d 6573 7361 6765 733a 2061 6464 207a   messages: add z
-000006c0: 2d69 6e64 6578 0a0a 5665 7273 696f 6e20  -index..Version 
-000006d0: 322e 312e 3220 2872 656c 6561 7365 6420  2.1.2 (released 
-000006e0: 3230 3233 2d30 342d 3132 290a 0a2d 2061  2023-04-12)..- a
-000006f0: 6464 2066 6c65 7820 7574 696c 6974 7920  dd flex utility 
-00000700: 636c 6173 7365 730a 2d20 6164 6420 7465  classes.- add te
-00000710: 7874 2073 697a 6573 2063 6c61 7373 6573  xt sizes classes
-00000720: 0a0a 5665 7273 696f 6e20 322e 312e 3120  ..Version 2.1.1 
-00000730: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
-00000740: 342d 3036 290a 0a2d 2061 6464 2064 6973  4-06)..- add dis
-00000750: 706c 6179 2075 7469 6c69 7479 2063 6c61  play utility cla
-00000760: 7373 6573 0a0a 5665 7273 696f 6e20 322e  sses..Version 2.
-00000770: 312e 3020 2872 656c 6561 7365 6420 3230  1.0 (released 20
-00000780: 3233 2d30 332d 3238 290a 0a2d 2061 6464  23-03-28)..- add
-00000790: 2067 6c6f 6261 6c20 7574 696c 6974 7920   global utility 
-000007a0: 7374 796c 696e 6720 636c 6173 7365 730a  styling classes.
-000007b0: 0a56 6572 7369 6f6e 2032 2e30 2e31 2028  .Version 2.0.1 (
-000007c0: 7265 6c65 6173 6564 2032 3032 332d 3033  released 2023-03
-000007d0: 2d30 3929 0a0a 2d20 6669 7820 7374 796c  -09)..- fix styl
-000007e0: 696e 6720 666f 7220 6275 7474 6f6e 730a  ing for buttons.
-000007f0: 2d20 6d6f 7665 2067 6c6f 6261 6c20 636c  - move global cl
-00000800: 6173 7320 666f 7220 6175 746f 2067 7269  ass for auto gri
-00000810: 640a 0a56 6572 7369 6f6e 2032 2e30 2e30  d..Version 2.0.0
-00000820: 2028 7265 6c65 6173 6564 2032 3032 332d   (released 2023-
-00000830: 3032 2d32 3829 0a0a 2d20 6472 6f70 2070  02-28)..- drop p
-00000840: 7974 686f 6e20 322e 3720 7375 7070 6f72  ython 2.7 suppor
-00000850: 740a 2d20 7265 6d6f 7665 2066 6c61 736b  t.- remove flask
-00000860: 5f62 6162 656c 6578 2069 6d70 6f72 7473  _babelex imports
-00000870: 0a2d 2075 7067 7261 6465 2069 6e76 656e  .- upgrade inven
-00000880: 696f 5f69 3138 6e0a 0a56 6572 7369 6f6e  io_i18n..Version
-00000890: 2031 2e34 2e38 2028 7265 6c65 6173 6564   1.4.8 (released
-000008a0: 2032 3032 332d 3032 2d30 3729 0a0a 2d20   2023-02-07)..- 
-000008b0: 7468 656d 653a 2061 6464 2061 7574 6f2d  theme: add auto-
-000008c0: 636f 6c75 6d6e 2d67 7269 6420 636c 6173  column-grid clas
-000008d0: 730a 0a56 6572 7369 6f6e 2031 2e34 2e37  s..Version 1.4.7
-000008e0: 2028 7265 6c65 6173 6564 2032 3032 332d   (released 2023-
-000008f0: 3031 2d30 3529 0a0a 2d20 6164 6420 7472  01-05)..- add tr
-00000900: 756e 6361 7465 206c 696e 6573 2073 7479  uncate lines sty
-00000910: 6c65 730a 0a56 6572 7369 6f6e 2031 2e34  les..Version 1.4
-00000920: 2e36 2028 7265 6c65 6173 6564 2032 3032  .6 (released 202
-00000930: 322d 3132 2d30 3829 0a0a 2d20 6669 7820  2-12-08)..- fix 
-00000940: 7374 796c 696e 6720 666f 7220 696e 6c69  styling for inli
-00000950: 6e65 2063 6c61 7373 2c20 6166 6665 6374  ne class, affect
-00000960: 696e 6720 666f 726d 2066 6965 6c64 730a  ing form fields.
-00000970: 0a56 6572 7369 6f6e 2031 2e34 2e35 2028  .Version 1.4.5 (
-00000980: 7265 6c65 6173 6564 2032 3032 322d 3132  released 2022-12
-00000990: 2d30 3129 0a0a 2d20 6669 7820 7365 6172  -01)..- fix sear
-000009a0: 6368 2072 6573 756c 7420 6974 656d 2073  ch result item s
-000009b0: 7479 6c69 6e67 0a2d 2061 6464 2067 6c6f  tyling.- add glo
-000009c0: 6261 6c20 6265 6861 7669 6f75 7220 636c  bal behaviour cl
-000009d0: 6173 7365 730a 2d20 6164 6420 706c 6163  asses.- add plac
-000009e0: 6568 6f6c 6465 7220 696d 6167 6520 6861  eholder image ha
-000009f0: 6e64 6c65 0a0a 5665 7273 696f 6e20 312e  ndle..Version 1.
-00000a00: 342e 3420 2872 656c 6561 7365 6420 3230  4.4 (released 20
-00000a10: 3232 2d31 312d 3138 290a 0a2d 2041 6464  22-11-18)..- Add
-00000a20: 2070 756c 6c65 6420 7472 616e 736c 6174   pulled translat
-00000a30: 696f 6e73 0a0a 5665 7273 696f 6e20 312e  ions..Version 1.
-00000a40: 342e 3320 2872 656c 6561 7365 6420 3230  4.3 (released 20
-00000a50: 3232 2d31 312d 3033 290a 0a2d 2061 6464  22-11-03)..- add
-00000a60: 2073 7479 6c69 6e67 2066 6f72 2064 726f   styling for dro
-00000a70: 7064 6f77 6e20 6d65 6e75 2069 7465 6d73  pdown menu items
-00000a80: 0a2d 2066 6978 206d 6973 7369 6e67 204d  .- fix missing M
-00000a90: 6564 6961 2063 6f6d 706f 6e65 6e74 2072  edia component r
-00000aa0: 616e 6765 0a0a 5665 7273 696f 6e20 312e  ange..Version 1.
-00000ab0: 342e 3220 2872 656c 6561 7365 6420 3230  4.2 (released 20
-00000ac0: 3232 2d31 302d 3236 290a 0a2d 2061 6464  22-10-26)..- add
-00000ad0: 204d 6564 6961 2074 6f20 7375 7070 6f72   Media to suppor
-00000ae0: 7420 7265 7370 6f6e 7369 7665 2072 6561  t responsive rea
-00000af0: 6374 2063 6f6d 706f 6e65 6e74 730a 0a56  ct components..V
-00000b00: 6572 7369 6f6e 2031 2e34 2e31 2028 7265  ersion 1.4.1 (re
-00000b10: 6c65 6173 6564 2032 3032 322d 3130 2d31  leased 2022-10-1
-00000b20: 3029 0a0a 2d20 6275 6d70 2053 656d 616e  0)..- bump Seman
-00000b30: 7469 6355 490a 0a56 6572 7369 6f6e 2031  ticUI..Version 1
-00000b40: 2e34 2e30 2028 7265 6c65 6173 6564 2032  .4.0 (released 2
-00000b50: 3032 322d 3130 2d30 3529 0a0a 2d20 6368  022-10-05)..- ch
-00000b60: 616e 6765 2067 6c6f 6261 6c20 666f 6e74  ange global font
-00000b70: 2074 6f20 4c61 746f 0a0a 5665 7273 696f   to Lato..Versio
-00000b80: 6e20 312e 332e 3331 2028 7265 6c65 6173  n 1.3.31 (releas
-00000b90: 6564 2032 3032 322d 3130 2d30 3529 0a0a  ed 2022-10-05)..
-00000ba0: 2d20 6164 6420 6d69 7373 696e 6720 7468  - add missing th
-00000bb0: 656d 6520 7661 7269 6162 6c65 730a 0a56  eme variables..V
-00000bc0: 6572 7369 6f6e 2031 2e33 2e33 3020 2872  ersion 1.3.30 (r
-00000bd0: 656c 6561 7365 6420 3230 3232 2d30 392d  eleased 2022-09-
-00000be0: 3236 290a 0a2d 2061 6464 2073 7479 6c69  26)..- add styli
-00000bf0: 6e67 2074 6f20 6164 6d69 6e69 7374 7261  ng to administra
-00000c00: 7469 6f6e 2064 6173 6862 6f61 7264 2070  tion dashboard p
-00000c10: 6167 650a 0a56 6572 7369 6f6e 2031 2e33  age..Version 1.3
-00000c20: 2e32 3920 2872 656c 6561 7365 6420 3230  .29 (released 20
-00000c30: 3232 2d30 392d 3232 290a 0a2d 2061 6464  22-09-22)..- add
-00000c40: 2061 646d 696e 6973 7472 6174 696f 6e20   administration 
-00000c50: 7061 6e65 6c20 7374 796c 696e 670a 2d20  panel styling.- 
-00000c60: 6164 6420 7472 616e 736c 6174 696f 6e20  add translation 
-00000c70: 776f 726b 666c 6f77 0a0a 5665 7273 696f  workflow..Versio
-00000c80: 6e20 312e 332e 3238 2028 7265 6c65 6173  n 1.3.28 (releas
-00000c90: 6564 2032 3032 322d 3037 2d30 3829 0a0a  ed 2022-07-08)..
-00000ca0: 2d20 6164 6420 7374 796c 696e 6720 636c  - add styling cl
-00000cb0: 6173 7365 7320 7769 7468 2061 6374 696f  asses with actio
-00000cc0: 6e20 636f 6c6f 7220 636f 6469 6e67 0a0a  n color coding..
-00000cd0: 5665 7273 696f 6e20 312e 332e 3237 2028  Version 1.3.27 (
-00000ce0: 7265 6c65 6173 6564 2032 3032 322d 3037  released 2022-07
-00000cf0: 2d30 3729 0a0a 2d20 6669 7820 6a71 7565  -07)..- fix jque
-00000d00: 7279 2072 6566 6572 656e 6365 0a0a 5665  ry reference..Ve
-00000d10: 7273 696f 6e20 312e 332e 3236 2028 7265  rsion 1.3.26 (re
-00000d20: 6c65 6173 6564 2032 3032 322d 3037 2d30  leased 2022-07-0
-00000d30: 3729 0a0a 2d20 6164 6420 696d 6167 6520  7)..- add image 
-00000d40: 706c 6163 6568 6f6c 6465 7220 6f6e 206c  placeholder on l
-00000d50: 6f61 6420 6572 726f 720a 0a56 6572 7369  oad error..Versi
-00000d60: 6f6e 2031 2e33 2e32 3520 2872 656c 6561  on 1.3.25 (relea
-00000d70: 7365 6420 3230 3232 2d30 362d 3237 290a  sed 2022-06-27).
-00000d80: 0a2d 2061 6464 2047 6572 6d61 6e20 7472  .- add German tr
-00000d90: 616e 736c 6174 696f 6e73 0a2d 2066 6978  anslations.- fix
-00000da0: 2064 726f 7064 6f77 6e20 7363 726f 6c6c   dropdown scroll
-00000db0: 206d 6973 616c 6967 6e6d 656e 740a 0a56   misalignment..V
-00000dc0: 6572 7369 6f6e 2031 2e33 2e32 3420 2872  ersion 1.3.24 (r
-00000dd0: 656c 6561 7365 6420 3230 3232 2d30 352d  eleased 2022-05-
-00000de0: 3233 290a 0a2d 2061 6464 2067 6c6f 6261  23)..- add globa
-00000df0: 6c20 4353 5320 636c 6173 7365 7320 666f  l CSS classes fo
-00000e00: 7220 6d61 7267 696e 7320 6175 746f 0a0a  r margins auto..
-00000e10: 5665 7273 696f 6e20 312e 332e 3233 2028  Version 1.3.23 (
-00000e20: 7265 6c65 6173 6564 2032 3032 322d 3035  released 2022-05
-00000e30: 2d31 3929 0a0a 2d20 6164 6420 6163 6365  -19)..- add acce
-00000e40: 7373 6962 696c 6974 7920 746f 2075 692d  ssibility to ui-
-00000e50: 6163 636f 7264 696f 6e73 0a0a 5665 7273  accordions..Vers
-00000e60: 696f 6e20 312e 332e 3232 2028 7265 6c65  ion 1.3.22 (rele
-00000e70: 6173 6564 2032 3032 322d 3034 2d32 3129  ased 2022-04-21)
-00000e80: 0a0a 2d20 696d 7072 6f76 6520 7365 6d61  ..- improve sema
-00000e90: 6e74 6963 2073 7479 6c69 6e67 206f 6620  ntic styling of 
-00000ea0: 4d79 2061 6363 6f75 6e74 2070 6167 650a  My account page.
-00000eb0: 0a56 6572 7369 6f6e 2031 2e33 2e32 3120  .Version 1.3.21 
-00000ec0: 2872 656c 6561 7365 6420 3230 3232 2d30  (released 2022-0
-00000ed0: 332d 3239 290a 0a2d 2066 6978 2068 746d  3-29)..- fix htm
-00000ee0: 6c20 7461 6773 2069 6e20 7465 6d70 6c61  l tags in templa
-00000ef0: 7465 730a 0a56 6572 7369 6f6e 2031 2e33  tes..Version 1.3
-00000f00: 2e32 3020 2872 656c 6561 7365 6420 3230  .20 (released 20
-00000f10: 3232 2d30 332d 3137 290a 0a2d 2072 6566  22-03-17)..- ref
-00000f20: 6163 746f 7220 7061 6765 2074 656d 706c  actor page templ
-00000f30: 6174 650a 2d20 6164 6420 7365 6d61 6e74  ate.- add semant
-00000f40: 6963 2075 6920 696e 7665 6e69 6f20 7061  ic ui invenio pa
-00000f50: 636b 6167 6564 2074 6865 6d65 2063 6f6e  ckaged theme con
-00000f60: 6669 6775 7261 7469 6f6e 0a2d 2065 7874  figuration.- ext
-00000f70: 656e 6420 7574 696c 7320 4353 5320 636c  end utils CSS cl
-00000f80: 6173 7365 730a 0a56 6572 7369 6f6e 2031  asses..Version 1
-00000f90: 2e33 2e31 3920 2872 656c 6561 7365 6420  .3.19 (released 
-00000fa0: 3230 3232 2d30 332d 3034 290a 0a2d 2041  2022-03-04)..- A
-00000fb0: 6464 2061 2072 6575 7361 626c 6520 4a69  dd a reusable Ji
-00000fc0: 6e6a 6120 6d61 6372 6f20 746f 2074 7275  nja macro to tru
-00000fd0: 6e63 6174 6520 6c6f 6e67 2074 6578 742e  ncate long text.
-00000fe0: 0a0a 5665 7273 696f 6e20 312e 332e 3138  ..Version 1.3.18
-00000ff0: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-00001000: 3033 2d30 3129 0a0a 2d20 5265 7665 7274  03-01)..- Revert
-00001010: 2066 6f6e 7420 6261 636b 2074 6f20 6465   font back to de
-00001020: 6661 756c 7420 7361 6e73 2d73 6172 6966  fault sans-sarif
-00001030: 2066 6f6e 7420 696e 7374 6561 6420 6f66   font instead of
-00001040: 204c 6174 6f2e 0a0a 5665 7273 696f 6e20   Lato...Version 
-00001050: 312e 332e 3137 2028 7265 6c65 6173 6564  1.3.17 (released
-00001060: 2032 3032 322d 3032 2d32 3829 0a0a 2d20   2022-02-28)..- 
-00001070: 4164 6473 2066 6176 6963 6f6e 0a2d 2046  Adds favicon.- F
-00001080: 6978 2069 7373 7565 2077 6974 6820 666c  ix issue with fl
-00001090: 6173 6820 6d65 7373 6167 6520 6f6e 206c  ash message on l
-000010a0: 6f67 696e 2070 6167 6520 6e6f 7420 6265  ogin page not be
-000010b0: 696e 6720 7369 6465 2074 6f20 7369 6465  ing side to side
-000010c0: 2e0a 0a56 6572 7369 6f6e 2031 2e33 2e31  ...Version 1.3.1
-000010d0: 3620 2872 656c 6561 7365 6420 3230 3232  6 (released 2022
-000010e0: 2d30 322d 3137 290a 0a2d 2041 6464 2063  -02-17)..- Add c
-000010f0: 6f6d 6d6f 6e20 6073 7175 6172 652d 706c  ommon `square-pl
-00001100: 6163 6568 6f6c 6465 722e 706e 6760 2069  aceholder.png` i
-00001110: 6d61 6765 2066 6f72 2067 656e 6572 616c  mage for general
-00001120: 2075 7365 2e0a 0a56 6572 7369 6f6e 2031   use...Version 1
-00001130: 2e33 2e31 3520 2872 656c 6561 7365 6420  .3.15 (released 
-00001140: 3230 3232 2d30 322d 3137 290a 0a2d 2052  2022-02-17)..- R
-00001150: 656d 6f76 6520 6375 7374 6f6d 206d 6172  emove custom mar
-00001160: 6769 6e20 6672 6f6d 2063 6c61 7373 6573  gin from classes
-00001170: 2074 6f20 696d 7072 6f76 6520 4353 5320   to improve CSS 
-00001180: 6f76 6572 7269 6461 6269 6c69 7479 2e0a  overridability..
-00001190: 0a56 6572 7369 6f6e 2031 2e33 2e31 3420  .Version 1.3.14 
-000011a0: 2872 656c 6561 7365 6420 3230 3232 2d30  (released 2022-0
-000011b0: 322d 3136 290a 0a2d 2046 6978 2069 7373  2-16)..- Fix iss
-000011c0: 7565 2077 6974 6820 4c61 746f 2066 6f6e  ue with Lato fon
-000011d0: 7420 6e6f 7420 6265 696e 6720 6c6f 6164  t not being load
-000011e0: 6564 2069 6e20 5365 6d61 6e74 6963 2055  ed in Semantic U
-000011f0: 4920 7468 656d 652e 0a2d 2053 6574 7320  I theme..- Sets 
-00001200: 5365 6d61 6e74 6963 2055 4920 406d 7574  Semantic UI @mut
-00001210: 6564 5465 7874 436f 6c6f 722e 0a0a 5665  edTextColor...Ve
-00001220: 7273 696f 6e20 312e 332e 3133 2028 7265  rsion 1.3.13 (re
-00001230: 6c65 6173 6564 2032 3032 322d 3032 2d31  leased 2022-02-1
-00001240: 3629 0a0a 2d20 456e 7375 7265 2063 6f6d  6)..- Ensure com
-00001250: 7069 6c65 6420 7472 616e 736c 6174 696f  piled translatio
-00001260: 6e20 6d65 7373 6167 6520 6361 7461 6c6f  n message catalo
-00001270: 6773 2061 7265 2069 6e63 6c75 6465 6420  gs are included 
-00001280: 696e 2074 6865 0a20 2064 6973 7472 6962  in the.  distrib
-00001290: 7574 696f 6e73 2075 706c 6f61 6465 6420  utions uploaded 
-000012a0: 6f6e 2050 7950 492e 0a0a 5665 7273 696f  on PyPI...Versio
-000012b0: 6e20 312e 332e 3132 2028 7265 6c65 6173  n 1.3.12 (releas
-000012c0: 6564 2032 3032 322d 3032 2d31 3429 0a0a  ed 2022-02-14)..
-000012d0: 2d20 4669 7865 7320 4131 3179 2069 7373  - Fixes A11y iss
-000012e0: 7565 2077 6974 6820 7468 6520 636c 6f73  ue with the clos
-000012f0: 6520 6275 7474 6f6e 2069 6e20 666c 6173  e button in flas
-00001300: 6820 6d65 7373 6167 6573 2e0a 0a56 6572  h messages...Ver
-00001310: 7369 6f6e 2031 2e33 2e31 3120 2872 656c  sion 1.3.11 (rel
-00001320: 6561 7365 6420 3230 3232 2d30 322d 3038  eased 2022-02-08
-00001330: 290a 0a2d 2041 6464 7320 6d61 7267 696e  )..- Adds margin
-00001340: 2067 656e 6572 6174 6f72 2e0a 2d20 4164   generator..- Ad
-00001350: 6473 2041 3131 7920 7061 6765 206c 616e  ds A11y page lan
-00001360: 646d 6172 6b73 2e0a 0a56 6572 7369 6f6e  dmarks...Version
-00001370: 2031 2e33 2e31 3020 2872 656c 6561 7365   1.3.10 (release
-00001380: 6420 3230 3231 2d31 312d 3233 290a 0a2d  d 2021-11-23)..-
-00001390: 2057 6562 2061 6363 6573 7369 6269 6c69   Web accessibili
-000013a0: 7479 2066 6978 2e0a 0a56 6572 7369 6f6e  ty fix...Version
-000013b0: 2031 2e33 2e39 2028 7265 6c65 6173 6564   1.3.9 (released
-000013c0: 2032 3032 312d 3037 2d31 3229 0a0a 2d20   2021-07-12)..- 
-000013d0: 4164 6473 2067 6572 6d61 6e20 7472 616e  Adds german tran
-000013e0: 736c 6174 696f 6e73 0a0a 5665 7273 696f  slations..Versio
-000013f0: 6e20 312e 332e 3820 2872 656c 6561 7365  n 1.3.8 (release
-00001400: 6420 3230 3231 2d30 322d 3130 290a 0a2d  d 2021-02-10)..-
-00001410: 2041 6464 7320 6272 616e 6420 636f 6c6f   Adds brand colo
-00001420: 7220 746f 206d 656e 7520 6974 656d 730a  r to menu items.
-00001430: 0a56 6572 7369 6f6e 2031 2e33 2e37 2028  .Version 1.3.7 (
-00001440: 7265 6c65 6173 6564 2032 3032 312d 3031  released 2021-01
-00001450: 2d32 3529 0a0a 2d20 4164 6473 2062 7261  -25)..- Adds bra
-00001460: 6e64 2063 6f6c 6f72 2069 6e20 7365 676d  nd color in segm
-00001470: 656e 7473 0a0a 5665 7273 696f 6e20 312e  ents..Version 1.
-00001480: 332e 3620 2872 656c 6561 7365 6420 3230  3.6 (released 20
-00001490: 3231 2d30 312d 3034 290a 0a2d 2041 6464  21-01-04)..- Add
-000014a0: 7320 606c 696e 6b60 2074 6865 6d65 2069  s `link` theme i
-000014b0: 636f 6e0a 2d20 4669 7865 7320 7769 6c64  con.- Fixes wild
-000014c0: 6361 7264 2069 636f 6e20 7265 736f 6c75  card icon resolu
-000014d0: 7469 6f6e 0a0a 5665 7273 696f 6e20 312e  tion..Version 1.
-000014e0: 332e 3520 2872 656c 6561 7365 6420 3230  3.5 (released 20
-000014f0: 3230 2d31 322d 3137 290a 0a2d 2046 6978  20-12-17)..- Fix
-00001500: 6573 2063 6865 636b 626f 782e 6f76 6572  es checkbox.over
-00001510: 7269 6465 7320 696e 2060 696e 7665 6e69  rides in `inveni
-00001520: 6f60 2053 5549 2070 6163 6b61 6765 6420  o` SUI packaged 
-00001530: 7468 656d 652e 0a0a 5665 7273 696f 6e20  theme...Version 
-00001540: 312e 332e 3420 2872 656c 6561 7365 6420  1.3.4 (released 
-00001550: 3230 3230 2d31 322d 3137 290a 0a2d 2041  2020-12-17)..- A
-00001560: 6464 7320 6120 6675 6c6c 2022 696e 7665  dds a full "inve
-00001570: 6e69 6f22 2053 656d 616e 7469 6320 5549  nio" Semantic UI
-00001580: 2070 6163 6b61 6765 6420 7468 656d 6520   packaged theme 
-00001590: 736f 2077 6520 6361 6e20 6561 7369 6572  so we can easier
-000015a0: 2063 7573 746f 6d69 7a65 0a20 206c 6179   customize.  lay
-000015b0: 6f75 7420 696e 2074 6865 2066 7574 7572  out in the futur
-000015c0: 652e 0a0a 2d20 4d6f 7665 7320 7468 656d  e...- Moves them
-000015d0: 652e 636f 6e66 6967 2074 6f20 7468 656d  e.config to them
-000015e0: 652e 636f 6e66 6967 2e65 7861 6d70 6c65  e.config.example
-000015f0: 2061 6e64 2061 6464 7320 6120 6e6f 7465   and adds a note
-00001600: 2074 6f20 6d61 6b65 2069 740a 2020 636c   to make it.  cl
-00001610: 6561 7220 7468 6520 6669 6c65 2069 7320  ear the file is 
-00001620: 6e6f 7420 6163 7475 616c 6c79 2075 7365  not actually use
-00001630: 642c 2062 7574 2069 7320 6a75 7374 2061  d, but is just a
-00001640: 6e20 6578 616d 706c 652e 0a0a 2d20 4164  n example...- Ad
-00001650: 6473 2068 656c 7065 7220 746f 6f6c 2066  ds helper tool f
-00001660: 6f72 2073 7570 706f 7274 696e 6720 7468  or supporting th
-00001670: 656d 6520 6465 7065 6e64 656e 7420 6963  eme dependent ic
-00001680: 6f6e 732e 0a0a 2d20 4669 7865 7320 6d61  ons...- Fixes ma
-00001690: 6e79 206d 696e 6f72 2073 7479 6c69 6e67  ny minor styling
-000016a0: 2069 7373 7565 7320 7375 6368 2061 7320   issues such as 
-000016b0: 616c 6967 6e6d 656e 7473 2c20 6275 7474  alignments, butt
-000016c0: 6f6e 206c 6f63 6174 696f 6e73 2c0a 2020  on locations,.  
-000016d0: 6772 6964 732e 0a0a 5665 7273 696f 6e20  grids...Version 
-000016e0: 312e 332e 3320 2872 656c 6561 7365 6420  1.3.3 (released 
-000016f0: 3230 3230 2d31 322d 3131 290a 0a2d 2049  2020-12-11)..- I
-00001700: 6e69 7469 616c 697a 6573 2073 656d 616e  nitializes seman
-00001710: 7469 6355 4920 6163 636f 7264 696f 6e20  ticUI accordion 
-00001720: 636f 6d70 6f6e 656e 7473 2e0a 0a56 6572  components...Ver
-00001730: 7369 6f6e 2031 2e33 2e32 2028 7265 6c65  sion 1.3.2 (rele
-00001740: 6173 6564 2032 3032 302d 3132 2d31 3129  ased 2020-12-11)
-00001750: 0a0a 2d20 5570 6461 7465 7320 7468 6520  ..- Updates the 
-00001760: 496e 7665 6e69 6f20 6c6f 676f 2061 6e64  Invenio logo and
-00001770: 2072 656d 6f76 6520 6f75 7464 6174 6564   remove outdated
-00001780: 2076 6572 7369 6f6e 732e 0a2d 2046 6978   versions..- Fix
-00001790: 6573 2074 6865 2064 726f 7064 6f77 6e20  es the dropdown 
-000017a0: 746f 2077 6f72 6b20 6f6e 2074 6865 2075  to work on the u
-000017b0: 7365 7220 7072 6f66 696c 6520 7061 6765  ser profile page
-000017c0: 2e0a 0a56 6572 7369 6f6e 2031 2e33 2e31  ...Version 1.3.1
-000017d0: 2028 7265 6c65 6173 6564 2032 3032 302d   (released 2020-
-000017e0: 3132 2d30 3929 0a0a 2d20 4d69 6e6f 7220  12-09)..- Minor 
-000017f0: 6669 7820 666f 7220 5365 6d61 6e74 6963  fix for Semantic
-00001800: 5549 2064 726f 7064 6f77 6e73 0a0a 5665  UI dropdowns..Ve
-00001810: 7273 696f 6e20 312e 332e 3020 2872 656c  rsion 1.3.0 (rel
-00001820: 6561 7365 6420 3230 3230 2d31 322d 3039  eased 2020-12-09
-00001830: 290a 0a2d 204d 616a 6f72 3a20 4e65 7720  )..- Major: New 
-00001840: 5365 6d61 6e74 6963 5549 2074 6865 6d65  SemanticUI theme
-00001850: 2068 6173 2062 6565 6e20 696e 7465 6772   has been integr
-00001860: 6174 6564 2e20 5468 6520 426f 6f74 7374  ated. The Bootst
-00001870: 7261 7020 3320 7468 656d 6520 7374 696c  rap 3 theme stil
-00001880: 6c0a 2020 6578 6973 7473 2e20 5468 6973  l.  exists. This
-00001890: 2063 6861 6e67 6520 6465 7065 6e64 7320   change depends 
-000018a0: 6f6e 2074 6865 206c 6174 6573 7420 7265  on the latest re
-000018b0: 6c65 6173 6564 2049 6e76 656e 696f 2d41  leased Invenio-A
-000018c0: 7373 6574 7320 7768 6963 680a 2020 6164  ssets which.  ad
-000018d0: 6473 2073 7570 706f 7274 7320 666f 7220  ds supports for 
-000018e0: 6d75 6c74 6970 6c65 2055 4920 6672 616d  multiple UI fram
-000018f0: 6577 6f72 6b73 2e0a 0a2d 2041 6464 7320  eworks...- Adds 
-00001900: 7375 7070 6f72 7420 666f 7220 6479 6e61  support for dyna
-00001910: 6d69 6320 6c6f 6164 696e 6720 6f66 2074  mic loading of t
-00001920: 656d 706c 6174 6573 2066 6f72 2052 6561  emplates for Rea
-00001930: 6374 2d4f 7665 7272 6964 6162 6c65 2e0a  ct-Overridable..
-00001940: 0a2d 2042 6163 6b77 6172 6473 2069 6e63  .- Backwards inc
-00001950: 6f6d 7061 7469 626c 653a 2054 6865 206f  ompatible: The o
-00001960: 6c64 2d73 7479 6c65 2046 6c61 736b 2d41  ld-style Flask-A
-00001970: 7373 6574 2062 756e 646c 6573 2077 6173  sset bundles was
-00001980: 2072 656d 6f76 6564 2028 7468 6573 650a   removed (these.
-00001990: 2020 6275 6e64 6c65 7320 7765 7265 2064    bundles were d
-000019a0: 6570 7265 6361 7465 6420 696e 2049 6e76  eprecated in Inv
-000019b0: 656e 696f 2076 332e 3129 2e0a 0a2d 2041  enio v3.1)...- A
-000019c0: 6464 7320 5475 726b 6973 6820 7472 616e  dds Turkish tran
-000019d0: 736c 6174 696f 6e73 2e0a 0a56 6572 7369  slations...Versi
-000019e0: 6f6e 2031 2e32 2e30 2028 7265 6c65 6173  on 1.2.0 (releas
-000019f0: 6564 2032 3032 302d 3033 2d32 3029 0a0a  ed 2020-03-20)..
-00001a00: 2d20 5265 706c 6163 6573 2046 6c61 736b  - Replaces Flask
-00001a10: 2064 6570 656e 6465 6e63 7920 7769 7468   dependency with
-00001a20: 2060 6069 6e76 656e 696f 2d62 6173 6560   ``invenio-base`
-00001a30: 602e 0a0a 5665 7273 696f 6e20 312e 312e  `...Version 1.1.
-00001a40: 3420 2872 656c 6561 7365 6420 3230 3139  4 (released 2019
-00001a50: 2d30 372d 3232 290a 0a2d 2049 6e74 726f  -07-22)..- Intro
-00001a60: 6475 6365 2068 616e 646c 696e 6720 6f66  duce handling of
-00001a70: 2074 6865 2065 7272 6f72 2034 3239 2e0a   the error 429..
-00001a80: 0a56 6572 7369 6f6e 2031 2e31 2e33 2028  .Version 1.1.3 (
-00001a90: 7265 6c65 6173 6564 2032 3031 392d 3033  released 2019-03
-00001aa0: 2d31 3329 0a0a 2d20 5265 7374 7275 6374  -13)..- Restruct
-00001ab0: 7572 6520 5343 5353 2066 696c 6573 2c20  ure SCSS files, 
-00001ac0: 696e 206f 7264 6572 2074 6f20 616c 6c6f  in order to allo
-00001ad0: 7720 6561 7369 6572 2063 7573 746f 6d69  w easier customi
-00001ae0: 7a61 7469 6f6e 2061 6e64 2065 7874 656e  zation and exten
-00001af0: 7369 6f6e 0a20 2069 6e20 6f76 6572 6c61  sion.  in overla
-00001b00: 7973 2e0a 0a56 6572 7369 6f6e 2031 2e31  ys...Version 1.1
-00001b10: 2e32 2028 7265 6c65 6173 6564 2032 3031  .2 (released 201
-00001b20: 392d 3032 2d31 3529 0a0a 2d20 5570 6772  9-02-15)..- Upgr
-00001b30: 6164 6564 206d 6f6d 656e 7420 746f 2032  aded moment to 2
-00001b40: 2e32 332e 300a 0a56 6572 7369 6f6e 2031  .23.0..Version 1
-00001b50: 2e31 2e31 2028 7265 6c65 6173 6564 2032  .1.1 (released 2
-00001b60: 3031 382d 3132 2d30 3529 0a0a 2d20 4669  018-12-05)..- Fi
-00001b70: 7865 7320 6973 7375 6573 2077 6974 6820  xes issues with 
-00001b80: 7765 6270 6163 6b20 616e 6420 7468 6520  webpack and the 
-00001b90: 4164 6d69 6e4c 5445 2074 6865 6d65 2e0a  AdminLTE theme..
-00001ba0: 0a56 6572 7369 6f6e 2031 2e31 2e30 2028  .Version 1.1.0 (
-00001bb0: 7265 6c65 6173 6564 2032 3031 382d 3131  released 2018-11
-00001bc0: 2d30 3629 0a0a 2d20 496e 7472 6f64 7563  -06)..- Introduc
-00001bd0: 6520 7765 6270 6163 6b20 7375 7070 6f72  e webpack suppor
-00001be0: 742e 0a0a 5665 7273 696f 6e20 312e 302e  t...Version 1.0.
-00001bf0: 3020 2872 656c 6561 7365 6420 3230 3138  0 (released 2018
-00001c00: 2d30 332d 3233 290a 0a2d 2049 6e69 7469  -03-23)..- Initi
-00001c10: 616c 2070 7562 6c69 6320 7265 6c65 6173  al public releas
-00001c20: 652e 0a                                  e..
+000000f0: 696f 6e20 332e 312e 3020 2872 656c 6561  ion 3.1.0 (relea
+00000100: 7365 6420 3230 3234 2d30 342d 3130 290a  sed 2024-04-10).
+00000110: 0a2d 2063 7373 3a20 6669 7820 6f76 6572  .- css: fix over
+00000120: 666c 6f77 2066 6f72 2064 6573 6372 6970  flow for descrip
+00000130: 7469 6f6e 2069 6e20 7265 636f 7264 2064  tion in record d
+00000140: 6574 6169 6c73 0a2d 2062 7567 3a20 6164  etails.- bug: ad
+00000150: 6420 6d69 7373 696e 6720 6060 3c74 6974  d missing ``<tit
+00000160: 6c65 3e73 6060 0a0a 5665 7273 696f 6e20  le>s``..Version 
+00000170: 332e 302e 3020 2872 656c 6561 7365 6420  3.0.0 (released 
+00000180: 3230 3234 2d30 332d 3139 290a 0a2d 2067  2024-03-19)..- g
+00000190: 6c6f 6261 6c3a 2072 656d 6f76 6520 6272  lobal: remove br
+000001a0: 6561 6463 7275 6d62 2073 7570 706f 7274  eadcrumb support
+000001b0: 0a2d 2067 6c6f 6261 6c3a 2069 6e74 726f  .- global: intro
+000001c0: 6475 6365 2073 6861 7265 6420 6d65 6e75  duce shared menu
+000001d0: 0a2d 2067 6c6f 6261 6c3a 2070 7265 7061  .- global: prepa
+000001e0: 7261 7469 6f6e 2066 6f72 2063 6f6d 7061  ration for compa
+000001f0: 7469 6269 6c69 7479 2077 6974 6820 466c  tibility with Fl
+00000200: 6173 6b20 7632 2e33 2e78 2064 6570 7265  ask v2.3.x depre
+00000210: 6361 7469 6f6e 730a 2d20 7265 6661 6374  cations.- refact
+00000220: 6f72 3a20 6375 7272 656e 745f 7468 656d  or: current_them
+00000230: 655f 6963 6f6e 7320 7769 7468 6f75 7420  e_icons without 
+00000240: 6170 706c 6963 6174 696f 6e20 636f 6e74  application cont
+00000250: 6578 740a 0a56 6572 7369 6f6e 2032 2e35  ext..Version 2.5
+00000260: 2e31 3020 2872 656c 6561 7365 6420 3230  .10 (released 20
+00000270: 3234 2d30 312d 3238 290a 0a2d 2069 6e73  24-01-28)..- ins
+00000280: 7461 6c6c 6174 696f 6e3a 2066 6978 2073  tallation: fix s
+00000290: 7068 696e 7820 6465 7065 6e64 656e 6379  phinx dependency
+000002a0: 0a0a 5665 7273 696f 6e20 322e 352e 3920  ..Version 2.5.9 
+000002b0: 2872 656c 6561 7365 6420 3230 3234 2d30  (released 2024-0
+000002c0: 312d 3238 290a 0a2d 2067 6c6f 6261 6c3a  1-28)..- global:
+000002d0: 2063 6861 6e67 6520 6d61 7468 206f 7065   change math ope
+000002e0: 7261 7469 6f6e 2074 6f20 6265 2063 6f6d  ration to be com
+000002f0: 7061 7469 626c 6520 7769 7468 2073 6173  patible with sas
+00000300: 7332 2e30 0a0a 5665 7273 696f 6e20 322e  s2.0..Version 2.
+00000310: 352e 3820 2872 656c 6561 7365 6420 3230  5.8 (released 20
+00000320: 3233 2d31 322d 3132 290a 0a2d 2072 6570  23-12-12)..- rep
+00000330: 6c61 6365 2063 6b65 6469 746f 7220 7769  lace ckeditor wi
+00000340: 7468 2074 696e 796d 6365 2064 7565 2074  th tinymce due t
+00000350: 6f20 6c69 6365 6e73 6520 6973 7375 650a  o license issue.
+00000360: 0a56 6572 7369 6f6e 2032 2e35 2e37 2028  .Version 2.5.7 (
+00000370: 7265 6c65 6173 6564 2032 3032 332d 3130  released 2023-10
+00000380: 2d32 3629 0a0a 2d20 636f 6d6d 756e 6974  -26)..- communit
+00000390: 7920 6c6f 676f 3a20 6669 7820 7265 6e64  y logo: fix rend
+000003a0: 6572 696e 6720 6120 706c 6163 6568 6f6c  ering a placehol
+000003b0: 6465 720a 0a56 6572 7369 6f6e 2032 2e35  der..Version 2.5
+000003c0: 2e36 2028 7265 6c65 6173 6564 2032 3032  .6 (released 202
+000003d0: 332d 3130 2d32 3029 0a0a 2d20 646f 6e27  3-10-20)..- don'
+000003e0: 7420 6f76 6572 7269 6465 206c 696e 6b73  t override links
+000003f0: 2073 7479 6c65 2069 6e20 666c 6173 6865   style in flashe
+00000400: 6420 6d65 7373 6167 6573 0a0a 5665 7273  d messages..Vers
+00000410: 696f 6e20 322e 352e 3520 2872 656c 6561  ion 2.5.5 (relea
+00000420: 7365 6420 3230 3233 2d30 392d 3139 290a  sed 2023-09-19).
+00000430: 0a2d 2073 7479 6c69 6e67 3a20 6164 6420  .- styling: add 
+00000440: 3320 636f 6c75 6d6e 2074 656d 706c 6174  3 column templat
+00000450: 6520 636c 6173 730a 0a56 6572 7369 6f6e  e class..Version
+00000460: 2032 2e35 2e34 2028 7265 6c65 6173 6564   2.5.4 (released
+00000470: 2032 3032 332d 3039 2d31 3129 0a0a 2d20   2023-09-11)..- 
+00000480: 7363 7373 3a20 6669 7820 636f 6d70 6174  scss: fix compat
+00000490: 6962 696c 6974 7920 7769 7468 206c 6174  ibility with lat
+000004a0: 6573 7420 6c65 7373 2076 6572 7369 6f6e  est less version
+000004b0: 0a0a 5665 7273 696f 6e20 322e 352e 3320  ..Version 2.5.3 
+000004c0: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
+000004d0: 382d 3038 290a 0a2d 2073 7479 6c65 7368  8-08)..- stylesh
+000004e0: 6565 7473 3a20 6164 6420 7072 6566 6f72  eets: add prefor
+000004f0: 6d61 7474 6564 2074 6167 2073 7479 6c69  matted tag styli
+00000500: 6e67 2066 6f6e 740a 0a56 6572 7369 6f6e  ng font..Version
+00000510: 2032 2e35 2e32 2028 7265 6c65 6173 6564   2.5.2 (released
+00000520: 2032 3032 332d 3038 2d31 3429 0a0a 2d20   2023-08-14)..- 
+00000530: 696e 7374 616c 6c61 7469 6f6e 3a20 7069  installation: pi
+00000540: 6e20 466c 6173 6b2d 4d65 6e75 2074 6f20  n Flask-Menu to 
+00000550: 6060 3c76 312e 302e 3060 602e 0a0a 5665  ``<v1.0.0``...Ve
+00000560: 7273 696f 6e20 322e 352e 3120 2872 656c  rsion 2.5.1 (rel
+00000570: 6561 7365 6420 3230 3233 2d30 382d 3134  eased 2023-08-14
+00000580: 290a 0a2d 2074 6865 6d65 3a20 6275 6766  )..- theme: bugf
+00000590: 6978 2074 6f20 6465 6372 6561 7365 207a  ix to decrease z
+000005a0: 2d69 6e64 6578 2076 616c 7565 0a0a 5665  -index value..Ve
+000005b0: 7273 696f 6e20 322e 352e 3020 2872 656c  rsion 2.5.0 (rel
+000005c0: 6561 7365 6420 3230 3233 2d30 382d 3039  eased 2023-08-09
+000005d0: 290a 0a2d 2074 6865 6d65 3a20 6164 6420  )..- theme: add 
+000005e0: 7574 696c 6974 7920 636c 6173 7365 730a  utility classes.
+000005f0: 0a56 6572 7369 6f6e 2032 2e34 2e30 2028  .Version 2.4.0 (
+00000600: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
+00000610: 2d30 3229 0a0a 2d20 7468 656d 653a 2061  -02)..- theme: a
+00000620: 6464 2073 6f6d 6520 6765 6e65 7261 6c20  dd some general 
+00000630: 636c 6173 7365 7320 616e 6420 6669 7865  classes and fixe
+00000640: 7320 616c 6967 6e6d 656e 7420 666f 7220  s alignment for 
+00000650: 6c61 6265 6c65 6420 666c 7569 6420 6275  labeled fluid bu
+00000660: 7474 6f6e 730a 0a56 6572 7369 6f6e 2032  ttons..Version 2
+00000670: 2e33 2e30 2028 7265 6c65 6173 6564 2032  .3.0 (released 2
+00000680: 3032 332d 3037 2d33 3129 0a0a 2d20 7365  023-07-31)..- se
+00000690: 7474 696e 6773 2070 6167 653a 2049 6d70  ttings page: Imp
+000006a0: 726f 7665 2074 656d 706c 6174 6520 666f  rove template fo
+000006b0: 7220 6131 3179 0a0a 5665 7273 696f 6e20  r a11y..Version 
+000006c0: 322e 322e 3020 2872 656c 6561 7365 6420  2.2.0 (released 
+000006d0: 3230 3233 2d30 372d 3236 290a 0a2d 2074  2023-07-26)..- t
+000006e0: 6865 6d65 3a20 6164 6420 6765 6e65 7261  heme: add genera
+000006f0: 6c20 7374 796c 6520 696d 7072 6f76 656d  l style improvem
+00000700: 656e 7473 0a0a 5665 7273 696f 6e20 322e  ents..Version 2.
+00000710: 312e 3320 2872 656c 6561 7365 6420 3230  1.3 (released 20
+00000720: 3233 2d30 372d 3234 290a 0a2d 206d 6573  23-07-24)..- mes
+00000730: 7361 6765 733a 2061 6464 207a 2d69 6e64  sages: add z-ind
+00000740: 6578 0a0a 5665 7273 696f 6e20 322e 312e  ex..Version 2.1.
+00000750: 3220 2872 656c 6561 7365 6420 3230 3233  2 (released 2023
+00000760: 2d30 342d 3132 290a 0a2d 2061 6464 2066  -04-12)..- add f
+00000770: 6c65 7820 7574 696c 6974 7920 636c 6173  lex utility clas
+00000780: 7365 730a 2d20 6164 6420 7465 7874 2073  ses.- add text s
+00000790: 697a 6573 2063 6c61 7373 6573 0a0a 5665  izes classes..Ve
+000007a0: 7273 696f 6e20 322e 312e 3120 2872 656c  rsion 2.1.1 (rel
+000007b0: 6561 7365 6420 3230 3233 2d30 342d 3036  eased 2023-04-06
+000007c0: 290a 0a2d 2061 6464 2064 6973 706c 6179  )..- add display
+000007d0: 2075 7469 6c69 7479 2063 6c61 7373 6573   utility classes
+000007e0: 0a0a 5665 7273 696f 6e20 322e 312e 3020  ..Version 2.1.0 
+000007f0: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
+00000800: 332d 3238 290a 0a2d 2061 6464 2067 6c6f  3-28)..- add glo
+00000810: 6261 6c20 7574 696c 6974 7920 7374 796c  bal utility styl
+00000820: 696e 6720 636c 6173 7365 730a 0a56 6572  ing classes..Ver
+00000830: 7369 6f6e 2032 2e30 2e31 2028 7265 6c65  sion 2.0.1 (rele
+00000840: 6173 6564 2032 3032 332d 3033 2d30 3929  ased 2023-03-09)
+00000850: 0a0a 2d20 6669 7820 7374 796c 696e 6720  ..- fix styling 
+00000860: 666f 7220 6275 7474 6f6e 730a 2d20 6d6f  for buttons.- mo
+00000870: 7665 2067 6c6f 6261 6c20 636c 6173 7320  ve global class 
+00000880: 666f 7220 6175 746f 2067 7269 640a 0a56  for auto grid..V
+00000890: 6572 7369 6f6e 2032 2e30 2e30 2028 7265  ersion 2.0.0 (re
+000008a0: 6c65 6173 6564 2032 3032 332d 3032 2d32  leased 2023-02-2
+000008b0: 3829 0a0a 2d20 6472 6f70 2070 7974 686f  8)..- drop pytho
+000008c0: 6e20 322e 3720 7375 7070 6f72 740a 2d20  n 2.7 support.- 
+000008d0: 7265 6d6f 7665 2066 6c61 736b 5f62 6162  remove flask_bab
+000008e0: 656c 6578 2069 6d70 6f72 7473 0a2d 2075  elex imports.- u
+000008f0: 7067 7261 6465 2069 6e76 656e 696f 5f69  pgrade invenio_i
+00000900: 3138 6e0a 0a56 6572 7369 6f6e 2031 2e34  18n..Version 1.4
+00000910: 2e38 2028 7265 6c65 6173 6564 2032 3032  .8 (released 202
+00000920: 332d 3032 2d30 3729 0a0a 2d20 7468 656d  3-02-07)..- them
+00000930: 653a 2061 6464 2061 7574 6f2d 636f 6c75  e: add auto-colu
+00000940: 6d6e 2d67 7269 6420 636c 6173 730a 0a56  mn-grid class..V
+00000950: 6572 7369 6f6e 2031 2e34 2e37 2028 7265  ersion 1.4.7 (re
+00000960: 6c65 6173 6564 2032 3032 332d 3031 2d30  leased 2023-01-0
+00000970: 3529 0a0a 2d20 6164 6420 7472 756e 6361  5)..- add trunca
+00000980: 7465 206c 696e 6573 2073 7479 6c65 730a  te lines styles.
+00000990: 0a56 6572 7369 6f6e 2031 2e34 2e36 2028  .Version 1.4.6 (
+000009a0: 7265 6c65 6173 6564 2032 3032 322d 3132  released 2022-12
+000009b0: 2d30 3829 0a0a 2d20 6669 7820 7374 796c  -08)..- fix styl
+000009c0: 696e 6720 666f 7220 696e 6c69 6e65 2063  ing for inline c
+000009d0: 6c61 7373 2c20 6166 6665 6374 696e 6720  lass, affecting 
+000009e0: 666f 726d 2066 6965 6c64 730a 0a56 6572  form fields..Ver
+000009f0: 7369 6f6e 2031 2e34 2e35 2028 7265 6c65  sion 1.4.5 (rele
+00000a00: 6173 6564 2032 3032 322d 3132 2d30 3129  ased 2022-12-01)
+00000a10: 0a0a 2d20 6669 7820 7365 6172 6368 2072  ..- fix search r
+00000a20: 6573 756c 7420 6974 656d 2073 7479 6c69  esult item styli
+00000a30: 6e67 0a2d 2061 6464 2067 6c6f 6261 6c20  ng.- add global 
+00000a40: 6265 6861 7669 6f75 7220 636c 6173 7365  behaviour classe
+00000a50: 730a 2d20 6164 6420 706c 6163 6568 6f6c  s.- add placehol
+00000a60: 6465 7220 696d 6167 6520 6861 6e64 6c65  der image handle
+00000a70: 0a0a 5665 7273 696f 6e20 312e 342e 3420  ..Version 1.4.4 
+00000a80: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
+00000a90: 312d 3138 290a 0a2d 2041 6464 2070 756c  1-18)..- Add pul
+00000aa0: 6c65 6420 7472 616e 736c 6174 696f 6e73  led translations
+00000ab0: 0a0a 5665 7273 696f 6e20 312e 342e 3320  ..Version 1.4.3 
+00000ac0: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
+00000ad0: 312d 3033 290a 0a2d 2061 6464 2073 7479  1-03)..- add sty
+00000ae0: 6c69 6e67 2066 6f72 2064 726f 7064 6f77  ling for dropdow
+00000af0: 6e20 6d65 6e75 2069 7465 6d73 0a2d 2066  n menu items.- f
+00000b00: 6978 206d 6973 7369 6e67 204d 6564 6961  ix missing Media
+00000b10: 2063 6f6d 706f 6e65 6e74 2072 616e 6765   component range
+00000b20: 0a0a 5665 7273 696f 6e20 312e 342e 3220  ..Version 1.4.2 
+00000b30: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
+00000b40: 302d 3236 290a 0a2d 2061 6464 204d 6564  0-26)..- add Med
+00000b50: 6961 2074 6f20 7375 7070 6f72 7420 7265  ia to support re
+00000b60: 7370 6f6e 7369 7665 2072 6561 6374 2063  sponsive react c
+00000b70: 6f6d 706f 6e65 6e74 730a 0a56 6572 7369  omponents..Versi
+00000b80: 6f6e 2031 2e34 2e31 2028 7265 6c65 6173  on 1.4.1 (releas
+00000b90: 6564 2032 3032 322d 3130 2d31 3029 0a0a  ed 2022-10-10)..
+00000ba0: 2d20 6275 6d70 2053 656d 616e 7469 6355  - bump SemanticU
+00000bb0: 490a 0a56 6572 7369 6f6e 2031 2e34 2e30  I..Version 1.4.0
+00000bc0: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
+00000bd0: 3130 2d30 3529 0a0a 2d20 6368 616e 6765  10-05)..- change
+00000be0: 2067 6c6f 6261 6c20 666f 6e74 2074 6f20   global font to 
+00000bf0: 4c61 746f 0a0a 5665 7273 696f 6e20 312e  Lato..Version 1.
+00000c00: 332e 3331 2028 7265 6c65 6173 6564 2032  3.31 (released 2
+00000c10: 3032 322d 3130 2d30 3529 0a0a 2d20 6164  022-10-05)..- ad
+00000c20: 6420 6d69 7373 696e 6720 7468 656d 6520  d missing theme 
+00000c30: 7661 7269 6162 6c65 730a 0a56 6572 7369  variables..Versi
+00000c40: 6f6e 2031 2e33 2e33 3020 2872 656c 6561  on 1.3.30 (relea
+00000c50: 7365 6420 3230 3232 2d30 392d 3236 290a  sed 2022-09-26).
+00000c60: 0a2d 2061 6464 2073 7479 6c69 6e67 2074  .- add styling t
+00000c70: 6f20 6164 6d69 6e69 7374 7261 7469 6f6e  o administration
+00000c80: 2064 6173 6862 6f61 7264 2070 6167 650a   dashboard page.
+00000c90: 0a56 6572 7369 6f6e 2031 2e33 2e32 3920  .Version 1.3.29 
+00000ca0: 2872 656c 6561 7365 6420 3230 3232 2d30  (released 2022-0
+00000cb0: 392d 3232 290a 0a2d 2061 6464 2061 646d  9-22)..- add adm
+00000cc0: 696e 6973 7472 6174 696f 6e20 7061 6e65  inistration pane
+00000cd0: 6c20 7374 796c 696e 670a 2d20 6164 6420  l styling.- add 
+00000ce0: 7472 616e 736c 6174 696f 6e20 776f 726b  translation work
+00000cf0: 666c 6f77 0a0a 5665 7273 696f 6e20 312e  flow..Version 1.
+00000d00: 332e 3238 2028 7265 6c65 6173 6564 2032  3.28 (released 2
+00000d10: 3032 322d 3037 2d30 3829 0a0a 2d20 6164  022-07-08)..- ad
+00000d20: 6420 7374 796c 696e 6720 636c 6173 7365  d styling classe
+00000d30: 7320 7769 7468 2061 6374 696f 6e20 636f  s with action co
+00000d40: 6c6f 7220 636f 6469 6e67 0a0a 5665 7273  lor coding..Vers
+00000d50: 696f 6e20 312e 332e 3237 2028 7265 6c65  ion 1.3.27 (rele
+00000d60: 6173 6564 2032 3032 322d 3037 2d30 3729  ased 2022-07-07)
+00000d70: 0a0a 2d20 6669 7820 6a71 7565 7279 2072  ..- fix jquery r
+00000d80: 6566 6572 656e 6365 0a0a 5665 7273 696f  eference..Versio
+00000d90: 6e20 312e 332e 3236 2028 7265 6c65 6173  n 1.3.26 (releas
+00000da0: 6564 2032 3032 322d 3037 2d30 3729 0a0a  ed 2022-07-07)..
+00000db0: 2d20 6164 6420 696d 6167 6520 706c 6163  - add image plac
+00000dc0: 6568 6f6c 6465 7220 6f6e 206c 6f61 6420  eholder on load 
+00000dd0: 6572 726f 720a 0a56 6572 7369 6f6e 2031  error..Version 1
+00000de0: 2e33 2e32 3520 2872 656c 6561 7365 6420  .3.25 (released 
+00000df0: 3230 3232 2d30 362d 3237 290a 0a2d 2061  2022-06-27)..- a
+00000e00: 6464 2047 6572 6d61 6e20 7472 616e 736c  dd German transl
+00000e10: 6174 696f 6e73 0a2d 2066 6978 2064 726f  ations.- fix dro
+00000e20: 7064 6f77 6e20 7363 726f 6c6c 206d 6973  pdown scroll mis
+00000e30: 616c 6967 6e6d 656e 740a 0a56 6572 7369  alignment..Versi
+00000e40: 6f6e 2031 2e33 2e32 3420 2872 656c 6561  on 1.3.24 (relea
+00000e50: 7365 6420 3230 3232 2d30 352d 3233 290a  sed 2022-05-23).
+00000e60: 0a2d 2061 6464 2067 6c6f 6261 6c20 4353  .- add global CS
+00000e70: 5320 636c 6173 7365 7320 666f 7220 6d61  S classes for ma
+00000e80: 7267 696e 7320 6175 746f 0a0a 5665 7273  rgins auto..Vers
+00000e90: 696f 6e20 312e 332e 3233 2028 7265 6c65  ion 1.3.23 (rele
+00000ea0: 6173 6564 2032 3032 322d 3035 2d31 3929  ased 2022-05-19)
+00000eb0: 0a0a 2d20 6164 6420 6163 6365 7373 6962  ..- add accessib
+00000ec0: 696c 6974 7920 746f 2075 692d 6163 636f  ility to ui-acco
+00000ed0: 7264 696f 6e73 0a0a 5665 7273 696f 6e20  rdions..Version 
+00000ee0: 312e 332e 3232 2028 7265 6c65 6173 6564  1.3.22 (released
+00000ef0: 2032 3032 322d 3034 2d32 3129 0a0a 2d20   2022-04-21)..- 
+00000f00: 696d 7072 6f76 6520 7365 6d61 6e74 6963  improve semantic
+00000f10: 2073 7479 6c69 6e67 206f 6620 4d79 2061   styling of My a
+00000f20: 6363 6f75 6e74 2070 6167 650a 0a56 6572  ccount page..Ver
+00000f30: 7369 6f6e 2031 2e33 2e32 3120 2872 656c  sion 1.3.21 (rel
+00000f40: 6561 7365 6420 3230 3232 2d30 332d 3239  eased 2022-03-29
+00000f50: 290a 0a2d 2066 6978 2068 746d 6c20 7461  )..- fix html ta
+00000f60: 6773 2069 6e20 7465 6d70 6c61 7465 730a  gs in templates.
+00000f70: 0a56 6572 7369 6f6e 2031 2e33 2e32 3020  .Version 1.3.20 
+00000f80: 2872 656c 6561 7365 6420 3230 3232 2d30  (released 2022-0
+00000f90: 332d 3137 290a 0a2d 2072 6566 6163 746f  3-17)..- refacto
+00000fa0: 7220 7061 6765 2074 656d 706c 6174 650a  r page template.
+00000fb0: 2d20 6164 6420 7365 6d61 6e74 6963 2075  - add semantic u
+00000fc0: 6920 696e 7665 6e69 6f20 7061 636b 6167  i invenio packag
+00000fd0: 6564 2074 6865 6d65 2063 6f6e 6669 6775  ed theme configu
+00000fe0: 7261 7469 6f6e 0a2d 2065 7874 656e 6420  ration.- extend 
+00000ff0: 7574 696c 7320 4353 5320 636c 6173 7365  utils CSS classe
+00001000: 730a 0a56 6572 7369 6f6e 2031 2e33 2e31  s..Version 1.3.1
+00001010: 3920 2872 656c 6561 7365 6420 3230 3232  9 (released 2022
+00001020: 2d30 332d 3034 290a 0a2d 2041 6464 2061  -03-04)..- Add a
+00001030: 2072 6575 7361 626c 6520 4a69 6e6a 6120   reusable Jinja 
+00001040: 6d61 6372 6f20 746f 2074 7275 6e63 6174  macro to truncat
+00001050: 6520 6c6f 6e67 2074 6578 742e 0a0a 5665  e long text...Ve
+00001060: 7273 696f 6e20 312e 332e 3138 2028 7265  rsion 1.3.18 (re
+00001070: 6c65 6173 6564 2032 3032 322d 3033 2d30  leased 2022-03-0
+00001080: 3129 0a0a 2d20 5265 7665 7274 2066 6f6e  1)..- Revert fon
+00001090: 7420 6261 636b 2074 6f20 6465 6661 756c  t back to defaul
+000010a0: 7420 7361 6e73 2d73 6172 6966 2066 6f6e  t sans-sarif fon
+000010b0: 7420 696e 7374 6561 6420 6f66 204c 6174  t instead of Lat
+000010c0: 6f2e 0a0a 5665 7273 696f 6e20 312e 332e  o...Version 1.3.
+000010d0: 3137 2028 7265 6c65 6173 6564 2032 3032  17 (released 202
+000010e0: 322d 3032 2d32 3829 0a0a 2d20 4164 6473  2-02-28)..- Adds
+000010f0: 2066 6176 6963 6f6e 0a2d 2046 6978 2069   favicon.- Fix i
+00001100: 7373 7565 2077 6974 6820 666c 6173 6820  ssue with flash 
+00001110: 6d65 7373 6167 6520 6f6e 206c 6f67 696e  message on login
+00001120: 2070 6167 6520 6e6f 7420 6265 696e 6720   page not being 
+00001130: 7369 6465 2074 6f20 7369 6465 2e0a 0a56  side to side...V
+00001140: 6572 7369 6f6e 2031 2e33 2e31 3620 2872  ersion 1.3.16 (r
+00001150: 656c 6561 7365 6420 3230 3232 2d30 322d  eleased 2022-02-
+00001160: 3137 290a 0a2d 2041 6464 2063 6f6d 6d6f  17)..- Add commo
+00001170: 6e20 6073 7175 6172 652d 706c 6163 6568  n `square-placeh
+00001180: 6f6c 6465 722e 706e 6760 2069 6d61 6765  older.png` image
+00001190: 2066 6f72 2067 656e 6572 616c 2075 7365   for general use
+000011a0: 2e0a 0a56 6572 7369 6f6e 2031 2e33 2e31  ...Version 1.3.1
+000011b0: 3520 2872 656c 6561 7365 6420 3230 3232  5 (released 2022
+000011c0: 2d30 322d 3137 290a 0a2d 2052 656d 6f76  -02-17)..- Remov
+000011d0: 6520 6375 7374 6f6d 206d 6172 6769 6e20  e custom margin 
+000011e0: 6672 6f6d 2063 6c61 7373 6573 2074 6f20  from classes to 
+000011f0: 696d 7072 6f76 6520 4353 5320 6f76 6572  improve CSS over
+00001200: 7269 6461 6269 6c69 7479 2e0a 0a56 6572  ridability...Ver
+00001210: 7369 6f6e 2031 2e33 2e31 3420 2872 656c  sion 1.3.14 (rel
+00001220: 6561 7365 6420 3230 3232 2d30 322d 3136  eased 2022-02-16
+00001230: 290a 0a2d 2046 6978 2069 7373 7565 2077  )..- Fix issue w
+00001240: 6974 6820 4c61 746f 2066 6f6e 7420 6e6f  ith Lato font no
+00001250: 7420 6265 696e 6720 6c6f 6164 6564 2069  t being loaded i
+00001260: 6e20 5365 6d61 6e74 6963 2055 4920 7468  n Semantic UI th
+00001270: 656d 652e 0a2d 2053 6574 7320 5365 6d61  eme..- Sets Sema
+00001280: 6e74 6963 2055 4920 406d 7574 6564 5465  ntic UI @mutedTe
+00001290: 7874 436f 6c6f 722e 0a0a 5665 7273 696f  xtColor...Versio
+000012a0: 6e20 312e 332e 3133 2028 7265 6c65 6173  n 1.3.13 (releas
+000012b0: 6564 2032 3032 322d 3032 2d31 3629 0a0a  ed 2022-02-16)..
+000012c0: 2d20 456e 7375 7265 2063 6f6d 7069 6c65  - Ensure compile
+000012d0: 6420 7472 616e 736c 6174 696f 6e20 6d65  d translation me
+000012e0: 7373 6167 6520 6361 7461 6c6f 6773 2061  ssage catalogs a
+000012f0: 7265 2069 6e63 6c75 6465 6420 696e 2074  re included in t
+00001300: 6865 0a20 2064 6973 7472 6962 7574 696f  he.  distributio
+00001310: 6e73 2075 706c 6f61 6465 6420 6f6e 2050  ns uploaded on P
+00001320: 7950 492e 0a0a 5665 7273 696f 6e20 312e  yPI...Version 1.
+00001330: 332e 3132 2028 7265 6c65 6173 6564 2032  3.12 (released 2
+00001340: 3032 322d 3032 2d31 3429 0a0a 2d20 4669  022-02-14)..- Fi
+00001350: 7865 7320 4131 3179 2069 7373 7565 2077  xes A11y issue w
+00001360: 6974 6820 7468 6520 636c 6f73 6520 6275  ith the close bu
+00001370: 7474 6f6e 2069 6e20 666c 6173 6820 6d65  tton in flash me
+00001380: 7373 6167 6573 2e0a 0a56 6572 7369 6f6e  ssages...Version
+00001390: 2031 2e33 2e31 3120 2872 656c 6561 7365   1.3.11 (release
+000013a0: 6420 3230 3232 2d30 322d 3038 290a 0a2d  d 2022-02-08)..-
+000013b0: 2041 6464 7320 6d61 7267 696e 2067 656e   Adds margin gen
+000013c0: 6572 6174 6f72 2e0a 2d20 4164 6473 2041  erator..- Adds A
+000013d0: 3131 7920 7061 6765 206c 616e 646d 6172  11y page landmar
+000013e0: 6b73 2e0a 0a56 6572 7369 6f6e 2031 2e33  ks...Version 1.3
+000013f0: 2e31 3020 2872 656c 6561 7365 6420 3230  .10 (released 20
+00001400: 3231 2d31 312d 3233 290a 0a2d 2057 6562  21-11-23)..- Web
+00001410: 2061 6363 6573 7369 6269 6c69 7479 2066   accessibility f
+00001420: 6978 2e0a 0a56 6572 7369 6f6e 2031 2e33  ix...Version 1.3
+00001430: 2e39 2028 7265 6c65 6173 6564 2032 3032  .9 (released 202
+00001440: 312d 3037 2d31 3229 0a0a 2d20 4164 6473  1-07-12)..- Adds
+00001450: 2067 6572 6d61 6e20 7472 616e 736c 6174   german translat
+00001460: 696f 6e73 0a0a 5665 7273 696f 6e20 312e  ions..Version 1.
+00001470: 332e 3820 2872 656c 6561 7365 6420 3230  3.8 (released 20
+00001480: 3231 2d30 322d 3130 290a 0a2d 2041 6464  21-02-10)..- Add
+00001490: 7320 6272 616e 6420 636f 6c6f 7220 746f  s brand color to
+000014a0: 206d 656e 7520 6974 656d 730a 0a56 6572   menu items..Ver
+000014b0: 7369 6f6e 2031 2e33 2e37 2028 7265 6c65  sion 1.3.7 (rele
+000014c0: 6173 6564 2032 3032 312d 3031 2d32 3529  ased 2021-01-25)
+000014d0: 0a0a 2d20 4164 6473 2062 7261 6e64 2063  ..- Adds brand c
+000014e0: 6f6c 6f72 2069 6e20 7365 676d 656e 7473  olor in segments
+000014f0: 0a0a 5665 7273 696f 6e20 312e 332e 3620  ..Version 1.3.6 
+00001500: 2872 656c 6561 7365 6420 3230 3231 2d30  (released 2021-0
+00001510: 312d 3034 290a 0a2d 2041 6464 7320 606c  1-04)..- Adds `l
+00001520: 696e 6b60 2074 6865 6d65 2069 636f 6e0a  ink` theme icon.
+00001530: 2d20 4669 7865 7320 7769 6c64 6361 7264  - Fixes wildcard
+00001540: 2069 636f 6e20 7265 736f 6c75 7469 6f6e   icon resolution
+00001550: 0a0a 5665 7273 696f 6e20 312e 332e 3520  ..Version 1.3.5 
+00001560: 2872 656c 6561 7365 6420 3230 3230 2d31  (released 2020-1
+00001570: 322d 3137 290a 0a2d 2046 6978 6573 2063  2-17)..- Fixes c
+00001580: 6865 636b 626f 782e 6f76 6572 7269 6465  heckbox.override
+00001590: 7320 696e 2060 696e 7665 6e69 6f60 2053  s in `invenio` S
+000015a0: 5549 2070 6163 6b61 6765 6420 7468 656d  UI packaged them
+000015b0: 652e 0a0a 5665 7273 696f 6e20 312e 332e  e...Version 1.3.
+000015c0: 3420 2872 656c 6561 7365 6420 3230 3230  4 (released 2020
+000015d0: 2d31 322d 3137 290a 0a2d 2041 6464 7320  -12-17)..- Adds 
+000015e0: 6120 6675 6c6c 2022 696e 7665 6e69 6f22  a full "invenio"
+000015f0: 2053 656d 616e 7469 6320 5549 2070 6163   Semantic UI pac
+00001600: 6b61 6765 6420 7468 656d 6520 736f 2077  kaged theme so w
+00001610: 6520 6361 6e20 6561 7369 6572 2063 7573  e can easier cus
+00001620: 746f 6d69 7a65 0a20 206c 6179 6f75 7420  tomize.  layout 
+00001630: 696e 2074 6865 2066 7574 7572 652e 0a0a  in the future...
+00001640: 2d20 4d6f 7665 7320 7468 656d 652e 636f  - Moves theme.co
+00001650: 6e66 6967 2074 6f20 7468 656d 652e 636f  nfig to theme.co
+00001660: 6e66 6967 2e65 7861 6d70 6c65 2061 6e64  nfig.example and
+00001670: 2061 6464 7320 6120 6e6f 7465 2074 6f20   adds a note to 
+00001680: 6d61 6b65 2069 740a 2020 636c 6561 7220  make it.  clear 
+00001690: 7468 6520 6669 6c65 2069 7320 6e6f 7420  the file is not 
+000016a0: 6163 7475 616c 6c79 2075 7365 642c 2062  actually used, b
+000016b0: 7574 2069 7320 6a75 7374 2061 6e20 6578  ut is just an ex
+000016c0: 616d 706c 652e 0a0a 2d20 4164 6473 2068  ample...- Adds h
+000016d0: 656c 7065 7220 746f 6f6c 2066 6f72 2073  elper tool for s
+000016e0: 7570 706f 7274 696e 6720 7468 656d 6520  upporting theme 
+000016f0: 6465 7065 6e64 656e 7420 6963 6f6e 732e  dependent icons.
+00001700: 0a0a 2d20 4669 7865 7320 6d61 6e79 206d  ..- Fixes many m
+00001710: 696e 6f72 2073 7479 6c69 6e67 2069 7373  inor styling iss
+00001720: 7565 7320 7375 6368 2061 7320 616c 6967  ues such as alig
+00001730: 6e6d 656e 7473 2c20 6275 7474 6f6e 206c  nments, button l
+00001740: 6f63 6174 696f 6e73 2c0a 2020 6772 6964  ocations,.  grid
+00001750: 732e 0a0a 5665 7273 696f 6e20 312e 332e  s...Version 1.3.
+00001760: 3320 2872 656c 6561 7365 6420 3230 3230  3 (released 2020
+00001770: 2d31 322d 3131 290a 0a2d 2049 6e69 7469  -12-11)..- Initi
+00001780: 616c 697a 6573 2073 656d 616e 7469 6355  alizes semanticU
+00001790: 4920 6163 636f 7264 696f 6e20 636f 6d70  I accordion comp
+000017a0: 6f6e 656e 7473 2e0a 0a56 6572 7369 6f6e  onents...Version
+000017b0: 2031 2e33 2e32 2028 7265 6c65 6173 6564   1.3.2 (released
+000017c0: 2032 3032 302d 3132 2d31 3129 0a0a 2d20   2020-12-11)..- 
+000017d0: 5570 6461 7465 7320 7468 6520 496e 7665  Updates the Inve
+000017e0: 6e69 6f20 6c6f 676f 2061 6e64 2072 656d  nio logo and rem
+000017f0: 6f76 6520 6f75 7464 6174 6564 2076 6572  ove outdated ver
+00001800: 7369 6f6e 732e 0a2d 2046 6978 6573 2074  sions..- Fixes t
+00001810: 6865 2064 726f 7064 6f77 6e20 746f 2077  he dropdown to w
+00001820: 6f72 6b20 6f6e 2074 6865 2075 7365 7220  ork on the user 
+00001830: 7072 6f66 696c 6520 7061 6765 2e0a 0a56  profile page...V
+00001840: 6572 7369 6f6e 2031 2e33 2e31 2028 7265  ersion 1.3.1 (re
+00001850: 6c65 6173 6564 2032 3032 302d 3132 2d30  leased 2020-12-0
+00001860: 3929 0a0a 2d20 4d69 6e6f 7220 6669 7820  9)..- Minor fix 
+00001870: 666f 7220 5365 6d61 6e74 6963 5549 2064  for SemanticUI d
+00001880: 726f 7064 6f77 6e73 0a0a 5665 7273 696f  ropdowns..Versio
+00001890: 6e20 312e 332e 3020 2872 656c 6561 7365  n 1.3.0 (release
+000018a0: 6420 3230 3230 2d31 322d 3039 290a 0a2d  d 2020-12-09)..-
+000018b0: 204d 616a 6f72 3a20 4e65 7720 5365 6d61   Major: New Sema
+000018c0: 6e74 6963 5549 2074 6865 6d65 2068 6173  nticUI theme has
+000018d0: 2062 6565 6e20 696e 7465 6772 6174 6564   been integrated
+000018e0: 2e20 5468 6520 426f 6f74 7374 7261 7020  . The Bootstrap 
+000018f0: 3320 7468 656d 6520 7374 696c 6c0a 2020  3 theme still.  
+00001900: 6578 6973 7473 2e20 5468 6973 2063 6861  exists. This cha
+00001910: 6e67 6520 6465 7065 6e64 7320 6f6e 2074  nge depends on t
+00001920: 6865 206c 6174 6573 7420 7265 6c65 6173  he latest releas
+00001930: 6564 2049 6e76 656e 696f 2d41 7373 6574  ed Invenio-Asset
+00001940: 7320 7768 6963 680a 2020 6164 6473 2073  s which.  adds s
+00001950: 7570 706f 7274 7320 666f 7220 6d75 6c74  upports for mult
+00001960: 6970 6c65 2055 4920 6672 616d 6577 6f72  iple UI framewor
+00001970: 6b73 2e0a 0a2d 2041 6464 7320 7375 7070  ks...- Adds supp
+00001980: 6f72 7420 666f 7220 6479 6e61 6d69 6320  ort for dynamic 
+00001990: 6c6f 6164 696e 6720 6f66 2074 656d 706c  loading of templ
+000019a0: 6174 6573 2066 6f72 2052 6561 6374 2d4f  ates for React-O
+000019b0: 7665 7272 6964 6162 6c65 2e0a 0a2d 2042  verridable...- B
+000019c0: 6163 6b77 6172 6473 2069 6e63 6f6d 7061  ackwards incompa
+000019d0: 7469 626c 653a 2054 6865 206f 6c64 2d73  tible: The old-s
+000019e0: 7479 6c65 2046 6c61 736b 2d41 7373 6574  tyle Flask-Asset
+000019f0: 2062 756e 646c 6573 2077 6173 2072 656d   bundles was rem
+00001a00: 6f76 6564 2028 7468 6573 650a 2020 6275  oved (these.  bu
+00001a10: 6e64 6c65 7320 7765 7265 2064 6570 7265  ndles were depre
+00001a20: 6361 7465 6420 696e 2049 6e76 656e 696f  cated in Invenio
+00001a30: 2076 332e 3129 2e0a 0a2d 2041 6464 7320   v3.1)...- Adds 
+00001a40: 5475 726b 6973 6820 7472 616e 736c 6174  Turkish translat
+00001a50: 696f 6e73 2e0a 0a56 6572 7369 6f6e 2031  ions...Version 1
+00001a60: 2e32 2e30 2028 7265 6c65 6173 6564 2032  .2.0 (released 2
+00001a70: 3032 302d 3033 2d32 3029 0a0a 2d20 5265  020-03-20)..- Re
+00001a80: 706c 6163 6573 2046 6c61 736b 2064 6570  places Flask dep
+00001a90: 656e 6465 6e63 7920 7769 7468 2060 6069  endency with ``i
+00001aa0: 6e76 656e 696f 2d62 6173 6560 602e 0a0a  nvenio-base``...
+00001ab0: 5665 7273 696f 6e20 312e 312e 3420 2872  Version 1.1.4 (r
+00001ac0: 656c 6561 7365 6420 3230 3139 2d30 372d  eleased 2019-07-
+00001ad0: 3232 290a 0a2d 2049 6e74 726f 6475 6365  22)..- Introduce
+00001ae0: 2068 616e 646c 696e 6720 6f66 2074 6865   handling of the
+00001af0: 2065 7272 6f72 2034 3239 2e0a 0a56 6572   error 429...Ver
+00001b00: 7369 6f6e 2031 2e31 2e33 2028 7265 6c65  sion 1.1.3 (rele
+00001b10: 6173 6564 2032 3031 392d 3033 2d31 3329  ased 2019-03-13)
+00001b20: 0a0a 2d20 5265 7374 7275 6374 7572 6520  ..- Restructure 
+00001b30: 5343 5353 2066 696c 6573 2c20 696e 206f  SCSS files, in o
+00001b40: 7264 6572 2074 6f20 616c 6c6f 7720 6561  rder to allow ea
+00001b50: 7369 6572 2063 7573 746f 6d69 7a61 7469  sier customizati
+00001b60: 6f6e 2061 6e64 2065 7874 656e 7369 6f6e  on and extension
+00001b70: 0a20 2069 6e20 6f76 6572 6c61 7973 2e0a  .  in overlays..
+00001b80: 0a56 6572 7369 6f6e 2031 2e31 2e32 2028  .Version 1.1.2 (
+00001b90: 7265 6c65 6173 6564 2032 3031 392d 3032  released 2019-02
+00001ba0: 2d31 3529 0a0a 2d20 5570 6772 6164 6564  -15)..- Upgraded
+00001bb0: 206d 6f6d 656e 7420 746f 2032 2e32 332e   moment to 2.23.
+00001bc0: 300a 0a56 6572 7369 6f6e 2031 2e31 2e31  0..Version 1.1.1
+00001bd0: 2028 7265 6c65 6173 6564 2032 3031 382d   (released 2018-
+00001be0: 3132 2d30 3529 0a0a 2d20 4669 7865 7320  12-05)..- Fixes 
+00001bf0: 6973 7375 6573 2077 6974 6820 7765 6270  issues with webp
+00001c00: 6163 6b20 616e 6420 7468 6520 4164 6d69  ack and the Admi
+00001c10: 6e4c 5445 2074 6865 6d65 2e0a 0a56 6572  nLTE theme...Ver
+00001c20: 7369 6f6e 2031 2e31 2e30 2028 7265 6c65  sion 1.1.0 (rele
+00001c30: 6173 6564 2032 3031 382d 3131 2d30 3629  ased 2018-11-06)
+00001c40: 0a0a 2d20 496e 7472 6f64 7563 6520 7765  ..- Introduce we
+00001c50: 6270 6163 6b20 7375 7070 6f72 742e 0a0a  bpack support...
+00001c60: 5665 7273 696f 6e20 312e 302e 3020 2872  Version 1.0.0 (r
+00001c70: 656c 6561 7365 6420 3230 3138 2d30 332d  eleased 2018-03-
+00001c80: 3233 290a 0a2d 2049 6e69 7469 616c 2070  23)..- Initial p
+00001c90: 7562 6c69 6320 7265 6c65 6173 652e 0a    ublic release..
```

### Comparing `invenio-theme-3.0.0/CONTRIBUTING.rst` & `invenio-theme-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/LICENSE` & `invenio-theme-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/MANIFEST.in` & `invenio-theme-3.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/PKG-INFO` & `invenio-theme-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 696e 7665  : 2.1.Name: inve
 00000020: 6e69 6f2d 7468 656d 650a 5665 7273 696f  nio-theme.Versio
-00000030: 6e3a 2033 2e30 2e30 0a53 756d 6d61 7279  n: 3.0.0.Summary
+00000030: 6e3a 2033 2e31 2e30 0a53 756d 6d61 7279  n: 3.1.0.Summary
 00000040: 3a20 2249 6e76 656e 696f 2073 7461 6e64  : "Invenio stand
 00000050: 6172 6420 7468 656d 652e 220a 486f 6d65  ard theme.".Home
 00000060: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 00000070: 6974 6875 622e 636f 6d2f 696e 7665 6e69  ithub.com/inveni
 00000080: 6f73 6f66 7477 6172 652f 696e 7665 6e69  osoftware/inveni
 00000090: 6f2d 7468 656d 650a 4175 7468 6f72 3a20  o-theme.Author: 
 000000a0: 496e 7665 6e69 6f20 436f 6c6c 6162 6f72  Invenio Collabor
@@ -119,610 +119,620 @@
 00000760: 2074 6865 204d 4954 204c 6963 656e 7365   the MIT License
 00000770: 3b20 7365 6520 4c49 4345 4e53 4520 6669  ; see LICENSE fi
 00000780: 6c65 2066 6f72 206d 6f72 6520 6465 7461  le for more deta
 00000790: 696c 732e 0a20 2020 2020 2020 200a 2020  ils..        .  
 000007a0: 2020 2020 2020 4368 616e 6765 730a 2020        Changes.  
 000007b0: 2020 2020 2020 3d3d 3d3d 3d3d 3d0a 2020        =======.  
 000007c0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
-000007d0: 6572 7369 6f6e 2033 2e30 2e30 2028 7265  ersion 3.0.0 (re
-000007e0: 6c65 6173 6564 2032 3032 342d 3033 2d31  leased 2024-03-1
-000007f0: 3929 0a20 2020 2020 2020 200a 2020 2020  9).        .    
-00000800: 2020 2020 2d20 676c 6f62 616c 3a20 7265      - global: re
-00000810: 6d6f 7665 2062 7265 6164 6372 756d 6220  move breadcrumb 
-00000820: 7375 7070 6f72 740a 2020 2020 2020 2020  support.        
-00000830: 2d20 676c 6f62 616c 3a20 696e 7472 6f64  - global: introd
-00000840: 7563 6520 7368 6172 6564 206d 656e 750a  uce shared menu.
-00000850: 2020 2020 2020 2020 2d20 676c 6f62 616c          - global
-00000860: 3a20 7072 6570 6172 6174 696f 6e20 666f  : preparation fo
-00000870: 7220 636f 6d70 6174 6962 696c 6974 7920  r compatibility 
-00000880: 7769 7468 2046 6c61 736b 2076 322e 332e  with Flask v2.3.
-00000890: 7820 6465 7072 6563 6174 696f 6e73 0a20  x deprecations. 
-000008a0: 2020 2020 2020 202d 2072 6566 6163 746f         - refacto
-000008b0: 723a 2063 7572 7265 6e74 5f74 6865 6d65  r: current_theme
-000008c0: 5f69 636f 6e73 2077 6974 686f 7574 2061  _icons without a
-000008d0: 7070 6c69 6361 7469 6f6e 2063 6f6e 7465  pplication conte
-000008e0: 7874 0a20 2020 2020 2020 200a 2020 2020  xt.        .    
-000008f0: 2020 2020 5665 7273 696f 6e20 322e 352e      Version 2.5.
-00000900: 3130 2028 7265 6c65 6173 6564 2032 3032  10 (released 202
-00000910: 342d 3031 2d32 3829 0a20 2020 2020 2020  4-01-28).       
-00000920: 200a 2020 2020 2020 2020 2d20 696e 7374   .        - inst
-00000930: 616c 6c61 7469 6f6e 3a20 6669 7820 7370  allation: fix sp
-00000940: 6869 6e78 2064 6570 656e 6465 6e63 790a  hinx dependency.
-00000950: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000960: 2056 6572 7369 6f6e 2032 2e35 2e39 2028   Version 2.5.9 (
-00000970: 7265 6c65 6173 6564 2032 3032 342d 3031  released 2024-01
-00000980: 2d32 3829 0a20 2020 2020 2020 200a 2020  -28).        .  
-00000990: 2020 2020 2020 2d20 676c 6f62 616c 3a20        - global: 
-000009a0: 6368 616e 6765 206d 6174 6820 6f70 6572  change math oper
-000009b0: 6174 696f 6e20 746f 2062 6520 636f 6d70  ation to be comp
-000009c0: 6174 6962 6c65 2077 6974 6820 7361 7373  atible with sass
-000009d0: 322e 300a 2020 2020 2020 2020 0a20 2020  2.0.        .   
-000009e0: 2020 2020 2056 6572 7369 6f6e 2032 2e35       Version 2.5
-000009f0: 2e38 2028 7265 6c65 6173 6564 2032 3032  .8 (released 202
-00000a00: 332d 3132 2d31 3229 0a20 2020 2020 2020  3-12-12).       
-00000a10: 200a 2020 2020 2020 2020 2d20 7265 706c   .        - repl
-00000a20: 6163 6520 636b 6564 6974 6f72 2077 6974  ace ckeditor wit
-00000a30: 6820 7469 6e79 6d63 6520 6475 6520 746f  h tinymce due to
-00000a40: 206c 6963 656e 7365 2069 7373 7565 0a20   license issue. 
-00000a50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000a60: 5665 7273 696f 6e20 322e 352e 3720 2872  Version 2.5.7 (r
-00000a70: 656c 6561 7365 6420 3230 3233 2d31 302d  eleased 2023-10-
-00000a80: 3236 290a 2020 2020 2020 2020 0a20 2020  26).        .   
-00000a90: 2020 2020 202d 2063 6f6d 6d75 6e69 7479       - community
-00000aa0: 206c 6f67 6f3a 2066 6978 2072 656e 6465   logo: fix rende
-00000ab0: 7269 6e67 2061 2070 6c61 6365 686f 6c64  ring a placehold
-00000ac0: 6572 0a20 2020 2020 2020 200a 2020 2020  er.        .    
-00000ad0: 2020 2020 5665 7273 696f 6e20 322e 352e      Version 2.5.
-00000ae0: 3620 2872 656c 6561 7365 6420 3230 3233  6 (released 2023
-00000af0: 2d31 302d 3230 290a 2020 2020 2020 2020  -10-20).        
-00000b00: 0a20 2020 2020 2020 202d 2064 6f6e 2774  .        - don't
-00000b10: 206f 7665 7272 6964 6520 6c69 6e6b 7320   override links 
-00000b20: 7374 796c 6520 696e 2066 6c61 7368 6564  style in flashed
-00000b30: 206d 6573 7361 6765 730a 2020 2020 2020   messages.      
-00000b40: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-00000b50: 6f6e 2032 2e35 2e35 2028 7265 6c65 6173  on 2.5.5 (releas
-00000b60: 6564 2032 3032 332d 3039 2d31 3929 0a20  ed 2023-09-19). 
-00000b70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000b80: 2d20 7374 796c 696e 673a 2061 6464 2033  - styling: add 3
-00000b90: 2063 6f6c 756d 6e20 7465 6d70 6c61 7465   column template
-00000ba0: 2063 6c61 7373 0a20 2020 2020 2020 200a   class.        .
-00000bb0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00000bc0: 322e 352e 3420 2872 656c 6561 7365 6420  2.5.4 (released 
-00000bd0: 3230 3233 2d30 392d 3131 290a 2020 2020  2023-09-11).    
-00000be0: 2020 2020 0a20 2020 2020 2020 202d 2073      .        - s
-00000bf0: 6373 733a 2066 6978 2063 6f6d 7061 7469  css: fix compati
-00000c00: 6269 6c69 7479 2077 6974 6820 6c61 7465  bility with late
-00000c10: 7374 206c 6573 7320 7665 7273 696f 6e0a  st less version.
-00000c20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000c30: 2056 6572 7369 6f6e 2032 2e35 2e33 2028   Version 2.5.3 (
-00000c40: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
-00000c50: 2d30 3829 0a20 2020 2020 2020 200a 2020  -08).        .  
-00000c60: 2020 2020 2020 2d20 7374 796c 6573 6865        - styleshe
-00000c70: 6574 733a 2061 6464 2070 7265 666f 726d  ets: add preform
-00000c80: 6174 7465 6420 7461 6720 7374 796c 696e  atted tag stylin
-00000c90: 6720 666f 6e74 0a20 2020 2020 2020 200a  g font.        .
-00000ca0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00000cb0: 322e 352e 3220 2872 656c 6561 7365 6420  2.5.2 (released 
-00000cc0: 3230 3233 2d30 382d 3134 290a 2020 2020  2023-08-14).    
-00000cd0: 2020 2020 0a20 2020 2020 2020 202d 2069      .        - i
-00000ce0: 6e73 7461 6c6c 6174 696f 6e3a 2070 696e  nstallation: pin
-00000cf0: 2046 6c61 736b 2d4d 656e 7520 746f 2060   Flask-Menu to `
-00000d00: 603c 7631 2e30 2e30 6060 2e0a 2020 2020  `<v1.0.0``..    
-00000d10: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00000d20: 7369 6f6e 2032 2e35 2e31 2028 7265 6c65  sion 2.5.1 (rele
-00000d30: 6173 6564 2032 3032 332d 3038 2d31 3429  ased 2023-08-14)
-00000d40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000d50: 2020 2d20 7468 656d 653a 2062 7567 6669    - theme: bugfi
-00000d60: 7820 746f 2064 6563 7265 6173 6520 7a2d  x to decrease z-
-00000d70: 696e 6465 7820 7661 6c75 650a 2020 2020  index value.    
-00000d80: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00000d90: 7369 6f6e 2032 2e35 2e30 2028 7265 6c65  sion 2.5.0 (rele
-00000da0: 6173 6564 2032 3032 332d 3038 2d30 3929  ased 2023-08-09)
-00000db0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000dc0: 2020 2d20 7468 656d 653a 2061 6464 2075    - theme: add u
-00000dd0: 7469 6c69 7479 2063 6c61 7373 6573 0a20  tility classes. 
-00000de0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000df0: 5665 7273 696f 6e20 322e 342e 3020 2872  Version 2.4.0 (r
-00000e00: 656c 6561 7365 6420 3230 3233 2d30 382d  eleased 2023-08-
-00000e10: 3032 290a 2020 2020 2020 2020 0a20 2020  02).        .   
-00000e20: 2020 2020 202d 2074 6865 6d65 3a20 6164       - theme: ad
-00000e30: 6420 736f 6d65 2067 656e 6572 616c 2063  d some general c
-00000e40: 6c61 7373 6573 2061 6e64 2066 6978 6573  lasses and fixes
-00000e50: 2061 6c69 676e 6d65 6e74 2066 6f72 206c   alignment for l
-00000e60: 6162 656c 6564 2066 6c75 6964 2062 7574  abeled fluid but
-00000e70: 746f 6e73 0a20 2020 2020 2020 200a 2020  tons.        .  
-00000e80: 2020 2020 2020 5665 7273 696f 6e20 322e        Version 2.
-00000e90: 332e 3020 2872 656c 6561 7365 6420 3230  3.0 (released 20
-00000ea0: 3233 2d30 372d 3331 290a 2020 2020 2020  23-07-31).      
-00000eb0: 2020 0a20 2020 2020 2020 202d 2073 6574    .        - set
-00000ec0: 7469 6e67 7320 7061 6765 3a20 496d 7072  tings page: Impr
-00000ed0: 6f76 6520 7465 6d70 6c61 7465 2066 6f72  ove template for
-00000ee0: 2061 3131 790a 2020 2020 2020 2020 0a20   a11y.        . 
-00000ef0: 2020 2020 2020 2056 6572 7369 6f6e 2032         Version 2
-00000f00: 2e32 2e30 2028 7265 6c65 6173 6564 2032  .2.0 (released 2
-00000f10: 3032 332d 3037 2d32 3629 0a20 2020 2020  023-07-26).     
-00000f20: 2020 200a 2020 2020 2020 2020 2d20 7468     .        - th
-00000f30: 656d 653a 2061 6464 2067 656e 6572 616c  eme: add general
-00000f40: 2073 7479 6c65 2069 6d70 726f 7665 6d65   style improveme
-00000f50: 6e74 730a 2020 2020 2020 2020 0a20 2020  nts.        .   
-00000f60: 2020 2020 2056 6572 7369 6f6e 2032 2e31       Version 2.1
-00000f70: 2e33 2028 7265 6c65 6173 6564 2032 3032  .3 (released 202
-00000f80: 332d 3037 2d32 3429 0a20 2020 2020 2020  3-07-24).       
-00000f90: 200a 2020 2020 2020 2020 2d20 6d65 7373   .        - mess
-00000fa0: 6167 6573 3a20 6164 6420 7a2d 696e 6465  ages: add z-inde
-00000fb0: 780a 2020 2020 2020 2020 0a20 2020 2020  x.        .     
-00000fc0: 2020 2056 6572 7369 6f6e 2032 2e31 2e32     Version 2.1.2
-00000fd0: 2028 7265 6c65 6173 6564 2032 3032 332d   (released 2023-
-00000fe0: 3034 2d31 3229 0a20 2020 2020 2020 200a  04-12).        .
-00000ff0: 2020 2020 2020 2020 2d20 6164 6420 666c          - add fl
-00001000: 6578 2075 7469 6c69 7479 2063 6c61 7373  ex utility class
-00001010: 6573 0a20 2020 2020 2020 202d 2061 6464  es.        - add
-00001020: 2074 6578 7420 7369 7a65 7320 636c 6173   text sizes clas
-00001030: 7365 730a 2020 2020 2020 2020 0a20 2020  ses.        .   
-00001040: 2020 2020 2056 6572 7369 6f6e 2032 2e31       Version 2.1
-00001050: 2e31 2028 7265 6c65 6173 6564 2032 3032  .1 (released 202
-00001060: 332d 3034 2d30 3629 0a20 2020 2020 2020  3-04-06).       
-00001070: 200a 2020 2020 2020 2020 2d20 6164 6420   .        - add 
-00001080: 6469 7370 6c61 7920 7574 696c 6974 7920  display utility 
-00001090: 636c 6173 7365 730a 2020 2020 2020 2020  classes.        
-000010a0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-000010b0: 2032 2e31 2e30 2028 7265 6c65 6173 6564   2.1.0 (released
-000010c0: 2032 3032 332d 3033 2d32 3829 0a20 2020   2023-03-28).   
-000010d0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-000010e0: 6164 6420 676c 6f62 616c 2075 7469 6c69  add global utili
-000010f0: 7479 2073 7479 6c69 6e67 2063 6c61 7373  ty styling class
-00001100: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
-00001110: 2020 2020 5665 7273 696f 6e20 322e 302e      Version 2.0.
-00001120: 3120 2872 656c 6561 7365 6420 3230 3233  1 (released 2023
-00001130: 2d30 332d 3039 290a 2020 2020 2020 2020  -03-09).        
-00001140: 0a20 2020 2020 2020 202d 2066 6978 2073  .        - fix s
-00001150: 7479 6c69 6e67 2066 6f72 2062 7574 746f  tyling for butto
-00001160: 6e73 0a20 2020 2020 2020 202d 206d 6f76  ns.        - mov
-00001170: 6520 676c 6f62 616c 2063 6c61 7373 2066  e global class f
-00001180: 6f72 2061 7574 6f20 6772 6964 0a20 2020  or auto grid.   
-00001190: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-000011a0: 7273 696f 6e20 322e 302e 3020 2872 656c  rsion 2.0.0 (rel
-000011b0: 6561 7365 6420 3230 3233 2d30 322d 3238  eased 2023-02-28
-000011c0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000011d0: 2020 202d 2064 726f 7020 7079 7468 6f6e     - drop python
-000011e0: 2032 2e37 2073 7570 706f 7274 0a20 2020   2.7 support.   
-000011f0: 2020 2020 202d 2072 656d 6f76 6520 666c       - remove fl
-00001200: 6173 6b5f 6261 6265 6c65 7820 696d 706f  ask_babelex impo
-00001210: 7274 730a 2020 2020 2020 2020 2d20 7570  rts.        - up
-00001220: 6772 6164 6520 696e 7665 6e69 6f5f 6931  grade invenio_i1
-00001230: 386e 0a20 2020 2020 2020 200a 2020 2020  8n.        .    
-00001240: 2020 2020 5665 7273 696f 6e20 312e 342e      Version 1.4.
-00001250: 3820 2872 656c 6561 7365 6420 3230 3233  8 (released 2023
-00001260: 2d30 322d 3037 290a 2020 2020 2020 2020  -02-07).        
-00001270: 0a20 2020 2020 2020 202d 2074 6865 6d65  .        - theme
-00001280: 3a20 6164 6420 6175 746f 2d63 6f6c 756d  : add auto-colum
-00001290: 6e2d 6772 6964 2063 6c61 7373 0a20 2020  n-grid class.   
-000012a0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-000012b0: 7273 696f 6e20 312e 342e 3720 2872 656c  rsion 1.4.7 (rel
-000012c0: 6561 7365 6420 3230 3233 2d30 312d 3035  eased 2023-01-05
-000012d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000012e0: 2020 202d 2061 6464 2074 7275 6e63 6174     - add truncat
-000012f0: 6520 6c69 6e65 7320 7374 796c 6573 0a20  e lines styles. 
-00001300: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001310: 5665 7273 696f 6e20 312e 342e 3620 2872  Version 1.4.6 (r
-00001320: 656c 6561 7365 6420 3230 3232 2d31 322d  eleased 2022-12-
-00001330: 3038 290a 2020 2020 2020 2020 0a20 2020  08).        .   
-00001340: 2020 2020 202d 2066 6978 2073 7479 6c69       - fix styli
-00001350: 6e67 2066 6f72 2069 6e6c 696e 6520 636c  ng for inline cl
-00001360: 6173 732c 2061 6666 6563 7469 6e67 2066  ass, affecting f
-00001370: 6f72 6d20 6669 656c 6473 0a20 2020 2020  orm fields.     
-00001380: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00001390: 696f 6e20 312e 342e 3520 2872 656c 6561  ion 1.4.5 (relea
-000013a0: 7365 6420 3230 3232 2d31 322d 3031 290a  sed 2022-12-01).
-000013b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000013c0: 202d 2066 6978 2073 6561 7263 6820 7265   - fix search re
-000013d0: 7375 6c74 2069 7465 6d20 7374 796c 696e  sult item stylin
-000013e0: 670a 2020 2020 2020 2020 2d20 6164 6420  g.        - add 
-000013f0: 676c 6f62 616c 2062 6568 6176 696f 7572  global behaviour
-00001400: 2063 6c61 7373 6573 0a20 2020 2020 2020   classes.       
-00001410: 202d 2061 6464 2070 6c61 6365 686f 6c64   - add placehold
-00001420: 6572 2069 6d61 6765 2068 616e 646c 650a  er image handle.
-00001430: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001440: 2056 6572 7369 6f6e 2031 2e34 2e34 2028   Version 1.4.4 (
-00001450: 7265 6c65 6173 6564 2032 3032 322d 3131  released 2022-11
-00001460: 2d31 3829 0a20 2020 2020 2020 200a 2020  -18).        .  
-00001470: 2020 2020 2020 2d20 4164 6420 7075 6c6c        - Add pull
-00001480: 6564 2074 7261 6e73 6c61 7469 6f6e 730a  ed translations.
-00001490: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000014a0: 2056 6572 7369 6f6e 2031 2e34 2e33 2028   Version 1.4.3 (
-000014b0: 7265 6c65 6173 6564 2032 3032 322d 3131  released 2022-11
-000014c0: 2d30 3329 0a20 2020 2020 2020 200a 2020  -03).        .  
-000014d0: 2020 2020 2020 2d20 6164 6420 7374 796c        - add styl
-000014e0: 696e 6720 666f 7220 6472 6f70 646f 776e  ing for dropdown
-000014f0: 206d 656e 7520 6974 656d 730a 2020 2020   menu items.    
-00001500: 2020 2020 2d20 6669 7820 6d69 7373 696e      - fix missin
-00001510: 6720 4d65 6469 6120 636f 6d70 6f6e 656e  g Media componen
-00001520: 7420 7261 6e67 650a 2020 2020 2020 2020  t range.        
-00001530: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-00001540: 2031 2e34 2e32 2028 7265 6c65 6173 6564   1.4.2 (released
-00001550: 2032 3032 322d 3130 2d32 3629 0a20 2020   2022-10-26).   
-00001560: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00001570: 6164 6420 4d65 6469 6120 746f 2073 7570  add Media to sup
-00001580: 706f 7274 2072 6573 706f 6e73 6976 6520  port responsive 
-00001590: 7265 6163 7420 636f 6d70 6f6e 656e 7473  react components
-000015a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015b0: 2020 5665 7273 696f 6e20 312e 342e 3120    Version 1.4.1 
-000015c0: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
-000015d0: 302d 3130 290a 2020 2020 2020 2020 0a20  0-10).        . 
-000015e0: 2020 2020 2020 202d 2062 756d 7020 5365         - bump Se
-000015f0: 6d61 6e74 6963 5549 0a20 2020 2020 2020  manticUI.       
-00001600: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
-00001610: 6e20 312e 342e 3020 2872 656c 6561 7365  n 1.4.0 (release
-00001620: 6420 3230 3232 2d31 302d 3035 290a 2020  d 2022-10-05).  
-00001630: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-00001640: 2063 6861 6e67 6520 676c 6f62 616c 2066   change global f
-00001650: 6f6e 7420 746f 204c 6174 6f0a 2020 2020  ont to Lato.    
-00001660: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00001670: 7369 6f6e 2031 2e33 2e33 3120 2872 656c  sion 1.3.31 (rel
-00001680: 6561 7365 6420 3230 3232 2d31 302d 3035  eased 2022-10-05
-00001690: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000016a0: 2020 202d 2061 6464 206d 6973 7369 6e67     - add missing
-000016b0: 2074 6865 6d65 2076 6172 6961 626c 6573   theme variables
-000016c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000016d0: 2020 5665 7273 696f 6e20 312e 332e 3330    Version 1.3.30
-000016e0: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-000016f0: 3039 2d32 3629 0a20 2020 2020 2020 200a  09-26).        .
-00001700: 2020 2020 2020 2020 2d20 6164 6420 7374          - add st
-00001710: 796c 696e 6720 746f 2061 646d 696e 6973  yling to adminis
-00001720: 7472 6174 696f 6e20 6461 7368 626f 6172  tration dashboar
-00001730: 6420 7061 6765 0a20 2020 2020 2020 200a  d page.        .
-00001740: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00001750: 312e 332e 3239 2028 7265 6c65 6173 6564  1.3.29 (released
-00001760: 2032 3032 322d 3039 2d32 3229 0a20 2020   2022-09-22).   
-00001770: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00001780: 6164 6420 6164 6d69 6e69 7374 7261 7469  add administrati
-00001790: 6f6e 2070 616e 656c 2073 7479 6c69 6e67  on panel styling
-000017a0: 0a20 2020 2020 2020 202d 2061 6464 2074  .        - add t
-000017b0: 7261 6e73 6c61 7469 6f6e 2077 6f72 6b66  ranslation workf
-000017c0: 6c6f 770a 2020 2020 2020 2020 0a20 2020  low.        .   
-000017d0: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
-000017e0: 2e32 3820 2872 656c 6561 7365 6420 3230  .28 (released 20
-000017f0: 3232 2d30 372d 3038 290a 2020 2020 2020  22-07-08).      
-00001800: 2020 0a20 2020 2020 2020 202d 2061 6464    .        - add
-00001810: 2073 7479 6c69 6e67 2063 6c61 7373 6573   styling classes
-00001820: 2077 6974 6820 6163 7469 6f6e 2063 6f6c   with action col
-00001830: 6f72 2063 6f64 696e 670a 2020 2020 2020  or coding.      
-00001840: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-00001850: 6f6e 2031 2e33 2e32 3720 2872 656c 6561  on 1.3.27 (relea
-00001860: 7365 6420 3230 3232 2d30 372d 3037 290a  sed 2022-07-07).
-00001870: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001880: 202d 2066 6978 206a 7175 6572 7920 7265   - fix jquery re
-00001890: 6665 7265 6e63 650a 2020 2020 2020 2020  ference.        
-000018a0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-000018b0: 2031 2e33 2e32 3620 2872 656c 6561 7365   1.3.26 (release
-000018c0: 6420 3230 3232 2d30 372d 3037 290a 2020  d 2022-07-07).  
-000018d0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-000018e0: 2061 6464 2069 6d61 6765 2070 6c61 6365   add image place
-000018f0: 686f 6c64 6572 206f 6e20 6c6f 6164 2065  holder on load e
-00001900: 7272 6f72 0a20 2020 2020 2020 200a 2020  rror.        .  
-00001910: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
-00001920: 332e 3235 2028 7265 6c65 6173 6564 2032  3.25 (released 2
-00001930: 3032 322d 3036 2d32 3729 0a20 2020 2020  022-06-27).     
-00001940: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
-00001950: 6420 4765 726d 616e 2074 7261 6e73 6c61  d German transla
-00001960: 7469 6f6e 730a 2020 2020 2020 2020 2d20  tions.        - 
-00001970: 6669 7820 6472 6f70 646f 776e 2073 6372  fix dropdown scr
-00001980: 6f6c 6c20 6d69 7361 6c69 676e 6d65 6e74  oll misalignment
-00001990: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000019a0: 2020 5665 7273 696f 6e20 312e 332e 3234    Version 1.3.24
-000019b0: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-000019c0: 3035 2d32 3329 0a20 2020 2020 2020 200a  05-23).        .
-000019d0: 2020 2020 2020 2020 2d20 6164 6420 676c          - add gl
-000019e0: 6f62 616c 2043 5353 2063 6c61 7373 6573  obal CSS classes
-000019f0: 2066 6f72 206d 6172 6769 6e73 2061 7574   for margins aut
-00001a00: 6f0a 2020 2020 2020 2020 0a20 2020 2020  o.        .     
-00001a10: 2020 2056 6572 7369 6f6e 2031 2e33 2e32     Version 1.3.2
-00001a20: 3320 2872 656c 6561 7365 6420 3230 3232  3 (released 2022
-00001a30: 2d30 352d 3139 290a 2020 2020 2020 2020  -05-19).        
-00001a40: 0a20 2020 2020 2020 202d 2061 6464 2061  .        - add a
-00001a50: 6363 6573 7369 6269 6c69 7479 2074 6f20  ccessibility to 
-00001a60: 7569 2d61 6363 6f72 6469 6f6e 730a 2020  ui-accordions.  
-00001a70: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
-00001a80: 6572 7369 6f6e 2031 2e33 2e32 3220 2872  ersion 1.3.22 (r
-00001a90: 656c 6561 7365 6420 3230 3232 2d30 342d  eleased 2022-04-
-00001aa0: 3231 290a 2020 2020 2020 2020 0a20 2020  21).        .   
-00001ab0: 2020 2020 202d 2069 6d70 726f 7665 2073       - improve s
-00001ac0: 656d 616e 7469 6320 7374 796c 696e 6720  emantic styling 
-00001ad0: 6f66 204d 7920 6163 636f 756e 7420 7061  of My account pa
-00001ae0: 6765 0a20 2020 2020 2020 200a 2020 2020  ge.        .    
-00001af0: 2020 2020 5665 7273 696f 6e20 312e 332e      Version 1.3.
-00001b00: 3231 2028 7265 6c65 6173 6564 2032 3032  21 (released 202
-00001b10: 322d 3033 2d32 3929 0a20 2020 2020 2020  2-03-29).       
-00001b20: 200a 2020 2020 2020 2020 2d20 6669 7820   .        - fix 
-00001b30: 6874 6d6c 2074 6167 7320 696e 2074 656d  html tags in tem
-00001b40: 706c 6174 6573 0a20 2020 2020 2020 200a  plates.        .
-00001b50: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00001b60: 312e 332e 3230 2028 7265 6c65 6173 6564  1.3.20 (released
-00001b70: 2032 3032 322d 3033 2d31 3729 0a20 2020   2022-03-17).   
-00001b80: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00001b90: 7265 6661 6374 6f72 2070 6167 6520 7465  refactor page te
-00001ba0: 6d70 6c61 7465 0a20 2020 2020 2020 202d  mplate.        -
-00001bb0: 2061 6464 2073 656d 616e 7469 6320 7569   add semantic ui
-00001bc0: 2069 6e76 656e 696f 2070 6163 6b61 6765   invenio package
-00001bd0: 6420 7468 656d 6520 636f 6e66 6967 7572  d theme configur
-00001be0: 6174 696f 6e0a 2020 2020 2020 2020 2d20  ation.        - 
-00001bf0: 6578 7465 6e64 2075 7469 6c73 2043 5353  extend utils CSS
-00001c00: 2063 6c61 7373 6573 0a20 2020 2020 2020   classes.       
-00001c10: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
-00001c20: 6e20 312e 332e 3139 2028 7265 6c65 6173  n 1.3.19 (releas
-00001c30: 6564 2032 3032 322d 3033 2d30 3429 0a20  ed 2022-03-04). 
-00001c40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001c50: 2d20 4164 6420 6120 7265 7573 6162 6c65  - Add a reusable
-00001c60: 204a 696e 6a61 206d 6163 726f 2074 6f20   Jinja macro to 
-00001c70: 7472 756e 6361 7465 206c 6f6e 6720 7465  truncate long te
-00001c80: 7874 2e0a 2020 2020 2020 2020 0a20 2020  xt..        .   
-00001c90: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
-00001ca0: 2e31 3820 2872 656c 6561 7365 6420 3230  .18 (released 20
-00001cb0: 3232 2d30 332d 3031 290a 2020 2020 2020  22-03-01).      
-00001cc0: 2020 0a20 2020 2020 2020 202d 2052 6576    .        - Rev
-00001cd0: 6572 7420 666f 6e74 2062 6163 6b20 746f  ert font back to
-00001ce0: 2064 6566 6175 6c74 2073 616e 732d 7361   default sans-sa
-00001cf0: 7269 6620 666f 6e74 2069 6e73 7465 6164  rif font instead
-00001d00: 206f 6620 4c61 746f 2e0a 2020 2020 2020   of Lato..      
-00001d10: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-00001d20: 6f6e 2031 2e33 2e31 3720 2872 656c 6561  on 1.3.17 (relea
-00001d30: 7365 6420 3230 3232 2d30 322d 3238 290a  sed 2022-02-28).
-00001d40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001d50: 202d 2041 6464 7320 6661 7669 636f 6e0a   - Adds favicon.
-00001d60: 2020 2020 2020 2020 2d20 4669 7820 6973          - Fix is
-00001d70: 7375 6520 7769 7468 2066 6c61 7368 206d  sue with flash m
-00001d80: 6573 7361 6765 206f 6e20 6c6f 6769 6e20  essage on login 
-00001d90: 7061 6765 206e 6f74 2062 6569 6e67 2073  page not being s
-00001da0: 6964 6520 746f 2073 6964 652e 0a20 2020  ide to side..   
-00001db0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-00001dc0: 7273 696f 6e20 312e 332e 3136 2028 7265  rsion 1.3.16 (re
-00001dd0: 6c65 6173 6564 2032 3032 322d 3032 2d31  leased 2022-02-1
-00001de0: 3729 0a20 2020 2020 2020 200a 2020 2020  7).        .    
-00001df0: 2020 2020 2d20 4164 6420 636f 6d6d 6f6e      - Add common
-00001e00: 2060 7371 7561 7265 2d70 6c61 6365 686f   `square-placeho
-00001e10: 6c64 6572 2e70 6e67 6020 696d 6167 6520  lder.png` image 
-00001e20: 666f 7220 6765 6e65 7261 6c20 7573 652e  for general use.
-00001e30: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001e40: 2020 5665 7273 696f 6e20 312e 332e 3135    Version 1.3.15
-00001e50: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-00001e60: 3032 2d31 3729 0a20 2020 2020 2020 200a  02-17).        .
-00001e70: 2020 2020 2020 2020 2d20 5265 6d6f 7665          - Remove
-00001e80: 2063 7573 746f 6d20 6d61 7267 696e 2066   custom margin f
-00001e90: 726f 6d20 636c 6173 7365 7320 746f 2069  rom classes to i
-00001ea0: 6d70 726f 7665 2043 5353 206f 7665 7272  mprove CSS overr
-00001eb0: 6964 6162 696c 6974 792e 0a20 2020 2020  idability..     
-00001ec0: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00001ed0: 696f 6e20 312e 332e 3134 2028 7265 6c65  ion 1.3.14 (rele
-00001ee0: 6173 6564 2032 3032 322d 3032 2d31 3629  ased 2022-02-16)
-00001ef0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001f00: 2020 2d20 4669 7820 6973 7375 6520 7769    - Fix issue wi
-00001f10: 7468 204c 6174 6f20 666f 6e74 206e 6f74  th Lato font not
-00001f20: 2062 6569 6e67 206c 6f61 6465 6420 696e   being loaded in
-00001f30: 2053 656d 616e 7469 6320 5549 2074 6865   Semantic UI the
-00001f40: 6d65 2e0a 2020 2020 2020 2020 2d20 5365  me..        - Se
-00001f50: 7473 2053 656d 616e 7469 6320 5549 2040  ts Semantic UI @
-00001f60: 6d75 7465 6454 6578 7443 6f6c 6f72 2e0a  mutedTextColor..
-00001f70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001f80: 2056 6572 7369 6f6e 2031 2e33 2e31 3320   Version 1.3.13 
-00001f90: 2872 656c 6561 7365 6420 3230 3232 2d30  (released 2022-0
-00001fa0: 322d 3136 290a 2020 2020 2020 2020 0a20  2-16).        . 
-00001fb0: 2020 2020 2020 202d 2045 6e73 7572 6520         - Ensure 
-00001fc0: 636f 6d70 696c 6564 2074 7261 6e73 6c61  compiled transla
-00001fd0: 7469 6f6e 206d 6573 7361 6765 2063 6174  tion message cat
-00001fe0: 616c 6f67 7320 6172 6520 696e 636c 7564  alogs are includ
-00001ff0: 6564 2069 6e20 7468 650a 2020 2020 2020  ed in the.      
-00002000: 2020 2020 6469 7374 7269 6275 7469 6f6e      distribution
-00002010: 7320 7570 6c6f 6164 6564 206f 6e20 5079  s uploaded on Py
-00002020: 5049 2e0a 2020 2020 2020 2020 0a20 2020  PI..        .   
-00002030: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
-00002040: 2e31 3220 2872 656c 6561 7365 6420 3230  .12 (released 20
-00002050: 3232 2d30 322d 3134 290a 2020 2020 2020  22-02-14).      
-00002060: 2020 0a20 2020 2020 2020 202d 2046 6978    .        - Fix
-00002070: 6573 2041 3131 7920 6973 7375 6520 7769  es A11y issue wi
-00002080: 7468 2074 6865 2063 6c6f 7365 2062 7574  th the close but
-00002090: 746f 6e20 696e 2066 6c61 7368 206d 6573  ton in flash mes
-000020a0: 7361 6765 732e 0a20 2020 2020 2020 200a  sages..        .
-000020b0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-000020c0: 312e 332e 3131 2028 7265 6c65 6173 6564  1.3.11 (released
-000020d0: 2032 3032 322d 3032 2d30 3829 0a20 2020   2022-02-08).   
-000020e0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-000020f0: 4164 6473 206d 6172 6769 6e20 6765 6e65  Adds margin gene
-00002100: 7261 746f 722e 0a20 2020 2020 2020 202d  rator..        -
-00002110: 2041 6464 7320 4131 3179 2070 6167 6520   Adds A11y page 
-00002120: 6c61 6e64 6d61 726b 732e 0a20 2020 2020  landmarks..     
-00002130: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00002140: 696f 6e20 312e 332e 3130 2028 7265 6c65  ion 1.3.10 (rele
-00002150: 6173 6564 2032 3032 312d 3131 2d32 3329  ased 2021-11-23)
-00002160: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002170: 2020 2d20 5765 6220 6163 6365 7373 6962    - Web accessib
-00002180: 696c 6974 7920 6669 782e 0a20 2020 2020  ility fix..     
-00002190: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-000021a0: 696f 6e20 312e 332e 3920 2872 656c 6561  ion 1.3.9 (relea
-000021b0: 7365 6420 3230 3231 2d30 372d 3132 290a  sed 2021-07-12).
-000021c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000021d0: 202d 2041 6464 7320 6765 726d 616e 2074   - Adds german t
-000021e0: 7261 6e73 6c61 7469 6f6e 730a 2020 2020  ranslations.    
-000021f0: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00002200: 7369 6f6e 2031 2e33 2e38 2028 7265 6c65  sion 1.3.8 (rele
-00002210: 6173 6564 2032 3032 312d 3032 2d31 3029  ased 2021-02-10)
-00002220: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002230: 2020 2d20 4164 6473 2062 7261 6e64 2063    - Adds brand c
-00002240: 6f6c 6f72 2074 6f20 6d65 6e75 2069 7465  olor to menu ite
-00002250: 6d73 0a20 2020 2020 2020 200a 2020 2020  ms.        .    
-00002260: 2020 2020 5665 7273 696f 6e20 312e 332e      Version 1.3.
-00002270: 3720 2872 656c 6561 7365 6420 3230 3231  7 (released 2021
-00002280: 2d30 312d 3235 290a 2020 2020 2020 2020  -01-25).        
-00002290: 0a20 2020 2020 2020 202d 2041 6464 7320  .        - Adds 
-000022a0: 6272 616e 6420 636f 6c6f 7220 696e 2073  brand color in s
-000022b0: 6567 6d65 6e74 730a 2020 2020 2020 2020  egments.        
-000022c0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-000022d0: 2031 2e33 2e36 2028 7265 6c65 6173 6564   1.3.6 (released
-000022e0: 2032 3032 312d 3031 2d30 3429 0a20 2020   2021-01-04).   
-000022f0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00002300: 4164 6473 2060 6c69 6e6b 6020 7468 656d  Adds `link` them
-00002310: 6520 6963 6f6e 0a20 2020 2020 2020 202d  e icon.        -
-00002320: 2046 6978 6573 2077 696c 6463 6172 6420   Fixes wildcard 
-00002330: 6963 6f6e 2072 6573 6f6c 7574 696f 6e0a  icon resolution.
-00002340: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002350: 2056 6572 7369 6f6e 2031 2e33 2e35 2028   Version 1.3.5 (
-00002360: 7265 6c65 6173 6564 2032 3032 302d 3132  released 2020-12
-00002370: 2d31 3729 0a20 2020 2020 2020 200a 2020  -17).        .  
-00002380: 2020 2020 2020 2d20 4669 7865 7320 6368        - Fixes ch
-00002390: 6563 6b62 6f78 2e6f 7665 7272 6964 6573  eckbox.overrides
-000023a0: 2069 6e20 6069 6e76 656e 696f 6020 5355   in `invenio` SU
-000023b0: 4920 7061 636b 6167 6564 2074 6865 6d65  I packaged theme
-000023c0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000023d0: 2020 2056 6572 7369 6f6e 2031 2e33 2e34     Version 1.3.4
-000023e0: 2028 7265 6c65 6173 6564 2032 3032 302d   (released 2020-
-000023f0: 3132 2d31 3729 0a20 2020 2020 2020 200a  12-17).        .
-00002400: 2020 2020 2020 2020 2d20 4164 6473 2061          - Adds a
-00002410: 2066 756c 6c20 2269 6e76 656e 696f 2220   full "invenio" 
-00002420: 5365 6d61 6e74 6963 2055 4920 7061 636b  Semantic UI pack
-00002430: 6167 6564 2074 6865 6d65 2073 6f20 7765  aged theme so we
-00002440: 2063 616e 2065 6173 6965 7220 6375 7374   can easier cust
-00002450: 6f6d 697a 650a 2020 2020 2020 2020 2020  omize.          
-00002460: 6c61 796f 7574 2069 6e20 7468 6520 6675  layout in the fu
-00002470: 7475 7265 2e0a 2020 2020 2020 2020 0a20  ture..        . 
-00002480: 2020 2020 2020 202d 204d 6f76 6573 2074         - Moves t
-00002490: 6865 6d65 2e63 6f6e 6669 6720 746f 2074  heme.config to t
-000024a0: 6865 6d65 2e63 6f6e 6669 672e 6578 616d  heme.config.exam
-000024b0: 706c 6520 616e 6420 6164 6473 2061 206e  ple and adds a n
-000024c0: 6f74 6520 746f 206d 616b 6520 6974 0a20  ote to make it. 
-000024d0: 2020 2020 2020 2020 2063 6c65 6172 2074           clear t
-000024e0: 6865 2066 696c 6520 6973 206e 6f74 2061  he file is not a
-000024f0: 6374 7561 6c6c 7920 7573 6564 2c20 6275  ctually used, bu
-00002500: 7420 6973 206a 7573 7420 616e 2065 7861  t is just an exa
-00002510: 6d70 6c65 2e0a 2020 2020 2020 2020 0a20  mple..        . 
-00002520: 2020 2020 2020 202d 2041 6464 7320 6865         - Adds he
-00002530: 6c70 6572 2074 6f6f 6c20 666f 7220 7375  lper tool for su
-00002540: 7070 6f72 7469 6e67 2074 6865 6d65 2064  pporting theme d
-00002550: 6570 656e 6465 6e74 2069 636f 6e73 2e0a  ependent icons..
-00002560: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002570: 202d 2046 6978 6573 206d 616e 7920 6d69   - Fixes many mi
-00002580: 6e6f 7220 7374 796c 696e 6720 6973 7375  nor styling issu
-00002590: 6573 2073 7563 6820 6173 2061 6c69 676e  es such as align
-000025a0: 6d65 6e74 732c 2062 7574 746f 6e20 6c6f  ments, button lo
-000025b0: 6361 7469 6f6e 732c 0a20 2020 2020 2020  cations,.       
-000025c0: 2020 2067 7269 6473 2e0a 2020 2020 2020     grids..      
-000025d0: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-000025e0: 6f6e 2031 2e33 2e33 2028 7265 6c65 6173  on 1.3.3 (releas
-000025f0: 6564 2032 3032 302d 3132 2d31 3129 0a20  ed 2020-12-11). 
-00002600: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002610: 2d20 496e 6974 6961 6c69 7a65 7320 7365  - Initializes se
-00002620: 6d61 6e74 6963 5549 2061 6363 6f72 6469  manticUI accordi
-00002630: 6f6e 2063 6f6d 706f 6e65 6e74 732e 0a20  on components.. 
-00002640: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002650: 5665 7273 696f 6e20 312e 332e 3220 2872  Version 1.3.2 (r
-00002660: 656c 6561 7365 6420 3230 3230 2d31 322d  eleased 2020-12-
-00002670: 3131 290a 2020 2020 2020 2020 0a20 2020  11).        .   
-00002680: 2020 2020 202d 2055 7064 6174 6573 2074       - Updates t
-00002690: 6865 2049 6e76 656e 696f 206c 6f67 6f20  he Invenio logo 
-000026a0: 616e 6420 7265 6d6f 7665 206f 7574 6461  and remove outda
-000026b0: 7465 6420 7665 7273 696f 6e73 2e0a 2020  ted versions..  
-000026c0: 2020 2020 2020 2d20 4669 7865 7320 7468        - Fixes th
-000026d0: 6520 6472 6f70 646f 776e 2074 6f20 776f  e dropdown to wo
-000026e0: 726b 206f 6e20 7468 6520 7573 6572 2070  rk on the user p
-000026f0: 726f 6669 6c65 2070 6167 652e 0a20 2020  rofile page..   
-00002700: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-00002710: 7273 696f 6e20 312e 332e 3120 2872 656c  rsion 1.3.1 (rel
-00002720: 6561 7365 6420 3230 3230 2d31 322d 3039  eased 2020-12-09
-00002730: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002740: 2020 202d 204d 696e 6f72 2066 6978 2066     - Minor fix f
-00002750: 6f72 2053 656d 616e 7469 6355 4920 6472  or SemanticUI dr
-00002760: 6f70 646f 776e 730a 2020 2020 2020 2020  opdowns.        
-00002770: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-00002780: 2031 2e33 2e30 2028 7265 6c65 6173 6564   1.3.0 (released
-00002790: 2032 3032 302d 3132 2d30 3929 0a20 2020   2020-12-09).   
-000027a0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-000027b0: 4d61 6a6f 723a 204e 6577 2053 656d 616e  Major: New Seman
-000027c0: 7469 6355 4920 7468 656d 6520 6861 7320  ticUI theme has 
-000027d0: 6265 656e 2069 6e74 6567 7261 7465 642e  been integrated.
-000027e0: 2054 6865 2042 6f6f 7473 7472 6170 2033   The Bootstrap 3
-000027f0: 2074 6865 6d65 2073 7469 6c6c 0a20 2020   theme still.   
-00002800: 2020 2020 2020 2065 7869 7374 732e 2054         exists. T
-00002810: 6869 7320 6368 616e 6765 2064 6570 656e  his change depen
-00002820: 6473 206f 6e20 7468 6520 6c61 7465 7374  ds on the latest
-00002830: 2072 656c 6561 7365 6420 496e 7665 6e69   released Inveni
-00002840: 6f2d 4173 7365 7473 2077 6869 6368 0a20  o-Assets which. 
-00002850: 2020 2020 2020 2020 2061 6464 7320 7375           adds su
-00002860: 7070 6f72 7473 2066 6f72 206d 756c 7469  pports for multi
-00002870: 706c 6520 5549 2066 7261 6d65 776f 726b  ple UI framework
-00002880: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00002890: 2020 2020 2d20 4164 6473 2073 7570 706f      - Adds suppo
-000028a0: 7274 2066 6f72 2064 796e 616d 6963 206c  rt for dynamic l
-000028b0: 6f61 6469 6e67 206f 6620 7465 6d70 6c61  oading of templa
-000028c0: 7465 7320 666f 7220 5265 6163 742d 4f76  tes for React-Ov
-000028d0: 6572 7269 6461 626c 652e 0a20 2020 2020  erridable..     
-000028e0: 2020 200a 2020 2020 2020 2020 2d20 4261     .        - Ba
-000028f0: 636b 7761 7264 7320 696e 636f 6d70 6174  ckwards incompat
-00002900: 6962 6c65 3a20 5468 6520 6f6c 642d 7374  ible: The old-st
-00002910: 796c 6520 466c 6173 6b2d 4173 7365 7420  yle Flask-Asset 
-00002920: 6275 6e64 6c65 7320 7761 7320 7265 6d6f  bundles was remo
-00002930: 7665 6420 2874 6865 7365 0a20 2020 2020  ved (these.     
-00002940: 2020 2020 2062 756e 646c 6573 2077 6572       bundles wer
-00002950: 6520 6465 7072 6563 6174 6564 2069 6e20  e deprecated in 
-00002960: 496e 7665 6e69 6f20 7633 2e31 292e 0a20  Invenio v3.1).. 
-00002970: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002980: 2d20 4164 6473 2054 7572 6b69 7368 2074  - Adds Turkish t
-00002990: 7261 6e73 6c61 7469 6f6e 732e 0a20 2020  ranslations..   
-000029a0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-000029b0: 7273 696f 6e20 312e 322e 3020 2872 656c  rsion 1.2.0 (rel
-000029c0: 6561 7365 6420 3230 3230 2d30 332d 3230  eased 2020-03-20
-000029d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000029e0: 2020 202d 2052 6570 6c61 6365 7320 466c     - Replaces Fl
-000029f0: 6173 6b20 6465 7065 6e64 656e 6379 2077  ask dependency w
-00002a00: 6974 6820 6060 696e 7665 6e69 6f2d 6261  ith ``invenio-ba
-00002a10: 7365 6060 2e0a 2020 2020 2020 2020 0a20  se``..        . 
-00002a20: 2020 2020 2020 2056 6572 7369 6f6e 2031         Version 1
-00002a30: 2e31 2e34 2028 7265 6c65 6173 6564 2032  .1.4 (released 2
-00002a40: 3031 392d 3037 2d32 3229 0a20 2020 2020  019-07-22).     
-00002a50: 2020 200a 2020 2020 2020 2020 2d20 496e     .        - In
-00002a60: 7472 6f64 7563 6520 6861 6e64 6c69 6e67  troduce handling
-00002a70: 206f 6620 7468 6520 6572 726f 7220 3432   of the error 42
-00002a80: 392e 0a20 2020 2020 2020 200a 2020 2020  9..        .    
-00002a90: 2020 2020 5665 7273 696f 6e20 312e 312e      Version 1.1.
-00002aa0: 3320 2872 656c 6561 7365 6420 3230 3139  3 (released 2019
-00002ab0: 2d30 332d 3133 290a 2020 2020 2020 2020  -03-13).        
-00002ac0: 0a20 2020 2020 2020 202d 2052 6573 7472  .        - Restr
-00002ad0: 7563 7475 7265 2053 4353 5320 6669 6c65  ucture SCSS file
-00002ae0: 732c 2069 6e20 6f72 6465 7220 746f 2061  s, in order to a
-00002af0: 6c6c 6f77 2065 6173 6965 7220 6375 7374  llow easier cust
-00002b00: 6f6d 697a 6174 696f 6e20 616e 6420 6578  omization and ex
-00002b10: 7465 6e73 696f 6e0a 2020 2020 2020 2020  tension.        
-00002b20: 2020 696e 206f 7665 726c 6179 732e 0a20    in overlays.. 
-00002b30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002b40: 5665 7273 696f 6e20 312e 312e 3220 2872  Version 1.1.2 (r
-00002b50: 656c 6561 7365 6420 3230 3139 2d30 322d  eleased 2019-02-
-00002b60: 3135 290a 2020 2020 2020 2020 0a20 2020  15).        .   
-00002b70: 2020 2020 202d 2055 7067 7261 6465 6420       - Upgraded 
-00002b80: 6d6f 6d65 6e74 2074 6f20 322e 3233 2e30  moment to 2.23.0
-00002b90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002ba0: 2020 5665 7273 696f 6e20 312e 312e 3120    Version 1.1.1 
-00002bb0: 2872 656c 6561 7365 6420 3230 3138 2d31  (released 2018-1
-00002bc0: 322d 3035 290a 2020 2020 2020 2020 0a20  2-05).        . 
-00002bd0: 2020 2020 2020 202d 2046 6978 6573 2069         - Fixes i
-00002be0: 7373 7565 7320 7769 7468 2077 6562 7061  ssues with webpa
-00002bf0: 636b 2061 6e64 2074 6865 2041 646d 696e  ck and the Admin
-00002c00: 4c54 4520 7468 656d 652e 0a20 2020 2020  LTE theme..     
-00002c10: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00002c20: 696f 6e20 312e 312e 3020 2872 656c 6561  ion 1.1.0 (relea
-00002c30: 7365 6420 3230 3138 2d31 312d 3036 290a  sed 2018-11-06).
-00002c40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002c50: 202d 2049 6e74 726f 6475 6365 2077 6562   - Introduce web
-00002c60: 7061 636b 2073 7570 706f 7274 2e0a 2020  pack support..  
-00002c70: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
-00002c80: 6572 7369 6f6e 2031 2e30 2e30 2028 7265  ersion 1.0.0 (re
-00002c90: 6c65 6173 6564 2032 3031 382d 3033 2d32  leased 2018-03-2
-00002ca0: 3329 0a20 2020 2020 2020 200a 2020 2020  3).        .    
-00002cb0: 2020 2020 2d20 496e 6974 6961 6c20 7075      - Initial pu
-00002cc0: 626c 6963 2072 656c 6561 7365 2e0a 2020  blic release..  
-00002cd0: 2020 2020 2020 0a4b 6579 776f 7264 733a        .Keywords:
-00002ce0: 2069 6e76 656e 696f 0a50 6c61 7466 6f72   invenio.Platfor
-00002cf0: 6d3a 2061 6e79 0a43 6c61 7373 6966 6965  m: any.Classifie
-00002d00: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
-00002d10: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
-00002d20: 6475 6374 696f 6e2f 5374 6162 6c65 0a52  duction/Stable.R
-00002d30: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00002d40: 3e3d 332e 370a 5072 6f76 6964 6573 2d45  >=3.7.Provides-E
-00002d50: 7874 7261 3a20 7465 7374 730a 5072 6f76  xtra: tests.Prov
-00002d60: 6964 6573 2d45 7874 7261 3a20 646f 6373  ides-Extra: docs
-00002d70: 0a                                       .
+000007d0: 6572 7369 6f6e 2033 2e31 2e30 2028 7265  ersion 3.1.0 (re
+000007e0: 6c65 6173 6564 2032 3032 342d 3034 2d31  leased 2024-04-1
+000007f0: 3029 0a20 2020 2020 2020 200a 2020 2020  0).        .    
+00000800: 2020 2020 2d20 6373 733a 2066 6978 206f      - css: fix o
+00000810: 7665 7266 6c6f 7720 666f 7220 6465 7363  verflow for desc
+00000820: 7269 7074 696f 6e20 696e 2072 6563 6f72  ription in recor
+00000830: 6420 6465 7461 696c 730a 2020 2020 2020  d details.      
+00000840: 2020 2d20 6275 673a 2061 6464 206d 6973    - bug: add mis
+00000850: 7369 6e67 2060 603c 7469 746c 653e 7360  sing ``<title>s`
+00000860: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
+00000870: 2020 2056 6572 7369 6f6e 2033 2e30 2e30     Version 3.0.0
+00000880: 2028 7265 6c65 6173 6564 2032 3032 342d   (released 2024-
+00000890: 3033 2d31 3929 0a20 2020 2020 2020 200a  03-19).        .
+000008a0: 2020 2020 2020 2020 2d20 676c 6f62 616c          - global
+000008b0: 3a20 7265 6d6f 7665 2062 7265 6164 6372  : remove breadcr
+000008c0: 756d 6220 7375 7070 6f72 740a 2020 2020  umb support.    
+000008d0: 2020 2020 2d20 676c 6f62 616c 3a20 696e      - global: in
+000008e0: 7472 6f64 7563 6520 7368 6172 6564 206d  troduce shared m
+000008f0: 656e 750a 2020 2020 2020 2020 2d20 676c  enu.        - gl
+00000900: 6f62 616c 3a20 7072 6570 6172 6174 696f  obal: preparatio
+00000910: 6e20 666f 7220 636f 6d70 6174 6962 696c  n for compatibil
+00000920: 6974 7920 7769 7468 2046 6c61 736b 2076  ity with Flask v
+00000930: 322e 332e 7820 6465 7072 6563 6174 696f  2.3.x deprecatio
+00000940: 6e73 0a20 2020 2020 2020 202d 2072 6566  ns.        - ref
+00000950: 6163 746f 723a 2063 7572 7265 6e74 5f74  actor: current_t
+00000960: 6865 6d65 5f69 636f 6e73 2077 6974 686f  heme_icons witho
+00000970: 7574 2061 7070 6c69 6361 7469 6f6e 2063  ut application c
+00000980: 6f6e 7465 7874 0a20 2020 2020 2020 200a  ontext.        .
+00000990: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+000009a0: 322e 352e 3130 2028 7265 6c65 6173 6564  2.5.10 (released
+000009b0: 2032 3032 342d 3031 2d32 3829 0a20 2020   2024-01-28).   
+000009c0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+000009d0: 696e 7374 616c 6c61 7469 6f6e 3a20 6669  installation: fi
+000009e0: 7820 7370 6869 6e78 2064 6570 656e 6465  x sphinx depende
+000009f0: 6e63 790a 2020 2020 2020 2020 0a20 2020  ncy.        .   
+00000a00: 2020 2020 2056 6572 7369 6f6e 2032 2e35       Version 2.5
+00000a10: 2e39 2028 7265 6c65 6173 6564 2032 3032  .9 (released 202
+00000a20: 342d 3031 2d32 3829 0a20 2020 2020 2020  4-01-28).       
+00000a30: 200a 2020 2020 2020 2020 2d20 676c 6f62   .        - glob
+00000a40: 616c 3a20 6368 616e 6765 206d 6174 6820  al: change math 
+00000a50: 6f70 6572 6174 696f 6e20 746f 2062 6520  operation to be 
+00000a60: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+00000a70: 7361 7373 322e 300a 2020 2020 2020 2020  sass2.0.        
+00000a80: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00000a90: 2032 2e35 2e38 2028 7265 6c65 6173 6564   2.5.8 (released
+00000aa0: 2032 3032 332d 3132 2d31 3229 0a20 2020   2023-12-12).   
+00000ab0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00000ac0: 7265 706c 6163 6520 636b 6564 6974 6f72  replace ckeditor
+00000ad0: 2077 6974 6820 7469 6e79 6d63 6520 6475   with tinymce du
+00000ae0: 6520 746f 206c 6963 656e 7365 2069 7373  e to license iss
+00000af0: 7565 0a20 2020 2020 2020 200a 2020 2020  ue.        .    
+00000b00: 2020 2020 5665 7273 696f 6e20 322e 352e      Version 2.5.
+00000b10: 3720 2872 656c 6561 7365 6420 3230 3233  7 (released 2023
+00000b20: 2d31 302d 3236 290a 2020 2020 2020 2020  -10-26).        
+00000b30: 0a20 2020 2020 2020 202d 2063 6f6d 6d75  .        - commu
+00000b40: 6e69 7479 206c 6f67 6f3a 2066 6978 2072  nity logo: fix r
+00000b50: 656e 6465 7269 6e67 2061 2070 6c61 6365  endering a place
+00000b60: 686f 6c64 6572 0a20 2020 2020 2020 200a  holder.        .
+00000b70: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00000b80: 322e 352e 3620 2872 656c 6561 7365 6420  2.5.6 (released 
+00000b90: 3230 3233 2d31 302d 3230 290a 2020 2020  2023-10-20).    
+00000ba0: 2020 2020 0a20 2020 2020 2020 202d 2064      .        - d
+00000bb0: 6f6e 2774 206f 7665 7272 6964 6520 6c69  on't override li
+00000bc0: 6e6b 7320 7374 796c 6520 696e 2066 6c61  nks style in fla
+00000bd0: 7368 6564 206d 6573 7361 6765 730a 2020  shed messages.  
+00000be0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+00000bf0: 6572 7369 6f6e 2032 2e35 2e35 2028 7265  ersion 2.5.5 (re
+00000c00: 6c65 6173 6564 2032 3032 332d 3039 2d31  leased 2023-09-1
+00000c10: 3929 0a20 2020 2020 2020 200a 2020 2020  9).        .    
+00000c20: 2020 2020 2d20 7374 796c 696e 673a 2061      - styling: a
+00000c30: 6464 2033 2063 6f6c 756d 6e20 7465 6d70  dd 3 column temp
+00000c40: 6c61 7465 2063 6c61 7373 0a20 2020 2020  late class.     
+00000c50: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00000c60: 696f 6e20 322e 352e 3420 2872 656c 6561  ion 2.5.4 (relea
+00000c70: 7365 6420 3230 3233 2d30 392d 3131 290a  sed 2023-09-11).
+00000c80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000c90: 202d 2073 6373 733a 2066 6978 2063 6f6d   - scss: fix com
+00000ca0: 7061 7469 6269 6c69 7479 2077 6974 6820  patibility with 
+00000cb0: 6c61 7465 7374 206c 6573 7320 7665 7273  latest less vers
+00000cc0: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
+00000cd0: 2020 2020 2056 6572 7369 6f6e 2032 2e35       Version 2.5
+00000ce0: 2e33 2028 7265 6c65 6173 6564 2032 3032  .3 (released 202
+00000cf0: 332d 3038 2d30 3829 0a20 2020 2020 2020  3-08-08).       
+00000d00: 200a 2020 2020 2020 2020 2d20 7374 796c   .        - styl
+00000d10: 6573 6865 6574 733a 2061 6464 2070 7265  esheets: add pre
+00000d20: 666f 726d 6174 7465 6420 7461 6720 7374  formatted tag st
+00000d30: 796c 696e 6720 666f 6e74 0a20 2020 2020  yling font.     
+00000d40: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00000d50: 696f 6e20 322e 352e 3220 2872 656c 6561  ion 2.5.2 (relea
+00000d60: 7365 6420 3230 3233 2d30 382d 3134 290a  sed 2023-08-14).
+00000d70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000d80: 202d 2069 6e73 7461 6c6c 6174 696f 6e3a   - installation:
+00000d90: 2070 696e 2046 6c61 736b 2d4d 656e 7520   pin Flask-Menu 
+00000da0: 746f 2060 603c 7631 2e30 2e30 6060 2e0a  to ``<v1.0.0``..
+00000db0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000dc0: 2056 6572 7369 6f6e 2032 2e35 2e31 2028   Version 2.5.1 (
+00000dd0: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
+00000de0: 2d31 3429 0a20 2020 2020 2020 200a 2020  -14).        .  
+00000df0: 2020 2020 2020 2d20 7468 656d 653a 2062        - theme: b
+00000e00: 7567 6669 7820 746f 2064 6563 7265 6173  ugfix to decreas
+00000e10: 6520 7a2d 696e 6465 7820 7661 6c75 650a  e z-index value.
+00000e20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000e30: 2056 6572 7369 6f6e 2032 2e35 2e30 2028   Version 2.5.0 (
+00000e40: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
+00000e50: 2d30 3929 0a20 2020 2020 2020 200a 2020  -09).        .  
+00000e60: 2020 2020 2020 2d20 7468 656d 653a 2061        - theme: a
+00000e70: 6464 2075 7469 6c69 7479 2063 6c61 7373  dd utility class
+00000e80: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
+00000e90: 2020 2020 5665 7273 696f 6e20 322e 342e      Version 2.4.
+00000ea0: 3020 2872 656c 6561 7365 6420 3230 3233  0 (released 2023
+00000eb0: 2d30 382d 3032 290a 2020 2020 2020 2020  -08-02).        
+00000ec0: 0a20 2020 2020 2020 202d 2074 6865 6d65  .        - theme
+00000ed0: 3a20 6164 6420 736f 6d65 2067 656e 6572  : add some gener
+00000ee0: 616c 2063 6c61 7373 6573 2061 6e64 2066  al classes and f
+00000ef0: 6978 6573 2061 6c69 676e 6d65 6e74 2066  ixes alignment f
+00000f00: 6f72 206c 6162 656c 6564 2066 6c75 6964  or labeled fluid
+00000f10: 2062 7574 746f 6e73 0a20 2020 2020 2020   buttons.       
+00000f20: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
+00000f30: 6e20 322e 332e 3020 2872 656c 6561 7365  n 2.3.0 (release
+00000f40: 6420 3230 3233 2d30 372d 3331 290a 2020  d 2023-07-31).  
+00000f50: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00000f60: 2073 6574 7469 6e67 7320 7061 6765 3a20   settings page: 
+00000f70: 496d 7072 6f76 6520 7465 6d70 6c61 7465  Improve template
+00000f80: 2066 6f72 2061 3131 790a 2020 2020 2020   for a11y.      
+00000f90: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
+00000fa0: 6f6e 2032 2e32 2e30 2028 7265 6c65 6173  on 2.2.0 (releas
+00000fb0: 6564 2032 3032 332d 3037 2d32 3629 0a20  ed 2023-07-26). 
+00000fc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000fd0: 2d20 7468 656d 653a 2061 6464 2067 656e  - theme: add gen
+00000fe0: 6572 616c 2073 7479 6c65 2069 6d70 726f  eral style impro
+00000ff0: 7665 6d65 6e74 730a 2020 2020 2020 2020  vements.        
+00001000: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00001010: 2032 2e31 2e33 2028 7265 6c65 6173 6564   2.1.3 (released
+00001020: 2032 3032 332d 3037 2d32 3429 0a20 2020   2023-07-24).   
+00001030: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001040: 6d65 7373 6167 6573 3a20 6164 6420 7a2d  messages: add z-
+00001050: 696e 6465 780a 2020 2020 2020 2020 0a20  index.        . 
+00001060: 2020 2020 2020 2056 6572 7369 6f6e 2032         Version 2
+00001070: 2e31 2e32 2028 7265 6c65 6173 6564 2032  .1.2 (released 2
+00001080: 3032 332d 3034 2d31 3229 0a20 2020 2020  023-04-12).     
+00001090: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
+000010a0: 6420 666c 6578 2075 7469 6c69 7479 2063  d flex utility c
+000010b0: 6c61 7373 6573 0a20 2020 2020 2020 202d  lasses.        -
+000010c0: 2061 6464 2074 6578 7420 7369 7a65 7320   add text sizes 
+000010d0: 636c 6173 7365 730a 2020 2020 2020 2020  classes.        
+000010e0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+000010f0: 2032 2e31 2e31 2028 7265 6c65 6173 6564   2.1.1 (released
+00001100: 2032 3032 332d 3034 2d30 3629 0a20 2020   2023-04-06).   
+00001110: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001120: 6164 6420 6469 7370 6c61 7920 7574 696c  add display util
+00001130: 6974 7920 636c 6173 7365 730a 2020 2020  ity classes.    
+00001140: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00001150: 7369 6f6e 2032 2e31 2e30 2028 7265 6c65  sion 2.1.0 (rele
+00001160: 6173 6564 2032 3032 332d 3033 2d32 3829  ased 2023-03-28)
+00001170: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001180: 2020 2d20 6164 6420 676c 6f62 616c 2075    - add global u
+00001190: 7469 6c69 7479 2073 7479 6c69 6e67 2063  tility styling c
+000011a0: 6c61 7373 6573 0a20 2020 2020 2020 200a  lasses.        .
+000011b0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+000011c0: 322e 302e 3120 2872 656c 6561 7365 6420  2.0.1 (released 
+000011d0: 3230 3233 2d30 332d 3039 290a 2020 2020  2023-03-09).    
+000011e0: 2020 2020 0a20 2020 2020 2020 202d 2066      .        - f
+000011f0: 6978 2073 7479 6c69 6e67 2066 6f72 2062  ix styling for b
+00001200: 7574 746f 6e73 0a20 2020 2020 2020 202d  uttons.        -
+00001210: 206d 6f76 6520 676c 6f62 616c 2063 6c61   move global cla
+00001220: 7373 2066 6f72 2061 7574 6f20 6772 6964  ss for auto grid
+00001230: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001240: 2020 5665 7273 696f 6e20 322e 302e 3020    Version 2.0.0 
+00001250: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
+00001260: 322d 3238 290a 2020 2020 2020 2020 0a20  2-28).        . 
+00001270: 2020 2020 2020 202d 2064 726f 7020 7079         - drop py
+00001280: 7468 6f6e 2032 2e37 2073 7570 706f 7274  thon 2.7 support
+00001290: 0a20 2020 2020 2020 202d 2072 656d 6f76  .        - remov
+000012a0: 6520 666c 6173 6b5f 6261 6265 6c65 7820  e flask_babelex 
+000012b0: 696d 706f 7274 730a 2020 2020 2020 2020  imports.        
+000012c0: 2d20 7570 6772 6164 6520 696e 7665 6e69  - upgrade inveni
+000012d0: 6f5f 6931 386e 0a20 2020 2020 2020 200a  o_i18n.        .
+000012e0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+000012f0: 312e 342e 3820 2872 656c 6561 7365 6420  1.4.8 (released 
+00001300: 3230 3233 2d30 322d 3037 290a 2020 2020  2023-02-07).    
+00001310: 2020 2020 0a20 2020 2020 2020 202d 2074      .        - t
+00001320: 6865 6d65 3a20 6164 6420 6175 746f 2d63  heme: add auto-c
+00001330: 6f6c 756d 6e2d 6772 6964 2063 6c61 7373  olumn-grid class
+00001340: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001350: 2020 5665 7273 696f 6e20 312e 342e 3720    Version 1.4.7 
+00001360: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
+00001370: 312d 3035 290a 2020 2020 2020 2020 0a20  1-05).        . 
+00001380: 2020 2020 2020 202d 2061 6464 2074 7275         - add tru
+00001390: 6e63 6174 6520 6c69 6e65 7320 7374 796c  ncate lines styl
+000013a0: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
+000013b0: 2020 2020 5665 7273 696f 6e20 312e 342e      Version 1.4.
+000013c0: 3620 2872 656c 6561 7365 6420 3230 3232  6 (released 2022
+000013d0: 2d31 322d 3038 290a 2020 2020 2020 2020  -12-08).        
+000013e0: 0a20 2020 2020 2020 202d 2066 6978 2073  .        - fix s
+000013f0: 7479 6c69 6e67 2066 6f72 2069 6e6c 696e  tyling for inlin
+00001400: 6520 636c 6173 732c 2061 6666 6563 7469  e class, affecti
+00001410: 6e67 2066 6f72 6d20 6669 656c 6473 0a20  ng form fields. 
+00001420: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001430: 5665 7273 696f 6e20 312e 342e 3520 2872  Version 1.4.5 (r
+00001440: 656c 6561 7365 6420 3230 3232 2d31 322d  eleased 2022-12-
+00001450: 3031 290a 2020 2020 2020 2020 0a20 2020  01).        .   
+00001460: 2020 2020 202d 2066 6978 2073 6561 7263       - fix searc
+00001470: 6820 7265 7375 6c74 2069 7465 6d20 7374  h result item st
+00001480: 796c 696e 670a 2020 2020 2020 2020 2d20  yling.        - 
+00001490: 6164 6420 676c 6f62 616c 2062 6568 6176  add global behav
+000014a0: 696f 7572 2063 6c61 7373 6573 0a20 2020  iour classes.   
+000014b0: 2020 2020 202d 2061 6464 2070 6c61 6365       - add place
+000014c0: 686f 6c64 6572 2069 6d61 6765 2068 616e  holder image han
+000014d0: 646c 650a 2020 2020 2020 2020 0a20 2020  dle.        .   
+000014e0: 2020 2020 2056 6572 7369 6f6e 2031 2e34       Version 1.4
+000014f0: 2e34 2028 7265 6c65 6173 6564 2032 3032  .4 (released 202
+00001500: 322d 3131 2d31 3829 0a20 2020 2020 2020  2-11-18).       
+00001510: 200a 2020 2020 2020 2020 2d20 4164 6420   .        - Add 
+00001520: 7075 6c6c 6564 2074 7261 6e73 6c61 7469  pulled translati
+00001530: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+00001540: 2020 2020 2056 6572 7369 6f6e 2031 2e34       Version 1.4
+00001550: 2e33 2028 7265 6c65 6173 6564 2032 3032  .3 (released 202
+00001560: 322d 3131 2d30 3329 0a20 2020 2020 2020  2-11-03).       
+00001570: 200a 2020 2020 2020 2020 2d20 6164 6420   .        - add 
+00001580: 7374 796c 696e 6720 666f 7220 6472 6f70  styling for drop
+00001590: 646f 776e 206d 656e 7520 6974 656d 730a  down menu items.
+000015a0: 2020 2020 2020 2020 2d20 6669 7820 6d69          - fix mi
+000015b0: 7373 696e 6720 4d65 6469 6120 636f 6d70  ssing Media comp
+000015c0: 6f6e 656e 7420 7261 6e67 650a 2020 2020  onent range.    
+000015d0: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+000015e0: 7369 6f6e 2031 2e34 2e32 2028 7265 6c65  sion 1.4.2 (rele
+000015f0: 6173 6564 2032 3032 322d 3130 2d32 3629  ased 2022-10-26)
+00001600: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001610: 2020 2d20 6164 6420 4d65 6469 6120 746f    - add Media to
+00001620: 2073 7570 706f 7274 2072 6573 706f 6e73   support respons
+00001630: 6976 6520 7265 6163 7420 636f 6d70 6f6e  ive react compon
+00001640: 656e 7473 0a20 2020 2020 2020 200a 2020  ents.        .  
+00001650: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001660: 342e 3120 2872 656c 6561 7365 6420 3230  4.1 (released 20
+00001670: 3232 2d31 302d 3130 290a 2020 2020 2020  22-10-10).      
+00001680: 2020 0a20 2020 2020 2020 202d 2062 756d    .        - bum
+00001690: 7020 5365 6d61 6e74 6963 5549 0a20 2020  p SemanticUI.   
+000016a0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
+000016b0: 7273 696f 6e20 312e 342e 3020 2872 656c  rsion 1.4.0 (rel
+000016c0: 6561 7365 6420 3230 3232 2d31 302d 3035  eased 2022-10-05
+000016d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000016e0: 2020 202d 2063 6861 6e67 6520 676c 6f62     - change glob
+000016f0: 616c 2066 6f6e 7420 746f 204c 6174 6f0a  al font to Lato.
+00001700: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001710: 2056 6572 7369 6f6e 2031 2e33 2e33 3120   Version 1.3.31 
+00001720: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
+00001730: 302d 3035 290a 2020 2020 2020 2020 0a20  0-05).        . 
+00001740: 2020 2020 2020 202d 2061 6464 206d 6973         - add mis
+00001750: 7369 6e67 2074 6865 6d65 2076 6172 6961  sing theme varia
+00001760: 626c 6573 0a20 2020 2020 2020 200a 2020  bles.        .  
+00001770: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001780: 332e 3330 2028 7265 6c65 6173 6564 2032  3.30 (released 2
+00001790: 3032 322d 3039 2d32 3629 0a20 2020 2020  022-09-26).     
+000017a0: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
+000017b0: 6420 7374 796c 696e 6720 746f 2061 646d  d styling to adm
+000017c0: 696e 6973 7472 6174 696f 6e20 6461 7368  inistration dash
+000017d0: 626f 6172 6420 7061 6765 0a20 2020 2020  board page.     
+000017e0: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+000017f0: 696f 6e20 312e 332e 3239 2028 7265 6c65  ion 1.3.29 (rele
+00001800: 6173 6564 2032 3032 322d 3039 2d32 3229  ased 2022-09-22)
+00001810: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001820: 2020 2d20 6164 6420 6164 6d69 6e69 7374    - add administ
+00001830: 7261 7469 6f6e 2070 616e 656c 2073 7479  ration panel sty
+00001840: 6c69 6e67 0a20 2020 2020 2020 202d 2061  ling.        - a
+00001850: 6464 2074 7261 6e73 6c61 7469 6f6e 2077  dd translation w
+00001860: 6f72 6b66 6c6f 770a 2020 2020 2020 2020  orkflow.        
+00001870: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00001880: 2031 2e33 2e32 3820 2872 656c 6561 7365   1.3.28 (release
+00001890: 6420 3230 3232 2d30 372d 3038 290a 2020  d 2022-07-08).  
+000018a0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+000018b0: 2061 6464 2073 7479 6c69 6e67 2063 6c61   add styling cla
+000018c0: 7373 6573 2077 6974 6820 6163 7469 6f6e  sses with action
+000018d0: 2063 6f6c 6f72 2063 6f64 696e 670a 2020   color coding.  
+000018e0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+000018f0: 6572 7369 6f6e 2031 2e33 2e32 3720 2872  ersion 1.3.27 (r
+00001900: 656c 6561 7365 6420 3230 3232 2d30 372d  eleased 2022-07-
+00001910: 3037 290a 2020 2020 2020 2020 0a20 2020  07).        .   
+00001920: 2020 2020 202d 2066 6978 206a 7175 6572       - fix jquer
+00001930: 7920 7265 6665 7265 6e63 650a 2020 2020  y reference.    
+00001940: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00001950: 7369 6f6e 2031 2e33 2e32 3620 2872 656c  sion 1.3.26 (rel
+00001960: 6561 7365 6420 3230 3232 2d30 372d 3037  eased 2022-07-07
+00001970: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00001980: 2020 202d 2061 6464 2069 6d61 6765 2070     - add image p
+00001990: 6c61 6365 686f 6c64 6572 206f 6e20 6c6f  laceholder on lo
+000019a0: 6164 2065 7272 6f72 0a20 2020 2020 2020  ad error.       
+000019b0: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
+000019c0: 6e20 312e 332e 3235 2028 7265 6c65 6173  n 1.3.25 (releas
+000019d0: 6564 2032 3032 322d 3036 2d32 3729 0a20  ed 2022-06-27). 
+000019e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000019f0: 2d20 6164 6420 4765 726d 616e 2074 7261  - add German tra
+00001a00: 6e73 6c61 7469 6f6e 730a 2020 2020 2020  nslations.      
+00001a10: 2020 2d20 6669 7820 6472 6f70 646f 776e    - fix dropdown
+00001a20: 2073 6372 6f6c 6c20 6d69 7361 6c69 676e   scroll misalign
+00001a30: 6d65 6e74 0a20 2020 2020 2020 200a 2020  ment.        .  
+00001a40: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001a50: 332e 3234 2028 7265 6c65 6173 6564 2032  3.24 (released 2
+00001a60: 3032 322d 3035 2d32 3329 0a20 2020 2020  022-05-23).     
+00001a70: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
+00001a80: 6420 676c 6f62 616c 2043 5353 2063 6c61  d global CSS cla
+00001a90: 7373 6573 2066 6f72 206d 6172 6769 6e73  sses for margins
+00001aa0: 2061 7574 6f0a 2020 2020 2020 2020 0a20   auto.        . 
+00001ab0: 2020 2020 2020 2056 6572 7369 6f6e 2031         Version 1
+00001ac0: 2e33 2e32 3320 2872 656c 6561 7365 6420  .3.23 (released 
+00001ad0: 3230 3232 2d30 352d 3139 290a 2020 2020  2022-05-19).    
+00001ae0: 2020 2020 0a20 2020 2020 2020 202d 2061      .        - a
+00001af0: 6464 2061 6363 6573 7369 6269 6c69 7479  dd accessibility
+00001b00: 2074 6f20 7569 2d61 6363 6f72 6469 6f6e   to ui-accordion
+00001b10: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
+00001b20: 2020 2056 6572 7369 6f6e 2031 2e33 2e32     Version 1.3.2
+00001b30: 3220 2872 656c 6561 7365 6420 3230 3232  2 (released 2022
+00001b40: 2d30 342d 3231 290a 2020 2020 2020 2020  -04-21).        
+00001b50: 0a20 2020 2020 2020 202d 2069 6d70 726f  .        - impro
+00001b60: 7665 2073 656d 616e 7469 6320 7374 796c  ve semantic styl
+00001b70: 696e 6720 6f66 204d 7920 6163 636f 756e  ing of My accoun
+00001b80: 7420 7061 6765 0a20 2020 2020 2020 200a  t page.        .
+00001b90: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00001ba0: 312e 332e 3231 2028 7265 6c65 6173 6564  1.3.21 (released
+00001bb0: 2032 3032 322d 3033 2d32 3929 0a20 2020   2022-03-29).   
+00001bc0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001bd0: 6669 7820 6874 6d6c 2074 6167 7320 696e  fix html tags in
+00001be0: 2074 656d 706c 6174 6573 0a20 2020 2020   templates.     
+00001bf0: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00001c00: 696f 6e20 312e 332e 3230 2028 7265 6c65  ion 1.3.20 (rele
+00001c10: 6173 6564 2032 3032 322d 3033 2d31 3729  ased 2022-03-17)
+00001c20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001c30: 2020 2d20 7265 6661 6374 6f72 2070 6167    - refactor pag
+00001c40: 6520 7465 6d70 6c61 7465 0a20 2020 2020  e template.     
+00001c50: 2020 202d 2061 6464 2073 656d 616e 7469     - add semanti
+00001c60: 6320 7569 2069 6e76 656e 696f 2070 6163  c ui invenio pac
+00001c70: 6b61 6765 6420 7468 656d 6520 636f 6e66  kaged theme conf
+00001c80: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+00001c90: 2020 2d20 6578 7465 6e64 2075 7469 6c73    - extend utils
+00001ca0: 2043 5353 2063 6c61 7373 6573 0a20 2020   CSS classes.   
+00001cb0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
+00001cc0: 7273 696f 6e20 312e 332e 3139 2028 7265  rsion 1.3.19 (re
+00001cd0: 6c65 6173 6564 2032 3032 322d 3033 2d30  leased 2022-03-0
+00001ce0: 3429 0a20 2020 2020 2020 200a 2020 2020  4).        .    
+00001cf0: 2020 2020 2d20 4164 6420 6120 7265 7573      - Add a reus
+00001d00: 6162 6c65 204a 696e 6a61 206d 6163 726f  able Jinja macro
+00001d10: 2074 6f20 7472 756e 6361 7465 206c 6f6e   to truncate lon
+00001d20: 6720 7465 7874 2e0a 2020 2020 2020 2020  g text..        
+00001d30: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00001d40: 2031 2e33 2e31 3820 2872 656c 6561 7365   1.3.18 (release
+00001d50: 6420 3230 3232 2d30 332d 3031 290a 2020  d 2022-03-01).  
+00001d60: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00001d70: 2052 6576 6572 7420 666f 6e74 2062 6163   Revert font bac
+00001d80: 6b20 746f 2064 6566 6175 6c74 2073 616e  k to default san
+00001d90: 732d 7361 7269 6620 666f 6e74 2069 6e73  s-sarif font ins
+00001da0: 7465 6164 206f 6620 4c61 746f 2e0a 2020  tead of Lato..  
+00001db0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+00001dc0: 6572 7369 6f6e 2031 2e33 2e31 3720 2872  ersion 1.3.17 (r
+00001dd0: 656c 6561 7365 6420 3230 3232 2d30 322d  eleased 2022-02-
+00001de0: 3238 290a 2020 2020 2020 2020 0a20 2020  28).        .   
+00001df0: 2020 2020 202d 2041 6464 7320 6661 7669       - Adds favi
+00001e00: 636f 6e0a 2020 2020 2020 2020 2d20 4669  con.        - Fi
+00001e10: 7820 6973 7375 6520 7769 7468 2066 6c61  x issue with fla
+00001e20: 7368 206d 6573 7361 6765 206f 6e20 6c6f  sh message on lo
+00001e30: 6769 6e20 7061 6765 206e 6f74 2062 6569  gin page not bei
+00001e40: 6e67 2073 6964 6520 746f 2073 6964 652e  ng side to side.
+00001e50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001e60: 2020 5665 7273 696f 6e20 312e 332e 3136    Version 1.3.16
+00001e70: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
+00001e80: 3032 2d31 3729 0a20 2020 2020 2020 200a  02-17).        .
+00001e90: 2020 2020 2020 2020 2d20 4164 6420 636f          - Add co
+00001ea0: 6d6d 6f6e 2060 7371 7561 7265 2d70 6c61  mmon `square-pla
+00001eb0: 6365 686f 6c64 6572 2e70 6e67 6020 696d  ceholder.png` im
+00001ec0: 6167 6520 666f 7220 6765 6e65 7261 6c20  age for general 
+00001ed0: 7573 652e 0a20 2020 2020 2020 200a 2020  use..        .  
+00001ee0: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001ef0: 332e 3135 2028 7265 6c65 6173 6564 2032  3.15 (released 2
+00001f00: 3032 322d 3032 2d31 3729 0a20 2020 2020  022-02-17).     
+00001f10: 2020 200a 2020 2020 2020 2020 2d20 5265     .        - Re
+00001f20: 6d6f 7665 2063 7573 746f 6d20 6d61 7267  move custom marg
+00001f30: 696e 2066 726f 6d20 636c 6173 7365 7320  in from classes 
+00001f40: 746f 2069 6d70 726f 7665 2043 5353 206f  to improve CSS o
+00001f50: 7665 7272 6964 6162 696c 6974 792e 0a20  verridability.. 
+00001f60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001f70: 5665 7273 696f 6e20 312e 332e 3134 2028  Version 1.3.14 (
+00001f80: 7265 6c65 6173 6564 2032 3032 322d 3032  released 2022-02
+00001f90: 2d31 3629 0a20 2020 2020 2020 200a 2020  -16).        .  
+00001fa0: 2020 2020 2020 2d20 4669 7820 6973 7375        - Fix issu
+00001fb0: 6520 7769 7468 204c 6174 6f20 666f 6e74  e with Lato font
+00001fc0: 206e 6f74 2062 6569 6e67 206c 6f61 6465   not being loade
+00001fd0: 6420 696e 2053 656d 616e 7469 6320 5549  d in Semantic UI
+00001fe0: 2074 6865 6d65 2e0a 2020 2020 2020 2020   theme..        
+00001ff0: 2d20 5365 7473 2053 656d 616e 7469 6320  - Sets Semantic 
+00002000: 5549 2040 6d75 7465 6454 6578 7443 6f6c  UI @mutedTextCol
+00002010: 6f72 2e0a 2020 2020 2020 2020 0a20 2020  or..        .   
+00002020: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
+00002030: 2e31 3320 2872 656c 6561 7365 6420 3230  .13 (released 20
+00002040: 3232 2d30 322d 3136 290a 2020 2020 2020  22-02-16).      
+00002050: 2020 0a20 2020 2020 2020 202d 2045 6e73    .        - Ens
+00002060: 7572 6520 636f 6d70 696c 6564 2074 7261  ure compiled tra
+00002070: 6e73 6c61 7469 6f6e 206d 6573 7361 6765  nslation message
+00002080: 2063 6174 616c 6f67 7320 6172 6520 696e   catalogs are in
+00002090: 636c 7564 6564 2069 6e20 7468 650a 2020  cluded in the.  
+000020a0: 2020 2020 2020 2020 6469 7374 7269 6275          distribu
+000020b0: 7469 6f6e 7320 7570 6c6f 6164 6564 206f  tions uploaded o
+000020c0: 6e20 5079 5049 2e0a 2020 2020 2020 2020  n PyPI..        
+000020d0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+000020e0: 2031 2e33 2e31 3220 2872 656c 6561 7365   1.3.12 (release
+000020f0: 6420 3230 3232 2d30 322d 3134 290a 2020  d 2022-02-14).  
+00002100: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00002110: 2046 6978 6573 2041 3131 7920 6973 7375   Fixes A11y issu
+00002120: 6520 7769 7468 2074 6865 2063 6c6f 7365  e with the close
+00002130: 2062 7574 746f 6e20 696e 2066 6c61 7368   button in flash
+00002140: 206d 6573 7361 6765 732e 0a20 2020 2020   messages..     
+00002150: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00002160: 696f 6e20 312e 332e 3131 2028 7265 6c65  ion 1.3.11 (rele
+00002170: 6173 6564 2032 3032 322d 3032 2d30 3829  ased 2022-02-08)
+00002180: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002190: 2020 2d20 4164 6473 206d 6172 6769 6e20    - Adds margin 
+000021a0: 6765 6e65 7261 746f 722e 0a20 2020 2020  generator..     
+000021b0: 2020 202d 2041 6464 7320 4131 3179 2070     - Adds A11y p
+000021c0: 6167 6520 6c61 6e64 6d61 726b 732e 0a20  age landmarks.. 
+000021d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000021e0: 5665 7273 696f 6e20 312e 332e 3130 2028  Version 1.3.10 (
+000021f0: 7265 6c65 6173 6564 2032 3032 312d 3131  released 2021-11
+00002200: 2d32 3329 0a20 2020 2020 2020 200a 2020  -23).        .  
+00002210: 2020 2020 2020 2d20 5765 6220 6163 6365        - Web acce
+00002220: 7373 6962 696c 6974 7920 6669 782e 0a20  ssibility fix.. 
+00002230: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002240: 5665 7273 696f 6e20 312e 332e 3920 2872  Version 1.3.9 (r
+00002250: 656c 6561 7365 6420 3230 3231 2d30 372d  eleased 2021-07-
+00002260: 3132 290a 2020 2020 2020 2020 0a20 2020  12).        .   
+00002270: 2020 2020 202d 2041 6464 7320 6765 726d       - Adds germ
+00002280: 616e 2074 7261 6e73 6c61 7469 6f6e 730a  an translations.
+00002290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000022a0: 2056 6572 7369 6f6e 2031 2e33 2e38 2028   Version 1.3.8 (
+000022b0: 7265 6c65 6173 6564 2032 3032 312d 3032  released 2021-02
+000022c0: 2d31 3029 0a20 2020 2020 2020 200a 2020  -10).        .  
+000022d0: 2020 2020 2020 2d20 4164 6473 2062 7261        - Adds bra
+000022e0: 6e64 2063 6f6c 6f72 2074 6f20 6d65 6e75  nd color to menu
+000022f0: 2069 7465 6d73 0a20 2020 2020 2020 200a   items.        .
+00002300: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00002310: 312e 332e 3720 2872 656c 6561 7365 6420  1.3.7 (released 
+00002320: 3230 3231 2d30 312d 3235 290a 2020 2020  2021-01-25).    
+00002330: 2020 2020 0a20 2020 2020 2020 202d 2041      .        - A
+00002340: 6464 7320 6272 616e 6420 636f 6c6f 7220  dds brand color 
+00002350: 696e 2073 6567 6d65 6e74 730a 2020 2020  in segments.    
+00002360: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00002370: 7369 6f6e 2031 2e33 2e36 2028 7265 6c65  sion 1.3.6 (rele
+00002380: 6173 6564 2032 3032 312d 3031 2d30 3429  ased 2021-01-04)
+00002390: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000023a0: 2020 2d20 4164 6473 2060 6c69 6e6b 6020    - Adds `link` 
+000023b0: 7468 656d 6520 6963 6f6e 0a20 2020 2020  theme icon.     
+000023c0: 2020 202d 2046 6978 6573 2077 696c 6463     - Fixes wildc
+000023d0: 6172 6420 6963 6f6e 2072 6573 6f6c 7574  ard icon resolut
+000023e0: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
+000023f0: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
+00002400: 2e35 2028 7265 6c65 6173 6564 2032 3032  .5 (released 202
+00002410: 302d 3132 2d31 3729 0a20 2020 2020 2020  0-12-17).       
+00002420: 200a 2020 2020 2020 2020 2d20 4669 7865   .        - Fixe
+00002430: 7320 6368 6563 6b62 6f78 2e6f 7665 7272  s checkbox.overr
+00002440: 6964 6573 2069 6e20 6069 6e76 656e 696f  ides in `invenio
+00002450: 6020 5355 4920 7061 636b 6167 6564 2074  ` SUI packaged t
+00002460: 6865 6d65 2e0a 2020 2020 2020 2020 0a20  heme..        . 
+00002470: 2020 2020 2020 2056 6572 7369 6f6e 2031         Version 1
+00002480: 2e33 2e34 2028 7265 6c65 6173 6564 2032  .3.4 (released 2
+00002490: 3032 302d 3132 2d31 3729 0a20 2020 2020  020-12-17).     
+000024a0: 2020 200a 2020 2020 2020 2020 2d20 4164     .        - Ad
+000024b0: 6473 2061 2066 756c 6c20 2269 6e76 656e  ds a full "inven
+000024c0: 696f 2220 5365 6d61 6e74 6963 2055 4920  io" Semantic UI 
+000024d0: 7061 636b 6167 6564 2074 6865 6d65 2073  packaged theme s
+000024e0: 6f20 7765 2063 616e 2065 6173 6965 7220  o we can easier 
+000024f0: 6375 7374 6f6d 697a 650a 2020 2020 2020  customize.      
+00002500: 2020 2020 6c61 796f 7574 2069 6e20 7468      layout in th
+00002510: 6520 6675 7475 7265 2e0a 2020 2020 2020  e future..      
+00002520: 2020 0a20 2020 2020 2020 202d 204d 6f76    .        - Mov
+00002530: 6573 2074 6865 6d65 2e63 6f6e 6669 6720  es theme.config 
+00002540: 746f 2074 6865 6d65 2e63 6f6e 6669 672e  to theme.config.
+00002550: 6578 616d 706c 6520 616e 6420 6164 6473  example and adds
+00002560: 2061 206e 6f74 6520 746f 206d 616b 6520   a note to make 
+00002570: 6974 0a20 2020 2020 2020 2020 2063 6c65  it.          cle
+00002580: 6172 2074 6865 2066 696c 6520 6973 206e  ar the file is n
+00002590: 6f74 2061 6374 7561 6c6c 7920 7573 6564  ot actually used
+000025a0: 2c20 6275 7420 6973 206a 7573 7420 616e  , but is just an
+000025b0: 2065 7861 6d70 6c65 2e0a 2020 2020 2020   example..      
+000025c0: 2020 0a20 2020 2020 2020 202d 2041 6464    .        - Add
+000025d0: 7320 6865 6c70 6572 2074 6f6f 6c20 666f  s helper tool fo
+000025e0: 7220 7375 7070 6f72 7469 6e67 2074 6865  r supporting the
+000025f0: 6d65 2064 6570 656e 6465 6e74 2069 636f  me dependent ico
+00002600: 6e73 2e0a 2020 2020 2020 2020 0a20 2020  ns..        .   
+00002610: 2020 2020 202d 2046 6978 6573 206d 616e       - Fixes man
+00002620: 7920 6d69 6e6f 7220 7374 796c 696e 6720  y minor styling 
+00002630: 6973 7375 6573 2073 7563 6820 6173 2061  issues such as a
+00002640: 6c69 676e 6d65 6e74 732c 2062 7574 746f  lignments, butto
+00002650: 6e20 6c6f 6361 7469 6f6e 732c 0a20 2020  n locations,.   
+00002660: 2020 2020 2020 2067 7269 6473 2e0a 2020         grids..  
+00002670: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+00002680: 6572 7369 6f6e 2031 2e33 2e33 2028 7265  ersion 1.3.3 (re
+00002690: 6c65 6173 6564 2032 3032 302d 3132 2d31  leased 2020-12-1
+000026a0: 3129 0a20 2020 2020 2020 200a 2020 2020  1).        .    
+000026b0: 2020 2020 2d20 496e 6974 6961 6c69 7a65      - Initialize
+000026c0: 7320 7365 6d61 6e74 6963 5549 2061 6363  s semanticUI acc
+000026d0: 6f72 6469 6f6e 2063 6f6d 706f 6e65 6e74  ordion component
+000026e0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+000026f0: 2020 2020 5665 7273 696f 6e20 312e 332e      Version 1.3.
+00002700: 3220 2872 656c 6561 7365 6420 3230 3230  2 (released 2020
+00002710: 2d31 322d 3131 290a 2020 2020 2020 2020  -12-11).        
+00002720: 0a20 2020 2020 2020 202d 2055 7064 6174  .        - Updat
+00002730: 6573 2074 6865 2049 6e76 656e 696f 206c  es the Invenio l
+00002740: 6f67 6f20 616e 6420 7265 6d6f 7665 206f  ogo and remove o
+00002750: 7574 6461 7465 6420 7665 7273 696f 6e73  utdated versions
+00002760: 2e0a 2020 2020 2020 2020 2d20 4669 7865  ..        - Fixe
+00002770: 7320 7468 6520 6472 6f70 646f 776e 2074  s the dropdown t
+00002780: 6f20 776f 726b 206f 6e20 7468 6520 7573  o work on the us
+00002790: 6572 2070 726f 6669 6c65 2070 6167 652e  er profile page.
+000027a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000027b0: 2020 5665 7273 696f 6e20 312e 332e 3120    Version 1.3.1 
+000027c0: 2872 656c 6561 7365 6420 3230 3230 2d31  (released 2020-1
+000027d0: 322d 3039 290a 2020 2020 2020 2020 0a20  2-09).        . 
+000027e0: 2020 2020 2020 202d 204d 696e 6f72 2066         - Minor f
+000027f0: 6978 2066 6f72 2053 656d 616e 7469 6355  ix for SemanticU
+00002800: 4920 6472 6f70 646f 776e 730a 2020 2020  I dropdowns.    
+00002810: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00002820: 7369 6f6e 2031 2e33 2e30 2028 7265 6c65  sion 1.3.0 (rele
+00002830: 6173 6564 2032 3032 302d 3132 2d30 3929  ased 2020-12-09)
+00002840: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002850: 2020 2d20 4d61 6a6f 723a 204e 6577 2053    - Major: New S
+00002860: 656d 616e 7469 6355 4920 7468 656d 6520  emanticUI theme 
+00002870: 6861 7320 6265 656e 2069 6e74 6567 7261  has been integra
+00002880: 7465 642e 2054 6865 2042 6f6f 7473 7472  ted. The Bootstr
+00002890: 6170 2033 2074 6865 6d65 2073 7469 6c6c  ap 3 theme still
+000028a0: 0a20 2020 2020 2020 2020 2065 7869 7374  .          exist
+000028b0: 732e 2054 6869 7320 6368 616e 6765 2064  s. This change d
+000028c0: 6570 656e 6473 206f 6e20 7468 6520 6c61  epends on the la
+000028d0: 7465 7374 2072 656c 6561 7365 6420 496e  test released In
+000028e0: 7665 6e69 6f2d 4173 7365 7473 2077 6869  venio-Assets whi
+000028f0: 6368 0a20 2020 2020 2020 2020 2061 6464  ch.          add
+00002900: 7320 7375 7070 6f72 7473 2066 6f72 206d  s supports for m
+00002910: 756c 7469 706c 6520 5549 2066 7261 6d65  ultiple UI frame
+00002920: 776f 726b 732e 0a20 2020 2020 2020 200a  works..        .
+00002930: 2020 2020 2020 2020 2d20 4164 6473 2073          - Adds s
+00002940: 7570 706f 7274 2066 6f72 2064 796e 616d  upport for dynam
+00002950: 6963 206c 6f61 6469 6e67 206f 6620 7465  ic loading of te
+00002960: 6d70 6c61 7465 7320 666f 7220 5265 6163  mplates for Reac
+00002970: 742d 4f76 6572 7269 6461 626c 652e 0a20  t-Overridable.. 
+00002980: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002990: 2d20 4261 636b 7761 7264 7320 696e 636f  - Backwards inco
+000029a0: 6d70 6174 6962 6c65 3a20 5468 6520 6f6c  mpatible: The ol
+000029b0: 642d 7374 796c 6520 466c 6173 6b2d 4173  d-style Flask-As
+000029c0: 7365 7420 6275 6e64 6c65 7320 7761 7320  set bundles was 
+000029d0: 7265 6d6f 7665 6420 2874 6865 7365 0a20  removed (these. 
+000029e0: 2020 2020 2020 2020 2062 756e 646c 6573           bundles
+000029f0: 2077 6572 6520 6465 7072 6563 6174 6564   were deprecated
+00002a00: 2069 6e20 496e 7665 6e69 6f20 7633 2e31   in Invenio v3.1
+00002a10: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
+00002a20: 2020 2020 2d20 4164 6473 2054 7572 6b69      - Adds Turki
+00002a30: 7368 2074 7261 6e73 6c61 7469 6f6e 732e  sh translations.
+00002a40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002a50: 2020 5665 7273 696f 6e20 312e 322e 3020    Version 1.2.0 
+00002a60: 2872 656c 6561 7365 6420 3230 3230 2d30  (released 2020-0
+00002a70: 332d 3230 290a 2020 2020 2020 2020 0a20  3-20).        . 
+00002a80: 2020 2020 2020 202d 2052 6570 6c61 6365         - Replace
+00002a90: 7320 466c 6173 6b20 6465 7065 6e64 656e  s Flask dependen
+00002aa0: 6379 2077 6974 6820 6060 696e 7665 6e69  cy with ``inveni
+00002ab0: 6f2d 6261 7365 6060 2e0a 2020 2020 2020  o-base``..      
+00002ac0: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
+00002ad0: 6f6e 2031 2e31 2e34 2028 7265 6c65 6173  on 1.1.4 (releas
+00002ae0: 6564 2032 3031 392d 3037 2d32 3229 0a20  ed 2019-07-22). 
+00002af0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002b00: 2d20 496e 7472 6f64 7563 6520 6861 6e64  - Introduce hand
+00002b10: 6c69 6e67 206f 6620 7468 6520 6572 726f  ling of the erro
+00002b20: 7220 3432 392e 0a20 2020 2020 2020 200a  r 429..        .
+00002b30: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00002b40: 312e 312e 3320 2872 656c 6561 7365 6420  1.1.3 (released 
+00002b50: 3230 3139 2d30 332d 3133 290a 2020 2020  2019-03-13).    
+00002b60: 2020 2020 0a20 2020 2020 2020 202d 2052      .        - R
+00002b70: 6573 7472 7563 7475 7265 2053 4353 5320  estructure SCSS 
+00002b80: 6669 6c65 732c 2069 6e20 6f72 6465 7220  files, in order 
+00002b90: 746f 2061 6c6c 6f77 2065 6173 6965 7220  to allow easier 
+00002ba0: 6375 7374 6f6d 697a 6174 696f 6e20 616e  customization an
+00002bb0: 6420 6578 7465 6e73 696f 6e0a 2020 2020  d extension.    
+00002bc0: 2020 2020 2020 696e 206f 7665 726c 6179        in overlay
+00002bd0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00002be0: 2020 2020 5665 7273 696f 6e20 312e 312e      Version 1.1.
+00002bf0: 3220 2872 656c 6561 7365 6420 3230 3139  2 (released 2019
+00002c00: 2d30 322d 3135 290a 2020 2020 2020 2020  -02-15).        
+00002c10: 0a20 2020 2020 2020 202d 2055 7067 7261  .        - Upgra
+00002c20: 6465 6420 6d6f 6d65 6e74 2074 6f20 322e  ded moment to 2.
+00002c30: 3233 2e30 0a20 2020 2020 2020 200a 2020  23.0.        .  
+00002c40: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00002c50: 312e 3120 2872 656c 6561 7365 6420 3230  1.1 (released 20
+00002c60: 3138 2d31 322d 3035 290a 2020 2020 2020  18-12-05).      
+00002c70: 2020 0a20 2020 2020 2020 202d 2046 6978    .        - Fix
+00002c80: 6573 2069 7373 7565 7320 7769 7468 2077  es issues with w
+00002c90: 6562 7061 636b 2061 6e64 2074 6865 2041  ebpack and the A
+00002ca0: 646d 696e 4c54 4520 7468 656d 652e 0a20  dminLTE theme.. 
+00002cb0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002cc0: 5665 7273 696f 6e20 312e 312e 3020 2872  Version 1.1.0 (r
+00002cd0: 656c 6561 7365 6420 3230 3138 2d31 312d  eleased 2018-11-
+00002ce0: 3036 290a 2020 2020 2020 2020 0a20 2020  06).        .   
+00002cf0: 2020 2020 202d 2049 6e74 726f 6475 6365       - Introduce
+00002d00: 2077 6562 7061 636b 2073 7570 706f 7274   webpack support
+00002d10: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00002d20: 2020 2056 6572 7369 6f6e 2031 2e30 2e30     Version 1.0.0
+00002d30: 2028 7265 6c65 6173 6564 2032 3031 382d   (released 2018-
+00002d40: 3033 2d32 3329 0a20 2020 2020 2020 200a  03-23).        .
+00002d50: 2020 2020 2020 2020 2d20 496e 6974 6961          - Initia
+00002d60: 6c20 7075 626c 6963 2072 656c 6561 7365  l public release
+00002d70: 2e0a 2020 2020 2020 2020 0a4b 6579 776f  ..        .Keywo
+00002d80: 7264 733a 2069 6e76 656e 696f 0a50 6c61  rds: invenio.Pla
+00002d90: 7466 6f72 6d3a 2061 6e79 0a43 6c61 7373  tform: any.Class
+00002da0: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+00002db0: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+00002dc0: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00002dd0: 6c65 0a52 6571 7569 7265 732d 5079 7468  le.Requires-Pyth
+00002de0: 6f6e 3a20 3e3d 332e 370a 5072 6f76 6964  on: >=3.7.Provid
+00002df0: 6573 2d45 7874 7261 3a20 7465 7374 730a  es-Extra: tests.
+00002e00: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00002e10: 646f 6373 0a                             docs.
```

### Comparing `invenio-theme-3.0.0/README.rst` & `invenio-theme-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/Makefile` & `invenio-theme-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/conf.py` & `invenio-theme-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/index.rst` & `invenio-theme-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/make.bat` & `invenio-theme-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/static/base.png` & `invenio-theme-3.1.0/docs/static/base.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/static/cover.png` & `invenio-theme-3.1.0/docs/static/cover.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/static/error.png` & `invenio-theme-3.1.0/docs/static/error.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/docs/static/settings.png` & `invenio-theme-3.1.0/docs/static/settings.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/__init__.py` & `invenio-theme-3.1.0/invenio_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,11 +486,11 @@
         flash('Testing flashing', category='info')
         return render_template('...')
 """
 
 from .ext import InvenioTheme
 from .shared import menu
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 
 __all__ = ("__version__", "InvenioTheme", "menu")
```

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss` & `invenio-theme-3.1.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides`

 * *Files 0% similar despite different names*

```diff
@@ -641,13 +641,17 @@
 .rich-input-content
  {
   table, td, th {
       border: 1px dashed @lightGray;
       border-collapse: collapse;
       padding: 1rem;
   }
+
+  pre {
+    white-space: pre-wrap;
+  }
 }
 blockquote{
   border-left: 4px solid @lightGray;
   margin-left: 1.5rem;
   padding-left: 1rem;
 }
```

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss` & `invenio-theme-3.1.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/config.py` & `invenio-theme-3.1.0/invenio_theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/ext.py` & `invenio-theme-3.1.0/invenio_theme/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/icons.py` & `invenio-theme-3.1.0/invenio_theme/icons.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/proxies.py` & `invenio-theme-3.1.0/invenio_theme/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-120.png` & `invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-120.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-152.png` & `invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-152.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-167.png` & `invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-167.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/apple-touch-icon-180.png` & `invenio-theme-3.1.0/invenio_theme/static/apple-touch-icon-180.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/favicon.ico` & `invenio-theme-3.1.0/invenio_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/images/invenio-white.svg` & `invenio-theme-3.1.0/invenio_theme/static/images/invenio-white.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/static/images/square-placeholder.png` & `invenio-theme-3.1.0/invenio_theme/static/images/square-placeholder.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/500.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/500.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/admin_header.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/admin_header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/admin_layout.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/admin_layout.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/breadcrumbs.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/footer.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/header.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/header_frontpage.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/header_frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/header_login.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/macros/messages.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/macros/messages.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/macros/truncate.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/macros/truncate.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_admin.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_admin.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_cover.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_cover.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/invenio_theme/page_settings.html` & `invenio-theme-3.1.0/invenio_theme/templates/invenio_theme/page_settings.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html` & `invenio-theme-3.1.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 {# -*- coding: utf-8 -*-
 
   This file is part of Invenio.
-  Copyright (C) 2015-2018 CERN.
+  Copyright (C) 2015-2024 CERN.
   Copyright (C) 2021 New York University.
   Copyright (C) 2022 TU Wien.
   Copyright (C) 2023 Graz University of Technology.
 
   Invenio is free software; you can redistribute it and/or modify it
   under the terms of the MIT License; see LICENSE file for more details.
 #}
 
 {%- extends config.THEME_BASE_TEMPLATE %}
 
+{%- set title = _("Settings") %}
+
 {%- block page_body scoped %}
 
 <div class="ui container fluid page-subheader-outer compact ml-0-mobile mr-0-mobile">
   <div class="ui container page-subheader">
     <h1 class="ui large header">{{_("My account")}}</h1>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-{# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2018
+{# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2024
 CERN. Copyright (C) 2021 New York University. Copyright (C) 2022 TU Wien.
 Copyright (C) 2023 Graz University of Technology. Invenio is free software; you
 can redistribute it and/or modify it under the terms of the MIT License; see
 LICENSE file for more details. #} {%- extends config.THEME_BASE_TEMPLATE %} {%-
-block page_body scoped %}
+set title = _("Settings") %} {%- block page_body scoped %}
 ************ {{{{__((""MMyy aaccccoouunntt""))}}}} ************
 {%- block settings_menu scoped %}
 {{{{ __((''SSeettttiinnggss'')) }}}} {%- for item in current_menu.submenu('settings').children
 if item.visible %} {%- block settings_menu_item scoped %}
 % if item.active %} aria-current="page" {% endif %} > {{ item.text|safe }}
 {%- endblock %} {%- endfor %}
 {%- endblock %} {%- block settings_content scoped %}
```

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/af/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/da/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/el/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/es/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/et/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/it/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/messages.pot` & `invenio-theme-3.1.0/invenio_theme/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/no/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-theme-3.1.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-theme-3.1.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/views.py` & `invenio-theme-3.1.0/invenio_theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme/webpack.py` & `invenio-theme-3.1.0/invenio_theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/invenio_theme.egg-info/PKG-INFO` & `invenio-theme-3.1.0/invenio_theme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 696e 7665  : 2.1.Name: inve
 00000020: 6e69 6f2d 7468 656d 650a 5665 7273 696f  nio-theme.Versio
-00000030: 6e3a 2033 2e30 2e30 0a53 756d 6d61 7279  n: 3.0.0.Summary
+00000030: 6e3a 2033 2e31 2e30 0a53 756d 6d61 7279  n: 3.1.0.Summary
 00000040: 3a20 2249 6e76 656e 696f 2073 7461 6e64  : "Invenio stand
 00000050: 6172 6420 7468 656d 652e 220a 486f 6d65  ard theme.".Home
 00000060: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 00000070: 6974 6875 622e 636f 6d2f 696e 7665 6e69  ithub.com/inveni
 00000080: 6f73 6f66 7477 6172 652f 696e 7665 6e69  osoftware/inveni
 00000090: 6f2d 7468 656d 650a 4175 7468 6f72 3a20  o-theme.Author: 
 000000a0: 496e 7665 6e69 6f20 436f 6c6c 6162 6f72  Invenio Collabor
@@ -119,610 +119,620 @@
 00000760: 2074 6865 204d 4954 204c 6963 656e 7365   the MIT License
 00000770: 3b20 7365 6520 4c49 4345 4e53 4520 6669  ; see LICENSE fi
 00000780: 6c65 2066 6f72 206d 6f72 6520 6465 7461  le for more deta
 00000790: 696c 732e 0a20 2020 2020 2020 200a 2020  ils..        .  
 000007a0: 2020 2020 2020 4368 616e 6765 730a 2020        Changes.  
 000007b0: 2020 2020 2020 3d3d 3d3d 3d3d 3d0a 2020        =======.  
 000007c0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
-000007d0: 6572 7369 6f6e 2033 2e30 2e30 2028 7265  ersion 3.0.0 (re
-000007e0: 6c65 6173 6564 2032 3032 342d 3033 2d31  leased 2024-03-1
-000007f0: 3929 0a20 2020 2020 2020 200a 2020 2020  9).        .    
-00000800: 2020 2020 2d20 676c 6f62 616c 3a20 7265      - global: re
-00000810: 6d6f 7665 2062 7265 6164 6372 756d 6220  move breadcrumb 
-00000820: 7375 7070 6f72 740a 2020 2020 2020 2020  support.        
-00000830: 2d20 676c 6f62 616c 3a20 696e 7472 6f64  - global: introd
-00000840: 7563 6520 7368 6172 6564 206d 656e 750a  uce shared menu.
-00000850: 2020 2020 2020 2020 2d20 676c 6f62 616c          - global
-00000860: 3a20 7072 6570 6172 6174 696f 6e20 666f  : preparation fo
-00000870: 7220 636f 6d70 6174 6962 696c 6974 7920  r compatibility 
-00000880: 7769 7468 2046 6c61 736b 2076 322e 332e  with Flask v2.3.
-00000890: 7820 6465 7072 6563 6174 696f 6e73 0a20  x deprecations. 
-000008a0: 2020 2020 2020 202d 2072 6566 6163 746f         - refacto
-000008b0: 723a 2063 7572 7265 6e74 5f74 6865 6d65  r: current_theme
-000008c0: 5f69 636f 6e73 2077 6974 686f 7574 2061  _icons without a
-000008d0: 7070 6c69 6361 7469 6f6e 2063 6f6e 7465  pplication conte
-000008e0: 7874 0a20 2020 2020 2020 200a 2020 2020  xt.        .    
-000008f0: 2020 2020 5665 7273 696f 6e20 322e 352e      Version 2.5.
-00000900: 3130 2028 7265 6c65 6173 6564 2032 3032  10 (released 202
-00000910: 342d 3031 2d32 3829 0a20 2020 2020 2020  4-01-28).       
-00000920: 200a 2020 2020 2020 2020 2d20 696e 7374   .        - inst
-00000930: 616c 6c61 7469 6f6e 3a20 6669 7820 7370  allation: fix sp
-00000940: 6869 6e78 2064 6570 656e 6465 6e63 790a  hinx dependency.
-00000950: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000960: 2056 6572 7369 6f6e 2032 2e35 2e39 2028   Version 2.5.9 (
-00000970: 7265 6c65 6173 6564 2032 3032 342d 3031  released 2024-01
-00000980: 2d32 3829 0a20 2020 2020 2020 200a 2020  -28).        .  
-00000990: 2020 2020 2020 2d20 676c 6f62 616c 3a20        - global: 
-000009a0: 6368 616e 6765 206d 6174 6820 6f70 6572  change math oper
-000009b0: 6174 696f 6e20 746f 2062 6520 636f 6d70  ation to be comp
-000009c0: 6174 6962 6c65 2077 6974 6820 7361 7373  atible with sass
-000009d0: 322e 300a 2020 2020 2020 2020 0a20 2020  2.0.        .   
-000009e0: 2020 2020 2056 6572 7369 6f6e 2032 2e35       Version 2.5
-000009f0: 2e38 2028 7265 6c65 6173 6564 2032 3032  .8 (released 202
-00000a00: 332d 3132 2d31 3229 0a20 2020 2020 2020  3-12-12).       
-00000a10: 200a 2020 2020 2020 2020 2d20 7265 706c   .        - repl
-00000a20: 6163 6520 636b 6564 6974 6f72 2077 6974  ace ckeditor wit
-00000a30: 6820 7469 6e79 6d63 6520 6475 6520 746f  h tinymce due to
-00000a40: 206c 6963 656e 7365 2069 7373 7565 0a20   license issue. 
-00000a50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000a60: 5665 7273 696f 6e20 322e 352e 3720 2872  Version 2.5.7 (r
-00000a70: 656c 6561 7365 6420 3230 3233 2d31 302d  eleased 2023-10-
-00000a80: 3236 290a 2020 2020 2020 2020 0a20 2020  26).        .   
-00000a90: 2020 2020 202d 2063 6f6d 6d75 6e69 7479       - community
-00000aa0: 206c 6f67 6f3a 2066 6978 2072 656e 6465   logo: fix rende
-00000ab0: 7269 6e67 2061 2070 6c61 6365 686f 6c64  ring a placehold
-00000ac0: 6572 0a20 2020 2020 2020 200a 2020 2020  er.        .    
-00000ad0: 2020 2020 5665 7273 696f 6e20 322e 352e      Version 2.5.
-00000ae0: 3620 2872 656c 6561 7365 6420 3230 3233  6 (released 2023
-00000af0: 2d31 302d 3230 290a 2020 2020 2020 2020  -10-20).        
-00000b00: 0a20 2020 2020 2020 202d 2064 6f6e 2774  .        - don't
-00000b10: 206f 7665 7272 6964 6520 6c69 6e6b 7320   override links 
-00000b20: 7374 796c 6520 696e 2066 6c61 7368 6564  style in flashed
-00000b30: 206d 6573 7361 6765 730a 2020 2020 2020   messages.      
-00000b40: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-00000b50: 6f6e 2032 2e35 2e35 2028 7265 6c65 6173  on 2.5.5 (releas
-00000b60: 6564 2032 3032 332d 3039 2d31 3929 0a20  ed 2023-09-19). 
-00000b70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000b80: 2d20 7374 796c 696e 673a 2061 6464 2033  - styling: add 3
-00000b90: 2063 6f6c 756d 6e20 7465 6d70 6c61 7465   column template
-00000ba0: 2063 6c61 7373 0a20 2020 2020 2020 200a   class.        .
-00000bb0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00000bc0: 322e 352e 3420 2872 656c 6561 7365 6420  2.5.4 (released 
-00000bd0: 3230 3233 2d30 392d 3131 290a 2020 2020  2023-09-11).    
-00000be0: 2020 2020 0a20 2020 2020 2020 202d 2073      .        - s
-00000bf0: 6373 733a 2066 6978 2063 6f6d 7061 7469  css: fix compati
-00000c00: 6269 6c69 7479 2077 6974 6820 6c61 7465  bility with late
-00000c10: 7374 206c 6573 7320 7665 7273 696f 6e0a  st less version.
-00000c20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000c30: 2056 6572 7369 6f6e 2032 2e35 2e33 2028   Version 2.5.3 (
-00000c40: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
-00000c50: 2d30 3829 0a20 2020 2020 2020 200a 2020  -08).        .  
-00000c60: 2020 2020 2020 2d20 7374 796c 6573 6865        - styleshe
-00000c70: 6574 733a 2061 6464 2070 7265 666f 726d  ets: add preform
-00000c80: 6174 7465 6420 7461 6720 7374 796c 696e  atted tag stylin
-00000c90: 6720 666f 6e74 0a20 2020 2020 2020 200a  g font.        .
-00000ca0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00000cb0: 322e 352e 3220 2872 656c 6561 7365 6420  2.5.2 (released 
-00000cc0: 3230 3233 2d30 382d 3134 290a 2020 2020  2023-08-14).    
-00000cd0: 2020 2020 0a20 2020 2020 2020 202d 2069      .        - i
-00000ce0: 6e73 7461 6c6c 6174 696f 6e3a 2070 696e  nstallation: pin
-00000cf0: 2046 6c61 736b 2d4d 656e 7520 746f 2060   Flask-Menu to `
-00000d00: 603c 7631 2e30 2e30 6060 2e0a 2020 2020  `<v1.0.0``..    
-00000d10: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00000d20: 7369 6f6e 2032 2e35 2e31 2028 7265 6c65  sion 2.5.1 (rele
-00000d30: 6173 6564 2032 3032 332d 3038 2d31 3429  ased 2023-08-14)
-00000d40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000d50: 2020 2d20 7468 656d 653a 2062 7567 6669    - theme: bugfi
-00000d60: 7820 746f 2064 6563 7265 6173 6520 7a2d  x to decrease z-
-00000d70: 696e 6465 7820 7661 6c75 650a 2020 2020  index value.    
-00000d80: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00000d90: 7369 6f6e 2032 2e35 2e30 2028 7265 6c65  sion 2.5.0 (rele
-00000da0: 6173 6564 2032 3032 332d 3038 2d30 3929  ased 2023-08-09)
-00000db0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000dc0: 2020 2d20 7468 656d 653a 2061 6464 2075    - theme: add u
-00000dd0: 7469 6c69 7479 2063 6c61 7373 6573 0a20  tility classes. 
-00000de0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000df0: 5665 7273 696f 6e20 322e 342e 3020 2872  Version 2.4.0 (r
-00000e00: 656c 6561 7365 6420 3230 3233 2d30 382d  eleased 2023-08-
-00000e10: 3032 290a 2020 2020 2020 2020 0a20 2020  02).        .   
-00000e20: 2020 2020 202d 2074 6865 6d65 3a20 6164       - theme: ad
-00000e30: 6420 736f 6d65 2067 656e 6572 616c 2063  d some general c
-00000e40: 6c61 7373 6573 2061 6e64 2066 6978 6573  lasses and fixes
-00000e50: 2061 6c69 676e 6d65 6e74 2066 6f72 206c   alignment for l
-00000e60: 6162 656c 6564 2066 6c75 6964 2062 7574  abeled fluid but
-00000e70: 746f 6e73 0a20 2020 2020 2020 200a 2020  tons.        .  
-00000e80: 2020 2020 2020 5665 7273 696f 6e20 322e        Version 2.
-00000e90: 332e 3020 2872 656c 6561 7365 6420 3230  3.0 (released 20
-00000ea0: 3233 2d30 372d 3331 290a 2020 2020 2020  23-07-31).      
-00000eb0: 2020 0a20 2020 2020 2020 202d 2073 6574    .        - set
-00000ec0: 7469 6e67 7320 7061 6765 3a20 496d 7072  tings page: Impr
-00000ed0: 6f76 6520 7465 6d70 6c61 7465 2066 6f72  ove template for
-00000ee0: 2061 3131 790a 2020 2020 2020 2020 0a20   a11y.        . 
-00000ef0: 2020 2020 2020 2056 6572 7369 6f6e 2032         Version 2
-00000f00: 2e32 2e30 2028 7265 6c65 6173 6564 2032  .2.0 (released 2
-00000f10: 3032 332d 3037 2d32 3629 0a20 2020 2020  023-07-26).     
-00000f20: 2020 200a 2020 2020 2020 2020 2d20 7468     .        - th
-00000f30: 656d 653a 2061 6464 2067 656e 6572 616c  eme: add general
-00000f40: 2073 7479 6c65 2069 6d70 726f 7665 6d65   style improveme
-00000f50: 6e74 730a 2020 2020 2020 2020 0a20 2020  nts.        .   
-00000f60: 2020 2020 2056 6572 7369 6f6e 2032 2e31       Version 2.1
-00000f70: 2e33 2028 7265 6c65 6173 6564 2032 3032  .3 (released 202
-00000f80: 332d 3037 2d32 3429 0a20 2020 2020 2020  3-07-24).       
-00000f90: 200a 2020 2020 2020 2020 2d20 6d65 7373   .        - mess
-00000fa0: 6167 6573 3a20 6164 6420 7a2d 696e 6465  ages: add z-inde
-00000fb0: 780a 2020 2020 2020 2020 0a20 2020 2020  x.        .     
-00000fc0: 2020 2056 6572 7369 6f6e 2032 2e31 2e32     Version 2.1.2
-00000fd0: 2028 7265 6c65 6173 6564 2032 3032 332d   (released 2023-
-00000fe0: 3034 2d31 3229 0a20 2020 2020 2020 200a  04-12).        .
-00000ff0: 2020 2020 2020 2020 2d20 6164 6420 666c          - add fl
-00001000: 6578 2075 7469 6c69 7479 2063 6c61 7373  ex utility class
-00001010: 6573 0a20 2020 2020 2020 202d 2061 6464  es.        - add
-00001020: 2074 6578 7420 7369 7a65 7320 636c 6173   text sizes clas
-00001030: 7365 730a 2020 2020 2020 2020 0a20 2020  ses.        .   
-00001040: 2020 2020 2056 6572 7369 6f6e 2032 2e31       Version 2.1
-00001050: 2e31 2028 7265 6c65 6173 6564 2032 3032  .1 (released 202
-00001060: 332d 3034 2d30 3629 0a20 2020 2020 2020  3-04-06).       
-00001070: 200a 2020 2020 2020 2020 2d20 6164 6420   .        - add 
-00001080: 6469 7370 6c61 7920 7574 696c 6974 7920  display utility 
-00001090: 636c 6173 7365 730a 2020 2020 2020 2020  classes.        
-000010a0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-000010b0: 2032 2e31 2e30 2028 7265 6c65 6173 6564   2.1.0 (released
-000010c0: 2032 3032 332d 3033 2d32 3829 0a20 2020   2023-03-28).   
-000010d0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-000010e0: 6164 6420 676c 6f62 616c 2075 7469 6c69  add global utili
-000010f0: 7479 2073 7479 6c69 6e67 2063 6c61 7373  ty styling class
-00001100: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
-00001110: 2020 2020 5665 7273 696f 6e20 322e 302e      Version 2.0.
-00001120: 3120 2872 656c 6561 7365 6420 3230 3233  1 (released 2023
-00001130: 2d30 332d 3039 290a 2020 2020 2020 2020  -03-09).        
-00001140: 0a20 2020 2020 2020 202d 2066 6978 2073  .        - fix s
-00001150: 7479 6c69 6e67 2066 6f72 2062 7574 746f  tyling for butto
-00001160: 6e73 0a20 2020 2020 2020 202d 206d 6f76  ns.        - mov
-00001170: 6520 676c 6f62 616c 2063 6c61 7373 2066  e global class f
-00001180: 6f72 2061 7574 6f20 6772 6964 0a20 2020  or auto grid.   
-00001190: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-000011a0: 7273 696f 6e20 322e 302e 3020 2872 656c  rsion 2.0.0 (rel
-000011b0: 6561 7365 6420 3230 3233 2d30 322d 3238  eased 2023-02-28
-000011c0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000011d0: 2020 202d 2064 726f 7020 7079 7468 6f6e     - drop python
-000011e0: 2032 2e37 2073 7570 706f 7274 0a20 2020   2.7 support.   
-000011f0: 2020 2020 202d 2072 656d 6f76 6520 666c       - remove fl
-00001200: 6173 6b5f 6261 6265 6c65 7820 696d 706f  ask_babelex impo
-00001210: 7274 730a 2020 2020 2020 2020 2d20 7570  rts.        - up
-00001220: 6772 6164 6520 696e 7665 6e69 6f5f 6931  grade invenio_i1
-00001230: 386e 0a20 2020 2020 2020 200a 2020 2020  8n.        .    
-00001240: 2020 2020 5665 7273 696f 6e20 312e 342e      Version 1.4.
-00001250: 3820 2872 656c 6561 7365 6420 3230 3233  8 (released 2023
-00001260: 2d30 322d 3037 290a 2020 2020 2020 2020  -02-07).        
-00001270: 0a20 2020 2020 2020 202d 2074 6865 6d65  .        - theme
-00001280: 3a20 6164 6420 6175 746f 2d63 6f6c 756d  : add auto-colum
-00001290: 6e2d 6772 6964 2063 6c61 7373 0a20 2020  n-grid class.   
-000012a0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-000012b0: 7273 696f 6e20 312e 342e 3720 2872 656c  rsion 1.4.7 (rel
-000012c0: 6561 7365 6420 3230 3233 2d30 312d 3035  eased 2023-01-05
-000012d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000012e0: 2020 202d 2061 6464 2074 7275 6e63 6174     - add truncat
-000012f0: 6520 6c69 6e65 7320 7374 796c 6573 0a20  e lines styles. 
-00001300: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001310: 5665 7273 696f 6e20 312e 342e 3620 2872  Version 1.4.6 (r
-00001320: 656c 6561 7365 6420 3230 3232 2d31 322d  eleased 2022-12-
-00001330: 3038 290a 2020 2020 2020 2020 0a20 2020  08).        .   
-00001340: 2020 2020 202d 2066 6978 2073 7479 6c69       - fix styli
-00001350: 6e67 2066 6f72 2069 6e6c 696e 6520 636c  ng for inline cl
-00001360: 6173 732c 2061 6666 6563 7469 6e67 2066  ass, affecting f
-00001370: 6f72 6d20 6669 656c 6473 0a20 2020 2020  orm fields.     
-00001380: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00001390: 696f 6e20 312e 342e 3520 2872 656c 6561  ion 1.4.5 (relea
-000013a0: 7365 6420 3230 3232 2d31 322d 3031 290a  sed 2022-12-01).
-000013b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000013c0: 202d 2066 6978 2073 6561 7263 6820 7265   - fix search re
-000013d0: 7375 6c74 2069 7465 6d20 7374 796c 696e  sult item stylin
-000013e0: 670a 2020 2020 2020 2020 2d20 6164 6420  g.        - add 
-000013f0: 676c 6f62 616c 2062 6568 6176 696f 7572  global behaviour
-00001400: 2063 6c61 7373 6573 0a20 2020 2020 2020   classes.       
-00001410: 202d 2061 6464 2070 6c61 6365 686f 6c64   - add placehold
-00001420: 6572 2069 6d61 6765 2068 616e 646c 650a  er image handle.
-00001430: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001440: 2056 6572 7369 6f6e 2031 2e34 2e34 2028   Version 1.4.4 (
-00001450: 7265 6c65 6173 6564 2032 3032 322d 3131  released 2022-11
-00001460: 2d31 3829 0a20 2020 2020 2020 200a 2020  -18).        .  
-00001470: 2020 2020 2020 2d20 4164 6420 7075 6c6c        - Add pull
-00001480: 6564 2074 7261 6e73 6c61 7469 6f6e 730a  ed translations.
-00001490: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000014a0: 2056 6572 7369 6f6e 2031 2e34 2e33 2028   Version 1.4.3 (
-000014b0: 7265 6c65 6173 6564 2032 3032 322d 3131  released 2022-11
-000014c0: 2d30 3329 0a20 2020 2020 2020 200a 2020  -03).        .  
-000014d0: 2020 2020 2020 2d20 6164 6420 7374 796c        - add styl
-000014e0: 696e 6720 666f 7220 6472 6f70 646f 776e  ing for dropdown
-000014f0: 206d 656e 7520 6974 656d 730a 2020 2020   menu items.    
-00001500: 2020 2020 2d20 6669 7820 6d69 7373 696e      - fix missin
-00001510: 6720 4d65 6469 6120 636f 6d70 6f6e 656e  g Media componen
-00001520: 7420 7261 6e67 650a 2020 2020 2020 2020  t range.        
-00001530: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-00001540: 2031 2e34 2e32 2028 7265 6c65 6173 6564   1.4.2 (released
-00001550: 2032 3032 322d 3130 2d32 3629 0a20 2020   2022-10-26).   
-00001560: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00001570: 6164 6420 4d65 6469 6120 746f 2073 7570  add Media to sup
-00001580: 706f 7274 2072 6573 706f 6e73 6976 6520  port responsive 
-00001590: 7265 6163 7420 636f 6d70 6f6e 656e 7473  react components
-000015a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015b0: 2020 5665 7273 696f 6e20 312e 342e 3120    Version 1.4.1 
-000015c0: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
-000015d0: 302d 3130 290a 2020 2020 2020 2020 0a20  0-10).        . 
-000015e0: 2020 2020 2020 202d 2062 756d 7020 5365         - bump Se
-000015f0: 6d61 6e74 6963 5549 0a20 2020 2020 2020  manticUI.       
-00001600: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
-00001610: 6e20 312e 342e 3020 2872 656c 6561 7365  n 1.4.0 (release
-00001620: 6420 3230 3232 2d31 302d 3035 290a 2020  d 2022-10-05).  
-00001630: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-00001640: 2063 6861 6e67 6520 676c 6f62 616c 2066   change global f
-00001650: 6f6e 7420 746f 204c 6174 6f0a 2020 2020  ont to Lato.    
-00001660: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00001670: 7369 6f6e 2031 2e33 2e33 3120 2872 656c  sion 1.3.31 (rel
-00001680: 6561 7365 6420 3230 3232 2d31 302d 3035  eased 2022-10-05
-00001690: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000016a0: 2020 202d 2061 6464 206d 6973 7369 6e67     - add missing
-000016b0: 2074 6865 6d65 2076 6172 6961 626c 6573   theme variables
-000016c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000016d0: 2020 5665 7273 696f 6e20 312e 332e 3330    Version 1.3.30
-000016e0: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-000016f0: 3039 2d32 3629 0a20 2020 2020 2020 200a  09-26).        .
-00001700: 2020 2020 2020 2020 2d20 6164 6420 7374          - add st
-00001710: 796c 696e 6720 746f 2061 646d 696e 6973  yling to adminis
-00001720: 7472 6174 696f 6e20 6461 7368 626f 6172  tration dashboar
-00001730: 6420 7061 6765 0a20 2020 2020 2020 200a  d page.        .
-00001740: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00001750: 312e 332e 3239 2028 7265 6c65 6173 6564  1.3.29 (released
-00001760: 2032 3032 322d 3039 2d32 3229 0a20 2020   2022-09-22).   
-00001770: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00001780: 6164 6420 6164 6d69 6e69 7374 7261 7469  add administrati
-00001790: 6f6e 2070 616e 656c 2073 7479 6c69 6e67  on panel styling
-000017a0: 0a20 2020 2020 2020 202d 2061 6464 2074  .        - add t
-000017b0: 7261 6e73 6c61 7469 6f6e 2077 6f72 6b66  ranslation workf
-000017c0: 6c6f 770a 2020 2020 2020 2020 0a20 2020  low.        .   
-000017d0: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
-000017e0: 2e32 3820 2872 656c 6561 7365 6420 3230  .28 (released 20
-000017f0: 3232 2d30 372d 3038 290a 2020 2020 2020  22-07-08).      
-00001800: 2020 0a20 2020 2020 2020 202d 2061 6464    .        - add
-00001810: 2073 7479 6c69 6e67 2063 6c61 7373 6573   styling classes
-00001820: 2077 6974 6820 6163 7469 6f6e 2063 6f6c   with action col
-00001830: 6f72 2063 6f64 696e 670a 2020 2020 2020  or coding.      
-00001840: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-00001850: 6f6e 2031 2e33 2e32 3720 2872 656c 6561  on 1.3.27 (relea
-00001860: 7365 6420 3230 3232 2d30 372d 3037 290a  sed 2022-07-07).
-00001870: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001880: 202d 2066 6978 206a 7175 6572 7920 7265   - fix jquery re
-00001890: 6665 7265 6e63 650a 2020 2020 2020 2020  ference.        
-000018a0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-000018b0: 2031 2e33 2e32 3620 2872 656c 6561 7365   1.3.26 (release
-000018c0: 6420 3230 3232 2d30 372d 3037 290a 2020  d 2022-07-07).  
-000018d0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-000018e0: 2061 6464 2069 6d61 6765 2070 6c61 6365   add image place
-000018f0: 686f 6c64 6572 206f 6e20 6c6f 6164 2065  holder on load e
-00001900: 7272 6f72 0a20 2020 2020 2020 200a 2020  rror.        .  
-00001910: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
-00001920: 332e 3235 2028 7265 6c65 6173 6564 2032  3.25 (released 2
-00001930: 3032 322d 3036 2d32 3729 0a20 2020 2020  022-06-27).     
-00001940: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
-00001950: 6420 4765 726d 616e 2074 7261 6e73 6c61  d German transla
-00001960: 7469 6f6e 730a 2020 2020 2020 2020 2d20  tions.        - 
-00001970: 6669 7820 6472 6f70 646f 776e 2073 6372  fix dropdown scr
-00001980: 6f6c 6c20 6d69 7361 6c69 676e 6d65 6e74  oll misalignment
-00001990: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000019a0: 2020 5665 7273 696f 6e20 312e 332e 3234    Version 1.3.24
-000019b0: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-000019c0: 3035 2d32 3329 0a20 2020 2020 2020 200a  05-23).        .
-000019d0: 2020 2020 2020 2020 2d20 6164 6420 676c          - add gl
-000019e0: 6f62 616c 2043 5353 2063 6c61 7373 6573  obal CSS classes
-000019f0: 2066 6f72 206d 6172 6769 6e73 2061 7574   for margins aut
-00001a00: 6f0a 2020 2020 2020 2020 0a20 2020 2020  o.        .     
-00001a10: 2020 2056 6572 7369 6f6e 2031 2e33 2e32     Version 1.3.2
-00001a20: 3320 2872 656c 6561 7365 6420 3230 3232  3 (released 2022
-00001a30: 2d30 352d 3139 290a 2020 2020 2020 2020  -05-19).        
-00001a40: 0a20 2020 2020 2020 202d 2061 6464 2061  .        - add a
-00001a50: 6363 6573 7369 6269 6c69 7479 2074 6f20  ccessibility to 
-00001a60: 7569 2d61 6363 6f72 6469 6f6e 730a 2020  ui-accordions.  
-00001a70: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
-00001a80: 6572 7369 6f6e 2031 2e33 2e32 3220 2872  ersion 1.3.22 (r
-00001a90: 656c 6561 7365 6420 3230 3232 2d30 342d  eleased 2022-04-
-00001aa0: 3231 290a 2020 2020 2020 2020 0a20 2020  21).        .   
-00001ab0: 2020 2020 202d 2069 6d70 726f 7665 2073       - improve s
-00001ac0: 656d 616e 7469 6320 7374 796c 696e 6720  emantic styling 
-00001ad0: 6f66 204d 7920 6163 636f 756e 7420 7061  of My account pa
-00001ae0: 6765 0a20 2020 2020 2020 200a 2020 2020  ge.        .    
-00001af0: 2020 2020 5665 7273 696f 6e20 312e 332e      Version 1.3.
-00001b00: 3231 2028 7265 6c65 6173 6564 2032 3032  21 (released 202
-00001b10: 322d 3033 2d32 3929 0a20 2020 2020 2020  2-03-29).       
-00001b20: 200a 2020 2020 2020 2020 2d20 6669 7820   .        - fix 
-00001b30: 6874 6d6c 2074 6167 7320 696e 2074 656d  html tags in tem
-00001b40: 706c 6174 6573 0a20 2020 2020 2020 200a  plates.        .
-00001b50: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-00001b60: 312e 332e 3230 2028 7265 6c65 6173 6564  1.3.20 (released
-00001b70: 2032 3032 322d 3033 2d31 3729 0a20 2020   2022-03-17).   
-00001b80: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00001b90: 7265 6661 6374 6f72 2070 6167 6520 7465  refactor page te
-00001ba0: 6d70 6c61 7465 0a20 2020 2020 2020 202d  mplate.        -
-00001bb0: 2061 6464 2073 656d 616e 7469 6320 7569   add semantic ui
-00001bc0: 2069 6e76 656e 696f 2070 6163 6b61 6765   invenio package
-00001bd0: 6420 7468 656d 6520 636f 6e66 6967 7572  d theme configur
-00001be0: 6174 696f 6e0a 2020 2020 2020 2020 2d20  ation.        - 
-00001bf0: 6578 7465 6e64 2075 7469 6c73 2043 5353  extend utils CSS
-00001c00: 2063 6c61 7373 6573 0a20 2020 2020 2020   classes.       
-00001c10: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
-00001c20: 6e20 312e 332e 3139 2028 7265 6c65 6173  n 1.3.19 (releas
-00001c30: 6564 2032 3032 322d 3033 2d30 3429 0a20  ed 2022-03-04). 
-00001c40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001c50: 2d20 4164 6420 6120 7265 7573 6162 6c65  - Add a reusable
-00001c60: 204a 696e 6a61 206d 6163 726f 2074 6f20   Jinja macro to 
-00001c70: 7472 756e 6361 7465 206c 6f6e 6720 7465  truncate long te
-00001c80: 7874 2e0a 2020 2020 2020 2020 0a20 2020  xt..        .   
-00001c90: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
-00001ca0: 2e31 3820 2872 656c 6561 7365 6420 3230  .18 (released 20
-00001cb0: 3232 2d30 332d 3031 290a 2020 2020 2020  22-03-01).      
-00001cc0: 2020 0a20 2020 2020 2020 202d 2052 6576    .        - Rev
-00001cd0: 6572 7420 666f 6e74 2062 6163 6b20 746f  ert font back to
-00001ce0: 2064 6566 6175 6c74 2073 616e 732d 7361   default sans-sa
-00001cf0: 7269 6620 666f 6e74 2069 6e73 7465 6164  rif font instead
-00001d00: 206f 6620 4c61 746f 2e0a 2020 2020 2020   of Lato..      
-00001d10: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-00001d20: 6f6e 2031 2e33 2e31 3720 2872 656c 6561  on 1.3.17 (relea
-00001d30: 7365 6420 3230 3232 2d30 322d 3238 290a  sed 2022-02-28).
-00001d40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001d50: 202d 2041 6464 7320 6661 7669 636f 6e0a   - Adds favicon.
-00001d60: 2020 2020 2020 2020 2d20 4669 7820 6973          - Fix is
-00001d70: 7375 6520 7769 7468 2066 6c61 7368 206d  sue with flash m
-00001d80: 6573 7361 6765 206f 6e20 6c6f 6769 6e20  essage on login 
-00001d90: 7061 6765 206e 6f74 2062 6569 6e67 2073  page not being s
-00001da0: 6964 6520 746f 2073 6964 652e 0a20 2020  ide to side..   
-00001db0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-00001dc0: 7273 696f 6e20 312e 332e 3136 2028 7265  rsion 1.3.16 (re
-00001dd0: 6c65 6173 6564 2032 3032 322d 3032 2d31  leased 2022-02-1
-00001de0: 3729 0a20 2020 2020 2020 200a 2020 2020  7).        .    
-00001df0: 2020 2020 2d20 4164 6420 636f 6d6d 6f6e      - Add common
-00001e00: 2060 7371 7561 7265 2d70 6c61 6365 686f   `square-placeho
-00001e10: 6c64 6572 2e70 6e67 6020 696d 6167 6520  lder.png` image 
-00001e20: 666f 7220 6765 6e65 7261 6c20 7573 652e  for general use.
-00001e30: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001e40: 2020 5665 7273 696f 6e20 312e 332e 3135    Version 1.3.15
-00001e50: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
-00001e60: 3032 2d31 3729 0a20 2020 2020 2020 200a  02-17).        .
-00001e70: 2020 2020 2020 2020 2d20 5265 6d6f 7665          - Remove
-00001e80: 2063 7573 746f 6d20 6d61 7267 696e 2066   custom margin f
-00001e90: 726f 6d20 636c 6173 7365 7320 746f 2069  rom classes to i
-00001ea0: 6d70 726f 7665 2043 5353 206f 7665 7272  mprove CSS overr
-00001eb0: 6964 6162 696c 6974 792e 0a20 2020 2020  idability..     
-00001ec0: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00001ed0: 696f 6e20 312e 332e 3134 2028 7265 6c65  ion 1.3.14 (rele
-00001ee0: 6173 6564 2032 3032 322d 3032 2d31 3629  ased 2022-02-16)
-00001ef0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001f00: 2020 2d20 4669 7820 6973 7375 6520 7769    - Fix issue wi
-00001f10: 7468 204c 6174 6f20 666f 6e74 206e 6f74  th Lato font not
-00001f20: 2062 6569 6e67 206c 6f61 6465 6420 696e   being loaded in
-00001f30: 2053 656d 616e 7469 6320 5549 2074 6865   Semantic UI the
-00001f40: 6d65 2e0a 2020 2020 2020 2020 2d20 5365  me..        - Se
-00001f50: 7473 2053 656d 616e 7469 6320 5549 2040  ts Semantic UI @
-00001f60: 6d75 7465 6454 6578 7443 6f6c 6f72 2e0a  mutedTextColor..
-00001f70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001f80: 2056 6572 7369 6f6e 2031 2e33 2e31 3320   Version 1.3.13 
-00001f90: 2872 656c 6561 7365 6420 3230 3232 2d30  (released 2022-0
-00001fa0: 322d 3136 290a 2020 2020 2020 2020 0a20  2-16).        . 
-00001fb0: 2020 2020 2020 202d 2045 6e73 7572 6520         - Ensure 
-00001fc0: 636f 6d70 696c 6564 2074 7261 6e73 6c61  compiled transla
-00001fd0: 7469 6f6e 206d 6573 7361 6765 2063 6174  tion message cat
-00001fe0: 616c 6f67 7320 6172 6520 696e 636c 7564  alogs are includ
-00001ff0: 6564 2069 6e20 7468 650a 2020 2020 2020  ed in the.      
-00002000: 2020 2020 6469 7374 7269 6275 7469 6f6e      distribution
-00002010: 7320 7570 6c6f 6164 6564 206f 6e20 5079  s uploaded on Py
-00002020: 5049 2e0a 2020 2020 2020 2020 0a20 2020  PI..        .   
-00002030: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
-00002040: 2e31 3220 2872 656c 6561 7365 6420 3230  .12 (released 20
-00002050: 3232 2d30 322d 3134 290a 2020 2020 2020  22-02-14).      
-00002060: 2020 0a20 2020 2020 2020 202d 2046 6978    .        - Fix
-00002070: 6573 2041 3131 7920 6973 7375 6520 7769  es A11y issue wi
-00002080: 7468 2074 6865 2063 6c6f 7365 2062 7574  th the close but
-00002090: 746f 6e20 696e 2066 6c61 7368 206d 6573  ton in flash mes
-000020a0: 7361 6765 732e 0a20 2020 2020 2020 200a  sages..        .
-000020b0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
-000020c0: 312e 332e 3131 2028 7265 6c65 6173 6564  1.3.11 (released
-000020d0: 2032 3032 322d 3032 2d30 3829 0a20 2020   2022-02-08).   
-000020e0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-000020f0: 4164 6473 206d 6172 6769 6e20 6765 6e65  Adds margin gene
-00002100: 7261 746f 722e 0a20 2020 2020 2020 202d  rator..        -
-00002110: 2041 6464 7320 4131 3179 2070 6167 6520   Adds A11y page 
-00002120: 6c61 6e64 6d61 726b 732e 0a20 2020 2020  landmarks..     
-00002130: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00002140: 696f 6e20 312e 332e 3130 2028 7265 6c65  ion 1.3.10 (rele
-00002150: 6173 6564 2032 3032 312d 3131 2d32 3329  ased 2021-11-23)
-00002160: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002170: 2020 2d20 5765 6220 6163 6365 7373 6962    - Web accessib
-00002180: 696c 6974 7920 6669 782e 0a20 2020 2020  ility fix..     
-00002190: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-000021a0: 696f 6e20 312e 332e 3920 2872 656c 6561  ion 1.3.9 (relea
-000021b0: 7365 6420 3230 3231 2d30 372d 3132 290a  sed 2021-07-12).
-000021c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000021d0: 202d 2041 6464 7320 6765 726d 616e 2074   - Adds german t
-000021e0: 7261 6e73 6c61 7469 6f6e 730a 2020 2020  ranslations.    
-000021f0: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-00002200: 7369 6f6e 2031 2e33 2e38 2028 7265 6c65  sion 1.3.8 (rele
-00002210: 6173 6564 2032 3032 312d 3032 2d31 3029  ased 2021-02-10)
-00002220: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002230: 2020 2d20 4164 6473 2062 7261 6e64 2063    - Adds brand c
-00002240: 6f6c 6f72 2074 6f20 6d65 6e75 2069 7465  olor to menu ite
-00002250: 6d73 0a20 2020 2020 2020 200a 2020 2020  ms.        .    
-00002260: 2020 2020 5665 7273 696f 6e20 312e 332e      Version 1.3.
-00002270: 3720 2872 656c 6561 7365 6420 3230 3231  7 (released 2021
-00002280: 2d30 312d 3235 290a 2020 2020 2020 2020  -01-25).        
-00002290: 0a20 2020 2020 2020 202d 2041 6464 7320  .        - Adds 
-000022a0: 6272 616e 6420 636f 6c6f 7220 696e 2073  brand color in s
-000022b0: 6567 6d65 6e74 730a 2020 2020 2020 2020  egments.        
-000022c0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-000022d0: 2031 2e33 2e36 2028 7265 6c65 6173 6564   1.3.6 (released
-000022e0: 2032 3032 312d 3031 2d30 3429 0a20 2020   2021-01-04).   
-000022f0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00002300: 4164 6473 2060 6c69 6e6b 6020 7468 656d  Adds `link` them
-00002310: 6520 6963 6f6e 0a20 2020 2020 2020 202d  e icon.        -
-00002320: 2046 6978 6573 2077 696c 6463 6172 6420   Fixes wildcard 
-00002330: 6963 6f6e 2072 6573 6f6c 7574 696f 6e0a  icon resolution.
-00002340: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002350: 2056 6572 7369 6f6e 2031 2e33 2e35 2028   Version 1.3.5 (
-00002360: 7265 6c65 6173 6564 2032 3032 302d 3132  released 2020-12
-00002370: 2d31 3729 0a20 2020 2020 2020 200a 2020  -17).        .  
-00002380: 2020 2020 2020 2d20 4669 7865 7320 6368        - Fixes ch
-00002390: 6563 6b62 6f78 2e6f 7665 7272 6964 6573  eckbox.overrides
-000023a0: 2069 6e20 6069 6e76 656e 696f 6020 5355   in `invenio` SU
-000023b0: 4920 7061 636b 6167 6564 2074 6865 6d65  I packaged theme
-000023c0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000023d0: 2020 2056 6572 7369 6f6e 2031 2e33 2e34     Version 1.3.4
-000023e0: 2028 7265 6c65 6173 6564 2032 3032 302d   (released 2020-
-000023f0: 3132 2d31 3729 0a20 2020 2020 2020 200a  12-17).        .
-00002400: 2020 2020 2020 2020 2d20 4164 6473 2061          - Adds a
-00002410: 2066 756c 6c20 2269 6e76 656e 696f 2220   full "invenio" 
-00002420: 5365 6d61 6e74 6963 2055 4920 7061 636b  Semantic UI pack
-00002430: 6167 6564 2074 6865 6d65 2073 6f20 7765  aged theme so we
-00002440: 2063 616e 2065 6173 6965 7220 6375 7374   can easier cust
-00002450: 6f6d 697a 650a 2020 2020 2020 2020 2020  omize.          
-00002460: 6c61 796f 7574 2069 6e20 7468 6520 6675  layout in the fu
-00002470: 7475 7265 2e0a 2020 2020 2020 2020 0a20  ture..        . 
-00002480: 2020 2020 2020 202d 204d 6f76 6573 2074         - Moves t
-00002490: 6865 6d65 2e63 6f6e 6669 6720 746f 2074  heme.config to t
-000024a0: 6865 6d65 2e63 6f6e 6669 672e 6578 616d  heme.config.exam
-000024b0: 706c 6520 616e 6420 6164 6473 2061 206e  ple and adds a n
-000024c0: 6f74 6520 746f 206d 616b 6520 6974 0a20  ote to make it. 
-000024d0: 2020 2020 2020 2020 2063 6c65 6172 2074           clear t
-000024e0: 6865 2066 696c 6520 6973 206e 6f74 2061  he file is not a
-000024f0: 6374 7561 6c6c 7920 7573 6564 2c20 6275  ctually used, bu
-00002500: 7420 6973 206a 7573 7420 616e 2065 7861  t is just an exa
-00002510: 6d70 6c65 2e0a 2020 2020 2020 2020 0a20  mple..        . 
-00002520: 2020 2020 2020 202d 2041 6464 7320 6865         - Adds he
-00002530: 6c70 6572 2074 6f6f 6c20 666f 7220 7375  lper tool for su
-00002540: 7070 6f72 7469 6e67 2074 6865 6d65 2064  pporting theme d
-00002550: 6570 656e 6465 6e74 2069 636f 6e73 2e0a  ependent icons..
-00002560: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002570: 202d 2046 6978 6573 206d 616e 7920 6d69   - Fixes many mi
-00002580: 6e6f 7220 7374 796c 696e 6720 6973 7375  nor styling issu
-00002590: 6573 2073 7563 6820 6173 2061 6c69 676e  es such as align
-000025a0: 6d65 6e74 732c 2062 7574 746f 6e20 6c6f  ments, button lo
-000025b0: 6361 7469 6f6e 732c 0a20 2020 2020 2020  cations,.       
-000025c0: 2020 2067 7269 6473 2e0a 2020 2020 2020     grids..      
-000025d0: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
-000025e0: 6f6e 2031 2e33 2e33 2028 7265 6c65 6173  on 1.3.3 (releas
-000025f0: 6564 2032 3032 302d 3132 2d31 3129 0a20  ed 2020-12-11). 
-00002600: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002610: 2d20 496e 6974 6961 6c69 7a65 7320 7365  - Initializes se
-00002620: 6d61 6e74 6963 5549 2061 6363 6f72 6469  manticUI accordi
-00002630: 6f6e 2063 6f6d 706f 6e65 6e74 732e 0a20  on components.. 
-00002640: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002650: 5665 7273 696f 6e20 312e 332e 3220 2872  Version 1.3.2 (r
-00002660: 656c 6561 7365 6420 3230 3230 2d31 322d  eleased 2020-12-
-00002670: 3131 290a 2020 2020 2020 2020 0a20 2020  11).        .   
-00002680: 2020 2020 202d 2055 7064 6174 6573 2074       - Updates t
-00002690: 6865 2049 6e76 656e 696f 206c 6f67 6f20  he Invenio logo 
-000026a0: 616e 6420 7265 6d6f 7665 206f 7574 6461  and remove outda
-000026b0: 7465 6420 7665 7273 696f 6e73 2e0a 2020  ted versions..  
-000026c0: 2020 2020 2020 2d20 4669 7865 7320 7468        - Fixes th
-000026d0: 6520 6472 6f70 646f 776e 2074 6f20 776f  e dropdown to wo
-000026e0: 726b 206f 6e20 7468 6520 7573 6572 2070  rk on the user p
-000026f0: 726f 6669 6c65 2070 6167 652e 0a20 2020  rofile page..   
-00002700: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-00002710: 7273 696f 6e20 312e 332e 3120 2872 656c  rsion 1.3.1 (rel
-00002720: 6561 7365 6420 3230 3230 2d31 322d 3039  eased 2020-12-09
-00002730: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002740: 2020 202d 204d 696e 6f72 2066 6978 2066     - Minor fix f
-00002750: 6f72 2053 656d 616e 7469 6355 4920 6472  or SemanticUI dr
-00002760: 6f70 646f 776e 730a 2020 2020 2020 2020  opdowns.        
-00002770: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
-00002780: 2031 2e33 2e30 2028 7265 6c65 6173 6564   1.3.0 (released
-00002790: 2032 3032 302d 3132 2d30 3929 0a20 2020   2020-12-09).   
-000027a0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-000027b0: 4d61 6a6f 723a 204e 6577 2053 656d 616e  Major: New Seman
-000027c0: 7469 6355 4920 7468 656d 6520 6861 7320  ticUI theme has 
-000027d0: 6265 656e 2069 6e74 6567 7261 7465 642e  been integrated.
-000027e0: 2054 6865 2042 6f6f 7473 7472 6170 2033   The Bootstrap 3
-000027f0: 2074 6865 6d65 2073 7469 6c6c 0a20 2020   theme still.   
-00002800: 2020 2020 2020 2065 7869 7374 732e 2054         exists. T
-00002810: 6869 7320 6368 616e 6765 2064 6570 656e  his change depen
-00002820: 6473 206f 6e20 7468 6520 6c61 7465 7374  ds on the latest
-00002830: 2072 656c 6561 7365 6420 496e 7665 6e69   released Inveni
-00002840: 6f2d 4173 7365 7473 2077 6869 6368 0a20  o-Assets which. 
-00002850: 2020 2020 2020 2020 2061 6464 7320 7375           adds su
-00002860: 7070 6f72 7473 2066 6f72 206d 756c 7469  pports for multi
-00002870: 706c 6520 5549 2066 7261 6d65 776f 726b  ple UI framework
-00002880: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00002890: 2020 2020 2d20 4164 6473 2073 7570 706f      - Adds suppo
-000028a0: 7274 2066 6f72 2064 796e 616d 6963 206c  rt for dynamic l
-000028b0: 6f61 6469 6e67 206f 6620 7465 6d70 6c61  oading of templa
-000028c0: 7465 7320 666f 7220 5265 6163 742d 4f76  tes for React-Ov
-000028d0: 6572 7269 6461 626c 652e 0a20 2020 2020  erridable..     
-000028e0: 2020 200a 2020 2020 2020 2020 2d20 4261     .        - Ba
-000028f0: 636b 7761 7264 7320 696e 636f 6d70 6174  ckwards incompat
-00002900: 6962 6c65 3a20 5468 6520 6f6c 642d 7374  ible: The old-st
-00002910: 796c 6520 466c 6173 6b2d 4173 7365 7420  yle Flask-Asset 
-00002920: 6275 6e64 6c65 7320 7761 7320 7265 6d6f  bundles was remo
-00002930: 7665 6420 2874 6865 7365 0a20 2020 2020  ved (these.     
-00002940: 2020 2020 2062 756e 646c 6573 2077 6572       bundles wer
-00002950: 6520 6465 7072 6563 6174 6564 2069 6e20  e deprecated in 
-00002960: 496e 7665 6e69 6f20 7633 2e31 292e 0a20  Invenio v3.1).. 
-00002970: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002980: 2d20 4164 6473 2054 7572 6b69 7368 2074  - Adds Turkish t
-00002990: 7261 6e73 6c61 7469 6f6e 732e 0a20 2020  ranslations..   
-000029a0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
-000029b0: 7273 696f 6e20 312e 322e 3020 2872 656c  rsion 1.2.0 (rel
-000029c0: 6561 7365 6420 3230 3230 2d30 332d 3230  eased 2020-03-20
-000029d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000029e0: 2020 202d 2052 6570 6c61 6365 7320 466c     - Replaces Fl
-000029f0: 6173 6b20 6465 7065 6e64 656e 6379 2077  ask dependency w
-00002a00: 6974 6820 6060 696e 7665 6e69 6f2d 6261  ith ``invenio-ba
-00002a10: 7365 6060 2e0a 2020 2020 2020 2020 0a20  se``..        . 
-00002a20: 2020 2020 2020 2056 6572 7369 6f6e 2031         Version 1
-00002a30: 2e31 2e34 2028 7265 6c65 6173 6564 2032  .1.4 (released 2
-00002a40: 3031 392d 3037 2d32 3229 0a20 2020 2020  019-07-22).     
-00002a50: 2020 200a 2020 2020 2020 2020 2d20 496e     .        - In
-00002a60: 7472 6f64 7563 6520 6861 6e64 6c69 6e67  troduce handling
-00002a70: 206f 6620 7468 6520 6572 726f 7220 3432   of the error 42
-00002a80: 392e 0a20 2020 2020 2020 200a 2020 2020  9..        .    
-00002a90: 2020 2020 5665 7273 696f 6e20 312e 312e      Version 1.1.
-00002aa0: 3320 2872 656c 6561 7365 6420 3230 3139  3 (released 2019
-00002ab0: 2d30 332d 3133 290a 2020 2020 2020 2020  -03-13).        
-00002ac0: 0a20 2020 2020 2020 202d 2052 6573 7472  .        - Restr
-00002ad0: 7563 7475 7265 2053 4353 5320 6669 6c65  ucture SCSS file
-00002ae0: 732c 2069 6e20 6f72 6465 7220 746f 2061  s, in order to a
-00002af0: 6c6c 6f77 2065 6173 6965 7220 6375 7374  llow easier cust
-00002b00: 6f6d 697a 6174 696f 6e20 616e 6420 6578  omization and ex
-00002b10: 7465 6e73 696f 6e0a 2020 2020 2020 2020  tension.        
-00002b20: 2020 696e 206f 7665 726c 6179 732e 0a20    in overlays.. 
-00002b30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002b40: 5665 7273 696f 6e20 312e 312e 3220 2872  Version 1.1.2 (r
-00002b50: 656c 6561 7365 6420 3230 3139 2d30 322d  eleased 2019-02-
-00002b60: 3135 290a 2020 2020 2020 2020 0a20 2020  15).        .   
-00002b70: 2020 2020 202d 2055 7067 7261 6465 6420       - Upgraded 
-00002b80: 6d6f 6d65 6e74 2074 6f20 322e 3233 2e30  moment to 2.23.0
-00002b90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002ba0: 2020 5665 7273 696f 6e20 312e 312e 3120    Version 1.1.1 
-00002bb0: 2872 656c 6561 7365 6420 3230 3138 2d31  (released 2018-1
-00002bc0: 322d 3035 290a 2020 2020 2020 2020 0a20  2-05).        . 
-00002bd0: 2020 2020 2020 202d 2046 6978 6573 2069         - Fixes i
-00002be0: 7373 7565 7320 7769 7468 2077 6562 7061  ssues with webpa
-00002bf0: 636b 2061 6e64 2074 6865 2041 646d 696e  ck and the Admin
-00002c00: 4c54 4520 7468 656d 652e 0a20 2020 2020  LTE theme..     
-00002c10: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
-00002c20: 696f 6e20 312e 312e 3020 2872 656c 6561  ion 1.1.0 (relea
-00002c30: 7365 6420 3230 3138 2d31 312d 3036 290a  sed 2018-11-06).
-00002c40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002c50: 202d 2049 6e74 726f 6475 6365 2077 6562   - Introduce web
-00002c60: 7061 636b 2073 7570 706f 7274 2e0a 2020  pack support..  
-00002c70: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
-00002c80: 6572 7369 6f6e 2031 2e30 2e30 2028 7265  ersion 1.0.0 (re
-00002c90: 6c65 6173 6564 2032 3031 382d 3033 2d32  leased 2018-03-2
-00002ca0: 3329 0a20 2020 2020 2020 200a 2020 2020  3).        .    
-00002cb0: 2020 2020 2d20 496e 6974 6961 6c20 7075      - Initial pu
-00002cc0: 626c 6963 2072 656c 6561 7365 2e0a 2020  blic release..  
-00002cd0: 2020 2020 2020 0a4b 6579 776f 7264 733a        .Keywords:
-00002ce0: 2069 6e76 656e 696f 0a50 6c61 7466 6f72   invenio.Platfor
-00002cf0: 6d3a 2061 6e79 0a43 6c61 7373 6966 6965  m: any.Classifie
-00002d00: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
-00002d10: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
-00002d20: 6475 6374 696f 6e2f 5374 6162 6c65 0a52  duction/Stable.R
-00002d30: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00002d40: 3e3d 332e 370a 5072 6f76 6964 6573 2d45  >=3.7.Provides-E
-00002d50: 7874 7261 3a20 7465 7374 730a 5072 6f76  xtra: tests.Prov
-00002d60: 6964 6573 2d45 7874 7261 3a20 646f 6373  ides-Extra: docs
-00002d70: 0a                                       .
+000007d0: 6572 7369 6f6e 2033 2e31 2e30 2028 7265  ersion 3.1.0 (re
+000007e0: 6c65 6173 6564 2032 3032 342d 3034 2d31  leased 2024-04-1
+000007f0: 3029 0a20 2020 2020 2020 200a 2020 2020  0).        .    
+00000800: 2020 2020 2d20 6373 733a 2066 6978 206f      - css: fix o
+00000810: 7665 7266 6c6f 7720 666f 7220 6465 7363  verflow for desc
+00000820: 7269 7074 696f 6e20 696e 2072 6563 6f72  ription in recor
+00000830: 6420 6465 7461 696c 730a 2020 2020 2020  d details.      
+00000840: 2020 2d20 6275 673a 2061 6464 206d 6973    - bug: add mis
+00000850: 7369 6e67 2060 603c 7469 746c 653e 7360  sing ``<title>s`
+00000860: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
+00000870: 2020 2056 6572 7369 6f6e 2033 2e30 2e30     Version 3.0.0
+00000880: 2028 7265 6c65 6173 6564 2032 3032 342d   (released 2024-
+00000890: 3033 2d31 3929 0a20 2020 2020 2020 200a  03-19).        .
+000008a0: 2020 2020 2020 2020 2d20 676c 6f62 616c          - global
+000008b0: 3a20 7265 6d6f 7665 2062 7265 6164 6372  : remove breadcr
+000008c0: 756d 6220 7375 7070 6f72 740a 2020 2020  umb support.    
+000008d0: 2020 2020 2d20 676c 6f62 616c 3a20 696e      - global: in
+000008e0: 7472 6f64 7563 6520 7368 6172 6564 206d  troduce shared m
+000008f0: 656e 750a 2020 2020 2020 2020 2d20 676c  enu.        - gl
+00000900: 6f62 616c 3a20 7072 6570 6172 6174 696f  obal: preparatio
+00000910: 6e20 666f 7220 636f 6d70 6174 6962 696c  n for compatibil
+00000920: 6974 7920 7769 7468 2046 6c61 736b 2076  ity with Flask v
+00000930: 322e 332e 7820 6465 7072 6563 6174 696f  2.3.x deprecatio
+00000940: 6e73 0a20 2020 2020 2020 202d 2072 6566  ns.        - ref
+00000950: 6163 746f 723a 2063 7572 7265 6e74 5f74  actor: current_t
+00000960: 6865 6d65 5f69 636f 6e73 2077 6974 686f  heme_icons witho
+00000970: 7574 2061 7070 6c69 6361 7469 6f6e 2063  ut application c
+00000980: 6f6e 7465 7874 0a20 2020 2020 2020 200a  ontext.        .
+00000990: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+000009a0: 322e 352e 3130 2028 7265 6c65 6173 6564  2.5.10 (released
+000009b0: 2032 3032 342d 3031 2d32 3829 0a20 2020   2024-01-28).   
+000009c0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+000009d0: 696e 7374 616c 6c61 7469 6f6e 3a20 6669  installation: fi
+000009e0: 7820 7370 6869 6e78 2064 6570 656e 6465  x sphinx depende
+000009f0: 6e63 790a 2020 2020 2020 2020 0a20 2020  ncy.        .   
+00000a00: 2020 2020 2056 6572 7369 6f6e 2032 2e35       Version 2.5
+00000a10: 2e39 2028 7265 6c65 6173 6564 2032 3032  .9 (released 202
+00000a20: 342d 3031 2d32 3829 0a20 2020 2020 2020  4-01-28).       
+00000a30: 200a 2020 2020 2020 2020 2d20 676c 6f62   .        - glob
+00000a40: 616c 3a20 6368 616e 6765 206d 6174 6820  al: change math 
+00000a50: 6f70 6572 6174 696f 6e20 746f 2062 6520  operation to be 
+00000a60: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+00000a70: 7361 7373 322e 300a 2020 2020 2020 2020  sass2.0.        
+00000a80: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00000a90: 2032 2e35 2e38 2028 7265 6c65 6173 6564   2.5.8 (released
+00000aa0: 2032 3032 332d 3132 2d31 3229 0a20 2020   2023-12-12).   
+00000ab0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00000ac0: 7265 706c 6163 6520 636b 6564 6974 6f72  replace ckeditor
+00000ad0: 2077 6974 6820 7469 6e79 6d63 6520 6475   with tinymce du
+00000ae0: 6520 746f 206c 6963 656e 7365 2069 7373  e to license iss
+00000af0: 7565 0a20 2020 2020 2020 200a 2020 2020  ue.        .    
+00000b00: 2020 2020 5665 7273 696f 6e20 322e 352e      Version 2.5.
+00000b10: 3720 2872 656c 6561 7365 6420 3230 3233  7 (released 2023
+00000b20: 2d31 302d 3236 290a 2020 2020 2020 2020  -10-26).        
+00000b30: 0a20 2020 2020 2020 202d 2063 6f6d 6d75  .        - commu
+00000b40: 6e69 7479 206c 6f67 6f3a 2066 6978 2072  nity logo: fix r
+00000b50: 656e 6465 7269 6e67 2061 2070 6c61 6365  endering a place
+00000b60: 686f 6c64 6572 0a20 2020 2020 2020 200a  holder.        .
+00000b70: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00000b80: 322e 352e 3620 2872 656c 6561 7365 6420  2.5.6 (released 
+00000b90: 3230 3233 2d31 302d 3230 290a 2020 2020  2023-10-20).    
+00000ba0: 2020 2020 0a20 2020 2020 2020 202d 2064      .        - d
+00000bb0: 6f6e 2774 206f 7665 7272 6964 6520 6c69  on't override li
+00000bc0: 6e6b 7320 7374 796c 6520 696e 2066 6c61  nks style in fla
+00000bd0: 7368 6564 206d 6573 7361 6765 730a 2020  shed messages.  
+00000be0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+00000bf0: 6572 7369 6f6e 2032 2e35 2e35 2028 7265  ersion 2.5.5 (re
+00000c00: 6c65 6173 6564 2032 3032 332d 3039 2d31  leased 2023-09-1
+00000c10: 3929 0a20 2020 2020 2020 200a 2020 2020  9).        .    
+00000c20: 2020 2020 2d20 7374 796c 696e 673a 2061      - styling: a
+00000c30: 6464 2033 2063 6f6c 756d 6e20 7465 6d70  dd 3 column temp
+00000c40: 6c61 7465 2063 6c61 7373 0a20 2020 2020  late class.     
+00000c50: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00000c60: 696f 6e20 322e 352e 3420 2872 656c 6561  ion 2.5.4 (relea
+00000c70: 7365 6420 3230 3233 2d30 392d 3131 290a  sed 2023-09-11).
+00000c80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000c90: 202d 2073 6373 733a 2066 6978 2063 6f6d   - scss: fix com
+00000ca0: 7061 7469 6269 6c69 7479 2077 6974 6820  patibility with 
+00000cb0: 6c61 7465 7374 206c 6573 7320 7665 7273  latest less vers
+00000cc0: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
+00000cd0: 2020 2020 2056 6572 7369 6f6e 2032 2e35       Version 2.5
+00000ce0: 2e33 2028 7265 6c65 6173 6564 2032 3032  .3 (released 202
+00000cf0: 332d 3038 2d30 3829 0a20 2020 2020 2020  3-08-08).       
+00000d00: 200a 2020 2020 2020 2020 2d20 7374 796c   .        - styl
+00000d10: 6573 6865 6574 733a 2061 6464 2070 7265  esheets: add pre
+00000d20: 666f 726d 6174 7465 6420 7461 6720 7374  formatted tag st
+00000d30: 796c 696e 6720 666f 6e74 0a20 2020 2020  yling font.     
+00000d40: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00000d50: 696f 6e20 322e 352e 3220 2872 656c 6561  ion 2.5.2 (relea
+00000d60: 7365 6420 3230 3233 2d30 382d 3134 290a  sed 2023-08-14).
+00000d70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000d80: 202d 2069 6e73 7461 6c6c 6174 696f 6e3a   - installation:
+00000d90: 2070 696e 2046 6c61 736b 2d4d 656e 7520   pin Flask-Menu 
+00000da0: 746f 2060 603c 7631 2e30 2e30 6060 2e0a  to ``<v1.0.0``..
+00000db0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000dc0: 2056 6572 7369 6f6e 2032 2e35 2e31 2028   Version 2.5.1 (
+00000dd0: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
+00000de0: 2d31 3429 0a20 2020 2020 2020 200a 2020  -14).        .  
+00000df0: 2020 2020 2020 2d20 7468 656d 653a 2062        - theme: b
+00000e00: 7567 6669 7820 746f 2064 6563 7265 6173  ugfix to decreas
+00000e10: 6520 7a2d 696e 6465 7820 7661 6c75 650a  e z-index value.
+00000e20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000e30: 2056 6572 7369 6f6e 2032 2e35 2e30 2028   Version 2.5.0 (
+00000e40: 7265 6c65 6173 6564 2032 3032 332d 3038  released 2023-08
+00000e50: 2d30 3929 0a20 2020 2020 2020 200a 2020  -09).        .  
+00000e60: 2020 2020 2020 2d20 7468 656d 653a 2061        - theme: a
+00000e70: 6464 2075 7469 6c69 7479 2063 6c61 7373  dd utility class
+00000e80: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
+00000e90: 2020 2020 5665 7273 696f 6e20 322e 342e      Version 2.4.
+00000ea0: 3020 2872 656c 6561 7365 6420 3230 3233  0 (released 2023
+00000eb0: 2d30 382d 3032 290a 2020 2020 2020 2020  -08-02).        
+00000ec0: 0a20 2020 2020 2020 202d 2074 6865 6d65  .        - theme
+00000ed0: 3a20 6164 6420 736f 6d65 2067 656e 6572  : add some gener
+00000ee0: 616c 2063 6c61 7373 6573 2061 6e64 2066  al classes and f
+00000ef0: 6978 6573 2061 6c69 676e 6d65 6e74 2066  ixes alignment f
+00000f00: 6f72 206c 6162 656c 6564 2066 6c75 6964  or labeled fluid
+00000f10: 2062 7574 746f 6e73 0a20 2020 2020 2020   buttons.       
+00000f20: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
+00000f30: 6e20 322e 332e 3020 2872 656c 6561 7365  n 2.3.0 (release
+00000f40: 6420 3230 3233 2d30 372d 3331 290a 2020  d 2023-07-31).  
+00000f50: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00000f60: 2073 6574 7469 6e67 7320 7061 6765 3a20   settings page: 
+00000f70: 496d 7072 6f76 6520 7465 6d70 6c61 7465  Improve template
+00000f80: 2066 6f72 2061 3131 790a 2020 2020 2020   for a11y.      
+00000f90: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
+00000fa0: 6f6e 2032 2e32 2e30 2028 7265 6c65 6173  on 2.2.0 (releas
+00000fb0: 6564 2032 3032 332d 3037 2d32 3629 0a20  ed 2023-07-26). 
+00000fc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000fd0: 2d20 7468 656d 653a 2061 6464 2067 656e  - theme: add gen
+00000fe0: 6572 616c 2073 7479 6c65 2069 6d70 726f  eral style impro
+00000ff0: 7665 6d65 6e74 730a 2020 2020 2020 2020  vements.        
+00001000: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00001010: 2032 2e31 2e33 2028 7265 6c65 6173 6564   2.1.3 (released
+00001020: 2032 3032 332d 3037 2d32 3429 0a20 2020   2023-07-24).   
+00001030: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001040: 6d65 7373 6167 6573 3a20 6164 6420 7a2d  messages: add z-
+00001050: 696e 6465 780a 2020 2020 2020 2020 0a20  index.        . 
+00001060: 2020 2020 2020 2056 6572 7369 6f6e 2032         Version 2
+00001070: 2e31 2e32 2028 7265 6c65 6173 6564 2032  .1.2 (released 2
+00001080: 3032 332d 3034 2d31 3229 0a20 2020 2020  023-04-12).     
+00001090: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
+000010a0: 6420 666c 6578 2075 7469 6c69 7479 2063  d flex utility c
+000010b0: 6c61 7373 6573 0a20 2020 2020 2020 202d  lasses.        -
+000010c0: 2061 6464 2074 6578 7420 7369 7a65 7320   add text sizes 
+000010d0: 636c 6173 7365 730a 2020 2020 2020 2020  classes.        
+000010e0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+000010f0: 2032 2e31 2e31 2028 7265 6c65 6173 6564   2.1.1 (released
+00001100: 2032 3032 332d 3034 2d30 3629 0a20 2020   2023-04-06).   
+00001110: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001120: 6164 6420 6469 7370 6c61 7920 7574 696c  add display util
+00001130: 6974 7920 636c 6173 7365 730a 2020 2020  ity classes.    
+00001140: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00001150: 7369 6f6e 2032 2e31 2e30 2028 7265 6c65  sion 2.1.0 (rele
+00001160: 6173 6564 2032 3032 332d 3033 2d32 3829  ased 2023-03-28)
+00001170: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001180: 2020 2d20 6164 6420 676c 6f62 616c 2075    - add global u
+00001190: 7469 6c69 7479 2073 7479 6c69 6e67 2063  tility styling c
+000011a0: 6c61 7373 6573 0a20 2020 2020 2020 200a  lasses.        .
+000011b0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+000011c0: 322e 302e 3120 2872 656c 6561 7365 6420  2.0.1 (released 
+000011d0: 3230 3233 2d30 332d 3039 290a 2020 2020  2023-03-09).    
+000011e0: 2020 2020 0a20 2020 2020 2020 202d 2066      .        - f
+000011f0: 6978 2073 7479 6c69 6e67 2066 6f72 2062  ix styling for b
+00001200: 7574 746f 6e73 0a20 2020 2020 2020 202d  uttons.        -
+00001210: 206d 6f76 6520 676c 6f62 616c 2063 6c61   move global cla
+00001220: 7373 2066 6f72 2061 7574 6f20 6772 6964  ss for auto grid
+00001230: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001240: 2020 5665 7273 696f 6e20 322e 302e 3020    Version 2.0.0 
+00001250: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
+00001260: 322d 3238 290a 2020 2020 2020 2020 0a20  2-28).        . 
+00001270: 2020 2020 2020 202d 2064 726f 7020 7079         - drop py
+00001280: 7468 6f6e 2032 2e37 2073 7570 706f 7274  thon 2.7 support
+00001290: 0a20 2020 2020 2020 202d 2072 656d 6f76  .        - remov
+000012a0: 6520 666c 6173 6b5f 6261 6265 6c65 7820  e flask_babelex 
+000012b0: 696d 706f 7274 730a 2020 2020 2020 2020  imports.        
+000012c0: 2d20 7570 6772 6164 6520 696e 7665 6e69  - upgrade inveni
+000012d0: 6f5f 6931 386e 0a20 2020 2020 2020 200a  o_i18n.        .
+000012e0: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+000012f0: 312e 342e 3820 2872 656c 6561 7365 6420  1.4.8 (released 
+00001300: 3230 3233 2d30 322d 3037 290a 2020 2020  2023-02-07).    
+00001310: 2020 2020 0a20 2020 2020 2020 202d 2074      .        - t
+00001320: 6865 6d65 3a20 6164 6420 6175 746f 2d63  heme: add auto-c
+00001330: 6f6c 756d 6e2d 6772 6964 2063 6c61 7373  olumn-grid class
+00001340: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001350: 2020 5665 7273 696f 6e20 312e 342e 3720    Version 1.4.7 
+00001360: 2872 656c 6561 7365 6420 3230 3233 2d30  (released 2023-0
+00001370: 312d 3035 290a 2020 2020 2020 2020 0a20  1-05).        . 
+00001380: 2020 2020 2020 202d 2061 6464 2074 7275         - add tru
+00001390: 6e63 6174 6520 6c69 6e65 7320 7374 796c  ncate lines styl
+000013a0: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
+000013b0: 2020 2020 5665 7273 696f 6e20 312e 342e      Version 1.4.
+000013c0: 3620 2872 656c 6561 7365 6420 3230 3232  6 (released 2022
+000013d0: 2d31 322d 3038 290a 2020 2020 2020 2020  -12-08).        
+000013e0: 0a20 2020 2020 2020 202d 2066 6978 2073  .        - fix s
+000013f0: 7479 6c69 6e67 2066 6f72 2069 6e6c 696e  tyling for inlin
+00001400: 6520 636c 6173 732c 2061 6666 6563 7469  e class, affecti
+00001410: 6e67 2066 6f72 6d20 6669 656c 6473 0a20  ng form fields. 
+00001420: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001430: 5665 7273 696f 6e20 312e 342e 3520 2872  Version 1.4.5 (r
+00001440: 656c 6561 7365 6420 3230 3232 2d31 322d  eleased 2022-12-
+00001450: 3031 290a 2020 2020 2020 2020 0a20 2020  01).        .   
+00001460: 2020 2020 202d 2066 6978 2073 6561 7263       - fix searc
+00001470: 6820 7265 7375 6c74 2069 7465 6d20 7374  h result item st
+00001480: 796c 696e 670a 2020 2020 2020 2020 2d20  yling.        - 
+00001490: 6164 6420 676c 6f62 616c 2062 6568 6176  add global behav
+000014a0: 696f 7572 2063 6c61 7373 6573 0a20 2020  iour classes.   
+000014b0: 2020 2020 202d 2061 6464 2070 6c61 6365       - add place
+000014c0: 686f 6c64 6572 2069 6d61 6765 2068 616e  holder image han
+000014d0: 646c 650a 2020 2020 2020 2020 0a20 2020  dle.        .   
+000014e0: 2020 2020 2056 6572 7369 6f6e 2031 2e34       Version 1.4
+000014f0: 2e34 2028 7265 6c65 6173 6564 2032 3032  .4 (released 202
+00001500: 322d 3131 2d31 3829 0a20 2020 2020 2020  2-11-18).       
+00001510: 200a 2020 2020 2020 2020 2d20 4164 6420   .        - Add 
+00001520: 7075 6c6c 6564 2074 7261 6e73 6c61 7469  pulled translati
+00001530: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+00001540: 2020 2020 2056 6572 7369 6f6e 2031 2e34       Version 1.4
+00001550: 2e33 2028 7265 6c65 6173 6564 2032 3032  .3 (released 202
+00001560: 322d 3131 2d30 3329 0a20 2020 2020 2020  2-11-03).       
+00001570: 200a 2020 2020 2020 2020 2d20 6164 6420   .        - add 
+00001580: 7374 796c 696e 6720 666f 7220 6472 6f70  styling for drop
+00001590: 646f 776e 206d 656e 7520 6974 656d 730a  down menu items.
+000015a0: 2020 2020 2020 2020 2d20 6669 7820 6d69          - fix mi
+000015b0: 7373 696e 6720 4d65 6469 6120 636f 6d70  ssing Media comp
+000015c0: 6f6e 656e 7420 7261 6e67 650a 2020 2020  onent range.    
+000015d0: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+000015e0: 7369 6f6e 2031 2e34 2e32 2028 7265 6c65  sion 1.4.2 (rele
+000015f0: 6173 6564 2032 3032 322d 3130 2d32 3629  ased 2022-10-26)
+00001600: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001610: 2020 2d20 6164 6420 4d65 6469 6120 746f    - add Media to
+00001620: 2073 7570 706f 7274 2072 6573 706f 6e73   support respons
+00001630: 6976 6520 7265 6163 7420 636f 6d70 6f6e  ive react compon
+00001640: 656e 7473 0a20 2020 2020 2020 200a 2020  ents.        .  
+00001650: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001660: 342e 3120 2872 656c 6561 7365 6420 3230  4.1 (released 20
+00001670: 3232 2d31 302d 3130 290a 2020 2020 2020  22-10-10).      
+00001680: 2020 0a20 2020 2020 2020 202d 2062 756d    .        - bum
+00001690: 7020 5365 6d61 6e74 6963 5549 0a20 2020  p SemanticUI.   
+000016a0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
+000016b0: 7273 696f 6e20 312e 342e 3020 2872 656c  rsion 1.4.0 (rel
+000016c0: 6561 7365 6420 3230 3232 2d31 302d 3035  eased 2022-10-05
+000016d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000016e0: 2020 202d 2063 6861 6e67 6520 676c 6f62     - change glob
+000016f0: 616c 2066 6f6e 7420 746f 204c 6174 6f0a  al font to Lato.
+00001700: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001710: 2056 6572 7369 6f6e 2031 2e33 2e33 3120   Version 1.3.31 
+00001720: 2872 656c 6561 7365 6420 3230 3232 2d31  (released 2022-1
+00001730: 302d 3035 290a 2020 2020 2020 2020 0a20  0-05).        . 
+00001740: 2020 2020 2020 202d 2061 6464 206d 6973         - add mis
+00001750: 7369 6e67 2074 6865 6d65 2076 6172 6961  sing theme varia
+00001760: 626c 6573 0a20 2020 2020 2020 200a 2020  bles.        .  
+00001770: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001780: 332e 3330 2028 7265 6c65 6173 6564 2032  3.30 (released 2
+00001790: 3032 322d 3039 2d32 3629 0a20 2020 2020  022-09-26).     
+000017a0: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
+000017b0: 6420 7374 796c 696e 6720 746f 2061 646d  d styling to adm
+000017c0: 696e 6973 7472 6174 696f 6e20 6461 7368  inistration dash
+000017d0: 626f 6172 6420 7061 6765 0a20 2020 2020  board page.     
+000017e0: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+000017f0: 696f 6e20 312e 332e 3239 2028 7265 6c65  ion 1.3.29 (rele
+00001800: 6173 6564 2032 3032 322d 3039 2d32 3229  ased 2022-09-22)
+00001810: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001820: 2020 2d20 6164 6420 6164 6d69 6e69 7374    - add administ
+00001830: 7261 7469 6f6e 2070 616e 656c 2073 7479  ration panel sty
+00001840: 6c69 6e67 0a20 2020 2020 2020 202d 2061  ling.        - a
+00001850: 6464 2074 7261 6e73 6c61 7469 6f6e 2077  dd translation w
+00001860: 6f72 6b66 6c6f 770a 2020 2020 2020 2020  orkflow.        
+00001870: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00001880: 2031 2e33 2e32 3820 2872 656c 6561 7365   1.3.28 (release
+00001890: 6420 3230 3232 2d30 372d 3038 290a 2020  d 2022-07-08).  
+000018a0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+000018b0: 2061 6464 2073 7479 6c69 6e67 2063 6c61   add styling cla
+000018c0: 7373 6573 2077 6974 6820 6163 7469 6f6e  sses with action
+000018d0: 2063 6f6c 6f72 2063 6f64 696e 670a 2020   color coding.  
+000018e0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+000018f0: 6572 7369 6f6e 2031 2e33 2e32 3720 2872  ersion 1.3.27 (r
+00001900: 656c 6561 7365 6420 3230 3232 2d30 372d  eleased 2022-07-
+00001910: 3037 290a 2020 2020 2020 2020 0a20 2020  07).        .   
+00001920: 2020 2020 202d 2066 6978 206a 7175 6572       - fix jquer
+00001930: 7920 7265 6665 7265 6e63 650a 2020 2020  y reference.    
+00001940: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00001950: 7369 6f6e 2031 2e33 2e32 3620 2872 656c  sion 1.3.26 (rel
+00001960: 6561 7365 6420 3230 3232 2d30 372d 3037  eased 2022-07-07
+00001970: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00001980: 2020 202d 2061 6464 2069 6d61 6765 2070     - add image p
+00001990: 6c61 6365 686f 6c64 6572 206f 6e20 6c6f  laceholder on lo
+000019a0: 6164 2065 7272 6f72 0a20 2020 2020 2020  ad error.       
+000019b0: 200a 2020 2020 2020 2020 5665 7273 696f   .        Versio
+000019c0: 6e20 312e 332e 3235 2028 7265 6c65 6173  n 1.3.25 (releas
+000019d0: 6564 2032 3032 322d 3036 2d32 3729 0a20  ed 2022-06-27). 
+000019e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000019f0: 2d20 6164 6420 4765 726d 616e 2074 7261  - add German tra
+00001a00: 6e73 6c61 7469 6f6e 730a 2020 2020 2020  nslations.      
+00001a10: 2020 2d20 6669 7820 6472 6f70 646f 776e    - fix dropdown
+00001a20: 2073 6372 6f6c 6c20 6d69 7361 6c69 676e   scroll misalign
+00001a30: 6d65 6e74 0a20 2020 2020 2020 200a 2020  ment.        .  
+00001a40: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001a50: 332e 3234 2028 7265 6c65 6173 6564 2032  3.24 (released 2
+00001a60: 3032 322d 3035 2d32 3329 0a20 2020 2020  022-05-23).     
+00001a70: 2020 200a 2020 2020 2020 2020 2d20 6164     .        - ad
+00001a80: 6420 676c 6f62 616c 2043 5353 2063 6c61  d global CSS cla
+00001a90: 7373 6573 2066 6f72 206d 6172 6769 6e73  sses for margins
+00001aa0: 2061 7574 6f0a 2020 2020 2020 2020 0a20   auto.        . 
+00001ab0: 2020 2020 2020 2056 6572 7369 6f6e 2031         Version 1
+00001ac0: 2e33 2e32 3320 2872 656c 6561 7365 6420  .3.23 (released 
+00001ad0: 3230 3232 2d30 352d 3139 290a 2020 2020  2022-05-19).    
+00001ae0: 2020 2020 0a20 2020 2020 2020 202d 2061      .        - a
+00001af0: 6464 2061 6363 6573 7369 6269 6c69 7479  dd accessibility
+00001b00: 2074 6f20 7569 2d61 6363 6f72 6469 6f6e   to ui-accordion
+00001b10: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
+00001b20: 2020 2056 6572 7369 6f6e 2031 2e33 2e32     Version 1.3.2
+00001b30: 3220 2872 656c 6561 7365 6420 3230 3232  2 (released 2022
+00001b40: 2d30 342d 3231 290a 2020 2020 2020 2020  -04-21).        
+00001b50: 0a20 2020 2020 2020 202d 2069 6d70 726f  .        - impro
+00001b60: 7665 2073 656d 616e 7469 6320 7374 796c  ve semantic styl
+00001b70: 696e 6720 6f66 204d 7920 6163 636f 756e  ing of My accoun
+00001b80: 7420 7061 6765 0a20 2020 2020 2020 200a  t page.        .
+00001b90: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00001ba0: 312e 332e 3231 2028 7265 6c65 6173 6564  1.3.21 (released
+00001bb0: 2032 3032 322d 3033 2d32 3929 0a20 2020   2022-03-29).   
+00001bc0: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001bd0: 6669 7820 6874 6d6c 2074 6167 7320 696e  fix html tags in
+00001be0: 2074 656d 706c 6174 6573 0a20 2020 2020   templates.     
+00001bf0: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00001c00: 696f 6e20 312e 332e 3230 2028 7265 6c65  ion 1.3.20 (rele
+00001c10: 6173 6564 2032 3032 322d 3033 2d31 3729  ased 2022-03-17)
+00001c20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001c30: 2020 2d20 7265 6661 6374 6f72 2070 6167    - refactor pag
+00001c40: 6520 7465 6d70 6c61 7465 0a20 2020 2020  e template.     
+00001c50: 2020 202d 2061 6464 2073 656d 616e 7469     - add semanti
+00001c60: 6320 7569 2069 6e76 656e 696f 2070 6163  c ui invenio pac
+00001c70: 6b61 6765 6420 7468 656d 6520 636f 6e66  kaged theme conf
+00001c80: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+00001c90: 2020 2d20 6578 7465 6e64 2075 7469 6c73    - extend utils
+00001ca0: 2043 5353 2063 6c61 7373 6573 0a20 2020   CSS classes.   
+00001cb0: 2020 2020 200a 2020 2020 2020 2020 5665       .        Ve
+00001cc0: 7273 696f 6e20 312e 332e 3139 2028 7265  rsion 1.3.19 (re
+00001cd0: 6c65 6173 6564 2032 3032 322d 3033 2d30  leased 2022-03-0
+00001ce0: 3429 0a20 2020 2020 2020 200a 2020 2020  4).        .    
+00001cf0: 2020 2020 2d20 4164 6420 6120 7265 7573      - Add a reus
+00001d00: 6162 6c65 204a 696e 6a61 206d 6163 726f  able Jinja macro
+00001d10: 2074 6f20 7472 756e 6361 7465 206c 6f6e   to truncate lon
+00001d20: 6720 7465 7874 2e0a 2020 2020 2020 2020  g text..        
+00001d30: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+00001d40: 2031 2e33 2e31 3820 2872 656c 6561 7365   1.3.18 (release
+00001d50: 6420 3230 3232 2d30 332d 3031 290a 2020  d 2022-03-01).  
+00001d60: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00001d70: 2052 6576 6572 7420 666f 6e74 2062 6163   Revert font bac
+00001d80: 6b20 746f 2064 6566 6175 6c74 2073 616e  k to default san
+00001d90: 732d 7361 7269 6620 666f 6e74 2069 6e73  s-sarif font ins
+00001da0: 7465 6164 206f 6620 4c61 746f 2e0a 2020  tead of Lato..  
+00001db0: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+00001dc0: 6572 7369 6f6e 2031 2e33 2e31 3720 2872  ersion 1.3.17 (r
+00001dd0: 656c 6561 7365 6420 3230 3232 2d30 322d  eleased 2022-02-
+00001de0: 3238 290a 2020 2020 2020 2020 0a20 2020  28).        .   
+00001df0: 2020 2020 202d 2041 6464 7320 6661 7669       - Adds favi
+00001e00: 636f 6e0a 2020 2020 2020 2020 2d20 4669  con.        - Fi
+00001e10: 7820 6973 7375 6520 7769 7468 2066 6c61  x issue with fla
+00001e20: 7368 206d 6573 7361 6765 206f 6e20 6c6f  sh message on lo
+00001e30: 6769 6e20 7061 6765 206e 6f74 2062 6569  gin page not bei
+00001e40: 6e67 2073 6964 6520 746f 2073 6964 652e  ng side to side.
+00001e50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001e60: 2020 5665 7273 696f 6e20 312e 332e 3136    Version 1.3.16
+00001e70: 2028 7265 6c65 6173 6564 2032 3032 322d   (released 2022-
+00001e80: 3032 2d31 3729 0a20 2020 2020 2020 200a  02-17).        .
+00001e90: 2020 2020 2020 2020 2d20 4164 6420 636f          - Add co
+00001ea0: 6d6d 6f6e 2060 7371 7561 7265 2d70 6c61  mmon `square-pla
+00001eb0: 6365 686f 6c64 6572 2e70 6e67 6020 696d  ceholder.png` im
+00001ec0: 6167 6520 666f 7220 6765 6e65 7261 6c20  age for general 
+00001ed0: 7573 652e 0a20 2020 2020 2020 200a 2020  use..        .  
+00001ee0: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00001ef0: 332e 3135 2028 7265 6c65 6173 6564 2032  3.15 (released 2
+00001f00: 3032 322d 3032 2d31 3729 0a20 2020 2020  022-02-17).     
+00001f10: 2020 200a 2020 2020 2020 2020 2d20 5265     .        - Re
+00001f20: 6d6f 7665 2063 7573 746f 6d20 6d61 7267  move custom marg
+00001f30: 696e 2066 726f 6d20 636c 6173 7365 7320  in from classes 
+00001f40: 746f 2069 6d70 726f 7665 2043 5353 206f  to improve CSS o
+00001f50: 7665 7272 6964 6162 696c 6974 792e 0a20  verridability.. 
+00001f60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001f70: 5665 7273 696f 6e20 312e 332e 3134 2028  Version 1.3.14 (
+00001f80: 7265 6c65 6173 6564 2032 3032 322d 3032  released 2022-02
+00001f90: 2d31 3629 0a20 2020 2020 2020 200a 2020  -16).        .  
+00001fa0: 2020 2020 2020 2d20 4669 7820 6973 7375        - Fix issu
+00001fb0: 6520 7769 7468 204c 6174 6f20 666f 6e74  e with Lato font
+00001fc0: 206e 6f74 2062 6569 6e67 206c 6f61 6465   not being loade
+00001fd0: 6420 696e 2053 656d 616e 7469 6320 5549  d in Semantic UI
+00001fe0: 2074 6865 6d65 2e0a 2020 2020 2020 2020   theme..        
+00001ff0: 2d20 5365 7473 2053 656d 616e 7469 6320  - Sets Semantic 
+00002000: 5549 2040 6d75 7465 6454 6578 7443 6f6c  UI @mutedTextCol
+00002010: 6f72 2e0a 2020 2020 2020 2020 0a20 2020  or..        .   
+00002020: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
+00002030: 2e31 3320 2872 656c 6561 7365 6420 3230  .13 (released 20
+00002040: 3232 2d30 322d 3136 290a 2020 2020 2020  22-02-16).      
+00002050: 2020 0a20 2020 2020 2020 202d 2045 6e73    .        - Ens
+00002060: 7572 6520 636f 6d70 696c 6564 2074 7261  ure compiled tra
+00002070: 6e73 6c61 7469 6f6e 206d 6573 7361 6765  nslation message
+00002080: 2063 6174 616c 6f67 7320 6172 6520 696e   catalogs are in
+00002090: 636c 7564 6564 2069 6e20 7468 650a 2020  cluded in the.  
+000020a0: 2020 2020 2020 2020 6469 7374 7269 6275          distribu
+000020b0: 7469 6f6e 7320 7570 6c6f 6164 6564 206f  tions uploaded o
+000020c0: 6e20 5079 5049 2e0a 2020 2020 2020 2020  n PyPI..        
+000020d0: 0a20 2020 2020 2020 2056 6572 7369 6f6e  .        Version
+000020e0: 2031 2e33 2e31 3220 2872 656c 6561 7365   1.3.12 (release
+000020f0: 6420 3230 3232 2d30 322d 3134 290a 2020  d 2022-02-14).  
+00002100: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00002110: 2046 6978 6573 2041 3131 7920 6973 7375   Fixes A11y issu
+00002120: 6520 7769 7468 2074 6865 2063 6c6f 7365  e with the close
+00002130: 2062 7574 746f 6e20 696e 2066 6c61 7368   button in flash
+00002140: 206d 6573 7361 6765 732e 0a20 2020 2020   messages..     
+00002150: 2020 200a 2020 2020 2020 2020 5665 7273     .        Vers
+00002160: 696f 6e20 312e 332e 3131 2028 7265 6c65  ion 1.3.11 (rele
+00002170: 6173 6564 2032 3032 322d 3032 2d30 3829  ased 2022-02-08)
+00002180: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002190: 2020 2d20 4164 6473 206d 6172 6769 6e20    - Adds margin 
+000021a0: 6765 6e65 7261 746f 722e 0a20 2020 2020  generator..     
+000021b0: 2020 202d 2041 6464 7320 4131 3179 2070     - Adds A11y p
+000021c0: 6167 6520 6c61 6e64 6d61 726b 732e 0a20  age landmarks.. 
+000021d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000021e0: 5665 7273 696f 6e20 312e 332e 3130 2028  Version 1.3.10 (
+000021f0: 7265 6c65 6173 6564 2032 3032 312d 3131  released 2021-11
+00002200: 2d32 3329 0a20 2020 2020 2020 200a 2020  -23).        .  
+00002210: 2020 2020 2020 2d20 5765 6220 6163 6365        - Web acce
+00002220: 7373 6962 696c 6974 7920 6669 782e 0a20  ssibility fix.. 
+00002230: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002240: 5665 7273 696f 6e20 312e 332e 3920 2872  Version 1.3.9 (r
+00002250: 656c 6561 7365 6420 3230 3231 2d30 372d  eleased 2021-07-
+00002260: 3132 290a 2020 2020 2020 2020 0a20 2020  12).        .   
+00002270: 2020 2020 202d 2041 6464 7320 6765 726d       - Adds germ
+00002280: 616e 2074 7261 6e73 6c61 7469 6f6e 730a  an translations.
+00002290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000022a0: 2056 6572 7369 6f6e 2031 2e33 2e38 2028   Version 1.3.8 (
+000022b0: 7265 6c65 6173 6564 2032 3032 312d 3032  released 2021-02
+000022c0: 2d31 3029 0a20 2020 2020 2020 200a 2020  -10).        .  
+000022d0: 2020 2020 2020 2d20 4164 6473 2062 7261        - Adds bra
+000022e0: 6e64 2063 6f6c 6f72 2074 6f20 6d65 6e75  nd color to menu
+000022f0: 2069 7465 6d73 0a20 2020 2020 2020 200a   items.        .
+00002300: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00002310: 312e 332e 3720 2872 656c 6561 7365 6420  1.3.7 (released 
+00002320: 3230 3231 2d30 312d 3235 290a 2020 2020  2021-01-25).    
+00002330: 2020 2020 0a20 2020 2020 2020 202d 2041      .        - A
+00002340: 6464 7320 6272 616e 6420 636f 6c6f 7220  dds brand color 
+00002350: 696e 2073 6567 6d65 6e74 730a 2020 2020  in segments.    
+00002360: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00002370: 7369 6f6e 2031 2e33 2e36 2028 7265 6c65  sion 1.3.6 (rele
+00002380: 6173 6564 2032 3032 312d 3031 2d30 3429  ased 2021-01-04)
+00002390: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000023a0: 2020 2d20 4164 6473 2060 6c69 6e6b 6020    - Adds `link` 
+000023b0: 7468 656d 6520 6963 6f6e 0a20 2020 2020  theme icon.     
+000023c0: 2020 202d 2046 6978 6573 2077 696c 6463     - Fixes wildc
+000023d0: 6172 6420 6963 6f6e 2072 6573 6f6c 7574  ard icon resolut
+000023e0: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
+000023f0: 2020 2020 2056 6572 7369 6f6e 2031 2e33       Version 1.3
+00002400: 2e35 2028 7265 6c65 6173 6564 2032 3032  .5 (released 202
+00002410: 302d 3132 2d31 3729 0a20 2020 2020 2020  0-12-17).       
+00002420: 200a 2020 2020 2020 2020 2d20 4669 7865   .        - Fixe
+00002430: 7320 6368 6563 6b62 6f78 2e6f 7665 7272  s checkbox.overr
+00002440: 6964 6573 2069 6e20 6069 6e76 656e 696f  ides in `invenio
+00002450: 6020 5355 4920 7061 636b 6167 6564 2074  ` SUI packaged t
+00002460: 6865 6d65 2e0a 2020 2020 2020 2020 0a20  heme..        . 
+00002470: 2020 2020 2020 2056 6572 7369 6f6e 2031         Version 1
+00002480: 2e33 2e34 2028 7265 6c65 6173 6564 2032  .3.4 (released 2
+00002490: 3032 302d 3132 2d31 3729 0a20 2020 2020  020-12-17).     
+000024a0: 2020 200a 2020 2020 2020 2020 2d20 4164     .        - Ad
+000024b0: 6473 2061 2066 756c 6c20 2269 6e76 656e  ds a full "inven
+000024c0: 696f 2220 5365 6d61 6e74 6963 2055 4920  io" Semantic UI 
+000024d0: 7061 636b 6167 6564 2074 6865 6d65 2073  packaged theme s
+000024e0: 6f20 7765 2063 616e 2065 6173 6965 7220  o we can easier 
+000024f0: 6375 7374 6f6d 697a 650a 2020 2020 2020  customize.      
+00002500: 2020 2020 6c61 796f 7574 2069 6e20 7468      layout in th
+00002510: 6520 6675 7475 7265 2e0a 2020 2020 2020  e future..      
+00002520: 2020 0a20 2020 2020 2020 202d 204d 6f76    .        - Mov
+00002530: 6573 2074 6865 6d65 2e63 6f6e 6669 6720  es theme.config 
+00002540: 746f 2074 6865 6d65 2e63 6f6e 6669 672e  to theme.config.
+00002550: 6578 616d 706c 6520 616e 6420 6164 6473  example and adds
+00002560: 2061 206e 6f74 6520 746f 206d 616b 6520   a note to make 
+00002570: 6974 0a20 2020 2020 2020 2020 2063 6c65  it.          cle
+00002580: 6172 2074 6865 2066 696c 6520 6973 206e  ar the file is n
+00002590: 6f74 2061 6374 7561 6c6c 7920 7573 6564  ot actually used
+000025a0: 2c20 6275 7420 6973 206a 7573 7420 616e  , but is just an
+000025b0: 2065 7861 6d70 6c65 2e0a 2020 2020 2020   example..      
+000025c0: 2020 0a20 2020 2020 2020 202d 2041 6464    .        - Add
+000025d0: 7320 6865 6c70 6572 2074 6f6f 6c20 666f  s helper tool fo
+000025e0: 7220 7375 7070 6f72 7469 6e67 2074 6865  r supporting the
+000025f0: 6d65 2064 6570 656e 6465 6e74 2069 636f  me dependent ico
+00002600: 6e73 2e0a 2020 2020 2020 2020 0a20 2020  ns..        .   
+00002610: 2020 2020 202d 2046 6978 6573 206d 616e       - Fixes man
+00002620: 7920 6d69 6e6f 7220 7374 796c 696e 6720  y minor styling 
+00002630: 6973 7375 6573 2073 7563 6820 6173 2061  issues such as a
+00002640: 6c69 676e 6d65 6e74 732c 2062 7574 746f  lignments, butto
+00002650: 6e20 6c6f 6361 7469 6f6e 732c 0a20 2020  n locations,.   
+00002660: 2020 2020 2020 2067 7269 6473 2e0a 2020         grids..  
+00002670: 2020 2020 2020 0a20 2020 2020 2020 2056        .        V
+00002680: 6572 7369 6f6e 2031 2e33 2e33 2028 7265  ersion 1.3.3 (re
+00002690: 6c65 6173 6564 2032 3032 302d 3132 2d31  leased 2020-12-1
+000026a0: 3129 0a20 2020 2020 2020 200a 2020 2020  1).        .    
+000026b0: 2020 2020 2d20 496e 6974 6961 6c69 7a65      - Initialize
+000026c0: 7320 7365 6d61 6e74 6963 5549 2061 6363  s semanticUI acc
+000026d0: 6f72 6469 6f6e 2063 6f6d 706f 6e65 6e74  ordion component
+000026e0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+000026f0: 2020 2020 5665 7273 696f 6e20 312e 332e      Version 1.3.
+00002700: 3220 2872 656c 6561 7365 6420 3230 3230  2 (released 2020
+00002710: 2d31 322d 3131 290a 2020 2020 2020 2020  -12-11).        
+00002720: 0a20 2020 2020 2020 202d 2055 7064 6174  .        - Updat
+00002730: 6573 2074 6865 2049 6e76 656e 696f 206c  es the Invenio l
+00002740: 6f67 6f20 616e 6420 7265 6d6f 7665 206f  ogo and remove o
+00002750: 7574 6461 7465 6420 7665 7273 696f 6e73  utdated versions
+00002760: 2e0a 2020 2020 2020 2020 2d20 4669 7865  ..        - Fixe
+00002770: 7320 7468 6520 6472 6f70 646f 776e 2074  s the dropdown t
+00002780: 6f20 776f 726b 206f 6e20 7468 6520 7573  o work on the us
+00002790: 6572 2070 726f 6669 6c65 2070 6167 652e  er profile page.
+000027a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000027b0: 2020 5665 7273 696f 6e20 312e 332e 3120    Version 1.3.1 
+000027c0: 2872 656c 6561 7365 6420 3230 3230 2d31  (released 2020-1
+000027d0: 322d 3039 290a 2020 2020 2020 2020 0a20  2-09).        . 
+000027e0: 2020 2020 2020 202d 204d 696e 6f72 2066         - Minor f
+000027f0: 6978 2066 6f72 2053 656d 616e 7469 6355  ix for SemanticU
+00002800: 4920 6472 6f70 646f 776e 730a 2020 2020  I dropdowns.    
+00002810: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
+00002820: 7369 6f6e 2031 2e33 2e30 2028 7265 6c65  sion 1.3.0 (rele
+00002830: 6173 6564 2032 3032 302d 3132 2d30 3929  ased 2020-12-09)
+00002840: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002850: 2020 2d20 4d61 6a6f 723a 204e 6577 2053    - Major: New S
+00002860: 656d 616e 7469 6355 4920 7468 656d 6520  emanticUI theme 
+00002870: 6861 7320 6265 656e 2069 6e74 6567 7261  has been integra
+00002880: 7465 642e 2054 6865 2042 6f6f 7473 7472  ted. The Bootstr
+00002890: 6170 2033 2074 6865 6d65 2073 7469 6c6c  ap 3 theme still
+000028a0: 0a20 2020 2020 2020 2020 2065 7869 7374  .          exist
+000028b0: 732e 2054 6869 7320 6368 616e 6765 2064  s. This change d
+000028c0: 6570 656e 6473 206f 6e20 7468 6520 6c61  epends on the la
+000028d0: 7465 7374 2072 656c 6561 7365 6420 496e  test released In
+000028e0: 7665 6e69 6f2d 4173 7365 7473 2077 6869  venio-Assets whi
+000028f0: 6368 0a20 2020 2020 2020 2020 2061 6464  ch.          add
+00002900: 7320 7375 7070 6f72 7473 2066 6f72 206d  s supports for m
+00002910: 756c 7469 706c 6520 5549 2066 7261 6d65  ultiple UI frame
+00002920: 776f 726b 732e 0a20 2020 2020 2020 200a  works..        .
+00002930: 2020 2020 2020 2020 2d20 4164 6473 2073          - Adds s
+00002940: 7570 706f 7274 2066 6f72 2064 796e 616d  upport for dynam
+00002950: 6963 206c 6f61 6469 6e67 206f 6620 7465  ic loading of te
+00002960: 6d70 6c61 7465 7320 666f 7220 5265 6163  mplates for Reac
+00002970: 742d 4f76 6572 7269 6461 626c 652e 0a20  t-Overridable.. 
+00002980: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002990: 2d20 4261 636b 7761 7264 7320 696e 636f  - Backwards inco
+000029a0: 6d70 6174 6962 6c65 3a20 5468 6520 6f6c  mpatible: The ol
+000029b0: 642d 7374 796c 6520 466c 6173 6b2d 4173  d-style Flask-As
+000029c0: 7365 7420 6275 6e64 6c65 7320 7761 7320  set bundles was 
+000029d0: 7265 6d6f 7665 6420 2874 6865 7365 0a20  removed (these. 
+000029e0: 2020 2020 2020 2020 2062 756e 646c 6573           bundles
+000029f0: 2077 6572 6520 6465 7072 6563 6174 6564   were deprecated
+00002a00: 2069 6e20 496e 7665 6e69 6f20 7633 2e31   in Invenio v3.1
+00002a10: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
+00002a20: 2020 2020 2d20 4164 6473 2054 7572 6b69      - Adds Turki
+00002a30: 7368 2074 7261 6e73 6c61 7469 6f6e 732e  sh translations.
+00002a40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002a50: 2020 5665 7273 696f 6e20 312e 322e 3020    Version 1.2.0 
+00002a60: 2872 656c 6561 7365 6420 3230 3230 2d30  (released 2020-0
+00002a70: 332d 3230 290a 2020 2020 2020 2020 0a20  3-20).        . 
+00002a80: 2020 2020 2020 202d 2052 6570 6c61 6365         - Replace
+00002a90: 7320 466c 6173 6b20 6465 7065 6e64 656e  s Flask dependen
+00002aa0: 6379 2077 6974 6820 6060 696e 7665 6e69  cy with ``inveni
+00002ab0: 6f2d 6261 7365 6060 2e0a 2020 2020 2020  o-base``..      
+00002ac0: 2020 0a20 2020 2020 2020 2056 6572 7369    .        Versi
+00002ad0: 6f6e 2031 2e31 2e34 2028 7265 6c65 6173  on 1.1.4 (releas
+00002ae0: 6564 2032 3031 392d 3037 2d32 3229 0a20  ed 2019-07-22). 
+00002af0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002b00: 2d20 496e 7472 6f64 7563 6520 6861 6e64  - Introduce hand
+00002b10: 6c69 6e67 206f 6620 7468 6520 6572 726f  ling of the erro
+00002b20: 7220 3432 392e 0a20 2020 2020 2020 200a  r 429..        .
+00002b30: 2020 2020 2020 2020 5665 7273 696f 6e20          Version 
+00002b40: 312e 312e 3320 2872 656c 6561 7365 6420  1.1.3 (released 
+00002b50: 3230 3139 2d30 332d 3133 290a 2020 2020  2019-03-13).    
+00002b60: 2020 2020 0a20 2020 2020 2020 202d 2052      .        - R
+00002b70: 6573 7472 7563 7475 7265 2053 4353 5320  estructure SCSS 
+00002b80: 6669 6c65 732c 2069 6e20 6f72 6465 7220  files, in order 
+00002b90: 746f 2061 6c6c 6f77 2065 6173 6965 7220  to allow easier 
+00002ba0: 6375 7374 6f6d 697a 6174 696f 6e20 616e  customization an
+00002bb0: 6420 6578 7465 6e73 696f 6e0a 2020 2020  d extension.    
+00002bc0: 2020 2020 2020 696e 206f 7665 726c 6179        in overlay
+00002bd0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00002be0: 2020 2020 5665 7273 696f 6e20 312e 312e      Version 1.1.
+00002bf0: 3220 2872 656c 6561 7365 6420 3230 3139  2 (released 2019
+00002c00: 2d30 322d 3135 290a 2020 2020 2020 2020  -02-15).        
+00002c10: 0a20 2020 2020 2020 202d 2055 7067 7261  .        - Upgra
+00002c20: 6465 6420 6d6f 6d65 6e74 2074 6f20 322e  ded moment to 2.
+00002c30: 3233 2e30 0a20 2020 2020 2020 200a 2020  23.0.        .  
+00002c40: 2020 2020 2020 5665 7273 696f 6e20 312e        Version 1.
+00002c50: 312e 3120 2872 656c 6561 7365 6420 3230  1.1 (released 20
+00002c60: 3138 2d31 322d 3035 290a 2020 2020 2020  18-12-05).      
+00002c70: 2020 0a20 2020 2020 2020 202d 2046 6978    .        - Fix
+00002c80: 6573 2069 7373 7565 7320 7769 7468 2077  es issues with w
+00002c90: 6562 7061 636b 2061 6e64 2074 6865 2041  ebpack and the A
+00002ca0: 646d 696e 4c54 4520 7468 656d 652e 0a20  dminLTE theme.. 
+00002cb0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002cc0: 5665 7273 696f 6e20 312e 312e 3020 2872  Version 1.1.0 (r
+00002cd0: 656c 6561 7365 6420 3230 3138 2d31 312d  eleased 2018-11-
+00002ce0: 3036 290a 2020 2020 2020 2020 0a20 2020  06).        .   
+00002cf0: 2020 2020 202d 2049 6e74 726f 6475 6365       - Introduce
+00002d00: 2077 6562 7061 636b 2073 7570 706f 7274   webpack support
+00002d10: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00002d20: 2020 2056 6572 7369 6f6e 2031 2e30 2e30     Version 1.0.0
+00002d30: 2028 7265 6c65 6173 6564 2032 3031 382d   (released 2018-
+00002d40: 3033 2d32 3329 0a20 2020 2020 2020 200a  03-23).        .
+00002d50: 2020 2020 2020 2020 2d20 496e 6974 6961          - Initia
+00002d60: 6c20 7075 626c 6963 2072 656c 6561 7365  l public release
+00002d70: 2e0a 2020 2020 2020 2020 0a4b 6579 776f  ..        .Keywo
+00002d80: 7264 733a 2069 6e76 656e 696f 0a50 6c61  rds: invenio.Pla
+00002d90: 7466 6f72 6d3a 2061 6e79 0a43 6c61 7373  tform: any.Class
+00002da0: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+00002db0: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+00002dc0: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00002dd0: 6c65 0a52 6571 7569 7265 732d 5079 7468  le.Requires-Pyth
+00002de0: 6f6e 3a20 3e3d 332e 370a 5072 6f76 6964  on: >=3.7.Provid
+00002df0: 6573 2d45 7874 7261 3a20 7465 7374 730a  es-Extra: tests.
+00002e00: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00002e10: 646f 6373 0a                             docs.
```

### Comparing `invenio-theme-3.0.0/invenio_theme.egg-info/SOURCES.txt` & `invenio-theme-3.1.0/invenio_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/requirements-devel.txt` & `invenio-theme-3.1.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/setup.cfg` & `invenio-theme-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/tests/conftest.py` & `invenio-theme-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/tests/helpers.py` & `invenio-theme-3.1.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/tests/test_invenio_theme.py` & `invenio-theme-3.1.0/tests/test_invenio_theme.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-3.0.0/tests/test_invenio_theme_error_handler.py` & `invenio-theme-3.1.0/tests/test_invenio_theme_error_handler.py`

 * *Files identical despite different names*

