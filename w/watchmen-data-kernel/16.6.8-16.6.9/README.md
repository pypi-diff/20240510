# Comparing `tmp/watchmen_data_kernel-16.6.8.tar.gz` & `tmp/watchmen_data_kernel-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_data_kernel-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_data_kernel-16.6.9.tar", max compression
```

## Comparing `watchmen_data_kernel-16.6.8.tar` & `watchmen_data_kernel-16.6.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/LICENSE
--rw-r--r--   0        0        0     1207 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/__init__.py
--rw-r--r--   0        0        0      187 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/__init__.py
--rw-r--r--   0        0        0     2808 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/cache_manager.py
--rw-r--r--   0        0        0     5991 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/cache_service.py
--rw-r--r--   0        0        0     1555 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/data_source_cache.py
--rw-r--r--   0        0        0     1048 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/external_writer_cache.py
--rw-r--r--   0        0        0     1097 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/internal_cache.py
--rw-r--r--   0        0        0     1442 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/key_store_cache.py
--rw-r--r--   0        0        0     1897 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py
--rw-r--r--   0        0        0     2292 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/pipeline_cache.py
--rw-r--r--   0        0        0      861 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/tenant_cache.py
--rw-r--r--   0        0        0     2811 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/topic_cache.py
--rw-r--r--   0        0        0      463 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/common/__init__.py
--rw-r--r--   0        0        0       44 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/common/exception.py
--rw-r--r--   0        0        0     3596 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/common/settings.py
--rw-r--r--   0        0        0      399 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/__init__.py
--rw-r--r--   0        0        0     1840 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/aes_encryptor.py
--rw-r--r--   0        0        0     4349 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/center_masker.py
--rw-r--r--   0        0        0     2642 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/date_masker.py
--rw-r--r--   0        0        0     1475 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/encryptor.py
--rw-r--r--   0        0        0     2936 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/encryptor_registry.py
--rw-r--r--   0        0        0     1607 2024-01-08 07:58:02.496594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/last_masker.py
--rw-r--r--   0        0        0      776 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/mail_masker.py
--rw-r--r--   0        0        0      807 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/md5_encryptor.py
--rw-r--r--   0        0        0      968 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/sha256_encryptor.py
--rw-r--r--   0        0        0      340 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/external_writer/__init__.py
--rw-r--r--   0        0        0     1029 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py
--rw-r--r--   0        0        0     2006 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/external_writer/external_writer_registry.py
--rw-r--r--   0        0        0      285 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1410 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/data_source_service.py
--rw-r--r--   0        0        0     1993 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/external_writer_service.py
--rw-r--r--   0        0        0     1091 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/key_store_service.py
--rw-r--r--   0        0        0     2227 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/pipeline_service.py
--rw-r--r--   0        0        0     1343 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/tenant_service.py
--rw-r--r--   0        0        0     3683 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/topic_service.py
--rw-r--r--   0        0        0      162 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/__init__.py
--rw-r--r--   0        0        0     1017 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/service_helper.py
--rw-r--r--   0        0        0     1535 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/storage_helper.py
--rw-r--r--   0        0        0     3078 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/topic_structure_helper.py
--rw-r--r--   0        0        0      319 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/__init__.py
--rw-r--r--   0        0        0     7280 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/data_entity_helper.py
--rw-r--r--   0        0        0    16527 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/data_service.py
--rw-r--r--   0        0        0     1560 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/factor_column_mapper.py
--rw-r--r--   0        0        0     4634 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/raw_data_service.py
--rw-r--r--   0        0        0     3146 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/regular_data_service.py
--rw-r--r--   0        0        0     2207 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/shaper.py
--rw-r--r--   0        0        0     3610 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/topic_storage.py
--rw-r--r--   0        0        0      639 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/__init__.py
--rw-r--r--   0        0        0      248 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/ask_action_defined_as.py
--rw-r--r--   0        0        0    36597 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py
--rw-r--r--   0        0        0    57849 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py
--rw-r--r--   0        0        0      250 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/time_utils.py
--rw-r--r--   0        0        0      941 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/topic_utils.py
--rw-r--r--   0        0        0     7540 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/utils.py
--rw-r--r--   0        0        0     3074 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/variables.py
--rw-r--r--   0        0        0      145 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/system/__init__.py
--rw-r--r--   0        0        0     1818 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/system/change_log_helper.py
--rw-r--r--   0        0        0     8377 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/system/operation_helper.py
--rw-r--r--   0        0        0       79 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/__init__.py
--rw-r--r--   0        0        0     2628 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py
--rw-r--r--   0        0        0     3235 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/date_time_factor.py
--rw-r--r--   0        0        0     2462 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/default_value_factor.py
--rw-r--r--   0        0        0     5245 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/encrypt_factor.py
--rw-r--r--   0        0        0      911 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/flatten_factor.py
--rw-r--r--   0        0        0     3656 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/topic_schema.py
--rw-r--r--   0        0        0     6189 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/utils.py
--rw-r--r--   0        0        0      113 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/utils/__init__.py
--rw-r--r--   0        0        0     2749 2024-01-08 07:58:02.500594 watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/utils/variable_helper.py
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 watchmen_data_kernel-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1207 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/__init__.py
+-rw-r--r--   0        0        0      187 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/__init__.py
+-rw-r--r--   0        0        0     2808 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/cache_manager.py
+-rw-r--r--   0        0        0     5991 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/cache_service.py
+-rw-r--r--   0        0        0     1555 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/data_source_cache.py
+-rw-r--r--   0        0        0     1048 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/external_writer_cache.py
+-rw-r--r--   0        0        0     1097 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/internal_cache.py
+-rw-r--r--   0        0        0     1442 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/key_store_cache.py
+-rw-r--r--   0        0        0     1897 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py
+-rw-r--r--   0        0        0     2292 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/pipeline_cache.py
+-rw-r--r--   0        0        0      861 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/tenant_cache.py
+-rw-r--r--   0        0        0     2811 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/topic_cache.py
+-rw-r--r--   0        0        0      463 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/common/__init__.py
+-rw-r--r--   0        0        0       44 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/common/exception.py
+-rw-r--r--   0        0        0     3596 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/common/settings.py
+-rw-r--r--   0        0        0      399 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/__init__.py
+-rw-r--r--   0        0        0     1840 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/aes_encryptor.py
+-rw-r--r--   0        0        0     4349 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/center_masker.py
+-rw-r--r--   0        0        0     2642 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/date_masker.py
+-rw-r--r--   0        0        0     1475 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/encryptor.py
+-rw-r--r--   0        0        0     2936 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/encryptor_registry.py
+-rw-r--r--   0        0        0     1607 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/last_masker.py
+-rw-r--r--   0        0        0      776 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/mail_masker.py
+-rw-r--r--   0        0        0      807 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/md5_encryptor.py
+-rw-r--r--   0        0        0      968 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/sha256_encryptor.py
+-rw-r--r--   0        0        0      340 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/external_writer/__init__.py
+-rw-r--r--   0        0        0     1029 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py
+-rw-r--r--   0        0        0     2006 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/external_writer/external_writer_registry.py
+-rw-r--r--   0        0        0      285 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1410 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/data_source_service.py
+-rw-r--r--   0        0        0     1993 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/external_writer_service.py
+-rw-r--r--   0        0        0     1091 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/key_store_service.py
+-rw-r--r--   0        0        0     2227 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/pipeline_service.py
+-rw-r--r--   0        0        0     1343 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/tenant_service.py
+-rw-r--r--   0        0        0     3683 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/topic_service.py
+-rw-r--r--   0        0        0      162 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/__init__.py
+-rw-r--r--   0        0        0     1017 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/service_helper.py
+-rw-r--r--   0        0        0     1535 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/storage_helper.py
+-rw-r--r--   0        0        0     3078 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/topic_structure_helper.py
+-rw-r--r--   0        0        0      319 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     7280 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/data_entity_helper.py
+-rw-r--r--   0        0        0    16527 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/data_service.py
+-rw-r--r--   0        0        0     1560 2024-02-01 01:32:37.231322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/factor_column_mapper.py
+-rw-r--r--   0        0        0     4634 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/raw_data_service.py
+-rw-r--r--   0        0        0     3146 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/regular_data_service.py
+-rw-r--r--   0        0        0     2207 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/shaper.py
+-rw-r--r--   0        0        0     3610 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/topic_storage.py
+-rw-r--r--   0        0        0      639 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/__init__.py
+-rw-r--r--   0        0        0      248 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/ask_action_defined_as.py
+-rw-r--r--   0        0        0    36597 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py
+-rw-r--r--   0        0        0    57849 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py
+-rw-r--r--   0        0        0      250 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/time_utils.py
+-rw-r--r--   0        0        0      941 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/topic_utils.py
+-rw-r--r--   0        0        0     7540 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/utils.py
+-rw-r--r--   0        0        0     3074 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/variables.py
+-rw-r--r--   0        0        0      145 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/system/__init__.py
+-rw-r--r--   0        0        0     1818 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/system/change_log_helper.py
+-rw-r--r--   0        0        0     8377 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/system/operation_helper.py
+-rw-r--r--   0        0        0       79 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/__init__.py
+-rw-r--r--   0        0        0     2628 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py
+-rw-r--r--   0        0        0     3235 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/date_time_factor.py
+-rw-r--r--   0        0        0     2462 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/default_value_factor.py
+-rw-r--r--   0        0        0     5245 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/encrypt_factor.py
+-rw-r--r--   0        0        0      911 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/flatten_factor.py
+-rw-r--r--   0        0        0     3656 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/topic_schema.py
+-rw-r--r--   0        0        0     6189 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/utils.py
+-rw-r--r--   0        0        0      113 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/utils/__init__.py
+-rw-r--r--   0        0        0     2749 2024-02-01 01:32:37.235322 watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/utils/variable_helper.py
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 watchmen_data_kernel-16.6.9/PKG-INFO
```

### Comparing `watchmen_data_kernel-16.6.8/LICENSE` & `watchmen_data_kernel-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/pyproject.toml` & `watchmen_data_kernel-16.6.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-data-kernel"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_data_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cacheout = "^0.13.1"
 pycryptodome = "^3.14.1"
-watchmen-meta = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
-watchmen-storage-oss = { version = "16.6.8", optional = true }
-watchmen-storage-s3 = { version = "16.6.8", optional = true }
+watchmen-meta = "16.6.9"
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
+watchmen-storage-oss = { version = "16.6.9", optional = true }
+watchmen-storage-s3 = { version = "16.6.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/cache_manager.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/cache_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/data_source_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/data_source_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/external_writer_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/external_writer_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/internal_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/internal_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/key_store_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/key_store_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/pipeline_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/pipeline_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/tenant_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/tenant_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/cache/topic_cache.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/cache/topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/common/settings.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/aes_encryptor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/aes_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/center_masker.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/center_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/date_masker.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/date_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/encryptor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/encryptor_registry.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/encryptor_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/last_masker.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/last_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/mail_masker.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/mail_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/md5_encryptor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/md5_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/encryption/sha256_encryptor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/encryption/sha256_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/external_writer/external_writer_registry.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/external_writer/external_writer_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/data_source_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/data_source_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/external_writer_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/external_writer_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/key_store_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/key_store_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/pipeline_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/tenant_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/tenant_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/meta/topic_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/meta/topic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/service_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/service_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/storage_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/storage_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/service/topic_structure_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/service/topic_structure_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/data_entity_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/data_entity_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/data_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/factor_column_mapper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/factor_column_mapper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/raw_data_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/raw_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/regular_data_service.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/regular_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/shaper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/shaper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage/topic_storage.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage/topic_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/__init__.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/topic_utils.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/utils.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/storage_bridge/variables.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/storage_bridge/variables.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/system/change_log_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/system/change_log_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/system/operation_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/system/operation_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/date_time_factor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/date_time_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/default_value_factor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/default_value_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/encrypt_factor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/encrypt_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/flatten_factor.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/flatten_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/topic_schema.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/topic_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/topic_schema/utils.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/topic_schema/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/src/watchmen_data_kernel/utils/variable_helper.py` & `watchmen_data_kernel-16.6.9/src/watchmen_data_kernel/utils/variable_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.6.8/PKG-INFO` & `watchmen_data_kernel-16.6.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-data-kernel
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: cacheout (>=0.13.1,<0.14.0)
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
-Requires-Dist: watchmen-meta (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.6.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.6.8) ; extra == "s3"
+Requires-Dist: watchmen-meta (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.6.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.6.9) ; extra == "s3"
```

