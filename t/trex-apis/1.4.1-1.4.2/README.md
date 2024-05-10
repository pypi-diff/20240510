# Comparing `tmp/trex-apis-1.4.1.tar.gz` & `tmp/trex-apis-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.4.1.tar", last modified: Mon May  6 09:16:13 2024, max compression
+gzip compressed data, was "trex-apis-1.4.2.tar", last modified: Fri May 10 06:12:08 2024, max compression
```

## Comparing `trex-apis-1.4.1.tar` & `trex-apis-1.4.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.210136 trex-apis-1.4.1/
--rw-r--r--   0 jacklok    (501) staff       (20)      547 2024-05-06 09:16:13.209949 trex-apis-1.4.1/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.4.1/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 09:16:13.210985 trex-apis-1.4.1/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      808 2024-05-06 09:15:24.000000 trex-apis-1.4.1/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.209149 trex-apis-1.4.1/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      547 2024-05-06 09:16:13.000000 trex-apis-1.4.1/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1658 2024-05-06 09:16:13.000000 trex-apis-1.4.1/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 09:16:13.000000 trex-apis-1.4.1/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       66 2024-05-06 09:16:13.000000 trex-apis-1.4.1/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-05-06 09:16:13.000000 trex-apis-1.4.1/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.177040 trex-apis-1.4.1/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.4.1/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1474 2024-05-04 13:45:53.000000 trex-apis-1.4.1/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.197755 trex-apis-1.4.1/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.4.1/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4562 2024-05-05 09:45:58.000000 trex-apis-1.4.1/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6424 2024-04-30 09:04:02.000000 trex-apis-1.4.1/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    44879 2024-04-30 09:15:08.000000 trex-apis-1.4.1/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.4.1/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.4.1/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14687 2024-04-29 08:25:29.000000 trex-apis-1.4.1/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14233 2024-04-29 09:09:32.000000 trex-apis-1.4.1/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    29768 2024-05-04 14:17:59.000000 trex-apis-1.4.1/trexapi/controllers/merchant_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7522 2024-05-05 09:48:00.000000 trex-apis-1.4.1/trexapi/controllers/message_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.4.1/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.4.1/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.4.1/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.4.1/trexapi/controllers/prepaid_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.4.1/trexapi/controllers/rating_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10026 2024-04-29 08:25:02.000000 trex-apis-1.4.1/trexapi/controllers/redemption_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27186 2024-05-05 10:03:43.000000 trex-apis-1.4.1/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-05-05 10:07:29.000000 trex-apis-1.4.1/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.4.1/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    97590 2024-05-06 09:12:51.000000 trex-apis-1.4.1/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.4.1/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16927 2024-05-05 10:11:04.000000 trex-apis-1.4.1/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.198872 trex-apis-1.4.1/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.4.1/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.4.1/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.202536 trex-apis-1.4.1/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.4.1/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7539 2024-04-24 10:25:39.000000 trex-apis-1.4.1/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.4.1/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.4.1/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.4.1/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.204714 trex-apis-1.4.1/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.4.1/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      913 2024-04-22 02:25:05.000000 trex-apis-1.4.1/trexapi/libs/api_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.4.1/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:16:13.207012 trex-apis-1.4.1/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.4.1/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2984 2024-05-05 10:11:27.000000 trex-apis-1.4.1/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.4.1/trexapi/utils/push_notification_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7293 2024-05-02 06:28:02.000000 trex-apis-1.4.1/trexapi/utils/redemption_catalogue_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)    79102 2024-05-06 09:13:00.000000 trex-apis-1.4.1/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.791378 trex-apis-1.4.2/
+-rw-r--r--   0 jacklok    (501) staff       (20)      547 2024-05-10 06:12:08.791262 trex-apis-1.4.2/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.4.2/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-10 06:12:08.792214 trex-apis-1.4.2/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      808 2024-05-10 06:10:57.000000 trex-apis-1.4.2/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.790680 trex-apis-1.4.2/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      547 2024-05-10 06:12:08.000000 trex-apis-1.4.2/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1658 2024-05-10 06:12:08.000000 trex-apis-1.4.2/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-10 06:12:08.000000 trex-apis-1.4.2/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       66 2024-05-10 06:12:08.000000 trex-apis-1.4.2/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-05-10 06:12:08.000000 trex-apis-1.4.2/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.750404 trex-apis-1.4.2/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.4.2/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1474 2024-05-04 13:45:53.000000 trex-apis-1.4.2/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.772648 trex-apis-1.4.2/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.4.2/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4562 2024-05-05 09:45:58.000000 trex-apis-1.4.2/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6739 2024-05-10 02:32:28.000000 trex-apis-1.4.2/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    44787 2024-05-08 13:46:41.000000 trex-apis-1.4.2/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.4.2/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.4.2/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14687 2024-04-29 08:25:29.000000 trex-apis-1.4.2/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14233 2024-04-29 09:09:32.000000 trex-apis-1.4.2/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    29768 2024-05-08 13:45:32.000000 trex-apis-1.4.2/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7522 2024-05-05 09:48:00.000000 trex-apis-1.4.2/trexapi/controllers/message_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.4.2/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.4.2/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.4.2/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.4.2/trexapi/controllers/prepaid_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.4.2/trexapi/controllers/rating_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10026 2024-04-29 08:25:02.000000 trex-apis-1.4.2/trexapi/controllers/redemption_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27186 2024-05-05 10:03:43.000000 trex-apis-1.4.2/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-05-05 10:07:29.000000 trex-apis-1.4.2/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.4.2/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    97590 2024-05-06 09:12:51.000000 trex-apis-1.4.2/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.4.2/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16927 2024-05-05 10:11:04.000000 trex-apis-1.4.2/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.774898 trex-apis-1.4.2/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.4.2/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.4.2/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.780296 trex-apis-1.4.2/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.4.2/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7539 2024-04-24 10:25:39.000000 trex-apis-1.4.2/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.4.2/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.4.2/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.4.2/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.784176 trex-apis-1.4.2/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.4.2/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      913 2024-04-22 02:25:05.000000 trex-apis-1.4.2/trexapi/libs/api_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.4.2/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:12:08.788594 trex-apis-1.4.2/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.4.2/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2984 2024-05-05 10:11:27.000000 trex-apis-1.4.2/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.4.2/trexapi/utils/push_notification_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7293 2024-05-02 06:28:02.000000 trex-apis-1.4.2/trexapi/utils/redemption_catalogue_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    79102 2024-05-06 09:13:00.000000 trex-apis-1.4.2/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.4.1/PKG-INFO` & `trex-apis-1.4.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-apis
-Version: 1.4.1
+Version: 1.4.2
 Summary: TRex APIs package
 Home-page: https://bitbucket.org/lokjac/trex-apis
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-apis-1.4.1/setup.py` & `trex-apis-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.4.1',
+     version='1.4.2',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.4.1/trex_apis.egg-info/PKG-INFO` & `trex-apis-1.4.2/trex_apis.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-apis
-Version: 1.4.1
+Version: 1.4.2
 Summary: TRex APIs package
 Home-page: https://bitbucket.org/lokjac/trex-apis
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-apis-1.4.1/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.4.2/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/conf.py` & `trex-apis-1.4.2/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/app_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/app_api_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     logger.debug('---app_setting---')
     
     banner_file_list = []
     db_client = create_db_client(caller_info="app_setting")
     with db_client.context():
         
         result_listing = AppBannerFile.list()
-        logger.debug('result_listing=%s', result_listing)
+        
                 
         if result_listing:
             for banner_file in result_listing:
                 #banner_file_list.append(banner_file.to_dict(dict_properties=['banner_file_public_url','sequence'], show_key=False))
                 banner_file_list.append({
                                         'image_url': banner_file.banner_file_public_url,
                                         'sequence': banner_file.sequence,
@@ -113,25 +113,32 @@
                         'banners': banner_file_list,
                         'message_box_settings'  : {
                                                 'max_read_count'                : 2,
                                                 'read_interval_in_second'       : 60,
                                                 'list_message_pagination_limit' : 10,
                                                 },
                         'account_settings'      :{
-                                                'login_session_length_in_hour'  : 96,
+                                                'login_session_length_in_hour'  : 120,
                                                 },
-                        'outlet_order_enabled'  : False,
+                        'outlet_order_enabled'          : False,
+                        'cache_settings': {
+                            
+                                            'cache_length_in_minute'        : 60,
+                                            'login_session_length_in_hour'  : 120,
+                                        }
+                        
                         
         
                     }
     '''
     return create_rest_message(status_code=StatusCode.OK,
                                                **app_settings,
                                                )
     '''
+    logger.debug('app_settings=%s', app_settings)
     return app_settings
 
 @app_api_bp.route('/promotions', methods=['GET'])
 def list_app_promotions():
     logger.debug('---list_app_promotions---')
     result_listing = [
```

### Comparing `trex-apis-1.4.1/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/customer_api_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,14 @@
                 user_details = customer.registered_user_acct
                 customer_details_dict = customer.to_dict(
                                                     date_format="%d-%m-%Y", 
                                                     datetime_format="%d-%m-%Y %H:%M:%S",
                                                     excluded_dict_properties = [
                                                             'registered_merchant_acct', 
                                                             'memberships_list', 
-                                                            'registered_merchant_acct_key',
                                                             'tier_membership_key',
                                                             
                                                             ],
                                                     )
                 customer_details_dict['customer_key']               = customer.key_in_str
                 customer_details_dict['is_email_verified']          = user_details.is_email_verified
                 customer_details_dict['is_mobile_phone_verified']   = user_details.is_mobile_phone_verified
```

### Comparing `trex-apis-1.4.1/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/merchant_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/merchant_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/message_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/message_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/prepaid_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/prepaid_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/rating_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/rating_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/redemption_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/redemption_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/user_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/user_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.4.2/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/decorators/api_decorators.py` & `trex-apis-1.4.2/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/forms/customer_api_forms.py` & `trex-apis-1.4.2/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/forms/reward_api_forms.py` & `trex-apis-1.4.2/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/forms/sales_api_forms.py` & `trex-apis-1.4.2/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/forms/user_api_forms.py` & `trex-apis-1.4.2/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/libs/api_decorator.py` & `trex-apis-1.4.2/trexapi/libs/api_decorator.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.4.2/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/utils/api_helpers.py` & `trex-apis-1.4.2/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/utils/redemption_catalogue_helper.py` & `trex-apis-1.4.2/trexapi/utils/redemption_catalogue_helper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.4.1/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.4.2/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

