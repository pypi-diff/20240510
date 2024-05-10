# Comparing `tmp/qlv-client-0.2.5.tar.gz` & `tmp/qlv-client-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.2.5.tar", last modified: Fri May 10 08:01:06 2024, max compression
+gzip compressed data, was "qlv-client-0.2.6.tar", last modified: Fri May 10 09:00:37 2024, max compression
```

## Comparing `qlv-client-0.2.5.tar` & `qlv-client-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:01:06.532405 qlv-client-0.2.5/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      456 2024-05-10 08:01:06.531909 qlv-client-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 08:01:06.529425 qlv-client-0.2.5/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.5/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.5/qlv_client/api.py
--rw-rw-rw-   0        0        0     1850 2024-05-10 05:14:14.000000 qlv-client-0.2.5/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.5/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.5/qlv_client/http_client.py
--rw-rw-rw-   0        0        0    10727 2024-05-10 08:00:12.000000 qlv-client-0.2.5/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.5/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.5/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.5/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:01:06.531909 qlv-client-0.2.5/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:01:06.532405 qlv-client-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-10 08:00:59.000000 qlv-client-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:00:37.234636 qlv-client-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-05-10 09:00:37.234139 qlv-client-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:00:37.231656 qlv-client-0.2.6/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.6/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.6/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1850 2024-05-10 05:14:14.000000 qlv-client-0.2.6/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.6/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.6/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0    10703 2024-05-10 09:00:17.000000 qlv-client-0.2.6/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.6/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.6/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.6/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:00:37.233642 qlv-client-0.2.6/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-05-10 09:00:37.000000 qlv-client-0.2.6/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-10 09:00:37.000000 qlv-client-0.2.6/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:00:37.000000 qlv-client-0.2.6/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 09:00:37.000000 qlv-client-0.2.6/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 09:00:37.000000 qlv-client-0.2.6/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:00:37.234636 qlv-client-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-10 09:00:30.000000 qlv-client-0.2.6/setup.py
```

### Comparing `qlv-client-0.2.5/LICENSE` & `qlv-client-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/api.py` & `qlv-client-0.2.6/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/config.py` & `qlv-client-0.2.6/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/converter.py` & `qlv-client-0.2.6/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/http_client.py` & `qlv-client-0.2.6/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/proxy.py` & `qlv-client-0.2.6/qlv_client/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             flag = cls.save_payment_info(**payment_info)
             if flag is True:
                 break
         return flag
 
     @classmethod
     def save_itinerary_info(cls, **kwargs) -> bool:
-        logger.info("开始向劲旅系统回填乘客票单信息...")
+        logger.info("开始向劲旅系统回填票号信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="fill_order_itinerary_info")
         order_itinerary_info = QlvConfigRepository.get_order_itinerary_info(**kwargs)
         args.update(order_itinerary_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.fill_order_itinerary_info(**args)
         if result.get("code") == 0:
             message = result.get("message") or ''
@@ -156,20 +156,20 @@
             elif "重复数据" in message:
                 # 说名已经填过了
                 return True
             else:
                 logger.error(result)
                 return False
         else:
-            logger.error("向劲旅系统回填乘客票单信息成功.")
+            logger.error("向劲旅系统回填票号信息成功.")
             return True
 
     @classmethod
     def save_itinerary_info_by_batch_itinerary(cls, pre_order_id: int, oper: str, itinerary_info: list) -> bool:
-        logger.info("开始向劲旅系统回填乘客票单信息...")
+        logger.info("开始向劲旅系统回填票号信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="fill_order_itinerary_info")
         ticket_infos = list()
         for info in itinerary_info:
             passenger = info.get("passenger")
             card_id = info.get("card_id")
             itinerary_id = info.get("itinerary_id")
             if itinerary_id:
@@ -194,15 +194,15 @@
                 elif "重复数据" in message:
                     # 说名已经填过了
                     return True
                 else:
                     logger.error(result)
                     return False
             else:
-                logger.info("向劲旅系统回填乘客票单信息成功.")
+                logger.info("向劲旅系统回填票号信息成功.")
                 return True
         else:
             return False
 
     @classmethod
     def loop_save_itinerary_info(cls, pre_order_id: int, itinerary_info: list, oper: str, attempts: int = 3) -> bool:
         flag = False
```

### Comparing `qlv-client-0.2.5/qlv_client/repository.py` & `qlv-client-0.2.6/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/test.py` & `qlv-client-0.2.6/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/qlv_client/utils.py` & `qlv-client-0.2.6/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.5/setup.py` & `qlv-client-0.2.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.2.5',
+    version='0.2.6',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```

