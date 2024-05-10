# Comparing `tmp/fiddler_client-3.2.0.dev1.tar.gz` & `tmp/fiddler_client-3.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler_client-3.2.0.dev1.tar", last modified: Wed May  8 14:30:18 2024, max compression
+gzip compressed data, was "fiddler_client-3.2.0.dev2.tar", last modified: Fri May 10 11:15:10 2024, max compression
```

## Comparing `fiddler_client-3.2.0.dev1.tar` & `fiddler_client-3.2.0.dev2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.488660 fiddler_client-3.2.0.dev1/
--rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)     1549 2024-05-08 14:30:18.488660 fiddler_client-3.2.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/PUBLIC.md
--rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.458657 fiddler_client-3.2.0.dev1/fiddler/
--rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/VERSION
--rw-r--r--   0 runner    (1001) runner    (1001)     3824 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/configs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/connection.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.468658 fiddler_client-3.2.0.dev1/fiddler/constants/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/common.py
--rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/constants/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/decorators.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.468658 fiddler_client-3.2.0.dev1/fiddler/entities/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11744 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5383 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19271 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3966 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4514 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/entities/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.468658 fiddler_client-3.2.0.dev1/fiddler/libs/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/libs/json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/libs/semver.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.468658 fiddler_client-3.2.0.dev1/fiddler/packtools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10484 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/packtools/template_model.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.478659 fiddler_client-3.2.0.dev1/fiddler/schemas/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1387 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      953 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/filter_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/server_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/schemas/xai_params.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.478659 fiddler_client-3.2.0.dev1/fiddler/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.478659 fiddler_client-3.2.0.dev1/fiddler/tests/apis/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13196 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_files.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_generate_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_mixin.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18779 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3350 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model_surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_segment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8099 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/conftest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/test_connection.py
--rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/test_logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/tests/utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.478659 fiddler_client-3.2.0.dev1/fiddler/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/utils/model_generator.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/utils/version.py
--rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/fiddler/version.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-08 14:30:18.488660 fiddler_client-3.2.0.dev1/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1549 2024-05-08 14:30:18.000000 fiddler_client-3.2.0.dev1/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-05-08 14:30:18.000000 fiddler_client-3.2.0.dev1/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-08 14:30:18.000000 fiddler_client-3.2.0.dev1/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-05-08 14:30:18.000000 fiddler_client-3.2.0.dev1/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-05-08 14:30:18.000000 fiddler_client-3.2.0.dev1/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-08 14:30:18.488660 fiddler_client-3.2.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-05-08 14:30:12.000000 fiddler_client-3.2.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.874448 fiddler_client-3.2.0.dev2/
+-rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)     1594 2024-05-10 11:15:10.874448 fiddler_client-3.2.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/PUBLIC.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.844446 fiddler_client-3.2.0.dev2/fiddler/
+-rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-05-10 11:15:05.000000 fiddler_client-3.2.0.dev2/fiddler/VERSION
+-rw-r--r--   0 runner    (1001) runner    (1001)     3824 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/configs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/connection.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.844446 fiddler_client-3.2.0.dev2/fiddler/constants/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/common.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/constants/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/decorators.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.844446 fiddler_client-3.2.0.dev2/fiddler/entities/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11744 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5383 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19271 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3966 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4514 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/entities/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.854447 fiddler_client-3.2.0.dev2/fiddler/libs/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/libs/json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/libs/semver.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.854447 fiddler_client-3.2.0.dev2/fiddler/packtools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10484 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/packtools/template_model.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.854447 fiddler_client-3.2.0.dev2/fiddler/schemas/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1387 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      953 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/filter_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/server_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/schemas/xai_params.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.854447 fiddler_client-3.2.0.dev2/fiddler/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.874448 fiddler_client-3.2.0.dev2/fiddler/tests/apis/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13196 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_files.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_generate_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_mixin.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18779 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3350 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model_surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_segment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8099 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/tests/utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.874448 fiddler_client-3.2.0.dev2/fiddler/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/utils/model_generator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/utils/version.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/fiddler/version.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-10 11:15:10.874448 fiddler_client-3.2.0.dev2/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1594 2024-05-10 11:15:10.000000 fiddler_client-3.2.0.dev2/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-05-10 11:15:10.000000 fiddler_client-3.2.0.dev2/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-10 11:15:10.000000 fiddler_client-3.2.0.dev2/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      167 2024-05-10 11:15:10.000000 fiddler_client-3.2.0.dev2/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-05-10 11:15:10.000000 fiddler_client-3.2.0.dev2/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-10 11:15:10.874448 fiddler_client-3.2.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1143 2024-05-10 11:15:04.000000 fiddler_client-3.2.0.dev2/setup.py
```

### Comparing `fiddler_client-3.2.0.dev1/LICENSE.txt` & `fiddler_client-3.2.0.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/PKG-INFO` & `fiddler_client-3.2.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.2.0.dev1
+Version: 3.2.0.dev2
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pip>=21.0
 Requires-Dist: requests<3
 Requires-Dist: requests-toolbelt
 Requires-Dist: pandas>=1.2.5
-Requires-Dist: pydantic<2,>=1.9.0
+Requires-Dist: pydantic<2,>=1.10.15
 Requires-Dist: deprecated==1.2.13
 Requires-Dist: tqdm
 Requires-Dist: simplejson>=3.17.0
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pyyaml
+Requires-Dist: typing-extensions<5,>=4.6.0
 
 Fiddler Client
 =============
 
 Python client for interacting with Fiddler. Provides a user-friendly interface to our REST API and enables event
 publishing for use with our monitoring features.
```

### Comparing `fiddler_client-3.2.0.dev1/PUBLIC.md` & `fiddler_client-3.2.0.dev2/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/README.md` & `fiddler_client-3.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/__init__.py` & `fiddler_client-3.2.0.dev2/fiddler/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/connection.py` & `fiddler_client-3.2.0.dev2/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/constants/alert_rule.py` & `fiddler_client-3.2.0.dev2/fiddler/constants/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/constants/model.py` & `fiddler_client-3.2.0.dev2/fiddler/constants/model.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/decorators.py` & `fiddler_client-3.2.0.dev2/fiddler/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/alert_record.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/alert_rule.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/base.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/base.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/baseline.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/custom_expression.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/dataset.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/events.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/events.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/file.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/file.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/job.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/job.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/model.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/model.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/model_artifact.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/model_deployment.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/organization.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/organization.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/project.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/project.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/surrogate.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/user.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/user.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/webhook.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/entities/xai.py` & `fiddler_client-3.2.0.dev2/fiddler/entities/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/exceptions.py` & `fiddler_client-3.2.0.dev2/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/libs/http_client.py` & `fiddler_client-3.2.0.dev2/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/libs/json_encoder.py` & `fiddler_client-3.2.0.dev2/fiddler/libs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/libs/semver.py` & `fiddler_client-3.2.0.dev2/fiddler/libs/semver.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/packtools/gem.py` & `fiddler_client-3.2.0.dev2/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/packtools/keras_ig_helpers.py` & `fiddler_client-3.2.0.dev2/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/packtools/project_attributions_helpers.py` & `fiddler_client-3.2.0.dev2/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/packtools/template_model.py` & `fiddler_client-3.2.0.dev2/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/alert_record.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/alert_rule.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/baseline.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/custom_expression.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/custom_features.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/dataset.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/filter_query.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/filter_query.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/model.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/model.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/model_deployment.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/model_schema.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/model_spec.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/model_task_params.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/response.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/response.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/schemas/xai.py` & `fiddler_client-3.2.0.dev2/fiddler/schemas/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_alert_record.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_alert_rule.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_baseline.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_custom_metric.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_custom_metric.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_dataset.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_events.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_events.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_files.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_files.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_generate_model.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_generate_model.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_job.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_mixin.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model_artifact.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model_deployment.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_model_surrogate.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_model_surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_project.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_segment.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_segment.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_webhook.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/apis/test_xai.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/apis/test_xai.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/conftest.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/constants.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/test_connection.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/test_json_encoder.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/tests/test_utils.py` & `fiddler_client-3.2.0.dev2/fiddler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/utils/helpers.py` & `fiddler_client-3.2.0.dev2/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/utils/logger.py` & `fiddler_client-3.2.0.dev2/fiddler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/utils/model_generator.py` & `fiddler_client-3.2.0.dev2/fiddler/utils/model_generator.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler/utils/version.py` & `fiddler_client-3.2.0.dev2/fiddler/utils/version.py`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/fiddler_client.egg-info/PKG-INFO` & `fiddler_client-3.2.0.dev2/fiddler_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.2.0.dev1
+Version: 3.2.0.dev2
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pip>=21.0
 Requires-Dist: requests<3
 Requires-Dist: requests-toolbelt
 Requires-Dist: pandas>=1.2.5
-Requires-Dist: pydantic<2,>=1.9.0
+Requires-Dist: pydantic<2,>=1.10.15
 Requires-Dist: deprecated==1.2.13
 Requires-Dist: tqdm
 Requires-Dist: simplejson>=3.17.0
 Requires-Dist: pyarrow>=7.0.0
 Requires-Dist: pyyaml
+Requires-Dist: typing-extensions<5,>=4.6.0
 
 Fiddler Client
 =============
 
 Python client for interacting with Fiddler. Provides a user-friendly interface to our REST API and enables event
 publishing for use with our monitoring features.
```

### Comparing `fiddler_client-3.2.0.dev1/fiddler_client.egg-info/SOURCES.txt` & `fiddler_client-3.2.0.dev2/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler_client-3.2.0.dev1/setup.py` & `fiddler_client-3.2.0.dev2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,21 @@
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
         'pip>=21.0',
         'requests<3',
         'requests-toolbelt',
         'pandas>=1.2.5',
-        'pydantic>=1.9.0,<2',
+        'pydantic>=1.10.15,<2',
         'deprecated==1.2.13',
         'tqdm',
         'simplejson>=3.17.0',
         'pyarrow>=7.0.0',
         'pyyaml',
+        'typing-extensions>=4.6.0,<5',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     python_requires='>3.8.0',
```

