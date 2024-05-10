# Comparing `tmp/orbitkit-0.6.4.tar.gz` & `tmp/orbitkit-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.6.4.tar", last modified: Mon Apr 29 03:18:56 2024, max compression
+gzip compressed data, was "dist/orbitkit-0.6.5.tar", last modified: Fri May 10 07:50:36 2024, max compression
```

## Comparing `orbitkit-0.6.4.tar` & `orbitkit-0.6.5.tar`

### file list

```diff
@@ -1,47 +1,55 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.4/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.4/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-04-29 03:18:56.000000 orbitkit-0.6.4/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.4/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2024-04-29 03:18:06.000000 orbitkit-0.6.4/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.4/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.4/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.4/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.4/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.4/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit/pdf_embedding/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.4/orbitkit/pdf_embedding/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.4/orbitkit/pdf_embedding/pdf_txt_embedding.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
--rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_extractor_azure.py
--rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_extractor_orbit.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.4/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.4/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.4/orbitkit/util/util_aliyun.py
--rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.4/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.4/orbitkit/util/util_aws_s3_wrapper.py
--rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.4/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.4/orbitkit/util/util_html.py
--rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.4/orbitkit/util/util_md5.py
--rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.4/orbitkit/util/util_selenium.py
--rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.4/orbitkit/util/util_simple_timer.py
--rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.4/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.4/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1119 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       74 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2024-04-29 03:18:56.000000 orbitkit-0.6.4/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2024-04-29 03:18:56.000000 orbitkit-0.6.4/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.4/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:36.000000 orbitkit-0.6.5/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.5/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.5/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-10 07:50:35.000000 orbitkit-0.6.5/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.5/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-10 07:19:16.000000 orbitkit-0.6.5/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.5/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.5/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.5/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.5/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.5/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/pdf_embedding/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.5/orbitkit/pdf_embedding/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.5/orbitkit/pdf_embedding/pdf_txt_embedding.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+-rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_extractor_azure.py
+-rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_extractor_orbit.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/
+-rw-r--r--   0 crown      (501) staff       (20)     3344 2024-05-10 07:36:30.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/base.py
+-rw-r--r--   0 crown      (501) staff       (20)     4270 2024-05-10 07:36:30.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/cloud_provider.py
+-rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)     8060 2024-05-10 07:49:09.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/extractors.py
+-rw-r--r--   0 crown      (501) staff       (20)      687 2024-05-10 07:36:30.000000 orbitkit-0.6.5/orbitkit/pdf_extractor_simple/utils.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.5/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.5/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.5/orbitkit/util/util_aliyun.py
+-rw-r--r--   0 crown      (501) staff       (20)     1078 2024-05-10 07:19:16.000000 orbitkit-0.6.5/orbitkit/util/util_aliyun_oss_simple.py
+-rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.5/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.5/orbitkit/util/util_aws_s3_wrapper.py
+-rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.5/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.5/orbitkit/util/util_html.py
+-rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.5/orbitkit/util/util_md5.py
+-rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.5/orbitkit/util/util_selenium.py
+-rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.5/orbitkit/util/util_simple_timer.py
+-rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.5/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.5/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1414 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-10 07:50:35.000000 orbitkit-0.6.5/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-10 07:50:36.000000 orbitkit-0.6.5/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.5/setup.py
```

### Comparing `orbitkit-0.6.4/LICENSE` & `orbitkit-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/PKG-INFO` & `orbitkit-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.4
+Version: 0.6.5
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.4/README.md` & `orbitkit-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/id_srv/id_gen.py` & `orbitkit-0.6.5/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/lark_send/lark.py` & `orbitkit-0.6.5/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_embedding/pdf_txt_embedding.py` & `orbitkit-0.6.5/orbitkit/pdf_embedding/pdf_txt_embedding.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_extractor/exceptions.py` & `orbitkit-0.6.5/orbitkit/pdf_extractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_extractor_azure.py` & `orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_extractor_azure.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/pdf_extractor/pdf_extractor_orbit.py` & `orbitkit-0.6.5/orbitkit/pdf_extractor/pdf_extractor_orbit.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/__init__.py` & `orbitkit-0.6.5/orbitkit/util/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/common.py` & `orbitkit-0.6.5/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_aws.py` & `orbitkit-0.6.5/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_aws_s3_wrapper.py` & `orbitkit-0.6.5/orbitkit/util/util_aws_s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_date.py` & `orbitkit-0.6.5/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_md5.py` & `orbitkit-0.6.5/orbitkit/util/util_md5.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_selenium.py` & `orbitkit-0.6.5/orbitkit/util/util_selenium.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_str.py` & `orbitkit-0.6.5/orbitkit/util/util_str.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit/util/util_type_mapping.py` & `orbitkit-0.6.5/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.4/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.6.5/orbitkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.4
+Version: 0.6.5
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.4/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.6.5/orbitkit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,17 +19,24 @@
 orbitkit/pdf_extractor/__init__.py
 orbitkit/pdf_extractor/exceptions.py
 orbitkit/pdf_extractor/pdf_block_extractor_base.py
 orbitkit/pdf_extractor/pdf_block_extractor_v1.py
 orbitkit/pdf_extractor/pdf_block_extractor_v2.py
 orbitkit/pdf_extractor/pdf_extractor_azure.py
 orbitkit/pdf_extractor/pdf_extractor_orbit.py
+orbitkit/pdf_extractor_simple/__init__.py
+orbitkit/pdf_extractor_simple/base.py
+orbitkit/pdf_extractor_simple/cloud_provider.py
+orbitkit/pdf_extractor_simple/exceptions.py
+orbitkit/pdf_extractor_simple/extractors.py
+orbitkit/pdf_extractor_simple/utils.py
 orbitkit/util/__init__.py
 orbitkit/util/common.py
 orbitkit/util/util_aliyun.py
+orbitkit/util/util_aliyun_oss_simple.py
 orbitkit/util/util_aws.py
 orbitkit/util/util_aws_s3_wrapper.py
 orbitkit/util/util_date.py
 orbitkit/util/util_html.py
 orbitkit/util/util_md5.py
 orbitkit/util/util_selenium.py
 orbitkit/util/util_simple_timer.py
```

### Comparing `orbitkit-0.6.4/setup.py` & `orbitkit-0.6.5/setup.py`

 * *Files identical despite different names*

