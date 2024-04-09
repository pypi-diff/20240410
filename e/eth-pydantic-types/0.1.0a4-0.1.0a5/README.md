# Comparing `tmp/eth-pydantic-types-0.1.0a4.tar.gz` & `tmp/eth-pydantic-types-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-pydantic-types-0.1.0a4.tar", last modified: Fri Dec  8 16:55:55 2023, max compression
+gzip compressed data, was "eth-pydantic-types-0.1.0a5.tar", last modified: Sat Dec 16 00:25:44 2023, max compression
```

## Comparing `eth-pydantic-types-0.1.0a4.tar` & `eth-pydantic-types-0.1.0a5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.678560 eth-pydantic-types-0.1.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.670560 eth-pydantic-types-0.1.0a4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-08 16:55:55.678560 eth-pydantic-types-0.1.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/methoddocs/address.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/methoddocs/hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/methoddocs/hex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.674560 eth-pydantic-types-0.1.0a4/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.678560 eth-pydantic-types-0.1.0a4/eth_pydantic_types/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/bip122.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/hex.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.678560 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-08 16:55:55.000000 eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 16:55:55.678560 eth-pydantic-types-0.1.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 16:55:55.678560 eth-pydantic-types-0.1.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/tests/test_bip122.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-12-08 16:55:39.000000 eth-pydantic-types-0.1.0a4/tests/test_hex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.917120 eth-pydantic-types-0.1.0a5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.909120 eth-pydantic-types-0.1.0a5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.909120 eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.909120 eth-pydantic-types-0.1.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-16 00:25:44.917120 eth-pydantic-types-0.1.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/methoddocs/address.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/methoddocs/hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/methoddocs/hex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/eth_pydantic_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/bip122.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.913120 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-16 00:25:44.000000 eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-16 00:25:44.917120 eth-pydantic-types-0.1.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:25:44.917120 eth-pydantic-types-0.1.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/tests/test_bip122.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-12-16 00:25:29.000000 eth-pydantic-types-0.1.0a5/tests/test_hex.py
```

### Comparing `eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/bug.md` & `eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/feature.md` & `eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/ISSUE_TEMPLATE/work-item.md` & `eth-pydantic-types-0.1.0a5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/PULL_REQUEST_TEMPLATE.md` & `eth-pydantic-types-0.1.0a5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/release-drafter.yml` & `eth-pydantic-types-0.1.0a5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/codeql.yml` & `eth-pydantic-types-0.1.0a5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/commitlint.yaml` & `eth-pydantic-types-0.1.0a5/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/docs.yaml` & `eth-pydantic-types-0.1.0a5/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/prtitle.yaml` & `eth-pydantic-types-0.1.0a5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/publish.yaml` & `eth-pydantic-types-0.1.0a5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/stale-prs.yml` & `eth-pydantic-types-0.1.0a5/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.github/workflows/test.yaml` & `eth-pydantic-types-0.1.0a5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.gitignore` & `eth-pydantic-types-0.1.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/.pre-commit-config.yaml` & `eth-pydantic-types-0.1.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/LICENSE` & `eth-pydantic-types-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/PKG-INFO` & `eth-pydantic-types-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-pydantic-types
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: eth-pydantic-types: Pydantic Types for Ethereum
 Home-page: https://github.com/ApeWorX/eth-pydantic-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eth-pydantic-types-0.1.0a4/README.md` & `eth-pydantic-types-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/build_docs.py` & `eth-pydantic-types-0.1.0a5/build_docs.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/docs/_static/custom.css` & `eth-pydantic-types-0.1.0a5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/docs/_static/custom.js` & `eth-pydantic-types-0.1.0a5/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/docs/_templates/layout.html` & `eth-pydantic-types-0.1.0a5/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/docs/conf.py` & `eth-pydantic-types-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/docs/favicon.ico` & `eth-pydantic-types-0.1.0a5/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/docs/logo.gif` & `eth-pydantic-types-0.1.0a5/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/__init__.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/_error.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/_error.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/address.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/address.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/bip122.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/bip122.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/hash.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/hash.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/hex.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/hex.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types/validators.py` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,24 +22,37 @@
     elif coerce:
         return validate_size(coerce(value), size)
 
     raise SizeError(size, value)
 
 
 def validate_bytes_size(value: bytes, size: int) -> bytes:
-    return validate_size(value, size, coerce=lambda v: _left_pad_bytes(v, size))
+    return validate_size(value, size, coerce=lambda v: _coerce_hexbytes_size(v, size))
 
 
 def validate_address_size(value: str) -> str:
     return validate_str_size(value, 40)
 
 
 def validate_str_size(value: str, size: int) -> str:
-    return validate_size(value, size, coerce=lambda v: _left_pad_str(v, size))
+    return validate_size(value, size, coerce=lambda v: _coerce_hexstr_size(v, size))
 
 
-def _left_pad_str(val: str, length: int) -> str:
-    return "0" * (length - len(val)) + val if len(val) < length else val
+def _coerce_hexstr_size(val: str, length: int) -> str:
+    val = val.replace("0x", "") if val.startswith("0x") else val
+    if len(val) == length:
+        return val
 
+    val_stripped = val.lstrip("0")
+    num_zeroes = max(0, length - len(val_stripped))
+    zeroes = "0" * num_zeroes
+    return f"{zeroes}{val_stripped}"
 
-def _left_pad_bytes(val: bytes, num_bytes: int) -> bytes:
-    return b"\x00" * (num_bytes - len(val)) + val if len(val) < num_bytes else val
+
+def _coerce_hexbytes_size(val: bytes, num_bytes: int) -> bytes:
+    if len(val) == num_bytes:
+        return val
+
+    val_stripped = val.lstrip(b"\x00")
+    num_zeroes = max(0, num_bytes - len(val_stripped))
+    zeroes = b"\x00" * num_zeroes
+    return zeroes + val_stripped
```

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/PKG-INFO` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-pydantic-types
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: eth-pydantic-types: Pydantic Types for Ethereum
 Home-page: https://github.com/ApeWorX/eth-pydantic-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/SOURCES.txt` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/eth_pydantic_types.egg-info/requires.txt` & `eth-pydantic-types-0.1.0a5/eth_pydantic_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/pyproject.toml` & `eth-pydantic-types-0.1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/setup.py` & `eth-pydantic-types-0.1.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/tests/test_address.py` & `eth-pydantic-types-0.1.0a5/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/tests/test_bip122.py` & `eth-pydantic-types-0.1.0a5/tests/test_bip122.py`

 * *Files identical despite different names*

### Comparing `eth-pydantic-types-0.1.0a4/tests/test_hash.py` & `eth-pydantic-types-0.1.0a5/tests/test_hash.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import pytest
 from pydantic import BaseModel, ValidationError
 
 from eth_pydantic_types.hash import (
     HashBytes8,
     HashBytes16,
+    HashBytes20,
     HashBytes32,
     HashBytes64,
     HashStr8,
     HashStr16,
     HashStr32,
     HashStr64,
 )
 from eth_pydantic_types.hex import HexBytes
 
 
 class Model(BaseModel):
     valuebytes8: HashBytes8
     valuebytes16: HashBytes16
+    valuebytes20: HashBytes20
     valuebytes32: HashBytes32
     valuebytes64: HashBytes64
     valuestr8: HashStr8
     valuestr16: HashStr16
     valuestr32: HashStr32
     valuestr64: HashStr64
 
     @classmethod
     def from_single(cls, value):
         return cls(
             valuebytes8=value,
             valuebytes16=value,
+            valuebytes20=value,
             valuebytes32=value,
             valuebytes64=value,
             valuestr8=value,
             valuestr16=value,
             valuestr32=value,
             valuestr64=value,
         )
@@ -50,14 +53,15 @@
 
 
 @pytest.mark.parametrize("value", ("0x32", HexBytes("0x32"), b"2", 50))
 def test_hash(value):
     model = Model.from_single(value)
     assert len(model.valuebytes8) == 8
     assert len(model.valuebytes16) == 16
+    assert len(model.valuebytes20) == 20
     assert len(model.valuebytes32) == 32
     assert len(model.valuebytes64) == 64
     assert len(model.valuestr8) == 18
     assert len(model.valuestr16) == 34
     assert len(model.valuestr32) == 66
     assert len(model.valuestr64) == 130
     assert model.valuebytes8.hex().endswith("32")
@@ -72,14 +76,27 @@
 
 @pytest.mark.parametrize("value", ("foo", -35, "0x" + ("F" * 100)))
 def test_invalid_hash(value):
     with pytest.raises(ValidationError):
         Model.from_single(value)
 
 
+def test_hash_removes_leading_zeroes_if_needed():
+    address = "0x000000000000000000000000cafac3dd18ac6c6e92c921884f9e4176737c052c"
+
+    class MyModel(BaseModel):
+        my_address: HashBytes20
+
+    # Test both str and bytes for input.
+    for addr in (address, HexBytes(address)):
+        model = MyModel(my_address=addr)
+        assert len(model.my_address) == 20
+        assert model.my_address == HexBytes("0xcafac3dd18ac6c6e92c921884f9e4176737c052c")
+
+
 def test_schema():
     actual = Model.model_json_schema()
     for name, prop in actual["properties"].items():
         is_bytes = "bytes" in name
         if is_bytes:
             size_from_name = int(name.replace("valuebytes", ""))
             expected_length = size_from_name
@@ -104,14 +121,15 @@
 def test_model_dump(bytes32str):
     model = Model.from_single(5)
     actual = model.model_dump()
     expected = {
         "valuebytes8": "0x0000000000000005",
         "valuestr8": "0x0000000000000005",
         "valuebytes16": "0x00000000000000000000000000000005",
+        "valuebytes20": "0x0000000000000000000000000000000000000005",
         "valuestr16": "0x00000000000000000000000000000005",
         "valuebytes32": "0x0000000000000000000000000000000000000000000000000000000000000005",
         "valuestr32": "0x0000000000000000000000000000000000000000000000000000000000000005",
         "valuebytes64": "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000005",  # noqa: E501
         "valuestr64": "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000005",  # noqa: E501
     }
     assert actual == expected
```

### Comparing `eth-pydantic-types-0.1.0a4/tests/test_hex.py` & `eth-pydantic-types-0.1.0a5/tests/test_hex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 from hexbytes import HexBytes as BaseHexBytes
 from pydantic import BaseModel, ValidationError
 
+from eth_pydantic_types import HashStr20
 from eth_pydantic_types.hex import HexBytes, HexStr
 
 
 class BytesModel(BaseModel):
     value: HexBytes
 
 
@@ -111,7 +112,20 @@
     assert actual == expected
 
 
 def test_from_bytes():
     value = b"\xb7\xfc\xef\x7f\xe7E\xf2\xa9U`\xff_U\x0e;\x8f"
     actual = HexStr.from_bytes(value)
     assert actual.startswith("0x")
+
+
+def test_hex_removes_leading_zeroes_if_needed():
+    address = "0x000000000000000000000000cafac3dd18ac6c6e92c921884f9e4176737c052c"
+
+    class MyModel(BaseModel):
+        my_address: HashStr20
+
+    # Test both str and bytes for input.
+    for addr in (address, HexBytes(address)):
+        model = MyModel(my_address=addr)
+        assert len(model.my_address) == 42
+        assert model.my_address == "0xcafac3dd18ac6c6e92c921884f9e4176737c052c"
```

