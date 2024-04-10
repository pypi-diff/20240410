# Comparing `tmp/protokolo-1.0.0.tar.gz` & `tmp/protokolo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-1.0.0.tar", max compression
+gzip compressed data, was "protokolo-1.0.1.tar", max compression
```

## Comparing `protokolo-1.0.0.tar` & `protokolo-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,33 @@
--rw-r--r--   0        0        0     2147 2024-04-09 10:54:02.994443 protokolo-1.0.0/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-1.0.0/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-1.0.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-1.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-1.0.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     6944 2024-04-09 10:45:20.520978 protokolo-1.0.0/README.md
--rw-r--r--   0        0        0     2770 2024-04-09 10:53:06.853855 protokolo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      177 2024-04-09 10:53:06.853855 protokolo-1.0.0/src/protokolo/__init__.py
--rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-1.0.0/src/protokolo/__main__.py
--rw-r--r--   0        0        0     3825 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     1435 2024-03-08 18:20:59.913097 protokolo-1.0.0/src/protokolo/_util.py
--rw-r--r--   0        0        0     7982 2024-04-09 07:14:59.883614 protokolo-1.0.0/src/protokolo/cli.py
--rw-r--r--   0        0        0    10126 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/compile.py
--rw-r--r--   0        0        0    11712 2024-04-08 09:03:05.349473 protokolo-1.0.0/src/protokolo/config.py
--rw-r--r--   0        0        0     3245 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/exceptions.py
--rw-r--r--   0        0        0     3773 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/initialise.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-1.0.0/src/protokolo/py.typed
--rw-r--r--   0        0        0     1520 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/replace.py
--rw-r--r--   0        0        0      931 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/types.py
--rw-r--r--   0        0        0     2231 2024-04-09 10:25:50.336818 protokolo-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0    18278 2024-04-09 10:25:50.336818 protokolo-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0    15949 2024-04-09 07:02:10.527188 protokolo-1.0.0/tests/test_compile.py
--rw-r--r--   0        0        0    11411 2024-03-29 19:44:07.383769 protokolo-1.0.0/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-1.0.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     6053 2024-04-09 10:25:50.336818 protokolo-1.0.0/tests/test_formatter.py
--rw-r--r--   0        0        0     4040 2024-04-09 07:02:10.527188 protokolo-1.0.0/tests/test_replace.py
--rw-r--r--   0        0        0     8018 1970-01-01 00:00:00.000000 protokolo-1.0.0/setup.py
--rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 protokolo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2214 2024-04-09 16:27:00.966441 protokolo-1.0.1/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-1.0.1/LICENSES/
+-rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-1.0.1/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-1.0.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-1.0.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     6944 2024-04-09 10:45:20.520978 protokolo-1.0.1/README.md
+-rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0     1531 2024-04-09 10:42:00.282891 protokolo-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      729 2024-04-09 10:33:37.509694 protokolo-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     7713 2024-04-09 10:25:50.336818 protokolo-1.0.1/docs/reference.md
+-rw-r--r--   0        0        0     2811 2024-04-09 16:26:49.794230 protokolo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-09 16:26:49.794230 protokolo-1.0.1/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-1.0.1/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     3825 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1435 2024-03-08 18:20:59.913097 protokolo-1.0.1/src/protokolo/_util.py
+-rw-r--r--   0        0        0     7982 2024-04-09 07:14:59.883614 protokolo-1.0.1/src/protokolo/cli.py
+-rw-r--r--   0        0        0    10126 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/compile.py
+-rw-r--r--   0        0        0    11712 2024-04-08 09:03:05.349473 protokolo-1.0.1/src/protokolo/config.py
+-rw-r--r--   0        0        0     3245 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     3773 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-1.0.1/src/protokolo/py.typed
+-rw-r--r--   0        0        0     1520 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/replace.py
+-rw-r--r--   0        0        0      931 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/types.py
+-rw-r--r--   0        0        0     2231 2024-04-09 10:25:50.336818 protokolo-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0    18278 2024-04-09 10:25:50.336818 protokolo-1.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0    15949 2024-04-09 07:02:10.527188 protokolo-1.0.1/tests/test_compile.py
+-rw-r--r--   0        0        0    11411 2024-03-29 19:44:07.383769 protokolo-1.0.1/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-1.0.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6053 2024-04-09 10:25:50.336818 protokolo-1.0.1/tests/test_formatter.py
+-rw-r--r--   0        0        0     4040 2024-04-09 07:02:10.527188 protokolo-1.0.1/tests/test_replace.py
+-rw-r--r--   0        0        0     8018 1970-01-01 00:00:00.000000 protokolo-1.0.1/setup.py
+-rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 protokolo-1.0.1/PKG-INFO
```

### Comparing `protokolo-1.0.0/CHANGELOG.md` & `protokolo-1.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 The versions follow [semantic versioning](https://semver.org) for the
 `protokolo` CLI command and its behaviour. There are no guarantees of stability
 for the `protokolo` Python library.
 
 <!-- protokolo-section-tag -->
 
+## 1.0.1 - 2024-04-09
+
+### Fixed
+
+- Include `docs/` in the sdist.
+
 ## 1.0.0 - 2024-04-09
 
 ### Changed
 
 - Renamed the concept of 'entry' to 'fragment'.
 - Changed the way newlines are handled for fragments. Newlines surrounding
   fragments are now significant when concatenation of fragments happens.
```

### Comparing `protokolo-1.0.0/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-1.0.1/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/LICENSES/CC0-1.0.txt` & `protokolo-1.0.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/LICENSES/GPL-3.0-or-later.txt` & `protokolo-1.0.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/README.md` & `protokolo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/pyproject.toml` & `protokolo-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "1.0.0"
+version = "1.0.1"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
@@ -25,14 +25,15 @@
     "Topic :: Utilities"
 ]
 
 packages = [
     { include = "protokolo", from = "src" }
 ]
 include = [
+    { path = "docs", format = "sdist" },
     { path = "tests", format = "sdist" },
     { path = "README.md", format = "sdist" },
     { path = "CHANGELOG.md", format = "sdist" },
     { path = "LICENSES", format = "sdist" },
 ]
 
 [tool.poetry.scripts]
@@ -76,15 +77,15 @@
 python-lsp-black = "*"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [bumpver]
-current_version = "v1.0.0"
+current_version = "v1.0.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `protokolo-1.0.0/src/protokolo/_formatter.py` & `protokolo-1.0.1/src/protokolo/_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/_util.py` & `protokolo-1.0.1/src/protokolo/_util.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/cli.py` & `protokolo-1.0.1/src/protokolo/cli.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/compile.py` & `protokolo-1.0.1/src/protokolo/compile.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/config.py` & `protokolo-1.0.1/src/protokolo/config.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/exceptions.py` & `protokolo-1.0.1/src/protokolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/initialise.py` & `protokolo-1.0.1/src/protokolo/initialise.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/replace.py` & `protokolo-1.0.1/src/protokolo/replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/src/protokolo/types.py` & `protokolo-1.0.1/src/protokolo/types.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/conftest.py` & `protokolo-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/test_cli.py` & `protokolo-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/test_compile.py` & `protokolo-1.0.1/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/test_config.py` & `protokolo-1.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/test_exceptions.py` & `protokolo-1.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/test_formatter.py` & `protokolo-1.0.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/tests/test_replace.py` & `protokolo-1.0.1/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.0/setup.py` & `protokolo-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['attrs>=22.1.0', 'click>=8.0']
 
 entry_points = \
 {'console_scripts': ['protokolo = protokolo.cli:main']}
 
 setup_kwargs = {
     'name': 'protokolo',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Protokolo is a change log generator.',
     'long_description': "<!--\nSPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\nSPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later\n-->\n\n# Protokolo\n\n[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)\n\nProtokolo is a change log generator.\n\nProtokolo allows you to maintain your change log fragments in separate files,\nand then finally aggregate them into a new section in CHANGELOG just before\nrelease.\n\n## Table of contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Maintainers](#maintainers)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Background\n\nChange logs are [a really good idea](https://keepachangelog.com/).\nUnfortunately, they are also a bit of a pain when combined with version control:\n\n- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll\n  need to resolve a conflict when trying to merge them both.\n- Just after you make a release, you need to create a new section in CHANGELOG\n  for your next release. If you forget this busywork, new feature branches will\n  need to create this section, which increases the chance of merge conflicts.\n- If a feature branch adds a change log entry to the section for the next v2.0\n  release, and v2.0 subsequently releases without merging that feature branch,\n  then merging that feature branch afterwards would still add the change log\n  entry to the v2.0 section, even though it should now go to the unreleased v3.0\n  section.\n\nLife would be a lot easier if you didn't have to deal with these problems.\n\nEnter Protokolo\n([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The\nidea is very simple: for every change log entry, create a new file. Finally,\njust before release, compile the contents of those files into a new section in\nCHANGELOG, and delete the files.\n\n### See also\n\n[Towncrier](https://github.com/twisted/towncrier) is an older and more widely\nused implementation of the same idea. Protokolo is distinct in that it uses a\ndirectory hierarchy instead of putting all metadata in the file name of each\nchange log fragment. Furthermore, Protokolo does no fancy formatting of\nfragments---what you write is what you get.\n\nThere are three main problems I encountered in Towncrier that Protokolo attempts\nto address:\n\n- When using Towncrier, I would always forget which fragment types are available\n  to me and had to look them up. These fragment types can also differ per\n  repository. In Protokolo, the types are always visible because they are\n  directories.\n- Towncrier fragments are sorted by their ID, which is typically an issue or PR\n  number. This isn't always what I want.\n- Because (some) Towncrier workflows put the PR number in the file name as\n  metadata, I would have to open the PR before I could create the change log\n  fragment.\n\nA much younger version of me also tried her hand at writing a program like this\nin [changelogdir](https://pypi.org/project/changelogdir/).\n\n## Install\n\nProtokolo is a regular Python package. You can install it using\n`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`\nwith `pipx ensurepath`.\n\n## Usage\n\nFor full documentation and options, read the documentation at\n<https://protokolo.readthedocs.io>.\n\n### Initial set-up\n\nTo set up your project for use with Protokolo, run `protokolo init`. This will\ncreate a `CHANGELOG.md` file (if one did not already exist) and a directory\nstructure under `changelog.d`. The directory structure uses the\n[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking\nlike this:\n\n```\n.\n├── changelog.d\n│   ├── added\n│   │   └── .protokolo.toml\n│   ├── changed\n│   │   └── .protokolo.toml\n│   ├── deprecated\n│   │   └── .protokolo.toml\n│   ├── fixed\n│   │   └── .protokolo.toml\n│   ├── removed\n│   │   └── .protokolo.toml\n│   ├── security\n│   │   └── .protokolo.toml\n│   └── .protokolo.toml\n├── CHANGELOG.md\n└── .protokolo.toml\n```\n\nThe `.protokolo.toml` files in `changelog.d` contain metadata for their\nrespective sections: the section title, heading level, and order. Their\ninclusion is mandatory.\n\nThe `.protokolo.toml` file in the root of the project contains configurations\nfor Protokolo that reduce the amount of typing you need to do when running\ncommands.\n\nIf a `CHANGELOG.md` file already existed, make sure to add a line containing\n`<!-- protokolo-section-tag -->` just before the heading of the latest release.\n\n### Adding fragments\n\nTo add a change log fragment, create the file `changelog.d/added/my_feature.md`,\nand write something like:\n\n```markdown\n- Added `--my-new-feature` option.\n```\n\nNote the item dash at the start---Protokolo does not add them for you. What you\nwrite is exactly what you get.\n\nYou can add more files. Change log fragments in the same section (read:\ndirectory) are sorted alphabetically by their file name. If you want to make\ncertain that some change log fragments go first or last, prefix the file with\n`000_` or `zzz_`. For example, you can create\n`changelog.d/added/000_important_feature.md` to make it appear first.\n\n### Compiling your change log\n\nYou compile your change log with `protokolo compile`. This will take all change\nlog fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run\nit now, the following section is added after the\n`<!-- protokolo-section-tag -->` comment:\n\n```markdown\n## ${version} - 2023-11-08\n\n### Added\n\n- Added important feature.\n- Added `--my-new-feature` option.\n```\n\nThe Markdown files in `changelog.d/added/` are deleted. You can manually replace\n`${version}` with a release version, or you can pass the option\n`--format version 1.0.0` to `protokolo compile` to format the heading at compile\ntime.\n\n## Maintainers\n\n- Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\n## Contributing\n\nThe code and issue tracker is hosted at\n<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any\nissues. For pull requests, bug fixes are always welcome, but new features should\nprobably be discussed in any issue first.\n\n## License\n\nAll code is licensed under GPL-3.0-or-later.\n\nAll documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.\n\nSome configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.\n\nThe repository is [REUSE](https://reuse.software)-compliant. Check the\nindividual files for their exact licensing.\n",
     'author': 'Carmen Bianca BAKKER',
     'author_email': 'carmen@carmenbianca.eu',
     'maintainer': 'Carmen Bianca BAKKER',
     'maintainer_email': 'carmen@carmenbianca.eu',
     'url': 'https://codeberg.org/carmenbianca/protokolo',
```

### Comparing `protokolo-1.0.0/PKG-INFO` & `protokolo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protokolo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Protokolo is a change log generator.
 Home-page: https://codeberg.org/carmenbianca/protokolo
 License: GPL-3.0-or-later
 Keywords: changelog,history,news
 Author: Carmen Bianca BAKKER
 Author-email: carmen@carmenbianca.eu
 Maintainer: Carmen Bianca BAKKER
```

