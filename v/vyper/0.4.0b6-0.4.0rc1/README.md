# Comparing `tmp/vyper-0.4.0b6.tar.gz` & `tmp/vyper-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.4.0b6.tar", last modified: Sat Apr  6 17:26:01 2024, max compression
+gzip compressed data, was "vyper-0.4.0rc1.tar", last modified: Wed Apr 10 17:15:53 2024, max compression
```

## Comparing `vyper-0.4.0b6.tar` & `vyper-0.4.0rc1.tar`

### file list

```diff
@@ -1,585 +1,585 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.812349 vyper-0.4.0b6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.812349 vyper-0.4.0b6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.812349 vyper-0.4.0b6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-06 17:25:51.000000 vyper-0.4.0b6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 17:25:51.000000 vyper-0.4.0b6/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-06 17:25:51.000000 vyper-0.4.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-06 17:25:51.000000 vyper-0.4.0b6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-06 17:26:01.876349 vyper-0.4.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-06 17:25:51.000000 vyper-0.4.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-06 17:25:51.000000 vyper-0.4.0b6/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (127)    37575 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/vyper-by-example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-06 17:25:51.000000 vyper-0.4.0b6/hooks/build
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 17:25:51.000000 vyper-0.4.0b6/make.cmd
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-06 17:25:51.000000 vyper-0.4.0b6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-04-06 17:25:51.000000 vyper-0.4.0b6/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 17:25:51.000000 vyper-0.4.0b6/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-06 17:26:01.876349 vyper-0.4.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-06 17:25:51.000000 vyper-0.4.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/fixtures/memorymock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.804349 vyper-0.4.0b6/tests/functional/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/builtins/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/codegen/calling_convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    59109 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.828349 vyper-0.4.0b6/tests/functional/codegen/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_blockhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.828349 vyper-0.4.0b6/tests/functional/codegen/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    16176 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    15725 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    33753 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_memory_alloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_flag_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_interface_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_module_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_module_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_stateless_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/storage_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_storage_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_call_graph_stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_selector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_selector_table_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/codegen/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/codegen/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_division.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_exponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_modulo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    50078 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/company/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/company/test_company.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_deploy_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (127)    25198 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/names/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/names/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/names/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/names/test_variable_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_addmulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_external_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_powmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/abi_types/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/abi_types/test_invalid_abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_boolop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_annotate_and_optimize_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_ast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_metadata_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_source_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.808349 vyper-0.4.0b6/tests/unit/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/cli/storage_layout/
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_source_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_convert_basicblock_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_dominator_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_duplicate_operands.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_liveness_simple_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_multi_entry_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_stack_at_external_return.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/tests/unit/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/tests/unit/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/utils/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    45995 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    90791 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC165.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC20.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC20Detailed.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC4626.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC721.vyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10389 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/vyper_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    43348 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/jumptable_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.872349 vyper-0.4.0b6/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45834 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.872349 vyper-0.4.0b6/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.872349 vyper-0.4.0b6/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37194 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/vyper/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/basicblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/bb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/dominators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/ir_node_to_venom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/vyper/venom/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/base_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/constant_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/simplify_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/stack_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/stack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/venom_to_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 17:25:59.000000 vyper-0.4.0b6/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.817755 vyper-0.4.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.817755 vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.817755 vyper-0.4.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38035 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/testing-contracts-ethtester.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/vyper-by-example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/hooks/build
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19787 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/fixtures/memorymock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.809755 vyper-0.4.0rc1/tests/functional/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.829755 vyper-0.4.0rc1/tests/functional/builtins/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20923 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.829755 vyper-0.4.0rc1/tests/functional/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.833755 vyper-0.4.0rc1/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.833755 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59140 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.833755 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_blockhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_memory_alloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.841755 vyper-0.4.0rc1/tests/functional/codegen/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_flag_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_interface_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_stateless_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.841755 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_storage_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_call_graph_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_selector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_selector_table_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.841755 vyper-0.4.0rc1/tests/functional/codegen/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_exponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_modulo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50402 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23876 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/company/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.853755 vyper-0.4.0rc1/tests/functional/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_deploy_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/names/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/names/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/names/test_variable_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_addmulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_external_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_powmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/unit/abi_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/abi_types/test_invalid_abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_annotate_and_optimize_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_ast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_metadata_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_source_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.809755 vyper-0.4.0rc1/tests/unit/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/cli/storage_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_source_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_convert_basicblock_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_duplicate_operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_liveness_simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_multi_entry_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_stack_at_external_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/utils/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.873755 vyper-0.4.0rc1/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45995 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.873755 vyper-0.4.0rc1/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91096 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.873755 vyper-0.4.0rc1/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC165.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC20.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC20Detailed.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC4626.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC721.vyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.877755 vyper-0.4.0rc1/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10533 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/vyper_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.877755 vyper-0.4.0rc1/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42565 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.877755 vyper-0.4.0rc1/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/jumptable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45834 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.885755 vyper-0.4.0rc1/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37194 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35107 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.885755 vyper-0.4.0rc1/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.885755 vyper-0.4.0rc1/vyper/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/basicblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/bb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/dominators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/ir_node_to_venom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/vyper/venom/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/base_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/constant_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/simplify_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/stack_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/stack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/venom_to_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 17:15:50.000000 vyper-0.4.0rc1/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.4.0b6/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/build.yml` & `vyper-0.4.0rc1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/codeql.yml` & `vyper-0.4.0rc1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/era-tester.yml` & `vyper-0.4.0rc1/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/ghcr.yml` & `vyper-0.4.0rc1/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/pull-request.yaml` & `vyper-0.4.0rc1/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/release-pypi.yml` & `vyper-0.4.0rc1/.github/workflows/release-pypi.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.github/workflows/test.yml` & `vyper-0.4.0rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/.pre-commit-config.yaml` & `vyper-0.4.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/Dockerfile` & `vyper-0.4.0rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/LICENSE` & `vyper-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/Makefile` & `vyper-0.4.0rc1/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/PKG-INFO` & `vyper-0.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0b6
+Version: 0.4.0rc1
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0b6/README.md` & `vyper-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/SECURITY.md` & `vyper-0.4.0rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/Makefile` & `vyper-0.4.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/_templates/versions.html` & `vyper-0.4.0rc1/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/built-in-functions.rst` & `vyper-0.4.0rc1/docs/built-in-functions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -129,21 +129,22 @@
     * Performs an ``EXTCODESIZE`` check to check there is code at ``target``
 * ``create_from_blueprint(target: address, ...)``
     * Deploys a contract using the initcode stored at ``target``
     * Cheap to call (no ``DELEGATECALL`` overhead), expensive to create (200 gas per deployed byte)
     * Invokes constructor, requires a special "blueprint" contract to be deployed
     * Performs an ``EXTCODESIZE`` check to check there is code at ``target``
 
-.. py:function:: create_minimal_proxy_to(target: address, value: uint256 = 0[, salt: bytes32]) -> address
+.. py:function:: create_minimal_proxy_to(target: address, value: uint256 = 0, revert_on_failure: bool = True[, salt: bytes32]) -> address
 
     Deploys a small, EIP1167-compliant "minimal proxy contract" that duplicates the logic of the contract at ``target``, but has its own state since every call to ``target`` is made using ``DELEGATECALL`` to ``target``. To the end user, this should be indistinguishable from an independently deployed contract with the same code as ``target``.
 
 
     * ``target``: Address of the contract to proxy to
     * ``value``: The wei value to send to the new contract address (Optional, default 0)
+    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the null address.
     * ``salt``: A ``bytes32`` value utilized by the deterministic ``CREATE2`` opcode (Optional, if not supplied, ``CREATE`` is used)
 
     Returns the address of the newly created proxy contract. If the create operation fails (for instance, in the case of a ``CREATE2`` collision), execution will revert.
 
     .. code-block:: vyper
 
         @external
@@ -159,20 +160,21 @@
   There is no runtime check that there is code already deployed at ``target`` (since a proxy may be deployed counterfactually). Most applications may want to insert this check.
 
 .. note::
 
   Before version 0.3.4, this function was named ``create_forwarder_to``.
 
 
-.. py:function:: create_copy_of(target: address, value: uint256 = 0[, salt: bytes32]) -> address
+.. py:function:: create_copy_of(target: address, value: uint256 = 0, revert_on_failure: bool = True[, salt: bytes32]) -> address
 
     Create a physical copy of the runtime code at ``target``. The code at ``target`` is byte-for-byte copied into a newly deployed contract.
 
     * ``target``: Address of the contract to copy
     * ``value``: The wei value to send to the new contract address (Optional, default 0)
+    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the null address.
     * ``salt``: A ``bytes32`` value utilized by the deterministic ``CREATE2`` opcode (Optional, if not supplied, ``CREATE`` is used)
 
     Returns the address of the created contract. If the create operation fails (for instance, in the case of a ``CREATE2`` collision), execution will revert. If there is no code at ``target``, execution will revert.
 
     .. code-block:: vyper
 
         @external
@@ -180,23 +182,24 @@
             return create_copy_of(target)
 
 .. note::
 
     The implementation of ``create_copy_of`` assumes that the code at ``target`` is smaller than 16MB. While this is much larger than the EIP-170 constraint of 24KB, it is a conservative size limit intended to future-proof deployer contracts in case the EIP-170 constraint is lifted. If the code at ``target`` is larger than 16MB, the behavior of ``create_copy_of`` is undefined.
 
 
-.. py:function:: create_from_blueprint(target: address, *args, value: uint256 = 0, raw_args: bool = False, code_offset: int = 3, [, salt: bytes32]) -> address
+.. py:function:: create_from_blueprint(target: address, *args, value: uint256 = 0, raw_args: bool = False, code_offset: int = 3, revert_on_failure: bool = True[, salt: bytes32]) -> address
 
     Copy the code of ``target`` into memory and execute it as initcode. In other words, this operation interprets the code at ``target`` not as regular runtime code, but directly as initcode. The ``*args`` are interpreted as constructor arguments, and are ABI-encoded and included when executing the initcode.
 
     * ``target``: Address of the blueprint to invoke
     * ``*args``: Constructor arguments to forward to the initcode.
     * ``value``: The wei value to send to the new contract address (Optional, default 0)
     * ``raw_args``: If ``True``, ``*args`` must be a single ``Bytes[...]`` argument, which will be interpreted as a raw bytes buffer to forward to the create operation (which is useful for instance, if pre- ABI-encoded data is passed in from elsewhere). (Optional, default ``False``)
     * ``code_offset``: The offset to start the ``EXTCODECOPY`` from (Optional, default 3)
+    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the null address.
     * ``salt``: A ``bytes32`` value utilized by the deterministic ``CREATE2`` opcode (Optional, if not supplied, ``CREATE`` is used)
 
     Returns the address of the created contract. If the create operation fails (for instance, in the case of a ``CREATE2`` collision), execution will revert. If ``code_offset >= target.codesize`` (ex. if there is no code at ``target``), execution will revert.
 
     .. code-block:: vyper
 
         @external
```

### Comparing `vyper-0.4.0b6/docs/compiler-exceptions.rst` & `vyper-0.4.0rc1/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/compiling-a-contract.rst` & `vyper-0.4.0rc1/docs/compiling-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/conf.py` & `vyper-0.4.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/constants-and-vars.rst` & `vyper-0.4.0rc1/docs/constants-and-vars.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/contributing.rst` & `vyper-0.4.0rc1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/control-structures.rst` & `vyper-0.4.0rc1/docs/control-structures.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/deploying-contracts.rst` & `vyper-0.4.0rc1/docs/deploying-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/event-logging.rst` & `vyper-0.4.0rc1/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/index.rst` & `vyper-0.4.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/installing-vyper.rst` & `vyper-0.4.0rc1/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/interfaces.rst` & `vyper-0.4.0rc1/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/logo.svg` & `vyper-0.4.0rc1/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/make.bat` & `vyper-0.4.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/natspec.rst` & `vyper-0.4.0rc1/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/release-notes.rst` & `vyper-0.4.0rc1/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/resources.rst` & `vyper-0.4.0rc1/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/scoping-and-declarations.rst` & `vyper-0.4.0rc1/docs/scoping-and-declarations.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/statements.rst` & `vyper-0.4.0rc1/docs/statements.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/structure-of-a-contract.rst` & `vyper-0.4.0rc1/docs/structure-of-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/style-guide.rst` & `vyper-0.4.0rc1/docs/style-guide.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/testing-contracts-brownie.rst` & `vyper-0.4.0rc1/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/testing-contracts-ethtester.rst` & `vyper-0.4.0rc1/docs/testing-contracts-ethtester.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/testing-contracts.rst` & `vyper-0.4.0rc1/docs/testing-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/toctree.rst` & `vyper-0.4.0rc1/docs/toctree.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/types.rst` & `vyper-0.4.0rc1/docs/types.rst`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 Values
 ******
 
 A value with a precision of 10 decimal places between -18707220957835557353007165858768422651595.9365500928 (-2\ :sup:`167` / 10\ :sup:`10`) and 18707220957835557353007165858768422651595.9365500927 ((2\ :sup:`167` - 1) / 10\ :sup:`10`).
 
 In order for a literal to be interpreted as ``decimal`` it must include a decimal point.
 
-The ABI type (for computing method identifiers) of ``decimal`` is ``fixed168x10``.
+The ABI type (for computing method identifiers) of ``decimal`` is ``int168``.
 
 Operators
 *********
 
 Comparisons
 ^^^^^^^^^^^
```

### Comparing `vyper-0.4.0b6/docs/versioning.rst` & `vyper-0.4.0rc1/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/docs/vyper-by-example.rst` & `vyper-0.4.0rc1/docs/vyper-by-example.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/auctions/blind_auction.vy` & `vyper-0.4.0rc1/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/auctions/simple_open_auction.vy` & `vyper-0.4.0rc1/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/crowdfund.vy` & `vyper-0.4.0rc1/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/factory/Exchange.vy` & `vyper-0.4.0rc1/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/factory/Factory.vy` & `vyper-0.4.0rc1/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.4.0rc1/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.4.0rc1/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/stock/company.vy` & `vyper-0.4.0rc1/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/tokens/ERC1155ownable.vy` & `vyper-0.4.0rc1/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/tokens/ERC20.vy` & `vyper-0.4.0rc1/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/tokens/ERC4626.vy` & `vyper-0.4.0rc1/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/tokens/ERC721.vy` & `vyper-0.4.0rc1/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/voting/ballot.vy` & `vyper-0.4.0rc1/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/examples/wallet/wallet.vy` & `vyper-0.4.0rc1/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/make.cmd` & `vyper-0.4.0rc1/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/setup.cfg` & `vyper-0.4.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/setup.py` & `vyper-0.4.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/conftest.py` & `vyper-0.4.0rc1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 from eth_utils import setup_DEBUG2_logging
 from eth_utils.toolz import compose
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.contract import Contract
 from web3.providers.eth_tester import EthereumTesterProvider
 
+import vyper.compiler.settings as compiler_settings
 import vyper.evm.opcodes as evm
 from tests.utils import working_directory
 from vyper import compiler
 from vyper.ast.grammar import parse_vyper_source
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.input_bundle import FilesystemInputBundle, InputBundle
-from vyper.compiler.settings import OptimizationLevel, Settings, _set_debug_mode
-from vyper.evm.opcodes import version_check
+from vyper.compiler.settings import (
+    OptimizationLevel,
+    Settings,
+    get_global_settings,
+    set_global_settings,
+)
+from vyper.evm.opcodes import EVM_VERSIONS, version_check
 from vyper.exceptions import EvmVersionException
 from vyper.ir import compile_ir, optimizer
 from vyper.utils import ERC5202_PREFIX, keccak256
 
 # Import the base fixtures
 pytest_plugins = ["tests.fixtures.memorymock"]
 
@@ -61,15 +67,15 @@
         help="change optimization mode",
     )
     parser.addoption("--enable-compiler-debug-mode", action="store_true")
     parser.addoption("--experimental-codegen", action="store_true")
 
     parser.addoption(
         "--evm-version",
-        choices=list(evm.EVM_VERSIONS.keys()),
+        choices=list(EVM_VERSIONS.keys()),
         default="shanghai",
         help="set evm version",
     )
 
 
 @pytest.fixture(scope="module")
 def output_formats():
@@ -77,34 +83,57 @@
     del output_formats["bb"]
     del output_formats["bb_runtime"]
     del output_formats["cfg"]
     del output_formats["cfg_runtime"]
     return output_formats
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture(scope="session")
 def optimize(pytestconfig):
     flag = pytestconfig.getoption("optimize")
     return OptimizationLevel.from_string(flag)
 
 
-@pytest.fixture(scope="session", autouse=True)
+@pytest.fixture(scope="session")
 def debug(pytestconfig):
     debug = pytestconfig.getoption("enable_compiler_debug_mode")
     assert isinstance(debug, bool)
-    _set_debug_mode(debug)
+    return debug
 
 
 @pytest.fixture(scope="session")
 def experimental_codegen(pytestconfig):
     ret = pytestconfig.getoption("experimental_codegen")
     assert isinstance(ret, bool)
     return ret
 
 
+@pytest.fixture(scope="session")
+def evm_version(pytestconfig):
+    # note: we configure the evm version that we emit code for,
+    # but eth-tester is only configured with the latest mainnet
+    # version. luckily, evms are backwards compatible.
+    evm_version_str = pytestconfig.getoption("evm_version")
+    assert isinstance(evm_version_str, str)
+    return evm_version_str
+
+
+@pytest.fixture(scope="session", autouse=True)
+def global_settings(evm_version, experimental_codegen, optimize, debug):
+    evm.DEFAULT_EVM_VERSION = evm_version
+    compiler_settings.DEFAULT_ENABLE_DECIMALS = True
+    settings = Settings(
+        optimize=optimize,
+        evm_version=evm_version,
+        experimental_codegen=experimental_codegen,
+        debug=debug,
+    )
+    set_global_settings(settings)
+
+
 @pytest.fixture(autouse=True)
 def check_venom_xfail(request, experimental_codegen):
     if not experimental_codegen:
         return
 
     marker = request.node.get_closest_marker("venom_xfail")
     if marker is None:
@@ -120,26 +149,14 @@
         if not experimental_codegen:
             return
         request.node.add_marker(pytest.mark.xfail(*args, strict=True, **kwargs))
 
     return _xfail
 
 
-@pytest.fixture(scope="session", autouse=True)
-def evm_version(pytestconfig):
-    # note: we configure the evm version that we emit code for,
-    # but eth-tester is only configured with the latest mainnet
-    # version.
-    evm_version_str = pytestconfig.getoption("evm_version")
-    evm.DEFAULT_EVM_VERSION = evm_version_str
-    # this should get overridden by anchor_evm_version,
-    # but set it anyway
-    evm.active_evm_version = evm.EVM_VERSIONS[evm_version_str]
-
-
 @pytest.fixture
 def chdir_tmp_path(tmp_path):
     # this is useful for when you want imports to have relpaths
     with working_directory(tmp_path):
         yield
 
 
@@ -360,15 +377,15 @@
     experimental_codegen,
     output_formats,
     *args,
     override_opt_level=None,
     input_bundle=None,
     **kwargs,
 ):
-    settings = Settings()
+    settings = get_global_settings()
     settings.optimize = override_opt_level or optimize
     settings.experimental_codegen = experimental_codegen
     out = compiler.compile_code(
         source_code,
         # test that all output formats can get generated
         output_formats=output_formats,
         settings=settings,
```

### Comparing `vyper-0.4.0b6/tests/fixtures/memorymock.py` & `vyper-0.4.0rc1/tests/fixtures/memorymock.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_decode.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from decimal import Decimal
-
 import pytest
 from eth.codecs import abi
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import ArgumentException, StackTooDeep, StructureException
 
 TEST_ADDR = "0x" + b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
 
 
 def test_abi_decode_complex(get_contract):
     contract = """
@@ -50,30 +49,36 @@
     human = _abi_decode(x, Human)
     return human
     """
 
     c = get_contract(contract)
 
     test_bytes32 = b"".join(chr(i).encode("utf-8") for i in range(32))
-    args = (TEST_ADDR, -1, True, Decimal("-123.4"), test_bytes32)
-    encoding = "(address,int128,bool,fixed168x10,bytes32)"
+    args = (TEST_ADDR, -1, True, decimal_to_int("-123.4"), test_bytes32)
+    encoding = "(address,int128,bool,int168,bytes32)"
     encoded = abi.encode(encoding, args)
-    assert tuple(c.abi_decode(encoded)) == (TEST_ADDR, -1, True, Decimal("-123.4"), test_bytes32)
+    assert tuple(c.abi_decode(encoded)) == (
+        TEST_ADDR,
+        -1,
+        True,
+        decimal_to_int("-123.4"),
+        test_bytes32,
+    )
 
     test_bytes32 = b"".join(chr(i).encode("utf-8") for i in range(32))
     human_tuple = (
         "foobar",
-        ("vyper", TEST_ADDR, 123, True, Decimal("123.4"), [123, 456, 789], test_bytes32),
+        ("vyper", TEST_ADDR, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
     )
     args = tuple([human_tuple[0]] + list(human_tuple[1]))
-    human_t = "((string,(string,address,int128,bool,fixed168x10,uint256[3],bytes32)))"
+    human_t = "((string,(string,address,int128,bool,int168,uint256[3],bytes32)))"
     human_encoded = abi.encode(human_t, (human_tuple,))
     assert tuple(c.abi_decode_struct(human_encoded)) == (
         "foobar",
-        ("vyper", TEST_ADDR, 123, True, Decimal("123.4"), [123, 456, 789], test_bytes32),
+        ("vyper", TEST_ADDR, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
     )
 
 
 @pytest.mark.parametrize(
     "expected,input_len,output_typ,abi_typ,unwrap_tuple",
     [
         (123, 32, "uint256", "uint256", False),
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_encode.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from decimal import Decimal
-
 import pytest
 from eth.codecs import abi
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import StackTooDeep
 
 
 # @pytest.mark.parametrize("string", ["a", "abc", "abcde", "potato"])
 def test_abi_encode(get_contract):
     code = """
 struct Animal:
@@ -105,18 +104,18 @@
         c.abi_encode2(arg, True, True).hex() == (method_id + abi.encode("(string)", (arg,))).hex()
     )
 
     test_addr = "0x" + b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
     test_bytes32 = b"".join(chr(i).encode("utf-8") for i in range(32))
     human_tuple = (
         "foobar",
-        ("vyper", test_addr, 123, True, Decimal("123.4"), [123, 456, 789], test_bytes32),
+        ("vyper", test_addr, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
     )
     args = tuple([human_tuple[0]] + list(human_tuple[1]))
-    human_t = "(string,(string,address,int128,bool,fixed168x10,uint256[3],bytes32))"
+    human_t = "(string,(string,address,int128,bool,int168,uint256[3],bytes32))"
     human_encoded = abi.encode(human_t, human_tuple)
     assert c.abi_encode(*args, False, False).hex() == human_encoded.hex()
     assert c.abi_encode(*args, False, True).hex() == (method_id + human_encoded).hex()
 
     human_encoded = abi.encode(f"({human_t})", (human_tuple,))
     assert c.abi_encode(*args, True, False).hex() == human_encoded.hex()
     assert c.abi_encode(*args, True, True).hex() == (method_id + human_encoded).hex()
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_addmod.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_addmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_as_wei_value.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_as_wei_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from decimal import Decimal
-
 import pytest
 
+from tests.utils import decimal_to_int
+from vyper.semantics.types import DecimalT
+from vyper.utils import quantize, round_towards_zero
+
 wei_denoms = {
     "femtoether": 3,
     "kwei": 3,
     "babbage": 3,
     "picoether": 6,
     "mwei": 6,
     "lovelace": 6,
@@ -57,19 +59,22 @@
 @pytest.mark.parametrize("denom,multiplier", wei_denoms.items())
 def test_wei_decimal(get_contract, tx_failed, denom, multiplier):
     code = f"""
 @external
 def foo(a: decimal) -> uint256:
     return as_wei_value(a, "{denom}")
     """
-
     c = get_contract(code)
-    value = Decimal((2**127 - 1) / (10**multiplier))
 
-    assert c.foo(value) == value * (10**multiplier)
+    denom_int = 10**multiplier
+    # TODO: test with more values
+    _, hi = DecimalT().ast_bounds
+    value = quantize(hi / denom_int)
+
+    assert c.foo(decimal_to_int(value)) == round_towards_zero(value * denom_int)
 
 
 @pytest.mark.parametrize("value", (-1, -(2**127)))
 @pytest.mark.parametrize("data_type", ["decimal", "int128"])
 def test_negative_value_reverts(get_contract, tx_failed, value, data_type):
     code = f"""
 @external
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_bitwise.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_ceil.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ceil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import math
 from decimal import Decimal
 
+from tests.utils import decimal_to_int
+
 
 def test_ceil(get_contract_with_gas_estimation):
     code = """
 x: decimal
 
 @deploy
 def __init__():
@@ -98,16 +100,16 @@
     assert c.x_ceil() == -504
     assert c.foo() == -11
     assert c.fop() == -5
     assert c.foq() == 0
     assert c.fos() == -5472
     assert c.fot() == math.ceil(-(Decimal(2**167 - 1)) / 10**10)
     assert c.fou() == -3
-    assert c.ceil_param(Decimal("-0.5")) == 0
-    assert c.ceil_param(Decimal("-7777777.7777777")) == -7777777
+    assert c.ceil_param(decimal_to_int("-0.5")) == 0
+    assert c.ceil_param(decimal_to_int("-7777777.7777777")) == -7777777
 
 
 def test_ceil_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: decimal) -> decimal: payable
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_concat.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_convert.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import enum
 import itertools
-
-# import random
+import math
 from decimal import Decimal
 
 import eth.codecs.abi as abi
 import eth.codecs.abi.exceptions
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import InvalidLiteral, InvalidType, TypeMismatch
 from vyper.semantics.types import AddressT, BoolT, BytesM_T, BytesT, DecimalT, IntegerT, StringT
 from vyper.semantics.types.shortcuts import BYTES20_T, BYTES32_T, UINT, UINT160_T, UINT256_T
 from vyper.utils import (
     DECIMAL_DIVISOR,
     checksum_encode,
@@ -245,21 +245,28 @@
             head = padding_byte * len(head)
         return head + val_bits[:n]
 
 
 def _from_bits(val_bits, o_typ):
     # o_typ: the type to convert to
     try:
-        return abi.decode(o_typ.abi_type.selector_name(), val_bits)
+        ret = abi.decode(o_typ.abi_type.selector_name(), val_bits)
+        if isinstance(o_typ, DecimalT):
+            return Decimal(ret) / o_typ.divisor
+        return ret
     except eth.codecs.abi.exceptions.DecodeError:
         raise _OutOfBounds() from None
 
 
 def _to_bits(val, i_typ):
     # i_typ: the type to convert from
+    if isinstance(i_typ, DecimalT):
+        val = val * i_typ.divisor
+        assert math.ceil(val) == math.floor(val)
+        val = int(val)
     return abi.encode(i_typ.abi_type.selector_name(), val)
 
 
 def _signextend(val_bytes, bits):
     as_uint = int.from_bytes(val_bytes, byteorder="big")
 
     as_sint = unsigned_to_signed(as_uint, bits)
@@ -426,14 +433,21 @@
     get_contract_with_gas_estimation, assert_compile_failed, i_typ, o_typ, val
 ):
     expected_val = _py_convert(val, i_typ, o_typ)
     if isinstance(o_typ, AddressT) and expected_val == "0x" + "00" * 20:
         # web3 has special formatter for zero address
         expected_val = None
 
+    if isinstance(o_typ, DecimalT):
+        expected_val = decimal_to_int(expected_val)
+
+    input_val = val
+    if isinstance(i_typ, DecimalT):
+        input_val = decimal_to_int(val)
+
     contract_1 = f"""
 @external
 def test_convert() -> {o_typ}:
     return convert({_vyper_literal(val, i_typ)}, {o_typ})
     """
 
     c1_exception = None
@@ -457,15 +471,15 @@
     contract_2 = f"""
 @external
 def test_input_convert(x: {i_typ}) -> {o_typ}:
     return convert(x, {o_typ})
     """
 
     c2 = get_contract_with_gas_estimation(contract_2)
-    assert c2.test_input_convert(val) == expected_val
+    assert c2.test_input_convert(input_val) == expected_val
 
     contract_3 = f"""
 bar: {i_typ}
 
 @external
 def test_state_variable_convert() -> {o_typ}:
     self.bar = {_vyper_literal(val, i_typ)}
@@ -479,15 +493,15 @@
 @external
 def test_memory_variable_convert(x: {i_typ}) -> {o_typ}:
     y: {i_typ} = x
     return convert(y, {o_typ})
     """
 
     c4 = get_contract_with_gas_estimation(contract_4)
-    assert c4.test_memory_variable_convert(val) == expected_val
+    assert c4.test_memory_variable_convert(input_val) == expected_val
 
 
 @pytest.mark.parametrize("typ", ["uint8", "int128", "int256", "uint256"])
 @pytest.mark.parametrize("val", [1, 2, 2**128, 2**256 - 1, 2**256 - 2])
 def test_flag_conversion(get_contract_with_gas_estimation, assert_compile_failed, val, typ):
     roles = "\n    ".join([f"ROLE_{i}" for i in range(256)])
     contract = f"""
@@ -711,9 +725,12 @@
     contract_3 = f"""
 @external
 def foo(bar: {i_typ}) -> {o_typ}:
     return convert(bar, {o_typ})
     """
 
     c3 = get_contract_with_gas_estimation(contract_3)
+    input_val = val
+    if isinstance(i_typ, DecimalT):
+        input_val = decimal_to_int(input_val)
     with tx_failed():
-        c3.foo(val)
+        c3.foo(input_val)
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_create_functions.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_create_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,63 +106,81 @@
 
     receipt = w3.eth.get_transaction_receipt(tx_hash)
 
     assert receipt["status"] == 0
     assert receipt["gasUsed"] < GAS_SENT
 
 
-def test_create_minimal_proxy_to_create2(get_contract, create2_address_of, keccak, tx_failed):
-    code = """
+@pytest.mark.parametrize("revert_on_failure", [True, False, None])
+def test_create_minimal_proxy_to_create2(
+    get_contract, create2_address_of, keccak, tx_failed, revert_on_failure
+):
+    revert_arg = "" if revert_on_failure is None else f", revert_on_failure={revert_on_failure}"
+    code = f"""
 main: address
 
 @external
 def test(_salt: bytes32) -> address:
-    self.main = create_minimal_proxy_to(self, salt=_salt)
+    self.main = create_minimal_proxy_to(self, salt=_salt{revert_arg})
     return self.main
     """
 
     c = get_contract(code)
 
     salt = keccak(b"vyper")
     assert HexBytes(c.test(salt)) == create2_address_of(
         c.address, salt, eip1167_initcode(c.address)
     )
 
     c.test(salt, transact={})
     # revert on collision
-    with tx_failed():
-        c.test(salt, transact={})
+    if revert_on_failure is False:
+        assert not c.test(salt)
+    else:
+        with tx_failed():
+            c.test(salt, transact={})
 
 
 # test blueprints with various prefixes - 0xfe would block calls to the blueprint
 # contract, and 0xfe7100 is ERC5202 magic
 @pytest.mark.parametrize("blueprint_prefix", [b"", b"\xfe", ERC5202_PREFIX])
+@pytest.mark.parametrize("revert_on_failure", [True, False, None])
 def test_create_from_blueprint(
-    get_contract, deploy_blueprint_for, w3, keccak, create2_address_of, tx_failed, blueprint_prefix
+    get_contract,
+    deploy_blueprint_for,
+    w3,
+    keccak,
+    create2_address_of,
+    tx_failed,
+    blueprint_prefix,
+    revert_on_failure,
 ):
+    revert_arg = "" if revert_on_failure is None else f", revert_on_failure={revert_on_failure}"
     code = """
 @external
 def foo() -> uint256:
     return 123
     """
 
     prefix_len = len(blueprint_prefix)
     deployer_code = f"""
 created_address: public(address)
 
 @external
 def test(target: address):
-    self.created_address = create_from_blueprint(target, code_offset={prefix_len})
+    self.created_address = create_from_blueprint(target, code_offset={prefix_len}{revert_arg})
 
 @external
 def test2(target: address, salt: bytes32):
-    self.created_address = create_from_blueprint(target, code_offset={prefix_len}, salt=salt)
+    self.created_address = create_from_blueprint(
+        target, code_offset={prefix_len}, salt=salt{revert_arg}
+    )
     """
 
-    # deploy a foo so we can compare its bytecode with factory deployed version
+    # deploy a foo, so we can compare its bytecode with factory deployed version
     foo_contract = get_contract(code)
     expected_runtime_code = w3.eth.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code, initcode_prefix=blueprint_prefix)
 
     d = get_contract(deployer_code)
 
@@ -187,16 +205,19 @@
 
     # check if the create2 address matches our offchain calculation
     initcode = w3.eth.get_code(f.address)
     initcode = initcode[len(blueprint_prefix) :]  # strip the prefix
     assert HexBytes(test.address) == create2_address_of(d.address, salt, initcode)
 
     # can't collide addresses
-    with tx_failed():
-        d.test2(f.address, salt)
+    if revert_on_failure is False:
+        assert not d.test2(f.address, salt)
+    else:
+        with tx_failed():
+            d.test2(f.address, salt)
 
 
 # test blueprints with 0xfe7100 prefix, which is the EIP 5202 standard.
 # code offset by default should be 3 here.
 def test_create_from_blueprint_default_offset(
     get_contract, deploy_blueprint_for, w3, keccak, create2_address_of, tx_failed
 ):
@@ -421,24 +442,26 @@
     BAR = ("",)
     sig = keccak("should_fail(address,string,(string))".encode()).hex()[:10]
     encoded = abi.encode("(address,string,(string))", (f.address, FOO, BAR)).hex()
     with tx_failed():
         w3.eth.send_transaction({"to": d.address, "data": f"{sig}{encoded}"})
 
 
-def test_create_copy_of(get_contract, w3, keccak, create2_address_of, tx_failed):
-    code = """
+@pytest.mark.parametrize("revert_on_failure", [True, False, None])
+def test_create_copy_of(get_contract, w3, keccak, create2_address_of, tx_failed, revert_on_failure):
+    revert_arg = "" if revert_on_failure is None else f", revert_on_failure={revert_on_failure}"
+    code = f"""
 created_address: public(address)
 @internal
 def _create_copy_of(target: address):
-    self.created_address = create_copy_of(target)
+    self.created_address = create_copy_of(target{revert_arg})
 
 @internal
 def _create_copy_of2(target: address, salt: bytes32):
-    self.created_address = create_copy_of(target, salt=salt)
+    self.created_address = create_copy_of(target, salt=salt{revert_arg})
 
 @external
 def test(target: address) -> address:
     x: uint256 = 0
     self._create_copy_of(target)
     assert x == 0  # check memory not clobbered
     return self.created_address
@@ -469,22 +492,19 @@
     c.test2(c.address, salt, transact={})
     test2 = c.created_address()
     assert w3.eth.get_code(test2) == bytecode
 
     assert HexBytes(test2) == create2_address_of(c.address, salt, vyper_initcode(bytecode))
 
     # can't create2 where contract already exists
-    with tx_failed():
-        c.test2(c.address, salt, transact={})
-
-    # test single byte contract
-    # test2 = c.test2(b"\x01", salt)
-    # assert HexBytes(test2) == create2_address_of(c.address, salt, vyper_initcode(b"\x01"))
-    # with tx_failed():
-    #     c.test2(bytecode, salt)
+    if revert_on_failure is False:
+        assert not c.test2(c.address, salt)
+    else:
+        with tx_failed():
+            c.test2(c.address, salt)
 
 
 # XXX: these various tests to check the msize allocator for
 # create_copy_of and create_from_blueprint depend on calling convention
 # and variables writing to memory. think of ways to make more robust to
 # changes in calling convention and memory layout
 @pytest.mark.parametrize("blueprint_prefix", [b"", b"\xfe", b"\xfe\71\x00"])
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_ec.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_ecrecover.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ecrecover.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_empty.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_empty.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_extract32.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_floor.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_floor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import math
 from decimal import Decimal
 
+from tests.utils import decimal_to_int
+
 
 def test_floor(get_contract_with_gas_estimation):
     code = """
 x: decimal
 
 @deploy
 def __init__():
@@ -102,16 +104,16 @@
     assert c.x_floor() == -505
     assert c.foo() == -7
     assert c.fop() == -27
     assert c.foq() == -9001
     assert c.fos() == -1
     assert c.fot() == math.floor(-Decimal(2**167) / 10**10)
     assert c.fou() == -4
-    assert c.floor_param(Decimal("-5.6")) == -6
-    assert c.floor_param(Decimal("-0.0000000001")) == -1
+    assert c.floor_param(decimal_to_int("-5.6")) == -6
+    assert c.floor_param(decimal_to_int("-0.0000000001")) == -1
 
 
 def test_floor_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: decimal) -> decimal: nonpayable
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_is_contract.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_is_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_keccak256.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_length.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_length.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_method_id.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from decimal import Decimal
-
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.semantics.types import IntegerT
 
 
 def test_minmax(get_contract_with_gas_estimation):
     minmax_test = """
 @external
 def foo() -> decimal:
@@ -13,15 +12,15 @@
 
 @external
 def goo() -> uint256:
     return min(3, 5) + max(40, 80)
     """
 
     c = get_contract_with_gas_estimation(minmax_test)
-    assert c.foo() == Decimal("58223.123")
+    assert c.foo() == decimal_to_int("58223.123")
     assert c.goo() == 83
 
     print("Passed min/max test")
 
 
 @pytest.mark.parametrize("return_type", sorted(IntegerT.all()))
 def test_minmax_var_and_literal_and_bultin(get_contract_with_gas_estimation, return_type):
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax_value.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     code = f"""
 @external
 def foo() -> {typ}:
     return {op}({typ})
     """
     c = get_contract(code)
 
-    lo, hi = typ.ast_bounds
+    lo, hi = typ.int_bounds
     if op == "min_value":
         assert c.foo() == lo
     elif op == "max_value":
         assert c.foo() == hi
 
 
 @pytest.mark.parametrize("typ", sorted(IntegerT.all()))
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_mulmod.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_raw_call.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_send.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_sha256.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_sha256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_slice.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_uint2str.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_uint2str.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_unary.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from decimal import Decimal
-
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import InvalidOperation
 
 
 def test_unary_sub_uint256_fail(assert_compile_failed, get_contract):
     code = """@external
 def negate(a: uint256) -> uint256:
     return -(a)
@@ -59,16 +58,16 @@
 
 @external
 def bar() -> decimal:
     return -b
     """
 
     c = get_contract(code)
-    assert c.foo() == Decimal("-18707220957835557353007165858768422651595.9365500927")
-    assert c.bar() == Decimal("18707220957835557353007165858768422651595.9365500927")
+    assert c.foo() == decimal_to_int("-18707220957835557353007165858768422651595.9365500927")
+    assert c.bar() == decimal_to_int("18707220957835557353007165858768422651595.9365500927")
 
 
 def test_negation_int128(get_contract):
     code = """
 a: constant(int128) = min_value(int128)
 
 @external
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/codegen/test_unsafe_math.py` & `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_abs.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_addmod_mulmod.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_bitwise.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_floor_ceil.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_floor_ceil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from decimal import Decimal
 
 import pytest
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
-from tests.utils import parse_and_fold
+from tests.utils import decimal_to_int, parse_and_fold
 
 st_decimals = st.decimals(
     min_value=-(2**32), max_value=2**32, allow_nan=False, allow_infinity=False, places=10
 )
 
 
 @pytest.mark.fuzzing
@@ -27,8 +27,9 @@
     """
     contract = get_contract(source)
 
     vyper_ast = parse_and_fold(f"{fn_name}({value})")
     old_node = vyper_ast.body[0].value
     new_node = old_node.get_folded_value()
 
-    assert contract.foo(value) == new_node.value
+    assert isinstance(new_node.value, int)
+    assert contract.foo(decimal_to_int(value)) == new_node.value
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_fold_as_wei_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
-from tests.utils import parse_and_fold
+from tests.utils import decimal_to_int, parse_and_fold
 from vyper.builtins import functions as vy_fn
 from vyper.utils import SizeLimits
 
 denoms = [x for k in vy_fn.AsWeiValue.wei_denoms.keys() for x in k]
 
 
 st_decimals = st.decimals(
@@ -30,15 +30,16 @@
     """
     contract = get_contract(source)
 
     vyper_ast = parse_and_fold(f"as_wei_value({value:.10f}, '{denom}')")
     old_node = vyper_ast.body[0].value
     new_node = old_node.get_folded_value()
 
-    assert contract.foo(value) == new_node.value
+    assert isinstance(new_node.value, int)
+    assert contract.foo(decimal_to_int(value)) == new_node.value
 
 
 @pytest.mark.fuzzing
 @settings(max_examples=10)
 @given(value=st.integers(min_value=0, max_value=2**128))
 @pytest.mark.parametrize("denom", denoms)
 def test_integer(get_contract, value, denom):
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_keccak_sha.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_keccak_sha.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_len.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_min_max.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_min_max.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
-from tests.utils import parse_and_fold
+from tests.utils import decimal_to_int, parse_and_fold
 from vyper.utils import SizeLimits
 
 st_decimals = st.decimals(
     min_value=SizeLimits.MIN_AST_DECIMAL,
     max_value=SizeLimits.MAX_AST_DECIMAL,
     allow_nan=False,
     allow_infinity=False,
@@ -28,15 +28,16 @@
     """
     contract = get_contract(source)
 
     vyper_ast = parse_and_fold(f"{fn_name}({left}, {right})")
     old_node = vyper_ast.body[0].value
     new_node = old_node.get_folded_value()
 
-    assert contract.foo(left, right) == new_node.value
+    l, r = [decimal_to_int(t) for t in (left, right)]
+    assert contract.foo(l, r) == decimal_to_int(new_node.value)
 
 
 @pytest.mark.fuzzing
 @settings(max_examples=50)
 @given(left=st_int128, right=st_int128)
 @pytest.mark.parametrize("fn_name", ["min", "max"])
 def test_int128(get_contract, left, right, fn_name):
```

### Comparing `vyper-0.4.0b6/tests/functional/builtins/folding/test_powmod.py` & `vyper-0.4.0rc1/tests/functional/builtins/folding/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_function.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_parameters.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_parameters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_erc20_abi.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_erc20_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_external_contract_calls.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_external_contract_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from decimal import Decimal
-
 import pytest
 from eth.codecs import abi
 
+from tests.utils import decimal_to_int
 from vyper import compile_code
 from vyper.exceptions import (
     ArgumentException,
     InvalidType,
     StateAccessViolation,
     StructureException,
     UndeclaredDefinition,
@@ -513,15 +512,15 @@
 
 @external
 def bar(arg1: address) -> decimal:
     return staticcall Foo(arg1).foo()
 """
 
     c2 = get_contract(contract_2)
-    assert c2.bar(c.address) == Decimal("1e-10")
+    assert c2.bar(c.address) == decimal_to_int("1e-10")
 
 
 def test_decimal_too_long(get_contract, tx_failed):
     contract_1 = """
 @external
 def foo() -> uint256:
     return 2**255
@@ -566,15 +565,15 @@
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
     """
 
     c2 = get_contract(contract_2)
     assert c.foo() == [0, b"dog", 1]
     result = c2.bar(c.address)
-    assert result == [Decimal("0.0"), b"dog", Decimal("1e-10")]
+    assert result == [decimal_to_int("0.0"), b"dog", decimal_to_int("1e-10")]
 
 
 @pytest.mark.parametrize("a,b", [(8, 256), (256, 8), (256, 256)])
 def test_tuple_with_decimal_too_long(get_contract, tx_failed, a, b):
     contract_1 = f"""
 @external
 def foo() -> (uint{a}, Bytes[3], uint{b}):
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_return.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_self_call_struct.py` & `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_self_call_struct.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from decimal import Decimal
+from tests.utils import decimal_to_int
 
 
 def test_call_to_self_struct(w3, get_contract):
     code = """
 struct MyStruct:
     e1: decimal
     e2: uint256
@@ -20,20 +20,20 @@
 
 @external
 @view
 def wrap_get_my_struct_BROKEN(_e1: decimal) -> MyStruct:
     return self.get_my_struct(_e1, block.timestamp)
     """
     c = get_contract(code)
-    assert c.wrap_get_my_struct_WORKING(Decimal("0.1")) == (
-        Decimal("0.1"),
+    assert c.wrap_get_my_struct_WORKING(decimal_to_int("0.1")) == (
+        decimal_to_int("0.1"),
         w3.eth.get_block(w3.eth.block_number)["timestamp"],
     )
-    assert c.wrap_get_my_struct_BROKEN(Decimal("0.1")) == (
-        Decimal("0.1"),
+    assert c.wrap_get_my_struct_BROKEN(decimal_to_int("0.1")) == (
+        decimal_to_int("0.1"),
         w3.eth.get_block(w3.eth.block_number)["timestamp"],
     )
 
 
 def test_call_to_self_struct_2(get_contract):
     code = """
 struct MyStruct:
@@ -52,9 +52,9 @@
 
 @external
 @view
 def wrap_get_my_struct_BROKEN(_e1: decimal) -> MyStruct:
     return self.get_my_struct(_e1)
     """
     c = get_contract(code)
-    assert c.wrap_get_my_struct_WORKING(Decimal("0.1")) == (Decimal("0.1"),)
-    assert c.wrap_get_my_struct_BROKEN(Decimal("0.1")) == (Decimal("0.1"),)
+    assert c.wrap_get_my_struct_WORKING(decimal_to_int("0.1")) == (decimal_to_int("0.1"),)
+    assert c.wrap_get_my_struct_BROKEN(decimal_to_int("0.1")) == (decimal_to_int("0.1"),)
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_blockhash.py` & `vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_blockhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_nonreentrant.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_payable.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_private.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_private.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_public.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_pure.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_pure.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_view.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_view.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_break.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_break.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from decimal import Decimal
-
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import StructureException
 
 
 def test_break_test(get_contract_with_gas_estimation):
     break_test = """
 @external
 def foo(n: decimal) -> int128:
@@ -17,18 +16,18 @@
             output = i
             break
     return output
     """
 
     c = get_contract_with_gas_estimation(break_test)
 
-    assert c.foo(Decimal("1")) == 0
-    assert c.foo(Decimal("2")) == 3
-    assert c.foo(Decimal("10")) == 10
-    assert c.foo(Decimal("200")) == 23
+    assert c.foo(decimal_to_int("1")) == 0
+    assert c.foo(decimal_to_int("2")) == 3
+    assert c.foo(decimal_to_int("10")) == 10
+    assert c.foo(decimal_to_int("200")) == 23
 
     print("Passed for-loop break test")
 
 
 def test_break_test_2(get_contract_with_gas_estimation):
     break_test_2 = """
 @external
@@ -45,19 +44,19 @@
         if c < 1.0:
             output = output + i
             break
     return output
     """
 
     c = get_contract_with_gas_estimation(break_test_2)
-    assert c.foo(Decimal("1")) == 0
-    assert c.foo(Decimal("2")) == 3
-    assert c.foo(Decimal("10")) == 10
-    assert c.foo(Decimal("200")) == 23
-    assert c.foo(Decimal("4000000")) == 66
+    assert c.foo(decimal_to_int("1")) == 0
+    assert c.foo(decimal_to_int("2")) == 3
+    assert c.foo(decimal_to_int("10")) == 10
+    assert c.foo(decimal_to_int("200")) == 23
+    assert c.foo(decimal_to_int("4000000")) == 66
     print("Passed for-loop break test 2")
 
 
 def test_break_test_3(get_contract_with_gas_estimation):
     break_test_3 = """
 @external
 def foo(n: int128) -> int128:
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_continue.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_continue.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_in_list.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_in_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
-from decimal import Decimal
 
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     ArgumentException,
     ImmutableViolation,
     InvalidType,
     IteratorException,
     NamespaceCollision,
@@ -265,21 +265,21 @@
             return i
         count += 1
     return -1.111
     """
 
     c = get_contract_with_gas_estimation(code)
 
-    c.set(0, Decimal("0.0001"), transact={})
-    c.set(1, Decimal("1.1"), transact={})
-    c.set(2, Decimal("2.2"), transact={})
-
-    assert c.ret(2) == c.i_return(2) == Decimal("2.2")
-    assert c.ret(1) == c.i_return(1) == Decimal("1.1")
-    assert c.ret(0) == c.i_return(0) == Decimal("0.0001")
+    c.set(0, decimal_to_int("0.0001"), transact={})
+    c.set(1, decimal_to_int("1.1"), transact={})
+    c.set(2, decimal_to_int("2.2"), transact={})
+
+    assert c.ret(2) == c.i_return(2) == decimal_to_int("2.2")
+    assert c.ret(1) == c.i_return(1) == decimal_to_int("1.1")
+    assert c.ret(0) == c.i_return(0) == decimal_to_int("0.0001")
 
 
 def test_for_in_list_iter_type(get_contract_with_gas_estimation):
     code = """
 @external
 @view
 def func(amounts: uint256[3]) -> uint256:
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_range.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_range_in.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_range_in.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_assert.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_assert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_assert_unreachable.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_assert_unreachable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_assignment.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_assignment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_bytes_map_keys.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_bytes_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_clampers.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_clampers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from decimal import Decimal
 
 import pytest
 from eth.codecs import abi
 from eth_utils import keccak
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import StackTooDeep
 from vyper.utils import int_bounds
 
 
 def _make_tx(w3, address, signature, values):
     # helper function to broadcast transactions that fail clamping check
     sig = keccak(signature.encode()).hex()[:8]
@@ -313,15 +314,15 @@
 @external
 def foo(s: decimal) -> decimal:
     return s
     """
 
     c = get_contract(code)
 
-    assert c.foo(Decimal(value)) == Decimal(value)
+    assert c.foo(decimal_to_int(value)) == decimal_to_int(value)
 
 
 @pytest.mark.parametrize(
     "value",
     [
         2**167,
         -(2**167 + 1),
@@ -335,15 +336,15 @@
 def foo(s: decimal) -> decimal:
     return s
     """
 
     c = get_contract(code)
 
     with tx_failed():
-        _make_tx(w3, c.address, "foo(fixed168x10)", [value])
+        _make_tx(w3, c.address, "foo(int168)", [value])
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
 def test_int128_array_clamper_passing(w3, get_contract, value):
     code = """
 @external
 def foo(a: uint256, b: int128[5], c: uint256) -> int128[5]:
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_comparison.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_conditionals.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_constructor.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_constructor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_immutable.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_immutable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_init.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_internal_call.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_internal_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import string
-from decimal import Decimal
 
 import hypothesis.strategies as st
 import pytest
 from hypothesis import given, settings
 
+from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import ArgumentException, CallViolation
 
 pytestmark = pytest.mark.usefixtures("memory_mocker")
 
 
 def test_selfcall_code(get_contract_with_gas_estimation):
@@ -320,17 +320,17 @@
     y: int128[2] = [99, 66]
     return self._foo4(x, y)
 
     """
 
     c = get_contract_with_gas_estimation(code)
     assert c.bar() == 0
-    assert c.foo1([0, 0], Decimal("0")) == 0
+    assert c.foo1([0, 0], decimal_to_int("0")) == 0
     assert c.bar2() == 55
-    assert c.bar3() == Decimal("1.33")
+    assert c.bar3() == decimal_to_int("1.33")
     assert c.bar4() == 77
     assert c.bar5() == 88
 
 
 def test_multi_mixed_arg_list_call(get_contract_with_gas_estimation):
     code = """
 @internal
@@ -347,15 +347,15 @@
     y: decimal = 55.44
     z: int128[2] = [55, 66]
     a: decimal = 66.77
 
     return self._fooz(x, y, z, a), self._fooa(x, y, z, a)
     """
     c = get_contract_with_gas_estimation(code)
-    assert c.bar() == [66, Decimal("66.77")]
+    assert c.bar() == [66, decimal_to_int("66.77")]
 
 
 def test_internal_function_multiple_lists_as_args(get_contract_with_gas_estimation):
     code = """
 @internal
 def _foo(y: int128[2], x: Bytes[5]) -> int128:
     return y[0]
@@ -399,15 +399,15 @@
     y: decimal = 55.44
     z: Bytes[11] = b"hello world"
     a: decimal = 66.77
 
     return self._fooz(x, y, z, a), self._fooa(x, y, z, a), self._foox(x, y, z, a)
     """
     c = get_contract_with_gas_estimation(code)
-    assert c.bar() == [b"hello world", Decimal("66.77"), 44]
+    assert c.bar() == [b"hello world", decimal_to_int("66.77"), 44]
 
 
 FAILING_CONTRACTS_CALL_VIOLATION = [
     """
 # should not compile - public to public
 @external
 def bar() -> int128:
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_logging.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from decimal import Decimal
-
 import pytest
 from eth.codecs import abi
 
+from tests.utils import decimal_to_int
 from vyper import compile_code
 from vyper.exceptions import (
     ArgumentException,
     EventDeclarationException,
     InvalidType,
     NamespaceCollision,
     StructureException,
@@ -499,15 +498,15 @@
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     logs1 = receipt["logs"][0]
     logs2 = receipt["logs"][1]
     event_id1 = keccak(bytes("MyLog(int128,bytes)", "utf-8"))
-    event_id2 = keccak(bytes("YourLog(address,(uint256,bytes,(string,fixed168x10)))", "utf-8"))
+    event_id2 = keccak(bytes("YourLog(address,(uint256,bytes,(string,int168)))", "utf-8"))
 
     # Event id is always the first topic
     assert logs1["topics"][0] == "0x" + event_id1.hex()
     assert logs2["topics"][0] == "0x" + event_id2.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
@@ -529,15 +528,15 @@
                     {"name": "x", "type": "uint256"},
                     {"name": "y", "type": "bytes"},
                     {
                         "name": "z",
                         "type": "tuple",
                         "components": [
                             {"name": "t", "type": "string"},
-                            {"name": "w", "type": "fixed168x10"},
+                            {"name": "w", "type": "int168", "internalType": "decimal"},
                         ],
                     },
                 ],
                 "indexed": False,
             },
         ],
         "anonymous": False,
@@ -548,15 +547,15 @@
     logs = get_logs(tx_hash, c, "MyLog")
     args = logs[0].args
     assert args.arg1 == 1
     assert args.arg2 == b"bar"
     logs = get_logs(tx_hash, c, "YourLog")
     args = logs[0].args
     assert args.arg1 == c.address
-    assert args.arg2 == {"x": 1, "y": b"abc", "z": {"t": "house", "w": Decimal("13.5")}}
+    assert args.arg2 == {"x": 1, "y": b"abc", "z": {"t": "house", "w": decimal_to_int("13.5")}}
 
 
 def test_fails_when_input_is_the_wrong_type(tx_failed, get_contract_with_gas_estimation):
     loggy_code = """
 event MyLog:
     arg1: indexed(int128)
 
@@ -898,18 +897,18 @@
     log Bar([1.11, 2.22, 3.33, 4.44])
     """
     c = get_contract_with_gas_estimation(code)
 
     tx_hash = c.foo(transact={})
     logs = get_logs(tx_hash, c, "Bar")
     assert logs[0].args._value == [
-        Decimal("1.11"),
-        Decimal("2.22"),
-        Decimal("3.33"),
-        Decimal("4.44"),
+        decimal_to_int("1.11"),
+        decimal_to_int("2.22"),
+        decimal_to_int("3.33"),
+        decimal_to_int("4.44"),
     ]
 
 
 def test_storage_byte_packing(get_logs, bytes_helper, get_contract_with_gas_estimation):
     code = """
 event MyLog:
     arg1: Bytes[29]
@@ -950,23 +949,23 @@
 def set_list():
     self.x = [1.33, 2.33, 3.33, 4.33]
     """
     c = get_contract_with_gas_estimation(code)
 
     tx_hash = c.foo(transact={})
     logs = get_logs(tx_hash, c, "Bar")
-    assert logs[0].args._value == [Decimal("0"), Decimal("0"), Decimal("0"), Decimal("0")]
+    assert logs[0].args._value == [decimal_to_int("0")] * 4
     c.set_list(transact={})
     tx_hash = c.foo(transact={})
     logs = get_logs(tx_hash, c, "Bar")
     assert logs[0].args._value == [
-        Decimal("1.33"),
-        Decimal("2.33"),
-        Decimal("3.33"),
-        Decimal("4.33"),
+        decimal_to_int("1.33"),
+        decimal_to_int("2.33"),
+        decimal_to_int("3.33"),
+        decimal_to_int("4.33"),
     ]
 
 
 def test_logging_fails_when_input_is_too_big(tx_failed, get_contract_with_gas_estimation):
     code = """
 event Bar:
     _value: indexed(Bytes[32])
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_logging_bytes_extended.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_bytes_extended.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_logging_from_call.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_from_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_memory_dealloc.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_packing.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_packing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_reverting.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_reverting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_short_circuiting.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_short_circuiting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_string_map_keys.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_ternary.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/features/test_transient.py` & `vyper-0.4.0rc1/tests/functional/codegen/features/test_transient.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/integration/test_crowdfund.py` & `vyper-0.4.0rc1/tests/functional/codegen/integration/test_crowdfund.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/integration/test_escrow.py` & `vyper-0.4.0rc1/tests/functional/codegen/integration/test_escrow.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_events.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_exports.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_flag_imports.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_flag_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_interface_imports.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_interface_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_module_constants.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_module_variables.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_variables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/modules/test_stateless_functions.py` & `vyper-0.4.0rc1/tests/functional/codegen/modules/test_stateless_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_getters.py` & `vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_setters.py` & `vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_setters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_storage_variable.py` & `vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_storage_variable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/test_call_graph_stability.py` & `vyper-0.4.0rc1/tests/functional/codegen/test_call_graph_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/test_interfaces.py` & `vyper-0.4.0rc1/tests/functional/codegen/test_interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
-from decimal import Decimal
 
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     ArgumentException,
     DuplicateImport,
     InterfaceViolation,
     NamespaceCollision,
 )
@@ -242,15 +242,15 @@
 @pytest.mark.parametrize(
     "kwarg,typ,expected",
     [
         ("max_value(uint256)", "uint256", 2**256 - 1),
         ("min_value(int128)", "int128", -(2**127)),
         ("empty(uint8[2])", "uint8[2]", [0, 0]),
         ('method_id("vyper()", output_type=bytes4)', "bytes4", b"\x82\xcbE\xfb"),
-        ("epsilon(decimal)", "decimal", Decimal("1E-10")),
+        ("epsilon(decimal)", "decimal", decimal_to_int("1E-10")),
     ],
 )
 def test_external_call_to_interface_kwarg(get_contract, kwarg, typ, expected, make_input_bundle):
     interface_code = f"""
 @external
 @view
 def foo(_max: {typ} = {kwarg}) -> {typ}:
@@ -610,15 +610,15 @@
 
 type_str_params = [
     ("int128", -33),
     ("uint256", 42),
     ("bool", True),
     ("address", "0x1234567890123456789012345678901234567890"),
     ("bytes32", b"bytes32bytes32bytes32bytes32poop"),
-    ("decimal", Decimal("3.1337")),
+    ("decimal", decimal_to_int("3.1337")),
     ("Bytes[4]", b"newp"),
     ("String[6]", "potato"),
 ]
 
 interface_test_code = """
 @external
 @view
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/test_selector_table.py` & `vyper-0.4.0rc1/tests/functional/codegen/test_selector_table.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/test_selector_table_stability.py` & `vyper-0.4.0rc1/tests/functional/codegen/test_selector_table_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_constants.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
-from decimal import Decimal
 
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import TypeMismatch
 from vyper.utils import MemoryPositions
 
 
 def search_for_sublist(ir, sublist):
     _list = ir.to_list() if hasattr(ir, "to_list") else ir
@@ -55,23 +55,21 @@
     assert c.test_zaddress("0x0000000000000000000000000000000000000000") is True
     assert c.test_zaddress("0x0000000000000000000000000000000000000012") is False
 
     assert c.test_int128(2**127 - 1) == [True, False]
     assert c.test_int128(-(2**127)) == [False, True]
     assert c.test_int128(0) == [False, False]
 
-    assert c.test_decimal(Decimal("18707220957835557353007165858768422651595.9365500927")) == [
-        True,
-        False,
-    ]
-    assert c.test_decimal(Decimal("-18707220957835557353007165858768422651595.9365500928")) == [
-        False,
-        True,
-    ]
-    assert c.test_decimal(Decimal("0.1")) == [False, False]
+    assert c.test_decimal(
+        decimal_to_int("18707220957835557353007165858768422651595.9365500927")
+    ) == [True, False]
+    assert c.test_decimal(
+        decimal_to_int("-18707220957835557353007165858768422651595.9365500928")
+    ) == [False, True]
+    assert c.test_decimal(decimal_to_int("0.1")) == [False, False]
 
     assert c.test_uint256(2**256 - 1) is True
 
     assert c.test_arithmetic(5000) == 2**127 - 1 - 5000
 
 
 def test_builtin_constants_assignment(get_contract_with_gas_estimation):
@@ -117,16 +115,16 @@
     assert c.foo() == 2**127 - 1
     assert c.goo() == -(2**127)
 
     assert c.hoo() == b"\x00" * 32
 
     assert c.joo() is None
 
-    assert c.koo() == Decimal(2**167 - 1) / 10**10
-    assert c.loo() == Decimal(-(2**167)) / 10**10
+    assert c.koo() == (2**167 - 1)
+    assert c.loo() == -(2**167)
 
     assert c.zoo() == 2**256 - 1
 
 
 def test_custom_constants(get_contract):
     code = """
 X_VALUE: constant(uint256) = 33
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_decimals.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_decimals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,439 +1,529 @@
 00000000: 696d 706f 7274 2077 6172 6e69 6e67 730a  import warnings.
 00000010: 6672 6f6d 2064 6563 696d 616c 2069 6d70  from decimal imp
-00000020: 6f72 7420 4465 6369 6d61 6c2c 2067 6574  ort Decimal, get
-00000030: 636f 6e74 6578 740a 0a69 6d70 6f72 7420  context..import 
-00000040: 7079 7465 7374 0a0a 6672 6f6d 2076 7970  pytest..from vyp
-00000050: 6572 2069 6d70 6f72 7420 636f 6d70 696c  er import compil
-00000060: 655f 636f 6465 0a66 726f 6d20 7679 7065  e_code.from vype
-00000070: 722e 6578 6365 7074 696f 6e73 2069 6d70  r.exceptions imp
-00000080: 6f72 7420 280a 2020 2020 4465 6369 6d61  ort (.    Decima
-00000090: 6c4f 7665 7272 6964 6545 7863 6570 7469  lOverrideExcepti
-000000a0: 6f6e 2c0a 2020 2020 496e 7661 6c69 644f  on,.    InvalidO
-000000b0: 7065 7261 7469 6f6e 2c0a 2020 2020 4f76  peration,.    Ov
-000000c0: 6572 666c 6f77 4578 6365 7074 696f 6e2c  erflowException,
-000000d0: 0a20 2020 2054 7970 654d 6973 6d61 7463  .    TypeMismatc
-000000e0: 682c 0a29 0a66 726f 6d20 7679 7065 722e  h,.).from vyper.
-000000f0: 7574 696c 7320 696d 706f 7274 2044 4543  utils import DEC
-00000100: 494d 414c 5f45 5053 494c 4f4e 2c20 5369  IMAL_EPSILON, Si
-00000110: 7a65 4c69 6d69 7473 2c20 7175 616e 7469  zeLimits, quanti
-00000120: 7a65 0a0a 0a64 6566 2074 6573 745f 6465  ze...def test_de
-00000130: 6369 6d61 6c5f 6f76 6572 7269 6465 2829  cimal_override()
-00000140: 3a0a 2020 2020 6765 7463 6f6e 7465 7874  :.    getcontext
-00000150: 2829 2e70 7265 6320 3d20 3738 2020 2320  ().prec = 78  # 
-00000160: 7365 7474 696e 6720 7072 6563 2074 6f20  setting prec to 
-00000170: 3738 2069 7320 6f6b 0a0a 2020 2020 2320  78 is ok..    # 
-00000180: 636f 6e73 756d 6572 7320 6f66 2076 7970  consumers of vyp
-00000190: 6572 2c20 6576 656e 2061 7320 6120 6c69  er, even as a li
-000001a0: 6272 6172 792c 2061 7265 206e 6f74 2061  brary, are not a
-000001b0: 6c6c 6f77 6564 2074 6f20 7265 6475 6365  llowed to reduce
-000001c0: 2044 6563 696d 616c 2070 7265 6369 7369   Decimal precisi
-000001d0: 6f6e 0a20 2020 2077 6974 6820 7079 7465  on.    with pyte
-000001e0: 7374 2e72 6169 7365 7328 4465 6369 6d61  st.raises(Decima
-000001f0: 6c4f 7665 7272 6964 6545 7863 6570 7469  lOverrideExcepti
-00000200: 6f6e 293a 0a20 2020 2020 2020 2067 6574  on):.        get
-00000210: 636f 6e74 6578 7428 292e 7072 6563 203d  context().prec =
-00000220: 2037 370a 0a20 2020 2077 6974 6820 7761   77..    with wa
-00000230: 726e 696e 6773 2e63 6174 6368 5f77 6172  rnings.catch_war
-00000240: 6e69 6e67 7328 7265 636f 7264 3d54 7275  nings(record=Tru
-00000250: 6529 2061 7320 773a 0a20 2020 2020 2020  e) as w:.       
-00000260: 2067 6574 636f 6e74 6578 7428 292e 7072   getcontext().pr
-00000270: 6563 203d 2037 390a 2020 2020 2020 2020  ec = 79.        
-00000280: 2320 6368 6563 6b20 7761 726e 696e 6773  # check warnings
-00000290: 2077 6572 6520 6973 7375 6564 0a20 2020   were issued.   
-000002a0: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
-000002b0: 7729 203d 3d20 310a 2020 2020 2020 2020  w) == 1.        
-000002c0: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
-000002d0: 2020 2020 2073 7472 2877 5b2d 315d 2e6d       str(w[-1].m
-000002e0: 6573 7361 6765 2920 3d3d 2022 4368 616e  essage) == "Chan
-000002f0: 6769 6e67 2064 6563 696d 616c 7320 7072  ging decimals pr
-00000300: 6563 6973 696f 6e20 636f 756c 6420 6861  ecision could ha
-00000310: 7665 2075 6e69 6e74 656e 6465 6420 7369  ve unintended si
-00000320: 6465 2065 6666 6563 7473 2122 0a20 2020  de effects!".   
-00000330: 2020 2020 2029 0a0a 0a40 7079 7465 7374       )...@pytest
-00000340: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-00000350: 6528 226f 7022 2c20 5b22 2f2f 222c 2022  e("op", ["//", "
-00000360: 2a2a 222c 2022 2622 2c20 227c 222c 2022  **", "&", "|", "
-00000370: 5e22 5d29 0a64 6566 2074 6573 745f 696e  ^"]).def test_in
-00000380: 7661 6c69 645f 6f70 7328 6f70 293a 0a20  valid_ops(op):. 
-00000390: 2020 2063 6f64 6520 3d20 6622 2222 0a40     code = f""".@
-000003a0: 6578 7465 726e 616c 0a64 6566 2066 6f6f  external.def foo
-000003b0: 2878 3a20 6465 6369 6d61 6c2c 2079 3a20  (x: decimal, y: 
-000003c0: 6465 6369 6d61 6c29 202d 3e20 6465 6369  decimal) -> deci
-000003d0: 6d61 6c3a 0a20 2020 2072 6574 7572 6e20  mal:.    return 
-000003e0: 7820 7b6f 707d 2079 0a20 2020 2022 2222  x {op} y.    """
-000003f0: 0a20 2020 2077 6974 6820 7079 7465 7374  .    with pytest
-00000400: 2e72 6169 7365 7328 496e 7661 6c69 644f  .raises(InvalidO
-00000410: 7065 7261 7469 6f6e 293a 0a20 2020 2020  peration):.     
-00000420: 2020 2063 6f6d 7069 6c65 5f63 6f64 6528     compile_code(
-00000430: 636f 6465 290a 0a0a 4070 7974 6573 742e  code)...@pytest.
-00000440: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00000450: 2822 6f70 222c 205b 226e 6f74 225d 290a  ("op", ["not"]).
-00000460: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
-00000470: 5f75 6e61 7279 5f6f 7073 286f 7029 3a0a  _unary_ops(op):.
-00000480: 2020 2020 636f 6465 203d 2066 2222 220a      code = f""".
-00000490: 4065 7874 6572 6e61 6c0a 6465 6620 666f  @external.def fo
-000004a0: 6f28 783a 2064 6563 696d 616c 2920 2d3e  o(x: decimal) ->
-000004b0: 2064 6563 696d 616c 3a0a 2020 2020 7265   decimal:.    re
-000004c0: 7475 726e 207b 6f70 7d20 780a 2020 2020  turn {op} x.    
-000004d0: 2222 220a 2020 2020 7769 7468 2070 7974  """.    with pyt
-000004e0: 6573 742e 7261 6973 6573 2849 6e76 616c  est.raises(Inval
-000004f0: 6964 4f70 6572 6174 696f 6e29 3a0a 2020  idOperation):.  
-00000500: 2020 2020 2020 636f 6d70 696c 655f 636f        compile_co
-00000510: 6465 2863 6f64 6529 0a0a 0a64 6566 2074  de(code)...def t
-00000520: 6573 745f 6465 6369 6d61 6c5f 7465 7374  est_decimal_test
-00000530: 2867 6574 5f63 6f6e 7472 6163 745f 7769  (get_contract_wi
-00000540: 7468 5f67 6173 5f65 7374 696d 6174 696f  th_gas_estimatio
-00000550: 6e29 3a0a 2020 2020 6465 6369 6d61 6c5f  n):.    decimal_
-00000560: 7465 7374 203d 2022 2222 0a40 6578 7465  test = """.@exte
-00000570: 726e 616c 0a64 6566 2066 6f6f 2829 202d  rnal.def foo() -
-00000580: 3e20 696e 7432 3536 3a0a 2020 2020 7265  > int256:.    re
-00000590: 7475 726e 2866 6c6f 6f72 2839 3939 2e30  turn(floor(999.0
-000005a0: 2929 0a0a 4065 7874 6572 6e61 6c0a 6465  ))..@external.de
-000005b0: 6620 666f 7028 2920 2d3e 2069 6e74 3235  f fop() -> int25
-000005c0: 363a 0a20 2020 2072 6574 7572 6e28 666c  6:.    return(fl
-000005d0: 6f6f 7228 3333 332e 3020 2b20 3636 362e  oor(333.0 + 666.
-000005e0: 3029 290a 0a40 6578 7465 726e 616c 0a64  0))..@external.d
-000005f0: 6566 2066 6f71 2829 202d 3e20 696e 7432  ef foq() -> int2
-00000600: 3536 3a0a 2020 2020 7265 7475 726e 2866  56:.    return(f
-00000610: 6c6f 6f72 2831 3333 322e 3120 2d20 3333  loor(1332.1 - 33
-00000620: 332e 3129 290a 0a40 6578 7465 726e 616c  3.1))..@external
-00000630: 0a64 6566 2062 6172 2829 202d 3e20 696e  .def bar() -> in
-00000640: 7432 3536 3a0a 2020 2020 7265 7475 726e  t256:.    return
-00000650: 2866 6c6f 6f72 2832 372e 3020 2a20 3337  (floor(27.0 * 37
-00000660: 2e30 2929 0a0a 4065 7874 6572 6e61 6c0a  .0))..@external.
-00000670: 6465 6620 6261 7a28 2920 2d3e 2069 6e74  def baz() -> int
-00000680: 3235 363a 0a20 2020 2078 3a20 6465 6369  256:.    x: deci
-00000690: 6d61 6c20 3d20 3237 2e30 0a20 2020 2072  mal = 27.0.    r
-000006a0: 6574 7572 6e28 666c 6f6f 7228 7820 2a20  eturn(floor(x * 
-000006b0: 3337 2e30 2929 0a0a 4065 7874 6572 6e61  37.0))..@externa
-000006c0: 6c0a 6465 6620 6d6f 6b28 2920 2d3e 2069  l.def mok() -> i
-000006d0: 6e74 3235 363a 0a20 2020 2072 6574 7572  nt256:.    retur
-000006e0: 6e28 666c 6f6f 7228 3939 3939 3939 2e30  n(floor(999999.0
-000006f0: 202f 2037 2e30 202f 2031 312e 3020 2f20   / 7.0 / 11.0 / 
-00000700: 3133 2e30 2929 0a0a 4065 7874 6572 6e61  13.0))..@externa
-00000710: 6c0a 6465 6620 6d6f 6c28 2920 2d3e 2069  l.def mol() -> i
-00000720: 6e74 3235 363a 0a20 2020 2072 6574 7572  nt256:.    retur
-00000730: 6e28 666c 6f6f 7228 3439 392e 3520 2f20  n(floor(499.5 / 
-00000740: 302e 3529 290a 0a40 6578 7465 726e 616c  0.5))..@external
-00000750: 0a64 6566 206d 6f6d 2829 202d 3e20 696e  .def mom() -> in
-00000760: 7432 3536 3a0a 2020 2020 7265 7475 726e  t256:.    return
-00000770: 2866 6c6f 6f72 2831 3439 382e 3520 2f20  (floor(1498.5 / 
-00000780: 312e 3529 290a 0a40 6578 7465 726e 616c  1.5))..@external
-00000790: 0a64 6566 206d 6f6f 2829 202d 3e20 696e  .def moo() -> in
-000007a0: 7432 3536 3a0a 2020 2020 7265 7475 726e  t256:.    return
-000007b0: 2866 6c6f 6f72 2832 3939 372e 3020 2f20  (floor(2997.0 / 
-000007c0: 332e 3029 290a 0a40 6578 7465 726e 616c  3.0))..@external
-000007d0: 0a64 6566 2066 6f6f 6d28 2920 2d3e 2069  .def foom() -> i
-000007e0: 6e74 3235 363a 0a20 2020 2072 6574 7572  nt256:.    retur
-000007f0: 6e28 666c 6f6f 7228 3139 3939 2e30 2025  n(floor(1999.0 %
-00000800: 2031 3030 302e 3029 290a 0a40 6578 7465   1000.0))..@exte
-00000810: 726e 616c 0a64 6566 2066 6f6f 7028 2920  rnal.def foop() 
-00000820: 2d3e 2069 6e74 3235 363a 0a20 2020 2072  -> int256:.    r
-00000830: 6574 7572 6e28 666c 6f6f 7228 3139 3939  eturn(floor(1999
-00000840: 2e30 2025 2031 3030 302e 3029 290a 2020  .0 % 1000.0)).  
-00000850: 2020 2222 220a 0a20 2020 2063 203d 2067    """..    c = g
-00000860: 6574 5f63 6f6e 7472 6163 745f 7769 7468  et_contract_with
-00000870: 5f67 6173 5f65 7374 696d 6174 696f 6e28  _gas_estimation(
-00000880: 6465 6369 6d61 6c5f 7465 7374 290a 0a20  decimal_test).. 
-00000890: 2020 2061 7373 6572 7420 632e 666f 6f28     assert c.foo(
-000008a0: 2920 3d3d 2039 3939 0a20 2020 2061 7373  ) == 999.    ass
-000008b0: 6572 7420 632e 666f 7028 2920 3d3d 2039  ert c.fop() == 9
-000008c0: 3939 0a20 2020 2061 7373 6572 7420 632e  99.    assert c.
-000008d0: 666f 7128 2920 3d3d 2039 3939 0a20 2020  foq() == 999.   
-000008e0: 2061 7373 6572 7420 632e 6261 7228 2920   assert c.bar() 
-000008f0: 3d3d 2039 3939 0a20 2020 2061 7373 6572  == 999.    asser
-00000900: 7420 632e 6261 7a28 2920 3d3d 2039 3939  t c.baz() == 999
-00000910: 0a20 2020 2061 7373 6572 7420 632e 6d6f  .    assert c.mo
-00000920: 6b28 2920 3d3d 2039 3939 0a20 2020 2061  k() == 999.    a
-00000930: 7373 6572 7420 632e 6d6f 6c28 2920 3d3d  ssert c.mol() ==
+00000020: 6f72 7420 6765 7463 6f6e 7465 7874 0a0a  ort getcontext..
+00000030: 696d 706f 7274 2070 7974 6573 740a 0a69  import pytest..i
+00000040: 6d70 6f72 7420 7679 7065 722e 636f 6d70  mport vyper.comp
+00000050: 696c 6572 2e73 6574 7469 6e67 7320 6173  iler.settings as
+00000060: 2063 6f6d 7069 6c65 725f 7365 7474 696e   compiler_settin
+00000070: 6773 0a66 726f 6d20 7465 7374 732e 7574  gs.from tests.ut
+00000080: 696c 7320 696d 706f 7274 2064 6563 696d  ils import decim
+00000090: 616c 5f74 6f5f 696e 740a 6672 6f6d 2076  al_to_int.from v
+000000a0: 7970 6572 2069 6d70 6f72 7420 636f 6d70  yper import comp
+000000b0: 696c 655f 636f 6465 0a66 726f 6d20 7679  ile_code.from vy
+000000c0: 7065 722e 6578 6365 7074 696f 6e73 2069  per.exceptions i
+000000d0: 6d70 6f72 7420 280a 2020 2020 4465 6369  mport (.    Deci
+000000e0: 6d61 6c4f 7665 7272 6964 6545 7863 6570  malOverrideExcep
+000000f0: 7469 6f6e 2c0a 2020 2020 4665 6174 7572  tion,.    Featur
+00000100: 6545 7863 6570 7469 6f6e 2c0a 2020 2020  eException,.    
+00000110: 496e 7661 6c69 644f 7065 7261 7469 6f6e  InvalidOperation
+00000120: 2c0a 2020 2020 4f76 6572 666c 6f77 4578  ,.    OverflowEx
+00000130: 6365 7074 696f 6e2c 0a20 2020 2054 7970  ception,.    Typ
+00000140: 654d 6973 6d61 7463 682c 0a29 0a66 726f  eMismatch,.).fro
+00000150: 6d20 7679 7065 722e 7574 696c 7320 696d  m vyper.utils im
+00000160: 706f 7274 2044 4543 494d 414c 5f45 5053  port DECIMAL_EPS
+00000170: 494c 4f4e 2c20 5369 7a65 4c69 6d69 7473  ILON, SizeLimits
+00000180: 2c20 7175 616e 7469 7a65 0a0a 0a64 6566  , quantize...def
+00000190: 2074 6573 745f 6465 6369 6d61 6c5f 6f76   test_decimal_ov
+000001a0: 6572 7269 6465 2829 3a0a 2020 2020 6765  erride():.    ge
+000001b0: 7463 6f6e 7465 7874 2829 2e70 7265 6320  tcontext().prec 
+000001c0: 3d20 3738 2020 2320 7365 7474 696e 6720  = 78  # setting 
+000001d0: 7072 6563 2074 6f20 3738 2069 7320 6f6b  prec to 78 is ok
+000001e0: 0a0a 2020 2020 2320 636f 6e73 756d 6572  ..    # consumer
+000001f0: 7320 6f66 2076 7970 6572 2c20 6576 656e  s of vyper, even
+00000200: 2061 7320 6120 6c69 6272 6172 792c 2061   as a library, a
+00000210: 7265 206e 6f74 2061 6c6c 6f77 6564 2074  re not allowed t
+00000220: 6f20 7265 6475 6365 2044 6563 696d 616c  o reduce Decimal
+00000230: 2070 7265 6369 7369 6f6e 0a20 2020 2077   precision.    w
+00000240: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+00000250: 7328 4465 6369 6d61 6c4f 7665 7272 6964  s(DecimalOverrid
+00000260: 6545 7863 6570 7469 6f6e 293a 0a20 2020  eException):.   
+00000270: 2020 2020 2067 6574 636f 6e74 6578 7428       getcontext(
+00000280: 292e 7072 6563 203d 2037 370a 0a20 2020  ).prec = 77..   
+00000290: 2077 6974 6820 7761 726e 696e 6773 2e63   with warnings.c
+000002a0: 6174 6368 5f77 6172 6e69 6e67 7328 7265  atch_warnings(re
+000002b0: 636f 7264 3d54 7275 6529 2061 7320 773a  cord=True) as w:
+000002c0: 0a20 2020 2020 2020 2067 6574 636f 6e74  .        getcont
+000002d0: 6578 7428 292e 7072 6563 203d 2037 390a  ext().prec = 79.
+000002e0: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+000002f0: 7761 726e 696e 6773 2077 6572 6520 6973  warnings were is
+00000300: 7375 6564 0a20 2020 2020 2020 2061 7373  sued.        ass
+00000310: 6572 7420 6c65 6e28 7729 203d 3d20 310a  ert len(w) == 1.
+00000320: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+00000330: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00000340: 2877 5b2d 315d 2e6d 6573 7361 6765 2920  (w[-1].message) 
+00000350: 3d3d 2022 4368 616e 6769 6e67 2064 6563  == "Changing dec
+00000360: 696d 616c 7320 7072 6563 6973 696f 6e20  imals precision 
+00000370: 636f 756c 6420 6861 7665 2075 6e69 6e74  could have unint
+00000380: 656e 6465 6420 7369 6465 2065 6666 6563  ended side effec
+00000390: 7473 2122 0a20 2020 2020 2020 2029 0a0a  ts!".        )..
+000003a0: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
+000003b0: 7261 6d65 7472 697a 6528 226f 7022 2c20  rametrize("op", 
+000003c0: 5b22 2f2f 222c 2022 2a2a 222c 2022 2622  ["//", "**", "&"
+000003d0: 2c20 227c 222c 2022 5e22 5d29 0a64 6566  , "|", "^"]).def
+000003e0: 2074 6573 745f 696e 7661 6c69 645f 6f70   test_invalid_op
+000003f0: 7328 6f70 293a 0a20 2020 2063 6f64 6520  s(op):.    code 
+00000400: 3d20 6622 2222 0a40 6578 7465 726e 616c  = f""".@external
+00000410: 0a64 6566 2066 6f6f 2878 3a20 6465 6369  .def foo(x: deci
+00000420: 6d61 6c2c 2079 3a20 6465 6369 6d61 6c29  mal, y: decimal)
+00000430: 202d 3e20 6465 6369 6d61 6c3a 0a20 2020   -> decimal:.   
+00000440: 2072 6574 7572 6e20 7820 7b6f 707d 2079   return x {op} y
+00000450: 0a20 2020 2022 2222 0a20 2020 2077 6974  .    """.    wit
+00000460: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
+00000470: 496e 7661 6c69 644f 7065 7261 7469 6f6e  InvalidOperation
+00000480: 293a 0a20 2020 2020 2020 2063 6f6d 7069  ):.        compi
+00000490: 6c65 5f63 6f64 6528 636f 6465 290a 0a0a  le_code(code)...
+000004a0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+000004b0: 616d 6574 7269 7a65 2822 6f70 222c 205b  ametrize("op", [
+000004c0: 226e 6f74 225d 290a 6465 6620 7465 7374  "not"]).def test
+000004d0: 5f69 6e76 616c 6964 5f75 6e61 7279 5f6f  _invalid_unary_o
+000004e0: 7073 286f 7029 3a0a 2020 2020 636f 6465  ps(op):.    code
+000004f0: 203d 2066 2222 220a 4065 7874 6572 6e61   = f""".@externa
+00000500: 6c0a 6465 6620 666f 6f28 783a 2064 6563  l.def foo(x: dec
+00000510: 696d 616c 2920 2d3e 2064 6563 696d 616c  imal) -> decimal
+00000520: 3a0a 2020 2020 7265 7475 726e 207b 6f70  :.    return {op
+00000530: 7d20 780a 2020 2020 2222 220a 2020 2020  } x.    """.    
+00000540: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+00000550: 6573 2849 6e76 616c 6964 4f70 6572 6174  es(InvalidOperat
+00000560: 696f 6e29 3a0a 2020 2020 2020 2020 636f  ion):.        co
+00000570: 6d70 696c 655f 636f 6465 2863 6f64 6529  mpile_code(code)
+00000580: 0a0a 0a64 6566 2074 6573 745f 6465 6369  ...def test_deci
+00000590: 6d61 6c5f 7465 7374 2867 6574 5f63 6f6e  mal_test(get_con
+000005a0: 7472 6163 745f 7769 7468 5f67 6173 5f65  tract_with_gas_e
+000005b0: 7374 696d 6174 696f 6e29 3a0a 2020 2020  stimation):.    
+000005c0: 6465 6369 6d61 6c5f 7465 7374 203d 2022  decimal_test = "
+000005d0: 2222 0a40 6578 7465 726e 616c 0a64 6566  "".@external.def
+000005e0: 2066 6f6f 2829 202d 3e20 696e 7432 3536   foo() -> int256
+000005f0: 3a0a 2020 2020 7265 7475 726e 2866 6c6f  :.    return(flo
+00000600: 6f72 2839 3939 2e30 2929 0a0a 4065 7874  or(999.0))..@ext
+00000610: 6572 6e61 6c0a 6465 6620 666f 7028 2920  ernal.def fop() 
+00000620: 2d3e 2069 6e74 3235 363a 0a20 2020 2072  -> int256:.    r
+00000630: 6574 7572 6e28 666c 6f6f 7228 3333 332e  eturn(floor(333.
+00000640: 3020 2b20 3636 362e 3029 290a 0a40 6578  0 + 666.0))..@ex
+00000650: 7465 726e 616c 0a64 6566 2066 6f71 2829  ternal.def foq()
+00000660: 202d 3e20 696e 7432 3536 3a0a 2020 2020   -> int256:.    
+00000670: 7265 7475 726e 2866 6c6f 6f72 2831 3333  return(floor(133
+00000680: 322e 3120 2d20 3333 332e 3129 290a 0a40  2.1 - 333.1))..@
+00000690: 6578 7465 726e 616c 0a64 6566 2062 6172  external.def bar
+000006a0: 2829 202d 3e20 696e 7432 3536 3a0a 2020  () -> int256:.  
+000006b0: 2020 7265 7475 726e 2866 6c6f 6f72 2832    return(floor(2
+000006c0: 372e 3020 2a20 3337 2e30 2929 0a0a 4065  7.0 * 37.0))..@e
+000006d0: 7874 6572 6e61 6c0a 6465 6620 6261 7a28  xternal.def baz(
+000006e0: 2920 2d3e 2069 6e74 3235 363a 0a20 2020  ) -> int256:.   
+000006f0: 2078 3a20 6465 6369 6d61 6c20 3d20 3237   x: decimal = 27
+00000700: 2e30 0a20 2020 2072 6574 7572 6e28 666c  .0.    return(fl
+00000710: 6f6f 7228 7820 2a20 3337 2e30 2929 0a0a  oor(x * 37.0))..
+00000720: 4065 7874 6572 6e61 6c0a 6465 6620 6d6f  @external.def mo
+00000730: 6b28 2920 2d3e 2069 6e74 3235 363a 0a20  k() -> int256:. 
+00000740: 2020 2072 6574 7572 6e28 666c 6f6f 7228     return(floor(
+00000750: 3939 3939 3939 2e30 202f 2037 2e30 202f  999999.0 / 7.0 /
+00000760: 2031 312e 3020 2f20 3133 2e30 2929 0a0a   11.0 / 13.0))..
+00000770: 4065 7874 6572 6e61 6c0a 6465 6620 6d6f  @external.def mo
+00000780: 6c28 2920 2d3e 2069 6e74 3235 363a 0a20  l() -> int256:. 
+00000790: 2020 2072 6574 7572 6e28 666c 6f6f 7228     return(floor(
+000007a0: 3439 392e 3520 2f20 302e 3529 290a 0a40  499.5 / 0.5))..@
+000007b0: 6578 7465 726e 616c 0a64 6566 206d 6f6d  external.def mom
+000007c0: 2829 202d 3e20 696e 7432 3536 3a0a 2020  () -> int256:.  
+000007d0: 2020 7265 7475 726e 2866 6c6f 6f72 2831    return(floor(1
+000007e0: 3439 382e 3520 2f20 312e 3529 290a 0a40  498.5 / 1.5))..@
+000007f0: 6578 7465 726e 616c 0a64 6566 206d 6f6f  external.def moo
+00000800: 2829 202d 3e20 696e 7432 3536 3a0a 2020  () -> int256:.  
+00000810: 2020 7265 7475 726e 2866 6c6f 6f72 2832    return(floor(2
+00000820: 3939 372e 3020 2f20 332e 3029 290a 0a40  997.0 / 3.0))..@
+00000830: 6578 7465 726e 616c 0a64 6566 2066 6f6f  external.def foo
+00000840: 6d28 2920 2d3e 2069 6e74 3235 363a 0a20  m() -> int256:. 
+00000850: 2020 2072 6574 7572 6e28 666c 6f6f 7228     return(floor(
+00000860: 3139 3939 2e30 2025 2031 3030 302e 3029  1999.0 % 1000.0)
+00000870: 290a 0a40 6578 7465 726e 616c 0a64 6566  )..@external.def
+00000880: 2066 6f6f 7028 2920 2d3e 2069 6e74 3235   foop() -> int25
+00000890: 363a 0a20 2020 2072 6574 7572 6e28 666c  6:.    return(fl
+000008a0: 6f6f 7228 3139 3939 2e30 2025 2031 3030  oor(1999.0 % 100
+000008b0: 302e 3029 290a 2020 2020 2222 220a 0a20  0.0)).    """.. 
+000008c0: 2020 2063 203d 2067 6574 5f63 6f6e 7472     c = get_contr
+000008d0: 6163 745f 7769 7468 5f67 6173 5f65 7374  act_with_gas_est
+000008e0: 696d 6174 696f 6e28 6465 6369 6d61 6c5f  imation(decimal_
+000008f0: 7465 7374 290a 0a20 2020 2061 7373 6572  test)..    asser
+00000900: 7420 632e 666f 6f28 2920 3d3d 2039 3939  t c.foo() == 999
+00000910: 0a20 2020 2061 7373 6572 7420 632e 666f  .    assert c.fo
+00000920: 7028 2920 3d3d 2039 3939 0a20 2020 2061  p() == 999.    a
+00000930: 7373 6572 7420 632e 666f 7128 2920 3d3d  ssert c.foq() ==
 00000940: 2039 3939 0a20 2020 2061 7373 6572 7420   999.    assert 
-00000950: 632e 6d6f 6d28 2920 3d3d 2039 3939 0a20  c.mom() == 999. 
-00000960: 2020 2061 7373 6572 7420 632e 6d6f 6f28     assert c.moo(
+00000950: 632e 6261 7228 2920 3d3d 2039 3939 0a20  c.bar() == 999. 
+00000960: 2020 2061 7373 6572 7420 632e 6261 7a28     assert c.baz(
 00000970: 2920 3d3d 2039 3939 0a20 2020 2061 7373  ) == 999.    ass
-00000980: 6572 7420 632e 666f 6f6d 2829 203d 3d20  ert c.foom() == 
-00000990: 3939 390a 2020 2020 6173 7365 7274 2063  999.    assert c
-000009a0: 2e66 6f6f 7028 2920 3d3d 2039 3939 0a0a  .foop() == 999..
-000009b0: 2020 2020 7072 696e 7428 2250 6173 7365      print("Passe
-000009c0: 6420 6261 7369 6320 6164 6469 7469 6f6e  d basic addition
-000009d0: 2c20 7375 6274 7261 6374 696f 6e20 616e  , subtraction an
-000009e0: 6420 6d75 6c74 6970 6c69 6361 7469 6f6e  d multiplication
-000009f0: 2074 6573 7473 2229 0a0a 0a64 6566 2074   tests")...def t
-00000a00: 6573 745f 6861 7264 6572 5f64 6563 696d  est_harder_decim
-00000a10: 616c 5f74 6573 7428 6765 745f 636f 6e74  al_test(get_cont
-00000a20: 7261 6374 5f77 6974 685f 6761 735f 6573  ract_with_gas_es
-00000a30: 7469 6d61 7469 6f6e 293a 0a20 2020 2068  timation):.    h
-00000a40: 6172 6465 725f 6465 6369 6d61 6c5f 7465  arder_decimal_te
-00000a50: 7374 203d 2022 2222 0a40 6578 7465 726e  st = """.@extern
-00000a60: 616c 0a64 6566 2070 686f 6f65 7928 696e  al.def phooey(in
-00000a70: 703a 2064 6563 696d 616c 2920 2d3e 2064  p: decimal) -> d
-00000a80: 6563 696d 616c 3a0a 2020 2020 783a 2064  ecimal:.    x: d
-00000a90: 6563 696d 616c 203d 2031 3030 3030 2e30  ecimal = 10000.0
-00000aa0: 0a20 2020 2066 6f72 2069 3a20 7569 6e74  .    for i: uint
-00000ab0: 3235 3620 696e 2072 616e 6765 2834 293a  256 in range(4):
-00000ac0: 0a20 2020 2020 2020 2078 203d 2078 202a  .        x = x *
-00000ad0: 2069 6e70 0a20 2020 2072 6574 7572 6e20   inp.    return 
-00000ae0: 780a 0a40 6578 7465 726e 616c 0a64 6566  x..@external.def
-00000af0: 2061 7267 2869 6e70 3a20 6465 6369 6d61   arg(inp: decima
-00000b00: 6c29 202d 3e20 6465 6369 6d61 6c3a 0a20  l) -> decimal:. 
-00000b10: 2020 2072 6574 7572 6e20 696e 700a 0a40     return inp..@
-00000b20: 6578 7465 726e 616c 0a64 6566 2067 6172  external.def gar
-00000b30: 6728 2920 2d3e 2064 6563 696d 616c 3a0a  g() -> decimal:.
-00000b40: 2020 2020 783a 2064 6563 696d 616c 203d      x: decimal =
-00000b50: 2034 2e35 0a20 2020 2078 202a 3d20 312e   4.5.    x *= 1.
-00000b60: 350a 2020 2020 7265 7475 726e 2078 0a0a  5.    return x..
-00000b70: 4065 7874 6572 6e61 6c0a 6465 6620 6861  @external.def ha
-00000b80: 7267 2829 202d 3e20 6465 6369 6d61 6c3a  rg() -> decimal:
-00000b90: 0a20 2020 2078 3a20 6465 6369 6d61 6c20  .    x: decimal 
-00000ba0: 3d20 342e 350a 2020 2020 7820 2a3d 2032  = 4.5.    x *= 2
-00000bb0: 2e30 0a20 2020 2072 6574 7572 6e20 780a  .0.    return x.
-00000bc0: 0a40 6578 7465 726e 616c 0a64 6566 2069  .@external.def i
-00000bd0: 6172 6728 2920 2d3e 2075 696e 7432 3536  arg() -> uint256
-00000be0: 3a0a 2020 2020 783a 2075 696e 7432 3536  :.    x: uint256
-00000bf0: 203d 2061 735f 7765 695f 7661 6c75 6528   = as_wei_value(
-00000c00: 372c 2022 7765 6922 290a 2020 2020 7820  7, "wei").    x 
-00000c10: 2a3d 2032 0a20 2020 2072 6574 7572 6e20  *= 2.    return 
-00000c20: 780a 2020 2020 2222 220a 0a20 2020 2063  x.    """..    c
-00000c30: 203d 2067 6574 5f63 6f6e 7472 6163 745f   = get_contract_
-00000c40: 7769 7468 5f67 6173 5f65 7374 696d 6174  with_gas_estimat
-00000c50: 696f 6e28 6861 7264 6572 5f64 6563 696d  ion(harder_decim
-00000c60: 616c 5f74 6573 7429 0a20 2020 2061 7373  al_test).    ass
-00000c70: 6572 7420 632e 7068 6f6f 6579 2844 6563  ert c.phooey(Dec
-00000c80: 696d 616c 2822 312e 3222 2929 203d 3d20  imal("1.2")) == 
-00000c90: 4465 6369 6d61 6c28 2232 3037 3336 2e30  Decimal("20736.0
-00000ca0: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
-00000cb0: 7068 6f6f 6579 2844 6563 696d 616c 2822  phooey(Decimal("
-00000cc0: 2d31 2e32 2229 2920 3d3d 2044 6563 696d  -1.2")) == Decim
-00000cd0: 616c 2822 3230 3733 362e 3022 290a 2020  al("20736.0").  
-00000ce0: 2020 6173 7365 7274 2063 2e61 7267 2844    assert c.arg(D
-00000cf0: 6563 696d 616c 2822 2d33 2e37 2229 2920  ecimal("-3.7")) 
-00000d00: 3d3d 2044 6563 696d 616c 2822 2d33 2e37  == Decimal("-3.7
-00000d10: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
-00000d20: 6172 6728 4465 6369 6d61 6c28 2233 2e37  arg(Decimal("3.7
-00000d30: 2229 2920 3d3d 2044 6563 696d 616c 2822  ")) == Decimal("
-00000d40: 332e 3722 290a 2020 2020 6173 7365 7274  3.7").    assert
-00000d50: 2063 2e67 6172 6728 2920 3d3d 2044 6563   c.garg() == Dec
-00000d60: 696d 616c 2822 362e 3735 2229 0a20 2020  imal("6.75").   
-00000d70: 2061 7373 6572 7420 632e 6861 7267 2829   assert c.harg()
-00000d80: 203d 3d20 4465 6369 6d61 6c28 2239 2e30   == Decimal("9.0
-00000d90: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
-00000da0: 6961 7267 2829 203d 3d20 4465 6369 6d61  iarg() == Decima
-00000db0: 6c28 2231 3422 290a 0a20 2020 2070 7269  l("14")..    pri
-00000dc0: 6e74 2822 5061 7373 6564 2066 7261 6374  nt("Passed fract
-00000dd0: 696f 6e61 6c20 6d75 6c74 6970 6c69 6361  ional multiplica
-00000de0: 7469 6f6e 2074 6573 7422 290a 0a0a 6465  tion test")...de
-00000df0: 6620 7465 7374 5f6d 756c 5f6f 7665 7266  f test_mul_overf
-00000e00: 6c6f 7728 7478 5f66 6169 6c65 642c 2067  low(tx_failed, g
-00000e10: 6574 5f63 6f6e 7472 6163 745f 7769 7468  et_contract_with
-00000e20: 5f67 6173 5f65 7374 696d 6174 696f 6e29  _gas_estimation)
-00000e30: 3a0a 2020 2020 6d75 6c5f 636f 6465 203d  :.    mul_code =
-00000e40: 2022 2222 0a0a 4065 7874 6572 6e61 6c0a   """..@external.
-00000e50: 6465 6620 5f6e 756d 5f6d 756c 2878 3a20  def _num_mul(x: 
-00000e60: 6465 6369 6d61 6c2c 2079 3a20 6465 6369  decimal, y: deci
-00000e70: 6d61 6c29 202d 3e20 6465 6369 6d61 6c3a  mal) -> decimal:
-00000e80: 0a20 2020 2072 6574 7572 6e20 7820 2a20  .    return x * 
-00000e90: 790a 0a20 2020 2022 2222 0a0a 2020 2020  y..    """..    
-00000ea0: 6320 3d20 6765 745f 636f 6e74 7261 6374  c = get_contract
-00000eb0: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
-00000ec0: 7469 6f6e 286d 756c 5f63 6f64 6529 0a0a  tion(mul_code)..
-00000ed0: 2020 2020 7820 3d20 4465 6369 6d61 6c28      x = Decimal(
-00000ee0: 2238 3530 3730 3539 3137 3330 3233 3436  "850705917302346
-00000ef0: 3135 3836 3538 3433 3635 3138 3537 3934  1586584365185794
-00000f00: 3230 3532 3836 3422 290a 2020 2020 7920  2052864").    y 
-00000f10: 3d20 4465 6369 6d61 6c28 2231 3336 3131  = Decimal("13611
-00000f20: 3239 3436 3736 3833 3735 3338 3533 3835  2946768375385385
-00000f30: 3334 3938 3432 3937 3322 290a 0a20 2020  349842973")..   
-00000f40: 2077 6974 6820 7478 5f66 6169 6c65 6428   with tx_failed(
-00000f50: 293a 0a20 2020 2020 2020 2063 2e5f 6e75  ):.        c._nu
-00000f60: 6d5f 6d75 6c28 782c 2079 290a 0a20 2020  m_mul(x, y)..   
-00000f70: 2078 203d 2053 697a 654c 696d 6974 732e   x = SizeLimits.
-00000f80: 4d41 585f 4153 545f 4445 4349 4d41 4c0a  MAX_AST_DECIMAL.
-00000f90: 2020 2020 7920 3d20 3120 2b20 4445 4349      y = 1 + DECI
-00000fa0: 4d41 4c5f 4550 5349 4c4f 4e0a 0a20 2020  MAL_EPSILON..   
-00000fb0: 2077 6974 6820 7478 5f66 6169 6c65 6428   with tx_failed(
-00000fc0: 293a 0a20 2020 2020 2020 2063 2e5f 6e75  ):.        c._nu
-00000fd0: 6d5f 6d75 6c28 782c 2079 290a 0a20 2020  m_mul(x, y)..   
-00000fe0: 2061 7373 6572 7420 632e 5f6e 756d 5f6d   assert c._num_m
-00000ff0: 756c 2878 2c20 4465 6369 6d61 6c28 3129  ul(x, Decimal(1)
-00001000: 2920 3d3d 2078 0a0a 2020 2020 6173 7365  ) == x..    asse
-00001010: 7274 2063 2e5f 6e75 6d5f 6d75 6c28 782c  rt c._num_mul(x,
-00001020: 2031 202d 2044 4543 494d 414c 5f45 5053   1 - DECIMAL_EPS
-00001030: 494c 4f4e 2920 3d3d 2071 7561 6e74 697a  ILON) == quantiz
-00001040: 6528 7820 2a20 2831 202d 2044 4543 494d  e(x * (1 - DECIM
-00001050: 414c 5f45 5053 494c 4f4e 2929 0a0a 2020  AL_EPSILON))..  
-00001060: 2020 7820 3d20 5369 7a65 4c69 6d69 7473    x = SizeLimits
-00001070: 2e4d 494e 5f41 5354 5f44 4543 494d 414c  .MIN_AST_DECIMAL
-00001080: 0a20 2020 2061 7373 6572 7420 632e 5f6e  .    assert c._n
-00001090: 756d 5f6d 756c 2878 2c20 3120 2d20 4445  um_mul(x, 1 - DE
-000010a0: 4349 4d41 4c5f 4550 5349 4c4f 4e29 203d  CIMAL_EPSILON) =
-000010b0: 3d20 7175 616e 7469 7a65 2878 202a 2028  = quantize(x * (
-000010c0: 3120 2d20 4445 4349 4d41 4c5f 4550 5349  1 - DECIMAL_EPSI
-000010d0: 4c4f 4e29 290a 0a0a 2320 6469 7669 7369  LON))...# divisi
-000010e0: 6f6e 2066 6169 6c75 7265 206d 6f64 6573  on failure modes
-000010f0: 2821 290a 6465 6620 7465 7374 5f64 6976  (!).def test_div
-00001100: 5f6f 7665 7266 6c6f 7728 6765 745f 636f  _overflow(get_co
-00001110: 6e74 7261 6374 2c20 7478 5f66 6169 6c65  ntract, tx_faile
-00001120: 6429 3a0a 2020 2020 636f 6465 203d 2022  d):.    code = "
-00001130: 2222 0a40 6578 7465 726e 616c 0a64 6566  "".@external.def
-00001140: 2066 6f6f 2878 3a20 6465 6369 6d61 6c2c   foo(x: decimal,
-00001150: 2079 3a20 6465 6369 6d61 6c29 202d 3e20   y: decimal) -> 
-00001160: 6465 6369 6d61 6c3a 0a20 2020 2072 6574  decimal:.    ret
-00001170: 7572 6e20 7820 2f20 790a 2020 2020 2222  urn x / y.    ""
-00001180: 220a 0a20 2020 2063 203d 2067 6574 5f63  "..    c = get_c
-00001190: 6f6e 7472 6163 7428 636f 6465 290a 0a20  ontract(code).. 
-000011a0: 2020 2078 203d 2053 697a 654c 696d 6974     x = SizeLimit
-000011b0: 732e 4d49 4e5f 4153 545f 4445 4349 4d41  s.MIN_AST_DECIMA
-000011c0: 4c0a 2020 2020 7920 3d20 2d44 4543 494d  L.    y = -DECIM
-000011d0: 414c 5f45 5053 494c 4f4e 0a0a 2020 2020  AL_EPSILON..    
-000011e0: 7769 7468 2074 785f 6661 696c 6564 2829  with tx_failed()
-000011f0: 3a0a 2020 2020 2020 2020 632e 666f 6f28  :.        c.foo(
-00001200: 782c 2079 290a 2020 2020 7769 7468 2074  x, y).    with t
-00001210: 785f 6661 696c 6564 2829 3a0a 2020 2020  x_failed():.    
-00001220: 2020 2020 632e 666f 6f28 782c 2044 6563      c.foo(x, Dec
-00001230: 696d 616c 2830 2929 0a20 2020 2077 6974  imal(0)).    wit
-00001240: 6820 7478 5f66 6169 6c65 6428 293a 0a20  h tx_failed():. 
-00001250: 2020 2020 2020 2063 2e66 6f6f 2879 2c20         c.foo(y, 
-00001260: 4465 6369 6d61 6c28 3029 290a 0a20 2020  Decimal(0))..   
-00001270: 2079 203d 2044 6563 696d 616c 2831 2920   y = Decimal(1) 
-00001280: 2d20 4445 4349 4d41 4c5f 4550 5349 4c4f  - DECIMAL_EPSILO
-00001290: 4e20 2023 2030 2e39 3939 3939 3939 3939  N  # 0.999999999
-000012a0: 0a20 2020 2077 6974 6820 7478 5f66 6169  .    with tx_fai
-000012b0: 6c65 6428 293a 0a20 2020 2020 2020 2063  led():.        c
-000012c0: 2e66 6f6f 2878 2c20 7929 0a0a 2020 2020  .foo(x, y)..    
-000012d0: 7920 3d20 4465 6369 6d61 6c28 2d31 290a  y = Decimal(-1).
-000012e0: 2020 2020 7769 7468 2074 785f 6661 696c      with tx_fail
-000012f0: 6564 2829 3a0a 2020 2020 2020 2020 632e  ed():.        c.
-00001300: 666f 6f28 782c 2079 290a 0a20 2020 2061  foo(x, y)..    a
-00001310: 7373 6572 7420 632e 666f 6f28 782c 2044  ssert c.foo(x, D
-00001320: 6563 696d 616c 2831 2929 203d 3d20 780a  ecimal(1)) == x.
-00001330: 2020 2020 6173 7365 7274 2063 2e66 6f6f      assert c.foo
-00001340: 2878 2c20 3120 2b20 4445 4349 4d41 4c5f  (x, 1 + DECIMAL_
-00001350: 4550 5349 4c4f 4e29 203d 3d20 7175 616e  EPSILON) == quan
-00001360: 7469 7a65 2878 202f 2028 3120 2b20 4445  tize(x / (1 + DE
-00001370: 4349 4d41 4c5f 4550 5349 4c4f 4e29 290a  CIMAL_EPSILON)).
-00001380: 0a20 2020 2078 203d 2053 697a 654c 696d  .    x = SizeLim
-00001390: 6974 732e 4d41 585f 4153 545f 4445 4349  its.MAX_AST_DECI
-000013a0: 4d41 4c0a 0a20 2020 2077 6974 6820 7478  MAL..    with tx
-000013b0: 5f66 6169 6c65 6428 293a 0a20 2020 2020  _failed():.     
-000013c0: 2020 2063 2e66 6f6f 2878 2c20 4445 4349     c.foo(x, DECI
-000013d0: 4d41 4c5f 4550 5349 4c4f 4e29 0a0a 2020  MAL_EPSILON)..  
-000013e0: 2020 7920 3d20 4465 6369 6d61 6c28 3129    y = Decimal(1)
-000013f0: 202d 2044 4543 494d 414c 5f45 5053 494c   - DECIMAL_EPSIL
-00001400: 4f4e 0a20 2020 2077 6974 6820 7478 5f66  ON.    with tx_f
-00001410: 6169 6c65 6428 293a 0a20 2020 2020 2020  ailed():.       
-00001420: 2063 2e66 6f6f 2878 2c20 7929 0a0a 2020   c.foo(x, y)..  
-00001430: 2020 6173 7365 7274 2063 2e66 6f6f 2878    assert c.foo(x
-00001440: 2c20 4465 6369 6d61 6c28 3129 2920 3d3d  , Decimal(1)) ==
-00001450: 2078 0a0a 2020 2020 6173 7365 7274 2063   x..    assert c
-00001460: 2e66 6f6f 2878 2c20 3120 2b20 4445 4349  .foo(x, 1 + DECI
-00001470: 4d41 4c5f 4550 5349 4c4f 4e29 203d 3d20  MAL_EPSILON) == 
-00001480: 7175 616e 7469 7a65 2878 202f 2028 3120  quantize(x / (1 
-00001490: 2b20 4445 4349 4d41 4c5f 4550 5349 4c4f  + DECIMAL_EPSILO
-000014a0: 4e29 290a 0a0a 6465 6620 7465 7374 5f64  N))...def test_d
-000014b0: 6563 696d 616c 5f6d 696e 5f6d 6178 5f6c  ecimal_min_max_l
-000014c0: 6974 6572 616c 7328 7478 5f66 6169 6c65  iterals(tx_faile
-000014d0: 642c 2067 6574 5f63 6f6e 7472 6163 745f  d, get_contract_
-000014e0: 7769 7468 5f67 6173 5f65 7374 696d 6174  with_gas_estimat
-000014f0: 696f 6e29 3a0a 2020 2020 636f 6465 203d  ion):.    code =
-00001500: 2022 2222 0a40 6578 7465 726e 616c 0a64   """.@external.d
-00001510: 6566 206d 6178 696d 756d 2829 3a0a 2020  ef maximum():.  
-00001520: 2020 613a 2064 6563 696d 616c 203d 2031    a: decimal = 1
-00001530: 3837 3037 3232 3039 3537 3833 3535 3537  8707220957835557
-00001540: 3335 3330 3037 3136 3538 3538 3736 3834  3530071658587684
-00001550: 3232 3635 3135 3935 2e39 3336 3535 3030  22651595.9365500
-00001560: 3932 370a 4065 7874 6572 6e61 6c0a 6465  927.@external.de
-00001570: 6620 6d69 6e69 6d75 6d28 293a 0a20 2020  f minimum():.   
-00001580: 2061 3a20 6465 6369 6d61 6c20 3d20 2d31   a: decimal = -1
-00001590: 3837 3037 3232 3039 3537 3833 3535 3537  8707220957835557
-000015a0: 3335 3330 3037 3136 3538 3538 3736 3834  3530071658587684
-000015b0: 3232 3635 3135 3935 2e39 3336 3535 3030  22651595.9365500
-000015c0: 3932 380a 2020 2020 2222 220a 2020 2020  928.    """.    
-000015d0: 6320 3d20 6765 745f 636f 6e74 7261 6374  c = get_contract
-000015e0: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
-000015f0: 7469 6f6e 2863 6f64 6529 0a0a 2020 2020  tion(code)..    
-00001600: 6173 7365 7274 2063 2e6d 6178 696d 756d  assert c.maximum
-00001610: 2829 203d 3d20 5b5d 0a20 2020 2061 7373  () == [].    ass
-00001620: 6572 7420 632e 6d69 6e69 6d75 6d28 2920  ert c.minimum() 
-00001630: 3d3d 205b 5d0a 0a0a 6465 6620 7465 7374  == []...def test
-00001640: 5f73 6369 656e 7469 6669 635f 6e6f 7461  _scientific_nota
-00001650: 7469 6f6e 2867 6574 5f63 6f6e 7472 6163  tion(get_contrac
-00001660: 745f 7769 7468 5f67 6173 5f65 7374 696d  t_with_gas_estim
-00001670: 6174 696f 6e29 3a0a 2020 2020 636f 6465  ation):.    code
-00001680: 203d 2022 2222 0a40 6578 7465 726e 616c   = """.@external
-00001690: 0a64 6566 2066 6f6f 2829 202d 3e20 6465  .def foo() -> de
-000016a0: 6369 6d61 6c3a 0a20 2020 2072 6574 7572  cimal:.    retur
-000016b0: 6e20 3165 2d31 300a 0a40 6578 7465 726e  n 1e-10..@extern
-000016c0: 616c 0a64 6566 2062 6172 286e 756d 3a20  al.def bar(num: 
-000016d0: 6465 6369 6d61 6c29 202d 3e20 6465 6369  decimal) -> deci
-000016e0: 6d61 6c3a 0a20 2020 2072 6574 7572 6e20  mal:.    return 
-000016f0: 6e75 6d20 2b20 2d31 6533 380a 2020 2020  num + -1e38.    
-00001700: 2222 220a 2020 2020 6320 3d20 6765 745f  """.    c = get_
-00001710: 636f 6e74 7261 6374 5f77 6974 685f 6761  contract_with_ga
-00001720: 735f 6573 7469 6d61 7469 6f6e 2863 6f64  s_estimation(cod
-00001730: 6529 0a0a 2020 2020 6173 7365 7274 2063  e)..    assert c
-00001740: 2e66 6f6f 2829 203d 3d20 4465 6369 6d61  .foo() == Decima
-00001750: 6c28 2231 652d 3130 2229 2020 2320 536d  l("1e-10")  # Sm
-00001760: 616c 6c65 7374 2070 6f73 7369 626c 6520  allest possible 
-00001770: 6465 6369 6d61 6c0a 2020 2020 6173 7365  decimal.    asse
-00001780: 7274 2063 2e62 6172 2844 6563 696d 616c  rt c.bar(Decimal
-00001790: 2822 3165 3337 2229 2920 3d3d 2044 6563  ("1e37")) == Dec
-000017a0: 696d 616c 2822 2d39 6533 3722 2920 2023  imal("-9e37")  #
-000017b0: 204d 6174 6820 6c69 6e65 7320 7570 0a0a   Math lines up..
-000017c0: 0a64 6566 2074 6573 745f 6578 706f 6e65  .def test_expone
-000017d0: 6e74 7328 293a 0a20 2020 2063 6f64 6520  nts():.    code 
-000017e0: 3d20 2222 220a 4065 7874 6572 6e61 6c0a  = """.@external.
-000017f0: 6465 6620 666f 6f28 2920 2d3e 2064 6563  def foo() -> dec
-00001800: 696d 616c 3a0a 2020 2020 7265 7475 726e  imal:.    return
-00001810: 2032 2e32 202a 2a20 322e 300a 2020 2020   2.2 ** 2.0.    
-00001820: 2222 220a 0a20 2020 2077 6974 6820 7079  """..    with py
-00001830: 7465 7374 2e72 6169 7365 7328 5479 7065  test.raises(Type
-00001840: 4d69 736d 6174 6368 293a 0a20 2020 2020  Mismatch):.     
-00001850: 2020 2063 6f6d 7069 6c65 5f63 6f64 6528     compile_code(
-00001860: 636f 6465 290a 0a0a 6465 6620 7465 7374  code)...def test
-00001870: 5f64 6563 696d 616c 5f6e 6573 7465 645f  _decimal_nested_
-00001880: 696e 7465 726d 6564 6961 7465 5f6f 7665  intermediate_ove
-00001890: 7266 6c6f 7728 293a 0a20 2020 2063 6f64  rflow():.    cod
-000018a0: 6520 3d20 2222 220a 4065 7874 6572 6e61  e = """.@externa
-000018b0: 6c0a 6465 6620 666f 6f28 293a 0a20 2020  l.def foo():.   
-000018c0: 2061 3a20 6465 6369 6d61 6c20 3d20 3138   a: decimal = 18
-000018d0: 3730 3732 3230 3935 3738 3335 3535 3733  7072209578355573
-000018e0: 3533 3030 3731 3635 3835 3837 3638 3432  5300716585876842
-000018f0: 3236 3531 3539 352e 3933 3635 3530 3039  2651595.93655009
-00001900: 3237 202b 2031 652d 3130 202d 2031 652d  27 + 1e-10 - 1e-
-00001910: 3130 0a20 2020 2022 2222 0a20 2020 2077  10.    """.    w
-00001920: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
-00001930: 7328 4f76 6572 666c 6f77 4578 6365 7074  s(OverflowExcept
-00001940: 696f 6e29 3a0a 2020 2020 2020 2020 636f  ion):.        co
-00001950: 6d70 696c 655f 636f 6465 2863 6f64 6529  mpile_code(code)
-00001960: 0a0a 0a64 6566 2074 6573 745f 7265 706c  ...def test_repl
-00001970: 6163 655f 6465 6369 6d61 6c5f 6e65 7374  ace_decimal_nest
-00001980: 6564 5f69 6e74 6572 6d65 6469 6174 655f  ed_intermediate_
-00001990: 756e 6465 7266 6c6f 7728 6475 6d6d 795f  underflow(dummy_
-000019a0: 696e 7075 745f 6275 6e64 6c65 293a 0a20  input_bundle):. 
-000019b0: 2020 2063 6f64 6520 3d20 2222 220a 4065     code = """.@e
-000019c0: 7874 6572 6e61 6c0a 6465 6620 666f 6f28  xternal.def foo(
-000019d0: 293a 0a20 2020 2061 3a20 6465 6369 6d61  ):.    a: decima
-000019e0: 6c20 3d20 2d31 3837 3037 3232 3039 3537  l = -18707220957
-000019f0: 3833 3535 3537 3335 3330 3037 3136 3538  8355573530071658
-00001a00: 3538 3736 3834 3232 3635 3135 3935 2e39  58768422651595.9
-00001a10: 3336 3535 3030 3932 3820 2d20 3165 2d31  365500928 - 1e-1
-00001a20: 3020 2b20 3165 2d31 300a 2020 2020 2222  0 + 1e-10.    ""
-00001a30: 220a 2020 2020 7769 7468 2070 7974 6573  ".    with pytes
-00001a40: 742e 7261 6973 6573 284f 7665 7266 6c6f  t.raises(Overflo
-00001a50: 7745 7863 6570 7469 6f6e 293a 0a20 2020  wException):.   
-00001a60: 2020 2020 2063 6f6d 7069 6c65 5f63 6f64       compile_cod
-00001a70: 6528 636f 6465 290a 0a0a 6465 6620 7465  e(code)...def te
-00001a80: 7374 5f69 6e76 616c 6964 5f66 6c6f 6f72  st_invalid_floor
-00001a90: 6469 7628 293a 0a20 2020 2063 6f64 6520  div():.    code 
-00001aa0: 3d20 2222 220a 4065 7874 6572 6e61 6c0a  = """.@external.
-00001ab0: 6465 6620 666f 6f28 293a 0a20 2020 2061  def foo():.    a
-00001ac0: 3a20 6465 6369 6d61 6c20 3d20 352e 3020  : decimal = 5.0 
-00001ad0: 2f2f 2039 2e30 0a20 2020 2022 2222 0a20  // 9.0.    """. 
-00001ae0: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-00001af0: 6169 7365 7328 496e 7661 6c69 644f 7065  aises(InvalidOpe
-00001b00: 7261 7469 6f6e 2920 6173 2065 3a0a 2020  ration) as e:.  
-00001b10: 2020 2020 2020 636f 6d70 696c 655f 636f        compile_co
-00001b20: 6465 2863 6f64 6529 0a0a 2020 2020 6173  de(code)..    as
-00001b30: 7365 7274 2065 2e76 616c 7565 2e5f 6869  sert e.value._hi
-00001b40: 6e74 203d 3d20 2264 6964 2079 6f75 206d  nt == "did you m
-00001b50: 6561 6e20 6035 2e30 202f 2039 2e30 603f  ean `5.0 / 9.0`?
-00001b60: 220a                                     ".
+00000980: 6572 7420 632e 6d6f 6b28 2920 3d3d 2039  ert c.mok() == 9
+00000990: 3939 0a20 2020 2061 7373 6572 7420 632e  99.    assert c.
+000009a0: 6d6f 6c28 2920 3d3d 2039 3939 0a20 2020  mol() == 999.   
+000009b0: 2061 7373 6572 7420 632e 6d6f 6d28 2920   assert c.mom() 
+000009c0: 3d3d 2039 3939 0a20 2020 2061 7373 6572  == 999.    asser
+000009d0: 7420 632e 6d6f 6f28 2920 3d3d 2039 3939  t c.moo() == 999
+000009e0: 0a20 2020 2061 7373 6572 7420 632e 666f  .    assert c.fo
+000009f0: 6f6d 2829 203d 3d20 3939 390a 2020 2020  om() == 999.    
+00000a00: 6173 7365 7274 2063 2e66 6f6f 7028 2920  assert c.foop() 
+00000a10: 3d3d 2039 3939 0a0a 2020 2020 7072 696e  == 999..    prin
+00000a20: 7428 2250 6173 7365 6420 6261 7369 6320  t("Passed basic 
+00000a30: 6164 6469 7469 6f6e 2c20 7375 6274 7261  addition, subtra
+00000a40: 6374 696f 6e20 616e 6420 6d75 6c74 6970  ction and multip
+00000a50: 6c69 6361 7469 6f6e 2074 6573 7473 2229  lication tests")
+00000a60: 0a0a 0a64 6566 2074 6573 745f 6861 7264  ...def test_hard
+00000a70: 6572 5f64 6563 696d 616c 5f74 6573 7428  er_decimal_test(
+00000a80: 6765 745f 636f 6e74 7261 6374 5f77 6974  get_contract_wit
+00000a90: 685f 6761 735f 6573 7469 6d61 7469 6f6e  h_gas_estimation
+00000aa0: 293a 0a20 2020 2068 6172 6465 725f 6465  ):.    harder_de
+00000ab0: 6369 6d61 6c5f 7465 7374 203d 2022 2222  cimal_test = """
+00000ac0: 0a40 6578 7465 726e 616c 0a64 6566 2070  .@external.def p
+00000ad0: 686f 6f65 7928 696e 703a 2064 6563 696d  hooey(inp: decim
+00000ae0: 616c 2920 2d3e 2064 6563 696d 616c 3a0a  al) -> decimal:.
+00000af0: 2020 2020 783a 2064 6563 696d 616c 203d      x: decimal =
+00000b00: 2031 3030 3030 2e30 0a20 2020 2066 6f72   10000.0.    for
+00000b10: 2069 3a20 7569 6e74 3235 3620 696e 2072   i: uint256 in r
+00000b20: 616e 6765 2834 293a 0a20 2020 2020 2020  ange(4):.       
+00000b30: 2078 203d 2078 202a 2069 6e70 0a20 2020   x = x * inp.   
+00000b40: 2072 6574 7572 6e20 780a 0a40 6578 7465   return x..@exte
+00000b50: 726e 616c 0a64 6566 2061 7267 2869 6e70  rnal.def arg(inp
+00000b60: 3a20 6465 6369 6d61 6c29 202d 3e20 6465  : decimal) -> de
+00000b70: 6369 6d61 6c3a 0a20 2020 2072 6574 7572  cimal:.    retur
+00000b80: 6e20 696e 700a 0a40 6578 7465 726e 616c  n inp..@external
+00000b90: 0a64 6566 2067 6172 6728 2920 2d3e 2064  .def garg() -> d
+00000ba0: 6563 696d 616c 3a0a 2020 2020 783a 2064  ecimal:.    x: d
+00000bb0: 6563 696d 616c 203d 2034 2e35 0a20 2020  ecimal = 4.5.   
+00000bc0: 2078 202a 3d20 312e 350a 2020 2020 7265   x *= 1.5.    re
+00000bd0: 7475 726e 2078 0a0a 4065 7874 6572 6e61  turn x..@externa
+00000be0: 6c0a 6465 6620 6861 7267 2829 202d 3e20  l.def harg() -> 
+00000bf0: 6465 6369 6d61 6c3a 0a20 2020 2078 3a20  decimal:.    x: 
+00000c00: 6465 6369 6d61 6c20 3d20 342e 350a 2020  decimal = 4.5.  
+00000c10: 2020 7820 2a3d 2032 2e30 0a20 2020 2072    x *= 2.0.    r
+00000c20: 6574 7572 6e20 780a 0a40 6578 7465 726e  eturn x..@extern
+00000c30: 616c 0a64 6566 2069 6172 6728 2920 2d3e  al.def iarg() ->
+00000c40: 2075 696e 7432 3536 3a0a 2020 2020 783a   uint256:.    x:
+00000c50: 2075 696e 7432 3536 203d 2061 735f 7765   uint256 = as_we
+00000c60: 695f 7661 6c75 6528 372c 2022 7765 6922  i_value(7, "wei"
+00000c70: 290a 2020 2020 7820 2a3d 2032 0a20 2020  ).    x *= 2.   
+00000c80: 2072 6574 7572 6e20 780a 2020 2020 2222   return x.    ""
+00000c90: 220a 0a20 2020 2063 203d 2067 6574 5f63  "..    c = get_c
+00000ca0: 6f6e 7472 6163 745f 7769 7468 5f67 6173  ontract_with_gas
+00000cb0: 5f65 7374 696d 6174 696f 6e28 6861 7264  _estimation(hard
+00000cc0: 6572 5f64 6563 696d 616c 5f74 6573 7429  er_decimal_test)
+00000cd0: 0a20 2020 2061 7373 6572 7420 632e 7068  .    assert c.ph
+00000ce0: 6f6f 6579 2864 6563 696d 616c 5f74 6f5f  ooey(decimal_to_
+00000cf0: 696e 7428 2231 2e32 2229 2920 3d3d 2064  int("1.2")) == d
+00000d00: 6563 696d 616c 5f74 6f5f 696e 7428 2232  ecimal_to_int("2
+00000d10: 3037 3336 2e30 2229 0a20 2020 2061 7373  0736.0").    ass
+00000d20: 6572 7420 632e 7068 6f6f 6579 2864 6563  ert c.phooey(dec
+00000d30: 696d 616c 5f74 6f5f 696e 7428 222d 312e  imal_to_int("-1.
+00000d40: 3222 2929 203d 3d20 6465 6369 6d61 6c5f  2")) == decimal_
+00000d50: 746f 5f69 6e74 2822 3230 3733 362e 3022  to_int("20736.0"
+00000d60: 290a 2020 2020 6173 7365 7274 2063 2e61  ).    assert c.a
+00000d70: 7267 2864 6563 696d 616c 5f74 6f5f 696e  rg(decimal_to_in
+00000d80: 7428 222d 332e 3722 2929 203d 3d20 6465  t("-3.7")) == de
+00000d90: 6369 6d61 6c5f 746f 5f69 6e74 2822 2d33  cimal_to_int("-3
+00000da0: 2e37 2229 0a20 2020 2061 7373 6572 7420  .7").    assert 
+00000db0: 632e 6172 6728 6465 6369 6d61 6c5f 746f  c.arg(decimal_to
+00000dc0: 5f69 6e74 2822 332e 3722 2929 203d 3d20  _int("3.7")) == 
+00000dd0: 6465 6369 6d61 6c5f 746f 5f69 6e74 2822  decimal_to_int("
+00000de0: 332e 3722 290a 2020 2020 6173 7365 7274  3.7").    assert
+00000df0: 2063 2e67 6172 6728 2920 3d3d 2064 6563   c.garg() == dec
+00000e00: 696d 616c 5f74 6f5f 696e 7428 2236 2e37  imal_to_int("6.7
+00000e10: 3522 290a 2020 2020 6173 7365 7274 2063  5").    assert c
+00000e20: 2e68 6172 6728 2920 3d3d 2064 6563 696d  .harg() == decim
+00000e30: 616c 5f74 6f5f 696e 7428 2239 2e30 2229  al_to_int("9.0")
+00000e40: 0a20 2020 2061 7373 6572 7420 632e 6961  .    assert c.ia
+00000e50: 7267 2829 203d 3d20 3134 0a0a 2020 2020  rg() == 14..    
+00000e60: 7072 696e 7428 2250 6173 7365 6420 6672  print("Passed fr
+00000e70: 6163 7469 6f6e 616c 206d 756c 7469 706c  actional multipl
+00000e80: 6963 6174 696f 6e20 7465 7374 2229 0a0a  ication test")..
+00000e90: 0a64 6566 2074 6573 745f 6d75 6c5f 6f76  .def test_mul_ov
+00000ea0: 6572 666c 6f77 2874 785f 6661 696c 6564  erflow(tx_failed
+00000eb0: 2c20 6765 745f 636f 6e74 7261 6374 5f77  , get_contract_w
+00000ec0: 6974 685f 6761 735f 6573 7469 6d61 7469  ith_gas_estimati
+00000ed0: 6f6e 293a 0a20 2020 206d 756c 5f63 6f64  on):.    mul_cod
+00000ee0: 6520 3d20 2222 220a 0a40 6578 7465 726e  e = """..@extern
+00000ef0: 616c 0a64 6566 205f 6e75 6d5f 6d75 6c28  al.def _num_mul(
+00000f00: 783a 2064 6563 696d 616c 2c20 793a 2064  x: decimal, y: d
+00000f10: 6563 696d 616c 2920 2d3e 2064 6563 696d  ecimal) -> decim
+00000f20: 616c 3a0a 2020 2020 7265 7475 726e 2078  al:.    return x
+00000f30: 202a 2079 0a0a 2020 2020 2222 220a 0a20   * y..    """.. 
+00000f40: 2020 2063 203d 2067 6574 5f63 6f6e 7472     c = get_contr
+00000f50: 6163 745f 7769 7468 5f67 6173 5f65 7374  act_with_gas_est
+00000f60: 696d 6174 696f 6e28 6d75 6c5f 636f 6465  imation(mul_code
+00000f70: 290a 0a20 2020 2078 203d 2064 6563 696d  )..    x = decim
+00000f80: 616c 5f74 6f5f 696e 7428 2238 3530 3730  al_to_int("85070
+00000f90: 3539 3137 3330 3233 3436 3135 3836 3538  5917302346158658
+00000fa0: 3433 3635 3138 3537 3934 3230 3532 3836  4365185794205286
+00000fb0: 3422 290a 2020 2020 7920 3d20 6465 6369  4").    y = deci
+00000fc0: 6d61 6c5f 746f 5f69 6e74 2822 3133 3631  mal_to_int("1361
+00000fd0: 3132 3934 3637 3638 3337 3533 3835 3338  1294676837538538
+00000fe0: 3533 3439 3834 3239 3733 2229 0a0a 2020  5349842973")..  
+00000ff0: 2020 7769 7468 2074 785f 6661 696c 6564    with tx_failed
+00001000: 2829 3a0a 2020 2020 2020 2020 632e 5f6e  ():.        c._n
+00001010: 756d 5f6d 756c 2878 2c20 7929 0a0a 2020  um_mul(x, y)..  
+00001020: 2020 7820 3d20 5369 7a65 4c69 6d69 7473    x = SizeLimits
+00001030: 2e4d 4158 5f41 5354 5f44 4543 494d 414c  .MAX_AST_DECIMAL
+00001040: 0a20 2020 2079 203d 2031 202b 2044 4543  .    y = 1 + DEC
+00001050: 494d 414c 5f45 5053 494c 4f4e 0a0a 2020  IMAL_EPSILON..  
+00001060: 2020 7769 7468 2074 785f 6661 696c 6564    with tx_failed
+00001070: 2829 3a0a 2020 2020 2020 2020 632e 5f6e  ():.        c._n
+00001080: 756d 5f6d 756c 2864 6563 696d 616c 5f74  um_mul(decimal_t
+00001090: 6f5f 696e 7428 7829 2c20 6465 6369 6d61  o_int(x), decima
+000010a0: 6c5f 746f 5f69 6e74 2879 2929 0a0a 2020  l_to_int(y))..  
+000010b0: 2020 6173 7365 7274 2063 2e5f 6e75 6d5f    assert c._num_
+000010c0: 6d75 6c28 6465 6369 6d61 6c5f 746f 5f69  mul(decimal_to_i
+000010d0: 6e74 2878 292c 2064 6563 696d 616c 5f74  nt(x), decimal_t
+000010e0: 6f5f 696e 7428 3129 2920 3d3d 2064 6563  o_int(1)) == dec
+000010f0: 696d 616c 5f74 6f5f 696e 7428 7829 0a0a  imal_to_int(x)..
+00001100: 2020 2020 6173 7365 7274 2063 2e5f 6e75      assert c._nu
+00001110: 6d5f 6d75 6c28 6465 6369 6d61 6c5f 746f  m_mul(decimal_to
+00001120: 5f69 6e74 2878 292c 2064 6563 696d 616c  _int(x), decimal
+00001130: 5f74 6f5f 696e 7428 3120 2d20 4445 4349  _to_int(1 - DECI
+00001140: 4d41 4c5f 4550 5349 4c4f 4e29 2920 3d3d  MAL_EPSILON)) ==
+00001150: 2064 6563 696d 616c 5f74 6f5f 696e 7428   decimal_to_int(
+00001160: 0a20 2020 2020 2020 2071 7561 6e74 697a  .        quantiz
+00001170: 6528 7820 2a20 2831 202d 2044 4543 494d  e(x * (1 - DECIM
+00001180: 414c 5f45 5053 494c 4f4e 2929 0a20 2020  AL_EPSILON)).   
+00001190: 2029 0a0a 2020 2020 7820 3d20 5369 7a65   )..    x = Size
+000011a0: 4c69 6d69 7473 2e4d 494e 5f41 5354 5f44  Limits.MIN_AST_D
+000011b0: 4543 494d 414c 0a20 2020 2061 7373 6572  ECIMAL.    asser
+000011c0: 7420 632e 5f6e 756d 5f6d 756c 2864 6563  t c._num_mul(dec
+000011d0: 696d 616c 5f74 6f5f 696e 7428 7829 2c20  imal_to_int(x), 
+000011e0: 6465 6369 6d61 6c5f 746f 5f69 6e74 2831  decimal_to_int(1
+000011f0: 202d 2044 4543 494d 414c 5f45 5053 494c   - DECIMAL_EPSIL
+00001200: 4f4e 2929 203d 3d20 6465 6369 6d61 6c5f  ON)) == decimal_
+00001210: 746f 5f69 6e74 280a 2020 2020 2020 2020  to_int(.        
+00001220: 7175 616e 7469 7a65 2878 202a 2028 3120  quantize(x * (1 
+00001230: 2d20 4445 4349 4d41 4c5f 4550 5349 4c4f  - DECIMAL_EPSILO
+00001240: 4e29 290a 2020 2020 290a 0a0a 2320 6469  N)).    )...# di
+00001250: 7669 7369 6f6e 2066 6169 6c75 7265 206d  vision failure m
+00001260: 6f64 6573 2821 290a 6465 6620 7465 7374  odes(!).def test
+00001270: 5f64 6976 5f6f 7665 7266 6c6f 7728 6765  _div_overflow(ge
+00001280: 745f 636f 6e74 7261 6374 2c20 7478 5f66  t_contract, tx_f
+00001290: 6169 6c65 6429 3a0a 2020 2020 636f 6465  ailed):.    code
+000012a0: 203d 2022 2222 0a40 6578 7465 726e 616c   = """.@external
+000012b0: 0a64 6566 2066 6f6f 2878 3a20 6465 6369  .def foo(x: deci
+000012c0: 6d61 6c2c 2079 3a20 6465 6369 6d61 6c29  mal, y: decimal)
+000012d0: 202d 3e20 6465 6369 6d61 6c3a 0a20 2020   -> decimal:.   
+000012e0: 2072 6574 7572 6e20 7820 2f20 790a 2020   return x / y.  
+000012f0: 2020 2222 220a 0a20 2020 2063 203d 2067    """..    c = g
+00001300: 6574 5f63 6f6e 7472 6163 7428 636f 6465  et_contract(code
+00001310: 290a 0a20 2020 2078 203d 2053 697a 654c  )..    x = SizeL
+00001320: 696d 6974 732e 4d49 4e5f 4153 545f 4445  imits.MIN_AST_DE
+00001330: 4349 4d41 4c0a 2020 2020 7920 3d20 2d44  CIMAL.    y = -D
+00001340: 4543 494d 414c 5f45 5053 494c 4f4e 0a0a  ECIMAL_EPSILON..
+00001350: 2020 2020 7769 7468 2074 785f 6661 696c      with tx_fail
+00001360: 6564 2829 3a0a 2020 2020 2020 2020 632e  ed():.        c.
+00001370: 666f 6f28 6465 6369 6d61 6c5f 746f 5f69  foo(decimal_to_i
+00001380: 6e74 2878 292c 2064 6563 696d 616c 5f74  nt(x), decimal_t
+00001390: 6f5f 696e 7428 7929 290a 2020 2020 7769  o_int(y)).    wi
+000013a0: 7468 2074 785f 6661 696c 6564 2829 3a0a  th tx_failed():.
+000013b0: 2020 2020 2020 2020 632e 666f 6f28 6465          c.foo(de
+000013c0: 6369 6d61 6c5f 746f 5f69 6e74 2878 292c  cimal_to_int(x),
+000013d0: 2030 290a 2020 2020 7769 7468 2074 785f   0).    with tx_
+000013e0: 6661 696c 6564 2829 3a0a 2020 2020 2020  failed():.      
+000013f0: 2020 632e 666f 6f28 6465 6369 6d61 6c5f    c.foo(decimal_
+00001400: 746f 5f69 6e74 2879 292c 2030 290a 0a20  to_int(y), 0).. 
+00001410: 2020 2079 203d 2031 202d 2044 4543 494d     y = 1 - DECIM
+00001420: 414c 5f45 5053 494c 4f4e 2020 2320 302e  AL_EPSILON  # 0.
+00001430: 3939 3939 3939 3939 390a 2020 2020 7769  999999999.    wi
+00001440: 7468 2074 785f 6661 696c 6564 2829 3a0a  th tx_failed():.
+00001450: 2020 2020 2020 2020 632e 666f 6f28 6465          c.foo(de
+00001460: 6369 6d61 6c5f 746f 5f69 6e74 2878 292c  cimal_to_int(x),
+00001470: 2064 6563 696d 616c 5f74 6f5f 696e 7428   decimal_to_int(
+00001480: 7929 290a 0a20 2020 2079 203d 202d 310a  y))..    y = -1.
+00001490: 2020 2020 7769 7468 2074 785f 6661 696c      with tx_fail
+000014a0: 6564 2829 3a0a 2020 2020 2020 2020 632e  ed():.        c.
+000014b0: 666f 6f28 6465 6369 6d61 6c5f 746f 5f69  foo(decimal_to_i
+000014c0: 6e74 2878 292c 2064 6563 696d 616c 5f74  nt(x), decimal_t
+000014d0: 6f5f 696e 7428 7929 290a 0a20 2020 2061  o_int(y))..    a
+000014e0: 7373 6572 7420 632e 666f 6f28 6465 6369  ssert c.foo(deci
+000014f0: 6d61 6c5f 746f 5f69 6e74 2878 292c 2064  mal_to_int(x), d
+00001500: 6563 696d 616c 5f74 6f5f 696e 7428 3129  ecimal_to_int(1)
+00001510: 2920 3d3d 2064 6563 696d 616c 5f74 6f5f  ) == decimal_to_
+00001520: 696e 7428 7829 0a20 2020 2061 7373 6572  int(x).    asser
+00001530: 7420 632e 666f 6f28 6465 6369 6d61 6c5f  t c.foo(decimal_
+00001540: 746f 5f69 6e74 2878 292c 2064 6563 696d  to_int(x), decim
+00001550: 616c 5f74 6f5f 696e 7428 3120 2b20 4445  al_to_int(1 + DE
+00001560: 4349 4d41 4c5f 4550 5349 4c4f 4e29 2920  CIMAL_EPSILON)) 
+00001570: 3d3d 2064 6563 696d 616c 5f74 6f5f 696e  == decimal_to_in
+00001580: 7428 0a20 2020 2020 2020 2071 7561 6e74  t(.        quant
+00001590: 697a 6528 7820 2f20 2831 202b 2044 4543  ize(x / (1 + DEC
+000015a0: 494d 414c 5f45 5053 494c 4f4e 2929 0a20  IMAL_EPSILON)). 
+000015b0: 2020 2029 0a0a 2020 2020 7820 3d20 5369     )..    x = Si
+000015c0: 7a65 4c69 6d69 7473 2e4d 4158 5f41 5354  zeLimits.MAX_AST
+000015d0: 5f44 4543 494d 414c 0a0a 2020 2020 7769  _DECIMAL..    wi
+000015e0: 7468 2074 785f 6661 696c 6564 2829 3a0a  th tx_failed():.
+000015f0: 2020 2020 2020 2020 632e 666f 6f28 6465          c.foo(de
+00001600: 6369 6d61 6c5f 746f 5f69 6e74 2878 292c  cimal_to_int(x),
+00001610: 2064 6563 696d 616c 5f74 6f5f 696e 7428   decimal_to_int(
+00001620: 4445 4349 4d41 4c5f 4550 5349 4c4f 4e29  DECIMAL_EPSILON)
+00001630: 290a 0a20 2020 2079 203d 2031 202d 2044  )..    y = 1 - D
+00001640: 4543 494d 414c 5f45 5053 494c 4f4e 0a20  ECIMAL_EPSILON. 
+00001650: 2020 2077 6974 6820 7478 5f66 6169 6c65     with tx_faile
+00001660: 6428 293a 0a20 2020 2020 2020 2063 2e66  d():.        c.f
+00001670: 6f6f 2864 6563 696d 616c 5f74 6f5f 696e  oo(decimal_to_in
+00001680: 7428 7829 2c20 6465 6369 6d61 6c5f 746f  t(x), decimal_to
+00001690: 5f69 6e74 2879 2929 0a0a 2020 2020 6173  _int(y))..    as
+000016a0: 7365 7274 2063 2e66 6f6f 2864 6563 696d  sert c.foo(decim
+000016b0: 616c 5f74 6f5f 696e 7428 7829 2c20 6465  al_to_int(x), de
+000016c0: 6369 6d61 6c5f 746f 5f69 6e74 2831 2929  cimal_to_int(1))
+000016d0: 203d 3d20 6465 6369 6d61 6c5f 746f 5f69   == decimal_to_i
+000016e0: 6e74 2878 290a 0a20 2020 2061 7373 6572  nt(x)..    asser
+000016f0: 7420 632e 666f 6f28 6465 6369 6d61 6c5f  t c.foo(decimal_
+00001700: 746f 5f69 6e74 2878 292c 2064 6563 696d  to_int(x), decim
+00001710: 616c 5f74 6f5f 696e 7428 3120 2b20 4445  al_to_int(1 + DE
+00001720: 4349 4d41 4c5f 4550 5349 4c4f 4e29 2920  CIMAL_EPSILON)) 
+00001730: 3d3d 2064 6563 696d 616c 5f74 6f5f 696e  == decimal_to_in
+00001740: 7428 0a20 2020 2020 2020 2071 7561 6e74  t(.        quant
+00001750: 697a 6528 7820 2f20 2831 202b 2044 4543  ize(x / (1 + DEC
+00001760: 494d 414c 5f45 5053 494c 4f4e 2929 0a20  IMAL_EPSILON)). 
+00001770: 2020 2029 0a0a 0a64 6566 2074 6573 745f     )...def test_
+00001780: 6465 6369 6d61 6c5f 6d69 6e5f 6d61 785f  decimal_min_max_
+00001790: 6c69 7465 7261 6c73 2874 785f 6661 696c  literals(tx_fail
+000017a0: 6564 2c20 6765 745f 636f 6e74 7261 6374  ed, get_contract
+000017b0: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
+000017c0: 7469 6f6e 293a 0a20 2020 2063 6f64 6520  tion):.    code 
+000017d0: 3d20 2222 220a 4065 7874 6572 6e61 6c0a  = """.@external.
+000017e0: 6465 6620 6d61 7869 6d75 6d28 293a 0a20  def maximum():. 
+000017f0: 2020 2061 3a20 6465 6369 6d61 6c20 3d20     a: decimal = 
+00001800: 3138 3730 3732 3230 3935 3738 3335 3535  1870722095783555
+00001810: 3733 3533 3030 3731 3635 3835 3837 3638  7353007165858768
+00001820: 3432 3236 3531 3539 352e 3933 3635 3530  422651595.936550
+00001830: 3039 3237 0a40 6578 7465 726e 616c 0a64  0927.@external.d
+00001840: 6566 206d 696e 696d 756d 2829 3a0a 2020  ef minimum():.  
+00001850: 2020 613a 2064 6563 696d 616c 203d 202d    a: decimal = -
+00001860: 3138 3730 3732 3230 3935 3738 3335 3535  1870722095783555
+00001870: 3733 3533 3030 3731 3635 3835 3837 3638  7353007165858768
+00001880: 3432 3236 3531 3539 352e 3933 3635 3530  422651595.936550
+00001890: 3039 3238 0a20 2020 2022 2222 0a20 2020  0928.    """.   
+000018a0: 2063 203d 2067 6574 5f63 6f6e 7472 6163   c = get_contrac
+000018b0: 745f 7769 7468 5f67 6173 5f65 7374 696d  t_with_gas_estim
+000018c0: 6174 696f 6e28 636f 6465 290a 0a20 2020  ation(code)..   
+000018d0: 2061 7373 6572 7420 632e 6d61 7869 6d75   assert c.maximu
+000018e0: 6d28 2920 3d3d 205b 5d0a 2020 2020 6173  m() == [].    as
+000018f0: 7365 7274 2063 2e6d 696e 696d 756d 2829  sert c.minimum()
+00001900: 203d 3d20 5b5d 0a0a 0a64 6566 2074 6573   == []...def tes
+00001910: 745f 7363 6965 6e74 6966 6963 5f6e 6f74  t_scientific_not
+00001920: 6174 696f 6e28 6765 745f 636f 6e74 7261  ation(get_contra
+00001930: 6374 5f77 6974 685f 6761 735f 6573 7469  ct_with_gas_esti
+00001940: 6d61 7469 6f6e 293a 0a20 2020 2063 6f64  mation):.    cod
+00001950: 6520 3d20 2222 220a 4065 7874 6572 6e61  e = """.@externa
+00001960: 6c0a 6465 6620 666f 6f28 2920 2d3e 2064  l.def foo() -> d
+00001970: 6563 696d 616c 3a0a 2020 2020 7265 7475  ecimal:.    retu
+00001980: 726e 2031 652d 3130 0a0a 4065 7874 6572  rn 1e-10..@exter
+00001990: 6e61 6c0a 6465 6620 6261 7228 6e75 6d3a  nal.def bar(num:
+000019a0: 2064 6563 696d 616c 2920 2d3e 2064 6563   decimal) -> dec
+000019b0: 696d 616c 3a0a 2020 2020 7265 7475 726e  imal:.    return
+000019c0: 206e 756d 202b 202d 3165 3338 0a20 2020   num + -1e38.   
+000019d0: 2022 2222 0a20 2020 2063 203d 2067 6574   """.    c = get
+000019e0: 5f63 6f6e 7472 6163 745f 7769 7468 5f67  _contract_with_g
+000019f0: 6173 5f65 7374 696d 6174 696f 6e28 636f  as_estimation(co
+00001a00: 6465 290a 0a20 2020 2061 7373 6572 7420  de)..    assert 
+00001a10: 632e 666f 6f28 2920 3d3d 2064 6563 696d  c.foo() == decim
+00001a20: 616c 5f74 6f5f 696e 7428 2231 652d 3130  al_to_int("1e-10
+00001a30: 2229 2020 2320 536d 616c 6c65 7374 2070  ")  # Smallest p
+00001a40: 6f73 7369 626c 6520 6465 6369 6d61 6c0a  ossible decimal.
+00001a50: 2020 2020 6173 7365 7274 2063 2e62 6172      assert c.bar
+00001a60: 2864 6563 696d 616c 5f74 6f5f 696e 7428  (decimal_to_int(
+00001a70: 2231 6533 3722 2929 203d 3d20 6465 6369  "1e37")) == deci
+00001a80: 6d61 6c5f 746f 5f69 6e74 2822 2d39 6533  mal_to_int("-9e3
+00001a90: 3722 2920 2023 204d 6174 6820 6c69 6e65  7")  # Math line
+00001aa0: 7320 7570 0a0a 0a64 6566 2074 6573 745f  s up...def test_
+00001ab0: 6578 706f 6e65 6e74 7328 293a 0a20 2020  exponents():.   
+00001ac0: 2063 6f64 6520 3d20 2222 220a 4065 7874   code = """.@ext
+00001ad0: 6572 6e61 6c0a 6465 6620 666f 6f28 2920  ernal.def foo() 
+00001ae0: 2d3e 2064 6563 696d 616c 3a0a 2020 2020  -> decimal:.    
+00001af0: 7265 7475 726e 2032 2e32 202a 2a20 322e  return 2.2 ** 2.
+00001b00: 300a 2020 2020 2222 220a 0a20 2020 2077  0.    """..    w
+00001b10: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+00001b20: 7328 5479 7065 4d69 736d 6174 6368 293a  s(TypeMismatch):
+00001b30: 0a20 2020 2020 2020 2063 6f6d 7069 6c65  .        compile
+00001b40: 5f63 6f64 6528 636f 6465 290a 0a0a 6465  _code(code)...de
+00001b50: 6620 7465 7374 5f64 6563 696d 616c 5f6e  f test_decimal_n
+00001b60: 6573 7465 645f 696e 7465 726d 6564 6961  ested_intermedia
+00001b70: 7465 5f6f 7665 7266 6c6f 7728 293a 0a20  te_overflow():. 
+00001b80: 2020 2063 6f64 6520 3d20 2222 220a 4065     code = """.@e
+00001b90: 7874 6572 6e61 6c0a 6465 6620 666f 6f28  xternal.def foo(
+00001ba0: 293a 0a20 2020 2061 3a20 6465 6369 6d61  ):.    a: decima
+00001bb0: 6c20 3d20 3138 3730 3732 3230 3935 3738  l = 187072209578
+00001bc0: 3335 3535 3733 3533 3030 3731 3635 3835  3555735300716585
+00001bd0: 3837 3638 3432 3236 3531 3539 352e 3933  8768422651595.93
+00001be0: 3635 3530 3039 3237 202b 2031 652d 3130  65500927 + 1e-10
+00001bf0: 202d 2031 652d 3130 0a20 2020 2022 2222   - 1e-10.    """
+00001c00: 0a20 2020 2077 6974 6820 7079 7465 7374  .    with pytest
+00001c10: 2e72 6169 7365 7328 4f76 6572 666c 6f77  .raises(Overflow
+00001c20: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+00001c30: 2020 2020 636f 6d70 696c 655f 636f 6465      compile_code
+00001c40: 2863 6f64 6529 0a0a 0a64 6566 2074 6573  (code)...def tes
+00001c50: 745f 7265 706c 6163 655f 6465 6369 6d61  t_replace_decima
+00001c60: 6c5f 6e65 7374 6564 5f69 6e74 6572 6d65  l_nested_interme
+00001c70: 6469 6174 655f 756e 6465 7266 6c6f 7728  diate_underflow(
+00001c80: 6475 6d6d 795f 696e 7075 745f 6275 6e64  dummy_input_bund
+00001c90: 6c65 293a 0a20 2020 2063 6f64 6520 3d20  le):.    code = 
+00001ca0: 2222 220a 4065 7874 6572 6e61 6c0a 6465  """.@external.de
+00001cb0: 6620 666f 6f28 293a 0a20 2020 2061 3a20  f foo():.    a: 
+00001cc0: 6465 6369 6d61 6c20 3d20 2d31 3837 3037  decimal = -18707
+00001cd0: 3232 3039 3537 3833 3535 3537 3335 3330  2209578355573530
+00001ce0: 3037 3136 3538 3538 3736 3834 3232 3635  0716585876842265
+00001cf0: 3135 3935 2e39 3336 3535 3030 3932 3820  1595.9365500928 
+00001d00: 2d20 3165 2d31 3020 2b20 3165 2d31 300a  - 1e-10 + 1e-10.
+00001d10: 2020 2020 2222 220a 2020 2020 7769 7468      """.    with
+00001d20: 2070 7974 6573 742e 7261 6973 6573 284f   pytest.raises(O
+00001d30: 7665 7266 6c6f 7745 7863 6570 7469 6f6e  verflowException
+00001d40: 293a 0a20 2020 2020 2020 2063 6f6d 7069  ):.        compi
+00001d50: 6c65 5f63 6f64 6528 636f 6465 290a 0a0a  le_code(code)...
+00001d60: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
+00001d70: 5f66 6c6f 6f72 6469 7628 293a 0a20 2020  _floordiv():.   
+00001d80: 2063 6f64 6520 3d20 2222 220a 4065 7874   code = """.@ext
+00001d90: 6572 6e61 6c0a 6465 6620 666f 6f28 293a  ernal.def foo():
+00001da0: 0a20 2020 2061 3a20 6465 6369 6d61 6c20  .    a: decimal 
+00001db0: 3d20 352e 3020 2f2f 2039 2e30 0a20 2020  = 5.0 // 9.0.   
+00001dc0: 2022 2222 0a20 2020 2077 6974 6820 7079   """.    with py
+00001dd0: 7465 7374 2e72 6169 7365 7328 496e 7661  test.raises(Inva
+00001de0: 6c69 644f 7065 7261 7469 6f6e 2920 6173  lidOperation) as
+00001df0: 2065 3a0a 2020 2020 2020 2020 636f 6d70   e:.        comp
+00001e00: 696c 655f 636f 6465 2863 6f64 6529 0a0a  ile_code(code)..
+00001e10: 2020 2020 6173 7365 7274 2065 2e76 616c      assert e.val
+00001e20: 7565 2e5f 6869 6e74 203d 3d20 2264 6964  ue._hint == "did
+00001e30: 2079 6f75 206d 6561 6e20 6035 2e30 202f   you mean `5.0 /
+00001e40: 2039 2e30 603f 220a 0a0a 6465 6620 7465   9.0`?"...def te
+00001e50: 7374 5f64 6563 696d 616c 735f 626c 6f63  st_decimals_bloc
+00001e60: 6b65 6428 293a 0a20 2020 2063 6f64 6520  ked():.    code 
+00001e70: 3d20 2222 220a 4065 7874 6572 6e61 6c0a  = """.@external.
+00001e80: 6465 6620 666f 6f28 783a 2064 6563 696d  def foo(x: decim
+00001e90: 616c 293a 0a20 2020 2070 6173 730a 2020  al):.    pass.  
+00001ea0: 2020 2222 220a 2020 2020 2320 656e 6162    """.    # enab
+00001eb0: 6c65 5f64 6563 696d 616c 7320 6465 6661  le_decimals defa
+00001ec0: 756c 7420 746f 2046 616c 7365 206e 6f72  ult to False nor
+00001ed0: 6d61 6c6c 792c 2062 7574 2064 6566 6175  mally, but defau
+00001ee0: 6c74 7320 746f 2054 7275 6520 696e 2074  lts to True in t
+00001ef0: 6865 0a20 2020 2023 2074 6573 7420 7375  he.    # test su
+00001f00: 6974 652e 2074 6869 7320 7465 7374 206d  ite. this test m
+00001f10: 616e 7561 6c6c 7920 6f76 6572 7269 6465  anually override
+00001f20: 7320 7468 6520 6465 6661 756c 7420 7661  s the default va
+00001f30: 6c75 6520 746f 2074 6573 7420 7468 650a  lue to test the.
+00001f40: 2020 2020 2320 226e 6f72 6d61 6c22 2062      # "normal" b
+00001f50: 6568 6176 696f 7220 6f66 2065 6e61 626c  ehavior of enabl
+00001f60: 655f 6465 6369 6d61 6c73 206f 7574 7369  e_decimals outsi
+00001f70: 6465 206f 6620 7468 6520 7465 7374 2073  de of the test s
+00001f80: 7569 7465 2e0a 2020 2020 7472 793a 0a20  uite..    try:. 
+00001f90: 2020 2020 2020 2061 7373 6572 7420 636f         assert co
+00001fa0: 6d70 696c 6572 5f73 6574 7469 6e67 732e  mpiler_settings.
+00001fb0: 4445 4641 554c 545f 454e 4142 4c45 5f44  DEFAULT_ENABLE_D
+00001fc0: 4543 494d 414c 5320 6973 2054 7275 650a  ECIMALS is True.
+00001fd0: 2020 2020 2020 2020 636f 6d70 696c 6572          compiler
+00001fe0: 5f73 6574 7469 6e67 732e 4445 4641 554c  _settings.DEFAUL
+00001ff0: 545f 454e 4142 4c45 5f44 4543 494d 414c  T_ENABLE_DECIMAL
+00002000: 5320 3d20 4661 6c73 650a 2020 2020 2020  S = False.      
+00002010: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+00002020: 6973 6573 2846 6561 7475 7265 4578 6365  ises(FeatureExce
+00002030: 7074 696f 6e29 2061 7320 653a 0a20 2020  ption) as e:.   
+00002040: 2020 2020 2020 2020 2063 6f6d 7069 6c65           compile
+00002050: 5f63 6f64 6528 636f 6465 290a 2020 2020  _code(code).    
+00002060: 2020 2020 6173 7365 7274 2065 2e76 616c      assert e.val
+00002070: 7565 2e5f 6d65 7373 6167 6520 3d3d 2022  ue._message == "
+00002080: 6465 6369 6d61 6c73 2061 7265 206e 6f74  decimals are not
+00002090: 2061 6c6c 6f77 6564 2075 6e6c 6573 7320   allowed unless 
+000020a0: 602d 2d65 6e61 626c 652d 6465 6369 6d61  `--enable-decima
+000020b0: 6c73 6020 6973 2073 6574 220a 2020 2020  ls` is set".    
+000020c0: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
+000020d0: 2063 6f6d 7069 6c65 725f 7365 7474 696e   compiler_settin
+000020e0: 6773 2e44 4546 4155 4c54 5f45 4e41 424c  gs.DEFAULT_ENABL
+000020f0: 455f 4445 4349 4d41 4c53 203d 2054 7275  E_DECIMALS = Tru
+00002100: 650a                                     e.
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_division.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_exponents.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_exponents.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_isqrt.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_isqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_modulo.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_modulo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from decimal import Decimal
-
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import ZeroDivisionException
 
 
 def test_modulo(get_contract_with_gas_estimation):
     code = """
 @external
 def num_modulo_num() -> int128:
@@ -22,28 +21,28 @@
 
 @external
 def num_modulo_decimal() -> decimal:
     return 1.5 % 1.0
 """
     c = get_contract_with_gas_estimation(code)
     assert c.num_modulo_num() == 1
-    assert c.decimal_modulo_decimal() == Decimal(".18")
-    assert c.decimal_modulo_num() == Decimal(".5")
-    assert c.num_modulo_decimal() == Decimal(".5")
+    assert c.decimal_modulo_decimal() == decimal_to_int(".18")
+    assert c.decimal_modulo_num() == decimal_to_int(".5")
+    assert c.num_modulo_decimal() == decimal_to_int(".5")
 
 
 def test_modulo_with_input_of_zero(tx_failed, get_contract_with_gas_estimation):
     code = """
 @external
 def foo(a: decimal, b: decimal) -> decimal:
     return a % b
 """
     c = get_contract_with_gas_estimation(code)
     with tx_failed():
-        c.foo(Decimal("1"), Decimal("0"))
+        c.foo(decimal_to_int("1"), decimal_to_int("0"))
 
 
 def test_literals_vs_evm(get_contract):
     code = """
 @external
 @view
 def foo() -> (int128, int128, int128, int128):
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_signed_ints.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_signed_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_sqrt.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_sqrt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from decimal import ROUND_FLOOR, Decimal
 
 import hypothesis
 import pytest
 from eth_tester.exceptions import TransactionFailed
 
+from tests.utils import decimal_to_int
 from vyper.utils import SizeLimits
 
 DECIMAL_PLACES = 10
 DECIMAL_RANGE = [Decimal("0." + "0" * d + "2") for d in range(0, DECIMAL_PLACES)]
 
 
 def decimal_truncate(val, decimal_places=DECIMAL_PLACES, rounding=ROUND_FLOOR):
@@ -15,27 +16,28 @@
     if decimal_places != 0:
         q += "." + "0" * decimal_places
 
     return val.quantize(Decimal(q), rounding=rounding)
 
 
 def decimal_sqrt(val):
-    return decimal_truncate(val.sqrt())
+    return decimal_to_int(decimal_truncate(val.sqrt()))
 
 
 def test_sqrt_literal(get_contract_with_gas_estimation):
     code = """
 @external
 def test() -> decimal:
     return sqrt(2.0)
     """
     c = get_contract_with_gas_estimation(code)
     assert c.test() == decimal_sqrt(Decimal("2"))
 
 
+# TODO: use parametrization here
 def test_sqrt_variable(get_contract_with_gas_estimation):
     code = """
 @external
 def test(a: decimal) -> decimal:
     return sqrt(a)
 
 @external
@@ -43,20 +45,20 @@
     a: decimal = 44.001
     return sqrt(a)
     """
 
     c = get_contract_with_gas_estimation(code)
 
     val = Decimal("33.33")
-    assert c.test(val) == decimal_sqrt(val)
+    assert c.test(decimal_to_int(val)) == decimal_sqrt(val)
 
     val = Decimal("0.1")
-    assert c.test(val) == decimal_sqrt(val)
+    assert c.test(decimal_to_int(val)) == decimal_sqrt(val)
 
-    assert c.test(Decimal("0.0")) == Decimal("0.0")
+    assert c.test(decimal_to_int("0.0")) == decimal_to_int("0.0")
     assert c.test2() == decimal_sqrt(Decimal("44.001"))
 
 
 def test_sqrt_storage(get_contract_with_gas_estimation):
     code = """
 s_var: decimal
 
@@ -69,17 +71,17 @@
 def test2() -> decimal:
     self.s_var = 444.44
     return sqrt(self.s_var)
     """
 
     c = get_contract_with_gas_estimation(code)
     val = Decimal("12.21")
-    assert c.test(val) == decimal_sqrt(val + 1)
+    assert c.test(decimal_to_int(val)) == decimal_sqrt(val + 1)
     val = Decimal("100.01")
-    assert c.test(val) == decimal_sqrt(val + 1)
+    assert c.test(decimal_to_int(val)) == decimal_sqrt(val + 1)
     assert c.test2() == decimal_sqrt(Decimal("444.44"))
 
 
 def test_sqrt_inline_memory_correct(get_contract_with_gas_estimation):
     code = """
 @external
 def test(a: decimal) -> (decimal, decimal, decimal, decimal, decimal, String[100]):
@@ -90,19 +92,19 @@
     f: String[100] = 'hello world'
     return a, x, y, z, e, f
     """
 
     c = get_contract_with_gas_estimation(code)
 
     val = Decimal("2.1")
-    assert c.test(val) == [
-        val,
-        Decimal("1"),
-        Decimal("2"),
-        Decimal("3"),
+    assert c.test(decimal_to_int(val)) == [
+        decimal_to_int(val),
+        decimal_to_int("1"),
+        decimal_to_int("2"),
+        decimal_to_int("3"),
         decimal_sqrt(val),
         "hello world",
     ]
 
 
 @pytest.mark.parametrize("value", DECIMAL_RANGE)
 def test_sqrt_sub_decimal_places(value, get_contract):
@@ -110,15 +112,15 @@
 @external
 def test(a: decimal) -> decimal:
     return sqrt(a)
     """
 
     c = get_contract(code)
 
-    vyper_sqrt = c.test(value)
+    vyper_sqrt = c.test(decimal_to_int(value))
     actual_sqrt = decimal_sqrt(value)
     assert vyper_sqrt == actual_sqrt
 
 
 @pytest.fixture(scope="module")
 def sqrt_contract(get_contract_module):
     code = """
@@ -128,37 +130,37 @@
     """
     c = get_contract_module(code)
     return c
 
 
 @pytest.mark.parametrize("value", [Decimal(0), Decimal(SizeLimits.MAX_INT128)])
 def test_sqrt_bounds(sqrt_contract, value):
-    vyper_sqrt = sqrt_contract.test(value)
+    vyper_sqrt = sqrt_contract.test(decimal_to_int(value))
     actual_sqrt = decimal_sqrt(value)
     assert vyper_sqrt == actual_sqrt
 
 
 @pytest.mark.fuzzing
 @hypothesis.given(
     value=hypothesis.strategies.decimals(
         min_value=Decimal(0), max_value=Decimal(SizeLimits.MAX_INT128), places=DECIMAL_PLACES
     )
 )
 @hypothesis.example(value=Decimal(SizeLimits.MAX_INT128))
 @hypothesis.example(value=Decimal(0))
 def test_sqrt_valid_range(sqrt_contract, value):
-    vyper_sqrt = sqrt_contract.test(value)
+    vyper_sqrt = sqrt_contract.test(decimal_to_int(value))
     actual_sqrt = decimal_sqrt(value)
     assert vyper_sqrt == actual_sqrt
 
 
 @pytest.mark.fuzzing
 @hypothesis.given(
     value=hypothesis.strategies.decimals(
         min_value=Decimal(SizeLimits.MIN_INT128), max_value=Decimal("-1E10"), places=DECIMAL_PLACES
     )
 )
 @hypothesis.example(value=Decimal(SizeLimits.MIN_INT128))
 @hypothesis.example(value=Decimal("-1E10"))
 def test_sqrt_invalid_range(sqrt_contract, value):
     with pytest.raises(TransactionFailed):
-        sqrt_contract.test(value)
+        sqrt_contract.test(decimal_to_int(value))
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_unsigned_ints.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_array_indexing.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_array_indexing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_bytes.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_literal.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_zero_padding.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_zero_padding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_dynamic_array.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_dynamic_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools
 
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     ArgumentException,
     ArrayIndexException,
     ImmutableViolation,
     OverflowException,
     StackTooDeep,
@@ -216,15 +217,18 @@
     assert c.noo([]) == []
     assert c.noo([3, 5]) == [3, 5]
     assert c.ooo([]) == []
     assert c.ooo([3, 5]) == [3, 5]
     assert c.poo([]) == []
     assert c.poo([[1, 2], [3, 4]]) == [[1, 2], [3, 4]]
     assert c.qoo([1, 2]) == [[1, 2], [3, 4]]
-    assert c.roo([1, 2]) == [[1.0, 2.0], [3.0, 4.0]]
+    assert c.roo([decimal_to_int(1), decimal_to_int(2)]) == [
+        [decimal_to_int(1), decimal_to_int(2)],
+        [decimal_to_int(3), decimal_to_int(4)],
+    ]
     assert c.soo() == [1, 2]
     assert c.too() == [2, 1]
     assert c.uoo([1, 2]) == [[1, 2], [2, 1]]
 
     print("Passed list output tests")
 
 
@@ -725,17 +729,23 @@
 def test_array_decimal_return3() -> DynArray[DynArray[decimal, 2], 2]:
     a: DynArray[DynArray[decimal, 2], 2] = [[1.0, 2.0], [3.0]]
     return a
 """
 
     c = get_contract_with_gas_estimation(code)
     assert c.test_array_num_return() == [[], [3, 4]]
-    assert c.test_array_decimal_return1() == [[1.0], [3.0, 4.0]]
-    assert c.test_array_decimal_return2() == [[1.0, 2.0]]
-    assert c.test_array_decimal_return3() == [[1.0, 2.0], [3.0]]
+    assert c.test_array_decimal_return1() == [
+        [decimal_to_int(1)],
+        [decimal_to_int(3), decimal_to_int(4)],
+    ]
+    assert c.test_array_decimal_return2() == [[decimal_to_int(1), decimal_to_int(2)]]
+    assert c.test_array_decimal_return3() == [
+        [decimal_to_int(1), decimal_to_int(2)],
+        [decimal_to_int(3)],
+    ]
 
 
 @pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_mult_list(get_contract_with_gas_estimation):
     code = """
 nest3: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 nest4: DynArray[DynArray[DynArray[DynArray[uint256, 2], 2], 2], 2]
@@ -1656,15 +1666,15 @@
 MY_LIST: constant(DynArray[decimal, 6]) = {some_good_primes}
 @external
 def ix(i: uint256) -> decimal:
     return MY_LIST[i]
     """
     c = get_contract(code)
     for i, p in enumerate(some_good_primes):
-        assert c.ix(i) == p
+        assert c.ix(i) == decimal_to_int(p)
     # assert oob
     with tx_failed():
         c.ix(len(some_good_primes) + 1)
 
 
 def test_public_dynarray(get_contract):
     code = """
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_flag.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_identifier_naming.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_lists.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import itertools
 
 import pytest
 
+from tests.utils import decimal_to_int
 from vyper.exceptions import ArrayIndexException, OverflowException, TypeMismatch
 
 
+def _map_nested(f, xs):
+    ret = []
+    for x in xs:
+        if isinstance(x, list):
+            ret.append(_map_nested(f, x))
+        else:
+            ret.append(f(x))
+    return ret
+
+
 def test_list_tester_code(get_contract_with_gas_estimation):
     list_tester_code = """
 z: int128[3]
 z2: int128[2][2]
 z3: int128[2]
 
 @external
@@ -114,17 +125,17 @@
     assert c.joo() == [3, 5]
     assert c.koo() == [[1, 2], [3, 4]]
     assert c.loo() == [[1, 2], [3, 4]]
     assert c.moo() == [[1, 2], [3, 4]]
     assert c.noo([3, 5]) == [3, 5]
     assert c.poo([[1, 2], [3, 4]]) == [[1, 2], [3, 4]]
     assert c.qoo([1, 2]) == [[1, 2], [3, 4]]
-    assert c.roo([1, 2]) == [[1.0, 2.0], [3.0, 4.0]]
-
-    print("Passed list output tests")
+    assert c.roo(_map_nested(decimal_to_int, [1.0, 2.0])) == _map_nested(
+        decimal_to_int, [[1.0, 2.0], [3.0, 4.0]]
+    )
 
 
 def test_array_accessor(get_contract_with_gas_estimation):
     array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[4] = [0, 0, 0, 0]
@@ -321,17 +332,17 @@
 def test_array_decimal_return3() -> decimal[2][2]:
     a: decimal[2][2] = [[1.0, 2.0], [3.0, 4.0]]
     return a
 """
 
     c = get_contract_with_gas_estimation(code)
     assert c.test_array_num_return() == [[1, 2], [3, 4]]
-    assert c.test_array_decimal_return1() == [[1.0, 2.0], [3.0, 4.0]]
-    assert c.test_array_decimal_return2() == [[1.0, 2.0], [3.0, 4.0]]
-    assert c.test_array_decimal_return3() == [[1.0, 2.0], [3.0, 4.0]]
+    assert c.test_array_decimal_return1() == _map_nested(decimal_to_int, [[1.0, 2.0], [3.0, 4.0]])
+    assert c.test_array_decimal_return2() == _map_nested(decimal_to_int, [[1.0, 2.0], [3.0, 4.0]])
+    assert c.test_array_decimal_return3() == _map_nested(decimal_to_int, [[1.0, 2.0], [3.0, 4.0]])
 
 
 def test_mult_list(get_contract_with_gas_estimation):
     code = """
 @external
 def test_multi3() -> uint256[2][2][2]:
     l: uint256[2][2][2] = [[[0, 0], [0, 4]], [[0, 0], [0, 123]]]
@@ -670,14 +681,17 @@
 MY_LIST: constant({type}[{len(value)}]) = {value}
 @external
 def ix(i: uint256) -> {type}:
     return MY_LIST[i]
     """
     c = get_contract(code)
     for i, p in enumerate(value):
+        if type == "decimal":
+            # special case to transform for decimal ABI
+            p = decimal_to_int(p)
         assert c.ix(i) == p
     # assert oob
     with tx_failed():
         c.ix(len(value) + 1)
 
 
 def test_nested_constant_list_accessor(get_contract):
@@ -805,14 +819,17 @@
 @external
 def ix(i: uint256, j: uint256) -> {type}:
     return MY_LIST[i][j]
     """
     c = get_contract(code)
     for i, p in enumerate(value):
         for j, q in enumerate(p):
+            if type == "decimal":
+                # special case for decimal ABI
+                q = decimal_to_int(q)
             assert c.ix(i, j) == q
     # assert oob
     with tx_failed():
         c.ix(len(value) + 1, len(value[0]) + 1)
 
 
 @pytest.mark.parametrize("storage_type,return_type", itertools.permutations(integer_types, 2))
```

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_node_types.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_string.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_string_literal.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/codegen/types/test_struct.py` & `vyper-0.4.0rc1/tests/functional/codegen/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/auctions/test_blind_auction.py` & `vyper-0.4.0rc1/tests/functional/examples/auctions/test_blind_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/auctions/test_simple_open_auction.py` & `vyper-0.4.0rc1/tests/functional/examples/auctions/test_simple_open_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/company/test_company.py` & `vyper-0.4.0rc1/tests/functional/examples/company/test_company.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/crowdfund/test_crowdfund_example.py` & `vyper-0.4.0rc1/tests/functional/examples/crowdfund/test_crowdfund_example.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/factory/test_factory.py` & `vyper-0.4.0rc1/tests/functional/examples/factory/test_factory.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.4.0rc1/tests/functional/examples/market_maker/test_on_chain_market_maker.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.4.0rc1/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/storage/test_advanced_storage.py` & `vyper-0.4.0rc1/tests/functional/examples/storage/test_advanced_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/storage/test_storage.py` & `vyper-0.4.0rc1/tests/functional/examples/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc1155.py` & `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc1155.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc20.py` & `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc4626.py` & `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc721.py` & `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/voting/test_ballot.py` & `vyper-0.4.0rc1/tests/functional/examples/voting/test_ballot.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/examples/wallet/test_wallet.py` & `vyper-0.4.0rc1/tests/functional/examples/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/grammar/test_grammar.py` & `vyper-0.4.0rc1/tests/functional/grammar/test_grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_argument_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_call_violation.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_constancy_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_function_declaration_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_function_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_instantiation_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_literal_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_payable.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_reference.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_type_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_namespace_collision.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_overflow_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_structure_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_syntax_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_type_mismatch_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_undeclared_definition.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_variable_declaration_exception.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_vyper_exception_pos.py` & `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/modules/test_deploy_visibility.py` & `vyper-0.4.0rc1/tests/functional/syntax/modules/test_deploy_visibility.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/modules/test_exports.py` & `vyper-0.4.0rc1/tests/functional/syntax/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/modules/test_implements.py` & `vyper-0.4.0rc1/tests/functional/syntax/modules/test_implements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/modules/test_initializers.py` & `vyper-0.4.0rc1/tests/functional/syntax/modules/test_initializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 initializes: lib1
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(InitializerException) as e:
         compile_code(main, input_bundle=input_bundle)
     assert e.value._message == "`lib2` uses `lib1`, but it is not initialized with `lib1`"
-    assert e.value._hint == "add `lib1` to its initializer list"
+    assert e.value._hint == "did you mean lib2[lib1 := lib1]?"
 
 
 def test_missing_uses(make_input_bundle):
     lib1 = """
 counter: uint256
     """
     lib2 = """
@@ -1224,7 +1224,71 @@
     lib1.counter += 1
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     assert (
         compile_code(main, input_bundle=input_bundle, output_formats=["annotated_ast_dict"])
         is not None
     )
+
+
+def test_hint_for_missing_initializer_in_list(make_input_bundle):
+    lib1 = """
+counter: uint256
+    """
+    lib3 = """
+counter: uint256
+        """
+    lib2 = """
+import lib1
+import lib3
+
+uses: lib1
+uses: lib3
+
+counter: uint256
+
+@internal
+def foo():
+    lib1.counter += 1
+    lib3.counter += 1
+    """
+    main = """
+import lib1
+import lib2
+import lib3
+
+initializes: lib2[lib1:=lib1]
+initializes: lib1
+initializes: lib3
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2, "lib3.vy": lib3})
+    with pytest.raises(InitializerException) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "`lib2` uses `lib3`, but it is not initialized with `lib3`"
+    assert e.value._hint == "add `lib3 := lib3` to its initializer list"
+
+
+def test_hint_for_missing_initializer_when_no_import(make_input_bundle):
+    lib1 = """
+counter: uint256
+    """
+    lib2 = """
+import lib1
+
+uses: lib1
+
+counter: uint256
+
+@internal
+def foo():
+    lib1.counter += 1
+    """
+    main = """
+import lib2
+
+initializes: lib2
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
+    with pytest.raises(InitializerException) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "`lib2` uses `lib1`, but it is not initialized with `lib1`"
+    assert e.value._hint == "try importing lib1 first"
```

### Comparing `vyper-0.4.0b6/tests/functional/syntax/names/test_event_names.py` & `vyper-0.4.0rc1/tests/functional/syntax/names/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/names/test_function_names.py` & `vyper-0.4.0rc1/tests/functional/syntax/names/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/names/test_variable_names.py` & `vyper-0.4.0rc1/tests/functional/syntax/names/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/signatures/test_invalid_function_decorators.py` & `vyper-0.4.0rc1/tests/functional/syntax/signatures/test_invalid_function_decorators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/signatures/test_method_id_conflicts.py` & `vyper-0.4.0rc1/tests/functional/syntax/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_abi_decode.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_abi_encode.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_abs.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_addmulmod.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_addmulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_address_code.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_address_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_ann_assign.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_as_uint256.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_as_wei_value.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_block.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_blockscope.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_bool.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_bool.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_bool_ops.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_bool_ops.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_bytes.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_chainid.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_chainid.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_code_size.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_codehash.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_codehash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_concat.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_constants.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_create_with_code_of.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_dynamic_array.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_external_calls.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_external_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_extract32.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_flag.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_for_range.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_functions_call.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_immutables.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_init.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_interfaces.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_invalids.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_keccak256.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_len.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_list.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_logging.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_method_id.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_minmax.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_minmax_value.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_msg_data.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_msg_data.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_nested_list.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_nested_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_no_none.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_no_none.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_powmod.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_print.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_public.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_raw_call.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_return_tuple.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_self_balance.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_self_balance.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_selfdestruct.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_send.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_slice.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_string.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_structs.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_structs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_ternary.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_tuple_assign.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/functional/syntax/test_unbalanced_return.py` & `vyper-0.4.0rc1/tests/functional/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/abi_types/test_invalid_abi_types.py` & `vyper-0.4.0rc1/tests/unit/abi_types/test_invalid_abi_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 import pytest
 
-from vyper.abi_types import (
-    ABI_Bytes,
-    ABI_BytesM,
-    ABI_DynamicArray,
-    ABI_FixedMxN,
-    ABI_GIntM,
-    ABI_String,
-)
+from vyper.abi_types import ABI_Bytes, ABI_BytesM, ABI_DynamicArray, ABI_GIntM, ABI_String
 from vyper.exceptions import InvalidABIType
 
 cases_invalid_types = [
     (ABI_GIntM, ((0, False), (7, False), (300, True), (300, False))),
-    (ABI_FixedMxN, ((0, 0, False), (8, 0, False), (256, 81, True), (300, 80, False))),
     (ABI_BytesM, ((0,), (33,), (-10,))),
     (ABI_Bytes, ((-1,), (-69,))),
     (ABI_DynamicArray, ((ABI_GIntM(256, False), -1), (ABI_String(256), -10))),
 ]
 
 
 @pytest.mark.parametrize("typ,params_variants", cases_invalid_types)
```

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_compare_nodes.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_decimal.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_decimal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from decimal import Decimal
 
 import pytest
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
-from tests.utils import parse_and_fold
+from tests.utils import decimal_to_int, parse_and_fold
 from vyper.exceptions import OverflowException, TypeMismatch, ZeroDivisionException
 from vyper.semantics.analysis.local import ExprVisitor
 from vyper.semantics.types import DecimalT
 
 DECIMAL_T = DecimalT()
 
 st_decimals = st.decimals(
@@ -35,22 +35,27 @@
     return a {op} b
     """
     contract = get_contract(source)
 
     try:
         vyper_ast = parse_and_fold(f"{left} {op} {right}")
         expr = vyper_ast.body[0].value
+
+        # check invalid values
         ExprVisitor().visit(expr, DecimalT())
+
         new_node = expr.get_folded_value()
         is_valid = True
     except (OverflowException, ZeroDivisionException):
         is_valid = False
 
+    left = decimal_to_int(left)
+    right = decimal_to_int(right)
     if is_valid:
-        assert contract.foo(left, right) == new_node.value
+        assert contract.foo(left, right) == decimal_to_int(new_node.value)
     else:
         with tx_failed():
             contract.foo(left, right)
 
 
 def test_binop_pow():
     # raises because Vyper does not support decimal exponentiation
@@ -77,21 +82,24 @@
     contract = get_contract(source)
 
     literal_op = " ".join(f"{a} {b}" for a, b in zip(values, ops))
     literal_op = literal_op.rsplit(maxsplit=1)[0]
     try:
         vyper_ast = parse_and_fold(literal_op)
         expr = vyper_ast.body[0].value
+
+        # check invalid intermediate values
         ExprVisitor().visit(expr, DecimalT())
+
         new_node = expr.get_folded_value()
         expected = new_node.value
-        lo, hi = DecimalT().decimal_bounds
-        is_valid = lo <= expected < hi
+        is_valid = True
     except (OverflowException, ZeroDivisionException):
         # for overflow or division/modulus by 0, expect the contract call to revert
         is_valid = False
 
+    values = [decimal_to_int(v) for v in values]
     if is_valid:
-        assert contract.foo(*values) == expected
+        assert contract.foo(*values) == decimal_to_int(expected)
     else:
         with tx_failed():
             contract.foo(*values)
```

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_int.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_boolop.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_compare.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_subscript.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_subscript.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_unaryop.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_from_node.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_get_children.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_get_descendants.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/nodes/test_hex.py` & `vyper-0.4.0rc1/tests/unit/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_annotate_and_optimize_ast.py` & `vyper-0.4.0rc1/tests/unit/ast/test_annotate_and_optimize_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_ast_dict.py` & `vyper-0.4.0rc1/tests/unit/ast/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_metadata_journal.py` & `vyper-0.4.0rc1/tests/unit/ast/test_metadata_journal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_natspec.py` & `vyper-0.4.0rc1/tests/unit/ast/test_natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_parser.py` & `vyper-0.4.0rc1/tests/unit/ast/test_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_pre_parser.py` & `vyper-0.4.0rc1/tests/unit/ast/test_pre_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+from vyper import compile_code
 from vyper.ast.pre_parser import pre_parse, validate_version_pragma
 from vyper.compiler.phases import CompilerData
 from vyper.compiler.settings import OptimizationLevel, Settings
 from vyper.exceptions import StructureException, VersionException
 
 SRC_LINE = (1, 0)  # Dummy source line
 COMPILER_VERSION = "0.1.1"
@@ -41,22 +42,22 @@
     "abc",
 ]
 
 
 @pytest.mark.parametrize("file_version", valid_versions)
 def test_valid_version_pragma(file_version, mock_version):
     mock_version(COMPILER_VERSION)
-    validate_version_pragma(f"{file_version}", (SRC_LINE))
+    validate_version_pragma(f"{file_version}", file_version, (SRC_LINE))
 
 
 @pytest.mark.parametrize("file_version", invalid_versions)
 def test_invalid_version_pragma(file_version, mock_version):
     mock_version(COMPILER_VERSION)
     with pytest.raises(VersionException):
-        validate_version_pragma(f"{file_version}", (SRC_LINE))
+        validate_version_pragma(f"{file_version}", file_version, (SRC_LINE))
 
 
 prerelease_valid_versions = [
     "<0.1.1-beta.9",
     "<0.1.1b9",
     "0.1.1b7",
     ">0.1.1b2",
@@ -78,22 +79,22 @@
     "<0.1.1a9",
 ]
 
 
 @pytest.mark.parametrize("file_version", prerelease_valid_versions)
 def test_prerelease_valid_version_pragma(file_version, mock_version):
     mock_version(PRERELEASE_COMPILER_VERSION)
-    validate_version_pragma(file_version, (SRC_LINE))
+    validate_version_pragma(file_version, file_version, (SRC_LINE))
 
 
 @pytest.mark.parametrize("file_version", prerelease_invalid_versions)
 def test_prerelease_invalid_version_pragma(file_version, mock_version):
     mock_version(PRERELEASE_COMPILER_VERSION)
     with pytest.raises(VersionException):
-        validate_version_pragma(file_version, (SRC_LINE))
+        validate_version_pragma(file_version, file_version, (SRC_LINE))
 
 
 pragma_examples = [
     (
         """
     """,
         Settings(),
@@ -180,15 +181,15 @@
     compiler_data = CompilerData(code)
 
     # check what happens after CompilerData constructor
     if compiler_data_settings is None:
         # None is sentinel here meaning that nothing changed
         compiler_data_settings = pre_parse_settings
 
-    # cannot be set via pragma, don't check
+    # experimental_codegen is False by default
     compiler_data_settings.experimental_codegen = False
 
     assert compiler_data.settings == compiler_data_settings
 
 
 invalid_pragmas = [
     # evm-versionnn
@@ -220,7 +221,36 @@
 ]
 
 
 @pytest.mark.parametrize("code", invalid_pragmas)
 def test_invalid_pragma(code):
     with pytest.raises(StructureException):
         pre_parse(code)
+
+
+def test_version_exception_in_import(make_input_bundle):
+    lib_version = "~=0.3.10"
+    lib = f"""
+#pragma version {lib_version}
+
+@external
+def foo():
+    pass
+    """
+
+    code = """
+import lib
+
+uses: lib
+
+@external
+def bar():
+    pass
+    """
+    input_bundle = make_input_bundle({"lib.vy": lib})
+
+    with pytest.raises(VersionException) as excinfo:
+        compile_code(code, input_bundle=input_bundle)
+    annotation = excinfo.value.annotations[0]
+    assert annotation.lineno == 2
+    assert annotation.col_offset == 0
+    assert annotation.full_source_code == lib
```

### Comparing `vyper-0.4.0b6/tests/unit/ast/test_source_annotation.py` & `vyper-0.4.0rc1/tests/unit/ast/test_source_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout.py` & `vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout_overrides.py` & `vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout_overrides.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_compile_files.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_compile_files.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_parse_args.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_compile_json.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_compile_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_inputs.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_inputs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_settings.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def test_unknown_evm():
     with pytest.raises(JSONError):
         get_evm_version({"settings": {"evmVersion": "foo"}})
 
 
 @pytest.mark.parametrize(
-    "evm_version",
+    "evm_version_str",
     [
         "homestead",
         "tangerineWhistle",
         "spuriousDragon",
         "byzantium",
         "constantinople",
         "petersburg",
         "istanbul",
         "berlin",
     ],
 )
-def test_early_evm(evm_version):
+def test_early_evm(evm_version_str):
     with pytest.raises(JSONError):
-        get_evm_version({"settings": {"evmVersion": evm_version}})
+        get_evm_version({"settings": {"evmVersion": evm_version_str}})
 
 
-@pytest.mark.parametrize("evm_version", ["london", "paris", "shanghai", "cancun"])
-def test_valid_evm(evm_version):
-    assert evm_version == get_evm_version({"settings": {"evmVersion": evm_version}})
+@pytest.mark.parametrize("evm_version_str", ["london", "paris", "shanghai", "cancun"])
+def test_valid_evm(evm_version_str):
+    assert evm_version_str == get_evm_version({"settings": {"evmVersion": evm_version_str}})
```

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_output_selection.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/asm/test_asm_optimizer.py` & `vyper-0.4.0rc1/tests/unit/compiler/asm/test_asm_optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/ir/test_compile_ir.py` & `vyper-0.4.0rc1/tests/unit/compiler/ir/test_compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/ir/test_optimize_ir.py` & `vyper-0.4.0rc1/tests/unit/compiler/ir/test_optimize_ir.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import pytest
 
 from vyper.codegen.ir_node import IRnode
-from vyper.evm.opcodes import EVM_VERSIONS, anchor_evm_version
+from vyper.evm.opcodes import version_check
 from vyper.exceptions import StaticAssertionException
 from vyper.ir import optimizer
 
-POST_CANCUN = {k: v for k, v in EVM_VERSIONS.items() if v >= EVM_VERSIONS["cancun"]}
-
-
 optimize_list = [
     (["eq", 1, 2], [0]),
     (["lt", 1, 2], [1]),
     (["eq", "x", 0], ["iszero", "x"]),
     (["ne", "x", 0], ["iszero", ["iszero", "x"]]),
     (["ne", "x", 1], None),
     (["iszero", ["ne", "x", 1]], ["iszero", ["iszero", ["iszero", ["xor", "x", 1]]]]),
@@ -364,18 +361,20 @@
         ],
         ["mcopy", 2**256 - 1 - 31 - 32, 0, 64],
     ),
 ]
 
 
 @pytest.mark.parametrize("ir", mload_merge_list)
-@pytest.mark.parametrize("evm_version", list(POST_CANCUN.keys()))
 def test_mload_merge(ir, evm_version):
-    with anchor_evm_version(evm_version):
+    # TODO: use something like pytest.mark.post_cancun
+    if version_check(begin="cancun"):
         optimized = optimizer.optimize(IRnode.from_list(ir[0]))
         if ir[1] is None:
             # no-op, assert optimizer does nothing
             expected = IRnode.from_list(ir[0])
         else:
             expected = IRnode.from_list(ir[1])
 
         assert optimized == expected
+    else:
+        pytest.skip("no mcopy available")
```

### Comparing `vyper-0.4.0b6/tests/unit/compiler/ir/test_with.py` & `vyper-0.4.0rc1/tests/unit/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_abi.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_abi.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,47 @@
     """
 
     out = compile_code(code, output_formats=["method_identifiers"])
 
     assert out["method_identifiers"] == {"foo(uint256)": "0x2fbebd38", "x()": "0xc55699c"}
 
 
+def test_decimal_abi():
+    code = """
+x: public(decimal)
+
+@external
+@view
+def foo(s: decimal) -> decimal:
+    return s
+    """
+
+    out = compile_code(code, output_formats=["method_identifiers", "abi"])
+
+    assert out["method_identifiers"] == {"foo(int168)": "0x929893b6", "x()": "0xc55699c"}
+
+    expected_abi = [
+        {
+            "stateMutability": "view",
+            "type": "function",
+            "name": "foo",
+            "inputs": [{"name": "s", "type": "int168", "internalType": "decimal"}],
+            "outputs": [{"name": "", "type": "int168", "internalType": "decimal"}],
+        },
+        {
+            "stateMutability": "view",
+            "type": "function",
+            "name": "x",
+            "inputs": [],
+            "outputs": [{"name": "", "type": "int168", "internalType": "decimal"}],
+        },
+    ]
+    assert out["abi"] == expected_abi
+
+
 def test_struct_abi():
     code = """
 struct MyStruct:
     a: address
     b: uint256
 
 @external
```

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_bytecode_runtime.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_bytecode_runtime.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_compile_code.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_compile_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_default_settings.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_default_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,16 @@
     assert compiler_data.settings.optimize == OptimizationLevel.GAS
 
 
 def test_default_opt_level():
     assert OptimizationLevel.default() == OptimizationLevel.GAS
 
 
-def test_codegen_opt_level():
-    assert core._opt_level == OptimizationLevel.GAS
-    assert core._opt_gas() is True
-    assert core._opt_none() is False
-    assert core._opt_codesize() is False
+def test_codegen_opt_level(optimize):
+    assert core._opt_gas() == (optimize == OptimizationLevel.GAS)
+    assert core._opt_none() == (optimize == OptimizationLevel.NONE)
+    assert core._opt_codesize() == (optimize == OptimizationLevel.CODESIZE)
 
 
 def test_debug_mode(pytestconfig):
     debug_mode = pytestconfig.getoption("enable_compiler_debug_mode")
     assert _is_debug_mode() == debug_mode
```

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_input_bundle.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_opcodes.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_opcodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,14 @@
 
 import vyper
 from vyper.compiler.output import _build_opcodes
 from vyper.evm import opcodes
 from vyper.exceptions import CompilerPanic
 
 
-@pytest.fixture(params=list(opcodes.EVM_VERSIONS))
-def evm_version(request):
-    default = opcodes.active_evm_version
-    try:
-        opcodes.active_evm_version = opcodes.EVM_VERSIONS[request.param]
-        yield request.param
-    finally:
-        opcodes.active_evm_version = default
-
-
 def test_opcodes():
     code = """
 @external
 def a() -> bool:
     return True
     """
```

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_pre_parser.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_sha3_32.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/test_source_map.py` & `vyper-0.4.0rc1/tests/unit/compiler/test_source_map.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/venom/test_convert_basicblock_simple.py` & `vyper-0.4.0rc1/tests/unit/compiler/venom/test_convert_basicblock_simple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/venom/test_dominator_tree.py` & `vyper-0.4.0rc1/tests/unit/compiler/venom/test_dominator_tree.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/venom/test_duplicate_operands.py` & `vyper-0.4.0rc1/tests/unit/compiler/venom/test_duplicate_operands.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/venom/test_make_ssa.py` & `vyper-0.4.0rc1/tests/unit/compiler/venom/test_make_ssa.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/compiler/venom/test_multi_entry_block.py` & `vyper-0.4.0rc1/tests/unit/compiler/venom/test_multi_entry_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/analysis/test_array_index.py` & `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/analysis/test_for_loop.py` & `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/analysis/test_potential_types.py` & `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/conftest.py` & `vyper-0.4.0rc1/tests/unit/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/test_namespace.py` & `vyper-0.4.0rc1/tests/unit/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/test_storage_slots.py` & `vyper-0.4.0rc1/tests/unit/semantics/test_storage_slots.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/types/test_event.py` & `vyper-0.4.0rc1/tests/unit/semantics/types/test_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import pytest
 
 from vyper.semantics.types.user import EventT
+from vyper.utils import keccak256
 
+
+def keccak256_int(signature_str):
+    return int.from_bytes(keccak256(signature_str.encode()), "big")
+
+
+# TODO: refactor these to all use keccak256_int util instead of hardcoded constants
 EVENT_ID_TESTS = [
     (
         "event MyLog: pass",
         # MyLog()
         0x375227D322F87546308335EBD7DD99C33B9D50E4DA37CE574E20471DA5E5CBE3,
     ),
     (
@@ -68,25 +75,23 @@
     e: String[1]""",
         # Nonsense(bytes,int128[4][38],address[3],uint256,string)
         0xEE1C420D3504F8A563AA99C8341A41C4C2A1A7F35665EE2F5F341CB8F451B5FC,
     ),
     (
         """event Bar:
     a: decimal[4]""",
-        # Bar(fixed168x10[4])
-        0x7F5D3D77DC11EED2D256D513EF1916FBA342AD13DD629E3C2FF3BD1BAEADF932,
+        keccak256_int("Bar(int168[4])"),
     ),
     (
         """event Rtadr:
     a: indexed(decimal)
     b: decimal[2][5]
     c: Bytes[4]
     d: decimal[666]""",
-        # Rtadr(fixed168x10,fixed168x10[2][5],bytes,fixed168x10[666])
-        0x20B4E04949A8E3B03C8DECC09D8B18B271D42E66F83B9FAA7B75EA7E22E27177,
+        keccak256_int("Rtadr(int168,int168[2][5],bytes,int168[666])"),
     ),
 ]
 
 
 @pytest.mark.parametrize("source,signature_hash", EVENT_ID_TESTS)
 def test_event_id(build_node, source, signature_hash):
     node = build_node(source)
```

### Comparing `vyper-0.4.0b6/tests/unit/semantics/types/test_pure_types.py` & `vyper-0.4.0rc1/tests/unit/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/types/test_size_in_bytes.py` & `vyper-0.4.0rc1/tests/unit/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_abi.py` & `vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_annotation.py` & `vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/__init__.py` & `vyper-0.4.0rc1/vyper/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/__main__.py` & `vyper-0.4.0rc1/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/abi_types.py` & `vyper-0.4.0rc1/vyper/abi_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,43 +105,14 @@
     def __init__(self):
         return super().__init__(8, False)
 
     def selector_name(self):
         return "bool"
 
 
-# fixed<M>x<N>: signed fixed-point decimal number of M bits, 8 <= M <= 256,
-#   M % 8 ==0, and 0 < N <= 80, which denotes the value v as v / (10 ** N).
-# ufixed<M>x<N>: unsigned variant of fixed<M>x<N>.
-# fixed, ufixed: synonyms for fixed128x18, ufixed128x18 respectively.
-#   For computing the function selector, fixed128x18 and ufixed128x18 have to be used.
-class ABI_FixedMxN(ABIType):
-    def __init__(self, m_bits, n_places, signed):
-        if not (0 < m_bits <= 256 and 0 == m_bits % 8):
-            raise InvalidABIType("Invalid M for FixedMxN")
-        if not (0 < n_places and n_places <= 80):
-            raise InvalidABIType("Invalid N for FixedMxN")
-
-        self.m_bits = m_bits
-        self.n_places = n_places
-        self.signed = signed
-
-    def is_dynamic(self):
-        return False
-
-    def static_size(self):
-        return 32
-
-    def selector_name(self):
-        return ("" if self.signed else "u") + f"fixed{self.m_bits}x{self.n_places}"
-
-    def is_complex_type(self):
-        return False
-
-
 # bytes<M>: binary type of M bytes, 0 < M <= 32.
 class ABI_BytesM(ABIType):
     def __init__(self, m_bytes):
         if not 0 < m_bytes <= 32:
             raise InvalidABIType("Invalid M for BytesM")
 
         self.m_bytes = m_bytes
```

### Comparing `vyper-0.4.0b6/vyper/ast/README.md` & `vyper-0.4.0rc1/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/grammar.lark` & `vyper-0.4.0rc1/vyper/ast/grammar.lark`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/grammar.py` & `vyper-0.4.0rc1/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/identifiers.py` & `vyper-0.4.0rc1/vyper/ast/identifiers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/metadata.py` & `vyper-0.4.0rc1/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/natspec.py` & `vyper-0.4.0rc1/vyper/ast/natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/nodes.py` & `vyper-0.4.0rc1/vyper/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/nodes.pyi` & `vyper-0.4.0rc1/vyper/ast/nodes.pyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/parse.py` & `vyper-0.4.0rc1/vyper/ast/parse.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/pre_parser.py` & `vyper-0.4.0rc1/vyper/ast/pre_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,44 @@
 # seems a bit early to be importing this but we want it to validate the
 # evm-version pragma
 from vyper.evm.opcodes import EVM_VERSIONS
 from vyper.exceptions import StructureException, SyntaxException, VersionException
 from vyper.typing import ModificationOffsets, ParserPosition
 
 
-def validate_version_pragma(version_str: str, start: ParserPosition) -> None:
+def validate_version_pragma(version_str: str, full_source_code: str, start: ParserPosition) -> None:
     """
     Validates a version pragma directive against the current compiler version.
     """
     from vyper import __version__
 
     if len(version_str) == 0:
-        raise VersionException("Version specification cannot be empty", start)
+        raise VersionException("Version specification cannot be empty", full_source_code, *start)
 
     # X.Y.Z or vX.Y.Z => ==X.Y.Z, ==vX.Y.Z
     if re.match("[v0-9]", version_str):
         version_str = "==" + version_str
     # convert npm to pep440
     version_str = re.sub("^\\^", "~=", version_str)
 
     try:
         spec = SpecifierSet(version_str)
     except InvalidSpecifier:
         raise VersionException(
-            f'Version specification "{version_str}" is not a valid PEP440 specifier', start
+            f'Version specification "{version_str}" is not a valid PEP440 specifier',
+            full_source_code,
+            *start,
         )
 
     if not spec.contains(__version__, prereleases=True):
         raise VersionException(
             f'Version specification "{version_str}" is not compatible '
             f'with compiler version "{__version__}"',
-            start,
+            full_source_code,
+            *start,
         )
 
 
 class ForParserState(enum.Enum):
     NOT_RUNNING = enum.auto()
     START_SOON = enum.auto()
     RUNNING = enum.auto()
@@ -172,26 +175,27 @@
 
             if typ == COMMENT:
                 contents = string[1:].strip()
                 if contents.startswith("@version"):
                     if settings.compiler_version is not None:
                         raise StructureException("compiler version specified twice!", start)
                     compiler_version = contents.removeprefix("@version ").strip()
-                    validate_version_pragma(compiler_version, start)
+                    validate_version_pragma(compiler_version, code, start)
                     settings.compiler_version = compiler_version
 
                 if contents.startswith("pragma "):
                     pragma = contents.removeprefix("pragma ").strip()
                     if pragma.startswith("version "):
                         if settings.compiler_version is not None:
                             raise StructureException("pragma version specified twice!", start)
                         compiler_version = pragma.removeprefix("version ").strip()
-                        validate_version_pragma(compiler_version, start)
+                        validate_version_pragma(compiler_version, code, start)
                         settings.compiler_version = compiler_version
 
+                    # TODO: refactor these to something like Settings.from_pragma
                     elif pragma.startswith("optimize "):
                         if settings.optimize is not None:
                             raise StructureException("pragma optimize specified twice!", start)
                         try:
                             mode = pragma.removeprefix("optimize").strip()
                             settings.optimize = OptimizationLevel.from_string(mode)
                         except ValueError:
@@ -205,14 +209,20 @@
                         settings.evm_version = evm_version
                     elif pragma.startswith("experimental-codegen"):
                         if settings.experimental_codegen is not None:
                             raise StructureException(
                                 "pragma experimental-codegen specified twice!", start
                             )
                         settings.experimental_codegen = True
+                    elif pragma.startswith("enable-decimals"):
+                        if settings.enable_decimals is not None:
+                            raise StructureException(
+                                "pragma enable_decimals specified twice!", start
+                            )
+                        settings.enable_decimals = True
 
                     else:
                         raise StructureException(f"Unknown pragma `{pragma.split()[0]}`")
 
             if typ == NAME and string in ("class", "yield"):
                 raise SyntaxException(
                     f"The `{string}` keyword is not allowed. ", code, start[0], start[1]
```

### Comparing `vyper-0.4.0b6/vyper/ast/utils.py` & `vyper-0.4.0rc1/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ast/validation.py` & `vyper-0.4.0rc1/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/builtins/_convert.py` & `vyper-0.4.0rc1/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/builtins/_signatures.py` & `vyper-0.4.0rc1/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/builtins/_utils.py` & `vyper-0.4.0rc1/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/builtins/functions.py` & `vyper-0.4.0rc1/vyper/builtins/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1538,24 +1538,24 @@
 # CREATE* functions
 
 CREATE2_SENTINEL = dummy_node_for_type(BYTES32_T)
 
 
 # create helper functions
 # generates CREATE op sequence + zero check for result
-def _create_ir(value, buf, length, salt, checked=True):
+def _create_ir(value, buf, length, salt, revert_on_failure=True):
     args = [value, buf, length]
     create_op = "create"
     if salt is not CREATE2_SENTINEL:
         create_op = "create2"
         args.append(salt)
 
     ret = IRnode.from_list(ensure_eval_once("create_builtin", [create_op, *args]))
 
-    if not checked:
+    if not revert_on_failure:
         return ret
 
     ret = clamp_nonzero(ret)
     ret.set_error_msg(f"{create_op} failed")
     return ret
 
 
@@ -1648,14 +1648,15 @@
     return ["or", bytes_to_int(evm), shl(shl_bits, codesize)], evm_len
 
 
 class _CreateBase(BuiltinFunctionT):
     _kwargs = {
         "value": KwargSettings(UINT256_T, zero_value),
         "salt": KwargSettings(BYTES32_T, empty_value),
+        "revert_on_failure": KwargSettings(BoolT(), True, require_literal=True),
     }
     _return_type = AddressT()
 
     @process_inputs
     def build_IR(self, expr, args, kwargs, context):
         # errmsg something like "Cannot use {self._id} in pure fn"
         context.check_is_not_constant("use {self._id}", expr)
@@ -1681,15 +1682,15 @@
     _inputs = [("target", AddressT())]
 
     def _add_gas_estimate(self, args, should_use_create2):
         a, b, c = eip1167_bytecode()
         bytecode_len = 20 + len(b) + len(c)
         return _create_addl_gas_estimate(bytecode_len, should_use_create2)
 
-    def _build_create_IR(self, expr, args, context, value, salt):
+    def _build_create_IR(self, expr, args, context, value, salt, revert_on_failure):
         target_address = args[0]
 
         buf = context.new_internal_variable(BytesT(96))
 
         loader_evm, forwarder_pre_evm, forwarder_post_evm = eip1167_bytecode()
         # Adjust to 32-byte boundaries
         preamble_length = len(loader_evm) + len(forwarder_pre_evm)
@@ -1709,15 +1710,15 @@
         buf_len = preamble_length + 20 + len(forwarder_post_evm)
 
         return [
             "seq",
             ["mstore", buf, forwarder_preamble],
             ["mstore", ["add", buf, preamble_length], aligned_target],
             ["mstore", ["add", buf, preamble_length + 20], forwarder_post],
-            _create_ir(value, buf, buf_len, salt=salt),
+            _create_ir(value, buf, buf_len, salt, revert_on_failure),
         ]
 
 
 class CreateForwarderTo(CreateMinimalProxyTo):
     _warned = False
 
     def build_IR(self, expr, context):
@@ -1738,15 +1739,15 @@
     def _preamble_len(self):
         return 11
 
     def _add_gas_estimate(self, args, should_use_create2):
         # max possible runtime length + preamble length
         return _create_addl_gas_estimate(EIP_170_LIMIT + self._preamble_len, should_use_create2)
 
-    def _build_create_IR(self, expr, args, context, value, salt):
+    def _build_create_IR(self, expr, args, context, value, salt, revert_on_failure):
         target = args[0]
 
         # something we can pass to scope_multi
         with scope_multi(
             (target, value, salt), ("create_target", "create_value", "create_salt")
         ) as (b1, (target, value, salt)):
             codesize = IRnode.from_list(["extcodesize", target])
@@ -1772,37 +1773,40 @@
                 # copy the target code into memory. current layout:
                 # msize | 00...00 (22 0's) | preamble | bytecode
                 ir.append(["extcodecopy", target, add_ofst(mem_ofst, 32), 0, codesize])
 
                 buf = add_ofst(mem_ofst, 32 - preamble_len)
                 buf_len = ["add", codesize, preamble_len]
 
-                ir.append(_create_ir(value, buf, buf_len, salt))
+                ir.append(_create_ir(value, buf, buf_len, salt, revert_on_failure))
 
                 return b1.resolve(b2.resolve(ir))
 
 
 class CreateFromBlueprint(_CreateBase):
     _id = "create_from_blueprint"
     _inputs = [("target", AddressT())]
     _kwargs = {
         "value": KwargSettings(UINT256_T, zero_value),
         "salt": KwargSettings(BYTES32_T, empty_value),
         "raw_args": KwargSettings(BoolT(), False, require_literal=True),
         "code_offset": KwargSettings(UINT256_T, IRnode.from_list(3, typ=UINT256_T)),
+        "revert_on_failure": KwargSettings(BoolT(), True, require_literal=True),
     }
     _has_varargs = True
 
     def _add_gas_estimate(self, args, should_use_create2):
         ctor_args = ir_tuple_from_args(args[1:])
         # max possible size of init code
         maxlen = EIP_170_LIMIT + ctor_args.typ.abi_type.size_bound()
         return _create_addl_gas_estimate(maxlen, should_use_create2)
 
-    def _build_create_IR(self, expr, args, context, value, salt, code_offset, raw_args):
+    def _build_create_IR(
+        self, expr, args, context, value, salt, code_offset, raw_args, revert_on_failure
+    ):
         target = args[0]
         ctor_args = args[1:]
 
         ctor_args = [ensure_in_memory(arg, context) for arg in ctor_args]
 
         if raw_args:
             if len(ctor_args) != 1 or not isinstance(ctor_args[0].typ, BytesT):
@@ -1870,15 +1874,15 @@
                 #    dst = add_ofst(mem_ofst, codesize)
                 #    encoded_args_len = self._encode_args(dst, ctor_args, context)
                 # else:
                 #    encoded_args_len = 0
 
                 length = ["add", codesize, encoded_args_len]
 
-                ir.append(_create_ir(value, mem_ofst, length, salt))
+                ir.append(_create_ir(value, mem_ofst, length, salt, revert_on_failure))
 
                 return b1.resolve(b2.resolve(ir))
 
 
 class _UnsafeMath(BuiltinFunctionT):
     # TODO add unsafe math for `decimal`s
     _inputs = [("a", IntegerT.any()), ("b", IntegerT.any())]
```

### Comparing `vyper-0.4.0b6/vyper/builtins/interfaces/IERC20.vyi` & `vyper-0.4.0rc1/vyper/builtins/interfaces/IERC20.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/builtins/interfaces/IERC4626.vyi` & `vyper-0.4.0rc1/vyper/builtins/interfaces/IERC4626.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/builtins/interfaces/IERC721.vyi` & `vyper-0.4.0rc1/vyper/builtins/interfaces/IERC721.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/cli/vyper_compile.py` & `vyper-0.4.0rc1/vyper/cli/vyper_compile.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 from typing import Any, Iterable, Iterator, Optional, Set, TypeVar
 
 import vyper
 import vyper.codegen.ir_node as ir_node
 import vyper.evm.opcodes as evm
 from vyper.cli import vyper_json
 from vyper.compiler.input_bundle import FileInput, FilesystemInputBundle
-from vyper.compiler.settings import (
-    VYPER_TRACEBACK_LIMIT,
-    OptimizationLevel,
-    Settings,
-    _set_debug_mode,
-)
+from vyper.compiler.settings import VYPER_TRACEBACK_LIMIT, OptimizationLevel, Settings
 from vyper.typing import ContractPath, OutputFormats
 
 T = TypeVar("T")
 
 format_options_help = """Format to print, one or more of:
 bytecode (default) - Deployable bytecode
 bytecode_runtime   - Bytecode at runtime
@@ -148,14 +143,15 @@
     parser.add_argument("-o", help="Set the output path", dest="output_path")
     parser.add_argument(
         "--experimental-codegen",
         help="The compiler use the new IR codegen. This is an experimental feature.",
         action="store_true",
         dest="experimental_codegen",
     )
+    parser.add_argument("--enable-decimals", help="Enable decimals", action="store_true")
 
     args = parser.parse_args(argv)
 
     if args.traceback_limit is not None:
         sys.tracebacklimit = args.traceback_limit
     elif VYPER_TRACEBACK_LIMIT is not None:
         sys.tracebacklimit = VYPER_TRACEBACK_LIMIT
@@ -168,17 +164,14 @@
         sys.tracebacklimit = 0
 
     if args.hex_ir:
         ir_node.AS_HEX_DEFAULT = True
 
     output_formats = tuple(uniq(args.format.split(",")))
 
-    if args.debug:
-        _set_debug_mode(True)
-
     if args.no_optimize and args.optimize:
         raise ValueError("Cannot use `--no-optimize` and `--optimize` at the same time!")
 
     settings = Settings()
 
     if args.no_optimize:
         settings.optimize = OptimizationLevel.NONE
@@ -187,14 +180,20 @@
 
     if args.evm_version:
         settings.evm_version = args.evm_version
 
     if args.experimental_codegen:
         settings.experimental_codegen = args.experimental_codegen
 
+    if args.debug:
+        settings.debug = args.debug
+
+    if args.enable_decimals:
+        settings.enable_decimals = args.enable_decimals
+
     if args.verbose:
         print(f"cli specified: `{settings}`", file=sys.stderr)
 
     compiled = compile_files(
         args.input_files,
         output_formats,
         args.paths,
```

### Comparing `vyper-0.4.0b6/vyper/cli/vyper_ir.py` & `vyper-0.4.0rc1/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/cli/vyper_json.py` & `vyper-0.4.0rc1/vyper/cli/vyper_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/abi_encoder.py` & `vyper-0.4.0rc1/vyper/codegen/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/arithmetic.py` & `vyper-0.4.0rc1/vyper/codegen/arithmetic.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/context.py` & `vyper-0.4.0rc1/vyper/codegen/context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/core.py` & `vyper-0.4.0rc1/vyper/codegen/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import contextlib
-from typing import Generator
-
 from vyper.codegen.ir_node import Encoding, IRnode
-from vyper.compiler.settings import OptimizationLevel
+from vyper.compiler.settings import _opt_codesize, _opt_gas, _opt_none
 from vyper.evm.address_space import (
     CALLDATA,
     DATA,
     IMMUTABLES,
     MEMORY,
     STORAGE,
     TRANSIENT,
@@ -912,48 +909,14 @@
 
     # Complex Types
     assert isinstance(left.typ, (SArrayT, TupleT, StructT))
 
     return _complex_make_setter(left, right)
 
 
-_opt_level = OptimizationLevel.GAS
-
-
-# FIXME: this is to get around the fact that we don't have a
-# proper context object in the IR generation phase.
-@contextlib.contextmanager
-def anchor_opt_level(new_level: OptimizationLevel) -> Generator:
-    """
-    Set the global optimization level variable for the duration of this
-    context manager.
-    """
-    assert isinstance(new_level, OptimizationLevel)
-
-    global _opt_level
-    try:
-        tmp = _opt_level
-        _opt_level = new_level
-        yield
-    finally:
-        _opt_level = tmp
-
-
-def _opt_codesize():
-    return _opt_level == OptimizationLevel.CODESIZE
-
-
-def _opt_gas():
-    return _opt_level == OptimizationLevel.GAS
-
-
-def _opt_none():
-    return _opt_level == OptimizationLevel.NONE
-
-
 def _complex_make_setter(left, right):
     if right.value == "~empty" and left.location == MEMORY:
         # optimized memzero
         return mzero(left, left.typ.memory_bytes_required)
 
     ret = ["seq"]
```

### Comparing `vyper-0.4.0b6/vyper/codegen/events.py` & `vyper-0.4.0rc1/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/expr.py` & `vyper-0.4.0rc1/vyper/codegen/expr.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/external_call.py` & `vyper-0.4.0rc1/vyper/codegen/external_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/function_definitions/common.py` & `vyper-0.4.0rc1/vyper/codegen/function_definitions/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/function_definitions/external_function.py` & `vyper-0.4.0rc1/vyper/codegen/function_definitions/external_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.4.0rc1/vyper/codegen/function_definitions/internal_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/ir_node.py` & `vyper-0.4.0rc1/vyper/codegen/ir_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/jumptable_utils.py` & `vyper-0.4.0rc1/vyper/codegen/jumptable_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/keccak256_helper.py` & `vyper-0.4.0rc1/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/memory_allocator.py` & `vyper-0.4.0rc1/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/module.py` & `vyper-0.4.0rc1/vyper/codegen/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/return_.py` & `vyper-0.4.0rc1/vyper/codegen/return_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/self_call.py` & `vyper-0.4.0rc1/vyper/codegen/self_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/codegen/stmt.py` & `vyper-0.4.0rc1/vyper/codegen/stmt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/compiler/README.md` & `vyper-0.4.0rc1/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/compiler/__init__.py` & `vyper-0.4.0rc1/vyper/compiler/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from typing import Any, Callable, Dict, Optional, Sequence, Union
 
 import vyper.ast as vy_ast  # break an import cycle
 import vyper.codegen.core as codegen
 import vyper.compiler.output as output
 from vyper.compiler.input_bundle import FileInput, InputBundle, PathLike
 from vyper.compiler.phases import CompilerData
-from vyper.compiler.settings import Settings
-from vyper.evm.opcodes import anchor_evm_version
+from vyper.compiler.settings import Settings, anchor_settings
 from vyper.typing import ContractPath, OutputFormats, StorageLayout
 
 OUTPUT_FORMATS = {
     # requires vyper_module
     "ast_dict": output.build_ast_dict,
     # requires annotated_vyper_module
     "annotated_ast_dict": output.build_annotated_ast_dict,
@@ -92,15 +91,14 @@
         Use experimental codegen. Defaults to False
 
     Returns
     -------
     Dict
         Compiler output as `{'output key': "output data"}`
     """
-
     settings = settings or Settings()
 
     if output_formats is None:
         output_formats = ("bytecode",)
 
     # make IR output the same between runs
     codegen.reset_names()
@@ -113,15 +111,15 @@
         settings,
         storage_layout_override,
         show_gas_estimates,
         no_bytecode_metadata,
     )
 
     ret = {}
-    with anchor_evm_version(compiler_data.settings.evm_version):
+    with anchor_settings(compiler_data.settings):
         for output_format in output_formats:
             if output_format not in OUTPUT_FORMATS:
                 raise ValueError(f"Unsupported format type {repr(output_format)}")
             try:
                 formatter = OUTPUT_FORMATS[output_format]
                 ret[output_format] = formatter(compiler_data)
             except Exception as exc:
```

### Comparing `vyper-0.4.0b6/vyper/compiler/input_bundle.py` & `vyper-0.4.0rc1/vyper/compiler/input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/compiler/output.py` & `vyper-0.4.0rc1/vyper/compiler/output.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/compiler/phases.py` & `vyper-0.4.0rc1/vyper/compiler/phases.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import warnings
 from functools import cached_property
 from pathlib import Path, PurePath
 from typing import Optional
 
 from vyper import ast as vy_ast
 from vyper.codegen import module
-from vyper.codegen.core import anchor_opt_level
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.input_bundle import FileInput, FilesystemInputBundle, InputBundle
-from vyper.compiler.settings import OptimizationLevel, Settings
+from vyper.compiler.settings import OptimizationLevel, Settings, anchor_settings
 from vyper.exceptions import StructureException
 from vyper.ir import compile_ir, optimizer
 from vyper.semantics import analyze_module, set_data_positions, validate_compilation_target
 from vyper.semantics.types.function import ContractFunctionT
 from vyper.semantics.types.module import ModuleT
 from vyper.typing import StorageLayout
 from vyper.utils import ERC5202_PREFIX
@@ -34,14 +33,15 @@
 def _merge_settings(cli: Settings, pragma: Settings):
     ret = Settings()
     ret.evm_version = _merge_one(cli.evm_version, pragma.evm_version, "evm version")
     ret.optimize = _merge_one(cli.optimize, pragma.optimize, "optimize")
     ret.experimental_codegen = _merge_one(
         cli.experimental_codegen, pragma.experimental_codegen, "experimental codegen"
     )
+    ret.enable_decimals = _merge_one(cli.enable_decimals, pragma.enable_decimals, "enable-decimals")
 
     return ret
 
 
 class CompilerData:
     """
     Object for fetching and storing compiler data for a Vyper contract.
@@ -174,15 +174,15 @@
         # ensure storage layout is computed
         _ = self.storage_layout
         return self.annotated_vyper_module._metadata["type"]
 
     @cached_property
     def _ir_output(self):
         # fetch both deployment and runtime IR
-        return generate_ir_nodes(self.global_ctx, self.settings.optimize)
+        return generate_ir_nodes(self.global_ctx, self.settings)
 
     @property
     def ir_nodes(self) -> IRnode:
         ir, ir_runtime = self._ir_output
         return ir
 
     @property
@@ -264,15 +264,15 @@
     with input_bundle.search_path(Path(vyper_module.resolved_path).parent):
         # note: analyze_module does type inference on the AST
         analyze_module(vyper_module, input_bundle)
 
     return vyper_module
 
 
-def generate_ir_nodes(global_ctx: ModuleT, optimize: OptimizationLevel) -> tuple[IRnode, IRnode]:
+def generate_ir_nodes(global_ctx: ModuleT, settings: Settings) -> tuple[IRnode, IRnode]:
     """
     Generate the intermediate representation (IR) from the contextualized AST.
 
     This phase also includes IR-level optimizations.
 
     This function returns three values: deployment bytecode, runtime bytecode
     and the function signatures of the contract
@@ -284,17 +284,17 @@
 
     Returns
     -------
     (IRnode, IRnode)
         IR to generate deployment bytecode
         IR to generate runtime bytecode
     """
-    with anchor_opt_level(optimize):
+    with anchor_settings(settings):
         ir_nodes, ir_runtime = module.generate_ir_for_module(global_ctx)
-    if optimize != OptimizationLevel.NONE:
+    if settings.optimize != OptimizationLevel.NONE:
         ir_nodes = optimizer.optimize(ir_nodes)
         ir_runtime = optimizer.optimize(ir_runtime)
     return ir_nodes, ir_runtime
 
 
 def generate_assembly(ir_nodes: IRnode, optimize: Optional[OptimizationLevel] = None) -> list:
     """
```

### Comparing `vyper-0.4.0b6/vyper/compiler/utils.py` & `vyper-0.4.0rc1/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/evm/address_space.py` & `vyper-0.4.0rc1/vyper/evm/address_space.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/evm/opcodes.py` & `vyper-0.4.0rc1/vyper/evm/opcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-import contextlib
-from typing import Dict, Generator, Optional
+from typing import Dict, Optional
 
+from vyper.compiler.settings import get_global_settings
 from vyper.exceptions import CompilerPanic
 from vyper.typing import OpcodeGasCost, OpcodeMap, OpcodeRulesetMap, OpcodeRulesetValue, OpcodeValue
 
 # EVM version rules work as follows:
 # 1. Fork rules go from oldest (lowest value) to newest (highest value).
 # 2. Fork versions aren't actually tied to anything. They are not a part of our
 #    official API. *DO NOT USE THE VALUES FOR ANYTHING IMPORTANT* besides versioning.
 # 3. Per VIP-3365, we support mainnet fork choice rules up to 3 years old
 #    (and may optionally have forward support for experimental/unreleased
 #    fork choice rules)
 _evm_versions = ("london", "paris", "shanghai", "cancun")
 EVM_VERSIONS: dict[str, int] = dict((v, i) for i, v in enumerate(_evm_versions))
 
-
-DEFAULT_EVM_VERSION: str = "shanghai"
-active_evm_version: int = EVM_VERSIONS[DEFAULT_EVM_VERSION]
+DEFAULT_EVM_VERSION = "shanghai"
 
 
 # opcode as hex value
 # number of values removed from stack
 # number of values added to stack
 # gas cost (london, paris, shanghai, cancun)
 OPCODES: OpcodeMap = {
@@ -204,26 +202,14 @@
     "DLOAD": (None, 1, 1, 9),
     "DLOADBYTES": (None, 3, 0, 3),
 }
 
 IR_OPCODES: OpcodeMap = {**OPCODES, **PSEUDO_OPCODES}
 
 
-@contextlib.contextmanager
-def anchor_evm_version(evm_version: Optional[str] = None) -> Generator:
-    global active_evm_version
-    anchor = active_evm_version
-    evm_version = evm_version or DEFAULT_EVM_VERSION
-    active_evm_version = EVM_VERSIONS[evm_version]
-    try:
-        yield
-    finally:
-        active_evm_version = anchor
-
-
 def _gas(value: OpcodeValue, idx: int) -> Optional[OpcodeRulesetValue]:
     gas: OpcodeGasCost = value[3]
     if isinstance(gas, int):
         return value[:3] + (gas,)
     if len(gas) <= idx:
         return value[:3] + (gas[-1],)
     if gas[idx] is None:
@@ -241,23 +227,31 @@
     v: _mk_version_opcodes(OPCODES, v) for v in EVM_VERSIONS.values()
 }
 _ir_opcodes: Dict[int, OpcodeRulesetMap] = {
     v: _mk_version_opcodes(IR_OPCODES, v) for v in EVM_VERSIONS.values()
 }
 
 
+def get_active_evm_version():
+    settings = get_global_settings()
+    evm_version_str = settings and settings.evm_version or DEFAULT_EVM_VERSION
+    return EVM_VERSIONS[evm_version_str]
+
+
 def get_opcodes() -> OpcodeRulesetMap:
-    return _evm_opcodes[active_evm_version]
+    return _evm_opcodes[get_active_evm_version()]
 
 
 def get_ir_opcodes() -> OpcodeRulesetMap:
-    return _ir_opcodes[active_evm_version]
+    return _ir_opcodes[get_active_evm_version()]
 
 
 def version_check(begin: Optional[str] = None, end: Optional[str] = None) -> bool:
+    active_evm_version = get_active_evm_version()
+
     if begin is None and end is None:
         raise CompilerPanic("Either beginning or end fork ruleset must be set.")
     if begin is None:
         begin_idx = min(EVM_VERSIONS.values())
     else:
         begin_idx = EVM_VERSIONS[begin]
     end_idx = max(EVM_VERSIONS.values()) if end is None else EVM_VERSIONS[end]
```

### Comparing `vyper-0.4.0b6/vyper/exceptions.py` & `vyper-0.4.0rc1/vyper/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     """Invalid structure for parsable syntax."""
 
 
 class InstantiationException(StructureException):
     """Variable or expression cannot be instantiated"""
 
 
-class VersionException(VyperException):
+class VersionException(SyntaxException):
     """Version string is malformed or incompatible with this compiler version."""
 
 
 class VariableDeclarationException(VyperException):
     """Invalid variable declaration."""
 
 
@@ -350,14 +350,18 @@
     """Contract source cannot be parsed."""
 
 
 class UnimplementedException(VyperException):
     """Some feature is known to be not implemented"""
 
 
+class FeatureException(VyperException):
+    """Some feature flag is not enabled"""
+
+
 class StaticAssertionException(VyperException):
     """An assertion is proven to fail at compile-time."""
 
 
 class VyperInternalException(_BaseVyperException):
     """
     Base Vyper internal exception class.
```

### Comparing `vyper-0.4.0b6/vyper/ir/README.md` & `vyper-0.4.0rc1/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ir/compile_ir.py` & `vyper-0.4.0rc1/vyper/ir/compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ir/optimizer.py` & `vyper-0.4.0rc1/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/ir/s_expressions.py` & `vyper-0.4.0rc1/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/README.md` & `vyper-0.4.0rc1/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/base.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/common.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/constant_folding.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/constant_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/data_positions.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/data_positions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/getters.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/global_.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/global_.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,20 @@
 
     err_list = ExceptionList()
 
     for u, uses in all_used_modules.items():
         if u not in all_initialized_modules:
             found_module = module_t.find_module_info(u)
             if found_module is not None:
-                hint = f"add `initializes: {found_module.alias}` to the top level of "
-                hint += "your main contract"
+                # TODO: do something about these constants
+                if str(module_t) in ("<unknown>", "VyperContract.vy"):
+                    module_str = "the top level of your main contract"
+                else:
+                    module_str = f"`{module_t}`"
+                hint = f"add `initializes: {found_module.alias}` to {module_str}"
             else:
                 # CMC 2024-02-06 is this actually reachable?
                 hint = f"ensure `{module_t}` is imported in your main contract!"
             err_list.append(
                 InitializerException(
                     f"module `{u}` is used but never initialized!", *uses, hint=hint
                 )
```

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/import_graph.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/import_graph.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/local.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/local.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     StateAccessViolation,
     StructureException,
     TypeCheckFailure,
     TypeMismatch,
     VariableDeclarationException,
     VyperException,
 )
+
+# TODO consolidate some of these imports
 from vyper.semantics.analysis.base import (
     Modifiability,
     ModuleInfo,
     ModuleOwnership,
     VarAccess,
     VarInfo,
 )
@@ -32,16 +34,14 @@
     get_common_types,
     get_exact_type_from_node,
     get_expr_info,
     get_possible_types_from_node,
     validate_expected_type,
 )
 from vyper.semantics.data_locations import DataLocation
-
-# TODO consolidate some of these imports
 from vyper.semantics.environment import CONSTANT_ENVIRONMENT_VARS
 from vyper.semantics.namespace import get_namespace
 from vyper.semantics.types import (
     TYPE_T,
     VOID_TYPE,
     AddressT,
     BoolT,
```

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/module.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,21 @@
 
         if len(should_initialize) > 0:
             err_list = ExceptionList()
             for s in should_initialize.values():
                 msg = "not initialized!"
                 hint = f"add `{s.module_info.alias}.__init__()` to "
                 hint += "your `__init__()` function"
-                err_list.append(InitializerException(msg, s.node, hint=hint))
+
+                # grab the init function AST node for error message
+                # (it could be None, it's ok since it's just for diagnostics)
+                init_func_node = None
+                if module_t.init_function:
+                    init_func_node = module_t.init_function.decl_node
+                err_list.append(InitializerException(msg, init_func_node, s.node, hint=hint))
 
             err_list.raise_if_not_empty()
 
     def _ast_from_file(self, file: FileInput) -> vy_ast.Module:
         # cache ast if we have seen it before.
         # this gives us the additional property of object equality on
         # two ASTs produced from the same source
@@ -433,16 +439,18 @@
             module_info.set_ownership(ModuleOwnership.USES, item)
 
             used_modules.append(module_info)
 
         node._metadata["uses_info"] = UsesInfo(used_modules, node)
 
     def visit_InitializesDecl(self, node):
-        module_ref = node.annotation
+        annotation = node.annotation
+
         dependencies_ast = ()
+        module_ref = annotation
         if isinstance(module_ref, vy_ast.Subscript):
             dependencies_ast = vy_ast.as_tuple(module_ref.slice)
             module_ref = module_ref.value
 
         # postcondition of InitializesDecl.validates()
         assert isinstance(module_ref, (vy_ast.Name, vy_ast.Attribute))
 
@@ -492,15 +500,31 @@
 
             del used_modules[lhs_module.module_t]
 
         if len(used_modules) > 0:
             item = next(iter(used_modules.values()))  # just pick one
             msg = f"`{module_info.alias}` uses `{item.alias}`, but it is not "
             msg += f"initialized with `{item.alias}`"
-            hint = f"add `{item.alias}` to its initializer list"
+
+            lhs = item.alias
+            rhs = None
+            # find the alias of the uninitialized module in this contract
+            # to fill out the error message with.
+            for k, v in self.namespace.items():
+                if isinstance(v, ModuleInfo) and v.module_t == item.module_t:
+                    rhs = k
+                    break
+
+            if rhs is None:
+                hint = f"try importing {item.alias} first"
+            elif not isinstance(annotation, vy_ast.Subscript):
+                # it's `initializes: foo` instead of `initializes: foo[...]`
+                hint = f"did you mean {module_ref.id}[{lhs} := {rhs}]?"
+            else:
+                hint = f"add `{lhs} := {rhs}` to its initializer list"
             raise InitializerException(msg, node, hint=hint)
 
         # note: try to refactor. not a huge fan of mutating the
         # ModuleInfo after it's constructed
         module_info.set_ownership(ModuleOwnership.INITIALIZES, node)
         node._metadata["initializes_info"] = InitializesInfo(module_info, dependencies, node)
```

### Comparing `vyper-0.4.0b6/vyper/semantics/analysis/utils.py` & `vyper-0.4.0rc1/vyper/semantics/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/environment.py` & `vyper-0.4.0rc1/vyper/semantics/environment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/namespace.py` & `vyper-0.4.0rc1/vyper/semantics/namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/__init__.py` & `vyper-0.4.0rc1/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/base.py` & `vyper-0.4.0rc1/vyper/semantics/types/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     @property
     def canonical_abi_type(self) -> str:
         """
         The canonical name of this type. Used for ABI types and generating function signatures.
         """
         return self.abi_type.selector_name()
 
-    def to_abi_arg(self, name: str = "") -> Dict[str, Any]:
+    def to_abi_arg(self, name: str = "") -> dict[str, Any]:
         """
         The JSON ABI description of this type. Note for complex types,
         the implementation is overridden to be compliant with the spec:
         https://docs.soliditylang.org/en/v0.8.14/abi-spec.html#json
         > An object with members name, type and potentially components
           describes a typed variable. The canonical type is determined
           until a tuple type is reached and the string description up to
```

### Comparing `vyper-0.4.0b6/vyper/semantics/types/bytestrings.py` & `vyper-0.4.0rc1/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/function.py` & `vyper-0.4.0rc1/vyper/semantics/types/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/module.py` & `vyper-0.4.0rc1/vyper/semantics/types/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/primitives.py` & `vyper-0.4.0rc1/vyper/semantics/types/primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # primitive types which occupy one word, like ints and addresses
 
 from decimal import Decimal
 from functools import cached_property
-from typing import Tuple, Union
+from typing import Any, Tuple, Union
 
 from vyper import ast as vy_ast
-from vyper.abi_types import ABI_Address, ABI_Bool, ABI_BytesM, ABI_FixedMxN, ABI_GIntM, ABIType
+from vyper.abi_types import ABI_Address, ABI_Bool, ABI_BytesM, ABI_GIntM, ABIType
 from vyper.exceptions import (
     CompilerPanic,
     InvalidLiteral,
     InvalidOperation,
     OverflowException,
     VyperException,
 )
@@ -335,15 +335,15 @@
         try:
             super().validate_numeric_op(node)
         except VyperException as e:
             raise _add_div_hint(node, e) from None
 
     @cached_property
     def abi_type(self) -> ABIType:
-        return ABI_FixedMxN(self._bits, self._decimal_places, self._is_signed)
+        return ABI_GIntM(self._bits, self._is_signed)
 
     @cached_property
     def decimals(self) -> int:
         # Alias for API compatibility with codegen
         return self._decimal_places
 
     @cached_property
@@ -360,14 +360,19 @@
 
     @cached_property
     def decimal_bounds(self) -> Tuple[Decimal, Decimal]:
         lo, hi = int_bounds(signed=self.is_signed, bits=self.bits)
         DIVISOR = Decimal(self.divisor)
         return lo / DIVISOR, hi / DIVISOR
 
+    def to_abi_arg(self, name: str = "") -> dict[str, Any]:
+        ret = super().to_abi_arg(name)
+        ret["internalType"] = repr(self)
+        return ret
+
 
 # maybe this even deserves its own module, address.py
 # should inherit from uint160?
 class AddressT(_PrimT):
     _id = "address"
     _valid_literal = (vy_ast.Hex,)
     _type_members = {
```

### Comparing `vyper-0.4.0b6/vyper/semantics/types/subscriptable.py` & `vyper-0.4.0rc1/vyper/semantics/types/subscriptable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/user.py` & `vyper-0.4.0rc1/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/semantics/types/utils.py` & `vyper-0.4.0rc1/vyper/semantics/types/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Dict
-
 from vyper import ast as vy_ast
+from vyper.compiler.settings import get_global_settings
 from vyper.exceptions import (
     ArrayIndexException,
     CompilerPanic,
+    FeatureException,
     InstantiationException,
     InvalidType,
     StructureException,
     UndeclaredDefinition,
     UnknownType,
 )
 from vyper.semantics.analysis.levenshtein_utils import get_levenshtein_error_suggestions
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.namespace import get_namespace
 from vyper.semantics.types.base import TYPE_T, VyperType
 
 # TODO maybe this should be merged with .types/base.py
 
 
-def type_from_abi(abi_type: Dict) -> VyperType:
+def type_from_abi(abi_type: dict) -> VyperType:
     """
     Return a type object from an ABI type definition.
 
     Arguments
     ---------
-    abi_type : Dict
+    abi_type : dict
        A type definition taken from the `input` or `output` field of an ABI.
 
     Returns
     -------
     BaseTypeDefinition
         Type definition object.
     """
     type_string = abi_type["type"]
-    if type_string == "fixed168x10":
+    if type_string == "int168" and abi_type.get("internalType") == "decimal":
         type_string = "decimal"
     if type_string in ("string", "bytes"):
         type_string = type_string.capitalize()
 
     namespace = get_namespace()
 
     if "[" in type_string:
@@ -81,21 +81,30 @@
         Vyper ast node from the `annotation` member of a `VariableDecl` or `AnnAssign` node.
 
     Returns
     -------
     VyperType
         Type definition object.
     """
-    typ_ = _type_from_annotation(node)
+    typ = _type_from_annotation(node)
 
-    if location in typ_._invalid_locations:
+    if location in typ._invalid_locations:
         location_str = "" if location is DataLocation.UNSET else f"in {location.name.lower()}"
-        raise InstantiationException(f"{typ_} is not instantiable {location_str}", node)
+        raise InstantiationException(f"{typ} is not instantiable {location_str}", node)
+
+    # TODO: cursed import cycle!
+    from vyper.semantics.types.primitives import DecimalT
+
+    if isinstance(typ, DecimalT):
+        # is there a better place to put this check?
+        settings = get_global_settings()
+        if settings and not settings.get_enable_decimals():
+            raise FeatureException("decimals are not allowed unless `--enable-decimals` is set")
 
-    return typ_
+    return typ
 
 
 def _type_from_annotation(node: vy_ast.VyperNode) -> VyperType:
     namespace = get_namespace()
 
     if isinstance(node, vy_ast.Tuple):
         tuple_t = namespace["$TupleT"]
```

### Comparing `vyper-0.4.0b6/vyper/utils.py` & `vyper-0.4.0rc1/vyper/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/README.md` & `vyper-0.4.0rc1/vyper/venom/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/__init__.py` & `vyper-0.4.0rc1/vyper/venom/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/analysis.py` & `vyper-0.4.0rc1/vyper/venom/analysis.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/basicblock.py` & `vyper-0.4.0rc1/vyper/venom/basicblock.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,98 +88,75 @@
     def __repr__(self) -> str:
         src = self.src if self.src else ""
         return f"\t# line {self.line_no}: {src}".expandtabs(20)
 
 
 class IROperand:
     """
-    IROperand represents an operand in IR. An operand is anything that can
-    be an argument to an IRInstruction
+    IROperand represents an IR operand. An operand is anything that can be
+    operated by instructions. It can be a literal, a variable, or a label.
     """
 
     value: Any
 
     @property
     def name(self) -> str:
         return self.value
 
+    def __hash__(self) -> int:
+        return hash(self.value)
 
-class IRValue(IROperand):
-    """
-    IRValue represents a value in IR. A value is anything that can be
-    operated by non-control flow instructions. That is, IRValues can be
-    IRVariables or IRLiterals.
-    """
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self.value == other.value
 
-    pass
+    def __repr__(self) -> str:
+        return str(self.value)
 
 
-class IRLiteral(IRValue):
+class IRLiteral(IROperand):
     """
     IRLiteral represents a literal in IR
     """
 
     value: int
 
     def __init__(self, value: int) -> None:
         assert isinstance(value, int), "value must be an int"
         self.value = value
 
-    def __hash__(self) -> int:
-        return self.value.__hash__()
-
-    def __eq__(self, other) -> bool:
-        if not isinstance(other, type(self)):
-            return False
-        return self.value == other.value
-
-    def __repr__(self) -> str:
-        return str(self.value)
-
 
-class IRVariable(IRValue):
+class IRVariable(IROperand):
     """
     IRVariable represents a variable in IR. A variable is a string that starts with a %.
     """
 
     value: str
-    offset: int = 0
 
     def __init__(self, value: str, version: Optional[str | int] = None) -> None:
         assert isinstance(value, str)
         assert ":" not in value, "Variable name cannot contain ':'"
         if version:
             assert isinstance(value, str) or isinstance(value, int), "value must be an str or int"
             value = f"{value}:{version}"
         if value[0] != "%":
             value = f"%{value}"
         self.value = value
-        self.offset = 0
 
     @property
     def name(self) -> str:
         return self.value.split(":")[0]
 
     @property
     def version(self) -> int:
         if ":" not in self.value:
             return 0
         return int(self.value.split(":")[1])
 
-    def __hash__(self) -> int:
-        return self.value.__hash__()
-
-    def __eq__(self, other) -> bool:
-        if not isinstance(other, type(self)):
-            return False
-        return self.value == other.value
-
-    def __repr__(self) -> str:
-        return self.value
-
 
 class IRLabel(IROperand):
     """
     IRLabel represents a label in IR. A label is a string that starts with a %.
     """
 
     # is_symbol is used to indicate if the label came from upstream
@@ -188,24 +165,22 @@
     value: str
 
     def __init__(self, value: str, is_symbol: bool = False) -> None:
         assert isinstance(value, str), "value must be an str"
         self.value = value
         self.is_symbol = is_symbol
 
-    def __hash__(self) -> int:
-        return hash(self.value)
-
-    def __eq__(self, other) -> bool:
-        if not isinstance(other, type(self)):
-            return False
-        return self.value == other.value
-
-    def __repr__(self) -> str:
-        return self.value
+    def __eq__(self, other):
+        # no need for is_symbol to participate in equality
+        return super().__eq__(other)
+
+    def __hash__(self):
+        # __hash__ is required when __eq__ is overridden --
+        # https://docs.python.org/3/reference/datamodel.html#object.__hash__
+        return super().__hash__()
 
 
 class IRInstruction:
     """
     IRInstruction represents an instruction in IR. Each instruction has an opcode,
     operands, and return value. For example, the following IR instruction:
         %1 = add %0, 1
```

### Comparing `vyper-0.4.0b6/vyper/venom/bb_optimizer.py` & `vyper-0.4.0rc1/vyper/venom/bb_optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/dominators.py` & `vyper-0.4.0rc1/vyper/venom/dominators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/function.py` & `vyper-0.4.0rc1/vyper/venom/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/ir_node_to_venom.py` & `vyper-0.4.0rc1/vyper/venom/ir_node_to_venom.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/passes/base_pass.py` & `vyper-0.4.0rc1/vyper/venom/passes/base_pass.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/passes/dft.py` & `vyper-0.4.0rc1/vyper/venom/passes/dft.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/passes/make_ssa.py` & `vyper-0.4.0rc1/vyper/venom/passes/make_ssa.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         """
         Rename variables. This follows the placement of phi nodes.
         """
         outs = []
 
         # Pre-action
         for inst in basic_block.instructions:
-            new_ops = []
+            new_ops: list[IROperand] = []
             if inst.opcode != "phi":
                 for op in inst.operands:
                     if not isinstance(op, IRVariable):
                         new_ops.append(op)
                         continue
 
                     new_ops.append(IRVariable(op.name, version=self.var_name_stacks[op.name][-1]))
@@ -139,15 +139,15 @@
             self.var_name_stacks[op_name].pop()
 
     def _remove_degenerate_phis(self, entry: IRBasicBlock):
         for inst in entry.instructions.copy():
             if inst.opcode != "phi":
                 continue
 
-            new_ops = []
+            new_ops: list[IROperand] = []
             for label, op in inst.phi_operands:
                 if op == inst.output:
                     continue
                 new_ops.extend([label, op])
             new_ops_len = len(new_ops)
             if new_ops_len == 0:
                 entry.instructions.remove(inst)
```

### Comparing `vyper-0.4.0b6/vyper/venom/passes/normalization.py` & `vyper-0.4.0rc1/vyper/venom/passes/normalization.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/passes/simplify_cfg.py` & `vyper-0.4.0rc1/vyper/venom/passes/simplify_cfg.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/passes/stack_reorder.py` & `vyper-0.4.0rc1/vyper/venom/passes/stack_reorder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/stack_model.py` & `vyper-0.4.0rc1/vyper/venom/stack_model.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper/venom/venom_to_assembly.py` & `vyper-0.4.0rc1/vyper/venom/venom_to_assembly.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper.egg-info/PKG-INFO` & `vyper-0.4.0rc1/vyper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0b6
+Version: 0.4.0rc1
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0b6/vyper.egg-info/SOURCES.txt` & `vyper-0.4.0rc1/vyper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b6/vyper.egg-info/requires.txt` & `vyper-0.4.0rc1/vyper.egg-info/requires.txt`

 * *Files identical despite different names*

