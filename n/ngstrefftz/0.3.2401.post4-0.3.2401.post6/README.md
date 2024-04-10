# Comparing `tmp/ngstrefftz-0.3.2401.post4.tar.gz` & `tmp/ngstrefftz-0.3.2401.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-0.3.2401.post4.tar", last modified: Thu Feb 15 13:36:38 2024, max compression
+gzip compressed data, was "ngstrefftz-0.3.2401.post6.tar", last modified: Tue Feb 20 08:53:33 2024, max compression
```

## Comparing `ngstrefftz-0.3.2401.post4.tar` & `ngstrefftz-0.3.2401.post6.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.573365 ngstrefftz-0.3.2401.post4/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.549364 ngstrefftz-0.3.2401.post4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.553364 ngstrefftz-0.3.2401.post4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/build_linux_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/ngsolve_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.553364 ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/build_in_docker.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-15 13:36:38.573365 ngstrefftz-0.3.2401.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.553364 ngstrefftz-0.3.2401.post4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.553364 ngstrefftz-0.3.2401.post4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/_static/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.553364 ngstrefftz-0.3.2401.post4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/_static/css/mytheme.css
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/docu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.557364 ngstrefftz-0.3.2401.post4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-adv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-helm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-poi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-stokes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-wave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/helmholtz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/laplace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/qtwave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/tunfitted.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/twave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/notebooks/twavetents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.557364 ngstrefftz-0.3.2401.post4/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/paper/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.549364 ngstrefftz-0.3.2401.post4/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.557364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.549364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.557364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.549364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.557364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/burgers1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/burgers2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/euler2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/maxwell/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/tents/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/tents/draw3dtent.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/tents/draw3dvertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/horn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/wave2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/wave3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.561364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/BurgersMTP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/INDEX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/StartPitching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.565364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/CausalityCond.png
--rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/dag.png
--rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/subtents.png
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.565364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.565364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/conslaw/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/conslaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.565364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/utils/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/utils/_drawtents2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.569364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.569364 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_burgers_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_causal_tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_conslaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_tent_height_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-15 13:36:07.000000 ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_tentlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 13:36:38.573365 ngstrefftz-0.3.2401.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.573365 ngstrefftz-0.3.2401.post4/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26205 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/monomialfespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.573365 ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-15 13:36:38.000000 ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-02-15 13:36:38.000000 ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 13:36:38.000000 ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-15 13:36:38.000000 ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-15 13:36:38.000000 ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/ngsttd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    48796 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    61083 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/specialintegrator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/specialintegrator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    51524 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    44030 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:36:38.573365 ngstrefftz-0.3.2401.post4/test/
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-02-15 13:36:05.000000 ngstrefftz-0.3.2401.post4/test/trefftz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.361580 ngstrefftz-0.3.2401.post6/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.333580 ngstrefftz-0.3.2401.post6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.337580 ngstrefftz-0.3.2401.post6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/build_linux_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/ngsolve_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.341580 ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/build_in_docker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-20 08:53:33.361580 ngstrefftz-0.3.2401.post6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.341580 ngstrefftz-0.3.2401.post6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.341580 ngstrefftz-0.3.2401.post6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/_static/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.341580 ngstrefftz-0.3.2401.post6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/_static/css/mytheme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/docu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.341580 ngstrefftz-0.3.2401.post6/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-adv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-helm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-poi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-stokes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-wave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/helmholtz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/laplace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/qtwave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/tunfitted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/twave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/notebooks/twavetents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.333580 ngstrefftz-0.3.2401.post6/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.333580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.337580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/burgers1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/burgers2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/euler2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.345580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/tents/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/tents/draw3dtent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/tents/draw3dvertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.349580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/horn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/wave2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/wave3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.349580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/BurgersMTP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/INDEX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/StartPitching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.349580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/CausalityCond.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/dag.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/subtents.png
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.349580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.349580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/conslaw/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/conslaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.349580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/utils/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/utils/_drawtents2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.353580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.353580 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_burgers_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_causal_tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_conslaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_tent_height_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-20 08:53:02.000000 ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_tentlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 08:53:33.361580 ngstrefftz-0.3.2401.post6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.357580 ngstrefftz-0.3.2401.post6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26412 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/monomialfespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.361580 ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-20 08:53:33.000000 ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-02-20 08:53:33.000000 ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 08:53:33.000000 ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-20 08:53:33.000000 ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-20 08:53:33.000000 ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/ngsttd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    48796 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    61083 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/specialintegrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/specialintegrator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    51524 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    44030 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:53:33.357580 ngstrefftz-0.3.2401.post6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-02-20 08:53:01.000000 ngstrefftz-0.3.2401.post6/test/trefftz.py
```

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/build.yml` & `ngstrefftz-0.3.2401.post6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/build_linux_test.sh` & `ngstrefftz-0.3.2401.post6/.github/workflows/build_linux_test.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2401.post6/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2401.post6/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2401.post6/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2401.post6/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/Dockerfile` & `ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/build_in_docker.sh` & `ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/build_in_docker.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/merge.py` & `ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/merge.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/.github/workflows/pyodide/requirements.txt` & `ngstrefftz-0.3.2401.post6/.github/workflows/pyodide/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/CONTRIBUTING.md` & `ngstrefftz-0.3.2401.post6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/Dockerfile` & `ngstrefftz-0.3.2401.post6/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/LICENSE` & `ngstrefftz-0.3.2401.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/PKG-INFO` & `ngstrefftz-0.3.2401.post6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2401.post4
+Version: 0.3.2401.post6
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2401.post24.dev0
```

### Comparing `ngstrefftz-0.3.2401.post4/README.md` & `ngstrefftz-0.3.2401.post6/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/conf.py` & `ngstrefftz-0.3.2401.post6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/docu.rst` & `ngstrefftz-0.3.2401.post6/docs/docu.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/index.rst` & `ngstrefftz-0.3.2401.post6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/intro.rst` & `ngstrefftz-0.3.2401.post6/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-adv.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-adv.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-helm.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-helm.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-poi.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-poi.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-stokes.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-stokes.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz-wave.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz-wave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/embTrefftz.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/embTrefftz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/helmholtz.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/helmholtz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/index.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/laplace.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/laplace.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/qtwave.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/qtwave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/tunfitted.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/tunfitted.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/twave.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/twave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/notebooks/twavetents.ipynb` & `ngstrefftz-0.3.2401.post6/docs/notebooks/twavetents.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/paper/codemeta.json` & `ngstrefftz-0.3.2401.post6/docs/paper/codemeta.json`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/paper/paper.bib` & `ngstrefftz-0.3.2401.post6/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/paper/paper.md` & `ngstrefftz-0.3.2401.post6/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/docs/requirements.txt` & `ngstrefftz-0.3.2401.post6/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build.yml` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/README.md` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/advection2d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/advection/advection2d_periodic.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/advection/advection2d_periodic.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/burgers1d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/burgers1d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/burgers/burgers2d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/burgers/burgers2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/euler2d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/euler2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/maxwell/maxwell3d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/maxwell/maxwell3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/tents/draw3dtent.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/tents/draw3dtent.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/tents/draw3dvertex.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/tents/draw3dvertex.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/horn.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/horn.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/wave2d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/wave2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/demo/wave/wave3d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/demo/wave/wave3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/BurgersMTP.ipynb` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/BurgersMTP.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/INDEX.ipynb` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/INDEX.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/StartPitching.ipynb` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/StartPitching.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/conf.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/CausalityCond.png` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/CausalityCond.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/dag.png` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/dag.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/map.png` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/map.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/figs/subtents.png` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/figs/subtents.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/index.rst` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/docs/requirements.txt` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/conslaw/__init__.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/conslaw/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/utils/_drawtents.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/utils/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/py/utils/_drawtents2d.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/py/utils/_drawtents2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/setup.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_burgers_2D.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_burgers_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_causal_tents.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_causal_tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_conslaw.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_conslaw.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_tent_height_2D.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_tent_height_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/external_dependencies/ngstents/tests/test_tentlayers.py` & `ngstrefftz-0.3.2401.post6/external_dependencies/ngstents/tests/test_tentlayers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/setup.py` & `ngstrefftz-0.3.2401.post6/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/CMakeLists.txt` & `ngstrefftz-0.3.2401.post6/src/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,25 @@
 endif(WIN32)
 #target_compile_options(_trefftz PRIVATE "$<$<CONFIG:DEBUG>:-W;-Wall;-Wextra;-Wpedantic;-Wno-unused-parameter;-g;>")
 #set_target_properties(_trefftz PROPERTIES COMPILE_DEFINITIONS "NGSTREFFTZ_EXPORTS")
 set(NGSTREFFTZ_USE_LAPACK ${NGSOLVE_USE_LAPACK} CACHE BOOL "Try to use lapack from ngsolve")
 if(NGSTREFFTZ_USE_LAPACK AND NOT WIN32)
     target_compile_definitions(_trefftz PRIVATE NGSTREFFTZ_USE_LAPACK)
 endif()
+if(USE_MKL AND NGSOLVE_USE_MKL)
+    find_package(MKL REQUIRED)
+    if(APPLE OR WIN32)
+      set(MKL_RT_NAME mkl_rt.2)
+    else()
+      set(MKL_RT_NAME libmkl_rt.so.2)
+    endif()
+    find_library(MKLRT ${MKL_RT_NAME} HINTS ${MKL_ROOT}/lib)
+    message("Linking with MKL_RT=${MKLRT}")
+    target_link_libraries(_trefftz PUBLIC ${MKLRT})
+endif()
 target_compile_definitions(_trefftz PRIVATE NGSTREFFTZ_EXPORTS)
 target_link_libraries(_trefftz PRIVATE _pytents)
 set_target_properties(_trefftz PROPERTIES
     LIBRARY_OUTPUT_DIRECTORY "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/ngstrefftz"
 )
 file(COPY ${CMAKE_SOURCE_DIR}/__init__.py DESTINATION ${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/ngstrefftz)
```

### Comparing `ngstrefftz-0.3.2401.post4/src/__init__.py` & `ngstrefftz-0.3.2401.post6/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/airy.cpp` & `ngstrefftz-0.3.2401.post6/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/diffopmapped.hpp` & `ngstrefftz-0.3.2401.post6/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/embtrefftz.cpp` & `ngstrefftz-0.3.2401.post6/src/embtrefftz.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -146,20 +146,17 @@
 
     vector<shared_ptr<Matrix<SCAL>>> ETmats (ne);
     VVector<SCAL> lfvec (ndof);
     lfvec = 0.0;
 
     size_t active_elements = 0;
     size_t test_local_ndof = test_fes->GetNDof () / ne;
-    Vector<SCAL> sing_val_avg (test_local_ndof);
-    sing_val_avg = 0;
-    Vector<double> sing_val_max (test_local_ndof);
-    sing_val_max = 0;
-    Vector<double> sing_val_min (test_local_ndof);
-    sing_val_min = DBL_MAX;
+    Vector<SCAL> sing_val_avg;
+    Vector<double> sing_val_max;
+    Vector<double> sing_val_min;
 
     bool has_hidden_dofs = false;
     for (DofId d = 0; d < ndof || !has_hidden_dofs; d++)
       if (HIDDEN_DOF == fes->GetDofCouplingType (d))
         has_hidden_dofs = true;
 
     ma->IterateElements (VOL, lh, [&] (auto ei, LocalHeap &mlh) {
@@ -266,14 +263,23 @@
             = make_shared<Matrix<SCAL>> (U.Cols (0, dofs.Size () - nz));
       else
         ETmats[ei.Nr ()] = make_shared<Matrix<SCAL>> (
             Trans (Vt.Rows (dofs.Size () - nz, dofs.Size ())));
 
       if (stats)
         {
+          if (sing_val_avg.Size () == 0)
+            {
+              sing_val_avg.SetSize (elmat.Height ());
+              sing_val_max.SetSize (elmat.Height ());
+              sing_val_min.SetSize (elmat.Height ());
+              sing_val_avg = 0;
+              sing_val_max = 0;
+              sing_val_min = DBL_MAX;
+            }
           active_elements += 1;
           for (size_t i = 0; i < elmat.Height (); i++)
             {
               sing_val_avg[i] += elmat (i, i);
               sing_val_max[i] = max (sing_val_max[i], abs (elmat (i, i)));
               sing_val_min[i] = min (sing_val_min[i], abs (elmat (i, i)));
             }
```

### Comparing `ngstrefftz-0.3.2401.post4/src/embtrefftz.hpp` & `ngstrefftz-0.3.2401.post6/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/mesh1dtents.cpp` & `ngstrefftz-0.3.2401.post6/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/monomialfespace.cpp` & `ngstrefftz-0.3.2401.post6/src/monomialfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/monomialfespace.hpp` & `ngstrefftz-0.3.2401.post6/src/monomialfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/PKG-INFO` & `ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2401.post4
+Version: 0.3.2401.post6
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2401.post24.dev0
```

### Comparing `ngstrefftz-0.3.2401.post4/src/ngstrefftz.egg-info/SOURCES.txt` & `ngstrefftz-0.3.2401.post6/src/ngstrefftz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/planewavefe.cpp` & `ngstrefftz-0.3.2401.post6/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/planewavefe.hpp` & `ngstrefftz-0.3.2401.post6/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/python_trefftz.cpp` & `ngstrefftz-0.3.2401.post6/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/scalarmappedfe.cpp` & `ngstrefftz-0.3.2401.post6/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/scalarmappedfe.hpp` & `ngstrefftz-0.3.2401.post6/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/specialcoefficientfunction.cpp` & `ngstrefftz-0.3.2401.post6/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/specialcoefficientfunction.hpp` & `ngstrefftz-0.3.2401.post6/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/specialintegrator.cpp` & `ngstrefftz-0.3.2401.post6/src/specialintegrator.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/specialintegrator.hpp` & `ngstrefftz-0.3.2401.post6/src/specialintegrator.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/trefftzfespace.cpp` & `ngstrefftz-0.3.2401.post6/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/trefftzfespace.hpp` & `ngstrefftz-0.3.2401.post6/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/twavetents.cpp` & `ngstrefftz-0.3.2401.post6/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/src/twavetents.hpp` & `ngstrefftz-0.3.2401.post6/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/test/embt.py` & `ngstrefftz-0.3.2401.post6/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/test/tents.py` & `ngstrefftz-0.3.2401.post6/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2401.post4/test/trefftz.py` & `ngstrefftz-0.3.2401.post6/test/trefftz.py`

 * *Files identical despite different names*

