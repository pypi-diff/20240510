# Comparing `tmp/trex-model-1.4.1.tar.gz` & `tmp/trex-model-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-1.4.1.tar", last modified: Mon May  6 09:16:26 2024, max compression
+gzip compressed data, was "trex-model-1.4.2.tar", last modified: Fri May 10 06:11:57 2024, max compression
```

## Comparing `trex-model-1.4.1.tar` & `trex-model-1.4.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.357923 trex-model-1.4.1/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.4.1/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.4.1/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      643 2024-05-06 09:16:26.357760 trex-model-1.4.1/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.4.1/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 09:16:26.358792 trex-model-1.4.1/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2024-05-06 09:14:52.000000 trex-model-1.4.1/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.357180 trex-model-1.4.1/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      643 2024-05-06 09:16:26.000000 trex-model-1.4.1/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     2326 2024-05-06 09:16:26.000000 trex-model-1.4.1/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 09:16:26.000000 trex-model-1.4.1/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2024-05-06 09:16:26.000000 trex-model-1.4.1/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2024-05-06 09:16:26.000000 trex-model-1.4.1/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.322645 trex-model-1.4.1/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.4.1/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2287 2024-04-22 08:11:53.000000 trex-model-1.4.1/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.324882 trex-model-1.4.1/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.4.1/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.353105 trex-model-1.4.1/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.4.1/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4893 2024-04-29 06:17:32.000000 trex-model-1.4.1/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3222 2024-05-02 05:47:34.000000 trex-model-1.4.1/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.4.1/trexmodel/models/datastore/app_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1645 2024-05-02 05:47:57.000000 trex-model-1.4.1/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15032 2024-04-25 01:46:35.000000 trex-model-1.4.1/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    55452 2024-05-02 05:48:07.000000 trex-model-1.4.1/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1453 2024-04-29 06:18:03.000000 trex-model-1.4.1/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8120 2024-05-02 05:34:16.000000 trex-model-1.4.1/trexmodel/models/datastore/import_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      876 2024-05-02 05:48:32.000000 trex-model-1.4.1/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8532 2024-05-02 05:48:57.000000 trex-model-1.4.1/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    41799 2024-05-02 05:34:22.000000 trex-model-1.4.1/trexmodel/models/datastore/lucky_draw_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12155 2024-05-02 05:34:31.000000 trex-model-1.4.1/trexmodel/models/datastore/marketing_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14631 2024-05-02 05:34:41.000000 trex-model-1.4.1/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    84856 2024-05-02 05:49:13.000000 trex-model-1.4.1/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22091 2024-05-02 05:34:47.000000 trex-model-1.4.1/trexmodel/models/datastore/message_model_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3892 2024-05-02 05:50:04.000000 trex-model-1.4.1/trexmodel/models/datastore/message_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.4.1/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19868 2024-05-02 05:50:11.000000 trex-model-1.4.1/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32178 2024-05-02 05:50:22.000000 trex-model-1.4.1/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    29746 2024-05-02 05:50:40.000000 trex-model-1.4.1/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38896 2024-05-02 05:50:57.000000 trex-model-1.4.1/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    49100 2024-05-02 05:51:10.000000 trex-model-1.4.1/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20631 2024-05-02 05:51:18.000000 trex-model-1.4.1/trexmodel/models/datastore/rating_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1876 2024-05-02 05:51:30.000000 trex-model-1.4.1/trexmodel/models/datastore/recruit_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    39734 2024-05-02 05:51:40.000000 trex-model-1.4.1/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16984 2024-05-02 05:35:09.000000 trex-model-1.4.1/trexmodel/models/datastore/redemption_catalogue_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16215 2024-05-02 05:51:58.000000 trex-model-1.4.1/trexmodel/models/datastore/referral_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7134 2024-05-02 05:35:18.000000 trex-model-1.4.1/trexmodel/models/datastore/reward_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    34841 2024-05-02 05:52:06.000000 trex-model-1.4.1/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.4.1/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8548 2024-05-02 05:52:23.000000 trex-model-1.4.1/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1332 2024-05-02 05:53:10.000000 trex-model-1.4.1/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      789 2024-05-02 05:52:53.000000 trex-model-1.4.1/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    41773 2024-05-02 02:32:39.000000 trex-model-1.4.1/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    23255 2024-05-02 05:53:27.000000 trex-model-1.4.1/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19217 2024-05-02 05:35:25.000000 trex-model-1.4.1/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10559 2024-05-02 05:53:36.000000 trex-model-1.4.1/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.4.1/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.4.1/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.4.1/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32618 2024-05-02 02:19:46.000000 trex-model-1.4.1/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.355189 trex-model-1.4.1/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.1/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.355934 trex-model-1.4.1/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.1/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.4.1/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:26.356681 trex-model-1.4.1/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.1/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2452 2024-05-02 05:53:44.000000 trex-model-1.4.1/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.501511 trex-model-1.4.2/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.4.2/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.4.2/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      643 2024-05-10 06:11:57.501200 trex-model-1.4.2/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.4.2/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-10 06:11:57.502406 trex-model-1.4.2/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2024-05-10 06:10:51.000000 trex-model-1.4.2/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.500732 trex-model-1.4.2/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      643 2024-05-10 06:11:57.000000 trex-model-1.4.2/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     2326 2024-05-10 06:11:57.000000 trex-model-1.4.2/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-10 06:11:57.000000 trex-model-1.4.2/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2024-05-10 06:11:57.000000 trex-model-1.4.2/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2024-05-10 06:11:57.000000 trex-model-1.4.2/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.454828 trex-model-1.4.2/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.4.2/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2287 2024-04-22 08:11:53.000000 trex-model-1.4.2/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.457268 trex-model-1.4.2/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.4.2/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.497098 trex-model-1.4.2/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.4.2/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4893 2024-04-29 06:17:32.000000 trex-model-1.4.2/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3222 2024-05-02 05:47:34.000000 trex-model-1.4.2/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.4.2/trexmodel/models/datastore/app_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1645 2024-05-02 05:47:57.000000 trex-model-1.4.2/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15032 2024-04-25 01:46:35.000000 trex-model-1.4.2/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    55630 2024-05-08 13:46:54.000000 trex-model-1.4.2/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1453 2024-04-29 06:18:03.000000 trex-model-1.4.2/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8120 2024-05-02 05:34:16.000000 trex-model-1.4.2/trexmodel/models/datastore/import_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      876 2024-05-02 05:48:32.000000 trex-model-1.4.2/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8532 2024-05-02 05:48:57.000000 trex-model-1.4.2/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    41799 2024-05-02 05:34:22.000000 trex-model-1.4.2/trexmodel/models/datastore/lucky_draw_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12155 2024-05-02 05:34:31.000000 trex-model-1.4.2/trexmodel/models/datastore/marketing_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14631 2024-05-02 05:34:41.000000 trex-model-1.4.2/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    87908 2024-05-09 06:03:00.000000 trex-model-1.4.2/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22091 2024-05-02 05:34:47.000000 trex-model-1.4.2/trexmodel/models/datastore/message_model_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3892 2024-05-02 05:50:04.000000 trex-model-1.4.2/trexmodel/models/datastore/message_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.4.2/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19868 2024-05-02 05:50:11.000000 trex-model-1.4.2/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32178 2024-05-02 05:50:22.000000 trex-model-1.4.2/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    29746 2024-05-02 05:50:40.000000 trex-model-1.4.2/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38896 2024-05-02 05:50:57.000000 trex-model-1.4.2/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    49100 2024-05-02 05:51:10.000000 trex-model-1.4.2/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20631 2024-05-02 05:51:18.000000 trex-model-1.4.2/trexmodel/models/datastore/rating_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1876 2024-05-02 05:51:30.000000 trex-model-1.4.2/trexmodel/models/datastore/recruit_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    39734 2024-05-02 05:51:40.000000 trex-model-1.4.2/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16984 2024-05-02 05:35:09.000000 trex-model-1.4.2/trexmodel/models/datastore/redemption_catalogue_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16215 2024-05-02 05:51:58.000000 trex-model-1.4.2/trexmodel/models/datastore/referral_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7134 2024-05-02 05:35:18.000000 trex-model-1.4.2/trexmodel/models/datastore/reward_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    34841 2024-05-02 05:52:06.000000 trex-model-1.4.2/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.4.2/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8548 2024-05-02 05:52:23.000000 trex-model-1.4.2/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1332 2024-05-02 05:53:10.000000 trex-model-1.4.2/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      789 2024-05-02 05:52:53.000000 trex-model-1.4.2/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    41773 2024-05-02 02:32:39.000000 trex-model-1.4.2/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    23255 2024-05-02 05:53:27.000000 trex-model-1.4.2/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19217 2024-05-02 05:35:25.000000 trex-model-1.4.2/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12264 2024-05-08 08:39:15.000000 trex-model-1.4.2/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.4.2/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.4.2/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.4.2/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32618 2024-05-02 02:19:46.000000 trex-model-1.4.2/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.498099 trex-model-1.4.2/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.2/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.498515 trex-model-1.4.2/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.2/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.4.2/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:57.499818 trex-model-1.4.2/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.2/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2452 2024-05-02 05:53:44.000000 trex-model-1.4.2/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-1.4.1/LICENSE` & `trex-model-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/PKG-INFO` & `trex-model-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-model
-Version: 1.4.1
+Version: 1.4.2
 Summary: TRex database module package
 Home-page: https://bitbucket.org/lokjac/trex-model
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-model-1.4.1/setup.py` & `trex-model-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.4.1',
+     version='1.4.2',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-1.4.1/trex_model.egg-info/PKG-INFO` & `trex-model-1.4.2/trex_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-model
-Version: 1.4.1
+Version: 1.4.2
 Summary: TRex database module package
 Home-page: https://bitbucket.org/lokjac/trex-model
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-model-1.4.1/trex_model.egg-info/SOURCES.txt` & `trex-model-1.4.2/trex_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/conf.py` & `trex-model-1.4.2/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/admin_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/app_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/app_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.4.2/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/customer_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/customer_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     
     fulltextsearch_field_name           = 'name'
     
     dict_properties     = ['name', 'mobile_phone', 'email', 'gender', 'birth_date', 'reference_code', 'merchant_reference_code',  
                            'tags_list', 'memberships_list', 'registered_merchant_acct', 'entitled_membership_reward_summary',
                            'reward_summary', 'entitled_voucher_summary', 'prepaid_summary', 'kpi_summary', 'entitled_lucky_draw_ticket_summary',
                            'entitled_birthday_reward_summary', 'tier_membership_key',
-                           'registered_outlet_key', 'registered_merchant_acct_key', 'registered_datetime', 'modified_datetime',
+                           'registered_outlet_key', 'merchant_account_key', 
+                           'registered_datetime', 'modified_datetime',
                            'registered_user_acct','referral_code',
                            
                            ]
     
     @property
     def is_any_entitled_voucher_active(self):
         
@@ -112,14 +113,19 @@
     def registered_merchant_acct(self):
         return MerchantAcct.fetch(self.merchant_acct.urlsafe())
     
     @property
     def registered_merchant_acct_key(self):
         if self.merchant_acct:
             return self.merchant_acct.urlsafe().decode("utf-8")
+        
+    @property
+    def merchant_account_key(self):
+        if self.merchant_acct:
+            return self.merchant_acct.urlsafe().decode("utf-8")    
     
     @property
     def registered_outlet(self):
         if self.outlet:
             return Outlet.fetch(self.outlet.urlsafe())
     
     @property
```

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/import_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/import_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.4.2/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/loyalty_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/lucky_draw_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/lucky_draw_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/marketing_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/marketing_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/membership_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/membership_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/merchant_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1888,8 +1888,80 @@
     
     @staticmethod
     def remove_file(banner_file, bucket):
         
         old_logo_blob = bucket.get_blob(banner_file.banner_file_storage_filename) 
         if old_logo_blob:
             old_logo_blob.delete()
-            banner_file.delete()    
+            banner_file.delete()   
+            
+class MerchantNewsFile(BaseNModel, DictModel):
+    '''
+    Merchant Account as ancestor
+    '''
+    label                         = ndb.StringProperty(required=False)
+    desc                          = ndb.StringProperty(required=False)
+    news_text                     = ndb.StringProperty(required=False)
+    
+    news_file_type                = ndb.StringProperty(required=True)
+    news_file_public_url          = ndb.StringProperty(required=True)
+    news_file_storage_filename    = ndb.StringProperty(required=True)
+    start_date                    = ndb.DateProperty(required=True)
+    end_date                      = ndb.DateProperty(required=True)
+    
+    
+    dict_properties = ['news_file_public_url', 'news_file_storage_filename', 'news_file_type', 'label', 'desc', 'news_text', 'start_date', 'end_date']
+    
+    @staticmethod
+    def list_by_merchant_acct(merchant_acct):
+        result = MerchantNewsFile.query(ancestor=merchant_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)
+        return result
+    
+    @staticmethod
+    def create(merchant_acct, label=None, desc=None, news_text=None):
+        news_file = MerchantNewsFile(
+                            parent      = merchant_acct.create_ndb_key(),
+                            label       = label,
+                            desc        = desc,
+                            news_text   = news_text,
+                            )
+        
+        news_file.put()
+    
+    @staticmethod
+    def upload_file(merchant_news, uploading_file, merchant_acct, bucket, news_file_type=None):
+        file_prefix                         = random_string(8)
+        news_file_storage_filename          = 'merchant/'+merchant_acct.key_in_str+'/news/'+file_prefix+'-'+uploading_file.filename
+        blob                                = bucket.blob(news_file_storage_filename)
+        
+        logger.debug('news_file_storage_filename=%s', news_file_storage_filename)
+        
+        blob.upload_from_string(
+                uploading_file.read(),
+                content_type=uploading_file.content_type
+            )
+        
+        uploaded_url        = blob.public_url
+        
+        logger.debug('uploaded_url=%s', uploaded_url)
+        logger.debug('news_file_type=%s', news_file_type)
+        
+        if is_not_empty(merchant_news.news_file_storage_filename):
+            old_logo_blob = bucket.get_blob(merchant_news.news_file_storage_filename)
+            if old_logo_blob:
+                old_logo_blob.delete()
+            
+        
+        merchant_news.news_file_public_url          = uploaded_url
+        merchant_news.news_file_storage_filename    = news_file_storage_filename
+        merchant_news.news_file_type                = news_file_type
+        
+        
+        merchant_news.put()
+    
+    @staticmethod
+    def remove_file(news_file, bucket):
+        
+        old_logo_blob = bucket.get_blob(news_file.news_file_storage_filename) 
+        if old_logo_blob:
+            old_logo_blob.delete()
+            news_file.delete()
```

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/message_model_helper.py` & `trex-model-1.4.2/trexmodel/models/datastore/message_model_helper.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/message_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/message_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.4.2/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/ndb_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/pos_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/pos_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/prepaid_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/product_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/program_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/program_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/rating_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/rating_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/recruit_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/recruit_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/redeem_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/redemption_catalogue_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/redemption_catalogue_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/referral_program_model.py` & `trex-model-1.4.2/trexmodel/models/datastore/referral_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/reward_model_helpers.py` & `trex-model-1.4.2/trexmodel/models/datastore/reward_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/reward_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/reward_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.4.2/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/system_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/task_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/test_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/transaction_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/user_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.4.2/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/program_conf.py` & `trex-model-1.4.2/trexmodel/program_conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.4.1/trexmodel/utils/model/model_util.py` & `trex-model-1.4.2/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

