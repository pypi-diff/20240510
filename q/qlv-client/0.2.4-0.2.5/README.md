# Comparing `tmp/qlv-client-0.2.4.tar.gz` & `tmp/qlv-client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.2.4.tar", last modified: Fri May 10 05:14:29 2024, max compression
+gzip compressed data, was "qlv-client-0.2.5.tar", last modified: Fri May 10 08:01:06 2024, max compression
```

## Comparing `qlv-client-0.2.4.tar` & `qlv-client-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:14:29.372692 qlv-client-0.2.4/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      456 2024-05-10 05:14:29.372692 qlv-client-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 05:14:29.370209 qlv-client-0.2.4/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.4/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.4/qlv_client/api.py
--rw-rw-rw-   0        0        0     1850 2024-05-10 05:14:14.000000 qlv-client-0.2.4/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.4/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.4/qlv_client/http_client.py
--rw-rw-rw-   0        0        0    10291 2024-05-10 03:54:21.000000 qlv-client-0.2.4/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.4/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.4/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.4/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:14:29.372196 qlv-client-0.2.4/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 05:14:29.000000 qlv-client-0.2.4/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 05:14:29.372692 qlv-client-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-10 05:14:21.000000 qlv-client-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:01:06.532405 qlv-client-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-05-10 08:01:06.531909 qlv-client-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 08:01:06.529425 qlv-client-0.2.5/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.5/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.5/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1850 2024-05-10 05:14:14.000000 qlv-client-0.2.5/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.5/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.5/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0    10727 2024-05-10 08:00:12.000000 qlv-client-0.2.5/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.5/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.5/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.5/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:01:06.531909 qlv-client-0.2.5/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 08:01:06.000000 qlv-client-0.2.5/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:01:06.532405 qlv-client-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-10 08:00:59.000000 qlv-client-0.2.5/setup.py
```

### Comparing `qlv-client-0.2.4/LICENSE` & `qlv-client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/api.py` & `qlv-client-0.2.5/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/config.py` & `qlv-client-0.2.5/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/converter.py` & `qlv-client-0.2.5/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/http_client.py` & `qlv-client-0.2.5/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/proxy.py` & `qlv-client-0.2.5/qlv_client/proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,17 +91,20 @@
         args = QlvConfigRepository.get_request_base_params(inter_name="save_order_pay_info")
         order_pay_info = QlvConfigRepository.get_order_pay_info(**kwargs)
         args.update(order_pay_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.save_order_pay_info(**args)
         if result.get("code") == 0:
             message = result.get("message") or ''
-            if message.find("票号保存") != -1:
+            if "支付保存" in message:
                 # 说名已经出票完成，再回填票号信息，就成了改签
                 return True
+            elif "重复数据" in message:
+                # 说名已经填过了
+                return True
             else:
                 logger.error(result)
                 return False
         else:
             logger.error("向劲旅系统回填采购信息成功.")
             return True
 
@@ -111,16 +114,19 @@
         args = QlvConfigRepository.get_request_base_params(inter_name="save_order_pay_info")
         order_pay_info = QlvConfigRepository.get_order_pay_info(**kwargs)
         args.update(order_pay_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.save_order_pay_info(**args)
         if result.get("code") == 0:
             message = result.get("message") or ''
-            if message.find("支付保存") != -1:
-                # 说名已经出票完成，再回填采购信息，就成了改签
+            if "支付保存" in message:
+                # 说名已经出票完成，再回填票号信息，就成了改签
+                return True
+            elif "重复数据" in message:
+                # 说名已经填过了
                 return True
             else:
                 logger.error(result)
                 return False
         else:
             logger.error("向劲旅系统回填采购信息成功.")
             return True
@@ -140,17 +146,20 @@
         args = QlvConfigRepository.get_request_base_params(inter_name="fill_order_itinerary_info")
         order_itinerary_info = QlvConfigRepository.get_order_itinerary_info(**kwargs)
         args.update(order_itinerary_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.fill_order_itinerary_info(**args)
         if result.get("code") == 0:
             message = result.get("message") or ''
-            if message.find("票号保存") != -1:
+            if "票号保存" in message:
                 # 说名已经出票完成，再回填票号信息，就成了改签
                 return True
+            elif "重复数据" in message:
+                # 说名已经填过了
+                return True
             else:
                 logger.error(result)
                 return False
         else:
             logger.error("向劲旅系统回填乘客票单信息成功.")
             return True
 
@@ -175,17 +184,20 @@
                 "ticket_infos": ";".join(ticket_infos)
             }
             args.update(order_itinerary_info)
             order_ser = OrderService(**QlvConfigRepository.get_host_params())
             result = order_ser.fill_order_itinerary_info(**args)
             if result.get("code") == 0:
                 message = result.get("message") or ''
-                if message.find("票号保存") != -1:
+                if "票号保存" in message:
                     # 说名已经出票完成，再回填票号信息，就成了改签
                     return True
+                elif "重复数据" in message:
+                    # 说名已经填过了
+                    return True
                 else:
                     logger.error(result)
                     return False
             else:
                 logger.info("向劲旅系统回填乘客票单信息成功.")
                 return True
         else:
```

### Comparing `qlv-client-0.2.4/qlv_client/repository.py` & `qlv-client-0.2.5/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/test.py` & `qlv-client-0.2.5/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/qlv_client/utils.py` & `qlv-client-0.2.5/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.4/setup.py` & `qlv-client-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.2.4',
+    version='0.2.5',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```

