# Comparing `tmp/neon-skill-stock-1.0.1a2.tar.gz` & `tmp/neon-skill-stock-1.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-stock-1.0.1a2.tar", last modified: Tue Apr  2 22:10:43 2024, max compression
+gzip compressed data, was "neon-skill-stock-1.0.1a3.tar", last modified: Tue Apr  9 22:35:00 2024, max compression
```

## Comparing `neon-skill-stock-1.0.1a2.tar` & `neon-skill-stock-1.0.1a3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11558 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/el-gr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/el-gr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/el-gr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/el-gr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/el-gr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/el-gr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/intent/stock_price.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/hu-hu/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/hu-hu/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/hu-hu/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/hu-hu/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ru-ru/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ru-ru/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ru-ru/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/ui/Stock.qml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.362290 neon-skill-stock-1.0.1a3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11558 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-09 22:35:00.362290 neon-skill-stock-1.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ca-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ca-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ca-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ca-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/de-de/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/de-de/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/de-de/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/de-de/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/el-gr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/el-gr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/el-gr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/el-gr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/el-gr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/el-gr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/en-us/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/en-us/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/en-us/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/en-us/intent/stock_price.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/es-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/es-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/es-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/es-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/fr-fr/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/fr-fr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/fr-fr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/fr-fr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.354291 neon-skill-stock-1.0.1a3/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/gl-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/gl-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/gl-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/gl-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/hu-hu/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/hu-hu/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/hu-hu/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/hu-hu/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/it-it/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/it-it/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/it-it/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/it-it/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/nl-nl/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/nl-nl/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/nl-nl/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/nl-nl/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/pt-br/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/pt-br/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/pt-br/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/pt-br/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ru-ru/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ru-ru/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/ru-ru/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.350291 neon-skill-stock-1.0.1a3/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/sv-se/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/sv-se/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/sv-se/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/locale/sv-se/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.358291 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-09 22:35:00.000000 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-09 22:35:00.000000 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:35:00.000000 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 22:35:00.000000 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 22:35:00.000000 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 22:35:00.000000 neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:35:00.362290 neon-skill-stock-1.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.362290 neon-skill-stock-1.0.1a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:35:00.362290 neon-skill-stock-1.0.1a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/ui/Stock.qml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-09 22:34:56.000000 neon-skill-stock-1.0.1a3/version.py
```

### Comparing `neon-skill-stock-1.0.1a2/LICENSE` & `neon-skill-stock-1.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a2/LICENSE.md` & `neon-skill-stock-1.0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a2/PKG-INFO` & `neon-skill-stock-1.0.1a3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-Metadata-Version: 2.1
-Name: neon-skill-stock
-Version: 1.0.1a2
-Home-page: https://github.com/NeonGeckoCom/skill-stock
-Author: Neongecko
-Author-email: developers@neon.ai
-License: BSD-3-Clause
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-License-File: LICENSE.md
-
 # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/money-check-alt.svg' card_color="#FF8600" width="50" style="vertical-align:bottom">Stock
 
 ## Summary
 
 This skill provides stock values.
 
 ## Description
 
-Use this skill to lookup stock prices. Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the
-Alpha Vantage API directly by providing a key in `~/alpha_vantage.txt`. You can generate an Alpha Vantage key
-[here](https://www.alphavantage.co/support/#api-key)
+Use this skill to lookup stock prices. Use of this skill requires use of 
+third-party APIs. This skill will use Neon AI servers by default, but you can 
+deploy your own instance of [Diana](https://github.com/NeonGeckoCom/neon-diana-utils).
 
 ## Examples
 
 * What is the share price for Amazon?
 * What is the stock price for Microsoft?
 
 ## Contact Support
```

### Comparing `neon-skill-stock-1.0.1a2/README.md` & `neon-skill-stock-1.0.1a3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+Metadata-Version: 2.1
+Name: neon-skill-stock
+Version: 1.0.1a3
+Home-page: https://github.com/NeonGeckoCom/skill-stock
+Author: Neongecko
+Author-email: developers@neon.ai
+License: BSD-3-Clause
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+License-File: LICENSE.md
+
 # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/money-check-alt.svg' card_color="#FF8600" width="50" style="vertical-align:bottom">Stock
 
 ## Summary
 
 This skill provides stock values.
 
 ## Description
 
-Use this skill to lookup stock prices. Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the
-Alpha Vantage API directly by providing a key in `~/alpha_vantage.txt`. You can generate an Alpha Vantage key
-[here](https://www.alphavantage.co/support/#api-key)
+Use this skill to lookup stock prices. Use of this skill requires use of 
+third-party APIs. This skill will use Neon AI servers by default, but you can 
+deploy your own instance of [Diana](https://github.com/NeonGeckoCom/neon-diana-utils).
 
 ## Examples
 
 * What is the share price for Amazon?
 * What is the stock price for Microsoft?
 
 ## Contact Support
```

### Comparing `neon-skill-stock-1.0.1a2/__init__.py` & `neon-skill-stock-1.0.1a3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,132 +24,108 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from typing import Optional
 from neon_utils.skills.neon_skill import NeonSkill
-from neon_api_proxy.client import alpha_vantage
+from neon_utils.hana_utils import request_backend
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
-
-from mycroft.skills import intent_file_handler
+from ovos_workshop.decorators import intent_handler
 
 
 class StockSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
         self.preferred_market = "United States"
         self.translate_co = {"3 m": "mmm",
                              "3m": "mmm",
                              "coca cola": "ko",
                              "coca-cola": "ko",
                              "google": "goog",
                              "exxonmobil": "xom"}
-        self._service = None
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
                                    requires_network=True,
                                    requires_gui=False,
                                    no_internet_fallback=False,
                                    no_network_fallback=False,
                                    no_gui_fallback=True)
 
-    @property
-    def service(self):
-        if not self._service:
-            service = self.settings.get('service') or "Alpha Vantage"
-            if service == "Financial Modeling Prep" and not self.api_key:
-                service = "Alpha Vantage"
-            self._service = service
-        return self._service
-
-    @property
-    def api_key(self):
-        return self.settings.get('api_keys', {}).get(self.service) or \
-               self.settings.get("api_key")
-
-    @property
-    def data_source(self):
-        return alpha_vantage
-
-    @intent_file_handler("stock_price.intent")
+    @intent_handler("stock_price.intent")
     def handle_stock_price(self, message):
         """
         Handle a query for stock value
         """
         company = message.data.get("company").lower().strip()
         LOG.debug(company)
 
         try:
-            # # Special case handling for 3m
-            # if company == 'm' and "3m" in str(message.data['utterance']).split():
-            #     company = "mmm"
-
             # Special case for common stocks that don't match accurately
             if company in self.translate_co:
+                LOG.info(f"{company} in {self.translate_co}")
                 company = self.translate_co[company]
-                LOG.debug(company)
 
             match_data = self._search_company(company)
             if not match_data:
                 self.speak_dialog("not.found", data={'company': company})
                 return
-            company = match_data.get("name")
-            symbol = match_data.get("symbol")
-            LOG.debug(f"found {company} with symbol {symbol}")
+            company = match_data.get("2. name")
+            symbol = match_data.get("1. symbol")
+            LOG.info(f"found {company} with symbol {symbol}")
             if symbol:
                 quote = self._get_stock_price(symbol)
             else:
                 quote = None
             if not all([symbol, company, quote]):
                 self.speak_dialog("not.found", data={'company': company})
             else:
                 response = {'symbol': symbol,
                             'company': company,
                             'price': quote,
-                            'provider': self.service}
+                            'provider': "Alpha Vantage"}
                 self.speak_dialog("stock.price", data=response)
                 self.gui["title"] = company
                 self.gui["text"] = f"${quote}"
                 self.gui.show_page("Stock.qml")
         except Exception as e:
             LOG.exception(e)
             self.speak_dialog("not.found", data={'company': company})
 
     def _search_company(self, company: str) -> Optional[dict]:
         """
         Find a traded company by name
         :param company: Company to search
         :return: dict company data: `symbol`, `name`, `region`, `currency`
         """
-        kwargs = {"region": self.preferred_market}
-        if self.api_key:
-            kwargs["api_key"] = self.api_key
-        stocks = self.data_source.search_stock_by_name(company, **kwargs)
-        LOG.debug(f"stocks={stocks}")
-        # TODO: Catch and warn on API error here
+        kwargs = {"region": self.preferred_market,
+                  "company": company}
+        # TODO: Remove `server_url`
+        stocks = request_backend("/proxy/stock/symbol", kwargs,
+                                 server_url="https://hana.neonaibeta.com")
+        LOG.info(f"stocks={stocks}")
         if stocks:
-            return stocks[0]
+            return stocks["bestMatches"][0]
         else:
             return None
 
-    def _get_stock_price(self, symbol: str):
+    @staticmethod
+    def _get_stock_price(symbol: str):
         """
         Get the current trade price by ticker symbol
         :param symbol: Ticker symbol to query
         :return:
         """
-        kwargs = {}
-        if self.api_key:
-            kwargs["api_key"] = self.api_key
-        stock_data = self.data_source.get_stock_quote(symbol)
-        # TODO: Catch and warn on API error here
-        if not stock_data.get("price"):
+        # TODO: Remove `server_url`
+        stock_data = request_backend("/proxy/stock/quote", {"symbol": symbol},
+                                     server_url="https://hana.neonaibeta.com")
+        price = stock_data.get("Global Quote", {}).get("05. price")
+        if not price:
             return None
-        return str(round(float(stock_data.get("price")), 2))
+        return str(round(float(price), 2))
```

### Comparing `neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/PKG-INFO` & `neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 1.0.1a2
+Version: 1.0.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -14,17 +14,17 @@
 
 ## Summary
 
 This skill provides stock values.
 
 ## Description
 
-Use this skill to lookup stock prices. Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the
-Alpha Vantage API directly by providing a key in `~/alpha_vantage.txt`. You can generate an Alpha Vantage key
-[here](https://www.alphavantage.co/support/#api-key)
+Use this skill to lookup stock prices. Use of this skill requires use of 
+third-party APIs. This skill will use Neon AI servers by default, but you can 
+deploy your own instance of [Diana](https://github.com/NeonGeckoCom/neon-diana-utils).
 
 ## Examples
 
 * What is the share price for Amazon?
 * What is the stock price for Microsoft?
 
 ## Contact Support
```

### Comparing `neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/SOURCES.txt` & `neon-skill-stock-1.0.1a3/neon_skill_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a2/setup.py` & `neon-skill-stock-1.0.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a2/skill.json` & `neon-skill-stock-1.0.1a3/skill.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742424242424242%*

 * *Differences: {"'description'": "'Use this skill to lookup stock prices. Use of this skill requires use of "*

 * *                  'third-party APIs. This skill will use Neon AI servers by default, but you can '*

 * *                  'deploy your own instance of '*

 * *                  "[Diana](https://github.com/NeonGeckoCom/neon-diana-utils).'",*

 * * "'requirements'": "{'python': {insert: [(0, 'neon-utils~=1.9'), (2, 'ovos-workshop~=0.0.15')], "*

 * *                   'delete: [1, 0]}}'}*

```diff
@@ -7,15 +7,15 @@
     ],
     "category": "Information",
     "credits": [
         "Mycroft AI",
         "NeonDaniel",
         "reginaneon"
     ],
-    "description": "Use this skill to lookup stock prices. Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the Alpha Vantage API directly by providing a key in `~/alpha_vantage.txt`. You can generate an Alpha Vantage key [here](https://www.alphavantage.co/support/#api-key)",
+    "description": "Use this skill to lookup stock prices. Use of this skill requires use of third-party APIs. This skill will use Neon AI servers by default, but you can deploy your own instance of [Diana](https://github.com/NeonGeckoCom/neon-diana-utils).",
     "desktopFile": false,
     "examples": [
         "What is the share price for Amazon?",
         "What is the stock price for Microsoft?"
     ],
     "foldername": null,
     "icon": "https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/money-check-alt.svg",
@@ -26,17 +26,17 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
-            "neon-api-proxy~=0.4",
-            "neon-utils~=1.0",
-            "ovos-utils~=0.0, >=0.0.28"
+            "neon-utils~=1.9",
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "This skill provides stock values.",
     "skillname": "skill-stock",
     "summary": "This skill provides stock values.",
```

### Comparing `neon-skill-stock-1.0.1a2/test/test_skill.py` & `neon-skill-stock-1.0.1a3/test/test_skill.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,21 +37,14 @@
         # Test any parameters expected to be set in init or initialize methods
         from neon_utils.skills.neon_skill import NeonSkill
 
         self.assertIsInstance(self.skill, NeonSkill)
         self.assertIsInstance(self.skill.translate_co, dict)
         self.assertIsInstance(self.skill.preferred_market, str)
 
-        self.assertIsInstance(self.skill.service, str)
-        self.assertIsNone(self.skill.api_key)
-        self.assertTrue(hasattr(self.skill.data_source,
-                                "search_stock_by_name"))
-        self.assertTrue(hasattr(self.skill.data_source,
-                                "get_stock_quote"))
-
     def test_handle_stock_price(self):
         message = Message("test", {"company": "3m"})
         self.skill.handle_stock_price(message)
         self.skill.speak_dialog.assert_called_once()
         args = self.skill.speak_dialog.call_args
         self.assertEqual(args[0][0], "stock.price")
         data = args[1]["data"]
```

### Comparing `neon-skill-stock-1.0.1a2/ui/Stock.qml` & `neon-skill-stock-1.0.1a3/ui/Stock.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a2/version.py` & `neon-skill-stock-1.0.1a3/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a2"
+__version__ = "1.0.1a3"
```

