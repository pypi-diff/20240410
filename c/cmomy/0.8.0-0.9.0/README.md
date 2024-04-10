# Comparing `tmp/cmomy-0.8.0.tar.gz` & `tmp/cmomy-0.9.0.tar.gz`

## Comparing `cmomy-0.8.0.tar` & `cmomy-0.9.0.tar`

### file list

```diff
@@ -1,161 +1,165 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 cmomy-0.8.0/.cruft.json
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 cmomy-0.8.0/.editorconfig
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cmomy-0.8.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cmomy-0.8.0/.gitattributes
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 cmomy-0.8.0/.markdownlint.yaml
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 cmomy-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cmomy-0.8.0/.prettierignore
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cmomy-0.8.0/.prettierrc.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cmomy-0.8.0/.recipe-append.yaml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 cmomy-0.8.0/AUTHORS.md
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 cmomy-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 cmomy-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmomy-0.8.0/Makefile
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 cmomy-0.8.0/README.md
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 cmomy-0.8.0/conftest.py
--rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 cmomy-0.8.0/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cmomy-0.8.0/changelog.d/README.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmomy-0.8.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cmomy-0.8.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 cmomy-0.8.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cmomy-0.8.0/config/README.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 cmomy-0.8.0/config/nbval.ini
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cmomy-0.8.0/config/recipe-append.yaml
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 cmomy-0.8.0/config/userconfig.example.toml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/Makefile
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/authors.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/changelog.md
--rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/conf.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/contributing.md
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/index.md
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/installation.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/license.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/make.bat
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/navigation.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_static/css/nist-combined.css
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_static/js/leave_notice.js
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_static/js/nist-header-footer.js
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/module-custom.rst
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/module-single.rst
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/module-template.rst
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autodocsumm/module.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/examples/index.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/examples/usage/motivation.ipynb -> ../../../examples/usage/motivation.ipynb
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/examples/usage/usage_notebook.ipynb -> ../../../examples/usage/usage_notebook.ipynb
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/reference/api-baseclasses.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/reference/api-modules.rst
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/reference/api-public.rst
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 cmomy-0.8.0/docs/reference/index.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/README.md
--rw-r--r--   0        0        0    70930 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/archived/bootstrap.ipynb
--rw-r--r--   0        0        0   136843 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/archived/central_moments.ipynb
--rw-r--r--   0        0        0    44860 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/archived/example_usage.ipynb
--rw-r--r--   0        0        0    12238 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/archived/parallel_test.ipynb
--rw-r--r--   0        0        0    58141 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/archived/test_accumulator.ipynb
--rw-r--r--   0        0        0   162183 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/usage/motivation.ipynb
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/usage/run_notebook.sh
--rw-r--r--   0        0        0   304977 2020-02-02 00:00:00.000000 cmomy-0.8.0/examples/usage/usage_notebook.ipynb
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/build.txt
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/dev-complete.txt
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/dev.txt
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/docs.txt
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py310-test-extras.yaml
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py310-test.yaml
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py310-typing.yaml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-dev-complete.yaml
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-dev.yaml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-docs.yaml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-test-extras.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-test-notebook.yaml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-test.yaml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py311-typing.yaml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py38-test-extras.yaml
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py38-test.yaml
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py38-typing.yaml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py39-test-extras.yaml
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py39-test.yaml
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/py39-typing.yaml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/test-extras.txt
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/test-notebook.txt
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/test.txt
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/typing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/.empty
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py310-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py310-test.txt.hash.json
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py310-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py310-typing.txt.hash.json
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-dev-base.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-dev-base.txt.hash.json
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-dev-complete.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-dev-complete.txt.hash.json
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-dev.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-dev.txt.hash.json
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-docs.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-docs.txt.hash.json
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-test-notebook.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-test-notebook.txt.hash.json
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-test.txt.hash.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py311-typing.txt.hash.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py38-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py38-test.txt.hash.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py38-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py38-typing.txt.hash.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py39-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py39-test.txt.hash.json
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py39-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.8.0/requirements/lock/py39-typing.txt.hash.json
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_compat.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_formatting.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_typing_compat.py
--rw-r--r--   0        0        0    37797 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/abstract_central.py
--rw-r--r--   0        0        0    54536 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/central.py
--rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/convert.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/docstrings.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/py.typed
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/random.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/resample.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/typing.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/utils.py
--rw-r--r--   0        0        0    68759 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/xcentral.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_lib/__init__.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_lib/convert.py
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_lib/pushers.py
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_lib/resample.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 cmomy-0.8.0/src/cmomy/_lib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/_simple_cmom.py
--rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0    17563 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_central.py
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_central_2.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_convert.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_random.py
--rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_resample.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_stability.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_utils.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_verify.py
--rw-r--r--   0        0        0    16425 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_xcentral.py
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 cmomy-0.8.0/tests/test_xcentral_constructors.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/__init__.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/clean_kernelspec.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/common_utils.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/create_pythons.py
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/dataclass_parser.py
--rw-r--r--   0        0        0    40812 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/noxtools.py
--rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 cmomy-0.8.0/tools/projectconfig.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 cmomy-0.8.0/.gitignore
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 cmomy-0.8.0/LICENSE
--rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 cmomy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 cmomy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 cmomy-0.9.0/.cruft.json
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 cmomy-0.9.0/.editorconfig
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cmomy-0.9.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cmomy-0.9.0/.gitattributes
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 cmomy-0.9.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 cmomy-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cmomy-0.9.0/.prettierignore
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cmomy-0.9.0/.prettierrc.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cmomy-0.9.0/.recipe-append.yaml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 cmomy-0.9.0/AUTHORS.md
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 cmomy-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0    16572 2020-02-02 00:00:00.000000 cmomy-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 cmomy-0.9.0/Makefile
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 cmomy-0.9.0/README.md
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 cmomy-0.9.0/conftest.py
+-rw-r--r--   0        0        0    36665 2020-02-02 00:00:00.000000 cmomy-0.9.0/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cmomy-0.9.0/changelog.d/README.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmomy-0.9.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cmomy-0.9.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 cmomy-0.9.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cmomy-0.9.0/config/README.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 cmomy-0.9.0/config/nbval.ini
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cmomy-0.9.0/config/recipe-append.yaml
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 cmomy-0.9.0/config/userconfig.example.toml
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/authors.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/changelog.md
+-rw-r--r--   0        0        0    15708 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/contributing.md
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/installation.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/license.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/navigation.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_static/css/nist-combined.css
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_static/js/nist-header-footer.js
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/module-custom.rst
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/module-single.rst
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/module-template.rst
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autodocsumm/module.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/examples/index.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/examples/usage/motivation.ipynb -> ../../../examples/usage/motivation.ipynb
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/examples/usage/usage_notebook.ipynb -> ../../../examples/usage/usage_notebook.ipynb
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/reference/api-baseclasses.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/reference/api-modules.rst
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/reference/api-public.rst
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 cmomy-0.9.0/docs/reference/index.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/README.md
+-rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/archived/bootstrap.ipynb
+-rw-r--r--   0        0        0   137061 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/archived/central_moments.ipynb
+-rw-r--r--   0        0        0    44788 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/archived/example_usage.ipynb
+-rw-r--r--   0        0        0    12167 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/archived/parallel_test.ipynb
+-rw-r--r--   0        0        0    58274 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/archived/test_accumulator.ipynb
+-rw-r--r--   0        0        0   156627 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/usage/motivation.ipynb
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/usage/run_notebook.sh
+-rw-r--r--   0        0        0   292234 2020-02-02 00:00:00.000000 cmomy-0.9.0/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/build.txt
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/dev-complete.txt
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/dev.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/docs.txt
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/pipxrun-tools.txt
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py310-test-extras.yaml
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py310-test.yaml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py310-typing.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-dev-complete.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-dev.yaml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-docs.yaml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-test-extras.yaml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-test-notebook.yaml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-test.yaml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py311-typing.yaml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py38-test-extras.yaml
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py38-test.yaml
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py38-typing.yaml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py39-test-extras.yaml
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py39-test.yaml
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/py39-typing.yaml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/test-extras.txt
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/test-notebook.txt
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/test.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/typing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/.empty
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py310-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py310-test.txt.hash.json
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py310-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py310-typing.txt.hash.json
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-dev-base.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-dev-base.txt.hash.json
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-dev-complete.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-dev-complete.txt.hash.json
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-dev.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-dev.txt.hash.json
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-docs.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-docs.txt.hash.json
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-pipxrun-tools.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-pipxrun-tools.txt.hash.json
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-test-notebook.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-test-notebook.txt.hash.json
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-test.txt.hash.json
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py311-typing.txt.hash.json
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py38-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py38-test.txt.hash.json
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py38-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py38-typing.txt.hash.json
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py39-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py39-test.txt.hash.json
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py39-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cmomy-0.9.0/requirements/lock/py39-typing.txt.hash.json
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_compat.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_formatting.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_typing_compat.py
+-rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/abstract_central.py
+-rw-r--r--   0        0        0    55036 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/central.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/convert.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/docstrings.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/py.typed
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/random.py
+-rw-r--r--   0        0        0    17389 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/resample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/typing.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/utils.py
+-rw-r--r--   0        0        0    69450 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/xcentral.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_lib/__init__.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_lib/convert.py
+-rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_lib/pushers.py
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_lib/resample.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 cmomy-0.9.0/src/cmomy/_lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/_simple_cmom.py
+-rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0    17563 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_central.py
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_central_2.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_convert.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_random.py
+-rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_resample.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_stability.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_verify.py
+-rw-r--r--   0        0        0    16425 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_xcentral.py
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 cmomy-0.9.0/tests/test_xcentral_constructors.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/clean_kernelspec.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/common_utils.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/create_pythons.py
+-rw-r--r--   0        0        0    10827 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/dataclass_parser.py
+-rw-r--r--   0        0        0    42224 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/noxtools.py
+-rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/pipxrun.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 cmomy-0.9.0/tools/projectconfig.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 cmomy-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 cmomy-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 cmomy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 cmomy-0.9.0/PKG-INFO
```

### Comparing `cmomy-0.8.0/.cruft.json` & `cmomy-0.9.0/.cruft.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'d9054feffe84e992cba4d2682fa571f11a0be89c'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "develop",
-    "commit": "ce1b977122d2269581a75ef434e90f5e3935a0ca",
+    "commit": "d9054feffe84e992cba4d2682fa571f11a0be89c",
     "context": {
         "cookiecutter": {
             "__answers": "",
             "_copy_without_render": [],
             "_template": "https://github.com/usnistgov/cookiecutter-nist-python.git",
             "command_line_interface": "none",
             "conda_channel": "conda-forge",
```

### Comparing `cmomy-0.8.0/.editorconfig` & `cmomy-0.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/.pre-commit-config.yaml` & `cmomy-0.9.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
----
 # pre-commit install
 # pre-commit run --all-files
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 default_install_hook_types:
   - pre-commit
   - commit-msg
 repos:
   # * Top level
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: check-json
@@ -25,141 +24,138 @@
   - repo: https://github.com/mxr/sync-pre-commit-deps
     rev: v0.0.1
     hooks:
       - id: sync-pre-commit-deps
 
   # * Pyproject-fmt
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "1.7.0"
+    rev: 1.7.0
     hooks:
       - id: pyproject-fmt
-        args: ["--indent=4", "--keep-full-version"]
+        args: [--indent=4, --keep-full-version]
         files: ^pyproject.toml$
 
   # * Prettier
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v4.0.0-alpha.8"
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         alias: markdownlint
         stages: [commit]
         additional_dependencies:
           - prettier-plugin-toml
 
   # * Markdown
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.12.1
+    rev: v0.13.0
     hooks:
       - id: markdownlint-cli2
         alias: markdownlint
-        args: ["--style prettier"]
+        args: [--style, prettier]
 
   # * Linting
   # To be replace by ruff analog when I find one ...
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.16.0"
+    rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==24.1.0
+          - black==24.3.0
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.1"
+    rev: v0.3.5
     hooks:
       - id: ruff
-        types_or: ["python", "pyi", "jupyter"]
-        args: ["--fix", "--show-fixes"]
+        types_or: &ruff-types-or [python, pyi, jupyter]
+        args: [--fix, --show-fixes]
       - id: ruff-format
-        types_or: ["python", "pyi", "jupyter"]
+        types_or: *ruff-types-or
 
   # * Spelling
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies: [tomli]
-        args: ["-I", "docs/spelling_wordlist.txt"]
+        args: [-I, docs/spelling_wordlist.txt]
         exclude_types: [jupyter]
 
-  # * Notebook formatting
+  # * Notebook spelling
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.7.1
+    rev: 1.8.5
     hooks:
       - id: nbqa
         alias: nbqa-codespell
         name: nbqa-codespell
-        additional_dependencies: [codespell==2.2.6, tomli]
+        additional_dependencies: &codespell-deps [codespell==2.2.6, tomli] # make sure same as above
         args:
-          [
-            "codespell",
-            "--ignore-words=docs/spelling_wordlist.txt",
-            "--nbqa-shell",
-          ]
+          [codespell, --ignore-words=docs/spelling_wordlist.txt, --nbqa-shell]
       - id: nbqa
         alias: nbqa-codespell
         name: nbqa-codespell-markdown
-        additional_dependencies: [codespell==2.2.6, tomli]
+        additional_dependencies: *codespell-deps
         args:
           [
-            "codespell",
-            "--ignore-words=docs/spelling_wordlist.txt",
-            "--nbqa-md",
-            "--nbqa-shell",
+            codespell,
+            --ignore-words=docs/spelling_wordlist.txt,
+            --nbqa-shell,
+            --nbqa-md,
           ]
 
-      # Use ruff for this instead ...
-      # - id: nbqa-ruff
-      #   additional_dependencies: [ruff==0.1.14]
-      #   # Replace with builtin if/when available
-      # - id: nbqa
-      #   alias: nbqa-ruff-format
-      #   name: nbqa-ruff-format
-      #   additional_dependencies: [ruff==0.1.14]
-      #   args: ["ruff format --force-exclude"]
+  # * Strip out metadata from notebooks
+  - repo: https://github.com/kynan/nbstripout
+    rev: 0.7.1
+    hooks:
+      - id: nbstripout
+        args: [
+            --keep-output, # keep output (needed for nbval testing)
+            --keep-count, # Errors with nbval without this...
+            --extra-keys, # strip out kernelspec.  If use this, always have to reselect kernel when open a notebook...
+            "metadata.kernelspec metadata.kernel_spec",
+          ]
 
   # * Commit message
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.14.1
+    rev: v3.21.3
     hooks:
       - id: commitizen
         stages: [commit-msg]
 
   # * Manual Linting ------------------------------------------------------------
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         stages: [manual]
         args: [--py38-plus]
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.7.1
+    rev: 1.8.5
     hooks:
       - id: nbqa-pyupgrade
         additional_dependencies: [pyupgrade]
         stages: [manual]
         args: [--py38-plus]
 
   # ** typos
   # Probably stick with codespell, but this might also be nice...
   - repo: https://github.com/crate-ci/typos
-    rev: v1.18.2
+    rev: v1.20.5
     hooks:
       - id: typos
-        # args: []
         stages: [manual]
         exclude: "[.]ipynb$"
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.7.1
+    rev: 1.8.5
     hooks:
       - id: nbqa
         alias: nbqa-typos
         name: nbqa-typos
-        additional_dependencies: [typos==1.18.2]
+        additional_dependencies: &typos-deps [typos==1.20.5] # make sure save version as above.
         stages: [manual]
-        exclude: "^examples/archived/"
-        args: ["typos", "--nbqa-shell"]
+        args: [typos, --nbqa-shell]
+        exclude: &nbqa-typos-exclude "^examples/archived/"
       - id: nbqa
         alias: nbqa-typos
         name: nbqa-typos-markdown
-        additional_dependencies: [typos==1.18.2]
+        additional_dependencies: *typos-deps
         stages: [manual]
-        exclude: "^examples/archived/"
-        args: ["typos", "--nbqa-shell", "--nbqa-md"]
+        args: [typos, --nbqa-shell, --nbqa-md]
+        exclude: *nbqa-typos-exclude
```

### Comparing `cmomy-0.8.0/.recipe-append.yaml` & `cmomy-0.9.0/.recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/CONTRIBUTING.md` & `cmomy-0.9.0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -119,21 +119,14 @@
 
   To test against multiple python versions, use [nox]:
 
   ```bash
   nox -s test
   ```
 
-  Additionally, you should run the following:
-
-  ```bash
-  make pre-commit-lint-markdown
-  make pre-commit-codespell
-  ```
-
 - Create changelog fragment. See [scriv] for more info.
 
   ```bash
   scriv create --edit
   ```
 
 - Commit your changes and push your branch to GitHub:
@@ -305,20 +298,18 @@
 ```
 
 ## ipykernel
 
 The environments created by nox `dev` and `docs-conda` will try to add
 meaningful display names for ipykernel. These are installed at the user level.
 To cleanup the kernels (meaning, removing installed kernels that point to a
-removed environment), You can use the script `tools/clean_kernelspec.py`. This
-script should be run from the environment of the jupyter server. For example, if
-you run jupyter from a conda environment named `notebook`, run
+removed environment), You can use the script `tools/clean_kernelspec.py`:
 
 ```bash
-conda run -n notebook python tools/clean_kernelspec.py
+python tools/clean_kernelspec.py
 ```
 
 ## Building the docs
 
 We use [nox] to isolate the documentation build. Specific tasks can be run with
 
 ```bash
@@ -436,14 +427,19 @@
 
 ```bash
 nox -s typing -- +m [commands] [options]
 ```
 
 Use `typing-conda` to test typing in a conda environment.
 
+Note that the repo is setup to use a single install of [mypy] and [pyright]. The
+script `tools/pipxrun.py` will run check if an appropriate version of the
+typecheckers is installed. If not, they will be run (and cached) using
+`pipx run`.
+
 ## Setup development environment
 
 This project uses a host of tools to (hopefully) make development easier. We
 recommend installing some of these tools system wide. For this, we recommend
 using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
 yours. For conda, we recommend actually using [mamba]. Alternatively, you can
 setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
@@ -498,62 +494,79 @@
 [autoenv](https://github.com/hyperupcall/autoenv) (if using bash) to auto
 activate the development environment when in the parent directory.
 
 Note that you can bootstrap the whole process with [pipx] using:
 
 ```bash
 pipx run --spec nox \
-     nox -s dev -- \
+     nox -s dev/dev-venv -- \
      ++dev-envname dev/dev-complete
 ```
 
 ### Development tools
 
 We recommend installing the following tools with [pipx] or [condax]. If you'd
 like to install them in the development environment instead, use the
 `dev-complete` version of the commands above.
 
 Additional tools are:
 
+- [pipx]
 - [pre-commit]
-- [scriv]
-- [nbqa]
-- [pyright]
+- [uv] (optional, highly recommended)
+- [scriv] (optional)
+- [pyright] (optional)
 - [cruft] (optional)
 - [commitizen] (optional)
 - [cog] (optional)
+- [nbqa] (optional)
 
 These are setup using the following:
 
 ```console
+# install pipx using something like ...
+pip install --user pipx
+
 condax/pipx install pre-commit
-pipx install scriv
-condax/pipx install nbqa
-condax/pipx install pyright
 
 # optional packages
+pipx install scriv
+condax/pipx install uv
+condax/pipx install pyright
 condax/pipx install cruft
 condax/pipx install commitizen
 condax/pipx install cogapp
+condax/pipx install nbqa
 ```
 
+Note that the repo is setup to automatically use pipx for many of these tools.
+Behind the scenes, the makefile and `noxfile.py` will invoke `tools/pipxrun.py`.
+This will either run the tool with `pipx run tool..`, or, if it is already
+installed (with proper version), run the tool from the install. This prevents
+having to install a bunch of tooling in the "dev" environment, and also avoid
+creating a bunch of through away [nox] environments. This is experimental, and I
+might change back to using small [nox] environments again in the future.
+
 ## Package version
 
 [hatch-vcs]: https://github.com/ofek/hatch-vcs
 
 Versioning is handled with [hatch-vcs]. The package version is set by the git
 tag. For convenience, you can override the version with nox setting
 `++version ...`. This is useful for updating the docs, etc.
 
 Note that the version in a given environment/session can become stale. The
 easiest way to update the installed package version version is to reinstall the
 package. This can be done using the following:
 
 ```bash
+# using pip
 pip install -e . --no-deps
+# using uv
+uv pip install -e . --no-deps
 ```
 
 To do this in a given session, use:
 
 ```bash
 nox -s {session} -- +P/++update-package
 ```
@@ -564,19 +577,21 @@
   https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
 [conda]: https://docs.conda.io/en/latest/
 [condax]: https://github.com/mariusvniekerk/condax
 [conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
 [cruft]: https://github.com/cruft/cruft
 [git-flow]: https://github.com/nvie/gitflow
 [mamba]: https://github.com/mamba-org/mamba
+[mypy]: https://github.com/python/mypy
 [nbqa]: https://github.com/nbQA-dev/nbQA
 [nbval]: https://github.com/computationalmodelling/nbval
 [nox]: https://github.com/wntrblm/nox
 [pip-tools]: https://github.com/jazzband/pip-tools
 [pipx]: https://github.com/pypa/pipx
 [pre-commit]: https://pre-commit.com/
 [pyenv]: https://github.com/pyenv/pyenv
 [pyproject2conda]: https://github.com/wpk-nist-gov/pyproject2conda
 [pyright]: https://github.com/microsoft/pyright
 [scriv]: https://github.com/nedbat/scrivl
+[uv]: https://github.com/astral-sh/uv
 [tox]: https://tox.wiki/en/latest/
 [virtualenv]: https://virtualenv.pypa.io/en/latest/
```

### Comparing `cmomy-0.8.0/Makefile` & `cmomy-0.9.0/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -122,153 +122,140 @@
 	nox -s requirements
 requirements/%.yaml: pyproject.toml
 	nox -s requirements
 requirements/%.txt: pyproject.toml
 	nox -s requirements
 
 ################################################################################
+# * Typing
+################################################################################
+PIPXRUN = python tools/pipxrun.py
+PIPXRUN_OPTS = -r requirements/lock/py311-pipxrun-tools.txt -v
+.PHONY: mypy pyright
+mypy: ## Run mypy
+	$(PIPXRUN) $(PIPXRUN_OPTS) -c mypy
+pyright: ## Run pyright
+	$(PIPXRUN) $(PIPXRUN_OPTS) -c pyright
+typecheck: ## Run mypy and pyright
+	$(PIPXRUN) $(PIPXRUN_OPTS) -c mypy -c pyright
+
+.PHONY: typecheck-tools
+typecheck-tools:
+	$(PIPXRUN) $(PIPXRUN_OPTS) -c "mypy --strict" -c pyright -- noxfile.py tools/*.py
+
+################################################################################
 # * NOX
 ###############################################################################
-# NOTE: Below, we use requirement of the form "requirements/dev.txt"
-# Since any of these files will trigger a rebuild of all requirements,
-# the actual "txt" or "yaml" file doesn't matter
-# ** dev
 NOX=nox
-.PHONY: dev-env
-dev-env: requirements/dev.txt ## create development environment using nox
-	$(NOX) -e dev
-
-# ** testing
-.PHONY: test-all
-test-all: requirements/test.txt ## run tests on every Python version with nox.
-	$(NOX) -s test
-
 # ** docs
-.PHONY: docs-build docs-release docs-clean
+.PHONY: docs-build docs-clean docs-clean-build docs-release
 docs-build: ## build docs in isolation
 	$(NOX) -s docs -- +d build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
 docs-release: ## release docs.
-	$(NOX) -s docs -- +d release
+	$(PIPXRUN) $(PIPXRUN_OPTS) -c "ghp-import -o -n -m \"update docs\" -b nist-pages" docs/_build/html
 
-.PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
+.PHONY: docs-open docs-spelling docs-livehtml docs-linkcheck
+docs-open: ## open the build
+	$(NOX) -s docs -- +d open
 docs-spelling: ## run spell check with sphinx
 	$(NOX) -s docs -- +d spelling
 docs-livehtml: ## use autobuild for docs
 	$(NOX) -s docs -- +d livehtml
-docs-open: ## open the build
-	$(NOX) -s docs -- +d open
 docs-linkcheck: ## check links
 	$(NOX) -s docs -- +d linkcheck
 
-docs-build docs-release docs-clean docs-livehtml docs-linkcheck: requirements/docs.txt
-
 # ** typing
-.PHONY: typing-mypy typing-pyright typing-pytype typing-all
+.PHONY: typing-mypy typing-pyright typing-typecheck
 typing-mypy: ## run mypy mypy_args=...
 	$(NOX) -s typing -- +m mypy
 typing-pyright: ## run pyright pyright_args=...
 	$(NOX) -s typing -- +m pyright
-typing-pytype: ## run pytype pytype_args=...
-	$(NOX) -s typing -- +m pytype
-typing-all:
-	$(NOX) -s typing -- +m mypy pyright pytype
-typing-mypy typing-pyright typing-pytype typing-all: requirements/typing.txt
+typing-typecheck:
+	$(NOX) -s typing -- +m mypy pyright
 
 # ** dist pypi
 .PHONY: build testrelease release
-build: requirements/build.txt ## build dist
+build: ## build dist
 	$(NOX) -s build
 testrelease: ## test release on testpypi
 	$(NOX) -s publish -- +p test
 release: ## release to pypi, can pass posargs=...
 	$(NOX) -s publish -- +p release
 
-.PHONY: check-release check-wheel check-dist
-check-release: ## run twine check on dist
-	$(NOX) -s publish -- +p check
-check-wheel: ## Run check-wheel-contents (requires check-wheel-contents to be installed)
-	check-wheel-contents dist/*.whl
-check-dist: check-release check-wheel ## Run check-release and check-wheel
-.PHONY:  list-wheel list-sdist list-dist
-list-wheel: ## Cat out contents of wheel
-	unzip -vl dist/*.whl
-list-sdist: ## Cat out contents of sdist
-	tar -tzvf dist/*.tar.gz
-list-dist: list-wheel list-sdist ## Cat out sdist and wheel contents
-
 # ** dist conda
 .PHONY: conda-recipe conda-build
 conda-recipe: ## build conda recipe can pass posargs=...
 	$(NOX) -s conda-recipe
 conda-build: ## build conda recipe can pass posargs=...
 	$(NOX) -s conda-build
 
 # ** list all options
 .PHONY: nox-list
 nox-list:
 	$(NOX) --list
 
-
 ################################################################################
-# * Installation
+# ** sdist/wheel check
 ################################################################################
-.PHONY: install install-dev
-install: ## install the package to the active Python's site-packages (run clean?)
-	pip install . --no-deps
-
-install-dev: ## install development version (run clean?)
-	pip install -e . --no-deps
-
+.PHONY: check-release check-wheel check-dist
+check-release: ## run twine check on dist
+	$(NOX) -s publish -- +p check
+check-wheel: ## Run check-wheel-contents (requires check-wheel-contents to be installed)
+	$(PIPXRUN) -c check-wheel-contents dist/*.whl
+check-dist: check-release check-wheel ## Run check-release and check-wheel
+.PHONY:  list-wheel list-sdist list-dist
+list-wheel: ## Cat out contents of wheel
+	unzip -vl dist/*.whl
+list-sdist: ## Cat out contents of sdist
+	tar -tzvf dist/*.tar.gz
+list-dist: list-wheel list-sdist ## Cat out sdist and wheel contents
 
 ################################################################################
 # * NOTEBOOK typing/testing
 ################################################################################
 NOTEBOOKS ?= examples/usage
-.PHONY: mypy-notebook pyright-notebook typing-notebook
+NBQA = $(PIPXRUN) $(PIPXRUN_OPTS) -c "nbqa --nbqa-shell \"$(PIPXRUN)\" $(NOTEBOOKS) $(PIPXRUN_OPTS) $(_NBQA)"
+.PHONY: mypy-notebook pyright-notebook typecheck-notebook test-notebook
+mypy-notebook: _NBQA = -c mypy
 mypy-notebook: ## run nbqa mypy
-	nbqa --nbqa-shell mypy $(NOTEBOOKS)
+	$(NBQA)
+pyright-notebook: _NBQA = -c pyright
 pyright-notebook: ## run nbqa pyright
-	nbqa --nbqa-shell pyright $(NOTEBOOKS)
-typing-notebook: mypy-notebook pyright-notebook ## run nbqa mypy/pyright
-
-.PHONY: pytest-nbval
-pytest-notebook:  ## run pytest --nbval
+	$(NBQA)
+typecheck-notebook: _NBQA = -c mypy -c pyright
+typecheck-notebook: ## run nbqa mypy/pyright
+	$(NBQA)
+test-notebook:  ## run pytest --nbval
 	pytest --nbval --nbval-current-env --nbval-sanitize-with=config/nbval.ini --dist loadscope -x $(NOTEBOOKS)
 
 .PHONY: clean-kernelspec
 clean-kernelspec: ## cleanup unused kernels (assuming notebooks handled by conda environment notebook)
-	conda run -n notebook python tools/clean_kernelspec.py
-
+	python tools/clean_kernelspec.py
 
 ################################################################################
 # * Other tools
 ################################################################################
-
 # Note that this requires `auto-changelog`, which can be installed with pip(x)
+.PHONY: auto-changelog
 auto-changelog: ## autogenerate changelog and print to stdout
 	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
 
+.PHONY:
 commitizen-changelog:
 	cz changelog --unreleased-version unreleased --dry-run --incremental
 
 # tuna analyze load time:
 .PHONY: tuna-analyze
 tuna-import: ## Analyze load time for module
 	python -X importtime -c 'import cmomy' 2> tuna-loadtime.log
-	tuna tuna-loadtime.log
+	$(PIPXRUN) -c tuna tuna-loadtime.log
 	rm tuna-loadtime.log
 
-.PHONY: typing-tools
-typing-tools:
-	mypy --strict noxfile.py tools/*.py
-	pyright noxfile.py tools/*.py
-
-
 .PHONY: test-all-cover
 test-all-cover:
 	nox -s test test-notebook -- ++test-opts --run-slow
 	nox -s test-3.11 coverage -- ++test-no-numba ++test-opts --run-slow ++test-no-numba
```

### Comparing `cmomy-0.8.0/README.md` & `cmomy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/conftest.py` & `cmomy-0.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/noxfile.py` & `cmomy-0.9.0/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """Config file for nox."""
+
 # * Imports ----------------------------------------------------------------------------
 from __future__ import annotations
 
-import os
 import shlex
 import shutil
 import sys
-from functools import lru_cache, wraps
+from functools import lru_cache, partial, wraps
 
 # Should only use on python version > 3.10
 if sys.version_info < (3, 10):
     msg = "python>=3.10 required"
     raise RuntimeError(msg)
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Annotated,
+    Any,
     Callable,
     Iterable,
     Iterator,
     Literal,
     Sequence,
     TypeAlias,
     TypedDict,
 )
 
 # fmt: off
 sys.path.insert(0, ".")
+from tools import pipxrun
 from tools.dataclass_parser import DataclassParser, add_option, option
 from tools.noxtools import (
     Installer,
+    cached_which,
     check_for_change_manager,
+    combine_list_list_str,
     combine_list_str,
     factory_conda_backend,
     factory_virtualenv_backend,
     infer_requirement_path,
     is_conda_session,
     load_nox_config,
     open_webpage,
@@ -59,38 +63,51 @@
 
 # * Names ------------------------------------------------------------------------------
 
 PACKAGE_NAME = "cmomy"
 IMPORT_NAME = "cmomy"
 KERNEL_BASE = "cmomy"
 
-# * Environments variables -------------------------------------------------------------
-
-# Set numba_cache directory for sharing
-os.environ["NUMBA_CACHE_DIR"] = str(Path(__file__).parent / ".numba_cache")
-
 # * nox options ------------------------------------------------------------------------
 
 ROOT = Path(__file__).parent
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = ["test"]
+nox.options.default_venv_backend = "uv"
 
 # * User Config ------------------------------------------------------------------------
 
 CONFIG = load_nox_config()
+# if you'd like to disallow uv.
+# You'll need to import this from tools.noxtools
+# DISALLOW_WHICH.append("uv")
+
 
 # * Options ---------------------------------------------------------------------------
 
 LOCK = True
 
 PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11"]
 PYTHON_DEFAULT_VERSION = "3.11"
 
-# conda/mamba
+
+PIPXRUN_LOCK_REQUIREMENTS = "requirements/lock/py{}-pipxrun-tools.txt".format(
+    PYTHON_DEFAULT_VERSION.replace(".", "")
+)
+PIPXRUN_MIN_REQUIREMENTS = "requirements/pipxrun-tools.txt"
+
+
+@lru_cache
+def get_pipxrun_specs(requirements: str | None = None) -> pipxrun.Specifications:
+    """Get specs for pipxrun."""
+    requirements = requirements or PIPXRUN_MIN_REQUIREMENTS
+    return pipxrun.Specifications.from_requirements(requirements=requirements)
+
+
 for backend in ["mamba", "micromamba", "conda"]:
     if shutil.which(backend):
         CONDA_BACKEND: Literal["mamba", "micromamba", "conda"] = backend  # type: ignore[assignment]
         break
 else:
     msg = "no conda-like backend found"
     raise ValueError(msg)
@@ -154,27 +171,25 @@
 
     # config
     dev_extras: OPT_TYPE = add_option(help="`extras` to include in dev environment")
     python_paths: OPT_TYPE = add_option(help="paths to python executables")
 
     # requirements
     requirements_force: bool = False
-    requirements_run: RUN_ANNO = None
     requirements_no_notify: bool = add_option(
         default=False,
         help="Skip notification of pip-compile",
     )
 
     # conda-lock
     conda_lock_channel: OPT_TYPE = add_option(help="conda channels")
-    conda_lock_platform: list[
-        Literal["osx-64", "linux-64", "win-64", "osx-arm64", "all"]
-    ] | None = add_option(help="platform(s) to buiuld lock file for.")
+    conda_lock_platform: (
+        list[Literal["osx-64", "linux-64", "win-64", "osx-arm64", "all"]] | None
+    ) = add_option(help="platform(s) to buiuld lock file for.")
     conda_lock_include: OPT_TYPE = add_option(help="lock files to create")
-    conda_lock_run: RUN_ANNO = None
     conda_lock_mamba: bool = False
     conda_lock_force: bool = False
 
     # pip-compile
     pip_compile_force: bool = False
     pip_compile_upgrade: bool = add_option(
         "--pip-compile-upgrade",
@@ -195,52 +210,49 @@
     test_opts: OPT_TYPE = add_option(help="Options to pytest")
     test_run: RUN_ANNO = None
     test_no_numba: bool = False
     no_cov: bool = False
 
     # coverage
     coverage: list[Literal["erase", "combine", "report", "html", "open"]] | None = None
-    coverage_run: RUN_ANNO = None
-    coverage_run_internal: RUN_TYPE = None
 
     # testdist
     testdist_run: RUN_ANNO = None
 
     # docs
-    docs: list[
-        Literal[
-            "html",
-            "build",
-            "symlink",
-            "clean",
-            "livehtml",
-            "linkcheck",
-            "spelling",
-            "showlinks",
-            "release",
-            "open",
-            "serve",
+    docs: (
+        list[
+            Literal[
+                "html",
+                "build",
+                "symlink",
+                "clean",
+                "livehtml",
+                "linkcheck",
+                "spelling",
+                "showlinks",
+                "open",
+                "serve",
+            ]
         ]
-    ] | None = add_option("--docs", "-d", help="doc commands")
+        | None
+    ) = add_option("--docs", "-d", help="doc commands")
     docs_run: RUN_ANNO = None
 
-    # lint (pre-commit)
-    lint_run: RUN_ANNO = None
-
     # typing
     typing: list[
         Literal[
             "clean",
             "mypy",
             "pyright",
             "pytype",
             "all",
             "mypy-notebook",
             "pyright-notebook",
-            "typing-notebook",
+            "typecheck-notebook",
         ]
     ] = add_option("--typing", "-m")
     typing_run: RUN_ANNO = None
     typing_run_internal: RUN_TYPE = add_option(
         help="Run internal (in session) commands.",
     )
 
@@ -252,19 +264,17 @@
     build_opts: OPT_ANNO = None
     build_silent: bool = False
 
     # publish
     publish: list[Literal["release", "test", "check"]] | None = add_option(
         "-p", "--publish"
     )
-    publish_run: RUN_ANNO = None
 
     # conda-recipe/grayskull
     conda_recipe: list[Literal["recipe", "recipe-full"]] | None = None
-    conda_recipe_run: RUN_ANNO = None
     conda_recipe_sdist_path: str | None = None
 
     # conda-build
     conda_build: list[Literal["build", "clean"]] | None = None
     conda_build_run: RUN_ANNO = None
 
 
@@ -341,76 +351,54 @@
     """Create the file ./config/userconfig.toml"""
     args: list[str] = []
     if opts.dev_extras:
         args += ["--dev-extras", *opts.dev_extras]
     if opts.python_paths:
         args += ["--python-paths", *opts.python_paths]
 
-    session.run("python", "tools/projectconfig.py", *args)
+    session.run(sys.executable, "tools/projectconfig.py", *args)
 
 
 # ** requirements
-@nox.session(python=False)
-def pyproject2conda(
-    session: Session,
-) -> None:
-    """Alias to reqs"""
-    session.notify("requirements")
-
-
-@nox.session
+@nox.session(name="requirements", python=False)
 @add_opts
 def requirements(
     session: Session,
     opts: SessionParams,
 ) -> None:
     """
     Create environment.yaml and requirement.txt files from pyproject.toml using pyproject2conda.
 
     These will be placed in the directory "./requirements".
     """
-    runner = Installer(
+    pipxrun.run(
+        "pyproject2conda>=0.11.0",
+        "project",
+        "--verbose",
+        *(["--overwrite=force"] if opts.requirements_force else []),
         session=session,
-        pip_deps="pyproject2conda>=0.11.0",
-        update=opts.update,
-    ).install_all(log_session=opts.log_session)
-
-    if opts.requirements_run:
-        runner.run_commands(opts.requirements_run)
-    else:
-        session.run(
-            "pyproject2conda",
-            "project",
-            "--verbose",
-            *(["--overwrite", "force"] if opts.requirements_force else []),
-        )
+        external=True,
+    )
 
-        if not opts.requirements_no_notify and opts.lock:
+    if not opts.requirements_no_notify and opts.lock:
+        if cached_which("uv"):
+            session.notify("uv-compile")
+        else:
             for py in PYTHON_ALL_VERSIONS:
                 session.notify(f"pip-compile-{py}")
 
 
 # # ** conda-lock
-@nox.session(name="conda-lock", **DEFAULT_KWS)
+@nox.session(name="conda-lock", python=False)
 @add_opts
 def conda_lock(
     session: Session,
     opts: SessionParams,
 ) -> None:
     """Create lock files using conda-lock."""
-    (
-        Installer(
-            session=session,
-            pip_deps="conda-lock>=2.2.0",
-            update=opts.update,
-        ).install_all()
-    )
-
-    session.run("conda-lock", "--version")
-
     conda_lock_exclude = ["test-extras"]
     conda_lock_include = opts.conda_lock_include or [
         "test",
         "dev",
         "dev-complete",
         "nox",
     ]
@@ -447,33 +435,109 @@
             force_write=opts.conda_lock_force,
         ) as changed:
             if opts.conda_lock_force or changed:
                 session.log(f"Creating {lockfile}")
                 # insert -f for each arg
                 if lockfile.exists():
                     lockfile.unlink()
-                session.run(
+                pipxrun.run(
                     "conda-lock",
                     "--mamba" if opts.conda_lock_mamba else "--no-mamba",
                     *prepend_flag("-c", *channel),
                     *prepend_flag("-p", *platform),
                     *prepend_flag("-f", *deps),
                     f"--lockfile={lockfile}",
+                    specs=get_pipxrun_specs(),
+                    session=session,
+                    external=True,
                 )
             else:
                 session.log(f"Skipping {lockfile} (exists)")
 
-    session_run_commands(session, opts.conda_lock_run)
     for path in (ROOT / "requirements").relative_to(ROOT.cwd()).glob("py*.yaml"):
         create_lock(path)
 
 
+def _run_compile_pre(
+    runner: Installer,
+    run: RUN_TYPE,
+    run_internal: RUN_TYPE,
+) -> bool:
+    if run:
+        runner.run_commands(run)
+        return True
+
+    if run_internal:
+        runner.run_commands(run_internal, external=False)
+        return True
+
+    return False
+
+
+def _run_compile_options(
+    options: OPT_TYPE,
+    force: bool,
+    upgrade: bool,
+    upgrade_package: OPT_TYPE,
+) -> tuple[list[str], bool]:
+    options = list(options) if options else []
+    if upgrade:
+        options = [*options, "-U"]
+
+    if upgrade_package:
+        options = [*options, *prepend_flag("-P", upgrade_package)]
+
+    force = force or upgrade or bool(upgrade_package)
+
+    return options, force
+
+
+def _run_compile_env(
+    session: nox.Session,
+    compile_command: Sequence[str],
+    python: str,
+    options: Sequence[str],
+    force: bool,
+    env: str,
+    envs_optional: Sequence[str],
+    **kwargs: Any,
+) -> None:
+    reqspath = infer_requirement_path(env, ext=".txt", check_exists=False)
+    if not reqspath.is_file():
+        if env in envs_optional:
+            return
+        msg = f"Missing file {reqspath}"
+        raise ValueError(msg)
+
+    lockpath = infer_requirement_path(
+        env,
+        ext=".txt",
+        python_version=python,
+        lock=True,
+        check_exists=False,
+    )
+
+    with check_for_change_manager(
+        reqspath,
+        target_path=lockpath,
+        force_write=force,
+    ) as changed:
+        if force or changed:
+            session.log(f"Creating {lockpath}")
+            session.run(
+                *compile_command, *options, "-o", str(lockpath), str(reqspath), **kwargs
+            )
+
+        else:
+            session.log(f"Skipping {lockpath}")
+
+
 @nox.session(name="pip-compile", **ALL_KWS)
 @add_opts
-def pip_compile(  # noqa: C901
+def pip_compile(
     session: Session,
     opts: SessionParams,
 ) -> None:
     """
     Run pip-compile.
 
     Note that this session is also used to run pip-sync with correct python version for
@@ -481,88 +545,110 @@
     """
     runner = Installer(
         session=session,
         pip_deps=["pip-tools"],
         update=opts.update,
     ).install_all(log_session=opts.log_session)
 
-    if opts.pip_compile_run:
-        # run commands and exit
-        runner.run_commands(opts.pip_compile_run)
-        return
+    if not isinstance(session.python, str):
+        msg = "must set python version"
+        raise TypeError(msg)
 
-    if opts.pip_compile_run_internal:
-        runner.run_commands(opts.pip_compile_run_internal, external=False)
+    if _run_compile_pre(runner, opts.pip_compile_run, opts.pip_compile_run_internal):
         return
 
-    options = opts.pip_compile_opts or []
-
-    force = (
-        opts.pip_compile_force
-        or opts.pip_compile_upgrade
-        or bool(opts.pip_compile_upgrade_package)
+    options, force = _run_compile_options(
+        options=opts.pip_compile_opts,
+        force=opts.pip_compile_force,
+        upgrade=opts.pip_compile_upgrade,
+        upgrade_package=opts.pip_compile_upgrade_package,
     )
 
-    if opts.pip_compile_upgrade:
-        options = [*options, "-U"]
-
-    if opts.pip_compile_upgrade_package:
-        options = options + prepend_flag("-P", opts.pip_compile_upgrade_package)
-
     envs_all = ["test", "typing"]
     envs_dev = ["dev", "dev-complete", "docs"]
-    envs_dev_optional = ["test-notebook"]
+    envs_dev_optional = ["test-notebook", "pipxrun-tools"]
 
     if session.python == PYTHON_DEFAULT_VERSION:
         envs = envs_all + envs_dev + envs_dev_optional
     else:
         envs = envs_all
 
     for env in envs:
-        if not isinstance(session.python, str):
-            msg = "session.python must be a string"
-            raise TypeError(msg)
-
-        reqspath = infer_requirement_path(env, ext=".txt", check_exists=False)
-        if not reqspath.is_file():
-            if env in envs_dev_optional:
-                continue
-            msg = f"Missing file {reqspath}"
-            raise ValueError(msg)
-
-        lockpath = infer_requirement_path(
-            env,
-            ext=".txt",
-            python_version=session.python,
-            lock=True,
-            check_exists=False,
+        _run_compile_env(
+            session=session,
+            compile_command=("pip-compile",),
+            python=session.python,
+            options=options,
+            force=force,
+            env=env,
+            envs_optional=envs_dev_optional,
+            external=False,
         )
 
-        with check_for_change_manager(
-            reqspath,
-            target_path=lockpath,
-            force_write=force,
-        ) as changed:
-            if force or changed:
-                session.log(f"Creating {lockpath}")
-                session.run("pip-compile", *options, "-o", str(lockpath), str(reqspath))
 
-            else:
-                session.log(f"Skipping {lockpath}")
+# ** uv pip compile
+@nox.session(name="uv-compile", python=False)
+@add_opts
+def uv_compile(
+    session: Session,
+    opts: SessionParams,
+) -> None:
+    """Run uv pip compile ..."""
+    uv_path = cached_which("uv")
+    if uv_path is None:
+        session.log("Need to install uv to use it...")
+        return
+
+    options, force = _run_compile_options(
+        options=opts.pip_compile_opts,
+        force=opts.pip_compile_force,
+        upgrade=opts.pip_compile_upgrade,
+        upgrade_package=opts.pip_compile_upgrade_package,
+    )
+
+    envs_all = ["test", "typing"]
+    envs_dev = ["dev", "dev-complete", "docs"]
+    envs_dev_optional = ["test-notebook", "pipxrun-tools"]
+
+    for python in set(PYTHON_ALL_VERSIONS).union({PYTHON_DEFAULT_VERSION}):
+        if python == PYTHON_DEFAULT_VERSION:
+            envs = envs_all + envs_dev + envs_dev_optional
+        else:
+            envs = envs_all
+
+        for env in envs:
+            _run_compile_env(
+                session=session,
+                compile_command=(
+                    uv_path,
+                    "pip",
+                    "compile",
+                    f"--python-version={python}",
+                    "--annotation-style=line",
+                ),
+                python=python,
+                options=options,
+                force=force,
+                env=env,
+                envs_optional=envs_dev_optional,
+                external=True,
+            )
 
 
 # ** testing
 def _test(
     session: nox.Session,
     run: RUN_TYPE,
     test_no_pytest: bool,
     test_opts: OPT_TYPE,
     no_cov: bool,
     test_no_numba: bool = False,
 ) -> None:
+    import os
+
     tmpdir = os.environ.get("TMPDIR", None)
 
     session_run_commands(session, run)
     if not test_no_pytest:
         opts = combine_list_str(test_opts or [])
 
         if test_no_numba:
@@ -684,50 +770,51 @@
         run=opts.test_run,
         test_no_pytest=opts.test_no_pytest,
         test_opts=test_opts,
         no_cov=opts.no_cov,
     )
 
 
-# *** coverage
-@nox.session
+@nox.session(python=False)
 @add_opts
 def coverage(
     session: Session,
     opts: SessionParams,
 ) -> None:
     """Run coverage."""
-    runner = Installer(
-        session=session,
-        pip_deps="coverage[toml]",
-        update=opts.update,
-    ).install_all()
+    cmd = opts.coverage or ["combine", "html", "report"]
 
-    runner.run_commands(opts.coverage_run)
+    run = partial(pipxrun.run, specs=get_pipxrun_specs(), session=session)
 
-    cmd = opts.coverage or []
-    if not cmd and not opts.coverage_run and not opts.coverage_run_internal:
-        cmd = ["combine", "html", "report"]
+    paths = list(Path(".nox").glob("test-*/tmp/.coverage*"))
 
-    session.log(f"{cmd}")
+    if "erase" in cmd:
+        for path in paths:
+            if path.exists():
+                session.log(f"removing {path}")
+                path.unlink()
 
     for c in cmd:
         if c == "combine":
-            paths = list(
-                Path(session.virtualenv.location).parent.glob("test-*/tmp/.coverage*"),
-            )
-            session.log(f"{paths=}")
             if update_target(".coverage", *paths):
-                session.run("coverage", "combine", "--keep", "-a", *map(str, paths))
+                run(
+                    "coverage",
+                    "combine",
+                    "--keep",
+                    "-a",
+                    *paths,
+                )
         elif c == "open":
             open_webpage(path="htmlcov/index.html")
-        else:
-            session.run("coverage", c)
 
-    runner.run_commands(opts.coverage_run_internal)
+        else:
+            run(
+                "coverage",
+                c,
+            )
 
 
 # *** testdist (conda)
 def testdist(
     session: Session,
 ) -> None:
     """Test conda distribution."""
@@ -831,37 +918,32 @@
 
 
 nox.session(name="docs", **DEFAULT_KWS)(docs)
 nox.session(name="docs-conda", **CONDA_DEFAULT_KWS)(docs)
 
 
 # ** lint
-@nox.session
-@add_opts
+@nox.session(python=False)
 def lint(
     session: nox.Session,
-    opts: SessionParams,
 ) -> None:
     """
     Run linters with pre-commit.
 
     Defaults to `pre-commit run --all-files`.
     To run something else pass, e.g.,
     `nox -s lint -- --lint-run "pre-commit run --hook-stage manual --all-files`
     """
-    runner = Installer(
+    pipxrun.run(
+        "pre-commit",
+        "run",
+        "--all-files",  # "--show-diff-on-failure",
+        specs=get_pipxrun_specs(),
         session=session,
-        pip_deps="pre-commit",
-        update=opts.update,
-    ).install_all(log_session=opts.log_session)
-
-    if opts.lint_run:
-        runner.run_commands(opts.lint_run, external=True)
-    else:
-        session.run("pre-commit", "run", "--all-files")
+    )
 
 
 # ** type checking
 @add_opts
 def typing(  # noqa: C901
     session: nox.Session,
     opts: SessionParams,
@@ -886,44 +968,49 @@
 
     if "all" in cmd:
         cmd = ["mypy", "pyright", "pytype"]
 
     # set the cache directory for mypy
     session.env["MYPY_CACHE_DIR"] = str(Path(session.create_tmp()) / ".mypy_cache")
 
-    def _run_info(cmd: str) -> None:
-        session.run("which", cmd, external=True)
-        session.run(cmd, "--version", external=True)
-
     if "clean" in cmd:
         cmd.remove("clean")
 
         for name in [".mypy_cache", ".pytype"]:
             p = Path(session.create_tmp()) / name
             if p.exists():
                 session.log(f"removing cache {p}")
                 shutil.rmtree(str(p))
 
+    if not isinstance(session.python, str):
+        raise TypeError
+
+    run = partial(
+        pipxrun.run,
+        specs=get_pipxrun_specs(PIPXRUN_LOCK_REQUIREMENTS),
+        session=session,
+        python_version=session.python,
+        python_executable=runner.python_full_path,
+        external=True,
+    )
+
     for c in cmd:
         if c.endswith("-notebook"):
             session.run("make", c, external=True)
-            continue
-
-        _run_info(c)
-
-        if c == "mypy":
-            session.run("mypy", "--color-output")
+        elif c == "mypy":
+            run("mypy", "--color-output")
         elif c == "pyright":
-            session.run("pyright", external=True)
-        elif c == "pytype":
-            session.run("pytype", "-o", str(Path(session.create_tmp()) / ".pytype"))
+            run("pyright")
         else:
-            session.log(f"skipping unknown command {c}")
+            session.log(f"Skipping unknown command {c}")
+
+    for cmds in combine_list_list_str(opts.typing_run_internal or []):
+        run(*cmds)
 
-    runner.run_commands(opts.typing_run_internal, external=False)
+    # runner.run_commands(opts.typing_run_internal, external=False)
 
 
 nox.session(name="typing", **ALL_KWS)(typing)
 nox.session(name="typing-conda", **CONDA_ALL_KWS)(typing)
 
 
 # # ** Dist pypi
@@ -932,34 +1019,32 @@
 def build(session: nox.Session, opts: SessionParams) -> None:
     """
     Build the distribution.
 
     Note that default is to not use build isolation.
     Pass `--build-isolation` to use build isolation.
     """
-    (
-        Installer.from_envname(
-            session=session,
-            envname="build",
-            update=opts.update,
-        ).install_all(log_session=opts.log_session)
-    )
+    runner = Installer.from_envname(
+        session=session,
+        envname="build",
+        update=opts.update,
+    ).install_all(log_session=opts.log_session)
 
     if opts.version:
         session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = opts.version
 
     for cmd in opts.build or ["build"]:
         if cmd == "version":
-            session.run("python", "-m", "hatchling", "version")
+            session.run(runner.python_full_path, "-m", "hatchling", "version")
 
         elif cmd == "build":
             if Path(outdir := opts.build_outdir).exists():
                 shutil.rmtree(outdir)
 
-            args = f"python -m build --outdir {outdir}".split()
+            args = f"{runner.python_full_path} -m build --outdir {outdir}".split()
             if not opts.build_isolation:
                 args.append("--no-isolation")
 
             if opts.build_opts:
                 args.extend(opts.build_opts)
 
             out = session.run(*args, silent=opts.build_silent)
@@ -987,131 +1072,140 @@
     that depend on python version (something like have session build-3.11 ....)
     """
     dist_location = Path(session.cache_dir) / "dist"
     if reuse and getattr(get_package_wheel, "_called", False):
         session.log("Reuse isolated build")
     else:
         cmd = f"nox -s build -- ++build-outdir {dist_location} ++build-opts -w ++build-silent"
-        session.run(*shlex.split(cmd), external=True)
+        session.run_always(*shlex.split(cmd), external=True)
 
         # save that this was called:
         if reuse:
             get_package_wheel._called = True  # type: ignore[attr-defined]  # noqa: SLF001
 
     paths = list(dist_location.glob("*.whl"))
     if len(paths) != 1:
         msg = f"something wonky with paths {paths}"
         raise ValueError(msg)
 
     path = str(paths[0])
 
+    if cached_which("uv"):
+        path = f"{PACKAGE_NAME}@{path}"
+
     if extras:
         if not isinstance(extras, str):
             extras = ",".join(extras)
         path = f"{path}[{extras}]"
 
     if opts:
         if not isinstance(opts, str):
             opts = " ".join(opts)
         path = f"{path} {opts}"
 
     return path
 
 
-@nox.session
+@nox.session(python=False)
 @add_opts
 def publish(session: nox.Session, opts: SessionParams) -> None:
     """Publish the distribution"""
-    (
-        Installer(session=session, pip_deps="twine", update=opts.update)
-        .install_all(log_session=opts.log_session)
-        .run_commands(opts.publish_run)
+    run = partial(
+        pipxrun.run, specs=get_pipxrun_specs(), session=session, external=True
     )
 
     for cmd in opts.publish or []:
         if cmd == "test":
-            session.run("twine", "upload", "--repository", "testpypi", "dist/*")
-
+            run("twine", "upload", "--repository", "testpypi", "dist/*")
         elif cmd == "release":
-            session.run("twine", "upload", "dist/*")
-
+            run("twine", "upload", "dist/*")
         elif cmd == "check":
-            session.run("twine", "check", "--strict", "dist/*")
+            run("twine", "check", "--strict", "dist/*")
 
 
 # # ** Dist conda
-@nox.session(name="conda-recipe")
+@nox.session(name="conda-recipe", python=False)
 @add_opts
 def conda_recipe(
     session: nox.Session,
     opts: SessionParams,
 ) -> None:
     """Run grayskull to create recipe"""
-    runner = Installer(
-        session=session,
-        pip_deps=["grayskull"],
-        update=opts.update,
-    ).install_all(log_session=opts.log_session)
+    commands = opts.conda_recipe or ["recipe"]
 
-    run, commands = opts.conda_recipe_run, opts.conda_recipe
+    run = partial(pipxrun.run, specs=get_pipxrun_specs(), session=session)
 
-    runner.run_commands(run)
-
-    if not run and not commands:
-        commands = ["recipe"]
-
-    if not commands:
-        return
-
-    sdist_path = opts.conda_recipe_sdist_path
-    if not sdist_path:
+    if not (sdist_path := opts.conda_recipe_sdist_path):
         sdist_path = PACKAGE_NAME
         if opts.version:
             sdist_path = f"{sdist_path}=={opts.version}"
 
     for command in commands:
         if command == "recipe":
             # make directory?
             if not (d := Path("./dist-conda")).exists():
                 d.mkdir()
 
-            session.run(
+            run(
                 "grayskull",
                 "pypi",
                 sdist_path,
                 "--sections",
                 "package",
                 "source",
                 "build",
                 "requirements",
                 "-o",
                 "dist-conda",
             )
+
             _append_recipe(
                 f"dist-conda/{PACKAGE_NAME}/meta.yaml",
                 "config/recipe-append.yaml",
             )
             session.run("cat", f"dist-conda/{PACKAGE_NAME}/meta.yaml", external=True)
 
         elif command == "recipe-full":
             import tempfile
 
             with tempfile.TemporaryDirectory() as d:  # type: ignore[assignment,unused-ignore]
-                session.run(
+                run(
                     "grayskull",
                     "pypi",
                     sdist_path,
                     "-o",
                     str(d),
                 )
-                session.run(
-                    "cat",
-                    str(Path(d) / PACKAGE_NAME / "meta.yaml"),
-                    external=True,
-                )
+                # session.run(
+                #     sys.executable,
+                #     "tools/pipxrun.py",
+                #     PIPXRUN_REQUIREMENTS,
+                #     "-v",
+                #     "-c",
+                #     " ".join(
+                #         [
+                #             "grayskull",
+                #             "pypi",
+                #             sdist_path,
+                #             "-o",
+                #             str(d),
+                #         ]
+                #     ),
+                # )
+                path = Path(d) / PACKAGE_NAME / "meta.yaml"
+                session.log(f"cat {path}:")
+                with path.open() as f:
+                    for line in f:
+                        print(line, end="")  # noqa: T201
+
+                # # session.run(
+                # #     "cat",
+                #     str(Path(d) / PACKAGE_NAME / "meta.yaml"),
+                #     external=True,
+                # )
 
 
 @nox.session(name="conda-build", **CONDA_DEFAULT_KWS)
 @add_opts
 def conda_build(session: nox.Session, opts: SessionParams) -> None:
     """Run `conda mambabuild`."""
     runner = Installer.from_envname(
```

### Comparing `cmomy-0.8.0/changelog.d/templates/auto-changelog/template.jinja2` & `cmomy-0.9.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/config/recipe-append.yaml` & `cmomy-0.9.0/config/recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/config/userconfig.example.toml` & `cmomy-0.9.0/config/userconfig.example.toml`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/Makefile` & `cmomy-0.9.0/docs/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,10 @@
 
 livehtml:
 	$(SPHINXAUTOBUILD) "$(SOURCEDIR)" "$(BUILDDIR)/html" $(ALLSPHINXAUTOOPTS) $(O)
 
 showlinks:
 	python -m sphinx.ext.intersphinx $(BUILDDIR)/html/objects.inv
 
-release_args ?= -m "update docs" -b nist-pages
-release:
-	ghp-import -o -n $(release_args) $(BUILDDIR)/html
-
 command ?= @echo pass "command=..."
 command:
 	$(command)
```

### Comparing `cmomy-0.8.0/docs/conf.py` & `cmomy-0.9.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 """Build docs."""
+
 from __future__ import annotations
 
 import os
 import sys
 from pathlib import Path
 from typing import Any
 
@@ -40,16 +41,16 @@
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "autodocsumm",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.autosectionlabel",
-    "IPython.sphinxext.ipython_directive",
-    "IPython.sphinxext.ipython_console_highlighting",
+    # "IPython.sphinxext.ipython_directive",
+    # "IPython.sphinxext.ipython_console_highlighting",
     # "nbsphinx",
     # - easier external links
     # "sphinx.ext.extlinks",
     # - view source code on created page
     # "sphinx.ext.viewcode",
     # - view source code on github
     "sphinx.ext.linkcode",
@@ -57,19 +58,27 @@
     "sphinx_copybutton",
     # - redirect stuff?
     # "sphinxext.rediraffe",
     # - pretty things up?
     # "sphinx_design"
     # - myst stuff
     "myst_nb",
+    # "myst_parser",
+    "sphinx_autodoc_typehints",
 ]
 
 nitpicky = True
-# nitpicky_ignore_regex = [(r"py:.*", r".*")]
-nitpicky_ignore = [("py:obj", "cmomy.typing.T_Array")]
+nitpicky_ignore_regex = [
+    (r"py:.*", r".*\.T_Array.*"),
+    (r"py:.*", r"numpy\._typing.*"),
+]
+# nitpicky_ignore = [
+#     ("py:obj", "cmomy.typing.T_Array"),
+#     # ("py:class", "numpy._typing.*"),
+# ]
 autosectionlabel_prefix_document = True
 
 # -- myst stuff ---------------------------------------------------------
 myst_enable_extensions = [
     "dollarmath",
     "amsmath",
     "deflist",
@@ -148,21 +157,41 @@
 autodoc_default_flags = [
     # Make sure that any autodoc declarations show the right members
     "members",
     "inherited-members",
     "private-members",
     "show-inheritance",
 ]
+
 autodoc_typehints = "none"
+# Attempted to get type hints working.  Pain points.
+# - Need to make type hint accessible at runtime (outside TYPE_CHECKING).
+# - Either expands type aliases (sphinx_autodoc_type), or lose links to type alias (regular autodoc.  Never got it to work).
+# autodoc_typehints = "both"
+# autodoc_typehints_description_target = "documented"
+# autodoc_typehints_format = "fully-qualified"
+# autodoc_typehints = "description"
+
+# autodoc_type_aliases = {
+#     "XvalStrict": "XvalStrict",
+#     "NDArrayAny": "NDArrayAny",
+# }
+
+typehints_document_rtype = False
+typehints_use_rtype = False
+typehints_defaults = "comma"
+# always_document_param_types = True
+# typehints_use_signature = True
+
 
 # -- napoleon ------------------------------------------------------------------
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 
-napoleon_use_param = False
+# napoleon_use_param = False
 napoleon_use_rtype = False
 napoleon_preprocess_types = True
 napoleon_type_aliases = {
     # general terms
     "sequence": ":term:`sequence`",
     "iterable": ":term:`iterable`",
     "callable": ":py:func:`callable`",
@@ -213,14 +242,15 @@
     "Series": "~pandas.Series",
     "DataFrame": "~pandas.DataFrame",
     "Categorical": "~pandas.Categorical",
     "Path": "~~pathlib.Path",
     # objects with abbreviated namespace (from pandas)
     "pd.Index": "~pandas.Index",
     "pd.NaT": "~pandas.NaT",
+    # "pd.Index[Any]": "~pandas.Index"
 }
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
```

### Comparing `cmomy-0.8.0/docs/make.bat` & `cmomy-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_static/css/nist-combined.css` & `cmomy-0.9.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_static/js/leave_notice.js` & `cmomy-0.9.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_static/js/nist-header-footer.js` & `cmomy-0.9.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_templates/class-individual-pages.rst` & `cmomy-0.9.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_templates/module-custom.rst` & `cmomy-0.9.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_templates/module-single.rst` & `cmomy-0.9.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_templates/module-template.rst` & `cmomy-0.9.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_templates/autosummary/class.rst` & `cmomy-0.9.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/docs/_templates/autosummary/module.rst` & `cmomy-0.9.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/examples/archived/bootstrap.ipynb` & `cmomy-0.9.0/examples/archived/bootstrap.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9462351190476189%*

 * *Differences: {"'cells'": "{0: {'execution_count': None}, 1: {'execution_count': None}, 2: {'execution_count': "*

 * *            "None}, 3: {'execution_count': None}, 4: {'execution_count': None}, 5: "*

 * *            "{'execution_count': None, 'outputs': {0: {'execution_count': None}}}, 6: "*

 * *            "{'execution_count': None}, 7: {'execution_count': None, 'outputs': {0: "*

 * *            "{'execution_count': None}}}, 8: {'execution_count': None}, 9: {'execution_count': "*

 * *            "None}, 10: {'execution_count': None}, 11: {' […]*

```diff
@@ -1,47 +1,47 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib inline\n",
                 "import numpy as np\n",
                 "from numba import njit"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "index = np.random.choice(100, (100, 50))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@njit\n",
                 "def _random_sample_with_replacement(ndat, nrep):\n",
                 "    out = np.empty((ndat, nrep), dtype=np.int64)\n",
                 "    for i in range(ndat):\n",
                 "        for j in range(nrep):\n",
                 "            out[i, j] = np.random.randint(0, ndat)\n",
                 "    return out"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@njit\n",
                 "def _random_sample_with_replacement_freq_out(freq) -> None:\n",
                 "    nrep = freq.shape[0]\n",
                 "    ndat = freq.shape[1]\n",
@@ -126,155 +126,155 @@
                 "\n",
                 "    outputs = [p.get() for p in pools]\n",
                 "    return np.concatenate(outputs, axis=0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ndat = 100\n",
                 "nrep = ndat * 10"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator.py'>"
                         ]
                     },
-                    "execution_count": 40,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from importlib import reload\n",
                 "\n",
                 "import accumulator as acc\n",
                 "\n",
                 "reload(acc)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ndat = 300\n",
                 "nrep = ndat * 100"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator.py'>"
                         ]
                     },
-                    "execution_count": 42,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(acc)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "index, freq = acc.randsamp_numpy(ndat, nrep)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 127,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# create synthetic data\n",
                 "x = np.random.rand(10000, ndat, 1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 128,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = acc.StatsAccumVec.from_vals(x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 129,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "g = s.to_array()\n",
                 "s2 = g.resample(index)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 130,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(300, 1, 3)"
                         ]
                     },
-                    "execution_count": 130,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.data.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 132,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "out = acc.resample_data(s.data, freq, parallel=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 133,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s2.data, out)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 134,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "176 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -284,15 +284,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = acc.resample_data(s.data, freq, parallel=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 135,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "12.7 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -302,15 +302,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = acc.resample_data(s.data, freq, parallel=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 136,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "135 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -320,15 +320,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = acc.resample_data(s.data, freq, nthread=100, parallel=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 137,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "277 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -338,15 +338,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = acc.resample_data(s.data, freq, nproc=5, parallel=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 138,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from numba import prange\n",
                 "\n",
                 "\n",
                 "@njit(parallel=True)\n",
@@ -609,15 +609,15 @@
                 "                acc._push_stat(out[irep, imeta], _w * f, a, v)\n",
                 "\n",
                 "    return out"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 165,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# this seems to be the best one by far.\n",
                 "\n",
                 "\n",
                 "@njit(parallel=True)\n",
@@ -657,29 +657,29 @@
                 "                out[irep, imeta, 2] += (v - var) * alpha + (1.0 - alpha) * delta * incr\n",
                 "\n",
                 "    return out"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 168,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# out2 = np.zeros_like(out)\n",
                 "\n",
                 "\n",
                 "out2 = _resample_2b(s.data, freq)\n",
                 "\n",
                 "np.testing.assert_allclose(out, out2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 169,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "11.4 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -688,54 +688,54 @@
             ],
             "source": [
                 "%timeit -n 1 -r 1 out2 = _resample_2b(s.data, freq)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 141,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "out3 = np.zeros_like(out)\n",
                 "\n",
                 "_resample_3(s.data, freq, out3)\n",
                 "\n",
                 "np.testing.assert_allclose(out, out3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 142,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "out4 = np.zeros_like(out)\n",
                 "\n",
                 "_resample_4(s.data, freq, out4)\n",
                 "\n",
                 "np.testing.assert_allclose(out, out4)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 143,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "out4b = np.zeros_like(out)\n",
                 "\n",
                 "_resample_4b(s.data, freq, out4b)\n",
                 "\n",
                 "np.testing.assert_allclose(out, out4b)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 424,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "13.5 ms \u00b1 1.03 ms per loop (mean \u00b1 std. dev. of 3 runs, 5 loops each)\n",
@@ -763,15 +763,15 @@
                 "\n",
                 "# out2 = _resample_2d(s.data, freq)\n",
                 "# np.testing.assert_allclose(out, out2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 405,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "282 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -781,15 +781,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "_resample_2(s.data, freq)  # , out2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 231,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "126 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -799,15 +799,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "_resample_3(s.data, freq, out3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 232,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "28.3 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -817,15 +817,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "_resample_4(s.data, freq, out3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 233,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "22.7 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 5 loops each)\n"
@@ -835,15 +835,15 @@
             "source": [
                 "%%timeit -n 5 -r 1\n",
                 "_resample_4b(s.data, freq, out3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 234,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "15 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 5 loops each)\n"
@@ -853,15 +853,15 @@
             "source": [
                 "%%timeit -n 5 -r 1\n",
                 "_resample_2b(s.data, freq)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 235,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "23.7 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 5 loops each)\n"
@@ -871,15 +871,15 @@
             "source": [
                 "%%timeit -n 5 -r 1\n",
                 "_resample_2c(s.data, freq)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 236,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "22.8 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 5 loops each)\n"
@@ -889,56 +889,56 @@
             "source": [
                 "%%timeit -n 5 -r 1\n",
                 "_resample_2d(s.data, freq)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "d = np.abs(out - out2)\n",
                 "w = np.where(d > 1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(array([   62,    66,   420, ..., 29961, 29994, 29997]),\n",
                             " array([0, 0, 0, ..., 2, 2, 2]),\n",
                             " array([0, 0, 0, ..., 0, 0, 0]))"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "w"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 596,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out, out2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 567,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "451 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -955,33 +955,33 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 564,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out2, out)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 534,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out, s2.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 540,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.14 s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -991,15 +991,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "s2 = g.resample(index)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 542,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "328 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1009,15 +1009,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "g.resample_and_reduce(freq, nthread=100)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 503,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(g.resample_and_reduce(freq, nthread=100).data, s2.data)"
             ]
         },
         {
@@ -1027,15 +1027,15 @@
             "outputs": [],
             "source": [
                 "%timeit -n 1 -r 1 out = acc.resample_data(s.data, freq)#, nproc=10)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 467,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "773 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1044,18 +1044,16 @@
             ],
             "source": [
                 "%timeit -n 1 -r 1 out = acc.resample_data(s.data, freq, nthread=200)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 463,
-            "metadata": {
-                "scrolled": false
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "717 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
                     ]
@@ -1185,15 +1183,15 @@
             ],
             "source": [
                 "%timeit -n 1 -r 1 out = acc.resample_data(s.data, freq, nproc=-1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 459,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Process ForkPoolWorker-398:\n",
@@ -1324,24 +1322,24 @@
             ],
             "source": [
                 "out = acc.resample_data(s.data, freq, nproc=-1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 476,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out, s2.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 500,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.04 s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1352,15 +1350,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "# g = s.to_array()\n",
                 "s2 = g.resample(index)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 501,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "447 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1370,15 +1368,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = resample_data(s.data, freq)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 356,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "985 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1388,15 +1386,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = resample_data_thread(s.data, freq, 10)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 357,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "704 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1525,15 +1523,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out = resample_data_mult(s.data, freq, -1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 228,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "3 (100, 10, 3) (100, 10, 3)\n",
@@ -1546,29 +1544,29 @@
             "source": [
                 "%%timeit -n 3 -r 1\n",
                 "resample_data(s.data, freqTT)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 341,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "g = s.to_array()\n",
                 "s2 = g.resample(index)\n",
                 "\n",
                 "out = resample_data(s.data, freq)\n",
                 "\n",
                 "np.testing.assert_allclose(out, s2.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 423,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def resample_data_thread(data, freq, nthread):\n",
                 "    nrep = freq.shape[1]\n",
                 "    out = np.zeros((nrep,) + data.shape[1:], dtype=data.dtype)\n",
                 "\n",
@@ -1593,15 +1591,15 @@
                 "        thread.join()\n",
                 "\n",
                 "    return out"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 188,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "2.19 s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1611,15 +1609,15 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out_thread = resample_data_thread(s.data, freq, nthread=400)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 179,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# multiprocessing\n",
                 "nthread = 8\n",
                 "\n",
                 "nr = 1000\n",
@@ -1643,15 +1641,15 @@
                 "\n",
                 "    outputs = [p.get() for p in pools]\n",
                 "    return np.concatenate(outputs, axis=0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 190,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.52 s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1794,42 +1792,42 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out_mult = resample_data_mult(s.data, freq, nthread=-1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 107,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "out = np.zeros((nr,) + s.data.shape[1:], dtype=s.data.dtype)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 108,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "nthread = 2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 109,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "chunk_size = (nr + nthread - 1) // nthread"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 110,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "args_list = [\n",
                 "    (\n",
                 "        s.data,\n",
                 "        fr[:, chunk_size * i : chunk_size * (i + 1)],\n",
@@ -1837,24 +1835,24 @@
                 "    )\n",
                 "    for i in range(nthread)\n",
                 "]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 111,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(525, 10, 3)"
                         ]
                     },
-                    "execution_count": 111,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "args_list[1][2].shape"
             ]
@@ -1865,37 +1863,37 @@
             "source": [
                 "for i in range(nthread):\n",
                 "    _ = resample_data(*args_list[i])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 112,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "threads = [threading.Thread(target=resample_data, args=args) for args in args_list]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 113,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "for thread in threads:\n",
                 "    thread.start()\n",
                 "\n",
                 "for thread in threads:\n",
                 "    thread.join()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 115,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[[0., 0., 0.],\n",
                             "        [0., 0., 0.],\n",
@@ -1944,26 +1942,26 @@
                             "        [0., 0., 0.],\n",
                             "        ...,\n",
                             "        [0., 0., 0.],\n",
                             "        [0., 0., 0.],\n",
                             "        [0., 0., 0.]]])"
                         ]
                     },
-                    "execution_count": 115,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out - resample_data(data, fr)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def resample_data(data, freq, out=None):\n",
                 "    \"\"\"Reduce data along axis=0 from freq table\"\"\"\n",
                 "    data_shape = data.shape\n",
                 "    assert data_shape[-1] == 3\n",
@@ -2027,19 +2025,14 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python [conda env:py37]",
-            "language": "python",
-            "name": "conda-env-py37-py"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/examples/archived/central_moments.ipynb` & `cmomy-0.9.0/examples/archived/central_moments.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.945704257246377%*

 * *Differences: {"'cells'": "{0: {'execution_count': None}, 1: {'execution_count': None}, 2: {'execution_count': "*

 * *            "None, 'outputs': {0: {'execution_count': None}}}, 4: {'execution_count': None}, 5: "*

 * *            "{'execution_count': None}, 6: {'execution_count': None, 'outputs': {0: "*

 * *            "{'execution_count': None}}}, 7: {'execution_count': None, 'outputs': {0: "*

 * *            "{'execution_count': None}}}, 8: {'execution_count': None}, 9: {'execution_count': "*

 * *            "None, 'metadata': {replace: Ord […]*

```diff
@@ -1,41 +1,41 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from importlib import reload\n",
                 "\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'cmomy.accumulator_central' from '/Users/wpk/Documents/python/projects/cmomy/examples/cmomy/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from cmomy import accumulator, accumulator_central\n",
                 "\n",
@@ -48,28 +48,28 @@
             "metadata": {},
             "source": [
                 "# Covariance (Higher order)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "u = np.random.rand(200)\n",
                 "x = np.random.rand(200)\n",
                 "\n",
                 "nu = 5\n",
                 "nx = 10"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "test = np.zeros((nu + 1, nx + 1))\n",
                 "dx = x - x.mean()\n",
                 "du = u - u.mean()\n",
                 "\n",
@@ -85,68 +85,66 @@
                 "\n",
                 "#        np.testing.assert_allclose(out[i,j], other)\n",
                 "#         print(i, j, out[i,j]- other)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 275,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(3, 2)"
                         ]
                     },
-                    "execution_count": 275,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "accumulator_central.central_comoments(u, x, (2, 1)).shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 214,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'cmomy.accumulator_central' from '/Users/wpk/Documents/python/projects/cmomy/examples/cmomy/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 214,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 215,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac = np.zeros((nu + 1, nx + 1))\n",
                 "# datac = np.zeros((10, 2))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 216,
-            "metadata": {
-                "scrolled": true
-            },
+            "execution_count": null,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "391 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
                     ]
@@ -156,57 +154,57 @@
                 "%%timeit -n 1 -r 1\n",
                 "datac[...] = 0.0\n",
                 "accumulator_central._push_vals_cov(datac, np.ones_like(u), u, x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 217,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datac, test)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 218,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'cmomy.accumulator_central' from '/Users/wpk/Documents/python/projects/cmomy/examples/cmomy/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 218,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 219,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = accumulator_central.StatsAccumCov((nu, nx))\n",
                 "\n",
                 "s.push_vals(u, x)\n",
                 "\n",
                 "np.testing.assert_allclose(s.data, datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 220,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.15 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -217,45 +215,45 @@
                 "%%timeit -n 1 -r 1\n",
                 "s = accumulator_central.StatsAccumCov.from_vals(u, x, moments=(nu, nx))\n",
                 "np.testing.assert_allclose(s.data, datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 221,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = accumulator_central.StatsAccum.from_data(datac)\n",
                 "np.testing.assert_allclose(s.data, datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 222,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'cmomy.accumulator_central' from '/Users/wpk/Documents/python/projects/cmomy/examples/cmomy/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 222,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 223,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "711 \u00b5s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -266,39 +264,39 @@
                 "%%timeit -n 1 -r 1\n",
                 "out = accumulator_central.central_comoments(u, x, (nu, nx))\n",
                 "np.testing.assert_allclose(out, s.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 224,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "a = np.random.rand(100, 100)\n",
                 "b = np.random.rand(100)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 225,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datav = np.zeros((nu + 1, nx + 1) + a.shape[1:])\n",
                 "datav[...] = 0\n",
                 "\n",
                 "accumulator_central._push_vals_cov_vec(\n",
                 "    datav, np.ones_like(a), a, np.broadcast_to(b[:, None], a.shape)\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 237,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "5.39 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -308,24 +306,24 @@
             "source": [
                 "%%timeit -n 1 -r 1\n",
                 "out2 = accumulator_central.central_comoments(a, b, (nu, nx), out=out)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 238,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out, datav)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 226,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "5.66 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -337,100 +335,100 @@
                 "out = accumulator_central.central_comoments(a, b, (nu, nx))\n",
                 "\n",
                 "np.testing.assert_allclose(datav, out)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 227,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac[...] = 0.0\n",
                 "accumulator_central._push_vals_cov(datac, np.ones_like(b), a[:, 5], b)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 257,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'cmomy.accumulator_central' from '/Users/wpk/Documents/python/projects/cmomy/examples/cmomy/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 257,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 258,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = accumulator_central.StatsAccumCovVec((nu, nx), shape=a.shape[1:])\n",
                 "s.push_vals(a, b, broadcast=True)\n",
                 "\n",
                 "np.testing.assert_allclose(s.data, datav)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 263,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "a = s.reduce(0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 264,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "b = accumulator_central.StatsAccumCov.from_datas(s.data, axis=2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 269,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]])"
                         ]
                     },
-                    "execution_count": 269,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a.data[..., 0] - b.data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 231,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "43 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -443,116 +441,116 @@
                 "    a, b, moments=(nu, nx), broadcast=True\n",
                 ")\n",
                 "np.testing.assert_allclose(s.data, datav)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 114,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s0 = s.zeros_like()\n",
                 "s1 = s.zeros_like()\n",
                 "\n",
                 "s0.push_vals(a[:20], b[:20], broadcast=True)\n",
                 "s1.push_vals(a[20:], b[20:], broadcast=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 115,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose((s0 + s1).data, s.data)\n",
                 "np.testing.assert_allclose((s - s1).data, s0.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 116,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s0 += s1\n",
                 "np.testing.assert_allclose(s0.data, s.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 117,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s0 -= s1\n",
                 "np.testing.assert_allclose(s0.data, (s - s1).data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 118,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose((s0 + s1).data, s.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 119,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "xx = np.random.rand(2, 3, 4, 5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 135,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(0.38953692)"
                         ]
                     },
-                    "execution_count": 135,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.squeeze(np.random.rand(10).mean(0, keepdims=True), 0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 129,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(1, 3, 4, 5)"
                         ]
                     },
-                    "execution_count": 129,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.expand_dims(np.randomxx.mean(0), 0).shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 132,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "ValueError",
                     "evalue": "cannot select an axis to squeeze out which has size not equal to one",
                     "output_type": "error",
                     "traceback": [
@@ -567,35 +565,35 @@
             ],
             "source": [
                 "np.squeeze(xx.mean(0, keepdims=True), 1).shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 124,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(2, 1, 1, 3, 4, 5)"
                         ]
                     },
-                    "execution_count": 124,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.expand_dims(xx, axis=[1, 2]).shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "662 \u00b5s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -606,44 +604,44 @@
                 "%%timeit -n 1 -r 1\n",
                 "datac[...] = 0.0\n",
                 "accumulator_central._central_cov_from_vals(datac, np.ones_like(u), u, x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datac, test)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 505,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datac, out)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 478,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "uu = np.random.rand(10000)\n",
                 "xx = np.random.rand(10000)\n",
                 "ww = np.ones_like(uu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 487,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "37.7 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -654,24 +652,24 @@
                 "%%timeit -n 1 -r 1\n",
                 "datac[...] = 0.0\n",
                 "accumulator_central._push_vals_cov(datac, ww, uu, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 489,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac2 = np.zeros_like(datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 490,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "7.55 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -682,15 +680,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "datac2[...] = 0.0\n",
                 "accumulator_central._central_cov_from_vals(datac2, ww, uu, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 492,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 0.00000000e+00,  2.55351296e-15, -2.63677968e-16,\n",
                             "         1.30104261e-18,  6.07153217e-17,  5.96311195e-19,\n",
@@ -714,26 +712,26 @@
                             "         5.84982129e-21, -8.23739541e-20],\n",
                             "       [ 3.15350366e-18, -4.57397792e-19, -5.25160427e-20,\n",
                             "        -4.06575815e-20, -7.07272511e-20, -1.09584888e-20,\n",
                             "        -1.56701095e-20,  1.59811294e-21, -1.70730078e-21,\n",
                             "         8.09396229e-22, -5.91020548e-22]])"
                         ]
                     },
-                    "execution_count": 492,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac - datac2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 485,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[-1.00000000e+04, -5.05747358e-01, -8.37505842e-02,\n",
                             "         5.62929357e-04, -1.26190181e-02,  1.83256401e-04,\n",
@@ -757,26 +755,26 @@
                             "         1.70754654e-07, -1.06663030e-06],\n",
                             "       [ 6.42003657e-06, -2.75857438e-05, -1.27221622e-05,\n",
                             "        -2.28794850e-06, -2.00741145e-06, -2.25593397e-07,\n",
                             "        -2.71200798e-07, -2.21896935e-08, -2.98333818e-08,\n",
                             "        -2.13102575e-09, -1.25480086e-09]])"
                         ]
                     },
-                    "execution_count": 485,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac - datac2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 476,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datac, out)"
             ]
         },
         {
@@ -788,15 +786,15 @@
                 "accumulator_central._push_vals_cov(datac, w, u, x)\n",
                 "\n",
                 "s = accumulator_central.StatsAccum.from_vals(x, W=w, nmom=nx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 405,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac0 = np.zeros_like(datac)\n",
                 "datac1 = np.zeros_like(datac)\n",
                 "datacS = np.zeros_like(datac)\n",
                 "\n",
@@ -807,346 +805,346 @@
                 "uu = u[20:]\n",
                 "xx = x[20:]\n",
                 "accumulator_central._push_vals_cov(datac1, np.ones_like(uu), uu, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 411,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datacS[...] = 0.0\n",
                 "accumulator_central._push_datas_cov(datacS, np.array([datac0, datac1]))\n",
                 "\n",
                 "np.testing.assert_allclose(datac, datacS)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 442,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'python_dropin_files.accumulator_central' from '../python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 442,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 443,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "A = np.stack([d[((1, 0), (0, 1))] for d in (datac0, datac1)], axis=0)\n",
                 "V = np.stack([d[1:, 1:] for d in (datac0, datac1)], axis=0)\n",
                 "W = np.array([d[0, 0] for d in [datac0, datac1]])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 444,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datacS[...] = 0.0\n",
                 "# accumulator_central._push_stats_cov(datacS, W, A, V)\n",
                 "accumulator_central._push_stat_cov(datacS, W[0], A[0], V[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 445,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([2.00000000e+01, 4.94065278e-01, 5.49867192e-06, 2.17657183e-06,\n",
                             "       1.16134927e-06, 5.07345753e-07])"
                         ]
                     },
-                    "execution_count": 445,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datacS[:, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 446,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([2.00000000e+01, 4.94065278e-01, 7.06087533e-02, 1.22993455e-04,\n",
                             "       1.12885602e-02, 1.48249169e-04])"
                         ]
                     },
-                    "execution_count": 446,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac0[:, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 379,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = accumulator_central.StatsAccum.from_datas(\n",
                 "    np.array([datac0[:, 0], datac1[:, 0]]), nmom=5\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 380,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([2.00000000e+03, 4.95026001e-01, 8.54259965e-02, 3.56203719e-04,\n",
                             "       1.29406646e-02, 1.85527035e-04])"
                         ]
                     },
-                    "execution_count": 380,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 337,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([2.00000000e+03, 4.95026001e-01, 8.54259965e-02, 3.56203719e-04,\n",
                             "       1.29406646e-02, 1.85527035e-04])"
                         ]
                     },
-                    "execution_count": 337,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[:, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 325,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 2.00000000e+03,  4.95026001e-01,  8.08198334e-06, -2.81530667e-07,\n",
                             "        1.22397665e-06, -4.23898766e-08])"
                         ]
                     },
-                    "execution_count": 325,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datacS[:, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 326,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([2.00000000e+03, 4.95026001e-01, 8.54259965e-02, 3.56203719e-04,\n",
                             "       1.29406646e-02, 1.85527035e-04])"
                         ]
                     },
-                    "execution_count": 326,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[:, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 319,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.49502600082312737"
                         ]
                     },
-                    "execution_count": 319,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datacS[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 316,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.49502600082312714"
                         ]
                     },
-                    "execution_count": 316,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 311,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.49503571, 0.50762568])"
                         ]
                     },
-                    "execution_count": 311,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "A[1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 312,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.49503571, 0.50762568])"
                         ]
                     },
-                    "execution_count": 312,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac1[((1, 0), (0, 1))]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 306,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.496796674548943"
                         ]
                     },
-                    "execution_count": 306,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "A[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 305,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.502211174994026"
                         ]
                     },
-                    "execution_count": 305,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datacS[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 304,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.5075173854302096"
                         ]
                     },
-                    "execution_count": 304,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 290,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 2.00000000e+00,  5.02211175e-01,  1.01080639e-04,\n",
                             "        -5.37992674e-05,  2.37286854e-05, -1.17291465e-05,\n",
@@ -1170,317 +1168,317 @@
                             "        -1.40998456e-06,  1.25809836e-06],\n",
                             "       [ 2.29778914e-07, -1.99357882e-04,  7.53104421e-05,\n",
                             "        -5.34670394e-05,  2.37327466e-05, -1.16534261e-05,\n",
                             "         5.55617776e-06, -2.52455227e-06,  1.22475892e-06,\n",
                             "        -5.47583774e-07,  2.65288225e-07]])"
                         ]
                     },
-                    "execution_count": 290,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datacS"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 219,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.49502600082312714, 0.49502600082312714)"
                         ]
                     },
-                    "execution_count": 219,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[1, 0], out[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 220,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.5075173854302097, 0.5075173854302096)"
                         ]
                     },
-                    "execution_count": 220,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[0, 1], out[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 201,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datac, out)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 243,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac[...] = 0.0\n",
                 "for uu, xx in zip(u, x):\n",
                 "    accumulator_central._push_stat_cov(\n",
                 "        datac, 1.0, np.array([uu, xx]), np.zeros((nu - 1, nx - 1))\n",
                 "    )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 249,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out, datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 247,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out[:4, :4], datac[:4, :4])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 224,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.00018849835769094766"
                         ]
                     },
-                    "execution_count": 224,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 225,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0001884983576909486"
                         ]
                     },
-                    "execution_count": 225,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 221,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.08542599652601496"
                         ]
                     },
-                    "execution_count": 221,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 223,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.08542599652601496"
                         ]
                     },
-                    "execution_count": 223,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 165,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac = np.zeros((nu + 1, nx + 1))\n",
                 "for uu, vv in zip(u, x):\n",
                 "    # accumulator_central._get_moments(datac, 1.0, uu, vv)\n",
                 "    accumulator_central._push_val_cov(datac, 1.0, uu, vv)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 124,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.5075173854302097"
                         ]
                     },
-                    "execution_count": 124,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 125,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.49502600082312714"
                         ]
                     },
-                    "execution_count": 125,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 126,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0044924415019052906"
                         ]
                     },
-                    "execution_count": 126,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[1, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 127,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.004492441501905286, 0.0044924415019052906)"
                         ]
                     },
-                    "execution_count": 127,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[1, 1], datac[1, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 114,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.49502600082312714"
                         ]
                     },
-                    "execution_count": 114,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 128,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(out, datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "a0 = 3\n",
                 "a1 = 5"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 67,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "other 0 0 0 3 5\n",
@@ -1526,35 +1524,35 @@
                 "        else:\n",
                 "            print(\"other\", i, b0, b1, c0, c1)\n",
                 "            i += 1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 99,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "6"
                         ]
                     },
-                    "execution_count": 99,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a1 + 1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 94,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "6\n",
@@ -1606,65 +1604,65 @@
                 "        else:\n",
                 "            print(\"other\", i, b0, b1, c0, c1)\n",
                 "            i += 1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x0, x1 = np.random.rand(2)\n",
                 "alpha = np.random.rand()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[0]"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "list(range(0 + 1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[]"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "list(range(-1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 70,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "alpha_0 = 1.0\n",
                 "minus_0 = 1.0\n",
                 "for b0 in range(a0 + 1):\n",
                 "    c0 = a0 - b0\n",
@@ -1679,184 +1677,184 @@
                 "\n",
                 "    alpha_0 *= alpha\n",
                 "    minus_0 *= -1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 77,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.08609356345020769, 0.08609356345020767)"
                         ]
                     },
-                    "execution_count": 77,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha_0, alpha ** (a0 + 1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 85,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.004014986031001154, 0.004014986031001153)"
                         ]
                     },
-                    "execution_count": 85,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha_bb, alpha ** (a0 + a1 + 1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.29341704696593157, 0.29341704696593157)"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha_0, alpha ** (a0 - 1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.046635147508131955, 0.04663514750813196)"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha ** (a0 + a1 - 3), alpha_bb"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(-1, -1.0)"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "(-1) ** (a0 + a1 - 3), minus_bb"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 969,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.3405555290380999"
                         ]
                     },
-                    "execution_count": 969,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha ** (a0 - 1 + a1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 963,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.58357135728041"
                         ]
                     },
-                    "execution_count": 963,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha ** (a0 + a1 - 4)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 952,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.2845897526522902"
                         ]
                     },
-                    "execution_count": 952,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha ** (a0 + a1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 953,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.23782120802282072"
                         ]
                     },
-                    "execution_count": 953,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha_bb * alpha_0 * alpha**2"
             ]
@@ -1866,64 +1864,64 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 918,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "range(0, 1)"
                         ]
                     },
-                    "execution_count": 918,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "range(1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 919,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.8539514687136144"
                         ]
                     },
-                    "execution_count": 919,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 920,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.8539514687136144"
                         ]
                     },
-                    "execution_count": 920,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "alpha_bb"
             ]
@@ -1933,15 +1931,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "AssertionError",
                     "evalue": "\nNot equal to tolerance rtol=1e-07, atol=0\n\nMismatched elements: 66 / 66 (100%)\nMax absolute difference: 1999.\nMax relative difference: 1999.\n x: array([[ 2.000000e+03,  5.075174e-01,  8.409365e-02, -8.856088e-04,\n         1.272233e-02, -2.829138e-04,  2.294010e-03, -7.759181e-05,\n         4.507539e-04, -2.041362e-05,  9.321942e-05],...\n y: array([[1.      , 0.141149, 0.      , 0.      , 0.      , 0.      ,\n        0.      , 0.      , 0.      , 0.      , 0.      ],\n       [0.597173, 0.      , 0.      , 0.      , 0.      , 0.      ,...",
                     "output_type": "error",
                     "traceback": [
@@ -1956,393 +1954,393 @@
             ],
             "source": [
                 "np.testing.assert_allclose(out, datac)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 862,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.00023076759905562492"
                         ]
                     },
-                    "execution_count": 862,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[1, 2]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 863,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.00023076759905562444"
                         ]
                     },
-                    "execution_count": 863,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[1, 2]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 845,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0033627321356257604"
                         ]
                     },
-                    "execution_count": 845,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 837,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0"
                         ]
                     },
-                    "execution_count": 837,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 0] - datac[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 834,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.08446688770432603"
                         ]
                     },
-                    "execution_count": 834,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 824,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.00012665210827644818"
                         ]
                     },
-                    "execution_count": 824,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 825,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0033627321356257604"
                         ]
                     },
-                    "execution_count": 825,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 801,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.08446688770432603"
                         ]
                     },
-                    "execution_count": 801,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 802,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "6.817508765979018e-07"
                         ]
                     },
-                    "execution_count": 802,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 796,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.08446620595344943"
                         ]
                     },
-                    "execution_count": 796,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 0] - datac[2, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 794,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0"
                         ]
                     },
-                    "execution_count": 794,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[0, 1] - datac[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 783,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "-1.726181513778298e-05"
                         ]
                     },
-                    "execution_count": 783,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 2] - out[2, 2]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 773,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.5030104742189434"
                         ]
                     },
-                    "execution_count": 773,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 774,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.5030104742189434"
                         ]
                     },
-                    "execution_count": 774,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[1, 0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 775,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.5044784891474983"
                         ]
                     },
-                    "execution_count": 775,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[0, 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 776,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.007103773039984232"
                         ]
                     },
-                    "execution_count": 776,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datac[2, 2]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 777,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.007121034855122015"
                         ]
                     },
-                    "execution_count": 777,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out[2, 2]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 778,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.5044784891474983"
                         ]
                     },
-                    "execution_count": 778,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 751,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(6, 11)"
                         ]
                     },
-                    "execution_count": 751,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 743,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from importlib import reload\n",
                 "\n",
                 "reload(accumulator_central)\n",
                 "\n",
@@ -2351,44 +2349,44 @@
                 "accumulator_central._push_vals(data, np.ones_like(u), u)\n",
                 "# for uu in u:\n",
                 "#     accumulator_central._push_val_nmom(data, 1.0, uu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 719,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator_central' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 719,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 720,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(data, test[:, 0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 721,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data0 = np.zeros(s)\n",
                 "for uu in u[:4]:\n",
                 "    accumulator_central._push_val(data0, 1.0, uu)\n",
                 "\n",
@@ -2399,85 +2397,85 @@
                 "data2 = np.zeros(s)\n",
                 "for uu in u[10:]:\n",
                 "    accumulator_central._push_val(data2, 1.0, uu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 722,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datac = np.zeros(s)\n",
                 "\n",
                 "for d in [data0, data1, data2]:\n",
                 "    accumulator_central._push_stat(datac, w=d[0], a=d[1], v=d[2:])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 723,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datac, test[:, 0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 724,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator_central' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 724,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 725,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = accumulator_central.StatsAccum(nmom=nu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 726,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator_central' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 726,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 727,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "222 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2488,15 +2486,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "s = accumulator_central.StatsAccum.from_vals(u, nmom=nu)\n",
                 "np.testing.assert_allclose(s.data, data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 728,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "262 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2507,320 +2505,320 @@
                 "%%timeit -n 1 -r 1\n",
                 "s = accumulator_central.StatsAccum.from_datas(np.stack([data0, data1, data2]), nmom=nu)\n",
                 "np.testing.assert_allclose(s.data, data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 729,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = accumulator_central.StatsAccum.from_datas(np.stack([data0, data1, data2]), nmom=nu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 730,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# adding"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 731,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator_central' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 731,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 732,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "a = len(u) // 3\n",
                 "b = 2 * a"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 704,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "su = accumulator_central.StatsAccum.from_vals(u, nmom=nu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 705,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s0 = accumulator_central.StatsAccum.from_vals(u[:a], nmom=nu)\n",
                 "s1 = accumulator_central.StatsAccum.from_vals(u[a:b], nmom=nu)\n",
                 "s2 = accumulator_central.StatsAccum.from_vals(u[b:], nmom=nu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 706,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "new = s0.copy()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 707,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "new.push_stat(w=s1.weight(), a=s1.mean(), v=s1.cmom())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 708,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 2.00000000e+03,  5.03010474e-01,  8.44668877e-02, -4.41663483e-04,\n",
                             "        1.26805092e-02, -1.52001435e-04])"
                         ]
                     },
-                    "execution_count": 708,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "(s0 + s1 + s2).data - data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 709,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 0.00000000e+00, -2.22044605e-16,  2.49800181e-16, -7.04731412e-18,\n",
                             "       -1.23165367e-16,  3.87602277e-18])"
                         ]
                     },
-                    "execution_count": 709,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "(su - s1 - s2).data - s0.data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 710,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# vector\n",
                 "su = accumulator_central.StatsAccum.from_vals(u, nmom=nu)\n",
                 "sx = accumulator_central.StatsAccum.from_vals(x, nmom=nu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 711,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "y = np.stack([u, x], -1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 712,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sv = accumulator_central.StatsAccumVec.from_vals(np.stack([u, x], -1), nmom=nu)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 523,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0., 0., 0., 0., 0., 0.])"
                         ]
                     },
-                    "execution_count": 523,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sv.data[:, 0] - su.data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 524,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0., 0., 0., 0., 0., 0.])"
                         ]
                     },
-                    "execution_count": 524,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sv.data[:, 1] - sx.data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 525,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 526,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "a = xr.DataArray(np.random.rand(5, 4), dims=[\"b\", \"a\"])\n",
                 "b = xr.DataArray(np.random.rand(4, 5, 6), dims=[\"a\", \"b\", \"c\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 562,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# playing with sizes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "reload(accumulator_central)\n",
                 "reload(accumulator)\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 121,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "nmom = 10\n",
                 "nv = 500"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 122,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "v = np.random.rand(10000, nv)\n",
                 "wv = np.ones_like(v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 123,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "y = np.array(v[:, 0], order=\"c\")\n",
                 "wy = np.ones_like(y)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 124,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data = np.zeros(nmom + 1)\n",
                 "datav = np.zeros((nmom + 1, nv))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 125,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datavc = np.zeros_like(datav)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 126,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'cmomy.accumulator_central' from '/Users/wpk/Documents/python/projects/cmomy/examples/cmomy/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 126,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 127,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.12 s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2831,15 +2829,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "datavc[...] = 0\n",
                 "accumulator_central._central_from_vals_vec(datavc, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 129,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "478 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2850,15 +2848,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav[...] = 0.0\n",
                 "accumulator_central._push_vals_vec(datav, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 112,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "56 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2869,24 +2867,24 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav[...] = 0.0\n",
                 "accumulator_central._push_vals_vec(datav, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 130,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datavc, datav)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 62,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 1.00000000e+03,  1.00000000e+03,  1.00000000e+03, ...,\n",
                             "         1.00000000e+03,  1.00000000e+03,  1.00000000e+03],\n",
@@ -2898,26 +2896,26 @@
                             "        -7.36768704e-04,  1.23353312e-03, -1.34180469e-03],\n",
                             "       [ 1.26651253e-02,  1.25223108e-02,  1.20719801e-02, ...,\n",
                             "         1.16175679e-02,  1.31191423e-02,  1.22497030e-02],\n",
                             "       [-3.77844935e-05, -3.34987237e-05, -5.47515372e-04, ...,\n",
                             "        -2.66155829e-04,  4.35729829e-04, -3.81241119e-04]])"
                         ]
                     },
-                    "execution_count": 62,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 63,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datav2 = np.zeros((nv, nmom + 1))"
             ]
         },
         {
@@ -2925,15 +2923,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 64,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "256 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2944,24 +2942,24 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav2[...] = 0.0\n",
                 "accumulator._push_vals_vec(datav2, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 65,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(datav[:3, ...], datav2.T[:3, ...])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 66,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "187 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -2972,15 +2970,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav2[...] = 0.0\n",
                 "accumulator_central._push_vals_vec(datav, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 73,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "26.9 \u00b5s \u00b1 726 ns per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n"
@@ -2991,24 +2989,24 @@
                 "%%timeit -n 10 -r 3\n",
                 "data[...] = 0.0\n",
                 "accumulator_central._push_vals(data, wy, y)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 70,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data2 = np.zeros_like(data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 74,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "177 \u00b5s \u00b1 31.6 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n"
@@ -3019,55 +3017,55 @@
                 "%%timeit -n 10 -r 3\n",
                 "data2[...] = 0.0\n",
                 "accumulator_central._central_from_vals(data2, wy, y)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(data, data2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(\n",
                 "    data, accumulator_central.StatsAccum.from_vals(y, nmom=nmom).data\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator_central' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 46,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "7.94 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -3078,55 +3076,55 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav[...] = 0.0\n",
                 "accumulator_central._push_vals_vec(datav, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 65,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(11, 100)"
                         ]
                     },
-                    "execution_count": 65,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 63,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(100,)"
                         ]
                     },
-                    "execution_count": 63,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "v[0, :].shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 69,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1000., 1000., 1000., 1000., 1000., 1000., 1000., 1000., 1000.,\n",
                             "       1000., 1000.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,\n",
@@ -3138,26 +3136,26 @@
                             "          0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,\n",
                             "          0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,\n",
                             "          0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,\n",
                             "          0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,    0.,\n",
                             "          0.])"
                         ]
                     },
-                    "execution_count": 69,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav[0, :]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 50,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 1.00000000e+03,  1.00000000e+03,  1.00000000e+03, ...,\n",
                             "         0.00000000e+00,  0.00000000e+00,  0.00000000e+00],\n",
@@ -3170,15 +3168,15 @@
                             "         0.00000000e+00,  0.00000000e+00,  0.00000000e+00],\n",
                             "       [ 5.30306436e-05, -3.03834063e-05, -4.67353197e-05, ...,\n",
                             "         0.00000000e+00,  0.00000000e+00,  0.00000000e+00],\n",
                             "       [ 1.04660234e-04,  9.29903994e-05,  8.49490620e-05, ...,\n",
                             "         0.00000000e+00,  0.00000000e+00,  0.00000000e+00]])"
                         ]
                     },
-                    "execution_count": 50,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "accumulator_central.StatsAccumVec.from_vals(v, nmom=nmom).data"
             ]
@@ -3190,15 +3188,15 @@
             "outputs": [],
             "source": [
                 "acc"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "AssertionError",
                     "evalue": "\nNot equal to tolerance rtol=1e-07, atol=0\n\n(shapes (11, 100), (100, 11) mismatch)\n x: array([[ 1.000000e+03,  1.000000e+03,  1.000000e+03, ...,  0.000000e+00,\n         0.000000e+00,  0.000000e+00],\n       [ 4.844688e-01,  5.099917e-01,  5.175260e-01, ...,  0.000000e+00,...\n y: array([[1000., 1000., 1000., ..., 1000., 1000., 1000.],\n       [   0.,    0.,    0., ...,    0.,    0.,    0.],\n       [   0.,    0.,    0., ...,    0.,    0.,    0.],...",
                     "output_type": "error",
                     "traceback": [
@@ -3215,24 +3213,24 @@
                 "np.testing.assert_allclose(\n",
                 "    datav, accumulator_central.StatsAccumVec.from_vals(v, nmom=nmom).data\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1010,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datav2 = np.zeros((nmom + 1, nv))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1011,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "498 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -3243,15 +3241,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav2[...] = 0.0\n",
                 "accumulator_central._push_vals_vec_nmom2(datav2, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1012,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "356 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -3262,41 +3260,41 @@
                 "%%timeit -n 1 -r 1\n",
                 "datav2[...] = 0.0\n",
                 "accumulator_central._vec_push_vals_nmom(datav2, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 973,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0., 0., 0.],\n",
                             "       [0., 0., 0.],\n",
                             "       [0., 0., 0.],\n",
                             "       ...,\n",
                             "       [0., 0., 0.],\n",
                             "       [0., 0., 0.],\n",
                             "       [0., 0., 0.]])"
                         ]
                     },
-                    "execution_count": 973,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav2.T - datav"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 913,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1.00000000e+03, 5.00754809e-01, 8.48214609e-02],\n",
                             "       [1.00000000e+03, 4.96995540e-01, 8.23855192e-02],\n",
@@ -3306,26 +3304,26 @@
                             "       [0.00000000e+00, 0.00000000e+00, 0.00000000e+00],\n",
                             "       [0.00000000e+00, 0.00000000e+00, 0.00000000e+00],\n",
                             "       [0.00000000e+00, 0.00000000e+00, 0.00000000e+00],\n",
                             "       [0.00000000e+00, 0.00000000e+00, 0.00000000e+00],\n",
                             "       [0.00000000e+00, 0.00000000e+00, 0.00000000e+00]])"
                         ]
                     },
-                    "execution_count": 913,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav2.T"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 910,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0.00000000e+00, 0.00000000e+00, 0.00000000e+00],\n",
                             "       [0.00000000e+00, 0.00000000e+00, 0.00000000e+00],\n",
@@ -3335,34 +3333,34 @@
                             "       [1.00000000e+03, 4.98194914e-01, 8.53425835e-02],\n",
                             "       [1.00000000e+03, 4.98087142e-01, 8.34877660e-02],\n",
                             "       [1.00000000e+03, 5.03279532e-01, 8.14883356e-02],\n",
                             "       [1.00000000e+03, 4.92091896e-01, 8.33388170e-02],\n",
                             "       [1.00000000e+03, 4.99164371e-01, 8.30120104e-02]])"
                         ]
                     },
-                    "execution_count": 910,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 890,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "wys = wy.reshape(-1, 1)\n",
                 "ys = y.reshape(-1, 1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 892,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.78 ms \u00b1 23.9 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n"
@@ -3373,66 +3371,66 @@
                 "%%timeit -n 10 -r 3\n",
                 "data2[...] = 0.0\n",
                 "accumulator_central._vec_push_vals_nmom(data2, wys, ys)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 880,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.00000000e+03, 4.82649028e-01, 8.48409676e-02])"
                         ]
                     },
-                    "execution_count": 880,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 881,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1.00000000e+03],\n",
                             "       [4.82649028e-01],\n",
                             "       [8.48409676e-02]])"
                         ]
                     },
-                    "execution_count": 881,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 855,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "datav2[...] = 0.0"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 858,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.24 ms \u00b1 9.9 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n"
@@ -3443,15 +3441,15 @@
                 "%%timeit -n 10 -r 3\n",
                 "datav2[...] = 0.0\n",
                 "accumulator_central._vec_push_vals_nmom(datav2, wv, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 833,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1.00000000e+03, 4.88233093e-01, 8.16752775e-02],\n",
                             "       [1.00000000e+03, 4.91592016e-01, 8.12709749e-02],\n",
@@ -3461,26 +3459,26 @@
                             "       [1.00000000e+03, 5.10687036e-01, 8.62974788e-02],\n",
                             "       [1.00000000e+03, 5.01327530e-01, 8.26025968e-02],\n",
                             "       [1.00000000e+03, 4.96930042e-01, 8.37995733e-02],\n",
                             "       [1.00000000e+03, 4.87614174e-01, 8.49292351e-02],\n",
                             "       [1.00000000e+03, 4.92219122e-01, 8.42484274e-02]])"
                         ]
                     },
-                    "execution_count": 833,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav - datav2.T"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 768,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1.00000000e+03, 4.88233093e-01, 8.16752775e-02],\n",
                             "       [1.00000000e+03, 4.91592016e-01, 8.12709749e-02],\n",
@@ -3490,15 +3488,15 @@
                             "       [1.00000000e+03, 5.10687036e-01, 8.62974788e-02],\n",
                             "       [1.00000000e+03, 5.01327530e-01, 8.26025968e-02],\n",
                             "       [1.00000000e+03, 4.96930042e-01, 8.37995733e-02],\n",
                             "       [1.00000000e+03, 4.87614174e-01, 8.49292351e-02],\n",
                             "       [1.00000000e+03, 4.92219122e-01, 8.42484274e-02]])"
                         ]
                     },
-                    "execution_count": 768,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav2.T"
             ]
@@ -3510,44 +3508,44 @@
             "outputs": [],
             "source": [
                 "accum"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 666,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data2 = np.zeros((nu + 1, 1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 693,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'python_dropin_files.accumulator_central' from '../python_dropin_files/accumulator_central.py'>"
                         ]
                     },
-                    "execution_count": 693,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 694,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "LoweringError",
                     "evalue": "Failed in nopython mode pipeline (step: nopython mode backend)\n\u001b[1m\u001b[1m\n\u001b[1m\nFile \"accumulator_central.py\", line 78:\u001b[0m\n\u001b[1mdef _push_vals_nmom(data, W, X, bfac):\n    <source elided>\n\n\u001b[1m@myjit\n\u001b[0m\u001b[1m^\u001b[0m\u001b[0m\n\u001b[0m\n\u001b[0m\u001b[1m[1] During: lowering \"$202binary_add.16.6153 = arrayexpr(expr=(<built-in function add>, [(<built-in function mul>, [(<built-in function mul>, [Var(_178binary_power_4_6141, accumulator_central.py:77), (<built-in function pow>, [Var(alpha_6079, accumulator_central.py:59), Var(b.6128, accumulator_central.py:71)])]), Var(one_alpha.6083, accumulator_central.py:60)]), (<built-in function mul>, [(<built-in function pow>, [Var(one_alpha.6083, accumulator_central.py:60), Var(b.6128, accumulator_central.py:71)]), Var(alpha.6079, accumulator_central.py:59)])]), ty=array(float64, 1d, C))\" at ../python_dropin_files/accumulator_central.py (78)\u001b[0m",
                     "output_type": "error",
                     "traceback": [
@@ -3601,53 +3599,53 @@
                 "# for yy in y:\n",
                 "#     accumulator_central._push_val_gen(data2, np.array([1.0]), np.array([yy]))\n",
                 "accumulator_central._push_vals_gen(data2, wy[:, None], y[:, None])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 689,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.])"
                         ]
                     },
-                    "execution_count": 689,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "wy[:, None][0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 690,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "accumulator_central._push_val_gen(data2, wy[:, None][0], y[:, None][0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 669,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data3 = np.zeros(3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 670,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "23.4 \u00b5s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -3658,44 +3656,44 @@
                 "%%timeit -n 1 -r 1\n",
                 "data3[...] = 0.0\n",
                 "accumulator._push_vals(data3, wy, y)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 671,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0., 0., 0.])"
                         ]
                     },
-                    "execution_count": 671,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data3 - data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 672,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data3v = np.zeros((3, 10))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 686,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.25 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -3706,35 +3704,35 @@
                 "%%timeit -n 1 -r 1\n",
                 "data3v[...] = 0.0\n",
                 "accumulator._push_vals(data3v, wy, v)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 677,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(10, 3)"
                         ]
                     },
-                    "execution_count": 677,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "datav.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 683,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1.00000000e+03, 4.93164127e-01, 8.57376084e-02],\n",
                             "       [1.00000000e+03, 4.94909316e-01, 8.26797779e-02],\n",
@@ -3744,56 +3742,56 @@
                             "       [1.00000000e+03, 4.95981720e-01, 8.14779074e-02],\n",
                             "       [1.00000000e+03, 4.82537471e-01, 8.67320718e-02],\n",
                             "       [1.00000000e+03, 5.02259324e-01, 8.18378637e-02],\n",
                             "       [1.00000000e+03, 4.88356759e-01, 8.42744313e-02],\n",
                             "       [1.00000000e+03, 5.04622471e-01, 8.67121726e-02]])"
                         ]
                     },
-                    "execution_count": 683,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data3v.T"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 639,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.00000000e+03, 4.93164127e-01, 8.57376084e-02])"
                         ]
                     },
-                    "execution_count": 639,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data3"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 640,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.00000000e+03, 4.93164127e-01, 8.57376084e-02, 1.09946962e-03,\n",
                             "       1.30475164e-02, 3.75993519e-04])"
                         ]
                     },
-                    "execution_count": 640,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data"
             ]
@@ -3823,131 +3821,131 @@
             "outputs": [],
             "source": [
                 "for"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 609,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.])"
                         ]
                     },
-                    "execution_count": 609,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "wy[:, None][0, ...]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 592,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 0.00000000e+00,  0.00000000e+00,  8.56934143e-02, -1.30104261e-18,\n",
                             "        1.73472348e-18,  2.16840434e-19])"
                         ]
                     },
-                    "execution_count": 592,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data2[:, 0] - data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 577,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.])"
                         ]
                     },
-                    "execution_count": 577,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "wy[:, None][0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 572,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1.00000000e+03],\n",
                             "       [4.93164127e-01],\n",
                             "       [8.57376084e-02],\n",
                             "       [1.09946962e-03],\n",
                             "       [1.30475164e-02],\n",
                             "       [3.75993519e-04]])"
                         ]
                     },
-                    "execution_count": 572,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 573,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.00000000e+03, 4.93164127e-01, 4.41940640e-05, 1.09946962e-03,\n",
                             "       1.30475164e-02, 3.75993519e-04])"
                         ]
                     },
-                    "execution_count": 573,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 556,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "tmp, a = accumulator_central._push_val_gen(data2, 1.0, np.array(yy))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 561,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data[a, ...] = tmp"
             ]
         },
         {
@@ -3968,15 +3966,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 423,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0.],\n",
@@ -3986,30 +3984,25 @@
                             "       [0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0., 0., 0.]])"
                         ]
                     },
-                    "execution_count": 423,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "accumulator_central.StatsAccumVec.from_vals(v, nmom=nu).data - datav"
             ]
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python [conda env:.conda-py37]",
-            "language": "python",
-            "name": "conda-env-.conda-py37-py"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/examples/archived/example_usage.ipynb` & `cmomy-0.9.0/examples/archived/example_usage.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.947265625%*

 * *Differences: {"'cells'": "{1: {'execution_count': None}, 2: {'execution_count': None}, 3: {'execution_count': "*

 * *            "None}, 4: {'execution_count': None}, 5: {'execution_count': None}, 6: "*

 * *            "{'execution_count': None}, 8: {'execution_count': None}, 9: {'execution_count': "*

 * *            "None}, 10: {'execution_count': None}, 11: {'execution_count': None}, 12: "*

 * *            "{'execution_count': None}, 13: {'execution_count': None}, 14: {'execution_count': "*

 * *            "None}, 15: {'execution_count': None […]*

```diff
@@ -5,27 +5,27 @@
             "metadata": {},
             "source": [
                 "# Central moments"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipy.stats\n",
                 "\n",
                 "import cmomy"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# setup some test data\n",
                 "x = np.random.rand(100)\n",
                 "\n",
                 "# number of moments\n",
@@ -36,33 +36,33 @@
                 "# cen_mom = ((x - x.mean())[:, None] ** np.arange(mom+1)).mean(0)\n",
                 "# prefer scipy.stats.moments as treats mom=1 correctly\n",
                 "cen_mom = scipy.stats.moment(x, moment=np.arange(mom + 1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(10000)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = x.sum()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "221 \u00b5s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -71,15 +71,15 @@
             ],
             "source": [
                 "%timeit -n 1 -r 1 np.testing.assert_allclose(s, x.sum())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# using cmomy\n",
                 "s = cmomy.CentralMoments.from_vals(x, mom=mom)"
             ]
         },
@@ -91,15 +91,15 @@
                 "behind the scenes, cmomy uses numba jit compiler.\n",
                 "first call to function compiles the numba function\n",
                 "subsequent calls very fast"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Help on property:\n",
@@ -121,40 +121,40 @@
                 "# attributes of s\n",
                 "# s.data -> 'moments data'\n",
                 "help(cmomy.CentralMoments.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# access to raw moments\n",
                 "np.testing.assert_allclose(s.rmom(), raw_mom)\n",
                 "\n",
                 "# access to central moments\n",
                 "np.testing.assert_allclose(s.cmom(), cen_mom)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# other attributes\n",
                 "np.testing.assert_allclose(s.mean(), x.mean())\n",
                 "np.testing.assert_allclose(s.var(), x.var(ddof=0))\n",
                 "np.testing.assert_allclose(s.weight(), len(x))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# converting raw/central\n",
                 "# note that this can run into numerical stability issues\n",
                 "\n",
                 "raw = s.to_raw()\n",
@@ -171,63 +171,63 @@
                 "\n",
                 "np.testing.assert_allclose(cen, cen2)\n",
                 "np.testing.assert_allclose(raw, raw2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 62,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# so whats the point?  The real power is in combining statistics\n",
                 "# using numerically stable methods based on central moments\n",
                 "\n",
                 "x2 = np.random.rand(200)\n",
                 "xc = np.concatenate((x, x2), axis=0)\n",
                 "\n",
                 "cen_mom = scipy.stats.moment(xc, moment=np.arange(mom + 1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 65,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# note, this is just for x2\n",
                 "s2 = cmomy.CentralMoments.from_vals(x2, mom=mom)\n",
                 "# sum two object\n",
                 "sc = s + s2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 68,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(sc.cmom(), cen_mom)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 71,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# could also create one object and build from there\n",
                 "sc = cmomy.CentralMoments.from_vals(x, mom=mom)\n",
                 "sc.push_vals(x2)\n",
                 "np.testing.assert_allclose(sc.cmom(), cen_mom)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 95,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# resampling\n",
                 "ndat = len(x)\n",
                 "nrep = 20\n",
                 "idx = np.random.choice(ndat, (nrep, ndat), replace=True)\n",
@@ -243,29 +243,29 @@
                 "    x, indices=idx, mom=mom, resample_kws={\"parallel\": True}\n",
                 ")\n",
                 "np.testing.assert_allclose(s.cmom(), cen_mom)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 126,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# resampling much faster for big-ish arrays\n",
                 "y = np.random.rand(20000)\n",
                 "ndat = len(y)\n",
                 "nrep = 1000\n",
                 "\n",
                 "idx = np.random.choice(ndat, (nrep, ndat), replace=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 127,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "672 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -280,15 +280,15 @@
                 "# cmomy puts moments in last axes\n",
                 "# so move first to last\n",
                 "cen_mom = np.moveaxis(cen_mom, 0, -1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 128,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "120 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -307,39 +307,39 @@
             "metadata": {},
             "source": [
                 "## Arbitrary weights"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 130,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(100)\n",
                 "w = np.random.rand(100)\n",
                 "\n",
                 "s = cmomy.CentralMoments.from_vals(x=x, w=w, mom=mom)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 134,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "cen_mom = np.average(\n",
                 "    (x[:, None] - np.average(x, weights=w)) ** np.arange(mom + 1), weights=w, axis=0\n",
                 ")\n",
                 "cen_mom[1] = 0"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 136,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(cen_mom, s.cmom())"
             ]
         },
         {
@@ -347,53 +347,53 @@
             "metadata": {},
             "source": [
                 "# Arbitrary shapes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 146,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(100, 20, 3)\n",
                 "\n",
                 "cen_mom = scipy.stats.moment(x, moment=np.arange(mom + 1), axis=0)\n",
                 "cen_mom = np.moveaxis(cen_mom, 0, -1)\n",
                 "\n",
                 "s = cmomy.CentralMoments.from_vals(x, mom=mom)\n",
                 "np.testing.assert_allclose(cen_mom, s.cmom())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 156,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# and now we can take advantage of some stuff\n",
                 "# reduce along an axis\n",
                 "sr = s.reduce(axis=0)\n",
                 "\n",
                 "test = scipy.stats.moment(x.reshape(-1, 3), moment=np.arange(mom + 1), axis=0)\n",
                 "test = np.moveaxis(test, 0, -1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 160,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(sr.cmom(), test)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 181,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# resample s along axis=0\n",
                 "ndat = s.shape[0]\n",
                 "nrep = 50\n",
                 "idx = np.random.choice(ndat, (nrep, ndat), True)\n",
@@ -407,15 +407,15 @@
                 "\n",
                 "\n",
                 "np.testing.assert_allclose(test, sr.cmom())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 182,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "479 \u00b5s \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -426,15 +426,15 @@
                 "%%timeit -n 1 -r 1\n",
                 "# also much faster\n",
                 "sr = s.resample_and_reduce(indices=idx, axis=0, resample_kws={\"parallel\": True})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 183,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "5.27 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -456,55 +456,55 @@
                 "# Wrapping things with xarray\n",
                 "\n",
                 "xarray gives a beautiful interface for woring with multidimensional data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 184,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 186,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(100, 2, 3, 4)\n",
                 "xx = xr.DataArray(x, dims=[\"rec\", \"a\", \"b\", \"c\"])\n",
                 "\n",
                 "mom = 4"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 193,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = cmomy.CentralMoments.from_vals(x, mom=mom, axis=0)\n",
                 "sx = cmomy.xCentralMoments.from_vals(xx, mom=mom, axis=\"rec\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 194,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.data, sx.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 196,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -982,27 +982,27 @@
                             "         [ 1.00000000e+02,  5.01595071e-01,  8.52583579e-02,\n",
                             "           2.29920778e-03,  1.28353683e-02],\n",
                             "         [ 1.00000000e+02,  5.20820889e-01,  8.37776495e-02,\n",
                             "           8.78129180e-04,  1.21244782e-02]]]])\n",
                             "Dimensions without coordinates: a, b, c, mom_0"
                         ]
                     },
-                    "execution_count": 196,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# values property gives access to xarray object\n",
                 "sx.values"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 203,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<CentralMoments(val_shape=(2, 4), mom=(4,))>\n",
                             "<xarray.DataArray (a: 2, c: 4, mom_0: 5)>\n",
@@ -1022,27 +1022,27 @@
                             "        [ 3.00000000e+02,  4.89474416e-01,  8.37243432e-02,\n",
                             "          2.81916286e-03,  1.23038060e-02],\n",
                             "        [ 3.00000000e+02,  4.92180451e-01,  8.73256720e-02,\n",
                             "          1.83216293e-03,  1.35473693e-02]]])\n",
                             "Dimensions without coordinates: a, c, mom_0"
                         ]
                     },
-                    "execution_count": 203,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# do things with xarray\n",
                 "sx.reduce(axis=\"b\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 205,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<CentralMoments(val_shape=(2, 2, 4), mom=(4,))>\n",
                             "<xarray.DataArray (a: 2, b: 2, c: 4, mom_0: 5)>\n",
@@ -1081,15 +1081,15 @@
                             "         [ 1.00000000e+02,  4.65567417e-01,  8.85726638e-02,\n",
                             "           6.39523575e-03,  1.34152640e-02],\n",
                             "         [ 1.00000000e+02,  4.56078856e-01,  1.02777743e-01,\n",
                             "           5.66368551e-03,  1.68612769e-02]]]])\n",
                             "Dimensions without coordinates: a, b, c, mom_0"
                         ]
                     },
-                    "execution_count": 205,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# do selection\n",
                 "sx.sel(b=[0, 1])"
@@ -1103,24 +1103,24 @@
                 "\n",
                 "all the routines work with comoments as well\n",
                 "just pass mom=(mom_0, mom_1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mom = (3, 3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "NameError",
                     "evalue": "name 'np' is not defined",
                     "output_type": "error",
                     "traceback": [
@@ -1139,15 +1139,15 @@
                 "# NOTE: for co moments, pass in two variables as tuple (x, y)\n",
                 "\n",
                 "s = cmomy.CentralMoments.from_vals((x, y), w=w, mom=mom)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 239,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# smart broadcasting\n",
                 "x = np.random.rand(100, 2, 3)\n",
                 "y = np.random.rand(100)\n",
                 "\n",
@@ -1160,15 +1160,15 @@
                 "s1 = cmomy.CentralMoments.from_vals((x, y), mom=mom, broadcast=True)\n",
                 "\n",
                 "np.testing.assert_allclose(s0.data, s1.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 249,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# super convinient to use xarray for this\n",
                 "\n",
                 "xx = xr.DataArray(x, dims=[\"rec\", \"a\", \"b\"])\n",
                 "yy = xr.DataArray(y, dims=[\"rec\"])\n",
@@ -1184,24 +1184,24 @@
                 "    mom_dims=[\"mom_x\", \"mom_y\"],\n",
                 "    broadcast=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 246,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(sx.data, s0.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 251,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# note, can also just pass arrays to xCentral\n",
                 "sx1 = cmomy.xCentralMoments.from_vals(\n",
                 "    (x, y),\n",
                 "    mom=mom,\n",
@@ -1212,24 +1212,24 @@
                 "    mom_dims=[\"mom_x\", \"mom_y\"],\n",
                 "    broadcast=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 253,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "xr.testing.assert_allclose(sx.values, sx1.values)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 255,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<CentralMoments(val_shape=(20, 2), mom=(3, 3))>\n",
                             "<xarray.DataArray (rep: 20, a: 2, mom_x: 4, mom_y: 4)>\n",
@@ -1273,31 +1273,26 @@
                             "         [ 9.08077631e-02,  1.17068156e-03,  9.32882192e-03,\n",
                             "          -5.69426727e-04],\n",
                             "         [-3.64767045e-03, -1.18909336e-04,  4.80609201e-06,\n",
                             "           3.54163005e-05]]]])\n",
                             "Dimensions without coordinates: rep, a, mom_x, mom_y"
                         ]
                     },
-                    "execution_count": 255,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# and of course, can do whatever now\n",
                 "sx.resample_and_reduce(nrep=20, axis=\"b\")"
             ]
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python [conda env:.conda-py37]",
-            "language": "python",
-            "name": "conda-env-.conda-py37-py"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/examples/archived/parallel_test.ipynb` & `cmomy-0.9.0/examples/archived/parallel_test.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9465876436781608%*

 * *Differences: {"'cells'": "{0: {'execution_count': None}, 1: {'execution_count': None, 'outputs': {0: "*

 * *            "{'execution_count': None}}}, 2: {'execution_count': None}, 4: {'execution_count': "*

 * *            "None}, 5: {'execution_count': None}, 6: {'execution_count': None}, 7: "*

 * *            "{'execution_count': None}, 8: {'execution_count': None}, 9: {'execution_count': "*

 * *            "None}, 10: {'execution_count': None}, 11: {'execution_count': None}, 12: "*

 * *            "{'execution_count': None}, 13: {'execution_c […]*

```diff
@@ -1,46 +1,46 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from importlib import reload\n",
                 "\n",
                 "import accumulator as Accum\n",
                 "import accumulator2 as Accum2\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator2' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator2.py'>"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(Accum)\n",
                 "reload(Accum2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(1000)\n",
                 "\n",
                 "data = np.zeros(3)\n",
                 "for xx in x:\n",
@@ -74,15 +74,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "520 \u00b5s \u00b1 116 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
@@ -96,15 +96,15 @@
                 "np.testing.assert_allclose(g.mean(), x.mean())\n",
                 "np.testing.assert_allclose(g.var(), x.var(ddof=0))\n",
                 "np.testing.assert_allclose(g.weight(), len(x))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "481 \u00b5s \u00b1 135 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
@@ -118,15 +118,15 @@
                 "np.testing.assert_allclose(g.mean(), x.mean())\n",
                 "np.testing.assert_allclose(g.var(), x.var(ddof=0))\n",
                 "np.testing.assert_allclose(g.weight(), len(x))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(5000, 100)\n",
                 "\n",
                 "\n",
                 "idx = np.cumsum(np.random.randint(1, 20, 1000))\n",
@@ -144,15 +144,15 @@
                 "\n",
                 "s = (slice(None),) + (None,) * (x.ndim - 1)\n",
                 "LW = np.broadcast_to(LW[s], LA.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "g = Accum.StatsAccumVec.from_stats(A=LA, V=LV, W=LW)\n",
                 "\n",
                 "np.testing.assert_allclose(g.mean(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(g.var(), x.var(axis=0, ddof=0))\n",
@@ -164,15 +164,15 @@
                 "np.testing.assert_allclose(g.mean(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(g.var(), x.var(axis=0, ddof=0))\n",
                 "np.testing.assert_allclose(g.weight(), np.count_nonzero(x, axis=0))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "998 \u00b5s \u00b1 27.1 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n",
@@ -183,76 +183,76 @@
             "source": [
                 "%timeit -n 10 -r 3 Accum.StatsAccumVec.from_stats(A=LA, V=LV, W=LW)\n",
                 "%timeit -n 10 -r 3 Accum2.StatsAccumVec.from_stats(A=LA, V=LV, W=LW)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# by value"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X = np.random.rand(10000, 100)\n",
                 "W = np.random.rand(10000, 1)\n",
                 "# W = np.ones((1000, 1), dtype=X.dtype)\n",
                 "W = np.broadcast_to(W, X.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "g = Accum.StatsAccumVec.from_vals(X, W=W)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data = np.zeros_like(g._datar)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data.fill(0.0)\n",
                 "Accum._push_vals_vec(data, W, X)\n",
                 "np.testing.assert_allclose(data, g.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data.fill(0.0)\n",
                 "Accum2._push_vals_vec(data, W, X)\n",
                 "np.testing.assert_allclose(data, g.data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "13.3 ms \u00b1 964 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n",
@@ -263,15 +263,15 @@
             "source": [
                 "%timeit -n 10 -r 3 Accum._push_vals_vec(data, W, X)\n",
                 "%timeit -n 10 -r 3 Accum2._push_vals_vec(data, W, X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# numba\n",
                 "from numba import jit, njit, prange\n",
                 "\n",
                 "_PARALLEL = True\n",
@@ -296,15 +296,15 @@
                 "\n",
                 "            data[m, 1] += incr\n",
                 "            data[m, 2] += (1.0 - alpha) * (delta * incr) - alpha * data[m, 2]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "3.02 ms \u00b1 340 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n"
@@ -317,15 +317,15 @@
                 "np.testing.assert_allclose(data, g.data)\n",
                 "\n",
                 "%timeit -n 10 -r 3  _push_vals_vec(data, W, X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "2.86 ms \u00b1 176 \u00b5s per loop (mean \u00b1 std. dev. of 3 runs, 10 loops each)\n"
@@ -338,35 +338,35 @@
                 "np.testing.assert_allclose(data, g.data)\n",
                 "\n",
                 "%timeit -n 10 -r 3  _push_vals_vec(data, W, X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 240,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "CPUDispatcher(<function _push_vals_vec at 0x615dd16a8>)"
                         ]
                     },
-                    "execution_count": 240,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "_push_vals_vec.py_func"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 235,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# @njit\n",
                 "# def _push_val(data, w, x):\n",
                 "#     if w == 0.0:\n",
                 "#         return\n",
@@ -411,74 +411,74 @@
                 "        for m in range(nmeta):\n",
                 "            out = _push_val_inc(data[m, :], W[s, m], X[s, m])\n",
                 "            data[m, :] += out  # _push_val_inc(data[m, :], W[s, m], X[s, m])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 237,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data.fill(0.0)\n",
                 "_push_vals_vec2(data, W, X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 232,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "a[0, :] += b"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 219,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(data, g.data)\n",
                 "\n",
                 "# %timeit -n 10 -r 3  _push_vals_vec2(data, W, X)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# random data\n",
                 "Data = np.random.rand(100, 5, 3)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 55,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "g = Accum.StatsAccumVec.from_datas(Data=Data, axis=0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 56,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data = np.zeros_like(g._datar)\n",
                 "Accum._push_stats_data_vec(data, Data)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(data, g.data)"
             ]
         },
         {
@@ -486,19 +486,14 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python [conda env:idp35]",
-            "language": "python",
-            "name": "conda-env-idp35-py"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/examples/archived/test_accumulator.ipynb` & `cmomy-0.9.0/examples/archived/test_accumulator.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9468377976190478%*

 * *Differences: {"'cells'": "{0: {'execution_count': None}, 2: {'execution_count': None, 'outputs': {0: "*

 * *            "{'execution_count': None}}}, 3: {'execution_count': None}, 4: {'execution_count': "*

 * *            "None}, 5: {'execution_count': None}, 6: {'execution_count': None}, 7: "*

 * *            "{'execution_count': None}, 8: {'execution_count': None, 'outputs': {0: "*

 * *            "{'execution_count': None}}}, 9: {'execution_count': None}, 10: {'execution_count': "*

 * *            "None, 'outputs': {0: {'execution_count': No […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from importlib import reload\n",
                 "\n",
                 "import accumulator as Accum\n",
                 "import numpy as np\n",
@@ -18,110 +18,110 @@
             "metadata": {},
             "source": [
                 "# Scalar data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator.py'>"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(Accum)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(1000)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccum.from_vals(x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), x.mean())\n",
                 "np.testing.assert_allclose(s.var(), x.var(ddof=0))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccum.from_stat(x.mean(), x.var(ddof=0), len(x))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sa = Accum.StatsArray.from_stats(x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<accumulator.StatsAccum at 0x7ff7508a00d0>"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "f = sa.to_xarray()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre>&lt;xarray.DataArray (rec: 1000, val: 3)&gt;\n",
                             "array([[1.        , 0.38241961, 0.        ],\n",
@@ -145,35 +145,35 @@
                             "       [1.        , 0.6610002 , 0.        ],\n",
                             "       [1.        , 0.59220549, 0.        ]])\n",
                             "Coordinates:\n",
                             "  * val      (val) <U3 'cnt' 'ave' 'var'\n",
                             "Dimensions without coordinates: rec"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "f"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre>&lt;xarray.DataArray (val: 3)&gt;\n",
                             "array([1.00000000e+03, 4.91282729e-01, 8.53000249e-02])\n",
@@ -183,84 +183,84 @@
                         "text/plain": [
                             "<xarray.DataArray (val: 3)>\n",
                             "array([1.00000000e+03, 4.91282729e-01, 8.53000249e-02])\n",
                             "Coordinates:\n",
                             "  * val      (val) <U3 'cnt' 'ave' 'var'"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "xr.DataArray(s._data, dims=\"val\", coords={\"val\": [\"cnt\", \"ave\", \"var\"]})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(np.cumsum(x) / (np.arange(len(x)) + 1.0), sa.cummean())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([1.00000000e+03, 4.91282729e-01, 8.53000249e-02])"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sa.cumdata_last"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "1.0"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.prod(s.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'a': 1}"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = {\"a\": 1}\n",
                 "b = {}\n",
@@ -268,51 +268,51 @@
                 "d.update(a)\n",
                 "d.update(b)\n",
                 "d"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "f = xr.DataArray(sa.data, dims=[\"rec\", \"val\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "f.coords.update({\"val\": [\"a\", \"b\", \"c\"]})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "f.coords[\"val\"] = list(\"abc\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre>&lt;xarray.DataArray (rec: 1000, val: 3)&gt;\n",
                             "array([[1.        , 0.38241961, 0.        ],\n",
@@ -336,137 +336,137 @@
                             "       [1.        , 0.6610002 , 0.        ],\n",
                             "       [1.        , 0.59220549, 0.        ]])\n",
                             "Coordinates:\n",
                             "  * val      (val) <U1 'a' 'b' 'c'\n",
                             "Dimensions without coordinates: rec"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "f"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# addition"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# x1 = np.random.rand(1000)\n",
                 "# x2 = np.random.rand(2000)\n",
                 "x1 = x[:500]\n",
                 "x2 = x[500:]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s1 = Accum.StatsAccum.from_vals(x1)\n",
                 "s2 = Accum.StatsAccum.from_vals(x2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s12 = s1 + s2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.00000000e+00, 2.22044605e-16, 1.11022302e-16])"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s12._data - s._data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 0.00000000e+00, -4.44089210e-16, -2.22044605e-16])"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ss = s - s2\n",
                 "ss._data - s1._data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 0.00000000e+00, -4.44089210e-16, -2.22044605e-16])"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ss = s - s1\n",
                 "ss._data - s2._data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccum.from_stat(x.mean(), x.var(ddof=0), len(x))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), x.mean())\n",
                 "np.testing.assert_allclose(s.var(), x.var(ddof=0))"
             ]
         },
@@ -475,35 +475,35 @@
             "metadata": {},
             "source": [
                 "# vector"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator.py'>"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(Accum)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "xs = np.random.rand(5000, 5)\n",
                 "\n",
                 "xs1 = xs[:2500, ...]\n",
                 "xs2 = xs[2500:, ...]\n",
@@ -530,15 +530,15 @@
                 "LAs = np.array(LAs)\n",
                 "LVs = np.array(LVs)\n",
                 "LWs = np.array(LWs)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumVec.from_vals(xs)"
             ]
         },
         {
@@ -546,398 +546,398 @@
             "metadata": {},
             "source": [
                 "s.zero()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "w = Accum.StatsArray(shape=s.shape, child=Accum.StatsAccumVec)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "w.push_stats(LA, LV, np.broadcast_to(LW[:, None], LA.shape))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(507, 5)"
                         ]
                     },
-                    "execution_count": 37,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "LA.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(LA, w.mean())\n",
                 "np.testing.assert_allclose(LV, w.var())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.5036704 , 0.49838795, 0.50379665, 0.50258301, 0.50365975])"
                         ]
                     },
-                    "execution_count": 39,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.mean()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.5036704 , 0.49838795, 0.50379665, 0.50258301, 0.50365975])"
                         ]
                     },
-                    "execution_count": 40,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "w.cummean()[-1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.08316448, 0.08375163, 0.08252745, 0.08294445, 0.08403148])"
                         ]
                     },
-                    "execution_count": 41,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "w.cumvar_last()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.28838252, 0.28939874, 0.28727591, 0.28800078, 0.28988184])"
                         ]
                     },
-                    "execution_count": 42,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "w.cumstd_last()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.08316448, 0.08375163, 0.08252745, 0.08294445, 0.08403148])"
                         ]
                     },
-                    "execution_count": 43,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.var()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([0.5036704 , 0.49838795, 0.50379665, 0.50258301, 0.50365975])"
                         ]
                     },
-                    "execution_count": 44,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.mean()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(507, 5)"
                         ]
                     },
-                    "execution_count": 45,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "LAs.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(507,)"
                         ]
                     },
-                    "execution_count": 46,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "LWs.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(507, 5)"
                         ]
                     },
-                    "execution_count": 47,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "LAs.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "w = np.broadcast_to(LWs[:, None], LAs.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 49,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "f = Accum.StatsArray.from_stats(\n",
                 "    LAs, LVs, w, child=Accum.StatsAccumVec, shape=xs.shape[1:]\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 50,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), xs.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var(), xs.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), xs.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 51,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumVec.from_stat(xs.mean(axis=0), xs.var(axis=0, ddof=0), xs.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), xs.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var(), xs.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), xs.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 53,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumVec.from_stats(LAs, LVs, LWs[:, None])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 54,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), xs.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var(), xs.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), xs.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 55,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "((507, 5), (507, 5), (507,))"
                         ]
                     },
-                    "execution_count": 55,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "LAs.shape, LVs.shape, LWs.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 56,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumVec(shape=xs.shape[1:])\n",
                 "for a, v, w in zip(LAs, LVs, LWs):\n",
                 "    s.push_stat(a, v, w)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 57,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), xs.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var(), xs.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), xs.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 58,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s1 = Accum.StatsAccumVec.from_vals(xs1, axis=0)\n",
                 "s2 = Accum.StatsAccumVec.from_vals(xs2, axis=0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = s1 + s2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 60,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean(), xs.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var(), xs.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), xs.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 61,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ss = s - s1\n",
                 "np.testing.assert_allclose(ss.mean(), xs2.mean(axis=0))\n",
                 "np.testing.assert_allclose(ss.var(), xs2.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(ss.weight(), xs2.shape[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 62,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ss = s - s2\n",
                 "np.testing.assert_allclose(ss.mean(), xs1.mean(axis=0))\n",
                 "np.testing.assert_allclose(ss.var(), xs1.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(ss.weight(), xs1.shape[0])"
@@ -955,15 +955,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 63,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(array([1766, 2903,  679, 2476, 3646, 4624, 2056,  491, 2649, 1216, 1075,\n",
                             "        1195,  928, 4702, 4162,  873, 2508, 3922, 3760, 1220, 4604, 4613,\n",
@@ -971,26 +971,26 @@
                             "         572, 1441, 2553, 3916,  206, 4729, 3084, 1323, 4113, 1892, 1000,\n",
                             "         880, 1026, 2394, 2351, 1237, 4522]),\n",
                             " array([0, 4, 1, 2, 1, 0, 3, 2, 1, 3, 1, 3, 3, 3, 0, 2, 2, 1, 2, 0, 2, 2,\n",
                             "        4, 0, 4, 3, 2, 0, 0, 0, 4, 3, 0, 3, 1, 2, 1, 0, 4, 0, 0, 0, 4, 2,\n",
                             "        2, 2, 3, 3, 3, 0]))"
                         ]
                     },
-                    "execution_count": 63,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.unravel_index(np.random.choice(np.arange(np.prod(x.shape)), 50), x.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 64,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = np.random.rand(1000, 3, 2)\n",
                 "xr = x.reshape(1000, -1)\n",
                 "\n",
                 "n_nan = 100\n",
@@ -1010,106 +1010,106 @@
                 "\n",
                 "x1r = x1.reshape(x1.shape[0], -1)\n",
                 "x2r = x2.reshape(x2.shape[0], -1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 65,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# %%timeit -n 3\n",
                 "ns = x.shape[1:] * 2\n",
                 "c = np.cov(xr.T, ddof=0).reshape(ns)\n",
                 "c1 = np.cov(x1r.T, ddof=0).reshape(ns)\n",
                 "c2 = np.cov(x2r.T, ddof=0).reshape(ns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 66,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator.py'>"
                         ]
                     },
-                    "execution_count": 66,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(Accum)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 67,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov(x.shape[1:])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 68,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "for xx in x:\n",
                 "    s.push_val(xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 69,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean_diag(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var_diag(), x.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.var(), c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 70,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov(x.shape[1:])\n",
                 "\n",
                 "s.push_vals(x, W=1.0)\n",
                 "\n",
                 "np.testing.assert_allclose(s.mean_diag(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var_diag(), x.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.var(), c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 71,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov.from_vals(x)\n",
                 "\n",
                 "np.testing.assert_allclose(s.mean_diag(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var_diag(), x.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.var(), c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 72,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s1 = Accum.StatsAccumCov.from_vals(x1, W=1.0, axis=0)\n",
                 "s2 = Accum.StatsAccumCov.from_vals(x2, W=1.0, axis=0)\n",
                 "\n",
                 "s = s1 + s2\n",
@@ -1125,40 +1125,40 @@
                 "np.testing.assert_allclose(s.mean_diag(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var_diag(), x.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.var(), c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 73,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov(x.shape[1:])\n",
                 "s.push_stat(x.mean(axis=0), c, w=x.shape[0])\n",
                 "np.testing.assert_allclose(s.mean_diag(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var_diag(), x.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.var(), c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 74,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov.from_stat(x.mean(axis=0), c, w=x.shape[0])\n",
                 "np.testing.assert_allclose(s.mean_diag(), x.mean(axis=0))\n",
                 "np.testing.assert_allclose(s.var_diag(), x.var(ddof=0, axis=0))\n",
                 "np.testing.assert_allclose(s.var(), c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 75,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_cov(a, ns):\n",
                 "    ave = np.nanmean(a, axis=1)\n",
                 "    np.zeros((a.shape[0],) * 2)\n",
                 "\n",
@@ -1183,35 +1183,35 @@
                 "cov, cnt = get_cov(a, ns)\n",
                 "cov1, cnt1 = get_cov(a1, ns)\n",
                 "cov2, cnt2 = get_cov(a2, ns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 76,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'accumulator' from '/Users/wpk/Documents/python/projects/python_dropin_files/accumulator.py'>"
                         ]
                     },
-                    "execution_count": 76,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reload(Accum)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 77,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov(shape=x.shape[1:])\n",
                 "\n",
                 "W = np.isfinite(x).astype(np.float)\n",
                 "W = W[..., None, None] * W[:, None, None, ...]\n",
@@ -1221,68 +1221,68 @@
                 "np.testing.assert_allclose(s.mean_diag(), np.nanmean(x, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), cnt)\n",
                 "np.testing.assert_allclose(s.cov_corrected(), cov)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 78,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = Accum.StatsAccumCov.from_vals(x, W)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 79,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean_diag(), np.nanmean(x, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), cnt)\n",
                 "np.testing.assert_allclose(s.cov_corrected(), cov)\n",
                 "np.testing.assert_allclose(s.var_diag(), np.nanvar(x, ddof=0, axis=0))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 80,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "Wi = []\n",
                 "for xx in [x1, x2]:\n",
                 "    w = np.isfinite(xx).astype(np.float)\n",
                 "    w = w[..., None, None] * w[:, None, None, ...]\n",
                 "    Wi.append(w)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 81,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s1 = Accum.StatsAccumCov.from_vals(x1, W=Wi[0])\n",
                 "s2 = Accum.StatsAccumCov.from_vals(x2, W=Wi[1])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 82,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = s1 + s2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 83,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(s.mean_diag(), np.nanmean(x, axis=0))\n",
                 "np.testing.assert_allclose(s.weight(), cnt)\n",
                 "np.testing.assert_allclose(s.cov_corrected(), cov)\n",
                 "np.testing.assert_allclose(s.var_diag(), np.nanvar(x, ddof=0, axis=0))"
@@ -1293,86 +1293,86 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 84,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(3,)"
                         ]
                     },
-                    "execution_count": 84,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.stack([1, 2, 3], axis=-1).shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 85,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "W = np.array([s.weight(), s.weight()])\n",
                 "A = np.array([s.mean(), s.mean()])\n",
                 "V = np.array([s.var(), s.var()])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 86,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(2, 3, 2, 3, 2)"
                         ]
                     },
-                    "execution_count": 86,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "W.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 87,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(2, 3, 2, 3, 2, 3)"
                         ]
                     },
-                    "execution_count": 87,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.stack([W, A, V], axis=-1).shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 88,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[[[[ 9.95000000e+02,  4.87198080e-01,  7.84195861e-02],\n",
                             "          [ 9.85000000e+02,  4.86397687e-01,  2.93751787e-03]],\n",
@@ -1432,26 +1432,26 @@
                             "         [[ 9.83000000e+02,  5.00243763e-01,  3.86197368e-03],\n",
                             "          [ 9.75000000e+02,  5.00183032e-01,  1.33996650e-03]],\n",
                             "\n",
                             "         [[ 9.81000000e+02,  5.00807373e-01,  1.14628007e-03],\n",
                             "          [ 9.87000000e+02,  4.99695367e-01,  8.15205187e-02]]]]])"
                         ]
                     },
-                    "execution_count": 88,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.stack([s.weight(), s.mean(), s.var()], axis=-1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 89,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[[[[ 9.95000000e+02,  9.85000000e+02],\n",
                             "          [ 9.91000000e+02,  9.83000000e+02],\n",
@@ -1532,15 +1532,15 @@
                             "          [ 8.30360487e-02,  1.14628007e-03]],\n",
                             "\n",
                             "         [[-1.01649386e-03,  2.75317105e-03],\n",
                             "          [ 3.86197368e-03,  1.33996650e-03],\n",
                             "          [ 1.14628007e-03,  8.15205187e-02]]]]])"
                         ]
                     },
-                    "execution_count": 89,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "np.array([s.weight(), s.mean(), s.var()])"
             ]
@@ -1557,15 +1557,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 96,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@njit\n",
                 "def _push_val_cov_data_general(data, w, x) -> None:\n",
                 "    # data[i,j,0] = weight[i,j]\n",
                 "    # data[i,j,1] = ave[i,j]\n",
@@ -1654,15 +1654,15 @@
                 "\n",
                 "                data[i, j, 2] = v\n",
                 "                data[j, i, 2] = v"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 97,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "NameError",
                     "evalue": "name '_push_val_cov_data' is not defined",
                     "output_type": "error",
                     "traceback": [
@@ -1694,15 +1694,15 @@
                 "\n",
                 "for xx in a.T:\n",
                 "    _push_val_cov_data_general(data, 1.0, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 92,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "AssertionError",
                     "evalue": "\nNot equal to tolerance rtol=1e-07, atol=0\n\n(shapes (6,), (3, 2, 3, 2) mismatch)\n x: array([0., 0., 0., 0., 0., 0.])\n y: array([[[[995., 985.],\n         [991., 983.],\n         [989., 982.]],...",
                     "output_type": "error",
                     "traceback": [
@@ -1729,15 +1729,15 @@
                 "c = data[:, :, 2] + cross\n",
                 "\n",
                 "np.testing.assert_allclose(c, cov)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 93,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "229 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n"
@@ -1753,15 +1753,15 @@
                 "    w = np.isfinite(xx).astype(np.float)\n",
                 "    w = w * w[:, None]\n",
                 "    _push_val_cov(data, w, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 94,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# %%timeit -n 1 -r 1\n",
                 "# another way\n",
                 "n = a.shape[0]\n",
                 "data = np.zeros((n, n, 3))\n",
@@ -1769,15 +1769,15 @@
                 "    w = np.isfinite(xx).astype(np.float)\n",
                 "    w = w * w[:, None]\n",
                 "    _push_val_cov(data, w, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 95,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "AssertionError",
                     "evalue": "\nNot equal to tolerance rtol=1e-07, atol=0\n\n(shapes (6, 6), (3, 2, 3, 2) mismatch)\n x: array([[995., 985., 991., 983., 989., 982.],\n       [985., 990., 986., 978., 984., 977.],\n       [991., 986., 996., 984., 990., 983.],...\n y: array([[[[995., 985.],\n         [991., 983.],\n         [989., 982.]],...",
                     "output_type": "error",
                     "traceback": [
@@ -1804,35 +1804,35 @@
                 "c = data[:, :, 2] + cross\n",
                 "\n",
                 "np.testing.assert_allclose(c, cov)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(1, 2, 3, 1, 2, 3)"
                         ]
                     },
-                    "execution_count": 36,
+                    "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "(1, 2, 3) * 2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@njit\n",
                 "def _push_stat_cov(data, w, a, v) -> None:\n",
                 "    n = a.shape[0]\n",
                 "    for i in range(n):\n",
@@ -1868,15 +1868,15 @@
                 "\n",
                 "                data[i, j, 2] = c\n",
                 "                data[j, i, 2] = c"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "n = a.shape[0]\n",
                 "data1 = np.zeros((n, n, 3))\n",
                 "data2 = np.zeros((n, n, 3))\n",
                 "\n",
@@ -1889,15 +1889,15 @@
                 "    w = np.isfinite(xx).astype(np.float)\n",
                 "    w = w * w[:, None]\n",
                 "    _push_val_cov(data2, w, xx)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data12 = np.zeros((n, n, 3))\n",
                 "_push_stat_cov(data12, data1[..., 0], data1[..., 1], data1[..., 2])\n",
                 "_push_stat_cov(data12, data2[..., 0], data2[..., 1], data2[..., 2])"
             ]
@@ -1907,15 +1907,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(data, data12)"
             ]
         },
         {
@@ -1937,19 +1937,14 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python [conda env:.conda-py37]",
-            "language": "python",
-            "name": "conda-env-.conda-py37-py"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/examples/usage/motivation.ipynb` & `cmomy-0.9.0/examples/usage/motivation.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9507207030668394%*

 * *Differences: {"'cells'": "{0: {'id': '0', 'metadata': {delete: ['execution']}}, 1: {'id': '1'}, 2: {'id': '2', "*

 * *            "'metadata': {replace: OrderedDict()}}, 3: {'id': '3', 'metadata': {replace: "*

 * *            "OrderedDict()}}, 4: {'id': '4', 'metadata': {delete: ['execution']}}, 5: {'id': '5'}, "*

 * *            "6: {'id': '6', 'metadata': {replace: OrderedDict()}}, 7: {'id': '7'}, 8: {'id': '8', "*

 * *            "'metadata': {replace: OrderedDict()}, 'outputs': {0: {'data': {'text/html': {insert: "*

 * *            '[(363,  […]*

```diff
@@ -1,20 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "e36e629b",
+            "id": "0",
             "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:15.685650Z",
-                    "iopub.status.busy": "2024-02-21T00:39:15.685339Z",
-                    "iopub.status.idle": "2024-02-21T00:39:15.693734Z",
-                    "shell.execute_reply": "2024-02-21T00:39:15.693144Z"
-                },
                 "tags": [
                     "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# mypy: disable-error-code=\"no-untyped-def, no-untyped-call, assignment\"\n",
@@ -31,15 +25,15 @@
                 "    p = p.parent\n",
                 "\n",
                 "os.environ[\"NUMBA_CACHE_DIR\"] = str(p / \".numba_cache\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4e729b26",
+            "id": "1",
             "metadata": {},
             "source": [
                 "# Why `cmomy`?\n",
                 "\n",
                 "$$\\newcommand{\\ave}[1]{\\langle{#1}\\rangle}$$\n",
                 "\n",
                 "We wish to calculate moments of the form $\\ave{x}$ and $\\ave{(\\delta x)^k}$, $\\delta x = (x - \\ave{x})$, where, in general we define averages\n",
@@ -69,23 +63,16 @@
                 "\n",
                 "In what follows, we'll arrange data in the from `output[moment]` where `output[0] = {total weight}`, `output[1] = {average value}`, `output[k > 1] = {kth order central moment}`.  We can generate the central moments using the following functions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "f3d00a97",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:15.697161Z",
-                    "iopub.status.busy": "2024-02-21T00:39:15.696950Z",
-                    "iopub.status.idle": "2024-02-21T00:39:15.703530Z",
-                    "shell.execute_reply": "2024-02-21T00:39:15.702934Z"
-                }
-            },
+            "id": "2",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def cmom_1(x, axis=0, mom=3):\n",
                 "    \"\"\"Create central moments using stable method\"\"\"\n",
                 "    # output shape\n",
                 "    shape = x.shape[:axis] + x.shape[axis + 1 :] + (mom + 1,)\n",
                 "    output = np.zeros(shape, dtype=x.dtype)\n",
@@ -126,23 +113,16 @@
                 "\n",
                 "    return output"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "17391a43",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:15.706790Z",
-                    "iopub.status.busy": "2024-02-21T00:39:15.706540Z",
-                    "iopub.status.idle": "2024-02-21T00:39:15.850540Z",
-                    "shell.execute_reply": "2024-02-21T00:39:15.849796Z"
-                }
-            },
+            "id": "3",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "rng = np.random.default_rng(seed=0)\n",
                 "\n",
                 "n = 1000\n",
@@ -153,51 +133,38 @@
                 "# same values\n",
                 "np.testing.assert_allclose(m1, m2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "327d72db",
+            "id": "4",
             "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:15.854213Z",
-                    "iopub.status.busy": "2024-02-21T00:39:15.853816Z",
-                    "iopub.status.idle": "2024-02-21T00:39:15.857697Z",
-                    "shell.execute_reply": "2024-02-21T00:39:15.857147Z"
-                },
                 "tags": [
                     "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "np.set_printoptions(precision=4)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "924d488a",
+            "id": "5",
             "metadata": {},
             "source": [
                 "OK, great.  But what if we have unscaled data?  For example, setting $y = a x + b$ gives $\\ave{y} = a \\ave{x} + b$, but for central moments, $\\ave{(y - \\ave{y})^n} = \\ave{(a x - b - \\ave{a x - b})^n} = a^n \\ave{(\\delta x)^n}$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "b2aad683",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:15.860802Z",
-                    "iopub.status.busy": "2024-02-21T00:39:15.860588Z",
-                    "iopub.status.idle": "2024-02-21T00:39:15.866780Z",
-                    "shell.execute_reply": "2024-02-21T00:39:15.866246Z"
-                }
-            },
+            "id": "6",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "abs error using central moments: [ 0.0000e+00 -1.8190e-12 -8.8373e-16  3.5155e-15]\n",
@@ -234,15 +201,15 @@
                 "rel error using raw moments    : {m2_error / expected}\n",
                 "\"\"\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f1bddbb6",
+            "id": "7",
             "metadata": {},
             "source": [
                 "## So what?\n",
                 "\n",
                 "OK, so central moments have some advantages.  But the two pass thing makes life difficult.  For example, what if we are running a slow experiment or simulation?  We could collect all the samples for `x`, then do the two pass algorithm at the end.  But it would be nice to calculate averages on the fly.  This is why we often turn to raw moments.  There easy to accumulate as data comes in, while central moments, at least as formulated above, are not.  \n",
                 "\n",
                 "Thankfully, smart people have figured out how to calculate central moments in a one-pass way.  Moreover, these methods allow central moments to be combined.  This makes resampling from central moments possible.  We don't go into detail on these formulas, but point the interested reader to the this [article](https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance), and citations within.\n",
@@ -257,23 +224,16 @@
                 "\n",
                 "The primary object for doing all this is {class}`~cmomy.CentralMoments`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "b50093e3",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:15.869905Z",
-                    "iopub.status.busy": "2024-02-21T00:39:15.869547Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.859083Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.858561Z"
-                }
-            },
+            "id": "8",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -633,15 +593,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([ 1.0000e+03,  5.1691e-01,  8.0989e-02, -2.0856e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-668248a7-0bb5-47cf-bf63-38badeb673ba' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-668248a7-0bb5-47cf-bf63-38badeb673ba' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b90ab6f4-8cb0-4198-afda-d3cf4a23999c' class='xr-array-in' type='checkbox' checked><label for='section-b90ab6f4-8cb0-4198-afda-d3cf4a23999c' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1e+03 0.5169 0.08099 -0.002086</span></div><div class='xr-array-data'><pre>array([ 1.000000e+03,  5.169063e-01,  8.098908e-02, -2.085567e-03])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([ 1.0000e+03,  5.1691e-01,  8.0989e-02, -2.0856e-03])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-63805cb0-67d0-496b-90a2-1820cf5d1c3d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-63805cb0-67d0-496b-90a2-1820cf5d1c3d' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-fac2b7dd-c746-4fdb-99b5-2f83f715c277' class='xr-array-in' type='checkbox' checked><label for='section-fac2b7dd-c746-4fdb-99b5-2f83f715c277' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1e+03 0.5169 0.08099 -0.002086</span></div><div class='xr-array-data'><pre>array([ 1.000000e+03,  5.169063e-01,  8.098908e-02, -2.085567e-03])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(3,))>\n",
                             "array([ 1.0000e+03,  5.1691e-01,  8.0989e-02, -2.0856e-03])"
                         ]
                     },
                     "execution_count": 6,
@@ -657,32 +617,25 @@
                 "\n",
                 "\n",
                 "cx"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "54d2ab80",
+            "id": "9",
             "metadata": {},
             "source": [
                 "You can access the underlying data using the {attr}`cmomy.CentralMoments.values` or {attr}`cmomy.CentralMoments.data` attributes."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "0a64afad",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.862262Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.861959Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.865461Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.864855Z"
-                }
-            },
+            "id": "10",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[ 1.0000e+03  5.1691e-01  8.0989e-02 -2.0856e-03]\n"
                     ]
@@ -690,59 +643,45 @@
             ],
             "source": [
                 "print(cx.values)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a8b92e55",
+            "id": "11",
             "metadata": {},
             "source": [
                 "Basically, the {class}`~cmomy.CentralMoments` object is just a collection of routines around {attr}`~cmomy.CentralMoments.data`, which is an array of central moments (with the convention that `data[..., 0]` is the total `weight`, `data[..., 1]` is the average, and `data[..., k > 1]` is the `kth` central moment).  It gives the same results as calculating central moments directly:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "c68b5deb",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.868371Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.868168Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.871429Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.870870Z"
-                }
-            },
+            "id": "12",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "np.testing.assert_allclose(cx.values, m1)\n",
                 "np.testing.assert_allclose(cy.values, m1_shift)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "be0e3c70",
+            "id": "13",
             "metadata": {},
             "source": [
                 "Nice!  But what can that's not all that special.  The real power comes in for multidimensional data.\n",
                 "Suppose that we have separate samples of the data $\\{x_a, x_b, ... \\}$, and want to get there central moments.  We can do the following."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "d9db01aa",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.874455Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.874217Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.879061Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.878483Z"
-                }
-            },
+            "id": "14",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 1.0000e+02,  4.7703e-01,  8.6779e-02, -2.0776e-03,  1.3134e-02],\n",
                             "       [ 1.0000e+02,  4.7149e-01,  8.9923e-02,  4.1844e-06,  1.3357e-02],\n",
                             "       [ 1.0000e+02,  4.9054e-01,  8.3374e-02,  6.0526e-03,  1.2658e-02],\n",
@@ -759,32 +698,25 @@
                 "x = rng.random((100, 5))\n",
                 "m1 = cmom_1(x, axis=0, mom=4)\n",
                 "m1"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c9bd6f9f",
+            "id": "15",
             "metadata": {},
             "source": [
                 "Wrapping the data in a central moments object gives"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "8caf651b",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.882332Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.882081Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.890113Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.889556Z"
-                }
-            },
+            "id": "16",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[5.0000e+02 4.9192e-01 8.8959e-02 1.3873e-04 1.3778e-02]\n",
                         "[5.0000e+02 4.9192e-01 8.8959e-02 1.3873e-04 1.3778e-02]\n"
@@ -800,32 +732,25 @@
                 "\n",
                 "# verify that this is the same as just accumulating all the data\n",
                 "print(cmom_1(x.reshape(-1), mom=4))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d1d2da11",
+            "id": "17",
             "metadata": {},
             "source": [
                 "Excellent! We can use {class}`~cmomy.CentralMoments` to accumulate data on the go"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
-            "id": "54a71048",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.893176Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.892955Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.901662Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.901064Z"
-                }
-            },
+            "id": "18",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -1185,15 +1110,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-8f1a95d5-7df8-4e2e-9a06-809ea79319b5' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-8f1a95d5-7df8-4e2e-9a06-809ea79319b5' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-56e532b5-73ea-42b8-84bf-39b7b5be2d5a' class='xr-array-in' type='checkbox' checked><label for='section-56e532b5-73ea-42b8-84bf-39b7b5be2d5a' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-f71494ac-2333-427e-865d-663e1e68f874' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f71494ac-2333-427e-865d-663e1e68f874' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-77d75d34-d630-490f-a5bf-7ab24fa7aca5' class='xr-array-in' type='checkbox' checked><label for='section-77d75d34-d630-490f-a5bf-7ab24fa7aca5' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])"
                         ]
                     },
                     "execution_count": 11,
@@ -1207,32 +1132,25 @@
                 "    # note: pushing multiple values\n",
                 "    c.push_vals(x[:, i])\n",
                 "c"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "29c07232",
+            "id": "19",
             "metadata": {},
             "source": [
                 "Or, you can push all the values one at a time!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "e4857256",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.904926Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.904674Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.918270Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.917797Z"
-                }
-            },
+            "id": "20",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -1592,15 +1510,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-1757ed37-221b-46e4-b49e-c6f9bbedd640' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1757ed37-221b-46e4-b49e-c6f9bbedd640' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-ab07e560-1182-433d-9a33-e8365ba3d76e' class='xr-array-in' type='checkbox' checked><label for='section-ab07e560-1182-433d-9a33-e8365ba3d76e' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-d0fed2f5-542b-4294-b996-a9f28ab37175' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d0fed2f5-542b-4294-b996-a9f28ab37175' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-7a691e3d-612a-43ef-b5c4-f1b7c562e889' class='xr-array-in' type='checkbox' checked><label for='section-7a691e3d-612a-43ef-b5c4-f1b7c562e889' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])"
                         ]
                     },
                     "execution_count": 12,
@@ -1615,32 +1533,25 @@
                 "    c.push_val(xx)\n",
                 "\n",
                 "c"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "81c5d81b",
+            "id": "21",
             "metadata": {},
             "source": [
                 "The values can even be differently weighted."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "id": "bd188c32",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.921185Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.920978Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.926123Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.925639Z"
-                }
-            },
+            "id": "22",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -2000,15 +1911,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-62f84188-90f3-4f9c-b069-989e6c8e5369' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-62f84188-90f3-4f9c-b069-989e6c8e5369' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4573ded6-9b6d-4002-99fc-98e827d1ae5b' class='xr-array-in' type='checkbox' checked><label for='section-4573ded6-9b6d-4002-99fc-98e827d1ae5b' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-462c12d3-c172-4b7c-89a8-6ae3a248a56b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-462c12d3-c172-4b7c-89a8-6ae3a248a56b' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-8911ff55-27d2-45ea-843e-f54202af306f' class='xr-array-in' type='checkbox' checked><label for='section-8911ff55-27d2-45ea-843e-f54202af306f' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])"
                         ]
                     },
                     "execution_count": 13,
@@ -2023,32 +1934,25 @@
                 "for v in xs:\n",
                 "    c.push_vals(v)\n",
                 "c"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7a853c98",
+            "id": "23",
             "metadata": {},
             "source": [
                 "Alternatively, you can add objects together."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
-            "id": "74e8be73",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.928762Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.928577Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.937286Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.936796Z"
-                }
-            },
+            "id": "24",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[<CentralMoments(val_shape=(), mom=(4,))>\n",
                         "array([5.0000e+01, 4.1743e-01, 7.3610e-02, 4.5490e-03, 1.0645e-02]), <CentralMoments(val_shape=(), mom=(4,))>\n",
@@ -2419,15 +2323,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-639bbd63-edc7-481d-ba87-ab9450d139f2' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-639bbd63-edc7-481d-ba87-ab9450d139f2' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-54d20124-5559-4266-8369-399b5ff7f30b' class='xr-array-in' type='checkbox' checked><label for='section-54d20124-5559-4266-8369-399b5ff7f30b' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 4</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-58398e27-ba0c-46b3-ad55-0d12480f843e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-58398e27-ba0c-46b3-ad55-0d12480f843e' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-03f34279-57b8-45cd-88bd-a8ee56564468' class='xr-array-in' type='checkbox' checked><label for='section-03f34279-57b8-45cd-88bd-a8ee56564468' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>500.0 0.4919 0.08896 0.0001387 0.01378</span></div><div class='xr-array-data'><pre>array([5.000000e+02, 4.919195e-01, 8.895944e-02, 1.387264e-04, 1.377840e-02])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(4,))>\n",
                             "array([5.0000e+02, 4.9192e-01, 8.8959e-02, 1.3873e-04, 1.3778e-02])"
                         ]
                     },
                     "execution_count": 14,
@@ -2441,32 +2345,25 @@
                 "\n",
                 "c_tot = cs[0] + cs[1] + cs[2] + cs[3]\n",
                 "c_tot"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "97085b70",
+            "id": "25",
             "metadata": {},
             "source": [
                 "Or more simply:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "id": "39a9d1c8",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.940550Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.940351Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.944000Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.943339Z"
-                }
-            },
+            "id": "26",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[5.0000e+02 4.9192e-01 8.8959e-02 1.3873e-04 1.3778e-02]\n"
                     ]
@@ -2474,42 +2371,35 @@
             ],
             "source": [
                 "print(sum(cs, start=cs[0].zeros_like()).values)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "86964e2f",
+            "id": "27",
             "metadata": {},
             "source": [
                 "Very cool!"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b9eddbb0",
+            "id": "28",
             "metadata": {},
             "source": [
                 "## weighted averages\n",
                 "\n",
                 "cmomy is setup to work with arbitrary weights.  We saw this work above when we considered unequal sample sizes.  For example,"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
-            "id": "b2ed66e7",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.946999Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.946798Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.951432Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.950849Z"
-                }
-            },
+            "id": "29",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "def get_cmom_with_weights(x, w, axis=0, mom=3):\n",
                 "    \"\"\"Create central moments using stable method\"\"\"\n",
                 "    # output shape\n",
                 "    shape = x.shape[:axis] + x.shape[axis + 1 :] + (mom + 1,)\n",
                 "    output = np.zeros(shape, dtype=x.dtype)\n",
@@ -2529,23 +2419,16 @@
                 "\n",
                 "    return output"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
-            "id": "48a3fab7",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.954589Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.954386Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.962269Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.961797Z"
-                }
-            },
+            "id": "30",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -2905,15 +2788,15 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>array([4.8363e+01, 5.0295e-01, 9.2209e-02, 6.3664e-04])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-62d1a2e3-de55-4c0c-9f6f-e0598a5f8015' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-62d1a2e3-de55-4c0c-9f6f-e0598a5f8015' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-bc0af5f2-ef69-476c-92dd-f0ddba710790' class='xr-array-in' type='checkbox' checked><label for='section-bc0af5f2-ef69-476c-92dd-f0ddba710790' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>48.36 0.503 0.09221 0.0006366</span></div><div class='xr-array-data'><pre>array([4.836319e+01, 5.029529e-01, 9.220858e-02, 6.366441e-04])</pre></div></div></li></ul></div></div>"
+                            "</style><pre class='xr-text-repr-fallback'>array([4.8363e+01, 5.0295e-01, 9.2209e-02, 6.3664e-04])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-0f36ec1d-8134-4962-8809-6c01c476a842' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-0f36ec1d-8134-4962-8809-6c01c476a842' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-27ffb660-658e-4950-90c9-d7074b6b5271' class='xr-array-in' type='checkbox' checked><label for='section-27ffb660-658e-4950-90c9-d7074b6b5271' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>48.36 0.503 0.09221 0.0006366</span></div><div class='xr-array-data'><pre>array([4.836319e+01, 5.029529e-01, 9.220858e-02, 6.366441e-04])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(3,))>\n",
                             "array([4.8363e+01, 5.0295e-01, 9.2209e-02, 6.3664e-04])"
                         ]
                     },
                     "execution_count": 17,
@@ -2929,35 +2812,28 @@
                 "moments\n",
                 "\n",
                 "cmomy.CentralMoments.from_vals(x, w=w, mom=3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "10b913f0",
+            "id": "31",
             "metadata": {},
             "source": [
                 "## comoments\n",
                 "\n",
                 "cmomy can also handle comoments (covariance, etc), like the $\\ave{(\\delta x)^i (\\delta y)^j}$    \n",
                 "For example"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
-            "id": "88bf86b5",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.964847Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.964672Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.972176Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.971719Z"
-                }
-            },
+            "id": "32",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -3319,15 +3195,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>array([[ 4.8363e+01,  4.8516e-01,  7.5856e-02],\n",
                             "       [ 5.0295e-01, -1.2237e-02,  3.2919e-04],\n",
-                            "       [ 9.2209e-02, -4.2304e-03,  6.5653e-03]])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: (2, 2)</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-0bf58349-b1ce-4b1f-8159-86e8a4ab277f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-0bf58349-b1ce-4b1f-8159-86e8a4ab277f' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4b5e453b-f97c-4757-923b-e35f49e64db4' class='xr-array-in' type='checkbox' checked><label for='section-4b5e453b-f97c-4757-923b-e35f49e64db4' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>48.36 0.4852 0.07586 0.503 ... 0.0003292 0.09221 -0.00423 0.006565</span></div><div class='xr-array-data'><pre>array([[ 4.836319e+01,  4.851622e-01,  7.585550e-02],\n",
+                            "       [ 9.2209e-02, -4.2304e-03,  6.5653e-03]])</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>CentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: (2, 2)</li></ul><div class='xr-obj-type'><class 'numpy.ndarray'></div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-7d8fed40-6d81-4032-97ff-a70a82ee942f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7d8fed40-6d81-4032-97ff-a70a82ee942f' class='xr-section-summary'  title='Expand/collapse section'>Info: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-5d13cf05-3db6-4332-801c-a141e1b1edab' class='xr-array-in' type='checkbox' checked><label for='section-5d13cf05-3db6-4332-801c-a141e1b1edab' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>48.36 0.4852 0.07586 0.503 ... 0.0003292 0.09221 -0.00423 0.006565</span></div><div class='xr-array-data'><pre>array([[ 4.836319e+01,  4.851622e-01,  7.585550e-02],\n",
                             "       [ 5.029529e-01, -1.223740e-02,  3.291919e-04],\n",
                             "       [ 9.220858e-02, -4.230387e-03,  6.565301e-03]])</pre></div></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<CentralMoments(val_shape=(), mom=(2, 2))>\n",
                             "array([[ 4.8363e+01,  4.8516e-01,  7.5856e-02],\n",
                             "       [ 5.0295e-01, -1.2237e-02,  3.2919e-04],\n",
@@ -3343,42 +3219,35 @@
                 "y = rng.random(100)\n",
                 "\n",
                 "cmomy.CentralMoments.from_vals(x=(x, y), w=w, mom=(2, 2))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bef2cea4",
+            "id": "33",
             "metadata": {},
             "source": [
                 "All the special sauce works for central moments or comoments.  "
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "eadaedc2",
+            "id": "34",
             "metadata": {},
             "source": [
                 "## xarray DataArray support\n",
                 "\n",
                 "cmomy also works with {class}`xarray.DataArray` objects.  For example"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
-            "id": "cc5e273d",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.974878Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.974695Z",
-                    "iopub.status.idle": "2024-02-21T00:39:16.980619Z",
-                    "shell.execute_reply": "2024-02-21T00:39:16.980067Z"
-                }
-            },
+            "id": "35",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -3747,22 +3616,22 @@
                             "        [0.4284, 0.4153, 0.0854]],\n",
                             "\n",
                             "       [[0.0821, 0.587 , 0.0041],\n",
                             "        [0.7317, 0.3686, 0.2628]],\n",
                             "\n",
                             "       [[0.951 , 0.0224, 0.627 ],\n",
                             "        [0.0179, 0.382 , 0.3126]]])\n",
-                            "Dimensions without coordinates: rec, a, b</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 3</li><li><span>a</span>: 2</li><li><span>b</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-26b5c123-70a5-4704-a678-df060dc21ec1' class='xr-array-in' type='checkbox' checked><label for='section-26b5c123-70a5-4704-a678-df060dc21ec1' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.06247 0.5585 0.01837 0.4284 0.4153 ... 0.627 0.01787 0.382 0.3126</span></div><div class='xr-array-data'><pre>array([[[0.0625, 0.5585, 0.0184],\n",
+                            "Dimensions without coordinates: rec, a, b</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 3</li><li><span>a</span>: 2</li><li><span>b</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-45bd465c-69d9-4a8b-bee6-f8ce812560c1' class='xr-array-in' type='checkbox' checked><label for='section-45bd465c-69d9-4a8b-bee6-f8ce812560c1' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.06247 0.5585 0.01837 0.4284 0.4153 ... 0.627 0.01787 0.382 0.3126</span></div><div class='xr-array-data'><pre>array([[[0.0625, 0.5585, 0.0184],\n",
                             "        [0.4284, 0.4153, 0.0854]],\n",
                             "\n",
                             "       [[0.0821, 0.587 , 0.0041],\n",
                             "        [0.7317, 0.3686, 0.2628]],\n",
                             "\n",
                             "       [[0.951 , 0.0224, 0.627 ],\n",
-                            "        [0.0179, 0.382 , 0.3126]]])</pre></div></div></li><li class='xr-section-item'><input id='section-223a2c0e-eeea-4906-99dc-41169dd4d965' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-223a2c0e-eeea-4906-99dc-41169dd4d965' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-4c9496cb-206b-4e88-9155-474aea04d39d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4c9496cb-206b-4e88-9155-474aea04d39d' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-65b9a8c0-e6db-4037-b2b3-45637a6a866b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-65b9a8c0-e6db-4037-b2b3-45637a6a866b' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "        [0.0179, 0.382 , 0.3126]]])</pre></div></div></li><li class='xr-section-item'><input id='section-a5478acf-62ca-4ffc-8e67-7ecb9aeea777' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a5478acf-62ca-4ffc-8e67-7ecb9aeea777' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-fd8871c1-46a5-4e5f-a167-78f33ac2c2f4' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-fd8871c1-46a5-4e5f-a167-78f33ac2c2f4' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-93f9eb92-94c9-45fc-99e8-478f36a79fd0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-93f9eb92-94c9-45fc-99e8-478f36a79fd0' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (rec: 3, a: 2, b: 3)> Size: 144B\n",
                             "array([[[0.0625, 0.5585, 0.0184],\n",
                             "        [0.4284, 0.4153, 0.0854]],\n",
                             "\n",
                             "       [[0.0821, 0.587 , 0.0041],\n",
@@ -3783,32 +3652,25 @@
                 "\n",
                 "x = xr.DataArray(rng.random((100, 2, 3)), dims=[\"rec\", \"a\", \"b\"])\n",
                 "x.head(3)  # type: ignore[attr-defined]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9f50accd",
+            "id": "36",
             "metadata": {},
             "source": [
                 "To create a cmomy object wrapping a {class}`xarray.DataArray`, use {class}`~cmomy.xCentralMoments`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
-            "id": "38a244b6",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:16.983156Z",
-                    "iopub.status.busy": "2024-02-21T00:39:16.982983Z",
-                    "iopub.status.idle": "2024-02-21T00:39:17.015211Z",
-                    "shell.execute_reply": "2024-02-21T00:39:17.014299Z"
-                }
-            },
+            "id": "37",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -4176,15 +4038,15 @@
                             "array([[[1.0000e+02, 4.0657e-01, 9.0470e-02, 1.3814e-02],\n",
                             "        [1.0000e+02, 4.9516e-01, 7.3811e-02, 1.1677e-03],\n",
                             "        [1.0000e+02, 4.6592e-01, 8.1210e-02, 3.3827e-03]],\n",
                             "\n",
                             "       [[1.0000e+02, 4.8831e-01, 8.2432e-02, 1.6465e-04],\n",
                             "        [1.0000e+02, 4.6920e-01, 9.2950e-02, 5.5999e-03],\n",
                             "        [1.0000e+02, 4.8891e-01, 7.6961e-02, 2.3232e-03]]])\n",
-                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: (2, 3)</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-b59da6fd-6f04-4caf-8287-3aa1490f4aa7' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b59da6fd-6f04-4caf-8287-3aa1490f4aa7' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>(a, b)</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: (2, 3)</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-44e26728-9b71-4749-a95b-c45eb6afc75f' class='xr-section-summary-in' type='checkbox'  checked><label for='section-44e26728-9b71-4749-a95b-c45eb6afc75f' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>(a, b)</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -4547,21 +4409,21 @@
                             "array([[[1.0000e+02, 4.0657e-01, 9.0470e-02, 1.3814e-02],\n",
                             "        [1.0000e+02, 4.9516e-01, 7.3811e-02, 1.1677e-03],\n",
                             "        [1.0000e+02, 4.6592e-01, 8.1210e-02, 3.3827e-03]],\n",
                             "\n",
                             "       [[1.0000e+02, 4.8831e-01, 8.2432e-02, 1.6465e-04],\n",
                             "        [1.0000e+02, 4.6920e-01, 9.2950e-02, 5.5999e-03],\n",
                             "        [1.0000e+02, 4.8891e-01, 7.6961e-02, 2.3232e-03]]])\n",
-                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>a</span>: 2</li><li><span>b</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-19e87ed5-a338-4d12-a14d-24f600bad700' class='xr-array-in' type='checkbox' checked><label for='section-19e87ed5-a338-4d12-a14d-24f600bad700' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>100.0 0.4066 0.09047 0.01381 100.0 ... 100.0 0.4889 0.07696 0.002323</span></div><div class='xr-array-data'><pre>array([[[1.0000e+02, 4.0657e-01, 9.0470e-02, 1.3814e-02],\n",
+                            "Dimensions without coordinates: a, b, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>a</span>: 2</li><li><span>b</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4e3d0f98-e860-4e6f-b422-8586464cf18b' class='xr-array-in' type='checkbox' checked><label for='section-4e3d0f98-e860-4e6f-b422-8586464cf18b' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>100.0 0.4066 0.09047 0.01381 100.0 ... 100.0 0.4889 0.07696 0.002323</span></div><div class='xr-array-data'><pre>array([[[1.0000e+02, 4.0657e-01, 9.0470e-02, 1.3814e-02],\n",
                             "        [1.0000e+02, 4.9516e-01, 7.3811e-02, 1.1677e-03],\n",
                             "        [1.0000e+02, 4.6592e-01, 8.1210e-02, 3.3827e-03]],\n",
                             "\n",
                             "       [[1.0000e+02, 4.8831e-01, 8.2432e-02, 1.6465e-04],\n",
                             "        [1.0000e+02, 4.6920e-01, 9.2950e-02, 5.5999e-03],\n",
-                            "        [1.0000e+02, 4.8891e-01, 7.6961e-02, 2.3232e-03]]])</pre></div></div></li><li class='xr-section-item'><input id='section-a971a035-39c8-4a9e-b522-b013446a77d8' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a971a035-39c8-4a9e-b522-b013446a77d8' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-210df2f3-a5fe-4074-956a-53222085cae0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-210df2f3-a5fe-4074-956a-53222085cae0' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-c6aba503-c146-42ea-96cc-fe9af4314c72' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c6aba503-c146-42ea-96cc-fe9af4314c72' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "        [1.0000e+02, 4.8891e-01, 7.6961e-02, 2.3232e-03]]])</pre></div></div></li><li class='xr-section-item'><input id='section-833e88b8-3411-438c-b840-a0ef15c71fd1' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-833e88b8-3411-438c-b840-a0ef15c71fd1' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-527192e1-0f9b-4d86-9656-64220d96c90b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-527192e1-0f9b-4d86-9656-64220d96c90b' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-6ef038df-2e31-46ef-a52c-bb18c508def9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-6ef038df-2e31-46ef-a52c-bb18c508def9' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(2, 3), mom=(3,))>\n",
                             "<xarray.DataArray (a: 2, b: 3, mom_0: 4)> Size: 192B\n",
                             "array([[[1.0000e+02, 4.0657e-01, 9.0470e-02, 1.3814e-02],\n",
                             "        [1.0000e+02, 4.9516e-01, 7.3811e-02, 1.1677e-03],\n",
                             "        [1.0000e+02, 4.6592e-01, 8.1210e-02, 3.3827e-03]],\n",
@@ -4580,28 +4442,23 @@
             "source": [
                 "c = cmomy.xCentralMoments.from_vals(x, dim=\"rec\", mom=3)\n",
                 "c"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f38b8581",
+            "id": "38",
             "metadata": {},
             "source": [
                 "Everything that {class}`~cmomy.CentralMoments` can do, {class}`~cmomy.xCentralMoments` can do."
             ]
         }
     ],
     "metadata": {
         "celltoolbar": "Tags",
-        "kernelspec": {
-            "display_name": "Python [venv: cmomy-dev]",
-            "language": "python",
-            "name": "cmomy-dev"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/examples/usage/usage_notebook.ipynb` & `cmomy-0.9.0/examples/usage/usage_notebook.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9468253423470643%*

 * *Differences: {"'cells'": "{0: {'id': '0', 'metadata': {delete: ['execution']}}, 1: {'id': '1', 'metadata': "*

 * *            "{delete: ['execution']}}, 2: {'id': '2', 'metadata': {delete: ['execution']}}, 3: "*

 * *            "{'id': '3'}, 4: {'id': '4', 'metadata': {replace: OrderedDict()}}, 5: {'id': '5', "*

 * *            "'metadata': {replace: OrderedDict()}, 'outputs': {1: {'data': {'text/html': {insert: "*

 * *            "[(365, 'Dimensions without coordinates: mom_0</pre><div class=\\'xr-wrap\\' "*

 * *            "style=\\'display:n […]*

```diff
@@ -1,20 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "5b49b6f2",
+            "id": "0",
             "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.158905Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.158567Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.166856Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.166269Z"
-                },
                 "tags": [
                     "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# mypy: disable-error-code=\"no-untyped-def, no-untyped-call\"\n",
@@ -30,22 +24,16 @@
                 "\n",
                 "os.environ[\"NUMBA_CACHE_DIR\"] = str(p / \".numba_cache\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "05468c0e",
+            "id": "1",
             "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.170041Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.169831Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.175569Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.175075Z"
-                },
                 "tags": [
                     "remove-cell"
                 ]
             },
             "outputs": [
                 {
                     "data": {
@@ -72,56 +60,43 @@
                 "    }\n",
                 "</style>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "4d374871",
+            "id": "2",
             "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.179032Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.178841Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.250503Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.250038Z"
-                },
                 "tags": [
                     "remove-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "np.set_printoptions(precision=4)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3a2a0582",
+            "id": "3",
             "metadata": {},
             "source": [
                 "# Usage\n",
                 "\n",
                 "The basic usage of cmomy is to manipulate central moments.  \n",
                 "We measure two quantities pretend quantities.  The 'energy' and the 'position' of a thing.  We'll construct the average value for each record. Lets say 100 samples each.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "a1b581d2",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.253671Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.253464Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.920233Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.919750Z"
-                }
-            },
+            "id": "4",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import xarray as xr\n",
                 "\n",
                 "import cmomy\n",
                 "\n",
@@ -139,23 +114,16 @@
                 "ce = cmomy.xCentralMoments.from_vals(x=energy, w=w, dim=\"samp\", mom=3)\n",
                 "cp = cmomy.xCentralMoments.from_vals(x=position, w=w, dim=\"samp\", mom=3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "d61a143f",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.923128Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.922855Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.930665Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.930152Z"
-                }
-            },
+            "id": "5",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "energy\n"
                     ]
@@ -524,15 +492,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5d85ddb0-b6bb-45d6-a34f-8c3e3b936655' class='xr-section-summary-in' type='checkbox'  checked><label for='section-5d85ddb0-b6bb-45d6-a34f-8c3e3b936655' class='xr-section-summary' >Info: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c423ca91-486d-41ea-806e-b785deeccb8a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c423ca91-486d-41ea-806e-b785deeccb8a' class='xr-section-summary' >Info: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -889,15 +857,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-4540fb0b-981e-4ce8-b5b8-b2a7de80780d' class='xr-array-in' type='checkbox' checked><label for='section-4540fb0b-981e-4ce8-b5b8-b2a7de80780d' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.11 0.5531 0.08638 -0.005746</span></div><div class='xr-array-data'><pre>array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])</pre></div></div></li><li class='xr-section-item'><input id='section-530bc122-05c5-476a-b7f1-47b90728eb08' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-530bc122-05c5-476a-b7f1-47b90728eb08' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-daada294-5015-4405-b2f2-d889a45397e9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-daada294-5015-4405-b2f2-d889a45397e9' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-974a7258-ea39-4442-9dba-253904dd3631' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-974a7258-ea39-4442-9dba-253904dd3631' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b820e168-fda8-4aee-a193-4bd2b56dfa83' class='xr-array-in' type='checkbox' checked><label for='section-b820e168-fda8-4aee-a193-4bd2b56dfa83' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.11 0.5531 0.08638 -0.005746</span></div><div class='xr-array-data'><pre>array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])</pre></div></div></li><li class='xr-section-item'><input id='section-f388a6aa-a4d3-48db-b459-4fde9de3b86a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f388a6aa-a4d3-48db-b459-4fde9de3b86a' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-0308069f-2dd5-4cdd-8721-0ff579fca5bd' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-0308069f-2dd5-4cdd-8721-0ff579fca5bd' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-b1fe9a4f-b1e3-4771-bc20-9ed84b7f009d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-b1fe9a4f-b1e3-4771-bc20-9ed84b7f009d' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(), mom=(3,))>\n",
                             "<xarray.DataArray (mom_0: 4)> Size: 32B\n",
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])\n",
                             "Dimensions without coordinates: mom_0"
                         ]
@@ -911,23 +879,16 @@
                 "print(\"energy\")\n",
                 "ce"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "fdf0d672",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.933629Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.933344Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.939905Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.939477Z"
-                }
-            },
+            "id": "6",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "position\n"
                     ]
@@ -1298,15 +1259,15 @@
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (dim: 3, mom_0: 4)&gt; Size: 96B\n",
                             "array([[ 5.3105e+01,  5.2437e-01,  6.9091e-02, -5.5768e-04],\n",
                             "       [ 5.3105e+01,  4.9062e-01,  9.5523e-02,  2.2967e-03],\n",
                             "       [ 5.3105e+01,  5.6372e-01,  8.7545e-02, -8.3042e-03]])\n",
-                            "Dimensions without coordinates: dim, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-719e06c9-5e14-42e6-93b9-699b26e8498a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-719e06c9-5e14-42e6-93b9-699b26e8498a' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>dim</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: dim, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-0272b16c-fe70-4ab6-b65e-b9b76f985e7c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-0272b16c-fe70-4ab6-b65e-b9b76f985e7c' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>dim</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -1665,17 +1626,17 @@
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (dim: 3, mom_0: 4)&gt; Size: 96B\n",
                             "array([[ 5.3105e+01,  5.2437e-01,  6.9091e-02, -5.5768e-04],\n",
                             "       [ 5.3105e+01,  4.9062e-01,  9.5523e-02,  2.2967e-03],\n",
                             "       [ 5.3105e+01,  5.6372e-01,  8.7545e-02, -8.3042e-03]])\n",
-                            "Dimensions without coordinates: dim, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>dim</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-881f530d-bfce-4423-bafe-68fee300420e' class='xr-array-in' type='checkbox' checked><label for='section-881f530d-bfce-4423-bafe-68fee300420e' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.11 0.5244 0.06909 -0.0005577 ... 53.11 0.5637 0.08754 -0.008304</span></div><div class='xr-array-data'><pre>array([[ 5.3105e+01,  5.2437e-01,  6.9091e-02, -5.5768e-04],\n",
+                            "Dimensions without coordinates: dim, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>dim</span>: 3</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-04c6be0a-f6d8-413b-b117-61258963aa93' class='xr-array-in' type='checkbox' checked><label for='section-04c6be0a-f6d8-413b-b117-61258963aa93' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.11 0.5244 0.06909 -0.0005577 ... 53.11 0.5637 0.08754 -0.008304</span></div><div class='xr-array-data'><pre>array([[ 5.3105e+01,  5.2437e-01,  6.9091e-02, -5.5768e-04],\n",
                             "       [ 5.3105e+01,  4.9062e-01,  9.5523e-02,  2.2967e-03],\n",
-                            "       [ 5.3105e+01,  5.6372e-01,  8.7545e-02, -8.3042e-03]])</pre></div></div></li><li class='xr-section-item'><input id='section-879997dc-81b2-46ee-b145-ca043f2d0300' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-879997dc-81b2-46ee-b145-ca043f2d0300' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-4000727d-269a-4797-9636-a84d2b426a14' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4000727d-269a-4797-9636-a84d2b426a14' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-a15e2866-4ae6-425b-b024-955b831c0bca' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a15e2866-4ae6-425b-b024-955b831c0bca' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [ 5.3105e+01,  5.6372e-01,  8.7545e-02, -8.3042e-03]])</pre></div></div></li><li class='xr-section-item'><input id='section-1a162ffc-4fa6-46ba-bdb8-ea43522bc9f1' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1a162ffc-4fa6-46ba-bdb8-ea43522bc9f1' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-bccab401-e3a2-471f-97cd-cfc2fc87fccd' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-bccab401-e3a2-471f-97cd-cfc2fc87fccd' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-0336bbc7-9dbc-4eaf-92f1-e3e7b7c94609' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-0336bbc7-9dbc-4eaf-92f1-e3e7b7c94609' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(3,), mom=(3,))>\n",
                             "<xarray.DataArray (dim: 3, mom_0: 4)> Size: 96B\n",
                             "array([[ 5.3105e+01,  5.2437e-01,  6.9091e-02, -5.5768e-04],\n",
                             "       [ 5.3105e+01,  4.9062e-01,  9.5523e-02,  2.2967e-03],\n",
                             "       [ 5.3105e+01,  5.6372e-01,  8.7545e-02, -8.3042e-03]])\n",
@@ -1690,46 +1651,39 @@
             "source": [
                 "print(\"position\")\n",
                 "cp"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1ef3e71b",
+            "id": "7",
             "metadata": {},
             "source": [
                 "Here, we've used the constructor {meth}`cmomy.CentralMoments.from_vals`.  There are a host of other constructors to create {class}`cmomy.CentralMoments` object.  Take a look at the docs for further info."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4b712407",
+            "id": "8",
             "metadata": {},
             "source": [
                 "## Basic attributes\n",
                 "\n",
                 "Notice that there are three `shape` parameters associated with a {class}`cmomy.CentralMoments` object:\n",
                 " \n",
                 "* {attr}`cmomy.CentralMoments.mom_shape` : shape of the moments.  For single variable, tuple (mom+1,).  For comoments, (mom_0+1, mom_1+1)\n",
                 "* {attr}`cmomy.CentralMoments.val_shape`: shape of the 'values' part of the data.  For scalar data, `val_shape = ()`.  For vector data, this is the shape of the passed observation data.\n",
                 "* {attr}`cmomy.CentralMoments.shape`: total shape of wrapped moments `shape = val_shape + mom_shape`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "d28bc091",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.942500Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.942299Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.945835Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.945295Z"
-                }
-            },
+            "id": "9",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "energy shapes:\n",
@@ -1756,36 +1710,29 @@
                 "    shape    : {c.shape}\n",
                 "\"\"\"\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7b7e0efe",
+            "id": "10",
             "metadata": {},
             "source": [
                 "To access the underlying data, use the {meth}`cmomy.CentralMoments.to_numpy` method or {attr}`cmomy.CentralMoments.values` attribute.  The structure is:\n",
                 "\n",
                 "* `values[...,0]`: total weight\n",
                 "* `values[...,1]`: average/mean value\n",
                 "* `values[...,k>1]`: `kth` central moment."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "5a5dfca3",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.949544Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.949318Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.953199Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.952787Z"
-                }
-            },
+            "id": "11",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])"
                         ]
                     },
@@ -1796,32 +1743,25 @@
             ],
             "source": [
                 "ce.to_numpy()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "fe3c6187",
+            "id": "12",
             "metadata": {},
             "source": [
                 "To access all the central moments (zeroth and first included), use the {meth}`cmomy.CentralMoments.cmom` method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "32753a2c",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.955616Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.955398Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.960642Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.960213Z"
-                }
-            },
+            "id": "13",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -2183,15 +2123,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([ 1.    ,  0.    ,  0.0864, -0.0057])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-0a2aefad-5eca-49c7-a6f6-7f644062a2fa' class='xr-array-in' type='checkbox' checked><label for='section-0a2aefad-5eca-49c7-a6f6-7f644062a2fa' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1.0 0.0 0.08638 -0.005746</span></div><div class='xr-array-data'><pre>array([ 1.    ,  0.    ,  0.0864, -0.0057])</pre></div></div></li><li class='xr-section-item'><input id='section-a6a15cdf-a003-4ff3-a679-39bd846fcdc0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a6a15cdf-a003-4ff3-a679-39bd846fcdc0' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-e692b822-eab8-4747-8015-571821cc0dca' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e692b822-eab8-4747-8015-571821cc0dca' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-6f06224e-c8f4-4c17-a1f2-21716ed65f39' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-6f06224e-c8f4-4c17-a1f2-21716ed65f39' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-650a7547-27cb-4d37-a19f-8025b4801b04' class='xr-array-in' type='checkbox' checked><label for='section-650a7547-27cb-4d37-a19f-8025b4801b04' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1.0 0.0 0.08638 -0.005746</span></div><div class='xr-array-data'><pre>array([ 1.    ,  0.    ,  0.0864, -0.0057])</pre></div></div></li><li class='xr-section-item'><input id='section-26763091-9752-4c60-bcc9-c2792d7c3e4a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-26763091-9752-4c60-bcc9-c2792d7c3e4a' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-4edd06c2-064b-4700-8d5f-7b64423a04b2' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4edd06c2-064b-4700-8d5f-7b64423a04b2' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-7767fdac-b4f9-4855-9fcb-e118c69044be' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7767fdac-b4f9-4855-9fcb-e118c69044be' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (mom_0: 4)> Size: 32B\n",
                             "array([ 1.    ,  0.    ,  0.0864, -0.0057])\n",
                             "Dimensions without coordinates: mom_0"
                         ]
                     },
@@ -2202,32 +2142,25 @@
             ],
             "source": [
                 "ce.cmom()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8b8f6b3e",
+            "id": "14",
             "metadata": {},
             "source": [
                 "Likewise, the central moments can be converted to raw moments using the {meth}`cmomy.CentralMoments.rmom` method.  This uses the {mod}`cmomy.convert` module behind the scenes.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "8f466ffd",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.963141Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.962928Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.972082Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.971676Z"
-                }
-            },
+            "id": "15",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -2589,15 +2522,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([1.    , 0.5531, 0.3923, 0.3068])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-476a0205-59ee-4929-9bfb-af556eb416b1' class='xr-array-in' type='checkbox' checked><label for='section-476a0205-59ee-4929-9bfb-af556eb416b1' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1.0 0.5531 0.3923 0.3068</span></div><div class='xr-array-data'><pre>array([1.    , 0.5531, 0.3923, 0.3068])</pre></div></div></li><li class='xr-section-item'><input id='section-837ad69b-395e-4efa-9175-563440ab0e71' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-837ad69b-395e-4efa-9175-563440ab0e71' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-35e1e4f9-2959-4fd9-af81-306b10210f77' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-35e1e4f9-2959-4fd9-af81-306b10210f77' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-bb0a4873-5def-4f69-9539-c9526aac724d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-bb0a4873-5def-4f69-9539-c9526aac724d' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-31c09c70-5127-484c-bf9a-29040ab5a9db' class='xr-array-in' type='checkbox' checked><label for='section-31c09c70-5127-484c-bf9a-29040ab5a9db' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>1.0 0.5531 0.3923 0.3068</span></div><div class='xr-array-data'><pre>array([1.    , 0.5531, 0.3923, 0.3068])</pre></div></div></li><li class='xr-section-item'><input id='section-9b3e2a63-dae4-49e4-99ef-64b959928e96' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-9b3e2a63-dae4-49e4-99ef-64b959928e96' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-5cb9257d-6876-42a3-8013-b85d939f25e9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5cb9257d-6876-42a3-8013-b85d939f25e9' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-3e024674-dafd-4bb7-b2d8-6a46113d86fd' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-3e024674-dafd-4bb7-b2d8-6a46113d86fd' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (mom_0: 4)> Size: 32B\n",
                             "array([1.    , 0.5531, 0.3923, 0.3068])\n",
                             "Dimensions without coordinates: mom_0"
                         ]
                     },
@@ -2609,32 +2542,25 @@
             "source": [
                 "# <x**k>\n",
                 "ce.rmom()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4dc5b22c",
+            "id": "16",
             "metadata": {},
             "source": [
                 "Additionally, there are {class}`xarray.DataArray` like attributes"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
-            "id": "c3789330",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.974756Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.974587Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.978510Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.978107Z"
-                }
-            },
+            "id": "17",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Coordinates:\n",
                             "    *empty*"
                         ]
@@ -2647,23 +2573,16 @@
             "source": [
                 "ce.coords"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "f6baa562",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.981876Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.981428Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.984891Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.984489Z"
-                }
-            },
+            "id": "18",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{}"
                         ]
                     },
@@ -2675,23 +2594,16 @@
             "source": [
                 "ce.attrs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "id": "1d2213eb",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.987535Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.987367Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.990659Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.990286Z"
-                }
-            },
+            "id": "19",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Frozen({'mom_0': 4})"
                         ]
                     },
@@ -2703,23 +2615,16 @@
             "source": [
                 "ce.sizes"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
-            "id": "9bec61fa",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.993301Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.993146Z",
-                    "iopub.status.idle": "2024-02-21T00:39:20.996644Z",
-                    "shell.execute_reply": "2024-02-21T00:39:20.996180Z"
-                }
-            },
+            "id": "20",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "('mom_0',)"
                         ]
                     },
@@ -2730,32 +2635,25 @@
             ],
             "source": [
                 "ce.dims"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9a5e33d7",
+            "id": "21",
             "metadata": {},
             "source": [
                 "To access the underlying data use {meth}`cmomy.xCentralMoments.to_dataarray` method or {attr}`cmomy.xCentralMoments.values` attribute to access the {class}`xarray.DataArray` style data, or {meth}`cmomy.xCentralMoments.to_numpy` method to access the underlying {class}`numpy.ndarray` data.b"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "id": "bdab5661",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:20.999424Z",
-                    "iopub.status.busy": "2024-02-21T00:39:20.999225Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.004631Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.004233Z"
-                }
-            },
+            "id": "22",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -3117,15 +3015,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-3b16674c-1e12-46ec-8afb-f6874f6a29b4' class='xr-array-in' type='checkbox' checked><label for='section-3b16674c-1e12-46ec-8afb-f6874f6a29b4' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.11 0.5531 0.08638 -0.005746</span></div><div class='xr-array-data'><pre>array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])</pre></div></div></li><li class='xr-section-item'><input id='section-c32b4a59-894e-4069-b192-a9be2d6c5fc8' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c32b4a59-894e-4069-b192-a9be2d6c5fc8' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-07930f97-ba4e-48df-8b3a-114cfc8dcc60' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-07930f97-ba4e-48df-8b3a-114cfc8dcc60' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-e4936d13-c640-4a94-88b6-a117149c22b1' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e4936d13-c640-4a94-88b6-a117149c22b1' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-19eef21b-ea27-4821-b251-ddef9d8ce089' class='xr-array-in' type='checkbox' checked><label for='section-19eef21b-ea27-4821-b251-ddef9d8ce089' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.11 0.5531 0.08638 -0.005746</span></div><div class='xr-array-data'><pre>array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])</pre></div></div></li><li class='xr-section-item'><input id='section-c9202770-8a73-4ca0-8d60-78ab0a35c09b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c9202770-8a73-4ca0-8d60-78ab0a35c09b' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-bb4bfc5f-1a66-4fe4-bc97-1c3e9e2babb3' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-bb4bfc5f-1a66-4fe4-bc97-1c3e9e2babb3' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-89bf4a26-9459-4387-82a3-12642c75da57' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-89bf4a26-9459-4387-82a3-12642c75da57' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (mom_0: 4)> Size: 32B\n",
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])\n",
                             "Dimensions without coordinates: mom_0"
                         ]
                     },
@@ -3137,23 +3035,16 @@
             "source": [
                 "ce.to_dataarray()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
-            "id": "ee92652b",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.007225Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.006939Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.010986Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.010536Z"
-                }
-            },
+            "id": "23",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 5.3105e+01,  5.5314e-01,  8.6378e-02, -5.7464e-03])"
                         ]
                     },
@@ -3164,40 +3055,33 @@
             ],
             "source": [
                 "ce.to_numpy()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "25d49331",
+            "id": "24",
             "metadata": {},
             "source": [
                 "## Manipulating (co)moments"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9a362f2a",
+            "id": "25",
             "metadata": {},
             "source": [
                 "So we have our averages.  Cool.  Not very special.  But what if instead we repeat our experiment.  Let's say we did the experiment 10 times each time giving a single record.   Then our data would look like"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
-            "id": "51bc711e",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.014089Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.013884Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.026813Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.026237Z"
-                }
-            },
+            "id": "26",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nsamp = 100\n",
                 "nrec = 10\n",
                 "energy = xr.DataArray(rng.random((nrec, nsamp)), dims=[\"rec\", \"samp\"])\n",
                 "position = xr.DataArray(rng.random((nrec, nsamp, 3)), dims=[\"rec\", \"samp\", \"dim\"])\n",
                 "\n",
@@ -3207,32 +3091,25 @@
                 "# average over the samples\n",
                 "ce = cmomy.xCentralMoments.from_vals(x=energy, w=w, dim=\"samp\", mom=3)\n",
                 "cp = cmomy.xCentralMoments.from_vals(x=position, w=w, dim=\"samp\", mom=3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d4dbeeeb",
+            "id": "27",
             "metadata": {},
             "source": [
                 "Consider just the energy.  We suspect that there is some correlation between the experiments (they where done in rapid succession).  So we'd like to consider two adjacent experiments as one experiment.  For this, we can use the {meth}`cmomy.xCentralMoments.block` method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
-            "id": "9cff75a0",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.029727Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.029399Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.036235Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.035658Z"
-                }
-            },
+            "id": "28",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -3603,15 +3480,15 @@
                             "       [ 5.0303e+01,  5.3773e-01,  6.9736e-02, -6.0640e-03],\n",
                             "       [ 4.8231e+01,  5.2371e-01,  7.8316e-02, -3.9247e-03],\n",
                             "       [ 5.1988e+01,  4.4939e-01,  8.1112e-02,  3.2211e-03],\n",
                             "       [ 4.6908e+01,  4.9788e-01,  9.3582e-02, -4.0934e-03],\n",
                             "       [ 5.4791e+01,  4.8149e-01,  8.2545e-02,  8.0189e-04],\n",
                             "       [ 5.3189e+01,  4.6463e-01,  9.5055e-02,  3.3487e-03],\n",
                             "       [ 5.1267e+01,  5.4169e-01,  9.3554e-02, -4.9880e-03]])\n",
-                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 10</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-239e27b3-f72d-443c-8e3b-0bdce2561803' class='xr-section-summary-in' type='checkbox'  checked><label for='section-239e27b3-f72d-443c-8e3b-0bdce2561803' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rec</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 10</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-03b5f2b2-65d4-4138-b3fe-0c52f3f20fdc' class='xr-section-summary-in' type='checkbox'  checked><label for='section-03b5f2b2-65d4-4138-b3fe-0c52f3f20fdc' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rec</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -3977,24 +3854,24 @@
                             "       [ 5.0303e+01,  5.3773e-01,  6.9736e-02, -6.0640e-03],\n",
                             "       [ 4.8231e+01,  5.2371e-01,  7.8316e-02, -3.9247e-03],\n",
                             "       [ 5.1988e+01,  4.4939e-01,  8.1112e-02,  3.2211e-03],\n",
                             "       [ 4.6908e+01,  4.9788e-01,  9.3582e-02, -4.0934e-03],\n",
                             "       [ 5.4791e+01,  4.8149e-01,  8.2545e-02,  8.0189e-04],\n",
                             "       [ 5.3189e+01,  4.6463e-01,  9.5055e-02,  3.3487e-03],\n",
                             "       [ 5.1267e+01,  5.4169e-01,  9.3554e-02, -4.9880e-03]])\n",
-                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 10</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-73094e1e-6f4e-491c-b8b1-4df974ce102a' class='xr-array-in' type='checkbox' checked><label for='section-73094e1e-6f4e-491c-b8b1-4df974ce102a' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.06 0.4729 0.08008 0.006516 46.74 ... 51.27 0.5417 0.09355 -0.004988</span></div><div class='xr-array-data'><pre>array([[ 5.3064e+01,  4.7292e-01,  8.0077e-02,  6.5155e-03],\n",
+                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 10</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-68f30ddb-aac2-4c16-b0a7-b0e8031f957a' class='xr-array-in' type='checkbox' checked><label for='section-68f30ddb-aac2-4c16-b0a7-b0e8031f957a' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>53.06 0.4729 0.08008 0.006516 46.74 ... 51.27 0.5417 0.09355 -0.004988</span></div><div class='xr-array-data'><pre>array([[ 5.3064e+01,  4.7292e-01,  8.0077e-02,  6.5155e-03],\n",
                             "       [ 4.6744e+01,  4.7915e-01,  7.8450e-02,  1.8555e-03],\n",
                             "       [ 5.3254e+01,  5.0665e-01,  9.3529e-02,  2.1183e-03],\n",
                             "       [ 5.0303e+01,  5.3773e-01,  6.9736e-02, -6.0640e-03],\n",
                             "       [ 4.8231e+01,  5.2371e-01,  7.8316e-02, -3.9247e-03],\n",
                             "       [ 5.1988e+01,  4.4939e-01,  8.1112e-02,  3.2211e-03],\n",
                             "       [ 4.6908e+01,  4.9788e-01,  9.3582e-02, -4.0934e-03],\n",
                             "       [ 5.4791e+01,  4.8149e-01,  8.2545e-02,  8.0189e-04],\n",
                             "       [ 5.3189e+01,  4.6463e-01,  9.5055e-02,  3.3487e-03],\n",
-                            "       [ 5.1267e+01,  5.4169e-01,  9.3554e-02, -4.9880e-03]])</pre></div></div></li><li class='xr-section-item'><input id='section-6f3aa89c-627b-40e7-9141-1cd97f30fc6c' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-6f3aa89c-627b-40e7-9141-1cd97f30fc6c' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-19e69b53-f696-4514-ba10-a4f8170c546d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-19e69b53-f696-4514-ba10-a4f8170c546d' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-0130af1a-904d-4017-bf2a-7d126bbf0ca1' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-0130af1a-904d-4017-bf2a-7d126bbf0ca1' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [ 5.1267e+01,  5.4169e-01,  9.3554e-02, -4.9880e-03]])</pre></div></div></li><li class='xr-section-item'><input id='section-3647b209-1176-4148-bd47-e650b703e549' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-3647b209-1176-4148-bd47-e650b703e549' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-1975fda1-8e8a-4ae4-ba22-7f2edb21462a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1975fda1-8e8a-4ae4-ba22-7f2edb21462a' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-8a2100f4-4ab0-40a2-9063-7751df420c00' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-8a2100f4-4ab0-40a2-9063-7751df420c00' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(10,), mom=(3,))>\n",
                             "<xarray.DataArray (rec: 10, mom_0: 4)> Size: 320B\n",
                             "array([[ 5.3064e+01,  4.7292e-01,  8.0077e-02,  6.5155e-03],\n",
                             "       [ 4.6744e+01,  4.7915e-01,  7.8450e-02,  1.8555e-03],\n",
                             "       [ 5.3254e+01,  5.0665e-01,  9.3529e-02,  2.1183e-03],\n",
@@ -4016,23 +3893,16 @@
             "source": [
                 "ce"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
-            "id": "7c55f5dc",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.038609Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.038439Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.046904Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.046225Z"
-                }
-            },
+            "id": "29",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -4398,15 +4268,15 @@
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (rec: 5, mom_0: 4)&gt; Size: 160B\n",
                             "array([[ 9.9808e+01,  4.7583e-01,  7.9325e-02,  4.3255e-03],\n",
                             "       [ 1.0356e+02,  5.2174e-01,  8.2213e-02, -2.4102e-03],\n",
                             "       [ 1.0022e+02,  4.8515e-01,  8.1146e-02, -3.6968e-04],\n",
                             "       [ 1.0170e+02,  4.8905e-01,  8.7702e-02, -1.3211e-03],\n",
                             "       [ 1.0446e+02,  5.0245e-01,  9.5802e-02, -8.2761e-04]])\n",
-                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 5</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-8b3300ec-bd44-48c1-bfb5-9c7b1b0703bc' class='xr-section-summary-in' type='checkbox'  checked><label for='section-8b3300ec-bd44-48c1-bfb5-9c7b1b0703bc' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rec</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 5</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-af3900e8-3da3-4a8a-bc57-42e7b56d19db' class='xr-section-summary-in' type='checkbox'  checked><label for='section-af3900e8-3da3-4a8a-bc57-42e7b56d19db' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rec</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -4767,19 +4637,19 @@
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (rec: 5, mom_0: 4)&gt; Size: 160B\n",
                             "array([[ 9.9808e+01,  4.7583e-01,  7.9325e-02,  4.3255e-03],\n",
                             "       [ 1.0356e+02,  5.2174e-01,  8.2213e-02, -2.4102e-03],\n",
                             "       [ 1.0022e+02,  4.8515e-01,  8.1146e-02, -3.6968e-04],\n",
                             "       [ 1.0170e+02,  4.8905e-01,  8.7702e-02, -1.3211e-03],\n",
                             "       [ 1.0446e+02,  5.0245e-01,  9.5802e-02, -8.2761e-04]])\n",
-                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 5</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-1d6b323c-8aeb-4f35-ba3f-25aaae4d65d8' class='xr-array-in' type='checkbox' checked><label for='section-1d6b323c-8aeb-4f35-ba3f-25aaae4d65d8' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>99.81 0.4758 0.07932 0.004325 103.6 ... 104.5 0.5025 0.0958 -0.0008276</span></div><div class='xr-array-data'><pre>array([[ 9.9808e+01,  4.7583e-01,  7.9325e-02,  4.3255e-03],\n",
+                            "Dimensions without coordinates: rec, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rec</span>: 5</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-f1f547a4-8485-4da2-873c-2c57bf8c8d4d' class='xr-array-in' type='checkbox' checked><label for='section-f1f547a4-8485-4da2-873c-2c57bf8c8d4d' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>99.81 0.4758 0.07932 0.004325 103.6 ... 104.5 0.5025 0.0958 -0.0008276</span></div><div class='xr-array-data'><pre>array([[ 9.9808e+01,  4.7583e-01,  7.9325e-02,  4.3255e-03],\n",
                             "       [ 1.0356e+02,  5.2174e-01,  8.2213e-02, -2.4102e-03],\n",
                             "       [ 1.0022e+02,  4.8515e-01,  8.1146e-02, -3.6968e-04],\n",
                             "       [ 1.0170e+02,  4.8905e-01,  8.7702e-02, -1.3211e-03],\n",
-                            "       [ 1.0446e+02,  5.0245e-01,  9.5802e-02, -8.2761e-04]])</pre></div></div></li><li class='xr-section-item'><input id='section-4993254b-93e7-4c88-9722-4b7bc98edc90' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4993254b-93e7-4c88-9722-4b7bc98edc90' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-1ef62605-e67b-4e7e-b79f-91d920680933' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1ef62605-e67b-4e7e-b79f-91d920680933' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-63fa02db-b486-4708-911d-14e39696c2c7' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-63fa02db-b486-4708-911d-14e39696c2c7' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [ 1.0446e+02,  5.0245e-01,  9.5802e-02, -8.2761e-04]])</pre></div></div></li><li class='xr-section-item'><input id='section-29f6ffce-cb58-4ba5-8037-659b69dc166c' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-29f6ffce-cb58-4ba5-8037-659b69dc166c' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-5a407ec8-0408-4e04-8999-0770656adfe6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5a407ec8-0408-4e04-8999-0770656adfe6' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-35e47df4-ae2b-44bf-a84d-eba5e422bad1' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-35e47df4-ae2b-44bf-a84d-eba5e422bad1' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(5,), mom=(3,))>\n",
                             "<xarray.DataArray (rec: 5, mom_0: 4)> Size: 160B\n",
                             "array([[ 9.9808e+01,  4.7583e-01,  7.9325e-02,  4.3255e-03],\n",
                             "       [ 1.0356e+02,  5.2174e-01,  8.2213e-02, -2.4102e-03],\n",
                             "       [ 1.0022e+02,  4.8515e-01,  8.1146e-02, -3.6968e-04],\n",
@@ -4795,32 +4665,25 @@
             ],
             "source": [
                 "ce.block(block_size=2, dim=\"rec\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "15e753f3",
+            "id": "30",
             "metadata": {},
             "source": [
                 "Instead, we can resample the already averaged data using {meth}`cmomy.xCentralMoments.resample_and_reduce`.  We produce a 20 new samples taken from the original (averaged) data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
-            "id": "c39038a7",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.049555Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.049393Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.076494Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.075814Z"
-                }
-            },
+            "id": "31",
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "OMP: Info #276: omp_set_nested routine deprecated, please use omp_set_max_active_levels instead.\n"
                     ]
@@ -5208,15 +5071,15 @@
                             "       [ 5.2529e+02,  4.9417e-01,  8.4350e-02,  1.1154e-03],\n",
                             "       [ 4.9973e+02,  4.9879e-01,  8.9895e-02, -2.9911e-04],\n",
                             "       [ 5.0993e+02,  4.8937e-01,  8.6093e-02,  8.3597e-04],\n",
                             "       [ 5.0860e+02,  4.7908e-01,  8.5023e-02,  9.4369e-04],\n",
                             "       [ 5.0110e+02,  4.9114e-01,  8.4371e-02, -1.0724e-03],\n",
                             "       [ 5.2742e+02,  4.8909e-01,  8.5711e-02,  1.4218e-03],\n",
                             "       [ 4.9154e+02,  4.9741e-01,  8.1855e-02, -3.3717e-04]])\n",
-                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 20</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-6758162e-32c8-4eae-9b49-cb6a9366765d' class='xr-section-summary-in' type='checkbox'  checked><label for='section-6758162e-32c8-4eae-9b49-cb6a9366765d' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rep</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 20</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c3b93435-a210-44c6-87c7-23bacd7bad1b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c3b93435-a210-44c6-87c7-23bacd7bad1b' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rep</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -5592,15 +5455,15 @@
                             "       [ 5.2529e+02,  4.9417e-01,  8.4350e-02,  1.1154e-03],\n",
                             "       [ 4.9973e+02,  4.9879e-01,  8.9895e-02, -2.9911e-04],\n",
                             "       [ 5.0993e+02,  4.8937e-01,  8.6093e-02,  8.3597e-04],\n",
                             "       [ 5.0860e+02,  4.7908e-01,  8.5023e-02,  9.4369e-04],\n",
                             "       [ 5.0110e+02,  4.9114e-01,  8.4371e-02, -1.0724e-03],\n",
                             "       [ 5.2742e+02,  4.8909e-01,  8.5711e-02,  1.4218e-03],\n",
                             "       [ 4.9154e+02,  4.9741e-01,  8.1855e-02, -3.3717e-04]])\n",
-                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rep</span>: 20</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-96787b9c-4b0d-4cb7-9171-ddc3a6abdad8' class='xr-array-in' type='checkbox' checked><label for='section-96787b9c-4b0d-4cb7-9171-ddc3a6abdad8' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>498.9 0.4848 0.084 0.0007661 503.2 ... 491.5 0.4974 0.08186 -0.0003372</span></div><div class='xr-array-data'><pre>array([[ 4.9894e+02,  4.8483e-01,  8.4004e-02,  7.6615e-04],\n",
+                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rep</span>: 20</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-c6d1581a-5ee9-4f40-86ad-a912f23d05d9' class='xr-array-in' type='checkbox' checked><label for='section-c6d1581a-5ee9-4f40-86ad-a912f23d05d9' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>498.9 0.4848 0.084 0.0007661 503.2 ... 491.5 0.4974 0.08186 -0.0003372</span></div><div class='xr-array-data'><pre>array([[ 4.9894e+02,  4.8483e-01,  8.4004e-02,  7.6615e-04],\n",
                             "       [ 5.0316e+02,  5.0209e-01,  8.0869e-02, -1.1553e-04],\n",
                             "       [ 5.1114e+02,  4.8697e-01,  8.6689e-02,  1.2299e-03],\n",
                             "       [ 5.2135e+02,  4.9141e-01,  8.4228e-02, -5.7084e-04],\n",
                             "       [ 5.0592e+02,  4.9809e-01,  8.5436e-02, -8.7446e-04],\n",
                             "       [ 5.1902e+02,  4.9260e-01,  8.5149e-02,  7.5026e-04],\n",
                             "       [ 5.0659e+02,  5.0687e-01,  8.3342e-02, -2.2954e-03],\n",
                             "       [ 5.0490e+02,  4.9669e-01,  8.6755e-02, -8.1764e-04],\n",
@@ -5611,15 +5474,15 @@
                             "       [ 4.9210e+02,  4.7666e-01,  8.3947e-02,  2.1234e-03],\n",
                             "       [ 5.2529e+02,  4.9417e-01,  8.4350e-02,  1.1154e-03],\n",
                             "       [ 4.9973e+02,  4.9879e-01,  8.9895e-02, -2.9911e-04],\n",
                             "       [ 5.0993e+02,  4.8937e-01,  8.6093e-02,  8.3597e-04],\n",
                             "       [ 5.0860e+02,  4.7908e-01,  8.5023e-02,  9.4369e-04],\n",
                             "       [ 5.0110e+02,  4.9114e-01,  8.4371e-02, -1.0724e-03],\n",
                             "       [ 5.2742e+02,  4.8909e-01,  8.5711e-02,  1.4218e-03],\n",
-                            "       [ 4.9154e+02,  4.9741e-01,  8.1855e-02, -3.3717e-04]])</pre></div></div></li><li class='xr-section-item'><input id='section-5e4b1e0e-0c93-45b7-b45f-2e6bd9f7b2cd' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5e4b1e0e-0c93-45b7-b45f-2e6bd9f7b2cd' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-52c53257-7021-4d79-9fc6-3af3e4e80568' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-52c53257-7021-4d79-9fc6-3af3e4e80568' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-5ec7091a-b6ac-41e2-a86c-c5fd5f36abd5' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5ec7091a-b6ac-41e2-a86c-c5fd5f36abd5' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [ 4.9154e+02,  4.9741e-01,  8.1855e-02, -3.3717e-04]])</pre></div></div></li><li class='xr-section-item'><input id='section-bf662f15-b0b0-450a-a748-b198f08b9ad0' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-bf662f15-b0b0-450a-a748-b198f08b9ad0' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-02fbc4b9-a3d0-40fc-a423-f98705fe7cfe' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-02fbc4b9-a3d0-40fc-a423-f98705fe7cfe' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-0d7e51be-1cea-474e-965b-c1c9a6e8341d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-0d7e51be-1cea-474e-965b-c1c9a6e8341d' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(20,), mom=(3,))>\n",
                             "<xarray.DataArray (rep: 20, mom_0: 4)> Size: 640B\n",
                             "array([[ 4.9894e+02,  4.8483e-01,  8.4004e-02,  7.6615e-04],\n",
                             "       [ 5.0316e+02,  5.0209e-01,  8.0869e-02, -1.1553e-04],\n",
                             "       [ 5.1114e+02,  4.8697e-01,  8.6689e-02,  1.2299e-03],\n",
@@ -5651,66 +5514,45 @@
             "source": [
                 "ce_resamp = ce.resample_and_reduce(nrep=20, dim=\"rec\")\n",
                 "ce_resamp"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0bbe0c1c",
+            "id": "32",
             "metadata": {},
             "source": [
                 "This is different than the usual 'resample values'.  This is also available if the original data is available."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
-            "id": "c880e93b",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.081244Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.080956Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.086691Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.085938Z"
-                }
-            },
+            "id": "33",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "a = energy.stack(c=[\"rec\", \"samp\"])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
-            "id": "ce3f1b1e",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.090770Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.090343Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.094949Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.094304Z"
-                }
-            },
+            "id": "34",
+            "metadata": {},
             "outputs": [],
             "source": [
                 "b = w.stack(c=[\"rec\", \"samp\"])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
-            "id": "50c3991e",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.098283Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.098059Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.130972Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.130214Z"
-                }
-            },
+            "id": "35",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -6091,19 +5933,15 @@
                             "       [ 5.0848e+02,  4.8416e-01,  8.4131e-02,  1.9068e-05],\n",
                             "       [ 5.0767e+02,  4.9133e-01,  8.2855e-02,  1.3108e-03],\n",
                             "       [ 5.2246e+02,  4.8245e-01,  8.5488e-02,  7.4083e-05],\n",
                             "       [ 5.1387e+02,  5.0965e-01,  8.5511e-02, -1.8175e-03],\n",
                             "       [ 5.2162e+02,  4.9756e-01,  8.8069e-02, -3.8196e-04],\n",
                             "       [ 5.0263e+02,  4.9969e-01,  8.5556e-02, -2.0398e-03],\n",
                             "       [ 5.0454e+02,  5.0938e-01,  8.2281e-02, -1.8049e-03]])\n",
-                            "Coordinates:\n",
-                            "    c        object 8B (0, 0)\n",
-                            "    rec      int64 8B 0\n",
-                            "    samp     int64 8B 0\n",
-                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 20</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-53aabdd7-1f2b-4ffd-bf86-cbc1b7194f5c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-53aabdd7-1f2b-4ffd-bf86-cbc1b7194f5c' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rep</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li><li><span>val_shape</span>: 20</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-9bb8e617-f28b-4fe1-b88f-0d3b53d6b1cb' class='xr-section-summary-in' type='checkbox'  checked><label for='section-9bb8e617-f28b-4fe1-b88f-0d3b53d6b1cb' class='xr-section-summary' >Info: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd><dt><span>val_dims :</span></dt><dd>rep</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -6479,19 +6317,15 @@
                             "       [ 5.0848e+02,  4.8416e-01,  8.4131e-02,  1.9068e-05],\n",
                             "       [ 5.0767e+02,  4.9133e-01,  8.2855e-02,  1.3108e-03],\n",
                             "       [ 5.2246e+02,  4.8245e-01,  8.5488e-02,  7.4083e-05],\n",
                             "       [ 5.1387e+02,  5.0965e-01,  8.5511e-02, -1.8175e-03],\n",
                             "       [ 5.2162e+02,  4.9756e-01,  8.8069e-02, -3.8196e-04],\n",
                             "       [ 5.0263e+02,  4.9969e-01,  8.5556e-02, -2.0398e-03],\n",
                             "       [ 5.0454e+02,  5.0938e-01,  8.2281e-02, -1.8049e-03]])\n",
-                            "Coordinates:\n",
-                            "    c        object 8B (0, 0)\n",
-                            "    rec      int64 8B 0\n",
-                            "    samp     int64 8B 0\n",
-                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rep</span>: 20</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b6c3a2f7-5f57-4233-9345-48f47ac6140b' class='xr-array-in' type='checkbox' checked><label for='section-b6c3a2f7-5f57-4233-9345-48f47ac6140b' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>504.7 0.5073 0.08354 -0.001736 ... 504.5 0.5094 0.08228 -0.001805</span></div><div class='xr-array-data'><pre>array([[ 5.0470e+02,  5.0732e-01,  8.3537e-02, -1.7364e-03],\n",
+                            "Dimensions without coordinates: rep, mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>rep</span>: 20</li><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-cd5a42ef-4349-4174-b551-5a7b6666adf1' class='xr-array-in' type='checkbox' checked><label for='section-cd5a42ef-4349-4174-b551-5a7b6666adf1' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>504.7 0.5073 0.08354 -0.001736 ... 504.5 0.5094 0.08228 -0.001805</span></div><div class='xr-array-data'><pre>array([[ 5.0470e+02,  5.0732e-01,  8.3537e-02, -1.7364e-03],\n",
                             "       [ 5.1471e+02,  5.0032e-01,  8.5279e-02, -1.9318e-04],\n",
                             "       [ 5.1740e+02,  4.8807e-01,  8.1873e-02, -6.0608e-04],\n",
                             "       [ 5.2171e+02,  5.0050e-01,  8.3951e-02, -2.8801e-04],\n",
                             "       [ 5.1191e+02,  4.9601e-01,  8.5987e-02,  5.9479e-04],\n",
                             "       [ 4.9898e+02,  5.0192e-01,  8.6259e-02, -4.8733e-04],\n",
                             "       [ 5.0383e+02,  5.0676e-01,  8.4769e-02, -9.1195e-04],\n",
                             "       [ 5.3502e+02,  4.8362e-01,  8.1934e-02,  8.0303e-04],\n",
@@ -6502,15 +6336,15 @@
                             "       [ 5.0575e+02,  4.8867e-01,  8.9293e-02,  9.5625e-04],\n",
                             "       [ 5.0848e+02,  4.8416e-01,  8.4131e-02,  1.9068e-05],\n",
                             "       [ 5.0767e+02,  4.9133e-01,  8.2855e-02,  1.3108e-03],\n",
                             "       [ 5.2246e+02,  4.8245e-01,  8.5488e-02,  7.4083e-05],\n",
                             "       [ 5.1387e+02,  5.0965e-01,  8.5511e-02, -1.8175e-03],\n",
                             "       [ 5.2162e+02,  4.9756e-01,  8.8069e-02, -3.8196e-04],\n",
                             "       [ 5.0263e+02,  4.9969e-01,  8.5556e-02, -2.0398e-03],\n",
-                            "       [ 5.0454e+02,  5.0938e-01,  8.2281e-02, -1.8049e-03]])</pre></div></div></li><li class='xr-section-item'><input id='section-4cee06fe-379e-47b1-bff4-f2501179a278' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4cee06fe-379e-47b1-bff4-f2501179a278' class='xr-section-summary' >Coordinates: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>c</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>object</div><div class='xr-var-preview xr-preview'>(0, 0)</div><input id='attrs-fab514c8-8f35-4c1f-ac98-e8f460b37be1' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-fab514c8-8f35-4c1f-ac98-e8f460b37be1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-89558929-542a-4c2b-bb38-5a63a4d9d53d' class='xr-var-data-in' type='checkbox'><label for='data-89558929-542a-4c2b-bb38-5a63a4d9d53d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array((0, 0), dtype=object)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>rec</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-56ce9d17-75af-445b-8fd4-352c63996e81' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-56ce9d17-75af-445b-8fd4-352c63996e81' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a573ae60-1747-4cdc-ac64-2813c4147361' class='xr-var-data-in' type='checkbox'><label for='data-a573ae60-1747-4cdc-ac64-2813c4147361' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(0)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>samp</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-7b8b2cfe-0b4c-4aab-ab75-070c71f252de' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-7b8b2cfe-0b4c-4aab-ab75-070c71f252de' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c9b13274-2836-48c7-ae18-87202ab9509b' class='xr-var-data-in' type='checkbox'><label for='data-c9b13274-2836-48c7-ae18-87202ab9509b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(0)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-1d75a08d-79ce-445a-8543-9af97f61e18d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1d75a08d-79ce-445a-8543-9af97f61e18d' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-f2f359a0-30cd-41f3-a606-1b55491e609b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-f2f359a0-30cd-41f3-a606-1b55491e609b' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "       [ 5.0454e+02,  5.0938e-01,  8.2281e-02, -1.8049e-03]])</pre></div></div></li><li class='xr-section-item'><input id='section-c99ab27e-8a93-4788-bbd5-4bd5155fdd5b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c99ab27e-8a93-4788-bbd5-4bd5155fdd5b' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-fd6ed3b6-81f1-4ed3-81aa-078f7bc2b1f4' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-fd6ed3b6-81f1-4ed3-81aa-078f7bc2b1f4' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-531d2630-e20b-4658-9cca-e3e71884a3cb' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-531d2630-e20b-4658-9cca-e3e71884a3cb' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(20,), mom=(3,))>\n",
                             "<xarray.DataArray (rep: 20, mom_0: 4)> Size: 640B\n",
                             "array([[ 5.0470e+02,  5.0732e-01,  8.3537e-02, -1.7364e-03],\n",
                             "       [ 5.1471e+02,  5.0032e-01,  8.5279e-02, -1.9318e-04],\n",
                             "       [ 5.1740e+02,  4.8807e-01,  8.1873e-02, -6.0608e-04],\n",
@@ -6527,18 +6361,14 @@
                             "       [ 5.0848e+02,  4.8416e-01,  8.4131e-02,  1.9068e-05],\n",
                             "       [ 5.0767e+02,  4.9133e-01,  8.2855e-02,  1.3108e-03],\n",
                             "       [ 5.2246e+02,  4.8245e-01,  8.5488e-02,  7.4083e-05],\n",
                             "       [ 5.1387e+02,  5.0965e-01,  8.5511e-02, -1.8175e-03],\n",
                             "       [ 5.2162e+02,  4.9756e-01,  8.8069e-02, -3.8196e-04],\n",
                             "       [ 5.0263e+02,  4.9969e-01,  8.5556e-02, -2.0398e-03],\n",
                             "       [ 5.0454e+02,  5.0938e-01,  8.2281e-02, -1.8049e-03]])\n",
-                            "Coordinates:\n",
-                            "    c        object 8B (0, 0)\n",
-                            "    rec      int64 8B 0\n",
-                            "    samp     int64 8B 0\n",
                             "Dimensions without coordinates: rep, mom_0"
                         ]
                     },
                     "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -6553,32 +6383,25 @@
                 "    mom=3,\n",
                 ")\n",
                 "out"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e7937d89",
+            "id": "36",
             "metadata": {},
             "source": [
                 "We see that the deviation in the moments is similar using the two resampling methods:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
-            "id": "e1688a0c",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.134488Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.134253Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.142818Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.142192Z"
-                }
-            },
+            "execution_count": 25,
+            "id": "37",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -6940,51 +6763,36 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 3)&gt; Size: 24B\n",
                             "array([0.0093, 0.0021, 0.0012])\n",
-                            "Coordinates:\n",
-                            "    c        object 8B (0, 0)\n",
-                            "    rec      int64 8B 0\n",
-                            "    samp     int64 8B 0\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-55c7140c-5842-4900-90ac-a626a26aee8d' class='xr-array-in' type='checkbox' checked><label for='section-55c7140c-5842-4900-90ac-a626a26aee8d' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.00929 0.002098 0.001161</span></div><div class='xr-array-data'><pre>array([0.0093, 0.0021, 0.0012])</pre></div></div></li><li class='xr-section-item'><input id='section-b6c5db2c-b73a-4ba9-aca9-9ec51d619309' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b6c5db2c-b73a-4ba9-aca9-9ec51d619309' class='xr-section-summary' >Coordinates: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>c</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>object</div><div class='xr-var-preview xr-preview'>(0, 0)</div><input id='attrs-02b9a189-09b7-482e-9bbe-b1e9e1d456ae' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-02b9a189-09b7-482e-9bbe-b1e9e1d456ae' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-54d6e7fa-fdc6-49db-a973-e093909a83b6' class='xr-var-data-in' type='checkbox'><label for='data-54d6e7fa-fdc6-49db-a973-e093909a83b6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array((0, 0), dtype=object)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>rec</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-ae98651b-09df-4bdb-ac15-027220eb05cb' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-ae98651b-09df-4bdb-ac15-027220eb05cb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-83021abd-8218-4faa-a814-97b79b76cb9e' class='xr-var-data-in' type='checkbox'><label for='data-83021abd-8218-4faa-a814-97b79b76cb9e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(0)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>samp</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-95aac433-a2d3-4690-a367-eb0a2157e55d' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-95aac433-a2d3-4690-a367-eb0a2157e55d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c6ddbe0b-bbc7-406d-8567-1af70c931692' class='xr-var-data-in' type='checkbox'><label for='data-c6ddbe0b-bbc7-406d-8567-1af70c931692' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array(0)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-57a5993d-c30c-4c5a-b3a0-6587182d6199' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-57a5993d-c30c-4c5a-b3a0-6587182d6199' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-a745aa90-6969-473a-9524-63c9cd75da13' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a745aa90-6969-473a-9524-63c9cd75da13' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-d5687641-95c0-4ac6-bf8b-c42f4a028d08' class='xr-array-in' type='checkbox' checked><label for='section-d5687641-95c0-4ac6-bf8b-c42f4a028d08' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.00929 0.002098 0.001161</span></div><div class='xr-array-data'><pre>array([0.0093, 0.0021, 0.0012])</pre></div></div></li><li class='xr-section-item'><input id='section-19449d89-6f78-4840-9c90-2bc74b972e0e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-19449d89-6f78-4840-9c90-2bc74b972e0e' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-7008ca3c-790e-4118-b4c5-823db917f8cc' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7008ca3c-790e-4118-b4c5-823db917f8cc' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-107bee40-e319-4689-a0d2-f211e39a9e62' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-107bee40-e319-4689-a0d2-f211e39a9e62' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (mom_0: 3)> Size: 24B\n",
                             "array([0.0093, 0.0021, 0.0012])\n",
-                            "Coordinates:\n",
-                            "    c        object 8B (0, 0)\n",
-                            "    rec      int64 8B 0\n",
-                            "    samp     int64 8B 0\n",
                             "Dimensions without coordinates: mom_0"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 25,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "out.to_dataarray().sel(mom_0=slice(1, None)).std(\"rep\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
-            "id": "035b4c90",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.146148Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.145920Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.153031Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.152231Z"
-                }
-            },
+            "execution_count": 26,
+            "id": "38",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -7346,51 +7154,44 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 3)&gt; Size: 24B\n",
                             "array([0.0072, 0.0024, 0.0012])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-27e6a625-ca3b-40be-bf27-3ce3461708c2' class='xr-array-in' type='checkbox' checked><label for='section-27e6a625-ca3b-40be-bf27-3ce3461708c2' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.007201 0.002359 0.001185</span></div><div class='xr-array-data'><pre>array([0.0072, 0.0024, 0.0012])</pre></div></div></li><li class='xr-section-item'><input id='section-57119431-a66f-4098-9de5-781fcae46154' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-57119431-a66f-4098-9de5-781fcae46154' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-39ecdc89-61bd-498f-b939-4e118a143e12' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-39ecdc89-61bd-498f-b939-4e118a143e12' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-cebd1f22-6521-4abb-9859-2abc75a673b5' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-cebd1f22-6521-4abb-9859-2abc75a673b5' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b231c9bc-792d-41d2-b5c2-59fb0e350d06' class='xr-array-in' type='checkbox' checked><label for='section-b231c9bc-792d-41d2-b5c2-59fb0e350d06' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>0.007201 0.002359 0.001185</span></div><div class='xr-array-data'><pre>array([0.0072, 0.0024, 0.0012])</pre></div></div></li><li class='xr-section-item'><input id='section-bb8a2bb2-e3a5-4360-8bd6-1fd0090532bf' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-bb8a2bb2-e3a5-4360-8bd6-1fd0090532bf' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-7336cf7c-e864-4c8a-a9de-dc8d46cd6c6f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-7336cf7c-e864-4c8a-a9de-dc8d46cd6c6f' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-4865ae96-daaf-4319-8c48-ecd80be8c9ee' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4865ae96-daaf-4319-8c48-ecd80be8c9ee' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray (mom_0: 3)> Size: 24B\n",
                             "array([0.0072, 0.0024, 0.0012])\n",
                             "Dimensions without coordinates: mom_0"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ce_resamp.to_dataarray().sel(mom_0=slice(1, None)).std(\"rep\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e8c601c6",
+            "id": "39",
             "metadata": {},
             "source": [
                 "We can also reduce our original data across all the records using {meth}`cmomy.xCentralMoments.reduce`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
-            "id": "a4313486",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2024-02-21T00:39:21.156629Z",
-                    "iopub.status.busy": "2024-02-21T00:39:21.156336Z",
-                    "iopub.status.idle": "2024-02-21T00:39:21.166175Z",
-                    "shell.execute_reply": "2024-02-21T00:39:21.165542Z"
-                }
-            },
+            "execution_count": 27,
+            "id": "40",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
@@ -7752,15 +7553,15 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([ 5.0974e+02,  4.9508e-01,  8.5572e-02, -6.5659e-05])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-0abd2ffb-3908-4164-b435-cd62a057bb7c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-0abd2ffb-3908-4164-b435-cd62a057bb7c' class='xr-section-summary' >Info: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xCentralMoments</div><ul class='xr-dim-list'><li><span>mom</span>: 3</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-91cf8d9a-f636-4466-8b59-75828b36a28a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-91cf8d9a-f636-4466-8b59-75828b36a28a' class='xr-section-summary' >Info: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>mom_dims :</span></dt><dd>mom_0</dd></dl></div></li></ul></div></div><div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
                             "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
                             "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
                             "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
                             "</symbol>\n",
                             "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
@@ -8117,40 +7918,43 @@
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray (mom_0: 4)&gt; Size: 32B\n",
                             "array([ 5.0974e+02,  4.9508e-01,  8.5572e-02, -6.5659e-05])\n",
-                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-8be36ef7-7ccb-4760-aaa5-86f44e18b649' class='xr-array-in' type='checkbox' checked><label for='section-8be36ef7-7ccb-4760-aaa5-86f44e18b649' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>509.7 0.4951 0.08557 -6.566e-05</span></div><div class='xr-array-data'><pre>array([ 5.0974e+02,  4.9508e-01,  8.5572e-02, -6.5659e-05])</pre></div></div></li><li class='xr-section-item'><input id='section-b86b57bf-3020-440c-90c3-7ed3cfc39ae1' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-b86b57bf-3020-440c-90c3-7ed3cfc39ae1' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-6d0fd674-47e2-411c-955c-b277b3087d01' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-6d0fd674-47e2-411c-955c-b277b3087d01' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-75b5f1d8-dd29-4b36-8bc0-a55e27acf3ac' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-75b5f1d8-dd29-4b36-8bc0-a55e27acf3ac' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "Dimensions without coordinates: mom_0</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'></div><ul class='xr-dim-list'><li><span>mom_0</span>: 4</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-301a000c-8ebf-486d-9d27-6cdbc3aee61d' class='xr-array-in' type='checkbox' checked><label for='section-301a000c-8ebf-486d-9d27-6cdbc3aee61d' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>509.7 0.4951 0.08557 -6.566e-05</span></div><div class='xr-array-data'><pre>array([ 5.0974e+02,  4.9508e-01,  8.5572e-02, -6.5659e-05])</pre></div></div></li><li class='xr-section-item'><input id='section-79fbcd42-1188-4756-91c5-45dc95a92f58' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-79fbcd42-1188-4756-91c5-45dc95a92f58' class='xr-section-summary'  title='Expand/collapse section'>Coordinates: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-dc9af496-4fce-4097-8082-d4254d7f550c' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-dc9af496-4fce-4097-8082-d4254d7f550c' class='xr-section-summary'  title='Expand/collapse section'>Indexes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'></ul></div></li><li class='xr-section-item'><input id='section-e2e4d12e-a6d9-4290-bf63-85d8c70e07b4' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e2e4d12e-a6d9-4290-bf63-85d8c70e07b4' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xCentralMoments(val_shape=(), mom=(3,))>\n",
                             "<xarray.DataArray (mom_0: 4)> Size: 32B\n",
                             "array([ 5.0974e+02,  4.9508e-01,  8.5572e-02, -6.5659e-05])\n",
                             "Dimensions without coordinates: mom_0"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ce.reduce(dim=\"rec\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "41",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "celltoolbar": "Tags",
-        "kernelspec": {
-            "display_name": "Python [venv: cmomy-dev]",
-            "language": "python",
-            "name": "cmomy-dev"
-        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
```

### Comparing `cmomy-0.8.0/requirements/dev-complete.txt` & `cmomy-0.9.0/requirements/dev-complete.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 # Instead edit the corresponding pyproject.toml file.
 #
 docstring-inheritance
 ipykernel
 ipython
 lazy_loader
 module-utilities>=0.6
-mypy>=1.5.1
-nbqa
+nbclient>=0.10.0
 nbval
-nox
+nox>=2024.3.2
 numba>=0.50
 numpy>=1.21
+packaging
 pandas-stubs
+pipx
 pre-commit
-pyright
 pytest
 pytest-accept
 pytest-cov
 pytest-sugar
 pytest-xdist
-pytype;python_version<"3.11"
 scriv
 typing-extensions;python_version<"3.11"
 xarray>=0.16
```

### Comparing `cmomy-0.8.0/requirements/py311-dev-complete.yaml` & `cmomy-0.9.0/requirements/py311-dev-complete.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 dependencies:
   - python=3.11
   - docstring-inheritance
   - ipykernel
   - ipython
   - lazy_loader
   - module-utilities>=0.6
-  - mypy>=1.5.1
-  - nbqa
+  - nbclient>=0.10.0
   - nbval
-  - nox
+  - nox>=2024.3.2
   - numba>=0.50
   - numpy>=1.21
+  - packaging
   - pandas-stubs
+  - pipx
   - pre-commit
-  - pyright
   - pytest
   - pytest-cov
   - pytest-sugar
   - pytest-xdist
   - xarray>=0.16
   - pip
   - pip:
```

### Comparing `cmomy-0.8.0/requirements/py311-dev.yaml` & `cmomy-0.9.0/requirements/py311-dev.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 dependencies:
   - python=3.11
   - docstring-inheritance
   - ipykernel
   - ipython
   - lazy_loader
   - module-utilities>=0.6
-  - mypy>=1.5.1
+  - nbclient>=0.10.0
   - nbval
-  - nox
+  - nox>=2024.3.2
   - numba>=0.50
   - numpy>=1.21
+  - packaging
   - pandas-stubs
   - pytest
   - pytest-cov
   - pytest-sugar
   - pytest-xdist
   - xarray>=0.16
   - pip
```

### Comparing `cmomy-0.8.0/requirements/lock/py311-dev-base.txt` & `cmomy-0.9.0/requirements/lock/py311-dev-base.txt`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/requirements/lock/py311-dev.txt` & `cmomy-0.9.0/requirements/lock/py311-dev-complete.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,196 +1,89 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --allow-unsafe --output-file=requirements/lock/py311-dev.txt --strip-extras requirements/dev.txt
-#
-appnope==0.1.4
-    # via ipykernel
-argcomplete==3.2.2
-    # via nox
-asttokens==2.4.1
-    # via stack-data
-attrs==23.2.0
-    # via
-    #   jsonschema
-    #   referencing
-colorlog==6.8.2
-    # via nox
-comm==0.2.1
-    # via ipykernel
-coverage==7.4.2
-    # via
-    #   nbval
-    #   pytest-cov
-debugpy==1.8.1
-    # via ipykernel
-decorator==5.1.1
-    # via ipython
-distlib==0.3.8
-    # via virtualenv
-docstring-inheritance==2.1.2
-    # via -r requirements/dev.txt
-execnet==2.0.2
-    # via pytest-xdist
-executing==2.0.1
-    # via stack-data
-fastjsonschema==2.19.1
-    # via nbformat
-filelock==3.13.1
-    # via virtualenv
-iniconfig==2.0.0
-    # via pytest
-ipykernel==6.29.2
-    # via
-    #   -r requirements/dev.txt
-    #   nbval
-ipython==8.21.0
-    # via
-    #   -r requirements/dev.txt
-    #   ipykernel
-jedi==0.19.1
-    # via ipython
-jsonschema==4.21.1
-    # via nbformat
-jsonschema-specifications==2023.12.1
-    # via jsonschema
-jupyter-client==8.6.0
-    # via
-    #   ipykernel
-    #   nbval
-jupyter-core==5.7.1
-    # via
-    #   ipykernel
-    #   jupyter-client
-    #   nbformat
-lazy-loader==0.3
-    # via -r requirements/dev.txt
-llvmlite==0.42.0
-    # via numba
-matplotlib-inline==0.1.6
-    # via
-    #   ipykernel
-    #   ipython
+# This file was autogenerated by uv via the following command:
+#    uv pip compile --python-version=3.11 --annotation-style=line -o requirements/lock/py311-dev-complete.txt requirements/dev-complete.txt
+appnope==0.1.4            # via ipykernel
+argcomplete==3.2.3        # via nox, pipx
+asttokens==2.4.1          # via stack-data
+attrs==23.2.0             # via jsonschema, referencing, scriv
+certifi==2024.2.2         # via requests
+cfgv==3.4.0               # via pre-commit
+charset-normalizer==3.3.2  # via requests
+click==8.1.7              # via click-log, scriv, userpath
+click-log==0.4.0          # via scriv
+colorlog==6.8.2           # via nox
+comm==0.2.2               # via ipykernel
+coverage==7.4.4           # via nbval, pytest-cov
+debugpy==1.8.1            # via ipykernel
+decorator==5.1.1          # via ipython
+distlib==0.3.8            # via virtualenv
+docstring-inheritance==2.2.0
+execnet==2.1.1            # via pytest-xdist
+executing==2.0.1          # via stack-data
+fastjsonschema==2.19.1    # via nbformat
+filelock==3.13.4          # via virtualenv
+identify==2.5.35          # via pre-commit
+idna==3.6                 # via requests
+iniconfig==2.0.0          # via pytest
+ipykernel==6.29.4         # via nbval
+ipython==8.23.0           # via ipykernel
+jedi==0.19.1              # via ipython
+jinja2==3.1.3             # via scriv
+jsonschema==4.21.1        # via nbformat
+jsonschema-specifications==2023.12.1  # via jsonschema
+jupyter-client==8.6.1     # via ipykernel, nbclient, nbval
+jupyter-core==5.7.2       # via ipykernel, jupyter-client, nbclient, nbformat
+lazy-loader==0.4
+llvmlite==0.42.0          # via numba
+markdown-it-py==3.0.0     # via scriv
+markupsafe==2.1.5         # via jinja2
+matplotlib-inline==0.1.6  # via ipykernel, ipython
+mdurl==0.1.2              # via markdown-it-py
 module-utilities==0.9.0
-    # via -r requirements/dev.txt
-mypy==1.8.0
-    # via -r requirements/dev.txt
-mypy-extensions==1.0.0
-    # via mypy
-nbformat==5.9.2
-    # via nbval
-nbval==0.10.0
-    # via -r requirements/dev.txt
-nest-asyncio==1.6.0
-    # via ipykernel
-nox==2023.4.22
-    # via -r requirements/dev.txt
-numba==0.59.0
-    # via -r requirements/dev.txt
-numpy==1.26.4
-    # via
-    #   -r requirements/dev.txt
-    #   numba
-    #   pandas
-    #   pandas-stubs
-    #   xarray
-packaging==23.2
-    # via
-    #   ipykernel
-    #   nox
-    #   pytest
-    #   pytest-sugar
-    #   xarray
-pandas==2.2.0
-    # via xarray
-pandas-stubs==2.2.0.240218
-    # via -r requirements/dev.txt
-parso==0.8.3
-    # via jedi
-pexpect==4.9.0
-    # via ipython
-platformdirs==4.2.0
-    # via
-    #   jupyter-core
-    #   virtualenv
-pluggy==1.4.0
-    # via pytest
-prompt-toolkit==3.0.43
-    # via ipython
-psutil==5.9.8
-    # via ipykernel
-ptyprocess==0.7.0
-    # via pexpect
-pure-eval==0.2.2
-    # via stack-data
-pygments==2.17.2
-    # via ipython
-pytest==8.0.1
-    # via
-    #   -r requirements/dev.txt
-    #   nbval
-    #   pytest-accept
-    #   pytest-cov
-    #   pytest-sugar
-    #   pytest-xdist
+nbclient==0.10.0
+nbformat==5.10.4          # via nbclient, nbval
+nbval==0.11.0
+nest-asyncio==1.6.0       # via ipykernel
+nodeenv==1.8.0            # via pre-commit
+nox==2024.3.2
+numba==0.59.1
+numpy==1.26.4             # via numba, pandas, pandas-stubs, xarray
+packaging==24.0           # via ipykernel, lazy-loader, nox, pipx, pytest, pytest-sugar, xarray
+pandas==2.2.1             # via xarray
+pandas-stubs==2.2.1.240316
+parso==0.8.4              # via jedi
+pexpect==4.9.0            # via ipython
+pipx==1.5.0
+platformdirs==4.2.0       # via jupyter-core, pipx, virtualenv
+pluggy==1.4.0             # via pytest
+pre-commit==3.7.0
+prompt-toolkit==3.0.43    # via ipython
+psutil==5.9.8             # via ipykernel
+ptyprocess==0.7.0         # via pexpect
+pure-eval==0.2.2          # via stack-data
+pygments==2.17.2          # via ipython
+pytest==8.1.1             # via nbval, pytest-accept, pytest-cov, pytest-sugar, pytest-xdist
 pytest-accept==0.1.10
-    # via -r requirements/dev.txt
-pytest-cov==4.1.0
-    # via -r requirements/dev.txt
+pytest-cov==5.0.0
 pytest-sugar==1.0.0
-    # via -r requirements/dev.txt
 pytest-xdist==3.5.0
-    # via -r requirements/dev.txt
-python-dateutil==2.8.2
-    # via
-    #   jupyter-client
-    #   pandas
-pytz==2024.1
-    # via pandas
-pyzmq==25.1.2
-    # via
-    #   ipykernel
-    #   jupyter-client
-referencing==0.33.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-rpds-py==0.18.0
-    # via
-    #   jsonschema
-    #   referencing
-six==1.16.0
-    # via
-    #   asttokens
-    #   python-dateutil
-stack-data==0.6.3
-    # via ipython
-termcolor==2.4.0
-    # via pytest-sugar
-tornado==6.4
-    # via
-    #   ipykernel
-    #   jupyter-client
-traitlets==5.14.1
-    # via
-    #   comm
-    #   ipykernel
-    #   ipython
-    #   jupyter-client
-    #   jupyter-core
-    #   matplotlib-inline
-    #   nbformat
-types-pytz==2024.1.0.20240203
-    # via pandas-stubs
-typing-extensions==4.9.0
-    # via
-    #   module-utilities
-    #   mypy
-tzdata==2024.1
-    # via pandas
-virtualenv==20.25.0
-    # via nox
-wcwidth==0.2.13
-    # via prompt-toolkit
-xarray==2024.2.0
-    # via -r requirements/dev.txt
+python-dateutil==2.9.0.post0  # via jupyter-client, pandas
+pytz==2024.1              # via pandas
+pyyaml==6.0.1             # via pre-commit
+pyzmq==25.1.2             # via ipykernel, jupyter-client
+referencing==0.34.0       # via jsonschema, jsonschema-specifications
+requests==2.31.0          # via scriv
+rpds-py==0.18.0           # via jsonschema, referencing
+scriv==1.5.1
+setuptools==69.2.0        # via nodeenv
+six==1.16.0               # via asttokens, python-dateutil
+stack-data==0.6.3         # via ipython
+termcolor==2.4.0          # via pytest-sugar
+tornado==6.4              # via ipykernel, jupyter-client
+traitlets==5.14.2         # via comm, ipykernel, ipython, jupyter-client, jupyter-core, matplotlib-inline, nbclient, nbformat
+types-pytz==2024.1.0.20240203  # via pandas-stubs
+typing-extensions==4.11.0  # via ipython, module-utilities
+tzdata==2024.1            # via pandas
+urllib3==2.2.1            # via requests
+userpath==1.9.2           # via pipx
+virtualenv==20.25.1       # via nox, pre-commit
+wcwidth==0.2.13           # via prompt-toolkit
+xarray==2024.3.0
```

### Comparing `cmomy-0.8.0/src/cmomy/__init__.py` & `cmomy-0.9.0/src/cmomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/src/cmomy/_compat.py` & `cmomy-0.9.0/src/cmomy/_compat.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/src/cmomy/_formatting.py` & `cmomy-0.9.0/src/cmomy/_formatting.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/src/cmomy/abstract_central.py` & `cmomy-0.9.0/src/cmomy/abstract_central.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Base class for central moments calculations."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from math import prod
 from typing import TYPE_CHECKING, Generic, cast, overload
 
 import numpy as np
 from module_utilities import cached
 
 from . import convert
 from .docstrings import docfiller
-from .typing import MyNDArray, T_Array
+from .typing import NDArrayAny, T_Array
 from .utils import normalize_axis_index
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Hashable, Literal, Mapping
 
     from numpy.typing import DTypeLike
 
@@ -55,15 +56,15 @@
         "_data_flat",
         "_mom_ndim",
     )
 
     def __init__(
         self, data: T_Array, mom_ndim: Mom_NDim = 1
     ) -> None:  # pragma: no cover
-        self._data = cast("MyNDArray", data)  # type: ignore[redundant-cast]
+        self._data = cast("NDArrayAny", data)  # type: ignore[redundant-cast]
         self._data_flat = self._data
 
         if mom_ndim not in {1, 2}:
             msg = f"{mom_ndim=} must be 1 or 2."
             raise ValueError(msg)
 
         self._mom_ndim = mom_ndim
@@ -74,15 +75,15 @@
     def _validate_data(self) -> None:  # pragma: no cover
         if np.shares_memory(self._data_flat, self._data):
             return
 
         raise ValueError
 
     @property
-    def data(self) -> MyNDArray:
+    def data(self) -> NDArrayAny:
         """
         Accessor to numpy array underlying data.
 
         By convention data has the following meaning for the moments indexes
 
         * `data[...,i=0,j=0]`, weights
         * `data[...,i=1,j=0]]`, if only one moment index is one and all others zero,
@@ -97,15 +98,15 @@
         """Access underlying central moments array."""
 
     @property
     def values(self) -> T_Array:
         """Access underlying central moments array."""
         return self.to_values()
 
-    def to_numpy(self) -> MyNDArray:
+    def to_numpy(self) -> NDArrayAny:
         """Access to numpy array underlying class."""
         return self._data
 
     @property
     def shape(self) -> tuple[int, ...]:
         """self.data.shape."""
         return self.data.shape
@@ -197,26 +198,26 @@
         return s + repr(self.to_values())
 
     def _repr_html_(self) -> str:  # noqa: PLW3201
         from ._formatting import repr_html  # pyright: ignore[reportUnknownVariableType]
 
         return repr_html(self)  # type: ignore[no-any-return,no-untyped-call]
 
-    def __array__(self, dtype: DTypeLike | None = None) -> MyNDArray:  # noqa: PLW3201
+    def __array__(self, dtype: DTypeLike | None = None) -> NDArrayAny:  # noqa: PLW3201
         """Used by np.array(self)."""  # D401
         return np.asarray(self.data, dtype=dtype)
 
     ###########################################################################
     # ** top level creation/copy/new
     ###########################################################################
     @abstractmethod
     @docfiller.decorate
     def new_like(
         self,
-        data: MyNDArray | T_Array | None = None,
+        data: NDArrayAny | T_Array | None = None,
         *,
         copy: bool = False,
         copy_kws: Mapping[str, Any] | None = None,
         verify: bool = False,
         strict: bool = False,
         **kwargs: Any,
     ) -> Self:
@@ -295,15 +296,15 @@
     # ** Access to underlying statistics
     ###########################################################################
 
     @cached.prop
     def _weight_index(self) -> tuple[int | ellipsis, ...]:  # noqa: F821
         index: tuple[int, ...] = (0,) * len(self.mom)
         if self.val_ndim > 0:
-            return (..., *index)
+            return (..., *index)  # pyright: ignore[reportUnknownVariableType]
         return index
 
     @cached.meth
     def _single_index(self, val: int) -> tuple[ellipsis | int | list[int], ...]:  # noqa: F821
         # index with things like data[..., 1,0] data[..., 0,1]
         # index = (...,[1,0],[0,1])
         dims = len(self.mom)
@@ -315,15 +316,15 @@
         else:
             # this is a bit more complicated
             index = [[0] * dims for _ in range(dims)]
             for i in range(dims):
                 index[i][i] = val
 
         if self.val_ndim > 0:
-            return (..., *index)
+            return (..., *index)  # pyright: ignore[reportUnknownVariableType]
         return tuple(index)
 
     def weight(self) -> float | T_Array:
         """Weight data."""
         return cast(
             "float | T_Array",
             self.to_values()[self._weight_index],  # pyright: ignore[reportGeneralTypeIssues, reportIndexIssue]
@@ -343,15 +344,15 @@
             self.to_values()[self._single_index(2)],  # pyright: ignore[reportGeneralTypeIssues, reportIndexIssue]
         )
 
     def std(self) -> float | T_Array:
         """Standard deviation."""  # D401
         return cast("float | T_Array", np.sqrt(self.var()))
 
-    def _wrap_like(self, x: MyNDArray) -> T_Array:  # noqa: PLR6301
+    def _wrap_like(self, x: NDArrayAny) -> T_Array:  # noqa: PLR6301
         return x  # type: ignore[return-value]
 
     def cmom(self) -> T_Array:
         r"""
         Central moments.
 
         Strict central moments of the form
@@ -368,15 +369,15 @@
         out = self.data.copy()
         # zeroth central moment
         out[self._weight_index] = 1
         # first central moment
         out[self._single_index(1)] = 0
         return self._wrap_like(out)
 
-    def to_raw(self, *, weights: float | MyNDArray | None = None) -> T_Array:
+    def to_raw(self, *, weights: float | NDArrayAny | None = None) -> T_Array:
         r"""
         Raw moments accumulation array.
 
         .. math::
 
             \text{raw[..., n, m]} = \begin{cases}
             \text{weight} & n = m = 0 \\
@@ -460,48 +461,48 @@
         return self.fill(value=0.0)
 
     @abstractmethod
     def _verify_value(  # pragma: no cover
         self,
         *,
         x: MultiArray[T_Array],
-        target: str | MyNDArray | T_Array,
+        target: str | NDArrayAny | T_Array,
         shape_flat: tuple[int, ...],
         axis: int | None = None,
         dim: Hashable | None = None,  # included here for consistency
         broadcast: bool = False,
         expand: bool = False,
-        other: MyNDArray | None = None,
-    ) -> tuple[MyNDArray, MyNDArray | T_Array]:
+        other: NDArrayAny | None = None,
+    ) -> tuple[NDArrayAny, NDArrayAny | T_Array]:
         pass
 
     def _check_weight(
         self,
         *,
         w: MultiArray[T_Array] | None,
-        target: MyNDArray | T_Array,
-    ) -> MyNDArray:
+        target: NDArrayAny | T_Array,
+    ) -> NDArrayAny:
         if w is None:
             w = 1.0
         return self._verify_value(
             x=w,
             target=target,
             shape_flat=self.val_shape_flat,
             broadcast=True,
             expand=True,
         )[0]
 
     def _check_weights(
         self,
         *,
         w: MultiArray[T_Array] | None,
-        target: MyNDArray | T_Array,
+        target: NDArrayAny | T_Array,
         axis: int | None = None,
         dim: Hashable | None = None,
-    ) -> MyNDArray:
+    ) -> NDArrayAny:
         if w is None:
             w = 1.0
         return self._verify_value(
             x=w,
             target=target,
             shape_flat=self.val_shape_flat,
             axis=axis,
@@ -510,64 +511,64 @@
             expand=True,
         )[0]
 
     def _check_val(
         self,
         *,
         x: MultiArray[T_Array],
-        target: str | MyNDArray | T_Array,
+        target: str | NDArrayAny | T_Array,
         broadcast: bool = False,
-    ) -> tuple[MyNDArray, MyNDArray | T_Array]:
+    ) -> tuple[NDArrayAny, NDArrayAny | T_Array]:
         return self._verify_value(
             x=x,
             target=target,
             shape_flat=self.val_shape_flat,
             broadcast=broadcast,
             expand=False,
         )
 
     def _check_vals(
         self,
         *,
         x: MultiArrayVals[T_Array],
-        target: str | MyNDArray | T_Array,
+        target: str | NDArrayAny | T_Array,
         axis: int | None,
         broadcast: bool = False,
         dim: Hashable | None = None,
-    ) -> tuple[MyNDArray, MyNDArray | T_Array]:
+    ) -> tuple[NDArrayAny, NDArrayAny | T_Array]:
         return self._verify_value(
             x=x,
             target=target,
             shape_flat=self.val_shape_flat,
             axis=axis,
             dim=dim,
             broadcast=broadcast,
             expand=broadcast,
         )
 
     def _check_var(
         self, *, v: MultiArray[T_Array], broadcast: bool = False
-    ) -> MyNDArray:
+    ) -> NDArrayAny:
         return self._verify_value(
             x=v,
             target="var",
             shape_flat=self.shape_flat_var,
             broadcast=broadcast,
             expand=False,
         )[0]
 
     def _check_vars(
         self,
         *,
         v: MultiArrayVals[T_Array],
-        target: MyNDArray | T_Array,
+        target: NDArrayAny | T_Array,
         axis: int | None,
         broadcast: bool = False,
         dim: Hashable | None = None,
-    ) -> MyNDArray:
+    ) -> NDArrayAny:
         # assert isinstance(target, np.ndarray)
         if not isinstance(target, np.ndarray):  # pragma: no cover
             msg = f"{type(target)=} must be numpy.ndarray."
             raise TypeError(msg)
         return self._verify_value(
             x=v,
             target="vars",
@@ -575,28 +576,28 @@
             axis=axis,
             dim=dim,
             broadcast=broadcast,
             expand=broadcast,
             other=target,
         )[0]
 
-    def _check_data(self, *, data: MultiArrayVals[T_Array]) -> MyNDArray:
+    def _check_data(self, *, data: MultiArrayVals[T_Array]) -> NDArrayAny:
         return self._verify_value(
             x=data,
             target="data",
             shape_flat=self.shape_flat,
         )[0]
 
     def _check_datas(
         self,
         *,
         datas: MultiArrayVals[T_Array],
         axis: int | None = None,
         dim: Hashable | None = None,
-    ) -> MyNDArray:
+    ) -> NDArrayAny:
         if axis is not None:
             axis = normalize_axis_index(axis, self.val_ndim + 1)
 
         return self._verify_value(
             x=datas,
             target="datas",
             shape_flat=self.shape_flat,
@@ -848,15 +849,15 @@
             raise ValueError(message)
 
     # * Universal reducers
 
     @docfiller.decorate
     def resample(
         self,
-        indices: MyNDArray,
+        indices: NDArrayAny,
         axis: int | None = 0,
         *,
         first: bool = True,
         verify: bool = False,
         **kwargs: Any,
     ) -> Self:
         """
@@ -963,18 +964,18 @@
 
     ###########################################################################
     # ** Constructors
     ###########################################################################
     # *** Utils
     @staticmethod
     def _datas_axis_to_first(
-        datas: MyNDArray,
+        datas: NDArrayAny,
         axis: int,
         mom_ndim: Mom_NDim,
-    ) -> tuple[MyNDArray, int]:
+    ) -> tuple[NDArrayAny, int]:
         """Move axis to first first position."""
         axis = normalize_axis_index(axis, datas.ndim - mom_ndim)
         if axis != 0:
             datas = np.moveaxis(datas, axis, 0)
         return datas, axis
 
     def _wrap_axis(
@@ -1153,72 +1154,82 @@
         """
 
     @overload
     @classmethod
     @abstractmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray] | T_Array | tuple[T_Array, T_Array],
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
+        | T_Array
+        | tuple[T_Array, T_Array],
         mom: Moments,
         *,
         full_output: Literal[False] = ...,
         **kwargs: Any,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     @overload
     @classmethod
     @abstractmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray] | T_Array | tuple[T_Array, T_Array],
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
+        | T_Array
+        | tuple[T_Array, T_Array],
         mom: Moments,
         *,
         full_output: Literal[True],
         **kwargs: Any,
-    ) -> tuple[Self, MyNDArray]:
-        ...
+    ) -> tuple[Self, NDArrayAny]: ...
 
     @overload
     @classmethod
     @abstractmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray] | T_Array | tuple[T_Array, T_Array],
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
+        | T_Array
+        | tuple[T_Array, T_Array],
         mom: Moments,
         *,
         full_output: bool,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
-        ...
+    ) -> Self | tuple[Self, NDArrayAny]: ...
 
     @classmethod
     @abstractmethod
     @docfiller.decorate
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray] | T_Array | tuple[T_Array, T_Array],
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
+        | T_Array
+        | tuple[T_Array, T_Array],
         mom: Moments,
         *,
         full_output: bool = False,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
+    ) -> Self | tuple[Self, NDArrayAny]:
         """
         Create from resample observations/values.
 
         This effectively resamples `x`.
 
         Parameters
         ----------
         x : array-like or tuple of array-like
             For moments, pass single array-like objects `x=x0`.
             For comoments, pass tuple of array-like objects `x=(x0, x1)`.
         {mom}
         {full_output}
         {nrep}
+        {nsamp}
         {freq}
         {indices}
         w : scalar or array-like, optional
             Optional weights.  If scalar or array, attempt to
             broadcast to `x0.shape`
         {axis_and_dim}
         {dtype}
```

### Comparing `cmomy-0.8.0/src/cmomy/central.py` & `cmomy-0.9.0/src/cmomy/central.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Central moments/comoments routines from :class:`np.ndarray` objects
 -------------------------------------------------------------------.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast, overload
 
 import numpy as np
+
+# pandas needed for autdoc typehints
+import pandas as pd  # noqa: F401  # pyright: ignore[reportUnusedImport]
 import xarray as xr
 
 from . import convert
 from .abstract_central import CentralMomentsABC
 from .docstrings import docfiller_central as docfiller
 from .utils import (
     axis_expand_broadcast,
@@ -39,30 +43,30 @@
         XArrayDimsType,
         XArrayIndexesType,
         XArrayNameType,
     )
     from .xcentral import xCentralMoments
 
 
-from .typing import MyNDArray
+from .typing import NDArrayAny
 
 
 ###############################################################################
 # central mom/comoments routines
 ###############################################################################
 def _central_moments(
     vals: ArrayLike,
     mom: Moments,
-    w: MyNDArray | None = None,
+    w: NDArrayAny | None = None,
     axis: int = 0,
     last: bool = True,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     """Calculate central mom along axis."""
     if isinstance(mom, tuple):  # pragma: no cover
         mom = mom[0]
 
     x = np.asarray(vals, dtype=dtype, order=order)
     if dtype is None:
         dtype = x.dtype
@@ -104,24 +108,24 @@
 
     if last:
         out = np.moveaxis(out, 0, -1)
     return out
 
 
 def _central_comoments(  # noqa: C901, PLR0912
-    vals: tuple[MyNDArray, MyNDArray],
+    vals: tuple[NDArrayAny, NDArrayAny],
     mom: tuple[int, int],
-    w: MyNDArray | None = None,
+    w: NDArrayAny | None = None,
     axis: int = 0,
     last: bool = True,
     broadcast: bool = False,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     """Calculate central co-mom (covariance, etc) along axis."""
     if not isinstance(
         mom, tuple
     ):  # pragma: no cover  # pyright: ignore[reportUnnecessaryIsInstance]
         raise TypeError
 
     if len(mom) != 2:
@@ -197,25 +201,25 @@
     if last:
         out = np.moveaxis(out, [0, 1], [-2, -1])
     return out
 
 
 @docfiller.decorate
 def central_moments(
-    x: MyNDArray | tuple[MyNDArray, MyNDArray],
+    x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
     mom: Moments,
     *,
-    w: MyNDArray | None = None,
+    w: NDArrayAny | None = None,
     axis: int = 0,
     last: bool = True,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
+    out: NDArrayAny | None = None,
     broadcast: bool = False,
-) -> MyNDArray:
+) -> NDArrayAny:
     """
     Calculate central moments or comoments along axis.
 
     Parameters
     ----------
     x : array-like or tuple of array-like
         if calculating moments, then this is the input array.
@@ -313,19 +317,19 @@
 ###############################################################################
 
 docfiller_abc = docfiller.factory_from_parent(CentralMomentsABC)
 docfiller_inherit_abc = docfiller.factory_inherit_from_parent(CentralMomentsABC)
 
 
 @docfiller(CentralMomentsABC)  # noqa: PLR0904
-class CentralMoments(CentralMomentsABC[MyNDArray]):  # noqa: D101
-    # def __new__(cls, data: MyNDArray, mom_ndim: Literal[1, 2] = 1):
+class CentralMoments(CentralMomentsABC[NDArrayAny]):  # noqa: D101
+    # def __new__(cls, data: NDArrayAny, mom_ndim: Literal[1, 2] = 1):
     #     return super().__new__(cls, data=data, mom_ndim=mom_ndim)
 
-    def __init__(self, data: MyNDArray, mom_ndim: Mom_NDim = 1) -> None:
+    def __init__(self, data: NDArrayAny, mom_ndim: Mom_NDim = 1) -> None:
         if mom_ndim not in {1, 2}:
             msg = (
                 "mom_ndim must be either 1 (for central moments)"
                 "or 2 (for central comoments)"
             )
             raise ValueError(msg)
 
@@ -346,26 +350,26 @@
             msg = "moments must be positive"
             raise ValueError(msg)
 
         self._validate_data()  # pragma: no cover
 
         self._cache: dict[str, Any] = {}
 
-    def to_values(self) -> MyNDArray:
+    def to_values(self) -> NDArrayAny:
         """Accesses for self.data."""
         return self._data
 
     ###########################################################################
     # SECTION: top level creation/copy/new
     ###########################################################################
     # @docfiller(CentralMomentsABC.new_like)
     @docfiller_abc()
     def new_like(
         self,
-        data: MyNDArray | None = None,
+        data: NDArrayAny | None = None,
         *,
         copy: bool = False,
         copy_kws: Mapping[str, Any] | None = None,
         verify: bool = False,
         strict: bool = False,
         **kwargs: Any,
     ) -> Self:
@@ -605,18 +609,18 @@
     ###########################################################################
     # SECTION: pushing routines
     ###########################################################################
     #  -> np.ndarray | float | Tuple[float|np.ndarray, None|float|np.ndarray] :
 
     def _get_target_shape(
         self,
-        x: MyNDArray,
+        x: NDArrayAny,
         style: VerifyValuesStyles,
         axis: int | None = None,
-        other: MyNDArray | None = None,
+        other: NDArrayAny | None = None,
     ) -> tuple[int, ...]:
         from .utils import shape_insert_axis
 
         if style == "val":
             target_shape = self.val_shape
         elif style == "vals":
             if axis is None:
@@ -646,23 +650,23 @@
             raise ValueError(msg)
 
         return target_shape
 
     def _verify_value(
         self,
         *,
-        x: MultiArray[MyNDArray],
-        target: str | MyNDArray,
+        x: MultiArray[NDArrayAny],
+        target: str | NDArrayAny,
         shape_flat: tuple[int, ...],
         axis: int | None = None,
         dim: Hashable | None = None,  # included here for consistency  # noqa: ARG002
         broadcast: bool = False,
         expand: bool = False,
-        other: MyNDArray | None = None,
-    ) -> tuple[MyNDArray, MyNDArray]:
+        other: NDArrayAny | None = None,
+    ) -> tuple[NDArrayAny, NDArrayAny]:
         """
         Verify input values.
 
         Parameters
         ----------
         x : array
         target : tuple or array
@@ -719,15 +723,15 @@
 
         if x.ndim == 0:
             x = x[()]
 
         return x, target_output
 
     @docfiller_inherit_abc()
-    def push_data(self, data: MultiArrayVals[MyNDArray]) -> Self:
+    def push_data(self, data: MultiArrayVals[NDArrayAny]) -> Self:
         """
         Examples
         --------
         >>> from cmomy.random import default_rng
         >>> rng = default_rng(0)
         >>> xs = rng.random((2, 10))
         >>> datas = [central_moments(x=x, mom=2) for x in xs]
@@ -750,15 +754,15 @@
 
         """
         return super().push_data(data=data)
 
     @docfiller_inherit_abc()
     def push_datas(
         self,
-        datas: MultiArray[MyNDArray],
+        datas: MultiArray[NDArrayAny],
         axis: int | None = 0,
         **kwargs: Any,  # noqa: ARG002
     ) -> Self:
         """
         Examples
         --------
         >>> from cmomy.random import default_rng
@@ -778,16 +782,17 @@
         array([20.    ,  0.5124,  0.1033])
         """
         return super().push_datas(datas=datas, axis=axis or 0)
 
     @docfiller_inherit_abc()
     def push_val(
         self,
-        x: MultiArray[MyNDArray] | tuple[MultiArray[MyNDArray], MultiArray[MyNDArray]],
-        w: MultiArray[MyNDArray] | None = None,
+        x: MultiArray[NDArrayAny]
+        | tuple[MultiArray[NDArrayAny], MultiArray[NDArrayAny]],
+        w: MultiArray[NDArrayAny] | None = None,
         broadcast: bool = False,
     ) -> Self:
         """
         Examples
         --------
         >>> from cmomy.random import default_rng
         >>> rng = default_rng(0)
@@ -824,17 +829,17 @@
 
         """
         return super().push_val(x=x, w=w, broadcast=broadcast)
 
     @docfiller_inherit_abc()
     def push_vals(
         self,
-        x: MultiArrayVals[MyNDArray]
-        | tuple[MultiArrayVals[MyNDArray], MultiArrayVals[MyNDArray]],
-        w: MultiArray[MyNDArray] | None = None,
+        x: MultiArrayVals[NDArrayAny]
+        | tuple[MultiArrayVals[NDArrayAny], MultiArrayVals[NDArrayAny]],
+        w: MultiArray[NDArrayAny] | None = None,
         axis: int | None = 0,
         broadcast: bool = False,
         **kwargs: Any,  # noqa: ARG002
     ) -> Self:
         """
         Examples
         --------
@@ -881,77 +886,79 @@
     ###########################################################################
     @overload
     def resample_and_reduce(
         self,
         nrep: int | None = ...,
         *,
         full_output: Literal[False] = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
         axis: int | None = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
         **kwargs: Any,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     @overload
     def resample_and_reduce(
         self,
         nrep: int | None = ...,
         *,
         full_output: Literal[True],
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
         axis: int | None = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
         **kwargs: Any,
-    ) -> tuple[Self, MyNDArray]:
-        ...
+    ) -> tuple[Self, NDArrayAny]: ...
 
     @overload
     def resample_and_reduce(
         self,
         nrep: int | None = ...,
         *,
         full_output: bool,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
         axis: int | None = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
-        ...
+    ) -> Self | tuple[Self, NDArrayAny]: ...
 
     @docfiller.decorate
     def resample_and_reduce(
         self,
         nrep: int | None = None,
         *,
         full_output: bool = False,
-        freq: MyNDArray | None = None,
-        indices: MyNDArray | None = None,
+        nsamp: int | None = None,
+        freq: NDArrayAny | None = None,
+        indices: NDArrayAny | None = None,
         axis: int | None = None,
         parallel: bool = True,
         resample_kws: Mapping[str, Any] | None = None,
         rng: np.random.Generator | None = None,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
+    ) -> Self | tuple[Self, NDArrayAny]:
         """
         Bootstrap resample and reduce.
 
         Parameters
         ----------
         {nrep}
         {full_output}
+        {nsamp}
         {freq}
         {indices}
         {axis}
         {parallel}
         {resample_kws}
         {rng}
         **kwargs
@@ -979,14 +986,15 @@
         axis = self._wrap_axis(axis)
         if resample_kws is None:
             resample_kws = {}
 
         freq = randsamp_freq(
             nrep=nrep,
             ndat=self.val_shape[axis],
+            nsamp=nsamp,
             indices=indices,
             freq=freq,
             check=True,
             rng=rng,
         )
         data = resample_data(
             self.data, freq, mom=self.mom, axis=axis, parallel=parallel, **resample_kws
@@ -1264,15 +1272,15 @@
         kwargs = dict(kwargs, verify=False, copy=False)
         return cls.from_data(data=data, mom_ndim=mom_ndim, **kwargs)
 
     @classmethod
     @docfiller_abc()
     def from_data(
         cls,
-        data: MyNDArray,
+        data: NDArrayAny,
         *,
         mom: Moments | None = None,
         mom_ndim: Mom_NDim | None = None,
         val_shape: tuple[int, ...] | None = None,
         copy: bool = True,
         copy_kws: Mapping[str, Any] | None = None,
         verify: bool = False,
@@ -1310,15 +1318,15 @@
 
         return cls(data=data_verified, mom_ndim=mom_ndim)
 
     @classmethod
     @docfiller_inherit_abc()
     def from_datas(
         cls,
-        datas: MyNDArray,
+        datas: NDArrayAny,
         *,
         mom: Moments | None = None,
         mom_ndim: Mom_NDim | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         verify: bool = False,
         axis: int | None = 0,
@@ -1363,18 +1371,18 @@
             **kwargs,
         ).push_datas(datas=datas, axis=0)
 
     @classmethod
     @docfiller_inherit_abc()
     def from_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray],
+        x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
         mom: Moments,
         *,
-        w: float | MyNDArray | None = None,
+        w: float | NDArrayAny | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         broadcast: bool = False,
         axis: int | None = 0,
         **kwargs: Any,
     ) -> Self:
         """
@@ -1390,108 +1398,109 @@
                [1.0000e+02, 5.5355e-01, 7.1942e-02],
                [1.0000e+02, 5.1413e-01, 1.0407e-01]])
         """
         axis = axis or 0
         mom_ndim = mom_to_mom_ndim(mom)
 
         x0 = x if mom_ndim == 1 else x[0]
-        x0 = cast("MyNDArray", x0)
+        x0 = cast("NDArrayAny", x0)
 
         if val_shape is None:
             val_shape = shape_reduce(shape=x0.shape, axis=axis)
         if dtype is None:
             dtype = x0.dtype
 
         return cls.zeros(val_shape=val_shape, mom=mom, dtype=dtype, **kwargs).push_vals(
             x=x, axis=axis, w=w, broadcast=broadcast
         )
 
     @overload
     @classmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray],
+        x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
         mom: Moments,
         *,
         full_output: Literal[False] = ...,
         nrep: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
-        w: MyNDArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
+        w: NDArrayAny | None = ...,
         axis: int | None = ...,
         dtype: DTypeLike | None = ...,
         broadcast: bool = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         **kwargs: Any,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     @overload
     @classmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray],
+        x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
         mom: Moments,
         *,
         full_output: Literal[True],
         nrep: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
-        w: MyNDArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
+        w: NDArrayAny | None = ...,
         axis: int | None = ...,
         dtype: DTypeLike | None = ...,
         broadcast: bool = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         **kwargs: Any,
-    ) -> tuple[Self, MyNDArray]:
-        ...
+    ) -> tuple[Self, NDArrayAny]: ...
 
     @overload
     @classmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray],
+        x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
         mom: Moments,
         *,
         full_output: bool,
         nrep: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
-        w: MyNDArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
+        w: NDArrayAny | None = ...,
         axis: int | None = ...,
         dtype: DTypeLike | None = ...,
         broadcast: bool = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
-        ...
+    ) -> Self | tuple[Self, NDArrayAny]: ...
 
     @classmethod
     @docfiller_inherit_abc()
     def from_resample_vals(
         cls,
-        x: MyNDArray | tuple[MyNDArray, MyNDArray],
+        x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
         mom: Moments,
         *,
         full_output: bool = False,
         nrep: int | None = None,
-        freq: MyNDArray | None = None,
-        indices: MyNDArray | None = None,
-        w: MyNDArray | None = None,
+        nsamp: int | None = None,
+        freq: NDArrayAny | None = None,
+        indices: NDArrayAny | None = None,
+        w: NDArrayAny | None = None,
         axis: int | None = 0,
         dtype: DTypeLike | None = None,
         broadcast: bool = False,
         parallel: bool = True,
         resample_kws: Mapping[str, Any] | None = None,
         rng: np.random.Generator | None = None,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
+    ) -> Self | tuple[Self, NDArrayAny]:
         """
         Examples
         --------
         >>> from cmomy.random import default_rng
         >>> rng = default_rng(0)
         >>> ndat, nrep = 10, 3
         >>> x = rng.random(ndat)
@@ -1519,18 +1528,19 @@
         """
         from .resample import randsamp_freq, resample_vals
 
         axis = axis or 0
         mom_ndim = mom_to_mom_ndim(mom)
 
         x0 = x if mom_ndim == 1 else x[0]
-        x0 = cast("MyNDArray", x0)
+        x0 = cast("NDArrayAny", x0)
         freq = randsamp_freq(
             nrep=nrep,
             ndat=x0.shape[axis],
+            nsamp=nsamp,
             freq=freq,
             indices=indices,
             check=True,
             rng=rng,
         )
 
         if resample_kws is None:
@@ -1560,15 +1570,15 @@
             return out, freq
         return out
 
     @classmethod
     @docfiller_inherit_abc()
     def from_raw(
         cls,
-        raw: MyNDArray,
+        raw: NDArrayAny,
         *,
         mom_ndim: Mom_NDim | None = None,
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         convert_kws: Mapping[str, Any] | None = None,
         **kwargs: Any,
@@ -1638,15 +1648,15 @@
             **kwargs,
         )
 
     @classmethod
     @docfiller_inherit_abc()
     def from_raws(
         cls,
-        raws: MyNDArray,
+        raws: NDArrayAny,
         *,
         mom_ndim: Mom_NDim | None = None,
         mom: Moments | None = None,
         axis: int | None = 0,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         convert_kws: Mapping[str, Any] | None = None,
@@ -1708,33 +1718,33 @@
         if mom_ndim != 1:
             msg = "only available for mom_ndim == 1"
             raise NotImplementedError(msg)
 
     # special, 1d only methods
     def push_stat(
         self,
-        a: MultiArray[MyNDArray],
-        v: MultiArray[MyNDArray] = 0.0,
-        w: MultiArray[MyNDArray] | None = None,
+        a: MultiArray[NDArrayAny],
+        v: MultiArray[NDArrayAny] = 0.0,
+        w: MultiArray[NDArrayAny] | None = None,
         broadcast: bool = True,
     ) -> Self:
         """Push statistics onto self."""
         self._raise_if_not_1d(self.mom_ndim)
 
         ar, target = self._check_val(x=a, target="val")
         vr = self._check_var(v=v, broadcast=broadcast)
         wr = self._check_weight(w=w, target=target)
         self._push.stat(self._data_flat, wr, ar, vr)  # type: ignore[misc]
         return self
 
     def push_stats(
         self,
-        a: MultiArrayVals[MyNDArray],
-        v: MultiArray[MyNDArray] = 0.0,
-        w: MultiArray[MyNDArray] | None = None,
+        a: MultiArrayVals[NDArrayAny],
+        v: MultiArray[NDArrayAny] = 0.0,
+        w: MultiArray[NDArrayAny] | None = None,
         axis: int = 0,
         broadcast: bool = True,
     ) -> Self:
         """Push multiple statistics onto self."""
         self._raise_if_not_1d(self.mom_ndim)
 
         ar, target = self._check_vals(x=a, target="vals", axis=axis)
@@ -1743,16 +1753,16 @@
         self._push.stats(self._data_flat, wr, ar, vr)  # type: ignore[misc]
         return self
 
     @classmethod
     def from_stat(
         cls,
         a: ArrayLike | float,
-        v: MyNDArray | float = 0.0,
-        w: MyNDArray | float | None = None,
+        v: NDArrayAny | float = 0.0,
+        w: NDArrayAny | float | None = None,
         mom: Moments = 2,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         order: ArrayOrder | None = None,
         **kwargs: Any,
     ) -> Self:
         """Create object from single weight, average, variance/covariance."""
@@ -1769,17 +1779,17 @@
         return cls.zeros(val_shape=val_shape, mom=mom, dtype=dtype, **kwargs).push_stat(
             w=w, a=a, v=v
         )
 
     @classmethod
     def from_stats(
         cls,
-        a: MyNDArray,
-        v: MyNDArray,
-        w: MyNDArray | float | None = None,
+        a: NDArrayAny,
+        v: NDArrayAny,
+        w: NDArrayAny | float | None = None,
         axis: int = 0,
         mom: Moments = 2,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         order: ArrayOrder | None = None,
         **kwargs: Any,
     ) -> Self:
```

### Comparing `cmomy-0.8.0/src/cmomy/convert.py` & `cmomy-0.9.0/src/cmomy/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Routines to convert central (co)moments to raw (co)moments. (:mod:`cmomy.convert`)
 ==================================================================================
 """
+
 from __future__ import annotations
 
 from math import prod
 from typing import TYPE_CHECKING
 
 import numpy as np
 from module_utilities.docfiller import DocFiller
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Sequence
 
     from numpy.typing import ArrayLike, DTypeLike
 
-    from .typing import ArrayOrder, MyNDArray
+    from .typing import ArrayOrder, NDArrayAny
 
 _shared_docs = r"""
 Parameters
 ----------
 x_cmom | x : ndarray
     Central moments array.  The expected structure is:
 
@@ -98,16 +99,16 @@
 def _convert_moments(
     data: ArrayLike,
     axis: int | Sequence[int],
     target_axis: int | Sequence[int],
     func: Callable[..., Any],
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     def _verify_tuple(x: int | Sequence[int]) -> tuple[int, ...]:
         if isinstance(x, int):
             return (x,)
         return tuple(x)
 
     axis = _verify_tuple(axis)
     target_axis = _verify_tuple(target_axis)
@@ -145,20 +146,20 @@
     func(data_r, out_r)
 
     return out_r.reshape(shape)
 
 
 @docfiller_decorate
 def to_raw_moments(
-    x: MyNDArray,
+    x: NDArrayAny,
     axis: int | None = -1,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     r"""
     Convert central moments to raw moments.
 
     Parameters
     ----------
     {x_cmom}
     {axis_mom}
@@ -186,20 +187,20 @@
         order=order,
         out=out,
     )
 
 
 @docfiller_decorate
 def to_raw_comoments(
-    x: MyNDArray,
+    x: NDArrayAny,
     axis: tuple[int, int] | None = (-2, -1),
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     r"""
     Convert central moments to raw moments.
 
     Parameters
     ----------
     {x_cocmom}
     {axis_comom}
@@ -227,20 +228,20 @@
         order=order,
         out=out,
     )
 
 
 @docfiller_decorate
 def to_central_moments(
-    x: MyNDArray,
+    x: NDArrayAny,
     axis: int | None = -1,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     r"""
     Convert central moments to raw moments.
 
     Parameters
     ----------
     {x_rmom}
     {axis_mom}
@@ -268,20 +269,20 @@
         order=order,
         out=out,
     )
 
 
 @docfiller_decorate
 def to_central_comoments(
-    x: MyNDArray,
+    x: NDArrayAny,
     axis: tuple[int, int] | None = (-2, -1),
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     r"""
     Convert raw comoments to central comoments.
 
     Parameters
     ----------
     {x_cormom}
     {axis_comom}
```

### Comparing `cmomy-0.8.0/src/cmomy/docstrings.py` & `cmomy-0.9.0/src/cmomy/docstrings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 """Common docstrings."""
+
 from __future__ import annotations
 
 from module_utilities.docfiller import DocFiller
 
 
 def _dummy_docstrings() -> None:
     """
     Parameters
     ----------
-    copy : bool, optional
+    copy : bool
         If True, copy the data.  If False, attempt to use view.
-    copy_kws : mapping, optional
+    copy_kws : mapping
         extra arguments to copy
-    verify : bool, optional
+    verify : bool
         If True, make sure data is c-contiguous.
     mom : int or tuple of int
         Order or moments.  If integer or length one tuple, then moments are for
         a single variable.  If length 2 tuple, then comoments of two variables
     mom_ndim : {1, 2}
         Value indicates if moments (``mom_ndim = 1``) or comoments (``mom_ndim=2``).
-    val_shape : tuple, optional
+    val_shape : tuple
         Shape of `values` part of data.  That is, the non-moment dimensions.
-    shape : tuple, optional
+    shape : tuple
         Total shape.  ``shape = val_shape + tuple(m+1 for m in mom)``
-    dtype : dtype, optional
+    dtype : dtype
         Optional ``dtype`` for output data.
-    zeros_kws : mapping, optional
+    zeros_kws : mapping
         Optional parameters to :func:`numpy.zeros`
     axis : int
         Axis to reduce along.
-    broadcast : bool, optional
+    broadcast : bool
         If True, and ``x=(x0, x1)``, then perform 'smart' broadcasting.
         In this case, if ``x1.ndim = 1`` and ``len(x1) == x0.shape[axis]``, then
         broadcast `x1` to ``x0.shape``.
-    freq : array of int, optional
+    freq : array of int
         Array of shape ``(nrep, size)`` where `nrep` is the number of replicates and
         ``size = self.shape[axis]``.  `freq` is the weight that each sample contributes
         to resamples values.  See :func:`~cmomy.resample.randsamp_freq`
-    indices : array of int, optional
+    indices : array of int
         Array of shape ``(nrep, size)``.  If passed, create `freq` from indices.
         See :func:`~cmomy.resample.randsamp_freq`.
-    nrep : int, optional
-        Number of replicates.  Create `freq` with this many replicates.
-        See :func:`~cmomy.resample.randsamp_freq`
+    nrep : int
+        Number of resample replicates.
+    nsamp : int
+        Number of samples in a single resampled replicate. Defaults to size of
+        data along sampled axis.
+    ndat : int
+        Size of data along resampled axis.
     pushed : object
         Same as object, with new data pushed onto `self.data`
     resample_kws : mapping
         Extra arguments to :func:`~cmomy.resample.resample_vals`
-    full_output : bool, optional
-        If True, also return `freq` array
+    full_output : bool
+        If True, also return ``freq`` array
     convert_kws : mapping
         Extra arguments to :func:`~cmomy.convert.to_central_moments` or
         :func:`~cmomy.convert.to_central_comoments`
-    dims : hashable or sequence of hashable, optional
+    dims : hashable or sequence of hashable
         Dimension of resulting :class:`xarray.DataArray`.
 
         * If ``len(dims) == self.ndim``, then dims specifies all dimensions.
         * If ``len(dims) == self.val_ndim``, ``dims = dims + mom_dims``
 
         Default to ``('dim_0', 'dim_1', ...)``
     mom_dims : hashable or tuple of hashable
@@ -68,25 +73,25 @@
     name : hashable
         Name of output
     indexes : Any
         indexes attribute.  This is ignored.
     template : DataArray
         If present, output will have attributes of `template`.
         Overrides other options.
-    dim : hashable, optional
+    dim : hashable
         Dimension to reduce along.
-    rep_dim : hashable, optional
+    rep_dim : hashable
         Name of new 'replicated' dimension:
-    rec_dim : hashable, optional
+    rec_dim : hashable
         Name of dimension for 'records', i.e., multiple observations.
     data : DataArray or ndarray
         Moment collection array
     parallel : bool, default=True
         flags to `numba.njit`
-    rng : :class:`~numpy.random.Generator`, optional
+    rng : :class:`~numpy.random.Generator`
         Random number generator object.  Defaults to output of :func:`~cmomy.random.default_rng`.
     kwargs | **kwargs
         Extra keyword arguments.
     """
 
 
 def _dummy_docstrings_central() -> None:
```

### Comparing `cmomy-0.8.0/src/cmomy/options.py` & `cmomy-0.9.0/src/cmomy/options.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/src/cmomy/random.py` & `cmomy-0.9.0/src/cmomy/random.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,21 +41,14 @@
 def set_internal_rng(rng: np.random.Generator) -> None:
     """
     Set the internal random number :class:`~numpy.random.Generator`.
 
     The function :func:`default_rng` will call `rng` if called with a new seed
     (or when called the first time). However, if want to override the internal
     rng, you can use this function.
-
-    Parameters
-    ----------
-    force: bool, default=False
-        If false, only set internal rng if not already set
-    If true, set internal rng
-
     """
     _DATA["rng"] = rng
 
 
 def get_internal_rng() -> np.random.Generator:
     """Get the internal random number :class:`~numpy.random.Generator`."""
     if "rng" not in _DATA:
@@ -70,26 +63,26 @@
 
 def default_rng(seed: SEED_TYPES | None = None) -> np.random.Generator:
     """
     Get default internal random number generator.
 
     Parameters
     ----------
-    seed: int, sequence of int, :class:`~numpy.random.SeedSequence`, :class:`~numpy.random.BitGenerator`, Generator, optional
+    seed:
         If specified, set the internal seed to this value. If pass in a
         :class:`numpy.random.Generator`, return that object.
 
     Returns
     -------
     Generator
-        If called with `seed=None` (default), return the previously created rng
-        (if already created). This means you can call `default_rng(seed=...)`
-        and subsequent calls of form `default_rng()` or `default_rng(None)`
-        will continue rng sequence from first call with `seed=...`. If New call
-        with `seed` set will create a new rng sequence. Note that if you pass a
+        If called with ``seed=None`` (default), return the previously created rng
+        (if already created). This means you can call ``default_rng(seed=...)``
+        and subsequent calls of form ``default_rng()`` or ``default_rng(None)``
+        will continue rng sequence from first call with ``seed=...``. If New call
+        with ``seed`` set will create a new rng sequence. Note that if you pass a
         :class:`~numpy.random.Generator` for seed, that object will be
         returned, but in this case, the internal generator will not be altered.
 
 
     """
     if isinstance(seed, np.random.Generator):
         return seed
@@ -108,22 +101,22 @@
     rng: np.random.Generator | None, seed: int | None = None
 ) -> np.random.Generator:
     """
     Decide whether to use passed :class:`~numpy.random.Generator` or that from :func:`default_rng`.
 
     Parameters
     ----------
-    rng : :class:`numpy.random.Generator`, optional
-        If pass a rng, then use it.  Otherwise, use `default_rng(seed)`
-    seed : int, optional
+    rng :
+        If pass a rng, then use it.  Otherwise, use ``default_rng(seed)``
+    seed :
         Seed to use if call :func:`default_rng`
 
     Returns
     -------
-    :class:`numpy.random.Generator`
+    Generator
     """
     if rng is None:
         return default_rng(seed=seed)
 
     if not isinstance(rng, np.random.Generator):  # pyright: ignore[reportUnnecessaryIsInstance]
         import warnings
```

### Comparing `cmomy-0.8.0/src/cmomy/resample.py` & `cmomy-0.9.0/src/cmomy/resample.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,222 +3,281 @@
 =====================================================
 """
 
 from __future__ import annotations
 
 from itertools import starmap
 from math import prod
-from typing import TYPE_CHECKING, cast
+
+# if TYPE_CHECKING:
+from typing import TYPE_CHECKING, Any, Hashable, Literal, Sequence, cast
 
 import numpy as np
 import xarray as xr
 
+from .docstrings import docfiller
 from .random import validate_rng
 from .utils import axis_expand_broadcast
 
 if TYPE_CHECKING:
-    from typing import Any, Hashable, Literal, Sequence
-
     from numpy.typing import ArrayLike, DTypeLike
 
-    from .typing import ArrayOrder, Mom_NDim, Moments, MyNDArray, XvalStrict
+    from .typing import ArrayOrder, Mom_NDim, Moments, NDArrayAny
 
 
 ##############################################################################
 # resampling
 ###############################################################################
+@docfiller.decorate
 def freq_to_indices(
-    freq: MyNDArray, shuffle: bool = True, rng: np.random.Generator | None = None
-) -> MyNDArray:
+    freq: NDArrayAny, shuffle: bool = True, rng: np.random.Generator | None = None
+) -> NDArrayAny:
     """
     Convert a frequency array to indices array.
 
     This creates an "indices" array that is compatible with "freq" array.
     Note that by default, the indices for a single sample (along output[k, :])
     are randomly shuffled.  If you pass `shuffle=False`, then the output will
     be something like [[0,0,..., 1,1,..., 2,2, ...]].
-    """
-    indices_all: list[MyNDArray] = []
+
+    Parameters
+    ----------
+    {freq}
+    shuffle :
+        If ``True`` (default), shuffle values for each row.
+    {rng}
+
+    Returns
+    -------
+    ndarray :
+        Indices array of shape ``(nrep, nsamp)`` where ``nsamp = freq[k,
+        :].sum()`` where `k` is any row.
+    """
+    indices_all: list[NDArrayAny] = []
+
+    # validate freq -> indices
+    nsamps = freq.sum(-1)  # pyright: ignore[reportUnknownMemberType]
+    if any(nsamps[0] != nsamps):
+        msg = "Inconsistent number of samples from freq array"
+        raise ValueError(msg)
 
     for f in freq:
         indices = np.concatenate(list(starmap(np.repeat, enumerate(f))))
         indices_all.append(indices)
 
     out = np.array(indices_all)
 
     if shuffle:
         rng = validate_rng(rng)
         rng.shuffle(out, axis=1)
 
     return out
 
 
-def indices_to_freq(indices: MyNDArray) -> MyNDArray:
-    """Convert indices to frequency array."""
+def indices_to_freq(indices: NDArrayAny, ndat: int | None = None) -> NDArrayAny:
+    """
+    Convert indices to frequency array.
+
+    It is assumed that ``indices.shape == (nrep, nsamp)`` with ``nsamp == ndat``.
+    For cases that ``nsamp != ndat``, pass in ``ndat``.
+    """
     from ._lib.resample import (
-        randsamp_freq_indices,  # pyright: ignore[reportUnknownVariableType]
+        randsamp_indices_to_freq,  # pyright: ignore[reportUnknownVariableType]
     )
 
-    freq = np.zeros_like(indices)
-    randsamp_freq_indices(indices, freq)
+    ndat = indices.shape[1] if ndat is None else ndat
+    freq = np.zeros((indices.shape[0], ndat), dtype=indices.dtype)
+
+    randsamp_indices_to_freq(indices, freq)
 
     return freq
 
 
+@docfiller.decorate
 def random_indices(
-    nrep: int, ndat: int, rng: np.random.Generator | None = None, replace: bool = True
-) -> MyNDArray:
+    nrep: int,
+    ndat: int,
+    nsamp: int | None = None,
+    rng: np.random.Generator | None = None,
+    replace: bool = True,
+) -> NDArrayAny:
     """
     Create indices for random resampling (bootstrapping).
 
     Parameters
     ----------
-    nrep, ndat : int
-        Number of repetitions (`nrep`) and size of data to sample along (ndat).
-    rng : Generator, optional
-        Optional Generator.
-    replace : bool, default=True
+    {nrep}
+    {ndat}
+    {nsamp}
+    {rng}
+    replace :
         Whether to allow replacement.
+
+    Returns
+    -------
+    indices : ndarray
+        Index array of integers of shape ``(nrep, nsamp)``.
     """
-    rng = validate_rng(rng)
-    return rng.choice(ndat, size=(nrep, ndat), replace=replace)
+    nsamp = ndat if nsamp is None else nsamp
+    return validate_rng(rng).choice(ndat, size=(nrep, nsamp), replace=replace)
 
 
+@docfiller.inherit(random_indices)
 def random_freq(
-    nrep: int, ndat: int, rng: np.random.Generator | None = None, replace: bool = True
-) -> MyNDArray:
+    nrep: int,
+    ndat: int,
+    nsamp: int | None = None,
+    rng: np.random.Generator | None = None,
+    replace: bool = True,
+) -> NDArrayAny:
     """
     Create frequencies for random resampling (bootstrapping).
 
+    Returns
+    -------
+    freq : ndarray
+        Frequency array. ``freq[rep, k]`` is the number of times to sample from the `k`th
+        observation for replicate `rep`.
+
     See Also
     --------
     random_indices
     """
     return indices_to_freq(
-        random_indices(nrep=nrep, ndat=ndat, rng=rng, replace=replace)
+        indices=random_indices(
+            nrep=nrep, ndat=ndat, nsamp=nsamp, rng=rng, replace=replace
+        ),
+        ndat=ndat,
     )
 
 
 def _validate_resample_array(
     x: ArrayLike,
+    ndat: int,
     nrep: int | None,
-    ndat: int | None,
+    is_freq: bool,
     check: bool = True,
-    name: str = "array",
-) -> MyNDArray:
+) -> NDArrayAny:
     x = np.asarray(x, dtype=np.int64)
     if check:
+        name = "freq" if is_freq else "indices"
         if x.ndim != 2:
             msg = f"{name}.ndim={x.ndim} != 2"
             raise ValueError(msg)
 
         if nrep is not None and x.shape[0] != nrep:
             msg = f"{name}.shape[0]={x.shape[0]} != {nrep}"
             raise ValueError(msg)
 
-        if ndat is None:
-            raise ValueError
+        if is_freq:
+            if x.shape[1] != ndat:
+                msg = f"{name} has wrong ndat"
+                raise ValueError(msg)
+
+        else:
+            # only restriction is that values in [0, ndat)
+            min_, max_ = x.min(), x.max()  # pyright: ignore[reportUnknownMemberType]
+            if min_ < 0 or max_ >= ndat:
+                msg = f"Indices range [{min_}, {max_}) outside [0, {ndat - 1})"
+                raise ValueError(msg)
 
-        if x.shape[1] != ndat:
-            msg = f"{name} has wrong ndat"
-            raise ValueError(msg)
     return x
 
 
+@docfiller.decorate
 def randsamp_freq(
+    ndat: int,
     nrep: int | None = None,
-    ndat: int | None = None,
+    nsamp: int | None = None,
     indices: ArrayLike | None = None,
     freq: ArrayLike | None = None,
     check: bool = False,
     rng: np.random.Generator | None = None,
-) -> MyNDArray:
+) -> NDArrayAny:
     """
     Produce a random sample for bootstrapping.
 
+    In order, the return will be one of ``freq``, frequencies from ``indices`` or
+    new sample from :func:`random_freq`.
+
     Parameters
     ----------
-    ndat : int, optional
-        data dimension ndat
-    freq : array-like,  optional
-        `shape=(nrep, ndat)`.
-        If passed, use this frequency array.
-        overrides ndat
-    indices : array-like, , optional
-        `shape=(nrep, ndat)`.
-        if passed and `freq` is `None`, construct frequency
-        array from this indices array
-
-    nrep : int, optional
-        if `freq` and `indices` are `None`, construct
-        sample with this number of repetitions
-    indices : array-like, optional
-        if passed, build frequency table based on this sampling.
-        shape = (nrep, ndat)
-    freq : array-like, optional
-        if passed, use this frequency array
+    {nrep}
+    {ndat}
+    {nsamp}
+    {freq}
+    {indices}
     check : bool, default=False
         if `check` is `True`, then check `freq` and `indices` against `ndat` and `nrep`
 
     Returns
     -------
-    output : ndarray
-        Frequency table of shape ``(nrep, ndat)``.
+    freq : ndarray
+        Frequency array.
+
+    See Also
+    --------
+    random_freq
+    indices_to_freq
     """
     if freq is not None:
         freq = _validate_resample_array(
-            freq, name="freq", nrep=nrep, ndat=ndat, check=check
+            freq,
+            nrep=nrep,
+            ndat=ndat,
+            check=check,
+            is_freq=True,
         )
 
     elif indices is not None:
         indices = _validate_resample_array(
-            indices, name="indices", nrep=nrep, ndat=ndat, check=check
+            indices,
+            nrep=nrep,
+            ndat=ndat,
+            check=check,
+            is_freq=False,
         )
-        freq = indices_to_freq(indices)
 
-    elif nrep is not None and ndat is not None:
-        freq = random_freq(nrep=nrep, ndat=ndat, rng=validate_rng(rng), replace=True)
+        freq = indices_to_freq(indices, ndat=ndat)
+
+    elif nrep is not None:
+        freq = random_freq(
+            nrep=nrep, ndat=ndat, nsamp=nsamp, rng=validate_rng(rng), replace=True
+        )
 
     else:
-        msg = "must specify freq, indices, or nrep and ndat"
+        msg = "must specify freq, indices, or nrep"
         raise ValueError(msg)
 
     return freq
 
 
+@docfiller.decorate
 def resample_data(  # noqa: PLR0914
     data: ArrayLike,
     freq: ArrayLike,
     mom: Moments,
     axis: int = 0,
     dtype: DTypeLike | None = None,
     order: ArrayOrder = None,
     parallel: bool = True,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
     """
     Resample data according to frequency table.
 
     Parameters
     ----------
     data : array-like
         central mom array to be resampled
-    freq : array-like
-        frequency array with shape (nrep, data.shape[axis])
-    mom : int or array-like
-        if int or length 1, then data contains central mom.
-        if length is 2, then data contains central comoments
-    axis : int, default=0
-        axis to reduce along
-    parallel : bool
-        option to run jitted pusher in parallel.
-    dtype, order : object
-        options to :func:`numpy.asarray`
+    {freq}
+    {mom}
+    {parallel}
     out : ndarray, optional
-      optional output array.
+        optional output array.
 
     Returns
     -------
     output : array
         output shape is `(nrep,) + shape + mom`, where shape is
         the shape of data less axis, and mom is the shape of the resulting mom.
     """
@@ -277,28 +336,54 @@
 
     outr.fill(0.0)
     resample(datar, freq, outr)
 
     return outr.reshape(out.shape)
 
 
+@docfiller.decorate
 def resample_vals(  # noqa: C901,PLR0912,PLR0914,PLR0915
-    x: XvalStrict,
-    freq: MyNDArray,
+    x: NDArrayAny | tuple[NDArrayAny, NDArrayAny],
+    freq: NDArrayAny,
     mom: Moments,
     axis: int = 0,
-    w: MyNDArray | None = None,
+    w: NDArrayAny | None = None,
     mom_ndim: Mom_NDim | None = None,
     broadcast: bool = False,
     dtype: DTypeLike | None = None,
     order: ArrayOrder = None,
     parallel: bool = True,
-    out: MyNDArray | None = None,
-) -> MyNDArray:
-    """Resample data according to frequency table."""
+    out: NDArrayAny | None = None,
+) -> NDArrayAny:
+    """
+    Resample data according to frequency table.
+
+    Parameters
+    ----------
+    x : ndarray or tuple of ndarray
+        Input values.
+    {freq}
+    {mom}
+    {axis}
+    w :
+        Weights array.
+    {mom_ndim}
+    {broadcast}
+    {dtype}
+    order :
+        Parameter ``order`` to :func:`numpy.asarray`.
+    {parallel}
+    out : ndarray
+        Optional output array.
+
+    Returns
+    -------
+    ndarray
+        Resampled central moments array.
+    """
     from ._lib.resample import factory_resample_vals
 
     if isinstance(mom, int):
         mom = (mom,)
     elif not isinstance(mom, tuple):  # pyright: ignore[reportUnnecessaryIsInstance]
         raise TypeError
 
@@ -388,21 +473,21 @@
         resample(wr, xr, freq, outr)
 
     return outr.reshape(out.shape)
 
 
 # TODO(wpk): add coverage for these
 def bootstrap_confidence_interval(  # pragma: no cover
-    distribution: MyNDArray,
-    stats_val: MyNDArray | Literal["percentile", "mean", "median"] | None = "mean",
+    distribution: NDArrayAny,
+    stats_val: NDArrayAny | Literal["percentile", "mean", "median"] | None = "mean",
     axis: int = 0,
     alpha: float = 0.05,
     style: Literal[None, "delta", "pm"] = None,
     **kwargs: Any,
-) -> MyNDArray:
+) -> NDArrayAny:
     """
     Calculate the error bounds.
 
     Parameters
     ----------
     distribution : array-like
         distribution of values to consider
@@ -474,15 +559,15 @@
     elif style == "pm":
         out = np.array([val, (high - low) / 2.0])
     return out
 
 
 def xbootstrap_confidence_interval(  # pragma: no cover
     x: xr.DataArray,
-    stats_val: MyNDArray | Literal["percentile", "mean", "median"] | None = "mean",
+    stats_val: NDArrayAny | Literal["percentile", "mean", "median"] | None = "mean",
     axis: int = 0,
     dim: Hashable | None = None,
     alpha: float = 0.05,
     style: Literal[None, "delta", "pm"] = None,
     bootstrap_dim: Hashable | None = "bootstrap",
     bootstrap_coords: str | Sequence[str] | None = None,
     **kwargs: Any,
```

### Comparing `cmomy-0.8.0/src/cmomy/typing.py` & `cmomy-0.9.0/src/cmomy/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Useful typing stuff."""
+"""
+Typing aliases (:mod:`cmomy.typing`)
+====================================
+"""
 
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -12,43 +15,53 @@
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 
+# put outside to get autodoc typehints working...
+import pandas as pd
+import xarray as xr
 from numpy.typing import ArrayLike, NDArray
 
 if TYPE_CHECKING:
-    import pandas as pd
-    import xarray as xr
-
     from ._typing_compat import TypeAlias
     from .abstract_central import CentralMomentsABC
 
-MyDType: TypeAlias = Any
-MyNDArray: TypeAlias = NDArray[MyDType]
 
-Moments: TypeAlias = Union[int, "tuple[int]", "tuple[int, int]"]
-MomentsStrict: TypeAlias = Union["tuple[int]", "tuple[int, int]"]
-XvalStrict: TypeAlias = Union[MyNDArray, "tuple[MyNDArray, MyNDArray]"]
+# Arrays
+DTypeAny: TypeAlias = Any
+NDArrayAny: TypeAlias = NDArray[DTypeAny]
 ArrayOrder = Literal["C", "F", "A", "K", None]
 
-T_Array = TypeVar("T_Array", "MyNDArray", "xr.DataArray")
-T_CentralMoments = TypeVar("T_CentralMoments", bound="CentralMomentsABC[MyDType]")
-
-MomDims = Union[Hashable, Tuple[Hashable], Tuple[Hashable, Hashable]]
+# Moments
+Moments: TypeAlias = Union[int, "tuple[int]", "tuple[int, int]"]
+MomentsStrict: TypeAlias = Union["tuple[int]", "tuple[int, int]"]
 Mom_NDim = Literal[1, 2]
 
+# Generic array
+T_Array = TypeVar("T_Array", NDArrayAny, xr.DataArray)
+T_CentralMoments = TypeVar("T_CentralMoments", bound="CentralMomentsABC[DTypeAny]")
+
+# Dummy function
 FuncType = Callable[..., Any]
 F = TypeVar("F", bound=FuncType)
 
 # xarray specific stuff
+MomDims = Union[Hashable, Tuple[Hashable], Tuple[Hashable, Hashable]]
+
+# fix if using autodoc typehints...
+if TYPE_CHECKING:
+    _Index: TypeAlias = "pd.Index[Any]"  # type: ignore[type-arg,unused-ignore]  # py38 type error
+else:
+    _Index: TypeAlias = pd.Index
+
 XArrayCoordsType: TypeAlias = Union[
-    Sequence[Union[Sequence[Any], "pd.Index[Any]", "xr.DataArray"]],
+    Sequence[Union[Sequence[Any], _Index, xr.DataArray]],
     Mapping[Any, Any],
     None,
 ]
 
 XArrayAttrsType: TypeAlias = Optional[Mapping[Any, Any]]
 XArrayNameType: TypeAlias = Optional[Hashable]
 XArrayDimsType: TypeAlias = Union[Hashable, Sequence[Hashable], None]
@@ -56,8 +69,10 @@
 
 
 # literals
 VerifyValuesStyles = Literal["val", "vals", "data", "datas", "var", "vars"]
 
 # pushing arrays
 MultiArray = Union[float, ArrayLike, T_Array]
+"""Generic array."""
 MultiArrayVals = Union[ArrayLike, T_Array]
+"""Generic value array."""
```

### Comparing `cmomy-0.8.0/src/cmomy/utils.py` & `cmomy-0.9.0/src/cmomy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Utilities."""
+
 from __future__ import annotations
 
 # from functools import lru_cache
 from typing import TYPE_CHECKING, cast
 
 import numpy as np
 
 from .docstrings import docfiller
 
 if TYPE_CHECKING:
     from typing import Sequence
 
     from numpy.typing import ArrayLike, DTypeLike
 
-    from .typing import ArrayOrder, Mom_NDim, Moments, MomentsStrict, MyNDArray
+    from .typing import ArrayOrder, Mom_NDim, Moments, MomentsStrict, NDArrayAny
 
 
 def normalize_axis_index(axis: int, ndim: int) -> int:
     """Interface to numpy.core.multiarray.normalize_axis_index"""
     import numpy.core.multiarray as ma
 
     return ma.normalize_axis_index(axis, ndim)  # type: ignore[no-any-return,attr-defined]
@@ -53,27 +54,27 @@
     axis: int | None,
     verify: bool = True,
     expand: bool = True,
     broadcast: bool = True,
     roll: bool = True,
     dtype: DTypeLike | None = None,
     order: ArrayOrder = None,
-) -> MyNDArray:
+) -> NDArrayAny:
     """
     Broadcast x to shape.
 
     If x is 1d, and shape is n-d, but len(x) is same as shape[axis],
     broadcast x across all dimensions
     """
     if verify is True:
         x = np.asarray(x, dtype=dtype, order=order)
     elif not isinstance(x, np.ndarray):
         msg = f"{type(x)=} must be np.ndarray"
         raise TypeError(msg)
-    x = cast("MyNDArray", x)
+    x = cast("NDArrayAny", x)
 
     # if array, and 1d with size same as shape[axis]
     # broadcast from here
     if expand and x.ndim == 1 and x.ndim != len(shape):
         if axis is None:
             msg = "trying to expand an axis with axis==None"
             raise ValueError(msg)
```

### Comparing `cmomy-0.8.0/src/cmomy/xcentral.py` & `cmomy-0.9.0/src/cmomy/xcentral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Thin wrapper around central routines with xarray support."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast, overload  # TYPE_CHECKING,
 
 import numpy as np
+
+# pandas needed for autdoc typehints
+import pandas as pd  # noqa: F401  # pyright: ignore[reportUnusedImport]
 import xarray as xr
 from module_utilities import cached
 
 from . import convert
 from ._compat import xr_dot
 from .abstract_central import CentralMomentsABC
 from .docstrings import docfiller_xcentral as docfiller
@@ -38,15 +42,15 @@
     from .central import CentralMoments
     from .typing import (
         Mom_NDim,
         MomDims,
         Moments,
         MultiArray,
         MultiArrayVals,
-        MyNDArray,
+        NDArrayAny,
         XArrayAttrsType,
         XArrayCoordsType,
         XArrayDimsType,
         XArrayIndexesType,
         XArrayNameType,
     )
 
@@ -105,16 +109,16 @@
         #     mom_dims = tuple(mom_dims)
         mom_dims = (mom_dims,) if isinstance(mom_dims, str) else tuple(mom_dims)  # type: ignore[arg-type]
 
         if mom_ndim is not None and len(mom_dims) != mom_ndim:
             msg = f"len(mom_dims)={len(mom_dims)} not equal to mom_ndim={mom_ndim}"
             raise ValueError(msg)
 
-        order = (..., *mom_dims)
-        x = x.transpose(*order)
+        order = (..., *mom_dims)  # pyright: ignore[reportUnknownVariableType]
+        x = x.transpose(*order)  # pyright: ignore[reportUnknownArgumentType]
 
     return x
 
 
 # * xcentral moments/comoments
 def _xcentral_moments(
     vals: xr.DataArray,
@@ -332,15 +336,15 @@
             raise TypeError(msg)
 
         if data.ndim < mom_ndim:
             msg = "not enough dimensions in data"
             raise ValueError(msg)
 
         self._mom_ndim = mom_ndim
-        self._data: MyNDArray = data.to_numpy()  # pyright: ignore[reportUnknownMemberType]
+        self._data: NDArrayAny = data.to_numpy()  # pyright: ignore[reportUnknownMemberType]
         self._data_flat = self._data.reshape(self.shape_flat)
         self._data = self._data_flat.reshape(data.shape)  # ensure same data
         self._xdata = data.copy(data=self._data)
 
         if any(m <= 0 for m in self.mom):
             msg = "moments must be positive"
             raise ValueError(msg)
@@ -405,21 +409,21 @@
 
     # ** top level creation/copy/new
     # @cached.prop
     # def _template_val(self) -> xr.DataArray:
     #     """Template for values part of data."""
     #     return self._xdata[self._weight_index]
 
-    def _wrap_like(self, x: MyNDArray) -> xr.DataArray:
+    def _wrap_like(self, x: NDArrayAny) -> xr.DataArray:
         return self._xdata.copy(data=x)
 
     @docfiller_abc()
     def new_like(
         self,
-        data: MyNDArray | xr.DataArray | None = None,
+        data: NDArrayAny | xr.DataArray | None = None,
         *,
         copy: bool = False,
         copy_kws: Mapping[str, Any] | None = None,
         verify: bool = False,
         strict: bool = False,
         **kwargs: Any,
     ) -> Self:
@@ -928,21 +932,21 @@
         )
 
     # ** Push/verify
     def _xverify_value(  # noqa: C901,PLR0912,PLR0915
         self,
         *,
         x: MultiArray[xr.DataArray],
-        target: str | MyNDArray | xr.DataArray | None = None,
+        target: str | NDArrayAny | xr.DataArray | None = None,
         dim: Hashable | None = None,
         axis: int | None = None,
         broadcast: bool = False,
         expand: bool = False,
         shape_flat: Any | None = None,
-    ) -> tuple[MyNDArray, xr.DataArray]:
+    ) -> tuple[NDArrayAny, xr.DataArray]:
         if isinstance(x, xr.DataArray):
             x = x.astype(dtype=self.dtype, copy=False)  # pyright: ignore[reportUnknownMemberType]
         else:
             x = np.asarray(x, dtype=self.dtype)
 
         target_dims: None | tuple[Hashable, ...] = None
         if isinstance(target, str):
@@ -1018,15 +1022,15 @@
                     x = xr.DataArray(x, dims=dim).broadcast_like(target)  # type: ignore[arg-type,unused-ignore] # pyright: ignore[reportArgumentType]
 
                 elif x.shape == target.shape:
                     x = xr.DataArray(x, dims=target.dims)
                 else:
                     raise ValueError
 
-        values: MyNDArray = x.to_numpy() if isinstance(x, xr.DataArray) else x  # pyright: ignore[reportUnknownMemberType, reportUnnecessaryIsInstance]
+        values: NDArrayAny = x.to_numpy() if isinstance(x, xr.DataArray) else x  # pyright: ignore[reportUnknownMemberType, reportUnnecessaryIsInstance]
 
         # check shape
         if values.shape != target_shape:  # pragma: no cover
             raise ValueError
         if dim is None:
             nrec: tuple[int, ...] = ()
         else:
@@ -1040,22 +1044,22 @@
 
         return values, target_output
 
     def _verify_value(
         self,
         *,
         x: MultiArray[xr.DataArray],
-        target: str | MyNDArray | xr.DataArray,
+        target: str | NDArrayAny | xr.DataArray,
         shape_flat: tuple[int, ...],
         axis: int | None = None,
         dim: Hashable | None = None,
         broadcast: bool = False,
         expand: bool = False,
-        other: MyNDArray | None = None,
-    ) -> tuple[MyNDArray, MyNDArray | xr.DataArray]:
+        other: NDArrayAny | None = None,
+    ) -> tuple[NDArrayAny, NDArrayAny | xr.DataArray]:
         if isinstance(x, xr.DataArray) or isinstance(target, xr.DataArray):
             return self._xverify_value(
                 x=x,
                 target=target,
                 axis=axis,
                 dim=dim,
                 # dim=axis,
@@ -1128,91 +1132,93 @@
     # ** Manipulation
     @overload
     def resample_and_reduce(
         self,
         nrep: int | None = ...,
         *,
         full_output: Literal[False] = ...,
+        nsamp: int | None = ...,
         dim: Hashable | None = ...,
         rep_dim: str = ...,
         axis: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
         **kwargs: Any,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     @overload
     def resample_and_reduce(
         self,
         nrep: int | None = ...,
         *,
         full_output: Literal[True],
+        nsamp: int | None = ...,
         dim: Hashable | None = ...,
         rep_dim: str = ...,
         axis: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
         **kwargs: Any,
-    ) -> tuple[Self, MyNDArray]:
-        ...
+    ) -> tuple[Self, NDArrayAny]: ...
 
     @overload
     def resample_and_reduce(
         self,
         nrep: int | None = ...,
         *,
         full_output: bool,
+        nsamp: int | None = ...,
         dim: Hashable | None = ...,
         rep_dim: str = ...,
         axis: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
         **kwwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
-        ...
+    ) -> Self | tuple[Self, NDArrayAny]: ...
 
     @docfiller.decorate
     def resample_and_reduce(
         self,
         nrep: int | None = None,
         *,
         full_output: bool = False,
+        nsamp: int | None = None,
         dim: Hashable | None = None,
         rep_dim: str = "rep",
         axis: int | None = None,
-        freq: MyNDArray | None = None,
-        indices: MyNDArray | None = None,
+        freq: NDArrayAny | None = None,
+        indices: NDArrayAny | None = None,
         parallel: bool = True,
         resample_kws: Mapping[str, Any] | None = None,
         rng: np.random.Generator | None = None,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
+    ) -> Self | tuple[Self, NDArrayAny]:
         """
 
         Parameters
         ----------
-        {freq}
-        {indices}
         {nrep}
-        {axis}
+        {full_output}
+        {nsamp}
         {dim}
         {rep_dim}
+        {axis}
+        {freq}
+        {indices}
         {parallel}
         {resample_kws}
-        {full_output}
         {rng}
         **kwargs
             Arguments to :meth:`CentralMoments.resample_and_reduce`
 
         Returns
         -------
         output : {klass}
@@ -1272,21 +1278,22 @@
 
         if dim in self.mom_dims:
             msg = f"can only resample from value dimensions {self.val_dims}"
             raise ValueError(msg)
 
         # Final form will move `dim` to front of array.
         # this will be replaced by rep_dimension
-        template = self.to_dataarray().isel({dim: 0})
+        template = self.to_dataarray().isel({dim: 0}, drop=True)
 
         out, freq = self.centralmoments_view.resample_and_reduce(
             freq=freq,
             indices=indices,
             nrep=nrep,
             axis=axis,
+            nsamp=nsamp,
             parallel=parallel,
             resample_kws=resample_kws,
             full_output=True,
             rng=rng,
             **kwargs,
         )
 
@@ -1310,15 +1317,15 @@
     ) -> Self:
         """
         Parameters
         ----------
         {dim}
         {axis}
         **kwargs
-        Extra arguments to :meth:`from_datas`
+            Extra arguments to :meth:`from_datas`
 
         Returns
         -------
         output : {klass}
             Reduced along dimension
 
         See Also
@@ -1457,15 +1464,15 @@
 
         start = 0 if coords_policy == "first" else block_size - 1
 
         # get template values
         template = (
             self.to_dataarray()
             .isel({dim: slice(start, block_size * nblock, block_size)})
-            .transpose(dim, ...)
+            .transpose(dim, ...)  # pyright: ignore[reportUnknownArgumentType]
         )
 
         if coords_policy is None:
             if not isinstance(dim, str):  # pragma: no cover
                 raise TypeError
             template = template.drop_vars(dim)
 
@@ -1541,15 +1548,15 @@
             **kwargs,
         ).zero()
 
     @classmethod
     @docfiller_inherit_abc()
     def from_data(  # noqa: PLR0913
         cls,
-        data: MyNDArray | xr.DataArray,
+        data: NDArrayAny | xr.DataArray,
         *,
         mom: Moments | None = None,
         mom_ndim: Mom_NDim | None = None,
         val_shape: tuple[int, ...] | None = None,
         copy: bool = True,
         copy_kws: Mapping[str, Any] | None = None,
         verify: bool = False,
@@ -1630,15 +1637,15 @@
             mom_dims=mom_dims,
         )
 
     @classmethod
     @docfiller_inherit_abc()
     def from_datas(  # noqa: PLR0913
         cls,
-        datas: MyNDArray | xr.DataArray,
+        datas: NDArrayAny | xr.DataArray,
         *,
         mom: Moments | None = None,
         mom_ndim: Mom_NDim | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         verify: bool = False,
         axis: int | None = None,
@@ -1676,21 +1683,21 @@
 
 
         """
         if isinstance(datas, xr.DataArray):
             axis, dim = _select_axis_dim(dims=datas.dims, axis=axis, dim=dim)
             mom_ndim = select_mom_ndim(mom=mom, mom_ndim=mom_ndim)
             # move moments to end and dim to beginning
-            datas = _move_mom_dims_to_end(datas, mom_dims, mom_ndim).transpose(dim, ...)
+            datas = _move_mom_dims_to_end(datas, mom_dims, mom_ndim).transpose(dim, ...)  # pyright: ignore[reportUnknownArgumentType]
 
             if verify:
                 datas = datas.astype(order="C", dtype=dtype, copy=False)  # pyright: ignore[reportUnknownMemberType]
 
             new = cls.from_data(
-                data=xr.zeros_like(datas.isel({dim: 0})),  # pyright: ignore[reportUnknownMemberType]
+                data=xr.zeros_like(datas.isel({dim: 0}, drop=True)),  # pyright: ignore[reportUnknownMemberType]
                 mom=mom,
                 mom_ndim=mom_ndim,
                 val_shape=val_shape,
                 dtype=dtype,
                 verify=False,  # already did this...
                 **kwargs,
             ).push_datas(datas, dim=dim)
@@ -1717,22 +1724,22 @@
 
         return new
 
     @classmethod
     @docfiller_inherit_abc()
     def from_vals(  # noqa: PLR0913
         cls,
-        x: MyNDArray
-        | tuple[MyNDArray, MyNDArray]
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray]
-        | tuple[xr.DataArray, MyNDArray],
+        | tuple[xr.DataArray, NDArrayAny],
         mom: Moments,
         *,
-        w: float | MyNDArray | xr.DataArray | None = None,
+        w: float | NDArrayAny | xr.DataArray | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         broadcast: bool = False,
         axis: int | None = None,
         dim: Hashable | None = None,
         dims: XArrayDimsType = None,
         attrs: XArrayAttrsType = None,
@@ -1765,15 +1772,15 @@
             axis, dim = _select_axis_dim(dims=x0.dims, axis=axis, dim=dim)
 
             if val_shape is None:
                 val_shape = shape_reduce(shape=x0.shape, axis=axis)
             if dtype is None:
                 dtype = x0.dtype  # pyright: ignore[reportUnknownMemberType]
 
-            template = x0.isel({dim: 0})
+            template = x0.isel({dim: 0}, drop=True)
 
             dims = template.dims
             if coords is None:
                 coords = {}
             coords = {**template.coords, **coords}  # type: ignore[dict-item] # pyright: ignore[reportUnknownMemberType,reportGeneralTypeIssues]
             if attrs is None:
                 attrs = {}
@@ -1816,25 +1823,26 @@
 
         return new
 
     @overload
     @classmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray
-        | tuple[MyNDArray, MyNDArray]
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray],
         mom: Moments,
         *,
         full_output: Literal[False] = ...,
         nrep: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
-        w: MyNDArray | xr.DataArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
+        w: NDArrayAny | xr.DataArray | None = ...,
         dim: Hashable | None = ...,
         rep_dim: str = ...,
         dtype: DTypeLike | None = ...,
         broadcast: bool = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
@@ -1843,32 +1851,32 @@
         dims: XArrayDimsType = ...,
         attrs: XArrayAttrsType = ...,
         coords: XArrayCoordsType = ...,
         indexes: XArrayIndexesType = ...,
         name: XArrayNameType = ...,
         mom_dims: MomDims | None = ...,
         **kwargs: Any,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     @overload
     @classmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray
-        | tuple[MyNDArray, MyNDArray]
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray],
         mom: Moments,
         *,
         full_output: Literal[True],
         nrep: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
-        w: MyNDArray | xr.DataArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
+        w: NDArrayAny | xr.DataArray | None = ...,
         dim: Hashable | None = ...,
         rep_dim: str = ...,
         dtype: DTypeLike | None = ...,
         broadcast: bool = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
@@ -1877,32 +1885,32 @@
         dims: XArrayDimsType = ...,
         attrs: XArrayAttrsType = ...,
         coords: XArrayCoordsType = ...,
         indexes: XArrayIndexesType = ...,
         name: XArrayNameType = ...,
         mom_dims: MomDims | None = ...,
         **kwargs: Any,
-    ) -> tuple[Self, MyNDArray]:
-        ...
+    ) -> tuple[Self, NDArrayAny]: ...
 
     @overload
     @classmethod
     def from_resample_vals(
         cls,
-        x: MyNDArray
-        | tuple[MyNDArray, MyNDArray]
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray],
         mom: Moments,
         *,
         full_output: bool,
         nrep: int | None = ...,
-        freq: MyNDArray | None = ...,
-        indices: MyNDArray | None = ...,
-        w: MyNDArray | xr.DataArray | None = ...,
+        nsamp: int | None = ...,
+        freq: NDArrayAny | None = ...,
+        indices: NDArrayAny | None = ...,
+        w: NDArrayAny | xr.DataArray | None = ...,
         dim: Hashable | None = ...,
         rep_dim: str = ...,
         dtype: DTypeLike | None = ...,
         broadcast: bool = ...,
         parallel: bool = ...,
         resample_kws: Mapping[str, Any] | None = ...,
         rng: np.random.Generator | None = ...,
@@ -1911,32 +1919,32 @@
         dims: XArrayDimsType = ...,
         attrs: XArrayAttrsType = ...,
         coords: XArrayCoordsType = ...,
         indexes: XArrayIndexesType = ...,
         name: XArrayNameType = ...,
         mom_dims: MomDims | None = ...,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
-        ...
+    ) -> Self | tuple[Self, NDArrayAny]: ...
 
     @classmethod
     @docfiller_inherit_abc()
     def from_resample_vals(  # noqa: C901,PLR0913,PLR0912
         cls,
-        x: MyNDArray
-        | tuple[MyNDArray, MyNDArray]
+        x: NDArrayAny
+        | tuple[NDArrayAny, NDArrayAny]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray],
         mom: Moments,
         *,
         full_output: bool = False,
         nrep: int | None = None,
-        freq: MyNDArray | None = None,
-        indices: MyNDArray | None = None,
-        w: MyNDArray | xr.DataArray | None = None,
+        nsamp: int | None = None,
+        freq: NDArrayAny | None = None,
+        indices: NDArrayAny | None = None,
+        w: NDArrayAny | xr.DataArray | None = None,
         dim: Hashable | None = None,
         rep_dim: str = "rep",
         dtype: DTypeLike | None = None,
         broadcast: bool = False,
         parallel: bool = True,
         resample_kws: Mapping[str, Any] | None = None,
         rng: np.random.Generator | None = None,
@@ -1945,15 +1953,15 @@
         dims: XArrayDimsType = None,
         attrs: XArrayAttrsType = None,
         coords: XArrayCoordsType = None,
         indexes: XArrayIndexesType = None,  # noqa: ARG003
         name: XArrayNameType = None,
         mom_dims: MomDims | None = None,
         **kwargs: Any,
-    ) -> Self | tuple[Self, MyNDArray]:
+    ) -> Self | tuple[Self, NDArrayAny]:
         """
         Parameters
         ----------
         x : array, tuple of array, DataArray, or tuple of DataArray
             For moments, `x=x0`.  For comoments, `x=(x0, x1)`.
             If pass DataArray, inherit attributes from `x0`.  If pass
             ndarray, use `dims`, `attrs`, etc to wrap final result
@@ -1970,51 +1978,52 @@
 
         x0 = x[0] if isinstance(x, tuple) else x
 
         if isinstance(x0, xr.DataArray):
             axis, dim = _select_axis_dim(dims=x0.dims, axis=axis, dim=dim)
             # TODO(wpk): create object, and verify y, and w against x
             # override final xarray stuff:
-            template = x0.isel({dim: 0})
+            template = x0.isel({dim: 0}, drop=True)
             dims = template.dims
             if coords is None:
                 coords = {}
             coords = {**template.coords, **coords}  # type: ignore[dict-item]  # pyright: ignore[reportUnknownMemberType,reportGeneralTypeIssues]
             if attrs is None:
                 attrs = {}
             attrs = dict(template.attrs, **attrs)
             if name is None:
                 name = template.name
 
-        w_values: MyNDArray | None
+        w_values: NDArrayAny | None
         if isinstance(w, xr.DataArray):
             if isinstance(x0, xr.DataArray):
                 w_values = w.broadcast_like(x0).to_numpy()  # pyright: ignore[reportUnknownMemberType]
 
             else:  # pragma: no cover
                 w_values = w.to_numpy()  # pyright: ignore[reportUnknownMemberType]
         else:
             w_values = w
 
         if dims is not None:
             if isinstance(dims, str):  # pragma: no cover
                 dims = (dims,)
             dims = (rep_dim, *dims)  # type: ignore[misc]
 
-        x_array: MyNDArray | tuple[MyNDArray, MyNDArray]
+        x_array: NDArrayAny | tuple[NDArrayAny, NDArrayAny]
         if isinstance(x, tuple):
             x_array = tuple(np.array(xx, copy=False) for xx in x)  # type: ignore[assignment]
         else:
             x_array = np.array(x, copy=False)
 
         out, freq = CentralMoments.from_resample_vals(
             x=x_array,
             freq=freq,
             indices=indices,
             nrep=nrep,
+            nsamp=nsamp,
             w=w_values,
             axis=axis,
             mom=mom,
             dtype=dtype,
             broadcast=broadcast,
             parallel=parallel,
             resample_kws=resample_kws,
@@ -2037,15 +2046,15 @@
             return (new, freq)
         return new
 
     @classmethod
     @docfiller_inherit_abc()
     def from_raw(
         cls,
-        raw: MyNDArray | xr.DataArray,
+        raw: NDArrayAny | xr.DataArray,
         *,
         mom_ndim: Mom_NDim | None = None,
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         convert_kws: Mapping[str, Any] | None = None,
         dims: XArrayDimsType = None,
@@ -2074,15 +2083,15 @@
             mom_ndim = select_mom_ndim(mom=mom, mom_ndim=mom_ndim)
 
             raw = _move_mom_dims_to_end(raw, mom_dims, mom_ndim)
 
             if convert_kws is None:
                 convert_kws = {}
 
-            values = cast("MyNDArray", raw.to_numpy())  # pyright: ignore[reportUnknownMemberType]
+            values = cast("NDArrayAny", raw.to_numpy())  # pyright: ignore[reportUnknownMemberType]
 
             if mom_ndim == 1:
                 data_values = convert.to_central_moments(
                     values, dtype=dtype, **convert_kws
                 )
             elif mom_ndim == 2:
                 data_values = convert.to_central_comoments(
@@ -2123,15 +2132,15 @@
 
         return new
 
     @classmethod
     @docfiller_inherit_abc()
     def from_raws(  # noqa: PLR0913
         cls,
-        raws: MyNDArray | xr.DataArray,
+        raws: NDArrayAny | xr.DataArray,
         *,
         mom_ndim: Mom_NDim | None = None,
         mom: Moments | None = None,
         axis: int | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
         convert_kws: Mapping[str, Any] | None = None,
```

### Comparing `cmomy-0.8.0/src/cmomy/_lib/convert.py` & `cmomy-0.9.0/src/cmomy/_lib/convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/src/cmomy/_lib/pushers.py` & `cmomy-0.9.0/src/cmomy/_lib/pushers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # mypy: disable-error-code="no-untyped-call,no-untyped-def"
 """low level routines to do pushing."""
+
 from __future__ import annotations
 
 from typing import Callable, NamedTuple
 
 from .utils import BINOMIAL_FACTOR, myjit
 
 # -- Scalars ---------------------------------------------------------------------------
```

### Comparing `cmomy-0.8.0/src/cmomy/_lib/resample.py` & `cmomy-0.9.0/src/cmomy/_lib/resample.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,25 @@
 from .utils import myjit
 
 # --- * Utilities ------------------------------------------------------------------------
 # put these here to avoid slow load up
 
 
 @myjit()
-def randsamp_freq_indices(indices, freq) -> None:
-    assert freq.shape == indices.shape
+def randsamp_indices_to_freq(indices, freq) -> None:
+    # allowed to pass in different number of samples than ndat.
     nrep, ndat = freq.shape
+
+    assert indices.shape[0] == nrep
+    assert indices.max() < ndat
+
+    nsamp = indices.shape[1]
+
     for r in range(nrep):
-        for d in range(ndat):
+        for d in range(nsamp):
             idx = indices[r, d]
             freq[r, idx] += 1
 
 
 # NOTE: this is all due to closures not being cache-able with numba
 # used to use the following
 #
```

### Comparing `cmomy-0.8.0/src/cmomy/_lib/utils.py` & `cmomy-0.9.0/src/cmomy/_lib/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..options import OPTIONS
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from numpy.typing import DTypeLike
 
-    from ..typing import F, MyNDArray
+    from ..typing import F, NDArrayAny
 
 
 def myjit(
     signature: str | list[str] | None = None,
     *,
     parallel: bool = False,
     inline: bool | None = None,
@@ -47,15 +47,15 @@
         return math.factorial(n) / (math.factorial(k) * math.factorial(n - k))
     if n == k:
         return 1.0
     # n < k
     return 0.0
 
 
-def factory_binomial(order: int, dtype: DTypeLike = np.float64) -> MyNDArray:
+def factory_binomial(order: int, dtype: DTypeLike = np.float64) -> NDArrayAny:
     """Create binomial coefs at given order."""
     out = np.zeros((order + 1, order + 1), dtype=dtype)
     for n in range(order + 1):
         for k in range(order + 1):
             out[n, k] = _binom(n, k)
 
     return out
```

### Comparing `cmomy-0.8.0/tests/_simple_cmom.py` & `cmomy-0.9.0/tests/_simple_cmom.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/conftest.py` & `cmomy-0.9.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import cmomy
 from cmomy import central, resample, xcentral
 
 from ._simple_cmom import get_cmom, get_comom
 
 if TYPE_CHECKING:
-    from cmomy.typing import Moments, MyNDArray
+    from cmomy.typing import Moments, NDArrayAny
 
 
 default_rng = cmomy.random.default_rng(0)
 
 
 @pytest.fixture(scope="session")
 def rng():
@@ -71,49 +71,49 @@
 
     @cached.prop
     def val_shape(self) -> tuple[int, ...]:
         val_shape = list(self.shape)
         val_shape.pop(self.axis)
         return tuple(val_shape)
 
-    def _get_data(self, style: str | None = None) -> MyNDArray:
+    def _get_data(self, style: str | None = None) -> NDArrayAny:
         if style is None or style == "total":
             return default_rng.random(self.shape)  # pyright: ignore[reportReturnType]
         if style == "broadcast":
             return default_rng.random(self.shape[self.axis])
         msg = "bad style"
         raise ValueError(msg)
 
     @cached.prop
-    def xdata(self) -> MyNDArray:
+    def xdata(self) -> NDArrayAny:
         return self._get_data()
 
     @cached.prop
-    def ydata(self) -> MyNDArray:
+    def ydata(self) -> NDArrayAny:
         return self._get_data(style=self.style)
 
     @cached.prop
-    def w(self) -> MyNDArray | None:
+    def w(self) -> NDArrayAny | None:
         if self.style is None:
             return None
         return self._get_data(style=self.style)
 
     @cached.prop
-    def x(self) -> MyNDArray | tuple[MyNDArray, MyNDArray]:
+    def x(self) -> NDArrayAny | tuple[NDArrayAny, NDArrayAny]:
         if self.cov:
             return (self.xdata, self.ydata)
         return self.xdata
 
     @cached.prop
-    def split_data(self) -> tuple[list[MyNDArray] | list[None], list[MyNDArray]]:
+    def split_data(self) -> tuple[list[NDArrayAny] | list[None], list[NDArrayAny]]:
         v = self.xdata.shape[self.axis] // self.nsplit
         splits = [v * i for i in range(1, self.nsplit)]
         X = np.split(self.xdata, splits, axis=self.axis)
 
-        W: list[MyNDArray] | list[None]
+        W: list[NDArrayAny] | list[None]
         if self.style == "total":
             W = np.split(self.w, splits, axis=self.axis)  # type: ignore[arg-type]
         elif self.style == "broadcast":
             W = np.split(self.w, splits)  # type: ignore[arg-type]
         else:
             W = cast("list[None]", [self.w for _ in X])
 
@@ -125,36 +125,36 @@
 
             # pack X, Y
             X = list(zip(X, Y))  # type: ignore[arg-type]
 
         return W, X  # pyright: ignore[reportReturnType]
 
     @property
-    def W(self) -> list[MyNDArray] | list[None]:
+    def W(self) -> list[NDArrayAny] | list[None]:
         return self.split_data[0]
 
     @property
-    def X(self) -> list[MyNDArray]:
+    def X(self) -> list[NDArrayAny]:
         return self.split_data[1]
 
     @cached.prop
-    def data_fix(self) -> MyNDArray:
+    def data_fix(self) -> NDArrayAny:
         if self.cov:
             return get_comom(  # type: ignore[no-any-return]
                 w=self.w,
                 x=self.x[0],
                 y=self.x[1],
                 moments=self.mom,
                 axis=self.axis,
                 broadcast=self.broadcast,
             )
         return get_cmom(w=self.w, x=self.x, moments=self.mom, axis=self.axis, last=True)  # type: ignore[no-any-return]
 
     @cached.prop
-    def data_test(self) -> MyNDArray:
+    def data_test(self) -> NDArrayAny:
         return central.central_moments(
             x=self.x,
             mom=self.mom,
             w=self.w,
             axis=self.axis,
             last=True,
             broadcast=self.broadcast,
@@ -172,30 +172,30 @@
             self.cls.from_vals(
                 x=xx, w=ww, axis=self.axis, mom=self.mom, broadcast=self.broadcast
             )
             for ww, xx in zip(self.W, self.X)
         ]
 
     # @property
-    # def values(self) -> MyNDArray:
+    # def values(self) -> NDArrayAny:
     #     return self.data_test
-    def to_values(self) -> MyNDArray:
+    def to_values(self) -> NDArrayAny:
         return self.data_test
 
     def unpack(self, *args) -> Any:
         out = tuple(getattr(self, x) for x in args)
         if len(out) == 1:
             out = out[0]
         return out
 
     def test_values(self, x, **kws) -> None:
         np.testing.assert_allclose(self.to_values(), x, **kws)
 
     @property
-    def raw(self) -> MyNDArray | None:
+    def raw(self) -> NDArrayAny | None:
         if self.style == "total":
             if not self.cov:
                 raw = np.array(
                     [
                         np.average(self.x**i, weights=self.w, axis=self.axis)  # type: ignore[operator]
                         for i in range(self.mom + 1)  # type: ignore[operator]
                     ]
@@ -216,64 +216,70 @@
 
                 raw[..., 0, 0] = self.w.sum(self.axis)  # type: ignore[union-attr]
 
         else:
             raw = None
         return raw
 
+    @property
+    def nrep(self) -> int:
+        return 10
+
+    @property
+    def ndat(self) -> int:
+        return self.xdata.shape[self.axis]
+
     @cached.prop
-    def indices(self) -> MyNDArray:
-        ndat = self.xdata.shape[self.axis]
-        nrep = 10
-        return default_rng.choice(ndat, (nrep, ndat), replace=True)
+    def indices(self) -> NDArrayAny:
+        return default_rng.choice(self.ndat, (self.nrep, self.ndat), replace=True)
 
     @cached.prop
-    def freq(self) -> MyNDArray:
-        return resample.randsamp_freq(indices=self.indices)
+    def freq(self) -> NDArrayAny:
+        return resample.randsamp_freq(indices=self.indices, ndat=self.ndat)
 
     @cached.prop
-    def xdata_resamp(self) -> MyNDArray:
+    def xdata_resamp(self) -> NDArrayAny:
         xdata = self.xdata
 
         if self.axis != 0:
             xdata = np.moveaxis(xdata, self.axis, 0)
 
         return np.take(xdata, self.indices, axis=0)
 
     @cached.prop
-    def ydata_resamp(self) -> MyNDArray:
+    def ydata_resamp(self) -> NDArrayAny:
         ydata = self.ydata
 
         if self.style == "broadcast":
             return np.take(ydata, self.indices, axis=0)
 
         if self.axis != 0:
             ydata = np.moveaxis(ydata, self.axis, 0)
         return np.take(ydata, self.indices, axis=0)
 
     @property
-    def x_resamp(self) -> MyNDArray | tuple[MyNDArray, MyNDArray]:
+    def x_resamp(self) -> NDArrayAny | tuple[NDArrayAny, NDArrayAny]:
         if self.cov:
             return (self.xdata_resamp, self.ydata_resamp)
         return self.xdata_resamp
 
     @cached.prop
-    def w_resamp(self) -> MyNDArray | None:
+    def w_resamp(self) -> NDArrayAny | None:
         w = self.w
 
         if self.style is None:
             return w
         if self.style == "broadcast":
             return np.take(w, self.indices, axis=0)  # type: ignore[arg-type]
         if self.axis != 0:
             w = np.moveaxis(w, self.axis, 0)  # type: ignore[arg-type]
         return np.take(w, self.indices, axis=0)  # type: ignore[arg-type]
 
     @cached.prop
-    def data_test_resamp(self) -> MyNDArray:
+    def data_test_resamp(self) -> NDArrayAny:
         return central.central_moments(
             x=self.x_resamp,
             mom=self.mom,
             w=self.w_resamp,
             axis=1,
             broadcast=self.broadcast,
         )
```

### Comparing `cmomy-0.8.0/tests/test_central.py` & `cmomy-0.9.0/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_central_2.py` & `cmomy-0.9.0/tests/test_central_2.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_convert.py` & `cmomy-0.9.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_random.py` & `cmomy-0.9.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_resample.py` & `cmomy-0.9.0/tests/test_resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import numpy as np
 import pytest
 
 import cmomy
 from cmomy import resample
 from cmomy.resample import (  # , xbootstrap_confidence_interval
     bootstrap_confidence_interval,
+    freq_to_indices,
 )
 
 
 @pytest.mark.parametrize("ndat", [50])
 def test_freq_indices(ndat, rng) -> None:
-    indices = rng.choice(10, (20, 10), replace=True)
+    indices = rng.choice(ndat, (20, ndat), replace=True)
 
     freq0 = resample.indices_to_freq(indices)
 
     freq1 = resample.randsamp_freq(indices=indices, ndat=ndat)
 
     np.testing.assert_allclose(freq0, freq1)
 
@@ -29,16 +30,24 @@
 
     freq1 = resample.randsamp_freq(nrep=10, ndat=ndat, rng=np.random.default_rng(456))
     assert not np.all(freq0 == freq1)
 
     freq1 = resample.randsamp_freq(nrep=10, ndat=ndat, rng=np.random.default_rng(123))
     np.testing.assert_allclose(freq0, freq1)
 
+    # test bad freq
+    freq = np.array([[5, 0], [0, 4]])
+    with pytest.raises(ValueError, match="Inconsistent number of samples .*"):
+        freq_to_indices(freq)
 
-@pytest.mark.parametrize("parallel", [True, False])
+
+parallel_parametrize = pytest.mark.parametrize("parallel", [True, False])
+
+
+@parallel_parametrize
 @pytest.mark.parametrize("mom", [2, (2, 2)])
 def test_resample_vec(parallel, mom):
     rng = cmomy.random.default_rng()
 
     x = rng.random((100, 10))
     xx = x[..., None]
 
@@ -73,35 +82,48 @@
         np.testing.assert_allclose(freq, cmomy.resample.indices_to_freq(idx))
 
 
 def test_validate_resample_array() -> None:
     np.zeros((2, 3, 4))
 
     with pytest.raises(ValueError):
-        cmomy.resample._validate_resample_array(np.zeros((2, 3, 4)), nrep=2, ndat=3)
+        cmomy.resample._validate_resample_array(
+            np.zeros((2, 3, 4)), nrep=2, ndat=3, is_freq=True
+        )
 
     with pytest.raises(ValueError):
-        cmomy.resample._validate_resample_array(np.zeros((2, 3)), nrep=3, ndat=3)
+        cmomy.resample._validate_resample_array(
+            np.zeros((2, 3)), nrep=3, ndat=3, is_freq=True
+        )
 
     with pytest.raises(ValueError):
-        cmomy.resample._validate_resample_array(np.zeros((2, 3)), nrep=2, ndat=None)
+        cmomy.resample._validate_resample_array(
+            np.zeros((2, 3)), nrep=2, ndat=5, is_freq=True
+        )
+
+    # indices
+    _ = cmomy.resample._validate_resample_array(
+        np.zeros((2, 3)), nrep=2, ndat=5, is_freq=False
+    )
 
     with pytest.raises(ValueError):
-        cmomy.resample._validate_resample_array(np.zeros((2, 3)), nrep=2, ndat=5)
+        cmomy.resample._validate_resample_array(
+            np.zeros((2, 3)) + 10, nrep=2, ndat=5, is_freq=False
+        )
 
 
 def test_randsamp_freq() -> None:
     f0 = cmomy.resample.randsamp_freq(nrep=10, ndat=5, rng=np.random.default_rng(0))
 
     f1 = cmomy.resample.random_freq(nrep=10, ndat=5, rng=np.random.default_rng(0))
 
     np.testing.assert_allclose(f0, f1)
 
     with pytest.raises(ValueError):
-        cmomy.resample.randsamp_freq()
+        cmomy.resample.randsamp_freq(ndat=10)
 
 
 def test_resample_resample_data(rng) -> None:
     x = rng.random((100, 10, 3))
 
     c = cmomy.CentralMoments.from_vals(x, mom=3)
 
@@ -160,15 +182,15 @@
 
     c2 = cmomy.CentralMoments.from_resample_vals((x, x), freq=freq, mom=(3, 3))
 
     np.testing.assert_allclose(c2.data[..., :, 0], c.data)
 
 
 @pytest.mark.slow()
-@pytest.mark.parametrize("parallel", [True, False])
+@parallel_parametrize
 def test_resample_vals(other, parallel) -> None:
     # test basic resampling
     if other.style == "total":
         datar = resample.resample_vals(
             x=other.x,
             mom=other.mom,
             freq=other.freq,
@@ -179,15 +201,15 @@
             parallel=parallel,
         )
 
         np.testing.assert_allclose(datar, other.data_test_resamp)
 
 
 @pytest.mark.slow()
-@pytest.mark.parametrize("parallel", [True, False])
+@parallel_parametrize
 def test_stats_resample_vals(other, parallel) -> None:
     if other.style == "total":
         t = other.cls.from_resample_vals(
             x=other.x,
             w=other.w,
             mom=other.mom,
             freq=other.freq,
@@ -208,38 +230,38 @@
             broadcast=other.broadcast,
             parallel=parallel,
         )
         np.testing.assert_allclose(t.data, other.data_test_resamp)
 
 
 @pytest.mark.slow()
-@pytest.mark.parametrize("parallel", [True, False])
+@parallel_parametrize
 def test_resample_data(other, parallel, rng) -> None:
     nrep = 10
 
     if len(other.val_shape) > 0:
         for axis in range(other.s.val_ndim):
             data = other.data_test
 
             ndat = data.shape[axis]
 
             idx = rng.choice(ndat, (nrep, ndat), replace=True)
-            freq = resample.randsamp_freq(indices=idx)
+            freq = resample.randsamp_freq(indices=idx, ndat=ndat)
 
             if axis != 0:
                 data = np.rollaxis(data, axis, 0)
             data = np.take(data, idx, axis=0)
             data_ref = other.cls.from_datas(data, mom_ndim=other.mom_ndim, axis=1)
 
             t = other.s.resample_and_reduce(freq=freq, axis=axis, parallel=parallel)
             np.testing.assert_allclose(data_ref, t.data)
 
 
 @pytest.mark.slow()
-@pytest.mark.parametrize("parallel", [True, False])
+@parallel_parametrize
 def test_resample_against_vals(other, parallel, rng) -> None:
     nrep = 10
 
     if len(other.val_shape) > 0:
         s = other.s
 
         for axis in range(s.val_ndim):
@@ -298,7 +320,34 @@
     stats_val = x.mean(axis=axis)
     val = stats_val
     low = 2 * stats_val - np.percentile(a=x, q=q_low, axis=axis)
     high = 2 * stats_val - np.percentile(a=x, q=q_high, axis=axis)
 
     expected = np.array([val, low, high])
     np.testing.assert_allclose(test, expected)
+
+
+# * Arbitrary number of samples in resample.
+
+
+@parallel_parametrize
+def test_resample_nsamp(other, parallel) -> None:
+    nrep = 10
+
+    if len(other.val_shape) > 0:
+        s = other.s
+
+        for axis in range(s.val_ndim):
+            ndat = s.val_shape[axis]
+
+            for nsamp in [ndat + 1, ndat - 1]:
+                indices = cmomy.resample.random_indices(
+                    nrep=nrep, ndat=ndat, nsamp=nsamp
+                )
+
+                t0 = s.resample_and_reduce(
+                    indices=indices, axis=axis, parallel=parallel
+                )
+
+                t1 = s.resample(indices, axis=axis).reduce(1)
+
+                np.testing.assert_allclose(t0.to_values(), t1.to_values())
```

### Comparing `cmomy-0.8.0/tests/test_stability.py` & `cmomy-0.9.0/tests/test_stability.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # mypy: disable-error-code="no-untyped-def, no-untyped-call"
 """Simple test for numerical stability"""
+
 import numpy as np
 import pytest
 
 import cmomy
 from cmomy._lib.utils import factory_binomial
```

### Comparing `cmomy-0.8.0/tests/test_utils.py` & `cmomy-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_verify.py` & `cmomy-0.9.0/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_xcentral.py` & `cmomy-0.9.0/tests/test_xcentral.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/tests/test_xcentral_constructors.py` & `cmomy-0.9.0/tests/test_xcentral_constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # mypy: disable-error-code="no-untyped-def, no-untyped-call"
 """Some simple tests for factory methods of xCentral"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
 import numpy as np
 import pytest
 import xarray as xr
```

### Comparing `cmomy-0.8.0/tools/clean_kernelspec.py` & `cmomy-0.9.0/tools/clean_kernelspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This script must be run from the environment with the notebook server.
 For example, if you have a conda environment `notebook` with your
 jupyter server, run the following:
 
 $ conda run -n notebook python path/to/clean_kernelspec.py
 """
+
 from __future__ import annotations
 
 import json
 import logging
 from pathlib import Path
 from subprocess import CalledProcessError
```

### Comparing `cmomy-0.8.0/tools/common_utils.py` & `cmomy-0.9.0/tools/common_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for tools."""
+
 from __future__ import annotations
 
 
 def get_conda_environment_map(simplify: bool = True) -> dict[str, str]:
     """Construct mapping from environment env_name to path"""
     import subprocess
     from pathlib import Path
```

### Comparing `cmomy-0.8.0/tools/create_pythons.py` & `cmomy-0.9.0/tools/create_pythons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Script to create pythons for use with virtualenvs"""
+
 from __future__ import annotations
 
 import sys
 from functools import lru_cache
 
 if sys.version_info < (3, 9):
     msg = "Requires python >= 3.9"
```

### Comparing `cmomy-0.8.0/tools/dataclass_parser.py` & `cmomy-0.9.0/tools/dataclass_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     other: RUN_TYPE = add_option(help="hello")
     version: str | None = None
     lock: bool = False
     no_cov: bool = False
 
 """
+
 from __future__ import annotations
 
 import sys
 from argparse import ArgumentParser
 from dataclasses import (
     dataclass,
     field,
```

### Comparing `cmomy-0.8.0/tools/noxtools.py` & `cmomy-0.9.0/tools/noxtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Utilities to work with nox"""
+
 from __future__ import annotations
 
+import functools
 import os
 import shlex
 from contextlib import contextmanager
 from functools import cached_property, reduce
 from pathlib import Path
 from typing import TYPE_CHECKING, cast
 
 # fmt: off
 from nox.sessions import SessionRunner
 
+DISALLOW_WHICH: list[str] = []
+
 # * Override SessionRunner._create_venv ------------------------------------------------
 
 _create_venv_super = SessionRunner._create_venv  # pyright: ignore[reportPrivateUsage]
 
+
 def override_sessionrunner_create_venv(self: SessionRunner) -> None:
     """Override SessionRunner._create_venv"""
     if callable(self.func.venv_backend):
         # if passed a callable backend, always use just that
         logger.info("Using custom callable venv_backend")
 
         self.venv = self.func.venv_backend(self)
@@ -29,14 +34,15 @@
         #     runner=self,
         # )
         return None
 
     logger.info("Using nox venv_backend")
     return _create_venv_super(self)
 
+
 SessionRunner._create_venv = override_sessionrunner_create_venv  # type: ignore[method-assign] # pyright: ignore[reportPrivateUsage]
 # fmt: on
 
 import operator
 
 from nox.logger import logger
 from nox.virtualenv import CondaEnv, VirtualEnv
@@ -79,37 +85,52 @@
             conda_cmd=backend,
         )
 
     return passthrough_venv_backend
 
 
 def factory_virtualenv_backend(
-    backend: Literal["virtualenv", "venv"] = "virtualenv",
+    backend: Literal["virtualenv", "venv", "uv"] = "virtualenv",
     location: str | None = None,
 ) -> Callable[..., CondaEnv | VirtualEnv]:
     """Factory virtualenv backend."""
 
     def passthrough_venv_backend(
         runner: SessionRunner,
     ) -> VirtualEnv:
         venv = VirtualEnv(
             location=location or runner.envdir,
             interpreter=runner.func.python,  # type: ignore[arg-type]
             reuse_existing=runner.func.reuse_venv
             or runner.global_config.reuse_existing_virtualenvs,
             venv_params=runner.func.venv_params,
-            venv=(backend == "venv"),
+            venv_backend=backend,
         )
         venv.create()
         return venv
 
     return passthrough_venv_backend
 
 
 # * Top level installation functions ---------------------------------------------------
+@functools.cache
+def cached_which(cmd: str) -> str | None:
+    """
+    Cached lookup of uv path.
+
+    Returns path or None if not installed.
+    """
+    if cmd in DISALLOW_WHICH:
+        return None
+
+    from shutil import which
+
+    return which(cmd)
+
+
 def py_prefix(python_version: Any) -> str:
     """
     Get python prefix.
 
     `python="3.8` -> "py38"
     """
     if isinstance(python_version, str):
@@ -269,14 +290,15 @@
         Can either be a full path or a envname (for example,
         "test" will get resolved to ./requirements/test.txt)
     constraints : str or list of str
         pip constraint file(s) (pip install -c ...)
     config_path :
         Where to save env config for future comparison.  Defaults to
         `session.virtualenv.location / "tmp" / "env.json"`.
+
     """
 
     def __init__(
         self,
         session: Session,
         *,
         update: bool = False,
@@ -577,14 +599,29 @@
             out = out.log_session()
 
         if save_config:
             out = out.save_config()
 
         return out
 
+    def uv_install(self, *args: str, **kwargs: Any) -> None:
+        """Run uv pip install if available"""
+        if uv_path := cached_which("uv"):
+            self.session.run_always(
+                uv_path,
+                "pip",
+                "install",
+                f"--python={self.python_full_path}",
+                *args,
+                **kwargs,
+                external=True,
+            )
+        else:
+            self.session.install(*args, **kwargs)
+
     def pip_install_package(
         self,
         *args: Any,
         update: bool = False,
         opts: str | list[str] | None = None,
         **kwargs: Any,
     ) -> Self:
@@ -597,15 +634,15 @@
 
             if update:
                 command.append("--upgrade")
 
             if opts:
                 command.extend(combine_list_str(opts))
 
-            self.session.install(*command, *args, **kwargs)
+            self.uv_install(*command, *args, **kwargs)
 
         return self
 
     def pip_install_deps(
         self,
         *args: Any,
         update: bool = False,
@@ -619,27 +656,38 @@
         elif self.changed or (update := update or self.update):
             # # Playing with using pip-sync.
             # # Not sure its worth it?
             if self.lock:
                 # Using pip-compile-{python_version} session.
                 if not isinstance(self.session.python, str):
                     raise TypeError
-                self.session.run_always(
-                    "nox",
-                    "-s",
-                    f"pip-compile-{self.session.python}",
-                    "--",
-                    "++pip-compile-run-internal",
-                    "pip-sync",
-                    "--python-executable",
-                    self.python_full_path,
-                    *map(str, self.requirements),
-                    silent=True,
-                    external=True,
-                )
+
+                if uv_path := cached_which("uv"):
+                    self.session.run_always(
+                        uv_path,
+                        "pip",
+                        "sync",
+                        f"--python={self.python_full_path}",
+                        *map(str, self.requirements),
+                        external=True,
+                    )
+                else:
+                    self.session.run_always(
+                        "nox",
+                        "-s",
+                        f"pip-compile-{self.session.python}",
+                        "--",
+                        "++pip-compile-run-internal",
+                        "pip-sync",
+                        "--python-executable",
+                        self.python_full_path,
+                        *map(str, self.requirements),
+                        silent=True,
+                        external=True,
+                    )
 
                 # Using central pip-sync
                 # The above fixes an fixes issue with using pip-sync on already
                 # created environments with dependencies like
                 # "thing; python_version < '3.9'".  For some reason
                 # the below will work fine on creation, but will not work
                 # correctly (python_version is not that of
@@ -663,15 +711,15 @@
 
                 if install_args:
                     if update:
                         install_args = ["--upgrade", *install_args]
 
                     if opts:
                         install_args.extend(combine_list_str(opts))
-                    self.session.install(*install_args, *args, **kwargs)
+                    self.uv_install(*install_args, *args, **kwargs)
 
         return self
 
     def create_conda_env(self, update: bool = False) -> Self:
         """Create conda environment."""
         venv = self.session.virtualenv
         if not isinstance(venv, CondaEnv):
@@ -694,15 +742,15 @@
 
         # create environment
         self.session.log(
             f"{cmd.capitalize()} conda environment in {venv.location_name}",
         )
 
         if cmd != "reuse":
-            extra_params = self._session_runner.func.venv_params or []
+            extra_params: list[str] = self._session_runner.func.venv_params or []
 
             if self.lock and not self.is_micromamba():
                 # use conda-lock
                 if self.conda_cmd == "conda":
                     extra_params.append("--no-mamba")
                 else:
                     extra_params.append("--mamba")
@@ -824,14 +872,15 @@
 
         Parameters
         ----------
         envname :
             Base name for file.  For example, passing
             envname = "dev" will convert to
             `requirements/py{py}-dev.yaml` for `filename`
+
         """
         if envname is not None and conda_yaml is None:
             if not isinstance(session.python, str):
                 msg = "session.python must be a string"
                 raise TypeError(msg)
             lock, conda_yaml = infer_requirement_path_with_fallback(
                 envname,
@@ -993,17 +1042,18 @@
 
 def _get_zipfile_hash(path: str | Path) -> str:
     import hashlib
     from zipfile import ZipFile
 
     md5 = hashlib.md5()
 
-    with ZipFile(path, "r") as f:
-        for thing in f.infolist():
-            md5 = hashlib.md5(f.read(thing))
+    with ZipFile(path, "r") as zipfile:
+        for item in sorted(zipfile.infolist(), key=lambda x: x.filename):
+            md5.update(item.filename.encode())
+            md5.update(zipfile.read(item))
 
     return md5.hexdigest()
 
 
 def get_package_hash(package: str) -> list[str]:
     """Get hash for wheel of package."""
     import re
@@ -1011,14 +1061,17 @@
     out: list[str] = []
 
     for x in shlex.split(package):
         out.append(x)
 
         # remove possible extras
         x_clean = re.sub(r"\[.*?\]$", "", x)
+        # remove possible thing@path -> path
+        x_clean = re.sub(r"^.*?\@", "", x_clean)
+
         if Path(x_clean).is_file():
             if x_clean.endswith(".whl"):
                 out.append(_get_zipfile_hash(x_clean))
             else:
                 out.append(_get_file_hash(x_clean))
 
     return out
@@ -1035,14 +1088,15 @@
     Context manager to look for changes in dependencies.
 
     Yields
     ------
     changed: bool
 
     If exit normally, write hashes to hash_path file
+
     """
     try:
         changed, hashes, hash_path = check_hash_path_for_change(
             *deps,
             target_path=target_path,
             hash_path=hash_path,
         )
```

### Comparing `cmomy-0.8.0/tools/projectconfig.py` & `cmomy-0.9.0/tools/projectconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Methods to work with config file (for personal setup) of nox and other project tools.
 
 Right now, this is only for user specific nox config.  But leaving open it could be used
 for other things in the future.
 """
+
 from __future__ import annotations
 
 import configparser
 import json
 import os
 from copy import deepcopy
 from pathlib import Path
```

### Comparing `cmomy-0.8.0/.gitignore` & `cmomy-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/LICENSE` & `cmomy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmomy-0.8.0/pyproject.toml` & `cmomy-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,64 +40,71 @@
     "numba >= 0.50",
     "numpy >= 1.21",
     "typing-extensions;python_version<'3.11'",
     "xarray >= 0.16",
 ]
 [project.optional-dependencies]
 dev = [
-    "cmomy[nbval]",
-    "cmomy[test]",
-    "cmomy[typing-extras]",
-    "cmomy[dev-extras]",
+    "cmomy[dev-extras,test,typing,pipxrun,nbval]",
 ]
 dev-complete = [
-    "cmomy[dev]",
-    "cmomy[tools]",
+    "cmomy[dev,tools]",
 ]
 dev-extras = [
     "ipykernel",
     "ipython",
-    "nox",
+    "nbclient >= 0.10.0",
+    "nox >= 2024.3.2",
     "pytest-accept",
 ]
 docs = [
     "autodocsumm",
-    "ghp-import",
-    "ipython",
     "myst-nb",
     "pyenchant",
     "sphinx >= 5.3.0",
     "sphinx-autobuild",
+    "sphinx-autodoc-typehints",
     "sphinx-book-theme",
     "sphinx-copybutton",
     "sphinxcontrib-spelling",
 ]
+mypy = [
+    "mypy >= 1.9.0",
+]
 nbval = [
     "nbval",
 ]
+pipxrun = [
+    # Anything needed to run tools/pipxrun.py
+    "packaging",
+]
+pipxrun-tools = [
+    # these used solely for specking tools to be used with tools/pipxrun.py
+    "cmomy[mypy]",
+    "conda-lock >= 2.5.5",
+    "grayskull >= 2.5.3",
+    "nbqa >= 1.8.4",
+    "pyright >= 1.1.358",
+    "twine >= 5.0.0",
+]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-sugar",
     "pytest-xdist",
 ]
 tools = [
-    "nbqa",
+    "pipx",
     "pre-commit",
-    "pyright",
     "scriv",
 ]
 typing = [
-    "cmomy[typing-extras]",
-    "pytest",
-]
-typing-extras = [
-    "mypy >= 1.5.1",
+    "cmomy[pipxrun]",
     "pandas-stubs",
-    "pytype; python_version < '3.11'",
+    "pytest",
 ]
 [project.urls]
 Documentation = "https://pages.nist.gov/cmomy/"
 Homepage = "https://github.com/usnistgov/cmomy"
 
 [tool.hatch.version]
 source = "vcs"
@@ -131,15 +138,15 @@
 ]
 unsafe-fixes = true
 
 [tool.ruff.lint]
 preview = true
 select = ["ALL"]
 # fixable = ["ALL"]
-# unfixable = []
+unfixable = ["T"]
 ignore = [
     "CPY",       # - Don't require copyright
     "ERA",       # - eradicate (want to keep some stuff)
     "FBT",       # - bools are ok
     # * Annotations
     "ANN101",    # - Leads to issues with methods and self
     "ANN102",    # - Leads to issues with classmethods and cls
@@ -193,26 +200,26 @@
 max-args = 15
 max-positional-args = 15
 max-public-methods = 30
 
 [tool.ruff.lint.per-file-ignores]
 "docs/conf.py" = ["INP001"]
 "noxfile.py" = ["RUF009"]
-"tools/*.py" = ["S", "A", "SLF001"]
+"tools/*.py" = ["S", "A", "SLF001", "D102"]
 "tests/*.py" = ["D", "S101"]
 "**/*.ipynb" = ["D100", "B018", "INP001"]
 
 [tool.ruff.lint.extend-per-file-ignores]
 # Project specific ignores (avoid changing per-file-ignores directly)
 "tests/*.py" = ["ANN", "N802", "N806", "PT011", "PLC2701", "PLR2004", "SLF001"]
 "src/cmomy/_{formatting,testing}.py" = ["ANN"]
 "src/cmomy/_formatting.py" = ["SLF001"]
 "src/cmomy/_lib/*.py" = ["PLR2004", "PLR0914", "S101", "ANN", "N803"]
 "src/cmomy/_testing.py" = ["S101"]
-"**/*.ipynb" = ["ANN", "T201", "D103", "PLR2004", "PD013"]
+"**/*.ipynb" = ["ANN", "T201", "D103", "PLR2004", "PD013", "E305", "E302"]
 "src/**/*.py" = ["TD003", "FIX002", "PLR2004", "D102"]
 "src/cmomy/abstract_central.py" = ["PLR2004"]
 "src/cmomy/central.py" = ["PLR2004", "D102"]
 "src/cmomy/_lib/convert.py" = ["PLR1702"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["cmomy"]
@@ -339,14 +346,19 @@
 
 [tool.pyproject2conda.envs.build]
 extras = "build-system.requires"
 reqs = ["build"]
 base = false
 style = "requirements"
 
+[tool.pyproject2conda.envs.pipxrun-tools]
+extras = "pipxrun-tools"
+base = false
+style = "requirements"
+
 [tool.pyproject2conda.envs.test-extras]
 extras = ["test"]
 base = false
 
 [tool.pyproject2conda.envs.test-notebook]
 extras = ["test", "nbval"]
 
@@ -375,8 +387,8 @@
 
 [tool.cruft]
 
 [tool.typos.default.extend-words]
 datas = "datas"
 
 [tool.typos.default.extend-identifiers]
-MyNDArray = "MyNDArray"
+NDArrayAny = "NDArrayAny"
```

### Comparing `cmomy-0.8.0/PKG-INFO` & `cmomy-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Central (co)moment calculation/manipulation
 Project-URL: Documentation, https://pages.nist.gov/cmomy/
 Project-URL: Homepage, https://github.com/usnistgov/cmomy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 License-File: LICENSE
 Keywords: cmomy
@@ -24,56 +24,59 @@
 Requires-Dist: lazy-loader
 Requires-Dist: module-utilities>=0.6
 Requires-Dist: numba>=0.50
 Requires-Dist: numpy>=1.21
 Requires-Dist: typing-extensions; python_version < '3.11'
 Requires-Dist: xarray>=0.16
 Provides-Extra: dev
-Requires-Dist: cmomy[dev-extras]; extra == 'dev'
-Requires-Dist: cmomy[nbval]; extra == 'dev'
-Requires-Dist: cmomy[test]; extra == 'dev'
-Requires-Dist: cmomy[typing-extras]; extra == 'dev'
+Requires-Dist: cmomy[dev-extras,nbval,pipxrun,test,typing]; extra == 'dev'
 Provides-Extra: dev-complete
-Requires-Dist: cmomy[dev]; extra == 'dev-complete'
-Requires-Dist: cmomy[tools]; extra == 'dev-complete'
+Requires-Dist: cmomy[dev,tools]; extra == 'dev-complete'
 Provides-Extra: dev-extras
 Requires-Dist: ipykernel; extra == 'dev-extras'
 Requires-Dist: ipython; extra == 'dev-extras'
-Requires-Dist: nox; extra == 'dev-extras'
+Requires-Dist: nbclient>=0.10.0; extra == 'dev-extras'
+Requires-Dist: nox>=2024.3.2; extra == 'dev-extras'
 Requires-Dist: pytest-accept; extra == 'dev-extras'
 Provides-Extra: docs
 Requires-Dist: autodocsumm; extra == 'docs'
-Requires-Dist: ghp-import; extra == 'docs'
-Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: pyenchant; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=5.3.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
+Provides-Extra: mypy
+Requires-Dist: mypy>=1.9.0; extra == 'mypy'
 Provides-Extra: nbval
 Requires-Dist: nbval; extra == 'nbval'
+Provides-Extra: pipxrun
+Requires-Dist: packaging; extra == 'pipxrun'
+Provides-Extra: pipxrun-tools
+Requires-Dist: cmomy[mypy]; extra == 'pipxrun-tools'
+Requires-Dist: conda-lock>=2.5.5; extra == 'pipxrun-tools'
+Requires-Dist: grayskull>=2.5.3; extra == 'pipxrun-tools'
+Requires-Dist: nbqa>=1.8.4; extra == 'pipxrun-tools'
+Requires-Dist: pyright>=1.1.358; extra == 'pipxrun-tools'
+Requires-Dist: twine>=5.0.0; extra == 'pipxrun-tools'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-sugar; extra == 'test'
 Requires-Dist: pytest-xdist; extra == 'test'
 Provides-Extra: tools
-Requires-Dist: nbqa; extra == 'tools'
+Requires-Dist: pipx; extra == 'tools'
 Requires-Dist: pre-commit; extra == 'tools'
-Requires-Dist: pyright; extra == 'tools'
 Requires-Dist: scriv; extra == 'tools'
 Provides-Extra: typing
-Requires-Dist: cmomy[typing-extras]; extra == 'typing'
+Requires-Dist: cmomy[pipxrun]; extra == 'typing'
+Requires-Dist: pandas-stubs; extra == 'typing'
 Requires-Dist: pytest; extra == 'typing'
-Provides-Extra: typing-extras
-Requires-Dist: mypy>=1.5.1; extra == 'typing-extras'
-Requires-Dist: pandas-stubs; extra == 'typing-extras'
-Requires-Dist: pytype; (python_version < '3.11') and extra == 'typing-extras'
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -241,14 +244,39 @@
 
 <!-- prettier-ignore-end -->
 
 <!-- markdownlint-enable MD013 -->
 
 <!-- scriv-insert-here -->
 
+## v0.9.0 — 2024-04-10
+
+### Changed
+
+- Can now resample with an arbitrary number of samples. Previously, it was
+  assumed that resampling should be done with a shape `(nrep, ndat)`, where
+  `nrep` is the number of replicates and `ndat` is the shape of the data along
+  the resampled axis. Now you can pass sample with shape `(nrep, nsamp)` where
+  `nsamp` is the specified number of samples in a replicate (defaulting to
+  `ndat`). This allows users to do things like jacknife resampling, etc, with
+  `resample_and_reduce` methods.
+- Preliminary support for using type hints in generated documentation. The
+  standard sphinx autodoc support doesn't quite work for `cmomy`, as it requires
+  type hints to be accessible at run time, and not in `TYPE_CHECKING` blocks.
+  Instead, we use
+  [`sphinx_autodoc_type`](https://github.com/tox-dev/sphinx-autodoc-typehints).
+  This has the downside of expanding type aliases, but handles (most things)
+  being in `TYPE_CHECKING` blocks. Over time, we'll replace some of the explicit
+  parameter type documentation with those from type hints.
+- Fixed creation of templates in reduction routines of `xCentralMoments`.
+  Previously, we build the template for the result using something like
+  `da.isel(dim=0)`. This kept scalar coordinates of `da` with `dim`. Now we use
+  `da.isel(dim=0, drop=True)` to drop these.
+- Updated dependencies.
+
 ## v0.8.0 — 2024-02-20
 
 ### Added
 
 - Added `to_values` method to access underlying array data. This should be
   preferred to `.values` attribute.
 - Added `to_numpy` method to access underlying `numpy.ndarray`.
```

