# Comparing `tmp/hexagon-0.58.1.tar.gz` & `tmp/hexagon-0.59.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexagon-0.58.1.tar", last modified: Mon Apr  8 22:18:59 2024, max compression
+gzip compressed data, was "hexagon-0.59.0.tar", last modified: Tue Apr  9 22:58:56 2024, max compression
```

## Comparing `hexagon-0.58.1.tar` & `hexagon-0.59.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/
--rw-r--r--   0 root         (0) root         (0)    27868 2024-04-08 22:18:57.000000 hexagon-0.58.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11345 2024-04-08 22:18:56.000000 hexagon-0.58.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-08 22:18:56.000000 hexagon-0.58.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2576 2024-04-08 22:18:59.637069 hexagon-0.58.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20317 2024-04-08 22:18:56.000000 hexagon-0.58.1/Pipfile.lock
--rw-r--r--   0 root         (0) root         (0)     2080 2024-04-08 22:18:57.000000 hexagon-0.58.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2045 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/__templates/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/__templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/__templates/custom_tool/
--rw-r--r--   0 root         (0) root         (0)     1546 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/__templates/custom_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/external/
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/external/__init__.py
--rw-r--r--   0 root         (0) root         (0)      228 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/external/open_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/actions/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/create_new_tool.py
--rw-r--r--   0 root         (0) root         (0)     2682 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/install_cli.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/replay.py
--rw-r--r--   0 root         (0) root         (0)     2599 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/save_new_alias.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/domain/
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/cli.py
--rw-r--r--   0 root         (0) root         (0)      204 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/env.py
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/errors.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hexagon_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/domain/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      741 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hooks/execution.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hooks/wax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/domain/tool/
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5598 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/dependencies/
--rw-r--r--   0 root         (0) root         (0)      800 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      389 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/fs.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/node.py
--rw-r--r--   0 root         (0) root         (0)     1247 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/execute/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7007 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/action.py
--rw-r--r--   0 root         (0) root         (0)     4600 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/errors.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/execution_hook.py
--rw-r--r--   0 root         (0) root         (0)     3260 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/tool.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/help.py
--rw-r--r--   0 root         (0) root         (0)     2103 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/options.py
--rw-r--r--   0 root         (0) root         (0)     5347 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/parse_args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/plugins/
--rw-r--r--   0 root         (0) root         (0)      861 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/singletons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/update/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/update/changelog/
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/fetch.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/format.py
--rw-r--r--   0 root         (0) root         (0)     2309 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/runtime/update/cli/
--rw-r--r--   0 root         (0) root         (0)     2158 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      693 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/cli/command.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/cli/git.py
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/github.py
--rw-r--r--   0 root         (0) root         (0)     2532 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/hexagon.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/shared.py
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/silent_fail.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/version.py
--rw-r--r--   0 root         (0) root         (0)     3151 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/wax.py
--rw-r--r--   0 root         (0) root         (0)     3480 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/hooks/
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1629 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/hooks/hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/input/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/input/args/
--rw-r--r--   0 root         (0) root         (0)     1504 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1216 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/cli_args.py
--rw-r--r--   0 root         (0) root         (0)     2933 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/hexagon_args.py
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/tool_args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/input/prompt/
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      307 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/for_all_methods.py
--rw-r--r--   0 root         (0) root         (0)     5053 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/hints.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/key_bindings.py
--rw-r--r--   0 root         (0) root         (0)    15635 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/prompt.py
--rw-r--r--   0 root         (0) root         (0)     2525 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/output/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/hexagon/support/output/printer/
--rw-r--r--   0 root         (0) root         (0)      149 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11084 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/en.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/i18n.py
--rw-r--r--   0 root         (0) root         (0)    11833 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/logger.py
--rw-r--r--   0 root         (0) root         (0)     2080 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/themes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/hexagon/support/storage/
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/storage/merge_dictionaries.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/tracer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/hexagon/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/utils/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2576 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3057 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.617069 hexagon-0.58.1/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.617069 hexagon-0.58.1/locales/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/locales/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    11084 2024-04-08 22:18:56.000000 hexagon-0.58.1/locales/en/LC_MESSAGES/hexagon.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.617069 hexagon-0.58.1/locales/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/locales/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    11728 2024-04-08 22:18:56.000000 hexagon-0.58.1/locales/es/LC_MESSAGES/hexagon.mo
--rw-r--r--   0 root         (0) root         (0)      582 2024-04-08 22:18:56.000000 hexagon-0.58.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 22:18:59.637069 hexagon-0.58.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-08 22:18:57.000000 hexagon-0.58.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.777560 hexagon-0.59.0/
+-rw-r--r--   0 root         (0) root         (0)    28060 2024-04-09 22:58:54.000000 hexagon-0.59.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11345 2024-04-09 22:58:53.000000 hexagon-0.59.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-09 22:58:53.000000 hexagon-0.59.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2576 2024-04-09 22:58:56.777560 hexagon-0.59.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20317 2024-04-09 22:58:53.000000 hexagon-0.59.0/Pipfile.lock
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-09 22:58:54.000000 hexagon-0.59.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.761560 hexagon-0.59.0/hexagon/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.761560 hexagon-0.59.0/hexagon/actions/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.761560 hexagon-0.59.0/hexagon/actions/__templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/__templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.761560 hexagon-0.59.0/hexagon/actions/__templates/custom_tool/
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/__templates/custom_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.761560 hexagon-0.59.0/hexagon/actions/external/
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/external/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      228 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/external/open_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.765560 hexagon-0.59.0/hexagon/actions/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/internal/create_new_tool.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/internal/install_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/internal/replay.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/internal/save_new_alias.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/actions/internal/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.765560 hexagon-0.59.0/hexagon/domain/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/cli.py
+-rw-r--r--   0 root         (0) root         (0)      204 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/env.py
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/errors.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/hexagon_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.765560 hexagon-0.59.0/hexagon/domain/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      741 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/hooks/execution.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/hooks/wax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.765560 hexagon-0.59.0/hexagon/domain/tool/
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/domain/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.765560 hexagon-0.59.0/hexagon/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5598 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.765560 hexagon-0.59.0/hexagon/runtime/dependencies/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/dependencies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      389 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/dependencies/fs.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/dependencies/node.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/dependencies/python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.769560 hexagon-0.59.0/hexagon/runtime/execute/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/execute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7007 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/execute/action.py
+-rw-r--r--   0 root         (0) root         (0)     4600 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/execute/errors.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/execute/execution_hook.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/execute/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/help.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/options.py
+-rw-r--r--   0 root         (0) root         (0)     5347 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/parse_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.769560 hexagon-0.59.0/hexagon/runtime/plugins/
+-rw-r--r--   0 root         (0) root         (0)      861 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/singletons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.769560 hexagon-0.59.0/hexagon/runtime/update/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.769560 hexagon-0.59.0/hexagon/runtime/update/changelog/
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/changelog/fetch.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/changelog/format.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/changelog/parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.769560 hexagon-0.59.0/hexagon/runtime/update/cli/
+-rw-r--r--   0 root         (0) root         (0)     2158 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/cli/command.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/cli/git.py
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/github.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/hexagon.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/shared.py
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/silent_fail.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/update/version.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/wax.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/runtime/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.769560 hexagon-0.59.0/hexagon/support/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/hooks/
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/hooks/hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/input/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/input/args/
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/args/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/args/cli_args.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/args/hexagon_args.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/args/tool_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/input/prompt/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/prompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      307 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/prompt/for_all_methods.py
+-rw-r--r--   0 root         (0) root         (0)     5053 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/prompt/hints.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/prompt/key_bindings.py
+-rw-r--r--   0 root         (0) root         (0)    15635 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/prompt/prompt.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/input/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/output/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/output/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/output/printer/
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/output/printer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11084 2024-04-09 22:58:54.000000 hexagon-0.59.0/hexagon/support/output/printer/en.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/output/printer/i18n.py
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/output/printer/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/output/printer/themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.773560 hexagon-0.59.0/hexagon/support/storage/
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/storage/merge_dictionaries.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/support/tracer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.777560 hexagon-0.59.0/hexagon/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-09 22:58:53.000000 hexagon-0.59.0/hexagon/utils/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.761560 hexagon-0.59.0/hexagon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2576 2024-04-09 22:58:56.000000 hexagon-0.59.0/hexagon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3057 2024-04-09 22:58:56.000000 hexagon-0.59.0/hexagon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 22:58:56.000000 hexagon-0.59.0/hexagon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-09 22:58:56.000000 hexagon-0.59.0/hexagon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-09 22:58:56.000000 hexagon-0.59.0/hexagon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-09 22:58:56.000000 hexagon-0.59.0/hexagon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.757560 hexagon-0.59.0/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.757560 hexagon-0.59.0/locales/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.777560 hexagon-0.59.0/locales/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    11084 2024-04-09 22:58:54.000000 hexagon-0.59.0/locales/en/LC_MESSAGES/hexagon.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.757560 hexagon-0.59.0/locales/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 22:58:56.777560 hexagon-0.59.0/locales/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    11728 2024-04-09 22:58:54.000000 hexagon-0.59.0/locales/es/LC_MESSAGES/hexagon.mo
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-09 22:58:53.000000 hexagon-0.59.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 22:58:56.777560 hexagon-0.59.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-09 22:58:54.000000 hexagon-0.59.0/setup.py
```

### Comparing `hexagon-0.58.1/CHANGELOG.md` & `hexagon-0.59.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.59.0 (2024-04-09)
+
+### Feature
+
+* **cli:** Allow configuring entrypoint on install ([`ed75377`](https://github.com/lt-mayonesa/hexagon/commit/ed7537743c6fdfe957a095d7ab51b7302df347ec))
+
 ## v0.58.1 (2024-04-08)
 
 ### Fix
 
 * **install:** Make bin_path optional arg ([`741044a`](https://github.com/lt-mayonesa/hexagon/commit/741044a2244770c18b66dfd972bc1220cab910ad))
 
 ## v0.58.0 (2024-03-30)
```

### Comparing `hexagon-0.58.1/LICENSE` & `hexagon-0.59.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/PKG-INFO` & `hexagon-0.59.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexagon
-Version: 0.58.1
+Version: 0.59.0
 Summary: Build your Team's CLI
 Home-page: https://github.com/lt-mayonesa/hexagon
 Author: Joaco Campero
 Author-email: juacocampero@gmail.com
 Project-URL: Bug Tracker, https://github.com/lt-mayonesa/hexagon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hexagon-0.58.1/Pipfile.lock` & `hexagon-0.59.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/README.md` & `hexagon-0.59.0/README.md`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/__main__.py` & `hexagon-0.59.0/hexagon/__main__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/actions/__templates/custom_tool/__init__.py` & `hexagon-0.59.0/hexagon/actions/__templates/custom_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/actions/internal/create_new_tool.py` & `hexagon-0.59.0/hexagon/actions/internal/create_new_tool.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/actions/internal/install_cli.py` & `hexagon-0.59.0/hexagon/actions/internal/install_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,18 +50,30 @@
     if not bin_path:
         if not cli_args.bin_path.value:
             bin_path = cli_args.bin_path.prompt().resolve()
         store_user_data(HexagonStorageKeys.cli_install_path.value, str(bin_path))
 
     command_path = os.path.join(bin_path, cli.command)
     with open(command_path, "w") as command:
+        pre_command = (
+            cli.entrypoint.pre_command + " " if cli.entrypoint.pre_command else ""
+        )
         command.write(
-            "#!/bin/bash\n"
-            "# file create by hexagon\n"
-            f"HEXAGON_CONFIG_FILE={cli_args.src_path.value.resolve()} hexagon $@"
+            "\n".join(
+                [
+                    f"#!{cli.entrypoint.shell or '/bin/bash'}",
+                    "# file created by hexagon",
+                    f"HEXAGON_CONFIG_FILE={cli_args.src_path.value.resolve()} \\",
+                    *[
+                        f"{key}={value} \\"
+                        for key, value in cli.entrypoint.environ.items()
+                    ],
+                    f"{pre_command}hexagon $@",
+                ]
+            )
         )
 
     _make_executable(command_path)
     scan_and_install_dependencies(configuration.custom_tools_path)
 
     log.info(
         _("msg.actions.internal.install_cli.success"),
```

### Comparing `hexagon-0.58.1/hexagon/actions/internal/replay.py` & `hexagon-0.59.0/hexagon/actions/internal/replay.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/actions/internal/save_new_alias.py` & `hexagon-0.59.0/hexagon/actions/internal/save_new_alias.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/actions/internal/schema.py` & `hexagon-0.59.0/hexagon/actions/internal/schema.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/domain/hexagon_error.py` & `hexagon-0.59.0/hexagon/domain/hexagon_error.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/domain/hooks/execution.py` & `hexagon-0.59.0/hexagon/domain/hooks/execution.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/domain/tool/__init__.py` & `hexagon-0.59.0/hexagon/domain/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/configuration.py` & `hexagon-0.59.0/hexagon/runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/dependencies/__init__.py` & `hexagon-0.59.0/hexagon/runtime/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/dependencies/node.py` & `hexagon-0.59.0/hexagon/runtime/dependencies/node.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/dependencies/python.py` & `hexagon-0.59.0/hexagon/runtime/dependencies/python.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/execute/action.py` & `hexagon-0.59.0/hexagon/runtime/execute/action.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/execute/errors.py` & `hexagon-0.59.0/hexagon/runtime/execute/errors.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/execute/execution_hook.py` & `hexagon-0.59.0/hexagon/runtime/execute/execution_hook.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/execute/tool.py` & `hexagon-0.59.0/hexagon/runtime/execute/tool.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/help.py` & `hexagon-0.59.0/hexagon/runtime/help.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/options.py` & `hexagon-0.59.0/hexagon/runtime/options.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/parse_args.py` & `hexagon-0.59.0/hexagon/runtime/parse_args.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/plugins/__init__.py` & `hexagon-0.59.0/hexagon/runtime/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/changelog/__init__.py` & `hexagon-0.59.0/hexagon/runtime/update/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/changelog/fetch.py` & `hexagon-0.59.0/hexagon/runtime/update/changelog/fetch.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/changelog/format.py` & `hexagon-0.59.0/hexagon/runtime/update/changelog/format.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/changelog/parse.py` & `hexagon-0.59.0/hexagon/runtime/update/changelog/parse.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/cli/__init__.py` & `hexagon-0.59.0/hexagon/runtime/update/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/cli/command.py` & `hexagon-0.59.0/hexagon/runtime/update/cli/command.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/cli/git.py` & `hexagon-0.59.0/hexagon/runtime/update/cli/git.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/hexagon.py` & `hexagon-0.59.0/hexagon/runtime/update/hexagon.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/shared.py` & `hexagon-0.59.0/hexagon/runtime/update/shared.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/update/version.py` & `hexagon-0.59.0/hexagon/runtime/update/version.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/wax.py` & `hexagon-0.59.0/hexagon/runtime/wax.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/runtime/yaml.py` & `hexagon-0.59.0/hexagon/runtime/yaml.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/hooks/__init__.py` & `hexagon-0.59.0/hexagon/support/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/hooks/hook.py` & `hexagon-0.59.0/hexagon/support/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/args/__init__.py` & `hexagon-0.59.0/hexagon/support/input/args/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/args/cli_args.py` & `hexagon-0.59.0/hexagon/support/input/args/cli_args.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/args/hexagon_args.py` & `hexagon-0.59.0/hexagon/support/input/args/hexagon_args.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/args/tool_args.py` & `hexagon-0.59.0/hexagon/support/input/args/tool_args.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/prompt/hints.py` & `hexagon-0.59.0/hexagon/support/input/prompt/hints.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/prompt/key_bindings.py` & `hexagon-0.59.0/hexagon/support/input/prompt/key_bindings.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/prompt/prompt.py` & `hexagon-0.59.0/hexagon/support/input/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/input/types.py` & `hexagon-0.59.0/hexagon/support/input/types.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/output/printer/en.py` & `hexagon-0.59.0/hexagon/support/output/printer/en.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/output/printer/i18n.py` & `hexagon-0.59.0/hexagon/support/output/printer/i18n.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/output/printer/logger.py` & `hexagon-0.59.0/hexagon/support/output/printer/logger.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/output/printer/themes.py` & `hexagon-0.59.0/hexagon/support/output/printer/themes.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/storage/__init__.py` & `hexagon-0.59.0/hexagon/support/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/support/tracer.py` & `hexagon-0.59.0/hexagon/support/tracer.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon/utils/typing.py` & `hexagon-0.59.0/hexagon/utils/typing.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/hexagon.egg-info/PKG-INFO` & `hexagon-0.59.0/hexagon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexagon
-Version: 0.58.1
+Version: 0.59.0
 Summary: Build your Team's CLI
 Home-page: https://github.com/lt-mayonesa/hexagon
 Author: Joaco Campero
 Author-email: juacocampero@gmail.com
 Project-URL: Bug Tracker, https://github.com/lt-mayonesa/hexagon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hexagon-0.58.1/hexagon.egg-info/SOURCES.txt` & `hexagon-0.59.0/hexagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/locales/en/LC_MESSAGES/hexagon.mo` & `hexagon-0.59.0/locales/en/LC_MESSAGES/hexagon.mo`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/locales/es/LC_MESSAGES/hexagon.mo` & `hexagon-0.59.0/locales/es/LC_MESSAGES/hexagon.mo`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/pyproject.toml` & `hexagon-0.59.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexagon-0.58.1/setup.py` & `hexagon-0.59.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import json
 from os.path import dirname
 
 import setuptools
 
 # this updates automatically https://python-semantic-release.readthedocs.io/en/latest/index.html
-__version__ = "0.58.1"
+__version__ = "0.59.0"
 
 
 def __markers(config: dict):
     return f"; {config['markers']}" if "markers" in config else ""
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
```

