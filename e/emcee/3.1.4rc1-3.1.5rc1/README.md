# Comparing `tmp/emcee-3.1.4rc1.tar.gz` & `tmp/emcee-3.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emcee-3.1.4rc1.tar", last modified: Fri Jan 27 03:17:26 2023, max compression
+gzip compressed data, was "emcee-3.1.5rc1.tar", last modified: Wed Apr 10 20:13:49 2024, max compression
```

## Comparing `emcee-3.1.4rc1.tar` & `emcee-3.1.5rc1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.282403 emcee-3.1.4rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.254403 emcee-3.1.4rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.254403 emcee-3.1.4rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-01-27 03:17:26.282403 emcee-3.1.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/VISION.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.254403 emcee-3.1.4rc1/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/binder/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.254403 emcee-3.1.4rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.258403 emcee-3.1.4rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.262403 emcee-3.1.4rc1/docs/_static/line/
--rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/line/line-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/line/line-least-squares.png
--rw-r--r--   0 runner    (1001) docker     (123)    34934 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/line/line-max-likelihood.png
--rw-r--r--   0 runner    (1001) docker     (123)    67232 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/line/line-mcmc.png
--rw-r--r--   0 runner    (1001) docker     (123)   404073 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/line/line-time.png
--rw-r--r--   0 runner    (1001) docker     (123)   126982 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/line/line-triangle.png
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/logo-sidebar.png
--rw-r--r--   0 runner    (1001) docker     (123)   150797 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/logo.pxm
--rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/logo2.png
--rw-r--r--   0 runner    (1001) docker     (123)   240605 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/_static/logo2.pxm
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/fix_internal_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.266403 emcee-3.1.4rc1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   515948 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/autocorr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   865248 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1100505 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/monitor.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   245392 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/moves.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/parallel.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/tutorials/tutorial_rst.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.270403 emcee-3.1.4rc1/docs/user/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/autocorr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/blobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/moves.rst
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/sampler.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/docs/user/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.270403 emcee-3.1.4rc1/document/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/document/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/document/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    66184 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/document/aastex.cls
--rw-r--r--   0 runner    (1001) docker     (123)    41540 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/document/ms.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.270403 emcee-3.1.4rc1/document/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/document/plots/oned.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/document/plots/plot_acor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.274403 emcee-3.1.4rc1/joss/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/joss/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/joss/make_latex.sh
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/joss/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/joss/paper.tex
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 03:17:26.282403 emcee-3.1.4rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2376 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.246403 emcee-3.1.4rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.274403 emcee-3.1.4rc1/src/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/autocorr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.278403 emcee-3.1.4rc1/src/emcee/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/backends/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee/emcee_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/interruptible_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.278403 emcee-3.1.4rc1/src/emcee/moves/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/de_snooker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/mh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/move.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/red_blue.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/moves/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/pbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/ptsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.278403 emcee-3.1.4rc1/src/emcee/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.282403 emcee-3.1.4rc1/src/emcee/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_de.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_de_snooker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_longdouble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/integration/test_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.282403 emcee-3.1.4rc1/src/emcee/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_autocorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_blobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/tests/unit/test_stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/src/emcee/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:17:26.278403 emcee-3.1.4rc1/src/emcee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 03:17:26.000000 emcee-3.1.4rc1/src/emcee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-27 03:17:12.000000 emcee-3.1.4rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/VISION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/_static/line/
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-least-squares.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-max-likelihood.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67232 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-mcmc.png
+-rw-r--r--   0 runner    (1001) docker     (127)   404073 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-time.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126982 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-triangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo-sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (127)   150797 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo.pxm
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   240605 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo2.pxm
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/fix_internal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.290466 emcee-3.1.5rc1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   515948 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/autocorr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   865248 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1100525 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/monitor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   245392 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/moves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/parallel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/tutorial_rst.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/autocorr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/blobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/moves.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    66184 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/aastex.cls
+-rw-r--r--   0 runner    (1001) docker     (127)    41540 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/ms.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/document/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/plots/oned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/plots/plot_acor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/joss/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/make_latex.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2376 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.278466 emcee-3.1.5rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.298467 emcee-3.1.5rc1/src/emcee/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/autocorr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.298467 emcee-3.1.5rc1/src/emcee/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee/emcee_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25923 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/interruptible_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/moves/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/de_snooker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/mh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/red_blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/ptsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_de_snooker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_longdouble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_autocorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_blobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/tox.ini
```

### Comparing `emcee-3.1.4rc1/.github/ISSUE_TEMPLATE.md` & `emcee-3.1.5rc1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/.github/workflows/tests.yml` & `emcee-3.1.5rc1/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,29 +12,29 @@
   pull_request:
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         os: ["ubuntu-latest"]
         include:
           - python-version: "3.9"
             os: "macos-latest"
           - python-version: "3.9"
             os: "windows-latest"
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U coveralls coverage[toml] tox tox-gh-actions
       - name: Run tests
@@ -45,73 +45,97 @@
           python -m coverage xml -i
           python -m coveralls --service=github
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           COVERALLS_PARALLEL: true
           COVERALLS_FLAG_NAME: ${{ matrix.python-version }}-${{ matrix.os }}
 
+  leading_edge:
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        python-version: ["3.12"]
+        os: ["ubuntu-latest"]
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+      - name: Setup Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install -U pip
+          python -m pip install pip install pytest "numpy>=2.0.0rc1"
+          python -m pip install -e.
+      - name: Run tests
+        run: pytest
+
   coverage:
     needs: tests
     runs-on: ubuntu-latest
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.9"
       - name: Finish coverage collection
         run: |
           python -m pip install -U pip
           python -m pip install -U coveralls
           python -m coveralls --finish
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
   lint:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.9"
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install tox
       - name: Lint the code
         run: python -m tox -e lint
 
   build:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: "3.9"
       - name: Build sdist and wheel
         run: |
           python -m pip install -U pip
           python -m pip install -U build
           python -m build .
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           path: dist/*
 
   upload_pypi:
     needs: [tests, lint, build]
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `emcee-3.1.4rc1/CODE_OF_CONDUCT.md` & `emcee-3.1.5rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/CONTRIBUTING.md` & `emcee-3.1.5rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/HISTORY.rst` & `emcee-3.1.5rc1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/LICENSE` & `emcee-3.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/PKG-INFO` & `emcee-3.1.5rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emcee
-Version: 3.1.4rc1
+Version: 3.1.5rc1
 Summary: The Python ensemble sampling toolkit for MCMC
 Home-page: https://emcee.readthedocs.io
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
@@ -12,18 +12,24 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
-Provides-Extra: extras
-Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: numpy
+Provides-Extra: extras
+Requires-Dist: h5py; extra == "extras"
+Requires-Dist: scipy; extra == "extras"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: coverage[toml]; extra == "tests"
 
 emcee
 =====
 
 **The Python ensemble sampling toolkit for affine-invariant MCMC**
 
 .. image:: https://img.shields.io/badge/GitHub-dfm%2Femcee-blue.svg?style=flat
```

### Comparing `emcee-3.1.4rc1/README.rst` & `emcee-3.1.5rc1/README.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/Makefile` & `emcee-3.1.5rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/favicon.png` & `emcee-3.1.5rc1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/line/line-data.png` & `emcee-3.1.5rc1/docs/_static/line/line-data.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/line/line-least-squares.png` & `emcee-3.1.5rc1/docs/_static/line/line-least-squares.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/line/line-max-likelihood.png` & `emcee-3.1.5rc1/docs/_static/line/line-max-likelihood.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/line/line-mcmc.png` & `emcee-3.1.5rc1/docs/_static/line/line-mcmc.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/line/line-time.png` & `emcee-3.1.5rc1/docs/_static/line/line-time.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/line/line-triangle.png` & `emcee-3.1.5rc1/docs/_static/line/line-triangle.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/logo-sidebar.png` & `emcee-3.1.5rc1/docs/_static/logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/logo.pxm` & `emcee-3.1.5rc1/docs/_static/logo.pxm`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/logo2.png` & `emcee-3.1.5rc1/docs/_static/logo2.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/_static/logo2.pxm` & `emcee-3.1.5rc1/docs/_static/logo2.pxm`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/conf.py` & `emcee-3.1.5rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/index.rst` & `emcee-3.1.5rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/tutorials/autocorr.ipynb` & `emcee-3.1.5rc1/docs/tutorials/autocorr.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/tutorials/line.ipynb` & `emcee-3.1.5rc1/docs/tutorials/line.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/tutorials/monitor.ipynb` & `emcee-3.1.5rc1/docs/tutorials/monitor.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999385683760684%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, '\\n')]}}, 15: {'source': {insert: [(1, '\\n')]}}}"}*

```diff
@@ -50,14 +50,15 @@
             "outputs": [],
             "source": [
                 "import emcee\n",
                 "import numpy as np\n",
                 "\n",
                 "np.random.seed(42)\n",
                 "\n",
+                "\n",
                 "# The definition of the log probability function\n",
                 "# We'll also use the \"blobs\" feature to track the \"log prior\" for each step\n",
                 "def log_prob(theta):\n",
                 "    log_prior = -0.5 * np.sum((theta - 1.0) ** 2 / 100.0)\n",
                 "    log_prob = -0.5 * np.sum(theta**2) + log_prior\n",
                 "    return log_prob, log_prior\n",
                 "\n",
@@ -334,14 +335,15 @@
                         "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 6000/6000 [00:42<00:00, 139.66it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "run2_backend = emcee.backends.HDFBackend(filename, name=\"mcmc_second_prior\")\n",
                 "\n",
+                "\n",
                 "# this time, with a subtly different prior\n",
                 "def log_prob2(theta):\n",
                 "    log_prior = -0.5 * np.sum((theta - 2.0) ** 2 / 100.0)\n",
                 "    log_prob = -0.5 * np.sum(theta**2) + log_prior\n",
                 "    return log_prob, log_prior\n",
                 "\n",
                 "\n",
```

### Comparing `emcee-3.1.4rc1/docs/tutorials/moves.ipynb` & `emcee-3.1.5rc1/docs/tutorials/moves.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333334%*

 * *Differences: {"'cells'": '{7: {\'source\': {insert: [(2, "In detail, this means that, at each step, we\'ll '*

 * *            'randomly select either a {class}`moves.DEMove` (with 80% probability) or a '*

 * *            '{class}`moves.DESnookerMove` (with 20% probability).")], delete: [2]}}}'}*

```diff
@@ -156,15 +156,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For \"lightly\" multimodal problems like these, some combination of the {class}`moves.DEMove` and {class}`moves.DESnookerMove` can often perform better than the default.\n",
                 "In this case, let's use a weighted mixture of the two moves.\n",
-                "In deatil, this means that, at each step, we'll randomly select either a :class:`moves.DEMove` (with 80% probability) or a {class}`moves.DESnookerMove` (with 20% probability)."
+                "In detail, this means that, at each step, we'll randomly select either a {class}`moves.DEMove` (with 80% probability) or a {class}`moves.DESnookerMove` (with 20% probability)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
```

### Comparing `emcee-3.1.4rc1/docs/tutorials/parallel.ipynb` & `emcee-3.1.5rc1/docs/tutorials/parallel.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/tutorials/quickstart.ipynb` & `emcee-3.1.5rc1/docs/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/tutorials/tutorial_rst.tpl` & `emcee-3.1.5rc1/docs/tutorials/tutorial_rst.tpl`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/user/backends.rst` & `emcee-3.1.5rc1/docs/user/backends.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/user/faq.rst` & `emcee-3.1.5rc1/docs/user/faq.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/user/install.rst` & `emcee-3.1.5rc1/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/user/moves.rst` & `emcee-3.1.5rc1/docs/user/moves.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/docs/user/upgrade.rst` & `emcee-3.1.5rc1/docs/user/upgrade.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/document/aastex.cls` & `emcee-3.1.5rc1/document/aastex.cls`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/document/ms.tex` & `emcee-3.1.5rc1/document/ms.tex`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/document/plots/oned.py` & `emcee-3.1.5rc1/document/plots/oned.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/joss/make_latex.sh` & `emcee-3.1.5rc1/joss/make_latex.sh`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/joss/metadata.yaml` & `emcee-3.1.5rc1/joss/metadata.yaml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/joss/paper.bib` & `emcee-3.1.5rc1/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/joss/paper.md` & `emcee-3.1.5rc1/joss/paper.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/joss/paper.tex` & `emcee-3.1.5rc1/joss/paper.tex`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/pyproject.toml` & `emcee-3.1.5rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/setup.py` & `emcee-3.1.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/__init__.py` & `emcee-3.1.5rc1/src/emcee/__init__.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/autocorr.py` & `emcee-3.1.5rc1/src/emcee/autocorr.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,48 +42,56 @@
 def auto_window(taus, c):
     m = np.arange(len(taus)) < c * taus
     if np.any(m):
         return np.argmin(m)
     return len(taus) - 1
 
 
-def integrated_time(x, c=5, tol=50, quiet=False):
+def integrated_time(x, c=5, tol=50, quiet=False, has_walkers=True):
     """Estimate the integrated autocorrelation time of a time series.
 
     This estimate uses the iterative procedure described on page 16 of
     `Sokal's notes <https://www.semanticscholar.org/paper/Monte-Carlo-Methods-in-Statistical-Mechanics%3A-and-Sokal/0bfe9e3db30605fe2d4d26e1a288a5e2997e7225>`_ to
     determine a reasonable window size.
 
     Args:
-        x: The time series. If multidimensional, set the time axis using the
-            ``axis`` keyword argument and the function will be computed for
-            every other axis.
+        x (numpy.ndarray): The time series. If 2-dimensional, the array
+            dimesions are interpreted as ``(n_step, n_walker)`` unless
+            ``has_walkers==False``, in which case they are interpreted as
+            ``(n_step, n_param)``. If 3-dimensional, the dimensions are
+            interperted as ``(n_step, n_walker, n_param)``.
         c (Optional[float]): The step size for the window search. (default:
             ``5``)
         tol (Optional[float]): The minimum number of autocorrelation times
             needed to trust the estimate. (default: ``50``)
         quiet (Optional[bool]): This argument controls the behavior when the
             chain is too short. If ``True``, give a warning instead of raising
             an :class:`AutocorrError`. (default: ``False``)
+        has_walkers (Optional[bool]): Whether the last axis should be
+            interpreted as walkers or parameters if ``x`` has 2 dimensions.
+            (default: ``True``)
 
     Returns:
         float or array: An estimate of the integrated autocorrelation time of
-            the time series ``x`` computed along the axis ``axis``.
+            the time series ``x``.
 
     Raises
         AutocorrError: If the autocorrelation time can't be reliably estimated
             from the chain and ``quiet`` is ``False``. This normally means
             that the chain is too short.
 
     """
     x = np.atleast_1d(x)
     if len(x.shape) == 1:
         x = x[:, np.newaxis, np.newaxis]
     if len(x.shape) == 2:
-        x = x[:, :, np.newaxis]
+        if not has_walkers:
+            x = x[:, np.newaxis, :]
+        else:
+            x = x[:, :, np.newaxis]
     if len(x.shape) != 3:
         raise ValueError("invalid dimensions")
 
     n_t, n_w, n_d = x.shape
     tau_est = np.empty(n_d)
     windows = np.empty(n_d, dtype=int)
```

### Comparing `emcee-3.1.4rc1/src/emcee/backends/backend.py` & `emcee-3.1.5rc1/src/emcee/backends/backend.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/backends/hdf.py` & `emcee-3.1.5rc1/src/emcee/backends/hdf.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/ensemble.py` & `emcee-3.1.5rc1/src/emcee/ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         moves (Optional): This can be a single move object, a list of moves,
             or a "weighted" list of the form ``[(emcee.moves.StretchMove(),
             0.1), ...]``. When running, the sampler will randomly select a
             move from this list (optionally with weights) for each proposal.
             (default: :class:`StretchMove`)
         args (Optional): A list of extra positional arguments for
             ``log_prob_fn``. ``log_prob_fn`` will be called with the sequence
-            ``log_pprob_fn(p, *args, **kwargs)``.
+            ``log_prob_fn(p, *args, **kwargs)``.
         kwargs (Optional): A dict of extra keyword arguments for
             ``log_prob_fn``. ``log_prob_fn`` will be called with the sequence
-            ``log_pprob_fn(p, *args, **kwargs)``.
+            ``log_prob_fn(p, *args, **kwargs)``.
         pool (Optional): An object with a ``map`` method that follows the same
             calling sequence as the built-in ``map`` function. This is
             generally used to compute the log-probabilities for the ensemble
             in parallel.
         backend (Optional): Either a :class:`backends.Backend` or a subclass
             (like :class:`backends.HDFBackend`) that is used to store and
             serialize the state of the chain. By default, the chain is stored
@@ -175,15 +175,15 @@
             # Check for duplicate names
             dupes = set()
             uniq = []
             for name in parameter_names:
                 if name not in dupes:
                     uniq.append(name)
                     dupes.add(name)
-            msg = f"duplicate paramters: {dupes}"
+            msg = f"duplicate parameters: {dupes}"
             assert len(uniq) == len(parameter_names), msg
 
             if isinstance(parameter_names, list):
                 # Check for all named
                 msg = "name all parameters or set `parameter_names` to `None`"
                 assert len(parameter_names) == ndim, msg
                 # Convert a list to a dict
@@ -485,28 +485,37 @@
             if self.pool is not None:
                 map_func = self.pool.map
             else:
                 map_func = map
             results = list(map_func(self.log_prob_fn, p))
 
         try:
-            log_prob = np.array([float(l[0]) for l in results])
-            blob = [l[1:] for l in results]
+            # perhaps log_prob_fn returns blobs?
+
+            # deal with the blobs first
+            # if l does not have a len attribute (i.e. not a sequence, no blob)
+            # then a TypeError is raised. However, no error will be raised if
+            # l is a length-1 array, np.array([1.234]). In that case blob
+            # will become an empty list.
+            blob = [l[1:] for l in results if len(l) > 1]
+            if not len(blob):
+                raise IndexError
+            log_prob = np.array([_scalar(l[0]) for l in results])
         except (IndexError, TypeError):
-            log_prob = np.array([float(l) for l in results])
+            log_prob = np.array([_scalar(l) for l in results])
             blob = None
         else:
             # Get the blobs dtype
             if self.blobs_dtype is not None:
                 dt = self.blobs_dtype
             else:
                 try:
                     with warnings.catch_warnings(record=True):
                         warnings.simplefilter(
-                            "error", np.VisibleDeprecationWarning
+                            "error", np.exceptions.VisibleDeprecationWarning
                         )
                         try:
                             dt = np.atleast_1d(blob[0]).dtype
                         except Warning:
                             deprecation_warning(
                                 "You have provided blobs that are not all the "
                                 "same shape or size. This means they must be "
@@ -678,7 +687,20 @@
         ``N`` is an integer
       key_map (Dict[str, Union[int, List[int]]):
 
     Returns:
       list of dictionaries of parameters
     """
     return [{key: xi[val] for key, val in key_map.items()} for xi in x]
+
+
+def _scalar(fx):
+    # Make sure a value is a true scalar
+    # 1.0, np.float64(1.0), np.array([1.0]), np.array(1.0)
+    if not np.isscalar(fx):
+        try:
+            fx = np.asarray(fx).item()
+        except (TypeError, ValueError) as e:
+            raise ValueError("log_prob_fn should return scalar") from e
+        return float(fx)
+    else:
+        return float(fx)
```

### Comparing `emcee-3.1.4rc1/src/emcee/moves/de.py` & `emcee-3.1.5rc1/src/emcee/moves/de_snooker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 
 from .red_blue import RedBlueMove
 
-__all__ = ["DEMove"]
+__all__ = ["DESnookerMove"]
 
 
-class DEMove(RedBlueMove):
-    r"""A proposal using differential evolution.
+class DESnookerMove(RedBlueMove):
+    """A snooker proposal using differential evolution.
 
-    This `Differential evolution proposal
-    <http://www.stat.columbia.edu/~gelman/stuff_for_blog/cajo.pdf>`_ is
-    implemented following `Nelson et al. (2013)
-    <https://arxiv.org/abs/1311.5229>`_.
+    Based on `Ter Braak & Vrugt (2008)
+    <http://link.springer.com/article/10.1007/s11222-008-9104-9>`_.
+
+    Credit goes to GitHub user `mdanthony17 <https://github.com/mdanthony17>`_
+    for proposing this as an addition to the original emcee package.
 
     Args:
-        sigma (float): The standard deviation of the Gaussian used to stretch
-            the proposal vector.
-        gamma0 (Optional[float]): The mean stretch factor for the proposal
-            vector. By default, it is :math:`2.38 / \sqrt{2\,\mathrm{ndim}}`
-            as recommended by the two references.
+        gammas (Optional[float]): The mean stretch factor for the proposal
+            vector. By default, it is :math:`1.7` as recommended by the
+            reference.
 
     """
 
-    def __init__(self, sigma=1.0e-5, gamma0=None, **kwargs):
-        self.sigma = sigma
-        self.gamma0 = gamma0
-        kwargs["nsplits"] = 3
-        super(DEMove, self).__init__(**kwargs)
-
-    def setup(self, coords):
-        self.g0 = self.gamma0
-        if self.g0 is None:
-            # Pure MAGIC:
-            ndim = coords.shape[1]
-            self.g0 = 2.38 / np.sqrt(2 * ndim)
+    def __init__(self, gammas=1.7, **kwargs):
+        self.gammas = gammas
+        kwargs["nsplits"] = 4
+        super(DESnookerMove, self).__init__(**kwargs)
 
     def get_proposal(self, s, c, random):
         Ns = len(s)
         Nc = list(map(len, c))
         ndim = s.shape[1]
-        q = np.empty((Ns, ndim), dtype=np.float64)
-        f = self.sigma * random.randn(Ns)
+        q = np.empty_like(s)
+        metropolis = np.empty(Ns, dtype=np.float64)
         for i in range(Ns):
-            w = np.array([c[j][random.randint(Nc[j])] for j in range(2)])
+            w = np.array([c[j][random.randint(Nc[j])] for j in range(3)])
             random.shuffle(w)
-            g = np.diff(w, axis=0) * self.g0 + f[i]
-            q[i] = s[i] + g
-        return q, np.zeros(Ns, dtype=np.float64)
+            z, z1, z2 = w
+            delta = s[i] - z
+            norm = np.linalg.norm(delta)
+            u = delta / np.sqrt(norm)
+            q[i] = s[i] + u * self.gammas * (np.dot(u, z1) - np.dot(u, z2))
+            metropolis[i] = np.log(np.linalg.norm(q[i] - z)) - np.log(norm)
+        return q, 0.5 * (ndim - 1.0) * metropolis
```

### Comparing `emcee-3.1.4rc1/src/emcee/moves/gaussian.py` & `emcee-3.1.5rc1/src/emcee/moves/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
             ndim = None
             proposal = _isotropic_proposal(np.sqrt(cov), factor, mode)
 
         super(GaussianMove, self).__init__(proposal, ndim=ndim)
 
 
 class _isotropic_proposal(object):
-
     allowed_modes = ["vector", "random", "sequential"]
 
     def __init__(self, scale, factor, mode):
         self.index = 0
         self.scale = scale
         if factor is None:
             self._log_factor = None
@@ -107,14 +106,13 @@
 
 class _diagonal_proposal(_isotropic_proposal):
     def get_updated_vector(self, rng, x0):
         return x0 + self.get_factor(rng) * self.scale * rng.randn(*(x0.shape))
 
 
 class _proposal(_isotropic_proposal):
-
     allowed_modes = ["vector"]
 
     def get_updated_vector(self, rng, x0):
         return x0 + self.get_factor(rng) * rng.multivariate_normal(
             np.zeros(len(self.scale)), self.scale
         )
```

### Comparing `emcee-3.1.4rc1/src/emcee/moves/kde.py` & `emcee-3.1.5rc1/src/emcee/moves/kde.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/moves/mh.py` & `emcee-3.1.5rc1/src/emcee/moves/mh.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/moves/move.py` & `emcee-3.1.5rc1/src/emcee/moves/move.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/moves/red_blue.py` & `emcee-3.1.5rc1/src/emcee/moves/red_blue.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/moves/stretch.py` & `emcee-3.1.5rc1/src/emcee/moves/stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/moves/walk.py` & `emcee-3.1.5rc1/src/emcee/moves/walk.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,14 @@
         self.s = s
         super(WalkMove, self).__init__(**kwargs)
 
     def get_proposal(self, s, c, random):
         c = np.concatenate(c, axis=0)
         Ns, Nc = len(s), len(c)
         ndim = s.shape[1]
-        q = np.empty((Ns, ndim), dtype=np.float64)
+        q = np.empty_like(s)
         s0 = Nc if self.s is None else self.s
         for i in range(Ns):
             inds = random.choice(Nc, s0, replace=False)
             cov = np.atleast_2d(np.cov(c[inds], rowvar=0))
             q[i] = random.multivariate_normal(s[i], cov)
         return q, np.zeros(Ns, dtype=np.float64)
```

### Comparing `emcee-3.1.4rc1/src/emcee/pbar.py` & `emcee-3.1.5rc1/src/emcee/pbar.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/state.py` & `emcee-3.1.5rc1/src/emcee/state.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/integration/test_gaussian.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/integration/test_kde.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_kde.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/integration/test_longdouble.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_longdouble.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/integration/test_proposal.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_proposal.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/integration/test_stretch.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_autocorr.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_autocorr.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,25 +24,31 @@
 
 def test_nd(seed=1234, ndim=3, N=150000):
     x = get_chain(seed=seed, ndim=ndim, N=N)
     tau = integrated_time(x)
     assert np.all(np.abs(tau - 19.0) / 19.0 < 0.2)
 
 
+def test_nd_without_walkers(seed=1234, ndim=3, N=10000):
+    x = get_chain(seed=seed, ndim=ndim, N=N)
+    tau1 = integrated_time(x[:, np.newaxis])
+    tau2 = integrated_time(x, has_walkers=False)
+    assert np.allclose(tau1, tau2)
+
+
 def test_too_short(seed=1234, ndim=3, N=100):
     x = get_chain(seed=seed, ndim=ndim, N=N)
     with pytest.raises(AutocorrError):
         integrated_time(x)
     tau = integrated_time(x, quiet=True)  # NOQA
 
 
 def test_autocorr_multi_works():
     np.random.seed(42)
     xs = np.random.randn(16384, 2)
 
-    # This throws exception unconditionally in buggy impl's
-    acls_multi = integrated_time(xs)
+    acls_multi = integrated_time(xs[:, np.newaxis])
     acls_single = np.array(
         [integrated_time(xs[:, i]) for i in range(xs.shape[1])]
-    )
+    ).squeeze()
 
-    assert np.all(np.abs(acls_multi - acls_single) < 2)
+    assert np.allclose(acls_multi, acls_single)
```

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_backends.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_backends.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_blobs.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_blobs.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_ensemble.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_ensemble.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Unit tests of some functionality in ensemble.py when the parameters are named
 """
+
 import string
 from unittest import TestCase
 
 import numpy as np
 import pytest
 
 from emcee.ensemble import EnsembleSampler, ndarray_to_list_of_dicts
@@ -178,7 +179,41 @@
         )
         guess = np.random.rand(n_walkers, len(self.names))
         n_steps = 50
         results = sampler.run_mcmc(guess, n_steps)
         assert results.coords.shape == (n_walkers, len(self.names))
         chain = sampler.chain
         assert chain.shape == (n_walkers, n_steps, len(self.names))
+
+
+class TestLnProbFn(TestCase):
+    # checks that the log_prob_fn can deal with a variety of 'scalar-likes'
+    def lnpdf(self, x):
+        v = np.log(np.sqrt(np.pi) * np.exp(-((x / 2.0) ** 2)))
+        v = float(v[0])
+        assert np.isscalar(v)
+        return v
+
+    def lnpdf_arr1(self, x):
+        v = self.lnpdf(x)
+        return np.array([v])
+
+    def lnpdf_float64(self, x):
+        v = self.lnpdf(x)
+        return np.float64(v)
+
+    def lnpdf_arr0D(self, x):
+        v = self.lnpdf(x)
+        return np.array(v)
+
+    def test_deal_with_scalar_likes(self):
+        rng = np.random.default_rng()
+        fns = [
+            self.lnpdf,
+            self.lnpdf_arr1,
+            self.lnpdf_float64,
+            self.lnpdf_arr0D,
+        ]
+        for fn in fns:
+            init = rng.random((50, 1))
+            sampler = EnsembleSampler(50, 1, fn)
+            _ = sampler.run_mcmc(initial_state=init, nsteps=20)
```

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_sampler.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_sampler.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_state.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_state.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/tests/unit/test_stretch.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee/utils.py` & `emcee-3.1.5rc1/src/emcee/utils.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.4rc1/src/emcee.egg-info/PKG-INFO` & `emcee-3.1.5rc1/src/emcee.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emcee
-Version: 3.1.4rc1
+Version: 3.1.5rc1
 Summary: The Python ensemble sampling toolkit for MCMC
 Home-page: https://emcee.readthedocs.io
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
@@ -12,18 +12,24 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
-Provides-Extra: extras
-Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: numpy
+Provides-Extra: extras
+Requires-Dist: h5py; extra == "extras"
+Requires-Dist: scipy; extra == "extras"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: coverage[toml]; extra == "tests"
 
 emcee
 =====
 
 **The Python ensemble sampling toolkit for affine-invariant MCMC**
 
 .. image:: https://img.shields.io/badge/GitHub-dfm%2Femcee-blue.svg?style=flat
```

### Comparing `emcee-3.1.4rc1/src/emcee.egg-info/SOURCES.txt` & `emcee-3.1.5rc1/src/emcee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 VISION.md
 pyproject.toml
-readthedocs.yml
 setup.py
 tox.ini
 .github/ISSUE_TEMPLATE.md
 .github/dependabot.yml
 .github/workflows/tests.yml
 binder/environment.yml
 docs/.gitignore
```

