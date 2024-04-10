# Comparing `tmp/go-inspector-0.2.0.tar.gz` & `tmp/go-inspector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go-inspector-0.2.0.tar", last modified: Tue Apr  9 13:57:45 2024, max compression
+gzip compressed data, was "go-inspector-0.2.1.tar", last modified: Wed Apr 10 08:52:30 2024, max compression
```

## Comparing `go-inspector-0.2.0.tar` & `go-inspector-0.2.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.553241 go-inspector-0.2.0/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       89 2024-02-29 13:17:31.000000 go-inspector-0.2.0/.gitattributes
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:31.225137 go-inspector-0.2.0/.github/
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.529241 go-inspector-0.2.0/.github/workflows/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      752 2024-02-29 13:17:31.000000 go-inspector-0.2.0/.github/workflows/docs-ci.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2023 2024-02-29 13:17:31.000000 go-inspector-0.2.0/.github/workflows/pypi-release.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      755 2024-02-29 13:17:31.000000 go-inspector-0.2.0/.gitignore
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      525 2024-02-29 13:17:31.000000 go-inspector-0.2.0/.readthedocs.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      144 2024-04-09 10:40:33.000000 go-inspector-0.2.0/AUTHORS.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      292 2024-04-09 11:37:50.000000 go-inspector-0.2.0/CHANGELOG.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     3422 2024-02-29 13:17:31.000000 go-inspector-0.2.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      217 2024-02-29 13:17:31.000000 go-inspector-0.2.0/MANIFEST.in
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1596 2024-02-29 13:17:31.000000 go-inspector-0.2.0/Makefile
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      829 2024-04-09 13:16:50.000000 go-inspector-0.2.0/NOTICE
--rw-r--r--   0 pombreda  (1001) pombreda  (1001)     4105 2024-04-09 13:57:45.553241 go-inspector-0.2.0/PKG-INFO
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2382 2024-04-09 13:23:33.000000 go-inspector-0.2.0/README.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    11357 2024-02-29 13:17:31.000000 go-inspector-0.2.0/apache-2.0.LICENSE
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2266 2024-04-09 11:37:22.000000 go-inspector-0.2.0/azure-pipelines.yml
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)     6328 2024-02-29 13:17:31.000000 go-inspector-0.2.0/configure
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     6948 2024-02-29 13:17:31.000000 go-inspector-0.2.0/configure.bat
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.529241 go-inspector-0.2.0/docs/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      890 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/Makefile
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1071 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/make.bat
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.529241 go-inspector-0.2.0/docs/scripts/
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)      131 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/scripts/doc8_style_check.sh
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      124 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/scripts/sphinx_build_link_check.sh
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.533241 go-inspector-0.2.0/docs/source/
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.533241 go-inspector-0.2.0/docs/source/_static/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      474 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/source/_static/theme_overrides.css
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     3518 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/source/conf.py
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.533241 go-inspector-0.2.0/docs/source/contribute/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    10245 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/source/contribute/contrib_doc.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      274 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/source/index.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     5491 2024-02-29 13:17:31.000000 go-inspector-0.2.0/docs/source/skeleton-usage.rst
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:31.225137 go-inspector-0.2.0/etc/
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.533241 go-inspector-0.2.0/etc/ci/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1700 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/azure-container-deb.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1753 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/azure-container-rpm.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1240 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/azure-posix.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1215 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/azure-win.yml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      257 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/install_sudo.sh
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     8365 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/macports-ci
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      684 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/macports-ci.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1022 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/ci/mit.LICENSE
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.537241 go-inspector-0.2.0/etc/scripts/
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)     3744 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/README.rst
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1301 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/check_thirdparty.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     9486 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/fetch_thirdparty.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     9699 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/gen_pypi_simple.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      354 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2776 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1715 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/gen_requirements.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2266 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/gen_requirements_dev.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      101 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/requirements.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     4497 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      504 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2839 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      773 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     6418 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_dejacode.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     6704 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      494 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2850 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_pypi_supported_tags.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      741 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     6152 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_requirements.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    75931 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_thirdparty.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      608 2024-02-29 13:17:31.000000 go-inspector-0.2.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      867 2024-02-29 13:17:31.000000 go-inspector-0.2.0/pyproject.toml
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)        0 2024-02-29 13:17:31.000000 go-inspector-0.2.0/requirements-dev.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       26 2024-02-29 13:17:31.000000 go-inspector-0.2.0/requirements.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1476 2024-04-09 13:57:45.557242 go-inspector-0.2.0/setup.cfg
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       92 2024-02-29 13:17:31.000000 go-inspector-0.2.0/setup.py
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:31.225137 go-inspector-0.2.0/src/
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.537241 go-inspector-0.2.0/src/go_inspector/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       22 2024-04-09 11:50:04.000000 go-inspector-0.2.0/src/go_inspector/__init__.py
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.537241 go-inspector-0.2.0/src/go_inspector/bin/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       78 2024-04-09 10:33:35.000000 go-inspector-0.2.0/src/go_inspector/bin/GoReSym.zip.sums
--rwxrw-r--   0 pombreda  (1001) pombreda  (1001)  4651346 2024-02-23 16:52:56.000000 go-inspector-0.2.0/src/go_inspector/bin/GoReSym_lin
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      516 2024-04-09 10:31:52.000000 go-inspector-0.2.0/src/go_inspector/bin/GoReSym_lin.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1064 2024-04-09 10:23:22.000000 go-inspector-0.2.0/src/go_inspector/bin/GoReSym_lin.LICENSE
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      618 2024-04-09 11:08:16.000000 go-inspector-0.2.0/src/go_inspector/bin/arch-52c3e6f60cffa0133a3f9b2fc7f6862504a6cba0.tar.gz.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      402 2024-04-09 11:08:48.000000 go-inspector-0.2.0/src/go_inspector/bin/binaryregexp-0.2.0.tar.gz.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1427 2024-04-09 11:07:22.000000 go-inspector-0.2.0/src/go_inspector/bin/bsd-new.LICENSE
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      615 2024-04-09 11:08:26.000000 go-inspector-0.2.0/src/go_inspector/bin/exp-89c5cff77bcbacf5bc89bd83d69d4fa8c80cf8af.tar.gz.ABOUT
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1302 2024-04-09 11:07:22.000000 go-inspector-0.2.0/src/go_inspector/bin/google-patent-license-golang.LICENSE
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1022 2024-04-09 11:07:22.000000 go-inspector-0.2.0/src/go_inspector/bin/mit.LICENSE
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      400 2024-04-09 11:08:38.000000 go-inspector-0.2.0/src/go_inspector/bin/orderedmap-1.4.0.tar.gz.ABOUT
--rwxrw-r--   0 pombreda  (1001) pombreda  (1001)      870 2024-04-09 11:09:42.000000 go-inspector-0.2.0/src/go_inspector/bin/update.sh
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     3680 2024-04-09 13:30:01.000000 go-inspector-0.2.0/src/go_inspector/plugin.py
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.549241 go-inspector-0.2.0/src/go_inspector.egg-info/
--rw-r--r--   0 pombreda  (1001) pombreda  (1001)     4105 2024-04-09 13:57:45.000000 go-inspector-0.2.0/src/go_inspector.egg-info/PKG-INFO
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     3026 2024-04-09 13:57:45.000000 go-inspector-0.2.0/src/go_inspector.egg-info/SOURCES.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)        1 2024-04-09 13:57:45.000000 go-inspector-0.2.0/src/go_inspector.egg-info/dependency_links.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       70 2024-04-09 13:57:45.000000 go-inspector-0.2.0/src/go_inspector.egg-info/entry_points.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)        1 2024-04-09 13:56:22.000000 go-inspector-0.2.0/src/go_inspector.egg-info/not-zip-safe
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      303 2024-04-09 13:57:45.000000 go-inspector-0.2.0/src/go_inspector.egg-info/requires.txt
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)       13 2024-04-09 13:57:45.000000 go-inspector-0.2.0/src/go_inspector.egg-info/top_level.txt
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.537241 go-inspector-0.2.0/tests/
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.541241 go-inspector-0.2.0/tests/data/
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    29462 2024-04-09 13:30:08.000000 go-inspector-0.2.0/tests/data/GoReSym_lin-goresym.json
-drwxrwxr-x   0 pombreda  (1001) pombreda  (1001)        0 2024-04-09 13:57:45.549241 go-inspector-0.2.0/tests/data/basic/
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)  1818279 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/data/basic/app_lin_exe
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    10732 2024-04-09 13:30:07.000000 go-inspector-0.2.0/tests/data/basic/app_lin_exe-goresym.json
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    11829 2024-04-09 13:30:10.000000 go-inspector-0.2.0/tests/data/basic/app_lin_exe-scancode.expected.json
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)  1182296 2024-04-09 13:21:18.000000 go-inspector-0.2.0/tests/data/basic/app_lin_exe_stripped
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    10732 2024-04-09 13:30:08.000000 go-inspector-0.2.0/tests/data/basic/app_lin_exe_stripped-goresym.json
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)  1975746 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/data/basic/app_mac_exe
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    11347 2024-04-09 13:30:08.000000 go-inspector-0.2.0/tests/data/basic/app_mac_exe-goresym.json
--rwxrwxr-x   0 pombreda  (1001) pombreda  (1001)  1930240 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/data/basic/app_win_exe
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    10520 2024-04-09 13:30:08.000000 go-inspector-0.2.0/tests/data/basic/app_win_exe-goresym.json
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)      121 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/data/basic/main.go
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)   193855 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/data/plain_arm_gentoo_elf
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)    45056 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/data/plain_windows.exe
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     2491 2024-04-09 13:22:01.000000 go-inspector-0.2.0/tests/test_go_inspector.py
--rw-rw-r--   0 pombreda  (1001) pombreda  (1001)     1305 2024-02-29 13:17:31.000000 go-inspector-0.2.0/tests/test_skeleton_codestyle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.934898 go-inspector-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 08:52:26.000000 go-inspector-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.910898 go-inspector-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.914898 go-inspector-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 08:52:26.000000 go-inspector-0.2.1/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-10 08:52:26.000000 go-inspector-0.2.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 08:52:26.000000 go-inspector-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-10 08:52:26.000000 go-inspector-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 08:52:26.000000 go-inspector-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 08:52:26.000000 go-inspector-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-10 08:52:26.000000 go-inspector-0.2.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-10 08:52:26.000000 go-inspector-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-10 08:52:26.000000 go-inspector-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-10 08:52:26.000000 go-inspector-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-10 08:52:30.934898 go-inspector-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-10 08:52:26.000000 go-inspector-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 08:52:26.000000 go-inspector-0.2.1/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 08:52:26.000000 go-inspector-0.2.1/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6328 2024-04-10 08:52:26.000000 go-inspector-0.2.1/configure
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-10 08:52:26.000000 go-inspector-0.2.1/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.914898 go-inspector-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.914898 go-inspector-0.2.1/docs/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.914898 go-inspector-0.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.918898 go-inspector-0.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.918898 go-inspector-0.2.1/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-10 08:52:26.000000 go-inspector-0.2.1/docs/source/skeleton-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.910898 go-inspector-0.2.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.918898 go-inspector-0.2.1/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.922898 go-inspector-0.2.1/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75931 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-10 08:52:26.000000 go-inspector-0.2.1/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-10 08:52:26.000000 go-inspector-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:26.000000 go-inspector-0.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 08:52:26.000000 go-inspector-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-10 08:52:30.934898 go-inspector-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 08:52:26.000000 go-inspector-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.910898 go-inspector-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.922898 go-inspector-0.2.1/src/go_inspector/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.926898 go-inspector-0.2.1/src/go_inspector/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/GoReSym.zip.sums
+-rwxr-xr-x   0 runner    (1001) docker     (127)  4651346 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/GoReSym_lin
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/GoReSym_lin.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/GoReSym_lin.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/arch-52c3e6f60cffa0133a3f9b2fc7f6862504a6cba0.tar.gz.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/binaryregexp-0.2.0.tar.gz.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/exp-89c5cff77bcbacf5bc89bd83d69d4fa8c80cf8af.tar.gz.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/google-patent-license-golang.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/orderedmap-1.4.0.tar.gz.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (127)      870 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/bin/update.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-10 08:52:26.000000 go-inspector-0.2.1/src/go_inspector/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.934898 go-inspector-0.2.1/src/go_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 08:52:30.000000 go-inspector-0.2.1/src/go_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.926898 go-inspector-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.926898 go-inspector-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/GoReSym_lin-goresym.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:52:30.934898 go-inspector-0.2.1/tests/data/basic/
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1818279 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_lin_exe
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_lin_exe-goresym.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_lin_exe-scancode.expected.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1182296 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_lin_exe_stripped
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_lin_exe_stripped-goresym.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1975746 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_mac_exe
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_mac_exe-goresym.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1930240 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_win_exe
+-rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/app_win_exe-goresym.json
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/basic/main.go
+-rw-r--r--   0 runner    (1001) docker     (127)   193855 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/plain_arm_gentoo_elf
+-rw-r--r--   0 runner    (1001) docker     (127)    45056 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/data/plain_windows.exe
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/test_go_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-10 08:52:26.000000 go-inspector-0.2.1/tests/test_skeleton_codestyle.py
```

### Comparing `go-inspector-0.2.0/.github/workflows/docs-ci.yml` & `go-inspector-0.2.1/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/.github/workflows/pypi-release.yml` & `go-inspector-0.2.1/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/.gitignore` & `go-inspector-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/.readthedocs.yml` & `go-inspector-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/CODE_OF_CONDUCT.rst` & `go-inspector-0.2.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/Makefile` & `go-inspector-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/NOTICE` & `go-inspector-0.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/PKG-INFO` & `go-inspector-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: go-inspector
-Version: 0.2.0
+Version: 0.2.1
 Summary: go-inspector is a scancode plugin to extract symbols and dependencies found in Go binaries.
 Home-page: https://github.com/nexB/go-inspector
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0 AND MIT AND BSD-3-Clause WITH LicenRef-scancode-google-patent-license-golang
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,26 +41,26 @@
 Requires-Dist: sphinx-rtd-dark-mode>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 
 go-inspector
 ================================
 
 go-inspector is a utility to extract dependencies and symbols from Go binaries.
-It is desigend to work as a ScanCode Toolkit plugin.
+It is designed to work as a ScanCode Toolkit plugin and integrated in ScanCode.io
 
 To install and use:
 
 - Run ``pip install go-inspector``
 - Use with ``scancode --json-pp - --go-symbol --verbose <PATH to a tree or file with Go binaries>``
 
 The JSON output will contain various dependencies and symbols found in Go binaries if any.
 
 
 - License: Apache-2.0 AND MIT AND BSD-3-Clause WITH LicenRef-scancode-google-patent-license-golang
-- Copyright (c) nexB Inc., Mandiant, The Go Authors, Elliot Chance and others
+- Copyright (c) nexB Inc., Mandiant, The Go Authors, Elliot Chance and others.
 - Homepage: https://github.com/nexB/go-inspector/
 
 See the src/go_inspector/bin for detailed license and credits for bundled third-party packages.
 
 
 Development
 ----------------
```

### Comparing `go-inspector-0.2.0/README.rst` & `go-inspector-0.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 go-inspector
 ================================
 
 go-inspector is a utility to extract dependencies and symbols from Go binaries.
-It is desigend to work as a ScanCode Toolkit plugin.
+It is designed to work as a ScanCode Toolkit plugin and integrated in ScanCode.io
 
 To install and use:
 
 - Run ``pip install go-inspector``
 - Use with ``scancode --json-pp - --go-symbol --verbose <PATH to a tree or file with Go binaries>``
 
 The JSON output will contain various dependencies and symbols found in Go binaries if any.
 
 
 - License: Apache-2.0 AND MIT AND BSD-3-Clause WITH LicenRef-scancode-google-patent-license-golang
-- Copyright (c) nexB Inc., Mandiant, The Go Authors, Elliot Chance and others
+- Copyright (c) nexB Inc., Mandiant, The Go Authors, Elliot Chance and others.
 - Homepage: https://github.com/nexB/go-inspector/
 
 See the src/go_inspector/bin for detailed license and credits for bundled third-party packages.
 
 
 Development
 ----------------
```

### Comparing `go-inspector-0.2.0/apache-2.0.LICENSE` & `go-inspector-0.2.1/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/azure-pipelines.yml` & `go-inspector-0.2.1/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/configure` & `go-inspector-0.2.1/configure`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/configure.bat` & `go-inspector-0.2.1/configure.bat`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/docs/Makefile` & `go-inspector-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/docs/make.bat` & `go-inspector-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/docs/source/conf.py` & `go-inspector-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/docs/source/contribute/contrib_doc.rst` & `go-inspector-0.2.1/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/docs/source/skeleton-usage.rst` & `go-inspector-0.2.1/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/azure-container-deb.yml` & `go-inspector-0.2.1/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/azure-container-rpm.yml` & `go-inspector-0.2.1/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/azure-posix.yml` & `go-inspector-0.2.1/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/azure-win.yml` & `go-inspector-0.2.1/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/macports-ci` & `go-inspector-0.2.1/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/macports-ci.ABOUT` & `go-inspector-0.2.1/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/ci/mit.LICENSE` & `go-inspector-0.2.1/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/README.rst` & `go-inspector-0.2.1/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/check_thirdparty.py` & `go-inspector-0.2.1/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/fetch_thirdparty.py` & `go-inspector-0.2.1/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/gen_pypi_simple.py` & `go-inspector-0.2.1/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `go-inspector-0.2.1/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/gen_requirements.py` & `go-inspector-0.2.1/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/gen_requirements_dev.py` & `go-inspector-0.2.1/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `go-inspector-0.2.1/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/test_utils_pypi_supported_tags.py` & `go-inspector-0.2.1/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `go-inspector-0.2.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_dejacode.py` & `go-inspector-0.2.1/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_pip_compatibility_tags.py` & `go-inspector-0.2.1/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_pypi_supported_tags.py` & `go-inspector-0.2.1/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `go-inspector-0.2.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_requirements.py` & `go-inspector-0.2.1/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_thirdparty.py` & `go-inspector-0.2.1/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/etc/scripts/utils_thirdparty.py.ABOUT` & `go-inspector-0.2.1/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/pyproject.toml` & `go-inspector-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/setup.cfg` & `go-inspector-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/GoReSym_lin` & `go-inspector-0.2.1/src/go_inspector/bin/GoReSym_lin`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/GoReSym_lin.ABOUT` & `go-inspector-0.2.1/src/go_inspector/bin/GoReSym_lin.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/GoReSym_lin.LICENSE` & `go-inspector-0.2.1/src/go_inspector/bin/GoReSym_lin.LICENSE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/arch-52c3e6f60cffa0133a3f9b2fc7f6862504a6cba0.tar.gz.ABOUT` & `go-inspector-0.2.1/src/go_inspector/bin/arch-52c3e6f60cffa0133a3f9b2fc7f6862504a6cba0.tar.gz.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/bsd-new.LICENSE` & `go-inspector-0.2.1/src/go_inspector/bin/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/exp-89c5cff77bcbacf5bc89bd83d69d4fa8c80cf8af.tar.gz.ABOUT` & `go-inspector-0.2.1/src/go_inspector/bin/exp-89c5cff77bcbacf5bc89bd83d69d4fa8c80cf8af.tar.gz.ABOUT`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/google-patent-license-golang.LICENSE` & `go-inspector-0.2.1/src/go_inspector/bin/google-patent-license-golang.LICENSE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/mit.LICENSE` & `go-inspector-0.2.1/src/go_inspector/bin/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/bin/update.sh` & `go-inspector-0.2.1/src/go_inspector/bin/update.sh`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector/plugin.py` & `go-inspector-0.2.1/src/go_inspector/plugin.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/src/go_inspector.egg-info/PKG-INFO` & `go-inspector-0.2.1/src/go_inspector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: go-inspector
-Version: 0.2.0
+Version: 0.2.1
 Summary: go-inspector is a scancode plugin to extract symbols and dependencies found in Go binaries.
 Home-page: https://github.com/nexB/go-inspector
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0 AND MIT AND BSD-3-Clause WITH LicenRef-scancode-google-patent-license-golang
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,26 +41,26 @@
 Requires-Dist: sphinx-rtd-dark-mode>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 
 go-inspector
 ================================
 
 go-inspector is a utility to extract dependencies and symbols from Go binaries.
-It is desigend to work as a ScanCode Toolkit plugin.
+It is designed to work as a ScanCode Toolkit plugin and integrated in ScanCode.io
 
 To install and use:
 
 - Run ``pip install go-inspector``
 - Use with ``scancode --json-pp - --go-symbol --verbose <PATH to a tree or file with Go binaries>``
 
 The JSON output will contain various dependencies and symbols found in Go binaries if any.
 
 
 - License: Apache-2.0 AND MIT AND BSD-3-Clause WITH LicenRef-scancode-google-patent-license-golang
-- Copyright (c) nexB Inc., Mandiant, The Go Authors, Elliot Chance and others
+- Copyright (c) nexB Inc., Mandiant, The Go Authors, Elliot Chance and others.
 - Homepage: https://github.com/nexB/go-inspector/
 
 See the src/go_inspector/bin for detailed license and credits for bundled third-party packages.
 
 
 Development
 ----------------
```

### Comparing `go-inspector-0.2.0/src/go_inspector.egg-info/SOURCES.txt` & `go-inspector-0.2.1/src/go_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/GoReSym_lin-goresym.json` & `go-inspector-0.2.1/tests/data/GoReSym_lin-goresym.json`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_lin_exe` & `go-inspector-0.2.1/tests/data/basic/app_lin_exe`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_lin_exe-goresym.json` & `go-inspector-0.2.1/tests/data/basic/app_lin_exe-goresym.json`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_lin_exe-scancode.expected.json` & `go-inspector-0.2.1/tests/data/basic/app_lin_exe-scancode.expected.json`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_lin_exe_stripped` & `go-inspector-0.2.1/tests/data/basic/app_lin_exe_stripped`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_lin_exe_stripped-goresym.json` & `go-inspector-0.2.1/tests/data/basic/app_lin_exe_stripped-goresym.json`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_mac_exe` & `go-inspector-0.2.1/tests/data/basic/app_mac_exe`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_mac_exe-goresym.json` & `go-inspector-0.2.1/tests/data/basic/app_mac_exe-goresym.json`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_win_exe` & `go-inspector-0.2.1/tests/data/basic/app_win_exe`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/basic/app_win_exe-goresym.json` & `go-inspector-0.2.1/tests/data/basic/app_win_exe-goresym.json`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/plain_arm_gentoo_elf` & `go-inspector-0.2.1/tests/data/plain_arm_gentoo_elf`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/data/plain_windows.exe` & `go-inspector-0.2.1/tests/data/plain_windows.exe`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/test_go_inspector.py` & `go-inspector-0.2.1/tests/test_go_inspector.py`

 * *Files identical despite different names*

### Comparing `go-inspector-0.2.0/tests/test_skeleton_codestyle.py` & `go-inspector-0.2.1/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

