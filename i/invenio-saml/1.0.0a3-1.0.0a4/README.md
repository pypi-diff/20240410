# Comparing `tmp/invenio-saml-1.0.0a3.tar.gz` & `tmp/invenio-saml-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-saml-1.0.0a3.tar", last modified: Fri Nov 18 09:06:03 2022, max compression
+gzip compressed data, was "invenio-saml-1.0.0a4.tar", last modified: Thu Dec 15 12:41:24 2022, max compression
```

## Comparing `invenio-saml-1.0.0a3.tar` & `invenio-saml-1.0.0a4.tar`

### file list

```diff
@@ -1,167 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/.tx/
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/.tx/config
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10112 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     5672 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/invenio_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4082 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/invenio_accounts/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/invenio_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/templates/invenio-saml/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/templates/invenio-saml/login_user.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/templates/semantic-ui/invenio_saml/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/templates/semantic-ui/invenio_saml/login_user.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.472140 invenio-saml-1.0.0a3/invenio_saml/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.476140 invenio-saml-1.0.0a3/invenio_saml/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/invenio_saml/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/invenio_saml/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.480140 invenio-saml-1.0.0a3/invenio_saml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-18 09:06:03.000000 invenio-saml-1.0.0a3/invenio_saml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      718 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:06:03.484140 invenio-saml-1.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4781 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/tests/test_invenio_saml.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-11-18 09:05:58.000000 invenio-saml-1.0.0a3/tests/tests_external.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.362061 invenio-saml-1.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.342061 invenio-saml-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.350061 invenio-saml-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2368 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.350061 invenio-saml-1.0.0a4/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3457 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2022-12-15 12:41:24.362061 invenio-saml-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.350061 invenio-saml-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7433 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10112 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6993 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8077 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9007 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5664 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/invenio_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/invenio_accounts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/invenio_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.342061 invenio-saml-1.0.0a4/invenio_saml/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/templates/invenio-saml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/templates/invenio-saml/login_user.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.342061 invenio-saml-1.0.0a4/invenio_saml/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/templates/semantic-ui/invenio_saml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/templates/semantic-ui/invenio_saml/login_user.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.342061 invenio-saml-1.0.0a4/invenio_saml/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.342061 invenio-saml-1.0.0a4/invenio_saml/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.342061 invenio-saml-1.0.0a4/invenio_saml/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1319 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1397 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1203 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.346061 invenio-saml-1.0.0a4/invenio_saml/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/invenio_saml/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2831 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5521 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/invenio_saml/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.354061 invenio-saml-1.0.0a4/invenio_saml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2022-12-15 12:41:24.000000 invenio-saml-1.0.0a4/invenio_saml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      326 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      675 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2022-12-15 12:41:24.362061 invenio-saml-1.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3909 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:41:24.358061 invenio-saml-1.0.0a4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/data/cert.crt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/data/cert.key
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/data/idp.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/data/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/data/slo_response.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     5409 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/data/sso_response.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4780 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/test_invenio_saml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4738 2022-12-15 12:41:19.000000 invenio-saml-1.0.0a4/tests/test_views.py
```

### Comparing `invenio-saml-1.0.0a3/.editorconfig` & `invenio-saml-1.0.0a4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/.github/workflows/i18n-pull.yml` & `invenio-saml-1.0.0a4/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/.github/workflows/i18n-push.yml` & `invenio-saml-1.0.0a4/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/.github/workflows/pypi-publish.yml` & `invenio-saml-1.0.0a4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/.github/workflows/tests.yml` & `invenio-saml-1.0.0a4/.github/workflows/tests.yml`

 * *Files 3% similar despite different names*

```diff
@@ -71,10 +71,13 @@
         run: |
           pip install -r .${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt
           pip install ".[$EXTRAS]"
           pip freeze
           docker --version
           docker-compose --version
 
+      - name: Run translations test
+        run: ./run-i18n-tests.sh
+
       - name: Run tests
         run: |
           ./run-tests.sh
```

### Comparing `invenio-saml-1.0.0a3/.tx/config` & `invenio-saml-1.0.0a4/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/CHANGES.rst` & `invenio-saml-1.0.0a4/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
     Invenio-SAML is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.0.0a4 (released 2022-12-15)
+
+- Migrate Flask-SSO-SAML code #31
+- Check before linking user #35
+- Add translations tests #36
+
 Version 1.0.0a2 (released 2022-09-12)
 
 - Add auto_confirm, confirm user email address
 
 Version 1.0.0a1 (released 2021-07-15)
 
 - Marking strings for translation
```

### Comparing `invenio-saml-1.0.0a3/CONTRIBUTING.rst` & `invenio-saml-1.0.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/LICENSE` & `invenio-saml-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/MANIFEST.in` & `invenio-saml-1.0.0a4/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2019 Esteban J. Garcia Gabancho.
+# Copyright (C) 2019, 2022 Esteban J. Garcia Gabancho.
 #
 # Invenio-SAML is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 include *.rst
 include *.sh
 include *.txt
@@ -19,11 +19,14 @@
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 recursive-include invenio_saml *.html
 recursive-include invenio_saml/translations *.po *.pot *.mo
 recursive-include tests *.py
+recursive-include tests *.crt
+recursive-include tests *.key
+recursive-include tests *.xml
 recursive-include .github/workflows *.yml
 
 
 include .git-blame-ignore-revs
```

### Comparing `invenio-saml-1.0.0a3/PKG-INFO` & `invenio-saml-1.0.0a4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-saml
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: "Invenio module that provides SAML integration."
 Home-page: https://github.com/inveniosoftware/invenio-saml
 Author: Esteban J. Garcia Gabancho
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019 Esteban J. Garcia Gabancho.
@@ -44,14 +44,20 @@
         
             Invenio-SAML is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.0.0a4 (released 2022-12-15)
+        
+        - Migrate Flask-SSO-SAML code #31
+        - Check before linking user #35
+        - Add translations tests #36
+        
         Version 1.0.0a2 (released 2022-09-12)
         
         - Add auto_confirm, confirm user email address
         
         Version 1.0.0a1 (released 2021-07-15)
         
         - Marking strings for translation
```

### Comparing `invenio-saml-1.0.0a3/README.rst` & `invenio-saml-1.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/docs/Makefile` & `invenio-saml-1.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/docs/conf.py` & `invenio-saml-1.0.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/docs/index.rst` & `invenio-saml-1.0.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/docs/make.bat` & `invenio-saml-1.0.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/__init__.py` & `invenio-saml-1.0.0a4/invenio_saml/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2019 Esteban J. Garcia Gabancho.
+# Copyright (C) 2019, 2022 Esteban J. Garcia Gabancho.
 #
 # Invenio-SAML is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module that provides SAML integration.
 
-This module is a thin layer on between Invenio and `Flask-SSO-SAML
-<https://flask-sso-saml.readthedocs.io/>`_, which provides you with a set of
-default handlers than can be used out of the box to authenticated users using
-SSO SAML.
+This module provides you with a set of default handlers than can be used out of
+the box to authenticated users using SSO SAML.
 
 Handlers
 --------
 
-Flass-SSO-SAML allows you to specify handlers for each SSO action, ``sso``,
+Invenio-SAML allows you to specify handlers for each SSO action, ``sso``,
 ``acs``, ``slo``, ``sls`` and ``metadata``.
 Typically the ones that matter the most are ``acs`` and ``sls``, because they
 are the ones that will authenticate and "unauthenticate" users from the
 application.
 
-Invenio-SAML provides default handlers for ``acs`` and``sls`` actions that will
+This module provides default handlers for ``acs`` and``sls`` actions that will
 be valid for most of the use cases.
-This is how you can use them (there is a more complete example on
-``examples/app.py``):
+This is how you can use them:
 
 .. code-block:: python
 
     from invenio_saml.handlers import acs_handler_factor, default_sls_handler
 
     def account_info(info):
         return dict(
@@ -67,12 +64,12 @@
 function is responsible of extracting the user information from the SSO reponse
 and transforming it so the rest of the handler understand it. You can check
 more information about it on the API documentation.
 """
 
 from __future__ import absolute_import, print_function
 
-from .ext import InvenioSAML
+from .ext import InvenioSSOSAML
 
-__version__ = "1.0.0a3"
+__version__ = "1.0.0a4"
 
-__all__ = ("__version__", "InvenioSAML")
+__all__ = ("__version__", "InvenioSSOSAML")
```

### Comparing `invenio-saml-1.0.0a3/invenio_saml/handlers.py` & `invenio-saml-1.0.0a4/invenio_saml/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2019, 2020 Esteban J. Garcia Gabancho.
+# Copyright (C) 2019, 2020, 2022 Esteban J. Garcia Gabancho.
 # Copyright (C) 2021-2022 Graz University of Technology.
 #
 # Invenio-SAML is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 """Default handlers for SSO-SAML."""
 
 from datetime import datetime
@@ -62,15 +62,15 @@
         user=dict(
             email=email,
             profile=dict(username=username, full_name=name + " " + surname),
         ),
         external_id=external_id,
         external_method=remote_app,
         active=True,
-        confirmed_at=datetime.utcnow().isoformat()
+        confirmed_at=datetime.utcnow()
         if remote_app_config.get("auto_confirm", False)
         else None,
     )
 
 
 def default_account_setup(user, account_info):
     """Default account setup which only links ``User`` and ``UserIdentity``."""
@@ -132,15 +132,15 @@
 
     :return: function to be used as ACS handler
     """
 
     def default_acs_handler(auth, next_url):
         """Default ACS handler.
 
-        :para auth: A :class:`flask_sso_saml.utils.SAMLAuth` instance.
+        :para auth: A :class:`invenio_saml.utils.SAMLAuth` instance.
         :param next_url: String with the next URL to redirect to.
 
         :return: Next URL
         """
         if not current_user.is_authenticated:
             current_app.logger.debug(
                 "Metadata received from IdP %s", auth.get_attributes()
```

### Comparing `invenio-saml-1.0.0a3/invenio_saml/invenio_accounts/utils.py` & `invenio-saml-1.0.0a4/invenio_saml/invenio_accounts/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2019 Esteban J. Garcia Gabancho.
 # Copyright (C) 2019-2021 CERN.
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2022 Graz University of Technology.
 #
 # Invenio-SAML is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Temporary file for, IMHO, Invenio-Accounts code."""
 
 from __future__ import absolute_import, print_function
 
 from flask import after_this_request, current_app
-from flask_security import login_user, logout_user
+from flask_security import login_user
 from flask_security.confirmable import requires_confirmation
 from flask_security.registerable import register_user
 
 # FIXME: modify import when integrated inside invenio_accounts
 # from .models import User
 from invenio_accounts.models import User
-from invenio_db import db
-from invenio_oauthclient.errors import AlreadyLinkedError
 from invenio_oauthclient.models import UserIdentity
-from sqlalchemy.exc import IntegrityError
 from werkzeug.local import LocalProxy
 
 _security = LocalProxy(lambda: current_app.extensions["security"])
 
 _datastore = LocalProxy(lambda: _security.datastore)
 
 
@@ -53,19 +50,18 @@
     :param account_info: The dictionary with the account info.
         (Default: ``None``)
     :returns: A :class:`invenio_accounts.models.User` instance or ``None``.
     """
     if account_info:
         external_id = _get_external_id(account_info)
         if external_id:
-            user_identity = UserIdentity.query.filter_by(
-                id=external_id["id"], method=external_id["method"]
-            ).first()
-            if user_identity:
-                return user_identity.user
+            user = UserIdentity.get_user(external_id["method"], external_id["id"])
+            if user:
+                return user
+
         email = account_info.get("user", {}).get("email")
         if email:
             return User.query.filter_by(email=email).one_or_none()
     return None
 
 
 def account_authenticate(user):
@@ -85,23 +81,20 @@
 
     :param user: A :class:`invenio_accounts.models.User` instance.
     :param external_id: The external id associated with the user.
         (Default: ``None``)
     :raises invenio_oauthclient.errors.AlreadyLinkedError: Raised if already
         exists a link.
     """
-    try:
-        with db.session.begin_nested():
-            db.session.add(
-                UserIdentity(
-                    id=external_id["id"], method=external_id["method"], id_user=user.id
-                )
-            )
-    except IntegrityError:
-        raise AlreadyLinkedError(user, external_id)
+    if UserIdentity.get_user(external_id["method"], external_id["id"]):
+        # already linked. should be fine to just return
+        # method and id form the composite primary key, so no other with these values can be linked
+        return
+
+    UserIdentity.create(user, external_id["method"], external_id["id"])
 
 
 def create_registrationform(*args, **kwargs):
     """Make a registration form."""
 
     class RegistrationForm(_security.confirm_register_form):
         password = None
```

### Comparing `invenio-saml-1.0.0a3/invenio_saml/invenio_app.py` & `invenio-saml-1.0.0a4/invenio_saml/invenio_app.py`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/templates/invenio-saml/login_user.html` & `invenio-saml-1.0.0a4/invenio_saml/templates/invenio-saml/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/templates/semantic-ui/invenio_saml/login_user.html` & `invenio-saml-1.0.0a4/invenio_saml/templates/semantic-ui/invenio_saml/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/af/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/ar/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/bg/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/ca/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/cs/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/da/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/de/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/el/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/es/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/et/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/fa/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/fr/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/gl/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/hr/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/hu/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/it/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/ja/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/ka/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/lt/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/messages.pot` & `invenio-saml-1.0.0a4/invenio_saml/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/no/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/pl/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/pt/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/ro/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/ru/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/rw/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/sk/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/sv/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/tr/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/uk/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-saml-1.0.0a4/invenio_saml/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-saml-1.0.0a3/invenio_saml.egg-info/PKG-INFO` & `invenio-saml-1.0.0a4/invenio_saml.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-saml
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: "Invenio module that provides SAML integration."
 Home-page: https://github.com/inveniosoftware/invenio-saml
 Author: Esteban J. Garcia Gabancho
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019 Esteban J. Garcia Gabancho.
@@ -44,14 +44,20 @@
         
             Invenio-SAML is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.0.0a4 (released 2022-12-15)
+        
+        - Migrate Flask-SSO-SAML code #31
+        - Check before linking user #35
+        - Add translations tests #36
+        
         Version 1.0.0a2 (released 2022-09-12)
         
         - Add auto_confirm, confirm user email address
         
         Version 1.0.0a1 (released 2021-07-15)
         
         - Marking strings for translation
```

### Comparing `invenio-saml-1.0.0a3/run-tests.sh` & `invenio-saml-1.0.0a4/run-tests.sh`

 * *Files 21% similar despite different names*

```diff
@@ -17,13 +17,12 @@
 function cleanup() {
     eval "$(docker-services-cli down --env)"
 }
 trap cleanup EXIT
 
 
 python -m check_manifest
-python -m setup extract_messages --dry-run
 python -m sphinx.cmd.build -qnNW docs docs/_build/html
 eval "$(docker-services-cli up --db ${DB:-postgresql} --cache ${CACHE:-redis} --env)"
 python -m pytest
 tests_exit_code=$?
 exit "$tests_exit_code"
```

### Comparing `invenio-saml-1.0.0a3/setup.cfg` & `invenio-saml-1.0.0a4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -14,38 +14,37 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
-	flask-sso-saml>=0.1.0
 	invenio-accounts>=1.4.5
 	uritools>=2.2.0
+	python3-saml>=1.5.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0,<0.3.10
 	invenio-app>=1.3.0
 	invenio-mail>=1.0.0
 	invenio-userprofiles>=1.0.0
 	mock>=2.0.0
 	redis>=2.10.5
-	pytest-invenio>=1.4.0
+	pytest-invenio>=2.1.0,<3.0.0
+	pytest-freezegun>=0.2.0
 	invenio-oauthclient>=1.5.1
 	Sphinx>=4.5.0
 	invenio-db[mysql,postgresql,versioning]>=1.0.9,<2.0.0
 
 [options.entry_points]
 invenio_base.apps = 
-	invenio_saml = invenio_saml:InvenioSAML
+	invenio_saml = invenio_saml:InvenioSSOSAML
 invenio_base.api_apps = 
-	invenio_saml = invenio_saml:InvenioSAML
-invenio_base.blueprints = 
-	invenio_saml = invenio_saml.views:blueprint
+	invenio_saml = invenio_saml:InvenioSSOSAML
 invenio_i18n.translations = 
 	invenio_saml = invenio_saml
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
```

### Comparing `invenio-saml-1.0.0a3/tests/test_handlers.py` & `invenio-saml-1.0.0a4/tests/test_handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 # Invenio-SAML is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 """Test handlers."""
 
 import pytest
 from flask_security import current_user, login_user
 from invenio_accounts.models import User
-from invenio_db import db
 from invenio_oauthclient.models import UserIdentity
 from mock import patch
 from werkzeug.exceptions import Unauthorized
 
 from invenio_saml.handlers import (
     acs_handler_factory,
     default_account_setup,
     default_sls_handler,
 )
 
 
 def test_default_account_setup(users):
     """Test default user account setup."""
     user = User.query.filter_by(email="federico@example.com").one()
-    account_info = dict(external_id=123456, external_method="external", other="foo")
+    account_info = dict(
+        external_id="123456",
+        external_method="external",
+        other="foo",
+    )
 
     default_account_setup(user, account_info)
 
     identities = UserIdentity.query.filter_by(id_user=user.id).all()
     assert len(identities) == 1
     assert identities[0].user == user
 
@@ -60,15 +63,15 @@
         surname=["Fernandez"],
         external_id=["12345679abcdf"],
     )
 
     acs_handler = acs_handler_factory("test")
 
     with appctx.test_request_context(), patch(
-        "flask_sso_saml.utils.SAMLAuth"
+        "invenio_saml.utils.SAMLAuth"
     ) as mock_saml_auth:
         mock_saml_auth.get_attributes.return_value = attrs
         next_url = acs_handler(mock_saml_auth, "/foo")
 
         assert next_url == "/foo"
         assert current_user.is_authenticated
         assert current_user.confirmed_at == None
@@ -94,15 +97,15 @@
         surname=["Fernandez"],
         external_id=["12345679abcdf"],
     )
 
     acs_handler = acs_handler_factory("test")
 
     with appctx.test_request_context(), patch(
-        "flask_sso_saml.utils.SAMLAuth"
+        "invenio_saml.utils.SAMLAuth"
     ) as mock_saml_auth:
         mock_saml_auth.get_attributes.return_value = attrs
         next_url = acs_handler(mock_saml_auth, "/foo")
 
         assert current_user.is_authenticated
         assert current_user.confirmed_at
 
@@ -115,15 +118,15 @@
         surname=["Fernandez"],
         external_id=["12345679abcdf"],
     )
 
     acs_handler = acs_handler_factory("test")
 
     with appctx.test_request_context(), patch(
-        "flask_sso_saml.utils.SAMLAuth"
+        "invenio_saml.utils.SAMLAuth"
     ) as mock_saml_auth, patch(
         "invenio_saml.handlers.account_authenticate"
     ) as mock_authenticate:
         mock_saml_auth.get_attributes.return_value = attrs
         mock_authenticate.return_value = False
         with pytest.raises(Unauthorized):
             next_url = acs_handler(mock_saml_auth, "/foo")
@@ -137,15 +140,15 @@
         surname=["Fernandez"],
         external_id=["12345679abcdf"],
     )
 
     acs_handler = acs_handler_factory("test")
 
     with appctx.test_request_context(), patch(
-        "flask_sso_saml.utils.SAMLAuth"
+        "invenio_saml.utils.SAMLAuth"
     ) as mock_saml_auth, patch(
         "invenio_saml.handlers.account_register"
     ) as mock_register:
         mock_saml_auth.get_attributes.return_value = attrs
         mock_register.return_value = None
         with pytest.raises(Unauthorized):
             next_url = acs_handler(mock_saml_auth, "/foo")
```

### Comparing `invenio-saml-1.0.0a3/tests/tests_external.py` & `invenio-saml-1.0.0a4/tests/test_external.py`

 * *Files identical despite different names*

