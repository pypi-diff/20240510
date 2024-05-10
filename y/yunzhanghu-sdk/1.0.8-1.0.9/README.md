# Comparing `tmp/yunzhanghu_sdk-1.0.8.tar.gz` & `tmp/yunzhanghu_sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunzhanghu_sdk-1.0.8.tar", last modified: Mon Oct 30 07:54:35 2023, max compression
+gzip compressed data, was "yunzhanghu_sdk-1.0.9.tar", last modified: Mon Dec 11 09:56:50 2023, max compression
```

## Comparing `yunzhanghu_sdk-1.0.8.tar` & `yunzhanghu_sdk-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-10-30 07:54:35.738375 yunzhanghu_sdk-1.0.8/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1071 2023-08-07 11:21:23.000000 yunzhanghu_sdk-1.0.8/LICENSE
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       39 2023-03-10 08:51:50.000000 yunzhanghu_sdk-1.0.8/MANIFEST.in
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4018 2023-10-30 07:54:35.738148 yunzhanghu_sdk-1.0.8/PKG-INFO
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     7088 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/README.md
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-10-30 07:54:35.738461 yunzhanghu_sdk-1.0.8/setup.cfg
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      885 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.8/setup.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-10-30 07:54:35.705772 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       41 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/__init__.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-10-30 07:54:35.711788 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       13 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/__init__.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-10-30 07:54:35.724539 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       10 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/__init__.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2469 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/apiusersign_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3979 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/authentication_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1115 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1648 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3511 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/dataservice_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1930 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/h5usersign_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3415 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/invoice_client.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-10-30 07:54:35.737847 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       12 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/__init__.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5422 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/apiusersign.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8459 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/authentication.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5882 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8034 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    14716 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/dataservice.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5499 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/h5usersign.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    13872 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/invoice.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    25959 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/payment.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2257 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/tax.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3798 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/uploadusersign.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5028 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/payment_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1079 2023-08-22 07:28:11.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/tax_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1183 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/uploadusersign_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3010 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/base.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1516 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/config.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     6130 2023-09-07 07:53:46.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/message.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      157 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/utils.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-10-30 07:54:35.709039 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4018 2023-10-30 07:54:35.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1441 2023-10-30 07:54:35.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)        1 2023-10-30 07:54:35.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-10-30 07:54:35.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/requires.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       15 2023-10-30 07:54:35.000000 yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/top_level.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3734 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.8/云账户SDK-for-Python-pypi.md
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-12-11 09:56:50.346117 yunzhanghu_sdk-1.0.9/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1071 2023-08-07 11:21:23.000000 yunzhanghu_sdk-1.0.9/LICENSE
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       39 2023-03-10 08:51:50.000000 yunzhanghu_sdk-1.0.9/MANIFEST.in
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4018 2023-12-11 09:56:50.345974 yunzhanghu_sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     7087 2023-12-11 09:54:15.000000 yunzhanghu_sdk-1.0.9/README.md
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-12-11 09:56:50.346166 yunzhanghu_sdk-1.0.9/setup.cfg
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      885 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.9/setup.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-12-11 09:56:50.285712 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       41 2023-12-11 09:54:15.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/__init__.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-12-11 09:56:50.303395 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       13 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/__init__.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-12-11 09:56:50.315142 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       10 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/__init__.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2469 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/apiusersign_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3979 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/authentication_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1115 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1648 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3511 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/dataservice_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1930 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/h5usersign_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3415 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/invoice_client.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-12-11 09:56:50.345690 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       12 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/__init__.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5422 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/apiusersign.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8459 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/authentication.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5882 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8034 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    14716 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/dataservice.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5499 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/h5usersign.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    13872 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/invoice.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    32280 2023-12-11 09:54:15.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/payment.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2257 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/tax.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3798 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/uploadusersign.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5467 2023-12-11 09:54:15.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/payment_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1079 2023-08-22 07:28:11.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/tax_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1183 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/uploadusersign_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3010 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/base.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1516 2023-10-30 07:18:34.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/config.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     6130 2023-09-07 07:53:46.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/message.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      157 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/utils.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-12-11 09:56:50.300797 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4018 2023-12-11 09:56:50.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1441 2023-12-11 09:56:50.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)        1 2023-12-11 09:56:50.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-12-11 09:56:50.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/requires.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       15 2023-12-11 09:56:50.000000 yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3734 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.9/云账户SDK-for-Python-pypi.md
```

### Comparing `yunzhanghu_sdk-1.0.8/LICENSE` & `yunzhanghu_sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/PKG-INFO` & `yunzhanghu_sdk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunzhanghu_sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: 云账户官方 SDK for Python
 Home-page: UNKNOWN
 Author: yunzhanghu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `yunzhanghu_sdk-1.0.8/README.md` & `yunzhanghu_sdk-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     )
     # 建议自定义并将 request-id 记录在日志中
     # request.request_id = "XXXXX"
     client = PaymentClient(config)
 
     # request-id：请求 ID，请求的唯一标识
     # 建议平台企业自定义 request-id，并记录在日志中，便于问题发现及排查
-    # 如平台企业未自定义 request-id，将使用 SDK 中的 UUID 方法自动生成。注意：UUID 方法生成的 request-id 不能保证全局唯一，推荐自定义
+    # 如未自定义 request-id，将使用 SDK 中的 UUID 方法自动生成。注意：UUID 方法生成的 request-id 不能保证全局唯一，推荐自定义 request-id
     request.request_id = "requestId"
     try:
         resp =  client.get_order(request)
         if resp.code == "0000":
             # 操作成功
             print("操作成功 ", resp.data)
         else:
```

### Comparing `yunzhanghu_sdk-1.0.8/setup.py` & `yunzhanghu_sdk-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/apiusersign_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/apiusersign_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/authentication_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/authentication_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/dataservice_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/dataservice_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/h5usersign_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/h5usersign_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/invoice_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/invoice_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/apiusersign.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/apiusersign.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/authentication.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/authentication.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/dataservice.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/dataservice.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/h5usersign.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/h5usersign.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/invoice.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/invoice.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/payment.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/payment.py`

 * *Files 8% similar despite different names*

```diff
@@ -871,15 +871,15 @@
         self.bank_name = bank_name
         self.project_id = project_id
         self.user_id = user_id
 
 
 class CreateBatchOrderRequest(BaseRequest):
     """
-    批量下单请求-请求
+    批次下单请求-请求
 
     :type batch_id: string
     :param batch_id: 平台企业批次号
 
     :type dealer_id: string
     :param dealer_id: 平台企业 ID
 
@@ -926,15 +926,15 @@
         self.total_count = total_count
         self.mode = mode
         self.order_list = order_list
 
 
 class BatchOrderInfo(BaseRequest):
     """
-    批量下单订单信息-响应
+    批次下单订单信息-响应
 
     :type order_id: string
     :param order_id: 平台企业订单号
 
     :type real_name: string
     :param real_name: 姓名
 
@@ -986,15 +986,15 @@
         self.pay = pay
         self.pay_remark = pay_remark
         self.notify_url = notify_url
 
 
 class CreateBatchOrderResponse(BaseRequest):
     """
-    批量下单返回-响应
+    批次下单返回-响应
 
     :type batch_id: string
     :param batch_id: 平台企业批次号
 
     :type result_list: list
     :param result_list: 订单结果列表
     """
@@ -1006,35 +1006,65 @@
         super().__init__()
         self.batch_id = batch_id
         self.result_list = result_list
 
 
 class BatchOrderResult(BaseRequest):
     """
-    批量下单返回订单信息-响应
+    批次下单返回订单信息-响应
 
     :type order_id: string
     :param order_id: 平台企业订单号
 
     :type ref: string
     :param ref: 综合服务平台流水号
 
     :type pay: string
     :param pay: 订单金额
+
+    :type status: string
+    :param status: 下单状态
+
+    :type error_reasons: list
+    :param error_reasons: 下单失败原因
     """
     def __init__(
         self,
         order_id=None,
         ref=None,
-        pay=None
+        pay=None,
+        status=None,
+        error_reasons=None
     ):
         super().__init__()
         self.order_id = order_id
         self.ref = ref
         self.pay = pay
+        self.status = status
+        self.error_reasons = error_reasons
+
+
+class BatchOrderErrorReasons(BaseRequest):
+    """
+    下单失败原因信息-响应
+
+    :type error_code: string
+    :param error_code: 不允许下单原因码
+
+    :type error_message: string
+    :param error_message: 不允许下单原因描述
+    """
+    def __init__(
+        self,
+        error_code=None,
+        error_message=None
+    ):
+        super().__init__()
+        self.error_code = error_code
+        self.error_message = error_message
 
 
 class ConfirmBatchOrderRequest(BaseRequest):
     """
     批次确认请求-请求
 
     :type batch_id: string
@@ -1065,14 +1095,229 @@
 
 class ConfirmBatchOrderResponse(BaseRequest):
     """
     批次确认返回-响应
     """
 
 
+class QueryBatchOrderRequest(BaseRequest):
+    """
+    查询批次订单信息请求-请求
+
+    :type batch_id: string
+    :param batch_id: 平台企业批次号
+
+    :type dealer_id: string
+    :param dealer_id: 平台企业 ID
+    """
+    def __init__(
+        self,
+        batch_id=None,
+        dealer_id=None
+    ):
+        super().__init__()
+        self.batch_id = batch_id
+        self.dealer_id = dealer_id
+
+
+class QueryBatchOrderResponse(BaseRequest):
+    """
+    查询批次订单信息返回-响应
+
+    :type broker_id: string
+    :param broker_id: 综合服务主体 ID
+
+    :type dealer_id: string
+    :param dealer_id: 平台企业 ID
+
+    :type batch_id: string
+    :param batch_id: 平台企业批次号
+
+    :type total_count: string
+    :param total_count: 总笔数
+
+    :type total_pay: string
+    :param total_pay: 订单总金额
+
+    :type channel: string
+    :param channel: 支付路径
+
+    :type batch_status: string
+    :param batch_status: 批次状态码
+
+    :type batch_status_message: string
+    :param batch_status_message: 批次状态码描述
+
+    :type batch_received_time: string
+    :param batch_received_time: 批次接收时间
+
+    :type order_list: list
+    :param order_list: 批次订单列表
+    """
+    def __init__(
+        self,
+        broker_id=None,
+        dealer_id=None,
+        batch_id=None,
+        total_count=None,
+        total_pay=None,
+        channel=None,
+        batch_status=None,
+        batch_status_message=None,
+        batch_received_time=None,
+        order_list=None
+    ):
+        super().__init__()
+        self.broker_id = broker_id
+        self.dealer_id = dealer_id
+        self.batch_id = batch_id
+        self.total_count = total_count
+        self.total_pay = total_pay
+        self.channel = channel
+        self.batch_status = batch_status
+        self.batch_status_message = batch_status_message
+        self.batch_received_time = batch_received_time
+        self.order_list = order_list
+
+
+class QueryBatchOrderInfo(BaseRequest):
+    """
+    查询批次订单信息订单详情-响应
+
+    :type order_id: string
+    :param order_id: 平台企业订单号
+
+    :type pay: string
+    :param pay: 订单金额
+
+    :type broker_id: string
+    :param broker_id: 综合服务主体 ID
+
+    :type dealer_id: string
+    :param dealer_id: 平台企业 ID
+
+    :type real_name: string
+    :param real_name: 姓名
+
+    :type card_no: string
+    :param card_no: 收款人账号
+
+    :type id_card: string
+    :param id_card: 身份证号码
+
+    :type phone_no: string
+    :param phone_no: 手机号
+
+    :type status: string
+    :param status: 订单状态码
+
+    :type status_detail: string
+    :param status_detail: 订单详情状态码
+
+    :type status_message: string
+    :param status_message: 订单状态码描述
+
+    :type status_detail_message: string
+    :param status_detail_message: 订单详情状态码描述
+
+    :type broker_amount: string
+    :param broker_amount: 综合服务主体支付金额
+
+    :type ref: string
+    :param ref: 综合服务平台流水号
+
+    :type broker_bank_bill: string
+    :param broker_bank_bill: 支付交易流水号
+
+    :type withdraw_platform: string
+    :param withdraw_platform: 支付路径
+
+    :type created_at: string
+    :param created_at: 订单接收时间
+
+    :type finished_time: string
+    :param finished_time: 订单完成时间
+
+    :type broker_fee: string
+    :param broker_fee: 综合服务主体加成服务费
+
+    :type broker_real_fee: string
+    :param broker_real_fee: 余额账户支出加成服务费
+
+    :type broker_deduct_fee: string
+    :param broker_deduct_fee: 加成服务费抵扣金额
+
+    :type pay_remark: string
+    :param pay_remark: 订单备注
+
+    :type user_fee: string
+    :param user_fee: 用户加成服务费
+
+    :type bank_name: string
+    :param bank_name: 银行名称
+
+    :type project_id: string
+    :param project_id: 业务线标识
+    """
+    def __init__(
+        self,
+        order_id=None,
+        pay=None,
+        broker_id=None,
+        dealer_id=None,
+        real_name=None,
+        card_no=None,
+        id_card=None,
+        phone_no=None,
+        status=None,
+        status_detail=None,
+        status_message=None,
+        status_detail_message=None,
+        broker_amount=None,
+        ref=None,
+        broker_bank_bill=None,
+        withdraw_platform=None,
+        created_at=None,
+        finished_time=None,
+        broker_fee=None,
+        broker_real_fee=None,
+        broker_deduct_fee=None,
+        pay_remark=None,
+        user_fee=None,
+        bank_name=None,
+        project_id=None
+    ):
+        super().__init__()
+        self.order_id = order_id
+        self.pay = pay
+        self.broker_id = broker_id
+        self.dealer_id = dealer_id
+        self.real_name = real_name
+        self.card_no = card_no
+        self.id_card = id_card
+        self.phone_no = phone_no
+        self.status = status
+        self.status_detail = status_detail
+        self.status_message = status_message
+        self.status_detail_message = status_detail_message
+        self.broker_amount = broker_amount
+        self.ref = ref
+        self.broker_bank_bill = broker_bank_bill
+        self.withdraw_platform = withdraw_platform
+        self.created_at = created_at
+        self.finished_time = finished_time
+        self.broker_fee = broker_fee
+        self.broker_real_fee = broker_real_fee
+        self.broker_deduct_fee = broker_deduct_fee
+        self.pay_remark = pay_remark
+        self.user_fee = user_fee
+        self.bank_name = bank_name
+        self.project_id = project_id
+
+
 class CancelBatchOrderRequest(BaseRequest):
     """
     批次撤销请求-请求
 
     :type batch_id: string
     :param batch_id: 平台企业批次号
```

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/tax.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/tax.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/model/uploadusersign.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/model/uploadusersign.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/payment_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/payment_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,27 @@
     
         :return: ConfirmBatchOrderResponse
         """
         return self._post(
             "/api/payment/v1/confirm-batch", 
             request.request_id, Utils.copy_dict(request.__dict__)
         )
+    
+    def query_batch_order(self, request: QueryBatchOrderRequest):
+        """ 查询批次订单信息
+   
+        :type request: QueryBatchOrderRequest
+        :param request: the QueryBatchOrderRequest request parameters class.
+    
+        :return: QueryBatchOrderResponse
+        """
+        return self._get(
+            "/api/payment/v1/query-batch", 
+            request.request_id, Utils.copy_dict(request.__dict__)
+        )
 
     def cancel_batch_order(self, request: CancelBatchOrderRequest):
         """ 批次撤销
    
         :type request: CancelBatchOrderRequest
         :param request: the CancelBatchOrderRequest request parameters class.
```

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/tax_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/tax_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/api/uploadusersign_client.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/api/uploadusersign_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/client/base.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/client/base.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/config.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/config.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk/message.py` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk/message.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/PKG-INFO` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunzhanghu-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: 云账户官方 SDK for Python
 Home-page: UNKNOWN
 Author: yunzhanghu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `yunzhanghu_sdk-1.0.8/yunzhanghu_sdk.egg-info/SOURCES.txt` & `yunzhanghu_sdk-1.0.9/yunzhanghu_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.8/云账户SDK-for-Python-pypi.md` & `yunzhanghu_sdk-1.0.9/云账户SDK-for-Python-pypi.md`

 * *Files identical despite different names*

