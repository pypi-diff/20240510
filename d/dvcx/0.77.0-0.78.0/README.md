# Comparing `tmp/dvcx-0.77.0.tar.gz` & `tmp/dvcx-0.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.77.0.tar", last modified: Tue May  7 22:04:32 2024, max compression
+gzip compressed data, was "dvcx-0.78.0.tar", last modified: Thu May  9 02:47:16 2024, max compression
```

## Comparing `dvcx-0.77.0.tar` & `dvcx-0.78.0.tar`

### file list

```diff
@@ -1,247 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.505053 dvcx-0.77.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 22:04:27.000000 dvcx-0.77.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 22:04:27.000000 dvcx-0.77.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.457053 dvcx-0.77.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.457053 dvcx-0.77.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-07 22:04:27.000000 dvcx-0.77.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 22:04:27.000000 dvcx-0.77.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 22:04:27.000000 dvcx-0.77.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 22:04:27.000000 dvcx-0.77.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-07 22:04:27.000000 dvcx-0.77.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-07 22:04:27.000000 dvcx-0.77.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-07 22:04:32.505053 dvcx-0.77.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-07 22:04:27.000000 dvcx-0.77.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-07 22:04:27.000000 dvcx-0.77.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-07 22:04:27.000000 dvcx-0.77.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-07 22:04:27.000000 dvcx-0.77.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:04:32.505053 dvcx-0.77.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.453053 dvcx-0.77.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.469053 dvcx-0.77.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.473053 dvcx-0.77.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72292 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.473053 dvcx-0.77.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.473053 dvcx-0.77.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45366 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30660 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    34621 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15901 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.477053 dvcx-0.77.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    60425 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.485053 dvcx-0.77.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.485053 dvcx-0.77.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.485053 dvcx-0.77.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14464 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.489053 dvcx-0.77.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113295 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26682 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.489053 dvcx-0.77.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.493053 dvcx-0.77.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.151313 dvcx-0.78.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-09 02:47:11.000000 dvcx-0.78.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 02:47:11.000000 dvcx-0.78.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.103313 dvcx-0.78.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.103313 dvcx-0.78.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.103313 dvcx-0.78.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-09 02:47:11.000000 dvcx-0.78.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-09 02:47:11.000000 dvcx-0.78.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-09 02:47:11.000000 dvcx-0.78.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.103313 dvcx-0.78.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-09 02:47:11.000000 dvcx-0.78.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-09 02:47:11.000000 dvcx-0.78.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-09 02:47:11.000000 dvcx-0.78.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-09 02:47:11.000000 dvcx-0.78.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-09 02:47:11.000000 dvcx-0.78.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.103313 dvcx-0.78.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 02:47:11.000000 dvcx-0.78.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-09 02:47:11.000000 dvcx-0.78.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-09 02:47:11.000000 dvcx-0.78.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-09 02:47:16.151313 dvcx-0.78.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-09 02:47:11.000000 dvcx-0.78.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.103313 dvcx-0.78.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-09 02:47:11.000000 dvcx-0.78.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.107313 dvcx-0.78.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.107313 dvcx-0.78.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.111312 dvcx-0.78.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.111312 dvcx-0.78.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-09 02:47:11.000000 dvcx-0.78.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-09 02:47:11.000000 dvcx-0.78.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-09 02:47:11.000000 dvcx-0.78.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 02:47:16.151313 dvcx-0.78.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.099312 dvcx-0.78.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.115312 dvcx-0.78.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 02:47:15.000000 dvcx-0.78.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.115312 dvcx-0.78.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72305 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30873 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.115312 dvcx-0.78.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.119313 dvcx-0.78.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45621 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30778 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34860 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.123313 dvcx-0.78.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.127313 dvcx-0.78.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60133 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.127313 dvcx-0.78.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.127313 dvcx-0.78.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.127313 dvcx-0.78.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.127313 dvcx-0.78.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.131312 dvcx-0.78.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-09 02:47:11.000000 dvcx-0.78.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.139313 dvcx-0.78.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-09 02:47:16.000000 dvcx-0.78.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-09 02:47:16.000000 dvcx-0.78.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 02:47:16.000000 dvcx-0.78.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 02:47:16.000000 dvcx-0.78.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 02:47:16.000000 dvcx-0.78.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 02:47:16.000000 dvcx-0.78.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.131312 dvcx-0.78.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.131312 dvcx-0.78.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14464 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.135313 dvcx-0.78.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113295 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26674 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.135313 dvcx-0.78.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.139313 dvcx-0.78.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.139313 dvcx-0.78.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.139313 dvcx-0.78.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:47:16.139313 dvcx-0.78.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-09 02:47:11.000000 dvcx-0.78.0/tests/utils.py
```

### Comparing `dvcx-0.77.0/.cruft.json` & `dvcx-0.78.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.78.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.78.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.github/workflows/benchmarks.yml` & `dvcx-0.78.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.github/workflows/release.yml` & `dvcx-0.78.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.github/workflows/tests.yml` & `dvcx-0.78.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.gitignore` & `dvcx-0.78.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/.pre-commit-config.yaml` & `dvcx-0.78.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/CODE_OF_CONDUCT.rst` & `dvcx-0.78.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/CONTRIBUTING.rst` & `dvcx-0.78.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/LICENSE` & `dvcx-0.78.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/LICENSES/Apache-2.0.txt` & `dvcx-0.78.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.78.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/LICENSES/Python-2.0.txt` & `dvcx-0.78.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/PKG-INFO` & `dvcx-0.78.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.77.0
+Version: 0.78.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.77.0/README.rst` & `dvcx-0.78.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/docs/udfs.md` & `dvcx-0.78.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/blip2_image_desc_lib.py` & `dvcx-0.78.0/examples/blip2_image_desc_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     device = "cpu"
 
 
 if __name__ == "__main__":
     results = (
         DatasetQuery(
             source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("cat*.jpg"))
         .limit(5)
         .add_signals(
             BLIP2describe(
                 # device=device,
                 device="cpu",
```

### Comparing `dvcx-0.77.0/examples/clip.py` & `dvcx-0.78.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/common_sql_functions.py` & `dvcx-0.78.0/examples/common_sql_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return ([],)
 
 
 def show(dataset):
     print(*dataset.results(), sep="\n", end="\n\n")
 
 
-kw = {"client_config": {"aws_anon": True}}
+kw = {"client_config": {"anon": True}}
 ds = DatasetQuery("gcs://dvcx-datalakes/dogs-and-cats/", **kw)
 show(ds.limit(5).add_signals(num_chars_udf).select(C.name, C.num_chars))
 show(
     ds.limit(5).select(
         C.name,
         string.length(C.name),
         string.split(C.name, literal(".")),
```

### Comparing `dvcx-0.77.0/examples/dir_expansion.py` & `dvcx-0.78.0/examples/dir_expansion.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 if len(sys.argv) > 1:
     if sys.argv[1] == "--show-ids":
         show_ids = True
     else:
         raise RuntimeError(f"Invalid arg: {sys.argv[1]}")
 
 source = "gcs://dvcx-datasets"
-catalog = get_catalog(client_config={"aws_anon": True})
+catalog = get_catalog(client_config={"anon": True})
 metastore = catalog.metastore
 warehouse = catalog.warehouse
 
 try:
     dataset = metastore.get_dataset("ds1")
 except DatasetNotFoundError:
     DatasetQuery(source).save("ds1")
```

### Comparing `dvcx-0.77.0/examples/hf_pipeline.py` & `dvcx-0.78.0/examples/hf_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 if __name__ == "__main__":
     print("** HuggingFace pipeline helper model zoo demo **")
     print("\nZero-shot object detection and classification:")
     results = (
         DatasetQuery(
             image_source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("*.jpg"))
         .limit(1)
         .add_signals(
             ImageHelper(
                 model="google/owlv2-base-patch16",
                 device=device,
@@ -37,15 +37,15 @@
     )
     print(*results, sep="\n")
 
     print("\nNot-safe-for-work image detection:")
     results = (
         DatasetQuery(
             image_source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("*.jpg"))
         .limit(1)
         .add_signals(
             ImageHelper(
                 model="Falconsai/nsfw_image_detection",
                 device=device,
@@ -57,15 +57,15 @@
     )
     print(*results, sep="\n")
 
     print("\nAudio emotion classification:")
     results = (
         DatasetQuery(
             audio_source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("*.wav"))
         .limit(1)
         .add_signals(
             RawHelper(
                 model="Krithika-p/my_awesome_emotions_model",
                 device=device,
@@ -76,15 +76,15 @@
         .results()
     )
     print(*results, sep="\n")
     print("\nLong text summarization:")
     results = (
         DatasetQuery(
             text_source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("*.story"))
         .limit(1)
         .add_signals(
             TextHelper(
                 model="pszemraj/led-large-book-summary",
                 device=device,
```

### Comparing `dvcx-0.77.0/examples/llava2_image_desc_lib.py` & `dvcx-0.78.0/examples/llava2_image_desc_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 else:
     device = "cpu"
 
 if __name__ == "__main__":
     results = (
         DatasetQuery(
             source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("cat*.jpg"))
         .limit(2)
         .add_signals(
             LLaVAdescribe(
                 device=device,
                 model=model,
```

### Comparing `dvcx-0.77.0/examples/llm-claude-aggregate-query.py` & `dvcx-0.78.0/examples/llm-claude-aggregate-query.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 the user that such plan does not exist. The dialog is not successful if the \
 conversation ends early or the 'user' requests additional functions the 'bot' \
 cannot perform. Read the dialogues and classify them into a fixed number of concise \
 failure reasons covering most failure cases. Present output as JSON list of reason \
 strings and nothing else.
 """
 
-chats = Dataset(SOURCE, client_config={"aws_anon": True}).filter(C.name.glob("*.txt"))
+chats = Dataset(SOURCE, client_config={"anon": True}).filter(C.name.glob("*.txt"))
 
 content = chats.limit(50).aggregate(
     AggregateTextAnalytics(
         prompt=PROMPT,
         model_name=model,
         messages=[
             {
```

### Comparing `dvcx-0.77.0/examples/llm-claude-simple-query.py` & `dvcx-0.78.0/examples/llm-claude-simple-query.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 the 'bot' cannot perform. Read the dialogue below and rate it 'Success' \
 if it is successful, and 'Failure' if not. After that, provide \
 one-sentence explanation of the reasons for this rating. Use only \
 JSON object as output with the keys 'status', and 'explanation'.
 """
 
 chats = (
-    Dataset(SOURCE, client_config={"aws_anon": True})
-    .filter(C.name.glob("*.txt"))
-    .limit(5)
+    Dataset(SOURCE, client_config={"anon": True}).filter(C.name.glob("*.txt")).limit(5)
 )
 
 content = chats.map(
     TextAnalytics(
         prompt=PROMPT,
         model_name=model,
         temperature=0.9,
```

### Comparing `dvcx-0.77.0/examples/llm-claude.py` & `dvcx-0.78.0/examples/llm-claude.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dvcx.query.schema import C
 
 SOURCE = "s3://ldb-public/remote/chatbots-public/"
 MODEL = "claude-3-opus-20240229"
 PROMPT = """Summarise the dialog in a sentence"""
 
 ds = (
-    Dataset(SOURCE, client_config={"aws_anon": True})
+    Dataset(SOURCE, client_config={"anon": True})
     .filter(C.name.glob("*.txt"))
     .limit(5)
     .map(
         ClaudeMessage(
             prompt=PROMPT,
             model_name=MODEL,
             temperature=0.9,
```

### Comparing `dvcx-0.77.0/examples/loader.py` & `dvcx-0.78.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/neurips/README` & `dvcx-0.78.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/neurips/distance_to_query.py` & `dvcx-0.78.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/neurips/llm_chat.py` & `dvcx-0.78.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/neurips/single_query.py` & `dvcx-0.78.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/neurips/text_loaders.py` & `dvcx-0.78.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/openai_image_desc_lib.py` & `dvcx-0.78.0/examples/openai_image_desc_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 source = "gcs://dvcx-datalakes/dogs-and-cats/"
 
 if __name__ == "__main__":
     results = (
         DatasetQuery(
             source,
-            client_config={"aws_anon": True},
+            client_config={"anon": True},
         )
         .filter(C.name.glob("cat*.jpg"))
         .limit(10)
         .add_signals(
             DescribeImage(
                 key=OPENAI_API_KEY, max_tokens=300, prompt="What is in this image?"
             ),
```

### Comparing `dvcx-0.77.0/examples/openimage-detect.py` & `dvcx-0.78.0/examples/openimage-detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
             yield fstream, bbox
 
 
 source = "s3://ldb-public/remote/data-lakes/open-images-v6-test-200"
 
 ds = (
-    Dataset(source, client_config={"aws_anon": True})
+    Dataset(source, client_config={"anon": True})
     .filter(C.name.glob("*.jpg") | C.name.glob("*.json"))
     .aggregate(
         OpenImageDetect(),
         partition_by=path.file_stem(C.name),
     )
 )
```

### Comparing `dvcx-0.77.0/examples/pose_detection.py` & `dvcx-0.78.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/torch-loader.py` & `dvcx-0.78.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/udfs/batching.py` & `dvcx-0.78.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/udfs/image_transformation.py` & `dvcx-0.78.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/udfs/parallel.py` & `dvcx-0.78.0/examples/udfs/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,14 @@
     else:
         return (len(name),)
 
 
 # Save as a new dataset
 DatasetQuery(
     path="gcs://dvcx-datalakes/dogs-and-cats/",
-    client_config={"aws_anon": True},
+    client_config={"anon": True},
 ).filter(C.name.glob("*cat*")).add_signals(name_len_benchmark, parallel=-1).save(
     "cats_with_signal"
 )
 
 # Output the contents of the new dataset.
 print(tabulate(DatasetQuery(name="cats_with_signal").results()[:10]))
```

### Comparing `dvcx-0.77.0/examples/udfs/simple.py` & `dvcx-0.78.0/examples/udfs/simple.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if __name__ == "__main__":
     ds_name = uuid.uuid4().hex
     print(f"Saving to dataset: {ds_name}")
     # Save as a new dataset
     DatasetQuery(
         path="gcs://dvcx-datalakes/dogs-and-cats/",
-        client_config={"aws_anon": True},
+        client_config={"anon": True},
     ).filter(C.name.glob("*cat*")).add_signals(name_len).save(ds_name)
 
     # Output the contents of the new dataset.
     print(
         tabulate(
             DatasetQuery(name=ds_name)
             .order_by(C.parent, C.name)
```

### Comparing `dvcx-0.77.0/examples/udfs/stateful.py` & `dvcx-0.78.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/udfs/stateful_similarity.py` & `dvcx-0.78.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/unstructured-text.py` & `dvcx-0.78.0/examples/unstructured-text.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     summary = helper(clean, max_length=200)[0]["summary_text"]
     return (summary,)
 
 
 ds = (
     Dataset(
         source,
-        client_config={"aws_anon": True},
+        client_config={"anon": True},
     )
     .filter(C.name.glob("*.pdf"))
     .limit(1)
     .map(PartitionObject(), parallel=False)
 )
 
 ds = ds.map(cleanse, output={"clean": String})
```

### Comparing `dvcx-0.77.0/examples/wds.py` & `dvcx-0.78.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/wds_filtered.py` & `dvcx-0.78.0/examples/wds_filtered.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 name = "wds"
 wds = Dataset(name=name)
 try:
     df = wds.limit(3).to_pandas()
 except dvcx.error.DatasetNotFoundError:
     (
-        Dataset("gcs://dvcx-datacomp-small/shards", client_config={"aws_anon": True})
+        Dataset("gcs://dvcx-datacomp-small/shards", client_config={"anon": True})
         .filter(C.name.glob("00000000.tar"))
         .generate(WebDataset())
         .save(name)
     )
     df = wds.limit(3).to_pandas()
 
 print(df.columns.tolist())
```

### Comparing `dvcx-0.77.0/examples/wds_meta.py` & `dvcx-0.78.0/examples/wds_meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 from dvcx.lib.dataset import C, Dataset
 from dvcx.lib.file import File
 from dvcx.lib.webdataset_meta import LaionMeta, parse_wds_meta
 
-ds = Dataset("s3://dvcx-datacomp-small", client_config={"aws_anon": True})
+ds = Dataset("s3://dvcx-datacomp-small", client_config={"anon": True})
 ds = ds.filter(C.name.glob("0020f*"))
 ds = ds.apply(parse_wds_meta)
 
 ds = ds.select(
     File.name,
     File.parent,
     LaionMeta.uid,
```

### Comparing `dvcx-0.77.0/examples/zalando/zalando_clip.py` & `dvcx-0.78.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.78.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/noxfile.py` & `dvcx-0.78.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/pyproject.toml` & `dvcx-0.78.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/asyn.py` & `dvcx-0.78.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/cache.py` & `dvcx-0.78.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/catalog/catalog.py` & `dvcx-0.78.0/src/dvcx/catalog/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1092,15 +1092,16 @@
 
         num_objects = dataset_version.num_objects
         size = dataset_version.size
         if not num_objects:
             num_objects, size = self.warehouse.dataset_stats(dataset, version)
 
         self.metastore.update_dataset_version(
-            dataset_version,
+            dataset,
+            version,
             num_objects=num_objects,
             size=size,
             **kwargs,
         )
 
     def update_dataset(
         self, dataset: DatasetRecord, conn=None, **kwargs
```

### Comparing `dvcx-0.77.0/src/dvcx/catalog/datasource.py` & `dvcx-0.78.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/catalog/formats.py` & `dvcx-0.78.0/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/catalog/loader.py` & `dvcx-0.78.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/cli.py` & `dvcx-0.78.0/src/dvcx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     parent_parser = ArgumentParser(add_help=False)
     parent_parser.add_argument(
         "--aws-endpoint-url",
         type=str,
         help="AWS endpoint URL",
     )
     parent_parser.add_argument(
-        "--aws-anon",
+        "--anon",
         action="store_true",
         help="AWS anon (aka awscli's --no-sign-request)",
     )
     parent_parser.add_argument(
         "--ttl",
         type=human_time_type,
         default=TTL_HUMAN,
@@ -878,15 +878,15 @@
 
     logger.addHandler(logging.StreamHandler())
     logging_level = get_logging_level(args)
     logger.setLevel(logging_level)
 
     client_config = {
         "aws_endpoint_url": args.aws_endpoint_url,
-        "aws_anon": args.aws_anon,
+        "anon": args.anon,
     }
 
     if args.debug_sql:
         # This also sets this environment variable for any subprocesses
         os.environ["DEBUG_SHOW_SQL_QUERIES"] = "True"
 
     try:
```

### Comparing `dvcx-0.77.0/src/dvcx/cli_utils.py` & `dvcx-0.78.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/client/azure.py` & `dvcx-0.78.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/client/fileslice.py` & `dvcx-0.78.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/client/fsspec.py` & `dvcx-0.78.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/client/gcs.py` & `dvcx-0.78.0/src/dvcx/client/gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     PREFIX = "gcs://"
     protocol = "gcs"
 
     @classmethod
     def create_fs(cls, **kwargs) -> GCSFileSystem:
         if os.environ.get("DVCX_GCP_CREDENTIALS"):
             kwargs["token"] = json.loads(os.environ["DVCX_GCP_CREDENTIALS"])
+        if kwargs.pop("anon", False):
+            kwargs["token"] = "anon"  # noqa: S105
 
         return cast(GCSFileSystem, super().create_fs(**kwargs))
 
     @staticmethod
     def parse_timestamp(timestamp: str) -> datetime:
         """
         Parse timestamp string returned by GCSFileSystem.
```

### Comparing `dvcx-0.77.0/src/dvcx/client/local.py` & `dvcx-0.78.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/client/s3.py` & `dvcx-0.78.0/src/dvcx/client/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, cast
 
+from botocore.exceptions import NoCredentialsError
 from s3fs import S3FileSystem
 
 from dvcx.node import Entry
 from dvcx.utils import TIME_ZERO
 
 from .fsspec import DELIMITER, Client
 
@@ -13,16 +14,14 @@
 class ClientS3(Client):
     FS_CLASS = S3FileSystem
     PREFIX = "s3://"
     protocol = "s3"
 
     @classmethod
     def create_fs(cls, **kwargs) -> S3FileSystem:
-        if "aws_anon" in kwargs:
-            kwargs.setdefault("anon", kwargs.pop("aws_anon"))
         if "aws_endpoint_url" in kwargs:
             kwargs.setdefault("client_kwargs", {}).setdefault(
                 "endpoint_url", kwargs.pop("aws_endpoint_url")
             )
         if "aws_key" in kwargs:
             kwargs.setdefault("key", kwargs.pop("aws_key"))
         if "aws_secret" in kwargs:
@@ -35,14 +34,23 @@
         kwargs.setdefault("cache_regions", True)
 
         # We want to use newer v4 signature version since regions added after
         # 2014 are not going to support v2 which is the older one.
         # All regions support v4.
         kwargs.setdefault("config_kwargs", {}).setdefault("signature_version", "s3v4")
 
+        if not kwargs.get("anon"):
+            try:
+                # Run an inexpensive check to see if credentials are available
+                super().create_fs(**kwargs).sign("s3://bucket/object")
+            except NoCredentialsError:
+                kwargs["anon"] = True
+            except NotImplementedError:
+                pass
+
         return cast(S3FileSystem, super().create_fs(**kwargs))
 
     async def _fetch_dir(
         self,
         prefix,
         pbar,
         result_queue,
```

### Comparing `dvcx-0.77.0/src/dvcx/config.py` & `dvcx-0.78.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.78.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.78.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.78.0/src/dvcx/data_storage/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,23 @@
         partial_id: Optional[int] = None,
     ):
         self.uri = uri
         self.partial_id: Optional[int] = partial_id
 
     @abstractmethod
     def clone(
-        self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
+        self,
+        uri: StorageURI = StorageURI(""),
+        partial_id: Optional[int] = None,
+        use_new_connection: bool = False,
     ) -> "AbstractMetastore":
-        """Clones AbstractMetastore implementation for some Storage input."""
+        """Clones AbstractMetastore implementation for some Storage input.
+        Setting use_new_connection will always use a new database connection.
+        New connections should only be used if needed due to errors with
+        closed connections."""
 
     def init(self, uri: StorageURI, partial_id: int) -> None:  # noqa: B027
         """Initialize metastore."""
 
     def close(self) -> None:  # noqa: B027
         """Closes any active database or HTTP connections."""
 
@@ -227,15 +233,15 @@
 
     @abstractmethod
     def update_dataset(self, dataset: DatasetRecord, **kwargs) -> DatasetRecord:
         """Updates dataset fields."""
 
     @abstractmethod
     def update_dataset_version(
-        self, dataset_version: DatasetVersion, **kwargs
+        self, dataset: DatasetRecord, version: int, **kwargs
     ) -> DatasetVersion:
         """Updates dataset version fields."""
 
     @abstractmethod
     def remove_dataset_version(
         self, dataset: DatasetRecord, version: int
     ) -> DatasetRecord:
@@ -527,15 +533,15 @@
             )
         return table
 
     #
     # Query Tables
     #
 
-    def _partials_table(self, uri: StorageURI):
+    def _partials_table(self, uri: StorageURI) -> Table:
         return self._get_storage_partial_table(self._partials_table_name(uri))
 
     @cached_property
     def _storages(self) -> Table:
         return Table(self.STORAGE_TABLE, self.db.metadata, *self._buckets_columns())
 
     @cached_property
@@ -1028,17 +1034,19 @@
         )  # type: ignore [attr-defined]
 
         result_ds = copy.deepcopy(dataset)
         result_ds.update(**dataset_values)
         return result_ds
 
     def update_dataset_version(
-        self, dataset_version: DatasetVersion, conn=None, **kwargs
+        self, dataset: DatasetRecord, version: int, conn=None, **kwargs
     ) -> DatasetVersion:
         """Updates dataset fields."""
+        dataset_version = dataset.get_version(version)
+
         values = {}
         for field, value in kwargs.items():
             if field in self._dataset_version_fields[1:]:
                 if field == "custom_column_types":
                     dataset_version.update(
                         **{field: DatasetRecord.parse_custom_column_types(value)}
                     )
@@ -1168,16 +1176,15 @@
         if status == DatasetStatus.FAILED:
             update_data["error_message"] = error_message
             update_data["error_stack"] = error_stack
 
         self.update_dataset(dataset, conn=conn, **update_data)
 
         if version:
-            dataset_version = dataset.get_version(version)
-            self.update_dataset_version(dataset_version, conn=conn, **update_data)
+            self.update_dataset_version(dataset, version, conn=conn, **update_data)
 
         return dataset
 
     #
     # Dataset dependencies
     #
```

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/schema.py` & `dvcx-0.78.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.78.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.78.0/src/dvcx/data_storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,18 @@
 
         self.db = db or SQLiteDatabaseEngine.from_db_file(db_file)
 
         self._init_storage_table()
         self._init_datasets_tables()
 
     def clone(
-        self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
+        self,
+        uri: StorageURI = StorageURI(""),
+        partial_id: Optional[int] = None,
+        use_new_connection: bool = False,
     ) -> "SQLiteMetastore":
         if not uri:
             if partial_id is not None:
                 raise ValueError("if partial_id is used, uri cannot be empty")
             if self.uri:
                 uri = self.uri
                 if self.partial_id:
@@ -517,15 +520,18 @@
     ):
         self.schema: "DefaultSchema" = DefaultSchema()
         super().__init__(id_generator, uri, partial_id)
 
         self.db = db or SQLiteDatabaseEngine.from_db_file(db_file)
 
     def clone(
-        self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
+        self,
+        uri: StorageURI = StorageURI(""),
+        partial_id: Optional[int] = None,
+        use_new_connection: bool = False,
     ) -> "SQLiteWarehouse":
         if not uri:
             if partial_id is not None:
                 raise ValueError("if partial_id is used, uri cannot be empty")
             if self.uri:
                 uri = self.uri
                 if self.partial_id:
```

### Comparing `dvcx-0.77.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.78.0/src/dvcx/data_storage/warehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,23 @@
         raise ValueError(
             f"Value {val!r} with type {value_type} incompatible for "
             f"column type {type(col_type).__name__}"
         ) from exc
 
     @abstractmethod
     def clone(
-        self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
+        self,
+        uri: StorageURI = StorageURI(""),
+        partial_id: Optional[int] = None,
+        use_new_connection: bool = False,
     ) -> "AbstractWarehouse":
-        """Clones Warehouse implementation for some Storage input"""
+        """Clones Warehouse implementation for some Storage input.
+        Setting use_new_connection will always use a new database connection.
+        New connections should only be used if needed due to errors with
+        closed connections."""
 
     def close(self) -> None:
         """Closes any active database connections."""
         self.db.close()
 
     @abstractmethod
     def init_db(self, uri: StorageURI, partial_id: int) -> None:
```

### Comparing `dvcx-0.77.0/src/dvcx/dataset.py` & `dvcx-0.78.0/src/dvcx/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,18 +508,23 @@
     def from_result_row(cls, columns: list[str], values: Iterable[Any]) -> "DatasetRow":
         row = dict(zip(columns, values))
         return cls.from_dict(row)
 
     @classmethod
     def from_dict(cls, row: dict[str, Any]) -> "DatasetRow":
         core_fields = {key: value for (key, value) in row.items() if hasattr(cls, key)}
+        if core_fields.get("last_modified") and isinstance(
+            core_fields["last_modified"], str
+        ):
+            core_fields["last_modified"] = isoparse(core_fields["last_modified"])
         custom_fields = {
             key: value for (key, value) in row.items() if key not in core_fields
         }
-        return cls(**core_fields, custom=custom_fields)
+        core_fields["custom"] = custom_fields
+        return cls(**core_fields)
 
     def for_insert(self) -> dict[str, Any]:
         """Prepares data for insert"""
         d = attrs.asdict(self)
         del d["id"]  # id will be autogenerated in DB
         del d["parent_id"]  # parent_id is deprecated
         d.update(d.pop("custom", {}))
```

### Comparing `dvcx-0.77.0/src/dvcx/error.py` & `dvcx-0.78.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.78.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/claude.py` & `dvcx-0.78.0/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/dataset.py` & `dvcx-0.78.0/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/feature.py` & `dvcx-0.78.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/feature_types.py` & `dvcx-0.78.0/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.78.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/file.py` & `dvcx-0.78.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.78.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.78.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.78.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/image.py` & `dvcx-0.78.0/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/image_transform.py` & `dvcx-0.78.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.78.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/param.py` & `dvcx-0.78.0/src/dvcx/lib/param.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/pytorch.py` & `dvcx-0.78.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/tar_file.py` & `dvcx-0.78.0/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/text.py` & `dvcx-0.78.0/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/udf.py` & `dvcx-0.78.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/unstructured.py` & `dvcx-0.78.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/utils.py` & `dvcx-0.78.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/webdataset.py` & `dvcx-0.78.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.78.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.78.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/listing.py` & `dvcx-0.78.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/node.py` & `dvcx-0.78.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.78.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.78.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/progress.py` & `dvcx-0.78.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/batch.py` & `dvcx-0.78.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/builtins.py` & `dvcx-0.78.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/dataset.py` & `dvcx-0.78.0/src/dvcx/query/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1182,28 +1182,18 @@
         """Cleanup any temporary tables."""
         if not self.temp_table_names:
             # Nothing to clean up.
             return
         # This is needed to always use a new connection with all metastore and warehouse
         # implementations, as errors may close or render unusable the existing
         # connections.
-        (
-            metastore_class,
-            metastore_args,
-            metastore_kwargs,
-        ) = self.catalog.metastore.clone_params()
-        metastore = metastore_class(*metastore_args, **metastore_kwargs)
+        metastore = self.catalog.metastore.clone(use_new_connection=True)
         metastore.cleanup_temp_tables(self.temp_table_names)
         metastore.close()
-        (
-            warehouse_class,
-            warehouse_args,
-            warehouse_kwargs,
-        ) = self.catalog.warehouse.clone_params()
-        warehouse = warehouse_class(*warehouse_args, **warehouse_kwargs)
+        warehouse = self.catalog.warehouse.clone(use_new_connection=True)
         warehouse.cleanup_temp_tables(self.temp_table_names)
         warehouse.close()
         self.temp_table_names = []
 
     def results(self, row_factory=None, **kwargs):
         with self.as_iterable(**kwargs) as result:
             if row_factory:
```

### Comparing `dvcx-0.77.0/src/dvcx/query/dispatch.py` & `dvcx-0.78.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/params.py` & `dvcx-0.78.0/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/schema.py` & `dvcx-0.78.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/session.py` & `dvcx-0.78.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/query/udf.py` & `dvcx-0.78.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/remote/studio.py` & `dvcx-0.78.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/default/base.py` & `dvcx-0.78.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/functions/array.py` & `dvcx-0.78.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/functions/path.py` & `dvcx-0.78.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/selectable.py` & `dvcx-0.78.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.78.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.78.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/types.py` & `dvcx-0.78.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/sql/utils.py` & `dvcx-0.78.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/storage.py` & `dvcx-0.78.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx/utils.py` & `dvcx-0.78.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.78.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.77.0
+Version: 0.78.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.77.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.78.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,15 @@
 tests/unit/test_catalog_loader.py
 tests/unit/test_cli_parsing.py
 tests/unit/test_client.py
 tests/unit/test_client_s3.py
 tests/unit/test_data_storage.py
 tests/unit/test_database_engine.py
 tests/unit/test_dataset.py
+tests/unit/test_dataset_row.py
 tests/unit/test_dispatch.py
 tests/unit/test_fileslice.py
 tests/unit/test_id_generator.py
 tests/unit/test_listing.py
 tests/unit/test_metastore.py
 tests/unit/test_query_params.py
 tests/unit/test_serializer.py
```

### Comparing `dvcx-0.77.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.78.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/benchmarks/conftest.py` & `dvcx-0.78.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/conftest.py` & `dvcx-0.78.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/data.py` & `dvcx-0.78.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_catalog.py` & `dvcx-0.78.0/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_client.py` & `dvcx-0.78.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_dataset_query.py` & `dvcx-0.78.0/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_datasets.py` & `dvcx-0.78.0/tests/func/test_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,16 @@
 def test_registering_dataset(
     cloud_test_catalog, dogs_dataset, cats_dataset, target_version
 ):
     catalog = cloud_test_catalog.catalog
 
     # make sure there is a custom columns inside, other than default ones
     catalog.metastore.update_dataset_version(
-        dogs_dataset.get_version(1),
+        dogs_dataset,
+        1,
         sources="s3://ldb-public",
         query_script="DatasetQuery()",
         error_message="no error",
         error_stack="no error stack",
         script_output="log",
     )
 
@@ -456,15 +457,16 @@
 
 
 def test_registering_dataset_source_version_in_non_final_status(
     cloud_test_catalog, cats_dataset, dogs_dataset
 ):
     catalog = cloud_test_catalog.catalog
     catalog.metastore.update_dataset_version(
-        dogs_dataset.get_version(1),
+        dogs_dataset,
+        1,
         status=DatasetStatus.PENDING,
     )
 
     with pytest.raises(ValueError) as exc_info:
         catalog.register_dataset(
             dogs_dataset,
             1,
```

### Comparing `dvcx-0.77.0/tests/func/test_ls.py` & `dvcx-0.78.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_pull.py` & `dvcx-0.78.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_pytorch.py` & `dvcx-0.78.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/func/test_query.py` & `dvcx-0.78.0/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/scripts/name_len_normal.py` & `dvcx-0.78.0/tests/scripts/name_len_normal.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     else:
         return (len(name),)
 
 
 # Save as a new dataset.
 DatasetQuery(
     path="gcs://dvcx-datalakes/dogs-and-cats/",
-    client_config={"aws_anon": True},
+    client_config={"anon": True},
 ).filter(C.name.glob("*cat*")).add_signals(name_len, parallel=-1).order_by(  # type: ignore[attr-defined]
     "name"
 ).limit(2).save("name_len")
 
 # Output the contents of the new dataset.
 print(DatasetQuery(name="name_len").select(C.name, C.name_len).results())
```

### Comparing `dvcx-0.77.0/tests/scripts/name_len_slow.py` & `dvcx-0.78.0/tests/scripts/name_len_slow.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,9 +39,9 @@
     else:
         return (len(name),)
 
 
 # Save as a new dataset.
 DatasetQuery(
     path="gcs://dvcx-datalakes/dogs-and-cats/",
-    client_config={"aws_anon": True},
+    client_config={"anon": True},
 ).filter(C.name.glob("*cat*")).add_signals(name_len, parallel=1).save("name_len")  # type: ignore[attr-defined]
```

### Comparing `dvcx-0.77.0/tests/test_cli_e2e.py` & `dvcx-0.78.0/tests/test_cli_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 # Note that these commands are tested in order.
 E2E_STEPS = (
     {
         "command": (
             "dvcx",
             "ls",
-            "--aws-anon",
+            "--anon",
             "s3://ldb-public/remote/datasets/dogs-and-cats/",
         ),
         "expected": dedent(
             """
             dogs-and-cats.tar.gz
             dogs-and-cats.zip
             license
@@ -109,48 +109,48 @@
         ),
         "listing": True,
     },
     {
         "command": (
             "dvcx",
             "du",
-            "--aws-anon",
+            "--anon",
             "s3://ldb-public/remote/datasets/dogs-and-cats/",
         ),
         "expected": "   9.2M s3://ldb-public/remote/datasets/dogs-and-cats/\n",
     },
     {
         "command": (
             "dvcx",
             "find",
             "--iname",
             "*DOG*",
-            "--aws-anon",
+            "--anon",
             "s3://ldb-public/remote/datasets/",
         ),
         "expected": dedent(
             """
             s3://ldb-public/remote/datasets/Stanford-dog-breeds/
             s3://ldb-public/remote/datasets/dogs-and-cats/
             s3://ldb-public/remote/datasets/dogs-and-cats/dogs-and-cats.tar.gz
             s3://ldb-public/remote/datasets/dogs-and-cats/dogs-and-cats.zip
             """
         ),
         "listing": True,
     },
     {
-        "command": ("dvcx", "du", "--aws-anon", "s3://ldb-public/remote/datasets/"),
+        "command": ("dvcx", "du", "--anon", "s3://ldb-public/remote/datasets/"),
         "expected": "  43.3G s3://ldb-public/remote/datasets/\n",
     },
     {
         "command": (
             "dvcx",
             "cp",
             "-r",
-            "--aws-anon",
+            "--anon",
             "s3://ldb-public/remote/datasets/mnist-tiny/",
             "mnt-cp",
         ),
         "expected": "",
         "downloading": True,
         "instantiating": True,
         "files": {
@@ -158,15 +158,15 @@
         },
     },
     {
         "command": (
             "dvcx",
             "clone",
             "-r",
-            "--aws-anon",
+            "--anon",
             "s3://ldb-public/remote/datasets/mnist-tiny/",
             "mnt",
         ),
         "expected": "",
         "downloading": True,
         "instantiating": True,
         "files": {
```

### Comparing `dvcx-0.77.0/tests/test_query_e2e.py` & `dvcx-0.78.0/tests/test_query_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 E2E_STEPS = (
     {
         "command": (
             "dvcx",
             "find",
-            "--aws-anon",
+            "--anon",
             "--name",
             "cat.1.*",
             "gcs://dvcx-datalakes/dogs-and-cats/",
         ),
         "expected": dedent(
             """
             gcs://dvcx-datalakes/dogs-and-cats/cat.1.jpg
```

### Comparing `dvcx-0.77.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.78.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/lib/test_feature.py` & `dvcx-0.78.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.78.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/lib/test_file.py` & `dvcx-0.78.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.78.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.78.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/sql/test_array.py` & `dvcx-0.78.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/sql/test_conditional.py` & `dvcx-0.78.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/sql/test_path.py` & `dvcx-0.78.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/sql/test_selectable.py` & `dvcx-0.78.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/sql/test_string.py` & `dvcx-0.78.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_asyn.py` & `dvcx-0.78.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_cache.py` & `dvcx-0.78.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_catalog.py` & `dvcx-0.78.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_catalog_formats.py` & `dvcx-0.78.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_catalog_loader.py` & `dvcx-0.78.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_cli_parsing.py` & `dvcx-0.78.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_client.py` & `dvcx-0.78.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_client_s3.py` & `dvcx-0.78.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_data_storage.py` & `dvcx-0.78.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_database_engine.py` & `dvcx-0.78.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_dataset.py` & `dvcx-0.78.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_dispatch.py` & `dvcx-0.78.0/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_fileslice.py` & `dvcx-0.78.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_id_generator.py` & `dvcx-0.78.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_listing.py` & `dvcx-0.78.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_metastore.py` & `dvcx-0.78.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_query_params.py` & `dvcx-0.78.0/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_serializer.py` & `dvcx-0.78.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_session.py` & `dvcx-0.78.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_storage.py` & `dvcx-0.78.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_udf.py` & `dvcx-0.78.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_utils.py` & `dvcx-0.78.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/unit/test_warehouse.py` & `dvcx-0.78.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.77.0/tests/utils.py` & `dvcx-0.78.0/tests/utils.py`

 * *Files identical despite different names*

