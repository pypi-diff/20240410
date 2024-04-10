# Comparing `tmp/sfapi_client-0.0.8.tar.gz` & `tmp/sfapi_client-0.0.9.tar.gz`

## Comparing `sfapi_client-0.0.8.tar` & `sfapi_client-0.0.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/LEGAL
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/mkdocs.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/pytest.ini
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/requirements-dev.txt
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.github/workflows/black.yml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.github/workflows/ruff.yml
--rwxr-xr-x   0        0        0     1086 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/gen_examples.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/gen_sync.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/index.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/community/contributing.md
--rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/examples/check_current_and_past_jobs.ipynb
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/examples/getting_bearer_token.ipynb
--rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/examples/run_job_and_check_status.ipynb
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/javascript/apiselector.js
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/quickstart/index.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/SUMMARY.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/client/index.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/compute/index.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/exceptions/index.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/groups/index.md
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/jobs/index.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/paths/index.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/projects/index.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/resources/index.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/docs/reference/async/users/index.md
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/scripts/run.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_compute.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_jobs.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_monitor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_utils.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/client.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/compute.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/exceptions.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/groups.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/jobs.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/paths.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/projects.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/resources.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/__init__.py
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/client.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/compute.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/groups.py
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/jobs.py
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/paths.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/projects.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_async/users.py
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_models/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_models/job_status_response_sacct.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_models/job_status_response_squeue.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_models/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/__init__.py
--rw-r--r--   0        0        0    15962 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/client.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/compute.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/groups.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/jobs.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/paths.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/projects.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/src/sfapi_client/_sync/users.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_api.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_api_async.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_client.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_client_async.py
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_compute.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_compute_async.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_groups.py
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_groups_async.py
--rwxr-xr-x   0        0        0     4617 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_jobs.py
--rwxr-xr-x   0        0        0     6390 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_jobs_async.py
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_paths.py
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_paths_async.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_projects.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_projects_async.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_resources.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_resources_async.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_users.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/tests/test_users_async.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/.gitignore
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/LICENSE
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/README.md
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 sfapi_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/LEGAL
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/mkdocs.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/pytest.ini
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/requirements-dev.txt
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.github/workflows/black.yml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.github/workflows/ruff.yml
+-rwxr-xr-x   0        0        0     1086 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/gen_examples.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/gen_sync.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/index.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/community/contributing.md
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/examples/check_current_and_past_jobs.ipynb
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/examples/getting_bearer_token.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/examples/run_job_and_check_status.ipynb
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/javascript/apiselector.js
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/quickstart/index.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/SUMMARY.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/client/index.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/compute/index.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/exceptions/index.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/groups/index.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/jobs/index.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/paths/index.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/projects/index.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/resources/index.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/docs/reference/async/users/index.md
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/scripts/run.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_compute.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_jobs.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_monitor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_utils.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/client.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/compute.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/exceptions.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/groups.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/jobs.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/paths.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/projects.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/resources.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/__init__.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/client.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/compute.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/groups.py
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/jobs.py
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/paths.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/projects.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_async/users.py
+-rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_models/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_models/job_status_response_sacct.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_models/job_status_response_squeue.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_models/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/__init__.py
+-rw-r--r--   0        0        0    16142 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/client.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/compute.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/groups.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/jobs.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/paths.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/projects.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/src/sfapi_client/_sync/users.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_api.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_api_async.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_client_async.py
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_compute.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_compute_async.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_groups.py
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_groups_async.py
+-rwxr-xr-x   0        0        0     4617 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_jobs.py
+-rwxr-xr-x   0        0        0     6390 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_jobs_async.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_paths.py
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_paths_async.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_projects.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_projects_async.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_resources.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_resources_async.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_users.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/tests/test_users_async.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/.gitignore
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 sfapi_client-0.0.9/PKG-INFO
```

### Comparing `sfapi_client-0.0.8/LEGAL` & `sfapi_client-0.0.9/LEGAL`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/mkdocs.yml` & `sfapi_client-0.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/.github/workflows/mkdocs.yml` & `sfapi_client-0.0.9/.github/workflows/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 permissions:
   contents: write
 jobs:
   deploy:
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/')
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.x
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           key: mkdocs-${{ github.ref }}
           path: .cache
           restore-keys: |
             mkdocs-
       - run: pip install .[docs]
       - run: mkdocs build
```

### Comparing `sfapi_client-0.0.8/.github/workflows/pypi.yml` & `sfapi_client-0.0.9/.github/workflows/pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   pull_request:
 
 jobs:
   build:
     name: Build wheel
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install pypa/build
         run: >-
           python -m
           pip install
           build
@@ -29,15 +29,15 @@
         run: >-
           python -m
           build
           --sdist
           --wheel
           --outdir dist/
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: wheel
           path: ./dist/
 
   pypi-publish:
     needs: build
     name: Upload release to PyPI
@@ -45,13 +45,13 @@
     environment:
       name: pypi
       url: https://pypi.org/p/sfapi_client
     permissions:
       id-token: write
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/')
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: wheel
           path: dist
       - name: Publish package PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `sfapi_client-0.0.8/.github/workflows/pytest.yml` & `sfapi_client-0.0.9/.github/workflows/pytest.yml`

 * *Files 25% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           if [ -f pyproject.toml ]; then pip install -e .[test]; fi
       - name: Test with pytest
```

### Comparing `sfapi_client-0.0.8/docs/gen_examples.py` & `sfapi_client-0.0.9/docs/gen_examples.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/gen_sync.py` & `sfapi_client-0.0.9/docs/gen_sync.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/index.md` & `sfapi_client-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/examples/check_current_and_past_jobs.ipynb` & `sfapi_client-0.0.9/docs/examples/check_current_and_past_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/examples/getting_bearer_token.ipynb` & `sfapi_client-0.0.9/docs/examples/getting_bearer_token.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/examples/run_job_and_check_status.ipynb` & `sfapi_client-0.0.9/docs/examples/run_job_and_check_status.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/javascript/apiselector.js` & `sfapi_client-0.0.9/docs/javascript/apiselector.js`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/quickstart/index.md` & `sfapi_client-0.0.9/docs/quickstart/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/reference/SUMMARY.txt` & `sfapi_client-0.0.9/docs/reference/SUMMARY.txt`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/reference/async/compute/index.md` & `sfapi_client-0.0.9/docs/reference/async/compute/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/reference/async/groups/index.md` & `sfapi_client-0.0.9/docs/reference/async/groups/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/reference/async/jobs/index.md` & `sfapi_client-0.0.9/docs/reference/async/jobs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/reference/async/paths/index.md` & `sfapi_client-0.0.9/docs/reference/async/paths/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/docs/reference/async/projects/index.md` & `sfapi_client-0.0.9/docs/reference/async/projects/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/scripts/run.py` & `sfapi_client-0.0.9/scripts/run.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_jobs.py` & `sfapi_client-0.0.9/src/sfapi_client/_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_monitor.py` & `sfapi_client-0.0.9/src/sfapi_client/_monitor.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/client.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,7 +508,14 @@
 AsyncCompute.model_rebuild()
 AsyncGroup.model_rebuild()
 AsyncUser.model_rebuild()
 AsyncProject.model_rebuild()
 AsyncRemotePath.model_rebuild()
 AsyncRole.model_rebuild()
 AsyncGroupMember.model_rebuild()
+
+# Ensure that the job models are built, we need to import here to
+# avoid circular imports
+from .jobs import AsyncJobSacct, AsyncJobSqueue  # noqa: E402
+
+AsyncJobSqueue.model_rebuild()
+AsyncJobSacct.model_rebuild()
```

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/compute.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/groups.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/jobs.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/paths.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,18 @@
             binary_file_data = b64decode(file_data)
             return BytesIO(binary_file_data)
         else:
             return StringIO(file_data)
 
     @staticmethod
     async def _ls(
-        compute: "Compute", path, directory=False, filter_dots=True  # noqa: F821
+        compute: "AsyncCompute",  # noqa: F821
+        path,
+        directory=False,
+        filter_dots=True,  # noqa: F821
     ) -> List["RemotePath"]:  # noqa: F821
         r = await compute.client.get(f"utilities/ls/{compute.name}/{path}")
 
         json_response = r.json()
         directory_listing_response = DirectoryListingResponse.model_validate(
             json_response
         )
```

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/projects.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_async/users.py` & `sfapi_client-0.0.9/src/sfapi_client/_async/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     client: Optional["AsyncClient"]  # noqa: F821
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     @staticmethod
     @check_auth
     async def _fetch_user(
-        client: "AsyncClient", username: Optional[str] = None  # noqa: F821
+        client: "AsyncClient",  # noqa: F821
+        username: Optional[str] = None,  # noqa: F821
     ):  # noqa: F821
         url = "account/"
         if username is not None:
             url = f"{url}?username={username}"
 
         response = await client.get(url)
         json_response = response.json()
```

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_models/__init__.py` & `sfapi_client-0.0.9/src/sfapi_client/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_models/job_status_response_sacct.py` & `sfapi_client-0.0.9/src/sfapi_client/_models/job_status_response_sacct.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_models/job_status_response_squeue.py` & `sfapi_client-0.0.9/src/sfapi_client/_models/job_status_response_squeue.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_models/resources.py` & `sfapi_client-0.0.9/src/sfapi_client/_models/resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/client.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,7 +508,13 @@
 Compute.model_rebuild()
 Group.model_rebuild()
 User.model_rebuild()
 Project.model_rebuild()
 RemotePath.model_rebuild()
 Role.model_rebuild()
 GroupMember.model_rebuild()
+
+# Ensure that the job models are built, we need to import here to
+# avoid circular imports
+from .jobs import JobSacct, JobSqueue
+JobSqueue.model_rebuild()
+JobSacct.model_rebuild()
```

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/compute.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/groups.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/jobs.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/paths.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/projects.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/src/sfapi_client/_sync/users.py` & `sfapi_client-0.0.9/src/sfapi_client/_sync/users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/conftest.py` & `sfapi_client-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_compute.py` & `sfapi_client-0.0.9/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_compute_async.py` & `sfapi_client-0.0.9/tests/test_compute_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_groups.py` & `sfapi_client-0.0.9/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_groups_async.py` & `sfapi_client-0.0.9/tests/test_groups_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_jobs.py` & `sfapi_client-0.0.9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_jobs_async.py` & `sfapi_client-0.0.9/tests/test_jobs_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_paths.py` & `sfapi_client-0.0.9/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_paths_async.py` & `sfapi_client-0.0.9/tests/test_paths_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_projects_async.py` & `sfapi_client-0.0.9/tests/test_projects_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_resources.py` & `sfapi_client-0.0.9/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_resources_async.py` & `sfapi_client-0.0.9/tests/test_resources_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_users.py` & `sfapi_client-0.0.9/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/tests/test_users_async.py` & `sfapi_client-0.0.9/tests/test_users_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/LICENSE` & `sfapi_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/README.md` & `sfapi_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/pyproject.toml` & `sfapi_client-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.8/PKG-INFO` & `sfapi_client-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sfapi_client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for NERSC SF API
 Author-email: Chris Harris <cjh@lbl.gov>, Nicholas Tyler <tylern@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

