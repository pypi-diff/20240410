# Comparing `tmp/protokolo-1.0.1.tar.gz` & `tmp/protokolo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-1.0.1.tar", max compression
+gzip compressed data, was "protokolo-2.0.0.tar", max compression
```

## Comparing `protokolo-1.0.1.tar` & `protokolo-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
--rw-r--r--   0        0        0     2214 2024-04-09 16:27:00.966441 protokolo-1.0.1/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-1.0.1/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-1.0.1/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-1.0.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-1.0.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     6944 2024-04-09 10:45:20.520978 protokolo-1.0.1/README.md
--rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-1.0.1/docs/Makefile
--rw-r--r--   0        0        0     1531 2024-04-09 10:42:00.282891 protokolo-1.0.1/docs/conf.py
--rw-r--r--   0        0        0      729 2024-04-09 10:33:37.509694 protokolo-1.0.1/docs/index.rst
--rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-1.0.1/docs/make.bat
--rw-r--r--   0        0        0     7713 2024-04-09 10:25:50.336818 protokolo-1.0.1/docs/reference.md
--rw-r--r--   0        0        0     2811 2024-04-09 16:26:49.794230 protokolo-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      177 2024-04-09 16:26:49.794230 protokolo-1.0.1/src/protokolo/__init__.py
--rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-1.0.1/src/protokolo/__main__.py
--rw-r--r--   0        0        0     3825 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     1435 2024-03-08 18:20:59.913097 protokolo-1.0.1/src/protokolo/_util.py
--rw-r--r--   0        0        0     7982 2024-04-09 07:14:59.883614 protokolo-1.0.1/src/protokolo/cli.py
--rw-r--r--   0        0        0    10126 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/compile.py
--rw-r--r--   0        0        0    11712 2024-04-08 09:03:05.349473 protokolo-1.0.1/src/protokolo/config.py
--rw-r--r--   0        0        0     3245 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/exceptions.py
--rw-r--r--   0        0        0     3773 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/initialise.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-1.0.1/src/protokolo/py.typed
--rw-r--r--   0        0        0     1520 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/replace.py
--rw-r--r--   0        0        0      931 2024-04-09 10:25:50.336818 protokolo-1.0.1/src/protokolo/types.py
--rw-r--r--   0        0        0     2231 2024-04-09 10:25:50.336818 protokolo-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0    18278 2024-04-09 10:25:50.336818 protokolo-1.0.1/tests/test_cli.py
--rw-r--r--   0        0        0    15949 2024-04-09 07:02:10.527188 protokolo-1.0.1/tests/test_compile.py
--rw-r--r--   0        0        0    11411 2024-03-29 19:44:07.383769 protokolo-1.0.1/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-1.0.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     6053 2024-04-09 10:25:50.336818 protokolo-1.0.1/tests/test_formatter.py
--rw-r--r--   0        0        0     4040 2024-04-09 07:02:10.527188 protokolo-1.0.1/tests/test_replace.py
--rw-r--r--   0        0        0     8018 1970-01-01 00:00:00.000000 protokolo-1.0.1/setup.py
--rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 protokolo-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3051 2024-04-10 10:13:03.510121 protokolo-2.0.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-2.0.0/LICENSES/
+-rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-2.0.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-2.0.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-2.0.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     6947 2024-04-10 09:40:37.511016 protokolo-2.0.0/README.md
+-rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-2.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2052 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0      744 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/index.rst
+-rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-2.0.0/docs/make.bat
+-rw-r--r--   0        0        0      271 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/man/index.rst
+-rw-r--r--   0        0        0     1638 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/man/protokolo-compile.rst
+-rw-r--r--   0        0        0     2078 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/man/protokolo-init.rst
+-rw-r--r--   0        0        0      854 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/man/protokolo.rst
+-rw-r--r--   0        0        0     7976 2024-04-10 09:40:37.511016 protokolo-2.0.0/docs/reference.md
+-rw-r--r--   0        0        0     2811 2024-04-10 10:11:55.520697 protokolo-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-10 10:11:55.520697 protokolo-2.0.0/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-2.0.0/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     3825 2024-04-09 10:25:50.336818 protokolo-2.0.0/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1424 2024-04-10 09:50:35.343820 protokolo-2.0.0/src/protokolo/_util.py
+-rw-r--r--   0        0        0     8367 2024-04-10 10:07:37.305507 protokolo-2.0.0/src/protokolo/cli.py
+-rw-r--r--   0        0        0    10167 2024-04-10 10:07:37.305507 protokolo-2.0.0/src/protokolo/compile.py
+-rw-r--r--   0        0        0    11712 2024-04-08 09:03:05.349473 protokolo-2.0.0/src/protokolo/config.py
+-rw-r--r--   0        0        0     3245 2024-04-09 10:25:50.336818 protokolo-2.0.0/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     3785 2024-04-10 09:40:37.511016 protokolo-2.0.0/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-2.0.0/src/protokolo/py.typed
+-rw-r--r--   0        0        0     1520 2024-04-09 10:25:50.336818 protokolo-2.0.0/src/protokolo/replace.py
+-rw-r--r--   0        0        0      931 2024-04-09 10:25:50.336818 protokolo-2.0.0/src/protokolo/types.py
+-rw-r--r--   0        0        0     2225 2024-04-10 09:40:37.511016 protokolo-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0    20279 2024-04-10 10:07:37.305507 protokolo-2.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0    15759 2024-04-10 10:07:37.305507 protokolo-2.0.0/tests/test_compile.py
+-rw-r--r--   0        0        0    11440 2024-04-10 09:40:37.515016 protokolo-2.0.0/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-2.0.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6053 2024-04-10 09:24:45.458848 protokolo-2.0.0/tests/test_formatter.py
+-rw-r--r--   0        0        0     3907 2024-04-10 09:40:37.515016 protokolo-2.0.0/tests/test_replace.py
+-rw-r--r--   0        0        0     8021 1970-01-01 00:00:00.000000 protokolo-2.0.0/setup.py
+-rw-r--r--   0        0        0     7917 1970-01-01 00:00:00.000000 protokolo-2.0.0/PKG-INFO
```

### Comparing `protokolo-1.0.1/CHANGELOG.md` & `protokolo-2.0.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,39 @@
 
 The versions follow [semantic versioning](https://semver.org) for the
 `protokolo` CLI command and its behaviour. There are no guarantees of stability
 for the `protokolo` Python library.
 
 <!-- protokolo-section-tag -->
 
+## 2.0.0 - 2024-04-10
+
+### Added
+
+- Wrote man pages, improved documentation.
+- The options `--changelog`, `--directory`, and `--markup` now also take the
+  short options `-c`, `-d`, and `-m` respectively.
+- The option `--format` now also has the short option `-f`.
+
+### Changed
+
+- `protokolo compile` now takes the change log directory as a `--directory`
+  option instead of as an argument. This makes it consistent with
+  `protokolo init`.
+
+### Fixed
+
+- Fixed a bug where, if a subdirectory in `changelog.d` did not contain a
+  `.protokolo.toml` file, the program would crash.
+- Made sure that `changelog.d` subdirectories that do not contain a
+  `.protokolo.toml` file retain all their files after `protokolo compile` is
+  run.
+- In `protokolo compile --help`, there was a `TODO` where a link to the
+  documentation should have been.
+
 ## 1.0.1 - 2024-04-09
 
 ### Fixed
 
 - Include `docs/` in the sdist.
 
 ## 1.0.0 - 2024-04-09
```

### Comparing `protokolo-1.0.1/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-2.0.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/LICENSES/CC0-1.0.txt` & `protokolo-2.0.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/LICENSES/GPL-3.0-or-later.txt` & `protokolo-2.0.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/README.md` & `protokolo-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Table of contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
-- [License](#license)
+- [Licensing](#licensing)
 
 ## Background
 
 Change logs are [a really good idea](https://keepachangelog.com/).
 Unfortunately, they are also a bit of a pain when combined with version control:
 
 - If two pull requests edit CHANGELOG, there is a non-zero chance that you'll
@@ -129,15 +129,15 @@
 To add a change log fragment, create the file `changelog.d/added/my_feature.md`,
 and write something like:
 
 ```markdown
 - Added `--my-new-feature` option.
 ```
 
-Note the item dash at the start---Protokolo does not add them for you. What you
+Note the bullet at the start---Protokolo does not add them for you. What you
 write is exactly what you get.
 
 You can add more files. Change log fragments in the same section (read:
 directory) are sorted alphabetically by their file name. If you want to make
 certain that some change log fragments go first or last, prefix the file with
 `000_` or `zzz_`. For example, you can create
 `changelog.d/added/000_important_feature.md` to make it appear first.
@@ -170,15 +170,15 @@
 ## Contributing
 
 The code and issue tracker is hosted at
 <https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any
 issues. For pull requests, bug fixes are always welcome, but new features should
 probably be discussed in any issue first.
 
-## License
+## Licensing
 
 All code is licensed under GPL-3.0-or-later.
 
 All documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.
 
 Some configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.
```

### Comparing `protokolo-1.0.1/docs/Makefile` & `protokolo-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/docs/conf.py` & `protokolo-2.0.0/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,7 +39,31 @@
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "furo"
 html_static_path = ["_static"]
+
+man_pages = [
+    (
+        "man/protokolo",
+        "protokolo",
+        "A change log generator",
+        "Carmen Bianca BAKKER",
+        1,
+    ),
+    (
+        "man/protokolo-compile",
+        "protokolo-compile",
+        "Compile the contents of the change log directory into a change log file.",
+        "Carmen Bianca BAKKER",
+        1,
+    ),
+    (
+        "man/protokolo-init",
+        "protokolo-init",
+        "Set up your project for use with protokolo",
+        "Carmen Bianca BAKKER",
+        1,
+    ),
+]
```

### Comparing `protokolo-1.0.1/docs/index.rst` & `protokolo-2.0.0/docs/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 -----------------
 
 .. toctree::
    :maxdepth: 2
 
    Overview<readme>
    reference
+   man/index
 
 API reference
 -------------
 .. toctree::
-   :maxdepth: 4
+   :maxdepth: 3
 
-   API<api/modules>
+   API<api/protokolo>
 
 Change log
 ----------
 .. toctree::
    :maxdepth: 2
 
    history
```

### Comparing `protokolo-1.0.1/docs/make.bat` & `protokolo-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/docs/reference.md` & `protokolo-2.0.0/docs/reference.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 SPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later
 -->
 
 # Reference
 
 This document aims to provide a full reference of the usage and behaviour of
-Protokolo. For basic usage, please read the
-[Usage section of the overview](project:./readme.md#usage).
+Protokolo. For a full reference of the command-line options, see
+<project:./man/index.rst>. For basic usage, please read the
+[Usage](project:./readme.md#usage) section of the
+[overview](project:./readme.md).
 
 (global-configuration)=
 
 ## Global configuration
 
 You can configure various global options in a TOML file. Protokolo loads the
 first match of the following files in your current working directory:
 
 - `.protokolo.toml`
 - `pyproject.toml`
 
 The configuration values go in the `[protokolo]` table, or the
-`[tool.protokolo]` table for `pyproject.toml`. An example section looks like
-this:
+`[tool.protokolo]` table for `pyproject.toml`. An example configuration looks
+like this:
 
 ```toml
 [protokolo]
 changelog = "CHANGELOG.md"
 directory = "changelog.d"
 markup = "markdown"
 ```
@@ -57,15 +59,16 @@
 The change log directory, typically named `changelog.d`, is a hierarchy of files
 (fragments) and directories (sections) that can be compiled into a change log
 file. The top section---the change log directory itself---typically maps to the
 section of a version release in your change log file.
 
 The change log directory and all its subdirectories must contain a
 `.protokolo.toml` [section configuration](#section-configuration) file. If a
-directory does not contain such a file, it is not a section.
+directory does not contain such a file, it is not a section, and is consequently
+ignored.
 
 The [fragments](#fragments) must have a file extension corresponding to their
 markup language. If a file does not have such a file extension, it is not a
 fragment, and is consequently ignored by Protokolo.
 
 As an example, the change log directory typically looks like this:
 
@@ -99,15 +102,15 @@
 
 (section-configuration)=
 
 ### Section configuration
 
 The `.protokolo.toml` file in each directory configures options of the
 corresponding section. The file format is TOML. The configuration values go in
-the `[protokolo.section]` table. An example section looks like this:
+the `[protokolo.section]` table. An example configuration looks like this:
 
 ```toml
 [protokolo.section]
 title = "${version} - ${date}"
 level = 2
 order = 1
 miscellaneous = "your-value-here"
@@ -122,15 +125,15 @@
 A string that contains the text of the section heading, for example "Added" or
 "${version} - ${date}".
 
 Words that are prefixed by `$` (e.g. `$version`) or surrounded with `${}` (e.g.
 `${version}`) can be replaced during compile time with `--format key value`
 (e.g. `--format version 1.0.0`). Alternatively, they can be replaced by the
 values of other keys in the `.protokolo.toml` file. See the
-[Miscellaneous keys](#miscellaneous-keys) section.
+<project:#miscellaneous-keys> section.
 
 `${date}` is a special case. If its value is not defined anywhere, the value of
 `${date}` is today's date in the format `YYYY-MM-DD`.
 
 `${title}` is not valid and will not be replaced by anything.
 
 The formatting rules of the title are identical to the Python
@@ -139,15 +142,15 @@
 
 If no title is defined, it is automatically replaced by the string "TODO: No
 section title defined".
 
 #### level
 
 The level of the heading as an integer. This defaults to 1, or the value of the
-parent section plus 1. This effectively means you really only need to define it
+parent level plus 1. This effectively means you really only need to define it
 once in the top section; the levels of the subsections are increased as the
 subdirectories are nested. You typically set this value to '2' in
 `changelog.d/.protokolo.toml`.
 
 ```{note}
 There are no standard symbols assigned to levels in reStructuredText. They are
 supposed to be determined from the succession of headings. Because Protokolo is
@@ -193,28 +196,28 @@
 file name with something like `000_` or `zzz_` respectively.
 
 Because of how the compilation works, you typically want to follow a few rules:
 
 - Do not start the fragment with a newline.
 - Do not include headings.
 - If the fragment represents a list item:
-  - Start with a bullet point, typically `- ` or `* `.
+  - Start with a bullet, typically `- ` or `* `.
   - End the fragment with zero or one newline.
 - If the fragment represents a paragraph:
   - Adjust its file name to make it appear exactly where you want it to appear.
   - End the fragment with two newlines.
 
 ## Compilation
 
 The main command of Protokolo is `protokolo compile`. It gathers all your change
 log fragment files and aggregates them into a new section in your change log
 file, after which the change log fragment files are deleted.
 
-The fragments are sorted alphabetically as described in [Fragments](#fragments),
-and the section sorting is described in [order](#order).
+The fragments are sorted alphabetically as described in <project:#fragments>,
+and the section sorting is described in <project:#order>.
 
 The section is inserted into the change log after the line containing the first
 instance of `protokolo-section-tag`. You typically want to comment that out. The
 insertion always inserts two newlines at the start, effectively placing your
 section two lines below `protokolo-section-tag`. An example change log file is
 as follows:
 
@@ -227,27 +230,30 @@
 
 ## 0.1.0 - 2023-10-25
 
 The latest release.
 ```
 
 The compilation of the change log directory makes sure that after each section,
-there are two newlines before the next section or fragment. Before each
-subsection there are also two newlines after the preceding section or fragment.
-These newlines can overlap. They are indicated below using `<--` arrows.
-
-```text
-# Top section<--
-<--
-## Subsection 1<--
-<--
-- A fragment.<--
-<--
-## Subsection 2<--
-<--
-- Another fragment
+there are at least two newlines before the next section heading or fragment.
+Before each subsection there are also at least two newlines after the preceding
+section heading or fragment. These newlines can overlap, and are indicated below
+using `←`. Newlines that belong to fragments are indicated using `↵`.
+
+<!-- prettier-ignore -->
+```markdown
+# Top section←
+←
+## Subsection 1←
+←
+- A fragment.↵
+- Another fragment.↵
+←
+## Subsection 2←
+←
+- Last fragment.↵
 ```
 
 Empty sections are not compiled.
 
 Fragments are inserted as-is without any modification, except a newline is
 appended at the end of a fragment if one was not present in the file.
```

### Comparing `protokolo-1.0.1/pyproject.toml` & `protokolo-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "1.0.1"
+version = "2.0.0"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
@@ -77,15 +77,15 @@
 python-lsp-black = "*"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [bumpver]
-current_version = "v1.0.1"
+current_version = "v2.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `protokolo-1.0.1/src/protokolo/_formatter.py` & `protokolo-2.0.0/src/protokolo/_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/src/protokolo/_util.py` & `protokolo-2.0.0/src/protokolo/_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Some miscellaneous utilities."""
 
 from collections.abc import Callable, Mapping
-from inspect import cleandoc as _cleandoc
+from inspect import cleandoc
 from types import UnionType
 from typing import Any
 
 
 def type_in_expected_type(value: type, expected_type: type | UnionType) -> bool:
     """Check whether the type *value* matches any of *expected_type*.
 
@@ -41,10 +41,10 @@
         for item in path:
             values = values[item]
         return values
 
     return browse
 
 
-def cleandoc(text: str) -> str:
+def cleandoc_nl(text: str) -> str:
     """Like :func:`inspect.cleandoc`, but with a newline at the end."""
-    return _cleandoc(text) + "\n"
+    return cleandoc(text) + "\n"
```

### Comparing `protokolo-1.0.1/src/protokolo/cli.py` & `protokolo-2.0.0/src/protokolo/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Main entry of program."""
 
-import os
 import tomllib
 from io import TextIOWrapper
 from pathlib import Path
 
 import click
 
 from ._formatter import MARKUP_EXTENSION_MAPPING as _MARKUP_EXTENSION_MAPPING
 from .compile import Section
 from .config import GlobalConfig
 from .exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
     HeadingFormatError,
+    ProtokoloTOMLIsADirectoryError,
+    ProtokoloTOMLNotFoundError,
 )
 from .initialise import (
     create_changelog,
     create_keep_a_changelog,
     create_root_toml,
 )
 from .replace import find_first_occurrence, insert_into_str
@@ -60,61 +61,65 @@
                 "directory": config.directory,
             }
 
 
 @main.command(name="compile")
 @click.option(
     "--changelog",
+    "-c",
     show_default="determined by config",
     type=click.File("r+", encoding="utf-8", lazy=True),
     required=True,
     help="File into which to compile.",
 )
 @click.option(
+    "--directory",
+    "-d",
+    show_default="determined by config",
+    type=click.Path(
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+        readable=True,
+        path_type=Path,
+    ),
+    required=True,
+)
+@click.option(
     "--markup",
+    "-m",
     default="markdown",
     show_default="determined by config, or markdown",
     type=click.Choice(SupportedMarkup.__args__),  # type: ignore
     help="Markup language.",
 )
 @click.option(
     "--format",
     "-f",
     "format_",
     type=(str, str),
     metavar="<KEY VALUE>...",
     multiple=True,
-    help="Use key-value pairs to string-format section headers.",
+    help="Use key-value pairs to string-format section headings.",
 )
 @click.option(
     "--dry-run",
     "-n",
     is_flag=True,
     help="Do not write to file system; print to STDOUT.",
 )
-@click.argument(
-    "directory",
-    type=click.Path(
-        exists=True,
-        file_okay=False,
-        dir_okay=True,
-        readable=True,
-        path_type=Path,
-    ),
-    required=True,
-)
 def compile_(
     changelog: click.File,
     markup: SupportedMarkup,
     format_: tuple[tuple[str, str], ...],
     dry_run: bool,
     directory: Path,
 ) -> None:
     """Aggregate all change log fragments from files in a directory into a
-    CHANGELOG file.
+    CHANGELOG file, then delete the fragment files.
 
     A change log directory should contain a '.protokolo.toml' file that defines
     some attributes of the section. This is an example file:
 
     \b
     [protokolo.section]
     title = "${version} - ${date}"
@@ -129,26 +134,28 @@
 
     The CHANGELOG file should contain the following comment, which is the
     location in the file after which the compiled section will be pasted:
 
     \b
     <!-- protokolo-section-tag -->
 
-    For more documentation and options, read the documentation at TODO.
+    For more documentation and options, read the documentation at
+    <https://protokolo.readthedocs.io>.
     """
     # TODO: Maybe split this up.
-    # pylint: disable=too-many-locals
     format_pairs: dict[str, str] = dict(format_)
 
     # Create Section
     try:
         section = Section.from_directory(
             directory, markup=markup, section_format_pairs=format_pairs
         )
     except (
+        ProtokoloTOMLNotFoundError,
+        ProtokoloTOMLIsADirectoryError,
         tomllib.TOMLDecodeError,
         DictTypeError,
         AttributeNotPositiveError,
         OSError,
     ) as error:
         raise click.UsageError(str(error)) from error
 
@@ -173,55 +180,54 @@
             if lineno is None:
                 raise click.UsageError(
                     f"There is no 'protokolo-section-tag' in"
                     f" {repr(changelog.name)}."
                 )
             new_contents = insert_into_str(f"\n{new_section}", contents, lineno)
             if dry_run:
-                click.echo(new_contents)
+                click.echo(new_contents, nl=False)
             else:
                 fp.seek(0)
                 fp.write(new_contents)
                 fp.truncate()
     except OSError as error:
         # TODO: This is a little tricky to test. click already exits early if
         # changelog isn't readable/writable.
         raise click.UsageError(str(error)) from error
 
     # Delete change log fragments
     if not dry_run:
-        for dirpath, _, filenames in os.walk(directory):
-            for filename in filenames:
-                path = Path(dirpath) / filename
-                if path.suffix in _MARKUP_EXTENSION_MAPPING[markup]:
-                    path.unlink()
+        _delete_fragments(section)
 
 
 @main.command(name="init")
 @click.option(
     "--changelog",
+    "-c",
     default="CHANGELOG.md",
     show_default="determined by config, or CHANGELOG.md",
     type=click.File("w", encoding="utf-8", lazy=True),
     help="CHANGELOG file to create.",
 )
 @click.option(
     "--directory",
+    "-d",
     default="changelog.d",
     show_default="determined by config, or changelog.d",
     type=click.Path(
         file_okay=False,
         dir_okay=True,
         readable=True,
         path_type=Path,
     ),
     help="Directory of change log sections and fragments.",
 )
 @click.option(
     "--markup",
+    "-m",
     default="markdown",
     show_default="determined by config, or markdown",
     type=click.Choice(SupportedMarkup.__args__),  # type: ignore
     help="Markup language.",
 )
 def init(
     changelog: click.File,
@@ -257,7 +263,16 @@
     """
     try:
         create_changelog(changelog.name, markup)
         create_keep_a_changelog(directory)
         create_root_toml(changelog.name, markup, directory)
     except OSError as error:
         raise click.UsageError(str(error)) from error
+
+
+def _delete_fragments(section: Section) -> None:
+    """Delete :class:`.compile.Fragment`s' source files recursively."""
+    for fragment in section.fragments:
+        if fragment.source:
+            fragment.source.unlink(missing_ok=True)
+    for subsection in section.subsections:
+        _delete_fragments(subsection)
```

### Comparing `protokolo-1.0.1/src/protokolo/compile.py` & `protokolo-2.0.0/src/protokolo/compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             DictTypeError: ``.protokolo.toml`` fields have the wrong type.
             AttributeNotPositiveError: value in ``.protokolo.toml`` should be a
                 positive integer.
         """
         subsections = set()
         fragments = set()
         for path in directory.iterdir():
-            if path.is_dir():
+            if path.is_dir() and (path / ".protokolo.toml").is_file():
                 subsections.add(
                     self.from_directory(
                         path,
                         level=level + 1,
                         markup=self.markup,
                         section_format_pairs=section_format_pairs,
                     )
```

### Comparing `protokolo-1.0.1/src/protokolo/config.py` & `protokolo-2.0.0/src/protokolo/config.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/src/protokolo/exceptions.py` & `protokolo-2.0.0/src/protokolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/src/protokolo/initialise.py` & `protokolo-2.0.0/src/protokolo/initialise.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Code related to ``protokolo init``."""
 
 from pathlib import Path
 
-from ._util import cleandoc
+from ._util import cleandoc_nl
 from .types import StrPath, SupportedMarkup
 
 CHANGELOG_MD = """# Change log
 
 This change log follows the [Keep a Changelog](http://keepachangelog.com/).
 recommendations. Every release contains the following sections:
 
@@ -58,15 +58,15 @@
 
 def create_keep_a_changelog(directory: StrPath) -> None:
     """Create a skeleton structure of changelog.d at *directory*."""
     directory = Path(directory)
     directory.mkdir(parents=True, exist_ok=True)
     if not (directory / ".protokolo.toml").exists():
         (directory / ".protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo.section]
                 title = "${version} - ${date}"
                 level = 2
                 """
             ),
             encoding="utf-8",
@@ -80,15 +80,15 @@
         {"dirname": "security", "title": "Security", "order": 6},
     ]
     for subdir in subdirs:
         (directory / str(subdir["dirname"])).mkdir(exist_ok=True)
         protokolo_toml = directory / str(subdir["dirname"]) / ".protokolo.toml"
         if not protokolo_toml.exists():
             protokolo_toml.write_text(
-                cleandoc(
+                cleandoc_nl(
                     """
                     [protokolo.section]
                     title = "{title}"
                     order = {order}
                     """
                 ).format(title=subdir["title"], order=subdir["order"]),
                 encoding="utf-8",
@@ -99,15 +99,15 @@
     changelog: StrPath, markup: SupportedMarkup | None, directory: StrPath
 ) -> None:
     """Create a ``.protokolo.toml`` file in the current working directory."""
     if markup is None:
         markup = "markdown"
 
     Path(".protokolo.toml").write_text(
-        cleandoc(
+        cleandoc_nl(
             """
             [protokolo]
             changelog = "{changelog}"
             markup = "{markup}"
             directory = "{directory}"
             """
         ).format(changelog=changelog, markup=markup, directory=directory),
```

### Comparing `protokolo-1.0.1/src/protokolo/replace.py` & `protokolo-2.0.0/src/protokolo/replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/src/protokolo/types.py` & `protokolo-2.0.0/src/protokolo/types.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/tests/conftest.py` & `protokolo-2.0.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Fixtures and stuff."""
 
-from inspect import cleandoc
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 
+from protokolo._util import cleandoc_nl
+
 # pylint: disable=unused-argument
 
 
 @pytest.fixture()
 def project_dir(tmpdir_factory, monkeypatch) -> Path:
     """Create a temporary project directory."""
     directory = Path(str(tmpdir_factory.mktemp("project_dir")))
 
     (directory / "CHANGELOG.md").write_text(
-        cleandoc(
+        cleandoc_nl(
             """
             # Change log
 
             Lorem ipsum.
 
             <!-- protokolo-section-tag -->
 
             ## 0.1.0 - 2020-01-01
 
             First release.
             """
         )
-        + "\n"
     )
     (directory / "CHANGELOG.rst").write_text(
-        cleandoc(
+        cleandoc_nl(
             """
             Change log
             ==========
 
             Lorem ipsum.
 
             ..
@@ -47,32 +47,31 @@
 
             0.1.0 - 2020-01-01
             ------------------
 
             First release.
             """
         )
-        + "\n"
     )
 
     changelog_d = directory / "changelog.d"
     changelog_d.mkdir()
     (changelog_d / ".protokolo.toml").write_text(
-        cleandoc(
+        cleandoc_nl(
             """
             [protokolo.section]
             title = "${version} - ${date}"
             level = 2
             """
         )
     )
     feature_section = changelog_d / "feature"
     feature_section.mkdir()
     (feature_section / ".protokolo.toml").write_text(
-        cleandoc(
+        cleandoc_nl(
             """
             [protokolo.section]
             title = "Features"
             """
         )
     )
```

### Comparing `protokolo-1.0.1/tests/test_cli.py` & `protokolo-2.0.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Test the formatting code."""
 
 import errno
-from inspect import cleandoc
 from pathlib import Path
 
 from freezegun import freeze_time
 
 import protokolo
 from protokolo import cli
+from protokolo._util import cleandoc_nl
 from protokolo.cli import main
 from protokolo.config import GlobalConfig, SectionAttributes
 
 # pylint: disable=unspecified-encoding
 
 
 def raise_permission(filename):
@@ -63,24 +63,25 @@
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code == 0
         changelog = Path("CHANGELOG.md").read_text()
 
         assert (
-            cleandoc(
+            cleandoc_nl(
                 """
                 Lorem ipsum.
 
                 <!-- protokolo-section-tag -->
 
                 ## ${version} - 2023-11-08
 
@@ -100,27 +101,28 @@
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
                 "--format",
                 "version",
                 "0.2.0",
-                "changelog.d",
             ],
         )
         assert result.exit_code == 0
         changelog = Path("CHANGELOG.md").read_text()
 
         assert (
-            cleandoc(
+            cleandoc_nl(
                 """
                 Lorem ipsum.
 
                 <!-- protokolo-section-tag -->
 
                 ## 0.2.0 - 2023-11-08
 
@@ -138,41 +140,43 @@
         Path(".protokolo.toml").write_text("{'Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert "Error: Invalid TOML in '.protokolo.toml'" in result.output
 
     def test_global_config_wrong_type(self, runner):
         """An element has the wrong type."""
         Path(".protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo]
                 changelog = 1
                 """
             )
         )
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
             "Error: .protokolo.toml: 'changelog' does not have the correct"
             " type. Expected str | None. Got 1."
         ) in result.output
@@ -185,88 +189,92 @@
         )
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert "Permission denied" in result.output
 
     def test_section_config_parse_error(self, runner):
         """.protokolo.toml cannot be parsed."""
         Path("changelog.d/.protokolo.toml").write_text("{'Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
             "Error: Invalid TOML in 'changelog.d/.protokolo.toml'"
             in result.output
         )
 
     def test_section_config_wrong_type(self, runner):
         """An element has the wrong type."""
         Path("changelog.d/.protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo.section]
                 title = 1
                 """
             )
         )
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
             "Error: changelog.d/.protokolo.toml:"
             " 'title' does not have the correct type. Expected str. Got 1."
         ) in result.output
 
     def test_section_config_not_positive(self, runner):
         """An element has should be positive."""
         Path("changelog.d/.protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo.section]
                 level = -1
                 """
             )
         )
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
             "Error: Wrong value in 'changelog.d/.protokolo.toml': level must be"
             " a positive integer, got -1" in result.output
         )
@@ -281,42 +289,44 @@
         )
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert "Permission denied" in result.output
 
     def test_heading_format_error(self, runner):
         """Could not format a heading."""
         Path("changelog.d/.protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo.section]
                 level = 10
                 """
             )
         )
         Path("changelog.d/foo.rst").write_text("Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.rst",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "restructuredtext",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
             "Error: Failed to format section heading of 'changelog.d': Heading"
             " level 10 is too deep." in result.output
         )
@@ -326,17 +336,18 @@
         changelog = Path("CHANGELOG.md").read_text()
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code == 0
         assert (
             result.output == "There are no change log fragments to compile.\n"
         )
         assert Path("CHANGELOG.md").read_text() == changelog
@@ -347,17 +358,18 @@
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
             "Error: There is no 'protokolo-section-tag' in 'CHANGELOG.md'"
             in result.output
         )
@@ -371,24 +383,25 @@
         Path("changelog.d/feature/bar.txt").write_text("Bar")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "markdown",
-                "changelog.d",
             ],
         )
         assert result.exit_code == 0
         changelog = Path("CHANGELOG.md").read_text()
 
         assert (
-            cleandoc(
+            cleandoc_nl(
                 """
                 Lorem ipsum.
 
                 <!-- protokolo-section-tag -->
 
                 ## ${version} - 2023-11-08
 
@@ -400,35 +413,81 @@
                 """
             )
             in changelog
         )
         assert not Path("changelog.d/feature/foo.md").exists()
         assert Path("changelog.d/feature/bar.txt").exists()
 
+    def test_no_protokolo_toml_in_changelog_d(self, runner):
+        """If changelog.d does not contain a .protokolo.toml file, TODO"""
+        Path("changelog.d/.protokolo.toml").unlink()
+        Path("changelog.d/foo.md").write_text("Foo")
+        result = runner.invoke(
+            main,
+            [
+                "compile",
+                "--changelog",
+                "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
+                "--markup",
+                "markdown",
+            ],
+        )
+        assert result.exit_code != 0
+        assert (
+            "No such file or directory: 'changelog.d/.protokolo.toml'"
+            in result.stdout
+        )
+
+    def test_files_in_ignored_subdirs_not_deleted(self, runner):
+        """'Fragment' files in subdirectories that do not contain a
+        .protokolo.toml file are not deleted.
+        """
+        Path("changelog.d/feature/.protokolo.toml").unlink()
+        Path("changelog.d/feature/hello.md").write_text("Hello, world!")
+        Path("changelog.d/foo.md").write_text("Foo")
+        result = runner.invoke(
+            main,
+            [
+                "compile",
+                "--changelog",
+                "CHANGELOG.md",
+                "--directory",
+                "changelog.d",
+                "--markup",
+                "markdown",
+            ],
+        )
+        assert result.exit_code == 0
+        assert "Hello, world!" not in Path("CHANGELOG.md").read_text()
+        assert Path("changelog.d/feature/hello.md").is_file()
+
     @freeze_time("2023-11-08")
     def test_restructuredtext(self, runner):
         """A simple test, but for restructuredtext."""
         Path("changelog.d/foo.rst").write_text("Foo")
         Path("changelog.d/feature/bar.rst").write_text("Bar")
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.rst",
+                "--directory",
+                "changelog.d",
                 "--markup",
                 "restructuredtext",
-                "changelog.d",
             ],
         )
         assert result.exit_code == 0
         changelog = Path("CHANGELOG.rst").read_text()
 
         assert (
-            cleandoc(
+            cleandoc_nl(
                 """
                 Lorem ipsum.
 
                 ..
                     protokolo-section-tag
 
                 ${version} - 2023-11-08
@@ -458,24 +517,25 @@
 
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
-                "--dry-run",
+                "--directory",
                 "changelog.d",
+                "--dry-run",
             ],
         )
         assert result.exit_code == 0
         assert Path("CHANGELOG.md").read_text() == changelog_text
         assert Path("changelog.d/foo.md").exists()
         assert Path("changelog.d/foo.md").read_text() == "Foo"
 
-        assert result.stdout.strip() == cleandoc(
+        assert result.stdout == cleandoc_nl(
             """
             # Change log
 
             Lorem ipsum.
 
             <!-- protokolo-section-tag -->
 
@@ -484,15 +544,14 @@
             Foo
 
             ## 0.1.0 - 2020-01-01
 
             First release.
             """
         )
-        assert result.stdout.endswith("\n")
 
 
 class TestInit:
     """Collect all tests for init."""
 
     def test_help_is_not_default(self, runner):
         """--help is not the default action."""
```

### Comparing `protokolo-1.0.1/tests/test_compile.py` & `protokolo-2.0.0/tests/test_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Test the compilation of change log sections and fragments."""
 
 import random
 import tomllib
-from inspect import cleandoc
 
 import pytest
 
+from protokolo._util import cleandoc_nl
 from protokolo.compile import Fragment, Section
 from protokolo.config import SectionAttributes
 from protokolo.exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
     ProtokoloTOMLIsADirectoryError,
     ProtokoloTOMLNotFoundError,
@@ -33,27 +33,24 @@
             attrs=SectionAttributes(title="Subsection", level=2)
         )
         subsection.fragments.add(Fragment("- world"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.fragments.add(Fragment("- hello"))
         section.subsections.add(subsection)
 
-        expected = (
-            cleandoc(
-                """
-                # Section
+        expected = cleandoc_nl(
+            """
+            # Section
 
-                - hello
+            - hello
 
-                ## Subsection
+            ## Subsection
 
-                - world
-                """
-            )
-            + "\n"
+            - world
+            """
         )
         assert section.compile() == expected
 
     def test_compile_multiple_fragments(self):
         """Test the compilation of a single section with multiple fragments.
 
         In this test, there are three types of newline configurations for
@@ -66,29 +63,26 @@
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.fragments.add(Fragment("- A", source="a"))
         section.fragments.add(Fragment("- B\n", source="b"))
         section.fragments.add(Fragment("- C\n\n", source="c"))
         section.fragments.add(Fragment("- D", source="d"))
         section.fragments.add(Fragment("\n- E", source="e"))
 
-        expected = (
-            cleandoc(
-                """
-                # Section
-
-                - A
-                - B
-                - C
+        expected = cleandoc_nl(
+            """
+            # Section
+
+            - A
+            - B
+            - C
 
-                - D
+            - D
 
-                - E
-                """
-            )
-            + "\n"
+            - E
+            """
         )
         assert section.compile() == expected
 
     def test_compile_empty(self):
         """A section that contains neither fragments nor subsections doesn't
         compile to anything.
         """
@@ -115,25 +109,22 @@
         subsection_2 = Section(
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=2)
         )
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = (
-            cleandoc(
-                """
-                # Section
+        expected = cleandoc_nl(
+            """
+            # Section
 
-                ## Subsection Foo
+            ## Subsection Foo
 
-                Foo
-                """
-            )
-            + "\n"
+            Foo
+            """
         )
         assert section.compile() == expected
 
     def test_compile_order_specified(self):
         """Respect the order specified on the subsection."""
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2, order=1)
@@ -143,29 +134,26 @@
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=2)
         )
         subsection_2.fragments.add(Fragment("Bar"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = (
-            cleandoc(
-                """
-                # Section
+        expected = cleandoc_nl(
+            """
+            # Section
 
-                ## Subsection Foo
+            ## Subsection Foo
 
-                Foo
+            Foo
 
-                ## Subsection Bar
+            ## Subsection Bar
 
-                Bar
-                """
-            )
-            + "\n"
+            Bar
+            """
         )
         assert section.compile() == expected
 
     def test_compile_order_alphabetic(self):
         """If no orders are specified, sort subsections alphabetically."""
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2)
@@ -175,29 +163,26 @@
             attrs=SectionAttributes(title="Subsection Bar", level=2)
         )
         subsection_2.fragments.add(Fragment("Bar"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = (
-            cleandoc(
-                """
-                # Section
+        expected = cleandoc_nl(
+            """
+            # Section
 
-                ## Subsection Bar
+            ## Subsection Bar
 
-                Bar
+            Bar
 
-                ## Subsection Foo
+            ## Subsection Foo
 
-                Foo
-                """
-            )
-            + "\n"
+            Foo
+            """
         )
         assert section.compile() == expected
 
     def test_compile_order_mixed(self):
         """Ordered subsections are sorted first, and all subsections with
         unspecified order are sorted afterwards, alphabetically.
         """
@@ -217,37 +202,34 @@
             attrs=SectionAttributes(title="Subsection Quz", level=2)
         )
         subsection_4.fragments.add(Fragment("Quz"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.update(
             {subsection_1, subsection_2, subsection_3, subsection_4}
         )
-        expected = (
-            cleandoc(
-                """
-                # Section
+        expected = cleandoc_nl(
+            """
+            # Section
 
-                ## Subsection Foo
+            ## Subsection Foo
 
-                Foo
+            Foo
 
-                ## Subsection Bar
+            ## Subsection Bar
 
-                Bar
+            Bar
 
-                ## Subsection Baz
+            ## Subsection Baz
 
-                Baz
+            Baz
 
-                ## Subsection Quz
+            ## Subsection Quz
 
-                Quz
-                """
-            )
-            + "\n"
+            Quz
+            """
         )
         assert section.compile() == expected
 
     def test_compile_order_same_order(self):
         """If two sections have the same order number, sort alphabetically."""
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2, order=1)
@@ -257,29 +239,26 @@
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=1)
         )
         subsection_2.fragments.add(Fragment("Bar"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = (
-            cleandoc(
-                """
-                # Section
+        expected = cleandoc_nl(
+            """
+            # Section
 
-                ## Subsection Bar
+            ## Subsection Bar
 
-                Bar
+            Bar
 
-                ## Subsection Foo
+            ## Subsection Foo
 
-                Foo
-                """
-            )
-            + "\n"
+            Foo
+            """
         )
         assert section.compile() == expected
 
     def test_compile_fragments_sorted_by_source(self):
         """Compiled fragments are sorted by their source."""
         section = Section(attrs=SectionAttributes(title="Section"))
         fragments = {
@@ -312,24 +291,21 @@
         """Compiled fragments that have a source are sorted before ones that
         don't.
         """
         section = Section(attrs=SectionAttributes(title="Section"))
         section.fragments.add(Fragment("- Foo", source="foo.md"))
         section.fragments.add(Fragment("- Bar"))
 
-        expected = (
-            cleandoc(
-                """
-                # Section
-
-                - Foo
-                - Bar
-                """
-            )
-            + "\n"
+        expected = cleandoc_nl(
+            """
+            # Section
+
+            - Foo
+            - Bar
+            """
         )
         assert section.compile() == expected
 
     def test_is_empty_simple(self):
         """A section with neither fragments nor subsections is empty."""
         section = Section()
         assert section.is_empty()
@@ -415,15 +391,15 @@
         )
 
     def test_from_directory_dict_type_error(self, project_dir):
         """If there is a type inconsistency is found in the toml file, raise a
         DictTypeError.
         """
         (project_dir / "changelog.d/.protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo.section]
                 level = "foo"
                 """
             )
         )
         with pytest.raises(DictTypeError) as exc_info:
@@ -432,15 +408,15 @@
         assert error.source == str(project_dir / "changelog.d/.protokolo.toml")
 
     def test_from_directory_attribute_not_positive_error(self, project_dir):
         """If a value in .protokolo.toml must be positive but isn't, raise
         AttributeNotPositiveError.
         """
         (project_dir / "changelog.d/.protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo.section]
                 level = 0
                 """
             )
         )
         with pytest.raises(AttributeNotPositiveError) as exc_info:
@@ -458,14 +434,22 @@
         with pytest.raises(ProtokoloTOMLNotFoundError) as exc_info:
             Section.from_directory(project_dir / "changelog.d")
         error = exc_info.value
         assert error.filename == str(
             project_dir / "changelog.d/.protokolo.toml"
         )
 
+    def test_from_directory_no_protokolo_toml_in_subdir(self, project_dir):
+        """If there is no .protokolo.toml in the subdirectory, don't count it as
+        a section.
+        """
+        (project_dir / "changelog.d/feature/.protokolo.toml").unlink()
+        section = Section.from_directory(project_dir / "changelog.d")
+        assert not section.subsections
+
     def test_from_directory_is_a_directory_error(self, project_dir):
         """If .protokolo.toml is not a file, raise
         ProtokoloTOMLIsADirectoryError.
         """
         (project_dir / "changelog.d/.protokolo.toml").unlink()
         (project_dir / "changelog.d/.protokolo.toml").mkdir()
         with pytest.raises(ProtokoloTOMLIsADirectoryError) as exc_info:
```

### Comparing `protokolo-1.0.1/tests/test_config.py` & `protokolo-2.0.0/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Test the config code."""
 
 import tomllib
 from datetime import date, datetime
-from inspect import cleandoc
 from io import BytesIO
 
 import pytest
 
+from protokolo._util import cleandoc_nl
 from protokolo.config import (
     GlobalConfig,
     SectionAttributes,
     TOMLConfig,
     parse_toml,
 )
 from protokolo.exceptions import (
@@ -26,15 +26,15 @@
 
 
 class TestParseToml:
     """Collect all tests for parse_toml."""
 
     def test_parse_toml_simple(self):
         """Provide all values in a toml string."""
-        toml = cleandoc(
+        toml = cleandoc_nl(
             """
             [protokolo.section]
             title = "Title"
             level = 2
             order = 3
             foo = "bar"
             """
@@ -45,35 +45,35 @@
         assert values["order"] == 3
         assert values["foo"] == "bar"
         parent = parse_toml(toml, section=["protokolo"])
         assert parent["section"] == values
 
     def test_parse_toml_no_values(self):
         """If there are no values, return an empty dictionary."""
-        toml = cleandoc(
+        toml = cleandoc_nl(
             """
             [protokolo.section]
             """
         )
         values = parse_toml(toml, section=["protokolo", "section"])
         assert not values
 
     def test_parse_toml_no_table(self):
         """If there is no [protokolo.section] table, return an empty dict."""
-        toml = cleandoc(
+        toml = cleandoc_nl(
             """
             title = "Title"
             """
         )
         assert parse_toml(toml, section=["protokolo"]) == {}
         assert parse_toml(toml, section=None) == {"title": "Title"}
 
     def test_parse_toml_decode_error(self):
         """Raise TOMLDecodeError when TOML can't be parsed."""
-        yaml = cleandoc(
+        yaml = cleandoc_nl(
             """
             hello:
               - world
             """
         )
         with pytest.raises(tomllib.TOMLDecodeError):
             parse_toml(yaml)
@@ -293,15 +293,15 @@
         """Return None if config file is a directory."""
         (project_dir / ".protokolo.toml").mkdir()
         assert GlobalConfig.find_config(project_dir) is None
 
     def test_from_file_protokolo_toml(self, project_dir):
         """Load from .protokolo.toml."""
         (project_dir / ".protokolo.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [protokolo]
                 changelog = "CHANGELOG"
                 markup = "markdown"
                 directory = "changelog.d"
                 """
             )
@@ -310,15 +310,15 @@
         assert config.changelog == "CHANGELOG"
         assert config.markup == "markdown"
         assert config.directory == "changelog.d"
 
     def test_from_file_pyproject_toml(self, project_dir):
         """Load from pyproject.toml."""
         (project_dir / "pyproject.toml").write_text(
-            cleandoc(
+            cleandoc_nl(
                 """
                 [tool.protokolo]
                 changelog = "CHANGELOG"
                 markup = "markdown"
                 directory = "changelog.d"
                 """
             )
```

### Comparing `protokolo-1.0.1/tests/test_exceptions.py` & `protokolo-2.0.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/tests/test_formatter.py` & `protokolo-2.0.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-1.0.1/tests/test_replace.py` & `protokolo-2.0.0/tests/test_replace.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Test the find-and-insert code."""
 
-from inspect import cleandoc
-
+from protokolo._util import cleandoc_nl
 from protokolo.replace import find_first_occurrence, insert_into_str
 
 
 class TestInsertIntoStr:
     """Collect all tests for insert_into_str."""
 
     def test_insert_into_str_simple(self):
         """Simple case."""
-        target = cleandoc(
+        target = cleandoc_nl(
             """
             Line 1
             Line 2
             Line 3
             """
         )
-        expected = cleandoc(
+        expected = cleandoc_nl(
             """
             Line 1
             Line 2
             Foo
             Line 3
             """
         )
         # The newline is implicit.
         assert insert_into_str("Foo\n", target, 2) == expected
         assert insert_into_str("Foo", target, 2) == expected
 
     def test_insert_into_str_multiple_lines(self):
         """Insert multiple lines into a string."""
-        target = cleandoc(
+        target = cleandoc_nl(
             """
             Line 1
             Line 2
             """
         )
-        expected = cleandoc(
+        expected = cleandoc_nl(
             """
             Line 1
             Foo
             Bar
             Line 2
             """
         )
         assert (
             insert_into_str(
-                cleandoc(
+                cleandoc_nl(
                     """
                     Foo
                     Bar
                     """
                 ),
                 target,
                 1,
@@ -67,102 +66,93 @@
         """Insert into an empty target."""
         target = ""
         expected = "Foo\n"
         assert insert_into_str("Foo", target, 0) == expected
 
     def test_insert_into_str_text_empty(self):
         """Insert empty string into target."""
-        target = cleandoc(
+        target = cleandoc_nl(
             """
             Line 1
             Line 2
             """
         )
         expected = target
         assert insert_into_str("", target, 1) == expected
 
     def test_insert_into_str_end(self):
         """Insert at the end of the target."""
-        target = cleandoc(
+        target = cleandoc_nl(
             """
             Line 1
             Line 2
             """
         )
-        expected = (
-            cleandoc(
-                """
-                Line 1
-                Line 2
-                Foo
-                """
-            )
-            + "\n"
+        expected = cleandoc_nl(
+            """
+            Line 1
+            Line 2
+            Foo
+            """
         )
         assert insert_into_str("Foo", target, 2) == expected
         assert insert_into_str("Foo\n", target, 2) == expected
 
     def test_insert_into_str_start(self):
         """Insert at the start of the target."""
-        target = cleandoc(
+        target = cleandoc_nl(
             """
             Line 1
             Line 2
             """
         )
-        expected = cleandoc(
+        expected = cleandoc_nl(
             """
             Foo
             Line 1
             Line 2
             """
         )
         assert insert_into_str("Foo", target, 0) == expected
 
     def test_insert_into_str_keep_newline_at_end(self):
         """The newline at the end is preserved."""
-        target = (
-            cleandoc(
-                """
+        target = cleandoc_nl(
+            """
                 Line 1
                 Line 2
                 """
-            )
-            + "\n"
         )
-        expected = (
-            cleandoc(
-                """
-                Foo
-                Line 1
-                Line 2
-                """
-            )
-            + "\n"
+        expected = cleandoc_nl(
+            """
+            Foo
+            Line 1
+            Line 2
+            """
         )
         assert insert_into_str("Foo", target, 0) == expected
 
 
 class TestFindFirstOccurrence:
     """Collect all tests for find_first_occurrence."""
 
     def test_find_first_occurrence_simple(self):
         """Simple case."""
-        source = cleandoc(
+        source = cleandoc_nl(
             """
             Line 1
             Line 2 hello world
             Line 3
             """
         )
         assert find_first_occurrence("hello world", source) == 2
 
     def test_find_first_occurrence_none(self):
         """There is no occurrence of the text."""
-        source = cleandoc(
+        source = cleandoc_nl(
             """
             Line 1
             Line 2
             Line 3
             """
         )
         assert find_first_occurrence("hello world", source) is None
```

### Comparing `protokolo-1.0.1/setup.py` & `protokolo-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['attrs>=22.1.0', 'click>=8.0']
 
 entry_points = \
 {'console_scripts': ['protokolo = protokolo.cli:main']}
 
 setup_kwargs = {
     'name': 'protokolo',
-    'version': '1.0.1',
+    'version': '2.0.0',
     'description': 'Protokolo is a change log generator.',
-    'long_description': "<!--\nSPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\nSPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later\n-->\n\n# Protokolo\n\n[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)\n\nProtokolo is a change log generator.\n\nProtokolo allows you to maintain your change log fragments in separate files,\nand then finally aggregate them into a new section in CHANGELOG just before\nrelease.\n\n## Table of contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Maintainers](#maintainers)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Background\n\nChange logs are [a really good idea](https://keepachangelog.com/).\nUnfortunately, they are also a bit of a pain when combined with version control:\n\n- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll\n  need to resolve a conflict when trying to merge them both.\n- Just after you make a release, you need to create a new section in CHANGELOG\n  for your next release. If you forget this busywork, new feature branches will\n  need to create this section, which increases the chance of merge conflicts.\n- If a feature branch adds a change log entry to the section for the next v2.0\n  release, and v2.0 subsequently releases without merging that feature branch,\n  then merging that feature branch afterwards would still add the change log\n  entry to the v2.0 section, even though it should now go to the unreleased v3.0\n  section.\n\nLife would be a lot easier if you didn't have to deal with these problems.\n\nEnter Protokolo\n([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The\nidea is very simple: for every change log entry, create a new file. Finally,\njust before release, compile the contents of those files into a new section in\nCHANGELOG, and delete the files.\n\n### See also\n\n[Towncrier](https://github.com/twisted/towncrier) is an older and more widely\nused implementation of the same idea. Protokolo is distinct in that it uses a\ndirectory hierarchy instead of putting all metadata in the file name of each\nchange log fragment. Furthermore, Protokolo does no fancy formatting of\nfragments---what you write is what you get.\n\nThere are three main problems I encountered in Towncrier that Protokolo attempts\nto address:\n\n- When using Towncrier, I would always forget which fragment types are available\n  to me and had to look them up. These fragment types can also differ per\n  repository. In Protokolo, the types are always visible because they are\n  directories.\n- Towncrier fragments are sorted by their ID, which is typically an issue or PR\n  number. This isn't always what I want.\n- Because (some) Towncrier workflows put the PR number in the file name as\n  metadata, I would have to open the PR before I could create the change log\n  fragment.\n\nA much younger version of me also tried her hand at writing a program like this\nin [changelogdir](https://pypi.org/project/changelogdir/).\n\n## Install\n\nProtokolo is a regular Python package. You can install it using\n`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`\nwith `pipx ensurepath`.\n\n## Usage\n\nFor full documentation and options, read the documentation at\n<https://protokolo.readthedocs.io>.\n\n### Initial set-up\n\nTo set up your project for use with Protokolo, run `protokolo init`. This will\ncreate a `CHANGELOG.md` file (if one did not already exist) and a directory\nstructure under `changelog.d`. The directory structure uses the\n[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking\nlike this:\n\n```\n.\n├── changelog.d\n│   ├── added\n│   │   └── .protokolo.toml\n│   ├── changed\n│   │   └── .protokolo.toml\n│   ├── deprecated\n│   │   └── .protokolo.toml\n│   ├── fixed\n│   │   └── .protokolo.toml\n│   ├── removed\n│   │   └── .protokolo.toml\n│   ├── security\n│   │   └── .protokolo.toml\n│   └── .protokolo.toml\n├── CHANGELOG.md\n└── .protokolo.toml\n```\n\nThe `.protokolo.toml` files in `changelog.d` contain metadata for their\nrespective sections: the section title, heading level, and order. Their\ninclusion is mandatory.\n\nThe `.protokolo.toml` file in the root of the project contains configurations\nfor Protokolo that reduce the amount of typing you need to do when running\ncommands.\n\nIf a `CHANGELOG.md` file already existed, make sure to add a line containing\n`<!-- protokolo-section-tag -->` just before the heading of the latest release.\n\n### Adding fragments\n\nTo add a change log fragment, create the file `changelog.d/added/my_feature.md`,\nand write something like:\n\n```markdown\n- Added `--my-new-feature` option.\n```\n\nNote the item dash at the start---Protokolo does not add them for you. What you\nwrite is exactly what you get.\n\nYou can add more files. Change log fragments in the same section (read:\ndirectory) are sorted alphabetically by their file name. If you want to make\ncertain that some change log fragments go first or last, prefix the file with\n`000_` or `zzz_`. For example, you can create\n`changelog.d/added/000_important_feature.md` to make it appear first.\n\n### Compiling your change log\n\nYou compile your change log with `protokolo compile`. This will take all change\nlog fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run\nit now, the following section is added after the\n`<!-- protokolo-section-tag -->` comment:\n\n```markdown\n## ${version} - 2023-11-08\n\n### Added\n\n- Added important feature.\n- Added `--my-new-feature` option.\n```\n\nThe Markdown files in `changelog.d/added/` are deleted. You can manually replace\n`${version}` with a release version, or you can pass the option\n`--format version 1.0.0` to `protokolo compile` to format the heading at compile\ntime.\n\n## Maintainers\n\n- Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\n## Contributing\n\nThe code and issue tracker is hosted at\n<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any\nissues. For pull requests, bug fixes are always welcome, but new features should\nprobably be discussed in any issue first.\n\n## License\n\nAll code is licensed under GPL-3.0-or-later.\n\nAll documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.\n\nSome configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.\n\nThe repository is [REUSE](https://reuse.software)-compliant. Check the\nindividual files for their exact licensing.\n",
+    'long_description': "<!--\nSPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\nSPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later\n-->\n\n# Protokolo\n\n[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)\n\nProtokolo is a change log generator.\n\nProtokolo allows you to maintain your change log fragments in separate files,\nand then finally aggregate them into a new section in CHANGELOG just before\nrelease.\n\n## Table of contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Maintainers](#maintainers)\n- [Contributing](#contributing)\n- [Licensing](#licensing)\n\n## Background\n\nChange logs are [a really good idea](https://keepachangelog.com/).\nUnfortunately, they are also a bit of a pain when combined with version control:\n\n- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll\n  need to resolve a conflict when trying to merge them both.\n- Just after you make a release, you need to create a new section in CHANGELOG\n  for your next release. If you forget this busywork, new feature branches will\n  need to create this section, which increases the chance of merge conflicts.\n- If a feature branch adds a change log entry to the section for the next v2.0\n  release, and v2.0 subsequently releases without merging that feature branch,\n  then merging that feature branch afterwards would still add the change log\n  entry to the v2.0 section, even though it should now go to the unreleased v3.0\n  section.\n\nLife would be a lot easier if you didn't have to deal with these problems.\n\nEnter Protokolo\n([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The\nidea is very simple: for every change log entry, create a new file. Finally,\njust before release, compile the contents of those files into a new section in\nCHANGELOG, and delete the files.\n\n### See also\n\n[Towncrier](https://github.com/twisted/towncrier) is an older and more widely\nused implementation of the same idea. Protokolo is distinct in that it uses a\ndirectory hierarchy instead of putting all metadata in the file name of each\nchange log fragment. Furthermore, Protokolo does no fancy formatting of\nfragments---what you write is what you get.\n\nThere are three main problems I encountered in Towncrier that Protokolo attempts\nto address:\n\n- When using Towncrier, I would always forget which fragment types are available\n  to me and had to look them up. These fragment types can also differ per\n  repository. In Protokolo, the types are always visible because they are\n  directories.\n- Towncrier fragments are sorted by their ID, which is typically an issue or PR\n  number. This isn't always what I want.\n- Because (some) Towncrier workflows put the PR number in the file name as\n  metadata, I would have to open the PR before I could create the change log\n  fragment.\n\nA much younger version of me also tried her hand at writing a program like this\nin [changelogdir](https://pypi.org/project/changelogdir/).\n\n## Install\n\nProtokolo is a regular Python package. You can install it using\n`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`\nwith `pipx ensurepath`.\n\n## Usage\n\nFor full documentation and options, read the documentation at\n<https://protokolo.readthedocs.io>.\n\n### Initial set-up\n\nTo set up your project for use with Protokolo, run `protokolo init`. This will\ncreate a `CHANGELOG.md` file (if one did not already exist) and a directory\nstructure under `changelog.d`. The directory structure uses the\n[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking\nlike this:\n\n```\n.\n├── changelog.d\n│   ├── added\n│   │   └── .protokolo.toml\n│   ├── changed\n│   │   └── .protokolo.toml\n│   ├── deprecated\n│   │   └── .protokolo.toml\n│   ├── fixed\n│   │   └── .protokolo.toml\n│   ├── removed\n│   │   └── .protokolo.toml\n│   ├── security\n│   │   └── .protokolo.toml\n│   └── .protokolo.toml\n├── CHANGELOG.md\n└── .protokolo.toml\n```\n\nThe `.protokolo.toml` files in `changelog.d` contain metadata for their\nrespective sections: the section title, heading level, and order. Their\ninclusion is mandatory.\n\nThe `.protokolo.toml` file in the root of the project contains configurations\nfor Protokolo that reduce the amount of typing you need to do when running\ncommands.\n\nIf a `CHANGELOG.md` file already existed, make sure to add a line containing\n`<!-- protokolo-section-tag -->` just before the heading of the latest release.\n\n### Adding fragments\n\nTo add a change log fragment, create the file `changelog.d/added/my_feature.md`,\nand write something like:\n\n```markdown\n- Added `--my-new-feature` option.\n```\n\nNote the bullet at the start---Protokolo does not add them for you. What you\nwrite is exactly what you get.\n\nYou can add more files. Change log fragments in the same section (read:\ndirectory) are sorted alphabetically by their file name. If you want to make\ncertain that some change log fragments go first or last, prefix the file with\n`000_` or `zzz_`. For example, you can create\n`changelog.d/added/000_important_feature.md` to make it appear first.\n\n### Compiling your change log\n\nYou compile your change log with `protokolo compile`. This will take all change\nlog fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run\nit now, the following section is added after the\n`<!-- protokolo-section-tag -->` comment:\n\n```markdown\n## ${version} - 2023-11-08\n\n### Added\n\n- Added important feature.\n- Added `--my-new-feature` option.\n```\n\nThe Markdown files in `changelog.d/added/` are deleted. You can manually replace\n`${version}` with a release version, or you can pass the option\n`--format version 1.0.0` to `protokolo compile` to format the heading at compile\ntime.\n\n## Maintainers\n\n- Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\n## Contributing\n\nThe code and issue tracker is hosted at\n<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any\nissues. For pull requests, bug fixes are always welcome, but new features should\nprobably be discussed in any issue first.\n\n## Licensing\n\nAll code is licensed under GPL-3.0-or-later.\n\nAll documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.\n\nSome configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.\n\nThe repository is [REUSE](https://reuse.software)-compliant. Check the\nindividual files for their exact licensing.\n",
     'author': 'Carmen Bianca BAKKER',
     'author_email': 'carmen@carmenbianca.eu',
     'maintainer': 'Carmen Bianca BAKKER',
     'maintainer_email': 'carmen@carmenbianca.eu',
     'url': 'https://codeberg.org/carmenbianca/protokolo',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `protokolo-1.0.1/PKG-INFO` & `protokolo-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protokolo
-Version: 1.0.1
+Version: 2.0.0
 Summary: Protokolo is a change log generator.
 Home-page: https://codeberg.org/carmenbianca/protokolo
 License: GPL-3.0-or-later
 Keywords: changelog,history,news
 Author: Carmen Bianca BAKKER
 Author-email: carmen@carmenbianca.eu
 Maintainer: Carmen Bianca BAKKER
@@ -45,15 +45,15 @@
 ## Table of contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
-- [License](#license)
+- [Licensing](#licensing)
 
 ## Background
 
 Change logs are [a really good idea](https://keepachangelog.com/).
 Unfortunately, they are also a bit of a pain when combined with version control:
 
 - If two pull requests edit CHANGELOG, there is a non-zero chance that you'll
@@ -154,15 +154,15 @@
 To add a change log fragment, create the file `changelog.d/added/my_feature.md`,
 and write something like:
 
 ```markdown
 - Added `--my-new-feature` option.
 ```
 
-Note the item dash at the start---Protokolo does not add them for you. What you
+Note the bullet at the start---Protokolo does not add them for you. What you
 write is exactly what you get.
 
 You can add more files. Change log fragments in the same section (read:
 directory) are sorted alphabetically by their file name. If you want to make
 certain that some change log fragments go first or last, prefix the file with
 `000_` or `zzz_`. For example, you can create
 `changelog.d/added/000_important_feature.md` to make it appear first.
@@ -195,15 +195,15 @@
 ## Contributing
 
 The code and issue tracker is hosted at
 <https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any
 issues. For pull requests, bug fixes are always welcome, but new features should
 probably be discussed in any issue first.
 
-## License
+## Licensing
 
 All code is licensed under GPL-3.0-or-later.
 
 All documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.
 
 Some configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.
```

