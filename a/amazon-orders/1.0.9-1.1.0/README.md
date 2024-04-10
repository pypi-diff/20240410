# Comparing `tmp/amazon-orders-1.0.9.tar.gz` & `tmp/amazon-orders-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-orders-1.0.9.tar", last modified: Wed Feb  7 21:57:18 2024, max compression
+gzip compressed data, was "amazon-orders-1.1.0.tar", last modified: Wed Apr 10 03:25:31 2024, max compression
```

## Comparing `amazon-orders-1.0.9.tar` & `amazon-orders-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.517719 amazon-orders-1.0.9/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.525720 amazon-orders-1.0.9/_build/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)    33058 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/coverage.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21865 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac___init___py.html
--rw-r--r--   0 runner    (1001) docker     (127)    75041 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_cli_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_conf_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    36477 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_constants_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_exception_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    79221 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_forms_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    34680 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_orders_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    81484 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_52b119045e3ef7ac_session_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879___init___py.html
--rw-r--r--   0 runner    (1001) docker     (127)    33844 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879_item_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    93973 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879_order_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    36386 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879_parsable_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879_recipient_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879_seller_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    19291 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/d_776673663093f879_shipment_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/status.json
--rw-r--r--   0 runner    (1001) docker     (127)    12406 2024-02-07 21:56:46.000000 amazon-orders-1.0.9/_build/coverage/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/amazon_orders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-02-07 21:57:18.000000 amazon-orders-1.0.9/amazon_orders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-07 21:57:18.000000 amazon-orders-1.0.9/amazon_orders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 21:57:18.000000 amazon-orders-1.0.9/amazon_orders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 21:57:18.000000 amazon-orders-1.0.9/amazon_orders.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 21:57:18.000000 amazon-orders-1.0.9/amazon_orders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-07 21:57:18.000000 amazon-orders-1.0.9/amazon_orders.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/amazonorders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/amazonorders/entity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/parsable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/seller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/entity/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/amazonorders/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 21:57:18.529719 amazon-orders-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/test_integration_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/test_integration_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-02-07 21:55:57.000000 amazon-orders-1.0.9/tests/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:25:31.051730 amazon-orders-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-10 03:25:31.051730 amazon-orders-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:25:31.047730 amazon-orders-1.1.0/amazon_orders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-10 03:25:31.000000 amazon-orders-1.1.0/amazon_orders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 03:25:31.000000 amazon-orders-1.1.0/amazon_orders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:25:31.000000 amazon-orders-1.1.0/amazon_orders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 03:25:31.000000 amazon-orders-1.1.0/amazon_orders.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-10 03:25:31.000000 amazon-orders-1.1.0/amazon_orders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 03:25:31.000000 amazon-orders-1.1.0/amazon_orders.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:25:31.047730 amazon-orders-1.1.0/amazonorders/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/banner.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:25:31.047730 amazon-orders-1.1.0/amazonorders/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/parsable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/seller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/entity/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/amazonorders/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:25:31.051730 amazon-orders-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:25:31.047730 amazon-orders-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/tests/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-04-10 03:24:47.000000 amazon-orders-1.1.0/tests/testcase.py
```

### Comparing `amazon-orders-1.0.9/CHANGELOG.md` & `amazon-orders-1.1.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,144 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased](https://github.com/alexdlaird/amazon-orders-python/compare/1.0.9...HEAD)
+## [Unreleased](https://github.com/alexdlaird/amazon-orders/compare/1.1.0...HEAD)
 
-## [1.0.9](https://github.com/alexdlaird/pyngrok/compare/1.0.8...1.0.9) - 2024-02-07
+## [1.1.0](https://github.com/alexdlaird/amazon-orders/compare/1.0.16...1.1.0) - 2024-04-09
+### Added
+- Build improvements.
+- Test improvements.
+
+### Changed
+- Renamed `kwarg` passed to `IODefault.prompt()` from `captcha_img_url` to `img_url`.
+- Renamed `kwarg` passed to `IODefault.prompt()` from `mfa_device_select_choices` to `choices`.
+
+## [1.0.16](https://github.com/alexdlaird/amazon-orders/compare/1.0.15...1.0.16) - 2024-03-24
+### Added
+- `constants.BASE_URL` will look for the environment variable `AMAZON_BASE_URL` before defaulting to "https://www.amazon.com".
+- Build and stability improvements.
+
+## [1.0.15](https://github.com/alexdlaird/amazon-orders/compare/1.0.14...1.0.15) - 2024-03-05
+### Added
+- Build and style improvements.
+- Documentation improvements.
+- `pytest` to streamline running unit and integration tests.
+
+### Removed
+- `conf.VERSION`, moved all version information to `amazonorders/__init__.py`. Get package version with `from amazonorders import __version__` instead.
+
+## [1.0.14](https://github.com/alexdlaird/amazon-orders/compare/1.0.13...1.0.14) - 2024-02-26
+### Added
+- Build improvements.
+
+### Changed
+- Renamed `make check-style` to `make check`.
+
+## [1.0.13](https://github.com/alexdlaird/amazon-orders/compare/1.0.12...1.0.13) - 2024-02-20
+### Added
+- `login` command to CLI.
+- If `--username` or `--password` are not given and no stored session, CLI will prompt.
+- Build improvements.
+
+### Fixed
+- Issue where `Parsable` objects could not be pickled due to BeautifulSoup `Tag` objects.
+
+## [1.0.12](https://github.com/alexdlaird/amazon-orders/compare/1.0.11...1.0.12) - 2024-02-11
+### Added
+- Relative dependency pinning in `pyproject.toml`.
+- Style and stability improvements (check `flake8` with `make check-style`).
+
+### Removed
+- `requirements.txt` files to streamline in to `pyproject.toml`.
+
+## [1.0.11](https://github.com/alexdlaird/amazon-orders/compare/1.0.10...1.0.11) - 2024-02-09
+### Changed
+- `version` command now includes Python version and doesn't printer banner, for easy parsing.
+
+## [1.0.10](https://github.com/alexdlaird/amazon-orders/compare/1.0.9...1.0.10) - 2024-02-08
+### Added
+- Migrated to `pyproject.toml`.
+
+## [1.0.9](https://github.com/alexdlaird/amazon-orders/compare/1.0.8...1.0.9) - 2024-02-07
 ### Added
 - [AuthForm](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.forms.AuthForm)'s now passes `captcha_img_url` to its `prompt()` fallback for Captcha, useful for overriding [IODefault](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.session.IODefault).
 - [MfaDeviceSelectForm](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.forms.MfaDeviceSelectForm) now passes `mfa_device_select_choices` to `prompt()`, useful for overrides [IODefault](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.session.IODefault).
 - Documentation improvements.
 
-## [1.0.8](https://github.com/alexdlaird/pyngrok/compare/1.0.7...1.0.8) - 2024-01-30
+## [1.0.8](https://github.com/alexdlaird/amazon-orders/compare/1.0.7...1.0.8) - 2024-01-30
 ### Added
 - Stability improvements.
 
-## [1.0.7](https://github.com/alexdlaird/pyngrok/compare/1.0.6...1.0.7) - 2024-01-29
+## [1.0.7](https://github.com/alexdlaird/amazon-orders/compare/1.0.6...1.0.7) - 2024-01-29
 ### Added
 - [AuthForm](https://amazon-orders.readthedocs.io/en/1.0.7/api.html#amazonorders.forms.AuthForm) abstract class, and migrated all auth flow items to subclasses of this class.
 - [Parsable.simple_parse()](https://amazon-orders.readthedocs.io/en/1.0.7/api.html#amazonorders.entities.parsable.Parsable.simple_parse), which can handle most basic fields when parised with CSS selectors.
 - Stability improvements.
 - Test improvements.
 
 ### Changed
 - Moved all constant variables (URLs, CSS selectors, etc.) to `constants.py`.
 - Migrated entities to use CSS selector constants.
 - `constants.SIGN_IN_URL` is now the landing page for login, the old value has been moved to `constants.SIGN_IN_REDIRECT_URL`.
 
-## [1.0.6](https://github.com/alexdlaird/pyngrok/compare/1.0.5...1.0.6) - 2024-01-25
+## [1.0.6](https://github.com/alexdlaird/amazon-orders/compare/1.0.5...1.0.6) - 2024-01-25
 ### Added
 - Support for when local session data is stale (Amazon prompts us to login again).
 - Documentation improvements.
 
 ### Fixed
 - Regression in the Captcha flow introduced in `1.0.5`.
 
-## [1.0.5](https://github.com/alexdlaird/pyngrok/compare/1.0.4...1.0.5) - 2024-01-25
+## [1.0.5](https://github.com/alexdlaird/amazon-orders/compare/1.0.4...1.0.5) - 2024-01-25
 ### Added
 - [Item.image_link](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.entity.item.Item.image_link).
 - [Item.quantity](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.entity.item.Item.quantity).
 - `version` command to CLI.
 - Test improvements.
 
 ### Changed
 - Migrated to using CSS selectors in [`AmazonSession`](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.session.AmazonSession)
 - Migrated to using CSS selectors in [`AmazonOrders`](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.orders.AmazonOrders)
 
-## [1.0.4](https://github.com/alexdlaird/pyngrok/compare/1.0.3...1.0.4) - 2024-01-24
+## [1.0.4](https://github.com/alexdlaird/amazon-orders/compare/1.0.3...1.0.4) - 2024-01-24
 ### Added
 - A new OTP auth flow from Amazon that can occur after Captcha.
 - Parameters `--max-auth-attempts` and `--output-dir` to CLI.
 - `DEFAULT_OUTPUT_DIR`, which defaults to `os.getcwd()`, but allows users to change where output files are written.
 - [`Troubleshooting`](https://amazon-orders.readthedocs.io/en/1.0.4/troubleshooting.html) section to the docs.
 - Test improvements, including the ability to run dynamic tests using private order data from JSON files.
 
 ### Changed
 - Improved string representations of entities, including [`Order`](https://amazon-orders.readthedocs.io/en/1.0.4/api.html#amazonorders.entity.order.Order), moved string representation of all fields back to `cli.py` out of the `__str__` method.
 - Moved `DEFAULT_COOKIE_JAR_PATH` to `conf.py`.
 
-## [1.0.3](https://github.com/alexdlaird/pyngrok/compare/1.0.2...1.0.3) - 2024-01-18
+## [1.0.3](https://github.com/alexdlaird/amazon-orders/compare/1.0.2...1.0.3) - 2024-01-18
 ### Added
 - CLI improvements.
 - Documentation improvements.
 
-## [1.0.2](https://github.com/alexdlaird/pyngrok/compare/1.0.1...1.0.2) - 2024-01-18
+## [1.0.2](https://github.com/alexdlaird/amazon-orders/compare/1.0.1...1.0.2) - 2024-01-18
 ### Added
 - `IODefault` for I/O operations, which can be extended to use something other than `print()` and `input()`.
 - Documentation improvements.
 - Test improvements.
 
 ### Removed
 - `Orders.print_output` variable, `cli.py` now handles output. 
 
-## [1.0.1](https://github.com/alexdlaird/pyngrok/compare/1.0.0...1.0.1) - 2024-01-17
+## [1.0.1](https://github.com/alexdlaird/amazon-orders/compare/1.0.0...1.0.1) - 2024-01-17
 ### Added
 - Auth flow now also checks session cookies in addition to parsing the page for signs of login.
 - All fields to string representation of [`Order`](https://amazon-orders.readthedocs.io/en/1.0.1/api.html#amazonorders.entity.order.Order), so they are not output on the CLI.
 - `logout` command to CLI.
 - Documentation improvements.
 - Test improvements.
 
 ### Fixed
 - Improvements to CLI, including error message cleanup on auth exceptions.
 - [`Order.order_details_link`](https://amazon-orders.readthedocs.io/en/1.0.1/api.html#amazonorders.entity.order.Order.order_details_link) is now properly populated even on the details page.
 - `.gitattributes` to HTML files are now ignore by Linguist.
 
-## [1.0.0](https://github.com/alexdlaird/amazon-orders-python/releases/tag/1.0.0) - 2024-01-16
+## [1.0.0](https://github.com/alexdlaird/amazon-orders/releases/tag/1.0.0) - 2024-01-16
 - First stable release of `amazon-orders`.
```

### Comparing `amazon-orders-1.0.9/LICENSE` & `amazon-orders-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.0.9/README.md` & `amazon-orders-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-[![PyPI Version](https://badge.fury.io/py/amazon-orders.svg)](https://badge.fury.io/py/amazon-orders)
-[![Build](https://github.com/alexdlaird/amazon-orders-python/actions/workflows/build.yml/badge.svg)](https://github.com/alexdlaird/amazon-orders-python/actions/workflows/build.yml)
-[![Codecov](https://codecov.io/gh/alexdlaird/amazon-orders-python/branch/main/graph/badge.svg)](https://codecov.io/gh/alexdlaird/amazon-orders-python)
-[![Python Versions](https://img.shields.io/pypi/pyversions/amazon-orders.svg)](https://pypi.org/project/amazon-orders/)
-[![PyPI License](https://img.shields.io/pypi/l/amazon-orders.svg)](https://pypi.org/project/amazon-orders/)
+<p align="center"><img alt="amazon-orders - a python library" src="https://amazon-orders.readthedocs.io/en/latest/_images/logo.png" /></p>
 
-# Amazon Orders
+[![Version](https://img.shields.io/pypi/v/amazon-orders)](https://pypi.org/project/amazon-orders)
+[![Python Versions](https://img.shields.io/pypi/pyversions/amazon-orders.svg)](https://pypi.org/project/amazon-orders)
+[![Coverage](https://img.shields.io/codecov/c/github/alexdlaird/amazon-orders)](https://codecov.io/gh/alexdlaird/amazon-orders)
+[![Build](https://img.shields.io/github/actions/workflow/status/alexdlaird/amazon-orders/build.yml)](https://github.com/alexdlaird/amazon-orders/actions/workflows/build.yml)
+[![Docs](https://img.shields.io/readthedocs/amazon-orders)](https://amazon-orders.readthedocs.io/en/latest)
+[![GitHub License](https://img.shields.io/github/license/alexdlaird/amazon-orders)](https://github.com/alexdlaird/amazon-orders/blob/main/LICENSE)
 
 `amazon-orders` is an unofficial library that provides a command line interface alongside a programmatic API that can
 be used to interact with Amazon.com's consumer-facing website.
 
-This works by parsing website data from Amazon.com. A nightly build validates functionality to ensure its
+This works by parsing website data from Amazon.com. A period build validates functionality to ensure its
 stability, but as Amazon provides no official API to use, this package may break at any time. This
 package only supports the English version of the website.
 
 ## Installation
 
 `amazon-orders` is available on [PyPI](https://pypi.org/project/amazon-orders/) and can be installed using `pip`:
 
@@ -41,20 +42,20 @@
                                "<AMAZON_PASSWORD>")
 amazon_session.login()
 
 amazon_orders = AmazonOrders(amazon_session)
 orders = amazon_orders.get_order_history(year=2023)
 
 for order in orders:
-    print("{} - {}".format(order.order_number, order.grand_total))
+    print(f"{order.order_number} - {order.grand_total}")
 ```
 
 ## Documentation
 
 For more advanced usage, `amazon-orders`'s official documentation is available at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
 
 ## Contributing
 
-If you would like to get involved, be sure to review the [Contribution Guide](https://github.com/alexdlaird/amazon-orders-python/blob/main/CONTRIBUTING.rst).
+If you would like to get involved, be sure to review the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
 
 Want to contribute financially? If you've found `amazon-orders` useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
 also be greatly appreciated!
```

### Comparing `amazon-orders-1.0.9/amazonorders/cli.py` & `amazon-orders-1.1.0/amazonorders/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,80 @@
+#!/usr/bin/env python
+
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import datetime
 import logging
+import os
+import platform
 from typing import Any, Optional
 
 import click
 from click.core import Context
 
+from amazonorders import __version__
 from amazonorders.conf import DEFAULT_OUTPUT_DIR
 from amazonorders.exception import AmazonOrdersError
 from amazonorders.orders import AmazonOrders
 from amazonorders.session import AmazonSession, IODefault
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.9"
-
 logger = logging.getLogger("amazonorders")
 
+banner_path = os.path.join(os.path.abspath(os.path.dirname(__file__)),
+                           "banner.txt")
+with open(banner_path) as f:
+    banner = f.read()
+
 
 class IOClick(IODefault):
     def echo(self,
              msg: str,
              fg: Optional[str] = None,
              **kwargs: Any):
         click.secho(msg, fg=fg)
 
     def prompt(self,
                msg: str,
-               type: str = None,
+               type: Optional[str] = None,
                **kwargs: Any):
-        return click.prompt("--> {}".format(msg), type=type)
+        for choice in kwargs.get("choices", []):
+            self.echo(choice, **kwargs)
+
+        return click.prompt(f"--> {msg}", type=type)
 
 
 @click.group()
 @click.option('--username', help="An Amazon username.")
 @click.option('--password', help="An Amazon password.")
-@click.option('--debug', is_flag=True, default=False, help="Enable debugging and send output to command line.")
+@click.option('--debug', is_flag=True, default=False,
+              help="Enable debugging and send output to "
+                   "command line.")
 @click.option('--max-auth-attempts', default=10,
               help="Will continue in the login auth loop this many times (successes and failures).")
 @click.option('--output-dir', default=DEFAULT_OUTPUT_DIR,
               help="The directory where any output files should be produced.")
 @click.pass_context
 def amazon_orders_cli(ctx: Context,
                       **kwargs: Any):
     """
     amazon-orders is an unofficial library that provides a command line interface alongside a programmatic API that
     can be used to interact with Amazon.com's consumer-facing website.
 
-    This works by parsing website data from Amazon.com. A nightly build validates functionality to ensure its
+    This works by parsing website data from Amazon.com. A periodic build validates functionality to ensure its
     stability, but as Amazon provides no official API to use, this package may break at any time. This
     package only supports the English version of the website.
 
     Documentation can be found at https://amazon-orders.readthedocs.io.
 
     Session data is persisted between requests and interactions with the CLI, minimizing the need to reauthenticate
     after a successful login attempt.
     """
-    _print_banner()
+    if ctx.invoked_subcommand != "version":
+        _print_banner()
 
     ctx.ensure_object(dict)
     for key, value in kwargs.items():
         if value:
             ctx.obj[key] = value
 
     if kwargs["debug"]:
@@ -69,60 +84,65 @@
     username = kwargs.get("username")
     password = kwargs.get("password")
 
     amazon_session = AmazonSession(username,
                                    password,
                                    debug=kwargs["debug"],
                                    io=IOClick(),
-                                   max_auth_attempts=kwargs["max_auth_attempts"],
+                                   max_auth_attempts=kwargs[
+                                       "max_auth_attempts"],
                                    output_dir=kwargs["output_dir"])
 
     ctx.obj["amazon_session"] = amazon_session
 
 
 @amazon_orders_cli.command()
 @click.pass_context
 @click.option('--year', default=datetime.date.today().year,
               help="The year for which to get order history, defaults to the current year.")
-@click.option('--start-index', help="Retrieve the single page of history at the given index.")
+@click.option('--start-index',
+              help="Retrieve the single page of history at the given index.")
 @click.option('--full-details', is_flag=True, default=False,
               help="Retrieve the full details for each order in the history.")
 def history(ctx: Context,
             **kwargs: Any):
     """
     Retrieve Amazon order history for a given year.
     """
     amazon_session = ctx.obj["amazon_session"]
 
-    year = kwargs["year"]
-    start_index = kwargs["start_index"]
-    full_details = kwargs["full_details"]
-
-    click.echo("""-----------------------------------------------------------------------
-Order History for {}{}{}
------------------------------------------------------------------------\n""".format(year,
-                                                                                    ", startIndex={}, one page".format(
-                                                                                        start_index) if start_index else ", all pages",
-                                                                                    ", with full details" if full_details else ""))
-
-    click.echo("Info: This might take a minute ...\n")
-
     try:
         _authenticate(ctx, amazon_session)
 
+        year = kwargs["year"]
+        start_index = kwargs["start_index"]
+        full_details = kwargs["full_details"]
+
+        optional_start_index = f", startIndex={start_index}, one page" if start_index else ", all pages"
+        optional_full_details = ", with full details" if full_details else ""
+        click.echo("""-----------------------------------------------------------------------
+Order History for {year}{optional_start_index}{optional_full_details}
+-----------------------------------------------------------------------\n"""
+                   .format(year=year,
+                           optional_start_index=optional_start_index,
+                           optional_full_details=optional_full_details))
+        click.echo("Info: This might take a minute ...\n")
+
         amazon_orders = AmazonOrders(amazon_session,
                                      debug=amazon_session.debug,
                                      output_dir=ctx.obj["output_dir"])
 
         orders = amazon_orders.get_order_history(year=kwargs["year"],
-                                                 start_index=kwargs["start_index"],
-                                                 full_details=kwargs["full_details"], )
+                                                 start_index=kwargs[
+                                                     "start_index"],
+                                                 full_details=kwargs[
+                                                     "full_details"], )
 
         for order in orders:
-            click.echo("{}\n".format(_order_output(order)))
+            click.echo(f"{_order_output(order)}\n")
     except AmazonOrdersError as e:
         logger.debug("An error occurred.", exc_info=True)
         ctx.fail(str(e))
 
 
 @amazon_orders_cli.command()
 @click.pass_context
@@ -139,15 +159,15 @@
 
         amazon_orders = AmazonOrders(amazon_session,
                                      debug=amazon_session.debug,
                                      output_dir=ctx.obj["output_dir"])
 
         order = amazon_orders.get_order(order_id)
 
-        click.echo("{}\n".format(_order_output(order)))
+        click.echo(f"{_order_output(order)}\n")
     except AmazonOrdersError as e:
         logger.debug("An error occurred.", exc_info=True)
         ctx.fail(str(e))
 
 
 @amazon_orders_cli.command(short_help="Check if persisted session exists.")
 @click.pass_context
@@ -160,89 +180,104 @@
         click.echo("Info: A persisted session exists.\n")
     else:
         click.echo("Info: No persisted session exists.\n")
 
 
 @amazon_orders_cli.command()
 @click.pass_context
+def login(ctx: Context):
+    """
+    Login to establish an Amazon session and cookies.
+    """
+    amazon_session = ctx.obj["amazon_session"]
+
+    if amazon_session.auth_cookies_stored():
+        click.echo(
+            "Info: A persisted session exists. Call the `logout` command first to change users.\n")
+    else:
+        _authenticate(ctx, amazon_session)
+
+        click.echo("Info: Successfully logged in to Amazon, session persisted.\n")
+
+
+@amazon_orders_cli.command()
+@click.pass_context
 def logout(ctx: Context):
     """
     Logout of existing Amazon sessions and clear cookies.
     """
     amazon_session = ctx.obj["amazon_session"]
     amazon_session.logout()
 
     click.echo("Info: Successfully logged out of the Amazon session.\n")
 
 
 @amazon_orders_cli.command()
-def version():
+@click.pass_context
+def version(ctx: Context):
     """
-    Get the package version.
+    Show the banner and package version.
     """
-    click.echo("Version: {}\n".format(__version__))
+    click.echo(f"hookee/{__version__} Python/{platform.python_version()}")
+    ctx.exit(0)
 
 
 def _print_banner():
-    click.echo("""
-=======================================================================
-  ___                                   _____         _               
- / _ \                                 |  _  |       | |              
-/ /_\ \_ __ ___   __ _ _______  _ __   | | | |_ __ __| | ___ _ __ ___ 
-|  _  | '_ ` _ \ / _` |_  / _ \| '_ \  | | | | '__/ _` |/ _ \ '__/ __|
-| | | | | | | | | (_| |/ / (_) | | | | \ \_/ / | | (_| |  __/ |  \__ \\
-\_| |_/_| |_| |_|\__,_/___\___/|_| |_|  \___/|_|  \__,_|\___|_|  |___/                                                                   
-=======================================================================\n""")
+    click.echo(banner.format(version=__version__))
 
 
 def _authenticate(ctx: Context,
                   amazon_session: AmazonSession):
-    if not amazon_session.username and not amazon_session.password:
-        click.echo(ctx.get_help())
-
-        ctx.fail("Amazon --username and --password must be provided, since no previous session was found.")
-
     if amazon_session.auth_cookies_stored():
         if amazon_session.username or amazon_session.password:
-            click.echo("Info: You've provided --username and --password, but because a previous session still exists,"
-                       "that is being ignored. If you would like to reauthenticate, call the `logout` command first.\n")
+            click.echo(
+                "Info: The --username and --password flags are ignored because a previous session "
+                "still exists. If you would like to reauthenticate, call the `logout` command "
+                "first.\n")
+    else:
+        if not amazon_session.username:
+            amazon_session.username = click.prompt("Username")
+        if not amazon_session.password:
+            amazon_session.password = click.prompt("Password", hide_input=True)
+            click.echo("")
 
     amazon_session.login()
 
 
 def _order_output(order):
     order_str = """-----------------------------------------------------------------------
 Order #{}
------------------------------------------------------------------------""".format(order.order_number)
+-----------------------------------------------------------------------""".format(
+        order.order_number)
 
-    order_str += "\n  Shipments: {}".format(order.shipments)
-    order_str += "\n  Order Details Link: {}".format(order.order_details_link)
-    order_str += "\n  Grand Total: ${:,.2f}".format(order.grand_total)
-    order_str += "\n  Order Placed Date: {}".format(order.order_placed_date)
-    order_str += "\n  {}".format(order.recipient)
+    order_str += f"\n  Shipments: {order.shipments}"
+    order_str += f"\n  Order Details Link: {order.order_details_link}"
+    order_str += f"\n  Grand Total: ${order.grand_total:,.2f}"
+    order_str += f"\n  Order Placed Date: {order.order_placed_date}"
+    order_str += f"\n  {order.recipient}"
     if order.payment_method:
-        order_str += "\n  Payment Method: {}".format(order.payment_method)
+        order_str += f"\n  Payment Method: {order.payment_method}"
     if order.payment_method_last_4:
-        order_str += "\n  Payment Method Last 4: {}".format(order.payment_method_last_4)
+        order_str += f"\n  Payment Method Last 4: {order.payment_method_last_4}"
     if order.subtotal:
-        order_str += "\n  Subtotal: ${:,.2f}".format(order.subtotal)
+        order_str += f"\n  Subtotal: ${order.subtotal:,.2f}"
     if order.shipping_total:
-        order_str += "\n  Shipping Total: ${:,.2f}".format(order.shipping_total)
+        order_str += f"\n  Shipping Total: ${order.shipping_total:,.2f}"
     if order.subscription_discount:
-        order_str += "\n  Subscription Discount: ${:,.2f}".format(order.subscription_discount)
+        order_str += f"\n  Subscription Discount: ${order.subscription_discount:,.2f}"
     if order.total_before_tax:
-        order_str += "\n  Total Before Tax: ${:,.2f}".format(order.total_before_tax)
+        order_str += f"\n  Total Before Tax: ${order.total_before_tax:,.2f}"
     if order.estimated_tax:
-        order_str += "\n  Estimated Tax: ${:,.2f}".format(order.estimated_tax)
+        order_str += f"\n  Estimated Tax: ${order.estimated_tax:,.2f}"
     if order.refund_total:
-        order_str += "\n  Refund Total: ${:,.2f}".format(order.refund_total)
+        order_str += f"\n  Refund Total: ${order.refund_total:,.2f}"
     if order.order_shipped_date:
-        order_str += "\n  Order Shipped Date: {}".format(order.order_shipped_date)
+        order_str += f"\n  Order Shipped Date: {order.order_shipped_date}"
     if order.refund_completed_date:
-        order_str += "\n  Refund Completed Date: {}".format(order.refund_completed_date)
+        order_str += f"\n  Refund Completed Date: {order.refund_completed_date}"
 
     order_str += "\n-----------------------------------------------------------------------"
 
     return order_str
 
 
 if __name__ == "__main__":
```

### Comparing `amazon-orders-1.0.9/amazonorders/constants.py` & `amazon-orders-1.1.0/amazonorders/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
+import os
 
 ##########################################################################
 # General URL
 ##########################################################################
 
-BASE_URL = "https://www.amazon.com"
+BASE_URL = os.environ.get("AMAZON_BASE_URL", "https://www.amazon.com")
 
 ##########################################################################
 # URLs for AmazonSession
 ##########################################################################
 
-SIGN_IN_URL = "{}/gp/sign-in.html".format(BASE_URL)
-SIGN_IN_REDIRECT_URL = "{}/ap/signin".format(BASE_URL)
-SIGN_OUT_URL = "{}/gp/sign-out.html".format(BASE_URL)
+SIGN_IN_URL = f"{BASE_URL}/gp/sign-in.html"
+SIGN_IN_REDIRECT_URL = f"{BASE_URL}/ap/signin"
+SIGN_OUT_URL = f"{BASE_URL}/gp/sign-out.html"
 
 ##########################################################################
 # URLs for AmazonOrders
 ##########################################################################
 
-ORDER_HISTORY_LANDING_URL = "{}/gp/css/order-history".format(BASE_URL)
-ORDER_HISTORY_URL = "{}/your-orders/orders".format(BASE_URL)
-ORDER_DETAILS_URL = "{}/gp/your-account/order-details".format(BASE_URL)
+ORDER_HISTORY_LANDING_URL = f"{BASE_URL}/gp/css/order-history"
+ORDER_HISTORY_URL = f"{BASE_URL}/your-orders/orders"
+ORDER_DETAILS_URL = f"{BASE_URL}/gp/your-account/order-details"
 HISTORY_FILTER_QUERY_PARAM = "timeFilter"
 
 ##########################################################################
 # Headers
 ##########################################################################
 
 BASE_HEADERS = {
-    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,"
+              "application/signed-exchange;v=b3;q=0.7",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "en-US,en;q=0.9",
     "Cache-Control": "max-age=0",
     "Content-Type": "application/x-www-form-urlencoded",
     "Origin": BASE_URL,
     "Referer": SIGN_IN_REDIRECT_URL,
     "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
@@ -42,15 +44,16 @@
     "Sec-Ch-Ua-Platform": "macOS",
     "Sec-Ch-Viewport-Width": "1393",
     "Sec-Fetch-Dest": "document",
     "Sec-Fetch-Mode": "navigate",
     "Sec-Fetch-Site": "same-origin",
     "Sec-Fetch-User": "?1",
     "Viewport-Width": "1393",
-    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) "
+                  "Chrome/120.0.0.0 Safari/537.36",
 }
 
 ##########################################################################
 # CSS selectors for AuthForms
 ##########################################################################
 
 SIGN_IN_FORM_SELECTOR = "form[name='signIn']"
@@ -98,15 +101,16 @@
 #####################################
 # CSS selectors for Order fields
 #####################################
 
 FIELD_ORDER_DETAILS_LINK_SELECTOR = "a.yohtmlc-order-details-link"
 FIELD_ORDER_NUMBER_SELECTOR = "bdi[dir='ltr']"
 FIELD_ORDER_GRAND_TOTAL_SELECTOR = "div.yohtmlc-order-total span.value"
-FIELD_ORDER_PLACED_DATE_SELECTOR = ["span.order-date-invoice-item", "div.a-span3"]
+FIELD_ORDER_PLACED_DATE_SELECTOR = ["span.order-date-invoice-item",
+                                    "div.a-span3"]
 FIELD_ORDER_PAYMENT_METHOD_SELECTOR = "img.pmts-payment-credit-card-instrument-logo"
 FIELD_ORDER_PAYMENT_METHOD_LAST_4_SELECTOR = "img.pmts-payment-credit-card-instrument-logo"
 FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR = "div#od-subtotals div.a-row"
 FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR = "div.a-span-last"
 FIELD_ORDER_ADDRESS_SELECTOR = "div.displayAddressDiv"
 FIELD_ORDER_ADDRESS_FALLBACK_1_SELECTOR = "div.recipient span.a-declarative"
 FIELD_ORDER_ADDRESS_FALLBACK_2_SELECTOR = "script[id^='shipToData']"
@@ -120,15 +124,16 @@
 FIELD_SHIPMENT_TRACKING_LINK_SELECTOR = "span.track-package-button a"
 FIELD_SHIPMENT_DELIVERY_STATUS_SELECTOR = "div.js-shipment-info-container div.a-row"
 
 #####################################
 # CSS selectors for Recipient fields
 #####################################
 
-FIELD_RECIPIENT_NAME_SELECTOR = ["li.displayAddressFullName", "div:nth-child(1)"]
+FIELD_RECIPIENT_NAME_SELECTOR = ["li.displayAddressFullName",
+                                 "div:nth-child(1)"]
 FIELD_RECIPIENT_ADDRESS1_SELECTOR = "li.displayAddressAddressLine1"
 FIELD_RECIPIENT_ADDRESS2_SELECTOR = "li.displayAddressAddressLine2"
 FIELD_RECIPIENT_ADDRESS_CITY_STATE_POSTAL_SELECTOR = "li.displayAddressCityStateOrRegionPostalCode"
 FIELD_RECIPIENT_ADDRESS_COUNTRY_SELECTOR = "li.displayAddressCountryName"
 FIELD_RECIPIENT_ADDRESS_FALLBACK_SELECTOR = "div:nth-child(2)"
 
 #####################################
```

### Comparing `amazon-orders-1.0.9/amazonorders/entity/item.py` & `amazon-orders-1.1.0/amazonorders/entity/item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import logging
 from datetime import datetime, date
 from typing import Optional
 
 from bs4 import Tag
 
 from amazonorders import constants
 from amazonorders.entity.parsable import Parsable
 from amazonorders.entity.seller import Seller
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.9"
-
 logger = logging.getLogger(__name__)
 
 
 class Item(Parsable):
     """
     An Item in an Amazon :class:`~amazonorders.entity.order.Order`.
     """
@@ -40,18 +39,18 @@
         self.image_link: Optional[str] = self.safe_simple_parse(selector=constants.FIELD_ITEM_IMG_LINK_SELECTOR,
                                                                 link=True)
         #: The Item quantity.
         self.quantity: Optional[int] = self.safe_simple_parse(selector=constants.FIELD_ITEM_QUANTITY_SELECTOR,
                                                               return_type=int)
 
     def __repr__(self) -> str:
-        return "<Item: \"{}\">".format(self.title)
+        return f"<Item: \"{self.title}\">"
 
     def __str__(self) -> str:  # pragma: no cover
-        return "Item: {}".format(self.title)
+        return f"Item: {self.title}"
 
     def __lt__(self, other):
         return self.title < other.title
 
     def _parse_price(self) -> Optional[float]:
         value = None
```

### Comparing `amazon-orders-1.0.9/amazonorders/entity/order.py` & `amazon-orders-1.1.0/amazonorders/entity/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import json
 import logging
 from datetime import datetime, date
 from typing import List, Optional, TypeVar
 from urllib.parse import urlparse, parse_qs
 
 from bs4 import BeautifulSoup, Tag
 
 from amazonorders import constants
 from amazonorders.entity.item import Item
 from amazonorders.entity.parsable import Parsable
 from amazonorders.entity.recipient import Recipient
 from amazonorders.entity.shipment import Shipment
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 logger = logging.getLogger(__name__)
 
 Entity = TypeVar('Entity', bound='Order')
 
 
 class Order(Parsable):
     """
@@ -51,39 +50,39 @@
             self._parse_order_placed_date)
         #: The Order Recipients.
         self.recipient: Recipient = clone.recipient if clone else self.safe_parse(self._parse_recipient)
 
         # Fields below this point are only populated if `full_details` is True
 
         #: The Order payment method. Only populated when ``full_details`` is ``True``.
-        self.payment_method: Optional[str] = self._parse_payment_method() if self.full_details else None
+        self.payment_method: Optional[str] = self._if_full_details(self._parse_payment_method())
         #: The Order payment method's last 4 digits. Only populated when ``full_details`` is ``True``.
-        self.payment_method_last_4: Optional[str] = self._parse_payment_method_last_4() if self.full_details else None
+        self.payment_method_last_4: Optional[str] = self._if_full_details(self._parse_payment_method_last_4())
         #: The Order subtotal. Only populated when ``full_details`` is ``True``.
-        self.subtotal: Optional[float] = self._parse_subtotal() if self.full_details else None
+        self.subtotal: Optional[float] = self._if_full_details(self._parse_subtotal())
         #: The Order shipping total. Only populated when ``full_details`` is ``True``.
-        self.shipping_total: Optional[float] = self._parse_shipping_total() if self.full_details else None
+        self.shipping_total: Optional[float] = self._if_full_details(self._parse_shipping_total())
         #: The Order Subscribe & Save discount. Only populated when ``full_details`` is ``True``.
-        self.subscription_discount: Optional[float] = self._parse_subscription_discount() if self.full_details else None
+        self.subscription_discount: Optional[float] = self._if_full_details(self._parse_subscription_discount())
         #: The Order total before tax. Only populated when ``full_details`` is ``True``.
-        self.total_before_tax: Optional[float] = self._parse_total_before_tax() if self.full_details else None
+        self.total_before_tax: Optional[float] = self._if_full_details(self._parse_total_before_tax())
         #: The Order estimated tax. Only populated when ``full_details`` is ``True``.
-        self.estimated_tax: Optional[float] = self._parse_estimated_tax() if self.full_details else None
+        self.estimated_tax: Optional[float] = self._if_full_details(self._parse_estimated_tax())
         #: The Order refund total. Only populated when ``full_details`` is ``True``.
-        self.refund_total: Optional[float] = self._parse_refund_total() if self.full_details else None
+        self.refund_total: Optional[float] = self._if_full_details(self._parse_refund_total())
         #: The Order shipped date. Only populated when ``full_details`` is ``True``.
-        self.order_shipped_date: Optional[date] = self._parse_order_shipping_date() if self.full_details else None
+        self.order_shipped_date: Optional[date] = self._if_full_details(self._parse_order_shipping_date())
         #: The Order refund total. Only populated when ``full_details`` is ``True``.
-        self.refund_completed_date: Optional[date] = self._parse_refund_completed_date() if self.full_details else None
+        self.refund_completed_date: Optional[date] = self._if_full_details(self._parse_refund_completed_date())
 
     def __repr__(self) -> str:
-        return "<Order #{}: \"{}\">".format(self.order_number, self.items)
+        return f"<Order #{self.order_number}: \"{self.items}\">"
 
     def __str__(self) -> str:  # pragma: no cover
-        return "Order #{}: {}".format(self.order_number, self.items)
+        return f"Order #{self.order_number}: {self.items}"
 
     def _parse_shipments(self) -> List[Shipment]:
         shipments = [Shipment(x) for x in self.parsed.select(constants.SHIPMENT_ENTITY_SELECTOR)]
         shipments.sort()
         return shipments
 
     def _parse_items(self) -> List[Item]:
@@ -91,22 +90,22 @@
         items.sort()
         return items
 
     def _parse_order_details_link(self) -> Optional[str]:
         value = self.simple_parse(constants.FIELD_ORDER_DETAILS_LINK_SELECTOR, link=True)
 
         if not value and self.order_number:
-            value = "{}?orderID={}".format(constants.ORDER_DETAILS_URL, self.order_number)
+            value = f"{constants.ORDER_DETAILS_URL}?orderID={self.order_number}"
 
         return value
 
     def _parse_order_number(self) -> str:
         try:
             order_details_link = self._parse_order_details_link()
-        except:
+        except Exception:
             # We're not using safe_parse here because it's fine if this fails, no need for noise
             order_details_link = None
 
         if order_details_link:
             parsed_url = urlparse(order_details_link)
             value = parse_qs(parsed_url.query)["orderID"][0]
         else:
@@ -150,15 +149,16 @@
 
             if value:
                 inline_content = value.get("data-a-popover", {}).get("inlineContent")
                 if inline_content:
                     value = BeautifulSoup(json.loads(inline_content), "html.parser")
 
         if not value:
-            # TODO: there are multiple shipToData tags, we should double check we're picking the right one associated with the order
+            # TODO: there are multiple shipToData tags, we should double check we're picking the right one
+            #  associated with the order
             parent_tag = self.parsed.find_parent().select_one(constants.FIELD_ORDER_ADDRESS_FALLBACK_2_SELECTOR)
             value = BeautifulSoup(str(parent_tag.contents[0]).strip(), "html.parser")
 
         return Recipient(value)
 
     def _parse_payment_method(self) -> Optional[str]:
         value = None
@@ -268,7 +268,10 @@
         value = self.simple_parse(constants.FIELD_ORDER_REFUND_COMPLETED_DATE, text_contains=match_text)
 
         if value:
             date_str = value.split(match_text)[1].strip().split("-")[0].strip()
             value = datetime.strptime(date_str, "%B %d, %Y").date()
 
         return value
+
+    def _if_full_details(self, value):
+        return value if self.full_details else None
```

### Comparing `amazon-orders-1.0.9/amazonorders/entity/parsable.py` & `amazon-orders-1.1.0/amazonorders/entity/parsable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import logging
 from typing import Callable, Any, Optional, Type, Union
 
 from bs4 import Tag
 
 from amazonorders.constants import BASE_URL
 from amazonorders.exception import AmazonOrdersError, AmazonOrderEntityError
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 logger = logging.getLogger(__name__)
 
 
 class Parsable:
     """
     A base class that contains a parsed representation of the entity, and can be extended to
     be made up of the entities fields utilizing the helper methods.
     """
 
     def __init__(self,
                  parsed: Tag) -> None:
         #: Parsed HTML data that can be used to populate the fields of the entity.
         self.parsed: Tag = parsed
 
+    def __getstate__(self):
+        state = self.__dict__.copy()
+        state.pop("parsed")
+        return state
+
     def safe_parse(self,
                    parse_function: Callable[..., Any],
                    **kwargs: Any) -> Any:
         """
         Execute the given parse function on a field, handling any common parse exceptions and passing
         them as warnings to the logger, suppressing them as exceptions.
 
@@ -37,18 +41,20 @@
         """
         if not parse_function.__name__.startswith("_parse_") and parse_function.__name__ != "simple_parse":
             raise AmazonOrdersError("The name of the `parse_function` passed to this method must start with `_parse_`")
 
         try:
             return parse_function(**kwargs)
         except (AttributeError, IndexError, ValueError):
-            logger.warning("When building {}, `{}` could not be parsed.".format(self.__class__.__name__,
-                                                                                parse_function.__name__.split(
-                                                                                    "_parse_")[1]),
-                           exc_info=True)
+            logger.warning(
+                "When building {name}, `{function}` "
+                "could not be parsed.".format(name=self.__class__.__name__,
+                                              function=parse_function.__name__.split(
+                                                  "_parse_")[1]),
+                exc_info=True)
 
     def simple_parse(self,
                      selector: Union[str, list],
                      link: bool = False,
                      return_type: Optional[Type] = None,
                      text_contains: Optional[str] = None,
                      required: bool = False, ) -> Any:
@@ -90,16 +96,16 @@
                     elif return_type == int:
                         value = int(value)
                 break
 
         # None of the selectors were found
         if not value and required:
             raise AmazonOrderEntityError(
-                "When building {}, field for selector `{}` was None, but this is not allowed.".format(
-                    self.__class__.__name__, selector))
+                "When building {name}, field for selector `{selector}` was None, but this is not allowed.".format(
+                    name=self.__class__.__name__, selector=selector))
 
         return value
 
     def safe_simple_parse(self,
                           selector: Union[str, list],
                           **kwargs) -> Any:
         """
@@ -115,9 +121,9 @@
         """
         If the given URL is relative, the ``BASE_URL`` will be prepended.
 
         :param url: The URL to check.
         :return: The fully qualified URL.
         """
         if not url.startswith("http"):
-            url = "{}{}".format(BASE_URL, url)
+            url = f"{BASE_URL}{url}"
         return url
```

### Comparing `amazon-orders-1.0.9/amazonorders/entity/recipient.py` & `amazon-orders-1.1.0/amazonorders/entity/recipient.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import logging
 from typing import Optional
 
 from bs4 import Tag
 
 from amazonorders import constants
 from amazonorders.entity.parsable import Parsable
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.9"
-
 logger = logging.getLogger(__name__)
 
 
 class Recipient(Parsable):
     """
     The person receiving an Amazon :class:`~amazonorders.entity.order.Order`.
     """
@@ -24,18 +23,18 @@
 
         #: The Recipient name.
         self.name: str = self.safe_simple_parse(selector=constants.FIELD_RECIPIENT_NAME_SELECTOR, required=True)
         #: The Recipient address.
         self.address: Optional[str] = self.safe_parse(self._parse_address)
 
     def __repr__(self) -> str:
-        return "<Recipient: \"{}\">".format(self.name)
+        return f"<Recipient: \"{self.name}\">"
 
     def __str__(self) -> str:  # pragma: no cover
-        return "Recipient: {}".format(self.name)
+        return f"Recipient: {self.name}"
 
     def _parse_address(self) -> Optional[str]:
         value = self.simple_parse(constants.FIELD_RECIPIENT_ADDRESS1_SELECTOR)
 
         if value:
             values = [
                 value,
```

### Comparing `amazon-orders-1.0.9/amazonorders/entity/seller.py` & `amazon-orders-1.1.0/amazonorders/entity/seller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import logging
 from typing import Optional
 
 from bs4 import Tag
 
 from amazonorders import constants
 from amazonorders.entity.parsable import Parsable
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.9"
-
 logger = logging.getLogger(__name__)
 
 
 class Seller(Parsable):
     """
     An Amazon Seller of an Amazon :class:`~amazonorders.entity.item.Item`.
     """
@@ -24,18 +23,18 @@
 
         #: The Seller name.
         self.name: str = self.safe_parse(self._parse_name)
         #: The Seller link.
         self.link: Optional[str] = self.safe_simple_parse(selector=constants.FIELD_SELLER_LINK_SELECTOR, link=True)
 
     def __repr__(self) -> str:
-        return "<Seller: \"{}\">".format(self.name)
+        return f"<Seller: \"{self.name}\">"
 
     def __str__(self) -> str:  # pragma: no cover
-        return "Seller: {}".format(self.name)
+        return f"Seller: {self.name}"
 
     def _parse_name(self) -> str:
         match_text = "Sold by:"
         value = self.simple_parse(constants.FIELD_SELLER_NAME_SELECTOR, text_contains=match_text)
 
         if value:
             value = value.split(match_text)[1]
```

### Comparing `amazon-orders-1.0.9/amazonorders/entity/shipment.py` & `amazon-orders-1.1.0/amazonorders/entity/shipment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import logging
 from typing import List, Optional
 
 from bs4 import Tag
 
 from amazonorders import constants
 from amazonorders.constants import ITEM_ENTITY_SELECTOR
 from amazonorders.entity.item import Item
 from amazonorders.entity.parsable import Parsable
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 logger = logging.getLogger(__name__)
 
 
 class Shipment(Parsable):
     """
     An Amazon Shipment, which should contain one or more :class:`~amazonorders.entity.item.Item`'s.
     """
@@ -31,18 +30,18 @@
             selector=constants.FIELD_SHIPMENT_DELIVERY_STATUS_SELECTOR)
         #: The Shipment tracking link.
         self.tracking_link: Optional[str] = self.safe_simple_parse(
             selector=constants.FIELD_SHIPMENT_TRACKING_LINK_SELECTOR,
             link=True)
 
     def __repr__(self) -> str:
-        return "<Shipment: \"{}\">".format(self.items)
+        return f"<Shipment: \"{self.items}\">"
 
     def __str__(self) -> str:  # pragma: no cover
-        return "Shipment: {}".format(self.items)
+        return f"Shipment: {self.items}"
 
     def __lt__(self, other):
         if self.delivery_status:
             return self.delivery_status < str(other.delivery_status if other.delivery_status else "")
         else:
             return str(self.items) < str(other.items)
```

### Comparing `amazon-orders-1.0.9/amazonorders/forms.py` & `amazon-orders-1.1.0/amazonorders/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 from abc import ABC
 from io import BytesIO
 from typing import Optional, Dict, Any
 from urllib.parse import urlparse
 
 from PIL import Image
 from amazoncaptcha import AmazonCaptcha
 from bs4 import Tag
 
 from amazonorders import constants
 from amazonorders.exception import AmazonOrdersError, AmazonOrdersAuthError
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.9"
-
 
 class AuthForm(ABC):
     """
     The base class of an authentication ``<form>`` that can be submitted.
 
     The base implementation will attempt to auto-solve Captcha. If this fails, it will
     use the default image view to show the Captcha prompt, and it will also pass the
@@ -66,15 +65,15 @@
         if not self.form:
             raise AmazonOrdersError("Call AuthForm.select_form() first.")
 
         self.data = {}
         for field in self.form.select("input"):
             try:
                 self.data[field["name"]] = field["value"]
-            except:
+            except Exception:
                 pass
         if additional_attrs:
             self.data.update(additional_attrs)
 
     def submit(self) -> None:
         """
         Submit the populated ``<form>``.
@@ -110,38 +109,37 @@
             img_response = self.amazon_session.session.get(url)
             img = Image.open(BytesIO(img_response.content))
             img.show()
 
             self.amazon_session.io.echo("Info: The Captcha couldn't be auto-solved.")
 
             captcha_response = self.amazon_session.io.prompt("Enter the characters shown in the image",
-                                                             captcha_img_url=url)
+                                                             img_url=url)
             self.amazon_session.io.echo("")
 
         return captcha_response
 
     def _get_form_action(self) -> str:
         action = self.form.get("action")
         if not action:
             return self.amazon_session.last_response.url
         elif not action.startswith("http"):
             if action.startswith("/"):
                 parsed_url = urlparse(self.amazon_session.last_response.url)
-                return "{}://{}{}".format(parsed_url.scheme, parsed_url.netloc,
-                                          action)
+                return f"{parsed_url.scheme}://{parsed_url.netloc}{action}"
             else:
-                return "{}/{}".format(
-                    "/".join(self.amazon_session.last_response.url.split("/")[:-1]), action)
+                return "{url}/{path}".format(url="/".join(self.amazon_session.last_response.url.split("/")[:-1]),
+                                             path=action)
         else:
             return action
 
     def _handle_errors(self) -> None:
         error_tag = self.amazon_session.last_response_parsed.select_one(self.error_selector)
         if error_tag:
-            error_msg = "An error occurred: {}\n".format(error_tag.text.strip())
+            error_msg = f"An error occurred: {error_tag.text.strip()}\n"
 
             if self.critical:
                 raise AmazonOrdersAuthError(error_msg)
             else:
                 self.amazon_session.io.echo(error_msg, fg="red")
 
 
@@ -192,23 +190,24 @@
     def fill_form(self,
                   additional_attrs: Optional[Dict[str, Any]] = None) -> None:
         if not additional_attrs:
             additional_attrs = {}
         super().fill_form()
 
         contexts = self.form.select(constants.MFA_DEVICE_SELECT_INPUT_SELECTOR)
-        i = 1
+        i = 0
+        choices = []
         for field in contexts:
-            self.amazon_session.io.echo("{}: {}".format(i, field["value"].strip()))
+            choices.append(f"{i}: {field['value'].strip()}")
             i += 1
 
         otp_device = int(
             self.amazon_session.io.prompt("Choose where you would like your one-time passcode sent",
                                           type=int,
-                                          mfa_device_select_choices=contexts)
+                                          choices=choices)
         )
         self.amazon_session.io.echo("")
 
         additional_attrs.update({self.solution_attr_key: contexts[otp_device - 1]["value"]})
         self.data.update(additional_attrs)
 
 
@@ -248,12 +247,12 @@
         if not additional_attrs:
             additional_attrs = {}
         super().fill_form(additional_attrs)
 
         # TODO: eliminate the use of find_parent() here
         img_url = self.form.find_parent().select_one("img")["src"]
         if not img_url.startswith("http"):
-            img_url = "{}{}".format(constants.BASE_URL, img_url)
+            img_url = f"{constants.BASE_URL}{img_url}"
         solution = self._solve_captcha(img_url)
 
         additional_attrs.update({self.solution_attr_key: solution})
         self.data.update(additional_attrs)
```

### Comparing `amazon-orders-1.0.9/amazonorders/orders.py` & `amazon-orders-1.1.0/amazonorders/orders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import datetime
 import logging
 from typing import List, Optional
 
 from amazonorders import constants
 from amazonorders.conf import DEFAULT_OUTPUT_DIR
 from amazonorders.entity.order import Order
 from amazonorders.exception import AmazonOrdersError
 from amazonorders.session import AmazonSession
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 logger = logging.getLogger(__name__)
 
 
 class AmazonOrders:
     """
     Using an authenticated :class:`~amazonorders.session.AmazonSession`, can be used to query Amazon
     for Order details and history.
     """
 
     def __init__(self,
                  amazon_session: AmazonSession,
                  debug: bool = False,
-                 output_dir: str = None) -> None:
+                 output_dir: Optional[str] = None) -> None:
         if not output_dir:
             output_dir = DEFAULT_OUTPUT_DIR
 
         #: The AmazonSession to use for requests.
         self.amazon_session: AmazonSession = amazon_session
 
         #: Set logger ``DEBUG`` and send output to ``stderr``.
@@ -43,29 +42,32 @@
                           start_index: Optional[int] = None,
                           full_details: bool = False) -> List[Order]:
         """
         Get the Amazon order history for the given year.
 
         :param year: The year for which to get history.
         :param start_index: The index to start at within the history.
-        :param full_details: Will execute an additional request per Order in the retrieved history to fully populate it.
+        :param full_details: Will execute an additional request per Order in the retrieved history to fully
+            populate it.
         :return: A list of the requested Orders.
         """
         if not self.amazon_session.is_authenticated:
             raise AmazonOrdersError("Call AmazonSession.login() to authenticate first.")
 
         self.amazon_session.get(constants.ORDER_HISTORY_LANDING_URL)
         if not self.amazon_session.last_response_parsed.select_one("select[name='timeFilter']"):
             constants.HISTORY_FILTER_QUERY_PARAM = "orderFilter"
 
         orders = []
-        next_page = "{}?{}=year-{}{}".format(constants.ORDER_HISTORY_URL,
-                                             constants.HISTORY_FILTER_QUERY_PARAM,
-                                             year,
-                                             "&startIndex={}".format(start_index) if start_index else "")
+        optional_start_index = f"&startIndex={start_index}" if start_index else ""
+        next_page = ("{url}?{query_param}=year-{year}"
+                     "{optional_start_index}").format(url=constants.ORDER_HISTORY_URL,
+                                                      query_param=constants.HISTORY_FILTER_QUERY_PARAM,
+                                                      year=year,
+                                                      optional_start_index=optional_start_index)
         while next_page:
             self.amazon_session.get(next_page)
             response_parsed = self.amazon_session.last_response_parsed
 
             for order_tag in response_parsed.select(constants.ORDER_HISTORY_ENTITY_SELECTOR):
                 order = Order(order_tag)
 
@@ -79,15 +81,15 @@
 
             next_page = None
             if start_index is None:
                 next_page_tag = response_parsed.select_one(constants.NEXT_PAGE_LINK_SELECTOR)
                 if next_page_tag:
                     next_page = next_page_tag["href"]
                     if not next_page.startswith("http"):
-                        next_page = "{}{}".format(constants.BASE_URL, next_page)
+                        next_page = f"{constants.BASE_URL}{next_page}"
                 else:
                     logger.debug("No next page")
             else:
                 logger.debug("start_index is given, not paging")
 
         return orders
 
@@ -98,13 +100,14 @@
 
         :param order_id: The Amazon Order ID to lookup.
         :return: The requested Order.
         """
         if not self.amazon_session.is_authenticated:
             raise AmazonOrdersError("Call AmazonSession.login() to authenticate first.")
 
-        self.amazon_session.get("{}?orderID={}".format(constants.ORDER_DETAILS_URL, order_id))
+        self.amazon_session.get(f"{constants.ORDER_DETAILS_URL}?orderID={order_id}")
 
-        order_details_tag = self.amazon_session.last_response_parsed.select_one(constants.ORDER_DETAILS_ENTITY_SELECTOR)
+        order_details_tag = self.amazon_session.last_response_parsed.select_one(
+            constants.ORDER_DETAILS_ENTITY_SELECTOR)
         order = Order(order_details_tag, full_details=True)
 
         return order
```

### Comparing `amazon-orders-1.0.9/amazonorders/session.py` & `amazon-orders-1.1.0/amazonorders/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import json
 import logging
 import os
 from typing import Optional, Any
 from urllib.parse import urlparse
 
 import requests
@@ -10,25 +13,23 @@
 from requests.utils import dict_from_cookiejar
 
 from amazonorders import constants
 from amazonorders.conf import DEFAULT_COOKIE_JAR_PATH, DEFAULT_OUTPUT_DIR
 from amazonorders.exception import AmazonOrdersAuthError
 from amazonorders.forms import SignInForm, MfaDeviceSelectForm, MfaForm, CaptchaForm
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.9"
-
 logger = logging.getLogger(__name__)
 
 AUTH_FORMS = [SignInForm(),
               MfaDeviceSelectForm(),
               MfaForm(),
               CaptchaForm(),
-              CaptchaForm(constants.CAPTCHA_2_FORM_SELECTOR, constants.CAPTCHA_2_ERROR_SELECTOR, "field-keywords"),
+              CaptchaForm(constants.CAPTCHA_2_FORM_SELECTOR,
+                          constants.CAPTCHA_2_ERROR_SELECTOR,
+                          "field-keywords"),
               MfaForm(constants.CAPTCHA_OTP_FORM_SELECTOR)]
 
 
 class IODefault:
     """
     Handles input/output from the application. By default, this uses console commands, but
     this class exists so that it can be overriden when constructing an :class:`AmazonSession`
@@ -44,25 +45,28 @@
         :param msg: The data to send to output.
         :param kwargs: Unused by the default implementation.
         """
         print(msg)
 
     def prompt(self,
                msg: str,
-               type: str = None,
+               type: Optional[str] = None,
                **kwargs: Any):
         """
         Prompt to the console for user input.
 
         :param msg: The data to use as the input prompt.
         :param type: Unused by the default implementation.
         :param kwargs: Unused by the default implementation.
         :return: The user input result.
         """
-        return input("--> {}: ".format(msg))
+        for choice in kwargs.get("choices", []):
+            self.echo(choice, **kwargs)
+
+        return input(f"--> {msg}: ")
 
 
 class AmazonSession:
     """
     An interface for interacting with Amazon and authenticating an underlying :class:`requests.Session`. Utilizing
     this class means session data is maintained between requests. Session data is also persisted after each request,
     meaning it will also be maintained between separate instantiations of the class or application.
@@ -84,15 +88,15 @@
             output_dir = DEFAULT_OUTPUT_DIR
 
         #: An Amazon username.
         self.username: str = username
         #: An Amazon password.
         self.password: str = password
 
-        #: Set logger ``DEBUG``, send output to ``stderr``, and write an HTML file for each request made on the session.
+        #: Set logger ``DEBUG``, send output to ``stderr``, and write an HTML file for requests made on the session.
         self.debug: bool = debug
         if self.debug:
             logger.setLevel(logging.DEBUG)
         #: Will continue in :func:`login`'s auth flow this many times (successes and failures).
         self.max_auth_attempts: int = max_auth_attempts
         #: The path to persist session cookies, defaults to ``conf.DEFAULT_COOKIE_JAR_PATH``.
         self.cookie_jar_path: str = cookie_jar_path
@@ -132,35 +136,34 @@
         :param kwargs: Remaining ``kwargs`` will be passed to :func:`requests.request`.
         :return: The Response from the executed request.
         """
         if "headers" not in kwargs:
             kwargs["headers"] = {}
         kwargs["headers"].update(constants.BASE_HEADERS)
 
-        logger.debug("{} request to {}".format(method, url))
+        logger.debug(f"{method} request to {url}")
 
         self.last_response = self.session.request(method, url, **kwargs)
         self.last_response_parsed = BeautifulSoup(self.last_response.text,
                                                   "html.parser")
 
         cookies = dict_from_cookiejar(self.session.cookies)
         if os.path.exists(self.cookie_jar_path):
             os.remove(self.cookie_jar_path)
         with open(self.cookie_jar_path, "w", encoding="utf-8") as f:
             f.write(json.dumps(cookies))
 
-        logger.debug("Response: {} - {}".format(self.last_response.url,
-                                                self.last_response.status_code))
+        logger.debug(f"Response: {self.last_response.url} - {self.last_response.status_code}")
 
         if self.debug:
             page_name = self._get_page_from_url(self.last_response.url)
             with open(os.path.join(self.output_dir, page_name), "w",
                       encoding="utf-8") as html_file:
                 logger.debug(
-                    "Response written to file: {}".format(html_file.name))
+                    f"Response written to file: {html_file.name}")
                 html_file.write(self.last_response.text)
 
         return self.last_response
 
     def get(self,
             url: str,
             **kwargs: Any):
@@ -204,15 +207,16 @@
         # If our local session data is stale, Amazon will redirect us to the signin page
         if self.auth_cookies_stored() and self.last_response.url.split("?")[0] == constants.SIGN_IN_REDIRECT_URL:
             self.logout()
             self.get(constants.SIGN_IN_URL)
 
         attempts = 0
         while not self.is_authenticated and attempts < self.max_auth_attempts:
-            # TODO: BeautifulSoup doesn't let us query for #nav-item-signout, maybe because it's dynamic on the page, but we should find a better way to do this
+            # TODO: BeautifulSoup doesn't let us query for #nav-item-signout, maybe because it's dynamic on the page,
+            #  but we should find a better way to do this
             if self.auth_cookies_stored() or \
                     ("Hello, sign in" not in self.last_response.text and
                      "nav-item-signout" in self.last_response.text):
                 self.is_authenticated = True
                 break
 
             form_found = False
@@ -251,28 +255,27 @@
     def _get_page_from_url(self,
                            url: str) -> str:
         page_name = os.path.splitext(os.path.basename(urlparse(url).path))[0]
         if not page_name:
             page_name = "index"
 
         i = 0
-        filename_frmt = "{}_{}.html"
-        while os.path.isfile(filename_frmt.format(page_name, i)):
+        filename_frmt = "{page_name}_{index}.html"
+        while os.path.isfile(filename_frmt.format(page_name=page_name, index=i)):
             i += 1
-        return filename_frmt.format(page_name, i)
+        return filename_frmt.format(page_name=page_name, index=i)
 
     def _raise_auth_error(self):
         debug_str = " To capture the page to a file, set the `debug` flag." if not self.debug else ""
         if self.last_response.ok:
-            error_msg = ("An error occurred, this is an unknown page, or its parsed contents don't match a "
-                         "known auth flow: {}.{}").format(self.last_response.url, debug_str)
+            error_msg = (f"An error occurred, this is an unknown page, or its parsed contents don't match a "
+                         f"known auth flow: {self.last_response.url}.{debug_str}")
         else:
-            error_msg = "An error occurred, the page {} returned {}.".format(self.last_response.url,
-                                                                             self.last_response.status_code)
+            error_msg = "An error occurred, the page {url} returned {status_code}."
             if 500 <= self.last_response.status_code < 600:
                 error_msg += (" Amazon had an issue on their end, or may be temporarily blocking your requests. "
-                              "Wait a bit before trying again.").format(self.last_response.url,
-                                                                        self.last_response.status_code)
+                              "Wait a bit before trying again.")
 
-            error_msg += debug_str
+            error_msg = error_msg.format(url=self.last_response.url,
+                                         status_code=self.last_response.status_code) + debug_str
 
         raise AmazonOrdersAuthError(error_msg)
```

### Comparing `amazon-orders-1.0.9/tests/test_cli.py` & `amazon-orders-1.1.0/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import os
 
 import responses
 from click.testing import CliRunner
 
 from amazonorders.cli import amazon_orders_cli
 from amazonorders.constants import ORDER_DETAILS_URL
 from tests.unittestcase import UnitTestCase
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 
 class TestCli(UnitTestCase):
     def setUp(self):
         super().setUp()
 
         self.runner = CliRunner()
 
@@ -63,16 +62,15 @@
         # GIVEN
         order_id = "112-2961628-4757846"
         self.given_login_responses_success()
         with open(os.path.join(self.RESOURCES_DIR, "order-details-112-2961628-4757846.html"), "r",
                   encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}?orderID={}".format(ORDER_DETAILS_URL,
-                                       order_id),
+                f"{ORDER_DETAILS_URL}?orderID={order_id}",
                 body=f.read(),
                 status=200,
             )
 
         # WHEN
         response = self.runner.invoke(amazon_orders_cli,
                                       ["--username", "some-username", "--password",
```

### Comparing `amazon-orders-1.0.9/tests/test_orders.py` & `amazon-orders-1.1.0/tests/test_orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import os
 
 import responses
 
 from amazonorders.constants import ORDER_HISTORY_URL, ORDER_DETAILS_URL
 from amazonorders.exception import AmazonOrdersError
 from amazonorders.orders import AmazonOrders
 from amazonorders.session import AmazonSession
 from tests.unittestcase import UnitTestCase
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 
 class TestOrders(UnitTestCase):
     def setUp(self):
         super().setUp()
 
         self.amazon_session = AmazonSession("some-username", "some-password")
 
@@ -48,20 +47,19 @@
     @responses.activate
     def test_get_order_history_paginated(self):
         # GIVEN
         self.amazon_session.is_authenticated = True
         year = 2010
         resp1 = self.given_order_history_landing_exists()
         resp2 = self.given_order_history_exists(year, 0)
-        with open(os.path.join(self.RESOURCES_DIR, "order-history-{}-10.html".format(year)), "r",
+        with open(os.path.join(self.RESOURCES_DIR, f"order-history-{year}-10.html"), "r",
                   encoding="utf-8") as f:
             resp3 = responses.add(
                 responses.GET,
-                "{}?timeFilter=year-2010&startIndex=10&ref_=ppx_yo2ov_dt_b_pagination_1_2".format(
-                    ORDER_HISTORY_URL, year),
+                f"{ORDER_HISTORY_URL}?timeFilter=year-{year}&startIndex=10&ref_=ppx_yo2ov_dt_b_pagination_1_2",
                 body=f.read(),
                 status=200,
             )
 
         # WHEN
         orders = self.amazon_orders.get_order_history(year=year)
 
@@ -172,19 +170,19 @@
         self.assertEqual(10, resp3.call_count)
 
     @responses.activate
     def test_get_order(self):
         # GIVEN
         self.amazon_session.is_authenticated = True
         order_id = "112-9685975-5907428"
-        with open(os.path.join(self.RESOURCES_DIR, "order-details-{}.html".format(order_id)), "r",
+        with open(os.path.join(self.RESOURCES_DIR, f"order-details-{order_id}.html"), "r",
                   encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}?orderID={}".format(ORDER_DETAILS_URL, order_id),
+                f"{ORDER_DETAILS_URL}?orderID={order_id}",
                 body=f.read(),
                 status=200,
             )
 
         # WHEN
         order = self.amazon_orders.get_order(order_id)
```

### Comparing `amazon-orders-1.0.9/tests/test_session.py` & `amazon-orders-1.1.0/tests/test_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import os
 import sys
 import unittest
 from unittest.mock import patch
 
 import responses
 from responses.matchers import query_string_matcher, urlencoded_params_matcher
 
 from amazonorders.constants import BASE_URL, SIGN_IN_REDIRECT_URL
 from amazonorders.exception import AmazonOrdersAuthError
 from amazonorders.session import AmazonSession
 from tests.unittestcase import UnitTestCase
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.7"
-
 
 class TestSession(UnitTestCase):
     def setUp(self):
         super().setUp()
 
         self.amazon_session = AmazonSession("some-username",
                                             "some-password")
@@ -37,15 +36,15 @@
 
     @responses.activate
     def test_login_invalid_username(self):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-invalid-email.html"), "r", encoding="utf-8") as f:
             resp2 = responses.add(
                 responses.POST,
                 SIGN_IN_REDIRECT_URL,
@@ -64,15 +63,15 @@
 
     @responses.activate
     def test_login_invalid_password(self):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-invalid-password.html"), "r", encoding="utf-8") as f:
             resp2 = responses.add(
                 responses.POST,
                 SIGN_IN_REDIRECT_URL,
@@ -92,15 +91,15 @@
     @responses.activate
     @patch('builtins.input')
     def test_mfa(self, input_mock):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-mfa.html"), "r", encoding="utf-8") as f:
             resp2 = responses.add(
                 responses.POST,
                 SIGN_IN_REDIRECT_URL,
@@ -128,15 +127,15 @@
     @responses.activate
     @patch('builtins.input')
     def test_new_otp(self, input_mock):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-new-otp.html"), "r", encoding="utf-8") as f:
             resp2 = responses.add(
                 responses.POST,
                 SIGN_IN_REDIRECT_URL,
@@ -171,28 +170,28 @@
 
     @responses.activate
     def test_captcha_1(self):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         resp2 = responses.add(
             responses.POST,
             SIGN_IN_REDIRECT_URL,
             status=302,
-            headers={"Location": "{}/ap/cvf/request".format(BASE_URL)}
+            headers={"Location": f"{BASE_URL}/ap/cvf/request"}
         )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-captcha-1.html"), "r", encoding="utf-8") as f:
             resp3 = responses.add(
                 responses.GET,
-                "{}/ap/cvf/request".format(BASE_URL),
+                f"{BASE_URL}/ap/cvf/request",
                 body=f.read(),
                 status=200
             )
         with open(os.path.join(self.RESOURCES_DIR, "captcha_easy.jpg"), "rb") as f:
             resp4 = responses.add(
                 responses.GET,
                 "https://opfcaptcha-prod.s3.amazonaws.com/d32ff4fa043d4f969a1693adfb5d663a.jpg",
@@ -200,29 +199,34 @@
                 headers={"Content-Type": "image/jpeg"},
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "order-history-2018-0.html"), "r", encoding="utf-8") as f:
             request_data = {
                 "clientContext": "132-7968344-2156059",
                 "cvf_captcha_captcha_action": "verifyCaptcha",
-                "cvf_captcha_captcha_token": "sEusNpCt1AQ2rRr2f39/fwAAAAAAAAABPjglplbzE96xUsCT0ZswRq/pkFbblKXbv1cN6hKjq04HzZIYdTBAsdTA9fOZZZsAXG/6qLx8k6IQ8N5gpuIxjtQRhgYiPGzs/b0x0UO9BpFhRTd5JGaUlxx3NdvsaBvaaCDpiGc3E6pzcmhqzqGOuMYMNCP0hLh1u1c+y+6xpzgSr9UYDWHZ9da61HQ8B/ay90YCc5vbiH556wwYffTosLN9LJzCydLp+zzJ2gU1NjWfGyDYvIWYt2h6dCxxJe1jIztakaLnkkJhYQEzHZMC9az8M0S+Yr87/IMh0m9/QMERYs+/cDlUT4jVsqii1qEt/m7pfJMz3G4f",
+                "cvf_captcha_captcha_token": "sEusNpCt1AQ2rRr2f39/fwAAAAAAAAABPjglplbzE96xUsCT0ZswRq/pkFbblKXbv1cN6"
+                                             "hKjq04HzZIYdTBAsdTA9fOZZZsAXG/6qLx8k6IQ8N5gpuIxjtQRhgYiPGzs/b0x0UO9Bp"
+                                             "FhRTd5JGaUlxx3NdvsaBvaaCDpiGc3E6pzcmhqzqGOuMYMNCP0hLh1u1c+y+6xpzgSr9U"
+                                             "YDWHZ9da61HQ8B/ay90YCc5vbiH556wwYffTosLN9LJzCydLp+zzJ2gU1NjWfGyDYvIWY"
+                                             "t2h6dCxxJe1jIztakaLnkkJhYQEzHZMC9az8M0S+Yr87/IMh0m9/QMERYs+/cDlUT4jVs"
+                                             "qii1qEt/m7pfJMz3G4f",
                 "cvf_captcha_captcha_type": "imageCaptcha",
                 "cvf_captcha_input": "FBJRAC",
                 "cvf_captcha_js_enabled_metric": "0",
                 "openid.assoc_handle": "usflex",
                 "openid.mode": "checkid_setup",
                 "openid.ns": "http://specs.openid.net/auth/2.0",
                 "openid.pape.max_auth_age": "900",
                 "openid.return_to": "https://www.amazon.com?",
                 "pageId": "usflex",
                 "verifyToken": "s|71202aba-23dd-378a-9cb3-75f90b00933e"
             }
             resp5 = responses.add(
                 responses.POST,
-                "{}/ap/cvf/verify".format(BASE_URL),
+                f"{BASE_URL}/ap/cvf/verify",
                 body=f.read(),
                 status=200,
                 match=[urlencoded_params_matcher(request_data)],
             )
 
         # WHEN
         self.amazon_session.login()
@@ -237,15 +241,15 @@
 
     @responses.activate
     def test_captcha_2(self):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-captcha-2.html"), "r", encoding="utf-8") as f:
             resp2 = responses.add(
                 responses.POST,
                 SIGN_IN_REDIRECT_URL,
@@ -259,19 +263,22 @@
                 body=f.read(),
                 headers={"Content-Type": "image/jpeg"},
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "order-history-2018-0.html"), "r", encoding="utf-8") as f:
             resp4 = responses.add(
                 responses.GET,
-                "{}/errors/validateCaptcha".format(BASE_URL),
+                f"{BASE_URL}/errors/validateCaptcha",
                 body=f.read(),
                 status=200,
                 match=[query_string_matcher(
-                    "amzn=Ozn2ONrAzGQc1ZETILqvvA%3D%3D&amzn-r=%2Fap%2Fsignin%3Fopenid.pape.max_auth_age%3D900%26openid.return_to%3Dhttps%253A%252F%252Fwww.amazon.com%253F%26openid.assoc_handle%3Dusflex%26openid.mode%3Dcheckid_setup%26openid.ns%3Dhttp%253A%252F%252Fspecs.openid.net%252Fauth%252F2.0&amzn-pt=AuthenticationPortal&field-keywords=FBJRAC")],
+                    "amzn=Ozn2ONrAzGQc1ZETILqvvA%3D%3D&amzn-r=%2Fap%2Fsignin%3Fopenid.pape.max_auth_age%3D900%26"
+                    "openid.return_to%3Dhttps%253A%252F%252Fwww.amazon.com%253F%26openid.assoc_handle%3Dusflex%2"
+                    "6openid.mode%3Dcheckid_setup%26openid.ns%3Dhttp%253A%252F%252Fspecs.openid.net%252Fauth%252"
+                    "F2.0&amzn-pt=AuthenticationPortal&field-keywords=FBJRAC")],
             )
 
         # WHEN
         self.amazon_session.login()
 
         # THEN
         self.assertTrue(self.amazon_session.is_authenticated)
@@ -284,43 +291,43 @@
     @responses.activate
     @patch('builtins.input')
     def test_captcha_1_hard(self, input_mock):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         resp2 = responses.add(
             responses.POST,
             SIGN_IN_REDIRECT_URL,
             status=302,
-            headers={"Location": "{}/ap/cvf/request".format(BASE_URL)}
+            headers={"Location": f"{BASE_URL}/ap/cvf/request"}
         )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-captcha-1.html"), "r", encoding="utf-8") as f:
             resp3 = responses.add(
                 responses.GET,
-                "{}/ap/cvf/request".format(BASE_URL),
+                f"{BASE_URL}/ap/cvf/request",
                 body=f.read(),
                 status=200
             )
         with open(os.path.join(self.RESOURCES_DIR, "captcha_hard.jpg"), "rb") as f:
             resp4 = responses.add(
                 responses.GET,
                 "https://opfcaptcha-prod.s3.amazonaws.com/d32ff4fa043d4f969a1693adfb5d663a.jpg",
                 body=f.read(),
                 headers={"Content-Type": "image/jpeg"},
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "order-history-2018-0.html"), "r", encoding="utf-8") as f:
             resp5 = responses.add(
                 responses.POST,
-                "{}/ap/cvf/verify".format(BASE_URL),
+                f"{BASE_URL}/ap/cvf/verify",
                 body=f.read(),
                 status=200,
             )
 
         # WHEN
         self.amazon_session.login()
 
@@ -336,29 +343,29 @@
     @responses.activate
     @patch('builtins.input')
     def test_captcha_otp(self, input_mock):
         # GIVEN
         with open(os.path.join(self.RESOURCES_DIR, "signin.html"), "r", encoding="utf-8") as f:
             resp1 = responses.add(
                 responses.GET,
-                "{}/gp/sign-in.html".format(BASE_URL),
+                f"{BASE_URL}/gp/sign-in.html",
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "post-signin-captcha-otp.html"), "r", encoding="utf-8") as f:
             resp2 = responses.add(
                 responses.POST,
                 SIGN_IN_REDIRECT_URL,
                 body=f.read(),
                 status=200,
             )
         with open(os.path.join(self.RESOURCES_DIR, "order-history-2018-0.html"), "r", encoding="utf-8") as f:
             resp3 = responses.add(
                 responses.POST,
-                "{}/ap/cvf/approval/verifyOtp".format(BASE_URL),
+                f"{BASE_URL}/ap/cvf/approval/verifyOtp",
                 body=f.read(),
                 status=200,
             )
 
         # WHEN
         self.amazon_session.login()
```

### Comparing `amazon-orders-1.0.9/tests/testcase.py` & `amazon-orders-1.1.0/tests/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+__copyright__ = "Copyright (c) 2024 Alex Laird"
+__license__ = "MIT"
+
 import unittest
 from datetime import date
 
-__author__ = "Alex Laird"
-__copyright__ = "Copyright 2024, Alex Laird"
-__version__ = "1.0.5"
-
 
 class TestCase(unittest.TestCase):
     def assert_order_112_0399923_3070642(self, order, full_details):
         self.assertEqual(34.01, order.grand_total)
         self.assertEqual("112-0399923-3070642", order.order_number)
         self.assertIsNotNone(order.order_details_link)
         self.assertEqual(date(2018, 12, 21), order.order_placed_date)
@@ -154,22 +153,24 @@
         self.assertEqual(2, len(order.items))
         found_cadeya = False
         found_amazon = False
         for order_item in order.items:
             if "Cadeya" in order_item.title:
                 found_cadeya = True
                 self.assertEqual(
-                    "Cadeya Egg Cleaning Brush Silicone, Egg Scrubber for Fresh Eggs, Reusable Cleaning Tools for Egg Washer (Pink)",
+                    "Cadeya Egg Cleaning Brush Silicone, Egg Scrubber for Fresh Eggs, Reusable Cleaning Tools "
+                    "for Egg Washer (Pink)",
                     order_item.title)
                 self.assertIsNotNone(order_item.link)
                 self.assertEqual(date(2024, 1, 31), order_item.return_eligible_date)
             else:
                 found_amazon = True
                 self.assertEqual(
-                    "Swiffer WetJet Hardwood and Floor Spray Mop Cleaner Starter Kit, Includes: 1 Power Mop, 10 Pads, Cleaning Solution, Batteries",
+                    "Swiffer WetJet Hardwood and Floor Spray Mop Cleaner Starter Kit, Includes: 1 Power Mop, "
+                    "10 Pads, Cleaning Solution, Batteries",
                     order_item.title)
                 self.assertIsNotNone(order_item.link)
                 self.assertEqual(date(2024, 1, 31), order_item.return_eligible_date)
         self.assertTrue(found_cadeya)
         self.assertTrue(found_amazon)
 
         self.assertEqual(order.full_details, full_details)
@@ -212,23 +213,25 @@
                          str(order.shipments[0].items))
         found_aaa = False
         found_aa = False
         for item in order.items:
             if "AAA" in item.title:
                 found_aaa = True
                 self.assertEqual(
-                    "AmazonBasics 36 Pack AAA High-Performance Alkaline Batteries, 10-Year Shelf Life, Easy to Open Value Pack",
+                    "AmazonBasics 36 Pack AAA High-Performance Alkaline Batteries, 10-Year Shelf Life, Easy to "
+                    "Open Value Pack",
                     item.title)
                 self.assertIsNotNone(item.link)
                 # TODO: this actually is shown on the page, it's just collapsed, find a way to parse it
                 self.assertIsNone(item.return_eligible_date)
             else:
                 found_aa = True
                 self.assertEqual(
-                    "AmazonBasics 48 Pack AA High-Performance Alkaline Batteries, 10-Year Shelf Life, Easy to Open Value Pack",
+                    "AmazonBasics 48 Pack AA High-Performance Alkaline Batteries, 10-Year Shelf Life, Easy to "
+                    "Open Value Pack",
                     item.title)
                 self.assertIsNotNone(item.link)
                 # TODO: this actually is shown on the page, it's just collapsed, find a way to parse it
                 self.assertIsNone(item.return_eligible_date)
         self.assertTrue(found_aaa)
         self.assertTrue(found_aa)
```

