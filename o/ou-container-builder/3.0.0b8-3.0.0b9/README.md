# Comparing `tmp/ou_container_builder-3.0.0b8.tar.gz` & `tmp/ou_container_builder-3.0.0b9.tar.gz`

## Comparing `ou_container_builder-3.0.0b8.tar` & `ou_container_builder-3.0.0b9.tar`

### file list

```diff
@@ -1,130 +1,175 @@
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/.gitlab-ci.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/.readthedocs.yml
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/CHANGELOG.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/Dockerfile
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/prepare_release.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tox.ini
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/Makefile
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/building.rst
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/conf.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/index.rst
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/installation.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/make.bat
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/paths.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/weights.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/_static/.gitkeep
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/builder.rst
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/index.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/main.rst
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/packs.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/settings.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/utils.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/base.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/content.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/env.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/hacks.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/jupyter_server.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/packages.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/scripts.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/services.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/startup.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/core/web_apps.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/packs/code_server.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/packs/jupyterlab.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/packs/mariadb.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/packs/nbclassic.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/api/packs/tutorial_server.rst
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/content.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/environment.rst
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/flags.rst
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/hacks.rst
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/image.rst
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/index.rst
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/jupyter_server_config.rst
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/module.rst
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/packages.rst
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/packs.rst
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/scripts.rst
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/server.rst
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/services.rst
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/sources.rst
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/configuration/web_apps.rst
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/packs/code-server.rst
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/packs/index.rst
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/packs/jupyterlab.rst
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/packs/mariadb.rst
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/packs/nbclassic.rst
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/docs/packs/tutorial_server.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/__about__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/__main__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/settings.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/state.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/util.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/cli/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/cli/base.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/cli/build.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/cli/clean.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/cli/generate.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/cli/version.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/apt.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/args.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/base.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/content.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/environment.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/python.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/rust.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/scripts.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/services.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/sources.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/user.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/webapp.py
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/server/__init__.py
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/core/server/startup.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/ipykernel.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/jupyterlab.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/notebook.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/code_server/__init__.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/code_server/vscode.svg
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/__init__.py
--rw-r--r--   0        0        0   177470 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/desktop.jpg
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/xfce4-desktop.xml
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/xfwm4.xml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/cli_tests/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/cli_tests/conftest.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/cli_tests/test_build.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/cli_tests/test_generate_and_clean.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/cli_tests/test_nocommand.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/cli_tests/test_version.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/.gitignore
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/demo-tests.sh
--rwxr-xr-x   0        0        0      194 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/run-all.sh
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/code_server/ContainerConfig.yaml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/jupyterlab/v3/ContainerConfig.yaml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/jupyterlab/v4/ContainerConfig.yaml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/demos/openrefine/ContainerConfig.yaml
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/test_state.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/test_util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_args_settings.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_content_settings.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_environment_settings.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_image_settings.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_module_settings.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_output_blocks.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_packages_settings.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_server_settings.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_sources_settings.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_webapps_settings.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/util.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/.gitignore
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/README.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/.gitlab-ci.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/.readthedocs.yml
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/CHANGELOG.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/Dockerfile
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/prepare_release.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tox.ini
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/_config.yml
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/_toc.yml
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/commands.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/index.md
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/installation.md
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/references.bib
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/todo.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/_static/favicon.svg
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/_static/logo-dark.svg
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/_static/logo-light.svg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/index.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.__about__.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.__main__.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.cli.base.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.cli.build.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.cli.clean.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.cli.generate.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.cli.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.cli.version.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.apt.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.args.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.base.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.content.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.environment.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.python.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.rust.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.scripts.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.server.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.services.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.sources.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.user.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.core.webapp.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.packs.code_server.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.packs.ipykernel.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.packs.jupyterlab.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.packs.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.packs.notebook.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.packs.xfce4.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.settings.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.state.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/api/ou_container_builder.util.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/configuration/index.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs/packs/index.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/Makefile
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/building.rst
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/conf.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/index.rst
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/installation.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/make.bat
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/paths.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/weights.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/_static/.gitkeep
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/builder.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/index.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/main.rst
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/packs.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/settings.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/utils.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/base.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/content.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/env.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/hacks.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/jupyter_server.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/packages.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/scripts.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/services.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/startup.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/core/web_apps.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/packs/code_server.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/packs/jupyterlab.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/packs/mariadb.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/packs/nbclassic.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/api/packs/tutorial_server.rst
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/content.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/environment.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/flags.rst
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/hacks.rst
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/image.rst
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/index.rst
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/jupyter_server_config.rst
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/module.rst
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/packages.rst
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/packs.rst
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/scripts.rst
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/server.rst
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/services.rst
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/sources.rst
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/configuration/web_apps.rst
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/packs/code-server.rst
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/packs/index.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/packs/jupyterlab.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/packs/mariadb.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/packs/nbclassic.rst
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/docs-old/packs/tutorial_server.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/__about__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/__main__.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/settings.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/state.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/util.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/cli/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/cli/base.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/cli/build.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/cli/clean.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/cli/generate.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/cli/version.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/apt.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/args.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/base.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/content.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/environment.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/python.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/rust.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/scripts.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/services.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/sources.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/user.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/webapp.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/server/__init__.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/core/server/startup.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/ipykernel.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/irkernel.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/jupyterlab.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/notebook.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/code_server/__init__.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/code_server/vscode.svg
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/__init__.py
+-rw-r--r--   0        0        0   177470 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/desktop.jpg
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/xfce4-desktop.xml
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/xfwm4.xml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/cli_tests/__init__.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/cli_tests/conftest.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/cli_tests/test_build.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/cli_tests/test_generate_and_clean.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/cli_tests/test_nocommand.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/cli_tests/test_version.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/.gitignore
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/demo-tests.sh
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/run-all.sh
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/code_server/ContainerConfig.yaml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/jupyterlab/v4/ContainerConfig.yaml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/demos/openrefine/ContainerConfig.yaml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/test_state.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/test_util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_args_settings.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_content_settings.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_environment_settings.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_image_settings.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_module_settings.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_output_blocks.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_packages_settings.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_server_settings.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_sources_settings.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_webapps_settings.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/util.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/.gitignore
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/README.md
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 ou_container_builder-3.0.0b9/PKG-INFO
```

### Comparing `ou_container_builder-3.0.0b8/.gitlab-ci.yml` & `ou_container_builder-3.0.0b9/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,31 @@
     - hatch build
   artifacts:
     paths:
       - dist
     expire_in: 300 seconds
   rules:
     - if: $CI_PIPELINE_SOURCE != 'schedule'
+  interruptible: true
+
+build-docs:
+  image: python:3.10
+  stage: build
+  script:
+    - pip install hatch
+    - hatch run docs --all
+    - cd docs/_build
+    - tar -jcf docs.tar.bz2 html
+  artifacts:
+    paths:
+      - docs/_build
+    expire_in: 300 seconds
+  rules:
+    - if: $CI_PIPELINE_SOURCE != 'schedule'
+  interruptible: true
 
 demo-tests:
   image: docker:latest
   stage: test
   services:
     - docker:dind
   before_script:
@@ -52,14 +69,15 @@
           - openrefine
   dependencies:
     - build-package
   needs:
     - build-package
   rules:
     - if: $CI_PIPELINE_SOURCE == "merge_request_event"
+  interruptible: true
 
 tests:
   image: python:${PYTHON_VERSION}
   stage: test
   script:
     - pip install hatch
     - hatch run cov-auto
@@ -68,22 +86,33 @@
       - PYTHON_VERSION: ["3.10", "3.11"]
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
   coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
+  interruptible: true
+
+code-style:
+  image: python:3.10
+  stage: test
+  script:
+    - pip install hatch
+    - hatch run lint:all
+  interruptible: true
 
-trigger-docs:
-  image: curlimages/curl:latest
+publish-docs:
+  image: quay.io/curl/curl:latest
   stage: publish
   script:
-    - curl -X POST -d "token=f4fb791db48804c4a30dfe809720b9600977141e" https://readthedocs.org/api/v2/webhook/ou-container-builder/206795/
+    - cd docs/_build
+    - 'curl -X PUT -H "Authorization: Bearer $DOCS_TOKEN" -F "archive=@docs.tar.bz2" https://docs-api.ocl.open.ac.uk/upload/container-builder/v3'
   rules:
-    - if: $CI_PIPELINE_SOURCE != "schedule" && $CI_COMMIT_BRANCH == "default"
+    - if: $CI_PIPELINE_SOURCE != "schedule" && $CI_COMMIT_BRANCH == "v3"
+  interruptible: true
 
 publish-package:
   image: python:3.10
   stage: publish
   script:
     - pip install hatch
     - hatch publish -u __token__ -a "$PYPI_TOKEN"
```

### Comparing `ou_container_builder-3.0.0b8/CHANGELOG.md` & `ou_container_builder-3.0.0b9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/prepare_release.py` & `ou_container_builder-3.0.0b9/prepare_release.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/Makefile` & `ou_container_builder-3.0.0b9/docs-old/Makefile`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/building.rst` & `ou_container_builder-3.0.0b9/docs-old/building.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/conf.py` & `ou_container_builder-3.0.0b9/docs-old/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Documentation configuration."""
+
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Path setup --------------------------------------------------------------
```

### Comparing `ou_container_builder-3.0.0b8/docs/index.rst` & `ou_container_builder-3.0.0b9/docs-old/index.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/make.bat` & `ou_container_builder-3.0.0b9/docs-old/make.bat`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/weights.md` & `ou_container_builder-3.0.0b9/docs-old/weights.md`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/content.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/content.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/environment.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/environment.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/flags.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/flags.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/hacks.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/hacks.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/image.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/image.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/index.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/jupyter_server_config.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/jupyter_server_config.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/module.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/module.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/packages.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/packages.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/scripts.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/scripts.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/server.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/server.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/services.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/services.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/sources.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/sources.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/configuration/web_apps.rst` & `ou_container_builder-3.0.0b9/docs-old/configuration/web_apps.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/packs/code-server.rst` & `ou_container_builder-3.0.0b9/docs-old/packs/code-server.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/packs/mariadb.rst` & `ou_container_builder-3.0.0b9/docs-old/packs/mariadb.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/docs/packs/tutorial_server.rst` & `ou_container_builder-3.0.0b9/docs-old/packs/tutorial_server.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/settings.py` & `ou_container_builder-3.0.0b9/ou_container_builder/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Configuration settings."""
+
 import shlex
 import sys
-
 from copy import deepcopy
-from pydantic import BaseModel, Field, HttpUrl, ValidationError, constr, model_validator, create_model
+from typing import Annotated, Any, Literal
+
+from pydantic import BaseModel, Field, HttpUrl, ValidationError, constr, create_model, model_validator
 from rich import print as cli_print
-from typing import Literal, Any, Optional
-from typing_extensions import Annotated
 from yaml import safe_load
 
 from ou_container_builder import packs
 
 
 class Module(BaseModel):
     """Settings for the module configuration."""
@@ -98,15 +98,15 @@
 class PipPackageEntry(BaseModel):
     """Settings for a single entry for a pip installation.
 
     Can either represent a single file or a requirements file.
     """
 
     name: constr(min_length=1)
-    type: Optional[Literal["package"] | Literal["requirements.txt"]] = "package"
+    type: Literal["package"] | Literal["requirements.txt"] | None = "package"
 
     @model_validator(mode="before")
     @classmethod
     def convert_simple_packages(cls: "PipPackageLists", data: Any) -> Any:
         """If only a list of packages is given, convert that to the target structure."""
         if isinstance(data, str):
             return {"name": data, "type": "package"}
@@ -170,15 +170,15 @@
 
     stage: Literal["startup"]
     name: str
     commands: list[str]
 
 
 PacksModel = create_model(
-    "PacksModel", **dict([(key, (value.Options | None, None)) for key, value in packs.EXTENSION_PACKS.items()])
+    "PacksModel", **{key: (value.Options | None, None) for key, value in packs.EXTENSION_PACKS.items()}
 )
 
 
 class OutputBlock(BaseModel):
     """Settings for a single block in the generated Dockerfile."""
 
     block: str
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/state.py` & `ou_container_builder-3.0.0b9/ou_container_builder/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Builder state handling."""
-from collections.abc import Mapping, Iterator
-from copy import deepcopy
 
-from typing import Any, Callable
+from collections.abc import Callable, Iterator, Mapping
+from copy import deepcopy
+from typing import Any
 
 
 def merge_settings(base: dict, new: dict) -> dict:
     """Return a new dictionary created by merging the settings from ``new`` into ``base``.
 
     :param base: The base dictionary to merge into
     :type base: ``dict``
@@ -15,21 +15,20 @@
     :return: A new merged dictionary
     :rtype: ``dict``
     """
     result = {}
     for base_key, base_value in list(base.items()):
         if base_key not in new:
             result[base_key] = deepcopy(base_value)
+        elif isinstance(base_value, list):
+            result[base_key] = list(base_value + new[base_key])
+        elif isinstance(base_value, dict):
+            result[base_key] = merge_settings(base_value, new[base_key])
         else:
-            if isinstance(base_value, list):
-                result[base_key] = list(base_value + new[base_key])
-            elif isinstance(base_value, dict):
-                result[base_key] = merge_settings(base_value, new[base_key])
-            else:
-                result[base_key] = new[base_key]
+            result[base_key] = new[base_key]
     for new_key, new_value in list(new.items()):
         if new_key not in base:
             result[new_key] = deepcopy(new_value)
     return result
 
 
 class State(Mapping):
@@ -56,20 +55,20 @@
         """Notify all listeners of a change."""
 
         def walk(current: dict, path: list[str] | None = None):
             """Walk the updated settings and send out notifications."""
             if path is None:
                 path = []
             for key, value in current.items():
-                prefix = ".".join(path + [key])
+                prefix = ".".join([*path, key])
                 if prefix in self._listeners:
                     for callback in self._listeners[prefix]:
                         callback(self)
                 if isinstance(value, dict):
-                    walk(value, path + [key])
+                    walk(value, [*path, key])
 
         walk(settings)
 
     def __getitem__(self: "State", key: str) -> Any:
         """Retrieve an item from the `State`."""
         return self._state[key]
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/util.py` & `ou_container_builder-3.0.0b9/ou_container_builder/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility functions for working with Docker."""
 
 
 def docker_run_cmd(commands: list[str]) -> str:
     """Generate a docker run command."""
     command_string = " && \\\n    ".join(commands)
-    return f'RUN {command_string}'
+    return f"RUN {command_string}"
 
 
 def docker_copy_cmd(src: str, target: str, from_stage: str | None = None, chmod: str | None = None) -> str:
     """Generate a docker copy command."""
     parts = ["COPY"]
     if from_stage is not None:
         parts.append(f"--from={from_stage}")
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/cli/build.py` & `ou_container_builder-3.0.0b9/ou_container_builder/cli/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Build function."""
-import subprocess
-import typer
 
+import subprocess
 from typing import Annotated, Optional
 
+import typer
 
 from ou_container_builder.cli.base import app
-from ou_container_builder.cli.generate import generate
 from ou_container_builder.cli.clean import clean
+from ou_container_builder.cli.generate import generate
 
 
 @app.command()
 def build(
-    tag: Annotated[Optional[list[str]], typer.Option(help="Docker tags to use")] = None,
-    cache: Annotated[Optional[bool], typer.Option(help="Cache intermediate layers (true)")] = True,
+    tag: Annotated[Optional[list[str]], typer.Option(help="Docker tags to use")] = None,  # noqa: UP007
+    cache: Annotated[bool, typer.Option(help="Cache intermediate layers (true)")] = True,  # noqa: FBT002
 ) -> None:
     """Build the container image."""
     generate()
     cmd = ["buildah", "build", "--jobs", "2"]
     if tag is not None:
         for t in tag:
             cmd.extend(["--tag", t])
     if cache:
         cmd.extend(["--layers"])
     cmd.append(".")
-    process = subprocess.run(cmd)
+    process = subprocess.run(cmd, check=False)  # noqa: S603
     if process.returncode == 0:
         clean()
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/cli/generate.py` & `ou_container_builder-3.0.0b9/ou_container_builder/cli/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """CLI interface for building the container."""
+
 import os
 import shutil
 
 from rich.progress import Progress
 
 from ou_container_builder import core, packs
 from ou_container_builder.cli.base import app
-from ou_container_builder.settings import load_settings, Settings
+from ou_container_builder.settings import Settings, load_settings
 from ou_container_builder.state import State
 
 
 @app.command()
 def generate():
     """Generate the Dockerfile."""
     with Progress() as progress:
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/__init__.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Core builder functionality."""
+
 from rich.progress import Progress
 
-from ou_container_builder.state import State
 from ou_container_builder.core import (
     apt,
     args,
     base,
     content,
     environment,
     python,
@@ -13,15 +13,15 @@
     scripts,
     server,
     services,
     sources,
     user,
     webapp,
 )
-
+from ou_container_builder.state import State
 
 CORE_PACKS = [apt, args, base, content, environment, python, rust, scripts, server, services, sources, user, webapp]
 
 
 def init(state: State, progress: Progress) -> None:
     """Initialise all core packs."""
     core_task = progress.add_task("Initialising core...", total=len(CORE_PACKS))
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/apt.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/apt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """Functionality to handle installing apt packages."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_run_cmd
 
 
-def init(state: State) -> None:
+def init(state: State) -> None:  # noqa: ARG001
     """Unused."""
     pass
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the blocks to install all apt packages in the build and deploy stages."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {
                         "block": docker_run_cmd(
                             [
                                 "DEBIAN_FRONTEND=noninteractive apt-get update -y",
                                 "DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y",
-                                f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['core'])}",
+                                f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['core'])}",  # noqa: E501
                             ]
                         ),
                         "weight": 91,
                     },
                 ],
                 "deploy": [
                     {
                         "block": docker_run_cmd(
                             [
                                 "DEBIAN_FRONTEND=noninteractive apt-get update -y",
                                 "DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y",
-                                f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['core'])}",
+                                f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['core'])}",  # noqa: E501
                             ]
                         ),
                         "weight": 91,
                     },
                 ],
             }
         }
@@ -48,15 +49,15 @@
                 "output_blocks": {
                     "build": [
                         {
                             "block": docker_run_cmd(
                                 [
                                     "DEBIAN_FRONTEND=noninteractive apt-get update -y",
                                     "DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y",
-                                    f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['build'])}",
+                                    f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['build'])}",  # noqa: E501
                                 ]
                             ),
                             "weight": 141,
                         },
                     ],
                 }
             }
@@ -67,15 +68,15 @@
                 "output_blocks": {
                     "deploy": [
                         {
                             "block": docker_run_cmd(
                                 [
                                     "DEBIAN_FRONTEND=noninteractive apt-get update -y",
                                     "DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y",
-                                    f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['deploy'])}",
+                                    f"DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends {' '.join(state['packages']['apt']['deploy'])}",  # noqa: E501
                                 ]
                             ),
                             "weight": 141,
                         },
                     ],
                 }
             }
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/args.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/args.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Functionality for setting up the build arguments."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 
 
 def init(state: State) -> None:
     """Set the default ARGs."""
     state.update({"args": []})
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the ARG blocks for the two stages."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {
                         "block": "\n".join(
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/base.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for setting up the base system."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 
 
 def init(state: State) -> None:
     """Specify the base packages to install."""
@@ -22,15 +23,15 @@
                 },
                 "pip": {"system": ["pycurl"], "user": ["pycurl"]},
             }
         }
     )
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the FROM blocks for the two stages."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {"block": "# ###########\n# Build Stage\n# ###########\n\n", "weight": 0},
                     {"block": f"FROM {state['image']['base']} as base", "weight": 1},
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/content.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/content.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Functionality for copying content into the image."""
+
 import os
 import shutil
 import subprocess
 
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_copy_cmd
 
 
-def init(state: State) -> None:
+def init(state: State) -> None:  # noqa: ARG001
     """Unused."""
     pass
 
 
 def generate(state: State, progress: Progress) -> None:
     """Copy the content files."""
     content_task = progress.add_task("Compressing content to distribute...", target=len(state["content"]))
@@ -36,40 +37,42 @@
                     content["source"], os.path.join("ou-builder-build", "content", "archives", f"content-{idx}")
                 )
                 unpack_commands.append(f"cp /usr/share/ou/content/content-{idx} $HOME/{content['target']}")
             else:
                 basepath, itemname = os.path.split(content["source"])
                 if basepath:
                     subprocess.run(
-                        [
+                        [  # noqa: S603, S607
                             "tar",
                             "-jcf",
                             os.path.join("ou-builder-build", "content", "archives", f"content-{idx}.tar.bz2"),
                             "--directory",
                             basepath,
                             itemname,
-                        ]
+                        ],
+                        check=False,
                     )
                 else:
                     subprocess.run(
-                        [
+                        [  # noqa: S603, S607
                             "tar",
                             "-jcf",
                             os.path.join("ou-builder-build", "content", "archives", f"content-{idx}.tar.bz2"),
                             itemname,
-                        ]
+                        ],
+                        check=False,
                     )
                 unpack_commands.append(f"mkdir -p $HOME/{content['target']}")
                 if content["overwrite"] == "always":
                     unpack_commands.append(
-                        f"tar -jxf /usr/share/ou/content/content-{idx}.tar.bz2 --directory $HOME/{content['target']} --strip-components=1"
+                        f"tar -jxf /usr/share/ou/content/content-{idx}.tar.bz2 --directory $HOME/{content['target']} --strip-components=1"  # noqa: E501
                     )
                 elif content["overwrite"] == "never":
                     unpack_commands.append(
-                        f"tar -jxf /usr/share/ou/content/content-{idx}.tar.bz2 --skip-old-files --directory $HOME/{content['target']} --strip-components=1"
+                        f"tar -jxf /usr/share/ou/content/content-{idx}.tar.bz2 --skip-old-files --directory $HOME/{content['target']} --strip-components=1"  # noqa: E501
                     )
         progress.update(content_task, advance=1)
     if len(unpack_commands) > 0:
         with open(os.path.join("ou-builder-build", "content", "020-distributing-files"), "w") as out_f:
             unpack_commmand_text = "\n".join(unpack_commands)
             out_f.write(
                 f"""#!/bin/bash
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/environment.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Functionality for setting up the system environment variables."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 
 
 def init(state: State) -> None:
-    """Unused."""
+    """Set the default environments."""
     state.update(
         {
             "environment": [
                 {"name": "USER", "value": None},
                 {"name": "UID", "value": "1000"},
                 {"name": "GID", "value": "100"},
                 {"name": "MODULE_CODE", "value": None},
@@ -31,15 +32,15 @@
             env["value"] = state["image"]["user"]
         elif env["name"] == "MODULE_CODE" and "module" in state and "code" in state["module"]:
             env["value"] = state["module"]["code"]
         elif env["name"] == "MODULE_PRESENTATION" and "module" in state and "presentation" in state["module"]:
             env["value"] = state["module"]["presentation"]
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the ENV blocks for the two stages."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {
                         "block": "\n".join(f'ENV {env["name"]}="{env["value"]}"' for env in state["environment"]),
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/python.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 The packages are downloaded and built in the build stage and then the wheels are copied over into the
 deploy stage. The system packages are then installed into a venv at /var/lib/ou/python/system.
 
 Packages are installed from requirements files. If packages are provided directly, then a requirements.txt
 is generated for those.
 """
+
 import os
 
 from rich.progress import Progress
 
 from ou_container_builder.state import State
-from ou_container_builder.util import docker_run_cmd, docker_copy_cmd
-
+from ou_container_builder.util import docker_copy_cmd, docker_run_cmd
 
 STARTUP_INSTALL_SCRIPT = """#/bin/bash
 pip install --user --no-index /usr/share/ou/python/user/*.whl
 """
 
 
-def init(state: State) -> None:
+def init(state: State) -> None:  # noqa: ARG001
     """Unused."""
     pass
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the python wheel build and install blocks."""
     # If there are any installed packages copy them from the build to the deploy stage
     if len(state["packages"]["pip"]["system"]) > 0 or len(state["packages"]["pip"]["user"]) > 0:
         state.update(
             {
                 "output_blocks": {
                     "deploy": [
@@ -43,15 +43,15 @@
     # Install any system python packages
     if len(state["packages"]["pip"]["system"]) > 0:
         system_packages = "\\n".join(
             [pkg["name"] for pkg in state["packages"]["pip"]["system"] if pkg["type"] == "package"]
         )
         requirement_files = " ".join(
             [
-                f'-r /usr/share/ou/python/system/requirements-{idx+1}.txt'
+                f"-r /usr/share/ou/python/system/requirements-{idx+1}.txt"
                 for idx, pkg in enumerate(state["packages"]["pip"]["system"])
                 if pkg["type"] == "requirements.txt"
             ]
         )
         state.update(
             {
                 "output_blocks": {
@@ -80,27 +80,27 @@
                                 ]
                             ),
                             "weight": 161,
                         },
                         {
                             "block": docker_run_cmd(
                                 [
-                                    f"pip wheel --no-cache-dir -w /usr/share/ou/python/system -r /usr/share/ou/python/system/requirements-0.txt {requirement_files}",
+                                    f"pip wheel --no-cache-dir -w /usr/share/ou/python/system -r /usr/share/ou/python/system/requirements-0.txt {requirement_files}",  # noqa: E501
                                 ]
                             ),
                             "weight": 162,
                         },
                     ],
                     "deploy": [
                         {
                             "block": docker_run_cmd(
                                 [
                                     "mkdir -p /var/lib/ou/python",
                                     "python -m venv /var/lib/ou/python/system",
-                                    "/var/lib/ou/python/system/bin/pip install --no-index --no-deps /usr/share/ou/python/system/*.whl",
+                                    "/var/lib/ou/python/system/bin/pip install --no-index --no-deps /usr/share/ou/python/system/*.whl",  # noqa: E501
                                     "/var/lib/ou/python/system/bin/pip uninstall -y ipykernel",
                                 ]
                             ),
                             "weight": 162,
                         },
                     ],
                 }
@@ -110,15 +110,15 @@
     if len(state["packages"]["pip"]["user"]) > 0:
         user_packages = "\\n".join(
             [pkg["name"] for pkg in state["packages"]["pip"]["user"] if pkg["type"] == "package"]
         )
         # Build and copy the requirements files
         requirement_files = " ".join(
             [
-                f'-r /usr/share/ou/python/user/requirements-{idx+1}.txt'
+                f"-r /usr/share/ou/python/user/requirements-{idx+1}.txt"
                 for idx, pkg in enumerate(state["packages"]["pip"]["user"])
                 if pkg["type"] == "requirements.txt"
             ]
         )
         state.update(
             {
                 "output_blocks": {
@@ -139,24 +139,24 @@
         state.update(
             {
                 "output_blocks": {
                     "build": [
                         {
                             "block": docker_run_cmd(
                                 [
-                                    'mkdir -p /usr/share/ou/python/user',
+                                    "mkdir -p /usr/share/ou/python/user",
                                     f'echo "{user_packages}" > /usr/share/ou/python/user/requirements-0.txt',
                                 ]
                             ),
                             "weight": 161,
                         },
                         {
                             "block": docker_run_cmd(
                                 [
-                                    f"pip wheel --no-cache-dir -w /usr/share/ou/python/user -r /usr/share/ou/python/user/requirements-0.txt {requirement_files}"
+                                    f"pip wheel --no-cache-dir -w /usr/share/ou/python/user -r /usr/share/ou/python/user/requirements-0.txt {requirement_files}"  # noqa: E501
                                 ]
                             ),
                             "weight": 164,
                         },
                     ]
                 }
             }
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/rust.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/rust.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Functionality for setting up rust in the build stage."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_run_cmd
 
 
 def init(state: State) -> None:
     """Specify the base packages to install."""
     state.update({"packages": {"apt": {"core": ["curl"]}}})
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the FROM blocks for the two stages."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {
                         "block": docker_run_cmd(
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/services.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for setting up additional apt sources in both stages."""
+
 import os
 import shutil
 
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_copy_cmd
@@ -15,15 +16,15 @@
 
 def services_listener(state: State) -> None:
     """If services are configured, add required core packages."""
     if len(state["services"]) > 0:
         state.update({"packages": {"apt": {"deploy": ["sudo"]}}})
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the commands to start services."""
     if os.path.exists(os.path.join("ou-builder-build", "services")):
         shutil.rmtree(os.path.join("ou-builder-build", "services"))
     os.makedirs(os.path.join("ou-builder-build", "services", "sudoers"), exist_ok=True)
     os.makedirs(os.path.join("ou-builder-build", "services", "startup"), exist_ok=True)
     if len(state["services"]) > 0:
         for idx, service in enumerate(state["services"]):
@@ -48,19 +49,19 @@
             {
                 "output_blocks": {
                     "deploy": [
                         {
                             "block": docker_copy_cmd(
                                 os.path.join("ou-builder-build", "services", "sudoers"), "/etc/sudoers.d", chmod="0440"
                             ),
-                            "weight": 241,
+                            "weight": 311,
                         },
                         {
                             "block": docker_copy_cmd(
                                 os.path.join("ou-builder-build", "services", "startup"), "/usr/share/ou/startup.d"
                             ),
-                            "weight": 241,
+                            "weight": 311,
                         },
                     ]
                 }
             }
         )
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/sources.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for setting up additional apt sources in both stages."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_run_cmd
 
 
 def init(state: State) -> None:
@@ -12,27 +13,27 @@
 
 def apt_sources_listener(state: State) -> None:
     """If additional sources are configured, add required core packages."""
     if len(state["sources"]["apt"]) > 0:
         state.update({"packages": {"apt": {"core": ["gnupg"]}}})
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the commands to download signing keys and create source list files."""
     if len(state["sources"]["apt"]) > 0:
         commands = []
         for source in state["sources"]["apt"]:
             if source["dearmor"]:
                 commands.append(
                     f'curl -fsSL "{source["key_url"]}" | gpg --dearmor -o "/usr/share/keyrings/{source["name"]}.gpg"'
                 )
             else:
                 commands.append(f'curl -fsSL "{source["key_url"]}" > "/usr/share/keyrings/{source["name"]}.gpg"')
             commands.append(
-                f'echo "deb [signed-by=/usr/share/keyrings/{source["name"]}.gpg] {source["deb"]["url"]} {source["deb"]["distribution"]} {source["deb"]["component"]}" > "/etc/apt/sources.list.d/{source["name"]}.list"'
+                f'echo "deb [signed-by=/usr/share/keyrings/{source["name"]}.gpg] {source["deb"]["url"]} {source["deb"]["distribution"]} {source["deb"]["component"]}" > "/etc/apt/sources.list.d/{source["name"]}.list"'  # noqa: E501
             )
         state.update(
             {
                 "output_blocks": {
                     "build": [
                         {
                             "block": docker_run_cmd(commands),
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/user.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Functionality for setting up the user in both stages."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_run_cmd
 
 
-def init(state: State) -> None:
+def init(state: State) -> None:  # noqa: ARG001
     """Unused."""
     pass
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the user setup for the two stages."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {
                         "block": docker_run_cmd(
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/webapp.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/webapp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Functionality for setting up the user in both stages."""
+
 from rich.progress import Progress
 
 from ou_container_builder.state import State
-from ou_container_builder.util import docker_run_cmd
 
 
 def init(state: State) -> None:
     """Add a listener for the web_apps key."""
     state.add_listener("web_apps", activate_webapps)
 
 
 def activate_webapps(state: State) -> None:
     """Activate the jupyter-server-proxy and set the config."""
     if len(state["web_apps"]) > 0:
         state.update({"packages": {"pip": {"system": ["jupyter-server-proxy>=4.1.0,<5"]}}})
         state.update(
             {
                 "jupyter_server_config": {
-                    "ServerProxy": {
-                        "servers": dict([(web_app["path"], web_app["options"]) for web_app in state["web_apps"]])
-                    }
+                    "ServerProxy": {"servers": {web_app["path"]: web_app["options"] for web_app in state["web_apps"]}}
                 }
             }
         )
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Unused."""
     pass
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/server/__init__.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Functionality for setting up the base server."""
+
 import json
 import os
+from importlib.resources import files
 
-from importlib.resources import open_text, files
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_copy_cmd, docker_run_cmd
 
-
 CONTAINER_SCRIPT = """#!/bin/bash
 
 mkdir -p $HOME
 sudo chmod 775 $HOME
 
 /var/lib/ou/python/system/bin/python /usr/share/ou/startup.py
 
@@ -27,15 +27,15 @@
 
 def init(state: State) -> None:
     """Specify the base server configuration."""
     state.update(
         {
             "packages": {"pip": {"system": ["jupyter_server>=2.12,<3", "jupyterhub>=4.0.0,<5"]}},
             "jupyter_server_config": {
-                "ServerApp": {"ip": "0.0.0.0", "port": 8888, "trust_xheaders": True},
+                "ServerApp": {"ip": "0.0.0.0", "port": 8888, "trust_xheaders": True},  # noqa: S104
                 "ZMQChannelsWebsocketConnection": {"iopub_data_rate_limit": 10000000},
             },
         }
     )
     state.add_listener("server", server_listener)
 
 
@@ -56,26 +56,26 @@
                         }
                     }
                 }
             }
         )
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the blocks for the deploy stage."""
     os.makedirs(os.path.join("ou-builder-build", "server"), exist_ok=True)
     with open(os.path.join("ou-builder-build", "server", "vce-start.sh"), "w") as out_f:
         out_f.write(CONTAINER_SCRIPT)
     with open(os.path.join("ou-builder-build", "server", "jupyter_server_config.json"), "w") as out_f:
         json.dump(state["jupyter_server_config"], out_f)
     with open(os.path.join("ou-builder-build", "server", "startup.py"), "w") as out_f:
         out_f.write(files("ou_container_builder.core.server").joinpath("startup.py").read_text())
     with open(os.path.join("ou-builder-build", "server", "99-chmod-homedir"), "w") as out_f:
         out_f.write(
-            f"{state['image']['user']} ALL=(root) NOPASSWD: /usr/bin/chmod 775 /home/{state['image']['user']}/{state['module']['code']}-{state['module']['presentation']}\n"
+            f"{state['image']['user']} ALL=(root) NOPASSWD: /usr/bin/chmod 775 /home/{state['image']['user']}/{state['module']['code']}-{state['module']['presentation']}\n"  # noqa: E501
         )
     state.update(
         {
             "output_blocks": {
                 "deploy": [
                     {
                         "block": docker_copy_cmd(
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/core/server/startup.py` & `ou_container_builder-3.0.0b9/ou_container_builder/core/server/startup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Startup script run when the VCE launches."""
 
 import asyncio
 import os
 import re
+from asyncio import subprocess
+
 import tornado
 import tornado.websocket
 
-from asyncio import subprocess
-
 HTML_TEMPLATE = """<!DOCTYPE html>
 <html lang="en">
 <head>
   <title>Your VCE is starting</title>
   <style>
     #status { position: absolute; left: 50%; top: 50%; max-width: 30rem; transform: translate(-50%,-50%); border-top-right-radius: 1rem; box-shadow: 0 0 #0000,var(--tw-ring-shadow, 0 0 #0000),0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.1); }
     h1 { font-size: 1rem; font-weight: bold; padding: 0.5rem 1rem; margin: 0; background-color: rgb(205 207 234); border-top-right-radius: 1rem; color: rgb(39 38 87); }
@@ -137,15 +137,15 @@
 
     def initialize(self: "ProgressHandler", queue: asyncio.queues.Queue) -> None:
         """Initialise the handler with the queue to use."""
         self._queue = queue
 
     def open(self: "ProgressHandler"):
         """Open the Websocket connection and start the queue tracking."""
-        asyncio.create_task(self.track_progress())
+        self._track_progress = asyncio.create_task(self.track_progress())
 
     async def track_progress(self: "ProgressHandler"):
         """Track the progress queue and send it on to the websocket."""
         while True:
             msg = await self._queue.get()
             self.write_message(msg)
 
@@ -153,38 +153,38 @@
 async def main():
     """Run the progress server and the startup scripts."""
     done_event = asyncio.Event()
     queue = asyncio.queues.Queue()
 
     async def run_startup_scripts():
         """Task to run the individual startup scripts."""
-        print("Preparing startup")
+        print("Preparing startup")  # noqa: T201
         await asyncio.sleep(1)
         filenames = os.listdir("/usr/share/ou/startup.d")
         filenames.sort()
-        print("Preparing startup complete")
+        print("Preparing startup complete")  # noqa: T201
         for filename in filenames:
-            tokens = filename.split('-')
+            tokens = filename.split("-")
             if len(tokens) > 0:
                 if re.match("^[0-9]+$", tokens[0]):
                     tokens = tokens[1:]
             if len(tokens) > 0:
                 tokens[0] = tokens[0].title()
                 message = " ".join(tokens)
             else:
                 message = "Unknown activity"
-            print(message, flush=True)
+            print(message, flush=True)  # noqa: T201
             await queue.put({"type": "start", "text": message})
             process = await subprocess.create_subprocess_exec("bash", f"/usr/share/ou/startup.d/{filename}")
             await process.wait()
             if process.returncode != 0:
                 await queue.put({"type": "done", "status": "failure"})
             else:
                 await queue.put({"type": "done", "status": "success"})
-                print(f"{message} complete", flush=True)
+                print(f"{message} complete", flush=True)  # noqa: T201
             await asyncio.sleep(0.5)
         done_event.set()
 
     prefix = os.environ["JUPYTERHUB_SERVICE_PREFIX"] if "JUPYTERHUB_SERVICE_PREFIX" in os.environ else "/"
     application = tornado.web.Application(
         [(f"{prefix}ocl-status", ProgressHandler, {"queue": queue}), ("/.*", IndexRequestHandler)]
     )
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/__init__.py` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Extension packs."""
+
+from collections.abc import Callable
 from importlib import import_module
 from importlib.metadata import entry_points
+from typing import Any
+
 from rich.progress import Progress
-from typing import Callable, Any
 
 from ou_container_builder.state import State
 
-
 EXTENSION_PACKS = {}
 for entry_point in entry_points().select(group="ou_container_builder"):
     EXTENSION_PACKS[entry_point.name] = import_module(entry_point.value)
 
 
 def make_listener(key: str, pack: Any) -> Callable[[State], None]:
     """Create a custom listener for the key and pack."""
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/ipykernel.py` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/ipykernel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Functionality to install an iPython kernel."""
 
 import os
 
 from pydantic import BaseModel
-
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_copy_cmd
 
 name = "ipykernel"
 STARTUP_KERNEL_SCRIPT = """#!/bin/bash
@@ -26,15 +25,15 @@
 
 def init(state: State) -> None:
     """Initialise packs.ipykernel."""
     state.update({"environment": [{"name": "PYDEVD_DISABLE_FILE_VALIDATION", "value": "1"}]})
     state.update({"packages": {"pip": {"user": ["ipykernel"]}}})
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the kernel installation script."""
     os.makedirs(os.path.join("ou-builder-build", "ipykernel"), exist_ok=True)
     with open(os.path.join("ou-builder-build", "ipykernel", "110-activating-the-python-kernel"), "w") as out_f:
         out_f.write(STARTUP_KERNEL_SCRIPT)
     state.update(
         {
             "output_blocks": {
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/jupyterlab.py` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/jupyterlab.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Functionality to install JupyterLab."""
 
-from pydantic import BaseModel
 from typing import Literal
 
+from pydantic import BaseModel
 from rich.progress import Progress
 
 from ou_container_builder.state import State
 from ou_container_builder.util import docker_run_cmd
 
 name = "jupyterlab"
 
@@ -16,31 +16,31 @@
 
     version: Literal[4] = 4
     announcements: bool = False
 
 
 def init(state: State) -> None:
     """Initialise packs.jupyterlab."""
-    if state["packs"]["jupyterlab"]["version"] == 4:
+    if state["packs"]["jupyterlab"]["version"] == 4:  # noqa: PLR2004
         state.update({"packages": {"pip": {"system": ["jupyterlab>=4.0.2,<5"]}}})
     if not state["packs"]["jupyterlab"]["announcements"]:
         state.update(
             {
                 "output_blocks": {
                     "deploy": [
                         {
                             "block": docker_run_cmd(
                                 [
-                                    '/var/lib/ou/python/system/bin/jupyter labextension disable "@jupyterlab/apputils-extension:announcements"'
+                                    '/var/lib/ou/python/system/bin/jupyter labextension disable "@jupyterlab/apputils-extension:announcements"'  # noqa: E501
                                 ]
                             ),
                             "weight": 1001,
                         }
                     ]
                 }
             }
         )
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Unused."""
     pass
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/code_server/__init__.py` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/code_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Functionality to install CodeServer."""
+
 import os
 import shutil
-
 from importlib.resources import open_text
-from pydantic import BaseModel
-from typing import Literal
 
+from pydantic import BaseModel
 from rich.progress import Progress
 
-from ou_container_builder.util import docker_copy_cmd, docker_run_cmd
 from ou_container_builder.state import State
-
+from ou_container_builder.util import docker_copy_cmd, docker_run_cmd
 
 name = "code_server"
 
 
 class Options(BaseModel):
     """Options for the CodeServer pack."""
 
-    version: str = "4.19.1"
+    version: str = "4.23.0"
     extensions: list[str] = []
 
 
 def init(state: State) -> None:
     """Initialise packs.code_server."""
     state.update(
         {
@@ -47,15 +45,15 @@
                     "options": {
                         "command": [
                             "code-server",
                             "--auth",
                             "none",
                             "--disable-update-check",
                             "--bind-addr",
-                            "0.0.0.0",
+                            "0.0.0.0",  # noqa: S104
                             "--port",
                             "{port}",
                         ],
                         "timeout": 60,
                         "new_browser_tab": False,
                         "launcher_entry": {
                             "title": "VS Code",
@@ -64,15 +62,15 @@
                     },
                 }
             ],
         }
     )
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the docker blocks to install Code Server."""
     if os.path.exists(os.path.join("ou-builder-build", "code_server")):
         shutil.rmtree(os.path.join("ou-builder-build", "code_server"))
     os.makedirs(os.path.join("ou-builder-build", "code_server"), exist_ok=True)
     with open(os.path.join("ou-builder-build", "code_server", "vscode.svg"), "w") as out_f:
         with open_text("ou_container_builder.packs.code_server", "vscode.svg") as in_f:
             out_f.write(in_f.read())
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/code_server/vscode.svg` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/code_server/vscode.svg`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/__init__.py` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Functionality to install XFCE4 virtual desktop."""
+
 import os
 import shutil
+from importlib.resources import open_binary, open_text
 
-from importlib.resources import open_text, open_binary
 from pydantic import BaseModel
 from rich.progress import Progress
 
 from ou_container_builder.state import State
-from ou_container_builder.util import docker_run_cmd, docker_copy_cmd
+from ou_container_builder.util import docker_copy_cmd, docker_run_cmd
 
 name = "xfce4"
 
 
 class Options(BaseModel):
     """Options for the XFCE4 pack."""
 
@@ -63,15 +64,15 @@
                     "overwrite": "always",
                 }
             ],
         }
     )
 
 
-def generate(state: State, progress: Progress) -> None:
+def generate(state: State, progress: Progress) -> None:  # noqa: ARG001
     """Generate the files to distribute and the Docker blocks."""
     state.update(
         {
             "output_blocks": {
                 "build": [
                     {
                         "block": docker_run_cmd(
@@ -89,15 +90,15 @@
                         "block": docker_run_cmd(
                             ["ln -s /var/lib/ou/python/system/bin/websockify /usr/local/bin/websockify"]
                         ),
                         "weight": 1021,
                     },
                     {
                         "block": docker_copy_cmd(
-                            "/tmp/websockify/rebind.so", "/usr/local/bin/rebind.so", from_stage="base"
+                            "/tmp/websockify/rebind.so", "/usr/local/bin/rebind.so", from_stage="base"  # noqa: S108
                         ),
                         "weight": 1022,
                     },
                     {
                         "block": docker_copy_cmd(
                             "ou-builder-build/xfce4/desktop.jpg", "/usr/share/backgrounds/xfce/open-university.jpg"
                         ),
```

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/desktop.jpg` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/desktop.jpg`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/xfce4-desktop.xml` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/xfce4-desktop.xml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/ou_container_builder/packs/xfce4/xfwm4.xml` & `ou_container_builder-3.0.0b9/ou_container_builder/packs/xfce4/xfwm4.xml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/tests/cli_tests/test_build.py` & `ou_container_builder-3.0.0b9/tests/cli_tests/test_build.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test that the builder works."""
+
 import os
 import subprocess
 
 from typer import Typer
 from typer.testing import CliRunner
 
 
@@ -16,15 +17,15 @@
         assert not os.path.exists("ou-builder-build")
         result = runner.invoke(app, ["build", "--tag", "code_server:test"])
         assert result.exit_code == 0
         assert not os.path.exists("Dockerfile")
         assert not os.path.exists("ou-builder-build")
     finally:
         os.chdir(cwd)
-        subprocess.run(["buildah", "rmi", "code_server:test"])
+        subprocess.run(["buildah", "rmi", "code_server:test"], check=False)  # noqa: S603, S607
 
 
 def test_build_jupyterlab_v3(runner: CliRunner, app: Typer):
     """Test that building the JupyterLab v3 demo works."""
     cwd = os.getcwd()
     try:
         os.chdir(os.path.join("tests", "demos", "jupyterlab", "v3"))
@@ -33,15 +34,15 @@
         assert not os.path.exists("ou-builder-build")
         result = runner.invoke(app, ["build", "--tag", "jupyterlab_v3:test"])
         assert result.exit_code == 0
         assert not os.path.exists("Dockerfile")
         assert not os.path.exists("ou-builder-build")
     finally:
         os.chdir(cwd)
-        subprocess.run(["buildah", "rmi", "jupyterlab_v3:test"])
+        subprocess.run(["buildah", "rmi", "jupyterlab_v3:test"], check=False)  # noqa: S603, S607
 
 
 def test_build_jupyterlab_v4(runner: CliRunner, app: Typer):
     """Test that building the JupyterLab v4 demo works."""
     cwd = os.getcwd()
     try:
         os.chdir(os.path.join("tests", "demos", "jupyterlab", "v4"))
@@ -50,15 +51,15 @@
         assert not os.path.exists("ou-builder-build")
         result = runner.invoke(app, ["build", "--tag", "jupyterlab_v4:test"])
         assert result.exit_code == 0
         assert not os.path.exists("Dockerfile")
         assert not os.path.exists("ou-builder-build")
     finally:
         os.chdir(cwd)
-        subprocess.run(["buildah", "rmi", "jupyterlab_v4:test"])
+        subprocess.run(["buildah", "rmi", "jupyterlab_v4:test"], check=False)  # noqa: S603, S607
 
 
 def test_build_custom_apt_key_dearmor(runner: CliRunner, app: Typer):
     """Test that building the custom_apt_key_dearmor demo works."""
     cwd = os.getcwd()
     try:
         os.chdir(os.path.join("tests", "demos", "custom_apt_key_dearmor"))
@@ -67,15 +68,15 @@
         assert not os.path.exists("ou-builder-build")
         result = runner.invoke(app, ["build", "--tag", "custom_apt_key_dearmor:test"])
         assert result.exit_code == 0
         assert not os.path.exists("Dockerfile")
         assert not os.path.exists("ou-builder-build")
     finally:
         os.chdir(cwd)
-        subprocess.run(["buildah", "rmi", "custom_apt_key_dearmor:test"])
+        subprocess.run(["buildah", "rmi", "custom_apt_key_dearmor:test"], check=False)  # noqa: S603, S607
 
 
 def test_build_openrefine(runner: CliRunner, app: Typer):
     """Test that building the openrefine demo works."""
     cwd = os.getcwd()
     try:
         os.chdir(os.path.join("tests", "demos", "openrefine"))
@@ -84,8 +85,8 @@
         assert not os.path.exists("ou-builder-build")
         result = runner.invoke(app, ["build", "--tag", "openrefine:test"])
         assert result.exit_code == 0
         assert not os.path.exists("Dockerfile")
         assert not os.path.exists("ou-builder-build")
     finally:
         os.chdir(cwd)
-        subprocess.run(["buildah", "rmi", "openrefine:test"])
+        subprocess.run(["buildah", "rmi", "openrefine:test"], check=False)  # noqa: S603, S607
```

### Comparing `ou_container_builder-3.0.0b8/tests/cli_tests/test_generate_and_clean.py` & `ou_container_builder-3.0.0b9/tests/cli_tests/test_generate_and_clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the generate and clean functions."""
+
 import os
 
 from typer import Typer
 from typer.testing import CliRunner
 
 
 def test_generate_and_clean(runner: CliRunner, app: Typer):
```

### Comparing `ou_container_builder-3.0.0b8/tests/cli_tests/test_nocommand.py` & `ou_container_builder-3.0.0b9/tests/cli_tests/test_nocommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test running without a command."""
+
 from typer import Typer
 from typer.testing import CliRunner
 
 
 def test_no_command(runner: CliRunner, app: Typer):
     """Test that not providing a command fails."""
     result = runner.invoke(app)
```

### Comparing `ou_container_builder-3.0.0b8/tests/demos/demo-tests.sh` & `ou_container_builder-3.0.0b9/tests/demos/demo-tests.sh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml` & `ou_container_builder-3.0.0b9/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod` & `ou_container_builder-3.0.0b9/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf` & `ou_container_builder-3.0.0b9/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/tests/demos/openrefine/ContainerConfig.yaml` & `ou_container_builder-3.0.0b9/tests/demos/openrefine/ContainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/test_state.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for the state management functionality."""
+
 from unittest.mock import Mock
 
-from ou_container_builder.state import merge_settings, State
+from ou_container_builder.state import State, merge_settings
 
 
 def test_basic_merge() -> None:
     """Test that a basic merge works."""
     result = merge_settings({}, {"a": "value"})
     assert result["a"] == "value"
 
@@ -88,11 +89,11 @@
     assert len(state) == 2
 
 
 def test_state_iterate() -> None:
     """Test that iterating over the top-level state keys works."""
     state = State()
     for _ in state:
-        assert False
+        raise AssertionError()
     state.update({"a": "value"})
     for value in state:
         assert value == "a"
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/test_util.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the utility functions."""
+
 from ou_container_builder.util import docker_copy_cmd, docker_run_cmd
 
 
 def test_basic_copy_command() -> None:
     """Test the basic copy command."""
     assert 'COPY ["source", "target"]' == docker_copy_cmd("source", "target")
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_content_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_content_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test the content settings validation."""
+
 from pydantic import ValidationError
 from pytest import raises
 
 from ou_container_builder.settings import Content
 
-from .util import error_locations
-
 
 def test_valid_content_settings():
     """Test that a valid content configurations pass."""
     Content(source="test", target="/var/lib/test", overwrite="always")
     Content(source="test", target="/var/lib/test", overwrite="never")
 
 
@@ -17,9 +16,9 @@
     """Test that the default settings are set correctly."""
     settings = Content(source="test", overwrite="always")
     assert settings.target == ""
 
 
 def test_invalid_overwrite_mode():
     """Test that an invalid overwrite setting fails."""
-    with raises(ValidationError) as e_info:
+    with raises(ValidationError):
         Content(source="test", overwrite="sometimes")
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_environment_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_environment_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the environment settings validation."""
+
 from pydantic import ValidationError
 from pytest import raises
 
 from ou_container_builder.settings import EnvironmentVariable
 
 from .util import error_locations
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_image_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_image_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the image settings validation."""
+
 from ou_container_builder.settings import Image
 
 
 def test_valid_image_settings():
     """Test that a valid module configuration passes."""
     settings = Image(base="debian:stable", user="jovyan")
     assert settings.base == "debian:stable"
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_module_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_module_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the module settings validation."""
+
 from pydantic import ValidationError
 from pytest import raises
 
 from ou_container_builder.settings import Module
 
 from .util import error_locations
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_packages_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_packages_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test the packages settings validation."""
-from ou_container_builder.settings import Packages, PipPackageLists, PipPackageEntry
+
+from ou_container_builder.settings import Packages, PipPackageEntry, PipPackageLists
 
 
 def test_valid_packages_settings():
     """Test that a valid packages configuration passes."""
     settings = Packages(apt=["curl"], pip=["jupyterlab"])
     assert settings.apt.build == ["curl"]
     assert settings.apt.deploy == ["curl"]
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_server_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_server_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the server settings validation."""
+
 from ou_container_builder.settings import Server
 
 
 def test_default_server_settings():
     """Test that the default server configuration passes."""
     settings = Server()
     assert settings.default_path == "/"
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_sources_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_sources_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the sources settings validation."""
+
 from pydantic import ValidationError
 from pytest import raises
 
 from ou_container_builder.settings import AptDebLine, AptSource, Sources
 
 from .util import error_locations
```

### Comparing `ou_container_builder-3.0.0b8/tests/functional_tests/validator_tests/test_webapps_settings.py` & `ou_container_builder-3.0.0b9/tests/functional_tests/validator_tests/test_webapps_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """Test the sources settings validation."""
-from pydantic import ValidationError
-from pytest import raises
 
 from ou_container_builder.settings import WebApp
 
-from .util import error_locations
-
 
 def test_valid_web_app_settings():
     """Test that a valid sources configuration passes."""
     WebApp(
         path="test",
         options={
             "command": ["python", "-m", "http.server", "{port}"],
```

### Comparing `ou_container_builder-3.0.0b8/README.md` & `ou_container_builder-3.0.0b9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,69 @@
-# OU Container Builder
+Metadata-Version: 2.3
+Name: ou-container-builder
+Version: 3.0.0b9
+Project-URL: Documentation, https://github.com/unknown/ou-container-builder#readme
+Project-URL: Issues, https://github.com/unknown/ou-container-builder/issues
+Project-URL: Source, https://github.com/unknown/ou-container-builder
+Author-email: Mark Hall <mark.hall@work.room3b.eu>
+License-Expression: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.10
+Requires-Dist: jinja2<4,>=3
+Requires-Dist: pydantic<3,>=2
+Requires-Dist: pyyaml<7,>=6
+Requires-Dist: rich<14,>=13
+Requires-Dist: typer
+Description-Content-Type: text/markdown
 
-Documentation for the OU Container Builder can be found here: https://ou-container-builder.readthedocs.io
+# OU Container Builder
 
-![Validation Status](https://github.com/mmh352/ou-container-builder/workflows/Validation/badge.svg) ![Tests](https://github.com/mmh352/ou-container-builder/workflows/Tests/badge.svg) ![Documentation](https://readthedocs.org/projects/ou-container-builder/badge/?version=latest)
+Documentation for the OU Container Builder can be found here: https://docs.ocl.open.ac.uk/container-builder/v3
 
 # Install and Run
 
-To run the OU Container Builder you need to install the following two requirements:
-
-* [Python 3.8 (or higher)](https://www.python.org/downloads/)
-* [Pipx](https://pipxproject.github.io/pipx/)
-
-Then, to install the OU Container Builder run
-
-```
-pipx install git+https://github.com/mmh352/ou-container-builder.git
-```
-
-To upgrade to the latest version, run:
-
-```
-pipx upgrade ou-container-builder
-```
 
-You can then run the OU Container Builder using the following command:
-
-```
-ou-container-builder
-```
-
-## Demo
-
-To build the demo container:
-
-1. Clone the repository
-2. Change into the ```demo``` directory
-3. Run
-
-   ```
-   ou-container-builder
-   ```
-
-The resulting container listens for connections on port 8888 and it is recommended that you mount the
-```/home/ou-user``` directory as a volume.
 
 ## Development
 
-To work on the OU Container Builder you need to install an additional dependency:
+The OU Container Builder has the following dependencies:
 
-* [Poetry](https://python-poetry.org/)
+* [Python](https://www.python.org/) 3.10 or 3.11 (higher may also work, but is not tested)
+* [Hatch](https://hatch.pypa.io/latest/)
+* [pre-commit]()
 
-Then use
+After installing these, use the following command to run the tests
 
 ```
-poetry install
+hatch run test
 ```
 
-to install all Python dependencies in a project-specific virtualenv. Then start a shell that runs commands
-within that virtualenv:
+To run the builder itself use
 
 ```
-poetry shell
+hatch shell
 ```
 
-You can now run
+and then you can run
 
 ```
-ou-container-builder
+ocb
 ```
 
-to run your development version of the code.
+to run the development version of the code.
 
-### Validation
+### Code Style
 
-To automatically check that any committed code follows the Python guidelines, install a git pre-commit hook using
+The OU Container Builder uses [Black](https://black.readthedocs.io/en/stable/) and [Ruff](https://docs.astral.sh/ruff/)
+to enforce a code style.
+
+To automatically check that any committed code follows the code style, install a git pre-commit hook using
 the following command:
 
 ```
 pre-commit install
 ```
-
-Validation checks are automatically run and must be passed before code can be merged into the default branch.
```

### Comparing `ou_container_builder-3.0.0b8/pyproject.toml` & `ou_container_builder-3.0.0b9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,43 +15,52 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["pyyaml", "jinja2", "typer[all]", "rich", "pydantic"]
+dependencies = [
+  "PyYAML>=6,<7",
+  "Jinja2>=3,<4",
+  "typer",
+  "rich>=13,<14",
+  "pydantic>=2,<3",
+]
 
 [project.urls]
 Documentation = "https://github.com/unknown/ou-container-builder#readme"
 Issues = "https://github.com/unknown/ou-container-builder/issues"
 Source = "https://github.com/unknown/ou-container-builder"
 
 [project.scripts]
 ou-container-builder = "ou_container_builder.__main__:app"
 ocb = "ou_container_builder.__main__:app"
 
 [project.entry-points.ou_container_builder]
 code_server = "ou_container_builder.packs.code_server"
 jupyterlab = "ou_container_builder.packs.jupyterlab"
 ipykernel = "ou_container_builder.packs.ipykernel"
+irkernel = "ou_container_builder.packs.irkernel"
 xfce4 = "ou_container_builder.packs.xfce4"
 notebook = "ou_container_builder.packs.notebook"
 
 [tool.hatch.version]
 path = "ou_container_builder/__about__.py"
 
 [tool.hatch.envs.default]
 extra-dependencies = [
-  "sphinx>=6.0.0,<7.0.0",
-  "sphinx_rtd_theme",
+  "ou-book-theme>=1.1.1,<2",
+  "jupyter-book>=1,<2",
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
+docs = "jb build docs {args}"
+docs-server = "jb obt serve docs {args}"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 cov-xml = ["- coverage combine", "coverage xml"]
 cov-auto = ["test-cov", "cov-xml"]
 
@@ -61,24 +70,27 @@
 [tool.hatch.envs.lint]
 detached = true
 dependencies = ["black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:ou_container_builder tests}"
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
-all = ["style", "typing"]
+all = ["style"]
 
 [tool.black]
 target-version = ["py310"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py310"
 line-length = 120
+exclude = ["ou_container_builder/core/server/startup.py"]
+
+[tool.ruff.lint]
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -119,21 +131,21 @@
   "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["ou_container_builder"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["ou_container_builder"]
 branch = true
 parallel = true
```

