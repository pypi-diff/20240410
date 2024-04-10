# Comparing `tmp/erlab-2.0.0.tar.gz` & `tmp/erlab-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.0.0.tar", last modified: Mon Apr  8 13:43:45 2024, max compression
+gzip compressed data, was "erlab-2.1.0.tar", last modified: Tue Apr  9 15:36:25 2024, max compression
```

## Comparing `erlab-2.0.0.tar` & `erlab-2.1.0.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.578651 erlab-2.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.538651 erlab-2.0.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.542651 erlab-2.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.542651 erlab-2.0.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-08 13:43:39.000000 erlab-2.0.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-08 13:43:39.000000 erlab-2.0.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-08 13:43:39.000000 erlab-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-08 13:43:39.000000 erlab-2.0.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)    98753 2024-04-08 13:43:41.000000 erlab-2.0.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-08 13:43:39.000000 erlab-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46760 2024-04-08 13:43:45.578651 erlab-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-08 13:43:39.000000 erlab-2.0.0/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4414 2024-04-08 13:43:39.000000 erlab-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.546651 erlab-2.0.0/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.546651 erlab-2.0.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    13912 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    13410 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/development.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     2888 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.554651 erlab-2.0.0/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.558651 erlab-2.0.0/docs/source/notebooks/
--rw-r--r--   0 root         (0) root         (0)   189769 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379533 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    15761 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/notebooks/plotting.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.558651 erlab-2.0.0/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2579 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2356 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/refs.bib
--rw-r--r--   0 root         (0) root         (0)     1259 2024-04-08 13:43:39.000000 erlab-2.0.0/docs/source/userguide.rst
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-08 13:43:39.000000 erlab-2.0.0/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-08 13:43:39.000000 erlab-2.0.0/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-08 13:43:39.000000 erlab-2.0.0/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-08 13:43:39.000000 erlab-2.0.0/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4351 2024-04-08 13:43:39.000000 erlab-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-08 13:43:39.000000 erlab-2.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:43:45.578651 erlab-2.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.538651 erlab-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.558651 erlab-2.0.0/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-08 13:43:41.000000 erlab-2.0.0/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35543 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      840 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9632 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)     9818 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15394 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17273 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10359 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     2775 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7810 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8659 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.562651 erlab-2.0.0/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.566651 erlab-2.0.0/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13943 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20867 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22451 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    14901 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.566651 erlab-2.0.0/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19391 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.566651 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52076 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114751 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25375 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16658 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    52417 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.570651 erlab-2.0.0/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30047 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6780 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.570651 erlab-2.0.0/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3674 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7448 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     5630 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.570651 erlab-2.0.0/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.574651 erlab-2.0.0/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     1857 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18275 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4294 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32411 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.574651 erlab-2.0.0/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-08 13:43:39.000000 erlab-2.0.0/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.578651 erlab-2.0.0/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46760 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4487 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-08 13:43:45.000000 erlab-2.0.0/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.574651 erlab-2.0.0/templates/
--rw-r--r--   0 root         (0) root         (0)      971 2024-04-08 13:43:39.000000 erlab-2.0.0/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-08 13:43:39.000000 erlab-2.0.0/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-08 13:43:39.000000 erlab-2.0.0/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:43:45.578651 erlab-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4485 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     5229 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-08 13:43:39.000000 erlab-2.0.0/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.373746 erlab-2.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.329746 erlab-2.1.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.337746 erlab-2.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.337746 erlab-2.1.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-09 15:36:19.000000 erlab-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-09 15:36:19.000000 erlab-2.1.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-09 15:36:19.000000 erlab-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-09 15:36:19.000000 erlab-2.1.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   102069 2024-04-09 15:36:21.000000 erlab-2.1.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-09 15:36:19.000000 erlab-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47662 2024-04-09 15:36:25.373746 erlab-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-09 15:36:19.000000 erlab-2.1.0/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4703 2024-04-09 15:36:19.000000 erlab-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.337746 erlab-2.1.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.341746 erlab-2.1.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    13912 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.349746 erlab-2.1.0/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.349746 erlab-2.1.0/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.349746 erlab-2.1.0/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     7084 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5606 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379533 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    15761 2024-04-09 15:36:19.000000 erlab-2.1.0/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-09 15:36:19.000000 erlab-2.1.0/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-09 15:36:19.000000 erlab-2.1.0/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-09 15:36:19.000000 erlab-2.1.0/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-09 15:36:19.000000 erlab-2.1.0/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4637 2024-04-09 15:36:19.000000 erlab-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-09 15:36:19.000000 erlab-2.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 15:36:25.373746 erlab-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.333746 erlab-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.353746 erlab-2.1.0/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-09 15:36:21.000000 erlab-2.1.0/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35543 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.353746 erlab-2.1.0/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      839 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)     9818 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15394 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17319 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10359 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7809 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8659 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.357746 erlab-2.1.0/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13943 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20867 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11371 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19391 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52076 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114751 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25375 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15728 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54144 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.361746 erlab-2.1.0/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30408 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.365746 erlab-2.1.0/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6278 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.365746 erlab-2.1.0/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     1858 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18275 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32411 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-09 15:36:19.000000 erlab-2.1.0/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47662 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4530 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-09 15:36:25.000000 erlab-2.1.0/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-09 15:36:19.000000 erlab-2.1.0/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-09 15:36:19.000000 erlab-2.1.0/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-09 15:36:19.000000 erlab-2.1.0/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:36:25.369746 erlab-2.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-09 15:36:19.000000 erlab-2.1.0/tests/test_utilities.py
```

### Comparing `erlab-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/.github/workflows/pr.yml` & `erlab-2.1.0/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/.github/workflows/release.yml` & `erlab-2.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/.gitignore` & `erlab-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/.pre-commit-config.yaml` & `erlab-2.1.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
 
   # Security & credential scanning/alerting
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: debug-statements
       - id: detect-aws-credentials
         args: ["--allow-missing-credentials"]
       - id: detect-private-key
       - id: check-builtin-literals
       - id: check-yaml
```

### Comparing `erlab-2.0.0/.readthedocs.yaml` & `erlab-2.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/CHANGELOG.md` & `erlab-2.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,110 @@
 # CHANGELOG
 
 
 
+## v2.1.0 (2024-04-09)
+
+### Chore
+
+* update changelog template ([`46a79e5`](https://github.com/kmnhan/erlabpy/commit/46a79e53c3bd6ce358d0fbf1a632d947671444c1))
+
+### Ci
+
+* (**pre-commit**) merge pull request #18 from kmnhan/pre-commit-ci-update-config ([`7018fd3`](https://github.com/kmnhan/erlabpy/commit/7018fd3cc9775db47478fe0782aa1fafd30f83a1))
+
+  [pre-commit.ci] pre-commit autoupdate
+
+### Documentation
+
+* improve io guide ([`28a2961`](https://github.com/kmnhan/erlabpy/commit/28a296131752e1df07d80c778e324adc2ef3746c))
+
+* add docstring for undocumented io functions ([`3583aad`](https://github.com/kmnhan/erlabpy/commit/3583aadbb1c707f11842ec4c154e8bcb99723056))
+
+* change directory structure, rename contributing guide ([`0b3d734`](https://github.com/kmnhan/erlabpy/commit/0b3d734b4f92cb9497bdfa7f133cbc66e6d99fb1))
+
+* update development documentation ([`38efae6`](https://github.com/kmnhan/erlabpy/commit/38efae6c591aa90dc6e1d280565df5c1dd1a004c))
+
+* update installation instructions to include conda-forge ([`c0ca81d`](https://github.com/kmnhan/erlabpy/commit/c0ca81d4c17fd7d97d1d684f4be8e5a4d49cc271))
+
+### Feature
+
+* (**interactive**) overhaul dtool ([`8e5ec38`](https://github.com/kmnhan/erlabpy/commit/8e5ec3827dd2bd52475d454d5c5ef8aef7d665aa))
+
+  Now supports interpolation, copying code, opening in imagetool, and 2D laplacian method.
+
+* (**interactive**) improve code generation ([`7cbe857`](https://github.com/kmnhan/erlabpy/commit/7cbe8572272f6c84a486599a990098ce8e3ff754))
+
+  Automatically shortens code and allows literals in kwargs
+
+* (**interactive**) extend xImageItem, add right-click menu to open imagetool ([`2b5bb2d`](https://github.com/kmnhan/erlabpy/commit/2b5bb2dfc3d4173d950135306b3b30a018c6d389))
+
+### Fix
+
+* sign error in minimum gradient ([`c45be0c`](https://github.com/kmnhan/erlabpy/commit/c45be0cf1a025c67e8af959ff83a9339cddbaaaa))
+
+* (**analysis.image**) normalize data for mingrad output for numerical stability ([`0fc3711`](https://github.com/kmnhan/erlabpy/commit/0fc3711a521ffb0cbb4f5206c06d923eced1200c))
+
+### Refactor
+
+* (**io**) validation now defaults to warning instead of raising an error ([`8867a07`](https://github.com/kmnhan/erlabpy/commit/8867a07304129beda749fa82d3909bf920fdb975))
+
+### Style
+
+* sort imports with ruff ([`81efec9`](https://github.com/kmnhan/erlabpy/commit/81efec9d3937d3ef9be1287d6275246682de296d))
+
+* avoid trailing whitespace in changelog ([`aafc441`](https://github.com/kmnhan/erlabpy/commit/aafc441003cb679624ee4521f97da8c490ebdcf4))
+
+### Test
+
+* fix tests according to minimum gradient behaviour change ([`41290f2`](https://github.com/kmnhan/erlabpy/commit/41290f210557ce48e029c9c4926f7a61f09bdd97))
+
+### Unknown
+
+* [pre-commit.ci] pre-commit autoupdate ([`1dc0de8`](https://github.com/kmnhan/erlabpy/commit/1dc0de892920d3487e6c85de700d9b8400930dd3))
+
+  updates:
+  - [github.com/pre-commit/pre-commit-hooks: v4.5.0 → v4.6.0](https://github.com/pre-commit/pre-commit-hooks/compare/v4.5.0...v4.6.0)
+
+
 ## v2.0.0 (2024-04-08)
 
 ### Breaking
 
-* **fit** unify dynamic function names ([`20d784c`](https://github.com/kmnhan/erlabpy/commit/20d784c1d8fdcd786ab73b3ae03d3e331dc04df5))
+* (**fit**) unify dynamic function names ([`20d784c`](https://github.com/kmnhan/erlabpy/commit/20d784c1d8fdcd786ab73b3ae03d3e331dc04df5))
 
   BREAKING CHANGE: `PolyFunc` is now `PolynomialFunction`, and `FermiEdge2dFunc` is now `FermiEdge2dFunction`. The corresponding model names are unchanged.
 
-* **fit** directly base models on lmfit.Model ([`59163d5`](https://github.com/kmnhan/erlabpy/commit/59163d5f0e000d65aa53690a51b6db82df1ce5f1))
+* (**fit**) directly base models on lmfit.Model ([`59163d5`](https://github.com/kmnhan/erlabpy/commit/59163d5f0e000d65aa53690a51b6db82df1ce5f1))
 
   BREAKING CHANGE: This change disables the use of guess_fit. All fitting must be performed in the syntax recommended by lmfit. Addition of a accessor or a convenience function for coordinate-aware fitting is planned in the next release.
 
 ### Build
 
 * add templates for changelog and release notes ([`be72b24`](https://github.com/kmnhan/erlabpy/commit/be72b245f1194d1bd894bd12c845f68eedbb8f3b))
 
 ### Chore
 
 * add setuptools_scm configuration ([`506faa6`](https://github.com/kmnhan/erlabpy/commit/506faa6bcb63b03bbce4add7fd5a7b5a4f761320))
 
-* **deps** update dependency to use igor2&gt;=0.5.6 now on conda-forge ([`b59fc5a`](https://github.com/kmnhan/erlabpy/commit/b59fc5a75071191e199c20424df6b76860d69029))
+* (**deps**) update dependency to use igor2&gt;=0.5.6 now on conda-forge ([`b59fc5a`](https://github.com/kmnhan/erlabpy/commit/b59fc5a75071191e199c20424df6b76860d69029))
 
-* **deps** remove igor2 direct dependency from requirements.txt ([`bfb5518`](https://github.com/kmnhan/erlabpy/commit/bfb551893d7858ed1816a376b25ef6aba5004b3b))
+* (**deps**) remove igor2 direct dependency from requirements.txt ([`bfb5518`](https://github.com/kmnhan/erlabpy/commit/bfb551893d7858ed1816a376b25ef6aba5004b3b))
 
-* **deps** remove importlib metadata ([`b5718e7`](https://github.com/kmnhan/erlabpy/commit/b5718e7aeb988b1cfe8e5026358640d49481db61))
+* (**deps**) remove importlib metadata ([`b5718e7`](https://github.com/kmnhan/erlabpy/commit/b5718e7aeb988b1cfe8e5026358640d49481db61))
 
-* **deps** update minimum versions and env configurations ([`18a3d67`](https://github.com/kmnhan/erlabpy/commit/18a3d67becacbfe2b907c206490917a85541df2c))
+* (**deps**) update minimum versions and env configurations ([`18a3d67`](https://github.com/kmnhan/erlabpy/commit/18a3d67becacbfe2b907c206490917a85541df2c))
 
-* **deps** update dependencies ([`b3e2494`](https://github.com/kmnhan/erlabpy/commit/b3e249460d99f429c403cdaad01d7f3ea16084e9))
+* (**deps**) update dependencies ([`b3e2494`](https://github.com/kmnhan/erlabpy/commit/b3e249460d99f429c403cdaad01d7f3ea16084e9))
 
-* **deps** remove importlib ([`8a6b818`](https://github.com/kmnhan/erlabpy/commit/8a6b818a1c38e87e648bdc80a82148d31083bf0d))
+* (**deps**) remove importlib ([`8a6b818`](https://github.com/kmnhan/erlabpy/commit/8a6b818a1c38e87e648bdc80a82148d31083bf0d))
 
 ### Ci
 
-* **github** swap pip installation order ([`afa4722`](https://github.com/kmnhan/erlabpy/commit/afa472259a564019c3d8e78fee158277eed9c923))
+* (**github**) swap pip installation order ([`afa4722`](https://github.com/kmnhan/erlabpy/commit/afa472259a564019c3d8e78fee158277eed9c923))
 
 ### Documentation
 
 * fix typo ([`dc8204a`](https://github.com/kmnhan/erlabpy/commit/dc8204aa67488e6efc29d50ccf73f8b0babc0f9c))
 
 * update conf.py ([`3f092c4`](https://github.com/kmnhan/erlabpy/commit/3f092c472ae5312dee18ab9be98d080124f02edc))
 
@@ -48,68 +112,67 @@
 
 * improve readability ([`bd8049d`](https://github.com/kmnhan/erlabpy/commit/bd8049d1060791f5df22ef6b610fe26a700c14cc))
 
 * update minimum gradient documentation ([`a8df0f3`](https://github.com/kmnhan/erlabpy/commit/a8df0f3ba04e979f0a8d6fb9b2598c65b28767e1))
 
 ### Feature
 
-* **itool** add copy code to PlotItem vb menu ([`7b4f30a`](https://github.com/kmnhan/erlabpy/commit/7b4f30ada21c5accc1d3824ad3d0f8097f9a99c1))
+* (**itool**) add copy code to PlotItem vb menu ([`7b4f30a`](https://github.com/kmnhan/erlabpy/commit/7b4f30ada21c5accc1d3824ad3d0f8097f9a99c1))
 
   For each plot in imagetool, a new &#39;copy selection code&#39; button has been added to the right-click menu that copies the code that can slice the data to recreate the data shown in the plot.
 
 * add 2D curvature, finally closes #14 ([`7fe95ff`](https://github.com/kmnhan/erlabpy/commit/7fe95ffcdf0531e456cfc97ae605467e4ae433c0))
 
-* **plotting** add N argument to plot_array_2d ([`2cd79f7`](https://github.com/kmnhan/erlabpy/commit/2cd79f7ee007058da09aff244cd75748698444ee))
+* (**plotting**) add N argument to plot_array_2d ([`2cd79f7`](https://github.com/kmnhan/erlabpy/commit/2cd79f7ee007058da09aff244cd75748698444ee))
 
 * add scaled laplace ([`079e1d2`](https://github.com/kmnhan/erlabpy/commit/079e1d21201c7523877b06a0f04f7640027b0614))
 
 * add gaussian filter and laplacian ([`8628d33`](https://github.com/kmnhan/erlabpy/commit/8628d336ff5b4219e4fd382293736e4cbf026d56))
 
 * add derivative module with minimum gradient implementation ([`e0eabde`](https://github.com/kmnhan/erlabpy/commit/e0eabde60e6860c3827959b45be6d4f491918363))
 
 ### Fix
 
-* **dynamic** properly broadcast xarray input ([`2f6672f`](https://github.com/kmnhan/erlabpy/commit/2f6672f3b003792ecd98b4fbc99fb11fcc0efb8b))
+* (**dynamic**) properly broadcast xarray input ([`2f6672f`](https://github.com/kmnhan/erlabpy/commit/2f6672f3b003792ecd98b4fbc99fb11fcc0efb8b))
 
-* **fit.functions** polynomial function now works for xarray input ([`3eb80de`](https://github.com/kmnhan/erlabpy/commit/3eb80dea31b6414fa9a694049b92b7334a4e10f5))
+* (**fit.functions**) polynomial function now works for xarray input ([`3eb80de`](https://github.com/kmnhan/erlabpy/commit/3eb80dea31b6414fa9a694049b92b7334a4e10f5))
 
-* **analysis.image** remove critical typo ([`fb7de0f`](https://github.com/kmnhan/erlabpy/commit/fb7de0fc3ba9049c488a90bef8ee3c4feb935341))
+* (**analysis.image**) remove critical typo ([`fb7de0f`](https://github.com/kmnhan/erlabpy/commit/fb7de0fc3ba9049c488a90bef8ee3c4feb935341))
 
-* **analysis.image** dtype safety of cfunc ([`b4f9b17`](https://github.com/kmnhan/erlabpy/commit/b4f9b17656c64be4cff876843ed0f3491d8310d4))
+* (**analysis.image**) dtype safety of cfunc ([`b4f9b17`](https://github.com/kmnhan/erlabpy/commit/b4f9b17656c64be4cff876843ed0f3491d8310d4))
 
 * set autodownsample off for colorbar ([`256bf2d`](https://github.com/kmnhan/erlabpy/commit/256bf2dc8c368d093a3578d7f9279b1ee4653534))
 
 * disable itool downsample ([`e626bba`](https://github.com/kmnhan/erlabpy/commit/e626bba9fcd4fd31387ca3a07a9a33b7690f3645))
 
 ### Performance
 
-* **itool** add explicit signatures to fastbinning ([`62e1d51`](https://github.com/kmnhan/erlabpy/commit/62e1d516f0260f661fe9cd8f1fae9cb81afbcabe))
+* (**itool**) add explicit signatures to fastbinning ([`62e1d51`](https://github.com/kmnhan/erlabpy/commit/62e1d516f0260f661fe9cd8f1fae9cb81afbcabe))
 
   Speedup initial binning by providing explicit signatures.
 
 ### Refactor
 
 * update dtool to use new functions ([`a6e46bb`](https://github.com/kmnhan/erlabpy/commit/a6e46bb8b19512e438291afbbd5e0e9a4eb4fe87))
 
-* **analysis.image** add documentation and reorder functions ([`340665d`](https://github.com/kmnhan/erlabpy/commit/340665dc507a99acc7d56c46a2a2326fbb56b1e3))
+* (**analysis.image**) add documentation and reorder functions ([`340665d`](https://github.com/kmnhan/erlabpy/commit/340665dc507a99acc7d56c46a2a2326fbb56b1e3))
 
 * rename module to image and add citation ([`b74a654`](https://github.com/kmnhan/erlabpy/commit/b74a654e07d9f4522cee2db0b897f1ffcdb86e94))
 
-* **dtool** cleanup unused code ([`f4abd34`](https://github.com/kmnhan/erlabpy/commit/f4abd34bbf3130c0ec0fd2f9c830c8da43849f13))
+* (**dtool**) cleanup unused code ([`f4abd34`](https://github.com/kmnhan/erlabpy/commit/f4abd34bbf3130c0ec0fd2f9c830c8da43849f13))
 
-### Unknown
+### Tests
 
-* tests: reduce test time by specifying explicit path ([`60fb0d0`](https://github.com/kmnhan/erlabpy/commit/60fb0d0cedd9f0aaeca7101dddf0848f8872ccc3))
+* reduce test time by specifying explicit path ([`60fb0d0`](https://github.com/kmnhan/erlabpy/commit/60fb0d0cedd9f0aaeca7101dddf0848f8872ccc3))
 
-  
   This will not trigger directory recursion, so tests will run a bit faster
 
-* tests: add tests for fitting functions ([`4992251`](https://github.com/kmnhan/erlabpy/commit/499225149346e970d00b60dcb5ca39af5e5ddb47))
+* add tests for fitting functions ([`4992251`](https://github.com/kmnhan/erlabpy/commit/499225149346e970d00b60dcb5ca39af5e5ddb47))
 
-* tests: add tests for image and shift ([`7e4daeb`](https://github.com/kmnhan/erlabpy/commit/7e4daeb5aea9689aadfe3eedb561d313e217684c))
+* add tests for image and shift ([`7e4daeb`](https://github.com/kmnhan/erlabpy/commit/7e4daeb5aea9689aadfe3eedb561d313e217684c))
 
 
 ## v1.6.5 (2024-04-03)
 
 ### Fix
 
 * make imports work without optional pip dependencies ([`b8ac11d`](https://github.com/kmnhan/erlabpy/commit/b8ac11d8fb4379f70a39c817332382c352391a64))
@@ -136,25 +199,25 @@
 * igor2 does not have to be installed on import time ([`186727a`](https://github.com/kmnhan/erlabpy/commit/186727ac8d50b662efeba8bee567cf1013ca936a))
 
 
 ## v1.6.1 (2024-04-03)
 
 ### Chore
 
-* **deps** add pre-commit to dev dependency ([`3a2fccd`](https://github.com/kmnhan/erlabpy/commit/3a2fccd978d23d806d2088ebd9ef60c7a2b20902))
+* (**deps**) add pre-commit to dev dependency ([`3a2fccd`](https://github.com/kmnhan/erlabpy/commit/3a2fccd978d23d806d2088ebd9ef60c7a2b20902))
 
 * make csaps optional ([`db31b06`](https://github.com/kmnhan/erlabpy/commit/db31b064c1f46edef7743fdd1c3ab7984e170b3c))
 
 * update issue templates ([`dfc2ab0`](https://github.com/kmnhan/erlabpy/commit/dfc2ab0fdfcf1fd5ab83dac2c9d6473b4d2cb7e1))
 
 ### Ci
 
-* **github** remove linting, let pre-commit handle it ([`b209ecb`](https://github.com/kmnhan/erlabpy/commit/b209ecbb3c0a35d2bbeba8155bea3da9ffa58fe1))
+* (**github**) remove linting, let pre-commit handle it ([`b209ecb`](https://github.com/kmnhan/erlabpy/commit/b209ecbb3c0a35d2bbeba8155bea3da9ffa58fe1))
 
-* **pre-commit** add hooks ([`9b401c3`](https://github.com/kmnhan/erlabpy/commit/9b401c328bb3ff18dddcce40b935afa2b6e2624a))
+* (**pre-commit**) add hooks ([`9b401c3`](https://github.com/kmnhan/erlabpy/commit/9b401c328bb3ff18dddcce40b935afa2b6e2624a))
 
 ### Documentation
 
 * rephrase kconv guide ([`dd2c022`](https://github.com/kmnhan/erlabpy/commit/dd2c022e42e692c2af640a1fc8d21c3e429781b2))
 
 * add ipykernel dependency to resolve failing builds ([`e5774a5`](https://github.com/kmnhan/erlabpy/commit/e5774a51c14ef6df190eb9f6198c274d2061cdd5))
 
@@ -231,15 +294,14 @@
 
 * apply linter suggestions ([`7295cbc`](https://github.com/kmnhan/erlabpy/commit/7295cbc5b08065d75447f80ab1d84eb1c15255f3))
 
 ### Unknown
 
 * [pre-commit.ci] auto fixes from pre-commit.com hooks ([`b86c995`](https://github.com/kmnhan/erlabpy/commit/b86c9952be94b4b7f5e5918ed28cbf39b750ef09))
 
-  
   for more information, see https://pre-commit.ci
 
 
 ## v1.5.2 (2024-04-01)
 
 ### Documentation
 
@@ -423,19 +485,19 @@
 
 ### Documentation
 
 * update README ([`79ba5b4`](https://github.com/kmnhan/erlabpy/commit/79ba5b42f5089d9fd81ccfc69dadda21914b42a7))
 
 ### Feature
 
-* **io** add new data loader plugin for DA30 + SES ([`7a27a2f`](https://github.com/kmnhan/erlabpy/commit/7a27a2f27d9658f1091aaa48bcc78dea562898d8))
+* (**io**) add new data loader plugin for DA30 + SES ([`7a27a2f`](https://github.com/kmnhan/erlabpy/commit/7a27a2f27d9658f1091aaa48bcc78dea562898d8))
 
 ### Fix
 
-* **io** properly handle registry getattr ([`499526f`](https://github.com/kmnhan/erlabpy/commit/499526fc1705bfbfbf8d3b80d50d65450dec7eae))
+* (**io**) properly handle registry getattr ([`499526f`](https://github.com/kmnhan/erlabpy/commit/499526fc1705bfbfbf8d3b80d50d65450dec7eae))
 
   This fixes an issue where _repr_html_ will fallback to __repr__. Additionally, `get` will now raise a KeyError instead of a ValueError.
 
 ### Style
 
 * adjust loader registry repr ([`1fc31af`](https://github.com/kmnhan/erlabpy/commit/1fc31af083654a6c093bf343a881fcab37f9fbe2))
 
@@ -592,15 +654,15 @@
 
 * update documentation ([`fa312c0`](https://github.com/kmnhan/erlabpy/commit/fa312c05cc9dabb858d9268808b3efd2bead1a3e))
 
 * update documentation ([`2e4e573`](https://github.com/kmnhan/erlabpy/commit/2e4e5736cec670f51e55e81db603c82b98a9e78b))
 
 * add some comments ([`e66bc31`](https://github.com/kmnhan/erlabpy/commit/e66bc31cd9f9905a16a94f3b491170556b29adbc))
 
-* **itool** improve tooltip ([`97ad19b`](https://github.com/kmnhan/erlabpy/commit/97ad19b1581613b6eb7012d4e04d79209f12075d))
+* (**itool**) improve tooltip ([`97ad19b`](https://github.com/kmnhan/erlabpy/commit/97ad19b1581613b6eb7012d4e04d79209f12075d))
 
 * update docstring ([`700a9a3`](https://github.com/kmnhan/erlabpy/commit/700a9a3982ddcd16756efacb53bd5be861f7ed18))
 
 * update documentation ([`e12b9af`](https://github.com/kmnhan/erlabpy/commit/e12b9afc1750823db4edb8034f4b225e51460cca))
 
 * update docstring and formatting ([`dc8e544`](https://github.com/kmnhan/erlabpy/commit/dc8e54415fd26090782075847fd78fa942f7efca))
 
@@ -648,79 +710,79 @@
 
 * update docstring ([`ee31e1f`](https://github.com/kmnhan/erlabpy/commit/ee31e1fe997c245981057c59a602fe1b7a253501))
 
 * update docstring ([`b32e92f`](https://github.com/kmnhan/erlabpy/commit/b32e92f0cee5c5aa2b7793a17d95c21ff49ce94d))
 
 ### Feature
 
-* **gold** apply automatic weights proportional to sqrt(count) on edge fit ([`717b9c8`](https://github.com/kmnhan/erlabpy/commit/717b9c814ce6fd38567695adb515973e6097ec50))
+* (**gold**) apply automatic weights proportional to sqrt(count) on edge fit ([`717b9c8`](https://github.com/kmnhan/erlabpy/commit/717b9c814ce6fd38567695adb515973e6097ec50))
 
 * add class to handle momentum conversion offsets ([`15416e5`](https://github.com/kmnhan/erlabpy/commit/15416e5aeca748225e35659c65dcc07b82b40007))
 
 * add translation layer between lmfit models and iminuit ([`0f2f894`](https://github.com/kmnhan/erlabpy/commit/0f2f894994a00714e50e934dd4d5b518540539df))
 
 * include all cmaps by default ([`3afe72e`](https://github.com/kmnhan/erlabpy/commit/3afe72ece2474c9adcfb89cb5037c50af2e2f0e5))
 
 * change default colormap to CET-L20 ([`274122a`](https://github.com/kmnhan/erlabpy/commit/274122a4b2e582a24385c4dd748206ae0165b4b8))
 
-* **goldtool** can access fit result after window close ([`4c9f232`](https://github.com/kmnhan/erlabpy/commit/4c9f232adfde874d975f033dc9bdcc8bf4969787))
+* (**goldtool**) can access fit result after window close ([`4c9f232`](https://github.com/kmnhan/erlabpy/commit/4c9f232adfde874d975f033dc9bdcc8bf4969787))
 
-* **io** style summary ([`6919929`](https://github.com/kmnhan/erlabpy/commit/6919929815401aa5d6ee4a37398c0593fab3657d))
+* (**io**) style summary ([`6919929`](https://github.com/kmnhan/erlabpy/commit/6919929815401aa5d6ee4a37398c0593fab3657d))
 
-* **io** summarize will now default to set directory ([`ca5b65a`](https://github.com/kmnhan/erlabpy/commit/ca5b65a0e850058837945b7f53864cfc6b32e933))
+* (**io**) summarize will now default to set directory ([`ca5b65a`](https://github.com/kmnhan/erlabpy/commit/ca5b65a0e850058837945b7f53864cfc6b32e933))
 
-* **constants** add neutron mass ([`379ef37`](https://github.com/kmnhan/erlabpy/commit/379ef3705eb2f952121c92c9b653f2ca715618ee))
+* (**constants**) add neutron mass ([`379ef37`](https://github.com/kmnhan/erlabpy/commit/379ef3705eb2f952121c92c9b653f2ca715618ee))
 
-* **io** make loaders accessible with __getattr__ ([`b4884e4`](https://github.com/kmnhan/erlabpy/commit/b4884e4989c3565fdeccb8e18ec6a840cc67a7d2))
+* (**io**) make loaders accessible with __getattr__ ([`b4884e4`](https://github.com/kmnhan/erlabpy/commit/b4884e4989c3565fdeccb8e18ec6a840cc67a7d2))
 
-* **io** add loader plugin for SSRL Beamline 5-2 ([`67ced64`](https://github.com/kmnhan/erlabpy/commit/67ced64352e0f071fad5ebe441348108b6834784))
+* (**io**) add loader plugin for SSRL Beamline 5-2 ([`67ced64`](https://github.com/kmnhan/erlabpy/commit/67ced64352e0f071fad5ebe441348108b6834784))
 
-* **io** show full table on summary in ipython ([`985046f`](https://github.com/kmnhan/erlabpy/commit/985046f8a13911dc2c0be7cc68e530e93de37683))
+* (**io**) show full table on summary in ipython ([`985046f`](https://github.com/kmnhan/erlabpy/commit/985046f8a13911dc2c0be7cc68e530e93de37683))
 
-* **io.dataloader** allow loaders to specify mapping dictionary on cut postprocessing ([`73abb0d`](https://github.com/kmnhan/erlabpy/commit/73abb0d1a078779130e6f82fadc9f44e62619799))
+* (**io.dataloader**) allow loaders to specify mapping dictionary on cut postprocessing ([`73abb0d`](https://github.com/kmnhan/erlabpy/commit/73abb0d1a078779130e6f82fadc9f44e62619799))
 
-* **io** new arg to get_files ([`a9be216`](https://github.com/kmnhan/erlabpy/commit/a9be2165b61082956d5118c328e6484bdd0694c5))
+* (**io**) new arg to get_files ([`a9be216`](https://github.com/kmnhan/erlabpy/commit/a9be2165b61082956d5118c328e6484bdd0694c5))
 
-* **io.igor** remove dependency on find_first_file ([`1d95292`](https://github.com/kmnhan/erlabpy/commit/1d95292ff4ba1c6ad5fcc95cae2d36c452d52ecf))
+* (**io.igor**) remove dependency on find_first_file ([`1d95292`](https://github.com/kmnhan/erlabpy/commit/1d95292ff4ba1c6ad5fcc95cae2d36c452d52ecf))
 
-* **io** dataloader now preserves more attributes ([`f1157ba`](https://github.com/kmnhan/erlabpy/commit/f1157ba7afcb0b259932062edb0dc2138c749c55))
+* (**io**) dataloader now preserves more attributes ([`f1157ba`](https://github.com/kmnhan/erlabpy/commit/f1157ba7afcb0b259932062edb0dc2138c749c55))
 
-* **io** new data loader! ([`6c85cba`](https://github.com/kmnhan/erlabpy/commit/6c85cba810936403734cfeefa65b005e2d2e329e))
+* (**io**) new data loader! ([`6c85cba`](https://github.com/kmnhan/erlabpy/commit/6c85cba810936403734cfeefa65b005e2d2e329e))
 
   Implemented  new class-based data loader. Currently only implemented for ALS BL4.0.3.
 
-* **io** add new utility function ([`a27a9f8`](https://github.com/kmnhan/erlabpy/commit/a27a9f89ce56b35a7a35fd1014c01269378a8148))
+* (**io**) add new utility function ([`a27a9f8`](https://github.com/kmnhan/erlabpy/commit/a27a9f89ce56b35a7a35fd1014c01269378a8148))
 
-* **igor** remove attribute renaming, keep original attribute as much as possible ([`912376c`](https://github.com/kmnhan/erlabpy/commit/912376c0216c901e85dd68b03817cbc8b85522a7))
+* (**igor**) remove attribute renaming, keep original attribute as much as possible ([`912376c`](https://github.com/kmnhan/erlabpy/commit/912376c0216c901e85dd68b03817cbc8b85522a7))
 
 * show elapsed time for momentum conversion ([`8889737`](https://github.com/kmnhan/erlabpy/commit/8889737aa6a8c5da2ef2ba17e5201816c99c574b))
 
 * add sample data generation in angles ([`1d2600d`](https://github.com/kmnhan/erlabpy/commit/1d2600d37b7fe323adb016a1daf2b9811d6f4593))
 
-* **constants** add electron rest energy mc^2 ([`8e46445`](https://github.com/kmnhan/erlabpy/commit/8e46445efd3fa5fe623e2ab65ee939039b4dc149))
+* (**constants**) add electron rest energy mc^2 ([`8e46445`](https://github.com/kmnhan/erlabpy/commit/8e46445efd3fa5fe623e2ab65ee939039b4dc149))
 
-* **ktool** full kz support ([`c3284f7`](https://github.com/kmnhan/erlabpy/commit/c3284f785484b5f506bd2025afa57661ac947eec))
+* (**ktool**) full kz support ([`c3284f7`](https://github.com/kmnhan/erlabpy/commit/c3284f785484b5f506bd2025afa57661ac947eec))
 
   Added inner potential spinbox and projected BZ overlay
 
-* **bz** add BZ extending ([`cbbb11a`](https://github.com/kmnhan/erlabpy/commit/cbbb11ac8997951cda17ec976fe321b8699d1eff))
+* (**bz**) add BZ extending ([`cbbb11a`](https://github.com/kmnhan/erlabpy/commit/cbbb11ac8997951cda17ec976fe321b8699d1eff))
 
-* **itool** allow different label maximum widths ([`3467ae1`](https://github.com/kmnhan/erlabpy/commit/3467ae1720363ebfc026e3f5fc4f9517a342a448))
+* (**itool**) allow different label maximum widths ([`3467ae1`](https://github.com/kmnhan/erlabpy/commit/3467ae1720363ebfc026e3f5fc4f9517a342a448))
 
   The controls took up too much space if one of the dim names was long
 
 * change transpose button order for 4D data ([`018002c`](https://github.com/kmnhan/erlabpy/commit/018002cd5606a091a528f866b2edcff051ce7570))
 
 * add support for automatic cut and hv-dependent momentum conversion ([`f5be05f`](https://github.com/kmnhan/erlabpy/commit/f5be05fb80a4e5dc4f2b976e8894bddc07d43d91))
 
 * add bz masking function ([`f3a7d21`](https://github.com/kmnhan/erlabpy/commit/f3a7d21c44784e4191011e8e95202889afc15ccc))
 
-* **interpolate** add more checks and warnings ([`f1c223f`](https://github.com/kmnhan/erlabpy/commit/f1c223fbce27d65ed196fafd196c8b9c28d978dd))
+* (**interpolate**) add more checks and warnings ([`f1c223f`](https://github.com/kmnhan/erlabpy/commit/f1c223fbce27d65ed196fafd196c8b9c28d978dd))
 
-* **ktool** frontend tweaks ([`d0050d0`](https://github.com/kmnhan/erlabpy/commit/d0050d02270c5ad8e51af281cb7a9f7a1cb89913))
+* (**ktool**) frontend tweaks ([`d0050d0`](https://github.com/kmnhan/erlabpy/commit/d0050d02270c5ad8e51af281cb7a9f7a1cb89913))
 
   Added wait dialog for showing imagetool and make labels prettier
 
 * add new momentum conversion tool ([`dfa96fe`](https://github.com/kmnhan/erlabpy/commit/dfa96fe9f20b57699d43d3d23755c663c3793d30))
 
 * implement new momentum conversion functions. Currently only supports kxky and kxkyE conversion. ([`956a0bd`](https://github.com/kmnhan/erlabpy/commit/956a0bd8e034754d0b208a7c654d77e690491b98))
 
@@ -730,321 +792,321 @@
 
 * misc. changes to momentum conversion tool ([`1221fd0`](https://github.com/kmnhan/erlabpy/commit/1221fd0403977b840e650221111ae3a72a69cb65))
 
 * load new resistance data ([`782cdf8`](https://github.com/kmnhan/erlabpy/commit/782cdf82c8b6b12d15c3f964dfe4a924131e5d4a))
 
 * add spline module (work in progress) ([`69f8e4c`](https://github.com/kmnhan/erlabpy/commit/69f8e4c60cd147fc677f27aee927607153db3ac6))
 
-* **goldtool** scale roi initial position to data ([`65f71d2`](https://github.com/kmnhan/erlabpy/commit/65f71d2c3ec1888f8e8fecb84b0e98189859f191))
+* (**goldtool**) scale roi initial position to data ([`65f71d2`](https://github.com/kmnhan/erlabpy/commit/65f71d2c3ec1888f8e8fecb84b0e98189859f191))
 
-* **goldtool** add remaining time to progress bar ([`348aaf7`](https://github.com/kmnhan/erlabpy/commit/348aaf7acde9421156bb6027bc0853a4142f166f))
+* (**goldtool**) add remaining time to progress bar ([`348aaf7`](https://github.com/kmnhan/erlabpy/commit/348aaf7acde9421156bb6027bc0853a4142f166f))
 
 * add atom plotting module ([`2fcf012`](https://github.com/kmnhan/erlabpy/commit/2fcf012c2866b598a82741961b9ad29602a63748))
 
 * minor tweaks to mplstyle ([`10972b8`](https://github.com/kmnhan/erlabpy/commit/10972b8f70c041835d0c8274448e53be67172d18))
 
 * add crop to  plot_array ([`36d8536`](https://github.com/kmnhan/erlabpy/commit/36d85366ffd1c84298df79d6721b26f17d8cf031))
 
-* **colors** make axes not required for nice_colorbar ([`48af74b`](https://github.com/kmnhan/erlabpy/commit/48af74b45e926f5ff9f2c0c717d27d05987837b8))
+* (**colors**) make axes not required for nice_colorbar ([`48af74b`](https://github.com/kmnhan/erlabpy/commit/48af74b45e926f5ff9f2c0c717d27d05987837b8))
 
-* **goldtool** add diffev to list of methods ([`d21c915`](https://github.com/kmnhan/erlabpy/commit/d21c915f7993c66f1a79dc7cfa28b06b63cc89f8))
+* (**goldtool**) add diffev to list of methods ([`d21c915`](https://github.com/kmnhan/erlabpy/commit/d21c915f7993c66f1a79dc7cfa28b06b63cc89f8))
 
-* **itool** plot class customization ([`fee3913`](https://github.com/kmnhan/erlabpy/commit/fee39133c4208e7733a18b31d77a7898ac4b5713))
+* (**itool**) plot class customization ([`fee3913`](https://github.com/kmnhan/erlabpy/commit/fee39133c4208e7733a18b31d77a7898ac4b5713))
 
 * better cache management for slicer ([`9f49374`](https://github.com/kmnhan/erlabpy/commit/9f49374ee98fb2cc101974292d959ee0f6898a9a))
 
-* **betterspinbox** make keyboardTracking off by default ([`753ddcd`](https://github.com/kmnhan/erlabpy/commit/753ddcd344ff6859ff44cecaff4fb641e4e981dd))
+* (**betterspinbox**) make keyboardTracking off by default ([`753ddcd`](https://github.com/kmnhan/erlabpy/commit/753ddcd344ff6859ff44cecaff4fb641e4e981dd))
 
-* **annotation** add axis unit scaling ([`a61b8f3`](https://github.com/kmnhan/erlabpy/commit/a61b8f38165828d3f118c682cbfe05325c413e22))
+* (**annotation**) add axis unit scaling ([`a61b8f3`](https://github.com/kmnhan/erlabpy/commit/a61b8f38165828d3f118c682cbfe05325c413e22))
 
-* **itool** add option to decouple colors ([`3e2f132`](https://github.com/kmnhan/erlabpy/commit/3e2f1325baa1011540b29f1f36fd8b12a7770114))
+* (**itool**) add option to decouple colors ([`3e2f132`](https://github.com/kmnhan/erlabpy/commit/3e2f1325baa1011540b29f1f36fd8b12a7770114))
 
-* **style** update poster style ([`da58226`](https://github.com/kmnhan/erlabpy/commit/da582267a69fea8efb86e93478c398d70c7e411c))
+* (**style**) update poster style ([`da58226`](https://github.com/kmnhan/erlabpy/commit/da582267a69fea8efb86e93478c398d70c7e411c))
 
-* **accessor** use pyarpes for 2d kconv ([`9cbe422`](https://github.com/kmnhan/erlabpy/commit/9cbe422d19bb95e17a13b4757b8239d08069d850))
+* (**accessor**) use pyarpes for 2d kconv ([`9cbe422`](https://github.com/kmnhan/erlabpy/commit/9cbe422d19bb95e17a13b4757b8239d08069d850))
 
 * improve extendability ([`ded8841`](https://github.com/kmnhan/erlabpy/commit/ded884139e25cea9549fd3e3e7b0519c03b1d447))
 
-* **itool** pass parent ([`c8feac4`](https://github.com/kmnhan/erlabpy/commit/c8feac43871fba3a0c12db56d33c819efdfd3e41))
+* (**itool**) pass parent ([`c8feac4`](https://github.com/kmnhan/erlabpy/commit/c8feac43871fba3a0c12db56d33c819efdfd3e41))
 
-* **itool** add base imagetool with only controls ([`fdb8a6b`](https://github.com/kmnhan/erlabpy/commit/fdb8a6b0e52f83c05441d03a06bd15d83b8a261a))
+* (**itool**) add base imagetool with only controls ([`fdb8a6b`](https://github.com/kmnhan/erlabpy/commit/fdb8a6b0e52f83c05441d03a06bd15d83b8a261a))
 
 * add option to return individual regions ([`7c5b081`](https://github.com/kmnhan/erlabpy/commit/7c5b08181f0cfc6d727fafe6a8789ec952ac895f))
 
-* **colors** add function to unify color limits ([`33d571f`](https://github.com/kmnhan/erlabpy/commit/33d571f4dfcdecec02d536f5f5a4cd9af349d2df))
+* (**colors**) add function to unify color limits ([`33d571f`](https://github.com/kmnhan/erlabpy/commit/33d571f4dfcdecec02d536f5f5a4cd9af349d2df))
 
-* **colors** add function that combines colormaps ([`f19d87c`](https://github.com/kmnhan/erlabpy/commit/f19d87ca5c3de53ca8623d7954a280b7050f2d15))
+* (**colors**) add function that combines colormaps ([`f19d87c`](https://github.com/kmnhan/erlabpy/commit/f19d87ca5c3de53ca8623d7954a280b7050f2d15))
 
 * add new colormap! ([`474ad52`](https://github.com/kmnhan/erlabpy/commit/474ad521c3c5726341c17b9b4759ee501661ce73))
 
 * k range freedom in sample data generation ([`9dd5b00`](https://github.com/kmnhan/erlabpy/commit/9dd5b0025aaf52ef0bf4685ef5e380ccd5a72ac4))
 
 * make BZ plotter standalone ([`3bec642`](https://github.com/kmnhan/erlabpy/commit/3bec64218de70cabf8a43b78bf6728bef6402b49))
 
-* **igorinterface** add to load wave menu ([`da704c5`](https://github.com/kmnhan/erlabpy/commit/da704c5c083a41db3999b031a5676bb69e33f46a))
+* (**igorinterface**) add to load wave menu ([`da704c5`](https://github.com/kmnhan/erlabpy/commit/da704c5c083a41db3999b031a5676bb69e33f46a))
 
-* **io** add DA30 loader ([`9afd149`](https://github.com/kmnhan/erlabpy/commit/9afd149ddfb21a64564f4d9d2bb1ccb6dcd6d808))
+* (**io**) add DA30 loader ([`9afd149`](https://github.com/kmnhan/erlabpy/commit/9afd149ddfb21a64564f4d9d2bb1ccb6dcd6d808))
 
-* **goldtool** add fit abort ([`693b1e4`](https://github.com/kmnhan/erlabpy/commit/693b1e474ebbc4989dba6ed900f85cad62b5cfcc))
+* (**goldtool**) add fit abort ([`693b1e4`](https://github.com/kmnhan/erlabpy/commit/693b1e474ebbc4989dba6ed900f85cad62b5cfcc))
 
 * pass kwargs to broadcast_model ([`82d11f2`](https://github.com/kmnhan/erlabpy/commit/82d11f24b6412f8c774264f5941863eaff7cef6b))
 
 * autolevel colorbar ([`f116155`](https://github.com/kmnhan/erlabpy/commit/f1161551fbf4665b65287d27a2312b3b052c1948))
 
 * set colorbar width ([`b13b5d2`](https://github.com/kmnhan/erlabpy/commit/b13b5d2abd89e98bee6e55d5aeba135a16b3fb50))
 
-* **gold** fully integrate spline fitting ([`d5b345c`](https://github.com/kmnhan/erlabpy/commit/d5b345cb5efc6e1e889c272d437e646935ff12e1))
+* (**gold**) fully integrate spline fitting ([`d5b345c`](https://github.com/kmnhan/erlabpy/commit/d5b345cb5efc6e1e889c272d437e646935ff12e1))
 
 * add lattice module ([`bafe36b`](https://github.com/kmnhan/erlabpy/commit/bafe36b7ab89f004f7ac0ac1d4aa2d1b5137698a))
 
 * estimate k resolution from data ([`457edc7`](https://github.com/kmnhan/erlabpy/commit/457edc72ffa755ffc2e8d3fee039df97bab53ae0))
 
 * add kspace conversion accessor ([`56da9e0`](https://github.com/kmnhan/erlabpy/commit/56da9e09c0dedc9cb066fbd641b5a92eca5b8635))
 
-* **itool** save individual plot as hdf5 ([`a5a88b9`](https://github.com/kmnhan/erlabpy/commit/a5a88b9402b5d538386547083b8d7dcc2335e032))
+* (**itool**) save individual plot as hdf5 ([`a5a88b9`](https://github.com/kmnhan/erlabpy/commit/a5a88b9402b5d538386547083b8d7dcc2335e032))
 
 * add ZT image view for 4D ([`bf66dfb`](https://github.com/kmnhan/erlabpy/commit/bf66dfbc948bbf585dde392b23b0e5586b2a1d35))
 
 * add igor procedure to load dataarrays ([`f8b93e0`](https://github.com/kmnhan/erlabpy/commit/f8b93e0e79adc6052e577304dd856a146de0c521))
 
-* **itool** enable sync across multiple windows! ([`d3a5056`](https://github.com/kmnhan/erlabpy/commit/d3a50561bd38c9040b9aae3b6c1b82453df1423b))
+* (**itool**) enable sync across multiple windows! ([`d3a5056`](https://github.com/kmnhan/erlabpy/commit/d3a50561bd38c9040b9aae3b6c1b82453df1423b))
 
-* **gold** automatic crop for corrected gold ([`dad4bb8`](https://github.com/kmnhan/erlabpy/commit/dad4bb886799fd11d5ecf6c8c18c4a118858d15f))
+* (**gold**) automatic crop for corrected gold ([`dad4bb8`](https://github.com/kmnhan/erlabpy/commit/dad4bb886799fd11d5ecf6c8c18c4a118858d15f))
 
-* **io** improve BL4 data loading, add basic log generator ([`e283262`](https://github.com/kmnhan/erlabpy/commit/e283262f138bc509d9f4481efd835626060f8b62))
+* (**io**) improve BL4 data loading, add basic log generator ([`e283262`](https://github.com/kmnhan/erlabpy/commit/e283262f138bc509d9f4481efd835626060f8b62))
 
-* **interp** improve interpolator syntax ([`c7b322b`](https://github.com/kmnhan/erlabpy/commit/c7b322b6bf4106320270b39b4aa423d94ffa94be))
+* (**interp**) improve interpolator syntax ([`c7b322b`](https://github.com/kmnhan/erlabpy/commit/c7b322b6bf4106320270b39b4aa423d94ffa94be))
 
-* **gold** configurable covariance matrix scaling ([`d051864`](https://github.com/kmnhan/erlabpy/commit/d051864da1dd2e3f5101d33743fa04720fab5411))
+* (**gold**) configurable covariance matrix scaling ([`d051864`](https://github.com/kmnhan/erlabpy/commit/d051864da1dd2e3f5101d33743fa04720fab5411))
 
-* **fit** add step function edge ([`3a7bc03`](https://github.com/kmnhan/erlabpy/commit/3a7bc03c666a946813ce79e95002475efb446046))
+* (**fit**) add step function edge ([`3a7bc03`](https://github.com/kmnhan/erlabpy/commit/3a7bc03c666a946813ce79e95002475efb446046))
 
 * handle rad2deg automatically ([`aea4a62`](https://github.com/kmnhan/erlabpy/commit/aea4a62d047cca0be231e0256ad3f519ef54eb0e))
 
-* **bz** add option for clip path ([`52daa2a`](https://github.com/kmnhan/erlabpy/commit/52daa2afa4fe98acb1c5ac39dfe6362d348d2e11))
+* (**bz**) add option for clip path ([`52daa2a`](https://github.com/kmnhan/erlabpy/commit/52daa2afa4fe98acb1c5ac39dfe6362d348d2e11))
 
 * add fast trilinear interpolation ([`ae77bee`](https://github.com/kmnhan/erlabpy/commit/ae77bee8050b3a80e5ab24bef447911d2e6a4ccd))
 
-* **io** add function for pxp debugging ([`1802e09`](https://github.com/kmnhan/erlabpy/commit/1802e099689062bf7e7f531b726ea8ce7ada91e0))
+* (**io**) add function for pxp debugging ([`1802e09`](https://github.com/kmnhan/erlabpy/commit/1802e099689062bf7e7f531b726ea8ce7ada91e0))
 
 * add W to ph/s conversion ([`a64039d`](https://github.com/kmnhan/erlabpy/commit/a64039d3ca2971b5a434a451fc8e956e40fa2e9b))
 
 * add 2D fermi edge fitting function ([`90c65de`](https://github.com/kmnhan/erlabpy/commit/90c65de986074dcce3ba658a0ec9ce1581da1dd2))
 
-* **itool** keep manual limits under transpose ([`bdec7e5`](https://github.com/kmnhan/erlabpy/commit/bdec7e5abe935072f91570af9fc58bb2f19582cb))
+* (**itool**) keep manual limits under transpose ([`bdec7e5`](https://github.com/kmnhan/erlabpy/commit/bdec7e5abe935072f91570af9fc58bb2f19582cb))
 
 * add more colortables from igor ([`03a615f`](https://github.com/kmnhan/erlabpy/commit/03a615f2ffbbf522bc8421757b7def3db037eab4))
 
 * add interactive brillouin zone plot ([`85f844f`](https://github.com/kmnhan/erlabpy/commit/85f844f5f7461489f924f8cf5096416791dec525))
 
 * update style files ([`5278c6c`](https://github.com/kmnhan/erlabpy/commit/5278c6c04213ce4230797bc34028d8befa2923af))
 
 * modernize plot_array ([`c5e7321`](https://github.com/kmnhan/erlabpy/commit/c5e7321dbbc124ae99d55b3959c020f59b1a2b7d))
 
-* **io** igor-compatible output ([`2a654e2`](https://github.com/kmnhan/erlabpy/commit/2a654e26fb0e53f79b705bb62db437f5d16e5735))
+* (**io**) igor-compatible output ([`2a654e2`](https://github.com/kmnhan/erlabpy/commit/2a654e26fb0e53f79b705bb62db437f5d16e5735))
 
-* **io** rewrite igor related backend ([`8739bef`](https://github.com/kmnhan/erlabpy/commit/8739befc3f30661e4d2ffd680888c3b06f3230cb))
+* (**io**) rewrite igor related backend ([`8739bef`](https://github.com/kmnhan/erlabpy/commit/8739befc3f30661e4d2ffd680888c3b06f3230cb))
 
 * polynomial model now takes positional args ([`a3000d5`](https://github.com/kmnhan/erlabpy/commit/a3000d55eca86fe2c1c1d8f7d468ab4051ceef08))
 
-* **goldtool** add smoothing spline fit ([`b25cd7c`](https://github.com/kmnhan/erlabpy/commit/b25cd7c19ced68c028f63cd3fbac533ae7a026b3))
+* (**goldtool**) add smoothing spline fit ([`b25cd7c`](https://github.com/kmnhan/erlabpy/commit/b25cd7c19ced68c028f63cd3fbac533ae7a026b3))
 
-* **itool** add performance benchmarks ([`9634af0`](https://github.com/kmnhan/erlabpy/commit/9634af0232afbf7f845b9694a03739b9111d516f))
+* (**itool**) add performance benchmarks ([`9634af0`](https://github.com/kmnhan/erlabpy/commit/9634af0232afbf7f845b9694a03739b9111d516f))
 
 * default cmap for analysis is now terrain ([`c1cc21c`](https://github.com/kmnhan/erlabpy/commit/c1cc21c2e7660245d1d0bcd1c3e4a5f45b757e15))
 
 * example dataset generator ([`6b6cadf`](https://github.com/kmnhan/erlabpy/commit/6b6cadf19d536dea990daacd687739953a33a2d1))
 
 * add curve fitting tool (alpha) ([`68356ab`](https://github.com/kmnhan/erlabpy/commit/68356ab6d7fc4ecb6653d36213acc8c22ef4f23b))
 
 * add new module for curve fitting ([`20c8be9`](https://github.com/kmnhan/erlabpy/commit/20c8be92116a0ce95f1dd55a2de131a1a9a16efe))
 
 * added boltzmann const. at constants ([`038930e`](https://github.com/kmnhan/erlabpy/commit/038930ebd9a48c000990c006ca794f8fc34b3d94))
 
 * add module for 3D plotting ([`4ec1bd2`](https://github.com/kmnhan/erlabpy/commit/4ec1bd2c81b17c775321d7b8197fe7ca84f1d03b))
 
-* **itool** add copy index action ([`6f25677`](https://github.com/kmnhan/erlabpy/commit/6f25677d2ba5d8cf1172a937d3370f67a7220781))
+* (**itool**) add copy index action ([`6f25677`](https://github.com/kmnhan/erlabpy/commit/6f25677d2ba5d8cf1172a937d3370f67a7220781))
 
 * parallelize multidimensional mean ([`7cfae81`](https://github.com/kmnhan/erlabpy/commit/7cfae816761e3169d1eb52b24d7adbbe8aeef848))
 
 * add 2D colormap ([`f5799d8`](https://github.com/kmnhan/erlabpy/commit/f5799d8d389ddf9c8cb03d7bfd05e9daa5331de0))
 
-* **itool** intuitive transpose for 4D data ([`38315f8`](https://github.com/kmnhan/erlabpy/commit/38315f83f98fa92313c8f7857c5b100f1b6f4fed))
+* (**itool**) intuitive transpose for 4D data ([`38315f8`](https://github.com/kmnhan/erlabpy/commit/38315f83f98fa92313c8f7857c5b100f1b6f4fed))
 
-* **polygon** add convenience function ([`a9e64c7`](https://github.com/kmnhan/erlabpy/commit/a9e64c7213952754c2ad70c2f7b92c73a4a1a45d))
+* (**polygon**) add convenience function ([`a9e64c7`](https://github.com/kmnhan/erlabpy/commit/a9e64c7213952754c2ad70c2f7b92c73a4a1a45d))
 
 * gradient fill under line plot ([`6a951c1`](https://github.com/kmnhan/erlabpy/commit/6a951c10060d454c8f5335d9081d1764881d1fc2))
 
 * plot 1D slices ([`36dee17`](https://github.com/kmnhan/erlabpy/commit/36dee178b9ffaa37216f74a4bf7810ff3021354c))
 
-* **io** add convenience function for BL4 data loading ([`0f3a4ea`](https://github.com/kmnhan/erlabpy/commit/0f3a4eac22e4738fe860117c6474bdab7923b959))
+* (**io**) add convenience function for BL4 data loading ([`0f3a4ea`](https://github.com/kmnhan/erlabpy/commit/0f3a4eac22e4738fe860117c6474bdab7923b959))
 
 * add igor colormaps ([`4bfcceb`](https://github.com/kmnhan/erlabpy/commit/4bfcceb8cca35df3fcb775743f73b127a7c48239))
 
 * new module for some common constants ([`c6aaede`](https://github.com/kmnhan/erlabpy/commit/c6aaede496725cb59548e26fff45f933f71883da))
 
 * update erplot ([`4bdbc10`](https://github.com/kmnhan/erlabpy/commit/4bdbc10e9556105df9f0250aeb1554ea3b862581))
 
 * add some annotations ([`4a37666`](https://github.com/kmnhan/erlabpy/commit/4a37666dcbd732f8c14c95c2ac1a2c24dee46e3b))
 
-* **io** add load functions ([`c654c44`](https://github.com/kmnhan/erlabpy/commit/c654c4444fd78ae64222b25559a881bdca1b6321))
+* (**io**) add load functions ([`c654c44`](https://github.com/kmnhan/erlabpy/commit/c654c4444fd78ae64222b25559a881bdca1b6321))
 
-* **itool** copy cursor position ([`cc39829`](https://github.com/kmnhan/erlabpy/commit/cc398299fb1d25ac1164a216cf68f68ec2e80555))
+* (**itool**) copy cursor position ([`cc39829`](https://github.com/kmnhan/erlabpy/commit/cc398299fb1d25ac1164a216cf68f68ec2e80555))
 
 * attempt better colorbar... this is probably stupid, fix later ([`2b26a3c`](https://github.com/kmnhan/erlabpy/commit/2b26a3c12e52c11d0468fa1268611b58ecf82b19))
 
 * fast peak fitting with broadened step edge ([`dc30094`](https://github.com/kmnhan/erlabpy/commit/dc300944a2ec0f25e0e4f16540b1edb42af0b154))
 
 * AxisItem scientific labeling ([`42b8860`](https://github.com/kmnhan/erlabpy/commit/42b8860a722dc4e20206b835e7fccb926975c460))
 
 * add diverging colormap normalizations ([`b085946`](https://github.com/kmnhan/erlabpy/commit/b085946ab554c6a4aaef19b4aa13d1071114dc3b))
 
-* **itool** add working colorbar ([`c326727`](https://github.com/kmnhan/erlabpy/commit/c326727c126c5081f1d7e60c2ce806699b8fb36f))
+* (**itool**) add working colorbar ([`c326727`](https://github.com/kmnhan/erlabpy/commit/c326727c126c5081f1d7e60c2ce806699b8fb36f))
 
-* **itool** full support for non-uniform coords ([`d3eface`](https://github.com/kmnhan/erlabpy/commit/d3eface36de9c15d788ab479d0f0a6860b36c9c8))
+* (**itool**) full support for non-uniform coords ([`d3eface`](https://github.com/kmnhan/erlabpy/commit/d3eface36de9c15d788ab479d0f0a6860b36c9c8))
 
-* **itool** auto-convert non-uniform dimensions to indices ([`1ad940d`](https://github.com/kmnhan/erlabpy/commit/1ad940d8bbc2b430cc54b7d9228ddc87e5235432))
+* (**itool**) auto-convert non-uniform dimensions to indices ([`1ad940d`](https://github.com/kmnhan/erlabpy/commit/1ad940d8bbc2b430cc54b7d9228ddc87e5235432))
 
-* **bz** add brillouin zone edge calculation ([`2b70d91`](https://github.com/kmnhan/erlabpy/commit/2b70d91ec8c77c27117637c1fec906a7a06c9571))
+* (**bz**) add brillouin zone edge calculation ([`2b70d91`](https://github.com/kmnhan/erlabpy/commit/2b70d91ec8c77c27117637c1fec906a7a06c9571))
 
-* **colors** add higher contrast PowerNorm ([`16b965c`](https://github.com/kmnhan/erlabpy/commit/16b965c224691103aabcfbb41c73524eb6b2244f))
+* (**colors**) add higher contrast PowerNorm ([`16b965c`](https://github.com/kmnhan/erlabpy/commit/16b965c224691103aabcfbb41c73524eb6b2244f))
 
-* **itool** add file open dialog ([`ba50354`](https://github.com/kmnhan/erlabpy/commit/ba5035491fa87ab44103d7041a81e15dee7a029e))
+* (**itool**) add file open dialog ([`ba50354`](https://github.com/kmnhan/erlabpy/commit/ba5035491fa87ab44103d7041a81e15dee7a029e))
 
-* **itool** move all cursors on drag with alt modifier ([`6ad638d`](https://github.com/kmnhan/erlabpy/commit/6ad638d9ef07c7b5dac05acc4977a39954abe96a))
+* (**itool**) move all cursors on drag with alt modifier ([`6ad638d`](https://github.com/kmnhan/erlabpy/commit/6ad638d9ef07c7b5dac05acc4977a39954abe96a))
 
-* **itool** add color limit lock and discrete cursor line ([`0929d61`](https://github.com/kmnhan/erlabpy/commit/0929d61973ef8ae62065820378d362a70cbbe110))
+* (**itool**) add color limit lock and discrete cursor line ([`0929d61`](https://github.com/kmnhan/erlabpy/commit/0929d61973ef8ae62065820378d362a70cbbe110))
 
-* **itool** parse ArrayLike input automatically ([`ce3d802`](https://github.com/kmnhan/erlabpy/commit/ce3d8027bf2ba2956ef80c8c28cbed28ab6d21be))
+* (**itool**) parse ArrayLike input automatically ([`ce3d802`](https://github.com/kmnhan/erlabpy/commit/ce3d8027bf2ba2956ef80c8c28cbed28ab6d21be))
 
-* **itool** add more menus ([`6b423eb`](https://github.com/kmnhan/erlabpy/commit/6b423eb0b56c0082ec0eee7de89761cbc56dfba5))
+* (**itool**) add more menus ([`6b423eb`](https://github.com/kmnhan/erlabpy/commit/6b423eb0b56c0082ec0eee7de89761cbc56dfba5))
 
 * add EDC fitting tool (WIP) ([`4fceef5`](https://github.com/kmnhan/erlabpy/commit/4fceef509c63b8f51661b37cb8470f5bcf514b4b))
 
 * add and modify styles ([`079f007`](https://github.com/kmnhan/erlabpy/commit/079f0070da78c1c44dcb67c46b38e84490d67f16))
 
-* **io** warn when modifying attrs ([`7692379`](https://github.com/kmnhan/erlabpy/commit/7692379416dda67c47a302d49b1c9a747514ef9c))
+* (**io**) warn when modifying attrs ([`7692379`](https://github.com/kmnhan/erlabpy/commit/7692379416dda67c47a302d49b1c9a747514ef9c))
 
-* **itool** add menubar ([`1614567`](https://github.com/kmnhan/erlabpy/commit/1614567a1287e3a099418190855ff54f8cadad95))
+* (**itool**) add menubar ([`1614567`](https://github.com/kmnhan/erlabpy/commit/1614567a1287e3a099418190855ff54f8cadad95))
 
-* **itool** better cursor colors ([`78dae09`](https://github.com/kmnhan/erlabpy/commit/78dae09619bfb79424eb0af930cc444467fce2c2))
+* (**itool**) better cursor colors ([`78dae09`](https://github.com/kmnhan/erlabpy/commit/78dae09619bfb79424eb0af930cc444467fce2c2))
 
-* **itool** enable handling multiple cursors ([`e971af7`](https://github.com/kmnhan/erlabpy/commit/e971af767f78d72acee064a0e87ae5764fd13d98))
+* (**itool**) enable handling multiple cursors ([`e971af7`](https://github.com/kmnhan/erlabpy/commit/e971af767f78d72acee064a0e87ae5764fd13d98))
 
 * pretty plot gold edge fit results ([`aa621c5`](https://github.com/kmnhan/erlabpy/commit/aa621c588b733eae683494422f1330da74e09b23))
 
 * add vertical Fermi energy indicators ([`80e2694`](https://github.com/kmnhan/erlabpy/commit/80e2694ed19dc18375b2dc26531fbda37525ca9e))
 
 * easier colorbar font size specification ([`5638d9c`](https://github.com/kmnhan/erlabpy/commit/5638d9c709c888fcfc24503196955e9d8df863c2))
 
 * add interactive progressbar for joblib ([`3fd24c7`](https://github.com/kmnhan/erlabpy/commit/3fd24c7dd57e2139c6f16af88fe0773323b928b4))
 
-* **itool** add axis labels ([`96f9e76`](https://github.com/kmnhan/erlabpy/commit/96f9e76315cbff362d11e16b2b33378c5d7deab0))
+* (**itool**) add axis labels ([`96f9e76`](https://github.com/kmnhan/erlabpy/commit/96f9e76315cbff362d11e16b2b33378c5d7deab0))
 
-* **itool** minor adjustments to layout ([`c5dcbe2`](https://github.com/kmnhan/erlabpy/commit/c5dcbe2ec3c143579fe2c7969eda65dcb741e876))
+* (**itool**) minor adjustments to layout ([`c5dcbe2`](https://github.com/kmnhan/erlabpy/commit/c5dcbe2ec3c143579fe2c7969eda65dcb741e876))
 
-* **goldtool** higher order polynomials ([`5f34c35`](https://github.com/kmnhan/erlabpy/commit/5f34c3579975ed48124a5a2cf89980735f8d53a8))
+* (**goldtool**) higher order polynomials ([`5f34c35`](https://github.com/kmnhan/erlabpy/commit/5f34c3579975ed48124a5a2cf89980735f8d53a8))
 
-* **gold** get full results from Fermi edge fitting ([`ce0d853`](https://github.com/kmnhan/erlabpy/commit/ce0d853adf51df174d01098b703db21e26859882))
+* (**gold**) get full results from Fermi edge fitting ([`ce0d853`](https://github.com/kmnhan/erlabpy/commit/ce0d853adf51df174d01098b703db21e26859882))
 
 * colorbar tick label customization ([`03e82bf`](https://github.com/kmnhan/erlabpy/commit/03e82bf100b3ca62fe781e1c82d54fce0ecab9b7))
 
-* **io** improve SSRL loader ([`8fe9a46`](https://github.com/kmnhan/erlabpy/commit/8fe9a467d348225d213909a95acf9d80d93d018b))
+* (**io**) improve SSRL loader ([`8fe9a46`](https://github.com/kmnhan/erlabpy/commit/8fe9a467d348225d213909a95acf9d80d93d018b))
 
-* **itool** multicursor binning ([`bb4430c`](https://github.com/kmnhan/erlabpy/commit/bb4430ced79bfec8850ef7724c6ce752b4cd707b))
+* (**itool**) multicursor binning ([`bb4430c`](https://github.com/kmnhan/erlabpy/commit/bb4430ced79bfec8850ef7724c6ce752b4cd707b))
 
 * add autoscale convenience function ([`36f838d`](https://github.com/kmnhan/erlabpy/commit/36f838d47bd5fdf8554e59b327b9bed9df961a0f))
 
 * delegate font handling to different styles ([`aabf87b`](https://github.com/kmnhan/erlabpy/commit/aabf87b05be49c8bfe19afaf570bb769656c5ccb))
 
 * simplify getting foreground color based on image ([`8034bfd`](https://github.com/kmnhan/erlabpy/commit/8034bfd15452f6032b0b2ff64cb14dc92d607c8b))
 
 * add fira font mplstyle ([`9c05702`](https://github.com/kmnhan/erlabpy/commit/9c05702d1ea822b5e138fca1e5f75c8d600397d7))
 
-* **itool** bind autorange to keyboard ([`98a236d`](https://github.com/kmnhan/erlabpy/commit/98a236deb88a9d74bc6763f49a75d465a097a264))
+* (**itool**) bind autorange to keyboard ([`98a236d`](https://github.com/kmnhan/erlabpy/commit/98a236deb88a9d74bc6763f49a75d465a097a264))
 
-* **itool** implement rad2deg ([`c074d74`](https://github.com/kmnhan/erlabpy/commit/c074d74a4ba62fda1e81e1dedf039ae939959975))
+* (**itool**) implement rad2deg ([`c074d74`](https://github.com/kmnhan/erlabpy/commit/c074d74a4ba62fda1e81e1dedf039ae939959975))
 
 * include styles ([`5281177`](https://github.com/kmnhan/erlabpy/commit/528117714f3f7b08d253036b7492aba48dfe833b))
 
 * add completely reimplemented imagetool with faster slicing and multicursor support ([`af0655e`](https://github.com/kmnhan/erlabpy/commit/af0655eebb1f27199eae5270c971b206cb3edb6b))
 
 * added interactive gold edge fitting tool ([`c4017b6`](https://github.com/kmnhan/erlabpy/commit/c4017b699b27af76b9aa912f3231d1a19864e5e9))
 
 * allow axes input to slice plotter ([`ab4c639`](https://github.com/kmnhan/erlabpy/commit/ab4c639c0b4d9e1cd34d03950846db2a4afdb138))
 
 * multiple axes input to bz overlay plotter ([`9820e34`](https://github.com/kmnhan/erlabpy/commit/9820e340584299f5bbf95aea4193e6c47c026304))
 
-* **fermiline** support multiple axes input ([`9dc59b1`](https://github.com/kmnhan/erlabpy/commit/9dc59b1fbb6605e82ed0dcf8e7f444978c2c05df))
+* (**fermiline**) support multiple axes input ([`9dc59b1`](https://github.com/kmnhan/erlabpy/commit/9dc59b1fbb6605e82ed0dcf8e7f444978c2c05df))
 
 * add interactive widget base classes ([`e6787cf`](https://github.com/kmnhan/erlabpy/commit/e6787cf567bfd1a1cc1a131a69700143eb6e17bb))
 
-* **colors** add colorbar creation macro ([`811ed52`](https://github.com/kmnhan/erlabpy/commit/811ed526dc99d165f3f0cf77dd577744973cb539))
+* (**colors**) add colorbar creation macro ([`811ed52`](https://github.com/kmnhan/erlabpy/commit/811ed526dc99d165f3f0cf77dd577744973cb539))
 
 * remove pyarpes dependency on labeling ([`71081fa`](https://github.com/kmnhan/erlabpy/commit/71081faf8404d256fb5b7f57fdc2304de6674445))
 
-* **io** silent loading of .pxp files ([`27d6b30`](https://github.com/kmnhan/erlabpy/commit/27d6b30fbff64237562ceaa9b3436d48b06a6e3b))
+* (**io**) silent loading of .pxp files ([`27d6b30`](https://github.com/kmnhan/erlabpy/commit/27d6b30fbff64237562ceaa9b3436d48b06a6e3b))
 
 * parallel processing helpers wip ([`ac88e26`](https://github.com/kmnhan/erlabpy/commit/ac88e264463f4647a1195bd4eb93d617cd38c972))
 
 * reliable gold edge and resolution fitting ([`653db58`](https://github.com/kmnhan/erlabpy/commit/653db5891f4573e069caaeb6f65edcffaa24b316))
 
-* **annotations** better high symmetry marking ([`8e6dfcb`](https://github.com/kmnhan/erlabpy/commit/8e6dfcbc3f26f1d17a5bc1400a60512c51aa8a4d))
+* (**annotations**) better high symmetry marking ([`8e6dfcb`](https://github.com/kmnhan/erlabpy/commit/8e6dfcbc3f26f1d17a5bc1400a60512c51aa8a4d))
 
-* **mask** completely reimplement masking ([`ccfb9b6`](https://github.com/kmnhan/erlabpy/commit/ccfb9b61b75aa5e1f17e88402fc6824fe14287e8))
+* (**mask**) completely reimplement masking ([`ccfb9b6`](https://github.com/kmnhan/erlabpy/commit/ccfb9b61b75aa5e1f17e88402fc6824fe14287e8))
 
-* **io** data loading functions for igor ([`dd333e1`](https://github.com/kmnhan/erlabpy/commit/dd333e199c5e2718b0bb712b1842e37b6c099ea6))
+* (**io**) data loading functions for igor ([`dd333e1`](https://github.com/kmnhan/erlabpy/commit/dd333e199c5e2718b0bb712b1842e37b6c099ea6))
 
-* **correlation** rewrite based on scipy ([`14b1b29`](https://github.com/kmnhan/erlabpy/commit/14b1b29c1752ccb3d93d67de6de160e714606133))
+* (**correlation**) rewrite based on scipy ([`14b1b29`](https://github.com/kmnhan/erlabpy/commit/14b1b29c1752ccb3d93d67de6de160e714606133))
 
 * add callable models for edge correction ([`3a6d8c3`](https://github.com/kmnhan/erlabpy/commit/3a6d8c3b5cc44078cd4b8f5056ccacb21d335428))
 
 * functions for gold edge related analysis ([`8c4941f`](https://github.com/kmnhan/erlabpy/commit/8c4941f6347c09a783b9e34ff17a132e05d16631))
 
 * rudimentary loader for SSRL ([`7e18e13`](https://github.com/kmnhan/erlabpy/commit/7e18e1354f95341440da2f020d992c4a38403261))
 
-* **itool** better dock, improved memory usage ([`04f0047`](https://github.com/kmnhan/erlabpy/commit/04f00472ce5b507c1d467620dcfe03bdde1700c0))
+* (**itool**) better dock, improved memory usage ([`04f0047`](https://github.com/kmnhan/erlabpy/commit/04f00472ce5b507c1d467620dcfe03bdde1700c0))
 
-* **itool** support 4D input ([`33a252f`](https://github.com/kmnhan/erlabpy/commit/33a252f42f88b9a0c182a3d771644b8e937d57be))
+* (**itool**) support 4D input ([`33a252f`](https://github.com/kmnhan/erlabpy/commit/33a252f42f88b9a0c182a3d771644b8e937d57be))
 
 * add sizebar ([`21f420f`](https://github.com/kmnhan/erlabpy/commit/21f420f362dbf2bb18d1b16e34051dc11034a08a))
 
-* **itool** add gamma slider ([`f5efcb7`](https://github.com/kmnhan/erlabpy/commit/f5efcb71c21696ccb9ed1e9b90b3c9e976bac01e))
+* (**itool**) add gamma slider ([`f5efcb7`](https://github.com/kmnhan/erlabpy/commit/f5efcb71c21696ccb9ed1e9b90b3c9e976bac01e))
 
-* **itool** subclass buttons for dark mode ([`e215470`](https://github.com/kmnhan/erlabpy/commit/e2154703986a8d35aa9b0b44b35a40c9dde62ec7))
+* (**itool**) subclass buttons for dark mode ([`e215470`](https://github.com/kmnhan/erlabpy/commit/e2154703986a8d35aa9b0b44b35a40c9dde62ec7))
 
 * initial commit of general interactive tool ([`bf00956`](https://github.com/kmnhan/erlabpy/commit/bf009565f26a95ead1cda41bb000409bc435062e))
 
-* **itool** add axes visibility controls ([`258ff3f`](https://github.com/kmnhan/erlabpy/commit/258ff3fcecf5743adb04c82606feeff54ed828eb))
+* (**itool**) add axes visibility controls ([`258ff3f`](https://github.com/kmnhan/erlabpy/commit/258ff3fcecf5743adb04c82606feeff54ed828eb))
 
-* **itool** hide and show individual axes ([`6a8c71e`](https://github.com/kmnhan/erlabpy/commit/6a8c71e514c8fd4755c47ff521ed5f242c72056d))
+* (**itool**) hide and show individual axes ([`6a8c71e`](https://github.com/kmnhan/erlabpy/commit/6a8c71e514c8fd4755c47ff521ed5f242c72056d))
 
-* **itool** enable latex labels ([`be0b25d`](https://github.com/kmnhan/erlabpy/commit/be0b25dcad9abf49859c766668e969cc800406b9))
+* (**itool**) enable latex labels ([`be0b25d`](https://github.com/kmnhan/erlabpy/commit/be0b25dcad9abf49859c766668e969cc800406b9))
 
-* **itool** add joystick for cursor ([`3faf410`](https://github.com/kmnhan/erlabpy/commit/3faf410676af1e85ebe27282a80d65c2d55c17a0))
+* (**itool**) add joystick for cursor ([`3faf410`](https://github.com/kmnhan/erlabpy/commit/3faf410676af1e85ebe27282a80d65c2d55c17a0))
 
 * cursor binning ([`9b3de32`](https://github.com/kmnhan/erlabpy/commit/9b3de32f3b1ee098b646b0ad663cd8a95de02e11))
 
 * new convenience function ([`e482cf6`](https://github.com/kmnhan/erlabpy/commit/e482cf6234e5b865b36ed2574c9566b199806c26))
 
 * add Fermi edge correction from fit result ([`607e6ee`](https://github.com/kmnhan/erlabpy/commit/607e6eedef84b05f83cef7097c7ce0aaedbb2f97))
 
 * add tool for analyzing dispersive features ([`7926238`](https://github.com/kmnhan/erlabpy/commit/792623836b77502f7d4ab065712465df007fb1ed))
 
 * add pyqtgraph-based itool, WIP ([`de462c7`](https://github.com/kmnhan/erlabpy/commit/de462c7ab22d5ba47b686e05eaa0cc6558d2d4be))
 
-* **itool** add invert colormap ([`bd616ad`](https://github.com/kmnhan/erlabpy/commit/bd616adf30cdee0f96433d9cb8ca8febedf5207c))
+* (**itool**) add invert colormap ([`bd616ad`](https://github.com/kmnhan/erlabpy/commit/bd616adf30cdee0f96433d9cb8ca8febedf5207c))
 
-* **itool** add color picker ([`cb40537`](https://github.com/kmnhan/erlabpy/commit/cb405377302855b357387a539a37f7f466b83447))
+* (**itool**) add color picker ([`cb40537`](https://github.com/kmnhan/erlabpy/commit/cb405377302855b357387a539a37f7f466b83447))
 
-* **itool** add binning ([`4d8155d`](https://github.com/kmnhan/erlabpy/commit/4d8155dd85da507ee87b09cb604ed2cba2ea7e42))
+* (**itool**) add binning ([`4d8155d`](https://github.com/kmnhan/erlabpy/commit/4d8155dd85da507ee87b09cb604ed2cba2ea7e42))
 
 * add dark mode ([`a0dfefd`](https://github.com/kmnhan/erlabpy/commit/a0dfefdc65676b631ceb380216cfbdbdeab6f2f8))
 
-* **itool** 2d image support ([`98d0af7`](https://github.com/kmnhan/erlabpy/commit/98d0af799729884f5ccec203ffacebbffbe72f91))
+* (**itool**) 2d image support ([`98d0af7`](https://github.com/kmnhan/erlabpy/commit/98d0af799729884f5ccec203ffacebbffbe72f91))
 
 * add toggle for cursor snap ([`d9ccfbd`](https://github.com/kmnhan/erlabpy/commit/d9ccfbdd8b36fce57655ffe04109fffda5c86189))
 
 * add energy and resolution slider to ktool ([`94e886a`](https://github.com/kmnhan/erlabpy/commit/94e886ab02d638059311b6c6cb43957c3bbde1a9))
 
 * add qt and mpl-based interactive tools ([`823c509`](https://github.com/kmnhan/erlabpy/commit/823c50972fb5afe92f10c9409ed61a7c626971fb))
 
@@ -1052,61 +1114,61 @@
 
 * added annotation macros ([`dd36878`](https://github.com/kmnhan/erlabpy/commit/dd36878e25acd2b7cff5f34442f93b40307ff452))
 
 * Add characterization module ([`e5c56e8`](https://github.com/kmnhan/erlabpy/commit/e5c56e8903d5bcfa95d0d665186b4c1bb33c81a7))
 
 ### Fix
 
-* **era.fit.models** undefined name in all ([`308f525`](https://github.com/kmnhan/erlabpy/commit/308f525dd291247b631ac8a878d572ea3bfd2230))
+* (**era.fit.models**) undefined name in all ([`308f525`](https://github.com/kmnhan/erlabpy/commit/308f525dd291247b631ac8a878d572ea3bfd2230))
 
 * invalid escape ([`a0a33b6`](https://github.com/kmnhan/erlabpy/commit/a0a33b6695471fb85060c35f17c0cb39d9a6338b))
 
-* **interpolate** make output shape consistent with scipy ([`0709493`](https://github.com/kmnhan/erlabpy/commit/07094935339bd29ab1c2fce5bf0a4478121a69c7))
+* (**interpolate**) make output shape consistent with scipy ([`0709493`](https://github.com/kmnhan/erlabpy/commit/07094935339bd29ab1c2fce5bf0a4478121a69c7))
 
 * do not reset offsets on accessor initialization if exists ([`5328483`](https://github.com/kmnhan/erlabpy/commit/5328483587da21de3e11966d4baab4bc0fefce12))
 
-* **itool** properly parse colorcet cmaps ([`cb81811`](https://github.com/kmnhan/erlabpy/commit/cb81811f4a1b9ea24657d2aa27a7455825fb4eff))
+* (**itool**) properly parse colorcet cmaps ([`cb81811`](https://github.com/kmnhan/erlabpy/commit/cb81811f4a1b9ea24657d2aa27a7455825fb4eff))
 
 * add some more guess constraints, fix type ([`82825a7`](https://github.com/kmnhan/erlabpy/commit/82825a79af122602435802d3a3aab349ef2e37b7))
 
-* **goldtool** round roi position to 3 decimal places ([`d83fafa`](https://github.com/kmnhan/erlabpy/commit/d83fafa0712726fee935755a0d3f816100f90666))
+* (**goldtool**) round roi position to 3 decimal places ([`d83fafa`](https://github.com/kmnhan/erlabpy/commit/d83fafa0712726fee935755a0d3f816100f90666))
 
-* **goldtool** disable memmapping for parallel fitting ([`0c8b053`](https://github.com/kmnhan/erlabpy/commit/0c8b053e2a741f28aa622a2d9ba7e847a82bd8d0))
+* (**goldtool**) disable memmapping for parallel fitting ([`0c8b053`](https://github.com/kmnhan/erlabpy/commit/0c8b053e2a741f28aa622a2d9ba7e847a82bd8d0))
 
 * duplicated data_dir ([`4b08754`](https://github.com/kmnhan/erlabpy/commit/4b087543059e730c0085b0a656424329cf99bf08))
 
 * missing import ([`a1241da`](https://github.com/kmnhan/erlabpy/commit/a1241da6cbdffb68cb9405236d0bbb40bcf16815))
 
-* **io** fix duplicated loader aliases ([`d832a48`](https://github.com/kmnhan/erlabpy/commit/d832a487e6e63befa24049992eed8a6fbd2a2be7))
+* (**io**) fix duplicated loader aliases ([`d832a48`](https://github.com/kmnhan/erlabpy/commit/d832a487e6e63befa24049992eed8a6fbd2a2be7))
 
 * syntax error ([`63214f3`](https://github.com/kmnhan/erlabpy/commit/63214f35fd9009e04d7ed4299bf9327ba18f08e0))
 
-* **io.plugins.merlin** files with non-standard names  are properly summarized ([`388dd02`](https://github.com/kmnhan/erlabpy/commit/388dd0266e82557a250f9d20dff3a918b139cf00))
+* (**io.plugins.merlin**) files with non-standard names  are properly summarized ([`388dd02`](https://github.com/kmnhan/erlabpy/commit/388dd0266e82557a250f9d20dff3a918b139cf00))
 
 * move positional to keyword only ([`ae300b3`](https://github.com/kmnhan/erlabpy/commit/ae300b3a9158940e07ccd585fc76750e3652593c))
 
-* **io** return full path for get_files ([`bbaab33`](https://github.com/kmnhan/erlabpy/commit/bbaab3328c09a385762c0d65d00e24ef50ed9273))
+* (**io**) return full path for get_files ([`bbaab33`](https://github.com/kmnhan/erlabpy/commit/bbaab3328c09a385762c0d65d00e24ef50ed9273))
 
 * make fit result accessible ([`a40ae66`](https://github.com/kmnhan/erlabpy/commit/a40ae6616721a320eac51e69b7206ec7bf70f243))
 
 * typo in multipeakfunction ([`cafe6cc`](https://github.com/kmnhan/erlabpy/commit/cafe6cc405650921b0a28cc9831b53b448e620ff))
 
-* **ktool** round angle offsets ([`31c4730`](https://github.com/kmnhan/erlabpy/commit/31c4730663b24a344ded9a658580981732445100))
+* (**ktool**) round angle offsets ([`31c4730`](https://github.com/kmnhan/erlabpy/commit/31c4730663b24a344ded9a658580981732445100))
 
-* **io** when given path to file, skip regex parsing ([`92019bb`](https://github.com/kmnhan/erlabpy/commit/92019bb56b5b8f818bc311a294150644149899ec))
+* (**io**) when given path to file, skip regex parsing ([`92019bb`](https://github.com/kmnhan/erlabpy/commit/92019bb56b5b8f818bc311a294150644149899ec))
 
 * more realistic angle data generation ([`498e7f5`](https://github.com/kmnhan/erlabpy/commit/498e7f52ce567efe8029f2d4baec7ccb12d607db))
 
 * return type ([`c089f44`](https://github.com/kmnhan/erlabpy/commit/c089f4404c4e63172e1da1d06d167ea75fef5841))
 
 * move doc comments to above ([`429c868`](https://github.com/kmnhan/erlabpy/commit/429c8681dd90bc3c7c890377eb37f4ad1414c3f7))
 
-* **docs** avoid direct import in conf.py ([`db930f0`](https://github.com/kmnhan/erlabpy/commit/db930f03f7d308f677dfa5c1385e3dd6c9bf3d0e))
+* (**docs**) avoid direct import in conf.py ([`db930f0`](https://github.com/kmnhan/erlabpy/commit/db930f03f7d308f677dfa5c1385e3dd6c9bf3d0e))
 
-* **ktool** default values and data orientation ([`1dcf1f4`](https://github.com/kmnhan/erlabpy/commit/1dcf1f4ca773c5ea5e30146a8fec927851ec54a5))
+* (**ktool**) default values and data orientation ([`1dcf1f4`](https://github.com/kmnhan/erlabpy/commit/1dcf1f4ca773c5ea5e30146a8fec927851ec54a5))
 
 * Update ktool.py to keep up with refactoring changes ([`f23afb2`](https://github.com/kmnhan/erlabpy/commit/f23afb25c5a2141a53e7427cb0e4ea1291e008f3))
 
 * fix typo in documentation ([`5c527a4`](https://github.com/kmnhan/erlabpy/commit/5c527a4da449867231cf4ca548cd147cd7657edb))
 
 * properly execute in ipython ([`262b965`](https://github.com/kmnhan/erlabpy/commit/262b96518e38cecacf36141614da44d7bf7e3deb))
 
@@ -1124,63 +1186,63 @@
 
 * Add version number to pyproject.toml ([`0caf0c4`](https://github.com/kmnhan/erlabpy/commit/0caf0c40f3dc943f786fe06e68d54b779367edad))
 
 * update version ([`d394f20`](https://github.com/kmnhan/erlabpy/commit/d394f204387a1f3fdb18006298002d03b0a8b0d3))
 
 * Update Sphinx configuration path in .readthedocs.yaml ([`21c1b1f`](https://github.com/kmnhan/erlabpy/commit/21c1b1f02b7e8b356d86074fe5c0f89895afbc90))
 
-* **itool** ignore zerodivision ([`97e2bf5`](https://github.com/kmnhan/erlabpy/commit/97e2bf56c6e351dcfe6bd382c5b888ef12b44f4a))
+* (**itool**) ignore zerodivision ([`97e2bf5`](https://github.com/kmnhan/erlabpy/commit/97e2bf56c6e351dcfe6bd382c5b888ef12b44f4a))
 
 * try to make autoscale_off context more reliable, needs testing ([`3a4726a`](https://github.com/kmnhan/erlabpy/commit/3a4726a90343bee7af916490a76679a027fc6aa1))
 
 * gradient_fill now doesn&#39;t mess with autoscale ([`040db5a`](https://github.com/kmnhan/erlabpy/commit/040db5a6aeaebbdb628a5ff05bddce53f5f825bd))
 
 * proper file handler termination ([`2ca7593`](https://github.com/kmnhan/erlabpy/commit/2ca7593b3036f8c13dda8ec7ae34a18ad8ef572c))
 
 * acf2 stack dimension mismatch resolved ([`8dde2da`](https://github.com/kmnhan/erlabpy/commit/8dde2da853bc756cabc79e0587b93d5f99c92efb))
 
 * validation changed, fixes #11 ([`8479814`](https://github.com/kmnhan/erlabpy/commit/84798146b8596ee4cd75e89282180f4e858176b3))
 
-* **interactive** override copy, temporarily fixes #10 ([`4e99863`](https://github.com/kmnhan/erlabpy/commit/4e99863b2ce5b6fe82f0fbe3658cf9b024f69fb0))
+* (**interactive**) override copy, temporarily fixes #10 ([`4e99863`](https://github.com/kmnhan/erlabpy/commit/4e99863b2ce5b6fe82f0fbe3658cf9b024f69fb0))
 
 * subclass scalarformatter for better compat ([`b69bfd6`](https://github.com/kmnhan/erlabpy/commit/b69bfd6607aa283c1e717e8183982ef1c40d9749))
 
 * nice horizontal colorbar ([`2766e36`](https://github.com/kmnhan/erlabpy/commit/2766e3689ef3ebe5152ec5ce8fe22373127a507b))
 
-* **colors** handle callable segmented cmaps ([`8135d73`](https://github.com/kmnhan/erlabpy/commit/8135d73e3d11f7e8126576b7b2281a15ec6e2920))
+* (**colors**) handle callable segmented cmaps ([`8135d73`](https://github.com/kmnhan/erlabpy/commit/8135d73e3d11f7e8126576b7b2281a15ec6e2920))
 
-* **itool** keyboard modifier syntax ([`d593258`](https://github.com/kmnhan/erlabpy/commit/d5932583b6b36f288a72a5d4965c81c805c55c66))
+* (**itool**) keyboard modifier syntax ([`d593258`](https://github.com/kmnhan/erlabpy/commit/d5932583b6b36f288a72a5d4965c81c805c55c66))
 
-* **io** fix da30 loading ([`ee0615d`](https://github.com/kmnhan/erlabpy/commit/ee0615dd31fff487139350df692045b646402c03))
+* (**io**) fix da30 loading ([`ee0615d`](https://github.com/kmnhan/erlabpy/commit/ee0615dd31fff487139350df692045b646402c03))
 
 * fix typo ([`6a84557`](https://github.com/kmnhan/erlabpy/commit/6a845573f8c0bc0d03c6003a218e6d1322c6a05e))
 
 * load da30 map angle in radians ([`8d08c65`](https://github.com/kmnhan/erlabpy/commit/8d08c6533cbb57b225d5ee9ae99d1795ab5ec300))
 
 * remove duplicate star ([`a018691`](https://github.com/kmnhan/erlabpy/commit/a0186915be3fc7065fbb19af5ff68d491167a468))
 
-* **itool** update io ([`8c082b0`](https://github.com/kmnhan/erlabpy/commit/8c082b0f2c814e101e25dd99002e5fb45fccd744))
+* (**itool**) update io ([`8c082b0`](https://github.com/kmnhan/erlabpy/commit/8c082b0f2c814e101e25dd99002e5fb45fccd744))
 
-* **itool** handle ambiguous datasets ([`9226c12`](https://github.com/kmnhan/erlabpy/commit/9226c12f93ddceb35ea5b8852989dcf15620f9c6))
+* (**itool**) handle ambiguous datasets ([`9226c12`](https://github.com/kmnhan/erlabpy/commit/9226c12f93ddceb35ea5b8852989dcf15620f9c6))
 
-* **itool** catch overflow ([`ae1afe1`](https://github.com/kmnhan/erlabpy/commit/ae1afe16e67b76789c5adc59f1e0b149010cfc2f))
+* (**itool**) catch overflow ([`ae1afe1`](https://github.com/kmnhan/erlabpy/commit/ae1afe16e67b76789c5adc59f1e0b149010cfc2f))
 
 * patch breaking changes in lmfit 1.2.2 ([`8179fc3`](https://github.com/kmnhan/erlabpy/commit/8179fc308976d3ac8ca8575136bea7382ee85eac))
 
 * make colorbar more robust ([`3a4968d`](https://github.com/kmnhan/erlabpy/commit/3a4968dd5983fc4bcde43bdf3056c3cc467be070))
 
 * resistance data loading ([`7db3c4a`](https://github.com/kmnhan/erlabpy/commit/7db3c4abae28ae2ef99d1e8a54aa2744a3bde025))
 
 * typo ([`a74732d`](https://github.com/kmnhan/erlabpy/commit/a74732d8429beb94a3009cbfde004387e4fae762))
 
 * fix critical typo ([`3e10834`](https://github.com/kmnhan/erlabpy/commit/3e10834a8f9f5f78a9a41f3567f2fb4a9d092245))
 
 * handle undetermined spectrum type ([`b59c3e9`](https://github.com/kmnhan/erlabpy/commit/b59c3e9068de1c26c1efced8ee0ffdc62c256f1c))
 
-* **ssrl52** improve compatibility with old data ([`135b022`](https://github.com/kmnhan/erlabpy/commit/135b022996259da7ee379a49a0bb13327182ef51))
+* (**ssrl52**) improve compatibility with old data ([`135b022`](https://github.com/kmnhan/erlabpy/commit/135b022996259da7ee379a49a0bb13327182ef51))
 
 * remove now-redundant patches ([`687ece9`](https://github.com/kmnhan/erlabpy/commit/687ece99866628da3fbb302981d005cf57552cfb))
 
 * improve ZT image view for 4D ([`c8d07b5`](https://github.com/kmnhan/erlabpy/commit/c8d07b522216f191a94a7ef40d7beda478e46074))
 
 * keep slicer object for expected signal behavior ([`e0ebe85`](https://github.com/kmnhan/erlabpy/commit/e0ebe8519d972467332965be4ac097df0c26d530))
 
@@ -1198,23 +1260,23 @@
 
 * circular import ([`186cb03`](https://github.com/kmnhan/erlabpy/commit/186cb03f4a93cba01773b2a5dac848ad16a761cd))
 
 * make qt progressbar more accurate ([`7c83b31`](https://github.com/kmnhan/erlabpy/commit/7c83b3100d7880577c533c3b17b77d6b643759c8))
 
 * revert default pad ([`8e5715c`](https://github.com/kmnhan/erlabpy/commit/8e5715ce5f2c89c236ae7791820dcf5a7411fcc1))
 
-* **goldtool** keyerror on code generation ([`e421719`](https://github.com/kmnhan/erlabpy/commit/e4217193441cabca6f8bce3e4001a530dea02678))
+* (**goldtool**) keyerror on code generation ([`e421719`](https://github.com/kmnhan/erlabpy/commit/e4217193441cabca6f8bce3e4001a530dea02678))
 
-* **io** make save and load work with datasets ([`a4f1a12`](https://github.com/kmnhan/erlabpy/commit/a4f1a1279fb0070f38119e80b04bdbf19739b50c))
+* (**io**) make save and load work with datasets ([`a4f1a12`](https://github.com/kmnhan/erlabpy/commit/a4f1a1279fb0070f38119e80b04bdbf19739b50c))
 
-* **style** nonzero pad on savefig ([`b21a178`](https://github.com/kmnhan/erlabpy/commit/b21a17829d95d69aee2affe4c590c082b1cb22ca))
+* (**style**) nonzero pad on savefig ([`b21a178`](https://github.com/kmnhan/erlabpy/commit/b21a17829d95d69aee2affe4c590c082b1cb22ca))
 
 * gold fit autoscale ([`b81e4e8`](https://github.com/kmnhan/erlabpy/commit/b81e4e86f72eedbc63e256de14b70298c2c591f4))
 
-* **io** can now load BL4 pxt files ([`d318c91`](https://github.com/kmnhan/erlabpy/commit/d318c91bdaa4adc2fb54be647e5932463e84474c))
+* (**io**) can now load BL4 pxt files ([`d318c91`](https://github.com/kmnhan/erlabpy/commit/d318c91bdaa4adc2fb54be647e5932463e84474c))
 
 * gold fit autoscaling ([`9ed8f86`](https://github.com/kmnhan/erlabpy/commit/9ed8f86f68006a648e0ed2868ff65dd451b9f2ff))
 
 * disable covariance matrix scaling ([`a3264c7`](https://github.com/kmnhan/erlabpy/commit/a3264c70bf9d2bb502b83f7265482ff462dba11a))
 
 * try to fix random segfault with numba ([`3505b42`](https://github.com/kmnhan/erlabpy/commit/3505b4291b34697732f2dccc33f81f5c32e5fcad))
 
@@ -1222,17 +1284,17 @@
 
 * stupid regression on rename ([`cc37d8e`](https://github.com/kmnhan/erlabpy/commit/cc37d8e86e7a0ea36a89b265b6409aa2898c302c))
 
 * wrong attributes ([`01812ba`](https://github.com/kmnhan/erlabpy/commit/01812bad65847dbe33d1afe013c564898c3c99a6))
 
 * invert before gamma ([`c70bff5`](https://github.com/kmnhan/erlabpy/commit/c70bff5b59a17d59260a1289e8c3df007194b762))
 
-* **io** fix livexy and livepolar loader dims ([`edcf9a8`](https://github.com/kmnhan/erlabpy/commit/edcf9a8640169bebb427f768baeb82735494ab40))
+* (**io**) fix livexy and livepolar loader dims ([`edcf9a8`](https://github.com/kmnhan/erlabpy/commit/edcf9a8640169bebb427f768baeb82735494ab40))
 
-* **itool** restore compatibility for float64 data ([`4e8baab`](https://github.com/kmnhan/erlabpy/commit/4e8baabb0f592294862bcbda41bdf1422748ab62))
+* (**itool**) restore compatibility for float64 data ([`4e8baab`](https://github.com/kmnhan/erlabpy/commit/4e8baabb0f592294862bcbda41bdf1422748ab62))
 
 * resolve type related problems ([`4ec5bdd`](https://github.com/kmnhan/erlabpy/commit/4ec5bddc2c82076eab3e973845d21f188cf09161))
 
 * fix typo in comment ([`8cd71df`](https://github.com/kmnhan/erlabpy/commit/8cd71df415b5715a64c81dcf338f44abee21fa7d))
 
 * remove type hints, were causing thread errors ([`1ed309c`](https://github.com/kmnhan/erlabpy/commit/1ed309c58ea3c8da696d352e1df0ba03903c223b))
 
@@ -1242,15 +1304,15 @@
 
 * fix curve fitting on notebook ([`4126aa0`](https://github.com/kmnhan/erlabpy/commit/4126aa0fa6061c880b03d188199b3d40d64c4b84))
 
 * compatibility with PyQt6 ([`01f550e`](https://github.com/kmnhan/erlabpy/commit/01f550e463ea14720d0e84cd43bf98501cf0b554))
 
 * stupid commit ([`d3b1f53`](https://github.com/kmnhan/erlabpy/commit/d3b1f53448805691c3de358e2cdfca3cb631866a))
 
-* **io** add compatibiity check, fixes #9 ([`35c6bd7`](https://github.com/kmnhan/erlabpy/commit/35c6bd73753af06f49130dddc642baca008044e4))
+* (**io**) add compatibiity check, fixes #9 ([`35c6bd7`](https://github.com/kmnhan/erlabpy/commit/35c6bd73753af06f49130dddc642baca008044e4))
 
 * correct color limits for new cursors ([`25e54f4`](https://github.com/kmnhan/erlabpy/commit/25e54f46bbca24ac54aa2cccf1abaacf9403ec68))
 
 * add PyQt6 compatibility ([`713cea2`](https://github.com/kmnhan/erlabpy/commit/713cea28683643f27c5b163c1aba0e332c168b30))
 
 * pyqt-compatible multiple inheritance, fixes #7 ([`de37753`](https://github.com/kmnhan/erlabpy/commit/de377534db051b852d528ab8dd6abf212bf3e1a0))
 
@@ -1266,39 +1328,39 @@
 
 * fixes #3 ([`1ae6ff8`](https://github.com/kmnhan/erlabpy/commit/1ae6ff8cd58db64fc439cd034f2f93f6961bd6c9))
 
 * fixes #1 along with some memory optimization ([`a667c6a`](https://github.com/kmnhan/erlabpy/commit/a667c6a44fda268b7a450b4522d2ada193de0639))
 
 * choose nearest for zero width when plotting slices ([`6ba03da`](https://github.com/kmnhan/erlabpy/commit/6ba03da2c6054044701accc20763bac424ac3bcf))
 
-* **itool** multicursor colorbar ([`65bd992`](https://github.com/kmnhan/erlabpy/commit/65bd9923680a11e96350b8f9dab079934199bd3a))
+* (**itool**) multicursor colorbar ([`65bd992`](https://github.com/kmnhan/erlabpy/commit/65bd9923680a11e96350b8f9dab079934199bd3a))
 
 * shift by DataArray ([`fd38eaf`](https://github.com/kmnhan/erlabpy/commit/fd38eaf479b1109f57f3dc30e7b4cc5964459bf7))
 
 * force qt api ([`3613853`](https://github.com/kmnhan/erlabpy/commit/36138538c31ba1baaf6c5606372039aeb5dcfb95))
 
 * temperature not required when fitting with broadened step edge ([`4b83d87`](https://github.com/kmnhan/erlabpy/commit/4b83d8713044e8dfdaf605653cc60f8fe6057ea5))
 
 * fix colorbar conflict with multiple cursors ([`6cb35b6`](https://github.com/kmnhan/erlabpy/commit/6cb35b68b9643dc19d9e197e67554c203e5c4b99))
 
 * wrong sign in powernorm ([`b4df421`](https://github.com/kmnhan/erlabpy/commit/b4df42102822da0e41991b9c176a24b900220088))
 
 * rewrite pyqtgraph colormap normalization ([`e2a807e`](https://github.com/kmnhan/erlabpy/commit/e2a807e7a0c7e556a6d2750cd4052df911b5ec3c))
 
-* **itool** fix misc. bugs ([`15c737c`](https://github.com/kmnhan/erlabpy/commit/15c737cd0096a27d5582ab1f084a7ad070b28bcc))
+* (**itool**) fix misc. bugs ([`15c737c`](https://github.com/kmnhan/erlabpy/commit/15c737cd0096a27d5582ab1f084a7ad070b28bcc))
 
 * retain clipboard after window close ([`e800bc7`](https://github.com/kmnhan/erlabpy/commit/e800bc72fae148e0f9fc4df646566013bf7082b8))
 
-* **bz** input reciprocal lattice vectors ([`32df4d7`](https://github.com/kmnhan/erlabpy/commit/32df4d7e673fbcfb886c959450d30c9bf1fa1d27))
+* (**bz**) input reciprocal lattice vectors ([`32df4d7`](https://github.com/kmnhan/erlabpy/commit/32df4d7e673fbcfb886c959450d30c9bf1fa1d27))
 
 * automatic figure detection ([`f0f2ef9`](https://github.com/kmnhan/erlabpy/commit/f0f2ef9810ec637a46d316b37578bc45307ea881))
 
-* **itool** regression: aspect ratio for 2D arrays ([`087ba24`](https://github.com/kmnhan/erlabpy/commit/087ba24cb99b12901ae928cd2b3288c25570c9eb))
+* (**itool**) regression: aspect ratio for 2D arrays ([`087ba24`](https://github.com/kmnhan/erlabpy/commit/087ba24cb99b12901ae928cd2b3288c25570c9eb))
 
-* **itool** better handle drag ([`23cdbf0`](https://github.com/kmnhan/erlabpy/commit/23cdbf039118980c50760a7ebf94b24b48a6b6c8))
+* (**itool**) better handle drag ([`23cdbf0`](https://github.com/kmnhan/erlabpy/commit/23cdbf039118980c50760a7ebf94b24b48a6b6c8))
 
 * replace bitwise inversion on boolean ([`5569060`](https://github.com/kmnhan/erlabpy/commit/5569060a356aad3d1d3141b5accce61f66e78418))
 
 * works properly with integer coordinates ([`adc0074`](https://github.com/kmnhan/erlabpy/commit/adc00746668456576709b1db9525ea5bb6e5bb11))
 
 * update some deprecated syntax ([`839f1a6`](https://github.com/kmnhan/erlabpy/commit/839f1a60132ff03b578224109553491e49a80aae))
 
@@ -1306,109 +1368,109 @@
 
 * better aspect ratio for 2D arrays ([`b002350`](https://github.com/kmnhan/erlabpy/commit/b002350164c4f9c7cd233f50488937f55dff8e46))
 
 * regression as per pyqtgraph/pyqtgraph@cead5cd ([`74c9f81`](https://github.com/kmnhan/erlabpy/commit/74c9f8181033c9f7cfbe8eaa15b64172dc287601))
 
 * stupid rad2deg handling ([`4a6d629`](https://github.com/kmnhan/erlabpy/commit/4a6d629261e6bc0da286b3c687d8fe8af46ee589))
 
-* **goldtool** catch varname exceptions ([`aa22dd7`](https://github.com/kmnhan/erlabpy/commit/aa22dd7833e1fd7e3f1a36fa48ccee7c6420dffe))
+* (**goldtool**) catch varname exceptions ([`aa22dd7`](https://github.com/kmnhan/erlabpy/commit/aa22dd7833e1fd7e3f1a36fa48ccee7c6420dffe))
 
-* **itool** wrong signals ([`a0f0036`](https://github.com/kmnhan/erlabpy/commit/a0f00366be305f302a52e84eac5e4fc97d7d9d54))
+* (**itool**) wrong signals ([`a0f0036`](https://github.com/kmnhan/erlabpy/commit/a0f00366be305f302a52e84eac5e4fc97d7d9d54))
 
 * colorbar aspect specification ([`456f370`](https://github.com/kmnhan/erlabpy/commit/456f370907ca163c30567992da8edbfebcf18caf))
 
 * docstring and labeling ([`4bbedda`](https://github.com/kmnhan/erlabpy/commit/4bbedda90b83f7be32494cfd63bc9ac7dfb94327))
 
 * attempts to overwrite read-only object ([`0cf8606`](https://github.com/kmnhan/erlabpy/commit/0cf8606cd69ccdeaae4d84945e181b9e2b07a846))
 
-* **plot_array** colorbar extents ([`2fe8a93`](https://github.com/kmnhan/erlabpy/commit/2fe8a930f2cf8fd37d88958231388e4a446b1443))
+* (**plot_array**) colorbar extents ([`2fe8a93`](https://github.com/kmnhan/erlabpy/commit/2fe8a930f2cf8fd37d88958231388e4a446b1443))
 
 * broken binning ([`f217938`](https://github.com/kmnhan/erlabpy/commit/f217938379ea7d69613fdef462b26ed41d4850cd))
 
-* **itool** isocurve wrong orientation ([`dfd6aac`](https://github.com/kmnhan/erlabpy/commit/dfd6aac29b846e5b187791aa7fe2708dc95abe76))
+* (**itool**) isocurve wrong orientation ([`dfd6aac`](https://github.com/kmnhan/erlabpy/commit/dfd6aac29b846e5b187791aa7fe2708dc95abe76))
 
-* **itool** tab position ([`a70af2b`](https://github.com/kmnhan/erlabpy/commit/a70af2be59c80231be605e49304d226ed5c24f0c))
+* (**itool**) tab position ([`a70af2b`](https://github.com/kmnhan/erlabpy/commit/a70af2be59c80231be605e49304d226ed5c24f0c))
 
 * fine-tune automatic colormap assignment ([`1d035bb`](https://github.com/kmnhan/erlabpy/commit/1d035bb6ce178f7c13b4c2cd35b20fb69342a627))
 
-* **itool** smarter mouse detection ([`3032c0c`](https://github.com/kmnhan/erlabpy/commit/3032c0cc15c23a3f345300de0eb57080d31b7604))
+* (**itool**) smarter mouse detection ([`3032c0c`](https://github.com/kmnhan/erlabpy/commit/3032c0cc15c23a3f345300de0eb57080d31b7604))
 
 * noisetool import ([`c99bfd2`](https://github.com/kmnhan/erlabpy/commit/c99bfd2980127f07fc6b361d9156e5a68be2711c))
 
 * invalid import ([`5fd9010`](https://github.com/kmnhan/erlabpy/commit/5fd90104cd8e2a2b8158df6acf88dfa7408bc102))
 
 * flickering cursor when moving ([`439157b`](https://github.com/kmnhan/erlabpy/commit/439157bf3fb3b377ebb17a9f6c7a37b87fafc905))
 
-* **itool** fix transpose ([`0b23f61`](https://github.com/kmnhan/erlabpy/commit/0b23f61dfb7c3dec8a534d5b5c7dae560418376f))
+* (**itool**) fix transpose ([`0b23f61`](https://github.com/kmnhan/erlabpy/commit/0b23f61dfb7c3dec8a534d5b5c7dae560418376f))
 
-* **itool** change wrong 2D layout ([`e04f162`](https://github.com/kmnhan/erlabpy/commit/e04f162ac0f88f1c576942e9eb820044a17ea791))
+* (**itool**) change wrong 2D layout ([`e04f162`](https://github.com/kmnhan/erlabpy/commit/e04f162ac0f88f1c576942e9eb820044a17ea791))
 
-* **itool** revert ([`ca4335a`](https://github.com/kmnhan/erlabpy/commit/ca4335a77ba467d46fa0d68e80927aa6ee8e8a24))
+* (**itool**) revert ([`ca4335a`](https://github.com/kmnhan/erlabpy/commit/ca4335a77ba467d46fa0d68e80927aa6ee8e8a24))
 
-* **itool** adjust blitting ([`0873882`](https://github.com/kmnhan/erlabpy/commit/0873882a7692da94ec05ee659030d0e26be51585))
+* (**itool**) adjust blitting ([`0873882`](https://github.com/kmnhan/erlabpy/commit/0873882a7692da94ec05ee659030d0e26be51585))
 
-* **itool** properly functioning pan &amp; zoom ([`26ce4e8`](https://github.com/kmnhan/erlabpy/commit/26ce4e8efce62eb2ab38f14b097f0121ef6205d4))
+* (**itool**) properly functioning pan &amp; zoom ([`26ce4e8`](https://github.com/kmnhan/erlabpy/commit/26ce4e8efce62eb2ab38f14b097f0121ef6205d4))
 
 * fix offset not syncing across energy ([`7ec4072`](https://github.com/kmnhan/erlabpy/commit/7ec4072c93e1b41f24e4247afc414244a43badac))
 
 * fix cursor issue and home resetting limits ([`f3374ab`](https://github.com/kmnhan/erlabpy/commit/f3374abaa8643aef78f33366dfab9a0994b475ce))
 
 * simplify cursor customization ([`a5ff97f`](https://github.com/kmnhan/erlabpy/commit/a5ff97f6cffcd2cc3da0a31f44d62ac590c663e3))
 
 * make plotting imports backwards compatible ([`82f132b`](https://github.com/kmnhan/erlabpy/commit/82f132b89ffd3c911208ae93fa8d47b1825e7928))
 
-* **plotting** fix UnboundLocalError ([`e4f5bca`](https://github.com/kmnhan/erlabpy/commit/e4f5bca381c881d159c9f6a09ebdc86616a4f467))
+* (**plotting**) fix UnboundLocalError ([`e4f5bca`](https://github.com/kmnhan/erlabpy/commit/e4f5bca381c881d159c9f6a09ebdc86616a4f467))
 
 * fix typo ([`39d160a`](https://github.com/kmnhan/erlabpy/commit/39d160a15a6d8990061de48a08b431a2ff35f699))
 
 ### Performance
 
-* **interpolate** make some jitted functions always inlined ([`4624b16`](https://github.com/kmnhan/erlabpy/commit/4624b16ec926546876a98864abe3c1d47b6fc221))
+* (**interpolate**) make some jitted functions always inlined ([`4624b16`](https://github.com/kmnhan/erlabpy/commit/4624b16ec926546876a98864abe3c1d47b6fc221))
 
-* **itool** fps optimization, add proper support for nonuniform dimensions ([`6df84db`](https://github.com/kmnhan/erlabpy/commit/6df84db7156de88b2ee8d100a2ce0c45f8b2135a))
+* (**itool**) fps optimization, add proper support for nonuniform dimensions ([`6df84db`](https://github.com/kmnhan/erlabpy/commit/6df84db7156de88b2ee8d100a2ce0c45f8b2135a))
 
 * cleanup, reduce import time ([`dbfcce3`](https://github.com/kmnhan/erlabpy/commit/dbfcce38f9b874b8532666ff7479dbc789fef657))
 
-* **itool** add cached properties ([`0124093`](https://github.com/kmnhan/erlabpy/commit/0124093a25ba47e5bc304125fcfd62f6768beb13))
+* (**itool**) add cached properties ([`0124093`](https://github.com/kmnhan/erlabpy/commit/0124093a25ba47e5bc304125fcfd62f6768beb13))
 
 * limit fps with SignalProxy ([`f7ce099`](https://github.com/kmnhan/erlabpy/commit/f7ce099f87e97adeb27a8e4f2d760b6ddd4f4d22))
 
 * get coords efficiently ([`5582afc`](https://github.com/kmnhan/erlabpy/commit/5582afc9e86e8306e6499da52b2f2c06604b029b))
 
 * better min/max performance, fixes #4 ([`3c4aa13`](https://github.com/kmnhan/erlabpy/commit/3c4aa1369fbbf10fa5a2597dc958bb559e4bb26a))
 
-* **slicer** contiguity optimizations ([`6f2b543`](https://github.com/kmnhan/erlabpy/commit/6f2b543a11d89d744961e1f1716ad542a9bab163))
+* (**slicer**) contiguity optimizations ([`6f2b543`](https://github.com/kmnhan/erlabpy/commit/6f2b543a11d89d744961e1f1716ad542a9bab163))
 
-* **itool** update only relevant axes ([`c561650`](https://github.com/kmnhan/erlabpy/commit/c5616502767e8f14425ba07bed4660355eba1203))
+* (**itool**) update only relevant axes ([`c561650`](https://github.com/kmnhan/erlabpy/commit/c5616502767e8f14425ba07bed4660355eba1203))
 
 ### Refactor
 
 * apply linter suggestions ([`edfc91a`](https://github.com/kmnhan/erlabpy/commit/edfc91a6712620588106471ae03975a76976f634))
 
 * apply linter suggestions ([`231f794`](https://github.com/kmnhan/erlabpy/commit/231f794a3aaf6575528df63b70a4478cb9769fe8))
 
 * apply some linter suggestions ([`4e1f66c`](https://github.com/kmnhan/erlabpy/commit/4e1f66c6b19eb2e3674511e19309c9127d610369))
 
-* **goldtool** ui changes ([`464d05e`](https://github.com/kmnhan/erlabpy/commit/464d05ee270cf601c322536b3dafd3c7bf0e9f7f))
+* (**goldtool**) ui changes ([`464d05e`](https://github.com/kmnhan/erlabpy/commit/464d05ee270cf601c322536b3dafd3c7bf0e9f7f))
 
 * rename variable ([`32a901e`](https://github.com/kmnhan/erlabpy/commit/32a901e0de1b7d0c5fb6858a275b8bf3cb69e801))
 
 * cleanup namespace ([`4779e46`](https://github.com/kmnhan/erlabpy/commit/4779e46920cf88a49f211d1d7f856f61e6c84c2a))
 
-* **io** minor changes to summary format ([`d26a8f7`](https://github.com/kmnhan/erlabpy/commit/d26a8f78f4d86f7b0654a0949e644d2f96652b50))
+* (**io**) minor changes to summary format ([`d26a8f7`](https://github.com/kmnhan/erlabpy/commit/d26a8f78f4d86f7b0654a0949e644d2f96652b50))
 
 * move functions  to submodule ([`824a2fb`](https://github.com/kmnhan/erlabpy/commit/824a2fb4847d5f29dc51f50517a51aae3709d3df))
 
 * fit functions submodule ([`2bc555c`](https://github.com/kmnhan/erlabpy/commit/2bc555cfb050d28523f805b75053dcf836759a7f))
 
-* **io.dataloader** fix _repr_html_ to return valid html table ([`73adb0f`](https://github.com/kmnhan/erlabpy/commit/73adb0ffffc618d28903a4c5814923dac5502186))
+* (**io.dataloader**) fix _repr_html_ to return valid html table ([`73adb0f`](https://github.com/kmnhan/erlabpy/commit/73adb0ffffc618d28903a4c5814923dac5502186))
 
-* **io.dataloader** make reverse_mapping a staticmethod ([`983c02b`](https://github.com/kmnhan/erlabpy/commit/983c02bda02c97a7eb179c35f98d0a89c0814cd9))
+* (**io.dataloader**) make reverse_mapping a staticmethod ([`983c02b`](https://github.com/kmnhan/erlabpy/commit/983c02bda02c97a7eb179c35f98d0a89c0814cd9))
 
-* **io** change dict format ([`a13b064`](https://github.com/kmnhan/erlabpy/commit/a13b06465f53c78b9edea538e9825d83f66b86f0))
+* (**io**) change dict format ([`a13b064`](https://github.com/kmnhan/erlabpy/commit/a13b06465f53c78b9edea538e9825d83f66b86f0))
 
 * add type annotation ([`7e08658`](https://github.com/kmnhan/erlabpy/commit/7e08658093fe24a383366f722f044029f097cb69))
 
 * use match-case for enum matching ([`cc9e112`](https://github.com/kmnhan/erlabpy/commit/cc9e1126f7571df3e68e568375773a3a4dce63b5))
 
 * change package directory structure; BREAKING CHANGE ([`5385ec7`](https://github.com/kmnhan/erlabpy/commit/5385ec70b23775ddd19b02459cbb0d0630143454))
 
@@ -1416,23 +1478,23 @@
 
 * remove code trying to infer spectrum from dataset ([`3fa6b1b`](https://github.com/kmnhan/erlabpy/commit/3fa6b1b25dc70add644e9719488ae55df314238c))
 
   From now on all data should be strictly a xr.DataArray
 
 * deprecate old ktool, replace ([`dbd972f`](https://github.com/kmnhan/erlabpy/commit/dbd972f0e56197c1796695921b6cc021b3f4d190))
 
-* **gold** add type annotation ([`06c39a7`](https://github.com/kmnhan/erlabpy/commit/06c39a790109e23a81e88c885a1fa0ee1f615e41))
+* (**gold**) add type annotation ([`06c39a7`](https://github.com/kmnhan/erlabpy/commit/06c39a790109e23a81e88c885a1fa0ee1f615e41))
 
 * Update requirements.txt so that igor2 is not editable ([`0e20bc4`](https://github.com/kmnhan/erlabpy/commit/0e20bc48d458a363b4c2e2b829a59ac6e1aba6cf))
 
 * temporarily disable annotate_cuts_erlab ([`08e4b52`](https://github.com/kmnhan/erlabpy/commit/08e4b527316b94b0a1d2912b67d1b67ea4571755))
 
-* **itool** modify test code ([`8934fba`](https://github.com/kmnhan/erlabpy/commit/8934fba1b20cf182455d2a70e24ff835d6ca96be))
+* (**itool**) modify test code ([`8934fba`](https://github.com/kmnhan/erlabpy/commit/8934fba1b20cf182455d2a70e24ff835d6ca96be))
 
-* **exampledata** tweak defaults ([`73eb495`](https://github.com/kmnhan/erlabpy/commit/73eb4955ff3ed7f568136efce5efaf9ab929dfba))
+* (**exampledata**) tweak defaults ([`73eb495`](https://github.com/kmnhan/erlabpy/commit/73eb4955ff3ed7f568136efce5efaf9ab929dfba))
 
 * cleanup ([`88b418f`](https://github.com/kmnhan/erlabpy/commit/88b418f61491917e275ec7b5cc544c157617429d))
 
 * try garbage collection, failed ([`ac75267`](https://github.com/kmnhan/erlabpy/commit/ac75267921884299970c5d78b1633835700dce6e))
 
 * typo ([`f1df9ea`](https://github.com/kmnhan/erlabpy/commit/f1df9ea0a4e128013d21e2f2b5e9a64f9acf57a3))
 
@@ -1440,15 +1502,15 @@
 
 * organize imports ([`70b2b9b`](https://github.com/kmnhan/erlabpy/commit/70b2b9bed7e395a824ee3e1b240937b570e670ec))
 
 * cleanup ([`8b01e73`](https://github.com/kmnhan/erlabpy/commit/8b01e7393b7d7a6ae23b85e6f784a7f760cdd74a))
 
 * relocate color related classes ([`b322fb8`](https://github.com/kmnhan/erlabpy/commit/b322fb8ced0b41a1ec8e7dbaf9ac50c8f7aa853c))
 
-* **io** cleanup imports ([`125f672`](https://github.com/kmnhan/erlabpy/commit/125f672edd3b6f94943c2a3d221e626f9a58c820))
+* (**io**) cleanup imports ([`125f672`](https://github.com/kmnhan/erlabpy/commit/125f672edd3b6f94943c2a3d221e626f9a58c820))
 
 * add submodules to analysis initialization ([`30ab7d0`](https://github.com/kmnhan/erlabpy/commit/30ab7d0f71a6c09633e54345c7317215934c1ca6))
 
 * rename igor procedure file ([`92d495c`](https://github.com/kmnhan/erlabpy/commit/92d495cb114a921a8ca9d1fde81a4e6400d53089))
 
 * cleanup ([`025b39b`](https://github.com/kmnhan/erlabpy/commit/025b39bb557ab364e6c2f5ff14ddb2956ba52467))
 
@@ -1480,15 +1542,15 @@
 
 * cleanup annotations ([`12e590c`](https://github.com/kmnhan/erlabpy/commit/12e590c2a771d089e29aff02492851448640b605))
 
 * transition to new polynomial api ([`5461c34`](https://github.com/kmnhan/erlabpy/commit/5461c342f7a84d1ba98f924c74be6ecde16cf6e4))
 
 * cleanup syntax ([`310c2ba`](https://github.com/kmnhan/erlabpy/commit/310c2babf15d7a22900806cac308643bb22f8bce))
 
-* **itool** changes to layout ([`7a684e4`](https://github.com/kmnhan/erlabpy/commit/7a684e400772036dde7af4f8a4747c8db208eb0f))
+* (**itool**) changes to layout ([`7a684e4`](https://github.com/kmnhan/erlabpy/commit/7a684e400772036dde7af4f8a4747c8db208eb0f))
 
 * remove dependency on darkdetect ([`81fa963`](https://github.com/kmnhan/erlabpy/commit/81fa963a91fddd1eb2b7f316fcec04eb27716d13))
 
 * format code ([`adf6cb3`](https://github.com/kmnhan/erlabpy/commit/adf6cb3cd48e494d708c79906347e3c54fcd3e20))
 
 * remove io module, add as package ([`5d1280a`](https://github.com/kmnhan/erlabpy/commit/5d1280a3c7893bb86a42fdf2a71b6825c5db6986))
 
@@ -1570,15 +1632,15 @@
 
 * reduce pyarpes dependency ([`14e85fb`](https://github.com/kmnhan/erlabpy/commit/14e85fbcfa7d95df674381f8882db80f39e7bda3))
 
 * format with black ([`7696b66`](https://github.com/kmnhan/erlabpy/commit/7696b66c6ef93a04c353e8e199c096c2458794ff))
 
 * format with black ([`f6fc29c`](https://github.com/kmnhan/erlabpy/commit/f6fc29ce22a541d9143397ffb902c34d752cdad3))
 
-* **itool** cleanup hide buttons ([`2649fe9`](https://github.com/kmnhan/erlabpy/commit/2649fe9ae12893e719a456f0cf22b7eee097df0f))
+* (**itool**) cleanup hide buttons ([`2649fe9`](https://github.com/kmnhan/erlabpy/commit/2649fe9ae12893e719a456f0cf22b7eee097df0f))
 
 * format code ([`c69b9cc`](https://github.com/kmnhan/erlabpy/commit/c69b9ccca3ee911b5b07bd6393a43444ba771f33))
 
 * trivial changes ([`6d5df90`](https://github.com/kmnhan/erlabpy/commit/6d5df9019932c4c6ad5930d952714e0bd181cacf))
 
 * easy import ([`b308d3d`](https://github.com/kmnhan/erlabpy/commit/b308d3d546ee92b04299d679042564149759206b))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `erlab-2.0.0/LICENSE` & `erlab-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/PKG-INFO` & `erlab-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,15 +683,15 @@
 Project-URL: Issues, https://github.com/kmnhan/erlabpy/issues
 Project-URL: Changelog, https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md
 Keywords: Condensed Matter Physics,ARPES
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
@@ -710,37 +710,55 @@
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: superqt>=0.6.2
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: uncertainties>=3.0.1
 Requires-Dist: varname>=0.13.0
 Requires-Dist: xarray>=2024.02.0
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: pybtex; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: viz
+Requires-Dist: cmasher; extra == "viz"
+Requires-Dist: cmocean; extra == "viz"
+Requires-Dist: colorcet; extra == "viz"
+Requires-Dist: hvplot; extra == "viz"
 
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/erlab.svg)](https://anaconda.org/conda-forge/erlab)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmnhan/erlabpy/main.svg)](https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main)
 
 A library that provides a set of tools and utilities to handle, manipulate, and
 visualize data from condensed matter physics experiments, with a focus on
 angle-resolved photoemission spectroscopy (ARPES).
 
-*ERLabPy* is built on top of the popular scientific computing libraries `numpy`,
-`scipy`, and `xarray`, and is designed to be easy to use and integrate with
-existing scientific Python workflows. It is also designed to be extensible,
-allowing users to easily add custom functionality and analysis tools.
+*ERLabPy* is built on top of the popular scientific computing libraries
+[*numpy*](https://numpy.org/), [*scipy*](https://scipy.org/), and
+[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and
+integrate with existing scientific Python workflows. It is also designed to be
+extensible, allowing users to easily add custom functionality and analysis
+tools.
 
 *ERLabPy* is developed and maintained by the electronic structure research
 laboratory at Korea Advanced Institute of Science and Technology (KAIST).
 
 ## Features
 
 - **Data Loading**: A flexible and extensible data loading system is included,
@@ -773,29 +791,28 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_dark.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_light.png?raw=true">
   <img alt="Imagetool in action." src="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_light.png?raw=true">
 </picture>
 
 
-## Documentation
+## Getting Started
 
-The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
+To get started, see [installation instructions](https://erlabpy.readthedocs.io/en/stable/getting-started.html).
 
-## Getting Started
+## Documentation
 
-To get started with ERLab, follow the [installation instructions](https://erlabpy.readthedocs.io/en/stable/getting-started.html).
+The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
 
 ## Contributing
 
-Contributions are welcome! Please open an issue or pull request if you have any
-suggestions or improvements. For more information on contributing, see the
-[development guide](https://erlabpy.readthedocs.io/en/stable/development.html).
+ERLabPy is an open-source project and we welcome contributions from the
+community. If you find any bugs, issues, or have any suggestions, please open an
+issue [here](https://github.com/kmnhan/erlabpy/issues). If you would like to add
+a new feature or fix a bug yourself, we would love to have your contribution.
+Feel free to fork the repository and submit a pull request with your changes.
+
+For more information on contributing, see our [Contributing page](https://erlabpy.readthedocs.io/en/stable/contributing.html).
 
 ## License
 
 This project is licensed under the terms of the [GPL-3.0 License](LICENSE).
-
-## Contact
-
-If you have any questions, issues, or suggestions, please open an issue
-[here](https://github.com/kmnhan/erlabpy/issues). We appreciate your feedback!
```

### Comparing `erlab-2.0.0/PythonInterface.ipf` & `erlab-2.1.0/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/README.md` & `erlab-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/erlab.svg)](https://anaconda.org/conda-forge/erlab)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmnhan/erlabpy/main.svg)](https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main)
 
 A library that provides a set of tools and utilities to handle, manipulate, and
 visualize data from condensed matter physics experiments, with a focus on
 angle-resolved photoemission spectroscopy (ARPES).
 
-*ERLabPy* is built on top of the popular scientific computing libraries `numpy`,
-`scipy`, and `xarray`, and is designed to be easy to use and integrate with
-existing scientific Python workflows. It is also designed to be extensible,
-allowing users to easily add custom functionality and analysis tools.
+*ERLabPy* is built on top of the popular scientific computing libraries
+[*numpy*](https://numpy.org/), [*scipy*](https://scipy.org/), and
+[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and
+integrate with existing scientific Python workflows. It is also designed to be
+extensible, allowing users to easily add custom functionality and analysis
+tools.
 
 *ERLabPy* is developed and maintained by the electronic structure research
 laboratory at Korea Advanced Institute of Science and Technology (KAIST).
 
 ## Features
 
 - **Data Loading**: A flexible and extensible data loading system is included,
@@ -51,29 +54,28 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_dark.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_light.png?raw=true">
   <img alt="Imagetool in action." src="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_light.png?raw=true">
 </picture>
 
 
-## Documentation
+## Getting Started
 
-The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
+To get started, see [installation instructions](https://erlabpy.readthedocs.io/en/stable/getting-started.html).
 
-## Getting Started
+## Documentation
 
-To get started with ERLab, follow the [installation instructions](https://erlabpy.readthedocs.io/en/stable/getting-started.html).
+The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
 
 ## Contributing
 
-Contributions are welcome! Please open an issue or pull request if you have any
-suggestions or improvements. For more information on contributing, see the
-[development guide](https://erlabpy.readthedocs.io/en/stable/development.html).
+ERLabPy is an open-source project and we welcome contributions from the
+community. If you find any bugs, issues, or have any suggestions, please open an
+issue [here](https://github.com/kmnhan/erlabpy/issues). If you would like to add
+a new feature or fix a bug yourself, we would love to have your contribution.
+Feel free to fork the repository and submit a pull request with your changes.
+
+For more information on contributing, see our [Contributing page](https://erlabpy.readthedocs.io/en/stable/contributing.html).
 
 ## License
 
 This project is licensed under the terms of the [GPL-3.0 License](LICENSE).
-
-## Contact
-
-If you have any questions, issues, or suggestions, please open an issue
-[here](https://github.com/kmnhan/erlabpy/issues). We appreciate your feedback!
```

### Comparing `erlab-2.0.0/docs/Makefile` & `erlab-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/environment.yml` & `erlab-2.1.0/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/make.bat` & `erlab-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/conf.py` & `erlab-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/development.rst` & `erlab-2.1.0/docs/source/contributing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-*****************
-Development Guide
-*****************
+******************
+Contributing Guide
+******************
 
 .. note::
 
   Parts of this document are based on `Contributing to pandas
   <http://pandas.pydata.org/pandas-docs/stable/contributing.html>`_ and
   `Contributing to xarray
   <https://docs.xarray.dev/en/stable/contributing.html>`_.
 
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 
 Creating a development environment
 ==================================
 
 First, you will need to install `git` and `conda` (or `mamba`).
 
 Installing git
@@ -256,33 +257,60 @@
 review.
 
 .. _development.code-standards:
 
 Code standards
 ==============
 
-Import sorting, formatting, and linting are enforced with `Ruff
-<https://github.com/astral-sh/ruff>`_. If you wish to contribute, using
-`pre-commit <https://pre-commit.com>`_ is recommended. This will ensure that
-your code is properly formatted before you commit it. A pre-commit configuration
-file for ruff is included in the repository.
+- Import sorting, formatting, and linting are enforced with `Ruff
+  <https://github.com/astral-sh/ruff>`_.
+
+- If you wish to contribute, using `pre-commit <https://pre-commit.com>`_ is
+  recommended. This will ensure that your code is properly formatted before you
+  commit it. A pre-commit configuration file for ruff is included in the
+  repository.
+
+- When writing code that uses Qt, please adhere to the following rules:
+
+  * Import all Qt bindings from `qtpy <https://github.com/spyder-ide/qtpy>`_,
+    and only import the top level modules: ::
+
+      from qtpy import QtWidgets, QtCore, QtGui
+
+  * Use fully qualified enum names from Qt6 instead of the short-form enums from
+    Qt5, i. e., ``QtCore.Qt.CheckState.Checked`` instead of
+    ``QtCore.Qt.Checked``.
+
+  * Use the signal and slot syntax from PySide6 (``QtCore.Signal`` and
+    ``QtCore.Slot`` instead of ``QtCore.pyqtSignal`` and ``QtCore.pyqtSlot``)
+
+  * When using Qt Designer, place ``.ui`` files in the same directory as the
+    Python file that   uses them. The files must be imported using the
+    ``loadUiType`` function from ``qtpy.uic``. For example: ::
+
+      from qtpy import uic
+
+      class MyWidget(*uic.loadUiType(os.path.join(os.path.dirname(__file__), "mywidget.ui"))):
+          def __init__(self):
+              super().__init__()
+              self.setupUi(self)
 
 Documentation
 =============
 
 The documentation is written in **reStructuredText**, which is almost like
 writing in plain English, and built using `Sphinx <http://sphinx-doc.org/>`__.
 The Sphinx Documentation has an excellent `introduction to reST
 <http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`__.
 Review the Sphinx docs to perform more complex changes to the documentation as
 well.
 
 Some other important things to know about the docs:
 
-- The *erlabpy* documentation consists of two parts: the docstrings in the code
+- The documentation consists of two parts: the docstrings in the code
   itself and the docs in this folder ``erlabpy/docs/source/``.
 
   The docstrings are meant to provide a clear explanation of the usage of the
   individual functions, while the documentation in this folder consists of
   tutorial-like overviews per topic together with some other information.
 
 - The docstrings follow the **NumPy Docstring Standard**, which is used widely
```

### Comparing `erlab-2.0.0/docs/source/images/imagetool_dark.png` & `erlab-2.1.0/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/images/imagetool_light.png` & `erlab-2.1.0/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/images/ktool_1_dark.png` & `erlab-2.1.0/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/images/ktool_1_light.png` & `erlab-2.1.0/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/images/ktool_2_dark.png` & `erlab-2.1.0/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/images/ktool_2_light.png` & `erlab-2.1.0/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/index.rst` & `erlab-2.1.0/docs/source/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
    .. image:: https://img.shields.io/pypi/pyversions/erlab
        :target: https://pypi.org/project/erlab/
        :alt: Supported Python Versions
    .. image:: https://img.shields.io/pypi/v/erlab.svg
        :target: https://pypi.org/project/erlab/
        :alt: PyPi
+   .. image:: https://img.shields.io/conda/vn/conda-forge/erlab.svg
+       :target: https://anaconda.org/conda-forge/erlab
+       :alt: Conda Version
    .. image:: https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg
        :target: https://github.com/kmnhan/erlabpy/actions/workflows/release.yml
        :alt: Workflow Status
    .. image:: https://readthedocs.org/projects/erlabpy/badge/?version=latest
        :target: https://erlabpy.readthedocs.io/en/latest/
        :alt: Documentation Status
    .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
@@ -36,32 +39,32 @@
         :link: getting-started
         :link-type: doc
 
          The getting started guide provides installation instructions and an
          overview on the dependencies.
 
     .. grid-item-card::  User guide
-        :link: userguide
+        :link: user-guide/index
         :link-type: doc
 
          The user guide provides some tutorials and examples on how to use
          ERLabPy.
 
     .. grid-item-card::  API reference
         :link: reference
         :link-type: doc
 
          The reference guide provides detailed information of the API, including
          descriptions of most available methods and parameters.
 
-    .. grid-item-card::  Development guide
-        :link: development
+    .. grid-item-card::  Contributing guide
+        :link: contributing
         :link-type: doc
 
-         The development guide contains information on how to contribute to the
+         The contributing guide contains information on how to contribute to the
          project.
 
 
 .. image:: images/imagetool_light.png
     :align: center
     :alt: Imagetool
     :class: only-light
@@ -73,11 +76,11 @@
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :caption: Contents
 
    getting-started
-   userguide
+   user-guide/index
    reference
-   development
+   contributing
    bibliography
```

### Comparing `erlab-2.0.0/docs/source/notebooks/kconv.ipynb` & `erlab-2.1.0/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/notebooks/plotting.ipynb` & `erlab-2.1.0/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/pyplots/norms.py` & `erlab-2.1.0/docs/source/pyplots/norms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import numpy as np
+import erlab.plotting.erplot as eplt
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
+import numpy as np
 from pyqtgraph.colormap import modulatedBarData
 
-import erlab.plotting.erplot as eplt
-
 plt.style.use("khan")
 
 gamma = 0.3
 
 
 def example_1():
     cmap = "Greys"
```

### Comparing `erlab-2.0.0/docs/source/reference.rst` & `erlab-2.1.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/refs.bib` & `erlab-2.1.0/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/docs/source/userguide.rst` & `erlab-2.1.0/docs/source/user-guide/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 User Guide
 **********
 
 .. admonition:: Work in Progress
    :class: warning
 
    The user guide is incomplete. For the full list of packages and modules
-   provided by ERLabPy, see :doc:`reference`.
+   provided by ERLabPy, see :doc:`../reference`.
 
 This section contains some examples for getting started with ARPES data analysis
 and visualization.
 
 
 Introduction
 ============
@@ -23,20 +23,20 @@
 
 Data in ERLabPy are mostly represented by :mod:`xarray` objects
 :cite:p:`hoyer2017xarray`. The `xarray user guide
 <https://docs.xarray.dev/en/stable/index.html>`_ and the `xarray tutorial
 <https://tutorial.xarray.dev/>`_ are great resources to get started with xarray.
 
 .. toctree::
-   notebooks/io
-   notebooks/indexing
-   notebooks/plotting
-   notebooks/kconv
+   io
+   indexing
+   plotting
+   kconv
 
-Further Reading
+Further reading
 ===============
 
 - `Lectures on scientific computing with Python
   <https://github.com/jrjohansson/scientific-python-lectures>`_
 - `The beginner's guide to numpy
   <https://numpy.org/doc/stable/user/absolute_beginners.html>`_
 - `Xarray tutorial <https://tutorial.xarray.dev/>`_
```

### Comparing `erlab-2.0.0/environment.yml` & `erlab-2.1.0/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/environment_apple.yml` & `erlab-2.1.0/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/environment_nogit.yml` & `erlab-2.1.0/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/environment_nogit_mkl.yml` & `erlab-2.1.0/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/pyproject.toml` & `erlab-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 keywords = ["Condensed Matter Physics", "ARPES"]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
+dynamic = ["version"]
 dependencies = [
     "h5netcdf>=1.2.0",
     "igor2>=0.5.6",
     "iminuit>=2.25.2",
     "joblib>=1.3.2",
     "lmfit>=1.2.0",
     "matplotlib>=3.8.0",
@@ -38,25 +39,41 @@
     "scipy>=1.12.0",
     "superqt>=0.6.2",
     "tqdm>=4.66.2",
     "uncertainties>=3.0.1",
     "varname>=0.13.0",
     "xarray>=2024.02.0",
 ]
-dynamic = ["version"]
+
+[project.optional-dependencies]
+docs = [
+    "sphinx",
+    "sphinx-autodoc-typehints",
+    "sphinx-copybutton",
+    "sphinxcontrib-bibtex",
+    "pybtex",
+    "nbsphinx",
+    "furo",
+    "sphinx-design",
+]
+dev = [
+    "pytest",
+    "pytest-xdist",
+    "python-semantic-release",
+    "ruff",
+    "pre-commit",
+]
+viz = ["cmasher", "cmocean", "colorcet", "hvplot"]
 
 [project.urls]
 Documentation = "https://erlabpy.readthedocs.io"
 Repository = "https://github.com/kmnhan/erlabpy.git"
 Issues = "https://github.com/kmnhan/erlabpy/issues"
 Changelog = "https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md"
 
-[project.optional-dependencies]
-dev = ["pytest", "python-semantic-release", "ruff", "pre-commit"]
-
 [tool.setuptools]
 package-dir = { "" = "src" }
 
 [tool.setuptools.dynamic]
 version = { attr = "erlab.__version__" }
 
 [tool.setuptools_scm]
@@ -108,14 +125,15 @@
     "docs",
     "feat",
     "fix",
     "perf",
     "style",
     "refactor",
     "test",
+    "tests",
 ]
 minor_tags = ["feat"]
 patch_tags = ["fix", "perf"]
 default_bump_level = 0
 
 [tool.semantic_release.remote]
 name = "origin"
```

### Comparing `erlab-2.0.0/src/erlab/accessors.py` & `erlab-2.1.0/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/__init__.py` & `erlab-2.1.0/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/correlation.py` & `erlab-2.1.0/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.1.0/src/erlab/analysis/fit/functions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,25 +25,24 @@
     "step_linbkg_broad",
     "step_broad",
     "PolynomialFunction",
     "MultiPeakFunction",
     "FermiEdge2dFunction",
 ]
 
+from erlab.analysis.fit.functions.dynamic import (
+    FermiEdge2dFunction,
+    MultiPeakFunction,
+    PolynomialFunction,
+)
 from erlab.analysis.fit.functions.general import (
     TINY,
     do_convolve,
     do_convolve_y,
-    gaussian_wh,
-    lorentzian_wh,
     fermi_dirac,
     fermi_dirac_linbkg,
     fermi_dirac_linbkg_broad,
-    step_linbkg_broad,
+    gaussian_wh,
+    lorentzian_wh,
     step_broad,
-)
-
-from erlab.analysis.fit.functions.dynamic import (
-    PolynomialFunction,
-    MultiPeakFunction,
-    FermiEdge2dFunction,
+    step_linbkg_broad,
 )
```

### Comparing `erlab-2.0.0/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.1.0/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/fit/functions/general.py` & `erlab-2.1.0/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/fit/minuit.py` & `erlab-2.1.0/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/fit/models.py` & `erlab-2.1.0/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/fit/spline.py` & `erlab-2.1.0/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/gold.py` & `erlab-2.1.0/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/image.py` & `erlab-2.1.0/src/erlab/analysis/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     a kernel function that computes the squared difference between each element of the
     input array and the central element, divided by the corresponding distance value.
     The gradient magnitude is then calculated as the square root of the sum of the
     squared differences.
     """
 
     dxy = np.sqrt(dx**2 + dy**2)
-    dist = np.array([[dxy, dy, dxy], [dx, 1.0, dx], [dxy, dy, dxy]]).flatten()
+    dist = np.array([[dxy, dy, dxy], [dx, 0.0, dx], [dxy, dy, dxy]]).flatten()
 
     @cfunc(
         types.intc(
             types.CPointer(types.float64),
             types.intp,
             types.CPointer(types.float64),
             types.voidptr,
@@ -364,22 +364,22 @@
 
     if darr.ndim != 2:
         raise ValueError("DataArray must be 2D")
 
     xvals = darr[darr.dims[1]].values
     yvals = darr[darr.dims[0]].values
 
-    dx = xvals[1] - xvals[0]
-    dy = yvals[1] - yvals[0]
+    dx = abs(xvals[1] - xvals[0])
+    dy = abs(yvals[1] - yvals[0])
 
     grad = gradient_magnitude(
         darr.values.astype(np.float64), dx, dy, mode=mode, cval=cval
     )
-    grad[grad == 0] = np.nan
-    return darr / grad
+    grad[np.isclose(grad, 0.0)] = np.nan
+    return darr / darr.max(skipna=True) / grad
 
 
 def scaled_laplace(
     darr,
     factor: float = 1.0,
     mode: str | Sequence[str] | dict[str, str] = "nearest",
     cval: float = 0.0,
```

### Comparing `erlab-2.0.0/src/erlab/analysis/interpolate.py` & `erlab-2.1.0/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/kspace.py` & `erlab-2.1.0/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/mask/__init__.py` & `erlab-2.1.0/src/erlab/analysis/mask/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     "mask_with_polygon",
     "polygon_mask",
     "polygon_mask_points",
     "mask_with_hex_bz",
     "hex_bz_mask_points",
 ]
 
-import numpy as np
 import numba
+import numpy as np
 import xarray as xr
 
 from erlab.analysis.mask import polygon
 
 
 def mask_with_polygon(arr, vertices, dims=("kx", "ky"), invert=False):
     mask = xr.DataArray(
```

### Comparing `erlab-2.0.0/src/erlab/analysis/mask/polygon.py` & `erlab-2.1.0/src/erlab/analysis/mask/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 Polygon mask generation code adapted from the `CGAL C++ library
 <https://doc.cgal.org/5.3.2/Polygon/index.html>`_.
 
 """
 
 from __future__ import annotations
 
-from typing import Annotated, Literal
-
 import enum
+from typing import Annotated, Literal
 
+import numba
 import numpy as np
 import numpy.typing as npt
-import numba
 
 
 class Comparison(enum.Enum):
     SMALLER = -1
     EQUAL = 0
     LARGER = 1
```

### Comparing `erlab-2.0.0/src/erlab/analysis/transform.py` & `erlab-2.1.0/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/analysis/utilities.py` & `erlab-2.1.0/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/characterization/resistance.py` & `erlab-2.1.0/src/erlab/characterization/resistance.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Functions related to analyzing temperature-dependent resistance data.
 
 Currently only supports loading raw data from ``.dat`` and ``.csv`` files output by
 physics lab III equipment.
 
 """
 
-import re
 import os
+import re
 from io import StringIO
 
 import numpy as np
-import xarray as xr
 import pandas as pd
+import xarray as xr
 
 __all__ = ["load_resistance_physlab"]
 
 
 def load_resistance_physlab(path: str, **kwargs) -> xr.Dataset:
     """Loads resistance measurement acquired with physics lab III equipment.
```

### Comparing `erlab-2.0.0/src/erlab/characterization/xrd.py` & `erlab-2.1.0/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/constants.py` & `erlab-2.1.0/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/__init__.py` & `erlab-2.1.0/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/bzplot.py` & `erlab-2.1.0/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/colors.py` & `erlab-2.1.0/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/curvefittingtool.py` & `erlab-2.1.0/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/exampledata.py` & `erlab-2.1.0/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/fermiedge.py` & `erlab-2.1.0/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/controls.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/core.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.1.0/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/kspace.py` & `erlab-2.1.0/src/erlab/interactive/kspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,49 +9,24 @@
 import numpy.typing as npt
 import pyqtgraph as pg
 import varname
 import xarray as xr
 from qtpy import QtCore, QtGui, QtWidgets, uic
 
 import erlab.analysis
-from erlab.interactive.colors import BetterColorBarItem  # noqa: F401
-from erlab.interactive.colors import BetterImageItem
-from erlab.interactive.colors import ColorMapComboBox  # noqa: F401
-from erlab.interactive.colors import ColorMapGammaWidget  # noqa: F401
+from erlab.interactive.colors import (
+    BetterColorBarItem,  # noqa: F401
+    ColorMapComboBox,  # noqa: F401
+    ColorMapGammaWidget,  # noqa: F401
+)
 from erlab.interactive.imagetool import ImageTool
-from erlab.interactive.utilities import array_rect, copy_to_clipboard, gen_function_code
+from erlab.interactive.utilities import copy_to_clipboard, gen_function_code, xImageItem
 from erlab.plotting.bz import get_bz_edge
 
 
-class KspaceToolImageItem(BetterImageItem):
-    def setDataArray(self, data=None, **kargs):
-        rect = array_rect(data)
-        if self.axisOrder == "row-major":
-            img = np.ascontiguousarray(data.values)
-        else:
-            img = np.asfortranarray(data.values.T)
-        pi = self.getPlotItem()
-        if pi is not None:
-            pi.setLabel("left", data.dims[0])
-            pi.setLabel("bottom", data.dims[1])
-        self.setImage(img, rect=rect, **kargs)
-
-    def getPlotItem(self) -> pg.PlotItem | None:
-        p = self
-        while True:
-            try:
-                p = p.parentItem()
-            except RuntimeError:
-                return None
-            if p is None:
-                return None
-            if isinstance(p, pg.PlotItem):
-                return p
-
-
 class KspaceToolGUI(
     *uic.loadUiType(os.path.join(os.path.dirname(__file__), "ktool.ui"))
 ):
     def __init__(self):
         # Start the QApplication if it doesn't exist
         self.qapp = QtCore.QCoreApplication.instance()
         if not self.qapp:
@@ -60,17 +35,17 @@
 
         # Initialize UI
         super().__init__()
         self.setupUi(self)
         self.setWindowTitle("Momentum Conversion")
 
         self.plotitems: tuple[pg.PlotItem, pg.PlotItem] = (pg.PlotItem(), pg.PlotItem())
-        self.images: tuple[KspaceToolImageItem] = (
-            KspaceToolImageItem(axisOrder="row-major"),
-            KspaceToolImageItem(axisOrder="row-major"),
+        self.images: tuple[xImageItem, xImageItem] = (
+            xImageItem(axisOrder="row-major"),
+            xImageItem(axisOrder="row-major"),
         )
 
         for i, plot in enumerate(self.plotitems):
             self.graphics_layout.addItem(plot, i, 0)
             plot.addItem(self.images[i])
             plot.showGrid(x=True, y=True, alpha=0.5)
```

### Comparing `erlab-2.0.0/src/erlab/interactive/ktool.ui` & `erlab-2.1.0/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/masktool.py` & `erlab-2.1.0/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/interactive/utilities.py` & `erlab-2.1.0/src/erlab/interactive/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy.typing as npt
 import pyperclip
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtGui, QtWidgets
 from superqt import QDoubleSlider
 
-from erlab.interactive.colors import pg_colormap_powernorm
+from erlab.interactive.colors import BetterImageItem, pg_colormap_powernorm
 
 __all__ = [
     "parse_data",
     "copy_to_clipboard",
     "gen_single_function_code",
     "gen_function_code",
     "BetterSpinBox",
@@ -115,17 +115,25 @@
             if v.startswith("|") and v.endswith("|"):
                 v = v[1:-1]
             else:
                 v = f'"{v}"'
         code += f"{tab}{v},\n"
     for k, v in kwargs.items():
         if isinstance(v, str):
-            v = f'"{v}"'
+            if v.startswith("|") and v.endswith("|"):
+                v = v[1:-1]
+            else:
+                v = f'"{v}"'
         code += f"{tab}{k}={v},\n"
     code += ")"
+
+    if len(code.replace("\n", "")) <= 88:
+        # If code fits in one line, remove newlines
+        code = " ".join([s.strip() for s in code.split("\n")])
+        code = code.replace(", )", ")").replace("( ", "(")
     return code
 
 
 def gen_function_code(copy: bool = True, **kwargs: dict):
     r"""Copies the Python code for function calls to the clipboard.
 
     The result can be copied to your clipboard in a form that can be pasted into an
@@ -658,15 +666,15 @@
         if np.isfinite(self.minimum()):
             param_info["min"] = float(self.minimum())
         if np.isfinite(self.maximum()):
             param_info["max"] = float(self.maximum())
         return {self.prefix() + self.param_name: param_info}
 
 
-class xImageItem(pg.ImageItem):
+class xImageItem(BetterImageItem):
     """
     :class:`pyqtgraph.ImageItem` with additional functionality, including
     :class:`xarray.DataArray` support and auto limits based on histogram analysis.
 
     Parameters
     ----------
     image
@@ -681,15 +689,15 @@
     """
 
     sigToleranceChanged = QtCore.Signal(float, float)  #: :meta private:
 
     def __init__(self, image: npt.NDArray | None = None, **kwargs):
         super().__init__(image, **kwargs)
         self.cut_tolerance = (30, 30)
-        self.data_array = None
+        self.data_array: None | xr.DataArray = None
 
     def set_cut_tolerance(self, cut_tolerance):
         try:
             self.cut_tolerance = list(cut_tolerance.__iter__)
         except AttributeError:
             self.cut_tolerance = [cut_tolerance] * 2
         self.setImage(levels=self.data_cut_levels())
@@ -711,23 +719,68 @@
         mn, mx = max(min(pl, ql), data.min()), min(max(pu, qu), data.max())
         return (mn, mx)
 
     def setImage(self, image=None, autoLevels=None, cut_to_data=False, **kargs):
         if cut_to_data:
             kargs["levels"] = self.data_cut_levels(data=image)
         super().setImage(image=image, autoLevels=autoLevels, **kargs)
+        self.data_array = None
 
-    def setDataArray(self, data=None, **kargs):
-        self.data_array = parse_data(data)
-        rect = array_rect(self.data_array)
+    def setDataArray(self, data: xr.DataArray, update_labels: bool = True, **kargs):
+        rect = array_rect(data)
         if self.axisOrder == "row-major":
-            img = np.ascontiguousarray(self.data_array.values)
+            img = np.ascontiguousarray(data.values)
         else:
-            img = np.asfortranarray(self.data_array.values.T)
+            img = np.asfortranarray(data.values.T)
+
+        if update_labels:
+            pi = self.getPlotItem()
+            if pi is not None:
+                pi.setLabel("left", data.dims[0])
+                pi.setLabel("bottom", data.dims[1])
+
         self.setImage(img, rect=rect, **kargs)
+        self.data_array = data
+
+    def getMenu(self):
+        if self.menu is None:
+            if not self.removable:
+                self.menu = QtWidgets.QMenu()
+            else:
+                super().getMenu()
+            if self.menu is not None:
+                itoolAct = QtGui.QAction("Open in ImageTool", self.menu)
+                itoolAct.triggered.connect(self.open_itool)
+                self.menu.addAction(itoolAct)
+                self.menu.itoolAct = itoolAct
+        return self.menu
+
+    def getPlotItem(self) -> pg.PlotItem | None:
+        p = self
+        while True:
+            try:
+                p = p.parentItem()
+            except RuntimeError:
+                return None
+            if p is None:
+                return None
+            if isinstance(p, pg.PlotItem):
+                return p
+
+    def open_itool(self):
+        from erlab.interactive.imagetool import ImageTool
+
+        if self.data_array is None:
+            if self.image is None:
+                return
+            da = xr.DataArray(np.asarray(self.image)).T
+        else:
+            da = self.data_array.T
+        self._itool = ImageTool(da)
+        self._itool.show()
 
 
 class ParameterGroup(QtWidgets.QGroupBox):
     """Easy creation of groupboxes with multiple varying parameters.
 
     Can be used in many different interactive tools for dynamic data analysis.
```

### Comparing `erlab-2.0.0/src/erlab/io/__init__.py` & `erlab-2.1.0/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/io/dataloader.py` & `erlab-2.1.0/src/erlab/io/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from __future__ import annotations
 
 import contextlib
 import datetime
 import itertools
 import os
+import warnings
 from typing import TYPE_CHECKING
 
 import joblib
 import numpy as np
 import numpy.typing as npt
 import pandas
 import xarray as xr
@@ -47,14 +48,18 @@
     return np.all(dif >= 0) or np.all(dif <= 0)
 
 
 class ValidationError(Exception):
     """This exception is raised when the loaded data fails validation checks."""
 
 
+class ValidationWarning(UserWarning):
+    """This warning is issued when the loaded data fails validation checks."""
+
+
 class LoaderBase:
     """Base class for all data loaders."""
 
     name: str | None = None
     """
     Name of the loader. Using a unique and descriptive name is recommended. For easy
     access, it is recommended to use a name that passes :func:`str.isidentifier`.
@@ -89,14 +94,20 @@
     If `True`, this indicates that all individual scans always lead to a single data
     file. No concatenation of data from multiple files will be performed.
     """
 
     skip_validate: bool = False
     """If `True`, validation checks will be skipped."""
 
+    strict_validation: bool = False
+    """
+    If `True`, validation check will raise a `ValidationError` on the first failure
+    instead of warning. Useful for debugging data loaders.
+    """
+
     @property
     def name_map_reversed(self) -> dict[str, str]:
         """A reversed version of the name_map dictionary."""
         return self.reverse_mapping(self.name_map)
 
     @staticmethod
     def reverse_mapping(mapping: dict[str, str | Iterable[str]]) -> dict[str, str]:
@@ -306,20 +317,20 @@
             given, it is assumed to be the path to the data file. If an integer is
             given, it is assumed to be a number that specifies the scan number, and is
             used to automatically determine the path to the data file(s).
         data_dir
             Where to look for the data. If `None`, the default data directory will be
             used.
         single
-            For some endstations, data for a single scan is saved over multiple files.
-            This argument only has effect for such endstations. When a single file
-            within a multiple file scan is provided to `identifier`, the default
-            behavior when `single` is `False` is to infer the coordinates and return a
-            single concatenated array that contains data from all files. If `single` is
-            set to `True`, only the data from the file given is returned.
+            For some setups, data for a single scan is saved over multiple files. This
+            argument is only used for such setups. When `identifier` is resolved to a
+            single file within a multiple file scan, the default behavior when `single`
+            is `False` is to return a single concatenated array that contains data from
+            all files in the same scan. If `single` is set to `True`, only the data from
+            the file given is returned.
         **kwargs
             Additional keyword arguments are passed to `identify`.
 
         Returns
         -------
         xarray.DataArray or xarray.Dataset or list of xarray.DataArray
             The loaded data.
@@ -599,15 +610,16 @@
         return data
 
     @classmethod
     def validate(cls, data: xr.DataArray | xr.Dataset):
         """Validate the input data to ensure it is in the correct format.
 
         Checks for the presence of all required coordinates and attributes. If the data
-        does not pass validation, a `ValidationError` is raised. Validation is skipped
+        does not pass validation, a `ValidationError` is raised or a warning is issued,
+        depending on the value of the `strict_validation` flag. Validation is skipped
         for loaders with attribute `skip_validate` set to `True`.
 
         Parameters
         ----------
         data
             The data to be validated.
 
@@ -624,31 +636,34 @@
         if isinstance(data, xr.Dataset):
             for v in data.data_vars.values():
                 cls.validate(v)
             return
 
         for c in ("alpha", "beta", "delta", "xi", "hv"):
             if c not in data.coords:
-                raise ValidationError(f"Missing coordinate {c}")
-                # print(f"Missing coordinate {c}")
+                cls._raise_or_warn(f"Missing coordinate {c}")
 
         for a in ("configuration", "temp_sample"):
             if a not in data.attrs:
-                raise ValidationError(f"Missing attribute {c}")
-                # print(f"Missing attribute {a}")
+                cls._raise_or_warn(f"Missing attribute {c}")
 
         if data.attrs["configuration"] not in (1, 2):
             if data.attrs["configuration"] not in (3, 4):
-                raise ValidationError(
+                cls._raise_or_warn(
                     f"Invalid configuration {data.attrs['configuration']}"
                 )
-                # print(f"Invalid configuration {data.attrs['configuration']}")
             elif "chi" not in data.coords:
-                raise ValidationError("Missing coordinate chi")
-                # print("Missing coordinate chi")
+                cls._raise_or_warn("Missing coordinate chi")
+
+    @classmethod
+    def _raise_or_warn(cls, msg: str):
+        if cls.strict_validation:
+            raise ValidationError(msg)
+        else:
+            warnings.warn(msg, ValidationWarning, stacklevel=2)
 
     def _load_multiple_parallel(
         self, file_paths: list[str]
     ) -> list[xr.DataArray | xr.Dataset]:
         if len(file_paths) < 15:
             n_jobs = 1
         else:
```

### Comparing `erlab-2.0.0/src/erlab/io/igor.py` & `erlab-2.1.0/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/io/plugins/__init__.py` & `erlab-2.1.0/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/io/plugins/da30.py` & `erlab-2.1.0/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/io/plugins/kriss.py` & `erlab-2.1.0/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/io/plugins/merlin.py` & `erlab-2.1.0/src/erlab/io/plugins/merlin.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Data loader for beamline 4.0.3 at ALS."""
 
+import datetime
 import glob
 import os
 import re
-import datetime
+
 import numpy as np
 import numpy.typing as npt
-import xarray as xr
 import pandas as pd
-
+import xarray as xr
 
 import erlab.io.utilities
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
 
 
 class BL403Loader(LoaderBase):
```

### Comparing `erlab-2.0.0/src/erlab/io/plugins/ssrl52.py` & `erlab-2.1.0/src/erlab/io/plugins/ssrl52.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Data loader for beamline 5-2 at SSRL."""
 
+import datetime
 import os
 import re
-import datetime
+
+import h5netcdf
 import numpy as np
 import numpy.typing as npt
-import xarray as xr
-import h5netcdf
 import pandas as pd
-
+import xarray as xr
 
 import erlab.io.utilities
 from erlab.io.dataloader import LoaderBase
 
 
 class SSRL52Loader(LoaderBase):
     name: str = "ssrl"
```

### Comparing `erlab-2.0.0/src/erlab/io/utilities.py` & `erlab-2.1.0/src/erlab/io/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import os
-import warnings
-from collections.abc import Sequence
-
-import numpy as np
-import xarray as xr
-
 __all__ = [
     "showfitsinfo",
     "get_files",
     "open_hdf5",
     "load_hdf5",
     "save_as_hdf5",
     "save_as_netcdf",
 ]
 
+import os
+import warnings
+from collections.abc import Sequence
+
+import numpy as np
+import xarray as xr
+
 
 def showfitsinfo(path: str | os.PathLike):
     """Prints raw metadata from a ``.fits`` file.
 
     Parameters
     ----------
     path
@@ -108,21 +108,49 @@
                     f"The attribute {key} with invalid type {dt} will be removed",
                     stacklevel=1,
                 )
     return da
 
 
 def open_hdf5(filename: str | os.PathLike) -> xr.DataArray | xr.Dataset:
+    """Open data from an HDF5 file saved with `save_as_hdf5`.
+
+    This is a thin wrapper around `xarray.open_dataarray` and `xarray.open_dataset`.
+
+    Parameters
+    ----------
+    filename
+        The path to the HDF5 file.
+
+    Returns
+    -------
+    xarray.DataArray or xarray.Dataset
+        The opened data.
+    """
     try:
         return xr.open_dataarray(filename, engine="h5netcdf")
     except ValueError:
         return xr.open_dataset(filename, engine="h5netcdf")
 
 
 def load_hdf5(filename: str | os.PathLike) -> xr.DataArray | xr.Dataset:
+    """Load data from an HDF5 file saved with `save_as_hdf5`.
+
+    This is a thin wrapper around `xarray.load_dataarray` and `xarray.load_dataset`.
+
+    Parameters
+    ----------
+    filename
+        The path to the HDF5 file.
+
+    Returns
+    -------
+    xarray.DataArray or xarray.Dataset
+        The loaded data.
+    """
     try:
         return xr.load_dataarray(filename, engine="h5netcdf")
     except ValueError:
         return xr.load_dataset(filename, engine="h5netcdf")
 
 
 def save_as_hdf5(
```

### Comparing `erlab-2.0.0/src/erlab/lattice.py` & `erlab-2.1.0/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/parallel.py` & `erlab-2.1.0/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.1.0/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.1.0/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/__init__.py` & `erlab-2.1.0/src/erlab/plotting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import pkgutil
 
 import matplotlib
 import matplotlib.colors
 import matplotlib.font_manager
 import matplotlib.style
 import numpy as np
+
 import erlab.io
 
 # Import colormaps if available
 if importlib.util.find_spec("cmasher"):
     importlib.import_module("cmasher")
 if importlib.util.find_spec("cmocean"):
     importlib.import_module("cmocean")
```

### Comparing `erlab-2.0.0/src/erlab/plotting/annotations.py` & `erlab-2.1.0/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/atoms.py` & `erlab-2.1.0/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/bz.py` & `erlab-2.1.0/src/erlab/plotting/bz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Utilities for plotting Brillouin zones."""
 
 __all__ = ["get_bz_edge", "plot_hex_bz"]
 
+import itertools
+
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
-import itertools
 import scipy.spatial
 from matplotlib.patches import RegularPolygon
 
 from erlab.plotting.colors import axes_textcolor
 
 abbrv_kws = {
     "facecolor": ["fc", "none"],
```

### Comparing `erlab-2.0.0/src/erlab/plotting/colors.py` & `erlab-2.1.0/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/erplot.py` & `erlab-2.1.0/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/general.py` & `erlab-2.1.0/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/plot3d.py` & `erlab-2.1.0/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.1.0/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.1.0/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.1.0/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.1.0/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.1.0/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.1.0/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/src/erlab.egg-info/PKG-INFO` & `erlab-2.1.0/src/erlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,15 +683,15 @@
 Project-URL: Issues, https://github.com/kmnhan/erlabpy/issues
 Project-URL: Changelog, https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md
 Keywords: Condensed Matter Physics,ARPES
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
@@ -710,37 +710,55 @@
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: superqt>=0.6.2
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: uncertainties>=3.0.1
 Requires-Dist: varname>=0.13.0
 Requires-Dist: xarray>=2024.02.0
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: pybtex; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: viz
+Requires-Dist: cmasher; extra == "viz"
+Requires-Dist: cmocean; extra == "viz"
+Requires-Dist: colorcet; extra == "viz"
+Requires-Dist: hvplot; extra == "viz"
 
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/erlab.svg)](https://anaconda.org/conda-forge/erlab)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kmnhan/erlabpy/main.svg)](https://results.pre-commit.ci/latest/github/kmnhan/erlabpy/main)
 
 A library that provides a set of tools and utilities to handle, manipulate, and
 visualize data from condensed matter physics experiments, with a focus on
 angle-resolved photoemission spectroscopy (ARPES).
 
-*ERLabPy* is built on top of the popular scientific computing libraries `numpy`,
-`scipy`, and `xarray`, and is designed to be easy to use and integrate with
-existing scientific Python workflows. It is also designed to be extensible,
-allowing users to easily add custom functionality and analysis tools.
+*ERLabPy* is built on top of the popular scientific computing libraries
+[*numpy*](https://numpy.org/), [*scipy*](https://scipy.org/), and
+[*xarray*](https://xarray.pydata.org/), and is designed to be easy to use and
+integrate with existing scientific Python workflows. It is also designed to be
+extensible, allowing users to easily add custom functionality and analysis
+tools.
 
 *ERLabPy* is developed and maintained by the electronic structure research
 laboratory at Korea Advanced Institute of Science and Technology (KAIST).
 
 ## Features
 
 - **Data Loading**: A flexible and extensible data loading system is included,
@@ -773,29 +791,28 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_dark.png?raw=true">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_light.png?raw=true">
   <img alt="Imagetool in action." src="https://github.com/kmnhan/erlabpy/blob/main/docs/source/images/ktool_1_light.png?raw=true">
 </picture>
 
 
-## Documentation
+## Getting Started
 
-The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
+To get started, see [installation instructions](https://erlabpy.readthedocs.io/en/stable/getting-started.html).
 
-## Getting Started
+## Documentation
 
-To get started with ERLab, follow the [installation instructions](https://erlabpy.readthedocs.io/en/stable/getting-started.html).
+The full documentation for ERLabPy is available on [Read the Docs](https://erlabpy.readthedocs.io/).
 
 ## Contributing
 
-Contributions are welcome! Please open an issue or pull request if you have any
-suggestions or improvements. For more information on contributing, see the
-[development guide](https://erlabpy.readthedocs.io/en/stable/development.html).
+ERLabPy is an open-source project and we welcome contributions from the
+community. If you find any bugs, issues, or have any suggestions, please open an
+issue [here](https://github.com/kmnhan/erlabpy/issues). If you would like to add
+a new feature or fix a bug yourself, we would love to have your contribution.
+Feel free to fork the repository and submit a pull request with your changes.
+
+For more information on contributing, see our [Contributing page](https://erlabpy.readthedocs.io/en/stable/contributing.html).
 
 ## License
 
 This project is licensed under the terms of the [GPL-3.0 License](LICENSE).
-
-## Contact
-
-If you have any questions, issues, or suggestions, please open an issue
-[here](https://github.com/kmnhan/erlabpy/issues). We appreciate your feedback!
```

### Comparing `erlab-2.0.0/src/erlab.egg-info/SOURCES.txt` & `erlab-2.1.0/src/erlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,40 +17,40 @@
 .github/workflows/release.yml
 docs/Makefile
 docs/environment.yml
 docs/make.bat
 docs/requirements.txt
 docs/source/bibliography.rst
 docs/source/conf.py
-docs/source/development.rst
+docs/source/contributing.rst
 docs/source/erlab.accessors.rst
 docs/source/erlab.analysis.rst
 docs/source/erlab.characterization.rst
 docs/source/erlab.constants.rst
 docs/source/erlab.interactive.rst
 docs/source/erlab.io.rst
 docs/source/erlab.lattice.rst
 docs/source/erlab.parallel.rst
 docs/source/erlab.plotting.rst
 docs/source/getting-started.rst
 docs/source/index.rst
 docs/source/reference.rst
 docs/source/refs.bib
-docs/source/userguide.rst
 docs/source/images/imagetool_dark.png
 docs/source/images/imagetool_light.png
 docs/source/images/ktool_1_dark.png
 docs/source/images/ktool_1_light.png
 docs/source/images/ktool_2_dark.png
 docs/source/images/ktool_2_light.png
-docs/source/notebooks/indexing.ipynb
-docs/source/notebooks/io.ipynb
-docs/source/notebooks/kconv.ipynb
-docs/source/notebooks/plotting.ipynb
 docs/source/pyplots/norms.py
+docs/source/user-guide/index.rst
+docs/source/user-guide/indexing.ipynb
+docs/source/user-guide/io.ipynb
+docs/source/user-guide/kconv.ipynb
+docs/source/user-guide/plotting.ipynb
 src/erlab/__init__.py
 src/erlab/accessors.py
 src/erlab/constants.py
 src/erlab/lattice.py
 src/erlab/parallel.py
 src/erlab.egg-info/PKG-INFO
 src/erlab.egg-info/SOURCES.txt
@@ -78,14 +78,15 @@
 src/erlab/characterization/resistance.py
 src/erlab/characterization/xrd.py
 src/erlab/interactive/__init__.py
 src/erlab/interactive/bzplot.py
 src/erlab/interactive/colors.py
 src/erlab/interactive/curvefittingtool.py
 src/erlab/interactive/derivative.py
+src/erlab/interactive/dtool.ui
 src/erlab/interactive/exampledata.py
 src/erlab/interactive/fermiedge.py
 src/erlab/interactive/kspace.py
 src/erlab/interactive/ktool.ui
 src/erlab/interactive/masktool.py
 src/erlab/interactive/utilities.py
 src/erlab/interactive/imagetool/__init__.py
```

### Comparing `erlab-2.0.0/templates/.macros.j2` & `erlab-2.1.0/templates/.macros.j2`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% macro render_single_commit(commit) -%}
-* {% if commit["scope"] is not none %}**{{ commit["scope"] }}** {% endif %}{{ commit["descriptions"][0].rstrip() }} ([`{{commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
-{% for line in commit["descriptions"][1:] %}
-{{ line | indent(2, first=True, blank=True) -}}
-{% endfor %}
+* {% if commit["scope"] is not none %}(**{{ commit["scope"] }}**) {% endif %}{{ commit["descriptions"][0].rstrip() }} ([`{{commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
+{% for line in commit["descriptions"][1:] %}{% if line | trim != "" %}
+{{ line.strip() | indent(2, first=True, blank=True) -}}
+{% endif %}{% endfor %}
 {%- endmacro %}
 
 {% macro render_unknown_commit(commit) -%}
 * {{ commit.message.rstrip().split("\n")[0] }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
-{% for line in commit.message.rstrip().split("\n")[1:] %}
-{{ line | indent(2, first=True, blank=True) -}}
-{% endfor %}
+{% for line in commit.message.rstrip().split("\n")[1:] %}{% if line | trim != "" %}
+{{ line.strip() | indent(2, first=True, blank=True) -}}
+{% endif %}{% endfor %}
 {%- endmacro %}
 
 {%- macro render_elements(elements) -%}
 {% for type_, commits in elements | dictsort %}
 ### {{ type_ | capitalize }}
 {% for commit in commits -%}{% if type_ != "unknown" %}
 {{ render_single_commit(commit).rstrip() }}
```

### Comparing `erlab-2.0.0/tests/test_fastbinning.py` & `erlab-2.1.0/tests/test_fastbinning.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from erlab.interactive.imagetool.fastbinning import nanmean_funcs, fast_nanmean
+from erlab.interactive.imagetool.fastbinning import fast_nanmean, nanmean_funcs
 
 
 def test_fast_nanmean():
     for nd, funcs in nanmean_funcs.items():
         x = np.random.RandomState(42).randn(*((10,) * nd))
         for axis, func in funcs.items():
             if isinstance(axis, frozenset):
```

### Comparing `erlab-2.0.0/tests/test_fit_functions_dynamic.py` & `erlab-2.1.0/tests/test_fit_functions_dynamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import pytest
 import xarray as xr
-
 from erlab.analysis.fit.functions.dynamic import (
     FermiEdge2dFunction,
     MultiPeakFunction,
     PolynomialFunction,
 )
 from erlab.analysis.fit.functions.general import gaussian_wh, lorentzian_wh
```

### Comparing `erlab-2.0.0/tests/test_fit_functions_general.py` & `erlab-2.1.0/tests/test_fit_functions_general.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
+import pytest
 import scipy.special
 from erlab.analysis.fit.functions.general import (
     _gen_kernel,
     do_convolve,
     fermi_dirac,
     fermi_dirac_linbkg,
     fermi_dirac_linbkg_broad,
     gaussian_wh,
     lorentzian_wh,
     step_broad,
     step_linbkg_broad,
 )
-import pytest
 
 KB_EV = 8.617333262145179e-5
 
 
 def test_gen_kernel():
     # Define test input values
     x = np.array([0, 1, 2, 3, 4])
```

### Comparing `erlab-2.0.0/tests/test_image.py` & `erlab-2.1.0/tests/test_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import erlab.analysis as era
 import numpy as np
 import xarray as xr
-import erlab.analysis as era
 
 
 def test_gaussian_filter():
     # Create a test input DataArray
     darr = xr.DataArray(np.arange(50, step=2).reshape((5, 5)), dims=["x", "y"])
 
     # Define the expected output
@@ -103,19 +103,19 @@
     # Create a test input DataArray
     darr = xr.DataArray(np.arange(50, step=2).reshape((5, 5)), dims=["x", "y"])
 
     # Define the expected output
     expected_output = xr.DataArray(
         np.array(
             [
-                [0.0, 0.13608276, 0.27216553, 0.40824829, 0.58345997],
-                [0.49507377, 0.58834841, 0.68640647, 0.78446454, 0.89113279],
-                [0.99014754, 1.07863874, 1.17669681, 1.27475488, 1.38620656],
-                [1.48522131, 1.56892908, 1.66698715, 1.76504522, 1.88128033],
-                [2.91729983, 2.85773803, 2.9938208, 3.12990356, 3.17887766],
+                [0.0, 0.00283506, 0.00567012, 0.00850517, 0.01215542],
+                [0.01031404, 0.01225726, 0.01430013, 0.01634301, 0.01856527],
+                [0.02062807, 0.02247164, 0.02451452, 0.02655739, 0.0288793],
+                [0.03094211, 0.03268602, 0.0347289, 0.03677177, 0.03919334],
+                [0.06077708, 0.05953621, 0.06237127, 0.06520633, 0.06622662],
             ]
         ),
         dims=["x", "y"],
     )
 
     # Apply the minimum_gradient function
     result = era.image.minimum_gradient(darr).astype(np.float32)
```

### Comparing `erlab-2.0.0/tests/test_interpolate.py` & `erlab-2.1.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/tests/test_kspace.py` & `erlab-2.1.0/tests/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.0.0/tests/test_utilities.py` & `erlab-2.1.0/tests/test_utilities.py`

 * *Files identical despite different names*

