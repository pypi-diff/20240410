# Comparing `tmp/flake8-async-24.3.6.tar.gz` & `tmp/flake8-async-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-async-24.3.6.tar", last modified: Wed Apr  3 18:39:14 2024, max compression
+gzip compressed data, was "flake8-async-24.4.1.tar", last modified: Wed Apr 10 03:09:32 2024, max compression
```

## Comparing `flake8-async-24.3.6.tar` & `flake8-async-24.4.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.174137 flake8-async-24.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-03 18:39:01.000000 flake8-async-24.3.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-03 18:39:01.000000 flake8-async-24.3.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 18:39:01.000000 flake8-async-24.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:39:01.000000 flake8-async-24.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21686 2024-04-03 18:39:14.174137 flake8-async-24.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-04-03 18:39:10.000000 flake8-async-24.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.154137 flake8-async-24.3.6/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.158137 flake8-async-24.3.6/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-03 18:39:01.000000 flake8-async-24.3.6/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.174137 flake8-async-24.3.6/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21686 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 18:39:14.000000 flake8-async-24.3.6/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-03 18:39:01.000000 flake8-async-24.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:39:14.174137 flake8-async-24.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-03 18:39:01.000000 flake8-async-24.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.162137 flake8-async-24.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.162137 flake8-async-24.3.6/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:14.174137 flake8-async-24.3.6/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async102_aclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async102_aclose_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-03 18:39:01.000000 flake8-async-24.3.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.021136 flake8-async-24.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-10 03:09:20.000000 flake8-async-24.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-10 03:09:20.000000 flake8-async-24.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 03:09:20.000000 flake8-async-24.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 03:09:20.000000 flake8-async-24.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21787 2024-04-10 03:09:32.021136 flake8-async-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-04-10 03:09:29.000000 flake8-async-24.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.005136 flake8-async-24.4.1/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.005136 flake8-async-24.4.1/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32798 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.021136 flake8-async-24.4.1/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21787 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-10 03:09:20.000000 flake8-async-24.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:09:32.021136 flake8-async-24.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-10 03:09:20.000000 flake8-async-24.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.009136 flake8-async-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.009136 flake8-async-24.4.1/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.021136 flake8-async-24.4.1/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29043 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tox.ini
```

### Comparing `flake8-async-24.3.6/CHANGELOG.md` & `flake8-async-24.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+
+## 24.4.1
+- ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
+
 ## 24.3.6
 - ASYNC100 no longer triggers if a context manager contains a `yield`.
 
 ## 24.3.5
 - ASYNC102 (no await inside finally or critical except) no longer raises warnings for calls to `aclose()` on objects in trio/anyio code. See https://github.com/python-trio/flake8-async/issues/156
 
 ## 24.3.4
```

### Comparing `flake8-async-24.3.6/CONTRIBUTING.md` & `flake8-async-24.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/LICENSE` & `flake8-async-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/PKG-INFO` & `flake8-async-24.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.3.6
+Version: 24.4.1
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -105,15 +105,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.3.6
+  rev: 24.4.1
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -217,14 +217,18 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+
+## 24.4.1
+- ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
+
 ## 24.3.6
 - ASYNC100 no longer triggers if a context manager contains a `yield`.
 
 ## 24.3.5
 - ASYNC102 (no await inside finally or critical except) no longer raises warnings for calls to `aclose()` on objects in trio/anyio code. See https://github.com/python-trio/flake8-async/issues/156
 
 ## 24.3.4
```

### Comparing `flake8-async-24.3.6/README.md` & `flake8-async-24.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.3.6
+  rev: 24.4.1
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
```

### Comparing `flake8-async-24.3.6/flake8_async/__init__.py` & `flake8-async-24.4.1/flake8_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.3.6"
+__version__ = "24.4.1"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
```

### Comparing `flake8-async-24.3.6/flake8_async/base.py` & `flake8-async-24.4.1/flake8_async/base.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/runner.py` & `flake8-async-24.4.1/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/__init__.py` & `flake8-async-24.4.1/flake8_async/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/flake8asyncvisitor.py` & `flake8-async-24.4.1/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/helpers.py` & `flake8-async-24.4.1/flake8_async/visitors/helpers.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor100.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor101.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor102.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor103_104.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor105.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor111.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor118.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor2xx.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor2xx.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor91x.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor91x.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,15 +450,15 @@
     #
     # try can jump into any except or into the finally* at any point during it's
     # execution so we need to make sure except & finally can handle worst-case
     # * unless there's a bare except / except BaseException - not implemented.
     def visit_Try(self, node: cst.Try):
         if not self.async_function:
             return
-        self.save_state(node, "try_state")
+        self.save_state(node, "try_state", copy=True)
         # except & finally guaranteed to enter with checkpoint if checkpointed
         # before try and no yield in try body.
         self.try_state.body_uncheckpointed_statements = (
             self.uncheckpointed_statements.copy()
         )
         # yields inside `try` can always be uncheckpointed
         for inner_node in m.findall(node.body, m.Yield()):
@@ -592,14 +592,16 @@
     def visit_While_body(self, node: cst.For | cst.While):
         if not self.async_function:
             return
 
         self.save_state(
             node,
             "uncheckpointed_statements",
+            # reference is overwritten below so don't need to copy
+            copy=False,
         )
 
         # inject an artificial uncheckpointed statement that won't raise an error,
         # but will be marked if an error would be generated. We can then generate
         # appropriate errors if the loop doesn't checkpoint
 
         if getattr(node, "asynchronous", None):
```

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitor_utility.py` & `flake8-async-24.4.1/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async/visitors/visitors.py` & `flake8-async-24.4.1/flake8_async/visitors/visitors.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/flake8_async.egg-info/PKG-INFO` & `flake8-async-24.4.1/flake8_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.3.6
+Version: 24.4.1
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -105,15 +105,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.3.6
+  rev: 24.4.1
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -217,14 +217,18 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+
+## 24.4.1
+- ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
+
 ## 24.3.6
 - ASYNC100 no longer triggers if a context manager contains a `yield`.
 
 ## 24.3.5
 - ASYNC102 (no await inside finally or critical except) no longer raises warnings for calls to `aclose()` on objects in trio/anyio code. See https://github.com/python-trio/flake8-async/issues/156
 
 ## 24.3.4
```

### Comparing `flake8-async-24.3.6/flake8_async.egg-info/SOURCES.txt` & `flake8-async-24.4.1/flake8_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/pyproject.toml` & `flake8-async-24.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/setup.py` & `flake8-async-24.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/autofix_files/async100.py` & `flake8-async-24.4.1/tests/autofix_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/autofix_files/async100_simple_autofix.py` & `flake8-async-24.4.1/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/autofix_files/async910.py` & `flake8-async-24.4.1/tests/autofix_files/async910.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,7 +597,20 @@
 async def await_in_gen_target():
     (print(x) for x in await foo())
 
 
 async def await_everywhere_except_gen_target():  # error: 0, "exit", Statement("function definition", lineno)
     (await x async for x in bar())
     await trio.lowlevel.checkpoint()
+
+
+# Issue #226
+async def fn_226():  # error: 0, "exit", Statement("function definition", lineno)
+    try:
+        while foo():
+            try:
+                await trio.sleep(1)
+            except Exception:
+                pass
+    except Exception:
+        pass
+    await trio.lowlevel.checkpoint()
```

### Comparing `flake8-async-24.3.6/tests/autofix_files/async911.py` & `flake8-async-24.4.1/tests/autofix_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/autofix_files/async91x_autofix.py` & `flake8-async-24.4.1/tests/autofix_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/autofix_files/noqa.py` & `flake8-async-24.4.1/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/conftest.py` & `flake8-async-24.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async100.py` & `flake8-async-24.4.1/tests/eval_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async100_asyncio.py` & `flake8-async-24.4.1/tests/eval_files/async100_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async100_noautofix.py` & `flake8-async-24.4.1/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async100_simple_autofix.py` & `flake8-async-24.4.1/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async101.py` & `flake8-async-24.4.1/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async102.py` & `flake8-async-24.4.1/tests/eval_files/async102.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async102_aclose.py` & `flake8-async-24.4.1/tests/eval_files/async102_aclose.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async102_aclose_args.py` & `flake8-async-24.4.1/tests/eval_files/async102_aclose_args.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async102_anyio.py` & `flake8-async-24.4.1/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async102_asyncio.py` & `flake8-async-24.4.1/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async102_trio.py` & `flake8-async-24.4.1/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async103.py` & `flake8-async-24.4.1/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async103_all_imported.py` & `flake8-async-24.4.1/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async103_both_imported.py` & `flake8-async-24.4.1/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async103_trio.py` & `flake8-async-24.4.1/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async104.py` & `flake8-async-24.4.1/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async104_anyio.py` & `flake8-async-24.4.1/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async105.py` & `flake8-async-24.4.1/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async106.py` & `flake8-async-24.4.1/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async109.py` & `flake8-async-24.4.1/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async110.py` & `flake8-async-24.4.1/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async111.py` & `flake8-async-24.4.1/tests/eval_files/async111.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async112.py` & `flake8-async-24.4.1/tests/eval_files/async112.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async113.py` & `flake8-async-24.4.1/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async113_trio.py` & `flake8-async-24.4.1/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async114.py` & `flake8-async-24.4.1/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async115.py` & `flake8-async-24.4.1/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async116.py` & `flake8-async-24.4.1/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async118.py` & `flake8-async-24.4.1/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async200.py` & `flake8-async-24.4.1/tests/eval_files/async200.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async210.py` & `flake8-async-24.4.1/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async211.py` & `flake8-async-24.4.1/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async212.py` & `flake8-async-24.4.1/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async22x.py` & `flake8-async-24.4.1/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async22x_asyncio.py` & `flake8-async-24.4.1/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async232.py` & `flake8-async-24.4.1/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async232_asyncio.py` & `flake8-async-24.4.1/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async23x.py` & `flake8-async-24.4.1/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async23x_asyncio.py` & `flake8-async-24.4.1/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async240.py` & `flake8-async-24.4.1/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async900.py` & `flake8-async-24.4.1/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async910.py` & `flake8-async-24.4.1/tests/eval_files/async910.py`

 * *Files 4% similar despite different names*

```diff
@@ -568,7 +568,19 @@
 
 async def await_in_gen_target():
     (print(x) for x in await foo())
 
 
 async def await_everywhere_except_gen_target():  # error: 0, "exit", Statement("function definition", lineno)
     (await x async for x in bar())
+
+
+# Issue #226
+async def fn_226():  # error: 0, "exit", Statement("function definition", lineno)
+    try:
+        while foo():
+            try:
+                await trio.sleep(1)
+            except Exception:
+                pass
+    except Exception:
+        pass
```

### Comparing `flake8-async-24.3.6/tests/eval_files/async911.py` & `flake8-async-24.4.1/tests/eval_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async91x_autofix.py` & `flake8-async-24.4.1/tests/eval_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/async91x_noautofix.py` & `flake8-async-24.4.1/tests/eval_files/async91x_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/eval_files/noqa.py` & `flake8-async-24.4.1/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/test_all_visitors_imported.py` & `flake8-async-24.4.1/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/test_changelog_and_version.py` & `flake8-async-24.4.1/tests/test_changelog_and_version.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/test_config_and_args.py` & `flake8-async-24.4.1/tests/test_config_and_args.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/test_decorator.py` & `flake8-async-24.4.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/test_exception_on_invalid_code.py` & `flake8-async-24.4.1/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tests/test_flake8_async.py` & `flake8-async-24.4.1/tests/test_flake8_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,15 @@
             message = error_class.error_codes[err_code + alt_code]
             try:
                 expected.append(Error(err_code, lineno, int(col), message, *args))
             except AttributeError as e:
                 msg = f"Line {lineno}: Failed to format\n {message!r}\nwith\n{args}"
                 raise ParseError(msg) from e
 
+    assert enabled_codes, "no codes enabled. Fix file name or add `# ARGS --enable=...`"
     enabled_codes_list = enabled_codes.split(",")
     for code in enabled_codes_list:
         assert re.fullmatch(
             r"ASYNC\d\d\d", code
         ), f"invalid code {code} in list {enabled_codes_list}"
 
     for error in expected:
```

### Comparing `flake8-async-24.3.6/tests/test_messages_documented.py` & `flake8-async-24.4.1/tests/test_messages_documented.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.6/tox.ini` & `flake8-async-24.4.1/tox.ini`

 * *Files identical despite different names*

