# Comparing `tmp/rococo-1.0.8.tar.gz` & `tmp/rococo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rococo-1.0.8.tar", last modified: Sat Apr 13 15:40:04 2024, max compression
+gzip compressed data, was "rococo-1.0.9.tar", last modified: Sun Apr 14 05:51:37 2024, max compression
```

## Comparing `rococo-1.0.8.tar` & `rococo-1.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-13 15:39:59.000000 rococo-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-13 15:40:04.722430 rococo-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-13 15:39:59.000000 rococo-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.710430 rococo-1.0.8/rococo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/surrealdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/emailing/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/mailjet.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/ses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/recovery_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/models/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/surreal_versioned_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/versioned_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/base_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/repositories/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/mysql/mysql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/mysql/organization_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/rococo/repositories/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/organization_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/person_organization_role_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/surreal_db_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/rococo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:40:04.722430 rococo-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-13 15:39:59.000000 rococo-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/base_repository_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/surreal_db_repository_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.028276 rococo-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 05:51:32.000000 rococo-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-14 05:51:37.028276 rococo-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-14 05:51:32.000000 rococo-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.016276 rococo-1.0.9/rococo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.020276 rococo-1.0.9/rococo/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.020276 rococo-1.0.9/rococo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.020276 rococo-1.0.9/rococo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/data/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/data/surrealdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.020276 rococo-1.0.9/rococo/emailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/mailjet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/emailing/ses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.020276 rococo-1.0.9/rococo/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/messaging/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/messaging/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.024276 rococo-1.0.9/rococo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/recovery_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.024276 rococo-1.0.9/rococo/models/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/surrealdb/surreal_versioned_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/models/versioned_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.024276 rococo-1.0.9/rococo/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/base_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.024276 rococo-1.0.9/rococo/repositories/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/mysql/mysql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/mysql/organization_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.028276 rococo-1.0.9/rococo/repositories/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/surrealdb/organization_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/surrealdb/person_organization_role_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-14 05:51:32.000000 rococo-1.0.9/rococo/repositories/surrealdb/surreal_db_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.028276 rococo-1.0.9/rococo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-14 05:51:37.000000 rococo-1.0.9/rococo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-14 05:51:37.000000 rococo-1.0.9/rococo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:51:37.000000 rococo-1.0.9/rococo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-14 05:51:37.000000 rococo-1.0.9/rococo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 05:51:37.000000 rococo-1.0.9/rococo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:51:37.028276 rococo-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 05:51:32.000000 rococo-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:37.028276 rococo-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 05:51:32.000000 rococo-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-14 05:51:32.000000 rococo-1.0.9/tests/base_repository_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-14 05:51:32.000000 rococo-1.0.9/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-14 05:51:32.000000 rococo-1.0.9/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-14 05:51:32.000000 rococo-1.0.9/tests/surreal_db_repository_test.py
```

### Comparing `rococo-1.0.8/LICENSE` & `rococo-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/PKG-INFO` & `rococo-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.8/README.md` & `rococo-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/auth/tokens.py` & `rococo-1.0.9/rococo/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/config/config.py` & `rococo-1.0.9/rococo/config/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/data/base.py` & `rococo-1.0.9/rococo/data/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
     @abstractmethod
     def __exit__(self, exc_type, exc_value, traceback):
         """Context manager exit point for closing DB connection."""
         pass
 
     @abstractmethod
+    def run_transaction(self, operations_list: List[Any]):
+        """Execute a list of queries / operations as a transaction."""
+        pass
+
+    @abstractmethod
     def execute_query(self, sql: str, _vars: Dict[str, Any] = None) -> Any:
         """Executes a raw SQL query against the DB."""
         pass
 
     @abstractmethod
     def parse_db_response(self, response: Any) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """Parses the raw response from the database and returns structured data."""
@@ -33,19 +38,29 @@
     @abstractmethod
     def get_many(self, table: str, conditions: Dict[str, Any] = None, sort: List[Tuple[str, str]] = None, 
                  limit: int = 100) -> List[Dict[str, Any]]:
         """Fetches multiple records from the specified table based on given conditions."""
         pass
 
     @abstractmethod
+    def get_move_entity_to_audit_table_query(self, table, entity_id):
+        """Returns query to move entity by entity_id to audit table."""
+        pass
+
+    @abstractmethod
     def move_entity_to_audit_table(self, table_name: str, entity_id: str):
         """Inserts the existing entities by entity_id in {table_name}_audit table."""
         pass
 
     @abstractmethod
+    def get_save_query(self, table: str, data: Dict[str, Any]):
+        """Returns query to save a data record in the table."""
+        pass
+
+    @abstractmethod
     def save(self, table: str, data: Dict[str, Any]) -> Union[Dict[str, Any], None]:
         """Saves or updates a record in the specified table."""
         pass
 
     @abstractmethod
     def delete(self, table: str, data: Dict[str, Any]) -> bool:
         """Deletes a record in the specified table based on given conditions."""
```

### Comparing `rococo-1.0.8/rococo/data/mysql.py` & `rococo-1.0.9/rococo/data/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,27 +76,42 @@
         elif isinstance(value, UUID):
             return f"{key}='{str(value)}'"
         elif isinstance(value, type(None)):
             return f"{key} IS NULL"
         else:
             raise Exception(f"Unsupported type {type(value)} for condition key: {key}, value: {value}")
 
+    def get_move_entity_to_audit_table_query(self, table, entity_id):
+        """Returns the query to move an entity to audit table."""
+        return f"""INSERT INTO {table}_audit (SELECT * FROM {table} WHERE entity_id=%s)""", (str(entity_id).replace('-', ''),)
+
     def move_entity_to_audit_table(self, table, entity_id):
-        query = f"""INSERT INTO {table}_audit (SELECT * FROM {table} WHERE entity_id="{str(entity_id).replace('-', '')}")"""
-        self._call_cursor('execute', query)
+        """Executes the query to move an entity to audit table."""
+        query, values = self.get_move_entity_to_audit_table_query(table, entity_id)
+        self._cursor.execute(query, values)
         self._connection.commit()
 
     def execute_query(self, sql, _vars=None):
         """Executes a query against the DB."""
         if _vars is None:
             _vars = {}
 
         self._call_cursor('execute', sql, _vars)
         return self._call_cursor('fetchall')
 
+    def run_transaction(self, queries_list):
+        """Executes a list of queries in a single transaction against the database."""
+        for query in queries_list:
+            if type(query) is tuple:
+                query, values = query
+            else:
+                values = ()
+            self._cursor.execute(query, values)
+        self._connection.commit()
+
     def parse_db_response(self, response: List[Dict[str, Any]]) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """
         Parse the response from SurrealDB.
 
         If the 'result' list has one item, return that item.
         If the 'result' list has multiple items, return the list.
         If the 'result' list is empty or if there's no 'result', return an empty list.
@@ -180,22 +195,28 @@
         if not db_response:
             return []
         elif isinstance(db_response, dict):
             return [db_response]
         else:
             return db_response
 
+    def get_save_query(self, table_name, data):
+        """Returns a query to save an entity in database."""
+        columns = ', '.join(data.keys())
+        placeholders = ', '.join(['%s'] * len(data))
+
+        values = tuple(data.values())
+        query = f"REPLACE INTO {table_name} ({columns}) VALUES ({placeholders})"
+
+        return query, values
+
     def _create_in_database(self, table_name, data):
         try:
-            columns = ', '.join(data.keys())
-            placeholders = ', '.join(['%s'] * len(data))
-            values = tuple(data.values())
-
-            sql = f"REPLACE INTO {table_name} ({columns}) VALUES ({placeholders})"
-            self._cursor.execute(sql, values)
+            query, values = self.get_save_query(table_name, data)
+            self._cursor.execute(query, values)
             self._connection.commit()
             return True
         except Exception as e:
             logging.error("Error in SQL:\n%s", e)
             raise e
 
     def save(self, table: str, data: Dict[str, Any]):
```

### Comparing `rococo-1.0.8/rococo/emailing/config.py` & `rococo-1.0.9/rococo/emailing/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/emailing/factory.py` & `rococo-1.0.9/rococo/emailing/factory.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/emailing/mailjet.py` & `rococo-1.0.9/rococo/emailing/mailjet.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/messaging/base.py` & `rococo-1.0.9/rococo/messaging/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/messaging/rabbitmq.py` & `rococo-1.0.9/rococo/messaging/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/messaging/sqs.py` & `rococo-1.0.9/rococo/messaging/sqs.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/login_method.py` & `rococo-1.0.9/rococo/models/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/organization.py` & `rococo-1.0.9/rococo/models/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/person_organization_role.py` & `rococo-1.0.9/rococo/models/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/surrealdb/login_method.py` & `rococo-1.0.9/rococo/models/surrealdb/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/surrealdb/organization.py` & `rococo-1.0.9/rococo/models/surrealdb/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/surrealdb/person_organization_role.py` & `rococo-1.0.9/rococo/models/surrealdb/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/surrealdb/surreal_versioned_model.py` & `rococo-1.0.9/rococo/models/surrealdb/surreal_versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/models/versioned_model.py` & `rococo-1.0.9/rococo/models/versioned_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,14 +143,16 @@
                     else:
                         results[key] = value.as_dict(convert_datetime_to_iso_string)
                 elif isinstance(value, UUID):
                     if convert_uuids:
                         results[key] = str(value)
                 elif isinstance(value, str):
                     results[key] = value
+                elif isinstance(value, dict):
+                    results[key] = str(value.get('entity_id')) if convert_uuids else value.get('entity_id')
                 else:
                     raise NotImplementedError
 
             if convert_datetime_to_iso_string:
                 if isinstance(value, datetime):
                     results[key] = value.isoformat()
             if convert_uuids:
```

### Comparing `rococo-1.0.8/rococo/repositories/base_repository.py` & `rococo-1.0.9/rococo/repositories/base_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,16 +69,18 @@
         self._process_data_from_db(records)
 
         return [self.model.from_dict(record) for record in records]
 
     def save(self, instance: VersionedModel, send_message: bool = False):
         """Save func"""
         data = self._process_data_before_save(instance)
-        self._execute_within_context(self.adapter.move_entity_to_audit_table, self.table_name, instance.entity_id)
-        self._execute_within_context(self.adapter.save, self.table_name, data)
+        with self.adapter:
+            move_entity_query = self.adapter.get_move_entity_to_audit_table_query(self.table_name, instance.entity_id)
+            save_entity_query = self.adapter.get_save_query(self.table_name, data)
+            self.adapter.run_transaction([move_entity_query, save_entity_query])
         if send_message:
             # This assumes that the instance is now in post-saved state with all the new DB updates
             message = json.dumps(instance.as_dict(convert_datetime_to_iso_string=True))
             self.message_adapter.send_message(self.queue_name, message)
 
         return instance
```

### Comparing `rococo-1.0.8/rococo/repositories/mysql/mysql_repository.py` & `rococo-1.0.9/rococo/repositories/mysql/mysql_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """MySqlDbRepository class"""
 
-import re
 from dataclasses import fields
 from datetime import datetime
+import json
+import re
 from typing import Any, Dict, List, Type, Union
 from uuid import UUID
 
 from rococo.data import MySqlAdapter
 from rococo.messaging import MessageAdapter
 from rococo.models import VersionedModel
 from rococo.repositories import BaseRepository
```

### Comparing `rococo-1.0.8/rococo/repositories/mysql/organization_repository.py` & `rococo-1.0.9/rococo/repositories/mysql/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/repositories/surrealdb/organization_repository.py` & `rococo-1.0.9/rococo/repositories/surrealdb/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/repositories/surrealdb/person_organization_role_repository.py` & `rococo-1.0.9/rococo/repositories/surrealdb/person_organization_role_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo/repositories/surrealdb/surreal_db_repository.py` & `rococo-1.0.9/rococo/repositories/surrealdb/surreal_db_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/rococo.egg-info/PKG-INFO` & `rococo-1.0.9/rococo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.8/rococo.egg-info/SOURCES.txt` & `rococo-1.0.9/rococo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/setup.py` & `rococo-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='rococo',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     url='https://github.com/EcorRouge/rococo',
     license='MIT',
     author='Jay Grieves',
     author_email='jaygrieves@gmail.com',
     description='A Python library to help build things the way we want them built',
     long_description=open('README.md').read(),
```

### Comparing `rococo-1.0.8/tests/base_repository_test.py` & `rococo-1.0.9/tests/base_repository_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,54 +104,58 @@
         mock_adapter.__enter__.assert_called()
         mock_adapter.__exit__.assert_called()
 
     def test_save(self, repository, mock_adapter):
         """
         Test saving a model instance
         """
-        mock_adapter.save.return_value = True
-        mock_adapter.move_entity_to_audit_table.return_value = None
+        mock_adapter.get_save_query.return_value = "", ()
+        mock_adapter.get_move_entity_to_audit_table_query.return_value = "", ()
+        mock_adapter.run_transaction.return_value = True
 
         model_instance = TestVersionedModel()
         result = repository.save(model_instance)
 
         assert result is model_instance
         assert result.entity_id is not None
         assert result.version is not None
 
-        mock_adapter.save.assert_called_with('testversionedmodel', {})
+        mock_adapter.run_transaction.assert_called_with([("", ()), ("", ())])
         mock_adapter.__enter__.assert_called()
         mock_adapter.__exit__.assert_called()
 
     def test_delete(self, repository, mock_adapter):
         """
         Test deleting by id
         """
-        mock_adapter.save.return_value = True
-        mock_adapter.move_entity_to_audit_table.return_value = None
+        mock_adapter.get_save_query.return_value = "", ()
+        mock_adapter.get_move_entity_to_audit_table_query.return_value = "", ()
+        mock_adapter.run_transaction.return_value = True
 
         model_instance = TestVersionedModel()
         result = repository.delete(model_instance)
 
         assert result is model_instance
         assert model_instance.active == False
-        mock_adapter.save.assert_called_with('testversionedmodel', {})
+
+        mock_adapter.run_transaction.assert_called_with([("", ()), ("", ())])
         mock_adapter.__enter__.assert_called()
         mock_adapter.__exit__.assert_called()
 
     def test_save_with_message(self, repository, mock_adapter, _mock_message_adapter):
         """
         Test saving and sending message
         """
-        mock_adapter.save.return_value = True
-        mock_adapter.move_entity_to_audit_table.return_value = None
+        mock_adapter.get_save_query.return_value = "", ()
+        mock_adapter.get_move_entity_to_audit_table_query.return_value = "", ()
+        mock_adapter.run_transaction.return_value = True
 
         model_instance = TestVersionedModel()
         result = repository.save(model_instance, True)
 
         assert result is model_instance
-        mock_adapter.save.assert_called_with('testversionedmodel', {})
+        mock_adapter.run_transaction.assert_called_with([("", ()), ("", ())])
         mock_adapter.__enter__.assert_called()
         mock_adapter.__exit__.assert_called()
 
 if __name__ == '__main__':
     pytest.main()
```

### Comparing `rococo-1.0.8/tests/config_test.py` & `rococo-1.0.9/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/tests/model_test.py` & `rococo-1.0.9/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.8/tests/surreal_db_repository_test.py` & `rococo-1.0.9/tests/surreal_db_repository_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,43 +39,45 @@
         )
 
     def test_save_sends_message(self):
         """
         test that saving sends the message
         """
         # Set up the mock to return a successful save
-        self.db_adapter_mock.save.return_value = True
+        self.db_adapter_mock.get_save_query.return_value = "", ()
+        self.db_adapter_mock.get_move_entity_to_audit_table_query.return_value = "", ()
+        self.db_adapter_mock.run_transaction.return_value = True
 
         # Call the save method
         saved_instance = self.repository.save(self.model_instance, send_message=True)
 
         surrealdb_dict = saved_instance.as_dict(convert_datetime_to_iso_string=True)
         surrealdb_dict['id'] = surrealdb_dict.pop('entity_id')
         # Assert the save method on the adapter was called once with the correct arguments
-        self.db_adapter_mock.save.assert_called_once_with(
-            "versionedmodelhelper", {**surrealdb_dict, 'id': f'{self.model_instance.__class__.__name__.lower()}:`{surrealdb_dict["id"]}`'}
-        )
+        self.db_adapter_mock.run_transaction.assert_called_once_with([("", ()), ("", ())])
 
         # Assert the send_message method was called once with the correct arguments
         self.message_adapter_mock.send_message.assert_called_once_with(
             self.queue_name, json.dumps(self.model_instance.as_dict(convert_datetime_to_iso_string=True))
         )
 
     def test_save_without_message(self):
         """
         Test save without sending message
         """
         # Set up the mock to return a successful save
-        self.db_adapter_mock.save.return_value = True
+        self.db_adapter_mock.get_save_query.return_value = "", ()
+        self.db_adapter_mock.get_move_entity_to_audit_table_query.return_value = "", ()
+        self.db_adapter_mock.run_transaction.return_value = True
 
         # Call the save method with send_message as False
         self.repository.save(self.model_instance, send_message=False)
 
         # Assert the save method on the adapter was called
-        self.db_adapter_mock.save.assert_called_once()
+        self.db_adapter_mock.run_transaction.assert_called_once_with([("", ()), ("", ())])
 
         # Assert the send_message method was not called
         self.message_adapter_mock.send_message.assert_not_called()
 
 
 if __name__ == '__main__':
     unittest.main()
```

