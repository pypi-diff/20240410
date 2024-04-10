# Comparing `tmp/pyodmongo-0.6.7.tar.gz` & `tmp/pyodmongo-0.6.8.tar.gz`

## Comparing `pyodmongo-0.6.7.tar` & `pyodmongo-0.6.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/coverage.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyproject.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    36227 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/delete.md
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/fastapi.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/find.md
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/getting_started.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/indexes.md
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/version.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_db_index.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_queries.py
--rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/tests/test_version.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/coverage.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyproject.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    36227 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/delete.md
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/find.md
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/getting_started.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/indexes.md
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/version.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_db_index.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_queries.py
+-rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/tests/test_version.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.6.8/PKG-INFO
```

### Comparing `pyodmongo-0.6.7/code_of_conduct.md` & `pyodmongo-0.6.8/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/mkdocs.yml` & `pyodmongo-0.6.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyproject.py` & `pyodmongo-0.6.8/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/requirements.txt` & `pyodmongo-0.6.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.6.8/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/.github/workflows/black_formatter.yml` & `pyodmongo-0.6.8/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.6.8/.github/workflows/publishing_docs_s3.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/.github/workflows/python_publish.yml` & `pyodmongo-0.6.8/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/.github/workflows/tests.yml` & `pyodmongo-0.6.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/assets/images/favicon.png` & `pyodmongo-0.6.8/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/assets/images/insomnia_request.png` & `pyodmongo-0.6.8/docs/assets/images/insomnia_request.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/assets/images/logo.png` & `pyodmongo-0.6.8/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.6.8/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/aggregation.md` & `pyodmongo-0.6.8/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/contributing.md` & `pyodmongo-0.6.8/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/db_model.md` & `pyodmongo-0.6.8/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/delete.md` & `pyodmongo-0.6.8/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/fastapi.md` & `pyodmongo-0.6.8/docs/en/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/find.md` & `pyodmongo-0.6.8/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/getting_started.md` & `pyodmongo-0.6.8/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/index.md` & `pyodmongo-0.6.8/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/indexes.md` & `pyodmongo-0.6.8/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/query.md` & `pyodmongo-0.6.8/docs/en/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/en/save.md` & `pyodmongo-0.6.8/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/aggregation.md` & `pyodmongo-0.6.8/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/contributing.md` & `pyodmongo-0.6.8/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/db_model.md` & `pyodmongo-0.6.8/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/delete.md` & `pyodmongo-0.6.8/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/fastapi.md` & `pyodmongo-0.6.8/docs/pt-BR/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/find.md` & `pyodmongo-0.6.8/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/getting_started.md` & `pyodmongo-0.6.8/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/index.md` & `pyodmongo-0.6.8/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/indexes.md` & `pyodmongo-0.6.8/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/query.md` & `pyodmongo-0.6.8/docs/pt-BR/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/docs/pt-BR/save.md` & `pyodmongo-0.6.8/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/async_engine/engine.py` & `pyodmongo-0.6.8/pyodmongo/async_engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/engine/engine.py` & `pyodmongo-0.6.8/pyodmongo/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/engine/utils.py` & `pyodmongo-0.6.8/pyodmongo/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/models/db_model.py` & `pyodmongo-0.6.8/pyodmongo/models/db_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pydantic import ConfigDict
 from pydantic_dbmodel_core import DbModelCore
 from .id_model import Id
 from datetime import datetime
 from typing import ClassVar
 from ..services.model_init import (
     resolve_indexes,
-    resolve_ref_pipeline,
     resolve_class_fields_db_info,
+    resolve_reference_pipeline,
 )
 
 
 class DbModel(DbModelCore):
     id: Id | None = None
     created_at: datetime | None = None
     updated_at: datetime | None = None
@@ -40,11 +40,11 @@
         if attrs.get("_id") is not None:
             attrs["id"] = attrs.pop("_id")
         super().__init__(**attrs)
 
     @classmethod
     def __pydantic_init_subclass__(cls):
         resolve_class_fields_db_info(cls=cls)
-        ref_pipeline = resolve_ref_pipeline(cls=cls, pipeline=[], path=[])
-        setattr(cls, "_reference_pipeline", ref_pipeline)
+        pipeline = resolve_reference_pipeline(cls=cls, pipeline=[])
+        setattr(cls, "_reference_pipeline", pipeline)
         indexes = resolve_indexes(cls=cls)
         setattr(cls, "_init_indexes", indexes)
```

### Comparing `pyodmongo-0.6.7/pyodmongo/models/fields.py` & `pyodmongo-0.6.8/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/models/id_model.py` & `pyodmongo-0.6.8/pyodmongo/models/id_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/queries/comparison_operators.py` & `pyodmongo-0.6.8/pyodmongo/queries/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/queries/logical_operators.py` & `pyodmongo-0.6.8/pyodmongo/queries/logical_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/queries/query_string.py` & `pyodmongo-0.6.8/pyodmongo/queries/query_string.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyodmongo/services/model_init.py` & `pyodmongo-0.6.8/pyodmongo/services/model_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from pydantic import BaseModel
 from pymongo import IndexModel, ASCENDING, TEXT
 from typing import Any, Union, get_origin, get_args
 from types import UnionType
 from ..models.id_model import Id
 from ..models.db_field_info import DbField
-from .aggregate_stages import lookup_and_set
+from .aggregate_stages import (
+    unwind,
+    group_set_replace_root,
+    unset,
+    lookup,
+    set_,
+)
+import copy
 
 
 def resolve_indexes(cls: BaseModel):
     indexes = []
     text_keys = []
     for key in cls.model_fields.keys():
         is_index = cls.model_fields[key]._attributes_set.get("index") or False
@@ -92,62 +99,70 @@
         field_type=field_type,
         by_reference=by_reference,
         is_list=is_list,
         has_model_fields=has_model_fields,
     )
 
 
-def resolve_project_pipeline(cls: BaseModel, path: list):
-    project = {}
+def _paths_to_ref_ids(cls: BaseModel, paths: list, db_field_path: list):
     for field, field_info in cls.model_fields.items():
-        db_field_info = field_annotation_infos(field=field, field_info=field_info)
-        path.append(db_field_info.field_alias)
-        path_str = ".".join(path)
-        project[path_str] = True
-        if db_field_info.has_model_fields:
-            if not db_field_info.by_reference:
-                project.pop(path_str)
-                project.update(
-                    resolve_project_pipeline(cls=db_field_info.field_type, path=path)
-                )
-        path.pop(-1)
-    return project
+        db_field = field_annotation_infos(field=field, field_info=field_info)
+        db_field_path.append(db_field)
+        if db_field.by_reference:
+            paths.append(copy.deepcopy(db_field_path))
+        elif db_field.has_model_fields:
+            _paths_to_ref_ids(
+                cls=db_field.field_type, paths=paths, db_field_path=db_field_path
+            )
+        db_field_path.pop(-1)
+    return paths
 
 
-def resolve_ref_pipeline(cls: BaseModel, pipeline: list, path: list):
-    for field, field_info in cls.model_fields.items():
-        db_field_info = field_annotation_infos(field=field, field_info=field_info)
-        path.append(db_field_info.field_alias)
-        path_str = ".".join(path)
-        if db_field_info.has_model_fields:
-            if db_field_info.by_reference:
-                collection = db_field_info.field_type._collection
-                pipeline += lookup_and_set(
-                    from_=collection,
-                    local_field=path_str,
-                    foreign_field="_id",
-                    as_=path_str,
-                    pipeline=resolve_ref_pipeline(
-                        cls=db_field_info.field_type, pipeline=[], path=[]
-                    ),
-                    is_reference_list=db_field_info.is_list,
-                )
-            else:
-                resolve_ref_pipeline(
-                    cls=db_field_info.field_type,
-                    pipeline=pipeline,
-                    path=path,
+def resolve_reference_pipeline(cls: BaseModel, pipeline: list):
+    paths = _paths_to_ref_ids(cls=cls, paths=[], db_field_path=[])
+    for db_field_path in paths:
+        path_str = ""
+        unwind_index_list = []
+        paths_str_to_group = []
+        db_field: DbField = None
+        for index, db_field in enumerate(db_field_path):
+            db_field: DbField
+            path_str += (
+                "." + db_field.field_alias if path_str != "" else db_field.field_alias
+            )
+
+            if db_field.is_list and not db_field.by_reference:
+                unwind_index_list.append(f"__unwind_{index}")
+                paths_str_to_group.append(path_str)
+                pipeline += unwind(
+                    path=path_str,
+                    array_index=unwind_index_list[-1],
+                    preserve_empty=True,
                 )
-        path.pop(-1)
-    # project = resolve_project_pipeline(cls=cls, path=[])
-    # try:
-    #     project_index = [list(dct.keys())[0] for dct in pipeline].index("$project")
-    #     pipeline[project_index] = {"$project": project}
-    # except ValueError:
-    #     pipeline += [{"$project": project}]
+
+        pipeline += lookup(
+            from_=db_field.field_type._collection,
+            local_field=path_str,
+            foreign_field="_id",
+            as_=path_str,
+            pipeline=resolve_reference_pipeline(cls=db_field.field_type, pipeline=[]),
+        )
+        if not db_field.is_list:
+            pipeline += set_(as_=path_str)
+
+        for index, path_str in enumerate(reversed(paths_str_to_group)):
+            reverse_index = len(paths_str_to_group) - index - 1
+            unwind_index = (
+                "_id" if reverse_index - 1 < 0 else unwind_index_list[reverse_index - 1]
+            )
+            pipeline += group_set_replace_root(
+                id_=unwind_index, field=path_str.split(".")[-1], path_str=path_str
+            )
+            pipeline += unset(fields=[unwind_index_list[reverse_index - 1]])
+
     return pipeline
 
 
 def _recursice_db_fields_info(db_field_info: DbField, path: list) -> DbField:
     if db_field_info.has_model_fields:
         for field, field_info in db_field_info.field_type.model_fields.items():
             rec_db_field_info = field_annotation_infos(
```

### Comparing `pyodmongo-0.6.7/pyodmongo/services/query_operators.py` & `pyodmongo-0.6.8/pyodmongo/services/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_async_aggregate.py` & `pyodmongo-0.6.8/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_async_crud_db.py` & `pyodmongo-0.6.8/tests/test_async_crud_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -484,37 +484,62 @@
 class ClassOne(DbModel):
     attr_1: str = "attr 1"
     _collection: ClassVar = "class_one"
 
 
 class ClassTwoA(BaseModel):
     attr_2_a: str = "attr 2 A"
-    class_one: list[ClassOne | Id] | None = []
+    class_one: list[ClassOne | Id] | None
 
 
 class ClassTwoB(BaseModel):
-    attr_2_b: str
+    attr_2_b: str = "attr 2 B"
     class_two_a: ClassTwoA | None
+    class_two_a_list: list[ClassTwoA] | None
 
 
 class ClassThree(DbModel):
     attr_3: str = "attr 3"
-    class_two: ClassTwoB | None = ClassTwoB(attr_2_b="attr 2 b", class_two_a=None)
+    class_two_b: ClassTwoB | None
+    class_two_b_list: list[ClassTwoB] | None
     _collection: ClassVar = "class_three"
 
 
 @pytest_asyncio.fixture()
 async def drop_collections_one_three():
     await db._db[ClassOne._collection].drop()
     await db._db[ClassThree._collection].drop()
     yield
-    await db._db[ClassOne._collection].drop()
-    await db._db[ClassThree._collection].drop()
+    # await db._db[ClassOne._collection].drop()
+    # await db._db[ClassThree._collection].drop()
 
 
 @pytest.mark.asyncio
-async def test_nested_none_object(drop_collections_one_three):
-    obj = ClassThree()
-    await db.save(obj=ClassOne())
-    await db.save(obj=obj)
+async def test_nested_list_objects(drop_collections_one_three):
+    obj_1 = ClassOne(attr_1="obj_1")
+    obj_2 = ClassOne(attr_1="obj_2")
+    obj_3 = ClassOne(attr_1="obj_3")
+    obj_4 = ClassOne(attr_1="obj_4")
+    obj_5 = ClassOne(attr_1="obj_5")
+    obj_6 = ClassOne(attr_1="obj_6")
+    obj_7 = ClassOne(attr_1="obj_7")
+    obj_8 = ClassOne(attr_1="obj_8")
+    await db.save_all([obj_1, obj_2, obj_3, obj_4, obj_5, obj_6, obj_7, obj_8])
+    obj_9 = ClassTwoA(attr_2_a="obj_9", class_one=[obj_1, obj_2])
+    obj_10 = ClassTwoA(attr_2_a="obj_10", class_one=[obj_3, obj_4])
+    obj_11 = ClassTwoA(attr_2_a="obj_11", class_one=[obj_5, obj_6])
+    obj_12 = ClassTwoA(attr_2_a="obj_12", class_one=[obj_7, obj_8])
+    obj_13 = ClassTwoB(
+        attr_2_b="obj_13", class_two_a=obj_9, class_two_a_list=[obj_9, obj_10]
+    )
+    obj_14 = ClassTwoB(
+        attr_2_b="obj_14", class_two_a=obj_11, class_two_a_list=[obj_11, obj_12]
+    )
+    obj_15 = ClassThree(
+        attr_3="obj_15", class_two_b=obj_13, class_two_b_list=[obj_13, obj_14]
+    )
+    await db.save(obj_15)
+    from pprint import pprint
+
     obj_found = await db.find_one(Model=ClassThree, populate=True)
-    assert obj_found == obj
+    assert obj_found.id == obj_15.id
+    assert obj_found.class_two_b.attr_2_b == "obj_13"
```

### Comparing `pyodmongo-0.6.7/tests/test_class.py` & `pyodmongo-0.6.8/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_db_field_info.py` & `pyodmongo-0.6.8/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_db_index.py` & `pyodmongo-0.6.8/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_dict_empty.py` & `pyodmongo-0.6.8/tests/test_dict_empty.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_fastapi.py` & `pyodmongo-0.6.8/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_model_init_functions.py` & `pyodmongo-0.6.8/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_object_id.py` & `pyodmongo-0.6.8/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_project_pipeline.py` & `pyodmongo-0.6.8/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_pydantic_validators.py` & `pyodmongo-0.6.8/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_queries.py` & `pyodmongo-0.6.8/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_reference_pipeline.py` & `pyodmongo-0.6.8/tests/test_reference_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_save_dict.py` & `pyodmongo-0.6.8/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_sync_aggregate.py` & `pyodmongo-0.6.8/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/tests/test_sync_crud_db.py` & `pyodmongo-0.6.8/tests/test_sync_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/.gitignore` & `pyodmongo-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/LICENSE` & `pyodmongo-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/README.md` & `pyodmongo-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.6.7/pyproject.toml` & `pyodmongo-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.6.7"
+version = "0.6.8"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pyodmongo-0.6.7/PKG-INFO` & `pyodmongo-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.6.7
+Version: 0.6.8
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

