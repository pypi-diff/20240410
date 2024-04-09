# Comparing `tmp/neon-skill-spelling-1.0.1a2.tar.gz` & `tmp/neon-skill-spelling-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-spelling-1.0.1a2.tar", last modified: Tue Apr  2 22:04:31 2024, max compression
+gzip compressed data, was "neon-skill-spelling-1.1.0.tar", last modified: Tue Apr  9 22:48:58 2024, max compression
```

## Comparing `neon-skill-spelling-1.0.1a2.tar` & `neon-skill-spelling-1.1.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.780978 neon-skill-spelling-1.0.1a2/regex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/ca-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/da-dk/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/de-de/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/el-gr/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/en-us/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/es-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/fa-ir/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/fr-fr/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/gl-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/hu-hu/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/it-it/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/nl-nl/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/pl-pl/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/pt-br/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/ro-ro/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/ru-ru/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/sv-se/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/tr-tr/word.rx
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/ca-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/da-dk/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/de-de/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/el-gr/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/en-us/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/es-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/fa-ir/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/fr-fr/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/gl-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/hu-hu/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/it-it/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/nl-nl/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/pl-pl/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/pt-br/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/ro-ro/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/ru-ru/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/sv-se/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/tr-tr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.869870 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-09 22:48:58.000000 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 22:48:58.000000 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:48:58.000000 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 22:48:58.000000 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 22:48:58.000000 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 22:48:58.000000 neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.869870 neon-skill-spelling-1.1.0/regex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.869870 neon-skill-spelling-1.1.0/regex/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/ca-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/da-dk/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/de-de/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/el-gr/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/en-us/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/es-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/fa-ir/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/fr-fr/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/gl-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/hu-hu/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/it-it/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/nl-nl/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/pl-pl/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/pt-br/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/ro-ro/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/ru-ru/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/sv-se/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/regex/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/regex/tr-tr/word.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.869870 neon-skill-spelling-1.1.0/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/ca-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/da-dk/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/de-de/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/el-gr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/en-us/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/es-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/fa-ir/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/fr-fr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.873870 neon-skill-spelling-1.1.0/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/gl-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/hu-hu/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/it-it/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/nl-nl/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/pl-pl/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/pt-br/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/ro-ro/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/ru-ru/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/sv-se/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:48:58.877870 neon-skill-spelling-1.1.0/vocab/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 22:48:56.000000 neon-skill-spelling-1.1.0/vocab/tr-tr/Spell.voc
```

### Comparing `neon-skill-spelling-1.0.1a2/LICENSE` & `neon-skill-spelling-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/LICENSE.md` & `neon-skill-spelling-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/PKG-INFO` & `neon-skill-spelling-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-spelling
-Version: 1.0.1a2
+Version: 1.1.0
 Home-page: https://github.com/NeonGeckoCom/skill-spelling
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-spelling-1.0.1a2/README.md` & `neon-skill-spelling-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/__init__.py` & `neon-skill-spelling-1.1.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/PKG-INFO` & `neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-spelling
-Version: 1.0.1a2
+Version: 1.1.0
 Home-page: https://github.com/NeonGeckoCom/skill-spelling
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/SOURCES.txt` & `neon-skill-spelling-1.1.0/neon_skill_spelling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/setup.py` & `neon-skill-spelling-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/skill.json` & `neon-skill-spelling-1.1.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a2/version.py` & `neon-skill-spelling-1.1.0/version.py`

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
+__version__ = "1.1.0"
```

