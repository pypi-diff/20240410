# Comparing `tmp/formation-studio-0.6.3.tar.gz` & `tmp/formation-studio-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formation-studio-0.6.3.tar", last modified: Thu Jan 11 23:40:32 2024, max compression
+gzip compressed data, was "formation-studio-0.7.0.tar", last modified: Wed Apr 10 17:10:23 2024, max compression
```

## Comparing `formation-studio-0.6.3.tar` & `formation-studio-0.7.0.tar`

### file list

```diff
@@ -1,130 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.953212 formation-studio-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-11 23:40:19.000000 formation-studio-0.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-11 23:40:19.000000 formation-studio-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-01-11 23:40:32.953212 formation-studio-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-01-11 23:40:19.000000 formation-studio-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.929212 formation-studio-0.6.3/formation/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.929212 formation-studio-0.6.3/formation/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/formats/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/formats/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/formats/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.929212 formation-studio-0.6.3/formation/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/handlers/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/handlers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/handlers/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/handlers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18745 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/meth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-01-11 23:40:19.000000 formation-studio-0.6.3/formation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.953212 formation-studio-0.6.3/formation_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-01-11 23:40:32.000000 formation-studio-0.6.3/formation_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-01-11 23:40:32.000000 formation-studio-0.6.3/formation_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 23:40:32.000000 formation-studio-0.6.3/formation_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-11 23:40:32.000000 formation-studio-0.6.3/formation_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-11 23:40:32.000000 formation-studio-0.6.3/formation_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-11 23:40:32.000000 formation-studio-0.6.3/formation_studio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.929212 formation-studio-0.6.3/hoverset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.941213 formation-studio-0.6.3/hoverset/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/image.bak
--rw-r--r--   0 runner    (1001) docker     (127)  6268365 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/image.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/image.dir
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/keymap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22989 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.941213 formation-studio-0.6.3/hoverset/platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/platform/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.941213 formation-studio-0.6.3/hoverset/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/color.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    18314 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/panels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/pickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.941213 formation-studio-0.6.3/hoverset/ui/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/themes/default.css
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/themes/light.css
--rw-r--r--   0 runner    (1001) docker     (127)   117200 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/ui/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.941213 formation-studio-0.6.3/hoverset/util/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/util/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/util/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-01-11 23:40:19.000000 formation-studio-0.6.3/hoverset/util/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-11 23:40:19.000000 formation-studio-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-11 23:40:19.000000 formation-studio-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 23:40:32.953212 formation-studio-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.945212 formation-studio-0.6.3/studio/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.945212 formation-studio-0.6.3/studio/debugtools/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/element_pane.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/debugtools/style_pane.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.949212 formation-studio-0.6.3/studio/feature/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/component_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/design.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/eventspane.py
--rw-r--r--   0 runner    (1001) docker     (127)    24252 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/stylepane.py
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/feature/variablepane.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.949212 formation-studio-0.6.3/studio/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35873 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/native.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/pseudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/toplevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/lib/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    38302 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.949212 formation-studio-0.6.3/studio/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/parsers/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.925212 formation-studio-0.6.3/studio/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.949212 formation-studio-0.6.3/studio/resources/images/
--rw-r--r--   0 runner    (1001) docker     (127)   225382 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/resources/images/formation.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/resources/images/formation.png
--rw-r--r--   0 runner    (1001) docker     (127)   218818 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/resources/images/formation_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/resources/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.953212 formation-studio-0.6.3/studio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/tools/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    45136 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/tools/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/tools/menus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:32.953212 formation-studio-0.6.3/studio/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/editors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/highlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-01-11 23:40:19.000000 formation-studio-0.6.3/studio/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.186184 formation-studio-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 17:10:13.000000 formation-studio-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 17:10:13.000000 formation-studio-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-10 17:10:23.186184 formation-studio-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-10 17:10:13.000000 formation-studio-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.158184 formation-studio-0.7.0/formation/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.162184 formation-studio-0.7.0/formation/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/formats/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/formats/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/formats/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.162184 formation-studio-0.7.0/formation/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/handlers/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/handlers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/handlers/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/handlers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/handlers/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/meth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-10 17:10:13.000000 formation-studio-0.7.0/formation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.186184 formation-studio-0.7.0/formation_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-10 17:10:23.000000 formation-studio-0.7.0/formation_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 17:10:23.000000 formation-studio-0.7.0/formation_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:10:23.000000 formation-studio-0.7.0/formation_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 17:10:23.000000 formation-studio-0.7.0/formation_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 17:10:23.000000 formation-studio-0.7.0/formation_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 17:10:23.000000 formation-studio-0.7.0/formation_studio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.162184 formation-studio-0.7.0/hoverset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.170184 formation-studio-0.7.0/hoverset/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/image.bak
+-rw-r--r--   0 runner    (1001) docker     (127)  3533931 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/image.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/image.dir
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/keymap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.154184 formation-studio-0.7.0/hoverset/data/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.154184 formation-studio-0.7.0/hoverset/data/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.170184 formation-studio-0.7.0/hoverset/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/locale/zh_CN/LC_MESSAGES/hoverset.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    24426 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.170184 formation-studio-0.7.0/hoverset/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/platform/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.174184 formation-studio-0.7.0/hoverset/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/color.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/panels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.174184 formation-studio-0.7.0/hoverset/ui/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/themes/default.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/themes/light.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121485 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/ui/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.174184 formation-studio-0.7.0/hoverset/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/util/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/util/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-10 17:10:13.000000 formation-studio-0.7.0/hoverset/util/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 17:10:13.000000 formation-studio-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 17:10:13.000000 formation-studio-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:10:23.186184 formation-studio-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.174184 formation-studio-0.7.0/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.178184 formation-studio-0.7.0/studio/debugtools/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/element_pane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/debugtools/style_pane.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.178184 formation-studio-0.7.0/studio/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/component_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19031 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42909 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/eventspane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29226 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/stylepane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/feature/variablepane.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.182184 formation-studio-0.7.0/studio/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/lib/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41356 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.182184 formation-studio-0.7.0/studio/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/parsers/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.158184 formation-studio-0.7.0/studio/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.182184 formation-studio-0.7.0/studio/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   225382 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/resources/images/formation.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/resources/images/formation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   218818 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/resources/images/formation_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/resources/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.158184 formation-studio-0.7.0/studio/resources/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.158184 formation-studio-0.7.0/studio/resources/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.186184 formation-studio-0.7.0/studio/resources/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/resources/locale/zh_CN/LC_MESSAGES/studio.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.186184 formation-studio-0.7.0/studio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/tools/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45483 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/tools/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/tools/menus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:23.186184 formation-studio-0.7.0/studio/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30717 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/editors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-10 17:10:13.000000 formation-studio-0.7.0/studio/updates.py
```

### Comparing `formation-studio-0.6.3/LICENSE.txt` & `formation-studio-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/PKG-INFO` & `formation-studio-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formation-studio
-Version: 0.6.3
+Version: 0.7.0
 Summary: Simplify GUI development in python
 Author-email: Emmanuel Obara <emmanuelobarany@gmail.com>
 License: MIT
 Project-URL: Documentation, https://formation-studio.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/ObaraEmmanuel/Formation/issues
 Project-URL: Source, https://github.com/ObaraEmmanuel/Formation
 Keywords: formation,gui,graphical-user-interface,drag drop,tkinter,hoverset,python
```

### Comparing `formation-studio-0.6.3/README.md` & `formation-studio-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/formats/__init__.py` & `formation-studio-0.7.0/formation/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/formats/_base.py` & `formation-studio-0.7.0/formation/formats/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/formats/_json.py` & `formation-studio-0.7.0/formation/formats/_json.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/formats/_xml.py` & `formation-studio-0.7.0/formation/formats/_xml.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from formation.formats._base import BaseFormat, Node
 
 namespaces = {
     "layout": "http://www.hoversetformationstudio.com/layouts/",
     "attr": "http://www.hoversetformationstudio.com/styles/",
     "menu": "http://www.hoversetformationstudio.com/menu",
+    "scroll": "http://www.hoversetformationstudio.com/scroll",
 }
 _reversed_namespaces = dict(zip(namespaces.values(), namespaces.keys()))
 _attr_rgx = re.compile(r"{(?P<namespace>.+)}(?P<attr>.+)")
 
 
 def _register_namespaces():
     for k in namespaces:
```

### Comparing `formation-studio-0.6.3/formation/handlers/__init__.py` & `formation-studio-0.7.0/formation/handlers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from formation.handlers import layout, image, misc
+from formation.handlers import layout, image, misc, scroll
 
 _namespace_handlers = {
     "attr": misc.AttrHandler,
     "menu": misc.MenuHandler,
     "layout": layout,
     "img": image,
+    "scroll": scroll
 }
 
 _handlers = {
     "image": image.parse_image
 }
```

### Comparing `formation-studio-0.6.3/formation/handlers/command.py` & `formation-studio-0.7.0/formation/handlers/command.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/handlers/image.py` & `formation-studio-0.7.0/formation/handlers/image.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/handlers/layout.py` & `formation-studio-0.7.0/formation/handlers/layout.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/handlers/misc.py` & `formation-studio-0.7.0/formation/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/loader.py` & `formation-studio-0.7.0/formation/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import tkinter as tk
 import tkinter.ttk as ttk
 
 from formation.formats import Node, BaseAdapter, infer_format
 from formation.handlers import dispatch_to_handlers, parse_arg
 from formation.meth import Meth
 from formation.handlers.image import parse_image
+from formation.handlers.scroll import apply_scroll_config
 import formation
 
 logger = logging.getLogger(__name__)
 
 _preloaded = {"tkinter": tk, "Tkinter": tk, "ttk": ttk, "tkinter.ttk": ttk}
 
 _variable_types = (
@@ -281,14 +282,17 @@
         # load meta and variables first
         self._load_meta(root_node, self)
         self._verify_version()
         # lazy load variables
         self._load_variables(root_node, self)
         node = self._load_widgets(root_node, self, self._parent)
         self._flush_var_cache()
+        if hasattr(self, "_scroll_map"):
+            apply_scroll_config(self, self._scroll_map)
+            delattr(self, "_scroll_map")
         return node
 
     def _load_variables(self, node, builder):
         for sub_node in node:
             if sub_node.is_var():
                 VariableLoaderAdapter.load(sub_node, builder)
```

### Comparing `formation-studio-0.6.3/formation/meth.py` & `formation-studio-0.7.0/formation/meth.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/preprocessors.py` & `formation-studio-0.7.0/formation/preprocessors.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation/utils.py` & `formation-studio-0.7.0/formation/utils.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/formation_studio.egg-info/PKG-INFO` & `formation-studio-0.7.0/formation_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formation-studio
-Version: 0.6.3
+Version: 0.7.0
 Summary: Simplify GUI development in python
 Author-email: Emmanuel Obara <emmanuelobarany@gmail.com>
 License: MIT
 Project-URL: Documentation, https://formation-studio.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/ObaraEmmanuel/Formation/issues
 Project-URL: Source, https://github.com/ObaraEmmanuel/Formation
 Keywords: formation,gui,graphical-user-interface,drag drop,tkinter,hoverset,python
```

### Comparing `formation-studio-0.6.3/formation_studio.egg-info/SOURCES.txt` & `formation-studio-0.7.0/formation_studio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 formation/__init__.py
+formation/__main__.py
 formation/loader.py
 formation/meth.py
 formation/preprocessors.py
 formation/utils.py
 formation/formats/__init__.py
 formation/formats/_base.py
 formation/formats/_json.py
 formation/formats/_xml.py
 formation/handlers/__init__.py
 formation/handlers/command.py
 formation/handlers/image.py
 formation/handlers/layout.py
 formation/handlers/misc.py
+formation/handlers/scroll.py
 formation_studio.egg-info/PKG-INFO
 formation_studio.egg-info/SOURCES.txt
 formation_studio.egg-info/dependency_links.txt
 formation_studio.egg-info/entry_points.txt
 formation_studio.egg-info/requires.txt
 formation_studio.egg-info/top_level.txt
 hoverset/__init__.py
 hoverset/data/__init__.py
 hoverset/data/actions.py
+hoverset/data/i18n.py
 hoverset/data/image.bak
 hoverset/data/image.dat
 hoverset/data/image.dir
 hoverset/data/images.py
 hoverset/data/keymap.py
 hoverset/data/preferences.py
 hoverset/data/utils.py
+hoverset/data/locale/zh_CN/LC_MESSAGES/hoverset.mo
 hoverset/platform/__init__.py
 hoverset/platform/functions.py
 hoverset/ui/__init__.py
 hoverset/ui/animation.py
 hoverset/ui/color.tcl
 hoverset/ui/dialogs.py
 hoverset/ui/icons.py
@@ -53,52 +57,60 @@
 hoverset/util/color.py
 hoverset/util/execution.py
 hoverset/util/validators.py
 studio/__init__.py
 studio/__main__.py
 studio/cli.py
 studio/context.py
+studio/i18n.py
 studio/launcher.py
 studio/main.py
 studio/preferences.py
 studio/resource_loader.py
+studio/selection.py
 studio/updates.py
 studio/debugtools/__init__.py
+studio/debugtools/__main__.py
 studio/debugtools/common.py
+studio/debugtools/console.py
 studio/debugtools/debugger.py
 studio/debugtools/defs.py
 studio/debugtools/element_pane.py
+studio/debugtools/hook.py
 studio/debugtools/layouts.py
 studio/debugtools/preferences.py
+studio/debugtools/selection.py
 studio/debugtools/style_pane.py
 studio/feature/__init__.py
 studio/feature/_base.py
 studio/feature/component_tree.py
 studio/feature/components.py
 studio/feature/design.py
 studio/feature/eventspane.py
 studio/feature/stylepane.py
 studio/feature/variablepane.py
 studio/lib/__init__.py
 studio/lib/canvas.py
 studio/lib/events.py
+studio/lib/handles.py
 studio/lib/layouts.py
 studio/lib/legacy.py
 studio/lib/menu.py
 studio/lib/native.py
 studio/lib/properties.py
 studio/lib/pseudo.py
 studio/lib/toplevel.py
 studio/lib/variables.py
 studio/parsers/__init__.py
 studio/parsers/loader.py
 studio/resources/images/formation.ico
 studio/resources/images/formation.png
 studio/resources/images/formation_icon.png
 studio/resources/images/logo.png
+studio/resources/locale/zh_CN/LC_MESSAGES/studio.mo
 studio/tools/__init__.py
 studio/tools/_base.py
 studio/tools/canvas.py
 studio/tools/menus.py
 studio/ui/__init__.py
 studio/ui/about.py
 studio/ui/editors.py
```

### Comparing `formation-studio-0.6.3/hoverset/data/actions.py` & `formation-studio-0.7.0/hoverset/data/actions.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/data/images.py` & `formation-studio-0.7.0/hoverset/data/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,16 @@
     color = to_rgb(color) if isinstance(color, str) else color
     # expand to RGBA color
     color = (*color, 255)
     pix = image.load()
 
     for x in range(image.size[0]):
         for y in range(image.size[1]):
-            if luminosity(pix[x, y]) > 65:
+            if pix[x, y][3] != 0:
                 pix[x, y] = color
-            else:
-                pix[x, y] = (0, 0, 0, 0)
 
     return image
 
 
 # We want to enable memoization to reduce the number of times we read the image database
 # An image can be accessed multiple times in the application lifetime hence a cache can improve performance greatly
 @functools.lru_cache()
```

### Comparing `formation-studio-0.6.3/hoverset/data/keymap.py` & `formation-studio-0.7.0/hoverset/data/keymap.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import hoverset.data.actions as actions
 from hoverset.data.preferences import SharedPreferences, Component
 from hoverset.data.images import get_tk_image
 from hoverset.platform import platform_is, LINUX
 from hoverset.ui.widgets import Frame, Label, CompoundList
 from hoverset.ui.dialogs import MessageDialog
 from hoverset.ui.menu import EnableIf
+from hoverset.data.i18n import _
 
 
 class Key:
 
     def __init__(self, label, *keycodes):
         self.label = label
         self._keycodes = frozenset(keycodes)
@@ -313,46 +314,46 @@
         self.shortcut_pane = shortcut_pane
 
     def on_key_change(self, event, with_alt=False):
         self.key = KeyMap.get_key(event, with_alt)
         if self.shortcut_pane is not None:
             routine = self.shortcut_pane.routine_from_shortcut(self.key)
             if routine is not None and self.shortcut_pane:
-                self._warning['text'] = f"Key already assigned to {routine.desc}"
+                self._warning['text'] = _("Key already assigned to {}").format(routine.desc)
                 self._warning.pack(fill="x")
             else:
                 self._warning.pack_forget()
         self.event_pad.config(text=self.key.label)
         # returning break ensures this event does not propagate
         # preventing the event from invoking currently set bindings
         return "break"
 
     def on_key_change_alt(self, event):
         self.on_key_change(event, with_alt=True)
 
-    def render(self, _):
+    def render(self, __):
         self.detail = Label(self, **self.style.text, text=self.message)
         self.detail.pack(fill="x")
         warn_frame = Frame(self, **self.style.surface)
         self._warning = Label(
             warn_frame,
             **self.style.text_passive,
             padx=5,
             anchor='w',
             compound="left",
             image=get_tk_image("dialog_warning", 15, 15),
         )
         self.event_pad = Label(
             self, **self.style.text_accent)
-        self._add_button(text="Cancel", value=None)
-        self._add_button(text="Okay", command=self.exit_with_key, focus=True)
+        self._add_button(text=_("Cancel"), value=None)
+        self._add_button(text=_("Okay"), command=self.exit_with_key, focus=True)
         warn_frame.pack(side="bottom", fill="x")
         self.event_pad.config(
             **self.style.bright, takefocus=True,
-            text="Tap here to begin capturing shortcuts."
+            text=_("Tap here to begin capturing shortcuts.")
         )
         self.event_pad.bind("<Any-KeyPress>", self.on_key_change)
         # for some reason alt needs to be bound separately
         self.event_pad.bind("<Alt-KeyPress>", self.on_key_change_alt)
         self.event_pad.bind("<Button-1>", lambda e: self.event_pad.focus_set())
         self.event_pad.pack(fill="both", expand=True)
 
@@ -402,31 +403,31 @@
             if flag:
                 self.desc.config(**self.style.text_passive)
                 self.key_label.config(**self.style.text_passive)
             else:
                 self.desc.config(**self.style.text)
                 self.key_label.config(**self.style.text_accent)
 
-    def __init__(self, master, pref: SharedPreferences, path, _, **__):
+    def __init__(self, master, pref: SharedPreferences, path, __, **___):
         super().__init__(master)
         self.config(**self.style.surface)
         self.bindings = {}
         self.is_disabled = False
         self.load(pref, path)
         self.shortcut_list = CompoundList(self)
         self.shortcut_list.set_item_class(ShortcutPane.ShortcutItem)
         self.shortcut_list.set_values(list(self.bindings.items()))
         self.shortcut_list.pack(fill="both", expand=True)
         self.shortcut_list.body.set_up_context((
             EnableIf(
                 lambda: (not self.is_disabled) and self.shortcut_list.get(),
-                ("command", "Change Shortcut", get_tk_image('edit', 14, 14), self.pick_key, {}),
+                ("command", _("Change Shortcut"), get_tk_image('edit', 14, 14), self.pick_key, {}),
                 EnableIf(
                     lambda: self.shortcut_list.get() and self.shortcut_list.get().value[1] != BlankKey,
-                    ("command", "Remove", get_tk_image('delete', 14, 14), self.remove_key, {})
+                    ("command", _("Remove"), get_tk_image('delete', 14, 14), self.remove_key, {})
                 ),
             ),
         ))
 
     def remove_key(self):
         if self.shortcut_list.get():
             item = self.shortcut_list.get()
```

### Comparing `formation-studio-0.6.3/hoverset/data/preferences.py` & `formation-studio-0.7.0/hoverset/data/preferences.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,41 @@
 import typing
 from pathlib import Path
 from collections import defaultdict
 
 from hoverset.data.utils import make_path
 from hoverset.data.images import get_tk_image
 from hoverset.data.actions import get_routine
+from hoverset.data.i18n import _
 from hoverset.util.validators import numeric_limit
 from hoverset.ui.icons import get_icon_image as icon
 from hoverset.ui.dialogs import MessageDialog
 from hoverset.ui.widgets import *
 
 __all__ = (
     "SharedPreferences",
+    "Choice",
     "Component",
     "ComponentGroup",
     "PreferenceManager",
     "DependentGroup",
     "Check",
     "RadioGroup",
     "Number",
     "LabeledScale",
     "Note",
     "ListControl"
 )
 
 
+def open_raw_shelve(app, author, file, *args):
+    path = os.path.join(platformdirs.AppDirs(app, author).user_config_dir, file)
+    return shelve.open(path, *args)
+
+
 class _PreferenceInstanceCreator(type):
     """
     We need to ensure only one config handler exists for a given config file
     """
     _instances = {}
 
     def __call__(cls, app, author, file, defaults, **kwargs):
@@ -445,14 +452,46 @@
         super(Check, self).disable(flag)
         if flag:
             self.config(state='disabled')
         else:
             self.config(state='normal')
 
 
+class Choice(Component, Frame):
+
+        def __init__(self, master, pref, path, desc, choices, **extra):
+            super().__init__(master, **extra)
+            self._choice_map = {}
+            for i, choice in choices:
+                self._choice_map[choice] = i
+                self._choice_map[i] = choice
+
+            self._label = Label(self, text=desc, **self.style.text)
+            self._label.pack(side="left")
+            self._spinner = Spinner(self, **extra)
+            self._spinner.set_values([i[1] for i in choices])
+            self._spinner.on_change(self._change)
+            self._spinner.config(width=max(map(lambda x: len(x[1]), choices)) * 8, height=25)
+            self._spinner.pack_propagate(0)
+            self._spinner.pack(side="left", padx=5)
+            self.config_all(**self.style.surface)
+            self.load(pref, path)
+
+        def disable(self, flag):
+            super(Choice, self).disable(flag)
+            self._spinner.disabled(flag)
+            self._label.disabled(flag)
+
+        def set(self, value):
+            self._spinner.set(self._choice_map.get(value, ''))
+
+        def get(self):
+            return self._choice_map.get(self._spinner.get(), '')
+
+
 class Note(Label):
     """
     Adds small extra notes between preferences components
     """
 
     def __init__(self, parent, desc, **extra):
         super(Note, self).__init__(parent)
@@ -538,15 +577,15 @@
             self.config_all(**self.style.surface)
 
         def on_hover_ended(self, *_):
             self.config_all(**self.style.bright)
 
     def __init__(self, master, pref, templates):
         super().__init__(master, self.render)
-        self.title("Preferences")
+        self.title(_("Preferences"))
         self.resizable(1, 1)
         self.nav.on_change(self._change_category)
         self.templates = templates
         self.pref = pref
         self.components = set()
         self._category_render = {}
         self._load_template(templates)
@@ -663,18 +702,18 @@
         pane.add(self.pref_frame, width=450, minsize=200, sticky="nswe")
         self._make_button_bar()
         warning_bar = Frame(self.bar, **self.style.surface)
         warning_bar.pack(side="left")
         self._restart_label = Label(
             warning_bar, **self.style.text, compound="left",
             image=get_tk_image("dialog_info", 20, 20),
-            text="Some changes require restart"
+            text=_("Some changes require restart")
         )
         self._restart_button = Button(
-            warning_bar, **self.style.button, text="restart", height=25,
+            warning_bar, **self.style.button, text=_("restart"), height=25,
         )
-        self._restart_button.configure(width=self._restart_button.measure_text("restart"))
+        self._restart_button.configure(width=self._restart_button.measure_text(_("restart")))
         self._restart_button.on_click(self.apply_and_restart)
         self._restart_button.configure(**self.style.highlight_active)
-        self.cancel_btn = self._add_button(text="Cancel", command=self.cancel)
-        self.okay_btn = self._add_button(text="Okay", command=self.okay, focus=True)
+        self.cancel_btn = self._add_button(text=_("Cancel"), command=self.cancel)
+        self.okay_btn = self._add_button(text=_("Okay"), command=self.okay, focus=True)
         pane.pack(side="top", fill='both', expand=True)
```

### Comparing `formation-studio-0.6.3/hoverset/data/utils.py` & `formation-studio-0.7.0/hoverset/data/utils.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/platform/__init__.py` & `formation-studio-0.7.0/hoverset/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/platform/functions.py` & `formation-studio-0.7.0/hoverset/platform/functions.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/animation.py` & `formation-studio-0.7.0/hoverset/ui/animation.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/color.tcl` & `formation-studio-0.7.0/hoverset/ui/color.tcl`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/dialogs.py` & `formation-studio-0.7.0/hoverset/ui/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # ======================================================================= #
 # Copyright (C) 2020 Hoverset Group.                                      #
 # ======================================================================= #
 
 from hoverset.ui.widgets import Frame, Label, Window, Button, Application, ProgressBar
 from hoverset.ui.icons import get_icon_image
 from hoverset.platform import platform_is, WINDOWS, MAC
+from hoverset.data.i18n import _
 
 
 class MessageDialog(Window):
     """
     Main class for creation of hoverset themed alert dialogs. It has the various initialization
     methods for the common dialogs. The supported forms/types are shown below:
 
@@ -144,15 +145,16 @@
             left displacement and positive for right displacement
         """
         # a value of -1 in self._reaction is a sentinel indicating no reaction is ongoing
         if self._reaction > MessageDialog._MAX_SHAKES:
             self._reaction = -1
             return
         try:
-            *_, x, y = self.get_geometry()
+            _, *xy = self.geometry().split("+")
+            x, y = map(int, xy)
             x += step
             self.geometry('+{}+{}'.format(x, y))
             self.after(100, lambda: self._react(step * -1))
             self._reaction += 1
         except Exception:
             self._reaction = -1
             pass
@@ -196,43 +198,43 @@
               text=text, anchor="w", compound="left", wrap=600, justify="left",
               pady=5, padx=15, image=get_icon_image(icon, 50, 50)
               ).pack(side="top", fill="x")
 
     def _ask_okay_cancel(self, **kw):
         self.title(kw.get("title", self.title()))
         self._message(kw.get("message"), kw.get("icon", self.ICON_INFO))
-        self._add_button(text="Cancel", focus=True, command=lambda _: self._terminate_with_val(False))
-        self._add_button(text="Ok", command=lambda _: self._terminate_with_val(True))
+        self._add_button(text=_("Cancel"), focus=True, command=lambda _: self._terminate_with_val(False))
+        self._add_button(text=_("Ok"), command=lambda _: self._terminate_with_val(True))
 
     def _ask_yes_no(self, **kw):
         self.title(kw.get("title", self.title()))
         self._message(kw.get("message"), kw.get("icon", self.ICON_INFO))
-        self._add_button(text="No", focus=True, command=lambda _: self._terminate_with_val(False))
-        self._add_button(text="Yes", command=lambda _: self._terminate_with_val(True))
+        self._add_button(text=_("No"), focus=True, command=lambda _: self._terminate_with_val(False))
+        self._add_button(text=_("Yes"), command=lambda _: self._terminate_with_val(True))
 
     def _ask_retry_cancel(self, **kw):
         self.title(kw.get("title", self.title()))
         self._message(kw.get("message"), kw.get("icon", self.ICON_WARNING))
-        self._add_button(text="Cancel", command=lambda _: self._terminate_with_val(False))
-        self._add_button(text="Retry", focus=True, command=lambda _: self._terminate_with_val(True))
+        self._add_button(text=_("Cancel"), command=lambda _: self._terminate_with_val(False))
+        self._add_button(text=_("Retry"), focus=True, command=lambda _: self._terminate_with_val(True))
 
     def _show_error(self, **kw):
         self.title(kw.get("title", self.title()))
         self._message(kw.get("message"), kw.get("icon", self.ICON_ERROR))
-        self._add_button(text="Ok", focus=True, command=lambda _: self.destroy())
+        self._add_button(text=_("Ok"), focus=True, command=lambda _: self.destroy())
 
     def _show_warning(self, **kw):
         self.title(kw.get("title", self.title()))
         self._message(kw.get("message"), kw.get("icon", self.ICON_WARNING))
-        self._add_button(text="Ok", focus=True, command=lambda _: self.destroy())
+        self._add_button(text=_("Ok"), focus=True, command=lambda _: self.destroy())
 
     def _show_info(self, **kw):
         self.title(kw.get("title", self.title()))
         self._message(kw.get("message"), kw.get("icon", self.ICON_INFO))
-        self._add_button(text="Ok", focus=True, command=lambda _: self.destroy())
+        self._add_button(text=_("Ok"), focus=True, command=lambda _: self.destroy())
 
     def _show_progress(self, **kw):
         self.title(kw.get("title", self.title()))
         text = kw.get('message', 'progress')
         icon = None
         if kw.get('icon'):
             icon = get_icon_image(kw.get('icon'), 50, 50)
```

### Comparing `formation-studio-0.6.3/hoverset/ui/loaders.py` & `formation-studio-0.7.0/hoverset/ui/loaders.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/menu.py` & `formation-studio-0.7.0/hoverset/ui/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,16 @@
                         {**style.context_menu_selectable} if _type in ("radiobutton", "checkbutton")
                         else {**style.context_menu_item})
                     if config.get('state') == tk.DISABLED:
                         # We need to work around tkinter default disabled look if possible
                         # look which tends to render incorrectly
                         config.update(**style.context_menu_disabled, state=tk.NORMAL)
                         command = None
+                        # Would be nice to gray out the icon but that is not possible, so we just remove it
+                        icon = None
                         # block the menu as well
                         if 'menu' in config:
                             config['menu'] = None
                 cls.image_cache.add(icon)
                 if template[0] == "cascade":
                     # Create cascade menu recursively
                     # the menu should be dynamic as well
```

### Comparing `formation-studio-0.6.3/hoverset/ui/panels.py` & `formation-studio-0.7.0/hoverset/ui/panels.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 
 from hoverset.ui.widgets import *
 from hoverset.ui.icons import get_icon_image
 from hoverset.util.color import to_hex, to_rgb, to_hsl, from_hsl, to_hsv, from_hsv
 from hoverset.util.validators import check_hex_color, numeric_limit
 from hoverset.platform.functions import image_grab
+from hoverset.data.i18n import _
 
 
 class _FloatingColorWindow(Frame):
 
     def __init__(self, master=None, **cnf):
         super().__init__(master, **cnf)
         self.label = Label(self, **self.style.surface)
@@ -47,15 +48,15 @@
         self.label.config(bg=self.color)
 
 
 class ColorPicker(Button):
 
     def __init__(self, master=None, **cnf):
         super().__init__(master, **cnf, image=get_icon_image("colorpicker", 15, 15))
-        self.tooltip('Pick color from anywhere')
+        self.tooltip(_('Pick color from anywhere'))
         self.image = None
         self.on_click(self.start)
         self._window = None
         self._on_pick = None
         self._color_win = None
         self._body = None
         self.active = False
@@ -126,15 +127,15 @@
         self._picker = picker = ColorPicker(self, width=25, height=25, **self.style.button)
         picker.grid(row=1, column=2, padx=2, pady=2, sticky="n")
         picker.on_pick(self.set)
         clipboard = Button(self, width=25, height=25,
                            image=get_icon_image("clipboard", 15, 15), **self.style.button)
         clipboard.grid(row=1, column=3, padx=2, pady=2, sticky="n")
         clipboard.on_click(self.pick_from_clipboard)
-        clipboard.tooltip('Pick color from clipboard')
+        clipboard.tooltip(_('Pick color from clipboard'))
         self.current_model = self.models.get(self.model_select.get())
         self.attach(self.current_model)
 
     @property
     def picker_active(self):
         return self._picker.active
 
@@ -340,16 +341,16 @@
         self.v.set(round(v))
         self.initial = hex_str
 
 
 class FontPicker(Button):
 
     def __init__(self, master=None, **cnf):
-        super().__init__(master, **cnf, image=get_icon_image("eye", 15, 15))
-        self.tooltip("Pick Font")
+        super().__init__(master, **cnf, image=get_icon_image("colorpicker", 15, 15, color="#A235D4"))
+        self.tooltip(_("Pick Font"))
         self.bind_all('<Button-1>', self.pick, add='+')
         self.bind_all('<Motion>', self._render, add='+')
         self.active = False
         self._grabbed = None
         self._window = None
         self._indicator = None
 
@@ -378,15 +379,15 @@
     def _render(self, event):
         if not self.active:
             return
         displace_x = 10 if self.winfo_screenwidth() - event.x_root > 160 else -160
         displace_y = 0 if self.winfo_screenheight() - event.y_root > 40 else -30
         font_value = self._get_font(event.x_root, event.y_root)
         _font = FontStyle(self, font=font_value)
-        self._indicator['text'] = _font.cget('family') or 'No font to extract'
+        self._indicator['text'] = _font.cget('family') or _('No font to extract')
         if font_value:
             self._indicator['font'] = _font
         else:
             self._indicator['font'] = 'TkDefaultFont'
 
         self._window.geometry(
             '{width}x{height}+{x}+{y}'.format(
```

### Comparing `formation-studio-0.6.3/hoverset/ui/pickers.py` & `formation-studio-0.7.0/hoverset/ui/pickers.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/styles.py` & `formation-studio-0.7.0/hoverset/ui/styles.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/themes/default.css` & `formation-studio-0.7.0/hoverset/ui/themes/default.css`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/themes/light.css` & `formation-studio-0.7.0/hoverset/ui/themes/light.css`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/ui/widgets.py` & `formation-studio-0.7.0/hoverset/ui/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 # ======================================================================= #
 # Copyright (C) 2019 Hoverset Group.                                      #
 # ======================================================================= #
 import abc
 import functools
 import logging
 import os
-import re
-import webbrowser
 import tkinter as tk
 import tkinter.ttk as ttk
+import webbrowser
 from collections import namedtuple
 from tkinter import font
 
+from tkinterDnD.tk import _init_tkdnd
+
+import hoverset.ui
 from hoverset.data.images import load_image_to_widget
 from hoverset.data.utils import get_resource_path, get_theme_path
 from hoverset.platform import platform_is, WINDOWS, LINUX, MAC
 from hoverset.ui.animation import Animate, Easing
 from hoverset.ui.icons import get_icon_image
+from hoverset.ui.menu import MenuUtils, LoadLater
 from hoverset.ui.styles import StyleDelegator
 from hoverset.ui.windows import DragWindow
-from hoverset.ui.menu import MenuUtils, LoadLater
-import hoverset.ui
-
-from tkinterDnD.tk import _init_tkdnd
 
 __all__ = (
     "Application",
+    "AutoScroll",
     "Button",
     "Canvas",
     "CenterWindowMixin",
     "Checkbutton",
     "ComboBox",
     "CompoundList",
     "ContextMenuMixin",
@@ -1119,21 +1119,22 @@
 
 
 class SpinBox(Widget, EditableMixin, tk.Spinbox):
 
     def __init__(self, master=None, **cnf):
         self.setup(master)
         super().__init__(master, **cnf)
-        self._var = tk.IntVar()
+        self._var = tk.DoubleVar()
         self.config(textvariable=self._var)
 
     def get(self):
         self.update_idletasks()
         try:
-            return self._var.get()
+            val = self._var.get()
+            return int(val) if val % 1 == 0 else val
         except tk.TclError:
             return ''
 
     def set(self, value):
         self._var.set(value)
         self.update_idletasks()
 
@@ -1372,14 +1373,35 @@
         bbox = self._canvas.bbox('all')
         return bbox[3] - bbox[1] + 3
 
     def scroll_to_start(self):
         self._canvas.yview_moveto(0.0)
         self._canvas.xview_moveto(0.0)
 
+    def scroll_to(self, widget):
+        self._canvas.update_idletasks()
+        widget.update_idletasks()
+        bbox = self._canvas.bbox('all')
+
+        if self._scroll_x.winfo_ismapped():
+            r_x = self._canvas.winfo_rootx()
+            w_x = widget.winfo_rootx()
+            w = bbox[2] - bbox[0]
+            x_off = self._canvas.xview()[0] * w
+            x = w_x - r_x + x_off
+            self._canvas.xview_moveto(x / w)
+
+        if self._scroll_y.winfo_ismapped():
+            r_y = self._canvas.winfo_rooty()
+            w_y = widget.winfo_rooty()
+            h = bbox[3] - bbox[1]
+            y_off = self._canvas.yview()[0] * h
+            y = w_y - r_y + y_off
+            self._canvas.yview_moveto(y / h)
+
     def xview_scroll(self, n, what):
         return self._canvas.xview_scroll(n, what)
 
     def yview_scroll(self, n, what):
         return self._canvas.yview_scroll(n, what)
 
     def xview_moveto(self, fraction):
@@ -2555,14 +2577,18 @@
             cls = self.__class__
             cls.EXPANDED_ICON = get_icon_image("chevron_down", 14, 14)
             cls.COLLAPSED_ICON = get_icon_image("chevron_right", 14, 14)
             cls.BLANK = get_icon_image("blank", 14, 14)
             cls.__icons_loaded = True
 
         @property
+        def selected(self):
+            return self._selected
+
+        @property
         def depth(self):
             return self._depth
 
         @depth.setter
         def depth(self, value):
             self._depth = value
             self._spacer["width"] = 14 * (value - 1) + 1  # width cannot be set to completely 0 so add 1 just in case
@@ -2706,34 +2732,32 @@
             elif node in self.nodes:
                 # We need a local copy of the expanded flag since calling collapse resets
                 was_expanded = self._expanded
                 # Collapse parent so that layout changes caused by removal of a node can be applied
                 self.collapse()
                 self.nodes.remove(node)
                 node.pack_forget()
-                if was_expanded:
+                if was_expanded and len(self.nodes) > 0:
                     # If the parent was expanded when we began removal we expand it again
                     self.expand()
-                if len(self.nodes) == 0:
+                if not self.nodes:
                     # remove the expansion icon
                     self._set_expander(self.BLANK)
 
         def expand(self):
-            if len(self.nodes) == 0:
-                # There is nothing to expand
+            if self._expanded or not self.nodes:
                 return
             self.pack_propagate(True)
             for node in filter(lambda n: n._visible, self.nodes):
                 node.pack(in_=self.body, fill="x", side="top", pady=self.PADDING)
             self._set_expander(self.EXPANDED_ICON)
             self._expanded = True
 
         def collapse(self):
-            if len(self.nodes) == 0:
-                # There is nothing to collapse
+            if not self._expanded:
                 return
             for node in self.nodes:
                 node.pack_forget()
             self.pack_propagate(False)
             self.config(height=self.strip.winfo_height())
             self._set_expander(self.COLLAPSED_ICON)
             self._expanded = False
@@ -2968,14 +2992,34 @@
     def expand_all(self):
         """
         Expand all nodes and sub-nodes so that their sub-nodes are displayed
         """
         for node in self.nodes:
             node.expand_all()
 
+    def see(self, node):
+        """
+        Expand all nodes from the root to the given node so that the node is visible
+
+        :param node: The node to be expanded to
+        """
+        hierarchy = []
+        orig_node = node
+        while hasattr(node.parent_node, "parent_node"):
+            hierarchy.append(node.parent_node)
+            node = node.parent_node
+
+        for node in reversed(hierarchy):
+            if hasattr(node, "expand"):
+                node.expand()
+
+        scrollframe: ScrolledFrame = Widget.ancestor_first(orig_node, ScrolledFrame)
+        if scrollframe:
+            scrollframe.scroll_to(orig_node)
+
     def selected_count(self) -> int:
         """
         Return the total number of items currently selected usually 1 if multi-select is disabled.
 
         :return: total number of items selected
         """
         return len(self._selected)
@@ -3423,14 +3467,95 @@
     def set(self, value):
         self.clear()
         super().insert("1.0", value)
         # this will suppress the next <<Modified>> event fired as a result
         self._last_edit_implicit = True
 
 
+class AutoScroll(Widget, ScrollableInterface, tk.Frame):
+    NONE = 0
+    Y = 1
+    X = 2
+    BOTH = 3
+
+    def __init__(self, master, **cnf):
+        self.setup(master)
+        super().__init__(master)
+        self.configure(**self.style.surface)
+        self.configure(**cnf)
+        self.child = None
+        self._scroll = False
+        self._y_bar = ttk.Scrollbar(self, orient='vertical')
+        self._x_bar = ttk.Scrollbar(self, orient='horizontal')
+        self.columnconfigure(0, weight=1)  # Ensure the child gets the rest of the left horizontal space
+        self.rowconfigure(0, weight=1)  # Ensure the child gets the rest of the left vertical space
+
+    def show_scroll(self, val):
+        self._scroll = val
+        if self.child is not None:
+            self._reconfig()
+
+    def set_child(self, child):
+        if self.child is not None:
+            self.child.configure(xscrollcommand=None, yscrollcommand=None)
+            self._y_bar.configure(command=None)
+            self._x_bar.configure(command=None)
+
+        self.child = child
+        self.child.configure(xscrollcommand=self._trigger_x, yscrollcommand=self._trigger_y)
+        self._y_bar.config(command=self.child.yview)
+        self._x_bar.config(command=self.child.xview)
+        self.child.grid(row=0, column=0, sticky='nsew')
+        self._reconfig()
+
+    def _reconfig(self):
+        if not self._scroll or not self.child:
+            self._y_bar.grid_forget()
+            self._x_bar.grid_forget()
+            return
+
+        if self._scroll & 1:
+            # y scroll
+            flag = self.child.yview() != (0.0, 1.0)
+            if flag and not self._y_bar.winfo_ismapped():
+                self._y_bar.grid(row=0, column=1, sticky='ns')
+            elif not flag:
+                self._y_bar.grid_forget()
+
+        if self._scroll & 2:
+            # x scroll
+            flag = self.child.xview() != (0.0, 1.0)
+            if flag and not self._x_bar.winfo_ismapped():
+                self._x_bar.grid(row=1, column=0, sticky='ew')
+            elif not flag:
+                self._x_bar.grid_forget()
+
+    def _trigger_x(self, start, end):
+        self._reconfig()
+        self._x_bar.set(start, end)
+
+    def _trigger_y(self, start, end):
+        self._reconfig()
+        self._y_bar.set(start, end)
+
+    def on_mousewheel(self, event):
+        # Enable the scrollbar to be scrolled using mouse wheel
+        # Occasionally throws unpredictable errors so we better wrap it up in a try block
+        try:
+            if event.state & EventMask.SHIFT and self._x_bar.winfo_ismapped():
+                self.handle_wheel(self.child, event)
+            elif self._y_bar.winfo_ismapped():
+                self.handle_wheel(self.child, event)
+        except tk.TclError:
+            pass
+
+    def scroll_position(self):
+        return self._y_bar.get()
+
+
 if __name__ == "__main__":
     # test
     r = Application()
     r.config(bg='red')
     r.load_styles("themes/default.css")
     r.geometry('500x400')
     tab = TabView(r, bg="red")
```

### Comparing `formation-studio-0.6.3/hoverset/ui/windows.py` & `formation-studio-0.7.0/hoverset/ui/windows.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/util/__init__.py` & `formation-studio-0.7.0/hoverset/util/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/util/color.py` & `formation-studio-0.7.0/hoverset/util/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     Takes in a rgb tuple (h, s, l) where h s and l lie between 0 and 255 or four bit hex color #xxx
     and returns a hex string that lies between #000000 and #ffffff
     It raises Value error if any of the values h s or l is not within 0 and 255
 
     :param rgb: rgb tuple (h, s, l) where h s and l lie between 0 and 255
     :return: hex string that lies between #000000 and #ffffff
     """
-    rgb = tuple(map(lambda x: hex(x)[2:], rgb))
+    rgb = tuple(map(lambda x: hex(int(x))[2:], rgb))
     rgb = tuple(map(lambda x: ("0" + x).zfill(2)[-2:], rgb))
     return "#" + "".join(rgb)
 
 
 @to_hex.register
 def _(hex_str: str) -> str:
     # TODO Add error handling
```

### Comparing `formation-studio-0.6.3/hoverset/util/execution.py` & `formation-studio-0.7.0/hoverset/util/execution.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/hoverset/util/validators.py` & `formation-studio-0.7.0/hoverset/util/validators.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/pyproject.toml` & `formation-studio-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["*.tests*", "venv"]
 namespaces = false
 
 [tool.setuptools.package-data]
-"hoverset.data" = ["image.*"]
+"hoverset.data" = ["image.*", "locale/*/LC_MESSAGES/*.mo"]
 "hoverset.ui" = ["themes/*", "*.tcl"]
-studio = ["resources/*/*"]
+studio = ["resources/images/*", "resources/locale/*/LC_MESSAGES/*.mo"]
 
 [project.scripts]
 formation-studio = "studio.launcher:main"
 formation-cli = "studio.cli:main"
-formation-dbg = "studio.debugtools.debugger:main"
+formation-dbg = "studio.debugtools.hook:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "formation.__version__"}
 
 [project.optional-dependencies]
 lxml = ["lxml"]
 docs = ["Sphinx==4.0.3", "sphinx-rtd-theme==1.0.0"]
```

### Comparing `formation-studio-0.6.3/studio/cli.py` & `formation-studio-0.7.0/studio/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import sys
 import logging
 import shutil
 import os
 import platformdirs
 
+from studio.i18n import _
+
 from hoverset.util.execution import elevate
 from hoverset.platform import platform_is, WINDOWS
 
 import studio
 from studio.preferences import Preferences
 
 dirs = platformdirs.AppDirs(appname="formation", appauthor="hoverset")
@@ -20,46 +22,46 @@
 logger.setLevel(logging.INFO)
 
 
 def get_parser():
 
     parser = argparse.ArgumentParser(
         prog="formation-cli",
-        description="Command line tools for formation studio"
+        description=_("Command line tools for formation studio")
     )
 
     parser.add_argument(
         "-r",
         "--remove",
         metavar="FILES",
         default=None,
-        help="""
+        help=_("""
             Removes and cleans internal app files. Can be set to
             config, cache or all.
-        """,
+        """),
     )
 
     parser.add_argument(
         "-c",
         "--config",
         action="store",
         nargs="+",
         metavar=("KEY", "VALUES"),
-        help="""
+        help=_("""
             Get or set studio configuration values.
-        """,
+        """),
     )
 
     parser.add_argument(
         "-u",
         "--upgrade",
         action="store_true",
-        help="""
+        help=_("""
             Upgrade formation studio to latest version
-        """,
+        """),
     )
 
     parser.add_argument(
         "-v", "--version", action="version", version="%(prog)s " + studio.__version__
     )
 
     return parser
@@ -67,34 +69,34 @@
 
 def _clear_config():
     if not os.path.exists(dirs.user_config_dir):
         sys.exit(0)
     try:
         Preferences.acquire()
     except Preferences.ConfigFileInUseError:
-        logger.error(
+        logger.error(_(
             "Config file currently in use. Close any open formation studio "
             "windows to continue."
-        )
+        ))
         sys.exit(1)
     except:
         pass
     try:
         shutil.rmtree(dirs.user_config_dir)
     except:
-        logger.error("Could not delete config files")
+        logger.error(_("Could not delete config files"))
 
 
 def _clear_cache():
     if not os.path.exists(dirs.user_cache_dir):
         sys.exit(0)
     try:
         shutil.rmtree(dirs.user_cache_dir)
     except:
-        logger.error("Could not delete cache files")
+        logger.error(_("Could not delete cache files"))
 
 
 def _parse(value):
     # try to convert to numerical type if possible
     if value.isdigit():
         value = int(value)
     else:
@@ -105,24 +107,24 @@
     return value
 
 
 def remove(args):
     arg = args.remove
     if arg == 'config':
         _clear_config()
-        logger.info("Removed config files")
+        logger.info(_("Removed config files"))
     elif arg == 'cache':
         _clear_cache()
-        logger.info("Removed cache files")
+        logger.info(_("Removed cache files"))
     elif arg == 'all':
         _clear_cache()
         _clear_config()
-        logger.info("Removed config and cache files")
+        logger.info(_("Removed config and cache files"))
     else:
-        logger.error("Unknown argument %s", arg)
+        logger.error(_("Unknown argument %s"), arg)
         sys.exit(1)
 
 
 def neat_print(value):
     if isinstance(value, list):
         for i in value:
             print(i)
@@ -130,34 +132,34 @@
         print(value)
 
 
 def handle_config(args):
     try:
         pref = Preferences.acquire()
     except Preferences.ConfigFileInUseError:
-        logger.error(
+        logger.error(_(
             "Config file currently in use. Close any open formation studio "
             "windows to continue."
-        )
+        ))
         sys.exit(1)
     except Exception:
-        logger.error("Unable to open config files")
+        logger.error(_("Unable to open config files"))
         sys.exit(1)
 
     param = args.config
     key = param[0].replace(".", "::")
     if pref.exists(key):
         if len(param) == 1:
             neat_print(pref.get(key))
         elif len(param) == 2:
             pref.set(key, _parse(param[1]))
         else:
             pref.set(key, [_parse(v) for v in param[1:]])
         sys.exit(0)
-    logger.error("Key %s not found", param[0])
+    logger.error(_("Key %s not found"), param[0])
     sys.exit(1)
 
 
 def upgrade(args):
     # elevate process to run in admin mode
     command = f"\"{sys.executable}\" -m pip install --upgrade formation-studio"
     if platform_is(WINDOWS):
```

### Comparing `formation-studio-0.6.3/studio/context.py` & `formation-studio-0.7.0/studio/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from hoverset.util.execution import Action
 from hoverset.ui.widgets import Frame
 from hoverset.ui.icons import get_icon_image as icon
 from hoverset.ui.menu import EnableIf
 
+from studio.i18n import _
+
 
 class BaseContext(Frame):
 
     def __init__(self, master, studio, *args, **kwargs):
         super(BaseContext, self).__init__(master)
         self.tab_view = master
         self.studio = studio
         self.pref = studio.pref
         self._undo_stack = []
         self._redo_stack = []
         self.tab_handle = None
         self.name = "tab"
-        self.icon = icon("data", 15, 15)
+        self.icon = icon("file", 15, 15)
         self.bind("<<TabDeleted>>", self._close_context)
         self.bind("<<TabToClose>>", self._close_check)
         self._force_close = False
 
     def _close_context(self, *_):
         self.studio.on_context_close(self)
         self.destroy()
@@ -40,22 +42,22 @@
 
     def on_context_unset(self):
         pass
 
     def on_context_mount(self):
         self.tab_handle.config_tab(text=self.name)
         self.tab_handle.set_up_context((
-            ("command", "close", icon("blank", 14, 14), self.close, {}),
+            ("command", _("close"), icon("blank", 18, 18), self.close, {}),
             EnableIf(
                 lambda: len(self.tab_view.tabs()) > 1,
-                ("command", "close other tabs", icon("blank", 14, 14), self.close_other, {})
+                ("command", _("close other tabs"), icon("blank", 18, 18), self.close_other, {})
             ),
             EnableIf(
                 lambda: self._contexts_right(),
-                ("command", "close tabs to the right", icon("blank", 14, 14), self.close_other_right, {})
+                ("command", _("close tabs to the right"), icon("blank", 18, 18), self.close_other_right, {})
             ),
             ("separator", ),
             *self.get_tab_menu()
         ))
 
     def _contexts_right(self):
         return [self.tab_view._tabs[i] for i in self.tab_view._tab_order[self.tab_view.index(self.tab_handle) + 1:]]
```

### Comparing `formation-studio-0.6.3/studio/debugtools/common.py` & `formation-studio-0.7.0/studio/debugtools/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import tkinter
 from tkinter import ttk
 from studio.lib import native, legacy
 from studio.lib.properties import get_properties
 
 
-def get_base_class(widget):
+def extract_base_class(widget):
     # we'll check the MRO
     # the first class is always itself
     classes = widget.__class__.mro()
     for c in classes:
         if c.__module__ in (ttk.__name__, tkinter.__name__):
             return c
     return None
 
 
+def get_base_class(widget):
+    return widget._class
+
+
 def get_studio_equiv(widget):
     base = get_base_class(widget)
     if base is None:
         return
 
     if base.__module__ == tkinter.__name__:
         # we'll look in legacy
```

### Comparing `formation-studio-0.6.3/studio/debugtools/element_pane.py` & `formation-studio-0.7.0/studio/debugtools/element_pane.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-import tkinter
-
 from hoverset.ui.widgets import Button, ToggleButton, Label
 from hoverset.ui.icons import get_icon_image
 
 from studio.ui.widgets import Pane
 from studio.ui.tree import MalleableTreeView
 from studio.feature.component_tree import ComponentTreeView
 from studio.debugtools import common
+from studio.debugtools.defs import RemoteWidget
+from studio.i18n import _
 
 
 class ElementTreeView(ComponentTreeView):
 
     class Node(MalleableTreeView.Node):
         # debugger widget to be ignored during loading
         # will be set at runtime
         debugger = None
 
         def __init__(self, master=None, **config):
             super().__init__(master, **config)
             self.widget = config.get("widget")
-            self.widget.bind('<Map>', self.on_map, add=True)
-            self.widget.bind('<Unmap>', self.on_unmap, add=True)
             setattr(self.widget, "_dbg_node", self)
             equiv = common.get_studio_equiv(self.widget)
             icon = equiv.icon if equiv else 'play'
             self.name_pad.configure(text=self.extract_name(self.widget))
             self.icon_pad.configure(image=get_icon_image(icon, 15, 15))
             self._loaded = False
             if not self.widget.winfo_ismapped():
@@ -37,48 +35,46 @@
             self.name_pad.configure(**self.style.text_passive)
 
         @property
         def loaded(self):
             return self._loaded
 
         def update_preload_status(self, added):
-            if self._loaded:
+            if self._loaded or self.widget.deleted:
                 return
             if added or self.widget.winfo_children():
                 # widget can expand
                 self._set_expander(self.COLLAPSED_ICON)
             else:
                 self._set_expander(self.BLANK)
 
         def extract_name(self, widget):
-            if isinstance(widget, tkinter.BaseWidget):
+            if isinstance(widget, RemoteWidget):
                 return str(widget._name).strip("!")
             return 'root'
 
         def load(self):
             # lazy loading
             # nodes will be loaded when parent node is expanded
-            if self._loaded:
+            if self._loaded or self.widget.deleted:
                 return
             for child in self.widget.winfo_children():
                 if getattr(child, "_dbg_ignore", False):
                     continue
                 self.add_as_node(widget=child).update_preload_status(False)
-                if not getattr(child, "_dbg_hooked", False):
-                    ElementTreeView.Node.debugger.hook_widget(child)
             self._loaded = True
 
         def expand(self):
             # load widgets first
             self.load()
             super().expand()
 
     def initialize_tree(self):
         super(ElementTreeView, self).initialize_tree()
-        self._show_empty("No items detected")
+        self._show_empty(_("No items detected"))
 
     def expand_to(self, widget):
         parent = widget.nametowidget(widget.winfo_parent())
         hierarchy = [parent]
         while parent not in (self.Node.debugger.root, self.Node.debugger):
             parent = parent.nametowidget(parent.winfo_parent())
             hierarchy.append(parent)
@@ -89,19 +85,21 @@
 
         assert hasattr(widget, "_dbg_node")
         return widget._dbg_node
 
 
 class ElementPane(Pane):
     name = "Widget tree"
+    display_name = _("Widget tree")
     MAX_STARTING_DEPTH = 4
 
     def __init__(self, master, debugger):
         super(ElementPane, self).__init__(master)
-        Label(self._header, **self.style.text_accent, text=self.name).pack(side="left")
+        self.debugger = debugger
+        Label(self._header, **self.style.text_accent, text=self.display_name).pack(side="left")
 
         ElementTreeView.Node.debugger = debugger
         self._tree = ElementTreeView(self)
         self._tree.pack(side="top", fill="both", expand=True, pady=4)
         self._tree.allow_multi_select(True)
         self._tree.on_select(self.on_select)
 
@@ -110,100 +108,72 @@
             image=get_icon_image("search", 15, 15), width=25, height=25,
         )
         self._search_btn.pack(side="right", padx=2)
         self._search_btn.on_click(self.start_search)
 
         self._reload_btn = Button(
             self._header, **self.style.button,
-            image=get_icon_image("rotate_clockwise", 15, 15), width=25, height=25,
+            image=get_icon_image("reload", 15, 15), width=25, height=25,
         )
         self._reload_btn.pack(side="right", padx=2)
-        self._reload_btn.tooltip("reload tree")
+        self._reload_btn.tooltip(_("reload tree"))
 
         self._toggle_btn = Button(
             self._header, image=get_icon_image("chevron_down", 15, 15),
             **self.style.button, width=25, height=25
         )
         self._toggle_btn.pack(side="right", padx=2)
 
         self._select_btn = ToggleButton(
             self._header, **self.style.button,
             image=get_icon_image("cursor", 15, 15), width=25, height=25,
         )
         self._select_btn.pack(side="right", padx=2)
-        self._select_btn.tooltip("select element to inspect")
+        self._select_btn.on_change(self.debugger.set_hover)
+        self._select_btn.tooltip(_("select element to inspect"))
 
-        self.debugger = debugger
         self._tree.add_as_node(widget=debugger.root).update_preload_status(False)
 
         self.debugger.bind("<<WidgetCreated>>", self.on_widget_created)
         self.debugger.bind("<<WidgetDeleted>>", self.on_widget_deleted)
         self.debugger.bind("<<WidgetModified>>", self.on_widget_modified)
 
-        tkinter.Misc.bind_all(self.debugger.root, "<Motion>", self.on_motion)
-        tkinter.Misc.bind_all(self.debugger.root, "<Button-1>", self.on_widget_tap)
-        tkinter.Misc.bind_all(self.debugger.root, "<Button-3>", self.on_widget_tap)
-        tkinter.Misc.bind_all(self.debugger.root, "<Map>", self.on_widget_map)
-        tkinter.Misc.bind_all(self.debugger.root, "<Unmap>", self.on_widget_unmap)
-        self.highlighted = None
-
     @property
     def selected(self):
         return self._tree.get()
 
     def on_select(self):
-        self.debugger.update_selection(self._tree.get())
+        self.debugger.selection.set(map(lambda node: node.widget, self._tree.get()))
 
-    def on_widget_tap(self, event):
-        if self._select_btn.get():
-            try:
-                # widget = self.debugger.root.winfo_containing(event.x_root, event.y_root)
-                widget = event.widget
-                # print(widget)
-                if widget.winfo_toplevel() == self.debugger or getattr(widget, "_dbg_ignore", False):
-                    widget = None
-            except (KeyError, AttributeError):
-                widget = None
-
-            if widget:
-                node = self._tree.expand_to(widget)
-                if node:
-                    node.select(event)
-
-    def on_motion(self, event):
-        if self._select_btn.get():
-            try:
-                # widget = self.debugger.root.winfo_containing(event.x_root, event.y_root)
-                widget = event.widget
-                if widget.winfo_toplevel() == self.debugger or getattr(widget, "_dbg_ignore", False):
-                    widget = None
-                # print(f"motion : {widget} <> {event.widget}")
-            except (KeyError, AttributeError):
-                widget = None
-            self.debugger.highlight_widget(widget)
-            self.highlighted = widget
+    def on_widget_tap(self, widget, event):
+        if widget:
+            node = self._tree.expand_to(widget)
+            if node:
+                self._tree.see(node)
+                node.select(event)
 
     def on_widget_created(self, _):
         widget = self.debugger.active_widget
         parent_node = getattr(widget.master, "_dbg_node", None)
         if parent_node:
             if parent_node.loaded:
                 parent_node.add_as_node(widget=widget)
-                self.debugger.hook_widget(widget)
             else:
                 parent_node.update_preload_status(True)
 
     def on_widget_deleted(self, _):
         widget = self.debugger.active_widget
         parent_node = getattr(widget.master, "_dbg_node", None)
         if parent_node:
             if parent_node.loaded:
                 node = widget._dbg_node
                 if node in self.selected:
                     self._tree.toggle_from_selection(node)
+                    if not self.selected:
+                        self._tree.see(self.debugger.root._dbg_node)
                 parent_node.remove(widget._dbg_node)
             else:
                 parent_node.update_preload_status(False)
 
     def on_widget_modified(self, _):
         if self.debugger.active_widget not in self.selected:
             return
```

### Comparing `formation-studio-0.6.3/studio/debugtools/layouts.py` & `formation-studio-0.7.0/studio/debugtools/layouts.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,28 @@
     return dict(filter(lambda x: x[0] not in ('width', 'height'), defs.items()))
 
 
 class BaseLayout:
     defs = {}
     name = ''
 
+    @staticmethod
+    def clean(value):
+        if isinstance(value, (list, tuple)):
+            return " ".join(map(str, value))
+        return value
+
     @classmethod
     def get_def(cls, widget):
         info = cls.configure(widget)
         # Ensure we use the dynamic definitions
         definition = dict(cls.defs)
         for key in definition:
             # will throw a key error if a definition value is not found in info
-            definition[key]["value"] = info[key]
+            definition[key]["value"] = cls.clean(info[key])
         return definition
 
     @classmethod
     def configure(cls, widget, **kw):
         if not kw:
             return {}
 
@@ -69,23 +75,23 @@
 class TabLayout(BaseLayout):
     defs = _filtered_def(layouts.TabLayoutStrategy.DEFINITION)
     name = 'Notebook'
 
     @classmethod
     def configure(cls, widget, **kw):
         parent = widget.master
-        if isinstance(parent, ttk.Notebook):
+        if issubclass(parent._class, ttk.Notebook):
             if not kw:
                 return parent.tab(widget) or {}
             parent.tab(widget, **kw)
 
     @classmethod
     def verify(cls, widget):
         parent = widget.master
-        return isinstance(parent, ttk.Notebook)
+        return issubclass(parent._class, ttk.Notebook)
 
 
 class PanedLayout(BaseLayout):
     defs = _filtered_def(layouts.PanedLayoutStrategy.DEFINITION)
     name = 'Pane'
 
     @classmethod
@@ -96,15 +102,15 @@
                 info = parent.paneconfig(widget) or {}
                 return {k: info[k][-1] for k in info}
             parent.paneconfig(widget, **kw)
 
     @classmethod
     def verify(cls, widget):
         parent = widget.master
-        return isinstance(parent, tkinter.PanedWindow) and not isinstance(parent, ttk.PanedWindow)
+        return issubclass(parent._class, tkinter.PanedWindow) and not issubclass(parent._class, ttk.PanedWindow)
 
 
 class NPanedLayout(BaseLayout):
     defs = _filtered_def(layouts.NPanedLayoutStrategy.DEFINITION)
     name = 'Pane'
 
     @classmethod
@@ -114,15 +120,15 @@
             if not kw:
                 return parent.pane(widget) or {}
             parent.pane(widget, **kw)
 
     @classmethod
     def verify(cls, widget):
         parent = widget.master
-        return isinstance(parent, ttk.PanedWindow)
+        return issubclass(parent._class, ttk.PanedWindow)
 
 
 _layout_map = {
     'pack': PackLayout,
     'grid': GridLayout,
     'place': PlaceLayout,
     'notebook': TabLayout,
@@ -134,17 +140,17 @@
 
 
 def get_layout(widget) -> BaseLayout:
     if not widget or not widget.winfo_ismapped():
         return None
     manager = widget.winfo_manager()
     if manager == 'panedwindow':
-        if isinstance(widget.master, ttk.PanedWindow):
+        if issubclass(widget.master._class, ttk.PanedWindow):
             return NPanedLayout
-        elif isinstance(widget.master, tkinter.PanedWindow):
+        elif issubclass(widget.master._class, tkinter.PanedWindow):
             return PanedLayout
         else:
             return None
     else:
         layout = _layout_map.get(manager, None)
 
     if layout and layout.verify(widget):
```

### Comparing `formation-studio-0.6.3/studio/feature/_base.py` & `formation-studio-0.7.0/studio/feature/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 from hoverset.ui.icons import get_icon_image
 from hoverset.ui.widgets import Label, Button, MenuButton, PanedWindow
 from hoverset.ui.menu import EnableIf
 from studio.ui.geometry import absolute_position, parse_geometry
 from studio.ui.widgets import Pane
 from studio.preferences import Preferences
+from studio.i18n import _
 
 
 class BaseFeature(Pane):
     _instance = None
     name = "Feature"
+    display_name = "Feature"
     pane = None
     bar = None
     icon = "blank"
     _view_mode = None
     _transparency_flag = None
     _side = None
     rec = (20, 20, 300, 300)  # Default window mode position
@@ -55,41 +57,41 @@
         if not self.__class__._view_mode:
             self.__class__._view_mode = StringVar(None, self.get_pref('mode'))
             self.__class__._transparency_flag = t = BooleanVar(None, self.get_pref('inactive_transparency'))
             self.__class__._side = StringVar(None, self.get_pref('side'))
             self.is_visible = BooleanVar(None, self.get_pref('visible'))
             t.trace_add("write", lambda *_: self.set_pref('inactive_transparency', t.get()))
         self.studio = studio
-        Label(self._header, **self.style.text_accent, text=self.name).pack(side="left")
+        Label(self._header, **self.style.text_accent, text=self.display_name).pack(side="left")
         self._min = Button(self._header, image=get_icon_image("close", 15, 15), **self.style.button, width=25,
                            height=25)
         self._min.pack(side="right")
         self._min.on_click(self.minimize)
         self._pref = MenuButton(self._header, **self.style.button)
         self._pref.configure(image=get_icon_image("settings", 15, 15))
         self._pref.pack(side="right")
         self._pref.tooltip("Options")
         menu = self.make_menu((
-            ("cascade", "View Mode", None, None, {"menu": (
-                ("radiobutton", "Docked", None, self.open_as_docked, {"variable": self._view_mode, "value": "docked"}),
-                ("radiobutton", "Window", None, self.open_as_window, {"variable": self._view_mode, "value": "window"}),
+            ("cascade", _("View Mode"), None, None, {"menu": (
+                ("radiobutton", _("Docked"), None, self.open_as_docked, {"variable": self._view_mode, "value": "docked"}),
+                ("radiobutton", _("Window"), None, self.open_as_window, {"variable": self._view_mode, "value": "window"}),
             )}),
-            ("cascade", "Position", None, None, {"menu": (
-                ("radiobutton", "Left", None, lambda: self.reposition("left"),
+            ("cascade", _("Position"), None, None, {"menu": (
+                ("radiobutton", _("Left"), None, lambda: self.reposition("left"),
                  {"variable": self._side, "value": "left"}),
-                ("radiobutton", "Right", None, lambda: self.reposition("right"),
+                ("radiobutton", _("Right"), None, lambda: self.reposition("right"),
                  {"variable": self._side, "value": "right"}),
             )}),
             EnableIf(lambda: self._view_mode.get() == 'window',
-                     ("cascade", "Window options", None, None, {"menu": (
+                     ("cascade", _("Window options"), None, None, {"menu": (
                          (
-                             "checkbutton", "Transparent when inactive", None, None,
+                             "checkbutton", _("Transparent when inactive"), None, None,
                              {"variable": self._transparency_flag}),
                      )})),
-            ("command", "Close", get_icon_image("close", 14, 14), self.minimize, {}),
+            ("command", _("Close"), get_icon_image("close", 18, 18), self.minimize, {}),
             ("separator",),
             *self.create_menu()
         ), self._pref)
         self._pref.config(menu=menu)
         # self._pref.on_click(self.minimize)
         self.config(**self.style.surface)
         self.indicator = None
@@ -114,63 +116,61 @@
     def set_pref(cls, short_path, value):
         Preferences.acquire().set(cls.get_pref_path(short_path), value)
 
     @classmethod
     def get_instance(cls):
         return cls._instance
 
-    def on_select(self, widget):
+    def on_widgets_change(self, widgets):
         """
-        Called when a widget is selected in the designer
-        :param widget: selected widget
-        :return:None
+        Called when the widgets in the designer are changed
+        :param widgets: list of widgets
+        :return: None
         """
         pass
 
-    def on_widget_change(self, old_widget, new_widget=None):
+    def on_widgets_layout_change(self, widgets):
         """
-        Called when a widget is fundamentally altered
-        :param old_widget: Altered widget
-        :param new_widget: The new widget taking the older widgets place
+        Called when layout options of a widgets are changed
+        :param widgets: Widgets with altered layout options
         :return: None
         """
         pass
 
-    def on_widget_layout_change(self, widget):
+    def on_widgets_reorder(self, indices):
         """
-        Called when layout options of a widget are changed
-        :param widget: Widget with altered layout options
-        :return: None
+        Called when the widgets in the designer are reordered within their parent.
+        Used to change stacking order of widgets
         """
         pass
 
     def on_widget_add(self, widget, parent):
         """
         Called when a new widget is added to the designer
         :param widget: widget
         :param parent: the container widget to which thw widget is added
         :return: None
         """
         pass
 
-    def on_widget_delete(self, widget, silently=False):
+    def on_widgets_delete(self, widgets, silently=False):
         """
-        Called when a widget is deleted from the designer
-        :param widget: deleted widget
+        Called when widgets are deleted from the designer
+        :param widgets: deleted widgets
         :param silently: flag indicating whether the deletion should be treated implicitly
         which is useful for instance when you don't want the deletion to be logged in the
         undo stack
         :return: None
         """
         pass
 
-    def on_widget_restore(self, widget):
+    def on_widgets_restore(self, widgets):
         """
         Called when a deleted widget is restored
-        :param widget: restored widget
+        :param widgets: widgets to be restored
         :return: None
         """
         pass
 
     def on_session_clear(self):
         """
         Override to perform operations before a session is cleared and the studio
```

### Comparing `formation-studio-0.6.3/studio/feature/component_tree.py` & `formation-studio-0.7.0/studio/feature/component_tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from hoverset.ui.icons import get_icon_image
 from hoverset.ui.widgets import Button, Label, Frame
 from hoverset.ui.menu import MenuUtils
 from studio.feature._base import BaseFeature
 from studio.lib.pseudo import PseudoWidget
 from studio.ui.tree import MalleableTreeView
+from studio.i18n import _
 
 
 class ComponentTreeView(MalleableTreeView):
 
     class Node(MalleableTreeView.Node):
 
         def __init__(self, master=None, **config):
@@ -23,45 +24,46 @@
             self.icon_pad.configure(image=get_icon_image(self.widget.icon, 15, 15))
 
     def initialize_tree(self):
         super(ComponentTreeView, self).initialize_tree()
         self._empty = Frame(self, **self.style.surface)
         self._empty_text = Label(self._empty, **self.style.text_passive)
         self._empty_text.pack(fill="both", expand=True, pady=30)
-        self._show_empty("No items created yet")
+        self._show_empty(_("No items created yet"))
 
     def add(self, node):
         super().add(node)
         self._remove_empty()
 
     def insert(self, index=None, *nodes):
         super(ComponentTreeView, self).insert(index, *nodes)
         self._remove_empty()
 
     def remove(self, node):
         super().remove(node)
         if len(self.nodes) == 0:
-            self._show_empty("No items created yet")
+            self._show_empty(_("No items created yet"))
 
     def _show_empty(self, text):
         self._empty_text["text"] = text
         self._empty.place(x=0, y=0, relheight=1, relwidth=1)
 
     def _remove_empty(self):
         self._empty.place_forget()
 
     def search(self, query):
         if not super().search(query):
-            self._show_empty("No items match your search")
+            self._show_empty(_("No items match your search"))
         else:
             self._remove_empty()
 
 
 class ComponentTree(BaseFeature):
     name = "Component Tree"
+    display_name = _("Component Tree")
     icon = "treeview"
 
     def __init__(self, master, studio=None,  **cnf):
         super().__init__(master, studio, **cnf)
         self._toggle_btn = Button(self._header, image=get_icon_image("chevron_down", 15, 15), **self.style.button,
                                   width=25,
                                   height=25)
@@ -73,39 +75,40 @@
             image=get_icon_image("search", 15, 15), width=25, height=25,
         )
         self._search_btn.pack(side="right")
         self._search_btn.on_click(self.start_search)
         self.body = Frame(self, **self.style.surface)
         self.body.pack(side="top", fill="both", expand=True)
         self._empty_label = Label(self.body, **self.style.text_passive)
+        self.studio.bind("<<SelectionChanged>>", self._select, "+")
 
-        self._selected = None
         self._expanded = False
         self._tree = None
 
     def on_context_switch(self):
         if self._tree:
             self._tree.pack_forget()
 
         if self.studio.designer:
             self.show_empty(None)
             if self.studio.designer.node:
                 self._tree = self.studio.designer.node
             else:
                 self._tree = ComponentTreeView(self.body)
+                self._tree.allow_multi_select(True)
                 self._tree.on_select(self._trigger_select)
                 self.studio.designer.node = self._tree
             self._tree.pack(fill="both", expand=True)
         else:
-            self.show_empty("No active Designer")
+            self.show_empty(_("No active Designer"))
 
     def create_menu(self):
         return (
-            ("command", "Expand all", get_icon_image("chevron_down", 14, 14), self._expand, {}),
-            ("command", "Collapse all", get_icon_image("chevron_up", 14, 14), self._collapse, {})
+            ("command", _("Expand all"), get_icon_image("chevron_down", 18, 18), self._expand, {}),
+            ("command", _("Collapse all"), get_icon_image("chevron_up", 18, 18), self._collapse, {})
         )
 
     def show_empty(self, text):
         if text:
             self._empty_label.lift()
             self._empty_label.place(x=0, y=0, relwidth=1, relheight=1)
             self._empty_label['text'] = text
@@ -138,59 +141,74 @@
         # let the designer render the menu for us
         MenuUtils.bind_all_context(
             node,
             lambda e: self.studio.designer.show_menu(e, widget) if self.studio.designer else None
         )
 
     def _trigger_select(self):
-        if self._selected and self._selected.widget == self._tree.get().widget:
+        if self.studio.selection == self.selection():
             return
-        self.studio.select(self._tree.get().widget, self)
-        self._selected = self._tree.get()
 
-    def select(self, widget):
-        if widget:
+        self.studio.selection.set(self.selection())
+
+    def _select(self, _):
+        if self.studio.selection == self.selection():
+            return
+
+        if not self._tree:
+            return
+        nodes = self.studio_selection()
+
+        for node in list(self._tree.get()):
+            if node not in nodes:
+                self._tree.deselect(node)
+
+        for node in nodes:
+            if not node.selected:
+                self._tree.see(node)
+                node.select(silently=True)
+
+    def selection(self):
+        if not self._tree:
+            return []
+        return [i.widget for i in self._tree.get()]
+
+    def studio_selection(self):
+        return [i.node for i in self.studio.selection]
+
+    def on_widgets_delete(self, widgets, silently=False):
+        for widget in widgets:
+            widget.node.remove()
+
+    def on_widgets_restore(self, widgets):
+        for widget in widgets:
+            widget.layout.node.add(widget.node)
+
+    def on_widgets_layout_change(self, widgets):
+        for widget in widgets:
             node = widget.node
-            self._selected = node
-            node.select(None, True)  # Select node silently to avoid triggering a duplicate selection event
-        elif widget is None:
-            if self._selected:
-                self._selected.deselect()
-                self._selected = None
-
-    def on_select(self, widget):
-        self.select(widget)
-
-    def on_widget_delete(self, widget, silently=False):
-        widget.node.remove()
-
-    def on_widget_restore(self, widget):
-        widget.layout.node.add(widget.node)
-
-    def on_widget_layout_change(self, widget):
-        node = widget.node
-        if widget.layout == self.studio.designer:
-            parent = self._tree
-        else:
-            parent = widget.layout.node
-        if node.parent_node != parent:
-            parent.insert(None, node)
+            if widget.layout == self.studio.designer:
+                parent = self._tree
+            else:
+                parent = widget.layout.node
+            if node.parent_node != parent:
+                parent.insert(None, node)
 
     def on_context_close(self, context):
         if hasattr(context, "designer"):
             # delete context's tree
             if hasattr(context.designer, "node") and context.designer.node:
                 context.designer.node.destroy()
 
     def on_session_clear(self):
         self._tree.clear()
 
-    def on_widget_change(self, old_widget, new_widget=None):
-        new_widget = new_widget if new_widget else old_widget
-        new_widget.node.widget_modified(new_widget)
+    def on_widgets_change(self, widgets):
+        for widget in widgets:
+            widget.node.widget_modified(widget)
 
     def on_search_query(self, query: str):
         self._tree.search(query)
 
     def on_search_clear(self):
         self._tree.search("")
         super(ComponentTree, self).on_search_clear()
```

### Comparing `formation-studio-0.6.3/studio/feature/components.py` & `formation-studio-0.7.0/studio/feature/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from hoverset.ui.dialogs import MessageDialog
 from hoverset.data.preferences import ListControl
 from hoverset.util.execution import import_path
 from studio.preferences import Preferences, templates
 from studio.feature._base import BaseFeature
 from studio.lib import legacy, native
 from studio.lib.pseudo import PseudoWidget, Container, WidgetMeta
+from studio.ui import geometry
+from studio.i18n import _
 
 
 class Component(Frame):
 
     def __init__(self, master, component: PseudoWidget.__class__, _=None):
         super().__init__(master)
         self.config(**self.style.surface)
@@ -21,26 +23,32 @@
         self._icon.pack(side="left")
         self._text = Label(self, **self.style.text, anchor="w", text=component.display_name)
         self._text.pack(side="left", fill="x")
         self.bind("<Enter>", self.select)
         self.bind("<Leave>", self.deselect)
         self.component = component
         self.allow_drag = True
+        self.designer = None
 
     def select(self, *_):
         self.config_all(**self.style.hover)
 
     def deselect(self, *_):
         self.config_all(**self.style.surface)
 
     def render_drag(self, window):
+        dim = getattr(self.component, "initial_dimensions", None)
+        if dim:
+            window.geometry(f"{dim[0]}x{dim[1]}")
         Label(window, **self.style.text_accent, image=get_icon_image(self.component.icon, 15, 15)).pack(side="left")
         Label(window, **self.style.text, anchor="w", text=self.component.display_name).pack(side="left", fill="x")
 
     def drag_start_pos(self, event):
+        self.designer = ComponentPane.get_instance().studio.designer
+        self.designer._refresh_container_sort()
         window = self.window.drag_window
         if window:
             window.update_idletasks()
             return (
                 event.x_root - int(window.winfo_width() / 2),
                 event.y_root - int(window.winfo_height() / 2)
             )
@@ -50,24 +58,29 @@
         # adjust event position so it appears out the drag window
         # this allows us to determine studio widget at said position
         if self.window.drag_window:
             event.x_root = self.window.drag_window.get_center()[0]
             event.y_root = self.window.drag_window.pos[1] - 1
 
     def on_drag(self, event):
-        self._adjust_event(event)
-        widget = self.event_first(event, self, Container)
+        if not self.designer:
+            return
+        widget = self.designer.layout_at_pos(*self.window.drag_window.get_center())
         if widget and self.window.drag_window:
-            widget.react(*self.window.drag_window.get_center())
+            bounds = geometry.absolute_bounds(self.window.drag_window)
+            widget.react(bounds)
 
     def on_drag_end(self, event):
-        self._adjust_event(event)
-        widget = self.event_first(event, self, Container)
+        if not self.designer:
+            return
+        widget = self.designer.layout_at_pos(*self.window.drag_window.get_center())
         if isinstance(widget, Container):
-            widget.add_new(self.component, *self.window.drag_window.get_center())
+            bounds = geometry.absolute_bounds(self.window.drag_window)
+            widget.add_new(self.component, *bounds[:2])
+            widget.clear_highlight()
 
 
 class SelectableComponent(Component):
 
     def __init__(self, master, component: PseudoWidget.__class__, controller):
         super(SelectableComponent, self).__init__(master, component)
         self.selected = False
@@ -97,16 +110,17 @@
         self.selected = False
         self.controller.deselect(self, silently)
 
 
 class Selector(Label):
 
     def __init__(self, master, **cnf):
+        name = cnf.pop("name", None)
         super().__init__(master, **cnf)
-        self.name = cnf.get("text")
+        self.name = name
         self.group = None
         self.config(**self.style.text, anchor="w")
 
     def select(self):
         self.config(**self.style.hover)
 
     def deselect(self):
@@ -173,23 +187,23 @@
 
 
 class CustomPathControl(ListControl):
 
     def __init__(self, master, pref_, path, desc, **extra):
         super(CustomPathControl, self).__init__(master, pref_, path, desc, **extra)
         clear_btn = self.create_action(
-            get_icon_image("close", 17, 17), self._clear_all, "Clear all"
+            get_icon_image("close", 17, 17), self._clear_all, _("Clear all")
         )
         clear_btn.pack(side="right", fill="y", padx=5)
         clear_btn.configure(**self.style.highlight_active)
         self._list.set_mode(self._list.MULTI_MODE)
 
-    def on_add(self, _=None):
+    def on_add(self, __=None):
         paths = filedialog.askopenfilenames(
-            parent=self.window, title="Pick custom widget search paths",
+            parent=self.window, title=_("Pick custom widget search paths"),
             filetypes=[("python", ".py .pyw .pyi")],
         )
         cur_paths = [i.value for i in self._list.items]
         # remove duplicates if any
         cur_paths.extend(list(filter(lambda e: e not in cur_paths, paths)))
         self._list.set_values(cur_paths)
         super(CustomPathControl, self).on_add(_)
@@ -198,46 +212,21 @@
         self._list.set_values([])
         self._change()
 
     def has_changes(self):
         return super(CustomPathControl, self).has_changes()
 
 
-_widget_pref_template = {
-    "Widgets": {
-        "_scroll": False,
-        "Custom Widgets": {
-            "layout": {
-                "fill": "both",
-                "expand": True,
-            },
-            "children": (
-                {
-                    "desc": "Custom widgets search paths",
-                    "path": "studio::custom_widget_paths",
-                    "element": CustomPathControl,
-                    "layout": {
-                        "fill": "both",
-                        "expand": True,
-                        "padx": 5,
-                        "pady": 5
-                    }
-                },
-            )
-        }
-    },
-}
-
-
 class ComponentPane(BaseFeature):
     CLASSES = {
         "native": {"widgets": native.widgets},
         "legacy": {"widgets": legacy.widgets},
     }
     name = "Components"
+    display_name = _("Components")
     _var_init = False
     _defaults = {
         **BaseFeature._defaults,
         "widget_set": "native"
     }
     _custom_pref_path = "studio::custom_widget_paths"
 
@@ -270,23 +259,49 @@
         self._widget_pane.place(relx=0.4, y=0, relwidth=0.6, relheight=1)
 
         self._pool = {}
         self._selectors = []
         self._selected = None
         self._component_cache = None
         self._extern_groups = []
-        self._widget = None
         self.collect_groups(self.get_pref("widget_set"))
         # add custom widgets config to settings
-        templates.update(_widget_pref_template)
+        templates.update(self._pref_template())
         self._custom_group = None
         self._custom_widgets = []
+        self.studio.bind("<<SelectionChanged>>", self.on_widget_select, add='+')
         Preferences.acquire().add_listener(self._custom_pref_path, self._init_custom)
         self._reload_custom()
 
+    def _pref_template(self):
+        return {
+            _("Widgets"): {
+                "_scroll": False,
+                _("Custom Widgets"): {
+                    "layout": {
+                        "fill": "both",
+                        "expand": True,
+                    },
+                    "children": (
+                        {
+                            "desc": _("Custom widgets search paths"),
+                            "path": "studio::custom_widget_paths",
+                            "element": CustomPathControl,
+                            "layout": {
+                                "fill": "both",
+                                "expand": True,
+                                "padx": 5,
+                                "pady": 5
+                            }
+                        },
+                    )
+                }
+            },
+        }
+
     @property
     def custom_widgets(self):
         return self._custom_widgets
 
     def auto_find_load_custom(self, *modules):
         # locate and load all custom widgets in modules
         # module can be a module or a path to module file
@@ -304,15 +319,15 @@
                     self._custom_widgets.append(getattr(module, attr))
         if errors:
             error_msg = "\n\n".join(
                 [f"{path}\n{error}" for path, error in errors.items()]
             )
             MessageDialog.show_error(
                 parent=self.window,
-                message=f"Error loading widgets \n\n{error_msg}"
+                message=_("Error loading widgets \n\n{}").format(error_msg)
             )
 
         return self._custom_widgets
 
     def _init_custom(self, paths):
         # reload custom widget modules
         try:
@@ -359,36 +374,36 @@
     @property
     def selectors(self):
         return self._selectors
 
     def create_menu(self):
         return (
             (
-                "command", "Reload custom widgets",
-                get_icon_image("rotate_clockwise", 14, 14), self._reload_custom, {}
+                "command", _("Reload custom widgets"),
+                get_icon_image("reload", 18, 18), self._reload_custom, {}
             ),
             (
-                "command", "Search",
-                get_icon_image("search", 14, 14), self.start_search, {}
+                "command", _("Search"),
+                get_icon_image("search", 18, 18), self.start_search, {}
             ),
-            ("cascade", "Widget set", get_icon_image("blank", 14, 14), None, {"menu": (
+            ("cascade", _("Widget set"), get_icon_image("blank", 18, 18), None, {"menu": (
                 *self._widget_sets_as_menu(),
             )}),
         )
 
     def collect_groups(self, widget_set):
         for other_set in [i for i in self.CLASSES if i != widget_set]:
             self.CLASSES[other_set]["var"].set(False)
         self.CLASSES[widget_set]["var"].set(True)
         self._widget_set.set(widget_set)
         self._select_pane.clear_children()
         self._pool = {}
         components = self.CLASSES.get(widget_set)["widgets"]
         for component in components:
-            group = component.group.name
+            group = component.group
             if group in self._pool:
                 self._pool[group].append(Component(self._widget_pane.body, component))
             else:
                 self._pool[group] = [Component(self._widget_pane.body, component)]
         self.render_groups()
         # component pool has changed so invalidate the cache
         self._component_cache = None
@@ -428,21 +443,21 @@
         else:
             self._widget_pane.clear_children()
             self._selected = None
 
     def render_groups(self):
         self._selectors = []
         for group in self._pool:
-            self.add_selector(Selector(self._select_pane.body, text=group))
+            self.add_selector(Selector(self._select_pane.body, text=group.value, name=group))
         self._auto_select()
         self.render_extern_groups()
 
     def render_extern_groups(self):
         for group in self._extern_groups:
-            if group.supports(self._widget):
+            if self.studio.selection and all(group.supports(w) for w in self.studio.selection):
                 self.add_selector(group.selector)
             else:
                 self.remove_selector(group.selector)
                 if self._selected == group.selector:
                     self._auto_select()
 
     def add_selector(self, selector):
@@ -476,16 +491,15 @@
 
     def unregister_group(self, group):
         if group in self._extern_groups:
             self.remove_selector(group.selector)
             self._extern_groups.remove(group)
             self._auto_select()
 
-    def on_select(self, widget):
-        self._widget = widget
+    def on_widget_select(self, _):
         self.render_extern_groups()
 
     def start_search(self, *_):
         super().start_search()
         self._widget_pane.scroll_to_start()
         if self._selected is not None:
             self._selected.deselect()
```

### Comparing `formation-studio-0.6.3/studio/feature/design.py` & `formation-studio-0.7.0/studio/feature/design.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,89 +3,103 @@
 """
 
 # ======================================================================= #
 # Copyright (C) 2019 Hoverset Group.                                      #
 # ======================================================================= #
 import os.path
 import time
-from tkinter import filedialog, ttk
+from tkinter import filedialog, ttk, TclError
 
 from hoverset.data import actions
 from hoverset.data.keymap import KeyMap
 from hoverset.data.images import get_tk_image
-from hoverset.ui.widgets import Label, Text, FontStyle, Checkbutton, CompoundList
+from hoverset.ui.widgets import Label, Text, FontStyle, Checkbutton, CompoundList, EventMask
 from hoverset.ui.dialogs import MessageDialog
 from hoverset.ui.icons import get_icon_image as icon
 from hoverset.ui.menu import MenuUtils, LoadLater, EnableIf
 from hoverset.util.execution import Action, as_thread
 
 from studio.lib import NameGenerator
-from studio.lib.layouts import PlaceLayoutStrategy
+from studio.lib.layouts import BaseLayoutStrategy, PlaceLayoutStrategy
 from studio.lib.pseudo import PseudoWidget, Container, Groups
 from studio.parsers.loader import DesignBuilder, BaseStudioAdapter
 from studio.ui import geometry
-from studio.ui.highlight import HighLight
 from studio.ui.widgets import DesignPad, CoordinateIndicator
+from studio.ui.highlight import RegionHighlighter
 from studio.context import BaseContext
+from studio.i18n import _
 from studio import __version__
 
 from formation.formats import get_file_types
 
 
 class DesignLayoutStrategy(PlaceLayoutStrategy):
     name = "DesignLayout"
+    DEFINITION = {
+        **BaseLayoutStrategy.DEFINITION,
+        "x": {
+            "display_name": "x",
+            "type": "dimension",
+            "name": "x",
+            "default": None
+        },
+        "y": {
+            "display_name": "y",
+            "type": "dimension",
+            "name": "y",
+            "default": None
+        }
+    }
 
     def add_new(self, widget, x, y):
         self.container.add(widget, x, y, layout=self.container)
 
-    def _move(self, widget, bounds):
-        self.container.position(widget, self.container.canvas_bounds(bounds))
+    def resize_widget(self, widget, direction, delta):
+        info = self._info_with_delta(widget, direction, delta)
+        self.container.place_child(widget, **info)
+
+    def move_widget(self, widget, delta):
+        self.container.position(widget, self.container.canvas_bounds(self.bounds_from_delta(widget, delta)))
 
     def add_widget(self, widget, bounds=None, **kwargs):
-        super(PlaceLayoutStrategy, self).add_widget(widget, bounds=None, **kwargs)
+        super(PlaceLayoutStrategy, self).add_widget(widget, bounds=bounds, **kwargs)
         super(PlaceLayoutStrategy, self).remove_widget(widget)
-        if bounds is None:
+        if bounds:
+            bounds = geometry.relative_bounds(bounds, self.container.body)
+            self.container.position(widget, bounds)
+        else:
             x = kwargs.get("x", 10)
             y = kwargs.get("y", 10)
             width = kwargs.get("width", 20)
             height = kwargs.get("height", 20)
             self.container.place_child(widget, x=x, y=y, width=width, height=height)
-        else:
-            x1, y1, x2, y2 = self.container.canvas_bounds(bounds)
-            self.container.place_child(widget, x=x1, y=y1, width=x2 - x1, height=y2 - y1)
-        self.children.append(widget)
+        self._insert(widget, widget.prev_stack_index if widget.layout == self.container else None)
 
     def remove_widget(self, widget):
         super().remove_widget(widget)
         self.container.forget_child(widget)
 
     def apply(self, prop, value, widget):
         if value == '':
             return
         self.container.config_child(widget, **{prop: value})
 
     def restore_widget(self, widget, data=None):
         data = widget.recent_layout_info if data is None else data
-        self.children.append(widget)
+        self._insert(widget, widget.prev_stack_index if widget.layout == self.container else None)
         widget.layout = self.container
         widget.level = self.level + 1
         self.container.place_child(widget, **data.get("info", {}))
 
     def get_restore(self, widget):
         return {
             "info": self.container.config_child(widget),
             "container": self,
         }
 
-    def get_def(self, widget):
-        definition = dict(self.DEFINITION)
-        # We don't need bordermode
-        definition.pop("bordermode")
-        return definition
-
     def info(self, widget):
         bounds = self.container.bbox(widget)
         width, height = geometry.dimensions(bounds)
         return {
             "x": bounds[0],
             "y": bounds[1],
             "width": width,
@@ -95,103 +109,127 @@
 
 class Designer(DesignPad, Container):
     MOVE = 0x2
     RESIZE = 0x3
     WIDGET_INIT_PADDING = 20
     WIDGET_INIT_HEIGHT = 25
     name = "Designer"
+    display_name = _("Designer")
     pane = None
     _coord_indicator = None
 
     def __init__(self, master, studio):
         super().__init__(master)
         self.id = None
+        self._level = -1
         self.context = master
         self.studio = studio
         self.name_generator = NameGenerator(self.studio.pref)
         self.setup_widget()
+        self.designer = self
         self.parent = self
         self.config(**self.style.bright, takefocus=True)
         self.objects = []
         self.root_obj = None
         self.layout_strategy = DesignLayoutStrategy(self)
-        self.highlight = HighLight(self)
-        self.highlight.on_resize(self._on_size_changed)
-        self.highlight.on_move(self._on_move)
-        self.highlight.on_release(self._on_release)
-        self.highlight.on_start(self._on_start)
-        self._update_throttling()
-        self.studio.pref.add_listener(
-            "designer::frame_skip",
-            self._update_throttling
-        )
         self.current_obj = None
         self.current_container = None
         self.current_action = None
         self._displace_active = False
         self._last_displace = time.time()
         self._frame.bind("<Button-1>", lambda _: self.focus_set(), '+')
         self._frame.bind("<Button-1>", self.set_pos, '+')
         self._frame.bind('<Motion>', self.on_motion, '+')
-        self._frame.bind('<KeyRelease>', self._stop_displace, '+')
         self._padding = 30
         self.design_path = None
         self.builder = DesignBuilder(self)
         self._shortcut_mgr = KeyMap(self._frame)
         self._set_shortcuts()
         self._last_click_pos = None
+        self._region_highlight = RegionHighlighter(self, self.style)
 
         self._empty = Label(
             self,
-            image=get_tk_image("paint", 30, 30), compound="top", text=" ",
+            image=get_tk_image("design", 30, 30), compound="top", text=" ",
             **self.style.text_passive
         )
         self._empty.config(**self.style.bright)
         self._show_empty(True)
 
         # create the dynamic menu
         self._context_menu = MenuUtils.make_dynamic(
             self.studio.menu_template +
             (LoadLater(self.studio.tool_manager.get_tool_menu), ) +
-            (LoadLater(lambda: self.current_obj.create_menu() if self.current_obj else ()),),
+            # Allow widget specific menu only when a single widget is selected
+            (LoadLater(lambda: self.studio.selection[0].create_menu() if self.studio.selection.is_single() else ()),),
             self.studio,
             self.style
         )
         design_menu = (
             EnableIf(
                 lambda: self.studio._clipboard is not None,
-                ("command", "paste", icon("clipboard", 14, 14),
+                ("command", _("paste"), icon("clipboard", 18, 18),
                  lambda: self.paste(self.studio._clipboard, paste_to=self), {})
             ),)
         self.set_up_context(design_menu)
         self._empty.set_up_context(design_menu)
         if Designer._coord_indicator is None:
             Designer._coord_indicator = self.studio.install_status_widget(CoordinateIndicator)
         self._text_editor = Text(self, wrap='none')
         self._text_editor.on_change(self._text_change)
         self._text_editor.bind("<FocusOut>", self._text_hide)
         self._base_font = FontStyle()
+        self._selected = set()
+        self._studio_bindings = []
+        self._move_selection = []
+        self._all_bound = None
+
+        # These variables help in skipping of several rendering frames to reduce lag when dragging items
+        self._skip_var = 0
+        # The maximum rendering to skip (currently 80%) for every one successful render. Ensure its
+        # not too big otherwise we won't be moving and resizing items at all and not too small otherwise the lag would
+        # be unbearable
+        self._skip_max = 4
+        self._surge_delta = (0, 0)
+        self._update_throttling()
+        self.studio.pref.add_listener(
+            "designer::frame_skip",
+            self._update_throttling
+        )
+        self._sorted_containers = []
+        self._realtime_layout_update = False
+        self._handle_active_data = None
+        # used to maintain id correlation for widget pasting
+        # do not touch
+        self._xlink_map = {}
+
+    def clear_studio_bindings(self):
+        for binding in self._studio_bindings:
+            self.studio.unbind(binding)
+
+    def add_studio_binding(self, *args):
+        self._studio_bindings.append(self.studio.bind(*args))
 
     def _get_designer(self):
         return self
 
     def focus_set(self):
         self._frame.focus_force()
 
     def set_pos(self, event):
         # store the click position for effective widget pasting
         self._last_click_pos = event.x_root, event.y_root
 
     def _update_throttling(self, *_):
-        self.highlight.set_skip_max(self.studio.pref.get("designer::frame_skip"))
+        self._skip_max = self.studio.pref.get("designer::frame_skip")
 
     def _show_empty(self, flag, **kw):
         if flag:
-            kw['image'] = kw.get('image', get_tk_image('paint', 30, 30))
-            kw['text'] = kw.get('text', "Drag or paste a container here to start")
+            kw['image'] = kw.get('image', get_tk_image('design', 30, 30))
+            kw['text'] = kw.get('text', _("Drag or paste a container here to start"))
             self._empty.configure(**kw, wraplength=max(400, self.width))
             self._empty.place(relwidth=1, relheight=1)
         else:
             self._empty.place_forget()
 
     def _set_shortcuts(self):
         shortcut_mgr = self._shortcut_mgr
@@ -199,21 +237,14 @@
         shortcut_mgr.add_routines(
             actions.get('STUDIO_COPY'),
             actions.get('STUDIO_CUT'),
             actions.get('STUDIO_DELETE'),
             actions.get('STUDIO_PASTE'),
             actions.get('STUDIO_DUPLICATE'),
         )
-        # allow control of widget position using arrow keys
-        shortcut_mgr.add_shortcut(
-            (lambda: self.displace('right'), KeyMap.RIGHT),
-            (lambda: self.displace('left'), KeyMap.LEFT),
-            (lambda: self.displace('up'), KeyMap.UP),
-            (lambda: self.displace('down'), KeyMap.DOWN),
-        )
 
     def _open_default(self):
         self.update_idletasks()
         from studio.lib import legacy
         width = max(self.width - self._padding * 2, 300)
         height = max(self.height - self._padding * 2, 300)
         self.add(
@@ -221,42 +252,40 @@
             width=width, height=height
         )
         self.builder.generate()
         self.design_path = None
 
     @property
     def _ids(self):
-        return [i.id for i in self.objects]
+        return {i.id for i in self.objects}
 
     def has_changed(self):
         # check if design has changed since last save or loading so we can prompt user to save changes
         builder = self.builder
         if self.root_obj:
             builder = DesignBuilder(self)
             builder.generate()
         return builder != self.builder
 
     def open_new(self):
         # open a blank design
         self.open_file(None)
 
     def to_tree(self):
-        """ Generate node form of current design state without needing to save"""
-        builder = DesignBuilder(self)
-        builder.generate()
-        return builder.root
+        """ Generate builder for current design state without needing to save"""
+        return DesignBuilder(self)
 
     def save_prompt(self):
         return MessageDialog.builder(
-            {"text": "Save", "value": True, "focus": True},
-            {"text": "Don't save", "value": False},
-            {"text": "Cancel", "value": None},
+            {"text": _("Save"), "value": True, "focus": True},
+            {"text": _("Don't save"), "value": False},
+            {"text": _("Cancel"), "value": None},
             wait=True,
-            title="Save design",
-            message=f"Design file \"{self.context.name}\" has unsaved changes. Do you want to save them?",
+            title=_("Save design"),
+            message=_("Design file \"{name}\" has unsaved changes. Do you want to save them?").format(name=self.context.name),
             parent=self.studio,
             icon=MessageDialog.ICON_INFO
         )
 
     def open_file(self, path=None):
         if self.has_changed():
             save = self.save_prompt()
@@ -269,45 +298,45 @@
             elif save is None:
                 # user made no choice or basically selected cancel
                 return
         if path:
             self.builder = DesignBuilder(self)
             progress = MessageDialog.show_progress(
                 mode=MessageDialog.INDETERMINATE,
-                message='Loading design file to studio...',
+                message=_('Loading design file to studio...'),
                 parent=self.studio
             )
             self._load_design(path, progress)
         else:
             # if no path is supplied the default behaviour is to open a blank design
             self._open_default()
 
     def clear(self):
         # Warning: this method deletes elements irreversibly
         # remove the current root objects and their descendants
-        self.studio.select(None)
+        self.studio.selection.clear()
         # create a copy since self.objects will mostly change during iteration
         # remove root and dangling objects
         for widget in self.objects:
             widget.destroy()
         self.objects.clear()
         self.root_obj = None
 
     def _verify_version(self):
         if self.builder.metadata.get("version"):
-            _, major, __ = __version__.split(".")
+            __, major, ___ = __version__.split(".")
             if major < self.builder.metadata["version"].get("major", 0):
                 MessageDialog.show_warning(
                     parent=self.studio,
-                    message=(
+                    message=(_(
                         "Design was made using a higher version of the studio. \n"
                         "Some features may not be supported on this version. \n"
                         "Update to a new version of Formation for proper handling. \n"
                         "Note that saving may irreversibly strip off any unsupported features"
-                    )
+                    ))
                 )
 
     @as_thread
     def _load_design(self, path, progress=None):
         # Loading designs is elaborate so better do it on its own thread
         # Capture any errors that occur while loading
         # This helps the user single out syntax errors and other value errors
@@ -315,29 +344,30 @@
             self.design_path = path
             self.root_obj = self.builder.load(path, self)
             self.context.on_load_complete()
         except Exception as e:
             self.clear()
             self.studio.on_session_clear(self)
             accelerator = actions.get_routine("STUDIO_RELOAD").accelerator
-            text = f"{str(e)}\nPress {accelerator} to reload" if accelerator else f"{str(e)} \n reload design"
+            text = f"{str(e)}\n" + _("Press {} to reload").format(accelerator) if accelerator else f"{str(e)} \n" + _("reload design")
             self._show_empty(True, text=text, image=get_tk_image("dialog_error", 50, 50))
+            raise e
             # MessageDialog.show_error(parent=self.studio, title='Error loading design', message=str(e))
         finally:
             if progress:
                 progress.destroy()
             self._verify_version()
 
     def reload(self, *_):
         if not self.design_path or self.studio.context != self.context:
             return
         if self.has_changed():
             okay = MessageDialog.ask_okay_cancel(
-                title="Confirm reload",
-                message="All changes made will be lost",
+                title=_("Confirm reload"),
+                message=_("All changes made will be lost"),
                 parent=self.studio
             )
             if not okay:
                 # user made no choice or basically selected cancel
                 return
         self.clear()
         self.studio.on_session_clear(self)
@@ -355,86 +385,243 @@
 
     def as_node(self, widget):
         builder = self.builder
         if builder is None:
             builder = DesignBuilder(self)
         return builder.to_tree(widget)
 
-    def paste(self, node, silently=False, paste_to=None):
-        if paste_to is None:
-            paste_to = self.current_obj
-        if paste_to is None:
-            return
-        obj_class = BaseStudioAdapter._get_class(node)
-        if obj_class.is_toplevel and paste_to != self:
-            self._show_toplevel_warning()
-            return
-        if obj_class.group != Groups.container and self.root_obj is None:
-            self._show_root_widget_warning()
-            return
-
-        layout = paste_to if isinstance(paste_to, Container) else paste_to.layout
-        width = int(node["layout"].get("width", 10))
-        height = int(node["layout"].get("height", 10))
-        x, y = self._last_click_pos or (self.winfo_rootx() + 50, self.winfo_rooty() + 50)
-        self._last_click_pos = x + 5, y + 5  # slightly displace click position so multiple pastes are still visible
-        bounds = geometry.resolve_bounds((x, y, x + width, y + height), self)
-        obj = self.builder.load_section(node, layout, bounds)
-        restore_point = layout.get_restore(obj)
-        # Create an undo redo point if add is not silent
-        if not silently:
-            self.studio.new_action(Action(
-                # Delete silently to prevent adding the event to the undo/redo stack
-                lambda _: self.delete(obj, True),
-                lambda _: self.restore(obj, restore_point, obj.layout)
-            ))
-        return obj
-
     def _get_unique(self, obj_class):
         """
         Generate a unique id for widget belonging to a given class
         """
         return self.name_generator.generate(obj_class, self._ids)
 
+    def _is_unique_id(self, id_):
+        return id_ not in self._ids
+
     def on_motion(self, event):
-        self.highlight.resize(event)
         geometry.make_event_relative(event, self)
         self._coord_indicator.set_coord(
             self._frame.canvasx(event.x),
             self._frame.canvasy(event.y)
         )
 
+    def _refresh_container_sort(self):
+        self._sorted_containers = sorted(
+            filter(lambda x: isinstance(x, Container) and x not in self._move_selection, self.objects),
+            key=lambda x: -x.level
+        )
+
+    def _on_handle_active_start(self, widget, direction):
+        self._handle_active_data = widget, direction
+
+    def _on_handle_active(self, widget, direction):
+        if direction == "all":
+            self._move_selection = self.studio.selection.siblings(widget)
+            self.current_container = self._move_selection[0].layout
+            self.current_container.show_highlight()
+            self._refresh_container_sort()
+
+            self._all_bound = geometry.overall_bounds([w.get_bounds() for w in self._move_selection])
+            self._realtime_layout_update = True
+            for obj in self._move_selection:
+                obj.layout.start_move(obj)
+                # disable realtime layout update if any widget's layout doesn't support it
+                if not obj.layout.layout_strategy.realtime_support:
+                    self._realtime_layout_update = False
+        else:
+            for obj in self._selected:
+                if not obj.layout.allow_resize:
+                    continue
+                obj.layout.start_resize(obj)
+
+            if all(w.layout.layout_strategy.realtime_support for w in self._selected):
+                self._realtime_layout_update = True
+
+    def _on_handle_inactive(self, widget, direction):
+        if self._handle_active_data is not None:
+            # no movement occurred so we can skip the post-processing
+            self._handle_active_data = None
+            return
+
+        layouts_changed = []
+        if direction == "all":
+            if not self.current_container:
+                return
+            container = self.current_container
+            self.current_container = None
+            container.clear_highlight()
+            objs = self.studio.selection.siblings(widget)
+            toplevel_warning = False
+            for obj in objs:
+                if obj.is_toplevel and container != self:
+                    toplevel_warning = True
+                    continue
+                if obj.layout != container:
+                    obj.layout.remove_widget(obj)
+                    container.add_widget(obj, obj.get_bounds())
+                else:
+                    container.end_move(obj)
+                layouts_changed.append(obj)
+                if obj == self.root_obj and container != self:
+                    self.root_obj = container
+
+            if toplevel_warning:
+                self._show_toplevel_warning()
+        else:
+            for obj in self._selected:
+                if not obj.layout.allow_resize:
+                    continue
+                obj.layout.widget_released(obj)
+                layouts_changed.append(obj)
+
+        self.create_restore(layouts_changed)
+        self.studio.widgets_layout_changed(layouts_changed)
+        self._realtime_layout_update = False
+        self._skip_var = 0
+
+    def _on_handle_resize(self, widget, direction, delta):
+        if self._handle_active_data is not None:
+            self._on_handle_active(*self._handle_active_data)
+            self._handle_active_data = None
+
+        if self._skip_var < self._skip_max:
+            self._skip_var += 1
+            self._surge_delta = (self._surge_delta[0] + delta[0], self._surge_delta[1] + delta[1])
+            return
+        self._skip_var = 0
+        delta = (self._surge_delta[0] + delta[0], self._surge_delta[1] + delta[1])
+        self._surge_delta = (0, 0)
+
+        if direction != "all":
+            # resize
+            for obj in self._selected:
+                if obj.layout.allow_resize:
+                    obj.layout.resize_widget(obj, direction, delta)
+            if self._realtime_layout_update:
+                self.studio.widgets_layout_changed(self._selected)
+        else:
+            # move
+            self._on_handle_move(widget, delta)
+
+    def _on_handle_move(self, _, delta):
+        dx, dy = delta
+        objs = self._move_selection
+        all_bound = self._all_bound
+        dx = 0 if all_bound[0] + dx < 0 else dx
+        dy = 0 if all_bound[1] + dy < 0 else dy
+
+        if dx == dy == 0:
+            return
+
+        all_bound = (all_bound[0] + dx, all_bound[1] + dy, all_bound[2] + dx, all_bound[3] + dy)
+        current = self.current_container
+        container = self.layout_at(all_bound)
+        self._all_bound = all_bound
+
+        if container != current and current is not None:
+            current.layout_strategy.on_move_exit()
+            current.clear_highlight()
+
+        if container is not None and container != current:
+            container.show_highlight()
+            self.current_container = current = container
+
+        realtime_update = self._realtime_layout_update
+
+        for w in objs:
+            current.move_widget(w, delta)
+            if self._realtime_layout_update and current != w.layout:
+                # we can no longer attempt to provide realtime position info
+                realtime_update = False
+
+        if realtime_update:
+            self.studio.widgets_layout_changed(objs)
+
+    def set_active_container(self, container):
+        if self.current_container is not None:
+            self.current_container.clear_highlight()
+        self.current_container = container
+
+    def layout_at(self, bounds):
+        candidate = None
+        for container in self._sorted_containers:
+            if geometry.is_within(geometry.bounds(container), bounds):
+                candidate = container
+                break
+        if self.current_container and geometry.compute_overlap(geometry.bounds(self.current_container), bounds):
+            if candidate and candidate.level > self.current_container.level:
+                return candidate
+            return self.current_container
+
+        return candidate or self
+
+    def layout_at_pos(self, x, y):
+        x, y = geometry.resolve_position((x, y), self)
+        for container in self._sorted_containers:
+            if geometry.is_pos_within(geometry.bounds(container), (x, y)):
+                return container
+        if geometry.is_pos_within(geometry.bounds(self), (x, y)):
+            return self
+
+    def show_select_region(self, bounds):
+        bounds = geometry.resolve_bounds(bounds, self)
+        self._region_highlight.highlight_bounds(bounds)
+
+    def clear_select_region(self):
+        self._region_highlight.clear()
+
+    def select_in_region(self, widget, bounds):
+        if isinstance(widget, Container):
+            bounds = geometry.resolve_bounds(bounds, self)
+            to_select = []
+            for child in widget._children:
+                if geometry.compute_overlap(child.get_bounds(), bounds):
+                    to_select.append(child)
+            if to_select:
+                self.studio.selection.set(to_select)
+
     def _attach(self, obj):
         # bind events for context menu and object selection
         # all widget additions call this method so clear empty message
         self._show_empty(False)
+        obj.on_handle_resize(self._on_handle_resize)
+        obj.on_handle_active(self._on_handle_active_start)
+        obj.on_handle_inactive(self._on_handle_inactive)
+
         MenuUtils.bind_all_context(obj, lambda e: self.show_menu(e, obj), add='+')
-        obj.bind_all('<Shift-ButtonPress-1>', lambda e: self.highlight.set_function(self.highlight.move, e), add='+')
         obj.bind_all('<Motion>', self.on_motion, '+')
-        obj.bind_all('<ButtonRelease>', self.highlight.clear_resize, '+')
-        obj.bind_all('<KeyRelease>', self._stop_displace, '+')
+
         if "text" in obj.keys():
             obj.bind_all("<Double-Button-1>", lambda _: self._show_text_editor(obj))
+
         self.objects.append(obj)
         if self.root_obj is None:
             self.root_obj = obj
         obj.bind_all("<Button-1>", lambda e: self._handle_select(obj, e), add='+')
         # bind shortcuts
         self._shortcut_mgr.bind_widget(obj)
 
     def show_menu(self, event, obj=None):
-        # select object generating the context menu event first
-        if obj is not None:
-            self.select(obj)
+        try:
+            self._last_click_pos = event.x_root, event.y_root
+        except TclError:
+            pass
+
+        if obj and obj not in self._selected:
+            self.studio.selection.set(obj)
         MenuUtils.popup(event, self._context_menu)
 
     def _handle_select(self, obj, event):
         # store the click position for effective widget pasting
         self._last_click_pos = event.x_root, event.y_root
-        self.select(obj)
+        if event.state & EventMask.CONTROL:
+            self.studio.selection.toggle(obj)
+        elif obj not in self.studio.selection:
+            self.studio.selection.set(obj)
 
     def load(self, obj_class, name, container, attributes, layout, bounds=None):
         obj = obj_class(self, name)
         obj.configure(**attributes)
         self._attach(obj)
         if bounds is not None:
             container.add_widget(obj, bounds)
@@ -442,22 +629,22 @@
             container.add_widget(obj, **layout)
         if container == self:
             container = None
         self.studio.add(obj, container)
         return obj
 
     def _show_root_widget_warning(self):
-        MessageDialog.show_warning(title='Invalid root widget', parent=self.studio,
-                                   message='Only containers are allowed as root widgets')
+        MessageDialog.show_warning(title=_('Invalid root widget'), parent=self.studio,
+                                   message=_('Only containers are allowed as root widgets'))
 
     def _show_toplevel_warning(self):
         MessageDialog.show_warning(
-            title='Invalid parent',
+            title=_('Invalid parent'),
             parent=self.studio,
-            message='Toplevel widgets cannot be placed inside other widgets'
+            message=_('Toplevel widgets cannot be placed inside other widgets')
         )
 
     def add(self, obj_class: PseudoWidget.__class__, x, y, **kwargs):
         layout = kwargs.get("layout")
         if obj_class.is_toplevel and layout not in (self, None):
             self._show_toplevel_warning()
             return
@@ -485,265 +672,202 @@
             layout.add_widget(obj, bounds)
             self.studio.add(obj, layout)
             restore_point = layout.get_restore(obj)
             # Create an undo redo point if add is not silent
             if not silent:
                 self.studio.new_action(Action(
                     # Delete silently to prevent adding the event to the undo/redo stack
-                    lambda _: self.delete(obj, True),
-                    lambda _: self.restore(obj, restore_point, obj.layout)
+                    lambda _: self.delete([obj], True),
+                    lambda _: self.restore([obj], [restore_point], [obj.layout])
                 ))
         elif obj.layout is None:
             # This only happens when adding the main layout. We dont need to add this action to the undo/redo stack
             # This main layout is attached directly to the designer
             obj.layout = self
             self.layout_strategy.add_widget(obj, x=x, y=y, width=width, height=height)
             self.studio.add(obj, None)
 
         return obj
 
+    def paste(self, clipboard, silently=False, paste_to=None):
+        if paste_to is None and len(self.studio.selection) != 1:
+            return
+
+        if paste_to is None:
+            paste_to = self.studio.selection[0]
+
+        if paste_to is None:
+            return
+
+        x, y = self._last_click_pos or (self.winfo_rootx() + 50, self.winfo_rooty() + 50)
+        # slightly displace click position so multiple pastes are still visible
+        self._last_click_pos = x + 5, y + 5
+
+        objs = []
+        restore_points = []
+
+        for node, bound in clipboard:
+            obj_class = BaseStudioAdapter._get_class(node)
+            if obj_class.is_toplevel and paste_to != self:
+                self._show_toplevel_warning()
+                return
+            if obj_class.group != Groups.container and self.root_obj is None:
+                self._show_root_widget_warning()
+                return
+
+            layout = paste_to if isinstance(paste_to, Container) else paste_to.layout
+            bound = geometry.resolve_bounds(geometry.displace(bound, x, y), self)
+            obj = self.builder.load_section(node, layout, bound)
+            objs.append(obj)
+            restore_points.append(layout.get_restore(obj))
+            # Create an undo redo point if add is not silent
+
+        if not silently:
+            self.studio.new_action(Action(
+                # Delete silently to prevent adding the event to the undo/redo stack
+                lambda _: self.delete(objs, True),
+                lambda _: self.restore(objs, restore_points, [w.layout for w in objs])
+            ))
+        return objs
+
     def select_layout(self, layout: Container):
         pass
 
-    def restore(self, widget, restore_point, container):
-        container.restore_widget(widget, restore_point)
-        self.studio.on_restore(widget)
-        self._replace_all(widget)
+    def restore(self, widgets, restore_points, containers):
+        for container, widget, restore_point in zip(containers, widgets, restore_points):
+            container.restore_widget(widget, restore_point)
+            self._replace_all(widget)
+        if self.root_obj in widgets:
+            self._show_empty(False)
+        self.studio.on_restore(widgets)
 
     def _replace_all(self, widget):
         # Recursively add widget and all its children to objects
         self.objects.append(widget)
         if self.root_obj is None:
             self.root_obj = widget
         if isinstance(widget, Container):
             for child in widget._children:
                 self._replace_all(child)
 
-    def delete(self, widget, silently=False):
-        if not widget:
+    def delete(self, widgets, silently=False):
+        if not widgets:
             return
         if not silently:
-            restore_point = widget.layout.get_restore(widget)
+            restore_points = [widget.layout.get_restore(widget) for widget in widgets]
+            layouts = [widget.layout for widget in widgets]
             self.studio.new_action(Action(
-                lambda _: self.restore(widget, restore_point, widget.layout),
-                lambda _: self.studio.delete(widget, True)
+                lambda _: self.restore(widgets, restore_points, layouts),
+                lambda _: self.studio.delete(widgets, True)
             ))
         else:
-            self.studio.delete(widget, self)
-        widget.layout.remove_widget(widget)
-        if widget == self.root_obj:
-            # try finding another toplevel widget that can be a root obj otherwise leave it as none
-            self.root_obj = None
-            for w in self.layout_strategy.children:
-                if isinstance(w, Container) or w.group == Groups.container:
-                    self.root_obj = w
-                    break
-        self._uproot_widget(widget)
+            self.studio.delete(widgets, self)
+
+        for widget in widgets:
+            widget.layout.remove_widget(widget)
+            if widget == self.root_obj:
+                # try finding another toplevel widget that can be a root obj otherwise leave it as none
+                self.root_obj = None
+                for w in self.layout_strategy.children:
+                    if isinstance(w, Container) or w.group == Groups.container:
+                        self.root_obj = w
+                        break
+            self._uproot_widget(widget)
         if not self.objects:
             self._show_empty(True)
 
     def _uproot_widget(self, widget):
         # Recursively remove widgets and all its children
         if widget in self.objects:
             self.objects.remove(widget)
         if isinstance(widget, Container):
             for child in widget._children:
                 self._uproot_widget(child)
 
-    def set_active_container(self, container):
-        if self.current_container is not None:
-            self.current_container.clear_highlight()
-        self.current_container = container
-
-    def compute_overlap(self, bound1, bound2):
-        return geometry.compute_overlap(bound1, bound2)
-
-    def layout_at(self, bounds):
-        for container in sorted(filter(lambda x: isinstance(x, Container) and x != self.current_obj, self.objects),
-                                key=lambda x: len(self.objects) - x.level):
-            if isinstance(self.current_obj, Container) and self.current_obj.level < container.level:
-                continue
-            if self.compute_overlap(geometry.bounds(container), bounds):
-                return container
-        return None
-
     def parse_bounds(self, bounds):
         return {
             "x": bounds[0],
             "y": bounds[1],
             "width": bounds[2] - bounds[0],
             "height": bounds[3] - bounds[1]
         }
 
     def position(self, widget, bounds):
         self.place_child(widget, **self.parse_bounds(bounds))
 
-    def select(self, obj, explicit=False):
-        if obj is None:
-            self.clear_obj_highlight()
-            self.studio.select(None, self)
-            self.highlight.clear()
+    def _select(self, _):
+        if self.studio.designer != self:
             return
-        self.focus_set()
-        if self.current_obj == obj:
+        current_selection = set(self.studio.selection.widgets)
+        if current_selection == self._selected:
             return
-        self.clear_obj_highlight()
-        self.current_obj = obj
-        self.draw_highlight(obj)
-        if not explicit:
-            # The event is originating from the designer
-            self.studio.select(obj, self)
-
-    def draw_highlight(self, obj):
-        self.highlight.surround(obj)
-
-    def _stop_displace(self, _):
-        if self._displace_active:
-            # this ensures event is added to undo redo stack
-            self._on_release(geometry.bounds(self.current_obj))
-            # mark the latest action as designer displace
-            latest = self.studio.last_action()
-            if latest is not None:
-                latest.key = "designer_displace"
-            self._displace_active = False
 
-    def displace(self, side):
-        if not self.current_obj:
-            return
-        if time.time() - self._last_displace < .5:
-            self.studio.pop_last_action("designer_displace")
+        for w in self._selected - current_selection:
+            w.clear_handle()
 
-        self._on_start()
-        self._displace_active = True
-        self._last_displace = time.time()
-        bounds = geometry.bounds(self.current_obj)
-        x1, y1, x2, y2 = bounds
-        if side == 'right':
-            bounds = x1 + 1, y1, x2 + 1, y2
-        elif side == 'left':
-            bounds = x1 - 1, y1, x2 - 1, y2
-        elif side == 'up':
-            bounds = x1, y1 - 1, x2, y2 - 1
-        elif side == 'down':
-            bounds = x1, y1 + 1, x2, y2 + 1
-        self._on_move(bounds)
-
-    def clear_obj_highlight(self):
-        if self.highlight is not None:
-            self.highlight.clear()
-            self.current_obj = None
-            if self.current_container is not None:
-                self.current_container.clear_highlight()
-                self.current_container = None
+        for w in current_selection - self._selected:
+            w.show_handle()
+
+        self._selected = current_selection
+        self.focus_set()
+
+    @property
+    def selected(self):
+        return self._selected
 
     def _on_start(self):
         obj = self.current_obj
         if obj is not None:
-            obj.layout.change_start(obj)
+            obj.layout.start_move(obj)
 
-    def _on_release(self, bound):
-        obj = self.current_obj
-        container = self.current_container
-        if obj is None:
+    def create_restore(self, widgets):
+        if not widgets:
             return
-        if container is not None and container != obj:
-            container.clear_highlight()
-            if self.current_action == self.MOVE:
-                if container != self and obj.is_toplevel:
-                    self._show_toplevel_warning()
-                    return
-                container.add_widget(obj, bound)
-                # If the enclosed widget was initially the root object, make the container the new root object
-                if obj == self.root_obj and obj != self:
-                    self.root_obj = self.current_container
-            else:
-                obj.layout.widget_released(obj)
-            self.studio.widget_layout_changed(obj)
-            self.current_action = None
-            self.create_restore(obj)
-        elif obj.layout == self and self.current_action == self.MOVE:
-            self.create_restore(obj)
-        elif self.current_action == self.RESIZE:
-            obj.layout.widget_released(obj)
-            self.current_action = None
-            self.create_restore(obj)
-
-    def create_restore(self, widget):
-        prev_restore_point = widget.recent_layout_info
-        cur_restore_point = widget.layout.get_restore(widget)
-        if prev_restore_point == cur_restore_point:
+
+        prev_restore_points = [widget.recent_layout_info for widget in widgets]
+        cur_restore_points = [widget.layout.get_restore(widget) for widget in widgets]
+
+        if prev_restore_points == cur_restore_points:
             return
-        prev_container = prev_restore_point["container"]
-        container = widget.layout
+
+        prev_containers = [i["container"] for i in prev_restore_points]
+        containers = [widget.layout for widget in widgets]
 
         def undo(_):
-            container.remove_widget(widget)
-            prev_container.restore_widget(widget, prev_restore_point)
+            for widget, prev_restore_point, container, prev_container in zip(
+                    widgets, prev_restore_points, containers, prev_containers):
+                container.remove_widget(widget)
+                prev_container.restore_widget(widget, prev_restore_point)
+            self.studio.widgets_layout_changed(widgets)
 
         def redo(_):
-            prev_container.remove_widget(widget)
-            container.restore_widget(widget, cur_restore_point)
+            for widget, cur_restore_point, container, prev_container in zip(
+                    widgets, cur_restore_points, containers, prev_containers):
+                prev_container.remove_widget(widget)
+                container.restore_widget(widget, cur_restore_point)
+            self.studio.widgets_layout_changed(widgets)
 
         self.studio.new_action(Action(undo, redo))
 
-    def _on_move(self, new_bound):
-        obj = self.current_obj
-        current = self.current_container
-        if obj is None:
-            return
-        self.current_action = self.MOVE
-        container: Container = self.layout_at(new_bound)
-        if container is not None and obj != container:
-            if container != current:
-                if current is not None:
-                    current.clear_highlight()
-                container.show_highlight()
-                self.current_container = container
-            container.move_widget(obj, new_bound)
-        else:
-            if current is not None:
-                current.clear_highlight()
-                self.current_container = self
-            obj.level = 0
-            obj.layout = self
-            self.move_widget(obj, new_bound)
-        if obj.layout.layout_strategy.realtime_support:
-            self.studio.widget_layout_changed(obj)
-
-    def _on_size_changed(self, new_bound):
-        obj = self.current_obj
-        if obj is None:
-            return
-        self.current_action = self.RESIZE
-        if self.current_obj.max_size or self.current_obj.min_size:
-            b = geometry.constrain_bounds(
-                new_bound,
-                self.current_obj.max_size,
-                self.current_obj.min_size
-            )
-            new_bound = b
-
-        if isinstance(obj.layout, Container):
-            obj.layout.resize_widget(obj, new_bound)
-
-        if obj.layout.layout_strategy.realtime_support:
-            self.studio.widget_layout_changed(obj)
-
     def _text_change(self):
-        self.studio.style_pane.apply_style("text", self._text_editor.get_all(), self.current_obj)
+        self.studio.style_pane.apply_style("text", self._text_editor.get_all())
 
     def _show_text_editor(self, widget):
-        assert widget == self.current_obj
-        self._text_editor.lift(widget)
+        if any("text" not in w.keys() for w in self.selected):
+            return
         cnf = self._collect_text_config(widget)
         self._text_editor.config(**cnf)
         self._text_editor.place(in_=widget, relwidth=1, relheight=1, x=0, y=0)
+        self._text_editor.lift(widget)
         self._text_editor.clear()
         self._text_editor.focus_set()
+        # suppress change event while we set initial value
+        self._text_editor.on_change(lambda *_: None)
         self._text_editor.insert("1.0", widget["text"])
+        self._text_editor.on_change(self._text_change)
 
     def _collect_text_config(self, widget):
         s = ttk.Style()
         config = dict(
             background="#ffffff",
             foreground="#000000",
             font="TkDefaultFont"
@@ -756,18 +880,80 @@
                 config[opt] = (s.lookup(widget.winfo_class(), opt) or config[opt])
         config["insertbackground"] = config["foreground"]
         return config
 
     def _text_hide(self, *_):
         self._text_editor.place_forget()
 
-    def on_select(self, widget):
-        self.select(widget)
+    def send_back(self, steps=0):
+        if not (self.studio.selection and self.studio.selection.is_same_parent()):
+            return
+
+        child_list = next(iter(self.studio.selection)).layout._children
+        widgets = sorted(self.studio.selection, key=child_list.index)
+
+        if steps == 0:
+            self._update_stacking({w: index for index, w in enumerate(widgets)})
+        else:
+            self._update_stacking({w: max(0, child_list.index(w) - steps) for w in widgets})
+
+    def bring_front(self, steps=0):
+        if not (self.studio.selection and self.studio.selection.is_same_parent()):
+            return
+
+        child_list = next(iter(self.studio.selection)).layout._children
+        widgets = sorted(self.studio.selection, key=child_list.index)
+
+        end = len(child_list) - 1
+        if steps == 0:
+            self._update_stacking({w: end for w in widgets})
+        else:
+            self._update_stacking({w: min(end, child_list.index(w) + steps) for w in widgets})
+
+    def _update_stacking(self, indices, silently=False):
+        if not indices:
+            return
+
+        child_list = next(iter(indices)).layout._children
+        # reorder child list based on indices
+
+        indices = sorted(
+            indices.items(),
+            key=lambda x: (x[1], -child_list.index(x[0]) if x[1] == 0 else child_list.index(x[0]))
+        )
+        for widget, _ in indices:
+            child_list.remove(widget)
+
+        for widget, index in indices:
+            child_list.insert(index, widget)
+
+        prev_data = {}
+        data = {}
+        for index, widget in enumerate(child_list):
+            if widget.prev_stack_index != index:
+                prev_data[widget] = widget.prev_stack_index
+                data[widget] = index
+            widget.prev_stack_index = index
+            if index > 0:
+                widget.lift(child_list[index - 1])
+            else:
+                widget.lift(widget.layout.body)
+
+        prev_data = dict(sorted(prev_data.items(), key=lambda x: x[1]))
+
+        if not silently and prev_data != data:
+            self.studio.new_action(Action(
+                lambda _: self._update_stacking(prev_data, True),
+                lambda _: self._update_stacking(data, True)
+            ))
 
-    def on_widget_change(self, old_widget, new_widget=None):
+    def on_widgets_reorder(self, indices):
+        pass
+
+    def on_widgets_change(self, widgets):
         pass
 
     def on_widget_add(self, widget, parent):
         pass
 
     def show_highlight(self, *_):
         pass
@@ -786,36 +972,52 @@
                 return False
         return True
 
 
 class DesignContext(BaseContext):
     _untitled_count = 0
 
+    _formats = {
+        "xml": "file_xml",
+        "json": "file_json",
+    }
+
     def __init__(self, master, studio, path=None):
         super(DesignContext, self).__init__(master, studio)
         self.designer = Designer(self, studio)
         self.designer.pack(fill="both", expand=True)
         self.path = path
-        self.icon = get_tk_image("paint", 15, 15)
+        self.icon = get_tk_image(self._formats.get(self.format_from_path(path), "file"), 15, 15)
         self.name = self.name_from_path(path) if path else self._create_name()
         self._loaded = False
 
     def _create_name(self):
         DesignContext._untitled_count += 1
         return f"untitled_{DesignContext._untitled_count}"
 
     def name_from_path(self, path):
         return os.path.basename(path)
 
+    def format_from_path(self, path):
+        if not path:
+            return ""
+        # get file extension
+        _, ext = os.path.splitext(path)
+        return ext[1:].lower()
+
     def save(self, new_path=None):
         path = self.designer.save(new_path)
         if path:
             self.path = path
             self.name = self.name_from_path(path)
-            self.tab_handle.config_tab(text=self.name, **self.style.text)
+            self.icon = get_tk_image(self._formats.get(self.format_from_path(path), "file"), 15, 15)
+            self.tab_handle.config_tab(
+                text=self.name, **self.style.text,
+                icon=self.icon
+            )
 
             if self.tab_view._selected == self.tab_handle:
                 # re-apply selection style
                 self.tab_handle.on_select()
         return path
 
     def on_context_set(self):
@@ -823,24 +1025,28 @@
         if not self._loaded:
             if self.path:
                 self.designer.open_file(self.path)
             else:
                 self.designer.open_new()
             self._loaded = True
         self.studio.set_path(self.path)
+        self.designer.add_studio_binding("<<SelectionChanged>>", self.designer._select, "+")
+
+    def on_context_unset(self):
+        self.designer.clear_studio_bindings()
 
     def on_load_complete(self):
         # the design load thread is done
         self.update_save_status()
 
     def get_tab_menu(self):
         return (
             EnableIf(
                 lambda: self.studio.context == self and self.designer.design_path,
-                ("command", "Reload", icon("rotate_clockwise", 14, 14), self.designer.reload, {})
+                ("command", _("Reload"), icon("reload", 18, 18), self.designer.reload, {})
             ),
         )
 
     def serialize(self):
         data = super().serialize()
         data["args"] = (self.path, )
         return data
@@ -875,17 +1081,14 @@
     def redo(self):
         super(DesignContext, self).redo()
         self.update_save_status()
 
     def can_persist(self):
         return self.path is not None
 
-    def on_context_unset(self):
-        pass
-
     def on_app_close(self):
         return self.designer.on_app_close()
 
     def on_context_close(self):
         return self.designer.on_app_close()
 
 
@@ -910,15 +1113,15 @@
         def on_hover_ended(self, *_):
             self.config_all(**self.style.bright)
 
     def __init__(self, master, studio, contexts=None):
         self.studio = studio
         self.check_contexts = contexts
         super(MultiSaveDialog, self).__init__(master, self.render)
-        self.title("Save dialog")
+        self.title(_("Save dialog"))
         self.value = None
 
     def cancel(self, *_):
         self.destroy()
 
     def discard(self, *_):
         self.value = []
@@ -936,18 +1139,18 @@
 
     def render(self, window):
         contexts = self.check_contexts if self.check_contexts is not None else self.studio.contexts
         self.contexts = [
             i for i in contexts if isinstance(i, DesignContext) and i.designer.has_changed()
         ]
         self.geometry("500x250")
-        self._message("Some files have changes. Select files to save", self.ICON_INFO)
+        self._message(_("Some files have changes. Select files to save"), self.ICON_INFO)
         self.context_choice = CompoundList(window)
         self.context_choice.config(padx=2, height=200)
         self.context_choice.set_item_class(MultiSaveDialog.CheckedItem)
         self.context_choice.set_values(self.contexts)
         self.context_choice.config_all(**self.style.hover)
         self._make_button_bar()
-        self.cancel_btn = self._add_button(text="Cancel", command=self.cancel)
-        self.save_btn = self._add_button(text="Don't save", command=self.discard)
-        self.discard_btn = self._add_button(text="Save", command=self.save, focus=True)
+        self.cancel_btn = self._add_button(text=_("Cancel"), command=self.cancel)
+        self.save_btn = self._add_button(text=_("Don't save"), command=self.discard)
+        self.discard_btn = self._add_button(text=_("Save"), command=self.save, focus=True)
         self.context_choice.pack(fill="both", expand=True, padx=10, pady=5)
```

### Comparing `formation-studio-0.6.3/studio/feature/eventspane.py` & `formation-studio-0.7.0/studio/feature/variablepane.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,256 +1,254 @@
+"""
+Variable management for the studio. Creates and manages variables making them available
+for widgets with variable and text-variable properties
+"""
+# ======================================================================= #
+# Copyright (C) 2020 Hoverset Group.                                      #
+# ======================================================================= #
+import functools
+import tkinter as tk
+
+import studio.ui.editors as editors
 from hoverset.ui.icons import get_icon_image
-from hoverset.ui.widgets import (
-    Label, CompoundList, Entry, Frame, Checkbutton, Button
-)
+from hoverset.ui.widgets import ScrolledFrame, Button, MenuButton, Frame, Label
 from studio.feature._base import BaseFeature
-from studio.lib.events import EventBinding, make_event
-
-
-class BindingsTable(CompoundList):
-    class EventItem(CompoundList.BaseItem):
-
-        def __init__(self, master, value: EventBinding, index, isolated=False):
-            super().__init__(master, value, index, isolated)
-            self.parent_list = master
-
-        @property
-        def id(self):
-            return self.value.id
-
-        def _on_value_change(self):
-            event = EventBinding(
-                self.id,
-                self.sequence.get(),
-                self.handler.get(),
-                self.add_arg.get(),
-            )
-            self.parent_list._item_changed(event)
-
-        def _delete_entry(self, *_):
-            self.parent_list._item_deleted(self)
-            # prevent event propagation since item will be deleted
-            return "break"
-
-        def render(self):
-            self.config(height=40)
-            seq_frame = Frame(self, **self.style.highlight)
-            seq_frame.grid(row=0, column=0, sticky="nsew")
-            seq_frame.pack_propagate(False)
-            self.sequence = Entry(seq_frame, **self.style.input)
-            self.sequence.place(x=0, y=0, relwidth=1, relheight=1, width=-40)
-            self.sequence.set(self.value.sequence)
-            self.sequence.configure(**self.style.no_highlight)
-            self.sequence.focus_set()
-            self.handler = Entry(self, **self.style.input)
-            self.handler.grid(row=0, column=1, sticky="ew")
-            self.handler.set(self.value.handler)
-            self.handler.config(**self.style.highlight)
-            self.add_arg = Checkbutton(self, **self.style.checkbutton)
-            self.add_arg.grid(row=0, column=2, sticky="ew")
-            self.add_arg.set(self.value.add)
-            del_btn = Label(
-                self, **self.style.button,
-                image=get_icon_image("delete", 14, 14)
-            )
-            del_btn.grid(row=0, column=3, sticky='nswe')
-            del_btn.bind("<Button-1>", self._delete_entry)
-            # set the first two columns to expand evenly
-            for column in range(2):
-                self.grid_columnconfigure(column, weight=1, uniform=1)
-
-            for widget in (self.sequence, self.handler):
-                widget.on_change(self._on_value_change)
-
-            self.add_arg._var.trace("w", lambda *_: self._on_value_change())
-
-        def hide(self):
-            self.pack_forget()
-
-        def show(self):
-            self.pack(fill="x", pady=1, side="top")
-
-        def on_hover(self, *_):
-            pass
-
-        def on_hover_ended(self, *_):
-            pass
-
-        def update_details(self, value, index):
-            self._index = index
-            self._value = value
-            self.sequence.set(value.sequence)
-            self.handler.set(value.handler)
-            self.add_arg.set(value.add)
-
-    def __init__(self, master=None, **kwargs):
-        super(BindingsTable, self).__init__(master, **kwargs)
-        self.set_item_class(BindingsTable.EventItem)
-        self._item_pool = []
-        self._on_value_change = None
-        self._on_delete = None
-
-    def clear(self):
-        for item in self.items:
-            item.pack_forget()
-            self._item_pool.append(item)
-        self._items.clear()
-
-    def add(self, *events):
-        self.add_values(events)
-
-    def _render(self, values):
-        for i, value in enumerate(values):
-            if self._item_pool:
-                item = self._item_pool[0]
-                self._item_pool.remove(item)
-                item.update_details(value, i)
-            else:
-                item = self._cls(self, value, i)
-            self._items.append(item)
-            item.show()
-            item.update_idletasks()
-
-    def _remove_item(self, item):
-        item.pack_forget()
-        self._item_pool.append(item)
-        # if item is selected deselect it
-        if self.get() == item:
-            item.deselect()
-            self._current_indices = []
-
-        self._items.remove(item)
-
-    def remove(self, _id):
-        for item in filter(lambda i: i.id == _id, self.items):
-            self._remove_item(item)
-        self._values = tuple(filter(lambda e: e.id != _id, self._values))
+from studio.lib.variables import VariableItem, VariableManager
+from studio.i18n import _
 
-    def on_value_change(self, callback, *args, **kwargs):
-        self._on_value_change = lambda value: callback(value, *args, **kwargs)
 
-    def on_item_delete(self, callback, *args, **kwargs):
-        self._on_delete = lambda value: callback(value, *args, **kwargs)
+class VariablePane(BaseFeature):
+    name = "Variablepane"
+    display_name = _("Variables")
+    icon = "text"
 
-    def _item_changed(self, value):
-        if self._on_value_change:
-            self._on_value_change(value)
-
-    def _item_deleted(self, item):
-        if self._on_delete:
-            self._on_delete(item)
-
-    def hide_all(self):
-        for item in self.items:
-            item.hide()
-
-
-class EventPane(BaseFeature):
-    name = "Event pane"
-    icon = "blank"
     _defaults = {
         **BaseFeature._defaults,
-        "side": "right",
+        "side": "right"
     }
-    NO_SELECTION_MSG = "You have not selected any widget selected"
-    NO_EVENT_MSG = "You have not added any bindings"
-    NO_MATCH_MSG = "No items match your search"
 
-    def __init__(self, master, studio, **cnf):
+    _definitions = {
+        "name": {
+            "name": "name",
+            "type": "text",
+        }
+    }
+
+    _empty_message = _("No variables added")
+
+    def __init__(self, master, studio=None, **cnf):
         super().__init__(master, studio, **cnf)
-        self.header = Frame(self, **self.style.surface)
-        self.header.pack(side="top", fill="x")
-        for i, title in enumerate(("Sequence", "Handler", "Add", " " * 3)):
-            Label(
-                self.header, **self.style.text_passive, text=title,
-                anchor="w",
-            ).grid(row=0, column=i, sticky='ew')
-
-        # set the first two columns to expand evenly
-        for column in range(2):
-            self.header.grid_columnconfigure(column, weight=1, uniform=1)
-
-        self.bindings = BindingsTable(self)
-        self.bindings.on_value_change(self.modify_item)
-        self.bindings.on_item_delete(self.delete_item)
-        self.bindings.pack(fill="both", expand=True)
-
-        self._add = Button(
-            self._header, **self.style.button, width=25, height=25,
-            image=get_icon_image("add", 15, 15)
+        f = Frame(self, **self.style.surface)
+        f.pack(side="top", fill="both", expand=True, pady=4)
+        f.pack_propagate(0)
+
+        self._variable_pane = ScrolledFrame(f, width=150)
+        self._variable_pane.place(x=0, y=0, relwidth=0.4, relheight=1)
+
+        self._detail_pane = ScrolledFrame(f, width=150)
+        self._detail_pane.place(relx=0.4, y=0, relwidth=0.6, relheight=1, x=15, width=-20)
+
+        Label(
+            self._detail_pane.body, **self.style.text_passive,
+            text=_("Type"), anchor="w"
+        ).pack(side="top", fill="x")
+        self.var_type_lbl = Label(
+            self._detail_pane.body, **self.style.text, anchor="w"
         )
-        self._add.pack(side="right")
-        self._add.tooltip("Add event binding")
-        self._add.on_click(self.add_new)
+        self.var_type_lbl.pack(side="top", fill="x")
+        Label(
+            self._detail_pane.body, **self.style.text_passive,
+            text=_("Name"), anchor="w"
+        ).pack(side="top", fill="x")
+        self.var_name = editors.get_editor(self._detail_pane.body, self._definitions["name"])
+        self.var_name.pack(side="top", fill="x")
+        Label(
+            self._detail_pane.body, **self.style.text_passive,
+            text=_("Value"), anchor="w"
+        ).pack(fill="x", side="top")
+        self._editors = {}
+        self._editor = None
 
-        self._search_btn = Button(
-            self._header, **self.style.button,
-            image=get_icon_image("search", 15, 15), width=25, height=25,
-        )
+        self._search_btn = Button(self._header, image=get_icon_image("search", 15, 15), width=25, height=25,
+                                  **self.style.button)
         self._search_btn.pack(side="right")
         self._search_btn.on_click(self.start_search)
+        self._search_query = None
 
-        self._empty_frame = Label(self.bindings, **self.style.text_passive)
-        self._show_empty(self.NO_SELECTION_MSG)
+        self._add = MenuButton(self._header, **self.style.button)
+        self._add.configure(image=get_icon_image("add", 15, 15))
+        self._add.pack(side="right")
+        self._delete_btn = Button(self._header, image=get_icon_image("delete", 15, 15), width=25, height=25,
+                                  **self.style.button)
+        self._delete_btn.pack(side="right")
+        self._delete_btn.on_click(self._delete)
+        self._var_types_menu = self.make_menu(
+            self._get_add_menu(),
+            self._add, title=_("Add variable"))
+        self._var_types_menu.configure(tearoff=True)
+        self._add.config(menu=self._var_types_menu)
+        self._selected = None
+        self._links = {}
+        self._overlay = Label(f, **self.style.text_passive, text=self._empty_message, compound="top")
+        self._overlay.configure(image=get_icon_image("add", 25, 25))
+        self._show_overlay(True)
 
-    def _show_empty(self, message):
-        self._empty_frame.place(x=0, y=0, relwidth=1, relheight=1)
-        self._empty_frame["text"] = message
+    def start_search(self, *_):
+        if self.variables:
+            super().start_search()
+            self._variable_pane.scroll_to_start()
 
-    def _remove_empty(self):
-        self._empty_frame.place_forget()
+    def on_search_query(self, query):
+        matches = []
+        self._variable_pane.clear_children()
+        for item in self.variables:
+            if query in item.name:
+                self._show(item)
+                matches.append(item)
+
+        if not matches:
+            self._show_overlay(True, text=_("No matches found"), image=get_icon_image("search", 25, 25))
+        else:
+            self.select(matches[0])
+            self._show_overlay(False)
+        self._search_query = query
 
-    def add_new(self, *_):
-        if self.studio.selected is None:
-            return
-        self._remove_empty()
-        new_binding = make_event("<>", "", False)
-        widget = self.studio.selected
-        if not hasattr(widget, "_event_map_"):
-            setattr(widget, "_event_map_", {})
-        widget._event_map_[new_binding.id] = new_binding
-        self.bindings.add(new_binding)
-
-    def delete_item(self, item):
-        widget = self.studio.selected
-        if widget is None:
-            return
-        widget._event_map_.pop(item.id)
-        self.bindings.remove(item.id)
+    def on_search_clear(self):
+        self.on_search_query("")
+        self._search_query = None
+        # remove overlay if we have variables otherwise show it
+        self._show_overlay(not self.variables)
+        super().on_search_clear()
 
-    def modify_item(self, value: EventBinding):
-        widget = self.studio.selected
-        widget._event_map_[value.id] = value
-
-    def on_select(self, widget):
-        if widget is None:
-            self._show_empty(self.NO_SELECTION_MSG)
+    def _get_add_menu(self):
+        _types = VariableItem._types
+        return [(
+            tk.COMMAND,
+            _types[i].get("name"),
+            get_icon_image(_types[i].get("icon"), 18, 18),
+            functools.partial(self.menu_add_var, i), {}
+        ) for i in _types]
+
+    def create_menu(self):
+        return (
+            ("cascade", _("Add"), get_icon_image("add", 18, 18), None, {"menu": self._get_add_menu()}),
+            ("command", _("Delete"), get_icon_image("delete", 18, 18), self._delete, {}),
+            ("command", _("Search"), get_icon_image("search", 18, 18), self.start_search, {}),
+        )
+
+    def _show_overlay(self, flag=True, **kwargs):
+        if flag:
+            kwargs["text"] = kwargs.get("text", self._empty_message)
+            kwargs["image"] = kwargs.get("image", get_icon_image("add", 25, 25))
+            self._overlay.lift()
+            self._overlay.configure(**kwargs)
+            self._overlay.place(x=0, y=0, relwidth=1, relheight=1)
+        else:
+            self._overlay.place_forget()
+
+    def menu_add_var(self, var_type, **kw):
+        item = self.add_var(var_type, **kw)
+        self.select(item)
+
+    def add_var(self, var_type, **kw):
+        var = var_type(self.studio)
+        item_count = len(list(filter(lambda x: x.var_type == var_type, self.variables))) + 1
+        name = kw.get('name', f"{var_type.__name__}_{item_count}")
+        value = kw.get('value')
+        item = VariableItem(self._variable_pane.body, var, name)
+        item.bind("<Button-1>", lambda e: self.select(item))
+        if value is not None:
+            item.set(value)
+
+        self._show(item)
+        self._show_overlay(False)
+        if self._search_query is not None:
+            # reapply search if any
+            self.on_search_query(self._search_query)
+        elif not self.variables:
+            self.select(item)
+        VariableManager.add(item)
+        return item
+
+    def delete_var(self, var):
+        self._hide(var)
+        VariableManager.remove(var)
+
+    def _delete(self, *_):
+        if self._selected:
+            self.delete_var(self._selected)
+        if self.variables:
+            self.select(self.variables[0])
+        else:
+            self._show_overlay(True)
+
+    def clear_variables(self):
+        # the list is likely to change during iteration, create local copy
+        variables = list(self.variables)
+        for var in variables:
+            self.delete_var(var)
+        self._show_overlay(True)
+
+    @property
+    def variables(self):
+        return VariableManager.variables()
+
+    def select(self, item):
+        if item == self._selected:
             return
-        self._remove_empty()
-        bindings = getattr(widget, "_event_map_", {})
-        values = bindings.values()
-        self.bindings.clear()
-        self.bindings.add(*values)
-        if not values:
-            self._show_empty(self.NO_EVENT_MSG)
+        item.select()
+        if self._selected:
+            self._selected.deselect()
+        self._selected = item
+        self._detail_for(item)
 
-    def start_search(self, *_):
-        if self.studio.selected:
-            super().start_search()
+    def _show(self, item):
+        item.pack(side="top", fill="x")
 
-    def on_search_query(self, query: str):
-        showing = 0
-        self._remove_empty()
-        self.bindings.hide_all()
-        for item in self.bindings.items:
-            if query in item.value.sequence or query in item.value.handler:
-                item.show()
-                showing += 1
-        if not showing:
-            self._show_empty(self.NO_MATCH_MSG)
+    def _hide(self, item):
+        item.pack_forget()
 
-    def on_search_clear(self):
-        self._remove_empty()
-        self.bindings.hide_all()
-        for item in self.bindings.items:
-            item.show()
-        super().on_search_clear()
+    def _get_editor(self, variable):
+        editor_type = variable.definition["type"]
+        if not self._editors.get(editor_type):
+            # we do not have that type of editor yet, create it
+            self._editors[editor_type] = editors.get_editor(self._detail_pane.body, variable.definition)
+        return self._editors[editor_type]
+
+    def refresh(self):
+        # redraw variables for current context
+        self._variable_pane.body.clear_children()
+        has_selection = False
+        if not self.variables:
+            self._show_overlay(True)
+        else:
+            self._show_overlay(False)
+        for item in self.variables:
+            self._show(item)
+            if not has_selection:
+                self.select(item)
+                has_selection = True
+        # reapply search query if any
+        if self._search_query is not None:
+            self.on_search_query(self._search_query)
+
+    def _detail_for(self, variable):
+        _editor = self._get_editor(variable)
+        if self._editor != _editor:
+            # we need to change current editor completely
+            if self._editor:
+                self._editor.pack_forget()
+            self._editor = _editor
+        self._editor.set(variable.value)
+        self._editor.pack(side="top", fill="x")
+        self._editor.on_change(variable.set)
+
+        self.var_name.set(variable.name)
+        self.var_name.on_change(variable.set_name)
+        self.var_type_lbl["text"] = variable.var_type_name
+
+    def on_session_clear(self):
+        self.clear_variables()
+
+    def on_context_switch(self):
+        VariableManager.set_context(self.studio.context)
+        self.refresh()
```

### Comparing `formation-studio-0.6.3/studio/feature/stylepane.py` & `formation-studio-0.7.0/studio/feature/stylepane.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 """
 # ======================================================================= #
 # Copyright (C) 2019 Hoverset Group.                                      #
 # ======================================================================= #
 
 import logging
 from collections import defaultdict
+import tkinter as tk
+from tkinter import ttk
 
 from hoverset.ui.icons import get_icon_image
 from hoverset.ui.widgets import ScrolledFrame, Frame, Label, Button, TabView
 from hoverset.util.execution import Action
 from hoverset.platform import platform_is, LINUX
 from studio.feature._base import BaseFeature
 from studio.ui.editors import StyleItem, get_display_name, get_editor
 from studio.ui.widgets import CollapseFrame
-from studio.lib.pseudo import Container
+from studio.lib.pseudo import Container, PseudoWidget
 from studio.lib.layouts import GridLayoutStrategy
-from studio.preferences import Preferences, get_active_pref
+from studio.preferences import Preferences
+from studio.lib.properties import get_combined_properties, combine_properties
+from studio.i18n import _
 
 
 class ReusableStyleItem(StyleItem):
     _pool = defaultdict(dict)
     _editor_pool = set()
 
     def __init__(self, parent, style_definition, on_change=None):
@@ -96,28 +100,28 @@
     Main subdivision of the Style pane
     """
     handles_layout = False
     self_positioned = False
 
     def __init__(self, master, pane, **cnf):
         super().__init__(master)
+        self.pane_row = 0
         self.style_pane = pane
         self.configure(**{**self.style.surface, **cnf})
-        self._empty_message = "Select an item to see styles"
+        self._empty_message = _("Select an item to see styles")
         self._empty = Frame(self.body, **self.style.surface)
         self._empty_label = Label(self._empty, **self.style.text_passive,)
         self._empty_label.pack(fill="both", expand=True, pady=15)
-        self._widget = None
         self._prev_widget = None
         self._has_initialized = False  # Flag to mark whether Style Items have been created
         self.items = {}
 
     @property
-    def widget(self):
-        return self._widget
+    def widgets(self):
+        return self.style_pane.selection
 
     def can_optimize(self):
         return False
 
     def add(self, style_item):
         self.items[style_item.name] = style_item
         if self.style_pane._search_query is not None:
@@ -159,147 +163,165 @@
         self._empty.pack(fill="both", expand=True)
         text = self._empty_message if text is None else text
         self._empty_label["text"] = text
 
     def _remove_empty(self):
         self._empty.pack_forget()
 
-    def on_widget_change(self, widget):
-        self._widget = widget
-        if widget is None:
+    def on_widgets_change(self):
+        if not self.widgets:
             self.collapse()
             return
         definitions = self.get_definition()
         if self.can_optimize() and self.items:
             for prop in definitions:
                 self.items[prop]._re_purposed(definitions[prop])
         else:
             self.style_pane.show_loading()
             # this unmaps all style items returning them to the pool for reuse
             self.clear_children()
             # make all items held by group available for reuse
             ReusableStyleItem.free_all(self.items.values())
             self.items.clear()
             add = self.add
-            list(map(lambda p: add(ReusableStyleItem.acquire(self, definitions[p], self.apply), ), definitions))
+            list(map(lambda p: add(ReusableStyleItem.acquire(self, definitions[p], self.apply), ), sorted(definitions)))
             if not self.items:
                 self._show_empty()
             else:
                 self._remove_empty()
             # self.style_pane.body.scroll_to_start()
 
         self._has_initialized = True
-        self._prev_widget = widget
+        self._prev_widgets = self.widgets
 
-    def _apply_action(self, prop, value, widget, data):
-        self.apply(prop, value, widget, True)
+    def _apply_action(self, prop, value, widgets, data):
+        self.apply(prop, value, widgets, True)
 
     def _get_action_data(self, widget, prop):
         return {}
 
-    def _get_key(self, widget, prop):
-        return f"{widget}:{self.__class__.__name__}:{prop}"
+    def _get_key(self, widgets, prop):
+        return f"{'.'.join([w.id for w in widgets])}:{self.__class__.__name__}:{prop}"
 
-    def apply(self, prop, value, widget=None, silent=False):
-        is_external = widget is not None
-        widget = self.widget if widget is None else widget
-        if widget is None:
+    def apply(self, prop, value, widgets=None, silent=False):
+        is_external = widgets is not None
+        widgets = self.widgets if widgets is None else widgets
+        if not widgets:
             return
         try:
-            prev_val = self._get_prop(prop, widget)
-            data = self._get_action_data(widget, prop)
-            self._set_prop(prop, value, widget)
-            new_data = self._get_action_data(widget, prop)
-            self.style_pane.widget_modified(widget)
+            prev_val = [self._get_prop(prop, widget) for widget in widgets]
+            data = [self._get_action_data(widget, prop) for widget in widgets]
             if is_external:
-                if widget == self.widget:
+                list(map(lambda x: self._set_prop(prop, x[0], x[1]), zip(value, widgets)))
+            else:
+                [self._set_prop(prop, value, widget) for widget in widgets]
+            new_data = [self._get_action_data(widget, prop) for widget in widgets]
+            self.style_pane.widgets_modified(widgets)
+            if is_external:
+                if widgets == self.widgets:
                     self.items[prop].set_silently(value)
             if silent:
                 return
-            key = self._get_key(widget, prop)
+            key = self._get_key(widgets, prop)
             action = self.style_pane.last_action()
+
             if action is None or action.key != key:
                 self.style_pane.new_action(Action(
-                    lambda _: self._apply_action(prop, prev_val, widget, data),
-                    lambda _: self._apply_action(prop, value, widget, new_data),
+                    lambda _: self._apply_action(prop, prev_val, widgets, data),
+                    lambda _: self._apply_action(prop, [value for _ in widgets], widgets, new_data),
                     key=key,
                 ))
             else:
-                action.update_redo(lambda _: self._apply_action(prop, value, widget, new_data))
+                action.update_redo(lambda _: self._apply_action(prop, [value for _ in widgets], widgets, new_data))
         except Exception as e:
             # Empty string values are too common to be useful in logger debug
             if value != '':
                 logging.error(e)
                 logging.error(f"Could not set {self.__class__.__name__} {prop} as {value}", )
 
     def get_definition(self):
         return {}
 
-    def supports_widget(self, widget):
+    def supports_widgets(self):
         return True
 
     def on_search_query(self, query):
         item_found = False
         for item in self.items.values():
             if self._match_query(item.definition, query):
                 self._show(item)
                 item_found = True
             else:
                 self._hide(item)
         if not item_found:
-            self._show_empty("No items match your search")
+            self._show_empty(_("No items match your search"))
         else:
             self._remove_empty()
 
     def on_search_clear(self):
         # Calling search query with empty query ensures all items are displayed
         self.clear_children()
         self.on_search_query("")
 
 
 class IdentityGroup(StyleGroup):
 
     def __init__(self, master, pane, **cnf):
         super().__init__(master, pane, **cnf)
-        self.label = "Widget identity"
+        self.label = _("Widget identity")
 
     def get_definition(self):
-        if hasattr(self.widget, 'identity'):
-            return self.widget.identity
+        if not self.widgets:
+            return
+        if hasattr(self.widgets[0], 'identity'):
+            return self.widgets[0].identity
         return None
 
     def can_optimize(self):
         return self._has_initialized
 
+    def supports_widgets(self):
+        return len(self.widgets) == 1
+
 
 class AttributeGroup(StyleGroup):
 
     def __init__(self, master, pane, **cnf):
         super().__init__(master, pane, **cnf)
-        self.label = "Attributes"
+        self.label = _("Attributes")
+        self._prev_classes = set()
 
     def get_definition(self):
-        if hasattr(self.widget, 'properties'):
-            return self.widget.properties
+        if self.widgets and all(isinstance(widget, PseudoWidget) for widget in self.widgets):
+            return get_combined_properties(self.widgets)
         return {}
 
     def _get_action_data(self, widget, prop):
         if prop == "layout" and isinstance(widget, Container):
             return widget.get_all_info()
         super()._get_action_data(widget, prop)
 
-    def _apply_action(self, prop, value, widget, data):
-        self.apply(prop, value, widget, True)
-        if prop == "layout" and data and isinstance(widget, Container):
-            widget.config_all_widgets(data)
-            if self.widget in widget._children:
-                self.style_pane._layout_group.on_widget_change(self.widget)
+    def _apply_action(self, prop, value, widgets, data):
+        self.apply(prop, value, widgets, True)
+        if prop == "layout":
+            has_change = False
+            for widget, info in zip(widgets, data):
+                widget.config_all_widgets(info)
+                if any(w in widget._children for w in self.widgets):
+                    has_change = True
+
+            if has_change:
+                self.style_pane._layout_group.on_widgets_change()
 
     def can_optimize(self):
-        return self._widget.__class__ == self._prev_widget.__class__ and self._has_initialized
+        classes = set(w.__class__ for w in self.widgets)
+        if classes != self._prev_classes:
+            self._prev_classes = classes
+            return False
+        return True
 
 
 class ColumnConfig(StyleGroup):
 
     handles_layout = True
     self_positioned = True
 
@@ -308,84 +330,98 @@
         self.clear_children()
         self._label_frame.pack_forget()
         self._index = StyleItem(self, self._get_index_def())
         self._show(self._index)
 
     def _get_index_def(self):
         definition = dict(GridLayoutStrategy.COLUMN_DEF)
-        column = self.widget.grid_info()["column"] if self.is_grid(self.widget) else 0
-        definition["value"] = column
+        if self.widgets:
+            definition["value"] = self.widgets[0].grid_info()["column"]
+
+        for w in self.widgets:
+            if w.grid_info()["column"] != definition["value"]:
+                definition["value"] = ''
+                break
+
         return definition
 
     def _get_prop(self, prop, widget):
-        info = widget.layout.columnconfigure(widget.grid_info()["column"])
+        info = widget.layout.body.columnconfigure(widget.grid_info()["column"])
         return info.get(prop)
 
     def _set_prop(self, prop, value, widget):
         column = int(widget.grid_info()["column"])
-        widget.layout.columnconfigure(column, **{prop: value})
+        widget.layout.body.columnconfigure(column, **{prop: value})
         if not hasattr(widget.layout, "_column_conf"):
             widget.layout._column_conf = {column}
         else:
             widget.layout._column_conf.add(column)
 
     def is_grid(self, widget):
         if not widget:
             return False
         return widget.layout.layout_strategy.__class__ == GridLayoutStrategy
 
     def get_definition(self):
-        if not self.is_grid(self.widget):
+        if not self.widgets and self.is_grid(self.widgets[0]):
             return {}
-        return self.widget.layout.layout_strategy.get_column_def(self.widget)
+        return combine_properties([w.layout.layout_strategy.get_column_def(w) for w in self.widgets])
 
     def can_optimize(self):
         return self._has_initialized
 
     def clear_children(self):
         for child in self.items.values():
             self._hide(child)
 
     def _update_index(self):
-        self._index.set(self.widget.grid_info()["column"])
+        if self.widgets:
+            self._index.set(self.widgets[0].grid_info()["column"])
 
-    def on_widget_change(self, widget):
-        if self.is_grid(widget):
-            super().on_widget_change(widget)
+    def on_widgets_change(self):
+        if self.widgets and all(self.is_grid(widget) for widget in self.widgets):
+            super().on_widgets_change()
             self._index._editor.set_def(self._get_index_def())
             self._update_index()
 
 
 class RowConfig(ColumnConfig):
 
     def _get_index_def(self):
         definition = dict(GridLayoutStrategy.ROW_DEF)
-        row = self.widget.grid_info()["row"] if self.is_grid(self.widget) else 0
-        definition["value"] = row
+        if self.widgets:
+            definition["value"] = self.widgets[0].grid_info()["row"]
+
+        for w in self.widgets:
+            if w.grid_info()["row"] != definition["value"]:
+                definition["value"] = ''
+                break
+
         return definition
 
     def _get_prop(self, prop, widget):
-        info = widget.layout.rowconfigure(widget.grid_info()["row"])
+        info = widget.layout.body.rowconfigure(widget.grid_info()["row"])
         return info.get(prop)
 
     def _set_prop(self, prop, value, widget):
         row = int(widget.grid_info()["row"])
-        widget.layout.rowconfigure(row, **{prop: value})
+        widget.layout.body.rowconfigure(row, **{prop: value})
         if not hasattr(widget.layout, "_row_conf"):
             widget.layout._row_conf = {row}
         else:
             widget.layout._row_conf.add(row)
 
     def _update_index(self):
-        self._index.set(self.widget.grid_info()["row"])
+        if self.widgets:
+            self._index.set(self.widgets[0].grid_info()["column"])
 
     def get_definition(self):
-        if not self.is_grid(self.widget):
+        if not self.widgets and self.is_grid(self.widgets[0]):
             return {}
-        return self.widget.layout.layout_strategy.get_row_def(self.widget)
+        return combine_properties([w.layout.layout_strategy.get_row_def(w) for w in self.widgets])
 
 
 class GridConfig(Frame):
 
     def __init__(self, master, pane, **cnf):
         super().__init__(master)
         self._title = Label(self, **self.style.text_accent)
@@ -400,90 +436,178 @@
 
 class LayoutGroup(StyleGroup):
 
     handles_layout = True
 
     def __init__(self, master, pane, **cnf):
         super().__init__(master, pane, **cnf)
-        self.label = "Layout"
+        self.label = _("Layout")
         self._prev_layout = None
         self._grid_config = GridConfig(self.body, pane)
+        self._last_keys = set()
 
     def _get_prop(self, prop, widget):
         info = widget.layout.layout_strategy.info(widget)
         return info.get(prop)
 
     def _set_prop(self, prop, value, widget):
         widget.layout.apply(prop, value, widget)
 
-    def on_widget_change(self, widget):
-        super().on_widget_change(widget)
-        self._prev_layout = widget.layout.layout_strategy
-        if widget:
-            self.label = f"Layout ({widget.layout.layout_strategy.name})"
+    def on_widgets_change(self):
+        super().on_widgets_change()
+        layout_strategy = self.widgets[0].layout.layout_strategy if self.widgets else None
+        self._prev_layout = layout_strategy
+
+        if self.widgets:
+            self.label = _("Layout") + f"({self.widgets[0].layout.layout_strategy.name})"
         else:
-            self.label = "Layout"
+            self.label = _("Layout")
 
-        if widget.layout.layout_strategy.__class__ == GridLayoutStrategy:
+        if layout_strategy.__class__ == GridLayoutStrategy:
             self._show_grid_conf(True)
         else:
             self._show_grid_conf(False)
 
     def _show_grid_conf(self, flag):
         if flag:
             if not self._grid_config.winfo_ismapped():
                 self._grid_config.pack(side="bottom", fill="x", pady=1)
         else:
             self._grid_config.pack_forget()
 
     def can_optimize(self):
-        layout_strategy = self.widget.layout.layout_strategy
-        return layout_strategy.__class__ == self._prev_layout.__class__ \
-               and self._layout_equal(self.widget, self._prev_widget)
+        keys = set(self.get_definition().keys())
+        layout = self.widgets[0].layout.layout_strategy if self.widgets else None
+        if self._last_keys != keys or self._prev_layout != layout:
+            self._last_keys = keys
+            self._prev_layout = layout
+            return False
+        return True
 
     def get_definition(self):
-        if self.widget is not None:
-            return self.widget.layout.definition_for(self.widget)
+        if self.widgets:
+            return combine_properties([w.layout.definition_for(w) for w in self.widgets])
         return {}
 
     def _layout_equal(self, widget1, widget2):
         def1 = widget1.layout.layout_strategy.get_def(widget1)
         def2 = widget2.layout.layout_strategy.get_def(widget2)
         return def1 == def2
 
-    def supports_widget(self, widget):
+    def supports_widgets(self):
         # toplevel widgets do not need layout
-        return not widget.is_toplevel
+        if any(widget.is_toplevel for widget in self.widgets):
+            return False
+        if not self.widgets:
+            return False
+        strategy = self.widgets[0].layout.layout_strategy
+        # only support widgets with the same layout strategy
+        return all(widget.layout.layout_strategy == strategy for widget in self.widgets)
 
 
 class WindowGroup(StyleGroup):
     handles_layout = True
 
     def __init__(self, master, pane, **cnf):
         super().__init__(master, pane, **cnf)
-        self.label = "Window"
+        self.label = _("Window")
         self._prev_layout = None
-        self._grid_config = GridConfig(self.body, pane)
 
     def _get_prop(self, prop, widget):
         return widget.get_win_prop(prop)
 
     def _set_prop(self, prop, value, widget):
         widget.set_win_prop(prop, value)
 
     def can_optimize(self):
         return True
 
     def get_definition(self):
-        if self.widget is not None:
-            return self.widget.window_definition()
+        if self.widgets:
+            return combine_properties([widget.window_definition() for widget in self.widgets])
+        return {}
+
+    def supports_widgets(self):
+        return all(widget.is_toplevel for widget in self.widgets)
+
+
+class ScrollGroup(StyleGroup):
+    handles_layout = False
+
+    DEF = {
+        "yscroll": {
+            "name": "yscroll",
+            "display_name": "Y Scroll",
+            "type": "widget",
+            "include": [tk.Scrollbar, ttk.Scrollbar],
+        },
+        "xscroll": {
+            "name": "xscroll",
+            "display_name": "X Scroll",
+            "type": "widget",
+            "include": [tk.Scrollbar, ttk.Scrollbar],
+        },
+    }
+
+    def __init__(self, master, pane, **cnf):
+        super().__init__(master, pane, **cnf)
+        self.label = _("Scroll")
+        self._last_keys = None
+
+    def _get_prop(self, prop, widget):
+        if prop == "yscroll":
+            return getattr(widget, "_cnf_y_scroll", '')
+        if prop == "xscroll":
+            return getattr(widget, "_cnf_x_scroll", '')
+
+    def _set_prop(self, prop, value, widget):
+        if prop == "yscroll":
+            widget._cnf_y_scroll = value
+        if prop == "xscroll":
+            widget._cnf_x_scroll = value
+
+    def _keys(self, widget):
+        keys = []
+        widget_keys = widget.keys()
+        if 'yscrollcommand' in widget_keys:
+            keys.append('yscroll')
+        if 'xscrollcommand' in widget_keys:
+            keys.append('xscroll')
+        return tuple(keys)
+
+    def can_optimize(self):
+        keys = set()
+        for widget in self.widgets:
+            for k in self._keys(widget):
+                keys.add(k)
+        if keys != self._last_keys:
+            self._last_keys = keys
+            return False
+        return True
+
+    def _definition(self, widget):
+        keys = widget.keys()
+        props = {}
+        if 'yscrollcommand' in keys:
+            props['yscroll'] = dict(**self.DEF['yscroll'], value=getattr(widget, '_cnf_y_scroll', ''))
+        if 'xscrollcommand' in keys:
+            props['xscroll'] = dict(**self.DEF['xscroll'], value=getattr(widget, '_cnf_x_scroll', ''))
+        return props
+
+    def get_definition(self):
+        if self.widgets:
+            return combine_properties([self._definition(widget) for widget in self.widgets])
         return {}
 
-    def supports_widget(self, widget):
-        return widget.is_toplevel
+    def _support(self, widget):
+        keys = widget.keys()
+        return any(x in keys for x in ('yscrollcommand', 'xscrollcommand'))
+
+    def supports_widgets(self):
+        return all(self._support(w) for w in self.widgets)
 
 
 class StylePaneFramework:
 
     def setup_style_pane(self):
         self.body = ScrolledFrame(self, **self.style.surface)
         self.body.pack(side="top", fill="both", expand=True)
@@ -499,131 +623,151 @@
         self._search_btn.pack(side="right")
         self._search_btn.on_click(self.start_search)
 
         self.groups = []
 
         self._empty_frame = Frame(self.body)
         self.show_empty()
-        self._current = None
+        self._selection = []
         self._expanded = False
         self._is_loading = False
         self._search_query = None
+        self._current_row = 0
+
+        self.body.body.columnconfigure(0, weight=1)
 
     def get_header(self):
         raise NotImplementedError()
 
     @property
-    def supported_groups(self):
-        return [group for group in self.groups if group.supports_widget(self._current)]
+    def selection(self):
+        return self._selection
+
+    @property
+    def widgets(self):
+        return self._selection
 
     def create_menu(self):
         return (
-            ("command", "Search", get_icon_image("search", 14, 14), self.start_search, {}),
-            ("command", "Expand all", get_icon_image("chevron_down", 14, 14), self.expand_all, {}),
-            ("command", "Collapse all", get_icon_image("chevron_up", 14, 14), self.collapse_all, {})
+            ("command", _("Search"), get_icon_image("search", 18, 18), self.start_search, {}),
+            ("command", _("Expand all"), get_icon_image("chevron_down", 18, 18), self.expand_all, {}),
+            ("command", _("Collapse all"), get_icon_image("chevron_up", 18, 18), self.collapse_all, {})
         )
 
-    def extern_apply(self, group_class, prop, value, widget=None, silent=False):
+    def extern_apply(self, group_class, prop, value, widgets=None, silent=False):
         for group in self.groups:
             if group.__class__ == group_class:
-                group.apply(prop, value, widget, silent)
+                group.apply(prop, value, widgets, silent)
                 return
         raise ValueError(f"Class {group_class.__class__.__name__} not found")
 
     def last_action(self):
         raise NotImplementedError()
 
     def new_action(self, action):
         raise NotImplementedError()
 
-    def widget_modified(self, widget):
+    def widgets_modified(self, widgets):
         raise NotImplementedError()
 
     def add_group(self, group_class, **kwargs) -> StyleGroup:
         if not issubclass(group_class, StyleGroup):
             raise ValueError('type required.')
         group = group_class(self.body.body, self, **kwargs)
+        group.pane_row = self._current_row
+        self._current_row += 1
         self.groups.append(group)
         self.show_group(group)
         return group
 
     def add_group_instance(self, group_instance, show=False):
         if not isinstance(group_instance, StyleGroup):
             raise ValueError('Expected object of type StyleGroup.')
+        group_instance.pane_row = self._current_row
+        self._current_row += 1
         self.groups.append(group_instance)
         if show:
             self.show_group(group_instance)
 
     def hide_group(self, group):
         if group.self_positioned:
             group._hide_group()
             return
-        group.pack_forget()
+        if not group.winfo_ismapped():
+            return
+        group.grid_forget()
 
     def show_group(self, group):
         if group.self_positioned:
             group._show_group()
             return
-        group.pack(side='top', fill='x', pady=12)
+        if group.winfo_ismapped():
+            return
+        group.grid(row=group.pane_row, column=0, sticky="nsew", pady=12)
 
     def show_empty(self):
         self.remove_empty()
         self._empty_frame.place(x=0, y=0, relheight=1, relwidth=1)
-        Label(self._empty_frame, text="You have not selected any item",
+        Label(self._empty_frame, text=_("You have not selected any item"),
               **self.style.text_passive).place(x=0, y=0, relheight=1, relwidth=1)
 
     def remove_empty(self):
         self._empty_frame.clear_children()
         self._empty_frame.place_forget()
 
     def show_loading(self):
         if platform_is(LINUX) or self._is_loading:
             # render transitions in linux are very fast and glitch free
             # for other platforms or at least for windows we need to hide the glitching
             return
         self.remove_empty()
         self._empty_frame.place(x=0, y=0, relheight=1, relwidth=1)
-        Label(self._empty_frame, text="Loading...",
+        Label(self._empty_frame, text=_("Loading..."),
               **self.style.text_passive).place(x=0, y=0, relheight=1, relwidth=1)
         self._is_loading = True
 
     def remove_loading(self):
         self.remove_empty()
         self._is_loading = False
 
-    def styles_for(self, widget):
-        self._current = widget
-        if widget is None:
+    def render_styles(self):
+        if not self.widgets:
             self.show_empty()
             return
+
         for group in self.groups:
-            if group.supports_widget(widget):
+            if group.supports_widgets():
                 self.show_group(group)
-                group.on_widget_change(widget)
+                group.on_widgets_change()
             else:
                 self.hide_group(group)
         self.remove_loading()
         self.body.update_idletasks()
 
-    def layout_for(self, widget):
+    def render_layouts(self):
         for group in self.groups:
-            if group.handles_layout and group.supports_widget(widget):
-                group.on_widget_change(widget)
+            if group.handles_layout and group.supports_widgets():
+                group.on_widgets_change()
         self.remove_loading()
 
-    def on_select(self, widget):
-        self.styles_for(widget)
+    def _select(self, _, selection=None):
+        selection = list(selection if selection is not None else self.studio.selection)
 
-    def on_widget_change(self, old_widget, new_widget=None):
-        if new_widget is None:
-            new_widget = old_widget
-        self.styles_for(new_widget)
+        if selection == self._selection:
+            return
+        self._selection = selection
+        self.render_styles()
 
-    def on_widget_layout_change(self, widget):
-        self.layout_for(widget)
+    def on_widgets_change(self, widgets):
+        if any(w in self.widgets for w in widgets):
+            self.render_styles()
+
+    def on_widgets_layout_change(self, widgets):
+        if any(w in self.widgets for w in widgets):
+            self.render_layouts()
 
     def expand_all(self):
         for group in self.groups:
             group.expand()
         self._expanded = True
         self._toggle_btn.config(image=get_icon_image("chevron_up", 15, 15))
 
@@ -644,15 +788,15 @@
             self.collapse_all()
 
     def __update_frames(self):
         for group in self.groups:
             group.update_state()
 
     def start_search(self, *_):
-        if self._current:
+        if self._selection:
             super().start_search()
             self.body.scroll_to_start()
 
     def on_search_query(self, query):
         for group in self.groups:
             group.on_search_query(query)
         self.__update_frames()
@@ -665,45 +809,49 @@
         # The search bar is being closed and we need to bring everything back
         super().on_search_clear()
         self._search_query = None
 
 
 class StylePane(StylePaneFramework, BaseFeature):
     name = "Style pane"
+    display_name = _("Style pane")
     icon = "edit"
     _defaults = {
         **BaseFeature._defaults,
         "side": "right",
     }
 
     def __init__(self, master, studio, **cnf):
         super().__init__(master, studio, **cnf)
         self.setup_style_pane()
 
         pref: Preferences = Preferences.acquire()
-        pref.add_listener("designer::descriptive_names", lambda _: self.styles_for(self._current))
+        pref.add_listener("designer::descriptive_names", lambda _: [self.render_styles(), self.render_layouts()])
 
         self._identity_group = self.add_group(IdentityGroup)
         self._layout_group = self.add_group(LayoutGroup)
         self._attribute_group = self.add_group(AttributeGroup)
         self.add_group(WindowGroup)
+        self.add_group(ScrollGroup)
 
         self.add_group_instance(self._layout_group._grid_config.column_config)
         self.add_group_instance(self._layout_group._grid_config.row_config)
 
-    def apply_style(self, prop, value, widget=None, silent=False):
-        self._attribute_group.apply(prop, value, widget, silent)
+        self.studio.bind("<<SelectionChanged>>", self._select, add='+')
+
+    def apply_style(self, prop, value, widgets=None, silent=False):
+        self._attribute_group.apply(prop, value, widgets, silent)
 
-    def apply_layout(self, prop, value, widget=None, silent=False):
-        self._layout_group.apply(prop, value, widget, silent)
+    def apply_layout(self, prop, value, widgets=None, silent=False):
+        self._layout_group.apply(prop, value, widgets, silent)
 
     def get_header(self):
         return self._header
 
     def last_action(self):
         return self.studio.last_action()
 
     def new_action(self, action):
         self.studio.new_action(action)
 
-    def widget_modified(self, widget):
-        self.studio.widget_modified(widget, self, None)
+    def widgets_modified(self, widgets):
+        self.studio.widgets_modified(widgets, self)
```

### Comparing `formation-studio-0.6.3/studio/lib/__init__.py` & `formation-studio-0.7.0/studio/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/lib/canvas.py` & `formation-studio-0.7.0/studio/lib/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,26 +423,26 @@
         super(Bitmap, self).__init__(canvas, x, y, **options)
 
     def _create(self, *args, **options):
         return self.canvas.create_bitmap(*args, **options)
 
 
 class Image(CanvasItem):
-    icon = "image_dark"
+    icon = "image"
     display_name = "Image"
 
     def __init__(self, canvas, x, y, **options):
         super(Image, self).__init__(canvas, x, y, **options)
 
     def _create(self, *args, **options):
         return self.canvas.create_image(*args, **options)
 
 
 class Line(CanvasItem):
-    icon = "line"
+    icon = "polyline"
     display_name = "Line"
     defaults = dict(width=2)
 
     def __init__(self, canvas, x0, y0, x1, y1, *args, **options):
         super(Line, self).__init__(canvas, x0, y0, x1, y1, *args, **options)
 
     def _create(self, *args, **options):
```

### Comparing `formation-studio-0.6.3/studio/lib/layouts.py` & `formation-studio-0.7.0/studio/lib/layouts.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Layout classes uses in the studio
 """
 
 # ======================================================================= #
 # Copyright (C) 2019 Hoverset Group.                                      #
 # ======================================================================= #
 from collections import defaultdict
+from copy import deepcopy
+import tkinter as tk
 
 from studio.ui import geometry
 from studio.ui.highlight import WidgetHighlighter, EdgeIndicator
 
 COMMON_DEFINITION = {
     "ipadx": {
         "display_name": "internal padding x",
@@ -52,82 +54,94 @@
         },
     }
     name = "base"  # A default name just in case
     icon = "frame"
     manager = "place"  # Default layout manager in use
     realtime_support = False  # dictates whether strategy supports realtime updates to its values, most do not
     dimensions_in_px = False  # Whether to use pixel units for width and height
+    allow_resize = False  # Whether to allow resizing of widgets
+    stacking_support = True  # Whether to allow modification of stacking order
 
     def __init__(self, container):
         self.parent = container.parent
         self.container = container
 
     @property
     def level(self):
         return self.container.level
 
     @property
     def children(self):
         return self.container._children
 
-    @property
-    def temporal_children(self):
-        return self.container.temporal_children
-
     def bounds(self):
         return geometry.bounds(self.container)
 
     def add_widget(self, widget, bounds=None, **kwargs):
         widget.level = self.level + 1
         widget.layout = self.container
-        try:
-            widget.lift(self.container.body)
-        except Exception:
-            pass
         self.container.clear_highlight()
 
+    def _insert(self, widget, index=None):
+        if index is None:
+            self.children.append(widget)
+        else:
+            self.children.insert(index, widget)
+
+        self._update_stacking()
+
+        if widget.prev_stack_index is None:
+            widget.prev_stack_index = len(self.children) - 1
+
+    def _update_stacking(self):
+        for index, widget in enumerate(self.children):
+            if index > 0:
+                widget.lift(self.children[index - 1])
+            else:
+                widget.lift(self.container.body)
+
     def widget_released(self, widget):
         pass
 
-    def change_start(self, widget):
+    def start_move(self, widget):
         widget.recent_layout_info = self.get_restore(widget)
+        widget.lift()
+        widget.lift_handle()
 
-    def move_widget(self, widget, bounds):
-        if widget in self.children:
-            self.remove_widget(widget)
-        if widget not in self.temporal_children:
-            self.temporal_children.append(widget)
-            widget.level = self.level + 1
-            widget.layout = self.container
-            # Lift widget above the last child of layout if any otherwise lift above the layout
-            try:
-                widget.lift((self.children[-1:] or [self.container.body])[0])
-            except Exception:
-                pass
-        self._move(widget, bounds)
+    def start_resize(self, widget):
+        widget.recent_layout_info = self.get_restore(widget)
 
-    def _move(self, widget, bounds):
-        # Make the bounds relative to the layout for proper positioning
-        bounds = geometry.relative_bounds(bounds, self.container.body)
+    def move_widget(self, widget, delta):
+        bounds = geometry.relative_bounds(self.bounds_from_delta(widget, delta), self.container.body)
         self.container.position(widget, bounds)
 
-    def resize_widget(self, widget, bounds):
-        self._move(widget, bounds)
+    def end_move(self, widget):
+        pass
+
+    def on_move_exit(self):
+        pass
+
+    def bounds_from_delta(self, widget, delta):
+        # Make the bounds relative to the layout for proper positioning
+        x1, y1, x2, y2 = widget.get_bounds()
+        dx, dy = delta
+        return [x1 + dx, y1 + dy, x2 + dx, y2 + dy]
+
+    def resize_widget(self, widget, direction, delta):
+        raise NotImplementedError("Layout should provide resize method")
 
     def restore_widget(self, widget, data=None):
         raise NotImplementedError("Layout should provide restoration method")
 
     def get_restore(self, widget):
         raise NotImplementedError("Layout should provide restoration data")
 
     def remove_widget(self, widget):
         if widget in self.children:
             self.children.remove(widget)
-        if widget in self.temporal_children:
-            self.temporal_children.remove(widget)
 
     def add_new(self, widget, x, y):
         self.parent.add(widget, x, y, layout=self.container)
 
     def apply(self, prop, value, widget):
         pass
 
@@ -145,16 +159,16 @@
     def config_widget(self, widget, config):
         raise NotImplementedError("Layout should provide configuration method")
 
     def get_def(self, widget):
         # May be overridden to return dynamic definitions based on the widget
         # Always use a copy to avoid messing with definition
         if self.dimensions_in_px:
-            return dict(self.DEFINITION)
-        props = dict(self.DEFINITION)
+            return deepcopy(self.DEFINITION)
+        props = deepcopy(self.DEFINITION)
         overrides = getattr(widget, 'DEF_OVERRIDES', {})
         for key in ('width', 'height'):
             if key in props and key in overrides:
                 props[key] = {**props[key], **overrides[key]}
         return props
 
     def definition_for(self, widget):
@@ -170,15 +184,15 @@
         # create a list of children and their bounds which won't change during iteration
         bounding_map = [(child, geometry.bounds(child)) for child in self.children]
         if former_strategy:
             former_strategy.clear_all()
         for child, bounds in bounding_map:
             self.add_widget(child, bounds)
 
-    def react_to_pos(self, x, y):
+    def react_to_pos(self, bounds):
         pass
 
     def copy_layout(self, widget, from_):
         pass
 
     def clear_indicators(self):
         pass
@@ -219,45 +233,116 @@
         },
         "bordermode": {
             "display_name": "border mode",
             "type": "choice",
             "options": ("outside", "inside", "ignore"),
             "name": "bordermode",
             "default": "inside",
-        }
+        },
+        "relx": {
+            "display_name": "relative x",
+            "type": "float",
+            "name": "relx",
+            "default": "0"
+        },
+        "rely": {
+            "display_name": "relative y",
+            "type": "float",
+            "name": "rely",
+            "default": "0"
+        },
+        "relwidth": {
+            "display_name": "relative width",
+            "type": "float",
+            "name": "relwidth",
+            "default": ""
+        },
+        "relheight": {
+            "display_name": "relative height",
+            "type": "float",
+            "name": "relheight",
+            "default": ""
+        },
     }
     name = "place"
-    icon = "frame"
+    icon = "place"
     manager = "place"
     realtime_support = True
     dimensions_in_px = True
+    allow_resize = True
 
     def clear_all(self):
         for child in self.children:
             child.place_forget()
 
     def add_widget(self, widget, bounds=None, **kwargs):
         super().add_widget(widget, bounds)
         super().remove_widget(widget)
         if bounds:
-            self.move_widget(widget, bounds)
+            bounds = geometry.relative_bounds(bounds, self.container.body)
+            self.container.position(widget, bounds)
         kwargs['in'] = self.container.body
         widget.place_configure(**kwargs)
-        self.children.append(widget)
+        self._insert(widget, widget.prev_stack_index if widget.layout == self.container else None)
+
+    def _info_with_delta(self, widget, direction, delta):
+        info = self.info(widget)
+        info.update(x=int(info["x"]), y=int(info["y"]), width=int(info["width"]), height=int(info["height"]))
+        dx, dy = delta
+        if direction == "n":
+            info.update(y=info["y"] + dy, height=info["height"] - dy)
+        elif direction == "s":
+            info["height"] = info["height"] + dy
+        elif direction == "e":
+            info["width"] = info["width"] + dx
+        elif direction == "w":
+            info.update(x=info["x"] + dx, width=info["width"] - dx)
+        elif direction == "nw":
+            info.update(x=info["x"] + dx, y=info["y"] + dy, width=info["width"] - dx, height=info["height"] - dy)
+        elif direction == "ne":
+            info.update(y=info["y"] + dy, width=info["width"] + dx, height=info["height"] - dy)
+        elif direction == "sw":
+            info.update(x=info["x"] + dx, width=info["width"] - dx, height=info["height"] + dy)
+        elif direction == "se":
+            info.update(width=info["width"] + dx, height=info["height"] + dy)
+        elif direction == "all":
+            info.update(x=info["x"] + dx, y=info["y"] + dy)
+        return info
+
+    def resize_widget(self, widget, direction, delta):
+        info = self._info_with_delta(widget, direction, delta)
+        widget.place_configure(**info)
+
+    def end_move(self, widget):
+        super().end_move(widget)
+        self._update_stacking()
+
+    def move_widget(self, widget, delta):
+        info = widget.place_info() or {}
+        ref = info.get("in")
+
+        if ref != self.container.body:
+            bounds = geometry.relative_bounds(self.bounds_from_delta(widget, delta), self.container.body)
+            self.container.position(widget, bounds)
+            return
+
+        info = self._info_with_delta(widget, "all", delta)
+        widget.place_configure(**info)
 
     def remove_widget(self, widget):
         super().remove_widget(widget)
         widget.place_forget()
 
     def config_widget(self, widget, config):
         widget.place_configure(**config)
 
     def restore_widget(self, widget, data=None):
         data = widget.recent_layout_info if data is None else data
-        self.children.append(widget)
+        self._insert(widget, widget.prev_stack_index if widget.layout == self.container else None)
+
         widget.layout = self.container
         widget.level = self.level + 1
         widget.place_configure(**data.get("info", {}))
 
     def get_restore(self, widget):
         return {
             "info": widget.place_info(),
@@ -271,15 +356,15 @@
         info = widget.place_info() or {}
         return info
 
     def copy_layout(self, widget, from_):
         info = from_.place_info()
         info["in_"] = self.container.body
         widget.place(**info)
-        self.children.append(widget)
+        self._insert(widget)
         super().add_widget(widget, (0, 0, 0, 0))
 
 
 class PackLayoutStrategy(BaseLayoutStrategy):
     DEFINITION = {
         **BaseLayoutStrategy.DEFINITION,
         **COMMON_DEFINITION,
@@ -308,71 +393,74 @@
             "type": "choice",
             "options": ("top", "bottom", "right", "left"),
             "name": "side",
             "default": "top"
         },
     }
     name = "pack"
-    icon = "frame"
+    icon = "pack"
     manager = "pack"
+    stacking_support = False
 
     def __init__(self, container):
         super().__init__(container)
         self._orientation = self.HORIZONTAL
         self.temp_info = {}
-        # Store for info on temporarily removed widgets to allow restoration
-        self._restoration_data = {}
 
     def add_widget(self, widget, bounds=None, **kwargs):
         super().remove_widget(widget)
         super().add_widget(widget, bounds, **kwargs)
         if self._orientation == self.HORIZONTAL:
             widget.pack(in_=self.container.body)
         elif self._orientation == self.VERTICAL:
             widget.pack(in_=self.container.body, side="left")
         self.config_widget(widget, kwargs)
-        self.children.append(widget)
+        self._insert(widget)
 
     def redraw(self):
         for widget in self.children:
             widget.pack(**self._pack_info(widget))
 
     def _redraw(self, start_index=0):
         affected = self.children[start_index:]
         cache = {}
         for child in affected:
             cache[child] = self._pack_info(child)
             child.pack_forget()
         for child in affected:
             child.pack(**cache.get(child, {}))
 
-    def resize_widget(self, widget, bounds):
-        if not self.temp_info:
-            self.temp_info = self._pack_info(widget)
-        self._move(widget, bounds)
+    def resize_widget(self, widget, direction, delta):
+        pass
 
     def _pack_info(self, widget):
         try:
             return widget.pack_info()
         except Exception:
             return self.temp_info or {"in_": self.container.body}
 
     def widget_released(self, widget):
         self.redraw()
         self.temp_info = None
 
     def remove_widget(self, widget):
-        self._restoration_data[widget] = self.get_restore(widget)
         super().remove_widget(widget)
         widget.pack_forget()
 
+    def end_move(self, widget):
+        super().end_move(widget)
+        widget.pack(in_=self.container.body)
+        self.config_widget(widget, widget.recent_layout_info.get("info", {}))
+        self._update_stacking()
+        self._redraw()
+
     def restore_widget(self, widget, data=None):
         # We need to be able to return a removed widget back to its initial position once removed
         restoration_data = widget.recent_layout_info if data is None else data
-        self.children.insert(restoration_data.get("index", -1), widget)
+        self._insert(widget, restoration_data.get("index", -1))
         widget.level = self.level + 1
         widget.layout = self.container
         widget.pack(in_=self.container.body)
         self.config_widget(widget, restoration_data.get("info", {}))
         self._redraw()
 
     def get_restore(self, widget):
@@ -424,15 +512,15 @@
                 info.update({prop: widget[prop]})
         return info
 
     def copy_layout(self, widget, from_):
         info = from_.pack_info()
         info["in_"] = self.container.body
         widget.pack(**info)
-        self.children.append(widget)
+        self._insert(widget)
         super().add_widget(widget, (0, 0, 0, 0))
 
     def clear_all(self):
         for child in self.children:
             child.pack_forget()
 
 
@@ -469,15 +557,15 @@
             return last.winfo_y() - self.container.body.winfo_y() + last.winfo_height()
         return 0
 
     def add_widget(self, widget, bounds=None, **kwargs):
         super().add_widget(widget, bounds, **kwargs)
         width, height = geometry.dimensions(bounds)
         self.attach(widget, width, height)
-        self.children.append(widget)
+        self._insert(widget)
 
     def attach(self, widget, width, height):
         y = self.get_last()
         widget.place(in_=self.container.body, x=0, y=y, width=width, height=height, bordermode="outside")
 
     def redraw(self, widget):
         from_ = self._children.index(widget)
@@ -485,32 +573,31 @@
         self._children = self._children[:from_]
         dimensions = {}
         for child in temp:
             dimensions[child] = [child.winfo_width(), child.winfo_height()]
             child.place_forget()
         for child in temp:
             self.attach(child, *dimensions[child])
-            self._children.append(child)
+            self._insert(child)
 
-    def resize_widget(self, widget, bounds):
-        super().resize_widget(widget, bounds)
+    def resize_widget(self, widget, direction, delta):
         widget.update_idletasks()
         self.redraw(widget)
 
     def remove_widget(self, widget):
         from_ = self._children.index(widget)
         dimensions = {}
         for child in self._children[from_:]:
             dimensions[child] = [child.winfo_width(), child.winfo_height()]
             child.place_forget()
         temp = self._children[from_ + 1:]
         self._children = self._children[:from_]
         for child in temp:
             self.attach(child, *dimensions[child])
-            self._children.append(child)
+            self._insert(child)
 
     def clear_children(self):
         for child in self.children:
             child.place_forget()
 
 
 class VerticalLinearLayout(PackLayoutStrategy):
@@ -614,20 +701,27 @@
         return {
             "info": widget.grid_info(),
             "container": self.container,
         }
 
     def restore_widget(self, widget, data=None):
         data = widget.recent_layout_info if data is None else data
-        self.children.append(widget)
+        self._insert(widget, widget.prev_stack_index if widget.layout == self.container else None)
         widget.level = self.level + 1
         widget.layout = self.container
         widget.grid(in_=self.container.body)
         self.config_widget(widget, data.get("info", {}))
 
+    def end_move(self, widget):
+        super().end_move(widget)
+        kw = widget.recent_layout_info.get("info", {})
+        self._grid_at_bounds(widget, widget.get_bounds(), **kw)
+        self._update_stacking()
+        self.clear_indicators()
+
     def react_to(self, bounds):
         bounds = geometry.relative_bounds(bounds, self.container.body)
         col, row = self.container.body.grid_location(bounds[0], bounds[1])
         widget = self.container.body.grid_slaves(row, col)
         if widget:
             self._highlighter.highlight(widget[0])
 
@@ -684,54 +778,63 @@
         widget.grid_configure(**config)
 
     def widget_released(self, widget):
         self._redraw_widget(widget)
         self._temp = None
         self.clear_indicators()
 
-    def resize_widget(self, widget, bounds):
-        if not self._temp:
-            self._temp = self._grid_info(widget)
-        self._move(widget, bounds)
+    def resize_widget(self, widget, direction, delta):
+        pass
 
-    def _move(self, widget, bounds):
-        super()._move(widget, bounds)
-        self._location_analysis(bounds)
+    def move_widget(self, widget, delta):
+        super().move_widget(widget, delta)
+        self._location_analysis(self.bounds_from_delta(widget, delta))
+
+    def on_move_exit(self):
+        super().on_move_exit()
+        self.clear_indicators()
 
     def add_widget(self, widget, bounds=None, **kwargs):
         super().remove_widget(widget)
         super().add_widget(widget, bounds, **kwargs)
         if bounds is not None:
-            row, col, row_shift, column_shift = self._location_analysis(bounds)
-            self._redraw(max(0, row), max(0, col), row_shift, column_shift)
-            kwargs.update({'in_': self.container.body, 'row': max(0, row), 'column': max(0, col)})
-            widget.grid(**kwargs)
+            self._grid_at_bounds(widget, bounds, **kwargs)
         else:
             widget.grid(in_=self.container.body)
             self.config_widget(widget, kwargs)
-        self.children.append(widget)
+        self._insert(widget, widget.prev_stack_index if widget.layout == self.container else None)
         self.clear_indicators()
 
+    def _grid_at_bounds(self, widget, bounds, **kwargs):
+        row, col, row_shift, column_shift = self._location_analysis(bounds)
+        self._redraw(max(0, row), max(0, col), row_shift, column_shift)
+        kwargs.update({'in_': self.container.body, 'row': max(0, row), 'column': max(0, col)})
+        widget.grid(**kwargs)
+
     def _widget_at(self, row, column):
         return self.container.body.grid_slaves(column, row)
 
     def _location_analysis(self, bounds):
         self.clear_indicators()
         self._edge_indicator.update_idletasks()
         bounds = geometry.relative_bounds(bounds, self.container.body)
         x, y = bounds[0], bounds[1]
+        w, h = geometry.dimensions(bounds)
         col, row = self.container.body.grid_location(x, y)
         x, y = geometry.upscale_bounds(bounds, self.container.body)[:2]
         slaves = self.container.body.grid_slaves(max(0, row), max(0, col))
         if len(slaves) == 0:
             self.container.body.update_idletasks()
             bbox = self.container.body.grid_bbox(col, row)
             bounds = *bbox[:2], bbox[0] + bbox[2], bbox[1] + bbox[3]
             # Make bounds relative to designer
             bounds = geometry.upscale_bounds(bounds, self.container.body)
+            if geometry.dimensions(bounds) == (0, 0):
+                w, h = w or 50, h or 25
+                bounds = bounds[0], bounds[1], bounds[0] + w, bounds[1] + h
         else:
             bounds = geometry.bounds(slaves[0])
         y_offset, x_offset = 10, 10  # 0.15*(bounds[3] - bounds[1]), 0.15*(bounds[2] - bounds[0])
         # If the position is empty no need to alter the row or column
         resize = 1 if slaves else 0
         if y - bounds[1] < y_offset:
             self._edge_indicator.top(bounds)
@@ -754,16 +857,17 @@
 
     def apply(self, prop, value, widget):
         if prop in ("width", "height"):
             widget.configure(**{prop: value})
         else:
             widget.grid_configure(**{prop: value})
 
-    def react_to_pos(self, x, y):
-        self._location_analysis((*geometry.resolve_position((x, y), self.container.parent), 0, 0))
+    def react_to_pos(self, bounds):
+        bounds = geometry.resolve_bounds(bounds, self.container.parent)
+        self._location_analysis(bounds)
 
     def info(self, widget):
         info = widget.grid_info() or {}
         keys = widget.keys()
         for prop in ("width", "height"):
             if prop in keys:
                 info.update({prop: widget[prop]})
@@ -791,28 +895,25 @@
             definition[key]["value"] = column_info[key]
         return definition
 
     def copy_layout(self, widget, from_):
         info = from_.grid_info()
         info["in_"] = self.container.body
         widget.grid(**info)
-        self.children.append(widget)
+        self._insert(widget)
         super().add_widget(widget, (0, 0, 0, 0))
 
     def clear_all(self):
         # remove the children but still maintain them in the children list
         for child in self.children:
             child.grid_forget()
 
 
 class TabLayoutStrategy(BaseLayoutStrategy):
     # TODO Extend support for side specific padding
-    name = "TabLayout"
-    icon = "notebook"
-    manager = "tab"
     DEFINITION = {
         "text": {
             "display_name": "tab text",
             "type": "text",
             "name": "text",
             "default": None
         },
@@ -852,26 +953,35 @@
             "display_name": "state",
             "name": "state",
             "type": "choice",
             "options": ("normal", "disabled", "hidden"),
             "default": 'normal'
         }
     }
+    name = "TabLayout"
+    icon = "notebook"
+    manager = "tab"
+    stacking_support = False
 
     def __init__(self, master):
         super().__init__(master)
         self._current_tab = None
         self.container.body.bind("<<NotebookTabChanged>>", self._tab_switched)
 
     def config_widget(self, widget, config):
         self.container.body.tab(widget, **config)
 
+    def end_move(self, widget):
+        self.container.body.add(widget)
+        self.container.body.tab(widget, **widget.recent_layout_info.get("info", {}))
+        self._redraw(widget.recent_layout_info.get("index", -1))
+
     def restore_widget(self, widget, data=None):
         restoration_data = widget.recent_layout_info if data is None else data
-        self.children.insert(restoration_data.get("index", -1), widget)
+        self._insert(widget, restoration_data.get("index", -1))
         widget.level = self.level + 1
         widget.layout = self.container
         self.container.body.add(widget)
         self.container.body.tab(widget, **restoration_data.get("info", {}))
         self._redraw(restoration_data.get("index", -1))
 
     def get_restore(self, widget):
@@ -887,27 +997,30 @@
         for child in affected:
             cache[child] = self.info(child)
             self.container.body.forget(child)
         for child in affected:
             self.container.body.add(child)
             self.container.body.tab(child, **cache.get(child, {}))
 
-    def resize_widget(self, widget, bounds):
+    def resize_widget(self, widget, direction, delta):
         pass
 
     def add_widget(self, widget, bounds=None, **kwargs):
         super().remove_widget(widget)
         super().add_widget(widget, bounds, **kwargs)
         self.container.body.add(widget, text=widget.id)
         self.container.body.tab(widget, **kwargs)
-        self.children.append(widget)
+        self._insert(widget)
 
     def remove_widget(self, widget):
         super().remove_widget(widget)
-        self.container.body.forget(widget)
+        try:
+            self.container.body.forget(widget)
+        except tk.TclError:
+            pass
 
     def info(self, widget):
         info = self.container.body.tab(widget) or {}
         if "padding" in info:
             # use the first padding value until we can support full padding
             info["padding"] = info["padding"][0]
         info["compound"] = info.get("compound", "") or "none"
@@ -930,17 +1043,14 @@
 
     def clear_all(self):
         # No implementation needed as the tab layout strategy never needs to change
         pass
 
 
 class PanedLayoutStrategy(BaseLayoutStrategy):
-    name = "PanedLayout"
-    icon = "flip_horizontal"
-    manager = "pane"
     DEFINITION = {
         **BaseLayoutStrategy.DEFINITION,  # width and height definition
         "padx": COMMON_DEFINITION.get("padx"),
         "pady": COMMON_DEFINITION.get("pady"),
         "sticky": {
             "display_name": "sticky",
             "type": "anchor",
@@ -964,28 +1074,37 @@
         "minsize": {
             "display_name": "minsize",
             "type": "dimension",
             "default": 0,
             "name": "minsize",
         }
     }
+    name = "PanedLayout"
+    icon = "flip_horizontal"
+    manager = "pane"
+    stacking_support = False
 
     def get_restore(self, widget):
         return {
             "info": self.info(widget),
             "index": self.children.index(widget),
             "container": self.container
         }
 
     def config_widget(self, widget, config):
         self._config(widget, **config)
 
+    def end_move(self, widget):
+        self.container.body.add(widget)
+        self._config(widget, **widget.recent_layout_info.get("info", {}))
+        self._redraw(widget.recent_layout_info.get("index", -1))
+
     def restore_widget(self, widget, data=None):
         restoration_data = widget.recent_layout_info if data is None else data
-        self.children.insert(restoration_data.get("index", -1), widget)
+        self._insert(widget, restoration_data.get("index", -1))
         widget.level = self.level + 1
         widget.layout = self.container
         self.container.body.add(widget)
         self._config(widget, **restoration_data.get("info", {}))
         self._redraw(restoration_data.get("index", -1))
 
     def _redraw(self, start_index=0):
@@ -997,23 +1116,24 @@
         for child in affected:
             self.container.body.add(child)
             self._config(child, **cache.get(child, {}))
 
     def clear_all(self):
         pass
 
-    def resize_widget(self, widget, bounds):
+    def resize_widget(self, widget, direction, delta):
         pass
 
     def add_widget(self, widget, bounds=None, **kwargs):
         super().remove_widget(widget)
         super().add_widget(widget, bounds, **kwargs)
-        self.container.body.add(widget)
+        if str(widget) not in self.container.body.panes():
+            self.container.body.add(widget)
         self._config(widget, **kwargs)
-        self.children.append(widget)
+        self._insert(widget)
 
     def _config(self, widget, **kwargs):
         if not kwargs:
             return self.container.body.paneconfig(widget)
         self.container.body.paneconfig(widget, **kwargs)
 
     def get_def(self, widget):
@@ -1031,15 +1151,18 @@
         return {k: info[k][-1] for k in info}
 
     def apply(self, prop, value, widget):
         self.container.body.paneconfig(widget, **{prop: value})
 
     def remove_widget(self, widget):
         super().remove_widget(widget)
-        self.container.body.forget(widget)
+        try:
+            self.container.body.forget(widget)
+        except tk.TclError:
+            pass
 
     def copy_layout(self, widget, from_):
         info = from_.layout.body.paneconfig(from_)
         info = {i: info[i][-1] for i in info}  # The value is usually the last item in the tuple
         self.add_widget(widget, (0, 0, 0, 0), **info)
 
 
@@ -1058,15 +1181,15 @@
     name = "NativePanedLayout"
 
     def apply(self, prop, value, widget):
         self.container.body.pane(widget, **{prop: value})
 
     def _config(self, widget, **kwargs):
         if not kwargs:
-            return self.container.pane(widget)
+            return self.container.body.pane(widget)
         self.container.body.pane(widget, **kwargs)
 
     def copy_layout(self, widget, from_):
         info = from_.layout.body.pane(from_)
         self.add_widget(widget, (0, 0, 0, 0), **info)
 
     def get_def(self, widget):
```

### Comparing `formation-studio-0.6.3/studio/lib/legacy.py` & `formation-studio-0.7.0/studio/lib/legacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import tkinter
 import tkinter as tk
 
 from studio.lib.pseudo import (
     PseudoWidget, Groups, Container, PanedContainer, _dimension_override
 )
-from studio.lib.toplevel import Toplevel
 from studio.lib.toplevel import Toplevel, Tk
 
 
 class Button(PseudoWidget, tk.Button):
     display_name = 'Button'
     group = Groups.widget
     icon = "button"
@@ -28,30 +28,35 @@
     def set_name(self, name):
         self.config(text=name)
 
 
 class Canvas(PseudoWidget, tk.Canvas):
     display_name = 'Canvas'
     group = Groups.container
-    icon = "paint"
+    icon = "object"
     impl = tk.Canvas
+    allow_direct_move = False
+    allow_drag_select = False
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
     def lift(self, above_this=None):
-        tk.Misc.lift(self, above_this)
+        return tk.Misc.lift(self, above_this)
+
+    def lower(self, below_this=None, *_):
+        return tk.Misc.lower(self, below_this)
 
 
 class Checkbutton(PseudoWidget, tk.Checkbutton):
     display_name = 'Checkbutton'
     group = Groups.widget
-    icon = "checkbutton"
+    icon = "checkbox"
     impl = tk.Checkbutton
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
@@ -62,14 +67,15 @@
 
 
 class Entry(PseudoWidget, tk.Entry):
     display_name = 'Entry'
     group = Groups.input
     icon = "entry"
     impl = tk.Entry
+    allow_direct_move = False
 
     DEF_OVERRIDES = {
         "state": {
             "options": ("normal", "readonly", "disabled")
         },
         "width": {
             "units": "char",
@@ -96,15 +102,15 @@
         self.id = id_
         self.setup_widget()
 
 
 class Label(PseudoWidget, tk.Label):
     display_name = 'Label'
     group = Groups.widget
-    icon = "text"
+    icon = "label"
     impl = tk.Label
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
@@ -130,14 +136,15 @@
 
 
 class Listbox(PseudoWidget, tk.Listbox):
     display_name = 'Listbox'
     group = Groups.container
     icon = "listbox"
     impl = tk.Listbox
+    allow_direct_move = False
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
@@ -158,14 +165,15 @@
 
 
 class Menubutton(PseudoWidget, tk.Menubutton):
     display_name = 'Menubutton'
     group = Groups.widget
     icon = "menubutton"
     impl = tk.Menubutton
+    allow_direct_move = False
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
@@ -173,30 +181,30 @@
     def set_name(self, name):
         self.config(text=name)
 
 
 class Message(PseudoWidget, tk.Message):
     display_name = 'Message'
     group = Groups.input
-    icon = "multiline_text"
+    icon = "message"
     impl = tk.Message
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
     def set_name(self, name):
         self.config(text=name)
 
 
 class PanedWindow(PanedContainer, tk.PanedWindow):
     display_name = 'PanedWindow'
     group = Groups.container
-    icon = "flip_horizontal"
+    icon = "dock_horizontal"
     impl = tk.PanedWindow
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
@@ -220,41 +228,44 @@
 
 class Scale(PseudoWidget, tk.Scale):
     display_name = 'Scale'
     group = Groups.input
     icon = "scale"
     impl = tk.Scale
     initial_dimensions = 45, 100
+    allow_direct_move = False
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.config(from_=0, to=100)
         self.set(40)
         self.setup_widget()
 
 
 class Scrollbar(PseudoWidget, tk.Scrollbar):
     display_name = 'Scrollbar'
     group = Groups.widget
-    icon = "play"
+    icon = "scrollbar"
     impl = tk.Scrollbar
     initial_dimensions = 20, 100
+    allow_direct_move = False
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
 
 class Spinbox(PseudoWidget, tk.Spinbox):
     display_name = 'Spinbox'
     group = Groups.input
     icon = "entry"
     impl = tk.Spinbox
+    allow_direct_move = False
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
@@ -264,14 +275,15 @@
 
 
 class Text(PseudoWidget, tk.Text):
     display_name = 'Text'
     group = Groups.input
     icon = "text"
     impl = tk.Text
+    allow_direct_move = False
 
     DEF_OVERRIDES = {
         "wrap": {
             "type": "choice",
             "options": ("char", "word", "none")
         },
         **_dimension_override
```

### Comparing `formation-studio-0.6.3/studio/lib/menu.py` & `formation-studio-0.7.0/studio/lib/menu.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/lib/native.py` & `formation-studio-0.7.0/studio/lib/native.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tkinter as tk
 import tkinter.ttk as ttk
 
 from studio.lib.layouts import NPanedLayoutStrategy
+from studio.lib.handles import LinearHandle
 from studio.lib.pseudo import (
     PseudoWidget, Groups, Container, TabContainer, PanedContainer,
     _dimension_override
 )
 
 
 class Button(PseudoWidget, ttk.Button):
@@ -24,15 +25,15 @@
     def set_name(self, name):
         self.config(text=name)
 
 
 class Checkbutton(PseudoWidget, ttk.Checkbutton):
     display_name = 'Checkbutton'
     group = Groups.widget
-    icon = "checkbutton"
+    icon = "checkbox"
     impl = ttk.Checkbutton
 
     DEF_OVERRIDES = {
         "width": {
             "units": "line",
             "negative": True
         }
@@ -46,16 +47,17 @@
     def set_name(self, name):
         self.config(text=name)
 
 
 class Combobox(PseudoWidget, ttk.Combobox):
     display_name = 'Combobox'
     group = Groups.input
-    icon = "combobox"
+    icon = "menubutton"
     impl = ttk.Combobox
+    allow_direct_move = False
 
     DEF_OVERRIDES = {
         "state": {
             "options": ("readonly",)
         },
         **_dimension_override
     }
@@ -70,14 +72,15 @@
 
 
 class Entry(PseudoWidget, ttk.Entry):
     display_name = 'Entry'
     group = Groups.input
     icon = "entry"
     impl = ttk.Entry
+    allow_direct_move = False
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
@@ -97,15 +100,15 @@
         self.id = id_
         self.setup_widget()
 
 
 class Label(PseudoWidget, ttk.Label):
     display_name = 'Label'
     group = Groups.widget
-    icon = "text"
+    icon = "label"
     impl = ttk.Label
 
     DEF_OVERRIDES = {
         "width": {
             "units": "line",
             "negative": True
         }
@@ -139,27 +142,29 @@
 
 class LabeledScale(PseudoWidget, ttk.LabeledScale):
     display_name = 'LabeledScale'
     group = Groups.input
     icon = "scale"
     impl = ttk.LabeledScale
     initial_dimensions = 150, 40
+    allow_direct_move = False
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
         self.state(['disabled'])
 
 
 class Menubutton(PseudoWidget, ttk.Menubutton):
     display_name = 'Menubutton'
     group = Groups.widget
     icon = "menubutton"
     impl = ttk.Menubutton
+    allow_direct_move = False
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
@@ -167,27 +172,27 @@
     def set_name(self, name):
         self.config(text=name)
 
 
 class Notebook(TabContainer, ttk.Notebook):
     display_name = 'Notebook'
     group = Groups.container
-    icon = "notebook"
+    icon = "tabs"
     impl = ttk.Notebook
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
 
 class VerticalPanedWindow(PanedContainer, ttk.PanedWindow):
     display_name = 'VerticalPanedWindow'
     group = Groups.container
-    icon = "flip_vertical"
+    icon = "dock_vertical"
     impl = ttk.PanedWindow
 
     def __init__(self, master, id_):
         super().__init__(master, orient=tk.VERTICAL)
         self.id = id_
         self.setup_widget()
         # Needs a modified PanedLayoutStrategy to work
@@ -204,15 +209,15 @@
         options['orient'] = str(self['orient'])
         return options
 
 
 class HorizontalPanedWindow(PanedContainer, ttk.PanedWindow):
     display_name = 'HorizontalPanedWindow'
     group = Groups.container
-    icon = "flip_horizontal"
+    icon = "dock_horizontal"
     impl = ttk.PanedWindow
 
     def __init__(self, master, id_):
         super().__init__(master, orient=tk.HORIZONTAL)
         self.id = id_
         self.setup_widget()
         # Needs a modified PanedLayoutStrategy to work
@@ -271,67 +276,71 @@
 
 class Scale(PseudoWidget, ttk.Scale):
     display_name = 'Scale'
     group = Groups.input
     icon = "scale"
     impl = ttk.Scale
     initial_dimensions = 150, 20
+    allow_direct_move = False
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
         self.state(['readonly'])
         self.set(40)
 
 
 class Scrollbar(PseudoWidget, ttk.Scrollbar):
     display_name = 'Scrollbar'
     group = Groups.widget
-    icon = "play"
+    icon = "scrollbar"
     impl = ttk.Scrollbar
     initial_dimensions = 20, 100
+    allow_direct_move = False
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
         self.state(['disabled'])
 
 
 class Separator(PseudoWidget, ttk.Separator):
     display_name = 'Separator'
     group = Groups.widget
-    icon = "play"
+    icon = "line"
     impl = ttk.Separator
     initial_dimensions = 150, 1
+    handle_class = LinearHandle
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
 
 class Sizegrip(Container, ttk.Sizegrip):
     display_name = 'Sizegrip'
     group = Groups.container
-    icon = "sizegrip"
+    icon = "frame"
     impl = ttk.Sizegrip
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
 
 
 class Spinbox(PseudoWidget, ttk.Spinbox):
     display_name = 'Spinbox'
     group = Groups.input
-    icon = "play"
+    icon = "entry"
     impl = ttk.Spinbox
+    allow_direct_move = False
 
     DEF_OVERRIDES = _dimension_override
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.setup_widget()
```

### Comparing `formation-studio-0.6.3/studio/lib/properties.py` & `formation-studio-0.7.0/studio/lib/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -630,11 +630,48 @@
     properties = widget.config()
     resolved_properties = {}
     # use extern overrides if DEF_OVERRIDES are not found
     overrides = getattr(widget, "DEF_OVERRIDES", extern_overrides or {})
     for prop in properties:
         definition = get_resolved(prop, overrides, PROPERTY_TABLE)
         if definition:
-            definition.update(value=widget[prop])
+            # TODO Remove this fix when no longer needed
+            definition.update(value=widget.get_prop(prop) if hasattr(widget, "get_prop") else widget[prop])
             resolved_properties[prop] = definition
 
     return resolved_properties
+
+
+def combine_properties(properties):
+    """
+    Return a dict of properties that are common to all widgets in the list.
+    """
+    if not properties:
+        return {}
+
+    # find the intersection of all the property names
+    common_properties = set.intersection(*[set(p.keys()) for p in properties])
+
+    # get the first definition for each common property
+    common_properties = {prop: properties[0][prop] for prop in common_properties}
+
+    # check that the values are the same for each widget
+    for prop, definition in common_properties.items():
+        for widget_properties in properties[1:]:
+            if widget_properties[prop]['value'] != definition['value']:
+                common_properties[prop]['value'] = ''
+                break
+
+    return common_properties
+
+
+def get_combined_properties(widgets):
+    """
+    Return a dict of properties that are common to all widgets in the list.
+    """
+    if not widgets:
+        return {}
+
+    # get all the properties for each widget
+    properties = [widget.properties for widget in widgets]
+
+    return combine_properties(properties)
```

### Comparing `formation-studio-0.6.3/studio/lib/pseudo.py` & `formation-studio-0.7.0/studio/lib/pseudo.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import tkinter
 import tkinter.ttk
 from enum import Enum
 
 from hoverset.data.images import load_tk_image, load_image, load_image_to_widget
 from hoverset.ui.icons import get_icon_image
 from hoverset.ui.menu import MenuUtils
+from hoverset.ui.widgets import EventMask
 from hoverset.util.execution import import_path
 from studio.lib import layouts
 from studio.lib.variables import VariableManager
 from studio.lib.properties import get_properties
-from studio.ui.highlight import WidgetHighlighter
+from studio.lib.handles import BoxHandle
 from studio.ui.tree import MalleableTree
+from studio.i18n import _
 
 
 # Applied to widgets whose width is specified in characters
 # and height in lines
 _dimension_override = {
     "width": {
         "units": "char",
@@ -25,19 +27,19 @@
     "height": {
         "units": "line"
     }
 }
 
 
 class Groups(Enum):
-    widget = 'Widget'
-    input = 'Input'
-    container = 'Container'
-    layout = 'Layout'
-    custom = 'Custom'
+    widget = _('Widget')
+    input = _('Input')
+    container = _('Container')
+    layout = _('Layout')
+    custom = _('Custom')
 
 
 class _ImageIntercept:
     __slots__ = []
 
     @staticmethod
     def set(widget, value, prop='image', **kw):
@@ -95,42 +97,188 @@
 
 class PseudoWidget:
     display_name = 'Widget'
     group = Groups.widget
     icon = "play"
     impl = None
     is_toplevel = False
+    allow_direct_move = True
+    allow_drag_select = False
     # special handlers (intercepts) for attributes that need additional processing
     # to interface with the studio easily
     _intercepts = {
         "image": _ImageIntercept,
         "selectimage": _ImageIntercept,
         "tristateimage": _ImageIntercept,
         "id": _IdIntercept,
         "textvariable": _VariableIntercept,
         "variable": _VariableIntercept,
         "listvariable": _VariableIntercept
     }
+    _no_defaults = {
+        "text",
+    }
 
     def setup_widget(self):
+        self.designer = self.master
         self.level = 0
         self.layout = None
         self.recent_layout_info = None
+        self.last_stable_bounds = None
         self._properties = get_properties(self)
         self.set_name(self.id)
         self.node = None
         self.__on_context = None
         self.last_menu_position = (0, 0)
+        self._pos_fix = (0, 0)
         self.max_size = None
         self.min_size = None
         MenuUtils.bind_context(self, self.__handle_context_menu, add='+')
+        self._handle_cls = getattr(self.__class__, "handle_class", BoxHandle)
+        self._handle = None
+
+        self._on_handle_active = getattr(self, "_on_handle_active", None)
+        self._on_handle_inactive = getattr(self, "_on_handle_inactive", None)
+        self._on_handle_resize = getattr(self, "_on_handle_resize", None)
+        self._on_handle_move = getattr(self, "_on_handle_move", None)
+
+        self.bind("<ButtonPress-1>", self._on_press, add='+')
+        self.bind("<ButtonRelease>", self._on_release, add='+')
+
+        self.bind("<Motion>", self._on_drag, add='+')
+
+        self._active = False
+        self._select_mode_active = False
+        self._select_bounds = None
+        self.prev_stack_index = None
 
     def set_name(self, name):
         pass
 
+    def get_bounds(self):
+        self.update_idletasks()
+        x1 = self.winfo_x()
+        y1 = self.winfo_y()
+        x2 = self.winfo_width() + x1
+        y2 = self.winfo_height() + y1
+        return x1, y1, x2, y2
+
+    def lift(self, above_this=None):
+        if isinstance(above_this, Container):
+            # first lift above container if possible
+            try:
+                super().lift(above_this.body)
+            except tkinter.TclError:
+                pass
+
+            # then lift above highest child if any
+            if above_this._children and self.layout != above_this:
+                super().lift(above_this._children[-1])
+        else:
+            super().lift(above_this)
+
+    def _on_press(self, event):
+        if not self.allow_direct_move and not event.state & EventMask.SHIFT:
+            if not self.allow_drag_select:
+                return
+            self._select_mode_active = True
+            self._pos_fix = (event.x_root, event.y_root)
+            return
+        if not self._handle:
+            return
+        self._pos_fix = (event.x_root, event.y_root)
+        self.handle_active('all')
+        self._active = True
+
+    def _on_release(self, _):
+        if self._select_mode_active:
+            self.designer.clear_select_region()
+            self._select_mode_active = False
+            if self._select_bounds is not None:
+                self.designer.select_in_region(self, self._select_bounds)
+                self._select_bounds = None
+
+        if not self._active:
+            return
+        self.handle_inactive('all')
+        self._active = False
+
+    def _on_drag(self, event):
+        if self._select_mode_active:
+            x1, y1 = self._pos_fix
+            x2, y2 = event.x_root, event.y_root
+            bounds = min(x1, x2), min(y1, y2), max(x1, x2), max(y1, y2)
+            self._select_bounds = bounds
+            self.designer.show_select_region(bounds)
+
+        if not self._active or not event.state & EventMask.MOUSE_BUTTON_1:
+            return
+        x, y = self._pos_fix
+        self._pos_fix = (event.x_root, event.y_root)
+        self.handle_resize('all', (event.x_root - x, event.y_root - y))
+
+    def show_handle(self, *_):
+        if not self._handle_cls:
+            return
+        if not self._handle:
+            self._handle = self._handle_cls.acquire(self, self.master, self.allow_direct_move)
+        self._handle.show()
+
+    def clear_handle(self):
+        if not self._handle:
+            return
+        self._handle.hide()
+        if not self._handle.active():
+            self._handle = None
+
+    def lift_handle(self):
+        if self._handle:
+            self._handle.lift()
+
+    def show_highlight(self, *_):
+        if not self._handle_cls:
+            return
+        if not self._handle:
+            self._handle = self._handle_cls.acquire(self, self.master)
+        self._handle.hover()
+
+    def clear_highlight(self):
+        if not self._handle:
+            return
+        self._handle.unhover()
+        if not self._handle.active():
+            self._handle = None
+
+    def on_handle_active(self, callback):
+        self._on_handle_active = callback
+
+    def on_handle_inactive(self, callback):
+        self._on_handle_inactive = callback
+
+    def on_handle_resize(self, callback):
+        self._on_handle_resize = callback
+
+    def on_handle_move(self, callback):
+        self._on_handle_move = callback
+
+    def handle_active(self, direction):
+        if self._on_handle_active:
+            self._on_handle_active(self, direction)
+
+    def handle_inactive(self, direction):
+        if self._on_handle_inactive:
+            self._on_handle_inactive(self, direction)
+
+    def handle_resize(self, direction, delta):
+        if self._on_handle_resize:
+            self._on_handle_resize(self, direction, delta)
+
+    def handle_move(self):
+        pass
+
     def get_image_path(self):
         if hasattr(self, "image_path"):
             return self.image_path
         return self['image']
 
     def set_tree_reference(self, node: MalleableTree.Node):
         self.node = node
@@ -165,23 +313,29 @@
             },
         }
 
     def get_prop(self, prop):
         intercept = self._intercepts.get(prop)
         if intercept:
             return intercept.get(self, prop)
-        return self[prop]
+        prop = self[prop]
+        if isinstance(prop, (tuple, list)):
+            prop = " ".join(map(str, prop))
+        return prop
 
     def configure(self, options=None, **kw):
         for opt in list(kw.keys()):
             intercept = self._intercepts.get(opt)
             if intercept:
                 intercept.set(self, kw[opt], opt)
                 kw.pop(opt)
-        return super().config(**kw)
+        ret = super().config(**kw)
+        if kw and self._handle:
+            self._handle.widget_config_changed()
+        return ret
 
     def bind_all(self, sequence, func=None, add=None):
         # we should be able to bind studio events
         # for complex hierarchies in custom widgets
         # this also overrides the default bind_all behaviour which
         # may cause problems for the studio if an external custom widget uses it
         def _deep_bind(widget):
@@ -225,15 +379,17 @@
             defaults = self.configure()
             defaults = {x: defaults[x][-2] for x in defaults}
         except TypeError:
             logging.error("options failed for" + str(self.id))
             return {}
         options = self.properties
         # Get options whose values are different from their default values
-        return {opt: self.get_prop(opt) for opt in options if str(defaults.get(opt)) != str(self.get_prop(opt))}
+        return {
+            opt: self.get_prop(opt) for opt in options if opt in self._no_defaults or str(defaults.get(opt)) != str(self.get_prop(opt))
+        }
 
     def get_method_defaults(self):
         return {}
 
     def get_methods(self):
         return {}
 
@@ -241,56 +397,63 @@
         # do not override
         defaults = self.get_method_defaults()
         return filter(lambda x: x != defaults.get(x.name), self.get_methods())
 
     def handle_method(self, name, *args, **kwargs):
         pass
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}<{self.id}>"
+
 
 class Container(PseudoWidget):
     LAYOUTS = layouts.layouts
+    allow_direct_move = False
+    allow_drag_select = True
 
     def setup_widget(self):
         self.parent = self.designer = self._get_designer()
         if not hasattr(self, 'body') or self.body is None:
             self.body = self
         self._level = 0
         self._children = []
-        self.temporal_children = []
-        self._highlighter = WidgetHighlighter(self.master)
         if len(self.LAYOUTS) == 0:
             raise ValueError("No layouts have been defined")
         self.layout_strategy = layouts.PlaceLayoutStrategy(self)
         self.layout_var = tkinter.StringVar()
         self.layout_var.set(self.layout_strategy.name)
         super().setup_widget()
 
     def _get_designer(self):
         return self.master
 
-    def show_highlight(self, *_):
-        self._highlighter.highlight(self)
-
-    def clear_highlight(self):
-        self._highlighter.clear()
-        self._temporal_children = []
-        self.layout_strategy.clear_indicators()
-
-    def lift(self, above_this):
+    def lift(self, above_this=None):
         super().lift(above_this)
         if self.body != self:
             self.body.lift(self)
-        for child in self._children:
-            child.lift(self.body)
+        if self._children:
+            self.layout_strategy._update_stacking()
 
-    def react(self, x, y):
+    def react(self, bounds):
         self.designer.set_active_container(self)
-        self.react_to_pos(x, y)
+        self.react_to_pos(bounds)
         self.show_highlight()
 
+    def clear_highlight(self):
+        super().clear_highlight()
+        self.layout_strategy.clear_indicators()
+
+    @property
+    def allow_resize(self):
+        return self.layout_strategy.allow_resize
+
+    @property
+    def realtime_support(self):
+        return self.layout_strategy.realtime_support
+
     @property
     def level(self):
         return self._level
 
     @level.setter
     def level(self, value):
         self._level = value
@@ -355,24 +518,24 @@
     def configure(self, **kwargs):
         if 'layout' in kwargs:
             self._switch_layout(kwargs['layout'])
             kwargs.pop('layout')
         return super().configure(**kwargs)
 
     def _set_layout(self, layout):
-        self.designer.studio.style_pane.apply_style("layout", layout, self)
+        self.designer.studio.style_pane.apply_style("layout", layout, None)
 
     def _get_layouts_as_menu(self):
         layout_templates = [
-            ("radiobutton", i.name, get_icon_image(i.icon, 14, 14),
+            ("radiobutton", i.name, get_icon_image(i.icon, 18, 18),
              functools.partial(self._set_layout, i),
              {"value": i.name, "variable": self.layout_var}
              ) for i in self.LAYOUTS
         ]
-        return (("cascade", "Change layout", get_icon_image("grid", 14, 14), None, {"menu": (
+        return (("cascade", _("Change layout"), get_icon_image("grid", 18, 18), None, {"menu": (
             layout_templates
         )}),)
 
     def create_menu(self):
         return (
             ("separator",),
             *self._get_layouts_as_menu()
@@ -396,22 +559,28 @@
 
     def add_widget(self, widget, bounds=None, **kwargs):
         self.layout_strategy.add_widget(widget, bounds, **kwargs)
 
     def widget_released(self, widget):
         self.layout_strategy.widget_released(widget)
 
-    def change_start(self, widget):
-        self.layout_strategy.change_start(widget)
+    def start_move(self, widget):
+        self.layout_strategy.start_move(widget)
 
-    def move_widget(self, widget, bounds):
-        self.layout_strategy.move_widget(widget, bounds)
+    def start_resize(self, widget):
+        self.layout_strategy.start_resize(widget)
 
-    def resize_widget(self, widget, bounds):
-        self.layout_strategy.resize_widget(widget, bounds)
+    def move_widget(self, widget, delta):
+        self.layout_strategy.move_widget(widget, delta)
+
+    def end_move(self, widget):
+        self.layout_strategy.end_move(widget)
+
+    def resize_widget(self, widget, direction, delta):
+        self.layout_strategy.resize_widget(widget, direction, delta)
 
     def get_restore(self, widget):
         return self.layout_strategy.get_restore(widget)
 
     def remove_widget(self, widget):
         self.layout_strategy.remove_widget(widget)
 
@@ -420,17 +589,17 @@
 
     def apply(self, prop, value, widget):
         self.layout_strategy.apply(prop, value, widget)
 
     def definition_for(self, widget):
         return self.layout_strategy.definition_for(widget)
 
-    def react_to_pos(self, x, y):
+    def react_to_pos(self, bounds):
         # react to position
-        self.layout_strategy.react_to_pos(x, y)
+        self.layout_strategy.react_to_pos(bounds)
 
     def copy_layout(self, widget, from_):
         self.layout_strategy.copy_layout(widget, from_)
 
     def get_altered_options_for(self, widget):
         return self.layout_strategy.get_altered_options(widget)
 
@@ -449,15 +618,15 @@
 
     def _get_layouts_as_menu(self):
         # Prevent changing of layout from tab layout
         return ()
 
     def create_menu(self):
         return super().create_menu() + (
-            ("command", "Add tab", get_icon_image("add", 14, 14), self._add_tab, {}),
+            ("command", _("Add tab"), get_icon_image("add", 18, 18), self._add_tab, {}),
         )
 
     def _add_tab(self):
         from studio.lib import legacy
         self.add_new(legacy.Frame, 0, 0)
 
     @property
@@ -490,15 +659,15 @@
 class PanedContainer(TabContainer):
     def setup_widget(self):
         super(TabContainer, self).setup_widget()
         self.layout_strategy = layouts.PanedLayoutStrategy(self)
 
     def create_menu(self):
         return super(TabContainer, self).create_menu() + (
-            ("command", "Add pane", get_icon_image("add", 14, 14), self._add_pane, {}),
+            ("command", _("Add pane"), get_icon_image("add", 18, 18), self._add_pane, {}),
         )
 
     def _add_pane(self):
         # add a legacy frame as a child
         from studio.lib import legacy
         self.add_new(legacy.Frame, 0, 0)
 
@@ -518,19 +687,19 @@
             base = PseudoWidget
 
         if dct.get("impl"):
             impl = dct["impl"]
         elif bases:
             impl = bases[0]
         else:
-            raise RuntimeError(
+            raise RuntimeError(_(
                 "Could not deduce base implementation for custom widget. "
                 "Inherit from base implementation or set the 'impl' attribute "
                 "to the base class"
-            )
+            ))
 
         attrs = dict(display_name=name, impl=impl, icon='play', group=Groups.custom)
         attrs.update(dct)
         obj_class = super().__new__(mcs, name, (base, *bases), attrs)
         return obj_class
 
     def __call__(cls, master, _id):
```

### Comparing `formation-studio-0.6.3/studio/lib/toplevel.py` & `formation-studio-0.7.0/studio/lib/toplevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
         self._menu = None
 
         if self._images is None:
             self._images = (
                 get_tk_image("close", 15, 15, color="#303030"),
                 get_tk_image("minimize", 15, 15, color="#000000"),
-                get_tk_image("rectangle", 10, 10, color="#000000"),
+                get_tk_image("maximize", 10, 10, color="#303030"),
                 get_tk_image("formation", 20, 20)
             )
 
         self.label = tk.Label(
             self.title, text="  title", image=self._images[3], compound="left")
         self.label.pack(side="left", padx=5, pady=5)
```

### Comparing `formation-studio-0.6.3/studio/lib/variables.py` & `formation-studio-0.7.0/studio/lib/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
         tk.StringVar: {
             "name": "String",
             "icon": "text",
             "type": "text",
         },
         tk.BooleanVar: {
             "name": "Boolean",
-            "icon": "checkbutton",
+            "icon": "checkbox",
             "type": "boolean",
         },
         tk.IntVar: {
             "name": "Integer",
             "icon": "entry",
             "type": "number",
         },
         tk.DoubleVar: {
             "name": "Double",
-            "icon": "math",
+            "icon": "ratio",
             "type": "number",
         }
     }
     supported_types = {".".join([i.__module__, i.__name__]): i for i in _types}
 
     def __init__(self, master, var, name=None):
         super().__init__(master)
```

### Comparing `formation-studio-0.6.3/studio/main.py` & `formation-studio-0.7.0/studio/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 # ======================================================================= #
 # Copyright (C) 2019 Hoverset Group.                                      #
 # ======================================================================= #
 
 import functools
 import os
+import subprocess
 import sys
 import time
 import tkinter
 import webbrowser
 from tkinter import filedialog
 
+import platformdirs
 import tkinterDnD
 
-from studio.feature.design import DesignContext, MultiSaveDialog
-from studio.feature import FEATURES, StylePane
-from studio.feature._base import BaseFeature, FeaturePane
-from studio.tools import ToolManager
-from studio.ui.widgets import SideBar
-from studio.ui.about import about_window
-from studio.preferences import Preferences, open_preferences
-from studio.resource_loader import ResourceLoader
-from studio.updates import Updater
-from studio.context import BaseContext
+# force locale setting
+from studio.i18n import _
 import studio
-
+from formation.formats import get_file_types, get_file_extensions
+from hoverset.data import actions
+from hoverset.data.images import load_tk_image
+from hoverset.data.keymap import ShortcutManager, CharKey, KeyMap, BlankKey, Symbol
+from hoverset.data.utils import get_resource_path
+from hoverset.platform import platform_is, MAC, WINDOWS
+from hoverset.ui.dialogs import MessageDialog
+from hoverset.ui.icons import get_icon_image
+from hoverset.ui.menu import MenuUtils, EnableIf, dynamic_menu, LoadLater, ShowIf
 from hoverset.ui.widgets import (
     Application, Frame, PanedWindow, Button,
     ActionNotifier, TabView, Label
 )
-from hoverset.ui.icons import get_icon_image
-from hoverset.data.images import load_tk_image
 from hoverset.util.execution import Action
-from hoverset.data.utils import get_resource_path
-from hoverset.ui.dialogs import MessageDialog
-from hoverset.ui.menu import MenuUtils, EnableIf, dynamic_menu, LoadLater
-from hoverset.data import actions
-from hoverset.data.keymap import ShortcutManager, CharKey, KeyMap, BlankKey
-from hoverset.platform import platform_is, MAC
-
-from formation import AppBuilder
-from formation.formats import get_file_types, get_file_extensions
+from hoverset.data.i18n import set_locale
+from studio.context import BaseContext
+from studio.feature import FEATURES, StylePane
+from studio.feature._base import BaseFeature, FeaturePane
+from studio.feature.design import DesignContext, MultiSaveDialog
+from studio.preferences import Preferences, open_preferences
+from studio.resource_loader import ResourceLoader
+from studio.selection import Selection
+from studio.tools import ToolManager
+from studio.ui import geometry
+from studio.ui.about import about_window
+from studio.ui.widgets import SideBar
+from studio.updates import Updater
 
 pref = Preferences.acquire()
 
 
 class StudioApplication(Application):
-    ICON_PATH = get_resource_path(studio, "resources/images/formation_icon.png")
+    if platform_is(WINDOWS):
+        ICON_PATH = get_resource_path(studio, "resources/images/formation.ico")
+    else:
+        ICON_PATH = get_resource_path(studio, "resources/images/formation_icon.png")
     THEME_PATH = pref.get("resource::theme")
+    dirs = platformdirs.AppDirs(appname="formation", appauthor="hoverset")
 
     def __init__(self, master=None, **cnf):
         super().__init__(master, **cnf)
         # Load icon asynchronously to prevent issues which have been known to occur when loading it synchronously
-        icon_image = load_tk_image(self.ICON_PATH)
+        self.icon_image = load_tk_image(self.ICON_PATH)
         self.load_styles(self.THEME_PATH)
-        self.iconphoto(True, icon_image)
+        self.iconphoto(True, self.icon_image)
         self.pref = pref
         self._restore_position()
         self.title('Formation Studio')
         self.protocol('WM_DELETE_WINDOW', self._on_close)
         self.shortcuts = ShortcutManager(self, pref)
         self.shortcuts.bind_all()
         self._register_actions()
@@ -95,136 +103,147 @@
             "right": (self._right, self._right_bar),
             "center": (self._center, None)
         }
 
         icon = get_icon_image
 
         self.actions = (
-            ("Delete", icon("delete", 20, 20), lambda e: self.delete(), "Delete selected widget"),
-            ("Undo", icon("undo", 20, 20), lambda e: self.undo(), "Undo action"),
-            ("Redo", icon("redo", 20, 20), lambda e: self.redo(), "Redo action"),
-            ("Cut", icon("cut", 20, 20), lambda e: self.cut(), "Cut selected widget"),
+            ("Delete", icon("remove", 20, 20), lambda e: self.delete(), _("Delete selected widgets")),
+            ("Undo", icon("undo", 20, 20), lambda e: self.undo(), _("Undo action")),
+            ("Redo", icon("redo", 20, 20), lambda e: self.redo(), _("Redo action")),
+            ("Cut", icon("cut", 20, 20), lambda e: self.cut(), _("Cut selected widgets")),
             ("separator",),
-            ("Fullscreen", icon("image_editor", 20, 20), lambda e: self.close_all(), "Design mode"),
-            ("Separate", icon("separate", 20, 20), lambda e: self.features_as_windows(),
-             "Open features in window mode"),
-            ("Dock", icon("flip_horizontal", 15, 15), lambda e: self.features_as_docked(),
-             "Dock all features"),
+            ("Fullscreen", icon("fullscreen", 20, 20), lambda e: self.close_all(), _("Design mode")),
+            ("Separate", icon("undock", 20, 20), lambda e: self.features_as_windows(),
+             _("Open features in window mode")),
+            ("Dock", icon("dock_horizontal", 15, 15), lambda e: self.features_as_docked(),
+             _("Dock all features")),
             ("separator",),
-            ("New", icon("add", 20, 20), lambda e: self.open_new(), "New design"),
-            ("Save", icon("save", 20, 20), lambda e: self.save(), "Save design"),
-            ("Preview", icon("play", 20, 20), lambda e: self.preview(), "Preview design"),
+            ("New", icon("add", 20, 20), lambda e: self.open_new(), _("New design")),
+            ("Save", icon("save", 20, 20), lambda e: self.save(), _("Save design")),
+            ("Preview", icon("play", 20, 20), lambda e: self.preview(), _("Preview design")),
         )
 
         self.init_toolbar()
-        self.selected = None
+        self._selection = Selection(self)
         # set the image option to blank if there is no image for the menu option
-        self.blank_img = blank_img = icon("blank", 14, 14)
+        self.blank_img = blank_img = icon("blank", 18, 18)
 
         self.tool_manager = ToolManager(self)
 
         # -------------------------------------------- menu definition ------------------------------------------------
         self.menu_template = (EnableIf(
-            lambda: self.selected,
+            lambda: bool(self.selection),
             ("separator",),
-            ("command", "copy", icon("copy", 14, 14), actions.get('STUDIO_COPY'), {}),
-            ("command", "duplicate", icon("copy", 14, 14), actions.get('STUDIO_DUPLICATE'), {}),
+            ("command", _("copy"), icon("copy", 18, 18), actions.get('STUDIO_COPY'), {}),
+            ("command", _("duplicate"), icon("blank", 18, 18), actions.get('STUDIO_DUPLICATE'), {}),
             EnableIf(
-                lambda: self._clipboard is not None,
-                ("command", "paste", icon("clipboard", 14, 14), actions.get('STUDIO_PASTE'), {})
+                lambda: self._clipboard is not None and len(self.selection) < 2,
+                ("command", _("paste"), icon("clipboard", 18, 18), actions.get('STUDIO_PASTE'), {})
+            ),
+            ("command", _("cut"), icon("cut", 18, 18), actions.get('STUDIO_CUT'), {}),
+            ("separator",),
+            ShowIf(
+                lambda: self.selection and self.selection[0].layout.layout_strategy.stacking_support,
+                EnableIf(
+                    lambda: self.selection.is_same_parent(),
+                    ("command", _("send to back"), icon("send_to_back", 18, 18), actions.get('STUDIO_BACK'), {}),
+                    ("command", _("bring to front"), icon("bring_to_front", 18, 18), actions.get('STUDIO_FRONT'), {}),
+                    ("command", _("back one step"), icon("send_to_back", 18, 18), actions.get('STUDIO_BACK_1'), {}),
+                    ("command", _("forward one step"), icon("bring_to_front", 18, 18), actions.get('STUDIO_FRONT_1'), {}),
+                ),
             ),
-            ("command", "cut", icon("cut", 14, 14), actions.get('STUDIO_CUT'), {}),
             ("separator",),
-            ("command", "delete", icon("delete", 14, 14), actions.get('STUDIO_DELETE'), {}),
+            ("command", _("delete"), icon("delete", 18, 18), actions.get('STUDIO_DELETE'), {}),
         ),)
 
         self.menu_bar = MenuUtils.make_dynamic(
             ((
-                 ("cascade", "formation", None, None, {"menu": (
-                     ("command", "Restart", None, actions.get('STUDIO_RESTART'), {}),
+                 ("cascade", _("formation"), None, None, {"menu": (
+                     ("command", _("Restart"), None, actions.get('STUDIO_RESTART'), {}),
                      ("separator", ),
-                     ("command", "About Formation", icon("formation", 14, 14), lambda: about_window(self), {}),
+                     ("command", _("About Formation"), icon("formation", 18, 18), lambda: about_window(self), {}),
                  ), "name": "apple"}),
              ) if platform_is(MAC) else ()) +
             (
-                ("cascade", "File", None, None, {"menu": (
-                    ("command", "New", icon("add", 14, 14), actions.get('STUDIO_NEW'), {}),
-                    ("command", "Open", icon("folder", 14, 14), actions.get('STUDIO_OPEN'), {}),
-                    ("cascade", "Recent", icon("clock", 14, 14), None, {"menu": self._create_recent_menu()}),
+                ("cascade", _("File"), None, None, {"menu": (
+                    ("command", _("New"), icon("add", 18, 18), actions.get('STUDIO_NEW'), {}),
+                    ("command", _("Open"), icon("folder", 18, 18), actions.get('STUDIO_OPEN'), {}),
+                    ("cascade", _("Recent"), icon("recent", 18, 18), None, {"menu": self._create_recent_menu()}),
                     ("separator",),
                     EnableIf(
                         lambda: self.designer,
-                        ("command", "Save", icon("save", 14, 14), actions.get('STUDIO_SAVE'), {}),
-                        ("command", "Save As", icon("blank", 14, 14), actions.get('STUDIO_SAVE_AS'), {})
+                        ("command", _("Save"), icon("save", 18, 18), actions.get('STUDIO_SAVE'), {}),
+                        ("command", _("Save As"), icon("blank", 18, 18), actions.get('STUDIO_SAVE_AS'), {})
                     ),
                     EnableIf(
                         # more than one design contexts open
                         lambda: len([i for i in self.contexts if isinstance(i, DesignContext)]) > 1,
-                        ("command", "Save All", icon("blank", 14, 14), actions.get('STUDIO_SAVE_ALL'), {})
+                        ("command", _("Save All"), icon("blank", 18, 18), actions.get('STUDIO_SAVE_ALL'), {})
                     ),
                     ("separator",),
-                    ("command", "Settings", icon("settings", 14, 14), actions.get('STUDIO_SETTINGS'), {}),
-                    ("command", "Restart", icon("blank", 14, 14), actions.get('STUDIO_RESTART'), {}),
-                    ("command", "Exit", icon("close", 14, 14), actions.get('STUDIO_EXIT'), {}),
+                    ("command", _("Settings"), icon("settings", 18, 18), actions.get('STUDIO_SETTINGS'), {}),
+                    ("command", _("Restart"), icon("blank", 18, 18), actions.get('STUDIO_RESTART'), {}),
+                    ("command", _("Exit"), icon("close", 18, 18), actions.get('STUDIO_EXIT'), {}),
                 )}),
-                ("cascade", "Edit", None, None, {"menu": (
+                ("cascade", _("Edit"), None, None, {"menu": (
                     EnableIf(lambda: self.context and self.context.has_undo(),
-                             ("command", "undo", icon("undo", 14, 14), actions.get('STUDIO_UNDO'), {})),
+                             ("command", _("undo"), icon("undo", 18, 18), actions.get('STUDIO_UNDO'), {})),
                     EnableIf(lambda: self.context and self.context.has_redo(),
-                             ("command", "redo", icon("redo", 14, 14), actions.get('STUDIO_REDO'), {})),
+                             ("command", _("redo"), icon("redo", 18, 18), actions.get('STUDIO_REDO'), {})),
                     *self.menu_template,
                 )}),
-                ("cascade", "Code", None, None, {"menu": (
+                ("cascade", _("Code"), None, None, {"menu": (
                     EnableIf(
                         lambda: self.designer and self.designer.root_obj,
-                        ("command", "Preview design", icon("play", 14, 14), actions.get('STUDIO_PREVIEW'), {}),
-                        ("command", "close preview", icon("close", 14, 14), actions.get('STUDIO_PREVIEW_CLOSE'), {}),
+                        ("command", _("Preview design"), icon("play", 18, 18), actions.get('STUDIO_PREVIEW'), {}),
+                        ("command", _("close preview"), icon("close", 18, 18), actions.get('STUDIO_PREVIEW_CLOSE'), {}),
                         ("separator", ),
                         EnableIf(
                             lambda: self.designer and self.designer.design_path,
-                            ("command", "Reload design file", icon("rotate_clockwise", 14, 14),
+                            ("command", _("Reload design file"), icon("reload", 18, 18),
                              actions.get('STUDIO_RELOAD'), {}),
                         ),
                     )
                 )}),
-                ("cascade", "View", None, None, {"menu": (
-                    ("command", "show all panes", blank_img, actions.get('FEATURE_SHOW_ALL'), {}),
-                    ("command", "close all panes", icon("close", 14, 14), actions.get('FEATURE_CLOSE_ALL'), {}),
-                    ("command", "close all panes on the right", blank_img, actions.get('FEATURE_CLOSE_RIGHT'), {}),
-                    ("command", "close all panes on the left", blank_img, actions.get('FEATURE_CLOSE_LEFT'), {}),
+                ("cascade", _("View"), None, None, {"menu": (
+                    ("command", _("show all panes"), blank_img, actions.get('FEATURE_SHOW_ALL'), {}),
+                    ("command", _("close all panes"), icon("close", 18, 18), actions.get('FEATURE_CLOSE_ALL'), {}),
+                    ("command", _("close all panes on the right"), blank_img, actions.get('FEATURE_CLOSE_RIGHT'), {}),
+                    ("command", _("close all panes on the left"), blank_img, actions.get('FEATURE_CLOSE_LEFT'), {}),
                     ("separator",),
-                    ("command", "Undock all windows", blank_img, actions.get('FEATURE_UNDOCK_ALL'), {}),
-                    ("command", "Dock all windows", blank_img, actions.get('FEATURE_DOCK_ALL'), {}),
+                    ("command", _("Undock all windows"), blank_img, actions.get('FEATURE_UNDOCK_ALL'), {}),
+                    ("command", _("Dock all windows"), blank_img, actions.get('FEATURE_DOCK_ALL'), {}),
                     ("separator",),
                     LoadLater(self.get_features_as_menu),
                     ("separator",),
                     EnableIf(
                         lambda: self.context,
-                        ("command", "close tab", icon("close", 14, 14), actions.get('CONTEXT_CLOSE'), {}),
-                        ("command", "close all tabs", blank_img, actions.get('CONTEXT_CLOSE_ALL'), {}),
+                        ("command", _("close tab"), icon("close", 18, 18), actions.get('CONTEXT_CLOSE'), {}),
+                        ("command", _("close all tabs"), blank_img, actions.get('CONTEXT_CLOSE_ALL'), {}),
                         EnableIf(
                             lambda: self.context and len(self.tab_view.tabs()) > 1,
-                            ("command", "close other tabs", blank_img, actions.get('CONTEXT_CLOSE_OTHER'), {})
+                            ("command", _("close other tabs"), blank_img, actions.get('CONTEXT_CLOSE_OTHER'), {})
                         ),
                         EnableIf(
                             lambda: self.context and self.context._contexts_right(),
-                            ("command", "close all tabs on the right", blank_img,
+                            ("command", _("close all tabs on the right"), blank_img,
                              actions.get('CONTEXT_CLOSE_OTHER_RIGHT'), {})
                         )
                     ),
                     ("separator",),
-                    ("command", "Save window positions", blank_img, actions.get('FEATURE_SAVE_POS'), {})
+                    ("command", _("Save window positions"), blank_img, actions.get('FEATURE_SAVE_POS'), {})
                 )}),
-                ("cascade", "Tools", None, None, {"menu": (LoadLater(self.tool_manager.get_tools_as_menu), )}),
-                ("cascade", "Help", None, None, {"menu": (
-                    ("command", "Help", icon('dialog_info', 14, 14), actions.get('STUDIO_HELP'), {}),
-                    ("command", "Report issue", blank_img, self.report_issue, {}),
-                    ("command", "Check for updates", icon("cloud", 14, 14), self._check_updates, {}),
+                ("cascade", _("Tools"), None, None, {"menu": (LoadLater(self.tool_manager.get_tools_as_menu), )}),
+                ("cascade", _("Help"), None, None, {"menu": (
+                    ("command", _("Help"), icon('dialog_info', 18, 18), actions.get('STUDIO_HELP'), {}),
+                    ("command", _("Report issue"), blank_img, self.report_issue, {}),
+                    ("command", _("Check for updates"), blank_img, self._check_updates, {}),
                     ("separator",),
-                    ("command", "About Formation", icon("formation", 14, 14), lambda: about_window(self), {}),
+                    ("command", _("About Formation"), icon("formation", 18, 18), lambda: about_window(self), {}),
                 )})
             ), self, self.style, False)
 
         self.config(menu=self.menu_bar)
 
         if platform_is(MAC):
             self.createcommand("tk::mac::ShowPreferences", lambda: actions.get('STUDIO_SETTINGS').invoke())
@@ -241,15 +260,15 @@
         self.tab_view.bind("<<TabSelectionChanged>>", self.on_context_switch)
         self.tab_view.bind("<<TabClosed>>", self.on_context_close)
         self.tab_view.bind("<<TabAdded>>", self.on_context_add)
         self.tab_view.bind("<<TabOrderChanged>>", lambda _: self.save_tab_status())
         self._center.add(self.tab_view, sticky='nswe')
         self._tab_view_empty = Label(
             self.tab_view, **self.style.text_passive, compound='top',
-            image=get_icon_image("paint", 60, 60)
+            image=get_icon_image("design", 60, 60)
         )
         self._tab_view_empty.config(**self.style.bright)
 
         # install features
         for feature in FEATURES:
             self.install(feature)
 
@@ -263,14 +282,18 @@
         self._startup()
         self._exit_failures = 0
         self._is_shutting_down = False
 
         self._left.restore_size()
         self._right.restore_size()
 
+    @property
+    def selection(self):
+        return self._selection
+
     def on_context_switch(self, _):
         selected = self.tab_view.selected
         if isinstance(self.context, BaseContext):
             self.context.on_context_unset()
 
         if isinstance(selected, BaseContext):
             self.context = selected
@@ -283,22 +306,22 @@
         self.tool_manager.on_context_switch()
 
         if self.context:
             selected.on_context_set()
 
         # switch selection to that of the new context
         if self.designer:
-            self.select(self.designer.current_obj, self.designer)
+            self.selection.set(self.designer.selected)
         else:
-            self.select(None)
+            self.selection.clear()
         self.save_tab_status()
 
     def on_context_close(self, context):
         if not self.tab_view.tabs():
-            self._show_empty("Open a design file")
+            self._show_empty(_("Open a design file"))
         if context in self.contexts:
             self.contexts.remove(context)
         for feature in self.features:
             feature.on_context_close(context)
         self.tool_manager.on_context_close(context)
         self.save_tab_status()
 
@@ -339,14 +362,18 @@
             self.context.close_other_right()
 
     @property
     def designer(self):
         if isinstance(self.context, DesignContext):
             return self.context.designer
 
+    def get_widgets(self):
+        if self.designer:
+            return self.designer.objects
+
     def _show_empty(self, text):
         if text:
             self._tab_view_empty.lift()
             self._tab_view_empty['text'] = text
             self._tab_view_empty.place(x=0, y=0, relwidth=1, relheight=1)
         else:
             self._tab_view_empty.place_forget()
@@ -354,30 +381,30 @@
     def _startup(self):
         on_startup = pref.get("studio::on_startup")
         if on_startup == "new":
             self.open_new()
         elif on_startup == "recent":
             self.restore_tabs()
         else:
-            self._show_empty("Open a design file")
+            self._show_empty(_("Open a design file"))
 
     def _get_window_state(self):
         try:
             if self.wm_attributes("-zoomed"):
                 return 'zoomed'
             return 'normal'
-        except:
+        except tkinter.TclError:
             # works for windows and mac os
             return self.state()
 
     def _set_window_state(self, state):
         try:
             # works in windows and mac os
             self.state(state)
-        except:
+        except tkinter.TclError:
             self.wm_attributes('-zoomed', state == 'zoomed')
 
     def _save_position(self):
         # self.update_idletasks()
         pref.set("studio::pos", dict(
             geometry=self.geometry(),
             state=self._get_window_state(),  # window state either zoomed or normal
@@ -413,34 +440,37 @@
         if self.context:
             return self.context.last_action()
 
     def pop_last_action(self, key=None):
         if self.context:
             self.context.pop_last_action(key)
 
-    def copy(self):
-        if self.designer and self.selected:
-            # store the current object as  node in the clipboard
-            self._clipboard = self.designer.as_node(self.selected)
-
     def install_status_widget(self, widget_class, *args, **kwargs):
         widget = widget_class(self._statusbar, *args, **kwargs)
         widget.pack(side='right', padx=2, fill='y')
         return widget
 
+    def send_back(self, steps=0):
+        if self.designer and self.selection:
+            self.designer.send_back(steps)
+
+    def bring_front(self, steps=0):
+        if self.designer and self.selection:
+            self.designer.bring_front(steps)
+
     def get_pane_info(self, pane):
         return self._panes.get(pane, [self._right, self._right_bar])
 
     def paste(self):
         if self.designer and self._clipboard is not None:
             self.designer.paste(self._clipboard)
 
     def close_all_on_side(self, side):
         for feature in self.features:
-            if feature.side == side:
+            if feature._side.get() == side:
                 feature.minimize()
         # To avoid errors when side is not a valid pane identifier we default to the right pane
         self._panes.get(side, (self._right, self._right_bar))[1].close_all()
 
     def close_all(self, *_):
         for feature in self.features:
             feature.minimize()
@@ -494,66 +524,69 @@
             self._adjust_pane(pane)
         else:
             bar.select(obj)
             obj.maximize()
         return obj
 
     def show_all_windows(self):
-        for feature in self.features:
+        for feature in self.features: 
             feature.maximize()
 
     def features_as_windows(self):
         for feature in self.features:
-            feature.open_as_window()
+            if feature.is_visible.get():
+                feature.open_as_window()
 
     def features_as_docked(self):
         for feature in self.features:
             feature.open_as_docked()
 
     def set_path(self, path):
         if path:
             file_dir = os.path.dirname(path)
             if os.path.exists(file_dir):
                 # change working directory
                 os.chdir(file_dir)
-        path = path or "untitled"
+        path = path or _("untitled")
         self.title("Formation studio" + " - " + str(path))
 
     @dynamic_menu
     def _create_recent_menu(self, menu):
         # Dynamically create recent file menu every time menu is posted
-        menu.image = get_icon_image("close", 14, 14)
+        menu.image = get_icon_image("close", 18, 18)
         menu.config(**self.style.context_menu)
         recent = pref.get_recent()
         for path, label in recent:
             menu.add_command(
                 label=label,
                 command=functools.partial(self.open_recent, path),
                 image=self.blank_img, compound='left',
             )
         menu.add_command(
-            label="Clear", image=menu.image, command=pref.clear_recent,
+            label=_("Clear"), image=menu.image, command=pref.clear_recent,
             compound="left"
         )
 
     def open_file(self, path=None):
         if path is None:
             path = filedialog.askopenfilename(parent=self, filetypes=get_file_types())
         elif not os.path.exists(path):
             MessageDialog.show_error(
                 parent=self,
-                title="Missing File",
-                message="File {} does not exist".format(path),
+                title=_("Missing File"),
+                message=_("File {} does not exist").format(path),
             )
             return
         elif path.split(".")[-1] not in get_file_extensions():
             MessageDialog.show_error(
                 parent=self,
-                title="Unsupported type",
-                message=f"File {path} is not of a supported file type ({get_file_extensions()}).",
+                title=_("Unsupported type"),
+                message=_("File {path} is not of a supported file type ({typ}).").format(
+                    path=path, typ=get_file_extensions()
+                )
             )
             return
         if path:
             # find if path is already open on the designer
             for context in self.contexts:
                 if isinstance(context, DesignContext) and context.path == path:
                     # path is open, select
@@ -602,15 +635,15 @@
                 return feature
         # returns None by if feature is not found
 
     def get_features_as_menu(self):
         # For each feature we create a menu template
         # The command value is the self.maximize method which will reopen the feature
         return [("checkbutton",  # Type
-                 f.name, None,  # Label, image
+                 f.display_name, None,  # Label, image
                  functools.partial(f.toggle),  # Command built from feature
                  {"variable": f.is_visible}) for f in self.features]
 
     def save_window_positions(self):
         for feature in self.features:
             feature.save_window_pos()
         self._save_position()
@@ -627,76 +660,100 @@
         self._adjust_pane(feature.pane)
 
     def maximize(self, feature):
         feature.pane.add(feature, minsize=100)
         feature.bar.select(feature)
         self._adjust_pane(feature.pane)
 
-    def select(self, widget, source=None):
-        self.selected = widget
-        if self.designer and source != self.designer:
-            # Select from the designer explicitly so the selection does not end up being re-fired
-            self.designer.select(widget, True)
-        for feature in self.features:
-            if feature != source:
-                feature.on_select(widget)
-        self.tool_manager.on_select(widget)
-
     def add(self, widget, parent=None):
         for feature in self.features:
             feature.on_widget_add(widget, parent)
+
         self.tool_manager.on_widget_add(widget, parent)
 
-    def widget_modified(self, widget1, source=None, widget2=None):
+    def widgets_modified(self, widgets, source=None):
         for feature in self.features:
             if feature != source:
-                feature.on_widget_change(widget1, widget2)
+                feature.on_widgets_change(widgets)
         if self.designer and self.designer != source:
-            self.designer.on_widget_change(widget1, widget2)
-        self.tool_manager.on_widget_change(widget1, widget2)
+            self.designer.on_widgets_change(widgets)
+
+        self.tool_manager.on_widgets_change(widgets)
 
-    def widget_layout_changed(self, widget):
+    def widgets_layout_changed(self, widgets):
         for feature in self.features:
-            feature.on_widget_layout_change(widget)
-        self.tool_manager.on_widget_layout_change(widget)
+            feature.on_widgets_layout_change(widgets)
 
-    def delete(self, widget=None, source=None):
-        widget = self.selected if widget is None else widget
-        if widget is None:
+        self.tool_manager.on_widgets_layout_change(widgets)
+
+    def reorder_widgets(self, indices, source=None):
+        for feature in self.features:
+            if feature != source:
+                feature.on_widgets_reorder(indices)
+
+        self.tool_manager.on_widgets_reorder(indices)
+
+    def make_clipboard(self, widgets):
+        bounds = geometry.overall_bounds([w.get_bounds() for w in widgets])
+        data = []
+        for widget in widgets:
+            data.append((
+                self.designer.as_node(widget),
+                geometry.relative_to_bounds(widget.get_bounds(), bounds),
+            ))
+        return data
+
+    def copy(self):
+        if self.designer and self.selection:
+            # store the current objects as  nodes in the clipboard
+            self._clipboard = self.make_clipboard(self.selection.compact())
+        pass
+
+    def delete(self, widgets=None, source=None):
+        widgets = list(self.selection.compact()) if widgets is None else widgets
+        if not widgets:
             return
-        if self.selected == widget:
-            self.select(None)
+
+        if any(widget in self.selection for widget in widgets):
+            self.selection.clear()
+
         if self.designer and source != self.designer:
-            self.designer.delete(widget)
+            self.designer.delete(widgets)
+
         for feature in self.features:
-            feature.on_widget_delete(widget)
-        self.tool_manager.on_widget_delete(widget)
+            feature.on_widgets_delete(widgets)
 
-    def cut(self, widget=None, source=None):
+        self.tool_manager.on_widgets_delete(widgets)
+
+    def cut(self, widgets=None, source=None):
         if not self.designer:
             return
-        widget = self.selected if widget is None else widget
-        if not widget:
+
+        widgets = list(self.selection.compact()) if widgets is None else widgets
+        if not widgets:
             return
-        if self.selected == widget:
-            self.select(None)
-        self._clipboard = self.designer.as_node(widget)
+
+        if any(widget in self.selection for widget in widgets):
+            self.selection.clear()
+
+        self._clipboard = self.make_clipboard(widgets)
         if source != self.designer:
-            self.designer.delete(widget, True)
+            self.designer.delete(widgets)
         for feature in self.features:
-            feature.on_widget_delete(widget, True)
-        self.tool_manager.on_widget_delete(widget)
+            feature.on_widgets_delete(widgets, True)
+
+        self.tool_manager.on_widgets_delete(widgets)
 
     def duplicate(self):
-        if self.designer and self.selected:
-            self.designer.paste(self.designer.as_node(self.selected))
+        if self.designer and self.selection:
+            self.designer.paste(self.make_clipboard(self.selection.compact()))
 
-    def on_restore(self, widget):
+    def on_restore(self, widgets):
         for feature in self.features:
-            feature.on_widget_restore(widget)
+            feature.on_widgets_restore(widgets)
 
     def on_feature_change(self, new, old):
         self.features.insert(self.features.index(old), new)
         self.features.remove(old)
 
     def on_session_clear(self, source):
         for feature in self.features:
@@ -716,15 +773,15 @@
                 select=context_dat["selected"],
                 **context_dat["kwargs"]
             )
             has_select = has_select or context_dat["selected"]
             first_context = context if first_context is None else first_context
             context.deserialize(context_dat["data"])
         if not first_context:
-            self._show_empty("Open a design file")
+            self._show_empty(_("Open a design file"))
         elif not has_select:
             first_context.select()
         self._ignore_tab_status = False
 
     def save_tab_status(self):
         if self._ignore_tab_status:
             return
@@ -756,40 +813,44 @@
         return True
 
     def preview(self):
         if self.designer.root_obj is None:
             # If there is no root object show a warning
             MessageDialog.show_warning(
                 parent=self,
-                title='Empty design',
-                message='There is nothing to preview. Please add a root widget')
+                title=_('Empty design'),
+                message=_('There is nothing to preview. Please add a root widget'))
             return
         # close previous preview if any
         self.close_preview()
-        self.current_preview = AppBuilder(node=self.designer.to_tree(), path=self.designer.design_path)
+        path = os.path.join(self.dirs.user_cache_dir, "temp_design.xml")
+        self.designer.to_tree().write(path)
+        self.current_preview = subprocess.Popen(
+            [sys.executable, "-m", "formation", path],
+        )
 
     def close_preview(self):
         if self.current_preview:
             try:
-                self.current_preview._app.destroy()
+                self.current_preview.terminate()
             except tkinter.TclError:
                 pass
             self.current_preview = None
 
     def reload(self):
         if self.designer:
             self.designer.reload()
 
     def _force_exit_prompt(self):
         return MessageDialog.builder(
-            {"text": "Force exit", "value": True, "focus": True},
-            {"text": "Return to app", "value": False},
+            {"text": _("Force exit"), "value": True, "focus": True},
+            {"text": _("Return to app"), "value": False},
             wait=True,
-            title="Exit Failure",
-            message="An internal failure is preventing the app from exiting. Force exit?",
+            title=_("Exit Failure"),
+            message=_("An internal failure is preventing the app from exiting. Force exit?"),
             parent=self,
             icon=MessageDialog.ICON_ERROR
         )
 
     def _on_close(self):
         """ Return ``True`` if exit successful otherwise ``False`` """
         if self._is_shutting_down:
@@ -830,16 +891,16 @@
 
     def settings(self):
         open_preferences(self)
 
     def _coming_soon(self):
         MessageDialog.show_info(
             parent=self,
-            title="Coming soon",
-            message="We are working hard to bring this feature to you. Hang in there.",
+            title=_("Coming soon"),
+            message=_("We are working hard to bring this feature to you. Hang in there."),
             icon="clock"
         )
 
     def _open_debugtools(self):
         from studio.debugtools.debugger import Debugger
 
         # close previous process if any
@@ -855,59 +916,67 @@
         Updater.check(self)
 
     def _register_actions(self):
         CTRL, ALT, SHIFT = KeyMap.CONTROL, KeyMap.ALT, KeyMap.SHIFT
         routine = actions.Routine
         # These actions are best bound separately to avoid interference with text entry widgets
         actions.add(
-            routine(self.cut, 'STUDIO_CUT', 'Cut selected widget', 'studio', CTRL + CharKey('x')),
-            routine(self.copy, 'STUDIO_COPY', 'Copy selected widget', 'studio', CTRL + CharKey('c')),
-            routine(self.paste, 'STUDIO_PASTE', 'Paste selected widget', 'studio', CTRL + CharKey('v')),
-            routine(self.delete, 'STUDIO_DELETE', 'Delete selected widget', 'studio', KeyMap.DELETE),
-            routine(self.duplicate, 'STUDIO_DUPLICATE', 'Duplicate selected widget', 'studio', CTRL + CharKey('d')),
+            routine(self.cut, 'STUDIO_CUT', _('Cut selected widgets'), 'studio', CTRL + CharKey('x')),
+            routine(self.copy, 'STUDIO_COPY', _('Copy selected widgets'), 'studio', CTRL + CharKey('c')),
+            routine(self.paste, 'STUDIO_PASTE', _('Paste selected widgets'), 'studio', CTRL + CharKey('v')),
+            routine(self.delete, 'STUDIO_DELETE', _('Delete selected widgets'), 'studio', KeyMap.DELETE),
+            routine(self.duplicate, 'STUDIO_DUPLICATE', _('Duplicate selected widgets'), 'studio', CTRL + CharKey('d')),
         )
         self.shortcuts.add_routines(
-            routine(self.undo, 'STUDIO_UNDO', 'Undo last action', 'studio', CTRL + CharKey('Z')),
-            routine(self.redo, 'STUDIO_REDO', 'Redo action', 'studio', CTRL + CharKey('Y')),
+            routine(self.undo, 'STUDIO_UNDO', _('Undo last action'), 'studio', CTRL + CharKey('Z')),
+            routine(self.redo, 'STUDIO_REDO', _('Redo action'), 'studio', CTRL + CharKey('Y')),
+            routine(self.send_back, 'STUDIO_BACK', _('Send selected widgets to back'), 'studio', Symbol(']')),
+            routine(self.bring_front, 'STUDIO_FRONT', _('Bring selected widgets to front'), 'studio', Symbol('[')),
+            routine(
+                lambda: self.send_back(1),
+                'STUDIO_BACK_1', _('Move selected widgets back one step'), 'studio', CTRL + Symbol(']')),
+            routine(
+                lambda: self.bring_front(1),
+                'STUDIO_FRONT_1', _('Bring selected widgets up one step'), 'studio', CTRL + Symbol('[')),
             # -----------------------------
-            routine(self.open_new, 'STUDIO_NEW', 'Open new design', 'studio', CTRL + CharKey('n')),
-            routine(self.open_file, 'STUDIO_OPEN', 'Open design from file', 'studio', CTRL + CharKey('o')),
-            routine(self.save, 'STUDIO_SAVE', 'Save current design', 'studio', CTRL + CharKey('s')),
-            routine(self.save_as, 'STUDIO_SAVE_AS', 'Save current design under a new file', 'studio',
+            routine(self.open_new, 'STUDIO_NEW', _('Open new design'), 'studio', CTRL + CharKey('n')),
+            routine(self.open_file, 'STUDIO_OPEN', _('Open design from file'), 'studio', CTRL + CharKey('o')),
+            routine(self.save, 'STUDIO_SAVE', _('Save current design'), 'studio', CTRL + CharKey('s')),
+            routine(self.save_as, 'STUDIO_SAVE_AS', _('Save current design under a new file'), 'studio',
                     CTRL + SHIFT + CharKey('s')),
-            routine(self.save_all, 'STUDIO_SAVE_ALL', 'Save all open designs', 'studio', CTRL + ALT + CharKey('s')),
-            routine(self.get_help, 'STUDIO_HELP', 'Show studio help', 'studio', KeyMap.F(12)),
-            routine(self.settings, 'STUDIO_SETTINGS', 'Open studio settings', 'studio', ALT + CharKey('s')),
-            routine(restart, 'STUDIO_RESTART', 'Restart application', 'studio', BlankKey),
-            routine(self._on_close, 'STUDIO_EXIT', 'Exit application', 'studio', CTRL + CharKey('q')),
+            routine(self.save_all, 'STUDIO_SAVE_ALL', _('Save all open designs'), 'studio', CTRL + ALT + CharKey('s')),
+            routine(self.get_help, 'STUDIO_HELP', _('Show studio help'), 'studio', KeyMap.F(12)),
+            routine(self.settings, 'STUDIO_SETTINGS', _('Open studio settings'), 'studio', ALT + CharKey('s')),
+            routine(restart, 'STUDIO_RESTART', _('Restart application'), 'studio', BlankKey),
+            routine(self._on_close, 'STUDIO_EXIT', _('Exit application'), 'studio', CTRL + CharKey('q')),
             # ------------------------------
-            routine(self.show_all_windows, 'FEATURE_SHOW_ALL', 'Show all feature windows', 'studio',
+            routine(self.show_all_windows, 'FEATURE_SHOW_ALL', _('Show all feature windows'), 'studio',
                     ALT + CharKey('a')),
-            routine(self.close_all, 'FEATURE_CLOSE_ALL', 'Close all feature windows', 'studio', ALT + CharKey('x')),
+            routine(self.close_all, 'FEATURE_CLOSE_ALL', _('Close all feature windows'), 'studio', ALT + CharKey('x')),
             routine(lambda: self.close_all_on_side('right'),
-                    'FEATURE_CLOSE_RIGHT', 'Close feature windows to the right', 'studio', ALT + CharKey('R')),
+                    'FEATURE_CLOSE_RIGHT', _('Close feature windows to the right'), 'studio', ALT + CharKey('R')),
             routine(lambda: self.close_all_on_side('left'),
-                    'FEATURE_CLOSE_LEFT', 'Close feature windows to the left', 'studio', ALT + CharKey('L')),
-            routine(self.features_as_docked, 'FEATURE_DOCK_ALL', 'Dock all feature windows', 'studio',
+                    'FEATURE_CLOSE_LEFT', _('Close feature windows to the left'), 'studio', ALT + CharKey('L')),
+            routine(self.features_as_docked, 'FEATURE_DOCK_ALL', _('Dock all feature windows'), 'studio',
                     ALT + CharKey('d')),
-            routine(self.features_as_windows, 'FEATURE_UNDOCK_ALL', 'Undock all feature windows', 'studio',
+            routine(self.features_as_windows, 'FEATURE_UNDOCK_ALL', _('Undock all feature windows'), 'studio',
                     ALT + CharKey('u')),
-            routine(self.save_window_positions, 'FEATURE_SAVE_POS', 'Save window positions', 'studio',
+            routine(self.save_window_positions, 'FEATURE_SAVE_POS', _('Save window positions'), 'studio',
                     ALT + SHIFT + CharKey('s')),
             # -----------------------------
-            routine(self.close_context, 'CONTEXT_CLOSE', 'Close tab', 'studio', CTRL + CharKey('T')),
-            routine(self.close_all_contexts, 'CONTEXT_CLOSE_ALL', 'Close all tabs', 'studio',
+            routine(self.close_context, 'CONTEXT_CLOSE', _('Close tab'), 'studio', CTRL + CharKey('T')),
+            routine(self.close_all_contexts, 'CONTEXT_CLOSE_ALL', _('Close all tabs'), 'studio',
                     CTRL + ALT + CharKey('T')),
-            routine(self.close_other_contexts, 'CONTEXT_CLOSE_OTHER', 'Close other tabs', 'studio', BlankKey),
-            routine(self.close_other_contexts_right, 'CONTEXT_CLOSE_OTHER_RIGHT', 'Close all tabs on the right',
+            routine(self.close_other_contexts, 'CONTEXT_CLOSE_OTHER', _('Close other tabs'), 'studio', BlankKey),
+            routine(self.close_other_contexts_right, 'CONTEXT_CLOSE_OTHER_RIGHT', _('Close all tabs on the right'),
                     'studio', BlankKey),
             # -----------------------------
-            routine(self.preview, 'STUDIO_PREVIEW', 'Show preview', 'studio', KeyMap.F(5)),
-            routine(self.close_preview, 'STUDIO_PREVIEW_CLOSE', 'Close any preview', 'studio', ALT + KeyMap.F(5)),
-            routine(self.reload, 'STUDIO_RELOAD', 'Reload current design', 'studio', CTRL + CharKey('R'))
+            routine(self.preview, 'STUDIO_PREVIEW', _('Show preview'), 'studio', KeyMap.F(5)),
+            routine(self.close_preview, 'STUDIO_PREVIEW_CLOSE', _('Close any preview'), 'studio', ALT + KeyMap.F(5)),
+            routine(self.reload, 'STUDIO_RELOAD', _('Reload current design'), 'studio', CTRL + CharKey('R'))
         )
 
 
 def restart():
     exit_success = actions.get_routine("STUDIO_EXIT").invoke()
     if not exit_success:
         return
@@ -916,13 +985,14 @@
     time.sleep(2)
     python = sys.executable
     os.execl(python, python, sys.argv[0])
 
 
 def main():
     # load resources first
+    set_locale(pref.get("locale::language"))
     ResourceLoader.load(pref)
     StudioApplication(className='Formation Studio').mainloop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `formation-studio-0.6.3/studio/parsers/loader.py` & `formation-studio-0.7.0/studio/parsers/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from studio.lib.variables import VariableItem, VariableManager
 from studio.lib import legacy, native
 from studio.lib.menu import menu_config
 from studio.lib.pseudo import Container, PseudoWidget
 from studio.lib.events import make_event
 from studio.lib.layouts import GridLayoutStrategy
 from studio.preferences import Preferences
+from studio.i18n import _
 from formation.loader import _ignore_tags
 from formation.meth import Meth
 from formation.handlers import parse_arg
 import studio
 
 
 def get_widget_impl(widget):
@@ -48,33 +49,41 @@
             component = list(filter(
                 lambda comp: comp.impl.__module__ == module and comp.impl.__name__ == impl,
                 components.custom_widgets,
             ))
             if component:
                 return component[0]
             else:
-                raise ModuleNotFoundError("Could not resolve studio compatible widget for \"{}\"".format(node.type))
+                raise ModuleNotFoundError(_("Could not resolve studio compatible widget for \"{}\"").format(node.type))
         if hasattr(module, impl):
             return getattr(module, impl)
         if impl == 'Panedwindow' and module == native:
             orient = node.attrib.get("attr", {}).get("orient")
             if orient == tk.HORIZONTAL:
                 return native.HorizontalPanedWindow
             return native.VerticalPanedWindow
-        raise NotImplementedError("class {} does not have a designer implementation variant in {}".format(impl, module))
+        raise NotImplementedError(_("class {} does not have a designer implementation variant in {}").format(impl, module))
 
     @classmethod
     def generate(cls, widget: PseudoWidget, parent=None):
         attr = widget.get_altered_options()
         node = Node(parent, get_widget_impl(widget))
         node.attrib['name'] = widget.id
         node["attr"] = attr
         layout_options = widget.layout.get_altered_options_for(widget)
         node["layout"] = layout_options
 
+        scroll_conf = {}
+        if isinstance(getattr(widget, "_cnf_x_scroll", None), PseudoWidget):
+            scroll_conf["x"] = widget._cnf_x_scroll.id
+        if isinstance(getattr(widget, "_cnf_y_scroll", None), PseudoWidget):
+            scroll_conf["y"] = widget._cnf_y_scroll.id
+        if scroll_conf:
+            node["scroll"] = scroll_conf
+
         if hasattr(widget, "_event_map_"):
             for binding in widget._event_map_.values():
                 bind_dict = binding._asdict()
                 # id is not needed and will be recreated on loading
                 bind_dict.pop("id")
                 # convert field values to string
                 bind_dict = {k: str(bind_dict[k]) for k in bind_dict}
@@ -114,33 +123,49 @@
         styles = attrib.get("attr", {})
         if obj_class in (native.VerticalPanedWindow, native.HorizontalPanedWindow):
             # use copy to maintain integrity of XMLForm on pop
             styles = dict(styles)
             if 'orient' in styles:
                 styles.pop('orient')
         layout = attrib.get("layout", {})
-        obj = designer.load(obj_class, attrib["name"], parent, styles, layout, bounds)
+
+        old_id = new_id = attrib["name"]
+        if not designer._is_unique_id(old_id):
+            new_id = designer._get_unique(obj_class)
+        obj = designer.load(obj_class, new_id, parent, styles, layout, bounds)
+
+        # store id cross-mapping for post-processing
+        if old_id != new_id:
+            designer._xlink_map[old_id] = obj
+
+        # load scroll configuration
+        scroll_conf = attrib.get("scroll", {})
+        if scroll_conf.get("x"):
+            obj._cnf_x_scroll = scroll_conf["x"]
+        if scroll_conf.get("y"):
+            obj._cnf_y_scroll = scroll_conf["y"]
+
         for sub_node in node:
             if sub_node.type == "event":
                 binding = make_event(**sub_node.attrib)
                 if not hasattr(obj, "_event_map_"):
                     obj._event_map_ = {}
                 obj._event_map_[binding.id] = binding
             elif sub_node.type == "grid":
                 # we may pop stuff so use a copy
                 sub_attrib = dict(sub_node.attrib)
                 if sub_attrib.get("column"):
                     column = sub_attrib.pop("column")
-                    obj.columnconfigure(column, sub_attrib)
+                    obj.body.columnconfigure(column, sub_attrib)
                     if not hasattr(obj, "_column_conf"):
                         obj._column_conf = set()
                     obj._column_conf.add(int(column))
                 elif sub_attrib.get("row"):
                     row = sub_attrib.pop("row")
-                    obj.rowconfigure(row, sub_attrib)
+                    obj.body.rowconfigure(row, sub_attrib)
                     if not hasattr(obj, "_row_conf"):
                         obj._row_conf = set()
                     obj._row_conf.add(int(row))
             elif sub_node.type == "meth":
                 meth = Meth.from_node(sub_node)
                 meth.call(
                     obj.handle_method,
@@ -255,14 +280,15 @@
         legacy.Tk: MenuStudioAdapter
     }
 
     def __init__(self, designer):
         self.designer = designer
         self.root = None
         self.metadata = {}
+        self._loaded_objs = set()
 
     @classmethod
     def add_adapter(cls, adapter, *obj_classes):
         """
         Connect an external adapter for a specific set of object types to the builder.
         """
         for obj_class in obj_classes:
@@ -285,15 +311,18 @@
     def get_adapter(self, widget_class):
         return self._adapter_map.get(widget_class, BaseStudioAdapter)
 
     def load(self, path, designer):
         self.root = infer_format(path)(path=path).load()
         self._load_meta(self.root)
         self._load_variables(self.root)
-        return self._load_widgets(self.root, designer, designer)
+        self._loaded_objs.clear()
+        root = self._load_widgets(self.root, designer, designer)
+        self._post_process(designer)
+        return root
 
     def _load_meta(self, node):
         for sub_node in node:
             if sub_node.type == 'meta' and sub_node.attrib.get('name'):
                 meta = dict(sub_node.attrib)
                 self.metadata[meta.pop('name')] = meta
 
@@ -308,37 +337,59 @@
         :param parent: Container widget to contain new widget group/section
         :param node: lxml node to be loaded as a widget/group
         :param bounds: tuple of 4 elements describing the intended location of
         the new loaded widget. If left as None, node layout attributes will
         be used instead
         :return:
         """
-        return self._load_widgets(node, self.designer, parent, bounds)
+        self._loaded_objs.clear()
+        root = self._load_widgets(node, self.designer, parent, bounds)
+        self._post_process(self.designer)
+        return root
 
     def _load_widgets(self, node, designer, parent, bounds=None):
         line_info = node.get_source_line_info()
         try:
             adapter = self.get_adapter(BaseStudioAdapter._get_class(node))
             widget = adapter.load(node, designer, parent, bounds)
+            # keep track of loaded objects
+            self._loaded_objs.add(widget)
         except Exception as e:
             # Append line number causing error before re-raising for easier debugging by user
             raise e.__class__("{}{}".format(line_info, e)) from e
         if not isinstance(widget, Container):
-            # We dont need to load child tags of non-container widgets
+            # We don't need to load child tags of non-container widgets
             return widget
         for sub_node in node:
             if sub_node.is_var() or sub_node.type in _ignore_tags:
                 # ignore variables and non widget nodes
                 continue
             if BaseStudioAdapter._get_class(sub_node) == legacy.Menu:
                 continue
             self._load_widgets(sub_node, designer, widget)
-        Meth.call_deferred(designer)
         return widget
 
+    def _post_process(self, designer):
+        # call deferred methods
+        Meth.call_deferred(designer)
+
+        lookup = {}
+        for obj in designer.objects:
+            lookup[obj.id] = obj
+
+        # override lookup with cross-reference map
+        lookup.update(designer._xlink_map)
+        designer._xlink_map.clear()
+
+        for w in self._loaded_objs:
+            if hasattr(w, "_cnf_y_scroll"):
+                w._cnf_y_scroll = lookup.get(w._cnf_y_scroll, '')
+            if hasattr(w, "_cnf_x_scroll"):
+                w._cnf_x_scroll = lookup.get(w._cnf_x_scroll, '')
+
     def to_tree(self, widget, parent=None, with_node=None):
         """
         Convert a PseudoWidget widget and its children to a node
         :param widget: widget to be converted to an xml node
         :param parent: The intended xml node to act as parent to the created
         :param with_node: This node will be used as starting point and no node
             will be created from widget
```

### Comparing `formation-studio-0.6.3/studio/preferences.py` & `formation-studio-0.7.0/studio/preferences.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,265 +56,296 @@
             "underscore": True,
             "case": 'lower',
         }
     },
     "resource": {
         "icon_cache_color": "#ffffff",
         "theme": "default.css"
+    },
+    "locale": {
+        "language": "en"
     }
 }
 
+templates = {}
 
-templates = {
-    "General": {
-        "Appearance": (
-            {
-                "desc": "Theme",
-                "path": "resource::theme",
-                "element": RadioGroup,
-                "requires_restart": True,
-                "extra": {
-                    "choices": (
-                        ("default.css", "Dark",),
-                        ("light.css", "Light",),
-                    )
-                }
-            },
-        ),
-        "Recent Files": (
-            {
-                "desc": "Recent files limit",
-                "path": "studio::recent_max",
-                "element": Number,
-                "extra": {
-                    "width": 4
-                },
-            },
-            {
-                "desc": "Show",
-                "path": "studio::recent_show",
-                "element": RadioGroup,
-                "extra": {
-                    "choices": (
-                        ("name", "Only file name"),
-                        ("path", "Full file path"),
+
+def _templates():
+    from studio.i18n import _
+
+    base = {
+        _("General"): {
+            _("Appearance"): (
+                {
+                    "desc": _("Theme"),
+                    "path": "resource::theme",
+                    "element": RadioGroup,
+                    "requires_restart": True,
+                    "extra": {
+                        "choices": (
+                            ("default.css", _("Dark"),),
+                            ("light.css", _("Light"),),
+                        )
+                    }
+                },
+            ),
+            _("Localization"): (
+                {
+                    "desc": _("Language"),
+                    "path": "locale::language",
+                    "element": Choice,
+                    "requires_restart": True,
+                    "extra": {
+                        "choices": (
+                            ("en", "English"),
+                            ("zh_CN", "Chinese (Simplified) - 简体中文")
+                        )
+                    }
+                },
+            ),
+            _("Recent Files"): (
+                {
+                    "desc": _("Recent files limit"),
+                    "path": "studio::recent_max",
+                    "element": Number,
+                    "extra": {
+                        "width": 4
+                    },
+                },
+                {
+                    "desc": _("Show"),
+                    "path": "studio::recent_show",
+                    "element": RadioGroup,
+                    "extra": {
+                        "choices": (
+                            ("name", _("Only file name")),
+                            ("path", _("Full file path")),
+                        )
+                    }
+                },
+                {
+                    "desc": _("Maximum path display length"),
+                    "path": "studio::recent_max_length",
+                    "element": Number,
+                    "extra": {
+                        "width": 4
+                    },
+                },
+            ),
+            _("Undo Redo"): (
+                DependentGroup({
+                    "controller": {
+                        "desc": _("Limit undo depth"),
+                        "path": "studio::use_undo_depth",
+                        "element": Check
+                    },
+                    "allow": [True, ],
+                    "children": (
+                        {
+                            "desc": _("Undo depth"),
+                            "path": "studio::undo_depth",
+                            "element": Number,
+                            "extra": {
+                                "width": 4,
+                            }
+                        },
                     )
+                }),
+            ),
+            _("Start up"): (
+                {
+                    "desc": _("At startup"),
+                    "path": "studio::on_startup",
+                    "element": RadioGroup,
+                    "extra": {
+                        "choices": (
+                            ("new", _("Open blank design tab")),
+                            ("recent", _("Restore previous tabs")),
+                            ("blank", _("Do not open any design tab"))
+                        )
+                    }
+                },
+            )
+        },
+        _("Designer"): {
+            _("Design pad"): (
+                {
+                    "desc": _("Drag rate throttling"),
+                    "path": "designer::frame_skip",
+                    "element": LabeledScale,
+                    "extra": {
+                        "step": 1,
+                        "_from": 1,
+                        "to": 5,
+                    }
+                },
+            ),
+            _("Naming options"): (
+                {
+                    "desc": _("Naming case"),
+                    "path": "designer::label::case",
+                    "element": RadioGroup,
+                    "extra": {
+                        "choices": (
+                            ("title", _("Title case") + " (Button1, Label_1...)"),
+                            ("lower", _("Lower case") + " (button2, label_2...)"),
+                            ("upper", _("Upper case") + " (BUTTON2, LABEL2...)"),
+                        )
+                    }
+                },
+                {
+                    "desc": _("Use underscore separator"),
+                    "path": "designer::label::underscore",
+                    "element": Check,
+                },
+                {
+                    "desc": _("Start numbering from"),
+                    "path": "designer::label::start",
+                    "element": Number,
+                    "extra": {
+                        "width": 4,
+                        "values": (0, 1)
+                    },
+                },
+                {
+                    "element": Note,
+                    "desc": _("(Widget names already created will not be affected)")
+                },
+            ),
+            _("XML options"): (
+                {
+                    "desc": _("Pretty print output xml"),
+                    "path": "designer::xml::pretty_print",
+                    "element": Check,
+                },
+                {
+                    "element": Note,
+                    "desc": _("(Requires lxml)")
                 }
-            },
-            {
-                "desc": "Maximum path display length",
-                "path": "studio::recent_max_length",
-                "element": Number,
-                "extra": {
-                    "width": 4
-                },
-            },
-        ),
-        "Undo Redo": (
-            DependentGroup({
-                "controller": {
-                    "desc": "Limit undo depth",
-                    "path": "studio::use_undo_depth",
+            ),
+            _("JSON options"): (
+                {
+                    "desc": _("Compact output"),
+                    "path": "designer::json::compact",
                     "element": Check
                 },
-                "allow": [True, ],
-                "children": (
-                    {
-                        "desc": "Undo depth",
-                        "path": "studio::undo_depth",
-                        "element": Number,
-                        "extra": {
-                            "width": 4,
-                        }
+                {
+                    "desc": _("Sort json keys"),
+                    "path": "designer::json::sort_keys",
+                    "element": Check
+                },
+                {
+                    "desc": _("Stringify json values"),
+                    "path": "designer::json::stringify_values",
+                    "element": Check
+                },
+                DependentGroup({
+                    "controller": {
+                        "desc": _("Pretty print output json"),
+                        "path": "designer::json::pretty_print",
+                        "element": Check
                     },
-                )
-            }),
-        ),
-        "Start up": (
-            {
-                "desc": "At startup",
-                "path": "studio::on_startup",
-                "element": RadioGroup,
-                "extra": {
-                    "choices": (
-                        ("new", "Open blank design tab"),
-                        ("recent", "Restore previous tabs"),
-                        ("blank", "Do not open any design tab")
-                    )
-                }
-            },
-        )
-    },
-    "Designer": {
-        "Design pad": (
-            {
-                "desc": "Drag rate throttling",
-                "path": "designer::frame_skip",
-                "element": LabeledScale,
-                "extra": {
-                    "step": 1,
-                    "_from": 1,
-                    "to": 5,
-                }
-            },
-        ),
-        "Naming options": (
-            {
-                "desc": "Naming case",
-                "path": "designer::label::case",
-                "element": RadioGroup,
-                "extra": {
-                    "choices": (
-                        ("title", "Title case (Button1, Label_1...)"),
-                        ("lower", "Lower case (button2, label_2...)"),
-                        ("upper", "Upper case (BUTTON2, LABEL2...)"),
+                    "allow": [True, ],
+                    "children": (
+                        DependentGroup({
+                            "controller": {
+                                "desc": _("For indentation use"),
+                                "path": "designer::json::indent",
+                                "element": RadioGroup,
+                                "extra": {
+                                    "choices": (
+                                        ("\t", _("Tabs")),
+                                        ("", _("Spaces"))
+                                    ),
+                                    "tristatevalue": '-'
+                                }
+                            },
+                            "allow": [""],
+                            "children": (
+                                {
+                                    "desc": _("number of indent spaces"),
+                                    "path": "designer::json::indent_count",
+                                    "element": Number,
+                                    "extra": {
+                                        "width": 4
+                                    }
+                                },
+                            )
+                        }),
                     )
+                })
+            ),
+            _("Image options"): (
+                {
+                    "desc": _("When selecting image"),
+                    "path": "designer::image_path",
+                    "element": RadioGroup,
+                    "extra": {
+                        "choices": (
+                            ("mixed", _("Use relative paths when in same directory as design file")),
+                            ("relative", _("Always use path relative to design file if possible")),
+                            ("absolute", _("Always use absolute paths"))
+                        )
+                    }
+                },
+                {
+                    "element": Note,
+                    "desc": _("(Existing paths will not be affected, Reset the image to take effect)")
                 }
-            },
-            {
-                "desc": "Use underscore separator",
-                "path": "designer::label::underscore",
-                "element": Check,
-            },
-{
-                "desc": "Start numbering from",
-                "path": "designer::label::start",
-                "element": Number,
-                "extra": {
-                    "width": 4,
-                    "values": (0, 1)
-                },
-            },
-            {
-                "element": Note,
-                "desc": "(Widget names already created will not be affected)"
-            },
-        ),
-        "Xml options": (
-            {
-                "desc": "Pretty print output xml",
-                "path": "designer::xml::pretty_print",
-                "element": Check,
-            },
-            {
-                "element": Note,
-                "desc": "(Requires lxml)"
-            }
-        ),
-        "JSON options": (
-            {
-                "desc": "Compact output",
-                "path": "designer::json::compact",
-                "element": Check
-            },
-            {
-                "desc": "Sort json keys",
-                "path": "designer::json::sort_keys",
-                "element": Check
-            },
-            {
-                "desc": "Stringify json values",
-                "path": "designer::json::stringify_values",
-                "element": Check
-            },
-            DependentGroup({
-                "controller": {
-                    "desc": "Pretty print output json",
-                    "path": "designer::json::pretty_print",
+            ),
+            _("Style pane options"): (
+                {
+                    "desc": _("Use descriptive names for style attributes"),
+                    "path": "designer::descriptive_names",
                     "element": Check
                 },
-                "allow": [True, ],
+            )
+        },
+        _("Key Map"): {
+            "_scroll": False,
+            "hotkeys": {
+                "layout": {
+                    "fill": "both",
+                    "expand": True,
+                },
                 "children": (
                     DependentGroup({
                         "controller": {
-                            "desc": "For indentation use",
-                            "path": "designer::json::indent",
-                            "element": RadioGroup,
-                            "extra": {
-                                "choices": (
-                                    ("\t", "Tabs"),
-                                    ("", "Spaces")
-                                ),
-                                "tristatevalue": '-'
-                            }
+                            "desc": _("Allow shortcut keys"),
+                            "path": "allow_hotkeys",
+                            "element": Check,
                         },
-                        "allow": [""],
+                        "allow": [True, ],  # Allow only when controller value is True
                         "children": (
                             {
-                                "desc": "number of indent spaces",
-                                "path": "designer::json::indent_count",
-                                "element": Number,
-                                "extra": {
-                                    "width": 4
+                                "desc": _("Configure shortcut keys"),
+                                "path": "hotkeys",
+                                "element": ShortcutPane,
+                                "layout": {
+                                    "fill": "both",
+                                    "expand": True,
+                                    "padx": 5,
+                                    "pady": 5
                                 }
                             },
                         )
                     }),
                 )
-            })
-        ),
-        "Image options": (
-            {
-                "desc": "When selecting image",
-                "path": "designer::image_path",
-                "element": RadioGroup,
-                "extra": {
-                    "choices": (
-                        ("mixed", "Use relative paths when in same directory as design file"),
-                        ("relative", "Always use path relative to design file if possible"),
-                        ("absolute", "Always use absolute paths")
-                    )
-                }
-            },
-            {
-                "element": Note,
-                "desc": "(Existing paths will not be affected, Reset the image to take effect)"
             }
-        ),
-        "Style pane options": (
-            {
-                "desc": "Use descriptive names for style attributes",
-                "path": "designer::descriptive_names",
-                "element": Check
-            },
-        )
-    },
-    "Key Map": {
-        "_scroll": False,
-        "hotkeys": {
-            "layout": {
-                "fill": "both",
-                "expand": True,
-            },
-            "children": (
-                DependentGroup({
-                    "controller": {
-                        "desc": "Allow shortcut keys",
-                        "path": "allow_hotkeys",
-                        "element": Check,
-                    },
-                    "allow": [True, ],  # Allow only when controller value is True
-                    "children": (
-                        {
-                            "desc": "Configure shortcut keys",
-                            "path": "hotkeys",
-                            "element": ShortcutPane,
-                            "layout": {
-                                "fill": "both",
-                                "expand": True,
-                                "padx": 5,
-                                "pady": 5
-                            }
-                        },
-                    )
-                }),
-            )
         }
     }
-}
+
+    for k in templates:
+        if _(k) in base:
+            base[_(k)].update(templates[k])
+        else:
+            base[k] = templates[k]
+
+    return base
+
 
 class Preferences(SharedPreferences):
 
     @classmethod
     def acquire(cls):
         return cls("formation", "hoverset", "config", defaults)
 
@@ -358,15 +389,15 @@
     def get_latest(self):
         if self.get("studio::recent"):
             return self.get("studio::recent")[0]
         return None
 
 
 def open_preferences(master):
-    PreferenceManager(master, Preferences.acquire(), templates)
+    PreferenceManager(master, Preferences.acquire(), _templates())
 
 
 def get_active_pref(widget):
     import hoverset.ui.widgets as widgets
     if hasattr(widget, 'window') and hasattr(widget.window, 'pref'):
         return widget.window.pref
     else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `formation-studio-0.6.3/studio/resources/images/formation.ico` & `formation-studio-0.7.0/studio/resources/images/formation.ico`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/resources/images/formation.png` & `formation-studio-0.7.0/studio/resources/images/formation.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/resources/images/formation_icon.png` & `formation-studio-0.7.0/studio/resources/images/formation_icon.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/resources/images/logo.png` & `formation-studio-0.7.0/studio/resources/images/logo.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/tools/__init__.py` & `formation-studio-0.7.0/studio/tools/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from studio.tools.menus import MenuTool
 from studio.tools.canvas import CanvasTool
 from studio.tools._base import BaseTool
 
 
 TOOLS = (
     MenuTool,
-    CanvasTool
+    CanvasTool,
 )
 
 
 class ToolManager:
     """
     This class manages all tools dynamically exposing tool functions through toplevel and
     context menus. Add in built tools here
@@ -43,20 +43,20 @@
             template = tool.get_menu(self.studio)
             # If tool does not provide a menu ignore it
             if len(template) < 1:
                 continue
             # if tool has more than one template entry use a cascade menu
             # otherwise use if only a single item is available, use as is
             if len(template) > 1:
-                icon = get_icon_image(tool.icon, 14, 14) if isinstance(tool.icon, str) else tool.icon
+                icon = get_icon_image(tool.icon, 18, 18) if isinstance(tool.icon, str) else tool.icon
                 template = ('cascade', tool.name, icon, None, {'menu': template})
             else:
                 template = template[0]
             templates += (
-                manipulator(partial(tool.supports, self.studio.selected), template),
+                manipulator(partial(tool.supports, self.studio.selection), template),
             )
         # prepend a separator for context menus
         if templates and hide_unsupported:
             templates = (('separator',),) + templates
         return tuple(templates)
 
     def get_tools_as_menu(self):
@@ -82,38 +82,38 @@
                 return tool
 
     def dispatch(self, action, *args):
         # dispatch action to all tools connected
         for tool in self._tools:
             getattr(tool, action)(*args)
 
-    def on_select(self, widget):
-        self.dispatch("on_select", widget)
-
-    def on_widget_delete(self, widget):
-        self.dispatch("on_widget_delete", widget)
+    def on_widgets_delete(self, widgets):
+        self.dispatch("on_widgets_delete", widgets)
 
     def on_app_close(self):
         for tool in self._tools:
             # block app close if any tool returns false
             if not tool.on_app_close():
                 return False
         return True
 
     def on_session_clear(self):
         self.dispatch("on_session_clear")
 
     def on_widget_add(self, widget, parent):
         self.dispatch("on_widget_add", widget, parent)
 
-    def on_widget_change(self, old_widget, new_widget):
-        self.dispatch("on_widget_change", old_widget, new_widget)
+    def on_widgets_change(self, widgets):
+        self.dispatch("on_widgets_change", widgets)
+
+    def on_widgets_layout_change(self, widgets):
+        self.dispatch("on_widgets_layout_change", widgets)
 
-    def on_widget_layout_change(self, widget):
-        self.dispatch("on_widget_layout_change", widget)
+    def on_widgets_reorder(self, indices):
+        self.dispatch("on_widgets_reorder", indices)
 
     def on_context_switch(self):
         self.dispatch("on_context_switch")
 
     def on_context_close(self, context):
         self.dispatch("on_context_close", context)
```

### Comparing `formation-studio-0.6.3/studio/tools/_base.py` & `formation-studio-0.7.0/studio/tools/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,41 +20,42 @@
         icon should be a tk image preferably 14px x 14px
         :param studio:
         :return:
         """
         # default behaviour is to return an empty template
         return ()
 
-    def supports(self, widget):
+    def supports(self, widgets=None):
         """
         Checks whether the tool can work on a given widget. This information is
         useful for the studio to allow it render dropdown menus correctly
-        :param widget: A tk Widget to be checked
+        :param widgets: A list of tk Widgets to be checked, if None, current studio selection is used
         :return: True if tool can work on the widget otherwise false
         """
-
-    def on_select(self, widget):
         pass
 
-    def on_widget_delete(self, widget):
+    def on_widgets_delete(self, widgets):
         pass
 
     def on_app_close(self):
         return True
 
     def on_session_clear(self):
         pass
 
     def on_widget_add(self, widget, parent):
         pass
 
-    def on_widget_change(self, old_widget, new_widget):
+    def on_widgets_change(self, widgets):
+        pass
+
+    def on_widgets_layout_change(self, widgets):
         pass
 
-    def on_widget_layout_change(self, widget):
+    def on_widgets_reorder(self, indices):
         pass
 
     def on_context_switch(self):
         pass
 
     def on_context_close(self, context):
         pass
```

### Comparing `formation-studio-0.6.3/studio/tools/canvas.py` & `formation-studio-0.7.0/studio/tools/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from studio.feature.components import ComponentPane, SelectToDrawGroup
 from studio.feature.stylepane import StyleGroup
 from studio.ui.tree import NestedTreeView
 from studio.lib import NameGenerator
 from studio.lib.canvas import *
 from studio.lib.legacy import Canvas
 from studio.parsers.loader import BaseStudioAdapter, DesignBuilder
+from studio.i18n import _
 
 
 class Coordinate:
     pool = defaultdict(list)
     active = set()
     min_radius = 3
     max_radius = 5
@@ -308,18 +309,18 @@
     _closed = False
 
     def __init__(self, canvas, tool, item=None, **kw):
         super(LinearController, self).__init__(canvas, tool, item, **kw)
         if item:
             self.highlight(item)
         self._link_context = MenuUtils.make_dynamic((
-            ("command", "add point", icon("add", 14, 14), self._add_point, {}),
+            ("command", _("add point"), icon("add", 18, 18), self._add_point, {}),
         ), tool.studio, tool.studio.style)
         self._coord_context = MenuUtils.make_dynamic((
-            ("command", "remove", icon("close", 14, 14), self._remove_point, {}),
+            ("command", _("remove"), icon("close", 18, 18), self._remove_point, {}),
         ), tool.studio, tool.studio.style)
         self._active_link = None
         self._active_coord = None
         self._active_point = None
 
     def on_link_context(self, link, event):
         MenuUtils.popup(event, self._link_context)
@@ -566,26 +567,26 @@
 
 
 class CanvasStyleGroup(StyleGroup):
 
     def __init__(self, master, pane, **cnf):
         self.tool = cnf.pop('tool', None)
         super().__init__(master, pane, **cnf)
-        self.label = "Canvas Item"
+        self.label = _("Canvas Item")
         self.prop_keys = None
         self._prev_prop_keys = set()
-        self._empty_message = "Select canvas item to see styles"
+        self._empty_message = _("Select canvas item to see styles")
 
     @property
     def cv_items(self):
         # selected canvas items
         return self.tool.selected_items
 
-    def supports_widget(self, widget):
-        return isinstance(widget, Canvas)
+    def supports_widgets(self):
+        return len(self.widgets) == 1 and isinstance(self.widgets[0], Canvas)
 
     def can_optimize(self):
         # probably needs a rethink if we consider definition overrides
         # in canvas items but there isn't much of that so this will do
         return self.prop_keys == self._prev_prop_keys
 
     def compute_prop_keys(self):
@@ -600,38 +601,38 @@
                     self.prop_keys = set(item.configure())
                 else:
                     self.prop_keys &= set(item.configure())
             if len(items) > 1:
                 # id cannot be set for multi-selected items
                 self.prop_keys.remove('id')
 
-    def on_widget_change(self, widget):
+    def on_widgets_change(self):
         self._prev_prop_keys = self.prop_keys
         self.compute_prop_keys()
-        super(CanvasStyleGroup, self).on_widget_change(widget)
+        super(CanvasStyleGroup, self).on_widgets_change()
         self.style_pane.remove_loading()
 
     def _get_prop(self, prop, widget):
         # not very useful to us
         return None
 
     def _get_key(self, widget, prop):
         # generate a key identifying the multi-selection state and prop modified
         return f"{','.join(map(lambda x: str(x._id), self.cv_items))}:{prop}"
 
     def _get_action_data(self, widget, prop):
         return {item: {prop: item.cget(prop)} for item in self.cv_items}
 
-    def _apply_action(self, prop, value, widget, data):
+    def _apply_action(self, prop, value, widgets, data):
         for item in data:
             item.configure(data[item])
             if item._controller:
                 item._controller.update()
-        if self.tool.canvas == widget:
-            self.on_widget_change(widget)
+        if self.tool.canvas == widgets[0]:
+            self.on_widgets_change()
         self.tool.on_items_modified(data.keys())
 
     def _set_prop(self, prop, value, widget):
         for item in self.cv_items:
             item.configure({prop: value})
             if item._controller:
                 item._controller.update()
@@ -660,15 +661,15 @@
         def __init__(self, master=None, **config):
             super().__init__(master, **config)
             self.item: CanvasItem = config.get("item")
             self.item.node = self
             self._color = self.style.colors["secondary1"]
             self.name_pad.configure(text=self.item.name)
             self.icon_pad.configure(
-                image=icon(self.item.icon, 15, 15, color=self._color)
+                image=icon(self.item.icon, 15, 15)
             )
             self.editable = True
             self.strict_mode = True
 
         def widget_modified(self, widget):
             self.item = widget
             self.name_pad.configure(text=self.item.name)
@@ -770,21 +771,21 @@
                 component, item=item, canvas=widget, silently=True
             )
         return widget
 
 
 class CanvasTool(BaseTool):
     name = "Canvas"
-    icon = "paint"
+    icon = "object"
 
     def __init__(self, studio, manager):
         super(CanvasTool, self).__init__(studio, manager)
         self._component_pane: ComponentPane = self.studio.get_feature(ComponentPane)
         self.item_select = self._component_pane.register_group(
-            "Canvas", CANVAS_ITEMS, SelectToDrawGroup, self._evaluator
+            _("Canvas"), CANVAS_ITEMS, SelectToDrawGroup, self._evaluator
         )
         self.style_group = studio.style_pane.add_group(
             CanvasStyleGroup, tool=self
         )
 
         CanvasStudioAdapter._tool = self
         # connect the canvas adapter to load canvas objects to the studio
@@ -796,15 +797,15 @@
         self.canvas = None
         self._cursor = "arrow"
         self.current_draw = None
         self.selected_items = []
         self._clipboard = None
         self._latch_pos = 0, 0
 
-        self._image_placeholder = icon("image_dark", 60, 60)
+        self._image_placeholder = icon("image", 60, 60)
 
         self.square_draw = SquareDraw(self)
         self.line_draw = LinearDraw(self)
         self.text_draw = TextDraw(self)
         self.bitmap_draw = PointDraw(self, bitmap="gray25")
         self.image_draw = PointDraw(self, image=self._image_placeholder)
 
@@ -846,39 +847,41 @@
         )
         self.keymap.add_routines(*self.routines)
 
         self._item_context_menu = MenuUtils.make_dynamic((
             EnableIf(
                 lambda: self.selected_items,
                 ("separator",),
-                ("command", "copy", icon("copy", 14, 14), self._get_routine('CV_COPY'), {}),
-                ("command", "duplicate", icon("copy", 14, 14), self._get_routine('CV_DUPLICATE'), {}),
+                ("command", _("copy"), icon("copy", 18, 18), self._get_routine('CV_COPY'), {}),
+                ("command", _("duplicate"), icon("blank", 18, 18), self._get_routine('CV_DUPLICATE'), {}),
                 EnableIf(
                     lambda: self._clipboard is not None,
-                    ("command", "paste", icon("clipboard", 14, 14), self._get_routine('CV_PASTE'), {})
+                    ("command", _("paste"), icon("clipboard", 18, 18), self._get_routine('CV_PASTE'), {})
                 ),
-                ("command", "cut", icon("cut", 14, 14), self._get_routine('CV_CUT'), {}),
+                ("command", _("cut"), icon("cut", 18, 18), self._get_routine('CV_CUT'), {}),
                 ("separator",),
-                ("command", "delete", icon("delete", 14, 14), self._get_routine('CV_DELETE'), {}),
+                ("command", _("delete"), icon("delete", 18, 18), self._get_routine('CV_DELETE'), {}),
                 ("separator",),
-                ("command", "send to back", icon("send_to_back", 14, 14), self._get_routine('CV_BACK'), {}),
-                ("command", "bring to front", icon("bring_to_front", 14, 14), self._get_routine('CV_FRONT'), {}),
-                ("command", "back one step", icon("send_to_back", 14, 14), self._get_routine('CV_BACK_1'), {}),
-                ("command", "forward one step", icon("bring_to_front", 14, 14), self._get_routine('CV_FRONT_1'), {}),
+                ("command", _("send to back"), icon("send_to_back", 18, 18), self._get_routine('CV_BACK'), {}),
+                ("command", _("bring to front"), icon("bring_to_front", 18, 18), self._get_routine('CV_FRONT'), {}),
+                ("command", _("back one step"), icon("send_to_back", 18, 18), self._get_routine('CV_BACK_1'), {}),
+                ("command", _("forward one step"), icon("bring_to_front", 18, 18), self._get_routine('CV_FRONT_1'), {}),
             ),
         ), self.studio, self.studio.style)
 
         self._canvas_menu = MenuUtils.make_dynamic((
             EnableIf(
                 lambda: self._clipboard is not None,
-                ("command", "paste", icon("clipboard", 14, 14),
+                ("command", _("paste"), icon("clipboard", 18, 18),
                  self._get_routine('CV_PASTE'), {})
             ),
         ), self.studio, self.studio.style)
 
+        self.studio.bind("<<SelectionChanged>>", self.on_select, "+")
+
     @property
     def _ids(self):
         return [item.name for item_set in self.items for item in item_set._cv_items]
 
     def initialize_canvas(self, canvas=None):
         canvas = canvas or self.canvas
         if canvas and not getattr(canvas, "_cv_initialized", False):
@@ -1150,20 +1153,20 @@
         controller = getattr(item, "_controller", None)
         if controller:
             controller.release()
         item._controller = None
 
     def selection_changed(self):
         # called when canvas item selection changes
-        self.style_group.on_widget_change(self.canvas)
+        self.style_group.on_widgets_change()
 
     def _update_selection(self, canvas):
         # update selections from the canvas tree
         if canvas != self.canvas:
-            self.studio.select(canvas)
+            self.studio.selection.set(canvas)
         # call to studio should cause canvas to be selected
         assert self.canvas == canvas
         selected = set(self.selected_items)
         to_select = {node.item for node in canvas._cv_tree.get()}
 
         # deselect items currently selected that shouldn't be
         for item in selected - to_select:
@@ -1219,18 +1222,24 @@
                 self.remove_controller(i)
                 i.canvas._cv_tree.deselect(i.node)
             if item in self.selected_items:
                 self.selected_items = [item]
             elif self.set_controller(item):
                 self.selected_items = [item]
                 item.node.select(silently=True)
+            item.node.tree.see(item.node)
 
         self.selection_changed()
 
-    def on_select(self, widget):
+    def on_select(self, _):
+        if len(self.studio.selection) == 1:
+            widget = self.studio.selection[0]
+        else:
+            widget = None
+
         if self.canvas == widget:
             return
         if self.canvas is not None:
             self._reset_cursor()
             self.release(self.canvas)
         if isinstance(widget, Canvas):
             self.canvas = widget
@@ -1267,16 +1276,17 @@
     def on_item_added(self, item):
         item._coord_restore = item.coords()
 
     def on_items_modified(self, items):
         for item in items:
             item.node.widget_modified(item)
 
-    def on_widget_delete(self, widget):
-        if isinstance(widget, Canvas):
-            if widget in self.items:
-                self.items.remove(widget)
+    def on_widgets_delete(self, widgets):
+        for widget in widgets:
+            if isinstance(widget, Canvas):
+                if widget in self.items:
+                    self.items.remove(widget)
 
     def propagate_move(self, delta_x, delta_y, source=None):
         for item in self.selected_items:
             if item != source:
                 item._controller.on_move(delta_x, delta_y, True)
```

### Comparing `formation-studio-0.6.3/studio/tools/menus.py` & `formation-studio-0.7.0/studio/tools/menus.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,33 @@
 from studio.lib.properties import PROPERTY_TABLE, get_properties
 from studio.lib.menu import menu_config, MENU_PROPERTY_TABLE, MENU_PROPERTIES
 from studio.ui.editors import StyleItem
 from studio.ui.tree import MalleableTreeView
 from studio.ui.widgets import CollapseFrame
 from studio.tools._base import BaseToolWindow, BaseTool
 from studio.preferences import get_active_pref
+from studio.i18n import _
 
 
 class MenuTree(MalleableTreeView):
     class Node(MalleableTreeView.Node):
         _type_def = {
             tk.CASCADE: ("menubutton",),
             tk.COMMAND: ("play",),
-            tk.CHECKBUTTON: ("checkbutton",),
-            tk.SEPARATOR: ("division",),
+            tk.CHECKBUTTON: ("checkbox",),
+            tk.SEPARATOR: ("line",),
             tk.RADIOBUTTON: ("radiobutton",),
         }
 
         def __init__(self, tree, **config):
             super().__init__(tree, **config)
             self._menu = config.get("menu")
             self.name_pad.config(text=config.get("label"))
             icon = self._type_def.get(config.get("type"))[0]
-            self.icon_pad.configure(image=get_icon_image(icon, 14, 14))
+            self.icon_pad.configure(image=get_icon_image(icon, 18, 18))
             self.editable = True
             self.type = config.get("type")
             if config.get("type") == tk.CASCADE:
                 self.is_terminal = False
                 menu = config.get("sub_menu") if config.get("sub_menu") else tk.Menu(self.tree._menu, tearoff=False)
                 self._sub_menu = menu
                 self._menu.entryconfigure(config.get("index", tk.END), menu=self._sub_menu)
@@ -152,19 +153,19 @@
             menu_config(self._menu, i, **node._prev_options)
 
 
 class MenuEditor(BaseToolWindow):
     # TODO Add context menu for nodes
     # TODO Add style search
     # TODO Handle widget change from the studio main control
-    _MESSAGE_EDITOR_EMPTY = "No item selected"
+    _MESSAGE_EDITOR_EMPTY = _("No item selected")
 
     def __init__(self, master, widget, menu=None):
         super().__init__(master, widget)
-        self.title(f'Edit menu for {widget.id}')
+        self.title(_('Edit menu for {id}').format(id=widget.id))
         if not isinstance(menu, tk.Menu):
             menu = tk.Menu(widget, tearoff=False)
             widget.configure(menu=menu)
         self._base_menu = menu
         self._tool_bar = Frame(self, **self.style.surface, **self.style.highlight_dim, height=30)
         self._tool_bar.pack(side="top", fill="x")
         self._tool_bar.pack_propagate(False)
@@ -180,43 +181,43 @@
         )
 
         self._editor_pane = ScrolledFrame(self._pane)
         self._editor_pane_cover = Label(self._editor_pane, **self.style.text_passive)
         self._editor_pane.pack(side="top", fill="both", expand=True)
         self._menu_item_styles = CollapseFrame(self._editor_pane.body)
         self._menu_item_styles.pack(side="top", fill="x", pady=4)
-        self._menu_item_styles.label = "Menu Item attributes"
+        self._menu_item_styles.label = _("Menu Item attributes")
         self._menu_styles = CollapseFrame(self._editor_pane.body)
         self._menu_styles.pack(side="top", fill="x", pady=4)
-        self._menu_styles.label = "Menu attributes"
+        self._menu_styles.label = _("Menu attributes")
         self._style_item_ref = {}
         self._menu_style_ref = {}
         self._prev_selection = None
 
         self._add = MenuButton(self._tool_bar, **self.style.button)
         self._add.pack(side="left")
-        self._add.configure(image=get_icon_image("add", 15, 15))
+        self._add.configure(image=get_icon_image("add", 18, 18))
         _types = MenuTree.Node._type_def
         menu_types = self._tool_bar.make_menu(
             [(
                 tk.COMMAND,
                 i.title(),
-                get_icon_image(_types[i][0], 14, 14),
+                get_icon_image(_types[i][0], 18, 18),
                 functools.partial(self.add_item, i), {}
             ) for i in _types],
-            self._add, title="Add menu item")
+            self._add, title=_("Add menu item"))
         menu_types.configure(tearoff=True)
         self._add.config(menu=menu_types)
-        self._delete_btn = Button(self._tool_bar, image=get_icon_image("delete", 15, 15), **self.style.button,
+        self._delete_btn = Button(self._tool_bar, image=get_icon_image("delete", 18, 18), **self.style.button,
                                   width=25,
                                   height=25)
         self._delete_btn.pack(side="left")
         self._delete_btn.on_click(self._delete)
 
-        self._preview_btn = Button(self._tool_bar, image=get_icon_image("play", 15, 15), **self.style.button,
+        self._preview_btn = Button(self._tool_bar, image=get_icon_image("play", 18, 18), **self.style.button,
                                    width=25, height=25)
         self._preview_btn.pack(side="left")
         self._preview_btn.on_click(self._preview)
 
         self._pane.pack(side="top", fill="both", expand=True)
         self._pane.add(self._tree, minsize=350, sticky='nswe', width=350, height=500)
         self._pane.add(self._editor_pane, minsize=320, sticky='nswe', width=320, height=500)
@@ -383,32 +384,33 @@
         widget.configure(menu='')
 
     def restore(self, widget):
         if widget in self._deleted:
             widget.configure(menu=self._deleted.get(widget))
             self._deleted.pop(widget)
 
-    def supports(self, widget):
-        if widget is None:
-            return widget
-        return 'menu' in widget.keys()
+    def supports(self, widgets=None):
+        widgets = widgets or self.studio.selection
+        if not widgets:
+            return False
+        return all('menu' in w.keys() for w in widgets)
 
     def get_menu(self, studio):
         icon = get_icon_image
         return (
-            ('command', 'Edit', icon('edit', 14, 14), lambda: self.edit(studio.selected), {}),
+            ('command', _('Edit'), icon('edit', 18, 18), lambda: self.edit(studio.selection[0]), {}),
             EnableIf(
-                lambda: studio.selected and studio.selected['menu'] != '',
-                ('command', 'Remove', icon('delete', 14, 14), lambda: self.remove(studio.selected), {})),
+                lambda: studio.selection and studio.selection[0]['menu'] != '',
+                ('command', _('Remove'), icon('delete', 18, 18), lambda: self.remove(studio.selection[0]), {})),
             EnableIf(
-                lambda: studio.selected and studio.selected in self._deleted,
-                ('command', 'Restore', icon('undo', 14, 14), lambda: self.restore(studio.selected), {})),
+                lambda: studio.selection and studio.selection[0] in self._deleted,
+                ('command', _('Restore'), icon('undo', 18, 18), lambda: self.restore(studio.selection[0]), {})),
             EnableIf(
                 lambda: MenuEditor._tool_map,
-                ('command', 'Close all editors', icon('close', 14, 14), self.close_editors, {}))
+                ('command', _('Close all editors'), icon('close', 18, 18), self.close_editors, {}))
         )
 
     def on_context_close(self, context):
         for editor in set(MenuTool._editors):
             if editor.context == context:
                 editor.destroy()
                 MenuTool._editors.remove(editor)
```

### Comparing `formation-studio-0.6.3/studio/ui/about.py` & `formation-studio-0.7.0/studio/ui/about.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import platform
 import sys
 import tkinter
 
-from hoverset.ui.widgets import Frame, Label, Application, Hyperlink
+from hoverset.ui.widgets import Frame, Label, Application, Hyperlink, Button, ActionNotifier
 from hoverset.ui.dialogs import MessageDialog
 from hoverset.data.images import load_tk_image
+from hoverset.ui.icons import get_icon_image
 from hoverset.data.utils import get_resource_path
 from hoverset.util import version_description
 
 import formation
 import studio
+from studio.i18n import _
 
 
 class About(Frame):
     class Spec(Frame):
 
         def __init__(self, parent, label, value):
             super().__init__(parent, height=20)
@@ -25,36 +27,62 @@
     def __init__(self, parent):
         super().__init__(parent)
         self.config(**self.style.surface)
         image = load_tk_image(get_resource_path("studio", 'resources/images/logo.png'), 320, 103)
         Label(self, image=image, **self.style.surface).pack(side="top", fill="y", pady=20, padx=50)
         About.Spec(self, "python", sys.version_info)
         About.Spec(self, "tcl/tk", tkinter.TkVersion)
-        About.Spec(self, "loader version", version_description(formation.__version__))
-        About.Spec(self, "studio version", version_description(studio.__version__))
-        About.Spec(self, "Platform", platform.platform())
+        About.Spec(self, _("loader version"), version_description(formation.__version__))
+        About.Spec(self, _("studio version"), version_description(studio.__version__))
+        About.Spec(self, _("Platform"), platform.platform())
+
+        copy_button = Button(
+            self,
+            text=_("  Copy"),
+            height=25,
+            image=get_icon_image("copy", 14, 14),
+            compound="left",
+            **self.style.button,
+        )
+        copy_button.pack(side="top", pady=8)
+        copy_button.configure(width=copy_button.measure_text(_("  Copy")) + 25, **self.style.highlight_active)
+        ActionNotifier.bind_event("<Button-1>", copy_button, self.copy_to_clipboard, text="Copied")
 
         f = Frame(self, **self.style.surface)
         f.pack(side="top", padx=10, pady=3)
         Hyperlink(
-            f, link="https://formation-studio.readthedocs.io/en/latest/", text="doucumentation"
+            f, link="https://formation-studio.readthedocs.io/en/latest/", text=_("doucumentation")
         ).pack(side='left', anchor='e', padx=3)
         Hyperlink(
-            f, link="https://github.com/ObaraEmmanuel/Formation", text="contribute"
+            f, link="https://github.com/ObaraEmmanuel/Formation", text=_("contribute")
         ).pack(side='right', anchor='w', padx=3)
         Hyperlink(
-            f, link="https://github.com/ObaraEmmanuel/Formation/issues", text="report issue"
+            f, link="https://github.com/ObaraEmmanuel/Formation/issues", text=_("report issue")
         ).pack(side='right', anchor='w', padx=3)
 
-        Label(self, text="Make designing user interfaces in python a breeze!",
+        Label(self, text=_("Make designing user interfaces in python a breeze!"),
               **self.style.text).pack(side="top", fill="y", pady=5)
-        copy_right = "Copyright © 2019-2023 Hoverset group"
+        f = Frame(self, **self.style.surface)
+        f.pack(side="top")
+        Label(f, text=_("Icons by"), **self.style.text_passive).pack(side="left")
+        Hyperlink(f, link="https://icons8.com", text="Icons8").pack(side="right")
+        copy_right = _("Copyright © 2019-{year} Hoverset group").format(year="2024")
         Label(self, text=copy_right, **self.style.text_passive).pack(side="top", fill="y")
         self.pack(fill="both", expand=True)
 
+    def copy_to_clipboard(self, _=None):
+        self.clipboard_clear()
+        self.clipboard_append(
+            f"- **Python**: {platform.python_version()} {sys.version_info.releaselevel} {sys.version_info.serial}\n"
+            f"- **Tcl/Tk**: {tkinter.TkVersion}\n"
+            f"- **Loader**: {formation.__version__}\n"
+            f"- **Studio**: {studio.__version__}\n"
+            f"- **Platform**: {platform.platform()}"
+        )
+
 
 def about_window(parent):
     dialog = MessageDialog(parent, About)
     dialog.title("Formation")
     dialog.focus_set()
     return dialog
```

### Comparing `formation-studio-0.6.3/studio/ui/editors.py` & `formation-studio-0.7.0/studio/ui/editors.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Copyright (C) 2019 Hoverset Group.                                      #
 # ======================================================================= #
 import logging
 import os
 import pathlib
 import re
 import sys
+import tkinter as tk
 from tkinter import BooleanVar, filedialog, StringVar
 
 from hoverset.ui.icons import get_icon_image
 from hoverset.ui.panels import FontInput, ColorPicker
 from hoverset.ui.pickers import ColorDialog
 from hoverset.ui.widgets import (CompoundList, Entry, SpinBox, Spinner, Frame, Application,
                                  Label, ToggleButton, Button, Checkbutton, suppress_change)
@@ -372,15 +373,15 @@
     }
 
     def __init__(self, master, style_def=None):
         super().__init__(master, style_def)
         self.config(**self.style.highlight_active)
         self._entry = SpinBox(self, from_=0, to=1e6, **self.style.spinbox)
         self._entry.config(**self.style.no_highlight)
-        self._entry.set_validator(numeric_limit, 0, 1e6)
+        self._entry.set_validator(numeric_limit, 0, None)
         self._entry.on_change(self._change)
         self._unit = Spinner(self, **self.style.input)
         self._unit.config(**self.style.no_highlight, width=50)
         self._unit.set_item_class(Choice.ChoiceItem)
         self._unit.set_values(Duration.UNITS)
         self._unit.pack(side="right")
         self._unit.on_change(self._change)
@@ -460,15 +461,19 @@
 
         if definition.get("negative", False):
             self._entry.set_validator(self._validator())
         else:
             self._entry.set_validator(numeric_limit, 0, None, self._validator())
 
     def _validator(self):
-        return is_numeric if self.style_def.get("float", False) else is_floating_numeric
+        return validate_any(
+            is_numeric if self.style_def.get("float", False) else is_floating_numeric,
+            is_empty,
+            is_signed
+        )
 
     def get(self):
         if self._entry.get() == '':
             return ''
         return f"{self._entry.get()}{Dimension.SHORT_FORMS.get(self._unit.get(), '')}"
 
     @suppress_change
@@ -675,14 +680,65 @@
     def on_var_context_change(self):
         values = [i.var for i in VariableManager.variables() if i.var.__class__ == StringVar]
         self._spinner.set_values((
             '', *values,
         ))
 
 
+class Widget(Choice):
+    _setup_once = False
+
+    class WidgetChoiceItem(Choice.ChoiceItem):
+
+        def render(self):
+            if self.value:
+                item = Label(
+                    self, text=f" {self.value.id}", **self.style.text,
+                    image=get_icon_image(self.value.icon, 15, 15),
+                    compound="left", anchor="w"
+                )
+                item.pack(fill="x")
+            else:
+                Label(self, text="", **self.style.text).pack(fill="x")
+
+    def _get_objs(self):
+        master = tk._default_root
+        if not hasattr(master, "get_widgets"):
+            master = self.winfo_toplevel()
+
+        if hasattr(master, "get_widgets"):
+            include = self.style_def.get("include", ())
+            exclude = self.style_def.get("exclude", ())
+            objs = master.get_widgets()
+            if include:
+                objs = list(filter(lambda x: isinstance(x, tuple(include)), objs))
+            if exclude:
+                objs = list(filter(lambda x: not isinstance(x, tuple(exclude)), objs))
+            return objs
+        return []
+
+    def set_up(self):
+        objs = self._get_objs()
+        self._spinner.set_item_class(Widget.WidgetChoiceItem)
+        self._spinner.set_values((
+            '', *objs,
+        ))
+
+    def set(self, value):
+        if isinstance(value, tk.Widget):
+            self._spinner.set(value)
+            return
+
+        # Override default conversion of value to string by Choice class
+        widget = list(filter(lambda x: x.id == value, self._get_objs()))
+        # if widget does not match anything in the obj list presume as empty
+        value = widget[0] if widget else ''
+        self._spinner.set(value)
+
+
 def get_editor(parent, definition):
     if "compose" in definition:
         type_ = "Compose"
     else:
         type_ = definition.get("type").capitalize()
 
     editor = getattr(sys.modules[__name__], type_, Text)
```

### Comparing `formation-studio-0.6.3/studio/ui/geometry.py` & `formation-studio-0.7.0/studio/ui/geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -82,14 +82,25 @@
     :param widget: Widget to which bounds are to be relative to
     :return: relative bound tuple
     """
     ref = bounds(widget)
     return bd[0] - ref[0], bd[1] - ref[1], bd[2] - ref[0], bd[3] - ref[1]
 
 
+def relative_to_bounds(bound1, bound2):
+    """
+    Convert bounds ``bound1`` to be relative to ``bound2``
+
+    :param bound1: bounds to be converted
+    :param bound2: bounds to which ``bound1`` is to be relative to
+    :return: relative bound tuple
+    """
+    return bound1[0] - bound2[0], bound1[1] - bound2[1], bound1[2] - bound2[0], bound1[3] - bound2[1]
+
+
 def resolve_position(position, widget):
     """
     Convert an absolute position such that it is relative to a ``widget``
 
     :param position: absolute position ``(x, y)`` to be resolved
     :param widget: widget to which position is to be made relative
     :return: position ``(x, y)`` resolved to be relative to ``widget``
@@ -134,26 +145,47 @@
 
     :param bound: a bound tuple
     :return: integer coordinates of center as a tuple ``(x, y)``
     """
     return (bound[2] - bound[0]) // 2, (bound[3] - bound[1]) // 2
 
 
+def displace(bound, dx, dy):
+    """
+    Displace a bound by ``dx`` and ``dy``
+
+    :param bound: a bound tuple
+    :param dx: displacement along x-axis
+    :param dy: displacement along y-axis
+    :return: displaced bound tuple
+    """
+    return bound[0] + dx, bound[1] + dy, bound[2] + dx, bound[3] + dy
+
+
 def is_within(bound1, bound2) -> bool:
     """
     Checks whether bound2 is within bound1 i.e bound1 completely encloses bound2
 
     :param bound1: A tuple, The enclosing bound
     :param bound2: A tuple, The enclosed bound
     :return: ``True`` if ``bound1`` encloses ``bound2`` else ``False``
     """
     overlap = compute_overlap(bound1, bound2)
-    if overlap == bound2:
-        return True
-    return False
+    return overlap == bound2
+
+
+def is_pos_within(bound, pos) -> bool:
+    """
+    Checks whether a position is within a bound
+
+    :param bound: A tuple, The enclosing bound
+    :param pos: A tuple, The position to be checked
+    :return: ``True`` if ``pos`` is within ``bound`` else ``False``
+    """
+    return bound[0] <= pos[0] <= bound[2] and bound[1] <= pos[1] <= bound[3]
 
 
 def dimensions(bound):
     """
     Get the width and height of a bound
 
     :param bound: a bound tuple
@@ -203,14 +235,31 @@
         min_w, min_h = -1, -1
 
     x1, y1, x2, y2 = bound
 
     return x1, y1, x1 + max(min(max_w, x2 - x1), min_w), y1 + max(min(max_h, y2 - y1), min_h)
 
 
+def overall_bounds(bound_list):
+    """
+    Get the bounds of a set of bounds
+
+    :param bound_list: A list of bounds
+    :return: A bound tuple containing the bounds of all the bounds
+        in the list
+    """
+    x1, y1, x2, y2 = float('inf'), float('inf'), -float('inf'), -float('inf')
+    for bound in bound_list:
+        x1 = min(x1, bound[0])
+        y1 = min(y1, bound[1])
+        x2 = max(x2, bound[2])
+        y2 = max(y2, bound[3])
+    return x1, y1, x2, y2
+
+
 def parse_geometry(geometry, default=None):
     """
     Parse a tk geometry string and return a dict with the width, height,
     x any y extracted from it. The geometry string is usually in the form
     ``<width>x<height>(-/+)<x>(-/+)<y>`` for instance ``200x200-10+40``.
     The dimensions part could be missing like in ``+60+67`` or the position
     part like in ``200x200`` or even both. If any of these parts is missing
```

### Comparing `formation-studio-0.6.3/studio/ui/tree.py` & `formation-studio-0.7.0/studio/ui/tree.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.3/studio/ui/widgets.py` & `formation-studio-0.7.0/studio/ui/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,22 +103,24 @@
         self._redraw()
 
     def _redraw(self):
         y = 0
         for feature in self.features:
             indicator = self.features[feature]
             font = FontStyle(self, self.itemconfig(indicator).get("font", "TkDefaultFont")[3])
-            y += font.measure(feature.name) + 20
+            y += font.measure(feature.display_name) + 20
             self.coords(indicator, 18, y)
 
     def add_feature(self, feature):
-        indicator = self.create_text(0, 0, angle=90, text=feature.name, fill=self.style.colors.get("accent"),
-                                     anchor="sw", activefill=self.style.colors.get("primarydarkaccent"))
+        indicator = self.create_text(
+            0, 0, angle=90, text=feature.display_name, fill=self.style.colors.get("accent"),
+            anchor="sw", activefill=self.style.colors.get("primarydarkaccent")
+        )
         font = FontStyle(self, self.itemconfig(indicator).get("font", "TkDefaultFont")[3])
-        y = font.measure(feature.name) + self.bbox("all")[3] + 20
+        y = font.measure(feature.display_name) + self.bbox("all")[3] + 20
         self.coords(indicator, 18, y)
         self.tag_bind(indicator, "<Button-1>", lambda event: self.toggle_feature(feature))
         feature.indicator = indicator
         self.features[feature] = indicator
 
     def change_feature(self, new, old):
         self.tag_unbind(old.indicator, "<Button-1>")
@@ -314,14 +316,19 @@
         self.on_configure()
 
     def forget_child(self, child):
         if self._child_map.get(child) is not None:
             self._frame.delete(self._child_map[child])
             self._child_map.pop(child)
 
+    def lift_child(self, child, above_this=None):
+        above_this = self._child_map[above_this] if above_this in self._child_map else 'all'
+        if self._child_map.get(child) is not None:
+            self._frame.tag_raise(self._child_map[child], above_this)
+
     def configure(self, cnf=None, **kw):
         self._frame.configure(cnf, **kw)
         return super().configure(cnf, **kw)
 
     config = configure
```

### Comparing `formation-studio-0.6.3/studio/updates.py` & `formation-studio-0.7.0/studio/updates.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from hoverset.ui.dialogs import MessageDialog
 from hoverset.ui.widgets import Frame, ProgressBar, Label, Button, Text
 from hoverset.ui.icons import get_icon_image
 from hoverset.util.execution import as_thread
 from hoverset.data.actions import get_routine
 
+from studio.i18n import _
+
 import formation
 
 
 class Updater(Frame):
 
     def __init__(self, master):
         super().__init__(master)
@@ -27,15 +29,15 @@
         self._progress_text.pack(side="top", fill="x", padx=20, pady=10)
         self._message = Label(
             self, **self.style.text,
             anchor="w", compound="left", wrap=400, justify="left",
             pady=5, padx=5,
         )
         self._action_btn = Button(
-            self, text="Retry", **self.style.button_highlight, width=80, height=25
+            self, text=_("Retry"), **self.style.button_highlight, width=80, height=25
         )
         self.extra_info = Text(self, width=40, height=6, state='disabled', font='consolas 10')
         self.pack(fill="both", expand=True)
         self.check_for_update()
 
     def show_button(self, text, func):
         self._action_btn.config(text=text)
@@ -46,82 +48,84 @@
         self.clear_children()
         self._progress_text.configure(text=message)
         self._progress.pack(side="top", fill="x", padx=20, pady=20)
         self._progress_text.pack(side="top", fill="x", padx=20, pady=10)
 
     def show_error(self, message, retry_func):
         self.show_error_plain(message)
-        self.show_button("Retry", retry_func)
+        self.show_button(_("Retry"), retry_func)
 
     def show_error_plain(self, message):
         self.show_message(message, MessageDialog.ICON_ERROR)
 
     def update_found(self, version):
-        self.show_info(f"New version formation-studio {version} found. Do you want to install?")
-        self.show_button("Install", lambda _: self.install(version))
+        self.show_info(
+            _("New version formation-studio {version} found. Do you want to install?").format(version=version)
+        )
+        self.show_button(_("Install"), lambda _: self.install(version))
 
     def show_info(self, message):
         self.show_message(message, MessageDialog.ICON_INFO)
 
     def show_message(self, message, icon):
         self.clear_children()
         self._message.configure(text=message, image=get_icon_image(icon, 50, 50))
         self._message.pack(side="top", padx=20, pady=10)
 
     def install(self, version):
-        self.show_progress(f"Updating to formation-studio {version}")
+        self.show_progress(_("Updating to formation-studio {version}").format(version=version))
         self.upgrade(version)
 
     @classmethod
     def check(cls, master):
         dialog = MessageDialog(master, cls)
-        dialog.title("Formation updater")
+        dialog.title(_("Formation updater"))
         dialog.focus_set()
         return dialog
 
     @as_thread
-    def check_for_update(self, *_):
+    def check_for_update(self, *__):
         self._progress.mode(ProgressBar.INDETERMINATE)
-        self.show_progress("Checking for updates ...")
+        self.show_progress(_("Checking for updates ..."))
         try:
             content = urlopen("https://pypi.org/pypi/formation-studio/json").read()
             data = json.loads(content)
             ver = data["info"]["version"]
             if ver <= formation.__version__:
-                self.show_info("You are using the latest version")
+                self.show_info(_("You are using the latest version"))
             else:
                 self.update_found(ver)
         except URLError:
             self.show_error(
-                "Failed to connect. Check your internet connection"
-                " and try again.",
+                _("Failed to connect. Check your internet connection"
+                " and try again."),
                 self.check_for_update
             )
 
     @as_thread
     def upgrade(self, version):
         try:
             # run formation cli upgrade command
             proc_info = subprocess.run(
                 [sys.executable, "-m", "studio", "-u"],
                 capture_output=True
             )
             if proc_info.returncode != 0 or proc_info.stderr:
                 self.show_error_plain(
-                    "Something went wrong. Failed to upgrade formation-studio"
-                    f" to version {version} ,"
-                    f" Exited with code: {proc_info.returncode}"
+                    _("Something went wrong. Failed to upgrade formation-studio to version {version} Exited with code: {code}").format(
+                        version=version, code=proc_info.returncode
+                    )
                 )
                 if proc_info.stderr:
                     self.extra_info.config(state="normal")
                     self.extra_info.pack(side="top", fill="x", padx=20, pady=10)
                     self.extra_info.clear()
                     self.extra_info.set(str(proc_info.stderr))
                     self.extra_info.config(state="disabled")
             else:
-                self.show_info("Upgrade successful. Restart to complete installation")
-                self.show_button("Restart", lambda _: get_routine("STUDIO_RESTART").invoke())
+                self.show_info(_("Upgrade successful. Restart to complete installation"))
+                self.show_button(_("Restart"), lambda _: get_routine("STUDIO_RESTART").invoke())
                 return
         except Exception as e:
             self.show_error_plain(e)
 
-        self.show_button("Retry", lambda _: self.install(version))
+        self.show_button(_("Retry"), lambda _: self.install(version))
```

