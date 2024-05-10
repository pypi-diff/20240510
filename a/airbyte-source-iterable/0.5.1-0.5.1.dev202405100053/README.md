# Comparing `tmp/airbyte_source_iterable-0.5.1.tar.gz` & `tmp/airbyte_source_iterable-0.5.1.dev202405100053.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_iterable-0.5.1.tar", max compression
+gzip compressed data, was "airbyte_source_iterable-0.5.1.dev202405100053.tar", max compression
```

## Comparing `airbyte_source_iterable-0.5.1.tar` & `airbyte_source_iterable-0.5.1.dev202405100053.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4532 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/README.md
--rw-r--r--   0        0        0      871 2024-05-07 13:31:02.610844 airbyte_source_iterable-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       65 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/__init__.py
--rw-r--r--   0        0        0     1374 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/components.py
--rw-r--r--   0        0        0    13996 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/run.py
--rw-r--r--   0        0        0     2494 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/campaigns.json
--rw-r--r--   0        0        0      168 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/campaigns_metrics.json
--rw-r--r--   0        0        0      605 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/channels.json
--rw-r--r--   0        0        0     1755 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_bounce.json
--rw-r--r--   0        0        0     2749 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_click.json
--rw-r--r--   0        0        0     1704 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_complaint.json
--rw-r--r--   0        0        0     2257 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_open.json
--rw-r--r--   0        0        0     5994 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_send.json
--rw-r--r--   0        0        0     6124 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_send_skip.json
--rw-r--r--   0        0        0     1773 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_subscribe.json
--rw-r--r--   0        0        0     2665 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/email_unsubscribe.json
--rw-r--r--   0        0        0     1193 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/events.json
--rw-r--r--   0        0        0      307 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/list_users.json
--rw-r--r--   0        0        0      521 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/lists.json
--rw-r--r--   0        0        0      437 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/message_types.json
--rw-r--r--   0        0        0      158 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/metadata.json
--rw-r--r--   0        0        0     1156 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/templates.json
--rw-r--r--   0        0        0    14569 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/schemas/users.json
--rw-r--r--   0        0        0     6482 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/slice_generators.py
--rw-r--r--   0        0        0     4537 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/source.py
--rw-r--r--   0        0        0     1009 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/spec.json
--rw-r--r--   0        0        0    19468 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/streams.py
--rw-r--r--   0        0        0      649 2024-05-07 10:34:29.000000 airbyte_source_iterable-0.5.1/source_iterable/utils.py
--rw-r--r--   0        0        0     5352 1970-01-01 00:00:00.000000 airbyte_source_iterable-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-10 00:50:18.809655 airbyte_source_iterable-0.5.1.dev202405100053/README.md
+-rw-r--r--   0        0        0      887 2024-05-10 00:53:28.700198 airbyte_source_iterable-0.5.1.dev202405100053/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/components.py
+-rw-r--r--   0        0        0    13996 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/run.py
+-rw-r--r--   0        0        0     2494 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/campaigns.json
+-rw-r--r--   0        0        0      168 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/campaigns_metrics.json
+-rw-r--r--   0        0        0      605 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/channels.json
+-rw-r--r--   0        0        0     1755 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_bounce.json
+-rw-r--r--   0        0        0     2749 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_click.json
+-rw-r--r--   0        0        0     1704 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_complaint.json
+-rw-r--r--   0        0        0     2257 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_open.json
+-rw-r--r--   0        0        0     5994 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send.json
+-rw-r--r--   0        0        0     6124 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send_skip.json
+-rw-r--r--   0        0        0     1773 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_subscribe.json
+-rw-r--r--   0        0        0     2665 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_unsubscribe.json
+-rw-r--r--   0        0        0     1193 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/events.json
+-rw-r--r--   0        0        0      307 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/list_users.json
+-rw-r--r--   0        0        0      521 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/lists.json
+-rw-r--r--   0        0        0      437 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/message_types.json
+-rw-r--r--   0        0        0      158 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/metadata.json
+-rw-r--r--   0        0        0     1156 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/templates.json
+-rw-r--r--   0        0        0    14569 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/users.json
+-rw-r--r--   0        0        0     6482 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/slice_generators.py
+-rw-r--r--   0        0        0     4537 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/source.py
+-rw-r--r--   0        0        0     1009 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/spec.json
+-rw-r--r--   0        0        0    19468 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/streams.py
+-rw-r--r--   0        0        0      649 2024-05-10 00:50:18.813655 airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/utils.py
+-rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 airbyte_source_iterable-0.5.1.dev202405100053/PKG-INFO
```

### Comparing `airbyte_source_iterable-0.5.1/README.md` & `airbyte_source_iterable-0.5.1.dev202405100053/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Iterable source connector
 
-
 This is the repository for the Iterable source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/iterable).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/iterable)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_iterable/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-iterable spec
 poetry run source-iterable check --config secrets/config.json
 poetry run source-iterable discover --config secrets/config.json
 poetry run source-iterable read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-iterable build
 ```
 
 An image will be available on your host with the tag `airbyte/source-iterable:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-iterable:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-iterable:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-iterable:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-iterable:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-iterable test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-iterable test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/iterable.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_iterable-0.5.1/pyproject.toml` & `airbyte_source_iterable-0.5.1.dev202405100053/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.1"
+version = "0.5.1.dev202405100053"
 name = "airbyte-source-iterable"
 description = "Source implementation for Iterable."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -19,15 +19,15 @@
 packages = [
     { include = "source_iterable" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 pendulum = "==2.1.2"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "0.88.1"
 requests = "==2.31.0"
 python-dateutil = "==2.8.2"
 
 [tool.poetry.scripts]
 source-iterable = "source_iterable.run:run"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/components.py` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/manifest.yaml` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/campaigns.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/channels.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/channels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_bounce.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_bounce.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_click.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_click.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_complaint.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_complaint.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_open.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_open.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_send.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_send_skip.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_send_skip.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_subscribe.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_subscribe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/email_unsubscribe.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/email_unsubscribe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/events.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/lists.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/templates.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/schemas/users.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/slice_generators.py` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/slice_generators.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/source.py` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/spec.json` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/streams.py` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/source_iterable/utils.py` & `airbyte_source_iterable-0.5.1.dev202405100053/source_iterable/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1/PKG-INFO` & `airbyte_source_iterable-0.5.1.dev202405100053/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,113 +1,127 @@
 Metadata-Version: 2.1
 Name: airbyte-source-iterable
-Version: 0.5.1
+Version: 0.5.1.dev202405100053
 Summary: Source implementation for Iterable.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (==0.88.1)
 Requires-Dist: pendulum (==2.1.2)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: requests (==2.31.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/iterable
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Iterable source connector
 
-
 This is the repository for the Iterable source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/iterable).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/iterable)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_iterable/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-iterable spec
 poetry run source-iterable check --config secrets/config.json
 poetry run source-iterable discover --config secrets/config.json
 poetry run source-iterable read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-iterable build
 ```
 
 An image will be available on your host with the tag `airbyte/source-iterable:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-iterable:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-iterable:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-iterable:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-iterable:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-iterable test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-iterable test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/iterable.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

