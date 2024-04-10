# Comparing `tmp/skyproj-1.2.2.tar.gz` & `tmp/skyproj-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyproj-1.2.2.tar", last modified: Fri Mar 15 16:47:43 2024, max compression
+gzip compressed data, was "skyproj-1.2.3.tar", last modified: Wed Apr 10 15:07:32 2024, max compression
```

## Comparing `skyproj-1.2.2.tar` & `skyproj-1.2.3.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.514526 skyproj-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.474527 skyproj-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.478527 skyproj-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-15 16:47:37.000000 skyproj-1.2.2/.github/workflows/python-package-pr-pip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-15 16:47:37.000000 skyproj-1.2.2/.github/workflows/python-package-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-15 16:47:37.000000 skyproj-1.2.2/.github/workflows/python-package-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-15 16:47:37.000000 skyproj-1.2.2/.github/workflows/python-package-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-15 16:47:37.000000 skyproj-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-15 16:47:37.000000 skyproj-1.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-15 16:47:37.000000 skyproj-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-15 16:47:37.000000 skyproj-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-15 16:47:43.514526 skyproj-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-15 16:47:37.000000 skyproj-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.482527 skyproj-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/basic_interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.486527 skyproj-1.2.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    94103 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/AlbersSkyproj_with_indicatrix.png
--rw-r--r--   0 runner    (1001) docker     (127)    43028 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/BLISS_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/DECaLS_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    93987 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/DESAlbers_survey_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    51893 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/DES_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    73327 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/DES_survey_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    78912 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/EqualEarthSkyproj_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    63405 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/GnomonicSkyproj_with_indicatrix.png
--rw-r--r--   0 runner    (1001) docker     (127)    98133 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/HammerSkyproj_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    90522 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/LaeaSkyproj_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    65432 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/MagLiTeS_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    81023 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/McBrydeSkyproj_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    88217 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/MollweideSkyproj_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)    79466 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/ObliqueMollweideSkyproj.png
--rw-r--r--   0 runner    (1001) docker     (127)    52120 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/Skyproj_with_indicatrices.png
--rw-r--r--   0 runner    (1001) docker     (127)   370290 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/healsparse_one.png
--rw-r--r--   0 runner    (1001) docker     (127)    81432 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/healsparse_two.png
--rw-r--r--   0 runner    (1001) docker     (127)    47640 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/healsparse_valid_pixels.png
--rw-r--r--   0 runner    (1001) docker     (127)    83072 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/hpxbin.png
--rw-r--r--   0 runner    (1001) docker     (127)   106704 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/hpxbin_reproject.png
--rw-r--r--   0 runner    (1001) docker     (127)    81719 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/lines_and_polygons_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    80741 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/milky_way.png
--rw-r--r--   0 runner    (1001) docker     (127)    71306 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/milky_way_galactic.png
--rw-r--r--   0 runner    (1001) docker     (127)    68894 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/images/skyproj_full_override_sizes.png
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/maps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/projections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-15 16:47:37.000000 skyproj-1.2.2/docs/surveys.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-15 16:47:37.000000 skyproj-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 16:47:37.000000 skyproj-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-15 16:47:43.514526 skyproj-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.490527 skyproj-1.2.2/skyproj/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    59977 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/_skyproj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.494526 skyproj-1.2.2/skyproj/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/bliss-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/ccd_corners_xy_fill.dat
--rw-r--r--   0 runner    (1001) docker     (127)   392256 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/constellationsANDstars.json
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/decals-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/derosita-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13851 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/des-round13-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/des-round17-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/des-round19-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/macho_corners_xy.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/maglites-poly.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16927 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/data/smash_fields_final.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/hpx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/mpl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/skyaxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/skycrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/skyproj.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    12888 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-15 16:47:37.000000 skyproj-1.2.2/skyproj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.514526 skyproj-1.2.2/skyproj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-15 16:47:43.000000 skyproj-1.2.2/skyproj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-03-15 16:47:43.000000 skyproj-1.2.2/skyproj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:47:43.000000 skyproj-1.2.2/skyproj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 16:47:43.000000 skyproj-1.2.2/skyproj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 16:47:43.000000 skyproj-1.2.2/skyproj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:47:43.000000 skyproj-1.2.2/skyproj.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.494526 skyproj-1.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.510527 skyproj-1.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    41765 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/BLISS_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    49364 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/DECaLS_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    71908 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/DESAlbers_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    51417 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/DES_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    65432 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/MagLiTeS_survey.png
--rw-r--r--   0 runner    (1001) docker     (127)    72157 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_-15.0_-45.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    59073 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_-20.0_15.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    72705 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_15.0_45.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    73384 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_full_-100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    72705 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_full_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    73222 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_full_100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    72623 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_full_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    39838 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/aea_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/cyl_full_-100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/cyl_full_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    29323 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/cyl_full_100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    28825 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/cyl_full_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    50704 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/cyl_tissot.png
--rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/cyl_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    66533 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/eqearth_full_-100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    61211 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/eqearth_full_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    66489 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/eqearth_full_100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    62476 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/eqearth_full_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    35858 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/eqearth_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    40001 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/gnom_-120.0_75.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/gnom_0.0_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/gnom_120.0_-75.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    83841 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hammer_full_-100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    79363 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hammer_full_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    83540 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hammer_full_100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    79434 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hammer_full_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    45158 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hammer_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    39131 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_bool.png
--rw-r--r--   0 runner    (1001) docker     (127)    47810 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_bool_valid_pixels.png
--rw-r--r--   0 runner    (1001) docker     (127)   383785 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_five.png
--rw-r--r--   0 runner    (1001) docker     (127)    50533 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_four.png
--rw-r--r--   0 runner    (1001) docker     (127)   367086 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_one.png
--rw-r--r--   0 runner    (1001) docker     (127)    98341 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_rec_array.png
--rw-r--r--   0 runner    (1001) docker     (127)    71520 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_three.png
--rw-r--r--   0 runner    (1001) docker     (127)    81432 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_two.png
--rw-r--r--   0 runner    (1001) docker     (127)    47248 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_valid_pixels.png
--rw-r--r--   0 runner    (1001) docker     (127)    38520 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/healsparse_wide_one.png
--rw-r--r--   0 runner    (1001) docker     (127)    64641 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hpxbin.png
--rw-r--r--   0 runner    (1001) docker     (127)    46030 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/hpxbin_two.png
--rw-r--r--   0 runner    (1001) docker     (127)    32715 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/laea_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    83969 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/lines_and_polygons_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    83381 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/lines_and_polygons_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    90720 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    92250 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    69515 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_full_-100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    64412 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_full_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    69986 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_full_100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    64751 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_full_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    65342 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_gaptest.png
--rw-r--r--   0 runner    (1001) docker     (127)    80206 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_tissot.png
--rw-r--r--   0 runner    (1001) docker     (127)    36435 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/mbtfpq_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    79900 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/milky_way.png
--rw-r--r--   0 runner    (1001) docker     (127)    70761 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/milky_way_galactic.png
--rw-r--r--   0 runner    (1001) docker     (127)    74885 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/moll_full_-100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/moll_full_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    74824 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/moll_full_100.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    71078 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/moll_full_180.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    72121 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/moll_gaptest.png
--rw-r--r--   0 runner    (1001) docker     (127)    36317 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/moll_zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    78142 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/obmoll_0.0_45.0_-90.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    79297 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/obmoll_100.0_80.0_0.0.png
--rw-r--r--   0 runner    (1001) docker     (127)    44705 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/plotting_routines.png
--rw-r--r--   0 runner    (1001) docker     (127)    66418 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/data/skyproj_full_override_sizes.png
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_healpix_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)    27516 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_healpix_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_lines_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_milky_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_projections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_skyproj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_tissot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-15 16:47:37.000000 skyproj-1.2.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.514526 skyproj-1.2.2/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-15 16:47:37.000000 skyproj-1.2.2/tutorial/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   432870 2024-03-15 16:47:37.000000 skyproj-1.2.2/tutorial/tutorial_baseclass.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1933628 2024-03-15 16:47:37.000000 skyproj-1.2.2/tutorial/tutorial_healsparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   551528 2024-03-15 16:47:37.000000 skyproj-1.2.2/tutorial/tutorial_surveys.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:47:43.514526 skyproj-1.2.2/ups/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-15 16:47:37.000000 skyproj-1.2.2/ups/skyproj.table
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.346696 skyproj-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.306695 skyproj-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.310695 skyproj-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-10 15:07:21.000000 skyproj-1.2.3/.github/workflows/python-package-pr-pip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-10 15:07:21.000000 skyproj-1.2.3/.github/workflows/python-package-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-10 15:07:21.000000 skyproj-1.2.3/.github/workflows/python-package-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 15:07:21.000000 skyproj-1.2.3/.github/workflows/python-package-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-10 15:07:21.000000 skyproj-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-10 15:07:21.000000 skyproj-1.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 15:07:21.000000 skyproj-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 15:07:21.000000 skyproj-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-10 15:07:32.346696 skyproj-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-10 15:07:21.000000 skyproj-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.314695 skyproj-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/basic_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.318695 skyproj-1.2.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    94103 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/AlbersSkyproj_with_indicatrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43028 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/BLISS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/DECaLS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93987 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/DESAlbers_survey_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51893 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/DES_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73327 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/DES_survey_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78912 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/EqualEarthSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63405 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/GnomonicSkyproj_with_indicatrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98133 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/HammerSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90522 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/LaeaSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65432 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/MagLiTeS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81023 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/McBrydeSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88217 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/MollweideSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79466 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/ObliqueMollweideSkyproj.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52120 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/Skyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   370290 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/healsparse_one.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81432 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/healsparse_two.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47640 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/healsparse_valid_pixels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83072 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/hpxbin.png
+-rw-r--r--   0 runner    (1001) docker     (127)   106704 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/hpxbin_reproject.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81719 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/lines_and_polygons_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80741 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/milky_way.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71306 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/milky_way_galactic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68894 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/images/skyproj_full_override_sizes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/maps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/projections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-10 15:07:21.000000 skyproj-1.2.3/docs/surveys.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 15:07:21.000000 skyproj-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-10 15:07:21.000000 skyproj-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 15:07:32.350695 skyproj-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.322695 skyproj-1.2.3/skyproj/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59994 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/_skyproj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.326695 skyproj-1.2.3/skyproj/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/bliss-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/ccd_corners_xy_fill.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   392256 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/constellationsANDstars.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/decals-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/derosita-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13851 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/des-round13-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/des-round17-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/des-round19-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/macho_corners_xy.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/maglites-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16927 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/data/smash_fields_final.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/hpx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/mpl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/skyaxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/skycrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/skyproj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12888 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-10 15:07:21.000000 skyproj-1.2.3/skyproj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.346696 skyproj-1.2.3/skyproj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-10 15:07:32.000000 skyproj-1.2.3/skyproj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-10 15:07:32.000000 skyproj-1.2.3/skyproj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:07:32.000000 skyproj-1.2.3/skyproj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 15:07:32.000000 skyproj-1.2.3/skyproj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 15:07:32.000000 skyproj-1.2.3/skyproj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:07:31.000000 skyproj-1.2.3/skyproj.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.326695 skyproj-1.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.342695 skyproj-1.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    41765 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/BLISS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49364 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/DECaLS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71908 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/DESAlbers_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51417 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/DES_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65432 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/MagLiTeS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72157 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_-15.0_-45.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59073 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_-20.0_15.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72705 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_15.0_45.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73384 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72705 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73222 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72623 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39838 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/aea_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/cyl_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/cyl_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29323 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/cyl_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28825 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/cyl_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50704 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/cyl_tissot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/cyl_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66533 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/eqearth_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61211 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/eqearth_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66489 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/eqearth_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62476 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/eqearth_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35858 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/eqearth_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40001 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/gnom_-120.0_75.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/gnom_0.0_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/gnom_120.0_-75.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83841 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hammer_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79363 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hammer_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83540 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hammer_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79434 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hammer_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45158 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hammer_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39131 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_bool.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47810 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_bool_valid_pixels.png
+-rw-r--r--   0 runner    (1001) docker     (127)   383785 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_five.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50533 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_four.png
+-rw-r--r--   0 runner    (1001) docker     (127)   367086 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_one.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98341 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_rec_array.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71520 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_three.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81432 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_two.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47248 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_valid_pixels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38520 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/healsparse_wide_one.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64641 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hpxbin.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46030 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/hpxbin_two.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32715 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/laea_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83969 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/lines_and_polygons_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83381 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/lines_and_polygons_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90720 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92250 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69515 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64412 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69986 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64751 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65342 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_gaptest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80206 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_tissot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36435 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/mbtfpq_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79900 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/milky_way.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70761 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/milky_way_galactic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74885 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/moll_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/moll_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74824 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/moll_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71078 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/moll_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72121 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/moll_gaptest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36317 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/moll_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78142 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/obmoll_0.0_45.0_-90.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79297 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/obmoll_100.0_80.0_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44705 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/plotting_routines.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66418 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/data/skyproj_full_override_sizes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_healpix_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_healpix_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_lines_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_milky_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_skyproj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_tissot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-10 15:07:21.000000 skyproj-1.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.346696 skyproj-1.2.3/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 15:07:21.000000 skyproj-1.2.3/tutorial/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   432870 2024-04-10 15:07:21.000000 skyproj-1.2.3/tutorial/tutorial_baseclass.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1933628 2024-04-10 15:07:21.000000 skyproj-1.2.3/tutorial/tutorial_healsparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   551528 2024-04-10 15:07:21.000000 skyproj-1.2.3/tutorial/tutorial_surveys.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:07:32.346696 skyproj-1.2.3/ups/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 15:07:21.000000 skyproj-1.2.3/ups/skyproj.table
```

### Comparing `skyproj-1.2.2/.github/workflows/python-package-pr-pip.yaml` & `skyproj-1.2.3/.github/workflows/python-package-pr-pip.yaml`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/.github/workflows/python-package-pr.yml` & `skyproj-1.2.3/.github/workflows/python-package-pr.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         show-channel-urls: true
         miniforge-version: latest
         miniforge-variant: Mambaforge
 
     - name: Configure conda and install code
       shell: bash -l {0}
       run: |
-        mamba config --set always_yes yes
-        mamba install numpy "astropy>=4.0" matplotlib hpgeom setuptools_scm setuptools_scm_git_archive healsparse "pyproj>=3.1" flake8 pytest jupyter "nbconvert<7"
+        mamba install -y numpy "astropy>=4.0" matplotlib hpgeom setuptools_scm setuptools_scm_git_archive healsparse "pyproj>=3.1" flake8 pytest jupyter "nbconvert<7"
         python -m pip install --no-deps .
 
     - name: Lint with flake8
       shell: bash -l {0}
       run: |
         # stop the build if it fails flake8 with default setup.cfg
         flake8 . --count --show-source --statistics
```

### Comparing `skyproj-1.2.2/.github/workflows/python-package-publish.yml` & `skyproj-1.2.3/.github/workflows/python-package-publish.yml`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/.github/workflows/python-package-push.yml` & `skyproj-1.2.3/.github/workflows/python-package-push.yml`

 * *Files 17% similar despite different names*

```diff
@@ -23,16 +23,15 @@
         show-channel-urls: true
         miniforge-version: latest
         miniforge-variant: Mambaforge
 
     - name: Configure conda and install code
       shell: bash -l {0}
       run: |
-        mamba config --set always_yes yes
-        mamba install numpy "astropy>=4.0" matplotlib hpgeom setuptools_scm setuptools_scm_git_archive healsparse "pyproj>=3.1" flake8 pytest jupyter "nbconvert<7"
+        mamba install -y numpy "astropy>=4.0" matplotlib hpgeom setuptools_scm setuptools_scm_git_archive healsparse "pyproj>=3.1" flake8 pytest jupyter "nbconvert<7"
         python -m pip install --no-deps .
 
     - name: Lint with flake8
       shell: bash -l {0}
       run: |
         # stop the build if it fails flake8 with default setup.cfg
         flake8 . --count --show-source --statistics
```

### Comparing `skyproj-1.2.2/.gitignore` & `skyproj-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/.readthedocs.yaml` & `skyproj-1.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/LICENSE` & `skyproj-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/PKG-INFO` & `skyproj-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyproj
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python tools for making sky projections and maps
 Home-page: https://github.com/lsstdesc/skyproj
 Author: Eli Rykoff, Alex Drlica-Wagner, and others
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `skyproj-1.2.2/README.md` & `skyproj-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/Makefile` & `skyproj-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/basic_interface.rst` & `skyproj-1.2.3/docs/basic_interface.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/conf.py` & `skyproj-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/AlbersSkyproj_with_indicatrix.png` & `skyproj-1.2.3/docs/images/AlbersSkyproj_with_indicatrix.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/BLISS_survey.png` & `skyproj-1.2.3/docs/images/BLISS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/DECaLS_survey.png` & `skyproj-1.2.3/docs/images/DECaLS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/DESAlbers_survey_with_indicatrices.png` & `skyproj-1.2.3/docs/images/DESAlbers_survey_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/DES_survey.png` & `skyproj-1.2.3/docs/images/DES_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/DES_survey_with_indicatrices.png` & `skyproj-1.2.3/docs/images/DES_survey_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/EqualEarthSkyproj_with_indicatrices.png` & `skyproj-1.2.3/docs/images/EqualEarthSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/GnomonicSkyproj_with_indicatrix.png` & `skyproj-1.2.3/docs/images/GnomonicSkyproj_with_indicatrix.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/HammerSkyproj_with_indicatrices.png` & `skyproj-1.2.3/docs/images/HammerSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/LaeaSkyproj_with_indicatrices.png` & `skyproj-1.2.3/docs/images/LaeaSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/MagLiTeS_survey.png` & `skyproj-1.2.3/docs/images/MagLiTeS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/McBrydeSkyproj_with_indicatrices.png` & `skyproj-1.2.3/docs/images/McBrydeSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/MollweideSkyproj_with_indicatrices.png` & `skyproj-1.2.3/docs/images/MollweideSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/ObliqueMollweideSkyproj.png` & `skyproj-1.2.3/docs/images/ObliqueMollweideSkyproj.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/Skyproj_with_indicatrices.png` & `skyproj-1.2.3/docs/images/Skyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/healsparse_one.png` & `skyproj-1.2.3/docs/images/healsparse_one.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/healsparse_two.png` & `skyproj-1.2.3/docs/images/healsparse_two.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/healsparse_valid_pixels.png` & `skyproj-1.2.3/docs/images/healsparse_valid_pixels.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/hpxbin.png` & `skyproj-1.2.3/docs/images/hpxbin.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/hpxbin_reproject.png` & `skyproj-1.2.3/docs/images/hpxbin_reproject.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/lines_and_polygons_0.0.png` & `skyproj-1.2.3/docs/images/lines_and_polygons_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/milky_way.png` & `skyproj-1.2.3/docs/images/milky_way.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/milky_way_galactic.png` & `skyproj-1.2.3/docs/images/milky_way_galactic.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/images/skyproj_full_override_sizes.png` & `skyproj-1.2.3/docs/images/skyproj_full_override_sizes.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/index.rst` & `skyproj-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/install.rst` & `skyproj-1.2.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/make.bat` & `skyproj-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/maps.rst` & `skyproj-1.2.3/docs/maps.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/modules.rst` & `skyproj-1.2.3/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/projections.rst` & `skyproj-1.2.3/docs/projections.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/docs/surveys.rst` & `skyproj-1.2.3/docs/surveys.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/setup.cfg` & `skyproj-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/_docstrings.py` & `skyproj-1.2.3/skyproj/_docstrings.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/_skyproj.py` & `skyproj-1.2.3/skyproj/_skyproj.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
                 else:
                     va = 'bottom'
 
                 # Skip any that are out of the y bounding box.
                 if lat_line_y[0] < extent_xy[2] or lat_line_y[0] > extent_xy[3]:
                     continue
 
-                if lat_line_x[0] < extent_xy[x0_index] or lat_line_y[0] > extent_xy[x1_index]:
+                if lat_line_x[0] < extent_xy[x0_index] or lat_line_x[0] > extent_xy[x1_index]:
                     continue
 
                 label = self._tick_formatter2(axis_side, factor, [lat_level])[0]
 
                 boundary_labels.append(self._ax.text(lat_line_x[0],
                                                      lat_line_y[0],
                                                      label,
@@ -980,15 +980,15 @@
             Array of latitude values.
 
         Returns
         -------
         extent : `list`
             Plotting extent [lon_max, lon_min, lat_min, lat_max]
         """
-        lon_wrap = wrap_values(lon)
+        lon_wrap = wrap_values(lon, wrap=self._wrap)
 
         # Compute lat range with cushion
         lat_min0 = np.min(lat)
         lat_max0 = np.max(lat)
         lat_range = lat_max0 - lat_min0
         lat_min = np.clip(lat_min0 - 0.05*lat_range, -90.0, None)
         lat_max = np.clip(lat_max0 + 0.05*lat_range, None, 90.0)
```

### Comparing `skyproj-1.2.2/skyproj/data/bliss-poly.txt` & `skyproj-1.2.3/skyproj/data/bliss-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/ccd_corners_xy_fill.dat` & `skyproj-1.2.3/skyproj/data/ccd_corners_xy_fill.dat`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/constellationsANDstars.json` & `skyproj-1.2.3/skyproj/data/constellationsANDstars.json`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/decals-poly.txt` & `skyproj-1.2.3/skyproj/data/decals-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/derosita-poly.txt` & `skyproj-1.2.3/skyproj/data/derosita-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/des-round13-poly.txt` & `skyproj-1.2.3/skyproj/data/des-round13-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/des-round17-poly.txt` & `skyproj-1.2.3/skyproj/data/des-round17-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/des-round19-poly.txt` & `skyproj-1.2.3/skyproj/data/des-round19-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/maglites-poly.txt` & `skyproj-1.2.3/skyproj/data/maglites-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/data/smash_fields_final.txt` & `skyproj-1.2.3/skyproj/data/smash_fields_final.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/hpx_utils.py` & `skyproj-1.2.3/skyproj/hpx_utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/mpl_utils.py` & `skyproj-1.2.3/skyproj/mpl_utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/skyaxes.py` & `skyproj-1.2.3/skyproj/skyaxes.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/skycrs.py` & `skyproj-1.2.3/skyproj/skycrs.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/skyproj.py` & `skyproj-1.2.3/skyproj/skyproj.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/survey.py` & `skyproj-1.2.3/skyproj/survey.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/transforms.py` & `skyproj-1.2.3/skyproj/transforms.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj/utils.py` & `skyproj-1.2.3/skyproj/utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/skyproj.egg-info/PKG-INFO` & `skyproj-1.2.3/skyproj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyproj
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python tools for making sky projections and maps
 Home-page: https://github.com/lsstdesc/skyproj
 Author: Eli Rykoff, Alex Drlica-Wagner, and others
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `skyproj-1.2.2/skyproj.egg-info/SOURCES.txt` & `skyproj-1.2.3/skyproj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/BLISS_survey.png` & `skyproj-1.2.3/tests/data/BLISS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/DECaLS_survey.png` & `skyproj-1.2.3/tests/data/DECaLS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/DESAlbers_survey.png` & `skyproj-1.2.3/tests/data/DESAlbers_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/DES_survey.png` & `skyproj-1.2.3/tests/data/DES_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/MagLiTeS_survey.png` & `skyproj-1.2.3/tests/data/MagLiTeS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_-15.0_-45.0.png` & `skyproj-1.2.3/tests/data/aea_-15.0_-45.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_-20.0_15.0.png` & `skyproj-1.2.3/tests/data/aea_-20.0_15.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_15.0_45.0.png` & `skyproj-1.2.3/tests/data/aea_15.0_45.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_full_-100.0.png` & `skyproj-1.2.3/tests/data/aea_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_full_0.0.png` & `skyproj-1.2.3/tests/data/aea_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_full_100.0.png` & `skyproj-1.2.3/tests/data/aea_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_full_180.0.png` & `skyproj-1.2.3/tests/data/aea_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/aea_zoom.png` & `skyproj-1.2.3/tests/data/aea_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/cyl_full_-100.0.png` & `skyproj-1.2.3/tests/data/cyl_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/cyl_full_0.0.png` & `skyproj-1.2.3/tests/data/cyl_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/cyl_full_100.0.png` & `skyproj-1.2.3/tests/data/cyl_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/cyl_full_180.0.png` & `skyproj-1.2.3/tests/data/cyl_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/cyl_tissot.png` & `skyproj-1.2.3/tests/data/cyl_tissot.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/cyl_zoom.png` & `skyproj-1.2.3/tests/data/cyl_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/eqearth_full_-100.0.png` & `skyproj-1.2.3/tests/data/eqearth_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/eqearth_full_0.0.png` & `skyproj-1.2.3/tests/data/eqearth_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/eqearth_full_100.0.png` & `skyproj-1.2.3/tests/data/eqearth_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/eqearth_full_180.0.png` & `skyproj-1.2.3/tests/data/eqearth_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/eqearth_zoom.png` & `skyproj-1.2.3/tests/data/eqearth_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/gnom_-120.0_75.0.png` & `skyproj-1.2.3/tests/data/gnom_-120.0_75.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/gnom_0.0_0.0.png` & `skyproj-1.2.3/tests/data/gnom_0.0_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/gnom_120.0_-75.0.png` & `skyproj-1.2.3/tests/data/gnom_120.0_-75.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hammer_full_-100.0.png` & `skyproj-1.2.3/tests/data/hammer_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hammer_full_0.0.png` & `skyproj-1.2.3/tests/data/hammer_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hammer_full_100.0.png` & `skyproj-1.2.3/tests/data/hammer_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hammer_full_180.0.png` & `skyproj-1.2.3/tests/data/hammer_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hammer_zoom.png` & `skyproj-1.2.3/tests/data/hammer_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_bool.png` & `skyproj-1.2.3/tests/data/healsparse_bool.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_bool_valid_pixels.png` & `skyproj-1.2.3/tests/data/healsparse_bool_valid_pixels.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_five.png` & `skyproj-1.2.3/tests/data/healsparse_five.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_four.png` & `skyproj-1.2.3/tests/data/healsparse_four.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_one.png` & `skyproj-1.2.3/tests/data/healsparse_one.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_rec_array.png` & `skyproj-1.2.3/tests/data/healsparse_rec_array.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_three.png` & `skyproj-1.2.3/tests/data/healsparse_three.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_two.png` & `skyproj-1.2.3/tests/data/healsparse_two.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_valid_pixels.png` & `skyproj-1.2.3/tests/data/healsparse_valid_pixels.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/healsparse_wide_one.png` & `skyproj-1.2.3/tests/data/healsparse_wide_one.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hpxbin.png` & `skyproj-1.2.3/tests/data/hpxbin.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/hpxbin_two.png` & `skyproj-1.2.3/tests/data/hpxbin_two.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/laea_zoom.png` & `skyproj-1.2.3/tests/data/laea_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/lines_and_polygons_0.0.png` & `skyproj-1.2.3/tests/data/lines_and_polygons_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/lines_and_polygons_180.0.png` & `skyproj-1.2.3/tests/data/lines_and_polygons_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png` & `skyproj-1.2.3/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png` & `skyproj-1.2.3/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_full_-100.0.png` & `skyproj-1.2.3/tests/data/mbtfpq_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_full_0.0.png` & `skyproj-1.2.3/tests/data/mbtfpq_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_full_100.0.png` & `skyproj-1.2.3/tests/data/mbtfpq_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_full_180.0.png` & `skyproj-1.2.3/tests/data/mbtfpq_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_gaptest.png` & `skyproj-1.2.3/tests/data/mbtfpq_gaptest.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_tissot.png` & `skyproj-1.2.3/tests/data/mbtfpq_tissot.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/mbtfpq_zoom.png` & `skyproj-1.2.3/tests/data/mbtfpq_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/milky_way.png` & `skyproj-1.2.3/tests/data/milky_way.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/milky_way_galactic.png` & `skyproj-1.2.3/tests/data/milky_way_galactic.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/moll_full_-100.0.png` & `skyproj-1.2.3/tests/data/moll_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/moll_full_0.0.png` & `skyproj-1.2.3/tests/data/moll_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/moll_full_100.0.png` & `skyproj-1.2.3/tests/data/moll_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/moll_full_180.0.png` & `skyproj-1.2.3/tests/data/moll_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/moll_gaptest.png` & `skyproj-1.2.3/tests/data/moll_gaptest.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/moll_zoom.png` & `skyproj-1.2.3/tests/data/moll_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/obmoll_0.0_45.0_-90.0.png` & `skyproj-1.2.3/tests/data/obmoll_0.0_45.0_-90.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/obmoll_100.0_80.0_0.0.png` & `skyproj-1.2.3/tests/data/obmoll_100.0_80.0_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/plotting_routines.png` & `skyproj-1.2.3/tests/data/plotting_routines.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/data/skyproj_full_override_sizes.png` & `skyproj-1.2.3/tests/data/skyproj_full_override_sizes.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_healpix_binning.py` & `skyproj-1.2.3/tests/test_healpix_binning.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_healpix_maps.py` & `skyproj-1.2.3/tests/test_healpix_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 
 import skyproj  # noqa: E402
 
 
 ROOT = os.path.abspath(os.path.dirname(__file__))
 
 
-def _get_hspmap():
+def _get_hspmap(ra_center=5.0):
     # Make a square noise field
     np.random.seed(1234)
 
     hspmap = hsp.HealSparseMap.make_empty(32, 4096, np.float32)
-    poly = hsp.geom.Polygon(ra=[0.0, 10.0, 10.0, 0.0], dec=[0.0, 0.0, 10.0, 10.0], value=1.0)
+    poly = hsp.geom.Polygon(ra=[ra_center-5.0, ra_center+5.0, ra_center+5.0, ra_center-5.0],
+                            dec=[0.0, 0.0, 10.0, 10.0], value=1.0)
     pixels = poly.get_pixels(nside=hspmap.nside_sparse)
     hspmap[pixels] = np.random.normal(size=pixels.size).astype(np.float32)
     # Add in a central square of fixed value.
-    poly2 = hsp.geom.Polygon(ra=[5, 5.2, 5.2, 5.0], dec=[5, 5.0, 5.2, 5.2], value=3.0)
+    poly2 = hsp.geom.Polygon(ra=[ra_center, ra_center + 0.2, ra_center + 0.2, ra_center],
+                             dec=[5, 5.0, 5.2, 5.2], value=3.0)
     pixels2 = poly2.get_pixels(nside=hspmap.nside_sparse)
     hspmap[pixels2] = 3.0
 
     return hspmap
 
 
 def _get_hspmap_bool():
@@ -742,7 +744,21 @@
     fname = 'hpxpix_rasterized_off.pdf'
     fig.savefig(tmp_path / fname)
 
     size_rasterized_off = os.path.getsize(tmp_path / fname)
 
     # The rasterized map will be smaller than the non-rasterized map.
     assert size_rasterized_on < size_rasterized_off
+
+
+@pytest.mark.parametrize("lon_0", [0.0, 180.0])
+def test_healsparse_gnomonic(tmp_path, lon_0):
+    """Test healsparse map with gnomonic projections."""
+    plt.rcParams.update(plt.rcParamsDefault)
+
+    hspmap = _get_hspmap(ra_center=lon_0)
+
+    fig = plt.figure(1, figsize=(8, 5))
+    fig.clf()
+    ax = fig.add_subplot(111)
+    sp = skyproj.GnomonicSkyproj(ax=ax, lon_0=lon_0, lat_0=0.0)
+    im, lon_raster, lat_raster, values_raster = sp.draw_hspmap(hspmap, zoom=True)
```

### Comparing `skyproj-1.2.2/tests/test_lines_polygons.py` & `skyproj-1.2.3/tests/test_lines_polygons.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_milky_way.py` & `skyproj-1.2.3/tests/test_milky_way.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_plotting.py` & `skyproj-1.2.3/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_projections.py` & `skyproj-1.2.3/tests/test_projections.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_skyproj.py` & `skyproj-1.2.3/tests/test_skyproj.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_survey.py` & `skyproj-1.2.3/tests/test_survey.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_tissot.py` & `skyproj-1.2.3/tests/test_tissot.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_tutorial.py` & `skyproj-1.2.3/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tests/test_utils.py` & `skyproj-1.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tutorial/tutorial_baseclass.ipynb` & `skyproj-1.2.3/tutorial/tutorial_baseclass.ipynb`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tutorial/tutorial_healsparse.ipynb` & `skyproj-1.2.3/tutorial/tutorial_healsparse.ipynb`

 * *Files identical despite different names*

### Comparing `skyproj-1.2.2/tutorial/tutorial_surveys.ipynb` & `skyproj-1.2.3/tutorial/tutorial_surveys.ipynb`

 * *Files identical despite different names*

