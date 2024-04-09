# Comparing `tmp/cheroot-8.6.0.tar.gz` & `tmp/cheroot-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheroot-8.6.0.tar", last modified: Tue Jan  4 01:03:01 2022, max compression
+gzip compressed data, was "cheroot-9.0.0.tar", last modified: Sat Nov 19 17:31:55 2022, max compression
```

## Comparing `cheroot-8.6.0.tar` & `cheroot-9.0.0.tar`

### file list

```diff
@@ -1,129 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.930219 cheroot-8.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-04 01:02:46.000000 cheroot-8.6.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-01-04 01:02:46.000000 cheroot-8.6.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (121)     9126 2022-01-04 01:02:46.000000 cheroot-8.6.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-04 01:02:46.000000 cheroot-8.6.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-01-04 01:02:46.000000 cheroot-8.6.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.922219 cheroot-8.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.922219 cheroot-8.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/ISSUE_TEMPLATE/Bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/ISSUE_TEMPLATE/Feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.922219 cheroot-8.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/workflows/bad-commit-message-blocker.yml
--rw-r--r--   0 runner    (1001) docker     (121)    25428 2022-01-04 01:02:46.000000 cheroot-8.6.0/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-01-04 01:02:46.000000 cheroot-8.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-01-04 01:02:46.000000 cheroot-8.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19057 2022-01-04 01:02:46.000000 cheroot-8.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-04 01:02:46.000000 cheroot-8.6.0/.pyup.yml
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-01-04 01:02:46.000000 cheroot-8.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-01-04 01:02:46.000000 cheroot-8.6.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-01-04 01:02:46.000000 cheroot-8.6.0/.zuul.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19987 2022-01-04 01:02:46.000000 cheroot-8.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-01-04 01:02:46.000000 cheroot-8.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-01-04 01:03:01.930219 cheroot-8.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-01-04 01:02:46.000000 cheroot-8.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.922219 cheroot-8.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3477 2022-01-04 01:02:46.000000 cheroot-8.6.0/bin/pip-wrapper
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-04 01:02:46.000000 cheroot-8.6.0/bindep.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.926219 cheroot-8.6.0/cheroot/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14723 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/connections.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/connections.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    16368 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/makefile.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/makefile.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    76777 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/server.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.926219 cheroot-8.6.0/cheroot/ssl/
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/ssl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    18045 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/ssl/builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/ssl/builtin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13339 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/ssl/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/ssl/pyopenssl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.930219 cheroot-8.6.0/cheroot/test/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test__compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    43739 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (121)    14652 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_makefile.py
--rw-r--r--   0 runner    (1001) docker     (121)    12813 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    23991 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/test_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (121)    19205 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/test/webtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/testing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.930219 cheroot-8.6.0/cheroot/workers/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/workers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10700 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/workers/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/workers/threadpool.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14870 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-01-04 01:02:46.000000 cheroot-8.6.0/cheroot/wsgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.926219 cheroot-8.6.0/cheroot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-01-04 01:03:01.000000 cheroot-8.6.0/cheroot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-01-04 01:03:01.000000 cheroot-8.6.0/cheroot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-04 01:03:01.000000 cheroot-8.6.0/cheroot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-04 01:03:01.000000 cheroot-8.6.0/cheroot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-01-04 01:03:01.000000 cheroot-8.6.0/cheroot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-04 01:03:01.000000 cheroot-8.6.0/cheroot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.930219 cheroot-8.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/devguide.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.930219 cheroot-8.6.0/docs/pkg/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/pkg/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/scm_tag_titles_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/spelling_stub_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-01-04 01:02:46.000000 cheroot-8.6.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-04 01:02:46.000000 cheroot-8.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-01-04 01:02:46.000000 cheroot-8.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-01-04 01:02:46.000000 cheroot-8.6.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 01:03:01.930219 cheroot-8.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/dist-build-constraints.in
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/dist-build-constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-build-dists-cp310-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-build-dists-cp310-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-build-dists-cp39-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-build-dists-cp39-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-build-dists.in
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-pre-commit-cp310-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-pre-commit-cp310-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-pre-commit-cp39-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-pre-commit-cp39-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-pre-commit.in
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-py27-cp27-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)     4850 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-py27-cp27-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-py310-cp310-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)     3376 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-py310-cp310-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-py39-cp39-linux-x86_64.in
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-01-04 01:02:46.000000 cheroot-8.6.0/requirements/tox-py39-cp39-linux-x86_64.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-01-04 01:03:01.934219 cheroot-8.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-01-04 01:02:46.000000 cheroot-8.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     6397 2022-01-04 01:02:46.000000 cheroot-8.6.0/tox.ini
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.794152 cheroot-9.0.0/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      473 2022-11-19 16:41:41.000000 cheroot-9.0.0/.codecov.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      330 2022-09-11 17:35:43.000000 cheroot-9.0.0/.darglint
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    10175 2022-11-19 16:41:41.000000 cheroot-9.0.0/.flake8
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       23 2022-09-11 17:35:43.000000 cheroot-9.0.0/.git_archival.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      163 2022-09-11 17:35:43.000000 cheroot-9.0.0/.gitattributes
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.754661 cheroot-9.0.0/.github/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3214 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1173 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/CONTRIBUTING.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      622 2022-11-19 16:41:41.000000 cheroot-9.0.0/.github/FUNDING.yml
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.755179 cheroot-9.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1752 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/ISSUE_TEMPLATE/Bug_report.md
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1233 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/ISSUE_TEMPLATE/Feature_request.md
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      577 2022-11-19 16:41:41.000000 cheroot-9.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1341 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1575 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       34 2022-11-19 16:41:41.000000 cheroot-9.0.0/.github/config.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      115 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/patchback.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      917 2022-11-19 16:41:41.000000 cheroot-9.0.0/.github/stale.yml
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.755749 cheroot-9.0.0/.github/workflows/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      410 2022-09-11 17:35:43.000000 cheroot-9.0.0/.github/workflows/bad-commit-message-blocker.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    32649 2022-11-19 17:31:01.000000 cheroot-9.0.0/.github/workflows/ci-cd.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    14223 2022-11-19 16:41:41.000000 cheroot-9.0.0/.github/workflows/pip-tools.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2636 2022-09-11 17:35:43.000000 cheroot-9.0.0/.gitignore
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5367 2022-11-19 16:41:41.000000 cheroot-9.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    19126 2022-11-19 16:41:41.000000 cheroot-9.0.0/.pylintrc
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      907 2022-11-19 16:41:41.000000 cheroot-9.0.0/.readthedocs.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       95 2022-11-19 16:41:41.000000 cheroot-9.0.0/.yamllint
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    20520 2022-11-19 17:31:01.000000 cheroot-9.0.0/CHANGES.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1511 2022-09-11 17:35:43.000000 cheroot-9.0.0/LICENSE.md
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5942 2022-11-19 17:31:55.794283 cheroot-9.0.0/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3971 2022-09-11 17:35:43.000000 cheroot-9.0.0/README.rst
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.756067 cheroot-9.0.0/bin/
+-rwxr-xr-x   0 jaraco   (697332) primarygroup (89939)      716 2022-09-11 17:35:43.000000 cheroot-9.0.0/bin/pip-wrapper
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3035 2022-09-11 17:35:43.000000 cheroot-9.0.0/bin/pip_constraint_helpers.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.759837 cheroot-9.0.0/cheroot/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      284 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       17 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/__init__.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      109 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/__main__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2046 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/_compat.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      588 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/_compat.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     6987 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/cli.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      828 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/cli.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    14461 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/connections.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      714 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/connections.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2854 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/errors.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      425 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/errors.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2306 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/makefile.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      542 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/makefile.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/py.typed
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    75996 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/server.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4910 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/server.pyi
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.762920 cheroot-9.0.0/cheroot/ssl/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1416 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/ssl/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      555 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/ssl/__init__.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    17906 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/ssl/builtin.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      561 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/ssl/builtin.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    13231 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/ssl/pyopenssl.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1086 2022-11-19 16:41:41.000000 cheroot-9.0.0/cheroot/ssl/pyopenssl.pyi
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.767039 cheroot-9.0.0/cheroot/test/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       26 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/test/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2365 2022-11-19 16:41:41.000000 cheroot-9.0.0/cheroot/test/_pytest_plugin.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2051 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/conftest.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4755 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/helper.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1661 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test__compat.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2664 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_cli.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    43866 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_conn.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    14897 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_core.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1210 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_dispatch.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      868 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/test/test_errors.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1191 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_makefile.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    12949 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_server.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    22508 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/test_ssl.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2823 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/test/test_wsgi.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    18509 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/test/webtest.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4104 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/testing.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      448 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/testing.pyi
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.768042 cheroot-9.0.0/cheroot/workers/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       25 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/workers/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/workers/__init__.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    10594 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/workers/threadpool.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      925 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/workers/threadpool.pyi
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    14178 2022-11-19 17:31:01.000000 cheroot-9.0.0/cheroot/wsgi.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1492 2022-09-11 17:35:43.000000 cheroot-9.0.0/cheroot/wsgi.pyi
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.760787 cheroot-9.0.0/cheroot.egg-info/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5942 2022-11-19 17:31:55.000000 cheroot-9.0.0/cheroot.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     6755 2022-11-19 17:31:55.000000 cheroot-9.0.0/cheroot.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2022-11-19 17:31:55.000000 cheroot-9.0.0/cheroot.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       45 2022-11-19 17:31:55.000000 cheroot-9.0.0/cheroot.egg-info/entry_points.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      385 2022-11-19 17:31:55.000000 cheroot-9.0.0/cheroot.egg-info/requires.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        8 2022-11-19 17:31:55.000000 cheroot-9.0.0/cheroot.egg-info/top_level.txt
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.769856 cheroot-9.0.0/docs/
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.770062 cheroot-9.0.0/docs/_templates/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2274 2022-11-19 17:31:01.000000 cheroot-9.0.0/docs/_templates/python_2_eol.html
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4725 2022-11-19 17:31:01.000000 cheroot-9.0.0/docs/conf.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3602 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/contribute.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      540 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/devguide.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      108 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/history.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      496 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/index.rst
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.770346 cheroot-9.0.0/docs/pkg/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       14 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/pkg/.gitignore
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3312 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/scm_tag_titles_ext.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      701 2022-09-11 17:35:43.000000 cheroot-9.0.0/docs/spelling_stub_ext.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      561 2022-11-19 17:31:01.000000 cheroot-9.0.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      245 2022-11-19 16:41:41.000000 cheroot-9.0.0/mypy.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      315 2022-11-19 16:41:41.000000 cheroot-9.0.0/pyproject.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4616 2022-11-19 17:31:01.000000 cheroot-9.0.0/pytest.ini
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-11-19 17:31:55.793960 cheroot-9.0.0/requirements/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      271 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/dist-build-constraints.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      745 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/dist-build-constraints.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tests.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       15 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-dists-cp310-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      478 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-dists-cp310-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       15 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-dists-cp311-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      672 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-build-dists-cp311-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       15 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-dists-cp39-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      474 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-dists-cp39-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       15 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-dists.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      226 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-build-docs-cp310-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4500 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-docs-cp310-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      226 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-build-docs-cp311-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5016 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-build-docs-cp311-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      226 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-build-docs-cp38-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4582 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-docs-cp38-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      226 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-build-docs-cp39-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4491 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-build-docs-cp39-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       48 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-docs-linkcheck.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      226 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-docs.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       48 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp310-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4536 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp310-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       48 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp311-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5001 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp311-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       48 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp38-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4623 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp38-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       48 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp39-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4532 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-linkcheck-docs-cp39-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      411 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-pre-commit-cp310-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1814 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-pre-commit-cp310-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      411 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-pre-commit-cp311-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1784 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pre-commit-cp311-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      411 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-pre-commit-cp39-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1804 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-pre-commit-cp39-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      411 2022-09-11 17:35:43.000000 cheroot-9.0.0/requirements/tox-pre-commit.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py27-cp27-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5039 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py27-cp27-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py27-cp27-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     5016 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py27-cp27-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py27-cp27-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4874 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py27-cp27-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py310-cp310-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3733 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py310-cp310-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py310-cp310-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3712 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py310-cp310-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py310-cp310-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3548 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py310-cp310-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py311-cp311-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3701 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py311-cp311-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py311-cp311-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3680 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py311-cp311-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py311-cp311-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3516 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py311-cp311-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py34-cp34-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2962 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py34-cp34-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py35-cp35-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4182 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py35-cp35-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py35-cp35-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4159 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py35-cp35-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py35-cp35-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4054 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py35-cp35-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py36-cp36-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3786 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py36-cp36-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py36-cp36-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3765 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py36-cp36-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py36-cp36-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3603 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py36-cp36-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py37-cp37-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3972 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py37-cp37-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py37-cp37-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3951 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py37-cp37-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py37-cp37-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3789 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py37-cp37-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py38-cp38-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3783 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py38-cp38-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py38-cp38-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3762 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py38-cp38-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py38-cp38-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3600 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py38-cp38-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py39-cp39-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3690 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py39-cp39-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py39-cp39-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3669 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py39-cp39-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py39-cp39-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3507 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-py39-cp39-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy27-pp27-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4990 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy27-pp27-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy27-pp27-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4967 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy27-pp27-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy27-pp27-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4823 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy27-pp27-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy36-pp36-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3964 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy36-pp36-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy36-pp36-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3799 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy36-pp36-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy37-pp37-darwin-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4172 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy37-pp37-darwin-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy37-pp37-linux-x86_64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4150 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy37-pp37-linux-x86_64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3386 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy37-pp37-win32-amd64.in
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3985 2022-11-19 16:41:41.000000 cheroot-9.0.0/requirements/tox-pypy37-pp37-win32-amd64.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2463 2022-11-19 17:31:55.794687 cheroot-9.0.0/setup.cfg
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      157 2022-09-11 17:35:43.000000 cheroot-9.0.0/setup.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1857 2022-09-11 17:35:43.000000 cheroot-9.0.0/stubtest_allowlist.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     7899 2022-11-19 16:41:41.000000 cheroot-9.0.0/tox.ini
```

### Comparing `cheroot-8.6.0/.flake8` & `cheroot-9.0.0/.flake8`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,35 @@
   # Metadata of `pip wheel` cmd is autogenerated
   pip-wheel-metadata,
 
 # IMPORTANT: avoid using ignore option, always use extend-ignore instead
 # Completely and unconditionally ignore the following errors:
 extend-ignore =
   # Legitimate cases, no need to "fix" these violations:
+  E501,  # "line too long", its function is replaced by `flake8-length`
+  W505,  # "doc line too long", its function is replaced by `flake8-length`
+  I  # flake8-isort is drunk + we have isort integrated into pre-commit
   WPS326  # "Found implicit string concatenation" -- nothing bad about this
 
+  # FIXME: These `flake8-annotations` errors need fixing and removal
+  ANN001,  # Missing type annotation for function argument 'argv'
+  ANN002,  # Missing type annotation for *exceptions
+  ANN003,  # Missing type annotation for **kwargs
+  ANN101,  # Missing type annotation for self in method
+  ANN102,  # Missing type annotation for cls in classmethod
+  ANN201,  # Missing return type annotation for public function
+  ANN202,  # Missing return type annotation for protected function
+  ANN204,  # Missing return type annotation for special method
+  ANN205,  # Missing return type annotation for staticmethod
+  ANN206,  # Missing return type annotation for classmethod
+
+  # FIXME: These `flake8-annotations` errors need fixing and removal
+  SC100,  # Possibly misspelt word / comments
+  SC200,  # Possibly misspelt word / names
+
 # https://wemake-python-stylegui.de/en/latest/pages/usage/formatter.html
 #format = wemake
 
 # Let's not overcomplicate the code:
 max-complexity = 10
 
 # Accessibility/large fonts and PEP8 friendly:
```

### Comparing `cheroot-8.6.0/.github/CODE_OF_CONDUCT.md` & `cheroot-9.0.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.github/CONTRIBUTING.rst` & `cheroot-9.0.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.github/ISSUE_TEMPLATE/Bug_report.md` & `cheroot-9.0.0/.github/ISSUE_TEMPLATE/Bug_report.md`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.github/ISSUE_TEMPLATE/Feature_request.md` & `cheroot-9.0.0/.github/ISSUE_TEMPLATE/Feature_request.md`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.github/ISSUE_TEMPLATE.md` & `cheroot-9.0.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `cheroot-9.0.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.github/stale.yml` & `cheroot-9.0.0/.github/stale.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+---
+
 # Configuration for probot-stale - https://github.com/probot/stale
 
 
 # Number of days of inactivity before an issue becomes stale
 daysUntilStale: 60
 
 # Number of days of inactivity before a stale issue is closed
 daysUntilClose: 7
 
 # Issues with these labels will never be considered stale
 exemptLabels:
-  - pinned
-  - security
-  - bug
+- pinned
+- security
+- bug
 
 # Label to use when marking an issue as stale
 staleLabel: stale
 
 # Comment to post when marking an issue as stale. Set to `false` to disable
 markComment: >
   This issue has been automatically marked as stale because it has not had
@@ -26,7 +28,9 @@
 unmarkComment: false
 
 # Comment to post when closing a stale issue. Set to `false` to disable
 closeComment: false
 
 # Limit to only `issues` or `pulls`
 # only: issues
+
+...
```

### Comparing `cheroot-8.6.0/.github/workflows/ci-cd.yml` & `cheroot-9.0.0/.github/workflows/ci-cd.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,101 @@
 ---
 name: CI/CD
 
 on:   # yamllint disable-line rule:truthy
   push:
+    branches-ignore:
+    - dependabot/**
+    - maintenance/pip-tools-constraint-lockfiles
+    - maintenance/pip-tools-constraint-lockfiles-**
+    - patchback/backports/**
+    - pre-commit-ci-update-config
   pull_request:
   workflow_dispatch:
     inputs:
       release-version:
         # github.event_name == 'workflow_dispatch'
         # && github.event.inputs.release-version
         description: >-
           Target PEP440-compliant version to release.
           Please, don't prepend `v`.
         required: true
+        type: string
       release-commitish:
         # github.event_name == 'workflow_dispatch'
         # && github.event.inputs.release-commitish
         default: ''
         description: >-
           The commit to be released to PyPI and tagged
           in Git as `release-version`. Normally, you
           should keep this empty.
+        type: string
       YOLO:
         default: false
         description: >-
           Flag whether test results should block the
-          release (true/false). Only use this under
-          extraordinary circumstances to ignore the
-          test failures and cut the release regardless.
+          release. Only use this under extraordinary
+          circumstances to ignore the test failures
+          and cut the release regardless.
+        type: boolean
   schedule:
   - cron: 1 0 * * *  # Run daily at 0:01 UTC
 
 concurrency:
   group: >-
     ${{
         github.workflow
     }}-${{
+        github.ref_type
+    }}-${{
         github.event.pull_request.number || github.sha
     }}
   cancel-in-progress: true
 
+env:
+  FORCE_COLOR: 1  # Request colored output from CLI tools supporting it
+  MYPY_FORCE_COLOR: 1  # MyPy's color enforcement
+  PIP_DISABLE_PIP_VERSION_CHECK: 1
+  PIP_NO_PYTHON_VERSION_WARNING: 1
+  PIP_NO_WARN_SCRIPT_LOCATION: 1
+  PY_COLORS: 1  # Recognized by the `py` package, dependency of `pytest`
+  TOX_PARALLEL_NO_SPINNER: 1
+  TOX_TESTENV_PASSENV: >-  # Make tox-wrapped tools see color requests
+    FORCE_COLOR
+    MYPY_FORCE_COLOR
+    NO_COLOR
+    PY_COLORS
+    PYTEST_THEME
+    PYTEST_THEME_MODE
+
+run-name: >-
+  ${{
+    github.event_name == 'workflow_dispatch'
+    && format('📦 Releasing v{0}...', github.event.inputs.release-version)
+    || ''
+  }}
+  ${{
+      github.event.pull_request.number && 'PR' || ''
+  }}${{
+      !github.event.pull_request.number && 'Commit' || ''
+  }}
+  ${{ github.event.pull_request.number || github.sha }}
+  triggered by: ${{ github.event_name }} of ${{
+    github.ref
+  }} ${{
+    github.ref_type
+  }}
+  (workflow run ID: ${{
+    github.run_id
+  }}; number: ${{
+    github.run_number
+  }}; attempt: ${{
+    github.run_attempt
+  }})
+
 jobs:
   pre-setup:
     name: ⚙️ Pre-set global build settings
     runs-on: ubuntu-latest
     defaults:
       run:
         shell: python
@@ -62,80 +114,117 @@
         }}
       cache-key-files: >-
         ${{ steps.calc-cache-key-files.outputs.files-hash-key }}
       git-tag: ${{ steps.git-tag.outputs.tag }}
       sdist-artifact-name: ${{ steps.artifact-name.outputs.sdist }}
       wheel-artifact-name: ${{ steps.artifact-name.outputs.wheel }}
     steps:
-    - name: Switch to using Python 3.10 by default
-      uses: actions/setup-python@v2
+    - name: Switch to using Python 3.11 by default
+      uses: actions/setup-python@v4
       with:
-        python-version: >-
-          3.10
+        python-version: 3.11
     - name: >-
         Mark the build as untagged '${{
             github.event.repository.default_branch
         }}' branch build
       id: untagged-check
       if: >-
         github.event_name == 'push' &&
         github.ref == format(
           'refs/heads/{0}', github.event.repository.default_branch
         )
-      run: >-
-        print('::set-output name=is-untagged-devel::true')
+      run: |
+        from os import environ
+        from pathlib import Path
+
+        FILE_APPEND_MODE = 'a'
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print('is-untagged-devel=true', file=outputs_file)
     - name: Mark the build as "release request"
       id: request-check
       if: github.event_name == 'workflow_dispatch'
-      run: >-
-        print('::set-output name=release-requested::true')
+      run: |
+        from os import environ
+        from pathlib import Path
+
+        FILE_APPEND_MODE = 'a'
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print('release-requested=true', file=outputs_file)
     - name: Check out src from Git
       if: >-
         steps.request-check.outputs.release-requested != 'true'
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
-        fetch-depth: 0
+        fetch-depth: >-
+          ${{
+            steps.request-check.outputs.release-requested == 'true'
+            && 1 || 0
+          }}
         ref: ${{ github.event.inputs.release-commitish }}
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       id: calc-cache-key-py
       run: |
         from hashlib import sha512
+        from os import environ
+        from pathlib import Path
         from sys import version
+
+        FILE_APPEND_MODE = 'a'
+
         hash = sha512(version.encode()).hexdigest()
-        print(f'::set-output name=py-hash-key::{hash}')
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(f'py-hash-key={hash}', file=outputs_file)
     - name: >-
         Calculate dependency files' combined hash value
         for use in the cache key
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       id: calc-cache-key-files
       run: |
-        print(
-          "::set-output name=files-hash-key::${{
-              hashFiles(
-                'setup.cfg', 'setup.py', 'tox.ini', 'pyproject.toml',
-                '.pre-commit-config.yaml', 'pytest.ini'
-              )
-          }}",
-        )
+        from os import environ
+        from pathlib import Path
+
+        FILE_APPEND_MODE = 'a'
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(
+                "files-hash-key=${{
+                    hashFiles(
+                      'setup.cfg', 'setup.py', 'tox.ini', 'pyproject.toml',
+                      '.pre-commit-config.yaml', 'pytest.ini'
+                    )
+                }}",
+                file=outputs_file,
+            )
     - name: Get pip cache dir
       id: pip-cache-dir
       if: >-
         steps.request-check.outputs.release-requested != 'true'
       run: >-
-        echo "::set-output name=dir::$(python -m pip cache dir)"
+        echo "dir=$(python -m pip cache dir)" >> "${GITHUB_OUTPUT}"
       shell: bash
     - name: Set up pip cache
       if: >-
         steps.request-check.outputs.release-requested != 'true'
-      uses: actions/cache@v2.1.7
+      uses: actions/cache@v3
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           steps.calc-cache-key-files.outputs.files-hash-key }}
         restore-keys: |
@@ -161,43 +250,77 @@
         --user
         setuptools-scm
       shell: bash
     - name: Set the current dist version from Git
       if: steps.request-check.outputs.release-requested != 'true'
       id: scm-version
       run: |
+        from os import environ
+        from pathlib import Path
+
         import setuptools_scm
+
+        FILE_APPEND_MODE = 'a'
+
         ver = setuptools_scm.get_version(
           ${{
               steps.untagged-check.outputs.is-untagged-devel == 'true'
               && 'local_scheme="no-local-version"' || ''
           }}
         )
-        print('::set-output name=dist-version::{ver}'.format(ver=ver))
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(f'dist-version={ver}', file=outputs_file)
     - name: Set the target Git tag
       id: git-tag
-      run: >-
-        print('::set-output name=tag::v${{
-            steps.request-check.outputs.release-requested == 'true'
-            && github.event.inputs.release-version
-            || steps.scm-version.outputs.dist-version
-        }}')
+      run: |
+        from os import environ
+        from pathlib import Path
+
+        FILE_APPEND_MODE = 'a'
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(
+                "tag=v${{
+                    steps.request-check.outputs.release-requested == 'true'
+                    && github.event.inputs.release-version
+                    || steps.scm-version.outputs.dist-version
+                }}",
+                file=outputs_file,
+            )
     - name: Set the expected dist artifact names
       id: artifact-name
       run: |
-        print('::set-output name=sdist::cheroot-${{
-            steps.request-check.outputs.release-requested == 'true'
-            && github.event.inputs.release-version
-            || steps.scm-version.outputs.dist-version
-        }}.tar.gz')
-        print('::set-output name=wheel::cheroot-${{
-            steps.request-check.outputs.release-requested == 'true'
-            && github.event.inputs.release-version
-            || steps.scm-version.outputs.dist-version
-        }}-py2.py3-none-any.whl')
+        from os import environ
+        from pathlib import Path
+
+        FILE_APPEND_MODE = 'a'
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(
+                "sdist=cheroot-${{
+                    steps.request-check.outputs.release-requested == 'true'
+                    && github.event.inputs.release-version
+                    || steps.scm-version.outputs.dist-version
+                }}.tar.gz",
+                file=outputs_file,
+            )
+            print(
+                "wheel=cheroot-${{
+                    steps.request-check.outputs.release-requested == 'true'
+                    && github.event.inputs.release-version
+                    || steps.scm-version.outputs.dist-version
+                }}-py2.py3-none-any.whl",
+                file=outputs_file,
+            )
 
   build:
     name: >-
       👷 dists ${{ needs.pre-setup.outputs.git-tag }}
       [mode: ${{
         fromJSON(needs.pre-setup.outputs.is-untagged-devel)
         && 'nightly' || ''
@@ -209,44 +332,60 @@
           !fromJSON(needs.pre-setup.outputs.is-untagged-devel)
           && !fromJSON(needs.pre-setup.outputs.release-requested)
         ) && 'test' || ''
       }}]
     needs:
     - pre-setup  # transitive, for accessing settings
 
-    runs-on: Ubuntu-latest
+    runs-on: ubuntu-latest
 
     env:
-      PY_COLORS: 1
-      TOX_PARALLEL_NO_SPINNER: 1
       TOXENV: cleanup-dists,build-dists
 
     steps:
-    - name: Switch to using Python v3.10
-      uses: actions/setup-python@v2
+    - name: Switch to using Python 3.11
+      uses: actions/setup-python@v4
       with:
-        python-version: >-
-          3.10
+        python-version: 3.11
+
+    - name: Grab the source from Git
+      uses: actions/checkout@v3
+      with:
+        fetch-depth: >-
+          ${{
+              fromJSON(needs.pre-setup.outputs.release-requested)
+              && 1 || 0
+          }}
+        ref: ${{ github.event.inputs.release-commitish }}
+
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
       id: calc-cache-key-py
       run: |
         from hashlib import sha512
+        from os import environ
+        from pathlib import Path
         from sys import version
 
+        FILE_APPEND_MODE = 'a'
+
         hash = sha512(version.encode()).hexdigest()
-        print(f'::set-output name=py-hash-key::{hash}')
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(f'py-hash-key={hash}', file=outputs_file)
       shell: python
     - name: Get pip cache dir
       id: pip-cache-dir
       run: >-
-        echo "::set-output name=dir::$(python -m pip cache dir)"
+        echo "dir=$(python -m pip cache dir)" >> "${GITHUB_OUTPUT}"
     - name: Set up pip cache
-      uses: actions/cache@v2.1.5
+      uses: actions/cache@v3
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           needs.pre-setup.outputs.cache-key-files }}
         restore-keys: |
@@ -257,51 +396,80 @@
     - name: Install tox
       run: >-
         python -m
         pip install
         --user
         tox
 
-    - name: Grab the source from Git
-      uses: actions/checkout@v2
-      with:
-        fetch-depth: >-
-          ${{
-              steps.request-check.outputs.release-requested == 'true'
-              && 1 || 0
-          }}
-        ref: ${{ github.event.inputs.release-commitish }}
-
     - name: Pre-populate the tox env
       run: >-
         python -m
         tox
         --parallel auto
         --parallel-live
         --skip-missing-interpreters false
         --notest
 
+    - name: Drop Git tags from HEAD for non-tag-create events
+      if: >-
+        !fromJSON(needs.pre-setup.outputs.release-requested)
+      run: >-
+        git tag --points-at HEAD
+        |
+        xargs git tag --delete
+      shell: bash
+
     - name: Setup git user as [bot]
       if: >-
-        fromJSON(needs.pre-setup.outputs.is-untagged-devel)
-        || fromJSON(needs.pre-setup.outputs.release-requested)
-      uses: fregante/setup-git-user@v1.0.1
+        fromJSON(needs.pre-setup.outputs.release-requested)
+        || fromJSON(needs.pre-setup.outputs.is-untagged-devel)
+      uses: fregante/setup-git-user@v1.1.0
     - name: >-
         Tag the release in the local Git repo
         as ${{ needs.pre-setup.outputs.git-tag }}
         for setuptools-scm to set the desired version
       if: >-
-        fromJSON(needs.pre-setup.outputs.is-untagged-devel)
-        || fromJSON(needs.pre-setup.outputs.release-requested)
+        fromJSON(needs.pre-setup.outputs.release-requested)
       run: >-
         git tag
         -m '${{ needs.pre-setup.outputs.git-tag }}'
         '${{ needs.pre-setup.outputs.git-tag }}'
         --
-        ${{ github.event.inputs.release-commitish }}
+        ${{
+          fromJSON(needs.pre-setup.outputs.release-requested)
+          && github.event.inputs.release-commitish || ''
+        }}
+
+    - name: Install tomlkit Python distribution package
+      if: >-
+        fromJSON(needs.pre-setup.outputs.is-untagged-devel)
+      run: >-
+        python -m pip install --user tomlkit
+    - name: Instruct setuptools-scm not to add a local version part
+      if: >-
+        fromJSON(needs.pre-setup.outputs.is-untagged-devel)
+      run: |
+        from pathlib import Path
+
+        import tomlkit
+
+        pyproject_toml_path = Path.cwd() / 'pyproject.toml'
+        pyproject_toml_txt = pyproject_toml_path.read_text()
+        pyproject_toml = tomlkit.loads(pyproject_toml_txt)
+        setuptools_scm_section = pyproject_toml['tool']['setuptools_scm']
+        setuptools_scm_section['local_scheme'] = 'no-local-version'
+        patched_pyproject_toml_txt = tomlkit.dumps(pyproject_toml)
+        pyproject_toml_path.write_text(patched_pyproject_toml_txt)
+      shell: python
+    - name: Pretend that pyproject.toml is unchanged
+      if: >-
+        fromJSON(needs.pre-setup.outputs.is-untagged-devel)
+      run: |
+        git diff --color=always
+        git update-index --assume-unchanged pyproject.toml
 
     - name: Build dists
       run: >-
         python -m
         tox
         --parallel auto
         --parallel-live
@@ -309,79 +477,96 @@
         --skip-pkg-install
     - name: Verify that the artifacts with expected names got created
       run: >-
         ls -1
         'dist/${{ needs.pre-setup.outputs.sdist-artifact-name }}'
         'dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}'
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: python-package-distributions
         # NOTE: Exact expected file names are specified here
         # NOTE: as a safety measure — if anything weird ends
         # NOTE: up being in this dir or not all dists will be
         # NOTE: produced, this will fail the workflow.
         path: |
           dist/${{ needs.pre-setup.outputs.sdist-artifact-name }}
           dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}
-        retention-days: 30  # Defaults to 90
+        retention-days: >-
+          ${{
+              (
+                fromJSON(needs.pre-setup.outputs.release-requested)
+              ) && 90 || 30
+          }}
 
   lint:
     name: 🧹 ${{ matrix.toxenv }}
     needs:
     - build
     - pre-setup  # transitive, for accessing settings
 
     runs-on: ${{ matrix.os }}-latest
     strategy:
       matrix:
         os:
-        - Ubuntu
+        - ubuntu
         python-version:
         - >-
           3.10
         toxenv:
         - pre-commit
         - setup-check
         - metadata-validation
         - build-docs
         - doctest-docs
         - linkcheck-docs
         - spellcheck-docs
       fail-fast: false
 
     env:
-      PY_COLORS: 1
-      TOX_PARALLEL_NO_SPINNER: 1
       TOXENV: ${{ matrix.toxenv }}
 
     steps:
     - name: >-
         Switch to using Python v${{ matrix.python-version }}
         by default
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+
+    - name: Grab the source from Git
+      uses: actions/checkout@v3
+      with:
+        ref: ${{ github.event.inputs.release-commitish }}
+
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
       id: calc-cache-key-py
       run: |
         from hashlib import sha512
+        from os import environ
+        from pathlib import Path
         from sys import version
 
+        FILE_APPEND_MODE = 'a'
+
         hash = sha512(version.encode()).hexdigest()
-        print(f'::set-output name=py-hash-key::{hash}')
+
+        with Path(environ['GITHUB_OUTPUT']).open(
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(f'py-hash-key={hash}', file=outputs_file)
       shell: python
     - name: Get pip cache dir
       id: pip-cache
       run: >-
-        echo "::set-output name=dir::$(pip cache dir)"
+        echo "dir=$(pip cache dir)" >> "${GITHUB_OUTPUT}"
     - name: Set up pip cache
-      uses: actions/cache@v2.1.7
+      uses: actions/cache@v3
       with:
         path: ${{ steps.pip-cache.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           needs.pre-setup.outputs.cache-key-files }}
         restore-keys: |
@@ -392,44 +577,41 @@
     - name: Install tox
       run: >-
         python -m
         pip install
         --user
         tox
 
-    - name: Grab the source from Git
-      uses: actions/checkout@v2
-      with:
-        ref: ${{ github.event.inputs.release-commitish }}
-
     - name: Make the env clean of non-test files
       if: matrix.toxenv == 'metadata-validation'
       run: |
         shopt -s extglob
         rm -rf !tox.ini
       shell: bash
     - name: Download all the dists
       if: matrix.toxenv == 'metadata-validation'
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
     - name: >-
         Pre-populate tox envs: `${{ env.TOXENV }}`
       run: >-
         python -m
         tox
         --parallel auto
         --parallel-live
         --skip-missing-interpreters false
         --notest
     - name: Initialize pre-commit envs if needed
-      run: |
-        test -d .tox/pre-commit && .tox/pre-commit/bin/python -m pre_commit install-hooks || :
+      run: >-
+        test -d .tox/pre-commit
+        && .tox/pre-commit/bin/python -m pre_commit install-hooks
+        || :
     - name: >-
         Run tox envs: `${{ env.TOXENV }}`
       run: >-
         python -m
         tox
         --parallel auto
         --parallel-live
@@ -449,153 +631,150 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version:
         # NOTE: The latest and the lowest supported Pythons are prioritized
         # NOTE: to improve the responsiveness. It's nice to see the most
         # NOTE: important results first.
-        - '3.10'
-        - pypy2
+        - 3.11
+        - >-
+          3.10
         - 3.9
         - 3.8
         - pypy-3.7
         - 3.7
         - 3.6
-        - 3.5
-        - 2.7
-        - 3.11.0-alpha - 3.11.0
         - pypy-3.6
         os:
         - ubuntu-20.04
         - ubuntu-18.04
-        - macOS-11.0
-        - macOS-latest
-        - windows-latest
-        - windows-2016
+        - macos-11.0
+        - macos-latest
+        - windows-2019
+        - windows-2022
         exclude:
         # NOTE: Windows PyPy jobs are excluded to address the tox bug
         # NOTE: https://github.com/tox-dev/tox/issues/1704.
         # NOTE: They should be re-added once it's fixed.
-        - os: windows-latest
-          python-version: pypy2
-        - os: windows-2016
-          python-version: pypy2
-        - os: windows-latest
+        - os: windows-2022
           python-version: pypy-3.6
-        - os: windows-2016
+        - os: windows-2019
           python-version: pypy-3.6
         # NOTE: Windows PyPy 3.7 jobs are excluded because of the lack
         # NOTE: of the build deps to compile cryptography.
         # NOTE: They should be re-added once it's fixed.
-        - os: windows-latest
+        - os: windows-2022
           python-version: pypy-3.7
-        - os: windows-2016
+        - os: windows-2019
           python-version: pypy-3.7
         # NOTE: macOS PyPy jobs are excluded because installing cryptography
         # NOTE: needs openssl headers that aren't present at the moment.
         # TODO: Remove the exclusions once this is addressed.
         - os: macOS-11.0
-          python-version: pypy2
-        - os: macOS-latest
-          python-version: pypy2
-        - os: macOS-11.0
           python-version: pypy-3.6
-        - os: macOS-latest
+        - os: macos-latest
           python-version: pypy-3.6
-        - os: macOS-11.0
+        - os: macos-11.0
           python-version: pypy-3.7
-        - os: macOS-latest
+        - os: macos-latest
           python-version: pypy-3.7
-        include:
-        # NOTE: The only GNU/Linux CPython 3.4 available is built for Ubuntu 18
-        # https://github.com/actions/python-versions/blob/c483657/versions-manifest.json#L1228
-        - os: ubuntu-18.04
-          python-version: 3.4
 
     continue-on-error: >-
       ${{
           (
             (
-              needs.pre-setup.outputs.release-requested == 'true' &&
-              !toJSON(github.event.inputs.YOLO)
+              fromJSON(needs.pre-setup.outputs.release-requested) &&
+              !github.event.inputs.YOLO
             ) ||
-            contains(matrix.python-version, 'alpha') ||
             (
-              matrix.python-version == '2.7' &&
-              startsWith(matrix.os, 'windows-')
-            )
+              startsWith(matrix.python-version, '~')
+            ) ||
+            contains(matrix.python-version, 'alpha')
           ) && true || false
       }}
 
     env:
       PIP_DISABLE_PIP_VERSION_CHECK: 1
       PIP_NO_PYTHON_VERSION_WARNING: 1
       PIP_NO_WARN_SCRIPT_LOCATION: 1
-      PYTEST_ADDOPTS: >-
-        ${{
-            (
-                matrix.python-version == 'pypy2' &&
-                startsWith(matrix.os, 'ubuntu-')
-            ) &&
-            '-p no:warnings' || ''
-        }}
       PY_COLORS: 1
-      TOXENV: >-
-        ${{
-            (
-                contains(matrix.python-version, 'pypy') &&
-                contains(matrix.python-version, '3')
-            )
-            && 'pypy3'
-            || ''
-        }}${{
-            (
-                contains(matrix.python-version, 'pypy') &&
-                contains(matrix.python-version, '2')
-            )
-            && 'pypy2'
-            || ''
-        }}${{
-            !contains(matrix.python-version, 'pypy')
-            && 'python'
-            || ''
-        }}
-      TOX_PARALLEL_NO_SPINNER: 1
+      TOXENV: python
 
     steps:
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      id: python-install
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+
+    - name: Grab the source from Git
+      uses: actions/checkout@v3
+      with:
+        ref: ${{ github.event.inputs.release-commitish }}
+
+    - name: Figure out if the interpreter ABI is stable
+      id: py-abi
+      run: |
+        from __future__ import print_function
+
+        from os import environ
+        from sys import version_info
+
+        FILE_APPEND_MODE = 'a'
+
+        is_stable_abi = version_info.releaselevel == 'final'
+
+        with open(
+                environ['GITHUB_OUTPUT'],
+                mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print(
+                'is-stable-abi={is_stable_abi}'.
+                format(is_stable_abi=str(is_stable_abi).lower()),
+                file=outputs_file,
+            )
+      shell: python
     - name: >-
         Calculate Python interpreter version hash value
         for use in the cache key
+      if: fromJSON(steps.py-abi.outputs.is-stable-abi)
       id: calc-cache-key-py
       run: |
+        from __future__ import print_function
+
         from hashlib import sha512
+        from os import environ
         from sys import version
 
+        FILE_APPEND_MODE = 'a'
+
         hash = sha512(version.encode()).hexdigest()
-        print('::set-output name=py-hash-key::{hash}'.format(hash=hash))
+
+        with open(
+                environ['GITHUB_OUTPUT'], mode=FILE_APPEND_MODE,
+        ) as outputs_file:
+            print('py-hash-key={hash}'.format(hash=hash), file=outputs_file)
       shell: python
     - name: Get pip cache dir
+      if: fromJSON(steps.py-abi.outputs.is-stable-abi)
       id: pip-cache
       run: |
         set +e
         pip_cache_dir="$(pip cache dir)"
         set -e
         if [ -n "${pip_cache_dir}" ]
         then
-          echo "::set-output name=dir::${pip_cache_dir}"
+          echo "dir=${pip_cache_dir}" >> "${GITHUB_OUTPUT}"
         else  # Python 3.4 under Ubuntu:
-          echo "::set-output name=dir::'~/.cache/pip'"
+          echo "dir='~/.cache/pip'" >> "${GITHUB_OUTPUT}"
         fi
       shell: bash
     - name: Set up pip cache
-      uses: actions/cache@v2.1.7
+      if: fromJSON(steps.py-abi.outputs.is-stable-abi)
+      uses: actions/cache@v3
       with:
         path: ${{ steps.pip-cache.outputs.dir }}
         key: >-
           ${{ runner.os }}-pip-${{
           steps.calc-cache-key-py.outputs.py-hash-key }}-${{
           needs.pre-setup.outputs.cache-key-files }}
         restore-keys: |
@@ -615,28 +794,23 @@
     - name: Install tox
       run: >-
         python -m
         pip install
         --user
         tox
 
-    - name: Grab the source from Git
-      uses: actions/checkout@v2
-      with:
-        ref: ${{ github.event.inputs.release-commitish }}
-
     - name: Download all the dists
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
     - name: >-
-        Pre-populate tox envs:
-        ${{ matrix.env.TOXENV }}
+        Pre-populate tox env:
+        ${{ env.TOXENV }}
       run: >-
         python -m
         tox
         --parallel auto
         --parallel-live
         --skip-missing-interpreters false
         --installpkg 'dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}'
@@ -677,24 +851,49 @@
     - name: Run the testing
       run: >-
         python -m
         tox
         --parallel auto
         --parallel-live
         --skip-missing-interpreters false
-        -vvvv
         --installpkg 'dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}'
+    - name: Produce markdown test summary from JUnit
+      if: always()
+      uses: test-summary/action@v2.0
+      with:
+        paths: .test-results/pytest/test.xml
+    - name: Re-run the failing tests with maximum verbosity
+      if: failure()
+      run: >-  # `exit 1` makes sure that the job remains red with flaky runs
+        python -m
+        tox
+        --parallel auto
+        --parallel-live
+        --skip-missing-interpreters false
+        -vvvvv
+        --installpkg 'dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}'
+        --
+        --no-cov -vvvvv --lf
+        && exit 1
+      shell: bash
     - name: Send coverage data to Codecov
-      uses: codecov/codecov-action@v2
+      uses: codecov/codecov-action@v3
       with:
         files: .test-results/pytest/cov.xml
         flags: >-
-          GHA,
-          ${{ runner.os }},
-          ${{ matrix.python-version }},
+          CI-GHA,
+          OS-${{
+            runner.os
+          }},
+          VM-${{
+            matrix.os
+          }},
+          Py-${{
+            steps.python-install.outputs.python-version
+          }},
           ${{ needs.pre-setup.outputs.wheel-artifact-name }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - lint
@@ -702,65 +901,71 @@
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
-        allowed-failures: docs, linters
+        allowed-failures: >-
+          ${{
+            (
+              fromJSON(needs.pre-setup.outputs.release-requested)
+              && github.event.inputs.YOLO
+            ) && 'lint, tests' || ''
+          }}
         jobs: ${{ toJSON(needs) }}
 
   publish-pypi:
     name: Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to PyPI
     needs:
     - check
     - pre-setup  # transitive, for accessing settings
     if: >-
       fromJSON(needs.pre-setup.outputs.release-requested)
-    runs-on: Ubuntu-latest
+    runs-on: ubuntu-latest
 
     environment:
       name: pypi
       url: >-
         https://pypi.org/project/cheroot/${{
           needs.pre-setup.outputs.dist-version
         }}
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: >-
         Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: ${{ secrets.PYPI_TOKEN }}
+        password: ${{ secrets.PYPI_API_TOKEN }}
 
   publish-testpypi:
     name: Publish 🐍📦 ${{ needs.pre-setup.outputs.git-tag }} to TestPyPI
     needs:
     - check
     - pre-setup  # transitive, for accessing settings
     if: >-
       fromJSON(needs.pre-setup.outputs.is-untagged-devel)
       || fromJSON(needs.pre-setup.outputs.release-requested)
-    runs-on: Ubuntu-latest
+    runs-on: ubuntu-latest
 
     environment:
       name: testpypi
       url: >-
         https://test.pypi.org/project/cheroot/${{
           needs.pre-setup.outputs.dist-version
         }}
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: >-
         Publish 🐍📦  ${{ needs.pre-setup.outputs.git-tag }} to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
@@ -770,72 +975,116 @@
   post-release-repo-update:
     name: >-
       Publish post-release Git tag
       for ${{ needs.pre-setup.outputs.git-tag }}
     needs:
     - publish-pypi
     - pre-setup  # transitive, for accessing settings
-    runs-on: Ubuntu-latest
+    runs-on: ubuntu-latest
 
     steps:
+    - name: >-
+        Check if the requested tag ${{ needs.pre-setup.outputs.git-tag }}
+        is present and is pointing at the required commit ${{
+          github.event.inputs.release-commitish
+        }}
+      id: existing-remote-tag-check
+      run: |
+        REMOTE_TAGGED_COMMIT_SHA="$(
+          git ls-remote --tags --refs $(git remote get-url origin) '${{
+            needs.pre-setup.outputs.git-tag
+          }}' | awk '{print $1}'
+        )"
+
+        if [[ "${REMOTE_TAGGED_COMMIT_SHA}" == '${{
+          github.event.inputs.release-commitish
+        }}' ]]
+        then
+          echo "already-exists=true" >> "${GITHUB_OUTPUT}"
+        fi
+
     - name: Fetch the src snapshot
-      uses: actions/checkout@v2
+      if: steps.existing-remote-tag-check.outputs.already-exists == 'true'
+      uses: actions/checkout@v3
       with:
         fetch-depth: 1
         ref: ${{ github.event.inputs.release-commitish }}
     - name: Setup git user as [bot]
-      uses: fregante/setup-git-user@v1.0.1
+      if: steps.existing-remote-tag-check.outputs.already-exists == 'true'
+      uses: fregante/setup-git-user@v1.1.0
 
     - name: >-
         Tag the release in the local Git repo
-        as v${{ needs.pre-setup.outputs.git-tag }}
+        as ${{ needs.pre-setup.outputs.git-tag }}
+      if: steps.existing-remote-tag-check.outputs.already-exists == 'true'
       run: >-
         git tag
         -m '${{ needs.pre-setup.outputs.git-tag }}'
+        -m 'Published at https://pypi.org/project/cheroot/${{
+          needs.pre-setup.outputs.dist-version
+        }}'
         '${{ needs.pre-setup.outputs.git-tag }}'
         --
         ${{ github.event.inputs.release-commitish }}
     - name: >-
         Push ${{ needs.pre-setup.outputs.git-tag }} tag corresponding
         to the just published release back to GitHub
+      if: steps.existing-remote-tag-check.outputs.already-exists == 'true'
       run: >-
         git push --atomic origin '${{ needs.pre-setup.outputs.git-tag }}'
 
   publish-github-release:
     name: >-
       Publish a GitHub Release for
       ${{ needs.pre-setup.outputs.git-tag }}
     needs:
     - post-release-repo-update
     - pre-setup  # transitive, for accessing settings
-    runs-on: Ubuntu-latest
+    runs-on: ubuntu-latest
 
     permissions:
       contents: write
       discussions: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
     - name: >-
         Publish a GitHub Release for
         ${{ needs.pre-setup.outputs.git-tag }}
-      uses: ncipollo/release-action@v1.9.0
+      uses: ncipollo/release-action@v1.11.1
       with:
         allowUpdates: false
         artifactErrorsFailBuild: false
         artifacts: |
           dist/${{ needs.pre-setup.outputs.sdist-artifact-name }}
           dist/${{ needs.pre-setup.outputs.wheel-artifact-name }}
         artifactContentType: raw  # Because whl and tgz are of different types
-        # body/bodyFile:  # FIXME: Use once Towncrier is integrated.
+        body: >
+          # Release ${{ needs.pre-setup.outputs.git-tag }}
+
+
+          This release is published to
+          https://pypi.org/project/cheroot/${{
+            needs.pre-setup.outputs.dist-version
+          }}.
+
+
+          This release has been produced by the following workflow run: ${{
+            github.server_url
+          }}/${{
+            github.repository
+          }}/actions/runs/${{
+            github.run_id
+          }}.
+        # bodyFile:  # FIXME: Use once Towncrier is integrated.
         commit: ${{ github.event.inputs.release-commitish }}
         discussionCategory: Announcements
         draft: false
         name: ${{ needs.pre-setup.outputs.git-tag }}
         # omitBody: false
         omitBodyDuringUpdate: true
         omitName: false
```

### Comparing `cheroot-8.6.0/.gitignore` & `cheroot-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/.pylintrc` & `cheroot-9.0.0/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
-load-plugins=pylint_pytest
+load-plugins =
+  # "stdlib":
+  pylint.extensions.no_self_use,
+  # third-party:
+  pylint_pytest,
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Min Python version to use for version dependend checks. Will default to the
 # version used to run pylint.
 py-version=3.9
```

### Comparing `cheroot-8.6.0/.readthedocs.yml` & `cheroot-9.0.0/.readthedocs.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+---
+
 # .readthedocs.yml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html
 # for details
 
 # Required
 version: 2
@@ -9,36 +11,36 @@
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   builder: dirhtml
   configuration: docs/conf.py
   fail_on_warning: true
 
 # Build documentation with MkDocs
-#mkdocs:
-#  configuration: mkdocs.yml
-#  fail_on_warning: true
+# mkdocs:
+#   configuration: mkdocs.yml
+#   fail_on_warning: true
 
 # Optionally build your docs in additional formats
 # such as PDF and ePub
 formats: []
 
 submodules:
   include: all  # []
   exclude: []
   recursive: true
 
 build:
   os: ubuntu-20.04
   tools:
-    python: >-  # PyYAML parses it as float `3.1` if it's not an explicit str
-      3.10
+    python: >-  # PyYAML parses it as float but RTD demands an explicit string
+      3.11
 
 # Optionally set the version of Python and requirements required
 # to build docs
 python:
   install:
-  - requirements: requirements/tests.in
   - method: pip
     path: .
-    extra_requirements:
-    - docs
+  - requirements: requirements/tox-build-docs-cp311-linux-x86_64.txt
   system_packages: false
+
+...
```

### Comparing `cheroot-8.6.0/CHANGES.rst` & `cheroot-9.0.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+.. scm-version-title:: v9.0.0
+
+- :issue:`252` via :pr:`339`: Cheroot now requires Python
+  3.6 or later. Python 3.5 and Python 2.7 are still supported
+  by the :gh:`maint/8.x branch
+  <cherrypy/cheroot/tree/maint/8.x>` and stabilizing
+  bugfixes will be accepted to that branch.
+
 .. scm-version-title:: v8.6.0
 
 Significant improvements:
 
 - :issue:`384` via :pr:`385`, :pr:`406`: Exposed type stubs with
   annotations for public API -- by :user:`kasium`.
 
 - :pr:`401` (related to the :pr:`352` effort): Started reusing the
-  the ``expriration_interval`` setting in the low-level
+  the ``expriration_interval`` setting as timeout in the low-level
   :py:func:`~select.select` invocation, effectively reducing the system
-  load under the Windows OS when idle, that is noticeable on low-end
-  hardware systems -- by :user:`MichaIng`.
+  load when idle, that is noticeable on low-end hardware systems. On
+  Windows OS, due to different :py:func:`~select.select` behavior, the
+  effect is less significant and comes with a theoretically decreased
+  performance on quickly repeating requests, which has however found
+  to be not significant in real world scenarios.
+  -- by :user:`MichaIng`.
 
 Internal changes:
 
 - Implemented a manual-trigger-based release workflow.
 - Integrated publishing GitHub Releases into the workflow.
 - Migrated the docs theme to `Furo <https://pradyunsg.me/furo>`__
   (created by :user:`pradyunsg`).
```

### Comparing `cheroot-8.6.0/LICENSE.md` & `cheroot-9.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/PKG-INFO` & `cheroot-9.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: cheroot
-Version: 8.6.0
+Version: 9.0.0
 Summary: Highly-optimized, pure-python HTTP server
 Home-page: https://cheroot.cherrypy.dev
 Author: CherryPy Team
 Author-email: team@cherrypy.dev
-License: UNKNOWN
 Project-URL: CI: GitHub, https://github.com/cherrypy/cheroot/actions
 Project-URL: Docs: RTD, https://cheroot.cherrypy.dev
 Project-URL: GitHub: issues, https://github.com/cherrypy/cheroot/issues
 Project-URL: GitHub: repo, https://github.com/cherrypy/cheroot
 Project-URL: Tidelift: funding, https://tidelift.com/subscription/pkg/pypi-cheroot?utm_source=pypi-cheroot&utm_medium=referral&utm_campaign=pypi
 Keywords: http,server,ssl,wsgi
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: CherryPy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Typing :: Typed
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE.md
 
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
+   :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+   :alt: SWUbanner
+
 .. image:: https://img.shields.io/pypi/v/cheroot.svg
    :target: https://pypi.org/project/cheroot
 
 .. image:: https://tidelift.com/badges/package/pypi/cheroot
    :target: https://tidelift.com/subscription/pkg/pypi-cheroot?utm_source=pypi-cheroot&utm_medium=readme
    :alt: Cheroot is available as part of the Tidelift Subscription
 
@@ -130,9 +131,7 @@
 
 
 License
 =======
 .. image:: https://app.fossa.io/api/projects/git%2Bgithub.com%2Fcherrypy%2Fcheroot.svg?type=large
    :target: https://app.fossa.io/projects/git%2Bgithub.com%2Fcherrypy%2Fcheroot?ref=badge_large
    :alt: FOSSA Status
-
-
```

### Comparing `cheroot-8.6.0/README.rst` & `cheroot-9.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
+   :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+   :alt: SWUbanner
+
 .. image:: https://img.shields.io/pypi/v/cheroot.svg
    :target: https://pypi.org/project/cheroot
 
 .. image:: https://tidelift.com/badges/package/pypi/cheroot
    :target: https://tidelift.com/subscription/pkg/pypi-cheroot?utm_source=pypi-cheroot&utm_medium=readme
    :alt: Cheroot is available as part of the Tidelift Subscription
```

### Comparing `cheroot-8.6.0/cheroot/cli.py` & `cheroot-9.0.0/cheroot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,22 @@
 
 .. spelling::
 
    cli
 """
 
 import argparse
-from importlib import import_module
 import os
 import sys
-
-import six
+import urllib.parse  # noqa: WPS301
+from importlib import import_module
+from contextlib import suppress
 
 from . import server
 from . import wsgi
-from ._compat import suppress
-
-
-__metaclass__ = type
 
 
 class BindLocation:
     """A class for storing the bind location for a Cheroot instance."""
 
 
 class TCPSocket(BindLocation):
@@ -139,15 +135,15 @@
     # this is the first condition to verify, otherwise the urlparse
     # validation would detect //@<value> as a valid url with a hostname
     # with value: "<value>" and port: None
     if bind_addr_string.startswith('@'):
         return AbstractSocket(bind_addr_string[1:])
 
     # try and match for an IP/hostname and port
-    match = six.moves.urllib.parse.urlparse(
+    match = urllib.parse.urlparse(
         '//{addr}'.format(addr=bind_addr_string),
     )
     try:
         addr = match.hostname
         port = match.port
         if addr is not None or port is not None:
             return TCPSocket(addr, port)
```

### Comparing `cheroot-8.6.0/cheroot/cli.pyi` & `cheroot-9.0.0/cheroot/cli.pyi`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/cheroot/connections.py` & `cheroot-9.0.0/cheroot/connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """Utilities to manage open connections."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import io
 import os
 import socket
 import threading
 import time
+import selectors
+from contextlib import suppress
 
 from . import errors
-from ._compat import selectors
-from ._compat import suppress
 from ._compat import IS_WINDOWS
 from .makefile import MakeFile
 
-import six
-
 try:
     import fcntl
 except ImportError:
     try:
         from ctypes import windll, WinError
         import ctypes.wintypes
         _SetHandleInformation = windll.kernel32.SetHandleInformation
@@ -306,16 +301,15 @@
                     buf = [
                         '%s 400 Bad Request\r\n' % self.server.protocol,
                         'Content-Length: %s\r\n' % len(msg),
                         'Content-Type: text/plain\r\n\r\n',
                         msg,
                     ]
 
-                    sock_to_make = s if not six.PY2 else s._sock
-                    wfile = mf(sock_to_make, 'wb', io.DEFAULT_BUFFER_SIZE)
+                    wfile = mf(s, 'wb', io.DEFAULT_BUFFER_SIZE)
                     try:
                         wfile.write(''.join(buf).encode('ISO-8859-1'))
                     except socket.error as ex:
                         if ex.args[0] not in errors.socket_errors_to_ignore:
                             raise
                     return
                 if not s:
@@ -323,18 +317,15 @@
                 mf = self.server.ssl_adapter.makefile
                 # Re-apply our timeout since we may have a new socket object
                 if hasattr(s, 'settimeout'):
                     s.settimeout(self.server.timeout)
 
             conn = self.server.ConnectionClass(self.server, s, mf)
 
-            if not isinstance(
-                    self.server.bind_addr,
-                    (six.text_type, six.binary_type),
-            ):
+            if not isinstance(self.server.bind_addr, (str, bytes)):
                 # optional values
                 # Until we do DNS lookups, omit REMOTE_HOST
                 if addr is None:  # sometimes this can happen
                     # figure out if AF_INET or AF_INET6.
                     if len(s.getsockname()) == 2:
                         # AF_INET
                         addr = ('0.0.0.0', 0)
```

### Comparing `cheroot-8.6.0/cheroot/connections.pyi` & `cheroot-9.0.0/cheroot/connections.pyi`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/cheroot/errors.py` & `cheroot-9.0.0/cheroot/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # -*- coding: utf-8 -*-
 """Collection of exceptions raised and/or processed by Cheroot."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import errno
 import sys
 
 
 class MaxSizeExceeded(Exception):
-    """Exception raised when a client sends more data then acceptable within limit.
+    """Exception raised when a client sends more data then allowed under limit.
 
-    Depends on ``request.body.maxbytes`` config option if used within CherryPy
+    Depends on ``request.body.maxbytes`` config option if used within CherryPy.
     """
 
 
 class NoSSLError(Exception):
     """Exception raised when a client speaks HTTP to an HTTPS socket."""
```

### Comparing `cheroot-8.6.0/cheroot/server.py` & `cheroot-9.0.0/cheroot/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,41 +61,32 @@
 
    from cheroot.server import HTTPServer
 
 >>> 'HTTPServer' in globals()
 True
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import os
 import io
 import re
 import email.utils
 import socket
 import sys
 import time
 import traceback as traceback_
 import logging
 import platform
+import queue
 import contextlib
 import threading
-
-try:
-    from functools import lru_cache
-except ImportError:
-    from backports.functools_lru_cache import lru_cache
-
-import six
-from six.moves import queue
-from six.moves import urllib
+import urllib.parse
+from functools import lru_cache
 
 from . import connections, errors, __version__
-from ._compat import bton, ntou
+from ._compat import bton
 from ._compat import IS_PPC
 from .workers import threadpool
 from .makefile import MakeFile, StreamWriter
 
 
 __all__ = (
     'HTTPRequest', 'HTTPConnection', 'HTTPServer',
@@ -602,16 +593,16 @@
                 break
             line = self.readline(sizehint)
         return lines
 
     def read_trailer_lines(self):
         """Read HTTP headers and yield them.
 
-        Returns:
-            Generator: yields CRLF separated lines.
+        :yields: CRLF separated lines
+        :ytype: bytes
 
         """
         if not self.closed:
             raise ValueError(
                 'Cannot read trailers until the request body has been read.',
             )
 
@@ -813,18 +804,14 @@
                 'RFC 7230 (section 3.1.1) and RFC 7231 (section 4.1) '
                 'method names are case-sensitive and uppercase.'
             )
             self.simple_response('400 Bad Request', resp)
             return False
 
         try:
-            if six.PY2:  # FIXME: Figure out better way to do this
-                # Ref: https://stackoverflow.com/a/196392/595220 (like this?)
-                """This is a dummy check for unicode in URI."""
-                ntou(bton(uri, 'ascii'), 'ascii')
             scheme, authority, path, qs, fragment = urllib.parse.urlsplit(uri)
         except UnicodeError:
             self.simple_response('400 Bad Request', 'Malformed Request-URI')
             return False
 
         uri_is_absolute_form = (scheme or authority)
 
@@ -1116,15 +1103,15 @@
             else:
                 # HTTP/1.0 had no 413/414 status nor Connection header.
                 # Emit 400 instead and trust the message body is enough.
                 status = '400 Bad Request'
 
         buf.append(CRLF)
         if msg:
-            if isinstance(msg, six.text_type):
+            if isinstance(msg, str):
                 msg = msg.encode('ISO-8859-1')
             buf.append(msg)
 
         try:
             self.conn.wfile.write(EMPTY.join(buf))
         except socket.error as ex:
             if ex.args[0] not in errors.socket_errors_to_ignore:
@@ -1418,18 +1405,15 @@
             """Non-Linux kernels don't support SO_PEERCRED.
 
             Refs:
             http://welz.org.za/notes/on-peer-cred.html
             https://github.com/daveti/tcpSockHack
             msdn.microsoft.com/en-us/commandline/wsl/release_notes#build-15025
             """
-            six.raise_from(  # 3.6+: raise RuntimeError from socket_err
-                RuntimeError,
-                socket_err,
-            )
+            raise RuntimeError from socket_err
         else:
             pid, uid, gid = struct.unpack(PEERCRED_STRUCT_DEF, peer_creds)
             return pid, uid, gid
 
     @property
     def peer_pid(self):
         """Return the id of the connected peer process."""
@@ -1585,15 +1569,15 @@
     peercreds_resolve_enabled = False
     """
     If :py:data:`True`, username/group will be looked up in the OS from
     ``PEERCREDS``-provided IDs.
     """
 
     keep_alive_conn_limit = 10
-    """The maximum number of waiting keep-alive connections that will be kept open.
+    """Maximum number of waiting keep-alive connections that will be kept open.
 
     Default is 10. Set to None to have unlimited connections."""
 
     def __init__(
         self, bind_addr, gateway,
         minthreads=10, maxthreads=-1, server_name=None,
         peercreds_enabled=False, peercreds_resolve_enabled=False,
@@ -1758,21 +1742,21 @@
 
         # Select the appropriate socket
         self.socket = None
         msg = 'No socket could be created'
         if os.getenv('LISTEN_PID', None):
             # systemd socket activation
             self.socket = socket.fromfd(3, socket.AF_INET, socket.SOCK_STREAM)
-        elif isinstance(self.bind_addr, (six.text_type, six.binary_type)):
+        elif isinstance(self.bind_addr, (str, bytes)):
             # AF_UNIX socket
             try:
                 self.bind_unix_socket(self.bind_addr)
             except socket.error as serr:
                 msg = '%s -- (%s: %s)' % (msg, self.bind_addr, serr)
-                six.raise_from(socket.error(msg), serr)
+                raise socket.error(msg) from serr
         else:
             # AF_INET or AF_INET6 socket
             # Get the correct address family for our host (allows IPv6
             # addresses)
             host, port = self.bind_addr
             try:
                 info = socket.getaddrinfo(
@@ -2003,18 +1987,15 @@
 
             Refs:
             * https://msdn.microsoft.com/en-us/library/ms740621(v=vs.85).aspx
             * https://github.com/cherrypy/cheroot/issues/114
             * https://gavv.github.io/blog/ephemeral-port-reuse/
             """
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        if nodelay and not isinstance(
-                bind_addr,
-                (six.text_type, six.binary_type),
-        ):
+        if nodelay and not isinstance(bind_addr, (str, bytes)):
             sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
 
         if ssl_adapter is not None:
             sock = ssl_adapter.bind(sock)
 
         # If listening on the IPV6 any address ('::' = IN6ADDR_ANY),
         # activate dual-stack. See
@@ -2055,15 +2036,15 @@
         ):
             """UNIX domain sockets are strings or bytes.
 
             In case of bytes with a leading null-byte it's an abstract socket.
             """
             return bind_addr[:2]
 
-        if isinstance(bind_addr, six.binary_type):
+        if isinstance(bind_addr, bytes):
             bind_addr = bton(bind_addr)
 
         return bind_addr
 
     def process_conn(self, conn):
         """Process an incoming HTTPConnection."""
         try:
@@ -2105,18 +2086,15 @@
             self._run_time += (time.time() - self._start_time)
         self._start_time = None
 
         self._connections.stop()
 
         sock = getattr(self, 'socket', None)
         if sock:
-            if not isinstance(
-                    self.bind_addr,
-                    (six.text_type, six.binary_type),
-            ):
+            if not isinstance(self.bind_addr, (str, bytes)):
                 # Touch our own socket to make accept() return immediately.
                 try:
                     host, port = sock.getsockname()[:2]
                 except socket.error as ex:
                     if ex.args[0] not in errors.socket_errors_to_ignore:
                         # Changed to use error code and not message
                         # See
@@ -2175,15 +2153,15 @@
     'pyopenssl': 'cheroot.ssl.pyopenssl.pyOpenSSLAdapter',
 }
 
 
 def get_ssl_adapter_class(name='builtin'):
     """Return an SSL adapter class for the given name."""
     adapter = ssl_adapters[name.lower()]
-    if isinstance(adapter, six.string_types):
+    if isinstance(adapter, str):
         last_dot = adapter.rfind('.')
         attr_name = adapter[last_dot + 1:]
         mod_path = adapter[:last_dot]
 
         try:
             mod = sys.modules[mod_path]
             if mod is None:
```

### Comparing `cheroot-8.6.0/cheroot/server.pyi` & `cheroot-9.0.0/cheroot/server.pyi`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/cheroot/ssl/__init__.py` & `cheroot-9.0.0/cheroot/ssl/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 """Implementation of the SSL adapter base interface."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 from abc import ABCMeta, abstractmethod
 
-from six import add_metaclass
-
 
-@add_metaclass(ABCMeta)
-class Adapter:
+class Adapter(metaclass=ABCMeta):
     """Base class for SSL driver library adapters.
 
     Required methods:
 
         * ``wrap(sock) -> (wrapped socket, ssl environ dict)``
         * ``makefile(sock, mode='r', bufsize=DEFAULT_BUFFER_SIZE) ->
           socket file object``
```

### Comparing `cheroot-8.6.0/cheroot/ssl/__init__.pyi` & `cheroot-9.0.0/cheroot/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/cheroot/ssl/builtin.py` & `cheroot-9.0.0/cheroot/ssl/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,46 +3,39 @@
 
 The :py:mod:`ssl` module must be importable for SSL functionality.
 
 To use this module, set ``HTTPServer.ssl_adapter`` to an instance of
 ``BuiltinSSLAdapter``.
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import socket
 import sys
 import threading
+from contextlib import suppress
 
 try:
     import ssl
 except ImportError:
     ssl = None
 
 try:
     from _pyio import DEFAULT_BUFFER_SIZE
 except ImportError:
     try:
         from io import DEFAULT_BUFFER_SIZE
     except ImportError:
         DEFAULT_BUFFER_SIZE = -1
 
-import six
-
 from . import Adapter
 from .. import errors
-from .._compat import IS_ABOVE_OPENSSL10, suppress
+from .._compat import IS_ABOVE_OPENSSL10
 from ..makefile import StreamReader, StreamWriter
 from ..server import HTTPServer
 
-if six.PY2:
-    generic_socket_error = socket.error
-else:
-    generic_socket_error = OSError
+generic_socket_error = OSError
 
 
 def _assert_ssl_exc_contains(exc, *msgs):
     """Check whether SSL exception contains either of messages provided."""
     if len(msgs) < 1:
         raise TypeError(
             '_assert_ssl_exc_contains() requires '
```

### Comparing `cheroot-8.6.0/cheroot/ssl/builtin.pyi` & `cheroot-9.0.0/cheroot/ssl/builtin.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
 from . import Adapter
 
-generic_socket_error: OSError
 DEFAULT_BUFFER_SIZE: int
 
 class BuiltinSSLAdapter(Adapter):
     CERT_KEY_TO_ENV: Any
     CERT_KEY_TO_LDAP_CODE: Any
     def __init__(self, certificate, private_key, certificate_chain: Any | None = ..., ciphers: Any | None = ...) -> None: ...
     @property
     def context(self): ...
     @context.setter
     def context(self, context) -> None: ...
     def bind(self, sock): ...
     def wrap(self, sock): ...
-    def get_environ(self): ...
+    def get_environ(self, sock): ...
     def makefile(self, sock, mode: str = ..., bufsize: int = ...): ...
```

### Comparing `cheroot-8.6.0/cheroot/ssl/pyopenssl.py` & `cheroot-9.0.0/cheroot/ssl/pyopenssl.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,19 @@
 will be read, and the context will be automatically created from them.
 
 .. spelling::
 
    pyopenssl
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import socket
 import sys
 import threading
 import time
 
-import six
-
 try:
     import OpenSSL.version
     from OpenSSL import SSL
     from OpenSSL import crypto
 
     try:
         ssl_conn_type = SSL.Connection
@@ -225,16 +220,15 @@
             nmspc[p] = make_property(p)
 
         # Doesn't work via super() for some reason.
         # Falling back to type() instead:
         return type(name, bases, nmspc)
 
 
-@six.add_metaclass(SSLConnectionProxyMeta)
-class SSLConnection:
+class SSLConnection(metaclass=SSLConnectionProxyMeta):
     r"""A thread-safe wrapper for an ``SSL.Connection``.
 
     :param tuple args: the arguments to create the wrapped \
                         :py:class:`SSL.Connection(*args) \
                         <pyopenssl:OpenSSL.SSL.Connection>`
     """
```

### Comparing `cheroot-8.6.0/cheroot/ssl/pyopenssl.pyi` & `cheroot-9.0.0/cheroot/ssl/pyopenssl.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from . import Adapter
 from ..makefile import StreamReader, StreamWriter
 from OpenSSL import SSL
-from typing import Any
+from typing import Any, Type
 
-ssl_conn_type: SSL.Connection
+ssl_conn_type: Type[SSL.Connection]
 
 class SSLFileobjectMixin:
     ssl_timeout: int
     ssl_retry: float
     def recv(self, size): ...
     def readline(self, size: int = ...): ...
     def sendall(self, *args, **kwargs): ...
     def send(self, *args, **kwargs): ...
 
-class SSLFileobjectStreamReader(SSLFileobjectMixin, StreamReader): ...  # type:ignore
-class SSLFileobjectStreamWriter(SSLFileobjectMixin, StreamWriter): ...  # type:ignore
+class SSLFileobjectStreamReader(SSLFileobjectMixin, StreamReader): ...  # type:ignore[misc]
+class SSLFileobjectStreamWriter(SSLFileobjectMixin, StreamWriter): ...  # type:ignore[misc]
 
 class SSLConnectionProxyMeta:
     def __new__(mcl, name, bases, nmspc): ...
 
-class SSLConnection():
+class SSLConnection:
     def __init__(self, *args) -> None: ...
 
 class pyOpenSSLAdapter(Adapter):
     def __init__(self, certificate, private_key, certificate_chain: Any | None = ..., ciphers: Any | None = ...) -> None: ...
     def bind(self, sock): ...
     def wrap(self, sock): ...
     def get_environ(self): ...
     def makefile(self, sock, mode: str = ..., bufsize: int = ...): ...
+    def get_context(self) -> SSL.Context: ...
```

### Comparing `cheroot-8.6.0/cheroot/test/_pytest_plugin.py` & `cheroot-9.0.0/cheroot/test/_pytest_plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 itself, useless for end-users' app testing.
 """
 
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import pytest
+import six
 
 
 pytest_version = tuple(map(int, pytest.__version__.split('.')))
 
 
 def pytest_load_initial_conftests(early_config, parser, args):
     """Drop unfilterable warning ignores."""
@@ -39,12 +40,21 @@
         '<socket.socket fd=-1, family=AF_INET, '
         'type=SocketKind.SOCK_STREAM, proto=.:'
         'pytest.PytestUnraisableExceptionWarning:_pytest.unraisableexception',
         'ignore:Exception ignored in. '
         '<socket.socket fd=-1, family=AF_INET6, '
         'type=SocketKind.SOCK_STREAM, proto=.:'
         'pytest.PytestUnraisableExceptionWarning:_pytest.unraisableexception',
-        'ignore:Exception ignored in. '
-        '<ssl.SSLSocket fd=-1, family=AddressFamily.AF_UNIX, '
-        'type=SocketKind.SOCK_STREAM, proto=.:'
-        'pytest.PytestUnraisableExceptionWarning:_pytest.unraisableexception',
+    ))
+
+    if six.PY2:
+        return
+
+    # NOTE: `ResourceWarning` does not exist under Python 2 and so using
+    # NOTE: it in warning filters results in an `_OptionError` exception
+    # NOTE: being raised.
+    early_config._inicache['filterwarnings'].extend((
+        # FIXME: Try to figure out what causes this and ensure that the socket
+        # FIXME: gets closed.
+        'ignore:unclosed <socket.socket fd=:ResourceWarning',
+        'ignore:unclosed <ssl.SSLSocket fd=:ResourceWarning',
     ))
```

### Comparing `cheroot-8.6.0/cheroot/test/conftest.py` & `cheroot-9.0.0/cheroot/test/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 """Pytest configuration module.
 
 Contains fixtures, which are tightly bound to the Cheroot framework
 itself, useless for end-users' app testing.
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type  # pylint: disable=invalid-name
-
 import threading
 import time
 
 import pytest
 
+from .._compat import IS_MACOS, IS_WINDOWS  # noqa: WPS436
 from ..server import Gateway, HTTPServer
 from ..testing import (  # noqa: F401  # pylint: disable=unused-import
     native_server, wsgi_server,
 )
 from ..testing import get_server_client
 
 
 @pytest.fixture
+def http_request_timeout():
+    """Return a common HTTP request timeout for tests with queries."""
+    computed_timeout = 0.1
+
+    if IS_MACOS:
+        computed_timeout *= 2
+
+    if IS_WINDOWS:
+        computed_timeout *= 10
+
+    return computed_timeout
+
+
+@pytest.fixture
 # pylint: disable=redefined-outer-name
 def wsgi_server_client(wsgi_server):  # noqa: F811
     """Create a test client out of given WSGI server."""
     return get_server_client(wsgi_server)
 
 
 @pytest.fixture
```

### Comparing `cheroot-8.6.0/cheroot/test/helper.py` & `cheroot-9.0.0/cheroot/test/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 """A library of helper functions for the Cheroot test suite."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import datetime
 import logging
 import os
 import sys
 import time
 import threading
 import types
-
-from six.moves import http_client
-
-import six
+import http.client
 
 import cheroot.server
 import cheroot.wsgi
 
 from cheroot.test import webtest
 
 log = logging.getLogger(__name__)
@@ -56,22 +50,22 @@
 
         cls.HOST, cls.PORT = cls.httpserver.bind_addr
         if cls.httpserver.ssl_adapter is None:
             ssl = ''
             cls.scheme = 'http'
         else:
             ssl = ' (ssl)'
-            cls.HTTP_CONN = http_client.HTTPSConnection
+            cls.HTTP_CONN = http.client.HTTPSConnection
             cls.scheme = 'https'
 
         v = sys.version.split()[0]
-        log.info('Python version used to run this test script: %s' % v)
-        log.info('Cheroot version: %s' % cheroot.__version__)
-        log.info('HTTP server version: %s%s' % (cls.httpserver.protocol, ssl))
-        log.info('PID: %s' % os.getpid())
+        log.info('Python version used to run this test script: %s', v)
+        log.info('Cheroot version: %s', cheroot.__version__)
+        log.info('HTTP server version: %s%s', cls.httpserver.protocol, ssl)
+        log.info('PID: %s', os.getpid())
 
         if hasattr(cls, 'setup_server'):
             # Clear the wsgi server so that
             # it can be updated with the new root
             cls.setup_server()
             cls.start()
 
@@ -131,17 +125,17 @@
         self.headers = {'Content-Type': 'text/html'}
         self.body = None
 
     def output(self):
         """Generate iterable response body object."""
         if self.body is None:
             return []
-        elif isinstance(self.body, six.text_type):
+        elif isinstance(self.body, str):
             return [self.body.encode('iso-8859-1')]
-        elif isinstance(self.body, six.binary_type):
+        elif isinstance(self.body, bytes):
             return [self.body]
         else:
             return [x.encode('iso-8859-1') for x in self.body]
 
 
 class Controller:
     """WSGI app for tests."""
```

### Comparing `cheroot-8.6.0/cheroot/test/test__compat.py` & `cheroot-9.0.0/cheroot/test/test__compat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-# -*- coding: utf-8 -*-
 """Test suite for cross-python compatibility helpers."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import pytest
-import six
 
-from cheroot._compat import extract_bytes, memoryview, ntob, ntou, bton
+from cheroot._compat import extract_bytes, ntob, ntou, bton
 
 
 @pytest.mark.parametrize(
     ('func', 'inp', 'out'),
     (
         (ntob, 'bar', b'bar'),
         (ntou, 'bar', u'bar'),
@@ -28,15 +23,15 @@
     (
         ntob,
         ntou,
     ),
 )
 def test_compat_functions_negative_nonnative(func):
     """Check that compatibility functions fail loudly for incorrect input."""
-    non_native_test_str = u'bar' if six.PY2 else b'bar'
+    non_native_test_str = b'bar'
     with pytest.raises(TypeError):
         func(non_native_test_str, encoding='utf-8')
 
 
 def test_ntou_escape():
     """Check that ``ntou`` supports escape-encoding under Python 2."""
     expected = u'hišřії'
```

### Comparing `cheroot-8.6.0/cheroot/test/test_cli.py` & `cheroot-9.0.0/cheroot/test/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Tests to verify the command line interface.
 
 .. spelling::
 
    cli
 """
-# -*- coding: utf-8 -*-
-# vim: set fileencoding=utf-8 :
 import sys
 
-import six
 import pytest
 
 from cheroot.cli import (
     Application,
     parse_wsgi_bind_addr,
 )
 
@@ -65,20 +62,14 @@
 
             It has an empty body because we are expecting to verify that
             the same method is return no the actual execution of it.
             """
     app = WSGIAppMock()
     # patch sys.modules, to include the an instance of WSGIAppMock
     # under a specific namespace
-    if six.PY2:
-        # python2 requires the previous namespaces to be part of sys.modules
-        #   (e.g. for 'a.b.c' we need to insert 'a', 'a.b' and 'a.b.c')
-        # otherwise it fails, we're setting the same instance on each level,
-        # we don't really care about those, just the last one.
-        monkeypatch.setitem(sys.modules, 'mypkg', app)
     monkeypatch.setitem(sys.modules, 'mypkg.wsgi', app)
     return app
 
 
 @pytest.mark.parametrize(
     ('app_name', 'app_method'),
     (
```

### Comparing `cheroot-8.6.0/cheroot/test/test_conn.py` & `cheroot-9.0.0/cheroot/test/test_conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Tests for TCP connection handling, including proper and timely close."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import errno
 import socket
 import time
 import logging
 import traceback as traceback_
 from collections import namedtuple
+import http.client
+import urllib.request
 
-from six.moves import range, http_client, urllib
-
-import six
 import pytest
 from jaraco.text import trim, unwrap
 
 from cheroot.test import helper, webtest
 from cheroot._compat import IS_CI, IS_MACOS, IS_PYPY, IS_WINDOWS
 import cheroot.server
 
@@ -90,16 +86,14 @@
 
     def _munge(string):
         """Encode PATH_INFO correctly depending on Python version.
 
         WSGI 1.0 is a mess around unicode. Create endpoints
         that match the PATH_INFO that it produces.
         """
-        if six.PY2:
-            return string
         return string.encode('utf-8').decode('latin-1')
 
     handlers = {
         '/hello': hello,
         '/pov': pov,
         '/page1': pov,
         '/page2': pov,
@@ -238,15 +232,15 @@
     actual_status = int(status_line[:3])
     assert actual_status == 200
     assert status_line[4:] == 'OK'
     assert actual_resp_body == pov.encode()
     assert header_has_value('Connection', 'close', actual_headers)
 
     # Make another request on the same connection, which should error.
-    with pytest.raises(http_client.NotConnected):
+    with pytest.raises(http.client.NotConnected):
         test_client.get('/pov', http_conn=http_connection)
 
 
 @pytest.mark.parametrize(
     'set_cl',
     (
         False,  # Without Content-Length
@@ -305,29 +299,32 @@
         if chunked_response:
             assert not header_has_value('Connection', 'close', actual_headers)
         else:
             assert header_has_value('Connection', 'close', actual_headers)
 
             # Make another request on the same connection, which should
             # error.
-            with pytest.raises(http_client.NotConnected):
+            with pytest.raises(http.client.NotConnected):
                 test_client.get('/pov', http_conn=http_connection)
 
         # Try HEAD.
         # See https://www.bitbucket.org/cherrypy/cherrypy/issue/864.
         # TODO: figure out how can this be possible on an closed connection
         # (chunked_response case)
         status_line, actual_headers, actual_resp_body = test_client.head(
             '/stream', http_conn=http_connection,
         )
         assert actual_status == 200
         assert status_line[4:] == 'OK'
         assert actual_resp_body == b''
         assert not header_exists('Transfer-Encoding', actual_headers)
 
+    # Prevent the resource warnings:
+    http_connection.close()
+
 
 @pytest.mark.parametrize(
     'set_cl',
     (
         False,  # Without Content-Length
         True,  # With Content-Length
     ),
@@ -385,22 +382,25 @@
         assert actual_resp_body == b'0123456789'
 
         assert not header_exists('Content-Length', actual_headers)
         assert not header_has_value('Connection', 'Keep-Alive', actual_headers)
         assert not header_exists('Transfer-Encoding', actual_headers)
 
         # Make another request on the same connection, which should error.
-        with pytest.raises(http_client.NotConnected):
+        with pytest.raises(http.client.NotConnected):
             test_client.get(
                 '/pov', http_conn=http_connection,
                 protocol='HTTP/1.0',
             )
 
     test_client.server_instance.protocol = original_server_protocol
 
+    # Prevent the resource warnings:
+    http_connection.close()
+
 
 @pytest.mark.parametrize(
     'http_server_protocol',
     (
         'HTTP/1.0',
         pytest.param(
             'HTTP/1.1',
@@ -462,14 +462,17 @@
     assert status_line[4:] == 'OK'
     assert actual_resp_body == pov.encode()
     assert not header_exists('Connection', actual_headers)
     assert not header_exists('Keep-Alive', actual_headers)
 
     test_client.server_instance.protocol = original_server_protocol
 
+    # Prevent the resource warnings:
+    http_connection.close()
+
 
 def test_keepalive_conn_management(test_client):
     """Test management of Keep-Alive connections."""
     test_client.server_instance.timeout = 2
 
     def connection():
         # Initialize a persistent HTTP connection
@@ -507,17 +510,17 @@
                 return
             assert time.time() <= deadline, (
                 'idle conn count mismatch, wanted {count}, got {n}'.
                 format(**locals()),
             )
 
     disconnect_errors = (
-        http_client.BadStatusLine,
-        http_client.CannotSendRequest,
-        http_client.NotConnected,
+        http.client.BadStatusLine,
+        http.client.CannotSendRequest,
+        http.client.NotConnected,
     )
 
     # Make a new connection.
     c1 = connection()
     request(c1)
     check_server_idle_conn_count(1)
 
@@ -561,14 +564,19 @@
     # But the second one should still be valid.
     request(c2)
     check_server_idle_conn_count(1)
 
     # Restore original timeout.
     test_client.server_instance.timeout = timeout
 
+    # Prevent the resource warnings:
+    c1.close()
+    c2.close()
+    c3.close()
+
 
 @pytest.mark.parametrize(
     ('simulated_exception', 'error_number', 'exception_leaks'),
     (
         pytest.param(
             socket.error, errno.ECONNRESET, False,
             id='socket.error(ECONNRESET)',
@@ -593,28 +601,26 @@
         pytest.param(
             socket.error, errno.ESHUTDOWN, False,
             id='socket.error(ESHUTDOWN)',
         ),
         pytest.param(RuntimeError, 666, True, id='RuntimeError(666)'),
         pytest.param(socket.error, -1, True, id='socket.error(-1)'),
     ) + (
-        () if six.PY2 else (
             pytest.param(
                 ConnectionResetError, errno.ECONNRESET, False,
                 id='ConnectionResetError(ECONNRESET)',
             ),
             pytest.param(
                 BrokenPipeError, errno.EPIPE, False,
                 id='BrokenPipeError(EPIPE)',
             ),
             pytest.param(
                 BrokenPipeError, errno.ESHUTDOWN, False,
                 id='BrokenPipeError(ESHUTDOWN)',
             ),
-        )
     ),
 )
 def test_broken_connection_during_tcp_fin(
         error_number, exception_leaks,
         mocker, monkeypatch,
         simulated_exception, test_client,
 ):
@@ -761,15 +767,15 @@
     # Make another request on the same socket, which should error
     conn._output(b'GET /hello HTTP/1.1')
     conn._output(('Host: %s' % conn.host).encode('ascii'))
     conn._send_output()
     response = conn.response_class(conn.sock, method='GET')
     try:
         response.begin()
-    except (socket.error, http_client.BadStatusLine):
+    except (socket.error, http.client.BadStatusLine):
         pass
     except Exception as ex:
         pytest.fail(fail_msg % ex)
     else:
         if response.status != 408:
             pytest.fail(fail_msg % response.read())
 
@@ -791,15 +797,15 @@
     # but timeout on the headers
     conn.send(b'GET /hello HTTP/1.1')
     # Wait for our socket timeout
     time.sleep(timeout * 2)
     response = conn.response_class(conn.sock, method='GET')
     try:
         response.begin()
-    except (socket.error, http_client.BadStatusLine):
+    except (socket.error, http.client.BadStatusLine):
         pass
     except Exception as ex:
         pytest.fail(fail_msg % ex)
     else:
         if response.status != 408:
             pytest.fail(fail_msg % response.read())
 
@@ -841,16 +847,15 @@
 
         # Retrieve previous response
         response = conn.response_class(conn.sock, method='GET')
         # there is a bug in python3 regarding the buffering of
         # ``conn.sock``. Until that bug get's fixed we will
         # monkey patch the ``response`` instance.
         # https://bugs.python.org/issue23377
-        if not six.PY2:
-            response.fp = conn.sock.makefile('rb', 0)
+        response.fp = conn.sock.makefile('rb', 0)
         response.begin()
         body = response.read(13)
         assert response.status == 200
         assert body == b'Hello, world!'
 
     # Retrieve final response
     response = conn.response_class(conn.sock, method='GET')
@@ -1022,14 +1027,17 @@
     )
     actual_status = int(status_line[:3])
     assert actual_status == 304
     assert not header_exists('Content-Length', actual_headers)
     assert actual_resp_body == b''
     assert not header_exists('Connection', actual_headers)
 
+    # Prevent the resource warnings:
+    http_connection.close()
+
 
 @pytest.mark.xfail(
     reason=unwrap(
         trim("""
         Headers from earlier request leak into the request
         line for a subsequent request, resulting in 400
         instead of 413. See cherrypy/cheroot#69 for details.
```

### Comparing `cheroot-8.6.0/cheroot/test/test_core.py` & `cheroot-9.0.0/cheroot/test/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 """Tests for managing HTTP issues (malformed requests, etc)."""
-# -*- coding: utf-8 -*-
-# vim: set fileencoding=utf-8 :
-
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
 
 import errno
 import socket
+import urllib.parse  # noqa: WPS301
 
 import pytest
-import six
-from six.moves import urllib
 
 from cheroot.test import helper
 
 
 HTTP_BAD_REQUEST = 400
 HTTP_LENGTH_REQUIRED = 411
 HTTP_NOT_FOUND = 404
@@ -50,24 +44,28 @@
 
     def _munge(string):
         """Encode PATH_INFO correctly depending on Python version.
 
         WSGI 1.0 is a mess around unicode. Create endpoints
         that match the PATH_INFO that it produces.
         """
-        if six.PY2:
-            return string
         return string.encode('utf-8').decode('latin-1')
 
     handlers = {
         '/hello': hello,
         '/no_body': hello,
         '/body_required': body_required,
         '/query_string': query_string,
+        # FIXME: Unignore the pylint rules in pylint >= 2.15.4.
+        # Refs:
+        # * https://github.com/PyCQA/pylint/issues/6592
+        # * https://github.com/PyCQA/pylint/pull/7395
+        # pylint: disable-next=too-many-function-args
         _munge('/привіт'): hello,
+        # pylint: disable-next=too-many-function-args
         _munge('/Юххууу'): hello,
         '/\xa0Ðblah key 0 900 4 data': hello,
         '/*': asterisk,
     }
 
 
 def _get_http_response(connection, method='GET'):
@@ -147,15 +145,14 @@
 def test_parse_acceptable_uri(test_client, uri):
     """Check that server responds with OK to valid GET queries."""
     status_line = test_client.get(uri)[0]
     actual_status = int(status_line[:3])
     assert actual_status == HTTP_OK
 
 
-@pytest.mark.xfail(six.PY2, reason='Fails on Python 2')
 def test_parse_uri_unsafe_uri(test_client):
     """Test that malicious URI does not allow HTTP injection.
 
     This effectively checks that sending GET request with URL
 
     /%A0%D0blah%20key%200%20900%204%20data
 
@@ -259,14 +256,16 @@
     c.request('POST', '/no_body')
     response = c.getresponse()
     actual_resp_body = response.read()
     actual_status = response.status
     assert actual_status == HTTP_OK
     assert actual_resp_body == b'Hello world!'
 
+    c.close()  # deal with the resource warning
+
 
 def test_content_length_required(test_client):
     """Test POST query with body failing because of missing Content-Length."""
     # Now send a message that has no Content-Length, but does send a body.
     # Verify that CP times out the socket and responds
     # with 411 Length Required.
 
@@ -274,14 +273,16 @@
     c.request('POST', '/body_required')
     response = c.getresponse()
     response.read()
 
     actual_status = response.status
     assert actual_status == HTTP_LENGTH_REQUIRED
 
+    c.close()  # deal with the resource warning
+
 
 @pytest.mark.xfail(
     reason='https://github.com/cherrypy/cheroot/issues/106',
     strict=False,  # sometimes it passes
 )
 def test_large_request(test_client_with_defaults):
     """Test GET query with maliciously large Content-Length."""
@@ -346,14 +347,16 @@
 
     response = c.getresponse()
     actual_status = response.status
     assert actual_status == HTTP_BAD_REQUEST
     actual_resp_body = response.read(21)
     assert actual_resp_body == b'Malformed method name'
 
+    c.close()  # deal with the resource warning
+
 
 def test_malformed_header(test_client):
     """Check that broken HTTP header results in Bad Request."""
     c = test_client.get_connection()
     c.putrequest('GET', '/')
     c.putheader('Content-Type', 'text/plain')
     # See https://www.bitbucket.org/cherrypy/cherrypy/issue/941
@@ -362,14 +365,16 @@
 
     response = c.getresponse()
     actual_status = response.status
     assert actual_status == HTTP_BAD_REQUEST
     actual_resp_body = response.read(20)
     assert actual_resp_body == b'Illegal header line.'
 
+    c.close()  # deal with the resource warning
+
 
 def test_request_line_split_issue_1220(test_client):
     """Check that HTTP request line of exactly 256 chars length is OK."""
     Request_URI = (
         '/hello?'
         'intervenant-entreprise-evenement_classaction='
         'evenement-mailremerciements'
```

### Comparing `cheroot-8.6.0/cheroot/test/test_dispatch.py` & `cheroot-9.0.0/cheroot/test/test_dispatch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 """Tests for the HTTP server."""
-# -*- coding: utf-8 -*-
-# vim: set fileencoding=utf-8 :
-
-from __future__ import absolute_import, division, print_function
 
 from cheroot.wsgi import PathInfoDispatcher
 
 
 def wsgi_invoke(app, environ):
     """Serve 1 request from a WSGI application."""
     response = {}
```

### Comparing `cheroot-8.6.0/cheroot/test/test_errors.py` & `cheroot-9.0.0/cheroot/test/test_errors.py`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/cheroot/test/test_makefile.py` & `cheroot-9.0.0/cheroot/test/test_makefile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Tests for :py:mod:`cheroot.makefile`."""
 
 from cheroot import makefile
 
 
-__metaclass__ = type
-
-
 class MockSocket:
     """A mock socket."""
 
     def __init__(self):
         """Initialize :py:class:`MockSocket`."""
         self.messages = []
```

### Comparing `cheroot-8.6.0/cheroot/test/test_server.py` & `cheroot-9.0.0/cheroot/test/test_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 """Tests for the HTTP server."""
-# -*- coding: utf-8 -*-
-# vim: set fileencoding=utf-8 :
-
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
 
 import os
+import queue
 import socket
 import tempfile
 import threading
 import uuid
+import urllib.parse  # noqa: WPS301
 
 import pytest
 import requests
 import requests_unixsocket
-import six
 
 from pypytools.gc.custom import DefaultGc
-from six.moves import queue, urllib
 
 from .._compat import bton, ntob
 from .._compat import IS_LINUX, IS_MACOS, IS_WINDOWS, SYS_PLATFORM
 from ..server import IS_UID_GID_RESOLVABLE, Gateway, HTTPServer
 from ..testing import (
     ANY_INTERFACE_IPV4,
     ANY_INTERFACE_IPV6,
@@ -255,68 +250,80 @@
     httpserver.gateway = _TestGateway
     httpserver.peercreds_enabled = True
     return httpserver
 
 
 @unix_only_sock_test
 @non_macos_sock_test
-def test_peercreds_unix_sock(peercreds_enabled_server):
+def test_peercreds_unix_sock(http_request_timeout, peercreds_enabled_server):
     """Check that ``PEERCRED`` lookup works when enabled."""
     httpserver = peercreds_enabled_server
     bind_addr = httpserver.bind_addr
 
-    if isinstance(bind_addr, six.binary_type):
+    if isinstance(bind_addr, bytes):
         bind_addr = bind_addr.decode()
 
     # pylint: disable=possibly-unused-variable
     quoted = urllib.parse.quote(bind_addr, safe='')
     unix_base_uri = 'http+unix://{quoted}'.format(**locals())
 
     expected_peercreds = os.getpid(), os.getuid(), os.getgid()
     expected_peercreds = '|'.join(map(str, expected_peercreds))
 
     with requests_unixsocket.monkeypatch():
-        peercreds_resp = requests.get(unix_base_uri + PEERCRED_IDS_URI)
+        peercreds_resp = requests.get(
+            unix_base_uri + PEERCRED_IDS_URI,
+            timeout=http_request_timeout,
+        )
         peercreds_resp.raise_for_status()
         assert peercreds_resp.text == expected_peercreds
 
-        peercreds_text_resp = requests.get(unix_base_uri + PEERCRED_TEXTS_URI)
+        peercreds_text_resp = requests.get(
+            unix_base_uri + PEERCRED_TEXTS_URI,
+            timeout=http_request_timeout,
+        )
         assert peercreds_text_resp.status_code == 500
 
 
 @pytest.mark.skipif(
     not IS_UID_GID_RESOLVABLE,
     reason='Modules `grp` and `pwd` are not available '
            'under the current platform',
 )
 @unix_only_sock_test
 @non_macos_sock_test
-def test_peercreds_unix_sock_with_lookup(peercreds_enabled_server):
+def test_peercreds_unix_sock_with_lookup(
+        http_request_timeout,
+        peercreds_enabled_server,
+):
     """Check that ``PEERCRED`` resolution works when enabled."""
     httpserver = peercreds_enabled_server
     httpserver.peercreds_resolve_enabled = True
 
     bind_addr = httpserver.bind_addr
 
-    if isinstance(bind_addr, six.binary_type):
+    if isinstance(bind_addr, bytes):
         bind_addr = bind_addr.decode()
 
     # pylint: disable=possibly-unused-variable
     quoted = urllib.parse.quote(bind_addr, safe='')
     unix_base_uri = 'http+unix://{quoted}'.format(**locals())
 
     import grp
     import pwd
     expected_textcreds = (
         pwd.getpwuid(os.getuid()).pw_name,
         grp.getgrgid(os.getgid()).gr_name,
     )
     expected_textcreds = '!'.join(map(str, expected_textcreds))
     with requests_unixsocket.monkeypatch():
-        peercreds_text_resp = requests.get(unix_base_uri + PEERCRED_TEXTS_URI)
+        peercreds_text_resp = requests.get(
+            unix_base_uri + PEERCRED_TEXTS_URI,
+            timeout=http_request_timeout,
+        )
         peercreds_text_resp.raise_for_status()
         assert peercreds_text_resp.text == expected_textcreds
 
 
 @pytest.mark.skipif(
     IS_WINDOWS,
     reason='This regression test is for a Linux bug, '
@@ -359,15 +366,18 @@
     # follow-up check wouldn't make sense
     assert len(native_process_conn.filenos) > 0
 
     # Check at least one of the sockets created are above the target number
     assert any(fn >= resource_limit for fn in native_process_conn.filenos)
 
 
-if not IS_WINDOWS:
+ISSUE511 = IS_MACOS
+
+
+if not IS_WINDOWS and not ISSUE511:
     test_high_number_of_file_descriptors = pytest.mark.forked(
         test_high_number_of_file_descriptors,
     )
 
 
 @pytest.fixture
 def _garbage_bin():
```

### Comparing `cheroot-8.6.0/cheroot/test/test_ssl.py` & `cheroot-9.0.0/cheroot/test/test_ssl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Tests for TLS support."""
-# -*- coding: utf-8 -*-
-# vim: set fileencoding=utf-8 :
-
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
 
 import functools
 import json
 import os
 import ssl
 import subprocess
 import sys
 import threading
 import time
 import traceback
+import http.client
 
 import OpenSSL.SSL
 import pytest
 import requests
-import six
 import trustme
 
 from .._compat import bton, ntob, ntou
 from .._compat import IS_ABOVE_OPENSSL10, IS_CI, IS_PYPY
 from .._compat import IS_LINUX, IS_MACOS, IS_WINDOWS
 from ..server import HTTPServer, get_ssl_adapter_class
 from ..testing import (
@@ -45,36 +40,32 @@
     )
 )
 IS_LIBRESSL_BACKEND = ssl.OPENSSL_VERSION.startswith('LibreSSL')
 IS_PYOPENSSL_SSL_VERSION_1_0 = (
     OpenSSL.SSL.SSLeay_version(OpenSSL.SSL.SSLEAY_VERSION).
     startswith(b'OpenSSL 1.0.')
 )
-PY27 = sys.version_info[:2] == (2, 7)
-PY34 = sys.version_info[:2] == (3, 4)
-PY3 = not six.PY2
 PY310_PLUS = sys.version_info[:2] >= (3, 10)
 
 
 _stdlib_to_openssl_verify = {
     ssl.CERT_NONE: OpenSSL.SSL.VERIFY_NONE,
     ssl.CERT_OPTIONAL: OpenSSL.SSL.VERIFY_PEER,
     ssl.CERT_REQUIRED:
         OpenSSL.SSL.VERIFY_PEER + OpenSSL.SSL.VERIFY_FAIL_IF_NO_PEER_CERT,
 }
 
 
 fails_under_py3 = pytest.mark.xfail(
-    not six.PY2,
     reason='Fails under Python 3+',
 )
 
 
 fails_under_py3_in_pypy = pytest.mark.xfail(
-    not six.PY2 and IS_PYPY,
+    IS_PYPY,
     reason='Fails under PyPy3',
 )
 
 
 missing_ipv6 = pytest.mark.skipif(
     not _probe_ipv6_sock('::1'),
     reason=''
@@ -209,14 +200,15 @@
     'adapter_type',
     (
         'builtin',
         'pyopenssl',
     ),
 )
 def test_ssl_adapters(
+    http_request_timeout,
     tls_http_server, adapter_type,
     tls_certificate,
     tls_certificate_chain_pem_path,
     tls_certificate_private_key_pem_path,
     tls_ca_certificate_pem_path,
 ):
     """Test ability to connect to server via HTTPS using adapters."""
@@ -237,14 +229,15 @@
 
     interface, _host, port = _get_conn_data(
         tlshttpserver.bind_addr,
     )
 
     resp = requests.get(
         'https://{host!s}:{port!s}/'.format(host=interface, port=port),
+        timeout=http_request_timeout,
         verify=tls_ca_certificate_pem_path,
     )
 
     assert resp.status_code == 200
     assert resp.text == 'Hello world!'
 
 
@@ -272,16 +265,17 @@
     ),
 )
 @pytest.mark.xfail(
     IS_PYPY and IS_CI,
     reason='Fails under PyPy in CI for unknown reason',
     strict=False,
 )
-def test_tls_client_auth(  # noqa: C901  # FIXME
+def test_tls_client_auth(  # noqa: C901, WPS213  # FIXME
     # FIXME: remove twisted logic, separate tests
+    http_request_timeout,
     mocker,
     tls_http_server, adapter_type,
     ca,
     tls_certificate,
     tls_certificate_chain_pem_path,
     tls_certificate_private_key_pem_path,
     tls_ca_certificate_pem_path,
@@ -327,14 +321,17 @@
 
         interface, _host, port = _get_conn_data(tlshttpserver.bind_addr)
 
         make_https_request = functools.partial(
             requests.get,
             'https://{host!s}:{port!s}/'.format(host=interface, port=port),
 
+            # Don't wait for the first byte forever:
+            timeout=http_request_timeout,
+
             # Server TLS certificate verification:
             verify=tls_ca_certificate_pem_path,
 
             # Client TLS certificate verification:
             cert=cl_pem,
         )
 
@@ -344,69 +341,56 @@
             if (
                     not is_req_successful
                     and IS_PYOPENSSL_SSL_VERSION_1_0
                     and adapter_type == 'builtin'
                     and tls_verify_mode == ssl.CERT_REQUIRED
                     and tls_client_identity == 'localhost'
                     and is_trusted_cert
-            ) or PY34:
+            ):
                 pytest.xfail(
                     'OpenSSL 1.0 has problems with verifying client certs',
                 )
             assert is_req_successful
             assert resp.text == 'Hello world!'
+            resp.close()
             return
 
         # xfail some flaky tests
         # https://github.com/cherrypy/cheroot/issues/237
         issue_237 = (
             IS_MACOS
             and adapter_type == 'builtin'
             and tls_verify_mode != ssl.CERT_NONE
         )
         if issue_237:
             pytest.xfail('Test sometimes fails')
 
-        expected_ssl_errors = (
-            requests.exceptions.SSLError,
-            OpenSSL.SSL.Error,
-        ) if PY34 else (
-            requests.exceptions.SSLError,
-        )
+        expected_ssl_errors = requests.exceptions.SSLError,
         if IS_WINDOWS or IS_GITHUB_ACTIONS_WORKFLOW:
             expected_ssl_errors += requests.exceptions.ConnectionError,
         with pytest.raises(expected_ssl_errors) as ssl_err:
-            make_https_request()
-
-        if PY34 and isinstance(ssl_err, OpenSSL.SSL.Error):
-            pytest.xfail(
-                'OpenSSL behaves wierdly under Python 3.4 '
-                'because of an outdated urllib3',
-            )
+            make_https_request().close()
 
         try:
             err_text = ssl_err.value.args[0].reason.args[0].args[0]
         except AttributeError:
-            if PY34:
-                pytest.xfail('OpenSSL behaves wierdly under Python 3.4')
-            elif IS_WINDOWS or IS_GITHUB_ACTIONS_WORKFLOW:
+            if IS_WINDOWS or IS_GITHUB_ACTIONS_WORKFLOW:
                 err_text = str(ssl_err.value)
             else:
                 raise
 
         if isinstance(err_text, int):
             err_text = str(ssl_err.value)
 
         expected_substrings = (
             'sslv3 alert bad certificate' if IS_LIBRESSL_BACKEND
             else 'tlsv1 alert unknown ca',
         )
-        if not six.PY2:
-            if IS_MACOS and IS_PYPY and adapter_type == 'pyopenssl':
-                expected_substrings = ('tlsv1 alert unknown ca',)
+        if IS_MACOS and IS_PYPY and adapter_type == 'pyopenssl':
+            expected_substrings = ('tlsv1 alert unknown ca',)
         if (
                 tls_verify_mode in (
                     ssl.CERT_REQUIRED,
                     ssl.CERT_OPTIONAL,
                 )
                 and not is_trusted_cert
                 and tls_client_identity == 'localhost'
@@ -465,17 +449,17 @@
 
 @pytest.mark.parametrize(  # noqa: C901  # FIXME
     'adapter_type',
     (
         pytest.param(
             'builtin',
             marks=pytest.mark.xfail(
-                IS_GITHUB_ACTIONS_WORKFLOW and IS_MACOS and PY310_PLUS,
+                IS_MACOS and PY310_PLUS,
                 reason='Unclosed TLS resource warnings happen on macOS '
-                'under Python 3.10',
+                'under Python 3.10 (#508)',
                 strict=False,
             ),
         ),
         'pyopenssl',
     ),
 )
 @pytest.mark.parametrize(
@@ -488,14 +472,15 @@
         (ssl.CERT_REQUIRED, True),
     ),
 )
 def test_ssl_env(  # noqa: C901  # FIXME
         thread_exceptions,
         recwarn,
         mocker,
+        http_request_timeout,
         tls_http_server, adapter_type,
         ca, tls_verify_mode, tls_certificate,
         tls_certificate_chain_pem_path,
         tls_certificate_private_key_pem_path,
         tls_ca_certificate_pem_path,
         use_client_cert,
 ):
@@ -528,21 +513,18 @@
 
         tlswsgiserver = tls_http_server((interface, port), tls_adapter)
 
         interface, _host, port = _get_conn_data(tlswsgiserver.bind_addr)
 
         resp = requests.get(
             'https://' + interface + ':' + str(port) + '/env',
+            timeout=http_request_timeout,
             verify=tls_ca_certificate_pem_path,
             cert=cl_pem if use_client_cert else None,
         )
-        if PY34 and resp.status_code != 200:
-            pytest.xfail(
-                'Python 3.4 has problems with verifying client certs',
-            )
 
         env = json.loads(resp.content.decode('utf-8'))
 
         # hard coded env
         assert env['wsgi.url_scheme'] == 'https'
         assert env['HTTPS'] == 'on'
 
@@ -616,52 +598,44 @@
     ),
 )
 def test_https_over_http_error(http_server, ip_addr):
     """Ensure that connecting over HTTPS to HTTP port is handled."""
     httpserver = http_server.send((ip_addr, EPHEMERAL_PORT))
     interface, _host, port = _get_conn_data(httpserver.bind_addr)
     with pytest.raises(ssl.SSLError) as ssl_err:
-        six.moves.http_client.HTTPSConnection(
+        http.client.HTTPSConnection(
             '{interface}:{port}'.format(
                 interface=interface,
                 port=port,
             ),
         ).request('GET', '/')
     expected_substring = (
         'wrong version number' if IS_ABOVE_OPENSSL10
         else 'unknown protocol'
     )
     assert expected_substring in ssl_err.value.args[-1]
 
 
-http_over_https_error_builtin_marks = []
-if IS_WINDOWS and six.PY2:
-    http_over_https_error_builtin_marks.append(
-        pytest.mark.flaky(reruns=5, reruns_delay=2),
-    )
-
-
 @pytest.mark.parametrize(
     'adapter_type',
     (
-        pytest.param(
-            'builtin',
-            marks=http_over_https_error_builtin_marks,
-        ),
+        'builtin',
         'pyopenssl',
     ),
 )
 @pytest.mark.parametrize(
     'ip_addr',
     (
         ANY_INTERFACE_IPV4,
         pytest.param(ANY_INTERFACE_IPV6, marks=missing_ipv6),
     ),
 )
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_http_over_https_error(
+    http_request_timeout,
     tls_http_server, adapter_type,
     ca, ip_addr,
     tls_certificate,
     tls_certificate_chain_pem_path,
     tls_certificate_private_key_pem_path,
 ):
     """Ensure that connecting over HTTP to HTTPS port is handled."""
@@ -693,55 +667,32 @@
     fqdn = interface
     if ip_addr is ANY_INTERFACE_IPV6:
         fqdn = '[{fqdn}]'.format(**locals())
 
     expect_fallback_response_over_plain_http = (
         (
             adapter_type == 'pyopenssl'
-            and (IS_ABOVE_OPENSSL10 or not six.PY2)
         )
-        or PY27
-    ) or (
-        IS_GITHUB_ACTIONS_WORKFLOW
-        and IS_WINDOWS
-        and six.PY2
-        and not IS_WIN2016
-    )
-    if (
-            IS_GITHUB_ACTIONS_WORKFLOW
-            and IS_WINDOWS
-            and six.PY2
-            and IS_WIN2016
-            and adapter_type == 'builtin'
-            and ip_addr is ANY_INTERFACE_IPV6
-    ):
-        expect_fallback_response_over_plain_http = True
-    if (
-            IS_GITHUB_ACTIONS_WORKFLOW
-            and IS_WINDOWS
-            and six.PY2
-            and not IS_WIN2016
-            and adapter_type == 'builtin'
-            and ip_addr is not ANY_INTERFACE_IPV6
-    ):
-        expect_fallback_response_over_plain_http = False
+    )
     if expect_fallback_response_over_plain_http:
         resp = requests.get(
             'http://{host!s}:{port!s}/'.format(host=fqdn, port=port),
+            timeout=http_request_timeout,
         )
         assert resp.status_code == 400
         assert resp.text == (
             'The client sent a plain HTTP request, '
             'but this server only speaks HTTPS on this port.'
         )
         return
 
     with pytest.raises(requests.exceptions.ConnectionError) as ssl_err:
         requests.get(  # FIXME: make stdlib ssl behave like PyOpenSSL
             'http://{host!s}:{port!s}/'.format(host=fqdn, port=port),
+            timeout=http_request_timeout,
         )
 
     if IS_LINUX:
         expected_error_code, expected_error_text = (
             104, 'Connection reset by peer',
         )
     if IS_MACOS:
```

### Comparing `cheroot-8.6.0/cheroot/test/test_wsgi.py` & `cheroot-9.0.0/cheroot/test/test_wsgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     # pylint: disable=possibly-unused-variable
     url = 'http://localhost:{port}/'.format(**locals())
     # pylint: disable=possibly-unused-variable
     with server._run_in_thread() as thread:
         yield locals()
 
 
+@pytest.mark.flaky(reruns=3, reruns_delay=2)
 def test_connection_keepalive(simple_wsgi_server):
     """Test the connection keepalive works (duh)."""
     session = Session(base_url=simple_wsgi_server['url'])
     pooled = requests.adapters.HTTPAdapter(
         pool_connections=1, pool_maxsize=1000,
     )
     session.mount('http://', pooled)
@@ -55,14 +56,15 @@
     with ThreadPoolExecutor(max_workers=10 if IS_SLOW_ENV else 50) as pool:
         tasks = [
             pool.submit(do_request)
             for n in range(250 if IS_SLOW_ENV else 1000)
         ]
         failures = sum(task.result() for task in tasks)
 
+    session.close()
     assert not failures
 
 
 def test_gateway_start_response_called_twice(monkeypatch):
     """Verify that repeat calls of ``Gateway.start_response()`` fail."""
     monkeypatch.setattr(wsgi.Gateway, 'get_environ', lambda self: {})
     wsgi_gateway = wsgi.Gateway(None)
```

### Comparing `cheroot-8.6.0/cheroot/test/webtest.py` & `cheroot-9.0.0/cheroot/test/webtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,27 @@
 same process (but in separate threads, obviously).
 When an error occurs in the framework, call server_error. It will print
 the traceback to stdout, and keep any assertions you have from running
 (the assumption is that, if the server errors, the page output will not
 be of further significance to your tests).
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import pprint
 import re
 import socket
 import sys
 import time
 import traceback
 import os
 import json
 import unittest  # pylint: disable=deprecated-module,preferred-module
 import warnings
 import functools
-
-from six.moves import http_client, map, urllib_parse
-import six
+import http.client
+import urllib.parse
 
 from more_itertools.more import always_iterable
 import jaraco.functools
 
 
 def interface(host):
     """Return an IP address for a client connection given the server host.
@@ -101,15 +97,15 @@
 
 
 class WebCase(unittest.TestCase):
     """Helper web test suite base."""
 
     HOST = '127.0.0.1'
     PORT = 8000
-    HTTP_CONN = http_client.HTTPConnection
+    HTTP_CONN = http.client.HTTPConnection
     PROTOCOL = 'HTTP/1.1'
 
     scheme = 'http'
     url = None
     ssl_context = None
 
     status = None
@@ -123,15 +119,15 @@
     @property
     def _Conn(self):
         """Return HTTPConnection or HTTPSConnection based on self.scheme.
 
         * from :py:mod:`python:http.client`.
         """
         cls_name = '{scheme}Connection'.format(scheme=self.scheme.upper())
-        return getattr(http_client, cls_name)
+        return getattr(http.client, cls_name)
 
     def get_conn(self, auto_open=False):
         """Return a connection to our HTTP server."""
         conn = self._Conn(self.interface(), self.PORT)
         # Automatically re-connect?
         conn.auto_open = auto_open
         conn.connect()
@@ -197,17 +193,17 @@
             ...             *args, **kwargs
             ...         )
 
         ``raise_subcls`` is passed through to :py:func:`openURL`.
         """
         ServerError.on = False
 
-        if isinstance(url, six.text_type):
+        if isinstance(url, str):
             url = url.encode('utf-8')
-        if isinstance(body, six.text_type):
+        if isinstance(body, str):
             body = body.encode('utf-8')
 
         # for compatibility, support raise_subcls is None
         raise_subcls = raise_subcls or ()
 
         self.url = url
         self.time = None
@@ -382,44 +378,44 @@
         if matches:
             if msg is None:
                 msg = '%r:%r in %r' % (key, value, hdrs)
             self._handlewebError(msg)
 
     def assertBody(self, value, msg=None):
         """Fail if value != self.body."""
-        if isinstance(value, six.text_type):
+        if isinstance(value, str):
             value = value.encode(self.encoding)
         if value != self.body:
             if msg is None:
                 msg = 'expected body:\n%r\n\nactual body:\n%r' % (
                     value, self.body,
                 )
             self._handlewebError(msg)
 
     def assertInBody(self, value, msg=None):
         """Fail if value not in self.body."""
-        if isinstance(value, six.text_type):
+        if isinstance(value, str):
             value = value.encode(self.encoding)
         if value not in self.body:
             if msg is None:
                 msg = '%r not in body: %s' % (value, self.body)
             self._handlewebError(msg)
 
     def assertNotInBody(self, value, msg=None):
         """Fail if value in self.body."""
-        if isinstance(value, six.text_type):
+        if isinstance(value, str):
             value = value.encode(self.encoding)
         if value in self.body:
             if msg is None:
                 msg = '%r found in body' % value
             self._handlewebError(msg)
 
     def assertMatchesBody(self, pattern, msg=None, flags=0):
         """Fail if value (a regex pattern) is not in self.body."""
-        if isinstance(pattern, six.text_type):
+        if isinstance(pattern, str):
             pattern = pattern.encode(self.encoding)
         if re.search(pattern, self.body, flags) is None:
             if msg is None:
                 msg = 'No match for %r in body' % pattern
             self._handlewebError(msg)
 
 
@@ -460,33 +456,15 @@
     return headers
 
 
 def shb(response):
     """Return status, headers, body the way we like from a response."""
     resp_status_line = '%s %s' % (response.status, response.reason)
 
-    if not six.PY2:
-        return resp_status_line, response.getheaders(), response.read()
-
-    h = []
-    key, value = None, None
-    for line in response.msg.headers:
-        if line:
-            if line[0] in ' \t':
-                value += line.strip()
-            else:
-                if key and value:
-                    h.append((key, value))
-                key, value = line.split(':', 1)
-                key = key.strip()
-                value = value.strip()
-    if key and value:
-        h.append((key, value))
-
-    return resp_status_line, h, response.read()
+    return resp_status_line, response.getheaders(), response.read()
 
 
 # def openURL(*args, raise_subcls=(), **kwargs):
 # py27 compatible signature:
 def openURL(*args, **kwargs):
     """
     Open a URL, retrying when it fails.
@@ -510,15 +488,15 @@
         cleanup=on_exception,
         trap=socket.error,
     )
 
 
 def _open_url_once(
     url, headers=None, method='GET', body=None,
-    host='127.0.0.1', port=8000, http_conn=http_client.HTTPConnection,
+    host='127.0.0.1', port=8000, http_conn=http.client.HTTPConnection,
     protocol='HTTP/1.1', ssl_context=None,
 ):
     """Open the given HTTP resource and return status, headers, and body."""
     headers = cleanHeaders(headers, method, body, host, port)
 
     # Allow http_conn to be a class or an instance
     if hasattr(http_conn, 'host'):
@@ -526,15 +504,15 @@
     else:
         kw = {}
         if ssl_context:
             kw['context'] = ssl_context
         conn = http_conn(interface(host), port, **kw)
     conn._http_vsn_str = protocol
     conn._http_vsn = int(''.join([x for x in protocol if x.isdigit()]))
-    if not six.PY2 and isinstance(url, bytes):
+    if isinstance(url, bytes):
         url = url.decode()
     conn.putrequest(
         method.upper(), url, skip_host=True,
         skip_accept_encoding=True,
     )
     for key, value in headers:
         conn.putheader(key, value.encode('Latin-1'))
@@ -568,18 +546,18 @@
 
     >>> strip_netloc('//google.com/foo/bar?bing#baz')
     '/foo/bar?bing'
 
     >>> strip_netloc('/foo/bar?bing#baz')
     '/foo/bar?bing'
     """
-    parsed = urllib_parse.urlparse(url)
+    parsed = urllib.parse.urlparse(url)
     _scheme, _netloc, path, params, query, _fragment = parsed
     stripped = '', '', path, params, query, ''
-    return urllib_parse.urlunparse(stripped)
+    return urllib.parse.urlunparse(stripped)
 
 
 # Add any exceptions which your web framework handles
 # normally (that you don't want server_error to trap).
 ignored_exceptions = []
 
 # You'll want set this to True when you can't guarantee
```

### Comparing `cheroot-8.6.0/cheroot/testing.py` & `cheroot-9.0.0/cheroot/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Pytest fixtures and other helpers for doing testing by end-users."""
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
-from contextlib import closing
+from contextlib import closing, contextmanager
 import errno
 import socket
 import threading
 import time
+import http.client
 
 import pytest
-from six.moves import http_client
 
 import cheroot.server
 from cheroot.test import webtest
 import cheroot.wsgi
 
 EPHEMERAL_PORT = 0
 NO_INTERFACE = None  # Using this or '' will cause an exception
@@ -29,14 +26,15 @@
     cheroot.server.HTTPServer: {
         'bind_addr': (NO_INTERFACE, EPHEMERAL_PORT),
         'gateway': cheroot.server.Gateway,
     },
 }
 
 
+@contextmanager
 def cheroot_server(server_factory):
     """Set up and tear down a Cheroot server instance."""
     conf = config[server_factory].copy()
     bind_port = conf.pop('bind_addr')[-1]
 
     for interface in ANY_INTERFACE_IPV6, ANY_INTERFACE_IPV4:
         try:
@@ -60,22 +58,22 @@
 
     httpserver.stop()  # destroy it
 
 
 @pytest.fixture
 def wsgi_server():
     """Set up and tear down a Cheroot WSGI server instance."""
-    for srv in cheroot_server(cheroot.wsgi.Server):
+    with cheroot_server(cheroot.wsgi.Server) as srv:
         yield srv
 
 
 @pytest.fixture
 def native_server():
     """Set up and tear down a Cheroot HTTP server instance."""
-    for srv in cheroot_server(cheroot.server.HTTPServer):
+    with cheroot_server(cheroot.server.HTTPServer) as srv:
         yield srv
 
 
 class _TestClient:
     def __init__(self, server):
         self._interface, self._host, self._port = _get_conn_data(
             server.bind_addr,
@@ -85,17 +83,17 @@
 
     def get_connection(self):
         name = '{interface}:{port}'.format(
             interface=self._interface,
             port=self._port,
         )
         conn_cls = (
-            http_client.HTTPConnection
+            http.client.HTTPConnection
             if self.server_instance.ssl_adapter is None else
-            http_client.HTTPSConnection
+            http.client.HTTPSConnection
         )
         return conn_cls(name)
 
     def request(
         self, uri, method='GET', headers=None, http_conn=None,
         protocol='HTTP/1.1',
     ):
```

### Comparing `cheroot-8.6.0/cheroot/workers/threadpool.py` & `cheroot-9.0.0/cheroot/workers/threadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 """A thread-based worker pool.
 
 .. spelling::
 
    joinable
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
-
 import collections
 import threading
 import time
 import socket
 import warnings
-
-from six.moves import queue
+import queue
 
 from jaraco.functools import pass_none
 
 
 __all__ = ('WorkerThread', 'ThreadPool')
 
 
@@ -174,15 +169,15 @@
     def start(self):
         """Start the pool of threads."""
         for _ in range(self.min):
             self._threads.append(WorkerThread(self.server))
         for worker in self._threads:
             worker.name = (
                 'CP Server {worker_name!s}'.
-                format(worker_name=worker.name),
+                format(worker_name=worker.name)
             )
             worker.start()
         for worker in self._threads:
             while not worker.ready:
                 time.sleep(.1)
 
     @property
@@ -224,15 +219,15 @@
             time.sleep(.1)
         self._threads.extend(workers)
 
     def _spawn_worker(self):
         worker = WorkerThread(self.server)
         worker.name = (
             'CP Server {worker_name!s}'.
-            format(worker_name=worker.name),
+            format(worker_name=worker.name)
         )
         worker.start()
         return worker
 
     def shrink(self, amount):
         """Kill off worker threads (not below self.min)."""
         # Grow/shrink the pool if necessary.
```

### Comparing `cheroot-8.6.0/cheroot/workers/threadpool.pyi` & `cheroot-9.0.0/cheroot/workers/threadpool.pyi`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/cheroot/wsgi.py` & `cheroot-9.0.0/cheroot/wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,16 @@
         '/': my_crazy_app,
         '/blog': my_blog_app,
     }
     d = wsgi.PathInfoDispatcher(path_map)
     server = wsgi.Server(addr, d)
 """
 
-from __future__ import absolute_import, division, print_function
-__metaclass__ = type
-
 import sys
 
-import six
-from six.moves import filter
-
 from . import server
 from .workers import threadpool
 from ._compat import ntob, bton
 
 
 class Server(server.HTTPServer):
     """A subclass of HTTPServer which calls a WSGI application."""
@@ -136,42 +130,40 @@
             iteration of the application return value that yields
             a NON-EMPTY string, or upon the application's first
             invocation of the write() callable.
         """
         response = self.req.server.wsgi_app(self.env, self.start_response)
         try:
             for chunk in filter(None, response):
-                if not isinstance(chunk, six.binary_type):
+                if not isinstance(chunk, bytes):
                     raise ValueError('WSGI Applications must yield bytes')
                 self.write(chunk)
         finally:
             # Send headers if not already sent
             self.req.ensure_headers_sent()
             if hasattr(response, 'close'):
                 response.close()
 
-    def start_response(self, status, headers, exc_info=None):
+    def start_response(self, status, headers, exc_info=None):  # noqa: WPS238
         """WSGI callable to begin the HTTP response."""
         # "The application may call start_response more than once,
         # if and only if the exc_info argument is provided."
         if self.started_response and not exc_info:
             raise RuntimeError(
                 'WSGI start_response called a second '
                 'time with no exc_info.',
             )
         self.started_response = True
 
         # "if exc_info is provided, and the HTTP headers have already been
         # sent, start_response must raise an error, and should raise the
         # exc_info tuple."
         if self.req.sent_headers:
-            try:
-                six.reraise(*exc_info)
-            finally:
-                exc_info = None
+            value = exc_info[1]
+            raise value
 
         self.req.status = self._encode_status(status)
 
         for k, v in headers:
             if not isinstance(k, str):
                 raise TypeError(
                     'WSGI response header key %r is not of type str.' % k,
@@ -192,16 +184,14 @@
         """Cast status to bytes representation of current Python version.
 
         According to :pep:`3333`, when using Python 3, the response status
         and headers must be bytes masquerading as Unicode; that is, they
         must be of type "str" but are restricted to code points in the
         "Latin-1" set.
         """
-        if six.PY2:
-            return status
         if not isinstance(status, str):
             raise TypeError('WSGI response status is not of type str.')
         return status.encode('ISO-8859-1')
 
     def write(self, chunk):
         """WSGI callable to write unbuffered data to the client.
 
@@ -269,15 +259,15 @@
             'wsgi.multiprocess': False,
             'wsgi.multithread': True,
             'wsgi.run_once': False,
             'wsgi.url_scheme': bton(req.scheme),
             'wsgi.version': self.version,
         }
 
-        if isinstance(req.server.bind_addr, six.string_types):
+        if isinstance(req.server.bind_addr, str):
             # AF_UNIX. This isn't really allowed by WSGI, which doesn't
             # address unix domain sockets. But it's better than nothing.
             env['SERVER_PORT'] = ''
             try:
                 env['X_REMOTE_PID'] = str(req_conn.peer_pid)
                 env['X_REMOTE_UID'] = str(req_conn.peer_uid)
                 env['X_REMOTE_GID'] = str(req_conn.peer_gid)
@@ -328,46 +318,31 @@
 
     version = 'u', 0
 
     def get_environ(self):
         """Return a new environ dict targeting the given wsgi.version."""
         req = self.req
         env_10 = super(Gateway_u0, self).get_environ()
-        env = dict(map(self._decode_key, env_10.items()))
+        env = dict(env_10.items())
 
         # Request-URI
-        enc = env.setdefault(six.u('wsgi.url_encoding'), six.u('utf-8'))
+        enc = env.setdefault('wsgi.url_encoding', 'utf-8')
         try:
             env['PATH_INFO'] = req.path.decode(enc)
             env['QUERY_STRING'] = req.qs.decode(enc)
         except UnicodeDecodeError:
             # Fall back to latin 1 so apps can transcode if needed.
             env['wsgi.url_encoding'] = 'ISO-8859-1'
             env['PATH_INFO'] = env_10['PATH_INFO']
             env['QUERY_STRING'] = env_10['QUERY_STRING']
 
-        env.update(map(self._decode_value, env.items()))
+        env.update(env.items())
 
         return env
 
-    @staticmethod
-    def _decode_key(item):
-        k, v = item
-        if six.PY2:
-            k = k.decode('ISO-8859-1')
-        return k, v
-
-    @staticmethod
-    def _decode_value(item):
-        k, v = item
-        skip_keys = 'REQUEST_URI', 'wsgi.input'
-        if not six.PY2 or not isinstance(v, bytes) or k in skip_keys:
-            return k, v
-        return k, v.decode('ISO-8859-1')
-
 
 wsgi_gateways = Gateway.gateway_map()
 
 
 class PathInfoDispatcher:
     """A WSGI dispatcher for dispatch based on the PATH_INFO."""
```

### Comparing `cheroot-8.6.0/cheroot.egg-info/PKG-INFO` & `cheroot-9.0.0/cheroot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: cheroot
-Version: 8.6.0
+Version: 9.0.0
 Summary: Highly-optimized, pure-python HTTP server
 Home-page: https://cheroot.cherrypy.dev
 Author: CherryPy Team
 Author-email: team@cherrypy.dev
-License: UNKNOWN
 Project-URL: CI: GitHub, https://github.com/cherrypy/cheroot/actions
 Project-URL: Docs: RTD, https://cheroot.cherrypy.dev
 Project-URL: GitHub: issues, https://github.com/cherrypy/cheroot/issues
 Project-URL: GitHub: repo, https://github.com/cherrypy/cheroot
 Project-URL: Tidelift: funding, https://tidelift.com/subscription/pkg/pypi-cheroot?utm_source=pypi-cheroot&utm_medium=referral&utm_campaign=pypi
 Keywords: http,server,ssl,wsgi
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: CherryPy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Typing :: Typed
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE.md
 
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
+   :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+   :alt: SWUbanner
+
 .. image:: https://img.shields.io/pypi/v/cheroot.svg
    :target: https://pypi.org/project/cheroot
 
 .. image:: https://tidelift.com/badges/package/pypi/cheroot
    :target: https://tidelift.com/subscription/pkg/pypi-cheroot?utm_source=pypi-cheroot&utm_medium=readme
    :alt: Cheroot is available as part of the Tidelift Subscription
 
@@ -130,9 +131,7 @@
 
 
 License
 =======
 .. image:: https://app.fossa.io/api/projects/git%2Bgithub.com%2Fcherrypy%2Fcheroot.svg?type=large
    :target: https://app.fossa.io/projects/git%2Bgithub.com%2Fcherrypy%2Fcheroot?ref=badge_large
    :alt: FOSSA Status
-
-
```

### Comparing `cheroot-8.6.0/docs/conf.py` & `cheroot-9.0.0/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 else:
     del _sphinxcontrib_spelling  # noqa: WPS100
     extensions.append('sphinxcontrib.spelling')
 
 # Tree-local extensions:
 extensions.append('scm_tag_titles_ext')
 
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
 master_doc = 'index'
 
 apidoc_excluded_paths = []
 apidoc_extra_args = [
     '--implicit-namespaces',
     '--private',  # include “_private” modules
 ]
@@ -70,21 +73,21 @@
 github_repo_name = 'cheroot'
 github_repo_slug = f'{github_repo_org}/{github_repo_name}'
 github_repo_url = f'{github_url}/{github_repo_slug}'
 cp_github_repo_url = f'{github_url}/{github_repo_org}/cherrypy'
 github_sponsors_url = f'{github_url}/sponsors'
 
 extlinks = {
-    'issue': (f'{github_repo_url}/issues/%s', '#'),
-    'pr': (f'{github_repo_url}/pull/%s', 'PR #'),
-    'commit': (f'{github_repo_url}/commit/%s', ''),
-    'cp-issue': (f'{cp_github_repo_url}/issues/%s', 'CherryPy #'),
-    'cp-pr': (f'{cp_github_repo_url}/pull/%s', 'CherryPy PR #'),
-    'gh': (f'{github_url}/%s', 'GitHub: '),
-    'user': (f'{github_sponsors_url}/%s', '@'),
+    'issue': (f'{github_repo_url}/issues/%s', '#%s'),
+    'pr': (f'{github_repo_url}/pull/%s', 'PR #%s'),
+    'commit': (f'{github_repo_url}/commit/%s', '%s'),
+    'cp-issue': (f'{cp_github_repo_url}/issues/%s', 'CherryPy #%s'),
+    'cp-pr': (f'{cp_github_repo_url}/pull/%s', 'CherryPy PR #%s'),
+    'gh': (f'{github_url}/%s', 'GitHub: %s'),
+    'user': (f'{github_sponsors_url}/%s', '@%s'),
 }
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'python2': ('https://docs.python.org/2', None),
     # Ref: https://github.com/cherrypy/cherrypy/issues/1872
     'cherrypy': (
@@ -105,30 +108,20 @@
     # "429 Client Error: too many requests for url"
     # Ref: https://github.com/sphinx-doc/sphinx/issues/7388
     r'https://github\.com/cherrypy/cheroot/issues',
     r'https://github\.com/cherrypy/cheroot/pull',
     r'https://github\.com/cherrypy/cherrypy/issues',
     r'https://github\.com/cherrypy/cherrypy/pull',
 
-    # Requires a more liberal 'Accept: ' HTTP request header:
-    # Ref: https://github.com/sphinx-doc/sphinx/issues/7247
-    r'https://github\.com/cherrypy/cheroot/workflows/[^/]+/badge\.svg',
-
     # Has an ephemeral anchor (line-range) but actual HTML has separate per-
     # line anchors.
     r'https://github\.com'
     r'/python/cpython/blob/c39b52f/Lib/poplib\.py#L297-L302',
     r'https://github\.com'
     r'/python/cpython/blob/c39b52f/Lib/poplib\.py#user-content-L297-L302',
-
-    # The domain is currently down. TODO: Revisit after Aug 3, 2021.
-    # Ref: https://github.com/cherrypy/cherrypy/issues/1872
-    r'https://cheroot\.cherrypy\.org',
-    r'https://docs\.cherrypy\.org',
-    r'https://www\.cherrypy\.org',
 ]
 linkcheck_workers = 25
 
 nitpicky = True
 
 # NOTE: consider having a separate ignore file
 # Ref: https://stackoverflow.com/a/30624034/595220
```

### Comparing `cheroot-8.6.0/docs/contribute.rst` & `cheroot-9.0.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/docs/devguide.rst` & `cheroot-9.0.0/docs/devguide.rst`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/docs/scm_tag_titles_ext.py` & `cheroot-9.0.0/docs/scm_tag_titles_ext.py`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/docs/spelling_stub_ext.py` & `cheroot-9.0.0/docs/spelling_stub_ext.py`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/docs/spelling_wordlist.txt` & `cheroot-9.0.0/docs/spelling_wordlist.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 AppVeyor
 Args
 backports
+bugfixes
 builtin
 b'xb
 compat
 config
 conftest
 conn
 chunked
```

### Comparing `cheroot-8.6.0/pytest.ini` & `cheroot-9.0.0/pytest.ini`

 * *Files 24% similar despite different names*

```diff
@@ -50,20 +50,28 @@
   ignore:Python 3.5 support will be dropped in the next release of cryptography. Please upgrade your Python.:UserWarning:OpenSSL.crypto
   # cryptography==3.2.1 warning:
   ignore:OpenSSL version 1.0.2 is no longer supported by the OpenSSL project, please upgrade. The next version of cryptography will completely remove support for it.:UserWarning:cryptography
   ignore:OpenSSL version 1.0.2 is no longer supported by the OpenSSL project, please upgrade. The next version of cryptography will completely remove support for it.:UserWarning:OpenSSL.crypto
   # cryptography=3.3.1 warning:
   ignore:Python 2 is no longer supported by the Python core team. Support for it is now deprecated in cryptography, and will be removed in the next release.:UserWarning:cryptography
   ignore:Python 2 is no longer supported by the Python core team. Support for it is now deprecated in cryptography, and will be removed in the next release.:UserWarning:OpenSSL.crypto
+  # cryptography == 38 warning:
+  ignore:Python 3.6 is no longer supported by the Python core team. Therefore, support for it is deprecated in cryptography and will be removed in a future release.:UserWarning:cryptography
+  ignore:Python 3.6 is no longer supported by the Python core team. Therefore, support for it is deprecated in cryptography and will be removed in a future release.:UserWarning:OpenSSL._util
+  ignore:Python 3.6 is no longer supported by the Python core team. Therefore, support for it is deprecated in cryptography and will be removed in a future release.:UserWarning:OpenSSL.crypto
 
-  # FIXME: drop once setuptools/six fix their importer implementations
-  # Ref: https://github.com/pypa/setuptools/issues/2481
-  ignore:VendorImporter.exec_module.. not found; falling back to load_module..:ImportWarning
-  ignore:VendorImporter.find_spec.. not found; falling back to find_module..:ImportWarning
-  ignore:_SixMetaPathImporter.exec_module.. not found; falling back to load_module..:ImportWarning
+  # FIXME: drop once certifi fixes their use of `importlib.resources`
+  # Ref: https://github.com/certifi/python-certifi/issues/183
+  ignore:path is deprecated. Use files.. instead. Refer to https.//importlib-resources.readthedocs.io/en/latest/using.html#migrating-from-legacy for migration advice.:DeprecationWarning:certifi.core
+
+  # FIXME: drop once requests-toolbelt stops importing `urllib3.contrib.pyopenssl`
+  # Refs:
+  # * https://github.com/requests/toolbelt/issues/331
+  # * https://github.com/urllib3/urllib3/issues/2680
+  ignore:'urllib3.contrib.pyopenssl' module is deprecated and will be removed in a future release of urllib3 2.x. Read more in this issue. https.//github.com/urllib3/urllib3/issues/2680:DeprecationWarning:requests_toolbelt._compat
 
 junit_duration_report = call
 junit_family = xunit2
 junit_suite_name = cheroot_test_suite
 
 # A mapping of markers to their descriptions allowed in strict mode:
 markers =
```

### Comparing `cheroot-8.6.0/requirements/dist-build-constraints.txt` & `cheroot-9.0.0/requirements/dist-build-constraints.txt`

 * *Files identical despite different names*

### Comparing `cheroot-8.6.0/requirements/tests.in` & `cheroot-9.0.0/requirements/tests.in`

 * *Files 26% similar despite different names*

```diff
@@ -12,49 +12,64 @@
 # ```
 # UserWarning: Trying to detect encoding from a tiny portion
 # of (12) byte(s).
 # ```
 # Ref: https://github.com/psf/requests/commit/2ed84f5
 # To avoid the warning, we declare a direct dependency on chardet
 # here so that it's use is adjusted across Python 2 and Python 3:
-chardet
+requests[use_chardet_on_py3]
+
+# Updating `charset-normalizer` on Python 3.5 under Ubuntu 18.04 causes
+# some weird issues with `cryptography` — it starts wanting `libffi7`
+# but only `libffi6` is available in that environment.
+# Note that there's no `charset-normalizer` for Python 2
+charset-normalizer < 2.1.0; python_version >= "3.0" and python_version <= "3.5"
 
 # Address https://github.com/tartley/colorama/issues/240.
 # It's a transitive dependency of pytest-watch plugin.
 colorama!=0.4.2; python_version == "3.4"
 
 # measure test coverage
-coverage == 6.2; python_version >= "3.6"
+coverage >= 6.2; python_version >= "3.6"
 coverage < 5; python_version == "3.4"
 coverage < 6; python_version < "3.6" and python_version != "3.4"
 futures; python_version == "2.7"
 jaraco.context
 
 jaraco.text>=3.1
 
 portend
-pyopenssl
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+# and pyopenssl == 22 started requiring cryptography 35+
+# which is why we need these restrictions for the dependency resolution
+# to succeed.
+pyopenssl; implementation_name != "pypy"
+pyopenssl >= 22.0.0; implementation_name == "pypy" and python_version >= "3.8"
+pyopenssl < 22.0.0; implementation_name == "pypy" and python_version < "3.8"
 
 # The pypytools library provides a cross-implementation context
 # manager for disabling garbage collection in specific blocks
 # of the control flow:
 pypytools
 
 pytest-cov==2.8.1; python_version == "3.4"  # pyup: < 2.9
 pytest-cov==2.12.0; python_version != "3.4"
 pytest-forked>=1.1.3; sys_platform != "win32" and python_version >= '3.0' and python_version <= '3.4'
 pytest-forked>=1.2.0; sys_platform != "win32" and (python_version < '3.0' or python_version > '3.4')
 pytest-mock>=1.11.0
-pytest-rerunfailures < 10; python_version >= "3.0" and python_version < "3.6"
-pytest-rerunfailures < 9; python_version <= "2.7"
+pytest-rerunfailures < 9; python_version <= "2.7" or python_version == "3.4"
+pytest-rerunfailures < 10; python_version == "3.5"
 pytest-rerunfailures; python_version >= "3.6"
 pytest-sugar>=0.9.3
 pytest-watch==4.2.0
 pytest-xdist>=1.28.0
-pytest>=4.6.6
+
+# pytest-forked is currently incompatible with pytest 7
+pytest >= 4.6.6, < 7
 
 # HTTP over UNIX socket
 requests-unixsocket
 requests_toolbelt
 
 # TLS
 trustme>=0.4.0
@@ -64,7 +79,10 @@
 # It's a transitive dependency of requests library.
 # Also: requests>=2.22.0 doesn't support Python 3.4
 # yet requests==2.21.0 doesn't support urllib3>=1.25
 # Allowing requests with a lower urllib3 version
 # so that tests'd pass
 urllib3>=1.25; python_version != "3.4"
 watchdog<1.0.0; python_version < "3.6"
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+cryptography < 3.4; implementation_name == "pypy" and python_version < "3.8"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheroot-8.6.0/requirements/tox-py27-cp27-linux-x86_64.in` & `cheroot-9.0.0/requirements/tox-py27-cp27-darwin-x86_64.in`

 * *Files 26% similar despite different names*

```diff
@@ -12,49 +12,64 @@
 # ```
 # UserWarning: Trying to detect encoding from a tiny portion
 # of (12) byte(s).
 # ```
 # Ref: https://github.com/psf/requests/commit/2ed84f5
 # To avoid the warning, we declare a direct dependency on chardet
 # here so that it's use is adjusted across Python 2 and Python 3:
-chardet
+requests[use_chardet_on_py3]
+
+# Updating `charset-normalizer` on Python 3.5 under Ubuntu 18.04 causes
+# some weird issues with `cryptography` — it starts wanting `libffi7`
+# but only `libffi6` is available in that environment.
+# Note that there's no `charset-normalizer` for Python 2
+charset-normalizer < 2.1.0; python_version >= "3.0" and python_version <= "3.5"
 
 # Address https://github.com/tartley/colorama/issues/240.
 # It's a transitive dependency of pytest-watch plugin.
 colorama!=0.4.2; python_version == "3.4"
 
 # measure test coverage
-coverage == 6.2; python_version >= "3.6"
+coverage >= 6.2; python_version >= "3.6"
 coverage < 5; python_version == "3.4"
 coverage < 6; python_version < "3.6" and python_version != "3.4"
 futures; python_version == "2.7"
 jaraco.context
 
 jaraco.text>=3.1
 
 portend
-pyopenssl
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+# and pyopenssl == 22 started requiring cryptography 35+
+# which is why we need these restrictions for the dependency resolution
+# to succeed.
+pyopenssl; implementation_name != "pypy"
+pyopenssl >= 22.0.0; implementation_name == "pypy" and python_version >= "3.8"
+pyopenssl < 22.0.0; implementation_name == "pypy" and python_version < "3.8"
 
 # The pypytools library provides a cross-implementation context
 # manager for disabling garbage collection in specific blocks
 # of the control flow:
 pypytools
 
 pytest-cov==2.8.1; python_version == "3.4"  # pyup: < 2.9
 pytest-cov==2.12.0; python_version != "3.4"
 pytest-forked>=1.1.3; sys_platform != "win32" and python_version >= '3.0' and python_version <= '3.4'
 pytest-forked>=1.2.0; sys_platform != "win32" and (python_version < '3.0' or python_version > '3.4')
 pytest-mock>=1.11.0
-pytest-rerunfailures < 10; python_version >= "3.0" and python_version < "3.6"
-pytest-rerunfailures < 9; python_version <= "2.7"
+pytest-rerunfailures < 9; python_version <= "2.7" or python_version == "3.4"
+pytest-rerunfailures < 10; python_version == "3.5"
 pytest-rerunfailures; python_version >= "3.6"
 pytest-sugar>=0.9.3
 pytest-watch==4.2.0
 pytest-xdist>=1.28.0
-pytest>=4.6.6
+
+# pytest-forked is currently incompatible with pytest 7
+pytest >= 4.6.6, < 7
 
 # HTTP over UNIX socket
 requests-unixsocket
 requests_toolbelt
 
 # TLS
 trustme>=0.4.0
@@ -64,7 +79,10 @@
 # It's a transitive dependency of requests library.
 # Also: requests>=2.22.0 doesn't support Python 3.4
 # yet requests==2.21.0 doesn't support urllib3>=1.25
 # Allowing requests with a lower urllib3 version
 # so that tests'd pass
 urllib3>=1.25; python_version != "3.4"
 watchdog<1.0.0; python_version < "3.6"
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+cryptography < 3.4; implementation_name == "pypy" and python_version < "3.8"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheroot-8.6.0/requirements/tox-py27-cp27-linux-x86_64.txt` & `cheroot-9.0.0/requirements/tox-py27-cp27-linux-x86_64.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #
 # This file is autogenerated by pip-compile
 # To update, run:
 #
 #    pip-compile --allow-unsafe --output-file=requirements/tox-py27-cp27-linux-x86_64.txt requirements/tox-py27-cp27-linux-x86_64.in
 #
-atomicwrites==1.4.0
+atomicwrites==1.4.1
     # via pytest
-attrs==21.2.0
+attrs==21.4.0
     # via pytest
 backports.functools-lru-cache==1.6.4
     # via
+    #   cheroot
     #   jaraco.functools
     #   wcwidth
 certifi==2021.10.8
     # via requests
-cffi==1.15.0
+cffi==1.15.1
     # via cryptography
 chardet==4.0.0
-    # via
-    #   -r requirements/tox-py27-cp27-linux-x86_64.in
-    #   requests
-colorama==0.4.4
+    # via requests
+colorama==0.4.6
     # via pytest-watch
 configparser==4.0.2
     # via importlib-metadata
 contextlib2==0.6.0.post1
     # via
     #   importlib-metadata
     #   importlib-resources
     #   jaraco.context
     #   yg.lockfile
     #   zipp
-coverage[toml]==5.5 ; python_version < "3.6" and python_version != "3.4"
+coverage==5.5 ; python_version < "3.6" and python_version != "3.4"
     # via
     #   -r requirements/tox-py27-cp27-linux-x86_64.in
     #   pytest-cov
 cryptography==3.3.2
     # via
     #   pyopenssl
     #   trustme
@@ -45,52 +44,55 @@
     # via cryptography
 execnet==1.9.0
     # via pytest-xdist
 funcsigs==1.0.2
     # via
     #   mock
     #   pytest
-futures==3.3.0 ; python_version == "2.7"
+futures==3.4.0 ; python_version == "2.7"
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 idna==2.10
     # via
     #   requests
     #   trustme
-importlib-metadata==2.1.2
+importlib-metadata==2.1.3
     # via
+    #   cheroot
     #   pluggy
     #   pytest
 importlib-resources==3.3.1
     # via jaraco.text
 ipaddress==1.0.23
     # via
     #   cryptography
     #   trustme
 jaraco.apt==2.0
     # via jaraco.context
 jaraco.context==2.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 jaraco.functools==2.0
     # via
+    #   cheroot
     #   jaraco.text
     #   tempora
     #   yg.lockfile
 jaraco.text==3.2.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 mock==3.0.5
     # via pytest-mock
 more-itertools==5.0.0
     # via
+    #   cheroot
     #   jaraco.functools
     #   pytest
 packaging==20.9
     # via
     #   pytest
     #   pytest-sugar
-pathlib2==2.3.6
+pathlib2==2.3.7.post1
     # via
     #   importlib-metadata
     #   importlib-resources
     #   pytest
 pathtools==0.1.2
     # via watchdog
 pluggy==0.13.1
@@ -100,31 +102,31 @@
 py==1.11.0
     # via
     #   pypytools
     #   pytest
     #   pytest-forked
 pycparser==2.21
     # via cffi
-pyopenssl==21.0.0
+pyopenssl==21.0.0 ; implementation_name != "pypy"
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 pyparsing==2.4.7
     # via packaging
 pypytools==0.6.2
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 pytest-cov==2.12.0 ; python_version != "3.4"
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 pytest-forked==1.3.0 ; sys_platform != "win32" and (python_version < "3.0" or python_version > "3.4")
     # via
     #   -r requirements/tox-py27-cp27-linux-x86_64.in
     #   pytest-xdist
 pytest-mock==2.0.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
-pytest-rerunfailures==8.0 ; python_version <= "2.7"
+pytest-rerunfailures==8.0 ; python_version <= "2.7" or python_version == "3.4"
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
-pytest-sugar==0.9.4
+pytest-sugar==0.9.6
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 pytest-watch==4.2.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 pytest-xdist==1.34.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 pytest==4.6.11
     # via
@@ -132,30 +134,34 @@
     #   pytest-cov
     #   pytest-forked
     #   pytest-mock
     #   pytest-rerunfailures
     #   pytest-sugar
     #   pytest-watch
     #   pytest-xdist
-pytz==2021.3
+pytz==2022.6
     # via tempora
-requests-toolbelt==0.9.1
+requests-toolbelt==0.10.1
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
-requests-unixsocket==0.2.0
+requests-unixsocket==0.3.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
-requests==2.26.0
+requests==2.27.1
     # via
+    #   -r requirements/tox-py27-cp27-linux-x86_64.in
     #   requests-toolbelt
     #   requests-unixsocket
 scandir==1.10.0
     # via pathlib2
+selectors2==2.0.2
+    # via cheroot
 singledispatch==3.7.0
     # via importlib-resources
 six==1.16.0
     # via
+    #   cheroot
     #   cryptography
     #   jaraco.apt
     #   jaraco.text
     #   mock
     #   more-itertools
     #   pathlib2
     #   pyopenssl
@@ -170,20 +176,21 @@
 termcolor==1.1.0
     # via pytest-sugar
 toml==0.10.2
     # via coverage
 trustme==0.9.0
     # via -r requirements/tox-py27-cp27-linux-x86_64.in
 typing==3.10.0.0
-    # via importlib-resources
-urllib3==1.26.7 ; python_version != "3.4"
+    # via
+    #   importlib-resources
+    #   pathlib2
+urllib3==1.26.12 ; python_version != "3.4"
     # via
     #   -r requirements/tox-py27-cp27-linux-x86_64.in
     #   requests
-    #   requests-unixsocket
 watchdog==0.10.7 ; python_version < "3.6"
     # via
     #   -r requirements/tox-py27-cp27-linux-x86_64.in
     #   pytest-watch
 wcwidth==0.2.5
     # via pytest
 yg.lockfile==2.3
```

### Comparing `cheroot-8.6.0/requirements/tox-py310-cp310-linux-x86_64.in` & `cheroot-9.0.0/requirements/tox-py27-cp27-linux-x86_64.in`

 * *Files 26% similar despite different names*

```diff
@@ -12,49 +12,64 @@
 # ```
 # UserWarning: Trying to detect encoding from a tiny portion
 # of (12) byte(s).
 # ```
 # Ref: https://github.com/psf/requests/commit/2ed84f5
 # To avoid the warning, we declare a direct dependency on chardet
 # here so that it's use is adjusted across Python 2 and Python 3:
-chardet
+requests[use_chardet_on_py3]
+
+# Updating `charset-normalizer` on Python 3.5 under Ubuntu 18.04 causes
+# some weird issues with `cryptography` — it starts wanting `libffi7`
+# but only `libffi6` is available in that environment.
+# Note that there's no `charset-normalizer` for Python 2
+charset-normalizer < 2.1.0; python_version >= "3.0" and python_version <= "3.5"
 
 # Address https://github.com/tartley/colorama/issues/240.
 # It's a transitive dependency of pytest-watch plugin.
 colorama!=0.4.2; python_version == "3.4"
 
 # measure test coverage
-coverage == 6.2; python_version >= "3.6"
+coverage >= 6.2; python_version >= "3.6"
 coverage < 5; python_version == "3.4"
 coverage < 6; python_version < "3.6" and python_version != "3.4"
 futures; python_version == "2.7"
 jaraco.context
 
 jaraco.text>=3.1
 
 portend
-pyopenssl
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+# and pyopenssl == 22 started requiring cryptography 35+
+# which is why we need these restrictions for the dependency resolution
+# to succeed.
+pyopenssl; implementation_name != "pypy"
+pyopenssl >= 22.0.0; implementation_name == "pypy" and python_version >= "3.8"
+pyopenssl < 22.0.0; implementation_name == "pypy" and python_version < "3.8"
 
 # The pypytools library provides a cross-implementation context
 # manager for disabling garbage collection in specific blocks
 # of the control flow:
 pypytools
 
 pytest-cov==2.8.1; python_version == "3.4"  # pyup: < 2.9
 pytest-cov==2.12.0; python_version != "3.4"
 pytest-forked>=1.1.3; sys_platform != "win32" and python_version >= '3.0' and python_version <= '3.4'
 pytest-forked>=1.2.0; sys_platform != "win32" and (python_version < '3.0' or python_version > '3.4')
 pytest-mock>=1.11.0
-pytest-rerunfailures < 10; python_version >= "3.0" and python_version < "3.6"
-pytest-rerunfailures < 9; python_version <= "2.7"
+pytest-rerunfailures < 9; python_version <= "2.7" or python_version == "3.4"
+pytest-rerunfailures < 10; python_version == "3.5"
 pytest-rerunfailures; python_version >= "3.6"
 pytest-sugar>=0.9.3
 pytest-watch==4.2.0
 pytest-xdist>=1.28.0
-pytest>=4.6.6
+
+# pytest-forked is currently incompatible with pytest 7
+pytest >= 4.6.6, < 7
 
 # HTTP over UNIX socket
 requests-unixsocket
 requests_toolbelt
 
 # TLS
 trustme>=0.4.0
@@ -64,7 +79,10 @@
 # It's a transitive dependency of requests library.
 # Also: requests>=2.22.0 doesn't support Python 3.4
 # yet requests==2.21.0 doesn't support urllib3>=1.25
 # Allowing requests with a lower urllib3 version
 # so that tests'd pass
 urllib3>=1.25; python_version != "3.4"
 watchdog<1.0.0; python_version < "3.6"
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+cryptography < 3.4; implementation_name == "pypy" and python_version < "3.8"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheroot-8.6.0/requirements/tox-py310-cp310-linux-x86_64.txt` & `cheroot-9.0.0/requirements/tox-py39-cp39-linux-x86_64.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,138 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
+# This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/tox-py310-cp310-linux-x86_64.txt --strip-extras requirements/tox-py310-cp310-linux-x86_64.in
+#    pip-compile --allow-unsafe --output-file=requirements/tox-py39-cp39-linux-x86_64.txt --resolver=backtracking --strip-extras requirements/tox-py39-cp39-linux-x86_64.in setup.cfg
 #
-attrs==21.2.0
+attrs==22.1.0
     # via pytest
-certifi==2021.10.8
+autocommand==2.2.1
+    # via jaraco-text
+certifi==2022.9.24
     # via requests
-cffi==1.15.0
+cffi==1.15.1
     # via cryptography
-chardet==4.0.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-charset-normalizer==2.0.9
+chardet==5.0.0
     # via requests
-colorama==0.4.4
+charset-normalizer==2.1.1
+    # via requests
+colorama==0.4.6
     # via pytest-watch
-coverage==6.2 ; python_version >= "3.6"
+coverage==6.5.0 ; python_version >= "3.6"
     # via
-    #   -r requirements/tox-py310-cp310-linux-x86_64.in
+    #   -r requirements/tox-py39-cp39-linux-x86_64.in
     #   pytest-cov
-cryptography==36.0.0
+cryptography==38.0.3
     # via
     #   pyopenssl
     #   trustme
 docopt==0.6.2
     # via pytest-watch
 execnet==1.9.0
     # via pytest-xdist
-idna==3.3
+idna==3.4
     # via
     #   requests
     #   trustme
+inflect==6.0.2
+    # via jaraco-text
 iniconfig==1.1.1
     # via pytest
-jaraco.context==4.1.1
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-jaraco.functools==3.4.0
+jaraco-context==4.1.2
+    # via
+    #   -r requirements/tox-py39-cp39-linux-x86_64.in
+    #   jaraco-text
+jaraco-functools==3.5.2
     # via
-    #   jaraco.text
+    #   cheroot (setup.cfg)
+    #   jaraco-text
     #   tempora
-jaraco.text==3.6.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-more-itertools==8.12.0
-    # via jaraco.functools
+jaraco-text==3.10.0
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+more-itertools==9.0.0 ; python_version >= "3.6"
+    # via
+    #   cheroot (setup.cfg)
+    #   jaraco-functools
+    #   jaraco-text
 packaging==21.3
     # via
     #   pytest
     #   pytest-sugar
 pluggy==1.0.0
     # via pytest
 portend==3.1.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
 py==1.11.0
     # via
     #   pypytools
     #   pytest
     #   pytest-forked
 pycparser==2.21
     # via cffi
-pyopenssl==21.0.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-pyparsing==3.0.6
+pydantic==1.10.2
+    # via inflect
+pyopenssl==22.1.0 ; implementation_name != "pypy"
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+pyparsing==3.0.9
     # via packaging
 pypytools==0.6.2
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
 pytest==6.2.5
     # via
-    #   -r requirements/tox-py310-cp310-linux-x86_64.in
+    #   -r requirements/tox-py39-cp39-linux-x86_64.in
     #   pytest-cov
     #   pytest-forked
     #   pytest-mock
     #   pytest-rerunfailures
     #   pytest-sugar
     #   pytest-watch
     #   pytest-xdist
 pytest-cov==2.12.0 ; python_version != "3.4"
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-pytest-forked==1.3.0 ; sys_platform != "win32" and (python_version < "3.0" or python_version > "3.4")
-    # via
-    #   -r requirements/tox-py310-cp310-linux-x86_64.in
-    #   pytest-xdist
-pytest-mock==3.6.1
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+pytest-forked==1.4.0 ; sys_platform != "win32" and (python_version < "3.0" or python_version > "3.4")
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+pytest-mock==3.10.0
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
 pytest-rerunfailures==10.2 ; python_version >= "3.6"
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-pytest-sugar==0.9.4
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+pytest-sugar==0.9.6
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
 pytest-watch==4.2.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-pytest-xdist==2.4.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-pytz==2021.3
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+pytest-xdist==3.0.2
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+pytz==2022.6
     # via tempora
-requests==2.26.0
+requests==2.28.1
     # via
+    #   -r requirements/tox-py39-cp39-linux-x86_64.in
     #   requests-toolbelt
     #   requests-unixsocket
-requests-toolbelt==0.9.1
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-requests-unixsocket==0.2.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
+requests-toolbelt==0.10.1
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+requests-unixsocket==0.3.0
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
 six==1.16.0
-    # via pyopenssl
-tempora==4.1.2
+    # via cheroot (setup.cfg)
+tempora==5.0.2
     # via portend
-termcolor==1.1.0
+termcolor==2.1.0
     # via pytest-sugar
 toml==0.10.2
     # via pytest
-tomli==1.2.2
+tomli==2.0.1
     # via coverage
 trustme==0.9.0
-    # via -r requirements/tox-py310-cp310-linux-x86_64.in
-urllib3==1.26.7 ; python_version != "3.4"
+    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+typing-extensions==4.4.0
+    # via pydantic
+urllib3==1.26.12 ; python_version != "3.4"
     # via
-    #   -r requirements/tox-py310-cp310-linux-x86_64.in
+    #   -r requirements/tox-py39-cp39-linux-x86_64.in
     #   requests
-    #   requests-unixsocket
-watchdog==2.1.6
+watchdog==2.1.9
     # via pytest-watch
 
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==59.5.0
+setuptools==65.5.1
     # via pytest-rerunfailures
```

### Comparing `cheroot-8.6.0/requirements/tox-py39-cp39-linux-x86_64.in` & `cheroot-9.0.0/requirements/tox-py27-cp27-win32-amd64.in`

 * *Files 26% similar despite different names*

```diff
@@ -12,49 +12,64 @@
 # ```
 # UserWarning: Trying to detect encoding from a tiny portion
 # of (12) byte(s).
 # ```
 # Ref: https://github.com/psf/requests/commit/2ed84f5
 # To avoid the warning, we declare a direct dependency on chardet
 # here so that it's use is adjusted across Python 2 and Python 3:
-chardet
+requests[use_chardet_on_py3]
+
+# Updating `charset-normalizer` on Python 3.5 under Ubuntu 18.04 causes
+# some weird issues with `cryptography` — it starts wanting `libffi7`
+# but only `libffi6` is available in that environment.
+# Note that there's no `charset-normalizer` for Python 2
+charset-normalizer < 2.1.0; python_version >= "3.0" and python_version <= "3.5"
 
 # Address https://github.com/tartley/colorama/issues/240.
 # It's a transitive dependency of pytest-watch plugin.
 colorama!=0.4.2; python_version == "3.4"
 
 # measure test coverage
-coverage == 6.2; python_version >= "3.6"
+coverage >= 6.2; python_version >= "3.6"
 coverage < 5; python_version == "3.4"
 coverage < 6; python_version < "3.6" and python_version != "3.4"
 futures; python_version == "2.7"
 jaraco.context
 
 jaraco.text>=3.1
 
 portend
-pyopenssl
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+# and pyopenssl == 22 started requiring cryptography 35+
+# which is why we need these restrictions for the dependency resolution
+# to succeed.
+pyopenssl; implementation_name != "pypy"
+pyopenssl >= 22.0.0; implementation_name == "pypy" and python_version >= "3.8"
+pyopenssl < 22.0.0; implementation_name == "pypy" and python_version < "3.8"
 
 # The pypytools library provides a cross-implementation context
 # manager for disabling garbage collection in specific blocks
 # of the control flow:
 pypytools
 
 pytest-cov==2.8.1; python_version == "3.4"  # pyup: < 2.9
 pytest-cov==2.12.0; python_version != "3.4"
 pytest-forked>=1.1.3; sys_platform != "win32" and python_version >= '3.0' and python_version <= '3.4'
 pytest-forked>=1.2.0; sys_platform != "win32" and (python_version < '3.0' or python_version > '3.4')
 pytest-mock>=1.11.0
-pytest-rerunfailures < 10; python_version >= "3.0" and python_version < "3.6"
-pytest-rerunfailures < 9; python_version <= "2.7"
+pytest-rerunfailures < 9; python_version <= "2.7" or python_version == "3.4"
+pytest-rerunfailures < 10; python_version == "3.5"
 pytest-rerunfailures; python_version >= "3.6"
 pytest-sugar>=0.9.3
 pytest-watch==4.2.0
 pytest-xdist>=1.28.0
-pytest>=4.6.6
+
+# pytest-forked is currently incompatible with pytest 7
+pytest >= 4.6.6, < 7
 
 # HTTP over UNIX socket
 requests-unixsocket
 requests_toolbelt
 
 # TLS
 trustme>=0.4.0
@@ -64,7 +79,10 @@
 # It's a transitive dependency of requests library.
 # Also: requests>=2.22.0 doesn't support Python 3.4
 # yet requests==2.21.0 doesn't support urllib3>=1.25
 # Allowing requests with a lower urllib3 version
 # so that tests'd pass
 urllib3>=1.25; python_version != "3.4"
 watchdog<1.0.0; python_version < "3.6"
+
+# cryptography >= 3.4 started using Rust but it's unstable w/ old PyPy
+cryptography < 3.4; implementation_name == "pypy" and python_version < "3.8"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheroot-8.6.0/requirements/tox-py39-cp39-linux-x86_64.txt` & `cheroot-9.0.0/requirements/tox-py38-cp38-linux-x86_64.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,126 +1,142 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
+# This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/tox-py39-cp39-linux-x86_64.txt --strip-extras requirements/tox-py39-cp39-linux-x86_64.in
+#    pip-compile --allow-unsafe --output-file=requirements/tox-py38-cp38-linux-x86_64.txt --resolver=backtracking --strip-extras requirements/tox-py38-cp38-linux-x86_64.in setup.cfg
 #
-attrs==21.2.0
+attrs==22.1.0
     # via pytest
-certifi==2021.10.8
+autocommand==2.2.1
+    # via jaraco-text
+certifi==2022.9.24
     # via requests
-cffi==1.15.0
+cffi==1.15.1
     # via cryptography
-chardet==4.0.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-charset-normalizer==2.0.9
+chardet==5.0.0
     # via requests
-colorama==0.4.4
+charset-normalizer==2.1.1
+    # via requests
+colorama==0.4.6
     # via pytest-watch
-coverage==6.2 ; python_version >= "3.6"
+coverage==6.5.0 ; python_version >= "3.6"
     # via
-    #   -r requirements/tox-py39-cp39-linux-x86_64.in
+    #   -r requirements/tox-py38-cp38-linux-x86_64.in
     #   pytest-cov
-cryptography==36.0.0
+cryptography==38.0.3
     # via
     #   pyopenssl
     #   trustme
 docopt==0.6.2
     # via pytest-watch
 execnet==1.9.0
     # via pytest-xdist
-idna==3.3
+idna==3.4
     # via
     #   requests
     #   trustme
+importlib-resources==5.10.0
+    # via jaraco-text
+inflect==6.0.2
+    # via jaraco-text
 iniconfig==1.1.1
     # via pytest
-jaraco.context==4.1.1
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-jaraco.functools==3.4.0
+jaraco-context==4.1.2
+    # via
+    #   -r requirements/tox-py38-cp38-linux-x86_64.in
+    #   jaraco-text
+jaraco-functools==3.5.2
     # via
-    #   jaraco.text
+    #   cheroot (setup.cfg)
+    #   jaraco-text
     #   tempora
-jaraco.text==3.6.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-more-itertools==8.12.0
-    # via jaraco.functools
+jaraco-text==3.10.0
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+more-itertools==9.0.0 ; python_version >= "3.6"
+    # via
+    #   cheroot (setup.cfg)
+    #   jaraco-functools
+    #   jaraco-text
 packaging==21.3
     # via
     #   pytest
     #   pytest-sugar
 pluggy==1.0.0
     # via pytest
 portend==3.1.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
 py==1.11.0
     # via
     #   pypytools
     #   pytest
     #   pytest-forked
 pycparser==2.21
     # via cffi
-pyopenssl==21.0.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-pyparsing==3.0.6
+pydantic==1.10.2
+    # via inflect
+pyopenssl==22.1.0 ; implementation_name != "pypy"
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+pyparsing==3.0.9
     # via packaging
 pypytools==0.6.2
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
 pytest==6.2.5
     # via
-    #   -r requirements/tox-py39-cp39-linux-x86_64.in
+    #   -r requirements/tox-py38-cp38-linux-x86_64.in
     #   pytest-cov
     #   pytest-forked
     #   pytest-mock
     #   pytest-rerunfailures
     #   pytest-sugar
     #   pytest-watch
     #   pytest-xdist
 pytest-cov==2.12.0 ; python_version != "3.4"
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
 pytest-forked==1.4.0 ; sys_platform != "win32" and (python_version < "3.0" or python_version > "3.4")
-    # via
-    #   -r requirements/tox-py39-cp39-linux-x86_64.in
-    #   pytest-xdist
-pytest-mock==3.6.1
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+pytest-mock==3.10.0
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
 pytest-rerunfailures==10.2 ; python_version >= "3.6"
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-pytest-sugar==0.9.4
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+pytest-sugar==0.9.6
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
 pytest-watch==4.2.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-pytest-xdist==2.5.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-pytz==2021.3
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+pytest-xdist==3.0.2
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+pytz==2022.6
     # via tempora
-requests==2.26.0
+requests==2.28.1
     # via
+    #   -r requirements/tox-py38-cp38-linux-x86_64.in
     #   requests-toolbelt
     #   requests-unixsocket
-requests-toolbelt==0.9.1
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-requests-unixsocket==0.2.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
+requests-toolbelt==0.10.1
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+requests-unixsocket==0.3.0
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
 six==1.16.0
-    # via pyopenssl
-tempora==4.1.2
+    # via cheroot (setup.cfg)
+tempora==5.0.2
     # via portend
-termcolor==1.1.0
+termcolor==2.1.0
     # via pytest-sugar
 toml==0.10.2
     # via pytest
-tomli==1.2.2
+tomli==2.0.1
     # via coverage
 trustme==0.9.0
-    # via -r requirements/tox-py39-cp39-linux-x86_64.in
-urllib3==1.26.7 ; python_version != "3.4"
+    # via -r requirements/tox-py38-cp38-linux-x86_64.in
+typing-extensions==4.4.0
+    # via pydantic
+urllib3==1.26.12 ; python_version != "3.4"
     # via
-    #   -r requirements/tox-py39-cp39-linux-x86_64.in
+    #   -r requirements/tox-py38-cp38-linux-x86_64.in
     #   requests
-    #   requests-unixsocket
-watchdog==2.1.6
+watchdog==2.1.9
     # via pytest-watch
+zipp==3.10.0
+    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==59.5.0
+setuptools==65.5.1
     # via pytest-rerunfailures
```

### Comparing `cheroot-8.6.0/setup.cfg` & `cheroot-9.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,22 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Framework :: CherryPy
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.4
-	Programming Language :: Python :: 3.5
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: Jython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: HTTP Servers
 	Topic :: Internet :: WWW/HTTP :: WSGI
@@ -47,23 +46,24 @@
 	http
 	server
 	ssl
 	wsgi
 
 [options]
 use_scm_version = True
-python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+python_requires = >=3.6
 packages = find:
 include_package_data = True
 setup_requires = 
 	setuptools_scm>=1.15.0
 	setuptools_scm_git_archive>=1.0
 install_requires = 
 	backports.functools_lru_cache; python_version < '3.3'
 	selectors2; python_version< '3.4'
+	importlib_metadata; python_version < '3.8'
 	six>=1.11.0
 	more_itertools >= 2.6, < 8.11.0; python_version < '3.6'
 	more_itertools >= 2.6; python_version >= '3.6'
 	jaraco.functools
 
 [options.extras_require]
 docs =
```

