# Comparing `tmp/byma-0.1.2.tar.gz` & `tmp/byma-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.2.tar", last modified: Sat Apr  6 16:28:33 2024, max compression
+gzip compressed data, was "byma-0.1.3.tar", last modified: Wed Apr 10 17:49:01 2024, max compression
```

## Comparing `byma-0.1.2.tar` & `byma-0.1.3.tar`

### file list

```diff
@@ -1,96 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.872532 byma-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-06 16:28:21.000000 byma-0.1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-06 16:28:21.000000 byma-0.1.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-06 16:28:21.000000 byma-0.1.2/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-06 16:28:21.000000 byma-0.1.2/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-06 16:28:21.000000 byma-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-06 16:28:33.872532 byma-0.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-06 16:28:21.000000 byma-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.861532 byma-0.1.2/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-06 16:28:21.000000 byma-0.1.2/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-06 16:28:33.000000 byma-0.1.2/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.862532 byma-0.1.2/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-06 16:28:21.000000 byma-0.1.2/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-06 16:28:21.000000 byma-0.1.2/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-06 16:28:21.000000 byma-0.1.2/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.862532 byma-0.1.2/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.863532 byma-0.1.2/byma/iteral/nonstationary/
--rw-rw-rw-   0 root         (0) root         (0)     5168 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/nonstationary/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/nonstationary/NonStationary.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/nonstationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.864532 byma-0.1.2/byma/iteral/stationary/
--rw-rw-rw-   0 root         (0) root         (0)     4730 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/stationary/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/stationary/Stationary.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/stationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.864532 byma-0.1.2/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7972 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.865532 byma-0.1.2/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-06 16:28:21.000000 byma-0.1.2/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-06 16:28:21.000000 byma-0.1.2/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1973 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.865532 byma-0.1.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-06 16:28:21.000000 byma-0.1.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-06 16:28:21.000000 byma-0.1.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-06 16:28:21.000000 byma-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.866532 byma-0.1.2/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.866532 byma-0.1.2/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.866532 byma-0.1.2/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3372 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/Stationary/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     4393 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4626 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4898 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.870532 byma-0.1.2/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     2752 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.870532 byma-0.1.2/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     2697 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/whatisbyma.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/examples/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-06 16:28:21.000000 byma-0.1.2/examples/example.py
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-06 16:28:21.000000 byma-0.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-06 16:28:21.000000 byma-0.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 16:28:33.872532 byma-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-06 16:28:21.000000 byma-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-06 16:28:21.000000 byma-0.1.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.985394 byma-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-10 17:48:47.000000 byma-0.1.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-10 17:48:47.000000 byma-0.1.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-10 17:48:47.000000 byma-0.1.3/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-10 17:48:47.000000 byma-0.1.3/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-10 17:48:47.000000 byma-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-10 17:49:01.985394 byma-0.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-10 17:48:47.000000 byma-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.970394 byma-0.1.3/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-10 17:48:47.000000 byma-0.1.3/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-10 17:49:01.000000 byma-0.1.3/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.972394 byma-0.1.3/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-10 17:48:47.000000 byma-0.1.3/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-10 17:48:47.000000 byma-0.1.3/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-10 17:48:47.000000 byma-0.1.3/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.972394 byma-0.1.3/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/Iteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.973394 byma-0.1.3/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.974394 byma-0.1.3/byma/numy/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/Numy.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/_numy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.975394 byma-0.1.3/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-10 17:48:47.000000 byma-0.1.3/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-10 17:48:47.000000 byma-0.1.3/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.984394 byma-0.1.3/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.975394 byma-0.1.3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-10 17:48:47.000000 byma-0.1.3/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-10 17:48:47.000000 byma-0.1.3/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 17:48:47.000000 byma-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3791 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/iteral/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.978394 byma-0.1.3/docs/source/autoapi/byma/iteral/Iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/Iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.978394 byma-0.1.3/docs/source/autoapi/byma/iteral/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1912 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.978394 byma-0.1.3/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2112 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.979394 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.979394 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.979394 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/Stationary/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.981394 byma-0.1.3/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.981394 byma-0.1.3/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.981394 byma-0.1.3/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/Numy/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/Numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/_numy/
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/_numy/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/integration/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.983394 byma-0.1.3/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     2752 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.983394 byma-0.1.3/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.984394 byma-0.1.3/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/whatisbyma.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-10 17:48:47.000000 byma-0.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-10 17:48:47.000000 byma-0.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 17:49:01.985394 byma-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-10 17:48:47.000000 byma-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.984394 byma-0.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 17:48:47.000000 byma-0.1.3/tests/__init__.py
```

### Comparing `byma-0.1.2/.gitlab-ci.yml` & `byma-0.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/LICENSE.md` & `byma-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/PKG-INFO` & `byma-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.2/README.md` & `byma-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/byma/__init__.py` & `byma-0.1.3/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/byma/interface/NonlinearHeat.py` & `byma-0.1.3/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/byma/iteral/nonstationary/Newton.py` & `byma-0.1.3/byma/iteral/Newton.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from ...interface.BaseInterface import BaseInterface as bs
-from .NonStationary import NonStationary as NonSt
+from ..interface.BaseInterface import BaseInterface as bs
+from .Iteral import Iteral as Int
 import scipy.sparse as sp
 
 _DEFAULT_OPTS = {
     'stop': 'normal', 
     'maxit': 1e4, 
     'tol': 1e-8, 
     'verbose': False,
@@ -43,15 +43,15 @@
             return x, dxnorm 
         else: 
             return x, fnorm
         
     elif ((mode == None) or (mode == False)):
         return x, dxnorm, fnorm
 
-@bs.set_defaults(default_cls = NonSt, default_opts=_DEFAULT_OPTS)
+@bs.set_defaults(default_cls = Int, default_opts=_DEFAULT_OPTS)
 def newton(x, f, df, **kwargs):
     """
     Perform Newton iterations to find the root of a given function.
 
     Parameters
     ----------
     x : array_like
```

### Comparing `byma-0.1.2/byma/iteral/stationary/OrthogonalSubspace.py` & `byma-0.1.3/byma/iteral/OrthogonalSubspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from scipy.linalg import lu, inv, solve
 from numpy.linalg import qr
-from ...interface.BaseInterface import BaseInterface as bs
-from .Stationary import Stationary as St
+from ..interface.BaseInterface import BaseInterface as bs
+from .Iteral import Iteral as Int
+import scipy.sparse as sp
 
 _DEFAULT_OPTS = {
         'stop': 'matrix',
         'maxit': 1e4,
         'tol': 1e-8,
         'method': 'standard',
         'verbose': True,
@@ -18,15 +19,15 @@
     if method == 'LU':
         y = solve(inv(U), P.dot(V))
         z = solve(inv(L), y)
     else:
         z = A @ V
     return z
 
-@bs.set_defaults(default_cls = St, default_opts=_DEFAULT_OPTS)
+@bs.set_defaults(default_cls = Int, default_opts=_DEFAULT_OPTS)
 def osim(A, V, **kwargs):
     """
     Orthogonal Subspace Iteration Method (OSIM).
 
     Args:
     A : numpy.ndarray
         The matrix to compute the eigenvalues and eigenvectors for.
@@ -54,27 +55,27 @@
         Tuple containing eigenvalues at each iteration.
 
     Notes:
     This function implements the Orthogonal Subspace Iteration Method (OSIM) to compute eigenvectors and eigenvalues of a matrix A.
 
     Examples:
     >>> import numpy as np
-    >>> from iteral import stationary as st
+    >>> from byma.interal import osim
     >>> A = np.array([[1, 0], [0, 1]])
     >>> V = np.array([[1], [0]])
-    >>> V, BV, iter = st.osim(A, V, tol=1e-8, maxit=1000, stop='eig', method='LU')
+    >>> V, BV, iter = osim(A, V, tol=1e-8, maxit=1000, stop='eig', method='LU')
 
     You can also pass keyword arguments using a dictionary. For example:
     >>> kwargs = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
     >>> V, BV, iter = osim(A, V, **kwargs)
 
     You can also pass keyword arguments using two separate dictionaries for parameters and interface. For example:
     >>> parameters = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
     >>> interface = {'verbose': True}
-    >>> V, BV, iter = st.osim(A, V, parameters=parameters, interface=interface)
+    >>> V, BV, iter = sosim(A, V, parameters=parameters, interface=interface)
     """
     
     # Check if the number of rows of V matches the number of columns of A
     if V.shape[0] != A.shape[1]:
         raise ValueError("Number of rows of V must match the number of columns of A.")
     
     _opts = bs.opts(**kwargs)
@@ -90,15 +91,18 @@
         print(f'maximum iter: {maxit}')
         print(f'stopping criteria: {stop}')
         print(f'Linear system solving method: {method}')
     
         print('------ Start iteration ------')
     
     if method == 'LU':
-        P, L, U = lu(A.toarray())
+        if sp.issparse(A):
+            P, L, U = lu(A.toarray())
+        else:
+            P, L, U = lu(A)
     else:
         P = L = U = None
 
     B = lambda V: V.T @ _Z(V = V, A = A, P = P, L = L, U = U, method = method)
 
     iter = []
     for n in range(maxit):
```

### Comparing `byma-0.1.2/byma/nuby/Continuation.py` & `byma-0.1.3/byma/nuby/Continuation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import scipy.sparse as sp
-from ..iteral.nonstationary import newton
+from ..iteral import newton
 from ..interface.BaseInterface import BaseInterface as bs
 from .Bifurcation import Bifurcation as Bf
 
 _DEFAULT_OPTS = {
     'maxit_cont' : 1000,
     'verbose': True,
     'mode': None, 
@@ -161,15 +161,15 @@
     _opts = bs.opts(**kwargs)
     mode_con = _opts['mode']
     method = _opts['method']
     maxit_con = _opts['maxit_cont']
     verbose = _opts['verbose']
     
     dx = dx0.copy()
-    mu = start.copy()
+    mu = start
 
     # Set some parameters
     if (target is None) and (dmu is None):
         raise ValueError("Either 'dmu' or 'target' should be not 'None'")
     
     else:
         mus = np.linspace(mu, target, maxit_con)
```

### Comparing `byma-0.1.2/byma/pyplot/plots.py` & `byma-0.1.3/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/byma.egg-info/PKG-INFO` & `byma-0.1.3/byma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.2/byma.egg-info/SOURCES.txt` & `byma-0.1.3/byma.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,50 +12,57 @@
 byma.egg-info/PKG-INFO
 byma.egg-info/SOURCES.txt
 byma.egg-info/dependency_links.txt
 byma.egg-info/top_level.txt
 byma/interface/BaseInterface.py
 byma/interface/NonlinearHeat.py
 byma/interface/__init__.py
+byma/iteral/Iteral.py
+byma/iteral/Newton.py
+byma/iteral/OrthogonalSubspace.py
 byma/iteral/__init__.py
-byma/iteral/nonstationary/Newton.py
-byma/iteral/nonstationary/NonStationary.py
-byma/iteral/nonstationary/__init__.py
-byma/iteral/stationary/OrthogonalSubspace.py
-byma/iteral/stationary/Stationary.py
-byma/iteral/stationary/__init__.py
 byma/nuby/Bifurcation.py
 byma/nuby/Continuation.py
 byma/nuby/__init__.py
 byma/nuby/_nuby.py
+byma/numy/Numy.py
+byma/numy/__init__.py
+byma/numy/_numy.py
+byma/numy/integration.py
 byma/pyplot/__init__.py
 byma/pyplot/plots.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/autoapi/index.rst
 docs/source/autoapi/byma/index.rst
 docs/source/autoapi/byma/_version/index.rst
 docs/source/autoapi/byma/interface/index.rst
 docs/source/autoapi/byma/interface/BaseInterface/index.rst
 docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
 docs/source/autoapi/byma/iteral/index.rst
+docs/source/autoapi/byma/iteral/Iteral/index.rst
+docs/source/autoapi/byma/iteral/Newton/index.rst
+docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
 docs/source/autoapi/byma/iteral/nonstationary/index.rst
 docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
 docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
 docs/source/autoapi/byma/iteral/stationary/index.rst
 docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
 docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
 docs/source/autoapi/byma/nuby/index.rst
 docs/source/autoapi/byma/nuby/Bifurcation/index.rst
 docs/source/autoapi/byma/nuby/Continuation/index.rst
 docs/source/autoapi/byma/nuby/_nuby/index.rst
+docs/source/autoapi/byma/numy/index.rst
+docs/source/autoapi/byma/numy/Numy/index.rst
+docs/source/autoapi/byma/numy/_numy/index.rst
+docs/source/autoapi/byma/numy/integration/index.rst
 docs/source/autoapi/byma/pyplot/index.rst
 docs/source/autoapi/byma/pyplot/plots/index.rst
 docs/source/user/Installation.rst
 docs/source/user/index.rst
 docs/source/user/quickstart.rst
 docs/source/user/whatisbyma.rst
-examples/example.py
 tests/__init__.py
```

### Comparing `byma-0.1.2/docs/Makefile` & `byma-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/make.bat` & `byma-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/autoapi/byma/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -30,10 +30,11 @@
 .. toctree::
    :titlesonly:
    :maxdepth: 3
 
    interface/index.rst
    iteral/index.rst
    nuby/index.rst
+   numy/index.rst
    pyplot/index.rst
```

### Comparing `byma-0.1.2/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/autoapi/byma/interface/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/interface/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,36 @@
 
       Returns
       -------
       dict
           A dictionary containing updated interface and parameters.
 
 
+   .. py:method:: check_none()
+
+      Check if any of the arguments are None.
+
+      Parameters
+      ----------
+      *args : tuple
+          Arbitrary number of arguments to check.
+
+      Returns
+      -------
+      bool
+          True if any argument is None, False otherwise.
+
+      Raises
+      ------
+      ValueError
+          If any argument is None, raises ValueError with the names of the None arguments.
+
+
+
+
 
 .. py:class:: NonlinearHeat
 
 
    Damped stationary heat equation with discretization using finite difference method.
 
    The equation is given by:
```

### Comparing `byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,52 @@
-:py:mod:`byma.nuby.Continuation`
-================================
+:orphan:
+
+:py:mod:`byma.nuby._nuby`
+=========================
+
+.. py:module:: byma.nuby._nuby
+
+.. autoapi-nested-parse::
+
+   Notes
+   -----
+   This module is has basic bifurcation analysis tools
 
-.. py:module:: byma.nuby.Continuation
 
 
 Module Contents
 ---------------
 
+Classes
+~~~~~~~
+
+.. autoapisummary::
+
+   byma.nuby._nuby.Bifurcation
+
+
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby.Continuation.step
-   byma.nuby.Continuation.cont
+   byma.nuby._nuby.step
+   byma.nuby._nuby.cont
 
 
 
-.. py:function:: step(x, df, dfmu, dx, dmu, **kwargs)
+.. py:function:: step(x, f, df, dfmu, dx, dmu, **kwargs)
 
    Perform one step of the continuation.
 
    :param x: array_like
        Current state.
+   :param f: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
    :param df: callable
        Function to evaluate the Jacobian matrix with respect to state variable x.
    :param dfmu: callable
        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
    :param dx: array_like
        Current tangent with respect to state variable.
    :param dmu: float or array_like
@@ -38,26 +57,28 @@
    :return: tuple
        A tuple containing the updated state x and the norm of the correction and the derivative of x w.r.t parameter
 
    :description:
    This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
 
-.. py:function:: cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs)
+.. py:function:: cont(x0, dx0, start, f, df, dfmu, dmu=None, target=None, **kwargs)
 
    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
    :param x0: array_like
        Initial state.
    :param dx0: array_like
        Initial tangent with respect to state variable.
    :param start: float
        Starting parameter value.
+   :param f: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
    :param df: callable
        Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
    :param dfmu: callable
        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
    :param dmu: float or array_like, optional
        Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
    :param target: float or None, optional
@@ -98,7 +119,13 @@
        >>> # Perform continuation from start value to target value
        >>> start = 0.0
        >>> target = 1.0
        >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
        >>> print(result)
 
 
+.. py:class:: Bifurcation
+
+
+   Defines default options for the Bifurcation package
+
+
```

### Comparing `byma-0.1.2/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/nuby/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,76 @@
-:orphan:
+:py:mod:`byma.nuby`
+===================
 
-:py:mod:`byma.nuby._nuby`
-=========================
-
-.. py:module:: byma.nuby._nuby
+.. py:module:: byma.nuby
 
 .. autoapi-nested-parse::
 
-   Notes
-   -----
-   This module is has basic bifurcation analysis tools
+   ``byma.nuby``
+   ================
+
+   The ByMa numerical bifurcation functions rely on 
+
+   Functions present in byma.nuby are listed below.
+
+
+   Continuation
+   --------------------------
+
+      step
+      cont
+      
+
+   Exceptions
+   ----------
 
+      NuByError
 
 
-Module Contents
----------------
+
+Submodules
+----------
+.. toctree::
+   :titlesonly:
+   :maxdepth: 1
+
+   Bifurcation/index.rst
+   Continuation/index.rst
+
+
+Package Contents
+----------------
 
 Classes
 ~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby._nuby.Bifurcation
+   byma.nuby.Bifurcation
 
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby._nuby.step
-   byma.nuby._nuby.cont
+   byma.nuby.step
+   byma.nuby.cont
 
 
 
-.. py:function:: step(x, df, dfmu, dx, dmu, **kwargs)
+.. py:function:: step(x, f, df, dfmu, dx, dmu, **kwargs)
 
    Perform one step of the continuation.
 
    :param x: array_like
        Current state.
+   :param f: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
    :param df: callable
        Function to evaluate the Jacobian matrix with respect to state variable x.
    :param dfmu: callable
        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
    :param dx: array_like
        Current tangent with respect to state variable.
    :param dmu: float or array_like
@@ -55,26 +81,28 @@
    :return: tuple
        A tuple containing the updated state x and the norm of the correction and the derivative of x w.r.t parameter
 
    :description:
    This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
 
-.. py:function:: cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs)
+.. py:function:: cont(x0, dx0, start, f, df, dfmu, dmu=None, target=None, **kwargs)
 
    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
    :param x0: array_like
        Initial state.
    :param dx0: array_like
        Initial tangent with respect to state variable.
    :param start: float
        Starting parameter value.
+   :param f: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
    :param df: callable
        Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
    :param dfmu: callable
        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
    :param dmu: float or array_like, optional
        Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
    :param target: float or None, optional
```

### Comparing `byma-0.1.2/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/nuby/Continuation/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,35 @@
-:py:mod:`byma.nuby`
-===================
+:py:mod:`byma.nuby.Continuation`
+================================
 
-.. py:module:: byma.nuby
+.. py:module:: byma.nuby.Continuation
 
-.. autoapi-nested-parse::
-
-   ``byma.nuby``
-   ================
-
-   The ByMa numerical bifurcation functions rely on 
-
-   Functions present in byma.nuby are listed below.
-
-
-   Continuation
-   --------------------------
-
-      step
-      cont
-      
-
-   Exceptions
-   ----------
-
-      NuByError
-
-
-
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
-
-   Bifurcation/index.rst
-   Continuation/index.rst
-
-
-Package Contents
-----------------
-
-Classes
-~~~~~~~
-
-.. autoapisummary::
-
-   byma.nuby.Bifurcation
 
+Module Contents
+---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby.step
-   byma.nuby.cont
+   byma.nuby.Continuation.step
+   byma.nuby.Continuation.cont
 
 
 
-.. py:function:: step(x, df, dfmu, dx, dmu, **kwargs)
+.. py:function:: step(x, f, df, dfmu, dx, dmu, **kwargs)
 
    Perform one step of the continuation.
 
    :param x: array_like
        Current state.
+   :param f: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
    :param df: callable
        Function to evaluate the Jacobian matrix with respect to state variable x.
    :param dfmu: callable
        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
    :param dx: array_like
        Current tangent with respect to state variable.
    :param dmu: float or array_like
@@ -79,26 +40,28 @@
    :return: tuple
        A tuple containing the updated state x and the norm of the correction and the derivative of x w.r.t parameter
 
    :description:
    This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
 
-.. py:function:: cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs)
+.. py:function:: cont(x0, dx0, start, f, df, dfmu, dmu=None, target=None, **kwargs)
 
    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
    :param x0: array_like
        Initial state.
    :param dx0: array_like
        Initial tangent with respect to state variable.
    :param start: float
        Starting parameter value.
+   :param f: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
    :param df: callable
        Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
    :param dfmu: callable
        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
    :param dmu: float or array_like, optional
        Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
    :param target: float or None, optional
@@ -139,13 +102,7 @@
        >>> # Perform continuation from start value to target value
        >>> start = 0.0
        >>> target = 1.0
        >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
        >>> print(result)
 
 
-.. py:class:: Bifurcation
-
-
-   Defines default options for the Bifurcation package
-
-
```

### Comparing `byma-0.1.2/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.3/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/conf.py` & `byma-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/docs/source/index.rst` & `byma-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/pyproject.toml` & `byma-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.2/setup.py` & `byma-0.1.3/setup.py`

 * *Files identical despite different names*

