# Comparing `tmp/apollo_orm-2.2.1.tar.gz` & `tmp/apollo_orm-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo_orm-2.2.1.tar", last modified: Fri Apr 26 15:16:15 2024, max compression
+gzip compressed data, was "apollo_orm-2.2.2.tar", last modified: Fri Apr 26 15:17:39 2024, max compression
```

## Comparing `apollo_orm-2.2.1.tar` & `apollo_orm-2.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.063059 apollo_orm-2.2.1/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo_orm-2.2.1/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-26 15:16:15.062059 apollo_orm-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo_orm-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.032564 apollo_orm-2.2.1/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo_orm-2.2.1/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.036655 apollo_orm-2.2.1/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo_orm-2.2.1/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.036655 apollo_orm-2.2.1/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo_orm-2.2.1/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.038194 apollo_orm-2.2.1/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.039208 apollo_orm-2.2.1/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.039734 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.040748 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.042746 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.043746 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.045814 apollo_orm-2.2.1/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.046979 apollo_orm-2.2.1/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.048991 apollo_orm-2.2.1/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo_orm-2.2.1/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.049991 apollo_orm-2.2.1/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo_orm-2.2.1/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.051991 apollo_orm-2.2.1/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo_orm-2.2.1/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo_orm-2.2.1/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo_orm-2.2.1/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    23411 2024-04-26 15:15:33.000000 apollo_orm-2.2.1/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.056057 apollo_orm-2.2.1/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo_orm-2.2.1/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo_orm-2.2.1/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo_orm-2.2.1/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo_orm-2.2.1/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.057058 apollo_orm-2.2.1/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo_orm-2.2.1/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.058061 apollo_orm-2.2.1/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo_orm-2.2.1/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo_orm-2.2.1/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.060058 apollo_orm-2.2.1/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo_orm-2.2.1/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo_orm-2.2.1/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.061059 apollo_orm-2.2.1/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-26 15:16:15.000000 apollo_orm-2.2.1/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-26 15:16:15.000000 apollo_orm-2.2.1/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 15:16:15.000000 apollo_orm-2.2.1/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 15:16:15.000000 apollo_orm-2.2.1/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-26 15:15:59.000000 apollo_orm-2.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 15:16:15.063059 apollo_orm-2.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 15:16:15.060058 apollo_orm-2.2.1/tests/
--rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo_orm-2.2.1/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.170305 apollo_orm-2.2.2/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo_orm-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-26 15:17:39.169308 apollo_orm-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo_orm-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.143126 apollo_orm-2.2.2/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo_orm-2.2.2/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.147127 apollo_orm-2.2.2/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo_orm-2.2.2/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.148126 apollo_orm-2.2.2/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo_orm-2.2.2/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.148126 apollo_orm-2.2.2/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.149127 apollo_orm-2.2.2/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.150127 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.151127 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.152219 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.154220 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.155221 apollo_orm-2.2.2/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.156220 apollo_orm-2.2.2/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.158219 apollo_orm-2.2.2/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo_orm-2.2.2/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.159220 apollo_orm-2.2.2/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo_orm-2.2.2/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.161220 apollo_orm-2.2.2/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo_orm-2.2.2/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo_orm-2.2.2/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo_orm-2.2.2/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    23414 2024-04-26 15:17:21.000000 apollo_orm-2.2.2/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.164306 apollo_orm-2.2.2/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo_orm-2.2.2/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo_orm-2.2.2/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo_orm-2.2.2/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo_orm-2.2.2/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.164306 apollo_orm-2.2.2/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo_orm-2.2.2/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.165305 apollo_orm-2.2.2/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo_orm-2.2.2/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo_orm-2.2.2/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.167305 apollo_orm-2.2.2/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo_orm-2.2.2/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo_orm-2.2.2/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.168307 apollo_orm-2.2.2/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-26 15:17:39.000000 apollo_orm-2.2.2/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-26 15:17:39.000000 apollo_orm-2.2.2/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 15:17:39.000000 apollo_orm-2.2.2/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 15:17:39.000000 apollo_orm-2.2.2/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-26 15:17:21.000000 apollo_orm-2.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 15:17:39.170305 apollo_orm-2.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 15:17:39.167305 apollo_orm-2.2.2/tests/
+-rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo_orm-2.2.2/tests/test_full_process.py
```

### Comparing `apollo_orm-2.2.1/LICENSE` & `apollo_orm-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/PKG-INFO` & `apollo_orm-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.2.1
+Version: 2.2.2
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo_orm-2.2.1/README.md` & `apollo_orm-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo_orm-2.2.2/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo_orm-2.2.2/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo_orm-2.2.2/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/orm/abstracts/idatabase.py` & `apollo_orm-2.2.2/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/orm/core.py` & `apollo_orm-2.2.2/apollo_orm/orm/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 protocol_version=protocol_version,
                 idle_heartbeat_interval=self._idle_heartbeat_interval,
                 execution_profiles={EXEC_PROFILE_DEFAULT: self._execution_profile},
                 reconnection_policy=ExponentialReconnectionPolicy(base_delay=1.0, max_delay=10.0, max_attempts=None)
             )
             self.session = self.cluster.connect(self._connection_config.credential.keyspace_name)
             self._scan_tables()
-            self.log.info(f"Connected to {self._connection_config.credential.hosts}")
+            self.log.debug(f"Connected to {self._connection_config.credential.hosts}")
             return
         except Exception as e:
             error_message = str(e) if str(e) else "Unknown error"
             raise ApolloORMException(f"Failed to connect after {self._attempts} attempts - {error_message}")
 
     def close(self):
         if self.session is not None:
@@ -358,23 +358,23 @@
                   sorted(filtered_columns.values(), key=lambda x: x.name)]
         if exec_async:
             return self._execute_async_query(prepared_statement, values)
         self._execute_query(prepared_statement, values)
 
     def _execute_async_query(self, statement: PreparedStatement, values: List[Any]) -> ResponseFuture:
         statement.is_idempotent = True
-        self.log.info(f"Executing query: {statement.query_string} with values: {values}")
+        self.log.debug(f"Executing query: {statement.query_string} with values: {values}")
         try:
             return self.session.execute_async(statement, values, )
         except Exception as e:
             self.log.error(f"Failed to execute query: {statement.query_string, values}")
             raise ApolloORMException(f"Failed to execute query: {statement.query_string, values} - {e}")
 
     def _execute_query(self, statement: PreparedStatement, values: List[Any]) -> ResultSet:
-        self.log.info(f"Executing query: {statement.query_string} with values: {values}")
+        self.log.debug(f"Executing query: {statement.query_string} with values: {values}")
         try:
             return self.session.execute(statement, values)
         except Exception as e:
             self.log.error(f"Connection error: {e}")
             raise ApolloORMException(f"Failed to execute query: {statement.query_string, values} - {e}")
 
     def _prepare_dynamic_statement(self, columns: Dict[str, Column], table_name: str,
```

### Comparing `apollo_orm-2.2.1/apollo_orm/orm/credentials/credential_service.py` & `apollo_orm-2.2.2/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/orm/credentials/json_credential_service.py` & `apollo_orm-2.2.2/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo_orm-2.2.2/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo_orm-2.2.2/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm/utils/logger/logger.py` & `apollo_orm-2.2.2/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/apollo_orm.egg-info/PKG-INFO` & `apollo_orm-2.2.2/apollo_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.2.1
+Version: 2.2.2
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo_orm-2.2.1/apollo_orm.egg-info/SOURCES.txt` & `apollo_orm-2.2.2/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.2.1/pyproject.toml` & `apollo_orm-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo_orm-2.2.1/tests/test_full_process.py` & `apollo_orm-2.2.2/tests/test_full_process.py`

 * *Files identical despite different names*

