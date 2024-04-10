# Comparing `tmp/changeguard-0.2.0.tar.gz` & `tmp/changeguard-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/changeguard/dist/.tmp-7uy9qfi5/changeguard-0.2.0.tar", last modified: Tue Mar 26 18:10:12 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/changeguard/dist/.tmp-dvsi0yo7/changeguard-0.3.0.tar", last modified: Wed Apr 10 12:03:02 2024, max compression
```

## Comparing `changeguard-0.2.0.tar` & `changeguard-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-26 18:10:12.383863 changeguard-0.2.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-25 22:57:28.000000 changeguard-0.2.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    10066 2024-03-26 18:10:12.373907 changeguard-0.2.0/PKG-INFO
--r-xr-xr-x   0 realz     (1000) realz     (1000)     5057 2024-03-26 18:02:26.000000 changeguard-0.2.0/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-26 18:10:12.235278 changeguard-0.2.0/changeguard/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      395 2024-03-25 09:52:33.000000 changeguard-0.2.0/changeguard/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    12864 2024-03-25 20:06:30.000000 changeguard-0.2.0/changeguard/changeguard.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6714 2024-03-26 00:43:19.000000 changeguard-0.2.0/changeguard/cli.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-26 18:10:12.350683 changeguard-0.2.0/changeguard.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    10066 2024-03-26 18:10:12.000000 changeguard-0.2.0/changeguard.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      317 2024-03-26 18:10:12.000000 changeguard-0.2.0/changeguard.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-03-26 18:10:12.000000 changeguard-0.2.0/changeguard.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       53 2024-03-26 18:10:12.000000 changeguard-0.2.0/changeguard.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1106 2024-03-26 18:10:12.000000 changeguard-0.2.0/changeguard.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       12 2024-03-26 18:10:12.000000 changeguard-0.2.0/changeguard.egg-info/top_level.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     3106 2024-03-26 18:00:03.000000 changeguard-0.2.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-03-26 18:10:12.385370 changeguard-0.2.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-10 12:03:02.844928 changeguard-0.3.0/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-25 22:57:28.000000 changeguard-0.3.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    11494 2024-04-10 12:03:02.836392 changeguard-0.3.0/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     5383 2024-04-10 12:02:17.000000 changeguard-0.3.0/README.md
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-10 12:03:02.709936 changeguard-0.3.0/changeguard/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      395 2024-03-25 09:52:33.000000 changeguard-0.3.0/changeguard/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    13811 2024-04-10 12:02:17.000000 changeguard-0.3.0/changeguard/changeguard.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1598 2024-04-10 12:02:17.000000 changeguard-0.3.0/changeguard/changeguard_test.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     6776 2024-04-10 12:02:17.000000 changeguard-0.3.0/changeguard/cli.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-10 12:03:02.818835 changeguard-0.3.0/changeguard.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    11494 2024-04-10 12:03:02.000000 changeguard-0.3.0/changeguard.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      349 2024-04-10 12:03:02.000000 changeguard-0.3.0/changeguard.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-10 12:03:02.000000 changeguard-0.3.0/changeguard.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       53 2024-04-10 12:03:02.000000 changeguard-0.3.0/changeguard.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1526 2024-04-10 12:03:02.000000 changeguard-0.3.0/changeguard.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       12 2024-04-10 12:03:02.000000 changeguard-0.3.0/changeguard.egg-info/top_level.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     3636 2024-04-10 12:02:17.000000 changeguard-0.3.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-10 12:03:02.845950 changeguard-0.3.0/setup.cfg
```

### Comparing `changeguard-0.2.0/LICENSE.md` & `changeguard-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `changeguard-0.2.0/PKG-INFO` & `changeguard-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changeguard
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to check if any of the original files in a repository/directory change over the course of a precommit script.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -55,56 +55,78 @@
 Requires-Dist: rich==13.7.1; extra == "prod"
 Requires-Dist: rich-argparse==1.4.0; extra == "prod"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "prod"
 Requires-Dist: typing-extensions==4.10.0; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.2.3; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
+Requires-Dist: certifi==2024.2.2; extra == "dev"
+Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
+Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
+Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: defusedxml==0.7.1; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
+Requires-Dist: docutils==0.20.1; extra == "dev"
 Requires-Dist: filelock==3.13.3; extra == "dev"
 Requires-Dist: identify==2.5.35; extra == "dev"
+Requires-Dist: idna==3.6; extra == "dev"
 Requires-Dist: importlib-metadata==7.1.0; extra == "dev"
+Requires-Dist: importlib-resources==6.4.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: jaraco-classes==3.3.1; extra == "dev"
+Requires-Dist: jaraco-context==4.3.0; extra == "dev"
+Requires-Dist: jaraco-functools==4.0.0; extra == "dev"
+Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
+Requires-Dist: keyring==25.0.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
+Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
+Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
 Requires-Dist: pexpect==4.9.0; extra == "dev"
 Requires-Dist: pip-licenses==4.3.4; extra == "dev"
+Requires-Dist: pkginfo==1.10.0; extra == "dev"
 Requires-Dist: platformdirs==4.2.0; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: prettytable==3.10.0; extra == "dev"
 Requires-Dist: ptyprocess==0.7.0; extra == "dev"
+Requires-Dist: pycparser==2.21; extra == "dev"
 Requires-Dist: pyflakes==3.2.0; extra == "dev"
 Requires-Dist: pygments==2.17.2; extra == "dev"
 Requires-Dist: pyright==1.1.352; extra == "dev"
 Requires-Dist: pyyaml==6.0.1; extra == "dev"
+Requires-Dist: readme-renderer==43.0; extra == "dev"
+Requires-Dist: requests==2.31.0; extra == "dev"
+Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
+Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
+Requires-Dist: secretstorage==3.3.3; extra == "dev"
 Requires-Dist: snipinator==1.0.9; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
+Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.25.1; extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
 Requires-Dist: yq==3.2.3; extra == "dev"
 Requires-Dist: zipp==3.18.1; extra == "dev"
-Requires-Dist: twine; extra == "dev"
 
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `README.md.jinja2`.
 
 -->
@@ -130,14 +152,16 @@
 
 Like hashdeep, but customized to check if any of the original files in a
 repository/directory change over the course of a precommit script.
 
 ## Features
 
 - Can use any sha256sum-like command (uses xxhash by default).
+- Use `.changeguard-ignore` to ignore files that should not be checked for
+  changes.
 
 ## Getting Started
 
 ### Install
 
 #### Tested on
 
@@ -154,15 +178,15 @@
   - Why: Some dev dependencies require Python 3.8+.
 
 ```bash
 # Install from pypi (https://pypi.org/project/changeguard/)
 pip install changeguard
 
 # Install from git (https://github.com/realazthat/changeguard)
-pip install git+https://github.com/realazthat/changeguard.git@v0.2.0
+pip install git+https://github.com/realazthat/changeguard.git@v0.3.0
 ```
 
 ### Use
 
 ## Contributions
 
 ### Development environment: Linux-like
@@ -207,34 +231,38 @@
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
    `bash scripts/deploy-to-pypi.sh`.
 7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
    `git push --tags`.
+8. `git checkout develop && git merge master` The `--no-ff` option adds a commit
+   to the master branch for the merge, so refork the develop branch from the
+   master branch.
+9. `git push origin develop` Push the develop branch to GitHub.
 
 [1]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml/badge.svg?branch=master
 [2]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml
 [3]: https://img.shields.io/github/license/realazthat/changeguard
 [4]: https://img.shields.io/pypi/v/changeguard
 [5]: https://pypi.org/project/changeguard/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/master
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/master
 [7]: https://img.shields.io/github/last-commit/realazthat/changeguard/master
 [8]: https://img.shields.io/pypi/pyversions/changeguard
 [9]:
   https://img.shields.io/github/languages/top/realazthat/changeguard.svg?&cacheSeconds=28800
 [10]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...master
+  https://github.com/realazthat/changeguard/compare/v0.3.0...master
 [11]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml/badge.svg?branch=develop
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/develop
 [13]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...develop
+  https://github.com/realazthat/changeguard/compare/v0.3.0...develop
 [14]: https://img.shields.io/github/last-commit/realazthat/changeguard/develop
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/develop
 [16]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...develop
+  https://github.com/realazthat/changeguard/compare/v0.3.0...develop
```

### Comparing `changeguard-0.2.0/README.md` & `changeguard-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 Like hashdeep, but customized to check if any of the original files in a
 repository/directory change over the course of a precommit script.
 
 ## Features
 
 - Can use any sha256sum-like command (uses xxhash by default).
+- Use `.changeguard-ignore` to ignore files that should not be checked for
+  changes.
 
 ## Getting Started
 
 ### Install
 
 #### Tested on
 
@@ -50,15 +52,15 @@
   - Why: Some dev dependencies require Python 3.8+.
 
 ```bash
 # Install from pypi (https://pypi.org/project/changeguard/)
 pip install changeguard
 
 # Install from git (https://github.com/realazthat/changeguard)
-pip install git+https://github.com/realazthat/changeguard.git@v0.2.0
+pip install git+https://github.com/realazthat/changeguard.git@v0.3.0
 ```
 
 ### Use
 
 ## Contributions
 
 ### Development environment: Linux-like
@@ -103,34 +105,38 @@
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
    `bash scripts/deploy-to-pypi.sh`.
 7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
    `git push --tags`.
+8. `git checkout develop && git merge master` The `--no-ff` option adds a commit
+   to the master branch for the merge, so refork the develop branch from the
+   master branch.
+9. `git push origin develop` Push the develop branch to GitHub.
 
 [1]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml/badge.svg?branch=master
 [2]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml
 [3]: https://img.shields.io/github/license/realazthat/changeguard
 [4]: https://img.shields.io/pypi/v/changeguard
 [5]: https://pypi.org/project/changeguard/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/master
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/master
 [7]: https://img.shields.io/github/last-commit/realazthat/changeguard/master
 [8]: https://img.shields.io/pypi/pyversions/changeguard
 [9]:
   https://img.shields.io/github/languages/top/realazthat/changeguard.svg?&cacheSeconds=28800
 [10]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...master
+  https://github.com/realazthat/changeguard/compare/v0.3.0...master
 [11]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml/badge.svg?branch=develop
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/develop
 [13]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...develop
+  https://github.com/realazthat/changeguard/compare/v0.3.0...develop
 [14]: https://img.shields.io/github/last-commit/realazthat/changeguard/develop
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/develop
 [16]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...develop
+  https://github.com/realazthat/changeguard/compare/v0.3.0...develop
```

### Comparing `changeguard-0.2.0/changeguard/changeguard.py` & `changeguard-0.3.0/changeguard/changeguard.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 from typing_extensions import Literal
 
 _VALID_METHODS = ('initial_iterdir', 'git', 'auto')
 _MethodLiteral = Literal['initial_iterdir', 'git', 'auto']
 
 
 def _Ignore(*, rel_path: Path, ignores: List[pathspec.PathSpec]) -> bool:
-  for ignore in ignores:
-    if ignore.match_file(str(rel_path)):
-      return True
-  return False
+  return any(ignore.match_file(str(rel_path)) for ignore in ignores)
 
 
 def _Execute(*,
              cmd: List[str],
              cwd: Path,
              expected_error_status: int = 0) -> str:
   try:
@@ -193,29 +190,55 @@
 
   console.print(f'{"-"*80}', style='bold red')
   console.print('Failures:', len(failures), style='bold red')
   console.print('Exiting due to failures', style='bold red')
   sys.exit(1)
 
 
-def _ConstructIgnorePathSpecs(
-    *, ignorefiles: List[TextIO], ignorelines: List[str],
-    ignore_metas: Dict[str, List[str]]) -> List[pathspec.PathSpec]:
-
-  ignores = []
-  ignorefile: TextIO
-  for ignorefile in ignorefiles:
-    ignorefile_contents = ignorefile.read()
-    ignorefile_lines: List[str] = ignorefile_contents.splitlines()
-    ignore_metas[ignorefile.name] = ignorefile_lines
-    ignores.append(
-        pathspec.PathSpec.from_lines('gitwildmatch', ignorefile_lines))
-  ignore_metas['~ignorelines'] = ignorelines
-  ignores.append(pathspec.PathSpec.from_lines('gitwildmatch', ignorelines))
-  return ignores
+def _FindIgnoreFile(cwd: Path) -> Optional[Path]:
+  """
+  Search for a '.changeguard-ignore' file in the current working directory and its ancestors.
+
+  Returns:
+      Optional[Path]: The path to the found '.changeguard-ignore' file, or None
+        if not found.
+  """
+  for directory in [cwd] + list(cwd.parents):
+    ignorefile = directory / '.changeguard-ignore'
+    if ignorefile.exists() and ignorefile.is_file():
+      return ignorefile
+  return None
+
+
+def _ConstructIgnorePathSpecs(*, ignorefiles: List[TextIO],
+                              ignorelines: List[str],
+                              ignore_metas: Dict[str, List[str]],
+                              cwd: Path) -> List[pathspec.PathSpec]:
+
+  found_ignore_file: Optional[TextIO] = None
+  try:
+    found_ignore_file_path: Optional[Path] = _FindIgnoreFile(cwd=cwd)
+    if found_ignore_file_path is not None:
+      found_ignore_file = found_ignore_file_path.open('r')
+      ignorefiles.append(found_ignore_file)
+
+    ignores = []
+    ignorefile: TextIO
+    for ignorefile in ignorefiles:
+      ignorefile_contents = ignorefile.read()
+      ignorefile_lines: List[str] = ignorefile_contents.splitlines()
+      ignore_metas[ignorefile.name] = ignorefile_lines
+      ignores.append(
+          pathspec.PathSpec.from_lines('gitwildmatch', ignorefile_lines))
+    ignore_metas['~ignorelines'] = ignorelines
+    ignores.append(pathspec.PathSpec.from_lines('gitwildmatch', ignorelines))
+    return ignores
+  finally:
+    if found_ignore_file is not None:
+      found_ignore_file.close()
 
 
 def Hash(*, hash_cmd: str, directory: Path, method: _MethodLiteral,
          audit_file: TextIO, ignores: List[pathspec.PathSpec],
          ignore_metas: Dict[str, List[str]], max_workers: int,
          tmp_backup_dir: Optional[Path], console: Console):
   failures: List[_Failure] = []
@@ -334,15 +357,16 @@
         'Error: No .git directory found. Test only makes sense inside a git repository.',
         style='bold red')
     sys.exit(1)
     return
 
   ignores = _ConstructIgnorePathSpecs(ignorefiles=ignorefiles,
                                       ignorelines=ignorelines,
-                                      ignore_metas={})
+                                      ignore_metas={},
+                                      cwd=directory)
   initial_iterdir_paths = _GetPathsViaIterDir(directory=directory,
                                               ignores=ignores)
   git_paths = _GetPathsViaGit(directory=directory, ignores=ignores)
   delta = set(initial_iterdir_paths.paths) ^ set(git_paths.paths)
   if len(delta) > 0:
     console.print('Error: initial_iterdir_paths and git_paths do not match.',
                   style='bold red')
```

### Comparing `changeguard-0.2.0/changeguard/cli.py` & `changeguard-0.3.0/changeguard/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,16 @@
 
     args = parser.parse_args()
 
     if args.cmd == 'hash':
       ignore_metas: Dict[str, List[str]] = {}
       ignores = _ConstructIgnorePathSpecs(ignorefiles=list(args.ignorefile),
                                           ignorelines=list(args.ignoreline),
-                                          ignore_metas=ignore_metas)
+                                          ignore_metas=ignore_metas,
+                                          cwd=args.directory)
       return Hash(hash_cmd=args.hash_cmd,
                   directory=args.directory,
                   method=args.method,
                   audit_file=args.audit_file,
                   ignores=ignores,
                   ignore_metas=ignore_metas,
                   max_workers=args.max_workers,
```

### Comparing `changeguard-0.2.0/changeguard.egg-info/PKG-INFO` & `changeguard-0.3.0/changeguard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changeguard
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to check if any of the original files in a repository/directory change over the course of a precommit script.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -55,56 +55,78 @@
 Requires-Dist: rich==13.7.1; extra == "prod"
 Requires-Dist: rich-argparse==1.4.0; extra == "prod"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "prod"
 Requires-Dist: typing-extensions==4.10.0; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.2.3; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
+Requires-Dist: certifi==2024.2.2; extra == "dev"
+Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
+Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
+Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: defusedxml==0.7.1; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
+Requires-Dist: docutils==0.20.1; extra == "dev"
 Requires-Dist: filelock==3.13.3; extra == "dev"
 Requires-Dist: identify==2.5.35; extra == "dev"
+Requires-Dist: idna==3.6; extra == "dev"
 Requires-Dist: importlib-metadata==7.1.0; extra == "dev"
+Requires-Dist: importlib-resources==6.4.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: jaraco-classes==3.3.1; extra == "dev"
+Requires-Dist: jaraco-context==4.3.0; extra == "dev"
+Requires-Dist: jaraco-functools==4.0.0; extra == "dev"
+Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
+Requires-Dist: keyring==25.0.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
+Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
+Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
 Requires-Dist: pexpect==4.9.0; extra == "dev"
 Requires-Dist: pip-licenses==4.3.4; extra == "dev"
+Requires-Dist: pkginfo==1.10.0; extra == "dev"
 Requires-Dist: platformdirs==4.2.0; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: prettytable==3.10.0; extra == "dev"
 Requires-Dist: ptyprocess==0.7.0; extra == "dev"
+Requires-Dist: pycparser==2.21; extra == "dev"
 Requires-Dist: pyflakes==3.2.0; extra == "dev"
 Requires-Dist: pygments==2.17.2; extra == "dev"
 Requires-Dist: pyright==1.1.352; extra == "dev"
 Requires-Dist: pyyaml==6.0.1; extra == "dev"
+Requires-Dist: readme-renderer==43.0; extra == "dev"
+Requires-Dist: requests==2.31.0; extra == "dev"
+Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
+Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
+Requires-Dist: secretstorage==3.3.3; extra == "dev"
 Requires-Dist: snipinator==1.0.9; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
+Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.25.1; extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
 Requires-Dist: yq==3.2.3; extra == "dev"
 Requires-Dist: zipp==3.18.1; extra == "dev"
-Requires-Dist: twine; extra == "dev"
 
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `README.md.jinja2`.
 
 -->
@@ -130,14 +152,16 @@
 
 Like hashdeep, but customized to check if any of the original files in a
 repository/directory change over the course of a precommit script.
 
 ## Features
 
 - Can use any sha256sum-like command (uses xxhash by default).
+- Use `.changeguard-ignore` to ignore files that should not be checked for
+  changes.
 
 ## Getting Started
 
 ### Install
 
 #### Tested on
 
@@ -154,15 +178,15 @@
   - Why: Some dev dependencies require Python 3.8+.
 
 ```bash
 # Install from pypi (https://pypi.org/project/changeguard/)
 pip install changeguard
 
 # Install from git (https://github.com/realazthat/changeguard)
-pip install git+https://github.com/realazthat/changeguard.git@v0.2.0
+pip install git+https://github.com/realazthat/changeguard.git@v0.3.0
 ```
 
 ### Use
 
 ## Contributions
 
 ### Development environment: Linux-like
@@ -207,34 +231,38 @@
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
    `bash scripts/deploy-to-pypi.sh`.
 7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
    `git push --tags`.
+8. `git checkout develop && git merge master` The `--no-ff` option adds a commit
+   to the master branch for the merge, so refork the develop branch from the
+   master branch.
+9. `git push origin develop` Push the develop branch to GitHub.
 
 [1]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml/badge.svg?branch=master
 [2]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml
 [3]: https://img.shields.io/github/license/realazthat/changeguard
 [4]: https://img.shields.io/pypi/v/changeguard
 [5]: https://pypi.org/project/changeguard/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/master
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/master
 [7]: https://img.shields.io/github/last-commit/realazthat/changeguard/master
 [8]: https://img.shields.io/pypi/pyversions/changeguard
 [9]:
   https://img.shields.io/github/languages/top/realazthat/changeguard.svg?&cacheSeconds=28800
 [10]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...master
+  https://github.com/realazthat/changeguard/compare/v0.3.0...master
 [11]:
   https://github.com/realazthat/changeguard/actions/workflows/build-and-test.yml/badge.svg?branch=develop
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/develop
 [13]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...develop
+  https://github.com/realazthat/changeguard/compare/v0.3.0...develop
 [14]: https://img.shields.io/github/last-commit/realazthat/changeguard/develop
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/changeguard/v0.3.0/develop
 [16]:
-  https://github.com/realazthat/changeguard/compare/v0.2.0...develop
+  https://github.com/realazthat/changeguard/compare/v0.3.0...develop
```

### Comparing `changeguard-0.2.0/changeguard.egg-info/requires.txt` & `changeguard-0.3.0/changeguard.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,56 +7,78 @@
 rich-argparse<2,>=1
 types-pyyaml<7,>=6
 typing-extensions<5,>=4
 
 [dev]
 argcomplete==3.2.3
 autoflake==2.3.1
+certifi==2024.2.2
+cffi==1.16.0
 cfgv==3.4.0
+charset-normalizer==3.3.2
 colorama==0.4.6
+cryptography==42.0.5
 defusedxml==0.7.1
 distlib==0.3.8
+docutils==0.20.1
 filelock==3.13.3
 identify==2.5.35
+idna==3.6
 importlib-metadata==7.1.0
+importlib-resources==6.4.0
 isort==5.13.2
+jaraco-classes==3.3.1
+jaraco-context==4.3.0
+jaraco-functools==4.0.0
+jeepney==0.8.0
 jinja2==3.1.3
+keyring==25.0.0
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
+more-itertools==10.2.0
 mypy==1.8.0
 mypy-extensions==1.0.0
+nh3==0.2.17
 nodeenv==1.8.0
 pathspec==0.12.1
 pexpect==4.9.0
 pip-licenses==4.3.4
+pkginfo==1.10.0
 platformdirs==4.2.0
 pre-commit==3.5.0
 prettytable==3.10.0
 ptyprocess==0.7.0
+pycparser==2.21
 pyflakes==3.2.0
 pygments==2.17.2
 pyright==1.1.352
 pyyaml==6.0.1
+readme-renderer==43.0
+requests==2.31.0
+requests-toolbelt==1.0.0
+rfc3986==2.0.0
 rich==13.7.1
 rich-argparse==1.4.0
+secretstorage==3.3.3
 snipinator==1.0.9
 toml-sort==0.23.1
 tomli==2.0.1
 tomlkit==0.12.4
+twine==5.0.0
 types-colorama==0.4.15.20240311
 types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
+urllib3==2.2.1
 virtualenv==20.25.1
 wcwidth==0.2.13
 xmltodict==0.13.0
 yapf==0.40.2
 yq==3.2.3
 zipp==3.18.1
-twine
 
 [prod]
 markdown-it-py==3.0.0
 mdurl==0.1.2
 pathspec==0.12.1
 pygments==2.17.2
 pyyaml==6.0.1
```

### Comparing `changeguard-0.2.0/pyproject.toml` & `changeguard-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "changeguard"
-version = "0.2.0"
+version = "0.3.0"
 description = "CLI to check if any of the original files in a repository/directory change over the course of a precommit script."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -51,67 +51,89 @@
 ]
 # Set of dev dependencies, all pinned, so that they are known to work. To add a
 # new dependency here, add the unpinned package name here, and then run
 # `EXTRA=dev bash scripts/pin-extra-reqs.sh`.
 dev = [
   "argcomplete==3.2.3",
   "autoflake==2.3.1",
+  "certifi==2024.2.2",
+  "cffi==1.16.0",
   "cfgv==3.4.0",
+  "charset-normalizer==3.3.2",
   "colorama==0.4.6",
+  "cryptography==42.0.5",
   "defusedxml==0.7.1",
   "distlib==0.3.8",
+  "docutils==0.20.1",
   "filelock==3.13.3",
   "identify==2.5.35",
+  "idna==3.6",
   "importlib-metadata==7.1.0",
+  "importlib-resources==6.4.0",
   "isort==5.13.2",
+  "jaraco-classes==3.3.1",
+  "jaraco-context==4.3.0",
+  "jaraco-functools==4.0.0",
+  "jeepney==0.8.0",
   "jinja2==3.1.3",
+  "keyring==25.0.0",
   "markdown-it-py==3.0.0",
   "markupsafe==2.1.5",
   "mdurl==0.1.2",
+  "more-itertools==10.2.0",
   "mypy==1.8.0",
   "mypy-extensions==1.0.0",
+  "nh3==0.2.17",
   "nodeenv==1.8.0",
   "pathspec==0.12.1",
   "pexpect==4.9.0",
   "pip-licenses==4.3.4",
+  "pkginfo==1.10.0",
   "platformdirs==4.2.0",
   "pre-commit==3.5.0",
   "prettytable==3.10.0",
   "ptyprocess==0.7.0",
+  "pycparser==2.21",
   "pyflakes==3.2.0",
   "pygments==2.17.2",
   "pyright==1.1.352",
   "pyyaml==6.0.1",
+  "readme-renderer==43.0",
+  "requests==2.31.0",
+  "requests-toolbelt==1.0.0",
+  "rfc3986==2.0.0",
   "rich==13.7.1",
   "rich-argparse==1.4.0",
+  "secretstorage==3.3.3",
   "snipinator==1.0.9",
   "toml-sort==0.23.1",
   "tomli==2.0.1",
   "tomlkit==0.12.4",
+  "twine==5.0.0",
   "types-colorama==0.4.15.20240311",
   "types-pyyaml==6.0.12.20240311",
   "typing-extensions==4.10.0",
+  "urllib3==2.2.1",
   "virtualenv==20.25.1",
   "wcwidth==0.2.13",
   "xmltodict==0.13.0",
   "yapf==0.40.2",
   "yq==3.2.3",
-  "zipp==3.18.1",
-  "twine"
+  "zipp==3.18.1"
 ]
 
 [project.scripts]
 changeguard = "changeguard.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/realazthat/changeguard"
 Documentation = "https://github.com/realazthat/changeguard"
 Repository = "https://github.com/realazthat/changeguard"
 
 [tool.changeguard-project-metadata]
-last_unstable_release = "0.2.0"
-last_stable_release = "0.2.0"
+last_unstable_release = "0.3.0"
+last_stable_release = "0.3.0"
 
 [tool.setuptools]
 packages = ["changeguard"]
 
 [tool.tomlsort]
```

