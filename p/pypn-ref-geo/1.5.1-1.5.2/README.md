# Comparing `tmp/pypn-ref-geo-1.5.1.tar.gz` & `tmp/pypn-ref-geo-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypn-ref-geo-1.5.1.tar", last modified: Mon Jan 29 15:57:58 2024, max compression
+gzip compressed data, was "pypn-ref-geo-1.5.2.tar", last modified: Wed Apr 10 05:22:00 2024, max compression
```

## Comparing `pypn-ref-geo-1.5.1.tar` & `pypn-ref-geo-1.5.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.646416 pypn-ref-geo-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-29 15:57:58.646416 pypn-ref-geo-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 15:57:58.646416 pypn-ref-geo-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.634416 pypn-ref-geo-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.646416 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-29 15:57:58.000000 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-29 15:57:58.000000 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 15:57:58.000000 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 15:57:58.000000 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-29 15:57:58.000000 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-29 15:57:58.000000 pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.638416 pypn-ref-geo-1.5.1/src/ref_geo/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.642416 pypn-ref-geo-1.5.1/src/ref_geo/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.642416 pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo_cor.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo_linear.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo_point.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:58.646416 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-29 15:57:46.000000 pypn-ref-geo-1.5.1/src/ref_geo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.914731 pypn-ref-geo-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.918731 pypn-ref-geo-1.5.2/src/ref_geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.918731 pypn-ref-geo-1.5.2/src/ref_geo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.918731 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_cor.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_linear.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_point.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/utils.py
```

### Comparing `pypn-ref-geo-1.5.1/CHANGELOG.md` & `pypn-ref-geo-1.5.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGELOG
 =========
 
+1.5.2 (2024-09-10)
+------------------
+
+**🚀 Nouveautés**
+
+ - Possibilité d'appeler la route `GET/areas` sans retourner les géométries (#22)
+
 1.5.1 (2024-01-29)
 ------------------
 
 - Ajout de la hiérachisation des types de zonages géographiques, avec l'ajout du champs `ref_geo.bib_areas_types.size_hierarchy` (#11)
 - Remplacement du champs `l_areas.geojson_4326` par `l_areas.geom_4326` et création de triggers permettant de garder en cohérence les champs `geom` et `geom_4326` (#6)
 - Mise à jour SQLAlchemy version 1.3 à 1.4 (#16)
 - Mise à jour de Flask version 2 à 3
```

### Comparing `pypn-ref-geo-1.5.1/LICENSE` & `pypn-ref-geo-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/PKG-INFO` & `pypn-ref-geo-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypn-ref-geo
-Version: 1.5.1
+Version: 1.5.2
 Summary: Référentiel géographique
 Home-page: https://github.com/PnX-SI/RefGeo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypn-ref-geo-1.5.1/README.md` & `pypn-ref-geo-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/setup.py` & `pypn-ref-geo-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/PKG-INFO` & `pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypn-ref-geo
-Version: 1.5.1
+Version: 1.5.2
 Summary: Référentiel géographique
 Home-page: https://github.com/PnX-SI/RefGeo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypn-ref-geo-1.5.1/src/pypn_ref_geo.egg-info/SOURCES.txt` & `pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/__init__.py` & `pypn-ref-geo-1.5.2/src/ref_geo/__init__.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/commands.py` & `pypn-ref-geo-1.5.2/src/ref_geo/commands.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/env.py` & `pypn-ref-geo-1.5.2/src/ref_geo/env.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo.sql` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo_cor.sql` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_cor.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo_linear.sql` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_linear.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/data/ref_geo_point.sql` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_point.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/env.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/utils.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py` & `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/models.py` & `pypn-ref-geo-1.5.2/src/ref_geo/models.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/routes.py` & `pypn-ref-geo-1.5.2/src/ref_geo/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 
 from flask import Blueprint, request, current_app
 from flask.json import jsonify
 import sqlalchemy as sa
 from sqlalchemy import func, select, asc, desc
 from sqlalchemy.sql import text
-from sqlalchemy.orm import joinedload, undefer
+from sqlalchemy.orm import joinedload, undefer, defer
 from werkzeug.exceptions import BadRequest
 
 from ref_geo.env import db
 from ref_geo.models import BibAreasTypes, LiMunicipalities, LAreas
 from ref_geo.schemas import AreaTypeSchema, MunicipalitySchema, AreaSchema
 
 
@@ -169,31 +169,36 @@
         q = q.where(LiMunicipalities.nom_com.ilike("{}%".format(parameters.get("nom_com"))))
     limit = int(parameters.get("limit")) if parameters.get("limit") else 100
 
     municipalities = db.session.scalars(q.limit(limit)).all()
     return jsonify(MunicipalitySchema().dump(municipalities, many=True))
 
 
+# FIXME: Transform to post and change the post /areas
 @routes.route("/areas", methods=["GET"])
 def get_areas():
     """
     Return the areas of ref_geo.l_areas
     .. :quickref: Ref Geo;
     """
     # change all args in a list of value
-    params = {key: request.args.getlist(key) for key, value in request.args.items()}
+    params = request.args
 
+    # allow to format response
+    output_format = request.args.get("format", default="", type=str)
+
+    marsh_params = dict(as_geojson=(output_format == "geojson"))
     query = (
         select(LAreas)
         .options(joinedload("area_type").load_only("type_code"))
         .order_by(LAreas.area_name.asc())
     )
 
     if "enable" in params:
-        enable_param = params["enable"][0].lower()
+        enable_param = params["enable"].lower()
         accepted_enable_values = ["true", "false", "all"]
         if enable_param not in accepted_enable_values:
             response = {
                 "message": f"Le paramètre 'enable' accepte seulement les valeurs: {', '.join(accepted_enable_values)}.",
                 "status": "warning",
             }
             return response, 400
@@ -201,36 +206,43 @@
             query = query.where(LAreas.enable == True)
         elif enable_param == "false":
             query = query.where(LAreas.enable == False)
     else:
         query = query.where(LAreas.enable == True)
 
     if "id_type" in params:
-        query = query.where(LAreas.id_type.in_(params["id_type"]))
+        query = query.where(LAreas.id_type.in_(params.getlist("id_type")))
 
     if "type_code" in params:
-        query = query.where(LAreas.area_type.has(BibAreasTypes.type_code.in_(params["type_code"])))
+        query = query.where(
+            LAreas.area_type.has(BibAreasTypes.type_code.in_(params.getlist("type_code")))
+        )
 
     if "area_name" in params:
-        query = query.where(LAreas.area_name.ilike("%{}%".format(params.get("area_name")[0])))
+        query = query.where(LAreas.area_name.ilike("%{}%".format(params.get("area_name"))))
 
-    limit = int(params.get("limit")[0]) if params.get("limit") else 100
+    without_geom = params.get("without_geom", False, lambda x: x == "true")
+    if without_geom:
+        query = query.options(defer("geom"))
+        marsh_params["exclude"] = ["geom"]
 
-    # allow to format response
-    format = request.args.get("format", default="", type=str)
+    limit = int(params.get("limit")[0]) if params.get("limit") else 100
 
     fields = {"area_type.type_code"}
-    if format == "geojson":
+    if output_format == "geojson" and not without_geom:
         fields |= {"+geom_4326"}
         query = query.options(undefer("geom_4326"))
 
     areas = db.session.scalars(query.limit(limit)).unique().all()
 
-    response = AreaSchema(only=fields, as_geojson=format == "geojson").dump(areas, many=True)
-    if format == "geojson":
+    marsh_params["only"] = fields
+
+    response = AreaSchema(**marsh_params).dump(areas, many=True)
+
+    if output_format == "geojson":
         # retro-compat: return a list of Features instead of the FeatureCollection
         response = response["features"]
     return response
 
 
 @routes.route("/area_size", methods=["Post"])
 def get_area_size():
```

### Comparing `pypn-ref-geo-1.5.1/src/ref_geo/schemas.py` & `pypn-ref-geo-1.5.2/src/ref_geo/schemas.py`

 * *Files identical despite different names*

