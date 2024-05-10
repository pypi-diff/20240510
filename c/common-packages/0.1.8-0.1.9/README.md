# Comparing `tmp/common_packages-0.1.8.tar.gz` & `tmp/common_packages-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_packages-0.1.8.tar", last modified: Thu Dec  7 06:59:05 2023, max compression
+gzip compressed data, was "common_packages-0.1.9.tar", last modified: Wed Dec 13 06:58:13 2023, max compression
```

## Comparing `common_packages-0.1.8.tar` & `common_packages-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.704260 common_packages-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-07 06:58:40.000000 common_packages-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-07 06:59:05.704260 common_packages-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-07 06:58:40.000000 common_packages-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.696260 common_packages-0.1.8/common_packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.700260 common_packages-0.1.8/common_packages/db_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/db_utils/clickhouse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/db_utils/mysql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.700260 common_packages-0.1.8/common_packages/email_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/email_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/email_utils/send_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.700260 common_packages-0.1.8/common_packages/file_storage_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/file_storage_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/file_storage_utils/file_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/file_storage_utils/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/file_storage_utils/tencent_cos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.700260 common_packages-0.1.8/common_packages/message_queue_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/message_queue_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/message_queue_utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/message_queue_utils/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/message_queue_utils/rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.700260 common_packages-0.1.8/common_packages/sms_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/sms_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/sms_utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/sms_utils/tencent_sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.704260 common_packages-0.1.8/common_packages/translate_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/translate_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/translate_utils/microsoft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/translate_utils/tencent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/translate_utils/youdao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.704260 common_packages-0.1.8/common_packages/tts/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/tts/microsoft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.704260 common_packages-0.1.8/common_packages/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/utils/tencent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-12-07 06:58:40.000000 common_packages-0.1.8/common_packages/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.704260 common_packages-0.1.8/common_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-07 06:59:05.000000 common_packages-0.1.8/common_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-07 06:59:05.000000 common_packages-0.1.8/common_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 06:59:05.000000 common_packages-0.1.8/common_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-07 06:59:05.000000 common_packages-0.1.8/common_packages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-07 06:59:05.000000 common_packages-0.1.8/common_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-12-07 06:58:40.000000 common_packages-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 06:59:05.704260 common_packages-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:59:05.704260 common_packages-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-07 06:58:40.000000 common_packages-0.1.8/tests/test_send_email_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-13 06:57:48.000000 common_packages-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-13 06:58:13.755798 common_packages-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-12-13 06:57:48.000000 common_packages-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.751798 common_packages-0.1.9/common_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.751798 common_packages-0.1.9/common_packages/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/db_utils/clickhouse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/db_utils/mysql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.751798 common_packages-0.1.9/common_packages/email_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/email_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/email_utils/send_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.751798 common_packages-0.1.9/common_packages/file_storage_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/file_storage_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/file_storage_utils/file_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/file_storage_utils/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/file_storage_utils/tencent_cos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/common_packages/message_queue_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/message_queue_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/message_queue_utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/message_queue_utils/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/message_queue_utils/rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/common_packages/sms_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/sms_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/sms_utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/sms_utils/tencent_sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/common_packages/translate_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/translate_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/translate_utils/microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/translate_utils/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/translate_utils/youdao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/common_packages/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/tts/microsoft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/common_packages/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/utils/tencent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2023-12-13 06:57:48.000000 common_packages-0.1.9/common_packages/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/common_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-13 06:58:13.000000 common_packages-0.1.9/common_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-12-13 06:58:13.000000 common_packages-0.1.9/common_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 06:58:13.000000 common_packages-0.1.9/common_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-13 06:58:13.000000 common_packages-0.1.9/common_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-12-13 06:57:48.000000 common_packages-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 06:58:13.755798 common_packages-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 06:58:13.755798 common_packages-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 06:57:48.000000 common_packages-0.1.9/tests/test_send_email_test.py
```

### Comparing `common_packages-0.1.8/LICENSE` & `common_packages-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/README.md` & `common_packages-0.1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 安装
 ```bash
 pip install common_packages-0.1.0.tar.gz
 ```
 pypi
 https://pypi.org/project/common-packages/#description
 
+依赖
+```bash
+    "requests",
+    'pika',
+    "tencentcloud-sdk-python-tmt",
+    "kafka-python",
+    "clickhouse-driver",
+    "numpy",
+    "pandas",
+    "sqlalchemy",
+    "pymysql",
+    "azure-cognitiveservices-speech",
+```
 ### sms
 腾讯云
 ```python
 
 ```
 
 ## django_utils
```

### Comparing `common_packages-0.1.8/common_packages/db_utils/clickhouse_utils.py` & `common_packages-0.1.9/common_packages/db_utils/clickhouse_utils.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/db_utils/mysql_utils.py` & `common_packages-0.1.9/common_packages/db_utils/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/email_utils/send_email.py` & `common_packages-0.1.9/common_packages/email_utils/send_email.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/file_storage_utils/file_interface.py` & `common_packages-0.1.9/common_packages/file_storage_utils/file_interface.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/file_storage_utils/local.py` & `common_packages-0.1.9/common_packages/file_storage_utils/local.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/file_storage_utils/tencent_cos.py` & `common_packages-0.1.9/common_packages/file_storage_utils/tencent_cos.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/message_queue_utils/interface.py` & `common_packages-0.1.9/common_packages/message_queue_utils/interface.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/message_queue_utils/kafka.py` & `common_packages-0.1.9/common_packages/message_queue_utils/kafka.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/message_queue_utils/rabbitmq.py` & `common_packages-0.1.9/common_packages/message_queue_utils/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/sms_utils/tencent_sms.py` & `common_packages-0.1.9/common_packages/sms_utils/tencent_sms.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/translate_utils/__init__.py` & `common_packages-0.1.9/common_packages/translate_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/translate_utils/tencent.py` & `common_packages-0.1.9/common_packages/translate_utils/tencent.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/translate_utils/youdao.py` & `common_packages-0.1.9/common_packages/translate_utils/youdao.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/tts/microsoft.py` & `common_packages-0.1.9/common_packages/tts/microsoft.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages/utils/tencent_utils.py` & `common_packages-0.1.9/common_packages/utils/tencent_utils.py`

 * *Files identical despite different names*

### Comparing `common_packages-0.1.8/common_packages.egg-info/SOURCES.txt` & `common_packages-0.1.9/common_packages.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 common_packages/__init__.py
 common_packages.egg-info/PKG-INFO
 common_packages.egg-info/SOURCES.txt
 common_packages.egg-info/dependency_links.txt
-common_packages.egg-info/requires.txt
 common_packages.egg-info/top_level.txt
 common_packages/db_utils/__init__.py
 common_packages/db_utils/clickhouse_utils.py
 common_packages/db_utils/mysql_utils.py
 common_packages/email_utils/__init__.py
 common_packages/email_utils/send_email.py
 common_packages/file_storage_utils/__init__.py
```

### Comparing `common_packages-0.1.8/pyproject.toml` & `common_packages-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -29,26 +29,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "common_packages"
 # 打包的版本号
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
-    "requests",
-    'pika',
-    "tencentcloud-sdk-python-tmt",
-    "kafka-python",
-    "clickhouse-driver",
-    "numpy",
-    "pandas",
-    "sqlalchemy",
-    "pymysql",
-    "azure-cognitiveservices-speech",
+    # "requests",
+    # 'pika',
+    # "tencentcloud-sdk-python-tmt",
+    # "kafka-python",
+    # "clickhouse-driver",
+    # "numpy",
+    # "pandas",
+    # "sqlalchemy",
+    # "pymysql",
+    # "azure-cognitiveservices-speech",
 ]
 
 [tool.setuptools]
 packages = [
     "common_packages",
     "common_packages.file_storage_utils",
     "common_packages.message_queue_utils",
```

### Comparing `common_packages-0.1.8/tests/test_send_email_test.py` & `common_packages-0.1.9/tests/test_send_email_test.py`

 * *Files identical despite different names*

