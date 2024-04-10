# Comparing `tmp/hdx_python_api-6.2.6.tar.gz` & `tmp/hdx_python_api-6.2.7.tar.gz`

## Comparing `hdx_python_api-6.2.6.tar` & `hdx_python_api-6.2.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     5565 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.config/coveragerc
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.config/pytest.ini
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    45086 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/documentation/main.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/api/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/api/_version.py
--rwxr-xr-x   0        0        0    24570 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/api/configuration.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/api/hdx_base_configuration.yaml
--rwxr-xr-x   0        0        0     4541 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/api/locations.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/api/remotehdx.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/__init__.py
--rwxr-xr-x   0        0        0   117939 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/dataset.py
--rwxr-xr-x   0        0        0     9438 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0        0        0     6706 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/date_helper.py
--rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0    28529 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/hdxobject.py
--rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/indicator_resource_view_template.yaml
--rwxr-xr-x   0        0        0    11087 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/organization.py
--rwxr-xr-x   0        0        0    29270 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/resource.py
--rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0        0        0     7672 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/resource_view.py
--rwxr-xr-x   0        0        0    15012 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/showcase.py
--rwxr-xr-x   0        0        0     9663 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/user.py
--rwxr-xr-x   0        0        0    22462 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/data/vocabulary.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3860 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/src/hdx/facades/simple.py
--rwxr-xr-x   0        0        0     6148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0        0        0   169337 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/Tag_Mapping_ChainRuleError.csv
--rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/dataset_search_results.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/empty.csv
--rwxr-xr-x   0        0        0    13843 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/organization_show_results.yaml
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/resource_formats.json
--rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/showcase_all_search_results.yaml
--rwxr-xr-x   0        0        0     1548 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/test_data.zip
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/CKAN/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_base_config.yaml
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0      561 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_email_configuration.yaml
--rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_organization_static.yaml
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_resource_static.yaml
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_resource_view_static.yaml
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_showcase_static.yaml
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_user_static.yaml
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/hdx_vocabulary_static.yaml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/gen_resource/test_data_no_years.csv
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/expected_resources_to_update.json
--rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   842237 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0        0        0    48524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0        0        0    38435 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_logic/update_logic_resources.yaml
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/fixtures/update_logic/update_logic_resources_new.yaml
--rwxr-xr-x   0        0        0    45086 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/conftest.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/api/test_ckan.py
--rwxr-xr-x   0        0        0    36252 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0        0        0     3009 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/api/test_locations.py
--rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/__init__.py
--rwxr-xr-x   0        0        0    49910 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0        0        0    77175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0        0        0    11850 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0        0        0    19579 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_organization.py
--rwxr-xr-x   0        0        0    48267 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_resource.py
--rwxr-xr-x   0        0        0    19115 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0        0        0    23052 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_showcase.py
--rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0        0        0    56414 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0        0        0    21178 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_user.py
--rwxr-xr-x   0        0        0   116053 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/data/test_vocabulary.py
--rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3184 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0        0        0     5962 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/tests/hdx/facades/test_simple.py
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/workingexample/my_code.py
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/workingexample/my_resource.csv
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/workingexample/my_resource.xlsx
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/workingexample/run.py
--rwxr-xr-x   0        0        0     1203 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/LICENSE
--rwxr-xr-x   0        0        0     1207 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/pyproject.toml
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 hdx_python_api-6.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4896 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/coveragerc
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/pytest.ini
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    45219 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/documentation/main.md
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24570 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4541 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/locations.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/remotehdx.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   118959 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9438 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     6706 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28529 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11087 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    29270 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7672 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15012 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9663 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22462 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3860 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169337 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13843 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1548 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/CKAN/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      561 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/expected_resources_to_update.json
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842237 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38435 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    45086 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/conftest.py
+-rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/api/test_ckan.py
+-rwxr-xr-x   0        0        0    36252 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3009 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49910 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    77175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11850 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0        0        0    19579 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    48267 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19115 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23052 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    56414 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21178 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116053 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3184 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5962 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/run.py
+-rwxr-xr-x   0        0        0     1203 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/LICENSE
+-rwxr-xr-x   0        0        0     1207 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/README.md
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/PKG-INFO
```

### Comparing `hdx_python_api-6.2.6/CONTRIBUTING.md` & `hdx_python_api-6.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/requirements.txt` & `hdx_python_api-6.2.7/requirements.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --all-extras --output-file=requirements.txt pyproject.toml
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile pyproject.toml --resolver=backtracking --all-extras -o requirements.txt
 annotated-types==0.6.0
     # via pydantic
 attrs==23.2.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
@@ -19,69 +15,60 @@
     # via cryptography
 cfgv==3.4.0
     # via pre-commit
 chardet==5.2.0
     # via frictionless
 charset-normalizer==3.3.2
     # via requests
-ckanapi==4.7
-    # via hdx-python-api (pyproject.toml)
+ckanapi==4.8
 click==8.1.7
     # via typer
-colorama==0.4.6
-    # via typer
-coverage[toml]==7.4.4
+coverage==7.4.4
     # via pytest-cov
 cryptography==42.0.5
     # via pyopenssl
 defopt==6.4.0
-    # via hdx-python-api (pyproject.toml)
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
-docutils==0.20.1
+docutils==0.21.post1
     # via defopt
 email-validator==2.1.1
-    # via hdx-python-api (pyproject.toml)
 et-xmlfile==1.1.0
     # via openpyxl
-filelock==3.13.1
+filelock==3.13.4
     # via virtualenv
 frictionless==5.16.1
     # via hdx-python-utilities
-google-auth==2.28.2
+google-auth==2.29.0
     # via
     #   google-auth-oauthlib
     #   gspread
 google-auth-oauthlib==1.2.0
     # via gspread
-gspread==6.0.2
-    # via hdx-python-api (pyproject.toml)
-hdx-python-country==3.6.9
-    # via hdx-python-api (pyproject.toml)
+gspread==6.1.0
+hdx-python-country==3.7.0
 hdx-python-utilities==3.6.7
-    # via
-    #   hdx-python-api (pyproject.toml)
-    #   hdx-python-country
+    # via hdx-python-country
 humanize==4.9.0
     # via frictionless
 identify==2.5.35
     # via pre-commit
 idna==3.6
     # via
     #   email-validator
     #   requests
 ijson==3.2.3
     # via hdx-python-utilities
-inflect==7.0.0
+inflect==7.2.0
     # via quantulum3
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.3
     # via frictionless
@@ -90,31 +77,29 @@
 jsonpath-ng==1.6.1
     # via libhxl
 jsonschema==4.17.3
     # via
     #   frictionless
     #   tableschema-to-template
 libhxl==5.2.1
-    # via
-    #   hdx-python-api (pyproject.toml)
-    #   hdx-python-country
+    # via hdx-python-country
 loguru==0.7.2
     # via hdx-python-utilities
 makefun==1.15.2
-    # via hdx-python-api (pyproject.toml)
 markdown-it-py==3.0.0
     # via rich
 marko==2.0.3
     # via frictionless
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
+more-itertools==10.2.0
+    # via inflect
 ndg-httpsclient==0.5.1
-    # via hdx-python-api (pyproject.toml)
 nodeenv==1.8.0
     # via pre-commit
 num2words==0.5.13
     # via quantulum3
 oauthlib==3.2.2
     # via requests-oauthlib
 openpyxl==3.1.2
@@ -129,48 +114,39 @@
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
 pockets==0.9.1
     # via sphinxcontrib-napoleon
-pre-commit==3.6.2
-    # via hdx-python-api (pyproject.toml)
-pyasn1==0.5.1
+pre-commit==3.7.0
+pyasn1==0.6.0
     # via
-    #   hdx-python-api (pyproject.toml)
     #   ndg-httpsclient
     #   pyasn1-modules
     #   rsa
-pyasn1-modules==0.3.0
+pyasn1-modules==0.4.0
     # via google-auth
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pydantic==2.6.4
-    # via
-    #   frictionless
-    #   inflect
+    # via frictionless
 pydantic-core==2.16.3
     # via pydantic
 pygments==2.17.2
     # via rich
 pyopenssl==24.1.0
-    # via
-    #   hdx-python-api (pyproject.toml)
-    #   ndg-httpsclient
+    # via ndg-httpsclient
 pyphonetics==0.5.3
     # via hdx-python-country
 pyrsistent==0.20.0
     # via jsonschema
 pytest==8.1.1
-    # via
-    #   hdx-python-api (pyproject.toml)
-    #   pytest-cov
-pytest-cov==4.1.0
-    # via hdx-python-api (pyproject.toml)
+    # via pytest-cov
+pytest-cov==5.0.0
 python-dateutil==2.8.2
     # via
     #   frictionless
     #   hdx-python-utilities
     #   libhxl
 python-io-wrapper==0.3.1
     # via libhxl
@@ -180,43 +156,47 @@
     #   frictionless
 pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 quantulum3==0.9.0
-    # via hdx-python-api (pyproject.toml)
 ratelimit==2.2.1
     # via hdx-python-utilities
 requests==2.31.0
     # via
     #   ckanapi
     #   frictionless
-    #   hdx-python-api (pyproject.toml)
     #   libhxl
     #   requests-file
     #   requests-oauthlib
 requests-file==2.0.0
     # via hdx-python-utilities
-requests-oauthlib==1.4.0
+requests-oauthlib==2.0.0
     # via google-auth-oauthlib
 rfc3986==2.0.0
     # via frictionless
 rich==13.7.1
     # via typer
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.18.6
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
+setuptools==69.2.0
+    # via
+    #   ckanapi
+    #   nodeenv
 shellingham==1.5.4
     # via typer
 simpleeval==0.9.13
     # via frictionless
+simplejson==3.19.2
+    # via ckanapi
 six==1.16.0
     # via
     #   ckanapi
     #   isodate
     #   pockets
     #   python-dateutil
     #   sphinxcontrib-napoleon
@@ -230,41 +210,41 @@
     # via libhxl
 tableschema-to-template==0.0.13
     # via hdx-python-utilities
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
-typer[all]==0.9.0
+typeguard==4.2.1
+    # via inflect
+typer==0.12.3
     # via frictionless
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   frictionless
     #   inflect
     #   pydantic
     #   pydantic-core
+    #   typeguard
     #   typer
 unidecode==1.3.8
     # via
     #   libhxl
     #   pyphonetics
 urllib3==2.2.1
     # via
     #   libhxl
     #   requests
-validators==0.23.1
+validators==0.28.0
     # via frictionless
 virtualenv==20.25.1
     # via pre-commit
 wheel==0.43.0
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
 xlsxwriter==3.2.0
     # via tableschema-to-template
 xlwt==1.3.0
     # via hdx-python-utilities
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `hdx_python_api-6.2.6/.config/pre-commit-config.yaml` & `hdx_python_api-6.2.7/.config/pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     hooks:
       # Run the linter.
       - id: ruff
         args: [--config, .config/ruff.toml, --fix]
       # Run the formatter.
       - id: ruff-format
         args: [--config, .config/ruff.toml]
-  - repo: https://github.com/jazzband/pip-tools
-    rev: 7.4.1
+  - repo: https://github.com/astral-sh/uv-pre-commit
+    rev: v0.1.24
     hooks:
+      # Run the pip compile
       - id: pip-compile
         name: pip-compile requirements.txt
         files: pyproject.toml
-        args: [pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt]
+        args: [ pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt ]
```

### Comparing `hdx_python_api-6.2.6/.github/workflows/publish.yaml` & `hdx_python_api-6.2.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/.github/workflows/run-python-tests.yaml` & `hdx_python_api-6.2.7/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/documentation/main.md` & `hdx_python_api-6.2.7/documentation/main.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 HDX.
 
 The code for the library is [here](https://github.com/OCHA-DAP/hdx-python-api).
 The library has detailed API documentation which can be found in the menu at the top.
 
 
 ## Breaking Changes
+From 6.2.7, generate_resource_from_iterator renamed to
+generate_resource_from_iterable with requirement of iterable rather iterator
+
 From 6.2.6, kwargs take preference over environment variables which take
 preference over configuration files
 
 From 6.2.5, environment variables take preference over kwargs which take
 preference over configuration files
 
 From 6.1.5, any method or parameter with "reference_period" in it is renamed
```

### Comparing `hdx_python_api-6.2.6/documentation/pydoc-markdown.yaml` & `hdx_python_api-6.2.7/documentation/pydoc-markdown.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - hdx.data
       - hdx.facades
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python API
-    theme: mkdocs
+    theme: material
     repo_url: "https://github.com/OCHA-DAP/hdx-python-api"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-api
   pages:
     - title: Home
```

### Comparing `hdx_python_api-6.2.6/src/hdx/api/configuration.py` & `hdx_python_api-6.2.7/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/api/hdx_base_configuration.yaml` & `hdx_python_api-6.2.7/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/api/locations.py` & `hdx_python_api-6.2.7/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/api/remotehdx.py` & `hdx_python_api-6.2.7/src/hdx/api/remotehdx.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/dataset.py` & `hdx_python_api-6.2.7/src/hdx/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2597,29 +2597,29 @@
             filename,
             qc_rows,
             resourcedata,
             headers=headers,
             encoding=encoding,
         )
 
-    def generate_resource_from_iterator(
+    def generate_resource_from_iterable(
         self,
         headers: ListTuple[str],
-        iterator: Iterator[Union[ListTuple, Dict]],
+        iterable: Iterable[Union[ListTuple, Dict]],
         hxltags: Dict[str, str],
         folder: str,
         filename: str,
         resourcedata: Dict,
         datecol: Optional[Union[int, str]] = None,
         yearcol: Optional[Union[int, str]] = None,
         date_function: Optional[Callable[[Dict], Optional[Dict]]] = None,
         quickcharts: Optional[Dict] = None,
         encoding: Optional[str] = None,
     ) -> Tuple[bool, Dict]:
-        """Given headers and an iterator, write rows to csv and create
+        """Given headers and an iterable, write rows to csv and create
         resource, adding to it the dataset. The returned dictionary will
         contain the resource in the key resource, headers in the key headers
         and list of rows in the key rows.
 
         The time period can optionally be set by supplying a column in
         which the date or year is to be looked up. Note that any timezone
         information is ignored and UTC assumed. Alternatively, a function can
@@ -2648,15 +2648,15 @@
         headers in qcheaders. If cutdown is 2, then a resource is created using
         the cut down list. If the key cutdownhashtags is supplied, then only
         the provided hashtags are used for cutting down otherwise the full list
         of HXL tags is used.
 
         Args:
             headers (ListTuple[str]): Headers
-            iterator (Iterator[Union[ListTuple,Dict]]): Iterator returning rows
+            iterable (Iterable[Union[ListTuple,Dict]]): Iterable returning rows
             hxltags (Dict[str,str]): Header to HXL hashtag mapping
             folder (str): Folder to which to write file containing rows
             filename (str): Filename of file to write rows
             resourcedata (Dict): Resource data
             datecol (Optional[Union[int,str]]): Date column for setting time period. Defaults to None (don't set).
             yearcol (Optional[Union[int,str]]): Year column for setting dataset year range. Defaults to None (don't set).
             date_function (Optional[Callable[[Dict],Optional[Dict]]]): Date function to call for each row. Defaults to None.
@@ -2734,15 +2734,15 @@
                     date = parse_date(date)
                     result["startdate"] = date
                     result["enddate"] = date
                 return result
 
             date_function = datecol_function
 
-        for row in iterator:
+        for row in iterable:
             if date_function is not None:
                 result = date_function(row)
                 if result is None:
                     continue
                 startdate = result.get("startdate")
                 if startdate is not None:
                     if startdate < dates[0]:
@@ -2809,14 +2809,46 @@
                         qc_resourcedata,
                         headers=qc["headers"],
                         encoding=encoding,
                     )
                     retdict["qc_resource"] = resource
         return True, retdict
 
+    def generate_resource_from_iterator(
+        self,
+        headers: ListTuple[str],
+        iterator: Iterator[Union[ListTuple, Dict]],
+        hxltags: Dict[str, str],
+        folder: str,
+        filename: str,
+        resourcedata: Dict,
+        datecol: Optional[Union[int, str]] = None,
+        yearcol: Optional[Union[int, str]] = None,
+        date_function: Optional[Callable[[Dict], Optional[Dict]]] = None,
+        quickcharts: Optional[Dict] = None,
+        encoding: Optional[str] = None,
+    ) -> Tuple[bool, Dict]:
+        warnings.warn(
+            "generate_resource_from_iterator() is deprecated, use generate_resource_from_iterable() instead",
+            DeprecationWarning,
+        )
+        return self.generate_resource_from_iterable(
+            headers,
+            iterator,
+            hxltags,
+            folder,
+            filename,
+            resourcedata,
+            datecol,
+            yearcol,
+            date_function,
+            quickcharts,
+            encoding,
+        )
+
     def download_and_generate_resource(
         self,
         downloader: BaseDownload,
         url: str,
         hxltags: Dict[str, str],
         folder: str,
         filename: str,
@@ -2894,15 +2926,15 @@
             url,
             dict_form=True,
             header_insertions=header_insertions,
             row_function=row_function,
             format="csv",
             **kwargs,
         )
-        return self.generate_resource_from_iterator(
+        return self.generate_resource_from_iterable(
             headers,
             iterator,
             hxltags,
             folder,
             filename,
             resourcedata,
             datecol=datecol,
```

### Comparing `hdx_python_api-6.2.6/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.2.7/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/date_helper.py` & `hdx_python_api-6.2.7/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.2.7/src/hdx/data/filestore_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/hdxobject.py` & `hdx_python_api-6.2.7/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/indicator_resource_view_template.yaml` & `hdx_python_api-6.2.7/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/organization.py` & `hdx_python_api-6.2.7/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/resource.py` & `hdx_python_api-6.2.7/src/hdx/data/resource.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.2.7/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/resource_view.py` & `hdx_python_api-6.2.7/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/showcase.py` & `hdx_python_api-6.2.7/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/user.py` & `hdx_python_api-6.2.7/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/data/vocabulary.py` & `hdx_python_api-6.2.7/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.2.7/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.2.7/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/src/hdx/facades/simple.py` & `hdx_python_api-6.2.7/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.2.7/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.2.7/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/dataset_search_results.yaml` & `hdx_python_api-6.2.7/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/organization_show_results.yaml` & `hdx_python_api-6.2.7/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/resource_formats.json` & `hdx_python_api-6.2.7/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/showcase_all_search_results.yaml` & `hdx_python_api-6.2.7/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/test_data.csv` & `hdx_python_api-6.2.7/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/test_data.zip` & `hdx_python_api-6.2.7/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/config/hdx_dataset_static.yaml` & `hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.2.7/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/config/hdx_resource_view_static.yaml` & `hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.2.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.2.7/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.2.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.2.7/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.2.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/expected_resources_to_update.json` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/expected_resources_to_update.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_logic/update_logic_resources.yaml` & `hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/fixtures/update_logic/update_logic_resources_new.yaml` & `hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/conftest.py` & `hdx_python_api-6.2.7/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/api/test_ckan.py` & `hdx_python_api-6.2.7/tests/hdx/api/test_ckan.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,15 +172,17 @@
 
         # check created dataset
         dataset = Dataset.read_from_hdx(name)
         assert dataset["name"] == name
         assert dataset["title"] == title
         assert dataset.get_tags() == tags
         assert dataset.get_maintainer()["id"] == maintainer_id
-        assert dataset.get_organization()["display_name"] == "INNAGO"
+        assert (
+            dataset.get_organization()["display_name"] == "INNAGO (inactive)"
+        )
         resources = dataset.get_resources()
         for i, resource in enumerate(resources):
             assert resource["name"] == f"test_resource_{i}"
             if i % 2 == 0:
                 assert resource.get_format() == "csv"
                 assert resource["url_type"] == "upload"
                 assert "humdata" in resource["url"]
@@ -223,15 +225,17 @@
         dataset = Dataset.read_from_hdx(name)
         assert dataset["name"] == name
         assert dataset["title"] == title
         assert dataset["notes"] == notes
         assert dataset["caveats"] == caveats
         assert dataset.get_tags() == tags
         assert dataset.get_maintainer()["id"] == maintainer_id
-        assert dataset.get_organization()["display_name"] == "INNAGO"
+        assert (
+            dataset.get_organization()["display_name"] == "INNAGO (inactive)"
+        )
         updated_resources = dataset.get_resources()
         for i, updated_resource in enumerate(updated_resources):
             resource = resources[i]
             assert updated_resource["name"] == resource["name"]
             assert updated_resource.get_format() == resource.get_format()
             assert updated_resource["url_type"].lower() == resource["url_type"]
             url = resource.get("url")
@@ -265,15 +269,17 @@
         # check dataset updated for second time
         dataset = Dataset.read_from_hdx(name)
         assert dataset["name"] == name
         assert dataset["title"] == title
         assert "caveats" not in dataset
         assert dataset.get_tags() == tags
         assert dataset.get_maintainer()["id"] == maintainer_id
-        assert dataset.get_organization()["display_name"] == "INNAGO"
+        assert (
+            dataset.get_organization()["display_name"] == "INNAGO (inactive)"
+        )
         updated_resources = dataset.get_resources()
         for i, updated_resource in enumerate(updated_resources):
             resource = resources[i]
             assert updated_resource["name"] == resource["name"]
             assert updated_resource.get_format() == resource.get_format()
             assert updated_resource["url_type"].lower() == resource["url_type"]
             url = resource.get("url")
```

### Comparing `hdx_python_api-6.2.6/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.2.7/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/api/test_locations.py` & `hdx_python_api-6.2.7/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/__init__.py` & `hdx_python_api-6.2.7/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_dataset_core.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_dataset_noncore.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_organization.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_resource.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_resource.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_update_dataset_resources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_user.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.2.7/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/facades/__init__.py` & `hdx_python_api-6.2.7/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.2.7/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.2.7/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.2.7/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/workingexample/my_resource.xlsx` & `hdx_python_api-6.2.7/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/.gitignore` & `hdx_python_api-6.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/LICENSE` & `hdx_python_api-6.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/README.md` & `hdx_python_api-6.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.6/pyproject.toml` & `hdx_python_api-6.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hdx-python-api"
 description = "HDX Python API for interacting with the Humanitarian Data Exchange"
-authors = [{name = "Michael Rans", email = "rans@email.com"}]
+authors = [{name = "Michael Rans"}]
 license = {text = "MIT"}
 keywords = ["HDX", "API", "CKAN", "humanitarian data exchange"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,18 +30,18 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "ckanapi>=4.7",
+    "ckanapi>=4.8",
     "defopt>=6.4.0",
     "email_validator",
-    "hdx-python-country>=3.6.9",
+    "hdx-python-country>=3.7.0",
     "hdx-python-utilities>=3.6.7",
     "libhxl>=5.2.1",
     "makefun",
     "ndg-httpsclient",
     "pyasn1",
     "pyOpenSSL",
     "quantulum3",
```

### Comparing `hdx_python_api-6.2.6/PKG-INFO` & `hdx_python_api-6.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: hdx-python-api
-Version: 6.2.6
+Version: 6.2.7
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
-Author-email: Michael Rans <rans@email.com>
+Author: Michael Rans
 License: MIT
 License-File: LICENSE
 Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -21,18 +21,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: ckanapi>=4.7
+Requires-Dist: ckanapi>=4.8
 Requires-Dist: defopt>=6.4.0
 Requires-Dist: email-validator
-Requires-Dist: hdx-python-country>=3.6.9
+Requires-Dist: hdx-python-country>=3.7.0
 Requires-Dist: hdx-python-utilities>=3.6.7
 Requires-Dist: libhxl>=5.2.1
 Requires-Dist: makefun
 Requires-Dist: ndg-httpsclient
 Requires-Dist: pyasn1
 Requires-Dist: pyopenssl
 Requires-Dist: quantulum3
```

