# Comparing `tmp/airbyte-source-rss-0.1.0.tar.gz` & `tmp/airbyte_source_rss-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-rss-0.1.0.tar", last modified: Wed Jan 31 18:10:18 2024, max compression
+gzip compressed data, was "airbyte_source_rss-1.0.0.tar", max compression
```

## Comparing `airbyte-source-rss-0.1.0.tar` & `airbyte_source_rss-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     5368 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5390 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5368 2024-01-31 18:10:18.000000 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2024-01-31 18:10:18.000000 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 18:10:18.000000 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-01-31 18:10:18.000000 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-01-31 18:10:18.000000 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-01-31 18:10:18.000000 airbyte-source-rss-0.1.0/airbyte_source_rss.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:10:18.663124 airbyte-source-rss-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1093 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1190 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)     1186 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/incremental_configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5200 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      943 2024-01-31 18:10:16.000000 airbyte-source-rss-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/source_rss/
--rw-r--r--   0 root         (0) root         (0)      118 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/source_rss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      221 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/source_rss/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/source_rss/schemas/
--rw-r--r--   0 root         (0) root         (0)      665 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/source_rss/schemas/items.json
--rw-r--r--   0 root         (0) root         (0)     4871 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/source_rss/source.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/source_rss/spec.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:10:18.667124 airbyte-source-rss-0.1.0/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2107 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)      347 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     3483 2024-01-31 17:51:56.000000 airbyte-source-rss-0.1.0/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4436 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/README.md
+-rw-r--r--   0        0        0      131 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/main.py
+-rw-r--r--   0        0        0      775 2024-04-10 04:00:04.515134 airbyte_source_rss-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/source_rss/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/source_rss/components.py
+-rw-r--r--   0        0        0     1971 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/source_rss/manifest.yaml
+-rw-r--r--   0        0        0      221 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/source_rss/run.py
+-rw-r--r--   0        0        0      472 2024-04-10 03:37:13.000000 airbyte_source_rss-1.0.0/source_rss/source.py
+-rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 airbyte_source_rss-1.0.0/PKG-INFO
```

### Comparing `airbyte-source-rss-0.1.0/README.md` & `airbyte_source_rss-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,124 @@
-# Rabbitmq Destination
+Metadata-Version: 2.1
+Name: airbyte-source-rss
+Version: 1.0.0
+Summary: Source implementation for rss.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: feedparser (==6.0.10)
+Requires-Dist: pytz (==2022.6)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/rss
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
-This is the repository for the Rabbitmq destination connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/destinations/rabbitmq).
+# Rss Source
+
+This is the repository for the Rss configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/rss).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
 
-#### Minimum Python version required `= 3.7.0`
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/destinations/rabbitmq)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `destination_rabbitmq/spec.json` file.
-Note that the `secrets` directory is gitignored by default, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/rss)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_rss/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `destination rabbitmq test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
+
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-rss spec
+poetry run source-rss check --config secrets/config.json
+poetry run source-rss discover --config secrets/config.json
+poetry run source-rss read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name destination-rabbitmq build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/destination-rabbitmq:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/destination-rabbitmq:dev .
+airbyte-ci connectors --name=source-rss build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-rss:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
-docker run --rm airbyte/destination-rabbitmq:dev spec
-docker run --rm -v $(pwd)/secrets:/secrets airbyte/destination-rabbitmq:dev check --config /secrets/config.json
-# messages.jsonl is a file containing line-separated JSON representing AirbyteMessages
-cat messages.jsonl | docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/destination-rabbitmq:dev write --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
+docker run --rm airbyte/source-rss:dev spec
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-rss:dev check --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-rss:dev discover --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-rss:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-rss test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
-### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-rss test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/rss.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/rss.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

