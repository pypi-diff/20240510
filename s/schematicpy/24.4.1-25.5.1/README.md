# Comparing `tmp/schematicpy-24.4.1.tar.gz` & `tmp/schematicpy-25.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-24.4.1.tar", max compression
+gzip compressed data, was "schematicpy-25.5.1.tar", max compression
```

## Comparing `schematicpy-24.4.1.tar` & `schematicpy-25.5.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1073 2024-04-25 22:42:45.634479 schematicpy-24.4.1/LICENSE
--rw-r--r--   0        0        0    18039 2024-04-25 22:42:45.634479 schematicpy-24.4.1/README.md
--rw-r--r--   0        0        0     4129 2024-04-25 22:44:14.830276 schematicpy-24.4.1/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/__init__.py
--rw-r--r--   0        0        0     1296 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/__main__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/configuration/__init__.py
--rw-r--r--   0        0        0     7438 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/configuration/configuration.py
--rw-r--r--   0        0        0     5034 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/configuration/dataclasses.py
--rw-r--r--   0        0        0      663 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2024-04-25 22:42:45.638479 schematicpy-24.4.1/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     3193 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/exceptions.py
--rw-r--r--   0        0        0    12587 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/help.py
--rw-r--r--   0        0        0     3415 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/loader.py
--rw-r--r--   0        0        0       59 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/manifest/__init__.py
--rw-r--r--   0        0        0    11844 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/manifest/commands.py
--rw-r--r--   0        0        0    89173 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/manifest/generator.py
--rw-r--r--   0        0        0    23370 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/__init__.py
--rw-r--r--   0        0        0     8057 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/commands.py
--rw-r--r--   0        0        0    19316 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/metadata.py
--rw-r--r--   0        0        0    83344 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    14384 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      515 2024-04-25 22:42:45.642479 schematicpy-24.4.1/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     5037 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/commands.py
--rw-r--r--   0        0        0     6100 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_edges.py
--rw-r--r--   0        0        0    36064 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_graph.py
--rw-r--r--   0        0        0    18286 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_json_schema.py
--rw-r--r--   0        0        0    22845 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_jsonld.py
--rw-r--r--   0        0        0    13333 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_nodes.py
--rw-r--r--   0        0        0    24666 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_parser.py
--rw-r--r--   0        0        0     9597 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_relationships.py
--rw-r--r--   0        0        0     7617 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/data_model_validator.py
--rw-r--r--   0        0        0     6974 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/schemas/json_schema_validator.py
--rw-r--r--   0        0        0       96 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/store/base.py
--rw-r--r--   0        0        0   122222 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/store/synapse.py
--rw-r--r--   0        0        0        0 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/__init__.py
--rw-r--r--   0        0        0     2936 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     3027 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0    10358 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/df_utils.py
--rw-r--r--   0        0        0    10288 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/general.py
--rw-r--r--   0        0        0     6086 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1221 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/io_utils.py
--rw-r--r--   0        0        0    18045 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0    11265 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     6299 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      724 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0      119 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/version.py
--rw-r--r--   0        0        0      164 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/__init__.py
--rw-r--r--   0        0        0    12584 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     5809 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/commands.py
--rw-r--r--   0        0        0    41350 2024-04-25 22:42:45.646479 schematicpy-24.4.1/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    20658 1970-01-01 00:00:00.000000 schematicpy-24.4.1/setup.py
--rw-r--r--   0        0        0    20649 1970-01-01 00:00:00.000000 schematicpy-24.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-10 17:57:35.038196 schematicpy-25.5.1/LICENSE
+-rw-r--r--   0        0        0    18039 2024-05-10 17:57:35.038196 schematicpy-25.5.1/README.md
+-rw-r--r--   0        0        0     4129 2024-05-10 17:59:00.766886 schematicpy-25.5.1/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-10 17:57:35.038196 schematicpy-25.5.1/schematic/__init__.py
+-rw-r--r--   0        0        0     1296 2024-05-10 17:57:35.038196 schematicpy-25.5.1/schematic/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-10 17:57:35.038196 schematicpy-25.5.1/schematic/configuration/__init__.py
+-rw-r--r--   0        0        0     7438 2024-05-10 17:57:35.038196 schematicpy-25.5.1/schematic/configuration/configuration.py
+-rw-r--r--   0        0        0     5034 2024-05-10 17:57:35.038196 schematicpy-25.5.1/schematic/configuration/dataclasses.py
+-rw-r--r--   0        0        0      663 2024-05-10 17:57:35.038196 schematicpy-25.5.1/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2024-05-10 17:57:35.042196 schematicpy-25.5.1/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3193 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/exceptions.py
+-rw-r--r--   0        0        0    12587 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/help.py
+-rw-r--r--   0        0        0     3415 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/loader.py
+-rw-r--r--   0        0        0       59 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0    11844 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    89173 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    23370 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/models/__init__.py
+-rw-r--r--   0        0        0     8057 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/models/commands.py
+-rw-r--r--   0        0        0    19316 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/models/metadata.py
+-rw-r--r--   0        0        0    83577 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    14470 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      515 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     5037 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     6100 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_edges.py
+-rw-r--r--   0        0        0    36064 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_graph.py
+-rw-r--r--   0        0        0    18286 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_json_schema.py
+-rw-r--r--   0        0        0    22845 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_jsonld.py
+-rw-r--r--   0        0        0    13333 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_nodes.py
+-rw-r--r--   0        0        0    24666 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_parser.py
+-rw-r--r--   0        0        0     9597 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_relationships.py
+-rw-r--r--   0        0        0     7617 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/data_model_validator.py
+-rw-r--r--   0        0        0     6974 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/schemas/json_schema_validator.py
+-rw-r--r--   0        0        0       96 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2024-05-10 17:57:35.046196 schematicpy-25.5.1/schematic/store/base.py
+-rw-r--r--   0        0        0   122222 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/store/synapse.py
+-rw-r--r--   0        0        0        0 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     2936 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     3027 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0    10358 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0    10288 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/general.py
+-rw-r--r--   0        0        0     6086 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1221 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0    18045 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0    11265 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     9178 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      724 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/version.py
+-rw-r--r--   0        0        0      164 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    12584 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     5809 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    41350 2024-05-10 17:57:35.050196 schematicpy-25.5.1/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    20658 1970-01-01 00:00:00.000000 schematicpy-25.5.1/setup.py
+-rw-r--r--   0        0        0    20649 1970-01-01 00:00:00.000000 schematicpy-25.5.1/PKG-INFO
```

### Comparing `schematicpy-24.4.1/LICENSE` & `schematicpy-25.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/README.md` & `schematicpy-25.5.1/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/pyproject.toml` & `schematicpy-25.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v24.4.1"
+version = "v25.5.1"
 description = "Package for biomedical data model and metadata ingress management"
 authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
```

### Comparing `schematicpy-24.4.1/schematic/__main__.py` & `schematicpy-25.5.1/schematic/__main__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/configuration/configuration.py` & `schematicpy-25.5.1/schematic/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/configuration/dataclasses.py` & `schematicpy-25.5.1/schematic/configuration/dataclasses.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/etc/README.md` & `schematicpy-25.5.1/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-25.5.1/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-25.5.1/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-25.5.1/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-25.5.1/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-25.5.1/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/exceptions.py` & `schematicpy-25.5.1/schematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/help.py` & `schematicpy-25.5.1/schematic/help.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/loader.py` & `schematicpy-25.5.1/schematic/loader.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/manifest/commands.py` & `schematicpy-25.5.1/schematic/manifest/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/manifest/generator.py` & `schematicpy-25.5.1/schematic/manifest/generator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/models/GE_Helpers.py` & `schematicpy-25.5.1/schematic/models/GE_Helpers.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/models/commands.py` & `schematicpy-25.5.1/schematic/models/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/models/metadata.py` & `schematicpy-25.5.1/schematic/models/metadata.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/models/validate_attribute.py` & `schematicpy-25.5.1/schematic/models/validate_attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from schematic.utils.validate_rules_utils import validation_rule_info
 from schematic.utils.validate_utils import (
     comma_separated_list_regex,
     parse_str_series_to_list,
     np_array_to_str_list,
     iterable_to_str_list,
     rule_in_rule_list,
+    get_list_robustness,
 )
 
 from synapseclient.core.exceptions import SynapseNoCredentialsError
 
 logger = logging.getLogger(__name__)
 
 MessageLevelType = Literal["warning", "error"]
@@ -54,14 +55,15 @@
         error_list, warning_list = GenerateError.raise_and_store_message(
             dmge=dmge,
             val_rule="schema",
             error_row=row_num,
             error_col=attribute_name,
             error_message=error_message,
             error_val=invalid_entry,
+            message_level="error",
         )
 
         return error_list, warning_list
 
     def generate_list_error(
         list_string: str,
         row_num: str,
@@ -471,15 +473,20 @@
         specified_level = rule_parts[-1].lower()
         specified_level = (
             specified_level if specified_level in ["warning", "error"] else None
         )
 
         is_schema_error = rule_name == "schema"
         col_is_recommended = rule_name == "recommended"
-        col_is_required = dmge.get_node_required(node_display_name=error_col_name)
+
+        if not is_schema_error:
+            col_is_required = dmge.get_node_required(node_display_name=error_col_name)
+        else:
+            col_is_required = False
+
         return (
             rule_parts,
             rule_name,
             specified_level,
             is_schema_error,
             col_is_recommended,
             col_is_required,
@@ -819,24 +826,25 @@
         """
 
         # For each 'list' (input as a string with a , delimiter) entered,
         # convert to a real list of strings, with leading and trailing
         # white spaces removed.
         errors = []
         warnings = []
+        replace_null = True
 
         csv_re = comma_separated_list_regex()
 
-        rule_parts = val_rule.lower().split(" ")
-        if len(rule_parts) > 1:
-            list_robustness = rule_parts[1]
-        else:
-            list_robustness = "strict"
+        # Check if lists -must- be a list, or can be a single value.
+        list_robustness = get_list_robustness(val_rule=val_rule)
+
+        if list_robustness == "like":
+            replace_null = False
 
-        if list_robustness == "strict":
+        elif list_robustness == "strict":
             manifest_col = manifest_col.astype(str)
 
             # This will capture any if an entry is not formatted properly. Only for strict lists
             for i, list_string in enumerate(manifest_col):
                 list_error = None
                 entry_has_value = self.get_entry_has_value(
                     entry=list_string,
@@ -860,15 +868,15 @@
                     )
                     if vr_errors:
                         errors.append(vr_errors)
                     if vr_warnings:
                         warnings.append(vr_warnings)
 
         # Convert string to list.
-        manifest_col = parse_str_series_to_list(manifest_col)
+        manifest_col = parse_str_series_to_list(manifest_col, replace_null=replace_null)
 
         return errors, warnings, manifest_col
 
     def regex_validation(
         self,
         val_rule: str,
         manifest_col: pd.core.series.Series,
```

### Comparing `schematicpy-24.4.1/schematic/models/validate_manifest.py` & `schematicpy-25.5.1/schematic/models/validate_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 
 from schematic.models.validate_attribute import ValidateAttribute, GenerateError
 
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 from schematic.store.synapse import SynapseStorage
 from schematic.models.GE_Helpers import GreatExpectationsHelpers
 from schematic.utils.validate_rules_utils import validation_rule_info
-from schematic.utils.validate_utils import rule_in_rule_list
+from schematic.utils.validate_utils import (
+    rule_in_rule_list,
+    convert_nan_entries_to_empty_strings,
+)
 from schematic.utils.schema_utils import extract_component_validation_rules
 
 logger = logging.getLogger(__name__)
 
 
 class ValidateManifest(object):
     def __init__(self, errors, manifest, manifestPath, dmge, jsonSchema):
@@ -99,17 +102,17 @@
         return errors
 
     def validate_manifest_rules(
         self,
         manifest: pd.core.frame.DataFrame,
         dmge: DataModelGraphExplorer,
         restrict_rules: bool,
-        project_scope: List,
+        project_scope: list[str],
         access_token: Optional[str] = None,
-    ) -> (pd.core.frame.DataFrame, List[List[str]]):
+    ) -> (pd.core.frame.DataFrame, list[list[str]]):
         """
         Purpose:
             Take validation rules set for a particular attribute
             and validate manifest entries based on these rules.
         Input:
             manifest: pd.core.frame.DataFrame
                 imported from models/metadata.py
@@ -291,16 +294,15 @@
     ) -> (List[List[str]], List[List[str]]):
         t_json_schema = perf_counter()
 
         errors = []
         warnings = []
         col_attr = {}  # save the mapping between column index and attribute name
 
-        # Replace nans with empty strings so jsonschema
-        manifest = manifest.replace({np.nan: ""})
+        manifest = convert_nan_entries_to_empty_strings(manifest=manifest)
 
         # numerical values need to be type string for the jsonValidator
         for col in manifest.select_dtypes(
             include=[int, np.int64, float, np.float64]
         ).columns:
             manifest[col] = manifest[col].astype("string")
         manifest = manifest.map(
@@ -343,23 +345,26 @@
     manifestPath,
     dmge,
     jsonSchema,
     restrict_rules,
     project_scope: List,
     access_token: str,
 ):
+    # Run Validation Rules
     vm = ValidateManifest(errors, manifest, manifestPath, dmge, jsonSchema)
     manifest, vmr_errors, vmr_warnings = vm.validate_manifest_rules(
         manifest, dmge, restrict_rules, project_scope, access_token
     )
+
     if vmr_errors:
         errors.extend(vmr_errors)
     if vmr_warnings:
         warnings.extend(vmr_warnings)
 
+    # Run JSON Schema Validation
     vmv_errors, vmv_warnings = vm.validate_manifest_values(manifest, jsonSchema, dmge)
     if vmv_errors:
         errors.extend(vmv_errors)
     if vmv_warnings:
         warnings.extend(vmv_warnings)
 
     return errors, warnings, manifest
```

### Comparing `schematicpy-24.4.1/schematic/schemas/__init__.py` & `schematicpy-25.5.1/schematic/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/commands.py` & `schematicpy-25.5.1/schematic/schemas/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_edges.py` & `schematicpy-25.5.1/schematic/schemas/data_model_edges.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_graph.py` & `schematicpy-25.5.1/schematic/schemas/data_model_graph.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_json_schema.py` & `schematicpy-25.5.1/schematic/schemas/data_model_json_schema.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_jsonld.py` & `schematicpy-25.5.1/schematic/schemas/data_model_jsonld.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_nodes.py` & `schematicpy-25.5.1/schematic/schemas/data_model_nodes.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_parser.py` & `schematicpy-25.5.1/schematic/schemas/data_model_parser.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_relationships.py` & `schematicpy-25.5.1/schematic/schemas/data_model_relationships.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/data_model_validator.py` & `schematicpy-25.5.1/schematic/schemas/data_model_validator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/schemas/json_schema_validator.py` & `schematicpy-25.5.1/schematic/schemas/json_schema_validator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/store/synapse.py` & `schematicpy-25.5.1/schematic/store/synapse.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/cli_utils.py` & `schematicpy-25.5.1/schematic/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/curie_utils.py` & `schematicpy-25.5.1/schematic/utils/curie_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/df_utils.py` & `schematicpy-25.5.1/schematic/utils/df_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/general.py` & `schematicpy-25.5.1/schematic/utils/general.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/google_api_utils.py` & `schematicpy-25.5.1/schematic/utils/google_api_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/io_utils.py` & `schematicpy-25.5.1/schematic/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/schema_utils.py` & `schematicpy-25.5.1/schematic/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/validate_rules_utils.py` & `schematicpy-25.5.1/schematic/utils/validate_rules_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/utils/validate_utils.py` & `schematicpy-25.5.1/schematic/utils/validate_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,14 +50,41 @@
         Pattern[str]:
     """
     csv_list_regex = re.compile("([^\,]+\,)(([^\,]+\,?)*)")
 
     return csv_list_regex
 
 
+def convert_nan_entries_to_empty_strings(
+    manifest: pd.core.frame.DataFrame,
+) -> pd.core.frame.DataFrame:
+    """
+    Nans need to be converted to empty strings for JSON Schema Validation. This helper
+    converts an a list with a single '<NA>' string or a single np.nan to empty strings.
+    These types of expected NANs come from different stages of conversion during import
+    and validation.
+
+    Args:
+        manifest: pd.core.frame.DataFrame, manifest prior to removing nans and
+            replacing with empty strings.
+    Returns:
+        manifest: pd.core.frame.DataFrame, manifest post removing nans and
+            replacing with empty strings.
+    """
+    # Replace nans with empty strings so jsonschema, address replace type infering depreciation.
+    with pd.option_context("future.no_silent_downcasting", True):
+        manifest = manifest.replace({np.nan: ""}).infer_objects(copy=False)  # type: ignore
+
+    for col in manifest.columns:
+        for index, value in manifest[col].items():
+            if value == ["<NA>"]:
+                manifest.loc[index, col] = [""]  # type: ignore
+    return manifest
+
+
 def rule_in_rule_list(rule: str, rule_list: list[str]) -> Optional[re.Match[str]]:
     """
     Function to standardize
     checking to see if a rule is contained in a list of rules.
     Uses regex to avoid issues arising from validation rules with arguments
     or rules that have arguments updated.
     """
@@ -66,26 +93,70 @@
 
     # Process string and list of strings for regex comparison
     rule_type = rule_type + "[^\|]*"
     rule_list_str = "|".join(rule_list)
     return re.search(rule_type, rule_list_str, flags=re.IGNORECASE)
 
 
-def parse_str_series_to_list(col: pd.Series) -> pd.Series:
+def get_list_robustness(val_rule: str) -> str:
+    """Helper function to extract list robustness from the validation rule.
+    List robustness defines if the input -must- be a list (several values
+    or a single value with a trailing comma),
+    or if a user is allowed to submit a single value.
+    List rules default to `strict` if not defined to be `like`
+    Args:
+        val_rule: str, validation rule string.
+    Returns:
+        list_robutness: str, list robustness extracted from validation rule.
+    """
+    list_robustness_options = ["like", "strict"]
+    list_robustness = None
+    default_robustness = list_robustness_options[1]
+
+    # Get the parts of a single rule, list is assumed to be in the first position, based on
+    # requirements that can be found in documentation.
+    rule_parts = val_rule.lower().split(" ")
+
+    if len(rule_parts) > 1:
+        # Check if list_robustness is defined in the rule, if not give them the default.
+        list_robustness_list = [
+            part for part in rule_parts if part in list_robustness_options
+        ]
+        if list_robustness_list:
+            list_robustness = list_robustness_list[0]
+
+    if not list_robustness:
+        # If no robustness has been defined by the user, set to the default.
+        list_robustness = default_robustness
+    return list_robustness
+
+
+def parse_str_series_to_list(col: pd.Series, replace_null: bool = True) -> pd.Series:
     """
     Parse a pandas series of comma delimited strings
-    into a series with values that are lists of strings
+    into a series with values that are lists of strings. If replace_null, fill null values
+    with nan. If the type of the value needs to be an array, fill with empty list.
     ex.
         Input:  'a,b,c'
         Output: ['a','b','c']
 
     """
-    col = col.apply(
-        lambda x: [s.strip() for s in str(x).split(",")] if not pd.isnull(x) else pd.NA
-    )
+    if replace_null:
+        col = col.apply(
+            lambda x: [s.strip() for s in str(x).split(",")]
+            if not pd.isnull(x)
+            else pd.NA
+        )
+    else:
+        col = col.apply(
+            lambda x: [s.strip() for s in str(x).split(",")]
+            if (isinstance(x, np.ndarray) and not x.any()) or not pd.isnull(x)
+            else []
+        )
+
     return col
 
 
 def np_array_to_str_list(np_array: Any) -> list[str]:
     """
     Parse a numpy array of ints to a list of strings
     """
```

### Comparing `schematicpy-24.4.1/schematic/utils/viz_utils.py` & `schematicpy-25.5.1/schematic/utils/viz_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/visualization/attributes_explorer.py` & `schematicpy-25.5.1/schematic/visualization/attributes_explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/visualization/commands.py` & `schematicpy-25.5.1/schematic/visualization/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/schematic/visualization/tangled_tree.py` & `schematicpy-25.5.1/schematic/visualization/tangled_tree.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.4.1/setup.py` & `schematicpy-25.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
  'aws': ['uWSGI>=2.0.21,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['schematic = schematic.__main__:main']}
 
 setup_kwargs = {
     'name': 'schematicpy',
-    'version': '24.4.1',
+    'version': '25.5.1',
     'description': 'Package for biomedical data model and metadata ingress management',
     'long_description': '# Schematic\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)\n\n# Table of contents\n- [Introduction](#introduction)\n- [Installation](#installation)\n  - [Installation Requirements](#installation-requirements)\n  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)\n  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)\n- [Other Contribution Guidelines](#other-contribution-guidelines)\n    - [Update readthedocs documentation](#update-readthedocs-documentation)\n- [Command Line Usage](#command-line-usage)\n- [Testing](#testing)\n  - [Updating Synapse test resources](#updating-synapse-test-resources)\n- [Code Style](#code-style)\n- [Contributors](#contributors)\n\n# Introduction\nSCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.\n\n# Installation\n## Installation Requirements\n* Python version 3.9.0≤x<3.11.0\n* You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/)\n\nNote: Our credential policy for Google credentials in order to create Google sheet files from Schematic, see tutorial [\'HERE\'](https://scribehow.com/shared/Get_Credentials_for_Google_Drive_and_Google_Sheets_APIs_to_use_with_schematicpy__yqfcJz_rQVeyTcg0KQCINA). If you plan to use `config.yml`, please ensure that the path of `schematic_service_account_creds.json` is indicated there (see `google_sheets > service_account_creds` section)\n\n\n## Installation guide for data curator app\n\nCreate and activate a virtual environment within which you can install the package:\n\n```\npython3 -m venv .venv\nsource .venv/bin/activate\n```\n\nNote: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.\n\nInstall and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):\n\n```\npython3 -m pip install schematicpy\n```\n\nIf you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:\n\n```\npip3 install --upgrade pip\n```\n\n## Installation guide for developers/contributors \n\nWhen contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.\n\nPlease note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.\n\n### Development environment setup\n1. Clone the `schematic` package repository.\n```\ngit clone https://github.com/Sage-Bionetworks/schematic.git\n```\n2. Install `poetry` (version 1.3.0 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. \n\n3. Start the virtual environment by doing: \n```\npoetry shell\n```\n4. Install the dependencies by doing: \n```\npoetry install\n```\nThis command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)\n\nIf you want to install the API you will need to install those dependencies as well:\n\n```\npoetry install --extras "api"\n```\n\nIf you want to install the uwsgi:\n\n```\npoetry install --extras "api"\n```\n\n5. Fill in credential files: \n*Note*: If you won\'t interact with Synapse, please ignore this section.\n\nThere are two main configuration files that need to be edited:\nconfig.yml\nand [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)\n\n<strong>Configure .synapseConfig File</strong>\n\nDownload a copy of the ``.synapseConfig`` file, open the file in the\neditor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section \n\n*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:\n>[authentication]<br> username = ABC <br> authtoken = abc\n\n<strong>Configure config.yml File</strong>\n\nThere are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:\n\n```text\n\n# This is an example config for Schematic.\n# All listed values are those that are the default if a config is not used.\n# Save this as config.yml, this will be gitignored.\n# Remove any fields in the config you don\'t want to change\n# Change the values of any fields you do want to change\n\n\n# This describes where assets such as manifests are stored\nasset_store:\n  # This is when assets are stored in a synapse project\n  synapse:\n    # Synapse ID of the file view listing all project data assets.\n    master_fileview_id: "syn23643253"\n    # Path to the synapse config file, either absolute or relative to this file\n    config: ".synapseConfig"\n    # Base name that manifest files will be saved as\n    manifest_basename: "synapse_storage_manifest"\n\n# This describes information about manifests as it relates to generation and validation\nmanifest:\n  # Location where manifests will saved to\n  manifest_folder: "manifests"\n  # Title or title prefix given to generated manifest(s)\n  title: "example"\n  # Data types of manifests to be generated or data type (singular) to validate manifest against\n  data_type:\n    - "Biospecimen"\n    - "Patient"\n\n# Describes the location of your schema\nmodel:\n  # Location of your schema jsonld, it must be a path relative to this file or absolute\n  location: "tests/data/example.model.jsonld"\n\n# This section is for using google sheets with Schematic\ngoogle_sheets:\n  # The Synapse id of the Google service account credentials.\n  service_acct_creds_synapse_id: "syn25171627"\n  # Path to the synapse config file, either absolute or relative to this file\n  service_acct_creds: "schematic_service_account_creds.json"\n  # When doing google sheet validation (regex match) with the validation rules.\n  #   true is alerting the user and not allowing entry of bad values.\n  #   false is warning but allowing the entry on to the sheet.\n  strict_validation: true\n```\n\nIf you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don\'t.\n\nFor example if you wanted to change the folder where manifests are downloaded your config should look like:\n\n```text\n\nmanifest:\n  manifest_folder: "my_manifest_folder_path"\n```\n\n_Note_: `config.yml` is ignored by git.\n\n_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.\n\n6. Login to Synapse by using the command line\nOn the CLI in your virtual environment, run the following command: \n```\nsynapse login -u <synapse username> -p <synapse password> --rememberMe\n```\n\n7. Obtain Google credential Files\nRunning `schematic init` is no longer supported due to security concerns. To obtain  `schematic_service_account_creds.json`, please follow the instructions [here](https://scribehow.com/shared/Enable_Google_Drive_and_Google_Sheets_APIs_for_project__yqfcJz_rQVeyTcg0KQCINA). \n\n> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google\'s decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. \n\n*Notes*: Use the ``schematic_service_account_creds.json`` file for the service\naccount mode of authentication (*for Google services/APIs*). Service accounts \nare special Google accounts that can be used by applications to access Google APIs \nprogrammatically via OAuth2.0, with the advantage being that they do not require \nhuman authorization. \n\n*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.\nMost Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality\nrequires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate\ntoken-based authentication and keep only service account authentication in the future. \n\n8. Set up pre-commit hooks\n\nThis repository is configured to utilize pre-commit hooks as part of the development process. To enable these hooks, please run the following command and look for the following success message:\n```\n$ pre-commit install\npre-commit installed at .git/hooks/pre-commit\n```\n\n### Development process instruction\n\nFor new features, bugs, enhancements\n\n1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)\n2. Checkout a new branch develop-<feature/fix-name> from the develop branch\n3. Do development on branch develop-<feature/fix-name>\n   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment\n4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)\n5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes\n6. Commits with work in progress are encouraged:\n   a. add WIP to the beginning of the commit message for “Work In Progress” commits\n7. Keep commit messages descriptive but less than a page long, see best practices\n8. Push code to develop-<feature/fix-name> in upstream repo\n9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base\n10. After feature work is complete and before creating a PR to the develop branch in upstream\n    a. ensure that code runs locally\n    b. test for logical correctness locally\n    c. wait for git workflow to complete (e.g. tests are run) on github\n11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo\n12. Request a code review on the PR\n13. Once code is approved merge in the develop branch\n14. Delete the develop-<feature/fix-name> branch\n\n*Note*: Make sure you have the latest version of the `develop` branch on your local machine.\n\n## Installation Guide - Docker \n\n1. Install docker from https://www.docker.com/ . <br>\n2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>\n    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>\n    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen\n3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>\n<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>\n<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>\n<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>\n<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>\n<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>\n\n### Example For REST API <br>\n\n#### Use file path of `config.yml` to run API endpoints: \n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: \n1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`\n\n2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`\n\n3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`\n\n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \\\n  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n\n### Example For Schematic on mac/linux <br>\nTo run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>\nThen update .synapseConfig with your credentials\n```\ndocker run \\\n  -v ~/schematic:/schematic \\\n  -w /schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic schematic model \\\n  -c /schematic/config.yml validate \\\n  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \\\n  -dt MockComponent \\\n  -js /schematic/tests/data/example.model.jsonld\n``` \n\n### Example For Schematic on Windows <br>\n```\ndocker run -v %cd%:/schematic \\\n  -w /schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  schematic model \\\n  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld\n```\n\n# Other Contribution Guidelines\n## Updating readthedocs documentation\n1. `cd docs`\n2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.\n3. Please contact the dev team to publish your updates\n\n*Other helpful resources*:\n\n1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n\n## Update toml file and lock file\nIf you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.\n\n## Reporting bugs or feature requests\nYou can **create bug and feature requests** through [Sage Bionetwork\'s FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:\n- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.\n- **Describe the exact steps which reproduce the problem** in as many details as possible.\n- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.\n- **Explain which behavior you expected to see** instead and why.\n- **Provide screenshots of the expected or actual behaviour** where applicable.\n\n# Command Line Usage\nPlease visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)\n\n\n\n# Testing \n\nAll code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.\n\nYou can run the test suite in the following way:\n\n```\npytest -vs tests/\n```\n\n## Updating Synapse test resources\n\n1. Duplicate the entity being updated (or folder if applicable).\n2. Edit the duplicates (_e.g._ annotations, contents, name).\n3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.\n4. Open a PR as per the usual process (see above).\n5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.\n   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.\n\n# Code style\n\n* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.\n* Be consistent and follow existing code conventions and spirit.\n\n\n# Contributors\n\nMain contributors and developers:\n\n- [Milen Nikolov](https://github.com/milen-sage)\n- [Mialy DeFelice](https://github.com/mialy-defelice)\n- [Sujay Patil](https://github.com/sujaypatil96)\n- [Bruno Grande](https://github.com/BrunoGrandePhD)\n- [Robert Allaway](https://github.com/allaway)\n- [Gianna Jordan](https://github.com/giajordan)\n- [Lingling Peng](https://github.com/linglp)\n',
     'author': 'Milen Nikolov',
     'author_email': 'milen.nikolov@sagebase.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Sage-Bionetworks/schematic',
```

### Comparing `schematicpy-24.4.1/PKG-INFO` & `schematicpy-25.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schematicpy
-Version: 24.4.1
+Version: 25.5.1
 Summary: Package for biomedical data model and metadata ingress management
 Home-page: https://github.com/Sage-Bionetworks/schematic
 Keywords: schema,metadata,validation,data model,linked data
 Author: Milen Nikolov
 Author-email: milen.nikolov@sagebase.org
 Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 4 - Beta
```

