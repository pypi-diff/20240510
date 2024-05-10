# Comparing `tmp/qlv-client-0.2.1.tar.gz` & `tmp/qlv-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.2.1.tar", last modified: Fri May 10 03:44:34 2024, max compression
+gzip compressed data, was "qlv-client-0.2.2.tar", last modified: Fri May 10 03:48:14 2024, max compression
```

## Comparing `qlv-client-0.2.1.tar` & `qlv-client-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:44:34.923977 qlv-client-0.2.1/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      456 2024-05-10 03:44:34.923480 qlv-client-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 03:44:34.920997 qlv-client-0.2.1/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.1/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.1/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.2.1/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.1/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.1/qlv_client/http_client.py
--rw-rw-rw-   0        0        0     9587 2024-05-10 03:43:31.000000 qlv-client-0.2.1/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.1/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.1/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.1/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:44:34.923480 qlv-client-0.2.1/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-05-10 03:44:34.000000 qlv-client-0.2.1/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-10 03:44:34.000000 qlv-client-0.2.1/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:44:34.000000 qlv-client-0.2.1/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 03:44:34.000000 qlv-client-0.2.1/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 03:44:34.000000 qlv-client-0.2.1/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:44:34.923977 qlv-client-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-10 03:44:31.000000 qlv-client-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:48:14.380742 qlv-client-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-05-10 03:48:14.380245 qlv-client-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 03:48:14.377762 qlv-client-0.2.2/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.2/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.2/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.2.2/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.2/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.2/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0    10097 2024-05-10 03:48:03.000000 qlv-client-0.2.2/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.2/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.2/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.2/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:48:14.379748 qlv-client-0.2.2/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:48:14.380742 qlv-client-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-10 03:48:10.000000 qlv-client-0.2.2/setup.py
```

### Comparing `qlv-client-0.2.1/LICENSE` & `qlv-client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/api.py` & `qlv-client-0.2.2/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/config.py` & `qlv-client-0.2.2/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/converter.py` & `qlv-client-0.2.2/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/http_client.py` & `qlv-client-0.2.2/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/proxy.py` & `qlv-client-0.2.2/qlv_client/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,21 @@
         logger.info("开始向劲旅系统回填采购信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="save_order_pay_info")
         order_pay_info = QlvConfigRepository.get_order_pay_info(**kwargs)
         args.update(order_pay_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.save_order_pay_info(**args)
         if result.get("code") == 0:
-            logger.error(result)
-            return False
+            message = result.get("message") or ''
+            if message.find("票号保存") != -1:
+                # 说名已经出票完成，再回填票号信息，就成了改签
+                return True
+            else:
+                logger.error(result)
+                return False
         else:
             logger.error("向劲旅系统回填采购信息成功.")
             return True
 
     @classmethod
     def save_payment_info(cls, **kwargs) -> bool:
         logger.info("开始向劲旅系统回填采购信息...")
@@ -164,16 +169,21 @@
                 "oper": oper,
                 "ticket_infos": ";".join(ticket_infos)
             }
             args.update(order_itinerary_info)
             order_ser = OrderService(**QlvConfigRepository.get_host_params())
             result = order_ser.fill_order_itinerary_info(**args)
             if result.get("code") == 0:
-                logger.error(result)
-                return False
+                message = result.get("message") or ''
+                if message.find("票号保存") != -1:
+                    # 说名已经出票完成，再回填票号信息，就成了改签
+                    return True
+                else:
+                    logger.error(result)
+                    return False
             else:
                 logger.info("向劲旅系统回填乘客票单信息成功.")
                 return True
         else:
             return False
 
     @classmethod
```

### Comparing `qlv-client-0.2.1/qlv_client/repository.py` & `qlv-client-0.2.2/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/test.py` & `qlv-client-0.2.2/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/qlv_client/utils.py` & `qlv-client-0.2.2/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.1/setup.py` & `qlv-client-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.2.1',
+    version='0.2.2',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```

