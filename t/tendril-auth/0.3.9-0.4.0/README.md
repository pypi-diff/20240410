# Comparing `tmp/tendril-auth-0.3.9.tar.gz` & `tmp/tendril-auth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-auth-0.3.9.tar", last modified: Tue Sep 12 04:43:10 2023, max compression
+gzip compressed data, was "tendril-auth-0.4.0.tar", last modified: Wed Apr 10 18:32:21 2024, max compression
```

## Comparing `tendril-auth-0.3.9.tar` & `tendril-auth-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,73 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.209657 tendril-auth-0.3.9/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-09-12 04:43:10.209657 tendril-auth-0.3.9/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.197657 tendril-auth-0.3.9/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.3.9/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-09-12 04:43:10.209657 tendril-auth-0.3.9/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.3.9/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.193657 tendril-auth-0.3.9/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.9/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.9/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-02-18 10:30:44.000000 tendril-auth-0.3.9/src/tendril/apiserver/routers/authn.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.201657 tendril-auth-0.3.9/src/tendril/authn/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-16 14:15:27.000000 tendril-auth-0.3.9/src/tendril/authn/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6160 2023-09-12 04:42:42.000000 tendril-auth-0.3.9/src/tendril/authn/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1836 2023-04-21 09:10:22.000000 tendril-auth-0.3.9/src/tendril/authn/client.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.205657 tendril-auth-0.3.9/src/tendril/authn/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.9/src/tendril/authn/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.3.9/src/tendril/authn/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.3.9/src/tendril/authn/db/mixins.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.3.9/src/tendril/authn/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1393 2023-04-21 12:28:51.000000 tendril-auth-0.3.9/src/tendril/authn/pydantic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2800 2023-04-19 15:44:25.000000 tendril-auth-0.3.9/src/tendril/authn/users.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.205657 tendril-auth-0.3.9/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.3.9/src/tendril/authz/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1926 2023-09-12 04:42:42.000000 tendril-auth-0.3.9/src/tendril/authz/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.3.9/src/tendril/authz/connector.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.205657 tendril-auth-0.3.9/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.3.9/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.3.9/src/tendril/authz/scopes/common.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.3.9/src/tendril/authz/scopes/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.209657 tendril-auth-0.3.9/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.3.9/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.3.9/src/tendril/config/auth.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.209657 tendril-auth-0.3.9/src/tendril_auth.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-09-12 04:43:10.000000 tendril-auth-0.3.9/src/tendril_auth.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1270 2023-09-12 04:43:10.000000 tendril-auth-0.3.9/src/tendril_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-09-12 04:43:10.000000 tendril-auth-0.3.9/src/tendril_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-09-12 04:43:10.000000 tendril-auth-0.3.9/src/tendril_auth.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-09-12 04:43:10.000000 tendril-auth-0.3.9/src/tendril_auth.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 04:43:10.209657 tendril-auth-0.3.9/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.3.9/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.482400 tendril-auth-0.4.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.4.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.4.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.478401 tendril-auth-0.4.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1198 2024-04-08 19:39:52.000000 tendril-auth-0.4.0/src/tendril/apiserver/routers/authn.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authn/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-16 14:15:27.000000 tendril-auth-0.4.0/src/tendril/authn/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6159 2024-04-09 12:57:03.000000 tendril-auth-0.4.0/src/tendril/authn/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1836 2023-04-21 09:10:22.000000 tendril-auth-0.4.0/src/tendril/authn/client.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authn/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/authn/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.4.0/src/tendril/authn/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.4.0/src/tendril/authn/db/mixins.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/authn/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1393 2023-04-21 12:28:51.000000 tendril-auth-0.4.0/src/tendril/authn/pydantic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2945 2024-04-09 12:57:04.000000 tendril-auth-0.4.0/src/tendril/authn/users.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.4.0/src/tendril/authz/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1926 2023-09-12 04:42:42.000000 tendril-auth-0.4.0/src/tendril/authz/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.4.0/src/tendril/authz/connector.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authz/domains/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril-auth-0.4.0/src/tendril/authz/domains/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      435 2024-04-09 13:07:58.000000 tendril-auth-0.4.0/src/tendril/authz/domains/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1030 2024-04-10 18:31:18.000000 tendril-auth-0.4.0/src/tendril/authz/domains/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1094 2024-04-08 20:14:41.000000 tendril-auth-0.4.0/src/tendril/authz/domains/scopes.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.4.0/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.4.0/src/tendril/authz/scopes/common.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.4.0/src/tendril/authz/scopes/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.4.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.4.0/src/tendril/config/auth.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/src/tendril_auth.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1415 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/tox.ini
```

### Comparing `tendril-auth-0.3.9/.gitignore` & `tendril-auth-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/.readthedocs.yml` & `tendril-auth-0.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/.travis.yml` & `tendril-auth-0.4.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/LICENSE` & `tendril-auth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/PKG-INFO` & `tendril-auth-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.3.9
+Version: 0.4.0
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
```

### Comparing `tendril-auth-0.3.9/README.rst` & `tendril-auth-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/Makefile` & `tendril-auth-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/_static/custom.css` & `tendril-auth-0.4.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/_static/favicon.ico` & `tendril-auth-0.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/_static/logo.png` & `tendril-auth-0.4.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/_static/logo_packed.png` & `tendril-auth-0.4.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/_templates/about.html` & `tendril-auth-0.4.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/conf.py` & `tendril-auth-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/index.rst` & `tendril-auth-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/docs/installation.rst` & `tendril-auth-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/setup.py` & `tendril-auth-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/apiserver/routers/authn.py` & `tendril-auth-0.4.0/src/tendril/apiserver/routers/authn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 
 from fastapi import APIRouter
 from fastapi import Depends
+from fastapi import BackgroundTasks
 
 from tendril.authn.users import authn_dependency
 from tendril.authn.users import AuthUserModel
 from tendril.authn.users import auth_spec
 from tendril.authn.users import verify_user_registration
 from tendril.authn.users import get_user_profile
 from tendril.authn.users import get_user_stub
@@ -14,16 +15,17 @@
 user_services = APIRouter(prefix='/user',
                           tags=["User Authentication Services"],
                           dependencies=[Depends(authn_dependency),
                                         auth_spec()])
 
 
 @user_services.get("/verify")
-async def verify(user: AuthUserModel = auth_spec()):
-    verify_user_registration(user)
+async def verify(background_tasks: BackgroundTasks,
+                 user: AuthUserModel = auth_spec()):
+    verify_user_registration(user, background_tasks=background_tasks)
     return {"message": "Logged in User Verified."}
 
 
 @user_services.get("/profile/me")
 async def my_profile(user: AuthUserModel = auth_spec()):
     return get_user_profile(user)
```

### Comparing `tendril-auth-0.3.9/src/tendril/authn/auth0.py` & `tendril-auth-0.4.0/src/tendril/authn/auth0.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
     return {
         'name': profile['name'],
         'nickname': profile['nickname'],
         'picture': profile['picture'],
         'user_id': profile['user_id'],
     }
 
-
 @management_api
 def get_connections(auth0: Auth0PythonClient = None):
     return auth0
 
 
 def get_mechanized_user_email(username, prefix):
     return f'{username}@{prefix}.{AUTH0_MECHANIZED_USER_DOMAIN}'
```

### Comparing `tendril-auth-0.3.9/src/tendril/authn/client.py` & `tendril-auth-0.4.0/src/tendril/authn/client.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/authn/db/controller.py` & `tendril-auth-0.4.0/src/tendril/authn/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/authn/db/model.py` & `tendril-auth-0.4.0/src/tendril/authn/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/authn/pydantic.py` & `tendril-auth-0.4.0/src/tendril/authn/pydantic.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/authn/users.py` & `tendril-auth-0.4.0/src/tendril/authn/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 
 import string
 import secrets
 
 from tendril.config import AUTH_PROVIDER
-from tendril.utils.pydantic import TendrilTBaseModel
-from tendril.authn.pydantic import UserStubTModel
+from tendril.authz import domains
 
 from .db.model import User
 from .db.controller import register_provider
 from .db.controller import register_user
 from .db.controller import get_user_by_id
 
 
@@ -55,21 +54,29 @@
 
 
 def get_user_stub(user):
     user = preprocess_user(user)
     return AuthProvider.get_user_stub(user)
 
 
-def verify_user_registration(user):
+def get_user_email(user):
+    profile = get_user_profile(user)
+    try:
+        return profile['auth0']['email']
+    except KeyError:
+        raise AttributeError(f"Could not find an email for user {user}")
+
+
+def verify_user_registration(user, background_tasks=None):
     user_id = preprocess_user(user)
     user, first_login = register_user(user_id, provider_name)
-    if first_login:
-        from tendril.authz.connector import add_user_scopes
-        from tendril.authz.scopes import default_user_scopes
-        add_user_scopes(user.puid, default_user_scopes)
+    if background_tasks:
+        background_tasks.add_task(domains.upsert,
+                                  user=user,
+                                  first_login=first_login)
 
 
 def _generate_password(length=32):
     alphabet = string.ascii_letters + string.digits
     password = ''.join(secrets.choice(alphabet) for i in range(length))
     return password
```

### Comparing `tendril-auth-0.3.9/src/tendril/authz/auth0.py` & `tendril-auth-0.4.0/src/tendril/authz/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/authz/connector.py` & `tendril-auth-0.4.0/src/tendril/authz/connector.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/authz/scopes/manager.py` & `tendril-auth-0.4.0/src/tendril/authz/scopes/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/config/__init__.py` & `tendril-auth-0.4.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril/config/auth.py` & `tendril-auth-0.4.0/src/tendril/config/auth.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/src/tendril_auth.egg-info/PKG-INFO` & `tendril-auth-0.4.0/src/tendril_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.3.9
+Version: 0.4.0
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
```

### Comparing `tendril-auth-0.3.9/src/tendril_auth.egg-info/SOURCES.txt` & `tendril-auth-0.4.0/src/tendril_auth.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 src/tendril/authn/db/__init__.py
 src/tendril/authn/db/controller.py
 src/tendril/authn/db/mixins.py
 src/tendril/authn/db/model.py
 src/tendril/authz/__init__.py
 src/tendril/authz/auth0.py
 src/tendril/authz/connector.py
+src/tendril/authz/domains/__init__.py
+src/tendril/authz/domains/base.py
+src/tendril/authz/domains/manager.py
+src/tendril/authz/domains/scopes.py
 src/tendril/authz/scopes/__init__.py
 src/tendril/authz/scopes/common.py
 src/tendril/authz/scopes/manager.py
 src/tendril/config/__init__.py
 src/tendril/config/auth.py
 src/tendril_auth.egg-info/PKG-INFO
 src/tendril_auth.egg-info/SOURCES.txt
```

### Comparing `tendril-auth-0.3.9/src/tendril_auth.egg-info/requires.txt` & `tendril-auth-0.4.0/src/tendril_auth.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/tests/coveralls.py` & `tendril-auth-0.4.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.9/tox.ini` & `tendril-auth-0.4.0/tox.ini`

 * *Files identical despite different names*

